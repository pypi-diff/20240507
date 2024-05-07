# Comparing `tmp/sourcespec-1.7.tar.gz` & `tmp/sourcespec-1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sourcespec-1.7.tar", last modified: Fri Mar 31 14:47:08 2023, max compression
+gzip compressed data, was "sourcespec-1.8.tar", last modified: Tue May  7 09:45:50 2024, max compression
```

## Comparing `sourcespec-1.7.tar` & `sourcespec-1.8.tar`

### file list

```diff
@@ -1,98 +1,120 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:47:08.860478 sourcespec-1.7/
--rw-r--r--   0 runner    (1001) docker     (123)    22102 2023-03-31 14:46:58.000000 sourcespec-1.7/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-03-31 14:46:58.000000 sourcespec-1.7/CONTRIBUTORS.txt
--rw-r--r--   0 runner    (1001) docker     (123)    21778 2023-03-31 14:46:58.000000 sourcespec-1.7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-03-31 14:46:58.000000 sourcespec-1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    17909 2023-03-31 14:47:08.864478 sourcespec-1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16205 2023-03-31 14:46:58.000000 sourcespec-1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:47:08.844478 sourcespec-1.7/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1486 2023-03-31 14:46:58.000000 sourcespec-1.7/bin/source_model.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1515 2023-03-31 14:46:58.000000 sourcespec-1.7/bin/source_residuals.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1584 2023-03-31 14:46:58.000000 sourcespec-1.7/bin/source_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:47:08.848478 sourcespec-1.7/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     5883 2023-03-31 14:46:58.000000 sourcespec-1.7/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-03-31 14:46:58.000000 sourcespec-1.7/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-03-31 14:46:58.000000 sourcespec-1.7/docs/bibliography.rst
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-31 14:46:58.000000 sourcespec-1.7/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-03-31 14:46:58.000000 sourcespec-1.7/docs/citing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-03-31 14:46:58.000000 sourcespec-1.7/docs/clipping_detection.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10177 2023-03-31 14:46:58.000000 sourcespec-1.7/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-03-31 14:46:58.000000 sourcespec-1.7/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-03-31 14:46:58.000000 sourcespec-1.7/docs/file_formats.rst
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-03-31 14:46:58.000000 sourcespec-1.7/docs/getting_help.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-03-31 14:46:58.000000 sourcespec-1.7/docs/getting_started.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-03-31 14:46:58.000000 sourcespec-1.7/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-03-31 14:46:58.000000 sourcespec-1.7/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-03-31 14:46:58.000000 sourcespec-1.7/docs/refs.bib
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-03-31 14:46:58.000000 sourcespec-1.7/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-03-31 14:46:58.000000 sourcespec-1.7/docs/sample_runs.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-03-31 14:46:58.000000 sourcespec-1.7/docs/signal_processing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7928 2023-03-31 14:46:58.000000 sourcespec-1.7/docs/theoretical_background.rst
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-03-31 14:47:08.864478 sourcespec-1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-03-31 14:46:58.000000 sourcespec-1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:47:08.864478 sourcespec-1.7/sourcespec/
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-03-31 14:46:58.000000 sourcespec-1.7/sourcespec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-03-31 14:47:08.864478 sourcespec-1.7/sourcespec/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:47:08.860478 sourcespec-1.7/sourcespec/adjustText/
--rw-r--r--   0 runner    (1001) docker     (123)    26358 2023-03-31 14:46:58.000000 sourcespec-1.7/sourcespec/adjustText/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-03-31 14:46:58.000000 sourcespec-1.7/sourcespec/cached_tiler.py
--rw-r--r--   0 runner    (1001) docker     (123)    18869 2023-03-31 14:46:58.000000 sourcespec-1.7/sourcespec/clipping_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-03-31 14:46:58.000000 sourcespec-1.7/sourcespec/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:47:08.860478 sourcespec-1.7/sourcespec/configobj/
--rw-r--r--   0 runner    (1001) docker     (123)    88030 2023-03-31 14:46:58.000000 sourcespec-1.7/sourcespec/configobj/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-31 14:46:58.000000 sourcespec-1.7/sourcespec/configobj/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    46990 2023-03-31 14:46:58.000000 sourcespec-1.7/sourcespec/configobj/validate.py
--rw-r--r--   0 runner    (1001) docker     (123)    23947 2023-03-31 14:46:58.000000 sourcespec-1.7/sourcespec/configspec.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:47:08.860478 sourcespec-1.7/sourcespec/html_report_template/
--rw-r--r--   0 runner    (1001) docker     (123)    21663 2023-03-31 14:46:58.000000 sourcespec-1.7/sourcespec/html_report_template/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-03-31 14:46:58.000000 sourcespec-1.7/sourcespec/html_report_template/misfit.html
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-03-31 14:46:58.000000 sourcespec-1.7/sourcespec/html_report_template/misfit_table_column.html
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-03-31 14:46:58.000000 sourcespec-1.7/sourcespec/html_report_template/quakeml_file_link.html
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-03-31 14:46:58.000000 sourcespec-1.7/sourcespec/html_report_template/spectra_plot.html
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-03-31 14:46:58.000000 sourcespec-1.7/sourcespec/html_report_template/station_table_row.html
--rw-r--r--   0 runner    (1001) docker     (123)     7457 2023-03-31 14:46:58.000000 sourcespec-1.7/sourcespec/html_report_template/style.css
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-03-31 14:46:58.000000 sourcespec-1.7/sourcespec/html_report_template/traces_plot.html
--rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-03-31 14:46:58.000000 sourcespec-1.7/sourcespec/kdtree.py
--rw-r--r--   0 runner    (1001) docker     (123)    26793 2023-03-31 14:46:58.000000 sourcespec-1.7/sourcespec/plot_sourcepars.py
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-03-31 14:46:58.000000 sourcespec-1.7/sourcespec/savefig.py
--rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-03-31 14:46:58.000000 sourcespec-1.7/sourcespec/source_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4629 2023-03-31 14:46:58.000000 sourcespec-1.7/sourcespec/source_residuals.py
--rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-03-31 14:46:58.000000 sourcespec-1.7/sourcespec/source_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-03-31 14:46:58.000000 sourcespec-1.7/sourcespec/spectrum.py
--rw-r--r--   0 runner    (1001) docker     (123)    24371 2023-03-31 14:46:58.000000 sourcespec-1.7/sourcespec/ssp_build_spectra.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-03-31 14:46:58.000000 sourcespec-1.7/sourcespec/ssp_correction.py
--rw-r--r--   0 runner    (1001) docker     (123)    17877 2023-03-31 14:46:58.000000 sourcespec-1.7/sourcespec/ssp_data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    16825 2023-03-31 14:46:58.000000 sourcespec-1.7/sourcespec/ssp_grid_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)    36022 2023-03-31 14:46:58.000000 sourcespec-1.7/sourcespec/ssp_html_report.py
--rw-r--r--   0 runner    (1001) docker     (123)    18209 2023-03-31 14:46:58.000000 sourcespec-1.7/sourcespec/ssp_inversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     7151 2023-03-31 14:46:58.000000 sourcespec-1.7/sourcespec/ssp_local_magnitude.py
--rw-r--r--   0 runner    (1001) docker     (123)    15098 2023-03-31 14:46:58.000000 sourcespec-1.7/sourcespec/ssp_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     9329 2023-03-31 14:46:58.000000 sourcespec-1.7/sourcespec/ssp_parse_arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-03-31 14:46:58.000000 sourcespec-1.7/sourcespec/ssp_plot_params_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)    25021 2023-03-31 14:46:58.000000 sourcespec-1.7/sourcespec/ssp_plot_spectra.py
--rw-r--r--   0 runner    (1001) docker     (123)     8956 2023-03-31 14:46:58.000000 sourcespec-1.7/sourcespec/ssp_plot_stacked_spectra.py
--rw-r--r--   0 runner    (1001) docker     (123)    17279 2023-03-31 14:46:58.000000 sourcespec-1.7/sourcespec/ssp_plot_stations.py
--rw-r--r--   0 runner    (1001) docker     (123)    15731 2023-03-31 14:46:58.000000 sourcespec-1.7/sourcespec/ssp_plot_traces.py
--rw-r--r--   0 runner    (1001) docker     (123)    16232 2023-03-31 14:46:58.000000 sourcespec-1.7/sourcespec/ssp_process_traces.py
--rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-03-31 14:46:58.000000 sourcespec-1.7/sourcespec/ssp_qml_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-03-31 14:46:58.000000 sourcespec-1.7/sourcespec/ssp_radiated_energy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4175 2023-03-31 14:46:58.000000 sourcespec-1.7/sourcespec/ssp_radiation_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)    12904 2023-03-31 14:46:58.000000 sourcespec-1.7/sourcespec/ssp_read_event_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     5954 2023-03-31 14:46:58.000000 sourcespec-1.7/sourcespec/ssp_read_sac_header.py
--rw-r--r--   0 runner    (1001) docker     (123)     6817 2023-03-31 14:46:58.000000 sourcespec-1.7/sourcespec/ssp_read_station_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    14218 2023-03-31 14:46:58.000000 sourcespec-1.7/sourcespec/ssp_read_traces.py
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-03-31 14:46:58.000000 sourcespec-1.7/sourcespec/ssp_residuals.py
--rw-r--r--   0 runner    (1001) docker     (123)    28846 2023-03-31 14:46:58.000000 sourcespec-1.7/sourcespec/ssp_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-03-31 14:46:58.000000 sourcespec-1.7/sourcespec/ssp_spectral_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11110 2023-03-31 14:46:58.000000 sourcespec-1.7/sourcespec/ssp_sqlite_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     8962 2023-03-31 14:46:58.000000 sourcespec-1.7/sourcespec/ssp_summary_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     9639 2023-03-31 14:46:58.000000 sourcespec-1.7/sourcespec/ssp_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     8809 2023-03-31 14:46:58.000000 sourcespec-1.7/sourcespec/ssp_wave_arrival.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:47:08.860478 sourcespec-1.7/sourcespec.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17909 2023-03-31 14:47:08.000000 sourcespec-1.7/sourcespec.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-03-31 14:47:08.000000 sourcespec-1.7/sourcespec.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 14:47:08.000000 sourcespec-1.7/sourcespec.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-03-31 14:47:08.000000 sourcespec-1.7/sourcespec.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-31 14:47:08.000000 sourcespec-1.7/sourcespec.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-31 14:47:08.000000 sourcespec-1.7/sourcespec.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    70144 2023-03-31 14:46:58.000000 sourcespec-1.7/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:45:50.508259 sourcespec-1.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    32858 2024-05-07 09:45:44.000000 sourcespec-1.8/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-07 09:45:44.000000 sourcespec-1.8/CONTRIBUTORS.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    21778 2024-05-07 09:45:44.000000 sourcespec-1.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-07 09:45:44.000000 sourcespec-1.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    21320 2024-05-07 09:45:50.508259 sourcespec-1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    19432 2024-05-07 09:45:44.000000 sourcespec-1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:45:50.488259 sourcespec-1.8/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1681 2024-05-07 09:45:44.000000 sourcespec-1.8/bin/plot_sourcepars.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1533 2024-05-07 09:45:44.000000 sourcespec-1.8/bin/source_model.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1550 2024-05-07 09:45:44.000000 sourcespec-1.8/bin/source_residuals.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1665 2024-05-07 09:45:44.000000 sourcespec-1.8/bin/source_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:45:50.492259 sourcespec-1.8/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     5883 2024-05-07 09:45:44.000000 sourcespec-1.8/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-05-07 09:45:44.000000 sourcespec-1.8/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-07 09:45:44.000000 sourcespec-1.8/docs/bibliography.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-07 09:45:44.000000 sourcespec-1.8/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-07 09:45:44.000000 sourcespec-1.8/docs/citing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-07 09:45:44.000000 sourcespec-1.8/docs/citing_conferences.bib
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-07 09:45:44.000000 sourcespec-1.8/docs/citing_literature.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5675 2024-05-07 09:45:44.000000 sourcespec-1.8/docs/citing_papers.bib
+-rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-05-07 09:45:44.000000 sourcespec-1.8/docs/clipping_detection.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10443 2024-05-07 09:45:44.000000 sourcespec-1.8/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-07 09:45:44.000000 sourcespec-1.8/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5722 2024-05-07 09:45:44.000000 sourcespec-1.8/docs/file_formats.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-07 09:45:44.000000 sourcespec-1.8/docs/getting_help.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-05-07 09:45:44.000000 sourcespec-1.8/docs/getting_started.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-05-07 09:45:44.000000 sourcespec-1.8/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3193 2024-05-07 09:45:44.000000 sourcespec-1.8/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3940 2024-05-07 09:45:44.000000 sourcespec-1.8/docs/refs.bib
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-07 09:45:44.000000 sourcespec-1.8/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-07 09:45:44.000000 sourcespec-1.8/docs/sample_runs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4161 2024-05-07 09:45:44.000000 sourcespec-1.8/docs/signal_processing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-05-07 09:45:44.000000 sourcespec-1.8/docs/source_spec_event_file.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9333 2024-05-07 09:45:44.000000 sourcespec-1.8/docs/spectral_file_formats.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    17584 2024-05-07 09:45:44.000000 sourcespec-1.8/docs/theoretical_background.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:45:50.496259 sourcespec-1.8/imgs/
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-07 09:45:44.000000 sourcespec-1.8/imgs/SourceSpec_icon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6984 2024-05-07 09:45:44.000000 sourcespec-1.8/imgs/SourceSpec_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4845 2024-05-07 09:45:44.000000 sourcespec-1.8/imgs/SourceSpec_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4711 2024-05-07 09:45:44.000000 sourcespec-1.8/imgs/SourceSpec_logo_simple.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5886 2024-05-07 09:45:44.000000 sourcespec-1.8/imgs/SourceSpec_logo_simple.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4845 2024-05-07 09:45:44.000000 sourcespec-1.8/imgs/SourceSpec_logo_white.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   132754 2024-05-07 09:45:44.000000 sourcespec-1.8/imgs/example_spectrum.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   287813 2024-05-07 09:45:44.000000 sourcespec-1.8/imgs/example_trace.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-07 09:45:50.508259 sourcespec-1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-05-07 09:45:44.000000 sourcespec-1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:45:50.508259 sourcespec-1.8/sourcespec/
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-07 09:45:44.000000 sourcespec-1.8/sourcespec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-07 09:45:50.508259 sourcespec-1.8/sourcespec/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:45:50.504259 sourcespec-1.8/sourcespec/adjustText/
+-rw-r--r--   0 runner    (1001) docker     (127)    26358 2024-05-07 09:45:44.000000 sourcespec-1.8/sourcespec/adjustText/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-05-07 09:45:44.000000 sourcespec-1.8/sourcespec/cached_tiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19422 2024-05-07 09:45:44.000000 sourcespec-1.8/sourcespec/clipping_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-07 09:45:44.000000 sourcespec-1.8/sourcespec/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:45:50.504259 sourcespec-1.8/sourcespec/config_files/
+-rw-r--r--   0 runner    (1001) docker     (127)    32125 2024-05-07 09:45:44.000000 sourcespec-1.8/sourcespec/config_files/configspec.conf
+-rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-05-07 09:45:44.000000 sourcespec-1.8/sourcespec/config_files/ssp_event.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:45:50.508259 sourcespec-1.8/sourcespec/configobj/
+-rw-r--r--   0 runner    (1001) docker     (127)    88030 2024-05-07 09:45:44.000000 sourcespec-1.8/sourcespec/configobj/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-07 09:45:44.000000 sourcespec-1.8/sourcespec/configobj/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46990 2024-05-07 09:45:44.000000 sourcespec-1.8/sourcespec/configobj/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:45:50.508259 sourcespec-1.8/sourcespec/html_report_template/
+-rw-r--r--   0 runner    (1001) docker     (127)    23856 2024-05-07 09:45:44.000000 sourcespec-1.8/sourcespec/html_report_template/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6087 2024-05-07 09:45:44.000000 sourcespec-1.8/sourcespec/html_report_template/misfit.html
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-07 09:45:44.000000 sourcespec-1.8/sourcespec/html_report_template/misfit_table_column.html
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-07 09:45:44.000000 sourcespec-1.8/sourcespec/html_report_template/quakeml_file_link.html
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-07 09:45:44.000000 sourcespec-1.8/sourcespec/html_report_template/spectra_plot.html
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-07 09:45:44.000000 sourcespec-1.8/sourcespec/html_report_template/station_table_row.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7938 2024-05-07 09:45:44.000000 sourcespec-1.8/sourcespec/html_report_template/style.css
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-07 09:45:44.000000 sourcespec-1.8/sourcespec/html_report_template/traces_plot.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5078 2024-05-07 09:45:44.000000 sourcespec-1.8/sourcespec/kdtree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-05-07 09:45:44.000000 sourcespec-1.8/sourcespec/map_tiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35406 2024-05-07 09:45:44.000000 sourcespec-1.8/sourcespec/plot_sourcepars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-07 09:45:44.000000 sourcespec-1.8/sourcespec/savefig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4649 2024-05-07 09:45:44.000000 sourcespec-1.8/sourcespec/source_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6339 2024-05-07 09:45:44.000000 sourcespec-1.8/sourcespec/source_residuals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-05-07 09:45:44.000000 sourcespec-1.8/sourcespec/source_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27839 2024-05-07 09:45:44.000000 sourcespec-1.8/sourcespec/spectrum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29256 2024-05-07 09:45:44.000000 sourcespec-1.8/sourcespec/ssp_build_spectra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-07 09:45:44.000000 sourcespec-1.8/sourcespec/ssp_correction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19184 2024-05-07 09:45:44.000000 sourcespec-1.8/sourcespec/ssp_data_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5819 2024-05-07 09:45:44.000000 sourcespec-1.8/sourcespec/ssp_db_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13576 2024-05-07 09:45:44.000000 sourcespec-1.8/sourcespec/ssp_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18090 2024-05-07 09:45:44.000000 sourcespec-1.8/sourcespec/ssp_grid_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39317 2024-05-07 09:45:44.000000 sourcespec-1.8/sourcespec/ssp_html_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21225 2024-05-07 09:45:44.000000 sourcespec-1.8/sourcespec/ssp_inversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7206 2024-05-07 09:45:44.000000 sourcespec-1.8/sourcespec/ssp_local_magnitude.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17245 2024-05-07 09:45:44.000000 sourcespec-1.8/sourcespec/ssp_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10645 2024-05-07 09:45:44.000000 sourcespec-1.8/sourcespec/ssp_parse_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-07 09:45:44.000000 sourcespec-1.8/sourcespec/ssp_pick.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6213 2024-05-07 09:45:44.000000 sourcespec-1.8/sourcespec/ssp_plot_params_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26543 2024-05-07 09:45:44.000000 sourcespec-1.8/sourcespec/ssp_plot_spectra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9419 2024-05-07 09:45:44.000000 sourcespec-1.8/sourcespec/ssp_plot_stacked_spectra.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26672 2024-05-07 09:45:44.000000 sourcespec-1.8/sourcespec/ssp_plot_stations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16574 2024-05-07 09:45:44.000000 sourcespec-1.8/sourcespec/ssp_plot_traces.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18658 2024-05-07 09:45:44.000000 sourcespec-1.8/sourcespec/ssp_process_traces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8392 2024-05-07 09:45:44.000000 sourcespec-1.8/sourcespec/ssp_qml_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9835 2024-05-07 09:45:44.000000 sourcespec-1.8/sourcespec/ssp_radiated_energy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4369 2024-05-07 09:45:44.000000 sourcespec-1.8/sourcespec/ssp_radiation_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20448 2024-05-07 09:45:44.000000 sourcespec-1.8/sourcespec/ssp_read_event_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6350 2024-05-07 09:45:44.000000 sourcespec-1.8/sourcespec/ssp_read_sac_header.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6994 2024-05-07 09:45:44.000000 sourcespec-1.8/sourcespec/ssp_read_station_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-05-07 09:45:44.000000 sourcespec-1.8/sourcespec/ssp_read_traces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-05-07 09:45:44.000000 sourcespec-1.8/sourcespec/ssp_residuals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35334 2024-05-07 09:45:44.000000 sourcespec-1.8/sourcespec/ssp_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-05-07 09:45:44.000000 sourcespec-1.8/sourcespec/ssp_spectral_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12728 2024-05-07 09:45:44.000000 sourcespec-1.8/sourcespec/ssp_sqlite_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9841 2024-05-07 09:45:44.000000 sourcespec-1.8/sourcespec/ssp_summary_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9304 2024-05-07 09:45:44.000000 sourcespec-1.8/sourcespec/ssp_update_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21242 2024-05-07 09:45:44.000000 sourcespec-1.8/sourcespec/ssp_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8973 2024-05-07 09:45:44.000000 sourcespec-1.8/sourcespec/ssp_wave_arrival.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:45:50.508259 sourcespec-1.8/sourcespec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    21320 2024-05-07 09:45:50.000000 sourcespec-1.8/sourcespec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-05-07 09:45:50.000000 sourcespec-1.8/sourcespec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 09:45:50.000000 sourcespec-1.8/sourcespec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-07 09:45:50.000000 sourcespec-1.8/sourcespec.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-07 09:45:50.000000 sourcespec-1.8/sourcespec.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-07 09:45:50.000000 sourcespec-1.8/sourcespec.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    70144 2024-05-07 09:45:44.000000 sourcespec-1.8/versioneer.py
```

### Comparing `sourcespec-1.7/CHANGELOG.md` & `sourcespec-1.8/CHANGELOG.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,218 @@
 # SourceSpec Changelog
 
 Earthquake source parameters from P- or S-wave displacement spectra
 
-Copyright (c) 2011-2023 Claudio Satriano <satriano@ipgp.fr>
+Copyright (c) 2011-2024 Claudio Satriano <satriano@ipgp.fr>
+
+## v1.8 - 2024-04-07
+
+This long overdue release brings many improvements, new features and bugfixes
+gradually introduced during the last year.
+
+Release highlights:
+
+- New file formats for events and spectra
+- New configuration options to better specifify velocity and density models
+- Better support for P-wave inversion and teleseismic events
+- Support for radiation pattern correction from focal mechanism
+- Option for travel time-based signal window length
+- More options to control the calculation of source radius and stress drop
+- Improved estimation of radiated energy
+- New source parameter: apparent stress
+- Fix for map tiles not plotted anymore
+
+This release requires at least Python 3.7.
+
+Warning: the SQLite database used by this version is not compatible with
+previous versions. You will need to upgrade your old database manually or using
+`source_spec -u DATABASE_FILE_NAME`.
+
+Make sure to read the detailed Changelog below 👇
+
+### Input/output
+
+- Introducing a new file format for providing event information
+  (hypocentral location, magnitude, focal mechanism, moment tensor):
+  the [SourceSpec Event File].
+- New HDF5 and TEXT file formats to store spectra
+- Station residuals are now saved in an HDF5 spectrum file, instead of a
+  pickle file
+- New config file option `save_spectra` to save the spectra to an HDF5 file
+  in the output directory
+- Changes in the YAML output file:
+  - `bsd` (Brune stress drop) parameter renamed to `ssd` (static stress drop)
+  - Store in the `event_info` section the values of vp, vs and rho close to
+    the hypocenter
+  - Store in the `inversion_info` section the type of wave used for the
+    inversion (P, S, SV or SH)
+- Changes in the SQLite database (warning: these changes break compatibility
+  with previous database versions):
+  - `bsd` (Brune stress drop) parameter renamed to `ssd` (static stress drop)
+  - Store the `Stations` table information on whether each parameter is an
+    outlier (see [#38])
+  - Make place in the `Stations` table for station-level errors on radiated
+    energy (even if they are currently not computed)
+  - Store in the `Events` table the number of observations used for computing
+    each summary parameter
+  - Store in the `Events` table weighted means for radiated energy and local
+    magnitude, even if those means are currently the same as the simple means,
+    since those parameters do not have station-level errors defined
+  - New columns for apparent stress in both `Events` and `Stations` tables
+  - Store in the `Events` table the values of vp, vs and rho close to the
+    hypocenter
+  - Store in the `Events` table the type of wave used for the inversion
+    (P, S, SV or SH)
+- New command line option (`-u` or `--updatedb`) to update an existing database
+  from a previous version
+- Input files are now linked symbolically in the `input_files` subdirectory
+  of the output directory (not implemented for Windows)
+- New command line option (`-R` or `--run_id_subdir`) to use `run_id`
+  (if defined) as a subdirectory of the event directory
+- Print event info to console and to log file
+- HTML report improvements:
+  - Event name in the summary table, if available
+  - Author, agency and run completion date in the summary table
+  - SourceSpec version in the inversion information table
+  - Link to input files
+  - Information on the type of wave used for the inversion (P, S, SV or SH)
+
+### Processing
+
+- Use all the available components to compute P-wave spectra (previously,
+  only the vertical component was used)
+- Possibility of specifying a free surface amplification factor different
+  from 2
+- Possibility of specifying a layered velocity and density model for the
+  source
+- Possibility of specifying a different density for the source and for the
+  stations
+- If density is not provided (i.e., it is `None`), use the density from the
+  global velocity model "iasp91"
+- Teleseismic geometrical spreading model (Okal, 1992)
+- New weighting option based on inverse frequency, so that lower frequencies
+  have larger weight in the inversion. If traces contain noise, weights will
+  be set to zero where SNR < 3 (see [#37])
+- For weights computed from spectral S/N ratio (noise weighting), set to zero
+  all the weights below 20% of the maximum weight, so that these weakly
+  constrained parts of the spectrum are ignored in the inversion
+- Possibility of using variable signal window lengths for each station
+  as a function of the travel time of the P or S wave (see [#48])
+
+### Inversion
+
+- Possibility of using the magnitude (or scalar moment) provided in the event
+  file as initial Mw value for the inversion
+- Reintroduced the possibility of providing the variability around the initial
+  Mw value
+- By combining the previous options, it is now possible to fix the Mw value
+  during the inversion to the value provided in the event file
+
+### Post-Inversion
+
+- Possibility of choosing the "k" coefficient to compute source radius from
+  corner frequency (Kaneko and Shearer, 2014)
+- Better control on the frequency range used for computing radiated energy
+  (see [#49])
+- Use station-specific radiation pattern (when available) for computing
+  radiated energy
+- Take into account for energy partition when computing radiated energy
+  (Boatwright and Choy, 1986). This affects mostly the radiated energy
+  computed from P waves
+- New source parameter: apparent stress
+- For parameters with no station-level uncertainty defined (currently,
+  radiated energy and local magnitude), use simple mean when computing summary
+  weighted averages (the previous behavior was to not compute weighted averages
+  for these parameters)
+
+### Plotting
+
+- Show the station radiated energy (Er) value on the station spectra plots
+- Show the summary radiated energy (Er) value on the stacked spectra plot
+- Station maps improvements:
+  - Possibility of choosing a basemap style or no basemap
+  - Possibility of not plotting the coastlines
+  - Exclude outliers when computing colorbar limits
+  - Improved computation of bounding box for regional and teleseismic events
+  - Use a global orthographic projection when using stations at large
+    teleseismic epicentral distances (more than 3000 km)
+- Changes to `plot_sourcepars`:
+  - Read vp, vs and rho from the SQLite database (previously: vs was hardcoded
+    to 3.5 km/s, rho to 2700 kg/m3 and vp was not used)
+  - Read the source radius "k" coefficient from the SQLite database
+    (previously: "k" was hardcoded to 0.3724, value for the Brune model)
+  - New command line option `--wave_type` to select the wave type (P, S, SV
+    or SH) for plots involving the corner frequency
+  - Possibility of plotting histogram of apparent stress
+  - Option to filter events by apparent stress
+
+### Config file
+
+- New config parameter `epi_dist_ranges` to select stations within one or
+  more ranges of epicentral distances. It replaces the old parameter
+  `max_epi_dist`.
+- New config parameter `free_surface_amplification` to specify the free surface
+  amplification factor (default: 2)
+- New config parameter `layer_top_depths` to specify the depth of the top of
+  the layers in a layered velocity and density model
+- The config parameters `vp_source`, `vs_source` and `rho_source` can now be
+  lists of values, to specify a layered velocity and density model for the
+  source
+- Config parameter `rho` renamed to `rho_source`
+- New config parameter `rho_stations`
+- New config parameter `geom_spread_min_teleseismic_distance` to set the
+  minimum epicentral distance for using the teleseismic geometrical
+  spreading model
+- New config parameters `kp` and `ks` to set the "k" coefficient for
+  computing source radius from corner frequency
+- Config parameter `pi_bsd_min_max` renamed to `pi_ssd_min_max`
+- New option `inv_frequency` for the config parameter `weighting` (see [#37])
+- Config parameter `max_freq_Er` replaced by `Er_freq_range` (see [#49])
+- New parameters, `qml_event_description` and `qml_event_description_regex`,
+  to obtain the event name from the QuakeML event "description" tag
+- New parameter `Mw_0_from_event_file` to use the magnitude (or scalar moment)
+  provided in the event file as initial Mw value for the inversion
+- Reintroduced the parameter `Mw_0_variability` to set the variability around
+  the initial Mw value
+- New parameter `plot_save_asap` to save plots as soon as they are ready.
+  This uses less memory but slows down the code.
+- New parameter `plot_map_style` to choose the map style
+- New parameter `plot_map_api_key` to provide a Stadia Maps
+  api key for Stamen Terrain basemap
+- New option for the parameter `plot_coastline_resolution`: `no_coastline`
+- New config parameter `variable_win_length_factor` to specify window
+  length as a fraction of the travel time of the P/S wave (see [#48])
+
+### Bugfixes
+
+- Fix source radius computation when using P waves (use P-wave velocity instead
+  of S-wave velocity)
+- Do not ignore picks labeled with lowercase "p" or "s"
+- Fixed: config parameter `p_arrival_tolerance` was used also for S waves,
+  instead of `s_arrival_tolerance` (see [#35])
+- Fix Boatwright spreading model (log10 instead of natural log)
+- Fix bug where signal and noise windows were plotted with the wrong length,
+  under certain circumstances (see [#35])
+- Fixes related to records with short signal windows (see [#39])
+- Fix for beachball not plotted anymore with recent versions of Matplotlib.
+- Fix bug where traces ignored because of low spectral S/N ratio, where still
+  plotted as if they were valid traces
+- Fix bug when specifying an absolute path for output directory: the path
+  was treated as relative (see [#40])
+- Fix bug where paths starting with tilde (~) were not parsed correctly
+  (see [#43] and [#44])
+- Fix bug where local magnitude was not written to the HYPO71 output file,
+  when using weighted mean as reference statistics
+- Fix for Stamen Terrain basemap now requiring an API key from Stadia Maps
+
+### Requirements
+
+- Python minimum version raised to 3.7
+- Matplotlib minimum version raised to 3.2
+- Cartopy minimum version raised to 0.21
 
 ## v1.7 - 2023-03-31
 
 This release improves trace processing through the use of modern routines for
 instrument correction, optional baseline removal, a new clipping detection
 algorithm and a better definition of signal and noise time windows.
 
@@ -24,29 +230,29 @@
 
 Big kudos to Kris Vanneste [@krisvanneste] who helped all along the development
 with code review and testing and submitted pull requests on noise windows and
 clipping detection.
 
 Below is the detailed Changelog 👇
 
-### Input/output
+### v1.7: Input/output
 
 - Possibility of using a single PAZ file as a "generic" PAZ file for all the
   stations
 - Command line option `--station_metadata` (or `-w`) for overriding the config
   file parameter with the same name (see pull request [#16])
 - Removed command line option `--no-response` for avoiding removing instrument
   response (use the config option `correct_instrumental_response` instead)
 - New output file in YAML format. The old `.out` file is still available but
   deprecated.
 - Information on the inversion procedure in YAML and HTML output
 - Option to add an agency logo to the HTML page
 - Possibility of generating HTML report without figures (see [#30])
 
-### Processing
+### v1.7: Processing
 
 - Use modern ObsPy `trace.remove_response()` routine for instrument correction
   (see [#27])
 - Option to remove the trace baseline after instrument correction and before
   filtering (`remove_baseline` config parameter) (see [#25])
 - New algorithms for clipping detection based on kernel density estimation of
   the trace amplitude values (see [#23], [#24], [#25])
@@ -73,42 +279,42 @@
     records with short S-P interval)
 - Extract source and station P and S velocities from global 'iasp91' velocity
   model, if both `v(p,s)_source` and `v(p,s)_stations` are set to `None`
   (see [#20])
 - Magnitude limits for inversion are now autoset between 90% of the minimum
   of the spectral plateau and 110% of its maximum (see [#22])
 
-### Post-Inversion
+### v1.7: Post-Inversion
 
 - Possibility of choosing the reference summary statistics that will be used
   for map plots, QuakeML and HYPO output, as well as for the "Event Summary"
   section in HTML report and for computing station spectral residuals.
   Available summary statistics are:
   - mean
   - weighted_mean
   - percentiles (new!)
 - Possibility of defining the number of sigmas for uncertainties on event means
   and weighted means
 
-### Plotting
+### v1.7: Plotting
 
 - New plot: stacked spectra
 - Do not zero-pad traces to common length when plotting, so that missing data
   at beginning or at the end can be easily detected (see [#21])
 - Plot noise and signal windows separately for each component (see [#21])
 - Show on the trace plot the reason why a trace has been ignored
 - Logscale for boxplots, if parameters span a large interval
   (see pull request [#15])
 - Support for SVG format for plot files (can be used in HTML output as
   alternative to PNG)
 - Improved trace plot quality for vector formats (PDF, SVG)
 - New command line tool: `plot_sourcepars` to make 1D or 2D plot of source
   parameters from a sqlite parameter file.
 
-### Config file
+### v1.7: Config file
 
 - Removed `sensitivity_only` option from `correct_instrumental_response`
 - Removed config parameter: `Mw_0_variability`
 - Removed config parameter: `clip_max_percent`
 - New config parameter: `remove_baseline`
 - New config parameters for clipping detection:
   - `clipping_detection_algorithm`
@@ -124,20 +330,20 @@
   `mid_percentage` and `upper_percentage`
 - New config parameters for filtering and spectral windowing of displacement
   signals:
   - `bp_freqmin_disp`, `bp_freqmax_disp`
   - `freq1_disp`, `freq2_disp`
 - Default values for `t_star_min_max` (instead of `None`)
 
-### Code improvements
+### v1.7: Code improvements
 
 - Large refactoring of the whole codebase, to make the code more modern and
   easier to maintain (see [#28])
 
-### Bugfixes
+### v1.7: Bugfixes
 
 - Properly ignore vertical components when `ignore_vertical` is `True`
 - Fix a bug preventing reading phase picks from HYPOINVERSE-2000 files
 - Fix for noise window not showing up in PNG trace plots in some cases
 - Fix reading velocities from NLL model (see [#20])
 - HTML report: better scrollbars for station table across all the browsers
 - Fix for cropped map for very large station-to-event distances (greater
@@ -495,14 +701,15 @@
 
 ## v0.1 - 2012-01-17
 
 Initial Python port.
 
 [Discussions]: https://github.com/SeismicSource/sourcespec/discussions
 [@krisvanneste]: https://github.com/krisvanneste
+[SourceSpec Event File]: https://sourcespec.readthedocs.io/en/latest/source_spec_event_file.html
 
 [#2]: https://github.com/SeismicSource/sourcespec/issues/2
 [#3]: https://github.com/SeismicSource/sourcespec/issues/3
 [#5]: https://github.com/SeismicSource/sourcespec/issues/5
 [#6]: https://github.com/SeismicSource/sourcespec/issues/6
 [#8]: https://github.com/SeismicSource/sourcespec/issues/8
 [#9]: https://github.com/SeismicSource/sourcespec/issues/9
@@ -516,7 +723,16 @@
 [#23]: https://github.com/SeismicSource/sourcespec/issues/23
 [#24]: https://github.com/SeismicSource/sourcespec/issues/24
 [#25]: https://github.com/SeismicSource/sourcespec/issues/25
 [#27]: https://github.com/SeismicSource/sourcespec/issues/27
 [#28]: https://github.com/SeismicSource/sourcespec/issues/28
 [#30]: https://github.com/SeismicSource/sourcespec/issues/30
 [#31]: https://github.com/SeismicSource/sourcespec/issues/31
+[#35]: https://github.com/SeismicSource/sourcespec/issues/35
+[#37]: https://github.com/SeismicSource/sourcespec/issues/37
+[#38]: https://github.com/SeismicSource/sourcespec/issues/38
+[#39]: https://github.com/SeismicSource/sourcespec/issues/39
+[#40]: https://github.com/SeismicSource/sourcespec/issues/40
+[#43]: https://github.com/SeismicSource/sourcespec/issues/43
+[#44]: https://github.com/SeismicSource/sourcespec/issues/44
+[#48]: https://github.com/SeismicSource/sourcespec/issues/48
+[#49]: https://github.com/SeismicSource/sourcespec/issues/49
```

### Comparing `sourcespec-1.7/LICENSE.txt` & `sourcespec-1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sourcespec-1.7/PKG-INFO` & `sourcespec-1.8/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,56 +1,27 @@
-Metadata-Version: 2.1
-Name: sourcespec
-Version: 1.7
-Summary: Earthquake source parameters from P- or S-wave displacement spectra
-Home-page: https://sourcespec.seismicsource.org
-Author: Claudio Satriano
-Author-email: satriano@ipgp.fr
-License: CeCILL Free Software License Agreement, Version 2.1
-Project-URL: Homepage, https://sourcespec.seismicsource.org
-Project-URL: Source, https://github.com/SeismicSource/sourcespec
-Project-URL: Documentation, https://sourcespec.readthedocs.io
-Platform: OS Independent
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: CEA CNRS Inria Logiciel Libre License, version 2.1 (CeCILL-2.1)
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-<img src="https://cdn.jsdelivr.net/gh/SeismicSource/sourcespec@14da5bf21ed6aa82da902d06d019487604c47ea2/imgs/SourceSpec_logo.svg" width="600">
+<img src="imgs/SourceSpec_logo.svg" width="600">
 
 # SourceSpec
 
 Earthquake source parameters from P- or S-wave displacement spectra
 
+[![changelog-badge]][changelog-link]
 [![PyPI-badge]][PyPI-link]
 [![license-badge]][license-link]
 [![docs-badge]][docs-link]
 [![DOI-badge]][DOI-link]
 
-Copyright (c) 2011-2023 Claudio Satriano <satriano@ipgp.fr>
+Copyright (c) 2011-2024 Claudio Satriano <satriano@ipgp.fr>
 
 ## Description
 
 SourceSpec is a collection of command line tools to compute earthquake source
 parameters (seismic moment, corner frequency, radiated energy, source size,
-stress drop) from the inversion of P-wave and S-wave displacement spectra
-recorded at one or more seismic stations.
+static stress drop, apparent stress) from the inversion of P-wave and S-wave
+displacement spectra recorded at one or more seismic stations.
 SourceSpec also computes attenuation parameters (t-star, quality factor) and,
 as a bonus, local magnitude.
 
 See [Madariaga (2011)][Madariaga2011] for a primer on earthquake source
 parameters and scaling laws.
 
 Go to section [Theoretical background](#theoretical-background) below to get
@@ -72,27 +43,43 @@
 - `plot_sourcepars`: 1D or 2D plot of source parameters from a sqlite
   parameter file.
 
 ## Getting Started
 
 ### For the impatient
 
+> Note that the default config parameters are suited for a M<5 earthquake
+> recorded within ~100 km. Adjust `win_length`, `noise_pre_time`, the
+> frequency bands (`bp_freqmin_*`, `bp_freqmax_*`, `freq1_*`, `freq2_*`),
+> and the bounds on `fc` and `t_star`, according to your problem.
+
+#### Use case: miniSEED + StationXML + QuakeML
+
 If you have seismic recordings in [miniSEED] format (e.g., `traces.mseed`),
 metadata in [StationXML] format (e.g., `station.xml`) and event information in
 [QuakeML] format (e.g., `event.xml`), then:
 
 1. Generate a config file via `source_spec -S`;
 2. Edit the config file variable `station_metadata` to point to `station.xml`
    file;
 3. Run `source_spec -t traces.mseed -q event.xml`.
 
-> Note that the default config parameters are suited for a M<5 earthquake
-> recorded within ~100 km. Adjust `win_length`, `noise_pre_time`, and the
-> frequency bands (`bp_freqmin_*`, `bp_freqmax_*`, `freq1_*`, `freq2_*`)
-> according to your setup.
+#### Use case: SAC + PAZ + SourceSpec Event File
+
+If you have seismic recordings in [SAC] format (e.g., in a directory named
+`sac_data`), metadata as [SAC polezero (PAZ)] (e.g., in a directory named
+`paz`) and event information in any format, then:
+
+1. Generate a config file via `source_spec -S`;
+2. Edit the config file variable `station_metadata` to point to the `paz`
+   directory;
+3. Generate a sample [SourceSpec Event File] using `source_spec -y`; this
+   will create a file named `ssp_event.yaml`;
+4. Edit the file `ssp_event.yaml` with your event information;
+5. Run `source_spec -t sac_data -H ssp_event.yaml`.
 
 ### Command line arguments
 
 After successfully installed SourceSpec (see [Installation](#installation)
 below), you can get help on the command line arguments used by each code by
 typing from your terminal:
 
@@ -101,18 +88,19 @@
 (or `source_model -h`, or `source_residuals -h`).
 
 `source_spec` and `source_model` require you to provide the path to seismic
 traces via the `--trace_path` command line argument (see
 [File formats](#file-formats) below).
 
 Information on the seismic event can be stored in the trace header ([SAC]
-format), or provided through a [QuakeML] file (`--qmlfile`) or a [HYPO71] or
-[HYPOINVERSE-2000] file (`--hypocenter`). See
-[File formats](#file-formats) below for more information on the supported file
-formats.
+format), or provided through a [QuakeML] file (`--qmlfile`) or
+or, alternatively (`--hypocenter`), through a [SourceSpec Event File],
+a [HYPO71] file, or a [HYPOINVERSE-2000] file.
+See [File formats](#file-formats) below for more information on the supported
+file formats.
 
 ### Configuration file
 
 `source_spec` and `source_model` require a configuration file. The default file
 name is `source_spec.conf`, other file names can be specified via the
 `--configfile` command line argument.
 
@@ -135,37 +123,51 @@
 
 - [miniSEED]
 - [SAC]
 
 The SAC format can carry additional information in its header, like event
 location and origin time, phase picks, instrument sensitivity.
 
+Input trace files can be provided --through the `-t` option-- as a list of
+files, as a directory containing the files, or as a TAR(GZ) or ZIP archive
+containing the files.
+
 ### Event formats
 
 SourceSpec can read event information (event ID, location, origin time) in the
 following formats:
 
-- [QuakeML]: SourceSpec will also read phase picks and
-  focal mechanism, if available
+- [SourceSpec Event File]: this file can contain additional event information,
+  such as magnitude, moment tensor or focal mechanism
+- [QuakeML]: this file can contain additional event information, such as
+  magnitude, moment tensor or focal mechanism. If phase picks are available,
+  they will be read as well
 - [HYPO71]
-- [HYPOINVERSE-2000]: SourceSpec will also read phase picks, if available
+- [HYPOINVERSE-2000]: if phase picks are available, they will be read as well
 
-Event information can also be stored in the SAC file headers (header fields:
+Event information can also be stored in the [SAC file header] (header fields:
 `EVLA`, `EVLO`, `EVDP`, `O`, `KEVNM`).
 
 ### Phase pick formats
 
 Phase picks for P and S waves can be read from one of the following formats:
 
 - [QuakeML]
 - [HYPO71]
 - [HYPOINVERSE-2000]
 
-Phase picks can also be stored in the SAC file headers (header fields: `A` and
-`T0`).
+Phase picks can also be stored in the [SAC file header], using the header
+fields `A` and `T0` through `T9`. A pick label can be specified (header fields
+`KA` and `KT0` through `KT9`) to identify the pick; the pick label can be a
+standard 4-characters SAC label (e.g., `"IPU0"`, `" S 1"`) or a label starting
+with `"P"` or `"S"` (lowercase or uppercase, e.g., `"P"`, `"pP"`, `"Pg"`,
+`"S"`, `"Sn"`).
+Picks with labels that cannot be parsed by SourceSpec will be ignored.
+If no label is specified, then SourceSpec will assume that `A` is the P-pick
+and `T0` is the S-pick.
 
 ### Station metadata formats
 
 Station metadata (coordinates, instrumental response) can be provided in one of
 the following formats:
 
 - [StationXML]
@@ -191,16 +193,16 @@
 - `EVID.ssp.yaml`: [YAML] file containing the estimated spectral parameters
   (summary values and per station values)
 - `EVID.ssp.out` (*deprecated*): text file containing the estimated spectral
   parameters (summary values and per station values)
 - `EVID.ssp.log`: log file in text format (including the command line arguments,
   for [reproducibility])
 - `EVID.ssp.conf`: the input config file (for [reproducibility])
-- `EVID-residuals.pickle`: station residuals in
-  [Python pickle format][pickle]
+- `EVID.residuals.hdf5`: station residuals in [HDF5] format
+- `EVID.spectra.hdf5`: (optional) spectra in [HDF5] format
 - `EVID.ssp.h`: hypocenter file in [HYPO71] format with the estimated moment
   magnitude (only if an input HYPO71 file is provided)
 - `EVID.xml`: updated [QuakeML] file with the results of the SourceSpec
   inversion (only if an input QuakeML file is provided)
 
 The following plots will be created, in png, pdf or svg format:
 
@@ -262,57 +264,84 @@
 - LM: [Levenberg-Marquardt algorithm]
   (warning: [Trust Region Reflective algorithm] will be used instead if
    bounds are provided)
 - BH: [basin-hopping algorithm]
 - GS: [grid search]
 - IS: [importance sampling] of misfit grid, using [k-d tree]
 
-Starting from the inverted parameters $M_0$ ( $M_w$ ), $fc$, $t^*$ and following
-the equations in [Madariaga (2011)][Madariaga2011], other quantities are
-computed for each station:
-
-- the Brune stress drop
-- the source radius
+Starting from the inverted parameters $M_0$ ( $M_w$ ), $fc$, $t^*$ and
+following the equations in [Madariaga (2011)][Madariaga2011] and
+[Lancieri (2012)][Lancieri2012], other quantities are computed for each
+station:
+
+- the static stress drop $\Delta \sigma$
+- the source radius $a$
+- the radiated energy $E_r$
+- the apparent stress $\sigma_a$
 - the quality factor $Q_0$ of P- or S-waves
 
-Finally, the radiated energy $E_r$ can be measured from the displacement
-spectra, following the approach described in [Lancieri et al.
-(2012)][Lancieri2012].
-
 As a bonus, local magnitude $M_l$ can be computed as well.
 
 Event summaries (mean, weighted mean, percentiles) are computed from single
 station estimates. For mean and weighted mean estimation, outliers are rejected
 based on the [interquartile range] rule.
 
 See the official [documentation] for more details.
 
-![Example Trace](https://cdn.jsdelivr.net/gh/SeismicSource/sourcespec@14da5bf21ed6aa82da902d06d019487604c47ea2/imgs/example_trace.svg) **Example three-component trace plot
+![Example Trace](imgs/example_trace.svg) **Example three-component trace plot
 (in velocity), showing noise and S-wave windows**
 
-![Example Spectrum](https://cdn.jsdelivr.net/gh/SeismicSource/sourcespec@14da5bf21ed6aa82da902d06d019487604c47ea2/imgs/example_spectrum.svg)
+![Example Spectrum](imgs/example_spectrum.svg)
 **Example displacement spectrum for noise and S-wave, including inversion
 results**
 
 ## Installation
 
-SourceSpec requires at least Python 3.6. All the required dependencies will be
+SourceSpec requires at least Python 3.7. All the required dependencies will be
 downloaded and installed during the setup process.
 
 ### Installing the latest release
 
-#### Using pip and PyPI (preferred method)
+### Using Anaconda
+
+The following command will automatically create an [Anaconda] environment
+named `sourcespec`, install the required packages and install the latest
+version of SourceSpec via `pip`:
+
+    conda env create --file https://raw.githubusercontent.com/SeismicSource/sourcespec/main/sourcespec_conda_env.yml
+
+If you want a different name for your environment, use:
+
+    conda env create -n YOUR_ENV_NAME --file https://raw.githubusercontent.com/SeismicSource/sourcespec/main/sourcespec_conda_env.yml
+
+Activate the environment with:
+
+    conda activate sourcespec
+
+(or `conda activate YOUR_ENV_NAME`)
+
+To keep SourceSpec updated run:
+
+    pip install --upgrade sourcespec
+
+from within your environment.
+
+#### Using pip and PyPI
 
 The latest release of SourceSpec is available on the
 [Python Package Index](https://pypi.org/project/sourcespec/).
 
 You can install it easily through `pip`:
 
     pip install sourcespec
 
+To upgrade from a previously installed version:
+
+    pip install --upgrade sourcespec
+
 #### From SourceSpec GitHub releases
 
 Download the latest release from the
 [releases page](https://github.com/SeismicSource/sourcespec/releases),
 in `zip` or `tar.gz` format, then:
 
     pip install sourcespec-X.Y.zip
@@ -323,19 +352,19 @@
 
 Where, `X.Y` is the version number (e.g., `1.2`).
 You don't need to uncompress the release files yourself.
 
 ### Installing a developer snapshot
 
 If you need a recent feature that is not in the latest release (see the
-`unreleased` section in [CHANGELOG](https://cdn.jsdelivr.net/gh/SeismicSource/sourcespec@14da5bf21ed6aa82da902d06d019487604c47ea2/CHANGELOG.md)), you want to use the more
+`unreleased` section in [CHANGELOG](CHANGELOG.md)), you want to use the more
 recent development snapshot from the
 [SourceSpec GitHub repository](https://github.com/SeismicSource/sourcespec).
 
-#### Using pip (preferred method)
+#### Using pip
 
 The easiest way to install the most recent development snapshot is to download
 and install it through `pip`, using its builtin `git` client:
 
     pip install git+https://github.com/SeismicSource/sourcespec.git
 
 Run this command again, from times to times, to keep SourceSpec updated with
@@ -391,66 +420,78 @@
 [Issue][Issues].
 Don't hesitate sending me pull requests with new features and/or bugfixes!
 
 ## How to Cite
 
 If you used SourceSpec for a scientific paper, please cite it as:
 
-> Satriano, C. (2023). SourceSpec – Earthquake source parameters from
+> Satriano, C. (2024). SourceSpec – Earthquake source parameters from
 > P- or S-wave displacement spectra (X.Y).
 > [doi: 10.5281/ZENODO.3688587]
 
 Please replace `X.Y` with the SourceSpec version number you used.
 
 You can also cite the following abstract presented at the
 2016 AGU Fall Meeting:
 
 > Satriano, C., Mejia Uquiche, A. R., & Saurel, J. M. (2016). Spectral
 > estimation of seismic moment, corner frequency and radiated energy for
 > earthquakes in the Lesser Antilles. In AGU Fall Meeting Abstracts
 > (Vol. 2016, pp. S13A-2518), [bibcode: 2016AGUFM.S13A2518S]
 
-
 ## References
 
 - Brune, J. N. (1970). Tectonic stress and the spectra of seismic shear waves
   from earthquakes, J. Geophys. Res., 75 (26), 4997– 5009,
   [doi: 10.1029/JB075i026p04997]
 - Lancieri, M., Madariaga, R., Bonilla, F. (2012). Spectral scaling of the
   aftershocks of the Tocopilla 2007 earthquake in northern Chile, Geophys. J.
   Int., 189 (1), 469–480, [doi: 10.1111/j.1365-246X.2011.05327.x]
 - Madariaga, R. (2011). Earthquake Scaling Laws. In "Extreme Environmental
   Events", pp. 364–383, [doi: 10.1007/978-1-4419-7695-6_22]. Available on
   [ResearchGate][Madariaga2011].
 
+## Citing literature
+
+A, probably incomplete, list of papers that used SourceSpec can be found in
+the [Citing Literature][citing_literature] section of the documentation.
+If you have used SourceSpec in a publication and would like to have it listed,
+please let me know.
+
 <!-- Badges and project links -->
 [PyPI-badge]: http://img.shields.io/pypi/v/sourcespec.svg
 [PyPI-link]: https://pypi.python.org/pypi/sourcespec
 [license-badge]: https://img.shields.io/badge/license-CeCILL--2.1-green.svg
 [license-link]: http://www.cecill.info/licences.en.html
 [docs-badge]: https://readthedocs.org/projects/sourcespec/badge/?version=latest
 [docs-link]: https://sourcespec.readthedocs.io/en/latest/?badge=latest
+[changelog-badge]: https://img.shields.io/badge/Changelog-136CB6.svg
+[changelog-link]: https://github.com/SeismicSource/sourcespec/blob/main/CHANGELOG.md
 [DOI-badge]: https://zenodo.org/badge/DOI/10.5281/zenodo.3688587.svg
 [DOI-link]: https://doi.org/10.5281/zenodo.3688587
 [documentation]: https://sourcespec.readthedocs.io
 [Discussions]: https://github.com/SeismicSource/sourcespec/discussions
 [Issues]: https://github.com/SeismicSource/sourcespec/issues
+[Anaconda]: https://www.anaconda.com/products/individual
+[citing_literature]: https://sourcespec.readthedocs.io/en/latest/citing_literature.html
 
 <!-- File formats -->
 [obspy_trace_formats]: https://docs.obspy.org/packages/autogen/obspy.core.stream.read.html
 [miniSEED]: http://ds.iris.edu/ds/nodes/dmc/data/formats/miniseed/
 [SAC]: https://ds.iris.edu/ds/support/faq/17/sac-file-format/
+[SAC file header]: https://ds.iris.edu/files/sac-manual/manual/file_format.html
+[SourceSpec Event File]: https://sourcespec.readthedocs.io/en/latest/source_spec_event_file.html
 [QuakeML]: https://quake.ethz.ch/quakeml/
 [HYPO71]: https://pubs.er.usgs.gov/publication/ofr72224
 [HYPOINVERSE-2000]: https://pubs.er.usgs.gov/publication/ofr02171
 [StationXML]: http://docs.fdsn.org/projects/stationxml/en/latest/
 [Dataless SEED]: https://ds.iris.edu/ds/nodes/dmc/data/formats/dataless-seed/
 [SEED resp]: https://ds.iris.edu/ds/nodes/dmc/data/formats/resp/
 [SAC polezero (PAZ)]: https://www.jakewalter.net/sacresponse.html
-[pickle]: https://docs.python.org/3/library/pickle.html
+[HDF5]: https://en.wikipedia.org/wiki/Hierarchical_Data_Format
 [Cartopy]: https://scitools.org.uk/cartopy/docs/latest
 [SQLite]: https://www.sqlite.org
 [YAML]: https://yaml.org
 
 <!-- Methods -->
 [reproducibility]: https://en.wikipedia.org/wiki/Reproducibility
 [box_plot]: https://en.wikipedia.org/wiki/Box_plot
```

### Comparing `sourcespec-1.7/README.md` & `sourcespec-1.8/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,65 @@
-<img src="imgs/SourceSpec_logo.svg" width="600">
+Metadata-Version: 2.1
+Name: sourcespec
+Version: 1.8
+Summary: Earthquake source parameters from P- or S-wave displacement spectra
+Home-page: https://sourcespec.seismicsource.org
+Author: Claudio Satriano
+Author-email: satriano@ipgp.fr
+License: CeCILL Free Software License Agreement, Version 2.1
+Project-URL: Homepage, https://sourcespec.seismicsource.org
+Project-URL: Source, https://github.com/SeismicSource/sourcespec
+Project-URL: Documentation, https://sourcespec.readthedocs.io
+Platform: OS Independent
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: CEA CNRS Inria Logiciel Libre License, version 2.1 (CeCILL-2.1)
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Physics
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+Requires-Dist: numpy>=1.10
+Requires-Dist: scipy>=0.17
+Requires-Dist: matplotlib>=3.2
+Requires-Dist: pillow>=4.0.0
+Requires-Dist: obspy>=1.2.0
+Requires-Dist: pyproj
+Requires-Dist: tzlocal
+Requires-Dist: pyyaml>=5.1
+Requires-Dist: h5py
+
+<img src="https://cdn.jsdelivr.net/gh/SeismicSource/sourcespec@721d460561daa0f48f7d4addb409ef11c6e98865/imgs/SourceSpec_logo.svg" width="600">
 
 # SourceSpec
 
 Earthquake source parameters from P- or S-wave displacement spectra
 
+[![changelog-badge]][changelog-link]
 [![PyPI-badge]][PyPI-link]
 [![license-badge]][license-link]
 [![docs-badge]][docs-link]
 [![DOI-badge]][DOI-link]
 
-Copyright (c) 2011-2023 Claudio Satriano <satriano@ipgp.fr>
+Copyright (c) 2011-2024 Claudio Satriano <satriano@ipgp.fr>
 
 ## Description
 
 SourceSpec is a collection of command line tools to compute earthquake source
 parameters (seismic moment, corner frequency, radiated energy, source size,
-stress drop) from the inversion of P-wave and S-wave displacement spectra
-recorded at one or more seismic stations.
+static stress drop, apparent stress) from the inversion of P-wave and S-wave
+displacement spectra recorded at one or more seismic stations.
 SourceSpec also computes attenuation parameters (t-star, quality factor) and,
 as a bonus, local magnitude.
 
 See [Madariaga (2011)][Madariaga2011] for a primer on earthquake source
 parameters and scaling laws.
 
 Go to section [Theoretical background](#theoretical-background) below to get
@@ -42,27 +81,43 @@
 - `plot_sourcepars`: 1D or 2D plot of source parameters from a sqlite
   parameter file.
 
 ## Getting Started
 
 ### For the impatient
 
+> Note that the default config parameters are suited for a M<5 earthquake
+> recorded within ~100 km. Adjust `win_length`, `noise_pre_time`, the
+> frequency bands (`bp_freqmin_*`, `bp_freqmax_*`, `freq1_*`, `freq2_*`),
+> and the bounds on `fc` and `t_star`, according to your problem.
+
+#### Use case: miniSEED + StationXML + QuakeML
+
 If you have seismic recordings in [miniSEED] format (e.g., `traces.mseed`),
 metadata in [StationXML] format (e.g., `station.xml`) and event information in
 [QuakeML] format (e.g., `event.xml`), then:
 
 1. Generate a config file via `source_spec -S`;
 2. Edit the config file variable `station_metadata` to point to `station.xml`
    file;
 3. Run `source_spec -t traces.mseed -q event.xml`.
 
-> Note that the default config parameters are suited for a M<5 earthquake
-> recorded within ~100 km. Adjust `win_length`, `noise_pre_time`, and the
-> frequency bands (`bp_freqmin_*`, `bp_freqmax_*`, `freq1_*`, `freq2_*`)
-> according to your setup.
+#### Use case: SAC + PAZ + SourceSpec Event File
+
+If you have seismic recordings in [SAC] format (e.g., in a directory named
+`sac_data`), metadata as [SAC polezero (PAZ)] (e.g., in a directory named
+`paz`) and event information in any format, then:
+
+1. Generate a config file via `source_spec -S`;
+2. Edit the config file variable `station_metadata` to point to the `paz`
+   directory;
+3. Generate a sample [SourceSpec Event File] using `source_spec -y`; this
+   will create a file named `ssp_event.yaml`;
+4. Edit the file `ssp_event.yaml` with your event information;
+5. Run `source_spec -t sac_data -H ssp_event.yaml`.
 
 ### Command line arguments
 
 After successfully installed SourceSpec (see [Installation](#installation)
 below), you can get help on the command line arguments used by each code by
 typing from your terminal:
 
@@ -71,18 +126,19 @@
 (or `source_model -h`, or `source_residuals -h`).
 
 `source_spec` and `source_model` require you to provide the path to seismic
 traces via the `--trace_path` command line argument (see
 [File formats](#file-formats) below).
 
 Information on the seismic event can be stored in the trace header ([SAC]
-format), or provided through a [QuakeML] file (`--qmlfile`) or a [HYPO71] or
-[HYPOINVERSE-2000] file (`--hypocenter`). See
-[File formats](#file-formats) below for more information on the supported file
-formats.
+format), or provided through a [QuakeML] file (`--qmlfile`) or
+or, alternatively (`--hypocenter`), through a [SourceSpec Event File],
+a [HYPO71] file, or a [HYPOINVERSE-2000] file.
+See [File formats](#file-formats) below for more information on the supported
+file formats.
 
 ### Configuration file
 
 `source_spec` and `source_model` require a configuration file. The default file
 name is `source_spec.conf`, other file names can be specified via the
 `--configfile` command line argument.
 
@@ -105,37 +161,51 @@
 
 - [miniSEED]
 - [SAC]
 
 The SAC format can carry additional information in its header, like event
 location and origin time, phase picks, instrument sensitivity.
 
+Input trace files can be provided --through the `-t` option-- as a list of
+files, as a directory containing the files, or as a TAR(GZ) or ZIP archive
+containing the files.
+
 ### Event formats
 
 SourceSpec can read event information (event ID, location, origin time) in the
 following formats:
 
-- [QuakeML]: SourceSpec will also read phase picks and
-  focal mechanism, if available
+- [SourceSpec Event File]: this file can contain additional event information,
+  such as magnitude, moment tensor or focal mechanism
+- [QuakeML]: this file can contain additional event information, such as
+  magnitude, moment tensor or focal mechanism. If phase picks are available,
+  they will be read as well
 - [HYPO71]
-- [HYPOINVERSE-2000]: SourceSpec will also read phase picks, if available
+- [HYPOINVERSE-2000]: if phase picks are available, they will be read as well
 
-Event information can also be stored in the SAC file headers (header fields:
+Event information can also be stored in the [SAC file header] (header fields:
 `EVLA`, `EVLO`, `EVDP`, `O`, `KEVNM`).
 
 ### Phase pick formats
 
 Phase picks for P and S waves can be read from one of the following formats:
 
 - [QuakeML]
 - [HYPO71]
 - [HYPOINVERSE-2000]
 
-Phase picks can also be stored in the SAC file headers (header fields: `A` and
-`T0`).
+Phase picks can also be stored in the [SAC file header], using the header
+fields `A` and `T0` through `T9`. A pick label can be specified (header fields
+`KA` and `KT0` through `KT9`) to identify the pick; the pick label can be a
+standard 4-characters SAC label (e.g., `"IPU0"`, `" S 1"`) or a label starting
+with `"P"` or `"S"` (lowercase or uppercase, e.g., `"P"`, `"pP"`, `"Pg"`,
+`"S"`, `"Sn"`).
+Picks with labels that cannot be parsed by SourceSpec will be ignored.
+If no label is specified, then SourceSpec will assume that `A` is the P-pick
+and `T0` is the S-pick.
 
 ### Station metadata formats
 
 Station metadata (coordinates, instrumental response) can be provided in one of
 the following formats:
 
 - [StationXML]
@@ -161,16 +231,16 @@
 - `EVID.ssp.yaml`: [YAML] file containing the estimated spectral parameters
   (summary values and per station values)
 - `EVID.ssp.out` (*deprecated*): text file containing the estimated spectral
   parameters (summary values and per station values)
 - `EVID.ssp.log`: log file in text format (including the command line arguments,
   for [reproducibility])
 - `EVID.ssp.conf`: the input config file (for [reproducibility])
-- `EVID-residuals.pickle`: station residuals in
-  [Python pickle format][pickle]
+- `EVID.residuals.hdf5`: station residuals in [HDF5] format
+- `EVID.spectra.hdf5`: (optional) spectra in [HDF5] format
 - `EVID.ssp.h`: hypocenter file in [HYPO71] format with the estimated moment
   magnitude (only if an input HYPO71 file is provided)
 - `EVID.xml`: updated [QuakeML] file with the results of the SourceSpec
   inversion (only if an input QuakeML file is provided)
 
 The following plots will be created, in png, pdf or svg format:
 
@@ -232,57 +302,84 @@
 - LM: [Levenberg-Marquardt algorithm]
   (warning: [Trust Region Reflective algorithm] will be used instead if
    bounds are provided)
 - BH: [basin-hopping algorithm]
 - GS: [grid search]
 - IS: [importance sampling] of misfit grid, using [k-d tree]
 
-Starting from the inverted parameters $M_0$ ( $M_w$ ), $fc$, $t^*$ and following
-the equations in [Madariaga (2011)][Madariaga2011], other quantities are
-computed for each station:
-
-- the Brune stress drop
-- the source radius
+Starting from the inverted parameters $M_0$ ( $M_w$ ), $fc$, $t^*$ and
+following the equations in [Madariaga (2011)][Madariaga2011] and
+[Lancieri (2012)][Lancieri2012], other quantities are computed for each
+station:
+
+- the static stress drop $\Delta \sigma$
+- the source radius $a$
+- the radiated energy $E_r$
+- the apparent stress $\sigma_a$
 - the quality factor $Q_0$ of P- or S-waves
 
-Finally, the radiated energy $E_r$ can be measured from the displacement
-spectra, following the approach described in [Lancieri et al.
-(2012)][Lancieri2012].
-
 As a bonus, local magnitude $M_l$ can be computed as well.
 
 Event summaries (mean, weighted mean, percentiles) are computed from single
 station estimates. For mean and weighted mean estimation, outliers are rejected
 based on the [interquartile range] rule.
 
 See the official [documentation] for more details.
 
-![Example Trace](imgs/example_trace.svg) **Example three-component trace plot
+![Example Trace](https://cdn.jsdelivr.net/gh/SeismicSource/sourcespec@721d460561daa0f48f7d4addb409ef11c6e98865/imgs/example_trace.svg) **Example three-component trace plot
 (in velocity), showing noise and S-wave windows**
 
-![Example Spectrum](imgs/example_spectrum.svg)
+![Example Spectrum](https://cdn.jsdelivr.net/gh/SeismicSource/sourcespec@721d460561daa0f48f7d4addb409ef11c6e98865/imgs/example_spectrum.svg)
 **Example displacement spectrum for noise and S-wave, including inversion
 results**
 
 ## Installation
 
-SourceSpec requires at least Python 3.6. All the required dependencies will be
+SourceSpec requires at least Python 3.7. All the required dependencies will be
 downloaded and installed during the setup process.
 
 ### Installing the latest release
 
-#### Using pip and PyPI (preferred method)
+### Using Anaconda
+
+The following command will automatically create an [Anaconda] environment
+named `sourcespec`, install the required packages and install the latest
+version of SourceSpec via `pip`:
+
+    conda env create --file https://raw.githubusercontent.com/SeismicSource/sourcespec/main/sourcespec_conda_env.yml
+
+If you want a different name for your environment, use:
+
+    conda env create -n YOUR_ENV_NAME --file https://raw.githubusercontent.com/SeismicSource/sourcespec/main/sourcespec_conda_env.yml
+
+Activate the environment with:
+
+    conda activate sourcespec
+
+(or `conda activate YOUR_ENV_NAME`)
+
+To keep SourceSpec updated run:
+
+    pip install --upgrade sourcespec
+
+from within your environment.
+
+#### Using pip and PyPI
 
 The latest release of SourceSpec is available on the
 [Python Package Index](https://pypi.org/project/sourcespec/).
 
 You can install it easily through `pip`:
 
     pip install sourcespec
 
+To upgrade from a previously installed version:
+
+    pip install --upgrade sourcespec
+
 #### From SourceSpec GitHub releases
 
 Download the latest release from the
 [releases page](https://github.com/SeismicSource/sourcespec/releases),
 in `zip` or `tar.gz` format, then:
 
     pip install sourcespec-X.Y.zip
@@ -293,19 +390,19 @@
 
 Where, `X.Y` is the version number (e.g., `1.2`).
 You don't need to uncompress the release files yourself.
 
 ### Installing a developer snapshot
 
 If you need a recent feature that is not in the latest release (see the
-`unreleased` section in [CHANGELOG](CHANGELOG.md)), you want to use the more
+`unreleased` section in [CHANGELOG](https://cdn.jsdelivr.net/gh/SeismicSource/sourcespec@721d460561daa0f48f7d4addb409ef11c6e98865/CHANGELOG.md)), you want to use the more
 recent development snapshot from the
 [SourceSpec GitHub repository](https://github.com/SeismicSource/sourcespec).
 
-#### Using pip (preferred method)
+#### Using pip
 
 The easiest way to install the most recent development snapshot is to download
 and install it through `pip`, using its builtin `git` client:
 
     pip install git+https://github.com/SeismicSource/sourcespec.git
 
 Run this command again, from times to times, to keep SourceSpec updated with
@@ -361,66 +458,78 @@
 [Issue][Issues].
 Don't hesitate sending me pull requests with new features and/or bugfixes!
 
 ## How to Cite
 
 If you used SourceSpec for a scientific paper, please cite it as:
 
-> Satriano, C. (2023). SourceSpec – Earthquake source parameters from
+> Satriano, C. (2024). SourceSpec – Earthquake source parameters from
 > P- or S-wave displacement spectra (X.Y).
 > [doi: 10.5281/ZENODO.3688587]
 
 Please replace `X.Y` with the SourceSpec version number you used.
 
 You can also cite the following abstract presented at the
 2016 AGU Fall Meeting:
 
 > Satriano, C., Mejia Uquiche, A. R., & Saurel, J. M. (2016). Spectral
 > estimation of seismic moment, corner frequency and radiated energy for
 > earthquakes in the Lesser Antilles. In AGU Fall Meeting Abstracts
 > (Vol. 2016, pp. S13A-2518), [bibcode: 2016AGUFM.S13A2518S]
 
-
 ## References
 
 - Brune, J. N. (1970). Tectonic stress and the spectra of seismic shear waves
   from earthquakes, J. Geophys. Res., 75 (26), 4997– 5009,
   [doi: 10.1029/JB075i026p04997]
 - Lancieri, M., Madariaga, R., Bonilla, F. (2012). Spectral scaling of the
   aftershocks of the Tocopilla 2007 earthquake in northern Chile, Geophys. J.
   Int., 189 (1), 469–480, [doi: 10.1111/j.1365-246X.2011.05327.x]
 - Madariaga, R. (2011). Earthquake Scaling Laws. In "Extreme Environmental
   Events", pp. 364–383, [doi: 10.1007/978-1-4419-7695-6_22]. Available on
   [ResearchGate][Madariaga2011].
 
+## Citing literature
+
+A, probably incomplete, list of papers that used SourceSpec can be found in
+the [Citing Literature][citing_literature] section of the documentation.
+If you have used SourceSpec in a publication and would like to have it listed,
+please let me know.
+
 <!-- Badges and project links -->
 [PyPI-badge]: http://img.shields.io/pypi/v/sourcespec.svg
 [PyPI-link]: https://pypi.python.org/pypi/sourcespec
 [license-badge]: https://img.shields.io/badge/license-CeCILL--2.1-green.svg
 [license-link]: http://www.cecill.info/licences.en.html
 [docs-badge]: https://readthedocs.org/projects/sourcespec/badge/?version=latest
 [docs-link]: https://sourcespec.readthedocs.io/en/latest/?badge=latest
+[changelog-badge]: https://img.shields.io/badge/Changelog-136CB6.svg
+[changelog-link]: https://github.com/SeismicSource/sourcespec/blob/main/CHANGELOG.md
 [DOI-badge]: https://zenodo.org/badge/DOI/10.5281/zenodo.3688587.svg
 [DOI-link]: https://doi.org/10.5281/zenodo.3688587
 [documentation]: https://sourcespec.readthedocs.io
 [Discussions]: https://github.com/SeismicSource/sourcespec/discussions
 [Issues]: https://github.com/SeismicSource/sourcespec/issues
+[Anaconda]: https://www.anaconda.com/products/individual
+[citing_literature]: https://sourcespec.readthedocs.io/en/latest/citing_literature.html
 
 <!-- File formats -->
 [obspy_trace_formats]: https://docs.obspy.org/packages/autogen/obspy.core.stream.read.html
 [miniSEED]: http://ds.iris.edu/ds/nodes/dmc/data/formats/miniseed/
 [SAC]: https://ds.iris.edu/ds/support/faq/17/sac-file-format/
+[SAC file header]: https://ds.iris.edu/files/sac-manual/manual/file_format.html
+[SourceSpec Event File]: https://sourcespec.readthedocs.io/en/latest/source_spec_event_file.html
 [QuakeML]: https://quake.ethz.ch/quakeml/
 [HYPO71]: https://pubs.er.usgs.gov/publication/ofr72224
 [HYPOINVERSE-2000]: https://pubs.er.usgs.gov/publication/ofr02171
 [StationXML]: http://docs.fdsn.org/projects/stationxml/en/latest/
 [Dataless SEED]: https://ds.iris.edu/ds/nodes/dmc/data/formats/dataless-seed/
 [SEED resp]: https://ds.iris.edu/ds/nodes/dmc/data/formats/resp/
 [SAC polezero (PAZ)]: https://www.jakewalter.net/sacresponse.html
-[pickle]: https://docs.python.org/3/library/pickle.html
+[HDF5]: https://en.wikipedia.org/wiki/Hierarchical_Data_Format
 [Cartopy]: https://scitools.org.uk/cartopy/docs/latest
 [SQLite]: https://www.sqlite.org
 [YAML]: https://yaml.org
 
 <!-- Methods -->
 [reproducibility]: https://en.wikipedia.org/wiki/Reproducibility
 [box_plot]: https://en.wikipedia.org/wiki/Box_plot
```

### Comparing `sourcespec-1.7/bin/source_model.py` & `sourcespec-1.8/bin/source_spec.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,45 +1,48 @@
 #!/usr/bin/env python3
 # -*- coding: utf8 -*-
 # SPDX-License-Identifier: CECILL-2.1
 """
-Wrapper to run source_model.py from source tree.
+Wrapper to run source_spec.py from source tree.
 
 :copyright:
-    2016-2023 Claudio Satriano <satriano@ipgp.fr>
+    2016-2024 Claudio Satriano <satriano@ipgp.fr>
 :license:
     CeCILL Free Software License Agreement v2.1
     (http://www.cecill.info/licences.en.html)
 """
 import sys
 import os
 import inspect
 
-MIN_PYTHON_VERSION = (3, 6)
+MIN_PYTHON_VERSION = (3, 7)
+# pylint: disable=consider-using-f-string
 MIN_PYTHON_VERSION_STR = '{}.{}'.format(*MIN_PYTHON_VERSION)
-PYTHON_VERSION_STR = '{}.{}.{}'.format(*sys.version_info[0:3])
+PYTHON_VERSION_STR = '{}.{}.{}'.format(*sys.version_info[:3])
 if sys.version_info < MIN_PYTHON_VERSION:
-    msg = 'SourceSpec requires Python version >= {}'.format(
-        MIN_PYTHON_VERSION_STR)
-    msg += ' you are using Python version {}'.format(PYTHON_VERSION_STR)
+    msg = f'SourceSpec requires Python version >= {MIN_PYTHON_VERSION_STR}'
+    msg += f' you are using Python version {PYTHON_VERSION_STR}'
     print(msg, file=sys.stderr)
     sys.exit(1)
 
 if __name__ == '__main__':
     try:
         # Make sure we use current-dir version over installed one
         path = os.path.abspath(os.path.join(os.path.dirname(inspect.getfile(
             inspect.currentframe())), os.pardir))
         sys.path.insert(0, path)
         # Try to import obspy, which requires most of the
-        # source_model dependencies
-        import obspy #NOQA
-        from sourcespec.source_model import main
+        # source_spec dependencies
+        import obspy  # NOQA  pylint: disable=unused-import
+        # Try to import tzlocal, which is required at the end of the run
+        import tzlocal  # NOQA  pylint: disable=unused-import
+        from sourcespec.source_spec import main
         main()
     except ImportError as msg:
-        mod_name = msg.name
-        if mod_name == 'PIL':
-            mod_name = 'pillow'
-        s = "Error: module '{}' is required by source_model.".format(mod_name)
-        s += " Please install it.\n"
-        sys.stderr.write(s)
+        MOD_NAME = msg.name
+        if MOD_NAME == 'PIL':
+            MOD_NAME = 'pillow'
+        sys.stderr.write(
+            f"Error: module '{MOD_NAME}' is required by source_spec. "
+            "Please install it.\n"
+        )
         sys.exit(1)
```

### Comparing `sourcespec-1.7/bin/source_residuals.py` & `sourcespec-1.8/bin/plot_sourcepars.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,48 @@
 #!/usr/bin/env python3
 # -*- coding: utf8 -*-
 # SPDX-License-Identifier: CECILL-2.1
 """
-Wrapper to run source_residuals.py from source tree.
+Wrapper to run plot_sourcepars.py from source tree.
 
 :copyright:
-    2016-2023 Claudio Satriano <satriano@ipgp.fr>
+    2016-2024 Claudio Satriano <satriano@ipgp.fr>
 :license:
     CeCILL Free Software License Agreement v2.1
     (http://www.cecill.info/licences.en.html)
 """
 import sys
 import os
 import inspect
 
-MIN_PYTHON_VERSION = (3, 6)
+MIN_PYTHON_VERSION = (3, 7)
+# pylint: disable=consider-using-f-string
 MIN_PYTHON_VERSION_STR = '{}.{}'.format(*MIN_PYTHON_VERSION)
-PYTHON_VERSION_STR = '{}.{}.{}'.format(*sys.version_info[0:3])
+PYTHON_VERSION_STR = '{}.{}.{}'.format(*sys.version_info[:3])
 if sys.version_info < MIN_PYTHON_VERSION:
-    msg = 'SourceSpec requires Python version >= {}'.format(
-        MIN_PYTHON_VERSION_STR)
-    msg += ' you are using Python version {}'.format(PYTHON_VERSION_STR)
+    msg = f'SourceSpec requires Python version >= {MIN_PYTHON_VERSION_STR}'
+    msg += f' you are using Python version {PYTHON_VERSION_STR}'
     print(msg, file=sys.stderr)
     sys.exit(1)
 
 if __name__ == '__main__':
     try:
         # Make sure we use current-dir version over installed one
         path = os.path.abspath(os.path.join(os.path.dirname(inspect.getfile(
             inspect.currentframe())), os.pardir))
         sys.path.insert(0, path)
         # Try to import obspy, which requires most of the
-        # source_residuals dependencies
-        import obspy #NOQA
-        from sourcespec.source_residuals import main
+        # plot_sourcepars dependencies
+        import obspy  # NOQA  pylint: disable=unused-import
+        # Try to import tzlocal, which is required at the end of the run
+        import tzlocal  # NOQA  pylint: disable=unused-import
+        from sourcespec.plot_sourcepars import main
         main()
     except ImportError as msg:
-        mod_name = msg.name
-        if mod_name == 'PIL':
-            mod_name = 'pillow'
-        s = "Error: module '{}' is required by source_residuals.".format(
-            mod_name)
-        s += " Please install it.\n"
-        sys.stderr.write(s)
+        MOD_NAME = msg.name
+        if MOD_NAME == 'PIL':
+            MOD_NAME = 'pillow'
+        sys.stderr.write(
+            f"Error: module '{MOD_NAME}' is required by plot_sourcepars. "
+            "Please install it.\n"
+        )
         sys.exit(1)
```

### Comparing `sourcespec-1.7/bin/source_spec.py` & `sourcespec-1.8/bin/source_residuals.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,47 +1,46 @@
 #!/usr/bin/env python3
 # -*- coding: utf8 -*-
 # SPDX-License-Identifier: CECILL-2.1
 """
-Wrapper to run source_spec.py from source tree.
+Wrapper to run source_residuals.py from source tree.
 
 :copyright:
-    2016-2023 Claudio Satriano <satriano@ipgp.fr>
+    2016-2024 Claudio Satriano <satriano@ipgp.fr>
 :license:
     CeCILL Free Software License Agreement v2.1
     (http://www.cecill.info/licences.en.html)
 """
 import sys
 import os
 import inspect
 
-MIN_PYTHON_VERSION = (3, 6)
+MIN_PYTHON_VERSION = (3, 7)
+# pylint: disable=consider-using-f-string
 MIN_PYTHON_VERSION_STR = '{}.{}'.format(*MIN_PYTHON_VERSION)
-PYTHON_VERSION_STR = '{}.{}.{}'.format(*sys.version_info[0:3])
+PYTHON_VERSION_STR = '{}.{}.{}'.format(*sys.version_info[:3])
 if sys.version_info < MIN_PYTHON_VERSION:
-    msg = 'SourceSpec requires Python version >= {}'.format(
-        MIN_PYTHON_VERSION_STR)
-    msg += ' you are using Python version {}'.format(PYTHON_VERSION_STR)
+    msg = f'SourceSpec requires Python version >= {MIN_PYTHON_VERSION_STR}'
+    msg += f' you are using Python version {PYTHON_VERSION_STR}'
     print(msg, file=sys.stderr)
     sys.exit(1)
 
 if __name__ == '__main__':
     try:
         # Make sure we use current-dir version over installed one
         path = os.path.abspath(os.path.join(os.path.dirname(inspect.getfile(
             inspect.currentframe())), os.pardir))
         sys.path.insert(0, path)
         # Try to import obspy, which requires most of the
-        # source_spec dependencies
-        import obspy #NOQA
-        # Try to import tzlocal, which is required at the end of the run
-        import tzlocal #NOQA
-        from sourcespec.source_spec import main
+        # source_residuals dependencies
+        import obspy  # NOQA  pylint: disable=unused-import
+        from sourcespec.source_residuals import main
         main()
     except ImportError as msg:
-        mod_name = msg.name
-        if mod_name == 'PIL':
-            mod_name = 'pillow'
-        s = "Error: module '{}' is required by source_spec.".format(mod_name)
-        s += " Please install it.\n"
-        sys.stderr.write(s)
+        MOD_NAME = msg.name
+        if MOD_NAME == 'PIL':
+            MOD_NAME = 'pillow'
+        sys.stderr.write(
+            f"Error: module '{MOD_NAME}' is required by source_residuals. "
+            "Please install it.\n"
+        )
         sys.exit(1)
```

### Comparing `sourcespec-1.7/docs/Makefile` & `sourcespec-1.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sourcespec-1.7/docs/api.rst` & `sourcespec-1.8/docs/api.rst`

 * *Files 6% similar despite different names*

```diff
@@ -78,14 +78,19 @@
    :members:
 
 ssp_plot_spectra
 ----------------
 .. automodule:: ssp_plot_spectra
    :members:
 
+ssp_plot_stacked_spectra
+------------------------
+.. automodule:: ssp_plot_stacked_spectra
+   :members:
+
 ssp_plot_params_stats
 ---------------------
 .. automodule:: ssp_plot_params_stats
    :members:
 
 ssp_plot_stations
 -----------------
@@ -109,19 +114,29 @@
    :members:
 
 ssp_data_types
 --------------
 .. automodule:: ssp_data_types
    :members:
 
+ssp_event
+---------
+.. automodule:: ssp_event
+   :members:
+
 ssp_grid_sampling
 -----------------
 .. automodule:: ssp_grid_sampling
    :members:
 
+ssp_pick
+--------
+.. automodule:: ssp_pick
+   :members:
+
 ssp_spectral_model
 ------------------
 .. automodule:: ssp_spectral_model
    :members:
 
 ssp_qml_output
 --------------
@@ -129,19 +144,34 @@
    :members:
 
 ssp_radiation_pattern
 ---------------------
 .. automodule:: ssp_radiation_pattern
    :members:
 
+ssp_read_sac_header
+-------------------
+.. automodule:: ssp_read_sac_header
+   :members:
+
+ssp_read_station_metadata
+-------------------------
+.. automodule:: ssp_read_station_metadata
+   :members:
+
 ssp_sqlite_output
 -----------------
 .. automodule:: ssp_sqlite_output
    :members:
 
+ssp_update_db
+-------------
+.. automodule:: ssp_update_db
+   :members:
+
 ssp_util
 --------
 .. automodule:: ssp_util
    :members:
 
 ssp_wave_arrival
 ----------------
```

### Comparing `sourcespec-1.7/docs/citing.rst` & `sourcespec-1.8/docs/citing.rst`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 ###########
 How to Cite
 ###########
 
 If you used SourceSpec for a scientific paper, please cite it as:
 
-   Satriano, C. (2023). SourceSpec – Earthquake source parameters from
+   Satriano, C. (2024). SourceSpec – Earthquake source parameters from
    P- or S-wave displacement spectra (X.Y). `doi:
    10.5281/ZENODO.3688587 <https://doi.org/10.5281/ZENODO.3688587>`__
 
 Please replace ``X.Y`` with the SourceSpec version number you used.
 
 You can also cite the following abstract presented at the
 2016 AGU Fall Meeting:
```

### Comparing `sourcespec-1.7/docs/clipping_detection.rst` & `sourcespec-1.8/docs/clipping_detection.rst`

 * *Files identical despite different names*

### Comparing `sourcespec-1.7/docs/conf.py` & `sourcespec-1.8/docs/conf.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 # -*- coding: utf-8 -*-
-#
-# SourceSpec documentation build configuration file, created by
-# sphinx-quickstart on Fri Oct 25 17:47:32 2013.
+"""Sphinx configuration file."""
+# pylint: disable=wrong-import-position,invalid-name
 import sys
 import os
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 sys.path.insert(0, os.path.abspath('..'))
 sys.path.insert(0, os.path.join(os.path.abspath('..'), 'sourcespec'))
-from sourcespec._version import get_versions #NOQA
+from sourcespec._version import get_versions  # NOQA
 __version__ = get_versions()['version']
 
 # -- General configuration ----------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 # needs_sphinx = '1.0'
 
@@ -43,20 +42,21 @@
     'scipy',
     'obspy',
     'cartopy',
     'pyproj',
     'lxml',
     'PIL',
     'shapely',
-    'tzlocal'
+    'tzlocal',
+    'h5py'
 ]
 napoleon_use_param = True
 napoleon_preprocess_types = True
 autosectionlabel_prefix_document = True
-bibtex_bibfiles = ['refs.bib']
+bibtex_bibfiles = ['refs.bib', 'citing_papers.bib', 'citing_conferences.bib']
 bibtex_reference_style = 'author_year'
 bibtex_default_style = 'unsrt'
 intersphinx_mapping = {
     'python': ('https://docs.python.org/3', None),
     'numpy': ('https://numpy.org/doc/stable/', None),
     'scipy': ('https://docs.scipy.org/doc/scipy/', None),
     'obspy': ('https://docs.obspy.org', None),
@@ -71,16 +71,16 @@
 # The encoding of source files.
 # source_encoding = 'utf-8-sig'
 
 # The master toctree document.
 master_doc = 'index'
 
 # General information about the project.
-project = u'SourceSpec'
-copyright = u'2013-2023, Claudio Satriano'
+project = 'SourceSpec'
+copyright = '2013-2024, Claudio Satriano'  # pylint: disable=redefined-builtin
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The full version, including alpha/beta/rc tags.
 release = __version__
@@ -225,16 +225,16 @@
     # 'preamble': '',
 }
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title, author,
 #  documentclass [howto/manual]).
 latex_documents = [
-  ('index', 'SourceSpec.tex', u'SourceSpec Documentation',
-   u'Claudio Satriano', 'manual'),
+    ('index', 'SourceSpec.tex', 'SourceSpec Documentation',
+     'Claudio Satriano', 'manual'),
 ]
 
 # The name of an image file (relative to this directory) to place at the top of
 # the title page.
 latex_logo = '../imgs/SourceSpec_logo.png'
 
 # For "manual" documents, if this is true, then toplevel headings are parts,
@@ -255,16 +255,16 @@
 
 
 # -- Options for manual page output -------------------------------------------
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
 man_pages = [
-    ('index', 'sourcespec', u'SourceSpec Documentation',
-     [u'Claudio Satriano'], 1)
+    ('index', 'sourcespec', 'SourceSpec Documentation',
+     ['Claudio Satriano'], 1),
 ]
 
 # If true, show URL addresses after external links.
 # man_show_urls = False
 
 
 # -- Options for Texinfo output -----------------------------------------------
@@ -289,38 +289,42 @@
 # texinfo_domain_indices = True
 
 # How to display URL addresses: 'footnote', 'no', or 'inline'.
 # texinfo_show_urls = 'footnote'
 
 
 # -- Custom functions for SourceSpec ------------------------------------------
-def update_configfile(app):
-    with open('configuration_file.rst', 'w') as fp:
+def write_configfile(app):
+    """Write configuration file documentation page."""
+    # pylint: disable=unused-argument
+    with open('configuration_file.rst', 'w', encoding='utf-8') as fp:
         fp.write('''.. _configuration_file:
 
 ##################
 Configuration File
 ##################
 
 Configuration file (default name: ``source_spec.conf``) is a plain text file
 with keys and values in the form ``key = value``.
 Comment lines start with ``#``.
 
 Here is the default config file, generated through ``source_spec -S``::
 
 ''')
-        configspec = os.path.join('..', 'sourcespec', 'configspec.conf')
-        for line in open(configspec):
+        configspec = os.path.join(
+            '..', 'sourcespec', 'config_files', 'configspec.conf')
+        for line in open(configspec, encoding='utf-8'):
             if '=' in line and line[0] != '#':
                 key, val = line.split(' = ')
                 val = val.split('default=')[1]
                 # remove the word "list" from val
                 val = val.replace('list', '')
                 # remove single quotes and parentheses from val
                 val = val.replace("'", '').replace('(', '').replace(')', '')
                 line = f'{key} = {val}'
             fp.write(f'  {line}')
 
 
 def setup(app):
-    app.connect('builder-inited', update_configfile)
+    """Add custom functions to Sphinx."""
+    app.connect('builder-inited', write_configfile)
     app.add_js_file('version-alert.js')
```

### Comparing `sourcespec-1.7/docs/getting_started.rst` & `sourcespec-1.8/docs/getting_started.rst`

 * *Files 26% similar despite different names*

```diff
@@ -3,33 +3,49 @@
 ###############
 Getting Started
 ###############
 
 For the impatient
 ~~~~~~~~~~~~~~~~~
 
-If you have seismic recordings in
-`miniSEED <http://ds.iris.edu/ds/nodes/dmc/data/formats/miniseed/>`__
-format (e.g., ``traces.mseed``), metadata in
-`StationXML <http://docs.fdsn.org/projects/stationxml/en/latest/>`__
-format (e.g., ``station.xml``) and event information in
-`QuakeML <https://quake.ethz.ch/quakeml/>`__ format (e.g.,
-``event.xml``), then:
+.. note::
+
+   Note that the default config parameters are suited for a M<5 earthquake
+   recorded within ~100 km. Adjust ``win_length``, ``noise_pre_time``, the
+   frequency bands (``bp_freqmin_*``, ``bp_freqmax_*``, ``freq1_*``,
+   ``freq2_*``) and the bounds on ``fc`` and ``t_star``, according to your
+   problem.
+
+Use case: miniSEED + StationXML + QuakeML
+------------------------------------------
+
+If you have seismic recordings in `miniSEED`_ format (e.g., ``traces.mseed``),
+metadata in `StationXML`_ format (e.g., ``station.xml``) and event information
+in `QuakeML`_ format (e.g., ``event.xml``), then:
 
 1. Generate a config file via ``source_spec -S``;
 2. Edit the config file variable ``station_metadata`` to point to
    ``station.xml`` file;
 3. Run ``source_spec -t traces.mseed -q event.xml``.
 
-.. note::
+Use case: SAC + PAZ + SourceSpec Event File
+--------------------------------------------
+
+If you have seismic recordings in `SAC`_ format (e.g., in a directory named
+``sac_data``), metadata as `SAC polezero (PAZ)`_ (e.g., in a directory named
+``paz``) and event information in any format, then:
+
+1. Generate a config file via ``source_spec -S``;
+2. Edit the config file variable ``station_metadata`` to point to the ``paz``
+   directory;
+3. Generate a sample :ref:`source_spec_event_file:SourceSpec Event File` using
+   ``source_spec -y``; this will create a file named ``ssp_event.yaml``;
+4. Edit the file ``ssp_event.yaml`` with your event information;
+5. Run ``source_spec -t sac_data -H ssp_event.yaml``.
 
-   Note that the default config parameters are suited for a M<5 earthquake
-   recorded within ~100 km. Adjust ``win_length``, ``noise_pre_time``, and the
-   frequency bands (``bp_freqmin_*``, ``bp_freqmax_*``, ``freq1_*``,
-   ``freq2_*``) according to your setup.
 
 Command line arguments
 ~~~~~~~~~~~~~~~~~~~~~~
 
 After successfully installed SourceSpec (see :ref:`installation:Installation`),
 you can get help on the command line arguments used by each code by typing from
 your terminal:
@@ -43,18 +59,20 @@
 ``source_spec`` and ``source_model`` require you to provide the path to
 seismic traces via the ``--trace_path`` command line argument (see
 :ref:`file_formats:File formats`).
 
 Information on the seismic event can be stored in the trace header
 (`SAC <https://ds.iris.edu/ds/support/faq/17/sac-file-format/>`__
 format), or provided through a
-`QuakeML <https://quake.ethz.ch/quakeml/>`__ file (``--qmlfile``) or a
-`HYPO71 <https://pubs.er.usgs.gov/publication/ofr72224>`__ or
-`HYPOINVERSE-2000 <https://pubs.er.usgs.gov/publication/ofr02171>`__
-file (``--hypocenter``). See :ref:`file_formats:File Formats` for more
+`QuakeML <https://quake.ethz.ch/quakeml/>`__ file (``--qmlfile``) or,
+alternatively (``--hypocenter``), through
+a :ref:`source_spec_event_file:SourceSpec Event File`,
+a `HYPO71 <https://pubs.er.usgs.gov/publication/ofr72224>`__ file, or
+a `HYPOINVERSE-2000 <https://pubs.er.usgs.gov/publication/ofr02171>`__
+file. See :ref:`file_formats:File Formats` for more
 information on the supported file formats.
 
 Configuration file
 ~~~~~~~~~~~~~~~~~~
 
 ``source_spec`` and ``source_model`` require a configuration file. The
 default file name is ``source_spec.conf``, other file names can be
@@ -66,8 +84,24 @@
 
    source_spec -S
 
 Take your time to go through the generated configuration file (named
 ``source_spec.conf``): the comments within the file will guide you on
 how to set up the different parameters.
 
-More details are in section :ref:`configuration_file:Configuration File`.
+More details are in section :ref:`configuration_file:Configuration File`.
+
+
+.. File format links:
+.. _miniSEED: http://ds.iris.edu/ds/nodes/dmc/data/formats/miniseed/
+.. _SAC: https://ds.iris.edu/ds/support/faq/17/sac-file-format/
+.. _SAC file header: https://ds.iris.edu/files/sac-manual/manual/file_format.html
+.. _QuakeML: https://quake.ethz.ch/quakeml/
+.. _HYPO71: https://pubs.er.usgs.gov/publication/ofr72224
+.. _HYPOINVERSE-2000: https://pubs.er.usgs.gov/publication/ofr02171
+.. _StationXML: http://docs.fdsn.org/projects/stationxml/en/latest/
+.. _Dataless SEED: https://ds.iris.edu/ds/nodes/dmc/data/formats/dataless-seed/
+.. _SEED resp: https://ds.iris.edu/ds/nodes/dmc/data/formats/resp/
+.. _SAC polezero (PAZ): https://www.jakewalter.net/sacresponse.html
+.. _Cartopy: https://scitools.org.uk/cartopy/docs/latest
+.. _SQLite: https://www.sqlite.org
+.. _YAML: https://yaml.org
```

### Comparing `sourcespec-1.7/docs/index.rst` & `sourcespec-1.8/docs/index.rst`

 * *Files 4% similar despite different names*

```diff
@@ -4,24 +4,24 @@
    contain the root `toctree` directive.
 
 SourceSpec documentation
 ========================
 
 Earthquake source parameters from P- or S-wave displacement spectra
 
-:Copyright: 2011-2023 Claudio Satriano satriano@ipgp.fr
+:Copyright: 2011-2024 Claudio Satriano satriano@ipgp.fr
 :Release: |release|
 :Date:    |today|
 
-SourceSpec is a collection of command line tools to compute earthquake
-source parameters (seismic moment, corner frequency, radiated energy,
-source size, stress drop) from the inversion of P-wave and S-wave
+SourceSpec is a collection of command line tools to compute earthquake source
+parameters (seismic moment, corner frequency, radiated energy, source size,
+static stress drop, apparent stress) from the inversion of P-wave and S-wave
 displacement spectra recorded at one or more seismic stations.
-SourceSpec also computes attenuation parameters (t-star, quality factor)
-and, as a bonus, local magnitude.
+SourceSpec also computes attenuation parameters (t-star, quality factor) and,
+as a bonus, local magnitude.
 
 See :cite:t:`Madariaga2011` for a primer on earthquake source parameters and
 scaling laws.
 
 Go to section :ref:`theoretical_background:Theoretical Background`
 to get more information on how the code works.
 
@@ -50,22 +50,25 @@
 
    theoretical_background
    signal_processing
    clipping_detection
    getting_started
    configuration_file
    file_formats
+   source_spec_event_file
+   spectral_file_formats
    installation
    sample_runs
    getting_help
    contributing
    citing
    api
    changelog
    bibliography
+   citing_literature
 
 
 Indices and tables
 ==================
 
 * :ref:`genindex`
 * :ref:`modindex`
```

### Comparing `sourcespec-1.7/docs/installation.rst` & `sourcespec-1.8/docs/installation.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,71 @@
 ############
 Installation
 ############
 
-SourceSpec requires at least Python 3.6. All the required dependencies
+SourceSpec requires at least Python 3.7. All the required dependencies
 will be downloaded and installed during the setup process.
 
 
 Installing the latest release
 -----------------------------
 
-Using pip and PyPI (preferred method)
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+Using Anaconda
+~~~~~~~~~~~~~~
+
+The following command will automatically create an `Anaconda <https://www.anaconda.com/products/individual>`__
+environment named ``sourcespec``, install the required packages and install the latest
+version of SourceSpec via ``pip``:
+
+::
+
+   conda env create --file https://raw.githubusercontent.com/SeismicSource/sourcespec/main/sourcespec_conda_env.yml
+
+If you want a different name for your environment, use:
+
+::
+
+   conda env create -n YOUR_ENV_NAME --file https://raw.githubusercontent.com/SeismicSource/sourcespec/main/sourcespec_conda_env.yml
+
+Activate the environment with:
+
+::
+
+   conda activate sourcespec
+
+(or ``conda activate YOUR_ENV_NAME``)
+
+To keep SourceSpec updated run:
+
+::
+
+   pip install --upgrade sourcespec
+
+from within your environment.
+
+
+Using pip and PyPI
+~~~~~~~~~~~~~~~~~~
 
 The latest release of SourceSpec is available on the `Python Package
 Index <https://pypi.org/project/sourcespec/>`__.
 
 You can install it easily through ``pip``:
 
 ::
 
    pip install sourcespec
 
+To upgrade from a previously installed version:
+
+::
+
+   pip install --upgrade sourcespec
+
+
 From SourceSpec GitHub releases
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 Download the latest release from the `releases
 page <https://github.com/SeismicSource/sourcespec/releases>`__, in
 ``zip`` or ``tar.gz`` format, then:
 
@@ -42,21 +83,20 @@
 uncompress the release files yourself.
 
 
 Installing a developer snapshot
 -------------------------------
 
 If you need a recent feature that is not in the latest release (see the
-``unreleased`` section in `CHANGELOG
-<https://github.com/SeismicSource/sourcespec/blob/master/CHANGELOG.md>`__),
+"unreleased" section in :ref:`changelog`),
 you want to use the more recent development snapshot from the `SourceSpec
 GitHub repository <https://github.com/SeismicSource/sourcespec>`__.
 
-Using pip (preferred method)
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+Using pip
+~~~~~~~~~
 
 The easiest way to install the most recent development snapshot is to download
 and install it through ``pip``, using its builtin ``git`` client:
 
 ::
 
     pip install git+https://github.com/SeismicSource/sourcespec.git
```

### Comparing `sourcespec-1.7/docs/signal_processing.rst` & `sourcespec-1.8/docs/signal_processing.rst`

 * *Files 5% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 
 12. The spectral signal to noise ratio is checked. Amplitude spectra with
     signal to noise ratio smaller than ``spectral_sn_min`` are skipped.
 
 13. The "H" component is built based on one or more spectral components,
     depending on the ``wave_type`` and ``ignore_vertical`` config parameters:
 
-    - if ``wave_type`` is ``S``:
+    - if ``wave_type`` is ``P`` or ``S``:
 
         - if ``ignore_vertical`` is ``False``, the two horizontals and the
           vertical components are combined;
         - if ``ignore_vertical`` is ``True``, only the two horizontals
           components are combined;
 
     - if ``wave_type`` is ``SV``:
@@ -94,19 +94,14 @@
           component are combined;
         - if ``ignore_vertical`` is ``True``, only the radial component is used;
 
     - if ``wave_type`` is ``SH``:
 
         - only the transverse component is used;
 
-    - if ``wave_type`` is ``P``:
-
-        - only the vertical component is used, independently from the value
-          of ``ignore_vertical``.
-
     Spectra are combined through the root sum of squares (see
     :ref:`theoretical_background:Overview`).
 
 14. All the amplitude spectra are converted to moment magnitude units (see
     :ref:`theoretical_background:Building Spectra`).
 
 15. Station corrections are applied, if requested (see
```

### Comparing `sourcespec-1.7/setup.py` & `sourcespec-1.8/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 # -*- coding: utf-8 -*-
 # SPDX-License-Identifier: CECILL-2.1
-"""setup.py: setuptools control."""
-from setuptools import setup
-import versioneer
+"""
+Setup script for SourceSpec
+"""
+# pylint: disable=wrong-import-position, consider-using-f-string
 import sys
 
-MIN_PYTHON_VERSION = (3, 6)
-MIN_PYTHON_VERSION_STR = '{}.{}'.format(*MIN_PYTHON_VERSION)
-PYTHON_VERSION_STR = '{}.{}.{}'.format(*sys.version_info[:3])
+MIN_PYTHON_VERSION = (3, 7)
+MIN_PYTHON_VERSION_STR = '.'.join(str(n) for n in MIN_PYTHON_VERSION)
+PYTHON_VERSION_STR = '.'.join(str(n) for n in sys.version_info[:3])
 if sys.version_info < MIN_PYTHON_VERSION:
-    msg = 'SourceSpec requires Python version >= {}'.format(
-        MIN_PYTHON_VERSION_STR)
-    msg += ' you are using Python version {}'.format(PYTHON_VERSION_STR)
-    print(msg, file=sys.stderr)
-    sys.exit(1)
+    MSG = (
+        'SourceSpec requires Python version >= {}'
+        ' you are using Python version {}'.format(
+            MIN_PYTHON_VERSION_STR, PYTHON_VERSION_STR)
+    )
+    sys.exit(MSG)
 
+from setuptools import setup  # noqa
+import versioneer # noqa
 revision = versioneer.get_versions()['full-revisionid']
 cdn_baseurl = 'https://cdn.jsdelivr.net/gh/SeismicSource/sourcespec@{}'\
     .format(revision)
 with open('README.md', 'rb') as f:
     long_descr = f.read().decode('utf-8').replace(
         'imgs/SourceSpec_logo.svg',
         '{}/imgs/SourceSpec_logo.svg'.format(cdn_baseurl)
@@ -69,24 +73,26 @@
         'Environment :: Console',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: CEA CNRS Inria Logiciel Libre '
             'License, version 2.1 (CeCILL-2.1)',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Topic :: Scientific/Engineering',
         'Topic :: Scientific/Engineering :: Physics'],
     python_requires='>={}'.format(MIN_PYTHON_VERSION_STR),
     install_requires=[
         'numpy>=1.10',
         'scipy>=0.17',
-        'matplotlib>=2.2',
+        'matplotlib>=3.2',
         'pillow>=4.0.0',
         'obspy>=1.2.0',
         'pyproj',
-        'tzlocal']
-    )
+        'tzlocal',
+        'pyyaml>=5.1',
+        'h5py'
+    ]
+)
```

### Comparing `sourcespec-1.7/sourcespec/adjustText/__init__.py` & `sourcespec-1.8/sourcespec/adjustText/__init__.py`

 * *Files identical despite different names*

### Comparing `sourcespec-1.7/sourcespec/cached_tiler.py` & `sourcespec-1.8/sourcespec/cached_tiler.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 """
 CachedTiler class for Catyopy.
 
 :copyright:
-    2018-2023 Claudio Satriano <satriano@ipgp.fr>
+    2018-2024 Claudio Satriano <satriano@ipgp.fr>
 :license:
     CeCILL Free Software License Agreement v2.1
     (http://www.cecill.info/licences.en.html)
 
 Adapted from
 https://github.com/SciTools/cartopy/issues/732#issuecomment-191423035
 """
 import os
 import types
+import logging
 import requests
 import PIL
-import logging
 import numpy as np
 from cartopy.io.img_tiles import _merge_tiles
-logger = logging.getLogger(__name__.split('.')[-1])
+logger = logging.getLogger(__name__.rsplit('.', maxsplit=1)[-1])
 logging.getLogger('PIL').setLevel(logging.WARNING)
 logging.getLogger('requests').setLevel(logging.WARNING)
 logging.getLogger('urllib3').setLevel(logging.WARNING)
 
 
-class CachedTiler(object):
+class CachedTiler():
     """A Cached Tiler for Cartopy."""
 
     def __init__(self, tiler, cache_dir=None):
         """Init with a Cartopy tiler."""
         self.tiler = tiler
         self.cache_dir = cache_dir
 
@@ -68,15 +68,16 @@
             cache_dir = os.path.join(cache_dir, tileset_name)
         if not os.path.exists(cache_dir):
             os.makedirs(cache_dir)
         tile_fname = os.path.join(
             cache_dir, '_'.join(str(v) for v in tile) + '.png')
         if not os.path.exists(tile_fname):
             try:
-                response = requests.get(self._image_url(tile), stream=True)
+                response = requests.get(
+                    self._image_url(tile), stream=True, timeout=5)
             except requests.exceptions.RequestException:
                 logger.warning(
                     'Cannot download map tiles. Check internet connection.')
                 # we call the original tiler, which will return an empty image
                 return self.tiler.get_image(tile)
             with open(tile_fname, 'wb') as fh:
                 for chunk in response:
```

### Comparing `sourcespec-1.7/sourcespec/clipping_detection.py` & `sourcespec-1.8/sourcespec/clipping_detection.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,27 +7,28 @@
 Two methods are available:
     1.  :func:`clipping_score()`: compute a trace clipping score based on the
         shape of the kernel density estimation.
     2.  :func:`clipping_peaks()`: check if trace is clipped, based on the
         number of peaks in the kernel density estimation;
 
 :copyright:
-    2023 Claudio Satriano <satriano@ipgp.fr>,
-         Kris Vanneste <kris.vanneste@oma.be>
+    2023-2024 Claudio Satriano <satriano@ipgp.fr>,
+              Kris Vanneste <kris.vanneste@oma.be>
 :license:
     CeCILL Free Software License Agreement v2.1
     (http://www.cecill.info/licences.en.html)
 """
 import numpy as np
 from scipy.stats import gaussian_kde
 from scipy.signal import find_peaks
 
 
 def _get_baseline(signal):
     """Get the signal baseline using a Savitzky-Golay filter."""
+    # pylint: disable=import-outside-toplevel
     from scipy.signal import savgol_filter
     # search for baselines with characteristic length of at least 1/3
     # of the signal
     wlen = len(signal) // 3
     if wlen % 2 == 0:
         wlen += 1
     return savgol_filter(signal, wlen, 3)
@@ -58,27 +59,27 @@
     return density, density_points
 
 
 def _get_histogram(trace):
     """Compute the histogram of a trace."""
     # Compute data histogram with a number of bins equal to 0.5% of data points
     # or 31, whichever is larger
-    nbins = max(31, int(len(trace.data)*0.005))
+    nbins = max(31, int(len(trace.data) * 0.005))
     if nbins % 2 == 0:
         nbins += 1
     counts, bins = np.histogram(trace.data, bins=nbins)
-    counts = counts/np.max(counts)
+    counts = counts / np.max(counts)
     bin_width = bins[1] - bins[0]
     return counts, bins, bin_width
 
 
 def _get_distance_weight(density_points, order=2, min_weight=1, max_weight=5):
     """Compute the distance weight for the kernel density."""
     dist_weight = np.abs(density_points)**order
-    dist_weight *= (max_weight-min_weight)/dist_weight.max()
+    dist_weight *= (max_weight - min_weight) / dist_weight.max()
     dist_weight += min_weight
     return dist_weight
 
 
 def clipping_peaks(trace, sensitivity=3, clipping_percentile=10, debug=False):
     """
     Check if a trace is clipped, based on the number of peaks in the kernel
@@ -142,35 +143,35 @@
     if clipping_percentile < 0 or clipping_percentile > 100:
         raise ValueError('clipping_percentile must be between 0 and 100')
     if clipping_percentile == 0:
         return False
     lower_clip_bound = 100 - clipping_percentile
     num_kde_bins = 101
     num_edge_bins = int(np.ceil(
-        (num_kde_bins/2.) * (100 - lower_clip_bound) / 100.))
+        (num_kde_bins / 2.) * (100 - lower_clip_bound) / 100.))
     trace, _, _ = _preprocess(
         trace, remove_linear_trend=False, remove_baseline=False)
     min_data = np.min(trace.data)
     max_data = np.max(trace.data)
     density, density_points = _get_kernel_density(
         trace, min_data, max_data, num_kde_bins, bw_method=0.1)
     # Distance weight, parabolic, between 1 and 5
     dist_weight = _get_distance_weight(
         density_points, order=2, min_weight=1, max_weight=5)
-    density_weight = density*dist_weight
+    density_weight = density * dist_weight
     # Add 1 bin at start/end with value equal to min. of 5 first/last
     # bins to ensure local maxima at start/end are recognized as peaks
     density_weight = np.hstack([[density_weight[:num_edge_bins].min()],
                                 density_weight,
                                 [density_weight[-num_edge_bins:].min()]])
     # find peaks with minimum prominence based on clipping sensitivity
     min_prominence = [0.5, 0.3, 0.2, 0.15, 0.125]
     peaks, props = find_peaks(
         density_weight,
-        prominence=min_prominence[sensitivity-1]
+        prominence=min_prominence[sensitivity - 1]
     )
     # Remove start/end bins again
     peaks = peaks[(peaks > 0) & (peaks < (num_kde_bins + 1))]
     peaks -= 1
     density_weight = density_weight[1:-1]
     npeaks = len(peaks)
     # Clipped peaks are peaks in the edge bins
@@ -192,15 +193,15 @@
         _plot_clipping_analysis(
             trace, abs_max_data, density_points, density, density_weight,
             peaks=peaks, num_edge_bins=num_edge_bins,
             num_kde_bins=num_kde_bins, trace_clipped=trace_clipped)
     return trace_clipped, properties
 
 
-def clipping_score(trace, remove_baseline=False, debug=False):
+def compute_clipping_score(trace, remove_baseline=False, debug=False):
     """
     Compute a trace clipping score based on the shape of the kernel density
     estimation of the trace amplitude values.
 
     The algorithm is based on the following steps:
 
     1.  The trace is detrended and demeaned. Optionally, the trace baseline
@@ -249,60 +250,67 @@
 
     A debug mode is available to plot the trace, the samples histogram, the
     kernel density (unweighted and weighted), the kernel baseline model,
     and the misfit.
     """
     trace, trace_baseline, max_data = _preprocess(
         trace, remove_linear_trend=True, remove_baseline=remove_baseline)
-    density, density_points = _get_kernel_density(
-        trace, -max_data, max_data, 101)
+    try:
+        density, density_points = _get_kernel_density(
+            trace, -max_data, max_data, 101)
+    except Exception:
+        # if the kernel density estimation fails (e.g., all samples are equal)
+        # return the maximum clipping score
+        return 100
     # Distance weight for full weighted kernel density,
     # 8th order, between 1 and 100
     dist_weight_full = _get_distance_weight(
         density_points, order=8, min_weight=1, max_weight=100)
     # Compute full weighted kernel density, including the central part
-    density_weight_full = density*dist_weight_full
+    density_weight_full = density * dist_weight_full
     # Distance weight for weighted kernel density without central peak,
     # 8th order, between 0 and 100
     dist_weight_no_central = _get_distance_weight(
         density_points, order=8, min_weight=0, max_weight=100)
     # Compute weighted kernel density, excluding the central part
-    density_weight_no_central = density*dist_weight_no_central
+    density_weight_no_central = density * dist_weight_no_central
     # Compute the clipping score
     clipping_score = 100 *\
-        np.sum(density_weight_no_central**2)/np.sum(density_weight_full**2)
+        np.sum(density_weight_no_central**2) / np.sum(density_weight_full**2)
     if debug:
         _plot_clipping_analysis(
             trace, max_data, density_points, density, density_weight_full,
             trace_baseline=trace_baseline,
             density_weight_no_central=density_weight_no_central,
             clipping_score=clipping_score)
     return clipping_score
 
 
 def _get_plotting_axes():
     """Get matplotlib axes for plotting"""
+    # pylint: disable=import-outside-toplevel unused-import
     # Force loading of a matplotlib GUI backend
     import matplotlib
     mpl_backends = 'macosx', 'qt5agg', 'qt4agg', 'gtk3agg', 'tkagg', 'wxagg'
     for backend in mpl_backends:
         try:
             matplotlib.use(backend, force=True)
-            from matplotlib import pyplot  #noqa
+            from matplotlib import pyplot  # noqa
             break
         except Exception:
             continue
     import matplotlib.pyplot as plt
     from matplotlib.ticker import ScalarFormatter
 
     class ScalarFormatterForceFormat(ScalarFormatter):
-        def _set_format(self, *args):
+        """ScalarFormatter with forced format"""
+        def _set_format(self, *_args):
             self.format = '%1.1f'
 
-    fig, (ax_trace, ax_density) = plt.subplots(
+    _fig, (ax_trace, ax_density) = plt.subplots(
         1, 2, figsize=(15, 5), sharey=True)
     yfmt = ScalarFormatterForceFormat()
     yfmt.set_powerlimits((0, 0))
     ax_trace.yaxis.set_major_formatter(yfmt)
     ax_trace.grid(True)
     ax_trace.set_xlabel('Time (s)')
     ax_trace.set_ylabel('Amplitude')
@@ -333,15 +341,15 @@
             trace.times(), trace_baseline, zorder=20, label='baseline')
         ax_trace.legend()
     ax_trace.set_ylim(-max_data, max_data)
     ax_trace.set_title(trace.id)
     # density plots
     counts, bins, bin_width = _get_histogram(trace.data)
     ax_density.hist(
-        bins[:-1] + bin_width/2., bins=len(counts), weights=counts,
+        bins[:-1] + bin_width / 2., bins=len(counts), weights=counts,
         orientation='horizontal', zorder=10)
     ax_density.plot(density, density_points, label='kernel density', zorder=20)
     ax_density.plot(
         density_weight, density_points,
         label='weighted kernel density', zorder=30)
     if density_weight_no_central is not None:
         ax_density.fill_betweenx(
@@ -354,26 +362,27 @@
             s=100, marker='x', color='red')
     ax_density.legend()
     if num_edge_bins is not None and num_kde_bins is not None:
         ax_density.axhspan(
             -max_data, density_points[num_edge_bins],
             alpha=0.5, color='yellow')
         ax_density.axhspan(
-            density_points[num_kde_bins-1-num_edge_bins], max_data,
+            density_points[num_kde_bins - 1 - num_edge_bins], max_data,
             alpha=0.5, color='yellow')
     if clipping_score is not None:
         ax_density.set_title(f'Clipping score: {clipping_score:.2f}%')
     if trace_clipped:
         ax_density.set_title('Clipped!')
     plt.tight_layout()
     plt.show()
 
 
 def _parse_arguments():
     """Parse command line arguments"""
+    # pylint: disable=import-outside-toplevel
     import sys
     import argparse
     description = """\
 Check for clipping in traces, based on the kernel density estimation of the
 trace amplitude values.
 
 Two methods are implemented:
@@ -424,49 +433,50 @@
         sys.stderr.write(
             'Error: at least one positional argument is required.\n')
         sys.exit(2)
     return args
 
 
 # ainsi codes for fancy output
-reset = "\u001b[0m"
-red = "\u001b[31m"
-green = "\u001b[32m"
-yellow = "\u001b[33m"
+RESET = "\u001b[0m"
+RED = "\u001b[31m"
+GREEN = "\u001b[32m"
+YELLOW = "\u001b[33m"
 
 
 def _run_clipping_peaks(trace, args):
     """Run clipping peaks method and print results"""
     trace_clipped, properties = clipping_peaks(
         trace, args.sensitivity, args.clipping_percentile, args.debug)
     msg = (
         f'{trace.id} - '
         f'total peaks: {properties["npeaks"]}, '
         f'clipped peaks: {properties["npeaks_clipped"]}'
     )
     if trace_clipped:
-        msg += f' - {red}clipped!{reset}'
+        msg += f' - {RED}clipped!{RESET}'
     print(msg)
 
 
 def _run_clipping_score(trace, args):
     """Run clipping score method and print results"""
-    score = clipping_score(
+    score = compute_clipping_score(
         trace, args.remove_baseline, args.debug)
     if score < 10:
-        color = green
+        color = GREEN
     elif score < 20:
-        color = yellow
+        color = YELLOW
     else:
-        color = red
-    print(f'{trace.id} - clipping score: {color}{score:.2f}%{reset}')
+        color = RED
+    print(f'{trace.id} - clipping score: {color}{score:.2f}%{RESET}')
 
 
 def _command_line_interface():
     """Command line interface"""
+    # pylint: disable=import-outside-toplevel
     from obspy import read, Stream
     args = _parse_arguments()
     st = Stream()
     for file in args.infile:
         try:
             st += read(file)
         except Exception as msg:
@@ -480,14 +490,16 @@
         if args.command == 'clipping_peaks':
             _run_clipping_peaks(tr, args)
         elif args.command == 'clipping_score':
             _run_clipping_score(tr, args)
 
 
 def main():
+    """Main function"""
+    # pylint: disable=import-outside-toplevel
     import sys
     try:
         _command_line_interface()
     except Exception as msg:
         sys.exit(msg)
     except KeyboardInterrupt:
         sys.exit()
```

### Comparing `sourcespec-1.7/sourcespec/config.py` & `sourcespec-1.8/sourcespec/config.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # -*- coding: utf8 -*-
 # SPDX-License-Identifier: CECILL-2.1
 """
 Config class for sourcespec.
 
 :copyright:
-    2013-2023 Claudio Satriano <satriano@ipgp.fr>
+    2013-2024 Claudio Satriano <satriano@ipgp.fr>
 :license:
     CeCILL Free Software License Agreement v2.1
     (http://www.cecill.info/licences.en.html)
 """
 
 
 class Config(dict):
     """Config class for sourcespec."""
 
     def __setitem__(self, key, value):
         """Make Config keys accessible as attributes."""
-        super(Config, self).__setattr__(key, value)
-        super(Config, self).__setitem__(key, value)
+        super().__setattr__(key, value)
+        super().__setitem__(key, value)
 
     def __getattr__(self, key):
         """Make Config keys accessible as attributes."""
         try:
             return self.__getitem__(key)
         except KeyError as err:
             raise AttributeError(err) from err
```

### Comparing `sourcespec-1.7/sourcespec/configobj/__init__.py` & `sourcespec-1.8/sourcespec/configobj/__init__.py`

 * *Files identical despite different names*

### Comparing `sourcespec-1.7/sourcespec/configobj/validate.py` & `sourcespec-1.8/sourcespec/configobj/validate.py`

 * *Files identical despite different names*

### Comparing `sourcespec-1.7/sourcespec/configspec.conf` & `sourcespec-1.8/sourcespec/config_files/configspec.conf`

 * *Files 25% similar despite different names*

```diff
@@ -37,16 +37,23 @@
 
 # List of traceids to use.
 # Use network.station.location.channel; wildcards are accepted
 # Example:
 #   use_traceids = FR.CIEL.*.*, AM.RA0D3.00.*
 use_traceids = force_list(default=None)
 
-# Maximum epicentral distance (km) to process a trace
-max_epi_dist = float(min=0, default=None)
+# Epicentral distance ranges (km) to select stations to be processed.
+# Use a list of alternating min/max values, ex.:
+#   to only use stations between 0 and 100 km:
+#       epi_dist_ranges = 0, 100
+#   to avoid teleseismic distances between 14° (1300 km) and 29° (3200 km)
+#   where the P-wave undergoes travel time triplications:
+#       epi_dist_ranges = 0, 1300, 3200, 999999
+# Leave it to None to use all stations.
+epi_dist_ranges = float_list(default=None)
 
 # Directory or single file name containing station metadata
 # (instrument response and station coordinates).
 # Note: this parameter can be overridden by the command line option
 #       with the same name.
 # Station metadata files can be in one of the following formats:
 #   StationXML, dataless SEED, SEED RESP, PAZ (SAC polezero format)
@@ -115,23 +122,29 @@
 # since they will be superseded by each station's coordinates.
 NLL_time_dir = string(default=None)
 
 # Arrival tolerances (in seconds) to accept a manual P or S pick
 p_arrival_tolerance = float(min=0, default=4.0)
 s_arrival_tolerance = float(min=0, default=4.0)
 
-# Start time (in seconds) of the noise window, respect to the P arrival time
-noise_pre_time = float(default=6.0)
+# Start time (in seconds) of the noise window, respect to the P window
+# If None, it will be set to the length of the signal (P or S) window plus
+# the value of "signal_pre_time" (see below)
+noise_pre_time = float(min=0.01, default=6.0)
 
 # Start time (in seconds) of the signal window, respect to the P or S arrival
 # times (see "wave_type" below)
 signal_pre_time = float(default=1.0)
 
 # Length (in seconds) for both noise and signal windows
 win_length = float(min=0, default=5.0)
+# Variable window length factor (fraction of travel time):
+#   win_length = max(win_length, variable_win_length_factor * travel_time)
+# Set to None to disable variable window length.
+variable_win_length_factor = float(min=0.01, default=None)
 # -------- TIME WINDOW PARAMETERS
 
 
 # SPECTRUM PARAMETERS --------
 # Wave type to analyse: 'P', 'S', 'SH' or 'SV'
 # If 'SH' or 'SV' are selected, traces are rotated in the radial-transverse
 # system. Transverse component is used for 'SH', radial component (and
@@ -170,16 +183,17 @@
 #  f1=f0/(10^0.5) and f2=f0*(10^0.5)
 #    or,
 #  f2/f1=10 (1 decade width)
 # Default value of 0.2 is generally a good choice
 spectral_smooth_width_decades = float(min=1e-99, default=0.2)
 
 # Residuals file path
-# (a pickle file with the mean residuals per station,
-# used for station correction):
+# An HDF5 file with the mean residuals per station, used for station
+# correction. This file is generally created using the command
+# "source_residuals" on a previous SourceSpec run.
 residuals_filepath = string(default=None)
 
 # Remove the signal baseline after instrument correction and before filtering
 remove_baseline = boolean(default=False)
 
 # Band-pass frequencies (Hz) for accelerometers, velocimeters
 # and displacement sensors.
@@ -204,14 +218,17 @@
 freq2_acc     = float(min=0, default=30.0)
 freq1_shortp  = float(min=0, default=1.0)
 freq2_shortp  = float(min=0, default=30.0)
 freq1_broadb  = float(min=0, default=0.5)
 freq2_broadb  = float(min=0, default=30.0)
 freq1_disp    = float(min=0, default=0.5)
 freq2_disp    = float(min=0, default=30.0)
+
+# Save the spectra to an HDF5 file in the output directory
+save_spectra = boolean(default=False)
 # -------- SPECTRUM PARAMETERS
 
 
 # SIGNAL/NOISE PARAMETERS --------
 # Minimum rms (in trace units before instrument corrections)
 # to consider a trace as noise
 rmsmin = float(min=0, default=0)
@@ -260,109 +277,199 @@
 clipping_peaks_percentile = float(min=0, max=100, default=10)
 
 # Maximum gap length for the whole trace, in seconds
 gap_max = float(min=0, default=None)
 # Maximum overlap length for the whole trace, in seconds
 overlap_max = float(min=0, default=None)
 
-# Spectral S/N ratio min, below which a spectrum will be skipped
+# Minimum average spectral S/N ratio, below which a spectrum will be skipped
 spectral_sn_min = float(min=0, default=0)
-# Frequency range (Hz) to compute the spectral S/N ratio
+# Frequency range (Hz) to compute the average spectral S/N ratio
 # (comment out or use None to indicate the whole frequency range)
 # Example:
 #  spectral_sn_freq_range = 0.1, 2
 spectral_sn_freq_range = float_list(min=0, default=None)
 # -------- SIGNAL/NOISE PARAMETERS
 
 
 # SPECTRAL MODEL PARAMETERS --------
+# Free-surface amplification factor
+free_surface_amplification = float(min=0.01, default=2.0)
+# Layer top depths (km, positive down), for layered models (see below)
+#  Note: generally, the first layer top depth should be 0 or a negative value
+layer_top_depths = force_list(default=None)
 # P and S wave velocity close to the source (km/s)
-vp_source = float(min=0, default=5.5)
-vs_source = float(min=0, default=3.2)
+# It can be a single value or a list of values (layered model)
+# Set to None to use velocity from the global Earth model 'iasp91'
+#   Note: specifying a layered model is useful when the same config file is
+#   used for several SourceSpec runs with sources at different depths
+vp_source = force_list(default=5.5)
+vs_source = force_list(default=3.2)
 # P and S wave velocity close to the stations (km/s)
 # If set to None, velocity values close to the source will be used
+# If set to None and velocity values close to the source are also set to None,
+# then the global Earth model 'iasp91' will be used
 vp_stations = float(min=0, default=None)
 vs_stations = float(min=0, default=None)
-# Note: if both v(p,s)_source and v(p,s)_stations are set to None, then
-# velocities will be extracted from the global velocity model 'iasp91'
-# As an alternative, a directory containing a NonLinLoc model can be specified
-# In this case, the values provided above will be ignored
+# As an alternative, a directory containing a NonLinLoc velocity model can be
+# specified. In this case, the values provided above will be ignored
 NLL_model_dir = string(default=None)
-# Density (kg/m3):
-rho = float(min=0, default=2500)
-# P-wave average radiation pattern coefficient:
-rpp = float(min=0, default=0.52)
-# S-wave average radiation pattern coefficient:
-rps = float(min=0, default=0.62)
-# Radiation pattern from focal mechanism, if available
-rp_from_focal_mechanism = boolean(default=False)
+# Density close to the source (kg/m3)
+# It can be a single value or a list of values (layered model)
+# Set to None to use density from the global Earth model 'iasp91'
+#   Note: specifying a layered model is useful when the same config file is
+#   used for several SourceSpec runs with sources at different depths
+rho_source = force_list(default=2500)
+# Density close to the stations (kg/m3)
+# If set to None, density value close to the source will be used
+# If set to None and the density value close to the source is also set to None,
+# then the global Earth model 'iasp91' will be used
+rho_stations = float(min=0, default=None)
 # Geometrical spreading correction of wave amplitude.
 # Spectra will be multiplied by this value to correct for the lost amplitude.
 # Possible options are:
-#    'r_power_n':  "r" to the power of "n" (rⁿ).
-#                  You must provide the value of the exponent "n"
-#                  (see "geom_spread_n_exponent" below).
-#    'boatwright': "r" (body waves) geometrical spreading for hypocentral
-#                  distances below a cutoff distance; frequency-dependent
-#                  geometrical spreading above the cutoff distance (Boatwright
-#                  et al., 2002). You must provide the cutoff distance (see
-#                  "geom_spread_cutoff_distance" below).
+#    'r_power_n':   "r" to the power of "n" (rⁿ).
+#                   You must provide the value of the exponent "n"
+#                   (see "geom_spread_n_exponent" below).
+#    'boatwright':  "r" (body waves) geometrical spreading for hypocentral
+#                   distances below a cutoff distance; frequency-dependent
+#                   geometrical spreading above the cutoff distance (Boatwright
+#                   et al., 2002). You must provide the cutoff distance (see
+#                   "geom_spread_cutoff_distance" below). This coefficient can
+#                   be a valid choice for regional distances (up to 200 km),
+#                   where S-waves, Lg waves and surface waves are mixed.
 geom_spread_model = option('r_power_n', 'boatwright', default='r_power_n')
 # Exponent "n" for the "r_power_n" geometrical spreading coefficient (positive
 # float). Examples:
 #   geom_spread_n_exponent = 1 (default, body wave in a homogeneous full-space)
 #   geom_spread_n_exponent = 0.5 (surface wave in a homogeneous half-space)
 geom_spread_n_exponent = float(min=0, default=1)
-# Geometrical spreading cutoff distance, in km, for the "boatwright" model:
-geom_spread_cutoff_distance = float(min=0, default=100)
+# Geometrical spreading cutoff hypocentral distance, in km, for the
+# "boatwright" model:
+geom_spread_cutoff_distance = float(min=0.01, default=50)
+# Minimum epicentral distance (in km) to use a teleseismic geometrical
+# spreading model. Above this distance, the model from Okal (1992) for body
+# waves spreading in a spherically symmetric Earth will be used.
+# Set to None to never use the teleseismic geometrical spreading model.
+# Note that this model might not be appropriate for very deep events.
+geom_spread_min_teleseismic_distance = float(min=0.01, default=None)
+# P-wave average radiation pattern coefficient:
+rpp = float(min=0, default=0.52)
+# S-wave average radiation pattern coefficient:
+rps = float(min=0, default=0.62)
+# Radiation pattern coefficient from focal mechanism, if available.
+#   Note: radiation pattern is computed for the first arriving phase and might
+#   not be correct for windows involving multiple phase arrivals (e.g.,
+#   Lg waves, surface waves at regional distances, depth phases at teleseismic
+#   distances)
+rp_from_focal_mechanism = boolean(default=False)
+# "kp" and "ks" coefficients to compute source radius a from the P-wave
+# corner frequency fc_p or the S-wave corner frequency fc_s and the shear
+# wave speed beta ("vs_source"):
+#
+#   a = kp * beta / fc_p
+#   a = ks * beta / fc_s
+#
+# (Madariaga, 2009; Kaneko and Shearer, 2014)
+#
+# The default value for S-waves is "ks = 0.3724", obtained by Brune (1970)
+# for a static circular crack.
+# Other values are discussed in Kaneko and Shearer (2014) for a dynamic
+# circular crack, as a function of the ratio Vr/beta, where Vr is the rupture
+# speed:
+#
+#   Vr/beta  kp(K&S)   ks(K&S)   kp(Mada)   ks(Mada)   kp(S&H)   ks(S&H)
+#   0.9      0.38      0.26      0.32       0.21       0.42      0.29
+#   0.8      0.35      0.26                            0.39      0.28
+#   0.7      0.32      0.26                            0.36      0.27
+#   0.6      0.30      0.25                            0.34      0.27
+#   0.5      0.28      0.22                            0.31      0.24
+#
+#   K&S: Kaneko and Shearer (2014)
+#   Mada: Madariaga (1976)
+#   S&H: Sato and Hirasawa (1973)
+kp = float(min=0, default=0.38)
+ks = float(min=0, default=0.3724)
 # -------- SPECTRAL MODEL PARAMETERS
 
 
 # INVERSION PARAMETERS --------
-# Weighting type: 'noise', 'frequency' or 'no_weight'
-weighting = option('noise', 'frequency', 'no_weight', default='noise')
-# Parameters for 'frequency' weighting (ignored for 'noise' weighting):
+# Weighting type: 'noise', 'frequency', 'inv_frequency' or 'no_weight'
+#   'noise':         spectral signal/noise ratio weighting
+#   'frequency':     a constant weight is applied for f<=f_weight
+#                    a weight of 1 is used for f>f_weight
+#                    (see "f_weight" and "weight" below)
+#   'inv_frequency': weight is computed as 1/(f-f0+0.25)**0.25 for f<=f1,
+#                    weight is 0 for f<f0 and f>f1.
+#                    f0 and f1 are the first and last frequencies where
+#                    spectral signal/noise ratio is above 3, or the first and
+#                    last frequencies of the entire spectrum if no noise window
+#                    is available
+#   'no_weight':     no weighting
+weighting = option('noise', 'frequency', 'inv_frequency', 'no_weight', default='noise')
+# Parameters for 'frequency' weighting (ignored for the other weighting types):
 #   weight for f<=f_weight (Hz)
 #   1      for f> f_weight (Hz)
 f_weight = float(min=0, default=7.)
 weight = float(min=0, default=10.)
 
-# Initial value for t_star (seconds)
-t_star_0 = float(default=0.045)
-# Try to invert for t_star_0.
-# If the inverted t_star_0 is non-positive, then fixed t_star_0 will be used
-invert_t_star_0 = boolean(default=False)
-# Allowed variability around inverted t_star_0 in the main inversion
-# (expressed as a fraction of t_star_0, between 0 and 1).
-# If the inverted t_star_0 is non-positive, then t_star_min_max is used
-# (see below).
-t_star_0_variability = float(min=0, default=0.1)
 # Inversion algorithm:
 # TNC: truncated Newton algorithm (with bounds)
 # LM: Levenberg-Marquardt algorithm
 # (warning: Trust Region Reflective algorithm will be used instead if
 #  bounds are provided)
 # BH: basin-hopping algorithm
 # GS: grid search
 # IS: importance sampling of misfit grid, using k-d tree
 inv_algorithm = option('TNC', 'LM', 'BH', 'GS', 'IS', default='TNC')
-# Parameter bounds:
-# Notes:
-# 1. Mw bounds are autoset between 0.9*min(Mw(f)) and 1.1*max(Mw(f)),
-#    where Mw(f) is the low frequency spectral plateau in magnitude units.
-#    If noise weighting is used, frequencies for which S/N(f) < 0.5*max(S/N(f))
-#    will be ignored, where S/N(f) is the spectral signal to noise ratio.
-# 2. If not specified, fc bounds will be autoset to fc0/10 and fc0*10, i.e. two
+
+# Mw initial value and bounds.
+# Set to True to use the magnitude (or scalar moment) from event file as
+# initial Mw value for the inversion, instead of computing it from the average
+# of the spectral plateau.
+# If the event file does not contain a magnitude value or a scalar moment,
+# then this parameter is ignored
+Mw_0_from_event_file = boolean(default=False)
+# Allowed variability for Mw in the inversion
+# (expressed as a fraction of Mw_0, between 0 and 1).
+# This parameter is interpreted differently, depending on whether
+# Mw_0_from_event_file is True or False:
+#   - If Mw_0_from_event_file is True, then Mw_variability is interpreted as
+#     the allowed variability around the Mw value provided in the event file.
+#   - If Mw_0_from_event_file is False, then the Mw bounds are defined as
+#       Mw_min = min(Mw(f))*(1-Mw_0_variability)
+#       Mw_max = max(Mw(f))*(1+Mw_0_variability),
+#     where Mw(f) is the low frequency spectral plateau in magnitude units.
+#     If noise weighting is used, frequencies for which
+#     S/N(f) < 0.5*max(S/N(f)) will be ignored, where S/N(f) is the spectral
+#     signal to noise ratio.
+Mw_0_variability = float(min=0, default=0.1)
+
+# Bounds for fc (Hz)
+# Specify bounds as a list, ex.:
+#   fc_min_max = 0.1, 40
+# Note:
+#    If not specified, fc bounds will be autoset to fc0/10 and fc0*10, i.e. two
 #    decades around fc0. The value of fc0 is set as the first maximum of
 #    spectral S/N (noise weighting), or at "f_weight" (frequency weighting),
-#    or at half of the frequency window (no weighting)
-# 3. Specify bounds as a list, ex.:
-#      fc_min_max = 0.1, 40
-#    (comment out or use None to indicate no bound)
+#    or at frequency where weight is 30% below the maximum (inverse-frequency
+#    weighting) or at half of the frequency window (no weighting)
 fc_min_max = float_list(min=0, default=None)
+
+# Initial value and bounds for t_star (seconds)
+t_star_0 = float(default=0.045)
+# Try to invert for t_star_0.
+# If False, then the fixed t_star_0 defined above will be used.
+# If the inverted t_star_0 is non-positive, then fixed t_star_0 will be used
+invert_t_star_0 = boolean(default=False)
+# Allowed variability around inverted t_star_0 in the inversion
+# (expressed as a fraction of t_star_0, between 0 and 1).
+# If the inverted t_star_0 is non-positive, then t_star_min_max is used
+# (see below).
+t_star_0_variability = float(min=0, default=0.1)
 # t_star_min_max does not supersede t_star_0_variability
 t_star_min_max = float_list(default=list(0.001, 0.25))
 # optional : Qo bounds (converted into t_star bounds in the code).
 # (comment out or use None to indicate no bound)
 # Note: if you want to explore negative t_star values, you have to specify
 # -Qo_min, Qo_min. This because t_star is proportional to 1/Qo.
 # Example, for searching only positive t_star values:
@@ -378,26 +485,42 @@
 # Sometimes it is better to be more permissive with inversion parameters and
 # reject "bad" solutions after the inversion, rather than forcing the
 # inversion to converge within strict bounds.
 # fc bounds, in Hz
 pi_fc_min_max = float_list(min=0, default=None)
 # t_star bounds, in s
 pi_t_star_min_max = float_list(default=None)
-# Brune stress drop bounds, in MPa
-pi_bsd_min_max = float_list(min=0, default=None)
+# Static stress drop bounds, in MPa
+pi_ssd_min_max = float_list(min=0, default=None)
 # Maximum acceptable misfit between inverted and observed spectrum
 pi_misfit_max = float(min=0, default=None)
 # -------- POST-INVERSION PARAMETERS
 
 
 # RADIATED-ENERGY PARAMETERS --------
-# Maximum frequency (Hz) to measure radiated energy Er
-# (above this frequency, the finite-band correction
-# of Di Bona & Rovelli, 1988, will be applied)
-max_freq_Er = float(min=0, default=None)
+# Minimum and maximum frequency (Hz) to measure radiated energy Er
+# Examples:
+#   Set min and max frequency to the "noise limits"
+#   (i.e. the frequency range where spectral signal/noise ratio is above 3):
+#       Er_freq_range = noise, noise
+#   Use the whole spectrum:
+#       Er_freq_range = None
+#           or
+#       Er_freq_range = None, None
+#   Use the lowest possible frequency, and set the max frequency
+#   to the "noise limit":
+#       Er_freq_range = None, noise
+#   Use frequencies between 1 and 10 Hz
+#       Er_freq_range = 1, 10
+#   Use frequencies between 1 and the "noise limit"
+#       Er_freq_range = 1, noise
+#
+# The finite-band correction of Di Bona & Rovelli (1988) will be applied
+# to account for the missing energy above the maximum frequency.
+Er_freq_range = list(default=list(None, None))
 # -------- RADIATED-ENERGY PARAMETERS
 
 
 # LOCAL MAGNITUDE PARAMETERS --------
 compute_local_magnitude = boolean(default=False)
 # Local magnitude parameters:
 #   ml = log10(A) + a * log10(R/100) + b * (R-100) + c
@@ -453,14 +576,17 @@
 
 
 # PLOT PARAMETERS --------
 # Show interactive plots (slower)
 plot_show = boolean(default=False)
 # Save plots to disk
 plot_save = boolean(default=True)
+# Save trace and spectrum plots as soon as they are ready.
+# This uses less memory but slows down the code.
+plot_save_asap = boolean(default=False)
 # Plot file format: 'png', 'pdf', 'pdf_multipage' or 'svg'
 plot_save_format = option('png', 'pdf', 'pdf_multipage', 'svg', default='png')
 # Plots an extra synthetic spectrum with no attenuation
 plot_spectra_no_attenuation = boolean(default=False)
 # Plots an extra synthetic spectrum with no fc
 plot_spectra_no_fc = boolean(default=False)
 # Max number of rows in plots
@@ -468,43 +594,75 @@
 plot_traces_maxrows = integer(min=1, default=3)
 # Plot ignored traces (clipped or low S/N)
 plot_traces_ignored = boolean(default=True)
 # Plot ignored spectra (low S/N)
 plot_spectra_ignored = boolean(default=True)
 # Plot station map
 plot_station_map = boolean(default=False)
+# Map style (for regional maps)
+#   Options: 'hillshade', 'hillshade_dark', 'ocean', 'satellite',
+#            'stamen_terrain', 'no_basemap'
+#   All basemap are from Esri, except 'stamen_terrain' which is from Stamen.
+#   Notes:
+#     1. The map style is only used for regional maps.
+#        At teleseismic distances, the global map will alyaws use the
+#        Natural Earth basemap.
+#     2. For the 'stamen_terrain' basemap, you need a (free) API key from
+#        Stadia Maps, see https://stadiamaps.com
+plot_map_style = option('hillshade', 'hillshade_dark', 'ocean', 'satellite', 'stamen_terrain', 'no_basemap', default='no_basemap')
+# API key for the 'stamen_terrain' basemap
+#   Note: for privacy reasons, this parameter is not transcripted to the
+#   output config file.
+plot_map_api_key = string(default=None)
 # Plot station names on map
 plot_station_names_on_map = boolean(default=False)
 # Text size for station names
 plot_station_text_size = float(min=0, default=8)
 # Coastline resolution
 # Use None to let the code autoset the coastline resolution.
-# Otherwise choose one of: 'full', 'high', 'intermediate', 'low' or 'crude'
-plot_coastline_resolution = option('full', 'high', 'intermediate', 'low', 'crude', default=None)
+# Otherwise choose one of:
+#   'full', 'high', 'intermediate', 'low', 'crude', 'no_coastline'
+plot_coastline_resolution = option('full', 'high', 'intermediate', 'low', 'crude', 'no_coastline', default=None)
 # Zoom level for map tiles
 # Use None to let the code autoset the zoom level
 # Otherwise choose an integer between 1 (minimum zoom) and 18 (maximum zoom)
 # Note: for zoom levels larger than 11, some map tiles could be missing
-plot_map_tiles_zoom_level = integer(min=1, max=18, default=None)
+plot_map_tiles_zoom_level = integer(min=1, max=23, default=None)
 # -------- PLOT PARAMETERS
 
 
 # HTML REPORT --------
 # Generate an HTML page summarizing the results of this run
 # Note: "plot_save_format" (above) must be "png" or "svg"
 html_report = boolean(default=False)
 # Link to event page. If set, the event ID on the HTML page will be a link to
 # the event page. Use $EVENTID to indicate the current event ID.
 # Example:
 #   event_url = https://earthquake.usgs.gov/earthquakes/eventpage/$EVENTID/executive
 event_url = string(default=None)
 # -------- HTML REPORT
 
+# QUAKEML INPUT PARAMETERS --------
+# Parameters for QuakeML input.
+# Set "qml_event_description" to True, if you want to obtain the event name
+# from the QuakeML event "description" tag
+qml_event_description = boolean(default=False)
+# If "qml_event_description" is True, then the following parameter can be used
+# to define a regular expression to extract the event name from the QuakeML
+# event "description" tag.
+# Examples:
+#   - For QuakeML produced by https://api.franceseisme.fr, we want to keep
+#     only the string "near of CITY NAME":
+#        qml_event_description_regex = 'near of .+'
+# Leave to None to use the full description as event name.
+qml_event_description_regex = string(default=None)
+# -------- QUAKEML INPUT PARAMETERS
+
 
-# QUAKEML PARAMETERS ----------------
+# QUAKEML OUTPUT PARAMETERS ----------------
 # Parameters for QuakeML output.
 #
 # A QuakeML file will be generated only if QuakeML is used for input.
 # The output file will be based on the input file, with additional information
 # on seismic moment, Mw and source parameters computed by SourceSpec.
 # Note: if you don't understand the parameters below, then probably you
 # don't need QuakeML output and you can leave all the parameters to their
@@ -533,8 +691,8 @@
 # Use $ORIGIN_ID to indicate the id of the associated Origin.
 smi_moment_tensor_template = string(default="$SMI_BASE/MomentTensor/Origin/$ORIGIN_ID#sourcespec")
 # Template for the FocalMechanism object id (smi) which is used to store
 # the scalar moment value.
 # Use $SMI_BASE to indicate smi_base defined above
 # Use $ORIGIN_ID to indicate the id of the associated Origin.
 smi_focal_mechanism_template = string(default="$SMI_BASE/FocalMechanism/Origin/$ORIGIN_ID#sourcespec")
-# -----------------QUAKEML PARAMETERS
+# -----------------QUAKEML OUTPUT PARAMETERS
```

### Comparing `sourcespec-1.7/sourcespec/html_report_template/index.html` & `sourcespec-1.8/sourcespec/html_report_template/index.html`

 * *Files 3% similar despite different names*

```diff
@@ -48,15 +48,29 @@
           </li>{MAP_MAG_COMMENT_END}{MAP_FC_COMMENT_BEGIN}
           <li>
             <a href="#corner_frequency">
               <i class="fas fa-image"></i>
               &nbsp;&nbsp;
               Corner Frequency
             </a>
-          </li>{MAP_FC_COMMENT_END}{TRACES_PLOTS_COMMENT_BEGIN}
+          </li>{MAP_FC_COMMENT_END}{STACKED_SPECTRA_COMMENT_BEGIN}
+          <li>
+            <a href="#stacked_spectra">
+              <i class="fas fa-image"></i>
+              &nbsp;&nbsp;
+              Stacked Spectra
+            </a>
+          </li>{STACKED_SPECTRA_COMMENT_END}
+          <li>
+            <a href="#inversion_info">
+              <i class="fas fa-info-circle"></i>
+              &nbsp;&nbsp;
+              Inversion Information
+            </a>
+          </li>{TRACES_PLOTS_COMMENT_BEGIN}
           <li>
             <a href="#traces">
               <i class="fas fa-image"></i>
               &nbsp;&nbsp;
               Traces
             </a>
           </li>{TRACES_PLOTS_COMMENT_END}{SPECTRA_PLOTS_COMMENT_BEGIN}
@@ -64,41 +78,27 @@
             <a href="#spectra">
               <i class="fas fa-image"></i>
               &nbsp;&nbsp;
               Spectra
             </a>
           </li>{SPECTRA_PLOTS_COMMENT_END}
           <li>
-            <a href="#inversion_info">
-              <i class="fas fa-table"></i>
-              &nbsp;&nbsp;
-              Inversion Information
-            </a>
-          </li>
-          <li>
             <a href="#summary_spectral_parameters">
               <i class="fas fa-table"></i>
               &nbsp;&nbsp;
               Summary Spectral Parameters
             </a>
           </li>{BOX_PLOTS_COMMENT_BEGIN}
           <li>
             <a href="#box_plots">
               <i class="fas fa-image"></i>
               &nbsp;&nbsp;
               Spectral Parameter<br>Box Plots
             </a>
-          </li>{BOX_PLOTS_COMMENT_END}{STACKED_SPECTRA_COMMENT_BEGIN}
-          <li>
-            <a href="#stacked_spectra">
-              <i class="fas fa-image"></i>
-              &nbsp;&nbsp;
-              Stacked Spectra
-            </a>
-          </li>{STACKED_SPECTRA_COMMENT_END}
+          </li>{BOX_PLOTS_COMMENT_END}
           <li>
             <a href="#station_parameters">
               <i class="fas fa-table"></i>
               &nbsp;&nbsp;
               Station Parameters
             </a>
           </li>{MISFIT_PLOT_COMMENT_BEGIN}
@@ -117,16 +117,15 @@
             </a>
           </li>
         </ul>
         <div class="sidebar-footer">
           SourceSpec {VERSION}<br/>
           Run completed on<br/>
           {RUN_COMPLETED}
-          {AUTHOR}
-          {AGENCY}
+          {AUTHOR_AND_AGENCY}
         </div>
       </nav>
 
       <!-- Page Content  -->
       <div id="content">
         <div id="sidebarCollapse">
             <button type="button" class="btn btn-info">
@@ -144,43 +143,61 @@
               <th scope="row">Event ID:</th>
               <td>{EVENT_URL_COMMENT_BEGIN}
                 <a href="{EVENT_URL}" title="Go to event page" target="_new">{EVENT_URL_COMMENT_END}
                   {EVENTID}{EVENT_URL_COMMENT_BEGIN}
                   &nbsp;<i class="fas fa-external-link-alt"></i>
                 </a>{EVENT_URL_COMMENT_END}
               </td>
-            </tr>{RUNID_COMMENT_BEGIN}
+            </tr>{EVENT_NAME_COMMENT_BEGIN}
+            <tr>
+              <th scope="row">Event Name:</th>
+              <td>{EVENT_NAME}</td>
+            </tr>{EVENT_NAME_COMMENT_END}{RUNID_COMMENT_BEGIN}
             <tr>
               <th scope="row">Run ID:</th>
               <td>{RUNID}</td>
             </tr>{RUNID_COMMENT_END}
             <tr>
+              <th scope="row">Origin Time:</th>
+              <td>{ORIGIN_TIME} UTC</td>
+            </tr>
+            <tr>
               <th scope="row">Longitude:</th>
               <td>{EVENT_LONGITUDE} °E</td>
             </tr>
             <tr>
               <th scope="row">Latitude:</th>
               <td>{EVENT_LATITUDE} °N</td>
             </tr>
             <tr>
               <th scope="row">Depth:</th>
               <td>{EVENT_DEPTH} km</td>
             </tr>
             <tr>
-              <th scope="row">Origin Time:</th>
-              <td>{ORIGIN_TIME}</td>
-            </tr>
-            <tr>
               <th scope="row">Moment Magnitude:</th>
-              <td>{MW_SUMMARY}</td>
+              <td>Mw {MW_SUMMARY}</td>
             </tr>
             <tr>
               <th scope="row">Corner Frequency:</th>
               <td>{FC_SUMMARY} Hz</td>
             </tr>
+            <tr>
+              <th scope="row">Run information:</th>
+              <td>
+                Run completed on {RUN_COMPLETED}
+                {AUTHOR_COMMENT_BEGIN}
+                <br>
+                {AUTHOR}
+                {AUTHOR_COMMENT_END}
+                {AGENCY_COMMENT_BEGIN}
+                <br>
+                {AGENCY}
+                {AGENCY_COMMENT_END}
+              </td>
+            </tr>
           </tbody>
         </table>
       </div> <!-- page -->
 
 {MAP_MAG_COMMENT_BEGIN}
       <div class="page">
         <div class="line" id="moment_magnitude"></div>
@@ -197,30 +214,45 @@
         <h2>Corner Frequency</h2>
         <div class="item" data-src="{MAP_FC}">
           <img class="station_map" src="{MAP_FC}"/>
         </div>
       </div>
 {MAP_FC_COMMENT_END}
 
-{TRACES_PLOTS_COMMENT_BEGIN}
-      <div class="line" id="traces"></div>
-{TRACES_PLOTS}
-{TRACES_PLOTS_COMMENT_END}
-
-{SPECTRA_PLOTS_COMMENT_BEGIN}
-      <div class="line" id="spectra"></div>
-{SPECTRA_PLOTS}
-{SPECTRA_PLOTS_COMMENT_END}
+{STACKED_SPECTRA_COMMENT_BEGIN}
+      <div class="page">
+        <div class="line" id="stacked_spectra"></div>
+        <h2>Stacked Spectra</h2>
+        <div class="item" data-src="{STACKED_SPECTRA}">
+          <img class="stacked_spectra" src="{STACKED_SPECTRA}"/>
+        </div>
+      </div>
+{STACKED_SPECTRA_COMMENT_END}
 
       <div class="page">
         <div class="line" id="inversion_info"></div>
         <h2>Inversion Information</h2>
         <table class="table">
           <tbody>
             <tr>
+              <th scope="row">SourceSpec version:</th>
+              <td>
+                {VERSION}&nbsp;
+                <a href="{SSP_URL}" title="SourceSpec homepage" target="_new">
+                  <i class="fas fa-external-link-alt"></i>
+                </a>
+              </td>
+            </tr>
+            <tr>
+              <th scope="row">Wave type:</th>
+              <td>
+                {INVERSION_WAVE_TYPE}
+              </td>
+            </tr>
+            <tr>
               <th scope="row">Algorithm:</th>
               <td>
                 {INVERSION_ALGORITHM}
               </td>
             </tr>
             <tr>
               <th scope="row">Weighting:</th>
@@ -264,116 +296,124 @@
                 {INVERSION_Q0_MIN_MAX}
               </td>
             </tr>
           </tbody>
         </table>
       </div> <!-- page -->
 
+{TRACES_PLOTS_COMMENT_BEGIN}
+      <div class="line" id="traces"></div>
+{TRACES_PLOTS}
+{TRACES_PLOTS_COMMENT_END}
+
+{SPECTRA_PLOTS_COMMENT_BEGIN}
+      <div class="line" id="spectra"></div>
+{SPECTRA_PLOTS}
+{SPECTRA_PLOTS_COMMENT_END}
+
       <div class="page">
         <div class="line" id="summary_spectral_parameters"></div>
         <h2>Summary Spectral Parameters</h2>
         <h6>
           Note: the highlighted column indicates the reference parameters used
           for <a href="#event_summary">Event Summary</a> and
           <a href="#moment_magnitude">Map Plots</a>.
         </h6>
-        <table class="table summary">
-          <colgroup>
-            <col>
-            <col {COL_MEAN_HIGHLIGHTED}>
-            <col {COL_WMEAN_HIGHLIGHTED}>
-            <col {COL_PERC_HIGHLIGHTED}>
-          </colgroup>
-          <thead>
-            <tr>
-              <th></th>
-              <th scope="col">Mean<div class="th_subtitle">({N_SIGMA})</div></th>
-              <th scope="col">Weighted Mean<div class="th_subtitle">({N_SIGMA})</div></th>
-              <th scope="col">Percentiles<div class="th_subtitle">({PERCENTAGES})</div></th>
-            </tr>
-          </thead>
-          <tbody>
-            <tr>
-              <th scope="row">Mw</th>
-              <td>{MW_MEAN_AND_ERR}</td>
-              <td>{MW_WMEAN_AND_ERR}</td>
-              <td>{MW_PERC_AND_ERR}</td>
-            </tr>
-            <tr>
-              <th scope="row">Seismic Moment (N&#183;m)</th>
-              <td>{M0_MEAN_AND_ERR}</td>
-              <td>{M0_WMEAN_AND_ERR}</td>
-              <td>{M0_PERC_AND_ERR}</td>
-            </tr>
-            <tr>
-              <th scope="row">Corner Frequency (Hz)</th>
-              <td>{FC_MEAN_AND_ERR}</td>
-              <td>{FC_WMEAN_AND_ERR}</td>
-              <td>{FC_PERC_AND_ERR}</td>
-            </tr>
-            <tr>
-              <th scope="row">t-star (s)</th>
-              <td>{TSTAR_MEAN_AND_ERR}</td>
-              <td>{TSTAR_WMEAN_AND_ERR}</td>
-              <td>{TSTAR_PERC_AND_ERR}</td>
-            </tr>
-            <tr>
-              <th scope="row">Qo</th>
-              <td>{Q0_MEAN_AND_ERR}</td>
-              <td>{Q0_WMEAN_AND_ERR}</td>
-              <td>{Q0_PERC_AND_ERR}</td>
-            </tr>
-            <tr>
-              <th scope="row">Source Radius (m)</th>
-              <td>{RADIUS_MEAN_AND_ERR}</td>
-              <td>{RADIUS_WMEAN_AND_ERR}</td>
-              <td>{RADIUS_PERC_AND_ERR}</td>
-            </tr>
-            <tr>
-              <th scope="row">Brune Stress Drop (MPa)</th>
-              <td>{BSD_MEAN_AND_ERR}</td>
-              <td>{BSD_WMEAN_AND_ERR}</td>
-              <td>{BSD_PERC_AND_ERR}</td>
-            </tr>
-            <tr>
-              <th scope="row">Radiated Energy (N&#183;m)</th>
-              <td>{ER_MEAN_AND_ERR}</td>
-              <td></td>
-              <td>{ER_PERC_AND_ERR}</td>
-            </tr>{ML_COMMENT_BEGIN}
-            <tr>
-              <th scope="row">Ml</th>
-              <td>{ML_MEAN_AND_ERR}</td>
-              <td></td>
-              <td>{ML_PERC_AND_ERR}</td>
-            </tr>{ML_COMMENT_END}
-          </tbody>
-        </table>
+        <div class="table_summary_wrapper">
+          <table class="table summary">
+            <colgroup>
+              <col>
+              <col {COL_MEAN_HIGHLIGHTED}>
+              <col {COL_WMEAN_HIGHLIGHTED}>
+              <col {COL_PERC_HIGHLIGHTED}>
+            </colgroup>
+            <thead>
+              <tr>
+                <th class="parameter"></th>
+                <th scope="col">Mean<div class="th_subtitle">({N_SIGMA})</div></th>
+                <th scope="col">Weighted Mean<div class="th_subtitle">({N_SIGMA})</div></th>
+                <th scope="col">Percentiles<div class="th_subtitle">({PERCENTAGES})</div></th>
+              </tr>
+            </thead>
+            <tbody>
+              <tr>
+                <th class="parameter" scope="row">Mw</th>
+                <td>{MW_MEAN_AND_ERR}</td>
+                <td>{MW_WMEAN_AND_ERR}</td>
+                <td>{MW_PERC_AND_ERR}</td>
+              </tr>
+              <tr>
+                <th class="parameter" scope="row">Seismic Moment (N&#183;m)</th>
+                <td>{M0_MEAN_AND_ERR}</td>
+                <td>{M0_WMEAN_AND_ERR}</td>
+                <td>{M0_PERC_AND_ERR}</td>
+              </tr>
+              <tr>
+                <th class="parameter" scope="row">Corner Frequency (Hz)</th>
+                <td>{FC_MEAN_AND_ERR}</td>
+                <td>{FC_WMEAN_AND_ERR}</td>
+                <td>{FC_PERC_AND_ERR}</td>
+              </tr>
+              <tr>
+                <th class="parameter" scope="row">t-star (s)</th>
+                <td>{TSTAR_MEAN_AND_ERR}</td>
+                <td>{TSTAR_WMEAN_AND_ERR}</td>
+                <td>{TSTAR_PERC_AND_ERR}</td>
+              </tr>
+              <tr>
+                <th class="parameter" scope="row">Qo</th>
+                <td>{Q0_MEAN_AND_ERR}</td>
+                <td>{Q0_WMEAN_AND_ERR}</td>
+                <td>{Q0_PERC_AND_ERR}</td>
+              </tr>
+              <tr>
+                <th class="parameter" scope="row">Source Radius (m)</th>
+                <td>{RADIUS_MEAN_AND_ERR}</td>
+                <td>{RADIUS_WMEAN_AND_ERR}</td>
+                <td>{RADIUS_PERC_AND_ERR}</td>
+              </tr>
+              <tr>
+                <th class="parameter" scope="row">Static Stress Drop (MPa)</th>
+                <td>{SSD_MEAN_AND_ERR}</td>
+                <td>{SSD_WMEAN_AND_ERR}</td>
+                <td>{SSD_PERC_AND_ERR}</td>
+              </tr>
+              <tr>
+                <th class="parameter" scope="row">Radiated Energy (N&#183;m)</th>
+                <td>{ER_MEAN_AND_ERR}</td>
+                <td>{ER_WMEAN_AND_ERR}</td>
+                <td>{ER_PERC_AND_ERR}</td>
+              </tr>
+              <tr>
+                <th class="parameter" scope="row">Apparent Stress (MPa)</th>
+                <td>{SIGMA_A_MEAN_AND_ERR}</td>
+                <td>{SIGMA_A_WMEAN_AND_ERR}</td>
+                <td>{SIGMA_A_PERC_AND_ERR}</td>
+              </tr>{ML_COMMENT_BEGIN}
+              <tr>
+                <th class="parameter" scope="row">Ml</th>
+                <td>{ML_MEAN_AND_ERR}</td>
+                <td>{ML_WMEAN_AND_ERR}</td>
+                <td>{ML_PERC_AND_ERR}</td>
+              </tr>{ML_COMMENT_END}
+            </tbody>
+          </table>
+        </div>
       </div> <!-- page -->
 
 {BOX_PLOTS_COMMENT_BEGIN}
       <div class="page">
         <div class="line" id="box_plots"></div>
         <h2>Spectral Parameter Box Plots</h2>
         <div class="item" data-src="{BOX_PLOTS}">
           <img class="box_plot" src="{BOX_PLOTS}"/>
         </div>
       </div>
 {BOX_PLOTS_COMMENT_END}
 
-{STACKED_SPECTRA_COMMENT_BEGIN}
-      <div class="page">
-        <div class="line" id="stacked_spectra"></div>
-        <h2>Stacked Spectra</h2>
-        <div class="item" data-src="{STACKED_SPECTRA}">
-          <img class="stacked_spectra" src="{STACKED_SPECTRA}"/>
-        </div>
-      </div>
-{STACKED_SPECTRA_COMMENT_END}
-
       <div class="page">
         <div class="line" id="station_parameters"></div>
         <h2>Station Parameters</h2>
         <h6>Note: outliers are greyed out</h6>
         <div class="table_wrapper">
           <table class="table stations" id="station_table">
             <thead>
@@ -398,33 +438,37 @@
                   <nobr><i class="fas fa-sort dontprint_inline"></i>&nbsp;Qo</nobr>
                 </th>
                 <th onclick="sortTable(6, numeric=true)" scope="col">
                   <nobr><i class="fas fa-sort dontprint_inline"></i>&nbsp;Seismic</nobr>
                     <br/>Moment<br/>(N&#183;m)
                 </th>
                 <th onclick="sortTable(7, numeric=true)" scope="col">
-                  <nobr><i class="fas fa-sort dontprint_inline"></i>&nbsp;Brune</nobr>
+                  <nobr><i class="fas fa-sort dontprint_inline"></i>&nbsp;Static</nobr>
                     <br/>stress<br/>drop<br/>(MPa)
                 </th>
                 <th onclick="sortTable(8, numeric=true)" scope="col">
                   <nobr><i class="fas fa-sort dontprint_inline"></i>&nbsp;Source</nobr>
                     <br/>radius<br/>(m)
                 </th>
                 <th onclick="sortTable(9, numeric=true)" scope="col">
                   <nobr><i class="fas fa-sort dontprint_inline"></i>&nbsp;Radiated</nobr>
                     <br/>Energy<br/>(N&#183;m)
                 </th>
                 <th onclick="sortTable(10, numeric=true)" scope="col">
+                  <nobr><i class="fas fa-sort dontprint_inline"></i>&nbsp;Apparent</nobr>
+                    <br/>Stress<br/>(MPa)
+                </th>
+                <th onclick="sortTable(11, numeric=true)" scope="col">
                   <nobr><i class="fas fa-sort dontprint_inline"></i>&nbsp;Hypocentral</nobr>
                     <br/>Distance<br/>(km)
                 </th>
-                <th onclick="sortTable(11, numeric=true)" scope="col">
+                <th onclick="sortTable(12, numeric=true)" scope="col">
                   <nobr><i class="fas fa-sort dontprint_inline"></i>&nbsp;Azimuth</nobr><br/>(°)
                 </th>{ML_COMMENT_BEGIN}
-                <th onclick="sortTable(12, numeric=true)" scope="col">
+                <th onclick="sortTable(13, numeric=true)" scope="col">
                   <nobr><i class="fas fa-sort"></i>&nbsp;Ml</nobr>
                 </th>{ML_COMMENT_END}
               </tr>
             </thead>
             <tbody>
   {STATION_TABLE_ROWS}
             </tbody>
@@ -443,14 +487,22 @@
 
       <div class="dontprint">
         <div class="line" id="files"></div>
         <h2>Files</h2>
         <table class="table">
           <tbody>
             <tr>
+              <th scope="row">Input Files:</th>
+              <td>
+                <a href="{INPUT_FILES}">
+                  {INPUT_FILES}
+                </a>
+              </td>
+            </tr>
+            <tr>
               <th scope="row">Configuration:</th>
               <td>
                 <a href="{CONF_FILE}" type="text/plain">
                   {CONF_FILE_BNAME}
                 </a>
               </td>
             </tr>
```

#### html2text {}

```diff
@@ -1,98 +1,116 @@
 {AGENCY_LOGO}_[_{_L_O_G_O___F_I_L_E_}_]
     * _ _ _ _E_v_e_n_t_ _S_u_m_m_a_r_y
     * {MAP_MAG_COMMENT_BEGIN}
     * _ _ _ _M_o_m_e_n_t_ _M_a_g_n_i_t_u_d_e
     * {MAP_MAG_COMMENT_END}{MAP_FC_COMMENT_BEGIN}
     * _ _ _ _C_o_r_n_e_r_ _F_r_e_q_u_e_n_c_y
-    * {MAP_FC_COMMENT_END}{TRACES_PLOTS_COMMENT_BEGIN}
+    * {MAP_FC_COMMENT_END}{STACKED_SPECTRA_COMMENT_BEGIN}
+    * _ _ _ _S_t_a_c_k_e_d_ _S_p_e_c_t_r_a
+    * {STACKED_SPECTRA_COMMENT_END}
+    * _ _ _ _I_n_v_e_r_s_i_o_n_ _I_n_f_o_r_m_a_t_i_o_n
+    * {TRACES_PLOTS_COMMENT_BEGIN}
     * _ _ _ _T_r_a_c_e_s
     * {TRACES_PLOTS_COMMENT_END}{SPECTRA_PLOTS_COMMENT_BEGIN}
     * _ _ _ _S_p_e_c_t_r_a
     * {SPECTRA_PLOTS_COMMENT_END}
-    * _ _ _ _I_n_v_e_r_s_i_o_n_ _I_n_f_o_r_m_a_t_i_o_n
     * _ _ _ _S_u_m_m_a_r_y_ _S_p_e_c_t_r_a_l_ _P_a_r_a_m_e_t_e_r_s
     * {BOX_PLOTS_COMMENT_BEGIN}
     * _ _ _ _S_p_e_c_t_r_a_l_ _P_a_r_a_m_e_t_e_r
       _B_o_x_ _P_l_o_t_s
-    * {BOX_PLOTS_COMMENT_END}{STACKED_SPECTRA_COMMENT_BEGIN}
-    * _ _ _ _S_t_a_c_k_e_d_ _S_p_e_c_t_r_a
-    * {STACKED_SPECTRA_COMMENT_END}
+    * {BOX_PLOTS_COMMENT_END}
     * _ _ _ _S_t_a_t_i_o_n_ _P_a_r_a_m_e_t_e_r_s
     * {MISFIT_PLOT_COMMENT_BEGIN}
     * _ _ _ _M_i_s_f_i_t_ _P_l_o_t_s
     * {MISFIT_PLOT_COMMENT_END}
     * _ _ _ _F_i_l_e_s
 SourceSpec {VERSION}
 Run completed on
-{RUN_COMPLETED} {AUTHOR} {AGENCY}
+{RUN_COMPLETED} {AUTHOR_AND_AGENCY}
 {PAGE_FOOTER}
 ********** EEvveenntt SSuummmmaarryy **********
                   {EVENT_URL_COMMENT_BEGIN}
 EEvveenntt IIDD::         _{_E_V_E_N_T___U_R_L___C_O_M_M_E_N_T___E_N_D_}_ _{_E_V_E_N_T_I_D_}_{_E_V_E_N_T___U_R_L___C_O_M_M_E_N_T___B_E_G_I_N_}_ _ 
                   {EVENT_URL_COMMENT_END}
+EEvveenntt NNaammee::       {EVENT_NAME}
 RRuunn IIDD::           {RUNID}
+OOrriiggiinn TTiimmee::      {ORIGIN_TIME} UTC
 LLoonnggiittuuddee::        {EVENT_LONGITUDE} °E
 LLaattiittuuddee::         {EVENT_LATITUDE} °N
 DDeepptthh::            {EVENT_DEPTH} km
-OOrriiggiinn TTiimmee::      {ORIGIN_TIME}
-MMoommeenntt MMaaggnniittuuddee:: {MW_SUMMARY}
+MMoommeenntt MMaaggnniittuuddee:: Mw {MW_SUMMARY}
 CCoorrnneerr FFrreeqquueennccyy:: {FC_SUMMARY} Hz
+                  Run completed on {RUN_COMPLETED} {AUTHOR_COMMENT_BEGIN}
+RRuunn iinnffoorrmmaattiioonn::  {AUTHOR} {AUTHOR_COMMENT_END} {AGENCY_COMMENT_BEGIN}
+                  {AGENCY} {AGENCY_COMMENT_END}
 {MAP_MAG_COMMENT_BEGIN}
 ********** MMoommeenntt MMaaggnniittuuddee **********
 [{MAP_MAG}]
 {MAP_MAG_COMMENT_END} {MAP_FC_COMMENT_BEGIN}
 ********** CCoorrnneerr FFrreeqquueennccyy **********
 [{MAP_FC}]
-{MAP_FC_COMMENT_END} {TRACES_PLOTS_COMMENT_BEGIN}
-{TRACES_PLOTS} {TRACES_PLOTS_COMMENT_END} {SPECTRA_PLOTS_COMMENT_BEGIN}
-{SPECTRA_PLOTS} {SPECTRA_PLOTS_COMMENT_END}
+{MAP_FC_COMMENT_END} {STACKED_SPECTRA_COMMENT_BEGIN}
+********** SSttaacckkeedd SSppeeccttrraa **********
+[{STACKED_SPECTRA}]
+{STACKED_SPECTRA_COMMENT_END}
 ********** IInnvveerrssiioonn IInnffoorrmmaattiioonn **********
+SSoouurrcceeSSppeecc vveerrssiioonn::   {VERSION} 
+WWaavvee ttyyppee::            {INVERSION_WAVE_TYPE}
 AAllggoorriitthhmm::            {INVERSION_ALGORITHM}
 WWeeiigghhttiinngg::            {INVERSION_WEIGHTING}
 tt--ssttaarr--00::             {INVERSION_T_STAR_0}
 IInnvveerrtt tt--ssttaarr--00::      {INVERSION_INVERT_T_STAR_0}
 tt--ssttaarr--00 vvaarriiaabbiilliittyy:: {INVERSION_T_STAR_0_VARIABILITY}
 tt--ssttaarr mmiinn,, mmaaxx::      {INVERSION_T_STAR_MIN_MAX}
 ffcc mmiinn,, mmaaxx::          {INVERSION_FC_MIN_MAX}
 QQoo mmiinn,, mmaaxx::          {INVERSION_Q0_MIN_MAX}
+{TRACES_PLOTS_COMMENT_BEGIN}
+{TRACES_PLOTS} {TRACES_PLOTS_COMMENT_END} {SPECTRA_PLOTS_COMMENT_BEGIN}
+{SPECTRA_PLOTS} {SPECTRA_PLOTS_COMMENT_END}
 ********** SSuummmmaarryy SSppeeccttrraall PPaarraammeetteerrss **********
 ** NNoottee:: tthhee hhiigghhlliigghhtteedd ccoolluummnn iinnddiiccaatteess tthhee rreeffeerreennccee ppaarraammeetteerrss uusseedd ffoorr
 _EE_vv_ee_nn_tt_ _SS_uu_mm_mm_aa_rr_yy aanndd _MM_aa_pp_ _PP_ll_oo_tt_ss.. **
-             MMeeaann                  WWeeiigghhtteedd MMeeaann          PPeerrcceennttiilleess
-             (({{NN__SSIIGGMMAA}}))           (({{NN__SSIIGGMMAA}}))            (({{PPEERRCCEENNTTAAGGEESS}}))
-MMww           {MW_MEAN_AND_ERR}     {MW_WMEAN_AND_ERR}     {MW_PERC_AND_ERR}
-SSeeiissmmiicc      {M0_MEAN_AND_ERR}     {M0_WMEAN_AND_ERR}     {M0_PERC_AND_ERR}
-MMoommeenntt ((NN?·mm))
+          MMeeaann                   WWeeiigghhtteedd MMeeaann           PPeerrcceennttiilleess
+          (({{NN__SSIIGGMMAA}}))            (({{NN__SSIIGGMMAA}}))             (({{PPEERRCCEENNTTAAGGEESS}}))
+MMww        {MW_MEAN_AND_ERR}      {MW_WMEAN_AND_ERR}      {MW_PERC_AND_ERR}
+SSeeiissmmiicc
+MMoommeenntt    {M0_MEAN_AND_ERR}      {M0_WMEAN_AND_ERR}      {M0_PERC_AND_ERR}
+((NN?·mm))
 CCoorrnneerr
-FFrreeqquueennccyy    {FC_MEAN_AND_ERR}     {FC_WMEAN_AND_ERR}     {FC_PERC_AND_ERR}
+FFrreeqquueennccyy {FC_MEAN_AND_ERR}      {FC_WMEAN_AND_ERR}      {FC_PERC_AND_ERR}
 ((HHzz))
-tt--ssttaarr ((ss))   {TSTAR_MEAN_AND_ERR}  {TSTAR_WMEAN_AND_ERR}  {TSTAR_PERC_AND_ERR}
-QQoo           {Q0_MEAN_AND_ERR}     {Q0_WMEAN_AND_ERR}     {Q0_PERC_AND_ERR}
-SSoouurrccee       {RADIUS_MEAN_AND_ERR} {RADIUS_WMEAN_AND_ERR} {RADIUS_PERC_AND_ERR}
-RRaaddiiuuss ((mm))
-BBrruunnee SSttrreessss {BSD_MEAN_AND_ERR}    {BSD_WMEAN_AND_ERR}    {BSD_PERC_AND_ERR}
-DDrroopp ((MMPPaa))
-RRaaddiiaatteedd     {ER_MEAN_AND_ERR}                            {ER_PERC_AND_ERR}
-EEnneerrggyy ((NN?·mm))
-MMll           {ML_MEAN_AND_ERR}                            {ML_PERC_AND_ERR}
+tt--ssttaarr    {TSTAR_MEAN_AND_ERR}   {TSTAR_WMEAN_AND_ERR}   {TSTAR_PERC_AND_ERR}
+((ss))
+QQoo        {Q0_MEAN_AND_ERR}      {Q0_WMEAN_AND_ERR}      {Q0_PERC_AND_ERR}
+SSoouurrccee
+RRaaddiiuuss    {RADIUS_MEAN_AND_ERR}  {RADIUS_WMEAN_AND_ERR}  {RADIUS_PERC_AND_ERR}
+((mm))
+SSttaattiicc
+SSttrreessss    {SSD_MEAN_AND_ERR}     {SSD_WMEAN_AND_ERR}     {SSD_PERC_AND_ERR}
+DDrroopp
+((MMPPaa))
+RRaaddiiaatteedd
+EEnneerrggyy    {ER_MEAN_AND_ERR}      {ER_WMEAN_AND_ERR}      {ER_PERC_AND_ERR}
+((NN?·mm))
+AAppppaarreenntt
+SSttrreessss    {SIGMA_A_MEAN_AND_ERR} {SIGMA_A_WMEAN_AND_ERR} {SIGMA_A_PERC_AND_ERR}
+((MMPPaa))
+MMll        {ML_MEAN_AND_ERR}      {ML_WMEAN_AND_ERR}      {ML_PERC_AND_ERR}
 {BOX_PLOTS_COMMENT_BEGIN}
 ********** SSppeeccttrraall PPaarraammeetteerr BBooxx PPlloottss **********
 [{BOX_PLOTS}]
-{BOX_PLOTS_COMMENT_END} {STACKED_SPECTRA_COMMENT_BEGIN}
-********** SSttaacckkeedd SSppeeccttrraa **********
-[{STACKED_SPECTRA}]
-{STACKED_SPECTRA_COMMENT_END}
+{BOX_PLOTS_COMMENT_END}
 ********** SSttaattiioonn PPaarraammeetteerrss **********
 ** NNoottee:: oouuttlliieerrss aarree ggrreeyyeedd oouutt **
 
-   FFrreeqquueennccyy      MMoommeenntt ssttrreessss rraaddiiuuss EEnneerrggyy DDiissttaannccee
-   ((HHzz))      ((ss))  ((NN?·mm))  ddrroopp   ((mm))    ((NN?·mm))  ((kkmm))     ((?°))
+   FFrreeqquueennccyy      MMoommeenntt ssttrreessss rraaddiiuuss EEnneerrggyy SSttrreessss DDiissttaannccee
+   ((HHzz))      ((ss))  ((NN?·mm))  ddrroopp   ((mm))    ((NN?·mm))  ((MMPPaa))  ((kkmm))     ((?°))
                          ((MMPPaa))
 {MISFIT_PLOT_COMMENT_BEGIN}
 ********** MMiissffiitt pplloottss **********
    _C_l_i_c_k_ _h_e_r_e_ _t_o_ _g_o_ _t_o_ _m_i_s_f_i_t_ _p_l_o_t_ _p_a_g_e
 {MISFIT_PLOT_COMMENT_END}
 ********** FFiilleess **********
+IInnppuutt FFiilleess::   _{_I_N_P_U_T___F_I_L_E_S_}
 CCoonnffiigguurraattiioonn:: _{_C_O_N_F___F_I_L_E___B_N_A_M_E_}
 OOuuttppuutt::        _{_Y_A_M_L___F_I_L_E___B_N_A_M_E_}
 LLoogg::           _{_L_O_G___F_I_L_E___B_N_A_M_E_}
```

### Comparing `sourcespec-1.7/sourcespec/html_report_template/misfit.html` & `sourcespec-1.8/sourcespec/html_report_template/misfit.html`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
   <body>
     <div class="wrapper">
       <span id="one_d_conditional"></span>
       <!-- Sidebar  -->
       <nav id="sidebar">
         <div class="sidebar-header">
-          <a href="https://github.com/SeismicSource/sourcespec" target="_blank">
+          <a href="{SSP_URL}" target="_blank">
             <img class="logo" src="{LOGO_FILE}"/>
           </a>
         </div>
         <ul class="list-unstyled components">
           <li>
             <a href="#one_d_conditional">
               <i class="fas fa-image"></i>
@@ -66,16 +66,15 @@
             </a>
           </li>
         </ul>
         <div class="sidebar-footer">
           SourceSpec {VERSION}<br/>
           Run completed on<br/>
           {RUN_COMPLETED}
-          {AUTHOR}
-          {AGENCY}
+          {AUTHOR_AND_AGENCY}
         </div>
       </nav>
 
       <!-- Page Content  -->
       <div id="content">
         <div id="sidebarCollapse">
             <button type="button" class="btn btn-info">
```

#### html2text {}

```diff
@@ -2,12 +2,12 @@
     * _ _ _ _1_D_ _c_o_n_d_i_t_i_o_n_a_l_ _m_i_s_f_i_t
     * _ _ _ _2_D_ _c_o_n_d_i_t_i_o_n_a_l_ _m_i_s_f_i_t_:_ _f_c_-_M_w
     * _ _ _ _2_D_ _c_o_n_d_i_t_i_o_n_a_l_ _m_i_s_f_i_t_:_ _f_c_-_t_*
     * _ _ _ _2_D_ _c_o_n_d_i_t_i_o_n_a_l_ _m_i_s_f_i_t_:_ _t_*_-_M_w
     * _ _ _ _B_a_c_k_ _t_o_ _m_a_i_n_ _e_v_e_n_t_ _p_a_g_e
 SourceSpec {VERSION}
 Run completed on
-{RUN_COMPLETED} {AUTHOR} {AGENCY}
+{RUN_COMPLETED} {AUTHOR_AND_AGENCY}
 ********** 11DD ccoonnddiittiioonnaall mmiissffiitt **********
 ********** 22DD ccoonnddiittiioonnaall mmiissffiitt:: ffcc--MMww **********
 ********** 22DD ccoonnddiittiioonnaall mmiissffiitt:: ffcc--tt** **********
 ********** 22DD ccoonnddiittiioonnaall mmiissffiitt:: tt**--MMww **********
```

### Comparing `sourcespec-1.7/sourcespec/html_report_template/station_table_row.html` & `sourcespec-1.8/sourcespec/html_report_template/station_table_row.html`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,15 @@
               <td class="station_id">{STATION_ID}</td>
               <td>{STATION_TYPE}</td>
               <td>{STATION_MW}<br/>{STATION_MW_ERR}</td>
               <td>{STATION_FC}<br/>{STATION_FC_ERR}</td>
               <td>{STATION_TSTAR}<br/>{STATION_TSTAR_ERR}</td>
               <td>{STATION_Q0}<br/>{STATION_Q0_ERR}</td>
               <td>{STATION_M0}<br/>{STATION_M0_ERR}</td>
-              <td>{STATION_BSD}<br/>{STATION_BSD_ERR}</td>
+              <td>{STATION_SSD}<br/>{STATION_SSD_ERR}</td>
               <td>{STATION_RA}<br/>{STATION_RA_ERR}</td>
               <td>{STATION_ER}</td>
+              <td>{STATION_SIGMA_A}<br/>{STATION_SIGMA_A_ERR}</td>
               <td>{STATION_DIST}</td>
               <td>{STATION_AZ}</td>{ML_COMMENT_BEGIN}
               <td>{STATION_ML}</td>{ML_COMMENT_END}
             </tr>
```

### Comparing `sourcespec-1.7/sourcespec/html_report_template/style.css` & `sourcespec-1.8/sourcespec/html_report_template/style.css`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 @import "https://fonts.googleapis.com/css?family=Poppins:300,400,500,600,700";
 
-html, body{ height:100% };
-
 body {
   font-family: 'Poppins', sans-serif;
   background: #fff;
 }
 
 p {
   font-family: 'Poppins', sans-serif;
@@ -43,22 +41,42 @@
   text-align: right;
 }
 
 table.summary th[scope=col] {
   text-align: right;
 }
 
+table.summary th.parameter {
+  background-color: white;
+  border-right: 2px dotted #dee2e6;
+  position: -webkit-sticky;
+  position: sticky;
+  left: 0;
+  z-index: 3;
+}
+
 .highlighted_column {
   border: 2px dotted #666;
+  background-color: #dadada;
 }
 
 .th_subtitle {
   font-size: 0.8em;
 }
 
+.table_summary_wrapper {
+  white-space: nowrap;
+  overflow: hidden;
+  /* scrollbar style for Firefox */
+  scrollbar-width: auto;
+}
+.table_summary_wrapper:hover {
+  overflow: scroll;
+}
+
 table.stations {
   font-size: 0.8em;
   text-align: right;
   border-collapse: separate;
   border-spacing: 0;
 }
 
@@ -211,15 +229,15 @@
   font-size: 1.3em;
   font-weight: bold;
 }
 
 #sidebar .sidebar-footer {
   margin-top: -20px;
   padding-left: 20px;
-  font-size: 1.6vh;
+  font-size: 0.8em;
   color: #94AFAB;
 }
 
 #sidebar .sidebar-footer a:hover {
   color: #e14d5b;
 }
 
@@ -372,14 +390,23 @@
     left: 246px;
   }
   #sidebarCollapse.active .btn.btn-info {
     font-size: 27.4px;
     background: #17054f;
     color: white;
   }
+  .station_map {
+    max-width: 100%;
+  }
+  .box_plot {
+    max-width: 100%;
+  }
+  .stacked_spectra {
+    max-width: 100%;
+  }
 }
 
 
 /* ---------------------------------------------------
     PRINTING
 ----------------------------------------------------- */
 
@@ -442,18 +469,18 @@
   .table_wrapper{
     height: auto;
     overflow: visible;
     white-space: normal;
     font-size: 0.8em;
   }
   .station_map {
-    max-width: 70%;
+    max-width: 65%;
   }
   .box_plot {
-    max-width: 60%;
+    max-width: 50%;
   }
   .stacked_spectra {
     max-width: 60%;
   }
   .text_footer {
     font-size: 0.8em;
     position: fixed;
```

### Comparing `sourcespec-1.7/sourcespec/kdtree.py` & `sourcespec-1.8/sourcespec/kdtree.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 # -*- coding: utf-8 -*-
 # SPDX-License-Identifier: CECILL-2.1
 """
 Grid importance sampling using a k-d tree.
 
 :copyright:
-    2022-2023 Claudio Satriano <satriano@ipgp.fr>
+    2022-2024 Claudio Satriano <satriano@ipgp.fr>
 :license:
     CeCILL Free Software License Agreement v2.1
     (http://www.cecill.info/licences.en.html)
 """
 import itertools
 import numpy as np
 from scipy.interpolate import griddata
 
 
 class KDTCell():
+    """A cell of a k-d tree."""
     def __init__(self, extent, calc_pdf, min_cell_prob=0,
                  ndiv=None, maxdiv=None):
         self.extent = extent
         self.coords = np.mean(extent, axis=1)
         self.delta = np.diff(extent)
         self.calc_pdf = calc_pdf
         self.pdf = calc_pdf(self.coords)
@@ -33,14 +34,15 @@
             self.prob_divisible = self.prob
         self.ndiv = ndiv
         if self.ndiv is None:
             self.ndiv = np.zeros(self.extent.shape[0])
         self.maxdiv = maxdiv
 
     def divide(self, parts):
+        """Divide the cell in `parts` parts along every dimension."""
         if not self.is_divisible:
             return [self, ]
         # dim is the dimension of the parameter space
         dim = self.extent.shape[0]
         # define a set of increments for all the spatial directions
         # the number of increments is "parts"
         # The code "np.mgrid...[1]" produces a 2D array of the type:
@@ -50,72 +52,79 @@
         # increments = np.mgrid[0:dim, 0:parts][1] * self.delta/(parts-1)
         increments = np.mgrid[0:dim, 0:parts][1]
         if self.maxdiv is not None:
             # dimensions that will not be divided
             increments[self.ndiv >= self.maxdiv] *= 0
             # dimensions that will be divided
             self.ndiv[self.ndiv < self.maxdiv] += parts
-        increments = increments * self.delta/(parts-1)
+        increments = increments * self.delta / (parts - 1)
         # take the minimum coordinate and transform it to a column vector
         mincoord = self.extent[:, 0].reshape(-1, 1)
         # add minimum coordinates to the increments
         coords = mincoord + increments
         cells = []
         # loop over all the possible n-uplets of coordinates
         # we use set() to avoid repetitions for dimensions that
         # will not be dvided
         for c in set(itertools.product(*coords)):
             # c is a coordinate n-uplet. Let's transform it to column vector
             c = np.array(c).reshape(-1, 1)
-            delta = self.delta/parts
+            delta = self.delta / parts
             # FIXME: I forgot my own code!
             #  should this `2` be `parts`? or is it related to delta/2?
-            inc = np.mgrid[0:dim, 0:2][1] * delta - delta/2
+            inc = np.mgrid[0:dim, 0:2][1] * delta - delta / 2
             extent = c + inc
             cells.append(
                 KDTCell(
                     extent, self.calc_pdf, self.min_cell_prob,
                     self.ndiv, self.maxdiv))
         return cells
 
 
 class KDTree():
+    """A k-d tree."""
     def __init__(self, extent, init_parts, calc_pdf, min_cell_prob=0.,
                  maxdiv=None):
         # extent defines the size of search hypervolume
         # reshape extent to (dim, 2), where dim is the
         # arbitrary dimension of the parameter space
         self.extent = np.array(extent).reshape(-1, 2)
         # create the first cell, with the same size
         # of the search hypervolume
         cell0 = KDTCell(self.extent, calc_pdf, maxdiv=maxdiv)
         self.init_prob = cell0.prob
-        cell0.min_cell_prob = cell0.prob*min_cell_prob
+        cell0.min_cell_prob = cell0.prob * min_cell_prob
         self.cells = cell0.divide(init_parts)
         self.ncells = len(self.cells)
 
     def divide(self):
-        # find the cell with highest probability and
-        # divide it in 2 parts along every dimension
+        """
+        Find the cell with highest probability and
+        divide it in 2 parts along every dimension
+        """
         # self.cells.sort(key=lambda c: c.prob)
         self.cells.sort(key=lambda c: c.prob_divisible)
         cell0 = self.cells.pop()
         # print(self.init_prob, cell0.prob, cell0.prob/self.init_prob)
         self.cells += cell0.divide(2)
         self.ncells = len(self.cells)
 
     def get_pdf(self, deltas):
+        """
+        Calculate the probability density function (PDF) on a grid
+        defined by deltas.
+        """
         deltas = np.array(deltas).reshape(-1, 1)
         extent = self.extent.copy()
         ranges = []
         extent_new = []
         for v in np.hstack((extent, deltas)):
             start, stop, step = v
             # add a small number to make sure end value is included
-            stop += stop/1e5
+            stop += stop / 1e5
             rng = np.arange(start, stop, step)
             ranges.append(rng)
             extent_new += [rng[0], rng[-1]]
         xi = np.meshgrid(*ranges, indexing='ij')
         coords = np.array([cell.coords for cell in self.cells])
         pdf_values = np.array([cell.pdf for cell in self.cells])
         pdf = griddata(coords, pdf_values, tuple(xi), method='linear')
```

### Comparing `sourcespec-1.7/sourcespec/plot_sourcepars.py` & `sourcespec-1.8/sourcespec/plot_sourcepars.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,34 +2,37 @@
 # SPDX-License-Identifier: CECILL-2.1
 """
 plot_sourcepars.py
 
 1D or 2D plot of source parameters from a sqlite parameter file.
 
 :copyright:
-    2023 Claudio Satriano <satriano@ipgp.fr>
+    2023-2024 Claudio Satriano <satriano@ipgp.fr>
 :license:
     CeCILL Free Software License Agreement v2.1
     (http://www.cecill.info/licences.en.html)
 """
 import argparse
 import contextlib
 import sys
 import os
+import sqlite3
 import numpy as np
 import matplotlib.pyplot as plt
 from scipy.optimize import curve_fit
-import sqlite3
 
 valid_plot_types = [
-    'fc', 'Er', 'bsd', 'ra', 'Mo', 't_star', 'Qo',
-    'fc_mw', 'Er_mw', 'bsd_mw']
+    'fc', 'Er', 'ssd', 'ra', 'Mo', 't_star', 'Qo', 'sigma_a',
+    'fc_mw', 'Er_mw', 'ssd_mw']
 
 
 class Annot():
+    """
+    Annotate the plot with the evid, Mw and the value of the parameter.
+    """
     def __init__(self, xdata, ydata, labels, yformat):
         self.xdata = xdata
         self.ydata = ydata
         self.labels = labels
         self.yformat = yformat
 
     def __call__(self, event):
@@ -38,62 +41,114 @@
         y = np.take(self.ydata, ind)
         label = np.take(self.labels, ind)
         for Mw, yvalue, evid in zip(x, y, label):
             ystring = self.yformat.format(yvalue)
             print(f'{evid} Mw {Mw:.1f} {ystring}')
 
 
-def mag_to_moment(mag):
+def mag_to_moment(mag, b=0.5):
+    """
+    Convert magnitude to moment.
+
+    The parameter b is used to change the slope of the fc-Mw stress drop curve.
+
+    The standard value of b is 0.5, which corresponds to a self-similar model.
+    """
     mag = np.asarray(mag)
-    return np.power(10, (1.5 * mag + 9.1))
+    return np.power(10, (3 * b * mag + 9.1))
 
 
-def stress_drop_curve_fc_mw(delta_sigma, vs, mw, b=-0.5):
+def stress_drop_curve_fc_mw(delta_sigma, vel, mw, k=0.3724, b=-0.5):
     """
     Constant stress drop curve in fc vs Mw.
 
-    Chounet et al. (2013), https://hal.science/hal-03965701, eq. 9, page 9.
+    Obtained by combining the equation for stress drop:
+
+        delta_sigma = 7/16 * Mo / a^3
+
+    with the equation for source radius:
+
+        a = k * vel * (delta_sigma / fc)
+
+    where k is a coefficient discussed in Kaneko and Shearer (2014).
+
+    For the Brune source model, k=0.3724.
+
+    Parameters
+    ----------
+    delta_sigma : float
+        Stress drop in MPa.
+    vel : float
+        P or S-wave velocity in km/s.
+    mw : float
+        Moment magnitude.
+    b : float, optional
+        The slope of the stress drop curve. Default is -0.5.
+    k : float, optional
+        Coefficient for the source radius. Default is 0.3724
+        (Brune source model).
+
+    Returns
+    -------
+    fc : float
+        Corner frequency in Hz.
     """
-    vs *= 1e3  # S-wave velocity in m/s
+    vel *= 1e3  # P or S-wave velocity in m/s
     delta_sigma *= 1e6  # stress drop in Pa
-    # b is the slope of stress-drop curve: b!=-0.5 means no self-similarity
-    power10 = 10**(-(-3*b*mw + 9.1)-0.935)
+    # compute moment from magnitude, allowing for non-self-similarity through
+    # the b parameter
+    moment = mag_to_moment(mw, -b)
     # return fc in Hz
-    return vs * (delta_sigma * power10)**(1./3)
+    return k*vel*(16/7 * delta_sigma / moment)**(1/3)
 
 
-def stress_drop_curve_Er_mw(delta_sigma, vs, rho, mw):
+def stress_drop_curve_Er_mw(delta_sigma, mu, mw):
     """
     Constant stress drop curve in Er vs Mw.
 
     Madariaga (2009), doi:10.1007/978-1-4419-7695-6_22, eq. 33., page 374.
     """
     # Eq. (33) of Madariaga (2009):
     #   0.2331 * delta_sigma = mu * Er / Mo
-    mu = (vs*1000)**2. * rho
     Mo = mag_to_moment(mw)
     delta_sigma *= 1e6
     # return Er in N·m
     return 0.2331 * delta_sigma * Mo / mu
 
 
+def apparent_stress_curve_Er_mw(sigma_a, mu, mw):
+    """
+    Constant apparent stress curve in Er vs Mw.
+
+    Madariaga (2009), doi:10.1007/978-1-4419-7695-6_22, eq. 33., page 374.
+    """
+    # Eq. (33) of Madariaga (2009):
+    #   sigma_a = mu * Er / Mo
+    Mo = mag_to_moment(mw)
+    sigma_a *= 1e6
+    # return Er in N·m
+    return sigma_a * Mo / mu
+
+
 def fc_mw_function(mw, a, b):
-    return a/3. + b*mw
+    """Function to fit fc vs Mw."""
+    return a / 3. + b * mw
 
 
-def calc_r2(x, y, yerr, a, b, f):
+def calc_r2(x, y, yerr, a, b):
     """Coefficient of determination."""
     y_mean = np.mean(y)
     y_calc = fc_mw_function(x, a, b)
-    SS_tot = np.sum(((y-y_mean)/yerr)**2.)
-    SS_res = np.sum(((y-y_calc)/yerr)**2.)
-    return 1 - SS_res/SS_tot
+    SS_tot = np.sum(((y - y_mean) / yerr)**2.)
+    SS_res = np.sum(((y - y_calc) / yerr)**2.)
+    return 1 - SS_res / SS_tot
 
 
 def parse_args():
+    """Parse command line arguments."""
     parser = argparse.ArgumentParser()
     parser.description =\
         '1D or 2D plot of source parameters from a sqlite parameter file'
     parser.add_argument('sqlite_file')
     valid_plot_types_str = str(valid_plot_types)[1:-1].replace("'", "\"")
     parser.add_argument(
         '-p', '--plot_type', default='fc_mw',
@@ -105,15 +160,15 @@
     )
     parser.add_argument(
         '-r', '--runid', default=None,
         help='Only select a specific runid. Default is all')
     parser.add_argument(
         '-s', '--statistics', default='mean',
         help='Statistics to use: "mean", "wmean" (weighted mean) '
-             'or "pctl" (precentiles). Default is "mean"')
+             'or "pctl" (percentiles). Default is "mean"')
     parser.add_argument(
         '-i', '--nbins', type=int, default=None,
         help='Number of bins in the histogram (default: autoset)')
     parser.add_argument(
         '-n', '--stamin', type=int, default=None,
         help='Minimum number of stations')
     parser.add_argument(
@@ -122,158 +177,239 @@
     parser.add_argument(
         '-m', '--magmin', type=float, default=None,
         help='Minimum magnitude')
     parser.add_argument(
         '-M', '--magmax', type=float, default=None,
         help='Maximum magnitude')
     parser.add_argument(
-        '-b', '--bsdmin', type=float, default=None,
-        help='Minimum Brune stress drop')
+        '-d', '--ssdmin', type=float, default=None,
+        help='Minimum static stress drop')
+    parser.add_argument(
+        '-D', '--ssdmax', type=float, default=None,
+        help='Maximum static stress drop')
     parser.add_argument(
-        '-B', '--bsdmax', type=float, default=None,
-        help='Maximum Brune stress drop')
+        '-a', '--sigmaamin', type=float, default=None,
+        help='Minimum apparent stress drop')
+    parser.add_argument(
+        '-A', '--sigmaamax', type=float, default=None,
+        help='Maximum apparent stress drop')
     parser.add_argument(
         '-H', '--hist', default=False, action='store_true',
         help='Draw an histogram instead of a scatter plot (only for 2D plots)')
     parser.add_argument(
         '-f', '--fit', default=False, action='store_true',
         help='Fit the scatter plot with a linear function (only for 2D plots)')
     parser.add_argument(
-        '-S', '--slope', default=False, action='store_true',
+        '-l', '--slope', default=False, action='store_true',
         help='Fit also the slope of the linear function (only for 2D plots)')
+    parser.add_argument(
+        '-w', '--wave_type', default='S',
+        help='Wave type. Only used for plots involving "fc". '
+             'One of "P", "S", "SV" or "SH". Default is "S".')
     args = parser.parse_args()
     if args.plot_type not in valid_plot_types:
         msg = f'Plot type must be one of {valid_plot_types_str}'
         raise ValueError(msg)
     if args.statistics not in ['mean', 'wmean', 'pctl']:
         msg = 'Statistics must be "mean", "wmean" or "pctl"'
         raise ValueError(msg)
+    if args.wave_type not in ['P', 'S', 'SV', 'SH']:
+        msg = 'Wave type must be "P", "S", "SV" or "SH"'
+        raise ValueError(msg)
     return args
 
 
 def query_event_params_into_numpy(cursor, param, param_type, query_condition):
-    query = f'select {param} from Events {query_condition}'
+    """
+    Query a parameter from the Events table and return it as a numpy array.
+    """
+    query = f'select {param} from Events {query_condition} order by evid,runid'
     cursor.execute(query)
     result = np.array(cursor.fetchall())
     if len(result) == 0:
         raise ValueError('No events found')
     return result[:, 0].astype(param_type)
 
 
-class Params(object):
-    def __init__(self, sqlite_file, runid, stat):
+class Params():
+    """
+    Class to handle the parameters from a sqlite file.
+    """
+    def __init__(self, args):
         """
         Initialize the class from a sqlite file.
         """
-        self.stat = stat
-        self.runid = runid
-        conn = sqlite3.connect(sqlite_file)
-        cur = conn.cursor()
+        self.args = args
+        self.sqlite_file = args.sqlite_file
+        self.runid = runid = args.runid
+        self.stat = stat = args.statistics
+        self._open_db(self.sqlite_file)
         query_condition = f'where runid="{runid}"' if runid is not None else ''
         self.evids = query_event_params_into_numpy(
-            cur, 'evid', str, query_condition)
+            self.cur, 'evid', str, query_condition)
+        self.vp = query_event_params_into_numpy(
+            self.cur, 'vp', np.float64, query_condition)
+        self.vs = query_event_params_into_numpy(
+            self.cur, 'vs', np.float64, query_condition)
+        self.rho = query_event_params_into_numpy(
+            self.cur, 'rho', np.float64, query_condition)
+        self.kp = query_event_params_into_numpy(
+            self.cur, 'kp', np.float64, query_condition)
+        self.ks = query_event_params_into_numpy(
+            self.cur, 'ks', np.float64, query_condition)
+        self.wave_type = query_event_params_into_numpy(
+            self.cur, 'wave_type', str, query_condition)
         self.nsta = query_event_params_into_numpy(
-            cur, 'nobs', np.int32, query_condition)
+            self.cur, 'nobs', np.int32, query_condition)
         self.Mo = query_event_params_into_numpy(
-            cur, f'Mo_{stat}', np.float64, query_condition)
+            self.cur, f'Mo_{stat}', np.float64, query_condition)
         self.mw = query_event_params_into_numpy(
-            cur, f'Mw_{stat}', np.float64, query_condition)
+            self.cur, f'Mw_{stat}', np.float64, query_condition)
         self.mw_err_minus = query_event_params_into_numpy(
-            cur, f'Mw_{stat}_err_minus', np.float64, query_condition)
+            self.cur, f'Mw_{stat}_err_minus', np.float64, query_condition)
         self.mw_err_plus = query_event_params_into_numpy(
-            cur, f'Mw_{stat}_err_plus', np.float64, query_condition)
+            self.cur, f'Mw_{stat}_err_plus', np.float64, query_condition)
         self.fc = query_event_params_into_numpy(
-            cur, f'fc_{stat}', np.float64, query_condition)
+            self.cur, f'fc_{stat}', np.float64, query_condition)
         self.fc_err_minus = query_event_params_into_numpy(
-            cur, f'fc_{stat}_err_minus', np.float64, query_condition)
+            self.cur, f'fc_{stat}_err_minus', np.float64, query_condition)
         self.fc_err_plus = query_event_params_into_numpy(
-            cur, f'fc_{stat}_err_plus', np.float64, query_condition)
+            self.cur, f'fc_{stat}_err_plus', np.float64, query_condition)
         self.Er = query_event_params_into_numpy(
-            cur, f'Er_{stat}', np.float64, query_condition)
+            self.cur, f'Er_{stat}', np.float64, query_condition)
         self.Er_err_minus = query_event_params_into_numpy(
-            cur, f'Er_{stat}_err_minus', np.float64, query_condition)
+            self.cur, f'Er_{stat}_err_minus', np.float64, query_condition)
         self.Er_err_plus = query_event_params_into_numpy(
-            cur, f'Er_{stat}_err_plus', np.float64, query_condition)
-        self.bsd = query_event_params_into_numpy(
-            cur, f'bsd_{stat}', np.float64, query_condition)
-        self.bsd_err_minus = query_event_params_into_numpy(
-            cur, f'bsd_{stat}_err_minus', np.float64, query_condition)
-        self.bsd_err_plus = query_event_params_into_numpy(
-            cur, f'bsd_{stat}_err_plus', np.float64, query_condition)
+            self.cur, f'Er_{stat}_err_plus', np.float64, query_condition)
+        self.ssd = query_event_params_into_numpy(
+            self.cur, f'ssd_{stat}', np.float64, query_condition)
+        self.ssd_err_minus = query_event_params_into_numpy(
+            self.cur, f'ssd_{stat}_err_minus', np.float64, query_condition)
+        self.ssd_err_plus = query_event_params_into_numpy(
+            self.cur, f'ssd_{stat}_err_plus', np.float64, query_condition)
         self.ra = query_event_params_into_numpy(
-            cur, f'ra_{stat}', np.float64, query_condition)
+            self.cur, f'ra_{stat}', np.float64, query_condition)
         self.ra_err_minus = query_event_params_into_numpy(
-            cur, f'ra_{stat}_err_minus', np.float64, query_condition)
+            self.cur, f'ra_{stat}_err_minus', np.float64, query_condition)
         self.ra_err_plus = query_event_params_into_numpy(
-            cur, f'ra_{stat}_err_plus', np.float64, query_condition)
+            self.cur, f'ra_{stat}_err_plus', np.float64, query_condition)
+        self.sigma_a = query_event_params_into_numpy(
+            self.cur, f'sigma_a_{stat}', np.float64, query_condition)
+        self.sigma_a_err_minus = query_event_params_into_numpy(
+            self.cur, f'sigma_a_{stat}_err_minus', np.float64, query_condition)
+        self.sigma_a_err_plus = query_event_params_into_numpy(
+            self.cur, f'sigma_a_{stat}_err_plus', np.float64, query_condition)
         self.t_star = query_event_params_into_numpy(
-            cur, f't_star_{stat}', np.float64, query_condition)
+            self.cur, f't_star_{stat}', np.float64, query_condition)
         self.t_star_err_minus = query_event_params_into_numpy(
-            cur, f't_star_{stat}_err_minus', np.float64, query_condition)
+            self.cur, f't_star_{stat}_err_minus', np.float64, query_condition)
         self.t_star_err_plus = query_event_params_into_numpy(
-            cur, f't_star_{stat}_err_plus', np.float64, query_condition)
+            self.cur, f't_star_{stat}_err_plus', np.float64, query_condition)
         self.Qo = query_event_params_into_numpy(
-            cur, f'Qo_{stat}', np.float64, query_condition)
+            self.cur, f'Qo_{stat}', np.float64, query_condition)
         self.Qo_err_minus = query_event_params_into_numpy(
-            cur, f'Qo_{stat}_err_minus', np.float64, query_condition)
+            self.cur, f'Qo_{stat}_err_minus', np.float64, query_condition)
         self.Qo_err_plus = query_event_params_into_numpy(
-            cur, f'Qo_{stat}_err_plus', np.float64, query_condition)
-        cur.close()
+            self.cur, f'Qo_{stat}_err_plus', np.float64, query_condition)
+        self.cur.close()
+        # other attributes
+        self.nbins_x = None
+        self.nbins_y = None
+
+    def _open_db(self, sqlite_file):
+        """
+        Open the sqlite file and check that it contains the required tables.
+        """
+        if not os.path.isfile(sqlite_file):
+            raise FileNotFoundError(f'File "{sqlite_file}" not found')
+        if os.stat(sqlite_file).st_size == 0:
+            raise ValueError(f'File "{sqlite_file}" is empty')
+        conn = sqlite3.connect(sqlite_file)
+        cur = conn.cursor()
+        try:
+            cur.execute("SELECT name FROM sqlite_master WHERE type='table';")
+        except sqlite3.DatabaseError as e:
+            raise ValueError(
+                f'File "{sqlite_file}" is not a valid sqlite file'
+            ) from e
+        tables = [t[0] for t in cur.fetchall()]
+        for table in 'Events', 'Stations':
+            if table not in tables:
+                raise ValueError(
+                    f'Table "{table}" not found in file "{sqlite_file}"')
+        self.cur = cur
 
     def skip_events(self, idx):
         """Skip events with index idx."""
         self.evids = np.delete(self.evids, idx)
+        self.vp = np.delete(self.vp, idx)
+        self.vs = np.delete(self.vs, idx)
+        self.rho = np.delete(self.rho, idx)
+        self.kp = np.delete(self.kp, idx)
+        self.ks = np.delete(self.ks, idx)
+        self.wave_type = np.delete(self.wave_type, idx)
         self.nsta = np.delete(self.nsta, idx)
         self.Mo = np.delete(self.Mo, idx)
         self.mw = np.delete(self.mw, idx)
         self.mw_err_minus = np.delete(self.mw_err_minus, idx)
         self.mw_err_plus = np.delete(self.mw_err_plus, idx)
         self.fc = np.delete(self.fc, idx)
         self.fc_err_minus = np.delete(self.fc_err_minus, idx)
         self.fc_err_plus = np.delete(self.fc_err_plus, idx)
         self.Er = np.delete(self.Er, idx)
         self.Er_err_minus = np.delete(self.Er_err_minus, idx)
         self.Er_err_plus = np.delete(self.Er_err_plus, idx)
-        self.bsd = np.delete(self.bsd, idx)
-        self.bsd_err_minus = np.delete(self.bsd_err_minus, idx)
-        self.bsd_err_plus = np.delete(self.bsd_err_plus, idx)
+        self.ssd = np.delete(self.ssd, idx)
+        self.ssd_err_minus = np.delete(self.ssd_err_minus, idx)
+        self.ssd_err_plus = np.delete(self.ssd_err_plus, idx)
         self.ra = np.delete(self.ra, idx)
         self.ra_err_minus = np.delete(self.ra_err_minus, idx)
         self.ra_err_plus = np.delete(self.ra_err_plus, idx)
+        self.sigma_a = np.delete(self.sigma_a, idx)
+        self.sigma_a_err_minus = np.delete(self.sigma_a_err_minus, idx)
+        self.sigma_a_err_plus = np.delete(self.sigma_a_err_plus, idx)
         self.t_star = np.delete(self.t_star, idx)
         self.t_star_err_minus = np.delete(self.t_star_err_minus, idx)
         self.t_star_err_plus = np.delete(self.t_star_err_plus, idx)
         self.Qo = np.delete(self.Qo, idx)
         self.Qo_err_minus = np.delete(self.Qo_err_minus, idx)
         self.Qo_err_plus = np.delete(self.Qo_err_plus, idx)
 
     def filter(self, stamin=None, stamax=None, magmin=None, magmax=None,
-               bsdmin=None, bsdmax=None):
+               ssdmin=None, ssdmax=None, sigmaamin=None, sigmaamax=None):
         """Filter the parameters based on one or more conditions."""
         cond = np.ones(len(self.nsta)).astype(bool)
         if stamin is not None:
             cond = np.logical_and(cond, self.nsta >= stamin)
         if stamax is not None:
             cond = np.logical_and(cond, self.nsta <= stamax)
         if magmin is not None:
             cond = np.logical_and(cond, self.mw >= magmin)
         if magmax is not None:
             cond = np.logical_and(cond, self.mw <= magmax)
-        if bsdmin is not None:
-            cond = np.logical_and(cond, self.bsd >= bsdmin)
-        if bsdmax is not None:
-            cond = np.logical_and(cond, self.bsd <= bsdmax)
+        if ssdmin is not None:
+            cond = np.logical_and(cond, self.ssd >= ssdmin)
+        if ssdmax is not None:
+            cond = np.logical_and(cond, self.ssd <= ssdmax)
+        if sigmaamin is not None:
+            cond = np.logical_and(cond, self.sigma_a >= sigmaamin)
+        if sigmaamax is not None:
+            cond = np.logical_and(cond, self.sigma_a <= sigmaamax)
         self.skip_events(np.where(~cond)[0])
 
     def _make_mw_axis(self):
         """Make the magnitude axis."""
-        mag_min = np.min(self.mw - self.mw_err_minus)
-        mag_max = np.max(self.mw + self.mw_err_plus)
-        mag_min = np.floor(mag_min)
-        mag_max = np.ceil(mag_max)
+        if self.args.magmin is not None:
+            mag_min = self.args.magmin
+        else:
+            mag_min = np.floor(np.min(self.mw - self.mw_err_minus))
+        if self.args.magmax is not None:
+            mag_max = self.args.magmax
+        else:
+            mag_max = np.ceil(np.max(self.mw + self.mw_err_plus))
         xlim_mag = (mag_min, mag_max)
         fig = plt.figure(figsize=(10, 6))
         ax_Mo = fig.add_subplot(111)
         ax_Mo.set_xscale('log')
         ax_Mo.set_xlim(mag_to_moment(xlim_mag))
         ax = ax_Mo.twiny()
         ax.set_xlim(xlim_mag)
@@ -286,224 +422,283 @@
         ax.grid(
             True, which='major', linestyle='solid',
             color='#999999', zorder=0)
         ax.grid(
             True, which='minor', linestyle='solid',
             color='#DDDDDD', zorder=0)
 
-    def _set_plot_title(self, ax):
+    def _set_plot_title(self, ax, nevs=None, extra_text=None):
         """Set the plot title."""
-        nevs = len(self.nsta)
+        if nevs is None:
+            nevs = len(self.evids)
         stat_descr = {
             'mean': 'mean',
             'wmean': 'weighted mean',
             'pctl': 'percentiles',
         }
         title = f'{nevs} events'
-        with contextlib.suppress(AttributeError):
+        if None not in (self.nbins_x, self.nbins_y):
             title += f', {self.nbins_x}x{self.nbins_y} bins'
         title += f' - {stat_descr[self.stat]}'
         if self.runid is not None:
             title += f' - runid: {self.runid}'
-        ax.set_title(title, y=0.92)
+        if extra_text is not None:
+            title += f'\n{extra_text}'
+        ax.set_title(title, y=0.95, verticalalignment='top')
 
-    def _stress_drop_curves_fc_mw(self, vs, ax):
+    def _stress_drop_curves_fc_mw(self, vel, k_parameter, ax):
         """Plot stress-drop curves for different delta_sigma."""
         mag_min, mag_max = ax.get_xlim()
         mw_step = 0.1
-        mw_test = np.arange(mag_min, mag_max-2*mw_step, mw_step)
+        mw_test = np.arange(mag_min, mag_max - 2 * mw_step, mw_step)
         fc_min = np.inf
         fc_max = 0.
         for delta_sigma in (0.1, 1., 10., 100.):
-            fc_test = stress_drop_curve_fc_mw(delta_sigma, vs, mw_test)
+            fc_test = stress_drop_curve_fc_mw(
+                delta_sigma, vel, mw_test, k_parameter)
             if fc_test.min() < fc_min:
                 fc_min = fc_test.min()
             if fc_test.max() > fc_max:
                 fc_max = fc_test.max()
             ax.plot(mw_test, fc_test, color='#555555')
             label = str(delta_sigma)
-            # Get rid of ".0" in floats
-            label = label.rstrip('.0') + ' MPa'
+            # Get rid of ".0" in label
+            if label.endswith('.0'):
+                label = label[:-2]
+            label += ' MPa'
             ax.text(mw_test[-1], fc_test[-1], label)
-        ax.set_ylim((fc_min*0.9, fc_max*1.1))
+        ax.set_ylim((fc_min * 0.9, fc_max * 1.1))
 
-    def _stress_drop_curves_Er_mw(self, vs, rho, ax):
+    def _stress_drop_curves_Er_mw(self, mu, ax):
         """Plot stress-drop curves for different delta_sigma."""
         mag_min, mag_max = ax.get_xlim()
         mw_step = 0.1
-        mw_test = np.arange(mag_min, mag_max-2*mw_step, mw_step)
+        mw_test = np.arange(mag_min, mag_max - 2 * mw_step, mw_step)
         Er_min = np.inf
         Er_max = 0.
         for delta_sigma in (0.1, 1., 10., 100.):
-            Er_test = stress_drop_curve_Er_mw(delta_sigma, vs, rho, mw_test)
+            Er_test = stress_drop_curve_Er_mw(delta_sigma, mu, mw_test)
             if Er_test.min() < Er_min:
                 Er_min = Er_test.min()
             if Er_test.max() > Er_max:
                 Er_max = Er_test.max()
             ax.plot(mw_test, Er_test, color='#555555')
             label = str(delta_sigma)
-            # Get rid of ".0" in floats
-            label = label.rstrip('.0') + ' MPa'
+            # Get rid of ".0" in label
+            if label.endswith('.0'):
+                label = label[:-2]
+            label += ' MPa'
             ax.text(mw_test[-1], Er_test[-1], label)
-        ax.set_ylim((Er_min*0.5, Er_max*2))
+        ax.set_ylim((Er_min * 0.5, Er_max * 2))
 
-    def _2d_hist_fc_mw(self, fig, ax, nbins=None):
+    def _apparent_stress_curves_Er_mw(self, mu, ax):
+        """Plot apparent stress curves for different delta_sigma."""
+        mag_min, mag_max = ax.get_xlim()
+        mw_step = 0.1
+        mw_test = np.arange(mag_min, mag_max - 2 * mw_step, mw_step)
+        Er_min = np.inf
+        Er_max = 0.
+        for sigma_a in (0.1, 1., 10., 100.):
+            Er_test = apparent_stress_curve_Er_mw(sigma_a, mu, mw_test)
+            if Er_test.min() < Er_min:
+                Er_min = Er_test.min()
+            if Er_test.max() > Er_max:
+                Er_max = Er_test.max()
+            ax.plot(mw_test, Er_test, color='#555555')
+            label = str(sigma_a)
+            # Get rid of ".0" in label
+            if label.endswith('.0'):
+                label = label[:-2]
+            label += ' MPa'
+            ax.text(mw_test[-1], Er_test[-1], label)
+        ax.set_ylim((Er_min * 0.5, Er_max * 2))
+
+    def _2d_hist_fc_mw(self, fig, ax, nbins=None, wave_type='S'):
         """Plot a 2d histogram of fc vs mw."""
         mw_min, mw_max = ax.get_xlim()
         fc_min, fc_max = ax.get_ylim()
         log_fc_min = np.log10(fc_min)
         log_fc_max = np.log10(fc_max)
         if nbins is None:
             mw_nbins = int((mw_max - mw_min) * 10)
             fc_nbins = int((log_fc_max - log_fc_min) * 10)
         else:
             mw_nbins = nbins
             fc_nbins = nbins
         self.nbins_x = mw_nbins
         self.nbins_y = fc_nbins
-        mw_bins = np.linspace(mw_min, mw_max+0.1, mw_nbins)
-        fc_bins = 10**np.linspace(log_fc_min, log_fc_max+0.1, fc_nbins)
-        counts, _, _ = np.histogram2d(
-            self.mw, self.fc, bins=(mw_bins, fc_bins))
+        mw_bins = np.linspace(mw_min, mw_max + 0.1, mw_nbins)
+        fc_bins = 10**np.linspace(log_fc_min, log_fc_max + 0.1, fc_nbins)
+        cond = self.wave_type == wave_type
+        mw = self.mw[cond]
+        if len(mw) == 0:
+            raise ValueError(f'No events found for wave type "{wave_type}"')
+        fc = self.fc[cond]
+        counts, _, _ = np.histogram2d(mw, fc, bins=(mw_bins, fc_bins))
         cm = ax.pcolormesh(
             mw_bins[:-1], fc_bins[:-1], counts.T,
             cmap='magma_r', shading='auto')
         cbaxes = fig.add_axes([0.15, 0.15, 0.02, 0.2])
         plt.colorbar(cm, cax=cbaxes, orientation='vertical', label='counts')
+        return len(fc)
 
     def _2d_hist_Er_mw(self, fig, ax, nbins=None):
         """Plot a 2d histogram of Er vs mw."""
         mw_min, mw_max = ax.get_xlim()
         Er_min, Er_max = ax.get_ylim()
         log_Er_min = np.log10(Er_min)
         log_Er_max = np.log10(Er_max)
         if nbins is None:
             mw_nbins = int((mw_max - mw_min) * 10)
             Er_nbins = int((log_Er_max - log_Er_min) * 5)
         else:
             mw_nbins = nbins
             Er_nbins = nbins
-        mw_bins = np.linspace(mw_min, mw_max+0.1, mw_nbins)
-        Er_bins = 10**np.linspace(log_Er_min, log_Er_max+0.1, Er_nbins)
+        mw_bins = np.linspace(mw_min, mw_max + 0.1, mw_nbins)
+        Er_bins = 10**np.linspace(log_Er_min, log_Er_max + 0.1, Er_nbins)
         self.nbins_x = mw_nbins
         self.nbins_y = Er_nbins
-        counts, _, _ = np.histogram2d(
-            self.mw, self.Er, bins=(mw_bins, Er_bins))
+        # Er can be NaN
+        cond = ~np.isnan(self.Er)
+        mw = self.mw[cond]
+        Er = self.Er[cond]
+        counts, _, _ = np.histogram2d(mw, Er, bins=(mw_bins, Er_bins))
         cm = ax.pcolormesh(
             mw_bins[:-1], Er_bins[:-1], counts.T,
             cmap='magma_r', shading='auto')
         cbaxes = fig.add_axes([0.15, 0.15, 0.02, 0.2])
         plt.colorbar(cm, cax=cbaxes, orientation='vertical', label='counts')
+        return len(Er)
 
-    def _2d_hist_bsd_mw(self, fig, ax, nbins=None):
-        """Plot a 2d histogram of bsd vs mw."""
+    def _2d_hist_ssd_mw(self, fig, ax, nbins=None):
+        """Plot a 2d histogram of ssd vs mw."""
         mw_min, mw_max = ax.get_xlim()
-        bsd_min, bsd_max = ax.get_ylim()
-        log_bsd_min = np.log10(bsd_min)
-        log_bsd_max = np.log10(bsd_max)
+        ssd_min, ssd_max = ax.get_ylim()
+        log_ssd_min = np.log10(ssd_min)
+        log_ssd_max = np.log10(ssd_max)
         if nbins is None:
             mw_nbins = int((mw_max - mw_min) * 10)
-            bsd_nbins = int((log_bsd_max - log_bsd_min) * 5)
+            ssd_nbins = int((log_ssd_max - log_ssd_min) * 5)
         else:
             mw_nbins = nbins
-            bsd_nbins = nbins
-        mw_bins = np.linspace(mw_min, mw_max+0.1, mw_nbins)
-        bsd_bins = 10**np.linspace(log_bsd_min, log_bsd_max+0.1, bsd_nbins)
+            ssd_nbins = nbins
+        mw_bins = np.linspace(mw_min, mw_max + 0.1, mw_nbins)
+        ssd_bins = 10**np.linspace(log_ssd_min, log_ssd_max + 0.1, ssd_nbins)
         self.nbins_x = mw_nbins
-        self.nbins_y = bsd_nbins
+        self.nbins_y = ssd_nbins
         counts, _, _ = np.histogram2d(
-            self.mw, self.bsd, bins=(mw_bins, bsd_bins))
+            self.mw, self.ssd, bins=(mw_bins, ssd_bins))
         cm = ax.pcolormesh(
-            mw_bins[:-1], bsd_bins[:-1], counts.T,
+            mw_bins[:-1], ssd_bins[:-1], counts.T,
             cmap='magma_r', shading='auto')
         cbaxes = fig.add_axes([0.15, 0.15, 0.02, 0.2])
         plt.colorbar(cm, cax=cbaxes, orientation='vertical', label='counts')
 
-    def _scatter_fc_mw(self, fig, ax):
+    def _scatter_fc_mw(self, fig, ax, wave_type='S'):
         """Plot the scatter plot of fc vs mw."""
+        cond = self.wave_type == wave_type
+        evids = self.evids[cond]
+        if len(evids) == 0:
+            raise ValueError(f'No events found for wave type "{wave_type}"')
+        mw = self.mw[cond]
+        mw_err_minus = self.mw_err_minus[cond]
+        mw_err_plus = self.mw_err_plus[cond]
+        fc = self.fc[cond]
+        fc_err_minus = self.fc_err_minus[cond]
+        fc_err_plus = self.fc_err_plus[cond]
         alpha = 1
         ax.errorbar(
-            self.mw, self.fc,
-            xerr=[self.mw_err_minus, self.mw_err_plus],
-            yerr=[self.fc_err_minus, self.fc_err_plus],
+            mw, fc,
+            xerr=[mw_err_minus, mw_err_plus],
+            yerr=[fc_err_minus, fc_err_plus],
             fmt='o', mec='black', mfc='#FCBA25', ecolor='#FCBA25',
             alpha=alpha)
-        ax.scatter(self.mw, self.fc, alpha=0, picker=True, zorder=20)
+        ax.scatter(mw, fc, alpha=0, picker=True, zorder=20)
         yformat = 'fc {:.2f} Hz'
-        annot = Annot(self.mw, self.fc, self.evids, yformat)
+        annot = Annot(mw, fc, evids, yformat)
         fig.canvas.mpl_connect('pick_event', annot)
+        return len(fc)
 
     def _scatter_Er_mw(self, fig, ax):
         """Plot the scatter plot of Er vs mw."""
+        # Er can be NaN
+        cond = ~np.isnan(self.Er)
+        mw = self.mw[cond]
+        mw_err_minus = self.mw_err_minus[cond]
+        mw_err_plus = self.mw_err_plus[cond]
+        Er = self.Er[cond]
+        Er_err_minus = self.Er_err_minus[cond]
+        Er_err_plus = self.Er_err_plus[cond]
+        evids = self.evids[cond]
         alpha = 1
         ax.errorbar(
-            self.mw, self.Er,
-            xerr=[self.mw_err_minus, self.mw_err_plus],
-            yerr=[self.Er_err_minus, self.Er_err_plus],
+            mw, Er,
+            xerr=[mw_err_minus, mw_err_plus],
+            yerr=[Er_err_minus, Er_err_plus],
             fmt='o', mec='black', mfc='#FCBA25', ecolor='#FCBA25',
             alpha=alpha)
-        ax.scatter(self.mw, self.Er, alpha=0, picker=True, zorder=20)
-        yformat = 'Er {:.1e} J'
-        annot = Annot(self.mw, self.Er, self.evids, yformat)
+        ax.scatter(mw, Er, alpha=0, picker=True, zorder=20)
+        yformat = 'Er {:.1e} N·m'
+        annot = Annot(mw, Er, evids, yformat)
         fig.canvas.mpl_connect('pick_event', annot)
+        return len(Er)
 
-    def _scatter_bsd_mw(self, fig, ax):
-        """Plot the scatter plot of bsd vs mw."""
+    def _scatter_ssd_mw(self, fig, ax):
+        """Plot the scatter plot of ssd vs mw."""
         alpha = 1
         ax.errorbar(
-            self.mw, self.bsd,
+            self.mw, self.ssd,
             xerr=[self.mw_err_minus, self.mw_err_plus],
-            yerr=[self.bsd_err_minus, self.bsd_err_plus],
+            yerr=[self.ssd_err_minus, self.ssd_err_plus],
             fmt='o', mec='black', mfc='#FCBA25', ecolor='#FCBA25',
             alpha=alpha)
-        ax.scatter(self.mw, self.bsd, alpha=0, picker=True, zorder=20)
-        yformat = 'bsd {:.2e} MPa'
-        annot = Annot(self.mw, self.bsd, self.evids, yformat)
+        ax.scatter(self.mw, self.ssd, alpha=0, picker=True, zorder=20)
+        yformat = 'ssd {:.2e} MPa'
+        annot = Annot(self.mw, self.ssd, self.evids, yformat)
         fig.canvas.mpl_connect('pick_event', annot)
 
-    def _fit_fc_mw(self, vs, ax, slope=False):
+    def _fit_fc_mw(self, vel, k_parameter, ax, slope=False):
         """Plot a linear regression of fc vs mw."""
         mag_min, mag_max = ax.get_xlim()
         mw_step = 0.1
-        mw_test = np.arange(mag_min, mag_max-2*mw_step, mw_step)
+        mw_test = np.arange(mag_min, mag_max - 2 * mw_step, mw_step)
         if slope:
             f = fc_mw_function
         else:
             def f(mw, a):
                 return fc_mw_function(mw, a, -0.5)
         y = np.log10(self.fc)
-        # yerr = np.log10(self.fc_err_max-self.fc_err_min)/2.
-        popt, pcov = curve_fit(f, self.mw, y)
-        # popt, pcov = curve_fit(f, self.mw, y, p0=popt, sigma=yerr)
-        # popt, pcov = curve_fit(f, self.mw, y, sigma=yerr)
+        # pylint: disable=unbalanced-tuple-unpacking
+        popt, _pcov = curve_fit(f, self.mw, y)
         try:
             a, b = popt
         except Exception:
             a, = popt
             b = -0.5
         print(f'a: {a:.1f} b {b:.1f}:')
-        slope = (3/2)/b
+        slope = (3 / 2) / b
         print(f'slope: {slope:.1f}')
-        r2 = calc_r2(self.mw, y, np.ones_like(y), a, b, f)
-        # r2_err = calc_r2(mw, y, yerr, a, b, f)
+        r2 = calc_r2(self.mw, y, np.ones_like(y), a, b)
         print('r2:', r2)
         # print('r2_err:', r2_err)
-        delta_sigma = 1./((vs*1000.)**3.) * 10**(a + 9.1 + 0.935)
+        delta_sigma = 1. / ((vel * 1000.)**3.) * 10**(a + 9.1 + 0.935)
         delta_sigma /= 1e6
         print('delta_sigma', delta_sigma)
-        fc_test = stress_drop_curve_fc_mw(delta_sigma, vs, mw_test, b)
+        fc_test = stress_drop_curve_fc_mw(
+            delta_sigma, vel, mw_test, k_parameter, b=b)
         ax.plot(
             mw_test, fc_test, color='red', zorder=10, label=f'r2: {r2:.2f}')
         ax.legend()
         if not slope:
             ax.text(
                 mw_test[-1], fc_test[-1], f'{delta_sigma:.1f} MPa',
                 color='red', backgroundcolor='white', zorder=50)
 
-    def plot_fc_mw(self, hist=False, fit=False, slope=False, nbins=None):
+    def plot_fc_mw(self, hist=False, fit=False, slope=False, nbins=None,
+                   wave_type='S'):
         """
         Plot the logarithm of the corner frequency vs the moment magnitude.
 
         Parameters
         ----------
         hist : bool
             If True, plot a 2D histogram instead of a scatter plot.
@@ -511,29 +706,37 @@
             If True, plot a linear regression of fc vs mw.
         slope : bool
             If True, also fit the slope of the linear regression.
         """
         fig, ax, ax_Mo = self._make_mw_axis()
         ax_Mo.set_yscale('log')
 
-        vs = 3.5
-        self._stress_drop_curves_fc_mw(vs, ax)
+        if wave_type == 'P':
+            vel = np.nanmean(self.vp)
+            k = np.nanmean(self.kp)
+        elif wave_type in ('S', 'SV', 'SH'):
+            vel = np.nanmean(self.vs)
+            k = np.nanmean(self.ks)
+        else:
+            raise ValueError('Wave type must be "P", "S", "SV" or "SH"')
+        self._stress_drop_curves_fc_mw(vel, k, ax)
 
         if hist:
-            self._2d_hist_fc_mw(fig, ax, nbins)
+            npoints = self._2d_hist_fc_mw(fig, ax, nbins, wave_type)
         else:
-            self._scatter_fc_mw(fig, ax)
+            npoints = self._scatter_fc_mw(fig, ax, wave_type)
         if fit:
-            self._fit_fc_mw(vs, ax, slope=slope)
-        self._set_plot_title(ax)
+            self._fit_fc_mw(vel, k, ax, slope=slope)
+        extra_text = 'Stress drop curves'
+        self._set_plot_title(ax, npoints, extra_text)
         self._add_grid(ax_Mo)
         ax_Mo.set_ylabel('fc (Hz)')
         plt.show()
 
-    def plot_Er_mw(self, hist=False, fit=False, slope=False, nbins=None):
+    def plot_Er_mw(self, hist=False, fit=False, nbins=None):
         """
         Plot the logarithm of the radiated energy vs the moment magnitude.
 
         Parameters
         ----------
         hist : bool
             If True, plot a 2D histogram instead of a scatter plot.
@@ -541,102 +744,113 @@
             If True, plot a linear regression of Er vs mw.
         slope : bool
             If True, also fit the slope of the linear regression.
         """
         fig, ax, ax_Mo = self._make_mw_axis()
         ax_Mo.set_yscale('log')
 
-        vs = 3.5
-        rho = 2700.
-        self._stress_drop_curves_Er_mw(vs, rho, ax)
+        mu = np.nanmean((self.vs * 1e3)**2 * self.rho)
+        self._apparent_stress_curves_Er_mw(mu, ax)
 
         if hist:
-            self._2d_hist_Er_mw(fig, ax, nbins)
+            npoints = self._2d_hist_Er_mw(fig, ax, nbins)
         else:
-            self._scatter_Er_mw(fig, ax)
+            npoints = self._scatter_Er_mw(fig, ax)
         if fit:
             raise NotImplementedError('Fit not implemented yet for Er_mw')
 
-        self._set_plot_title(ax)
+        extra_text = 'Apparent stress curves'
+        self._set_plot_title(ax, npoints, extra_text)
         self._add_grid(ax_Mo)
-        ax_Mo.set_ylabel('Er (J)')
+        ax_Mo.set_ylabel('Er (N·m)')
         plt.show()
 
-    def plot_bsd_mw(self, hist=False, fit=False, slope=False, nbins=None):
+    def plot_ssd_mw(self, hist=False, fit=False, nbins=None):
         """
-        Plot the logarithm of the Brune stress drop vs the moment magnitude.
+        Plot the logarithm of static stress drop vs moment magnitude.
 
         Parameters
         ----------
         hist : bool
             If True, plot a 2D histogram instead of a scatter plot.
         fit : bool
-            If True, plot a linear regression of bsd vs mw.
+            If True, plot a linear regression of ssd vs mw.
         slope : bool
             If True, also fit the slope of the linear regression.
         """
         fig, ax, ax_Mo = self._make_mw_axis()
         ax_Mo.set_yscale('log')
 
-        bsd_min = np.min(self.bsd - self.bsd_err_minus)
-        bsd_max = np.max(self.bsd + self.bsd_err_plus)
-        bsd_min = 10**(np.floor(np.log10(bsd_min)))
-        bsd_max = 10**(np.ceil(np.log10(bsd_max)))
-        ax.set_ylim(bsd_min, bsd_max)
+        ssd_min = np.min(self.ssd - self.ssd_err_minus)
+        ssd_max = np.max(self.ssd + self.ssd_err_plus)
+        ssd_min = 10**(np.floor(np.log10(ssd_min)))
+        ssd_max = 10**(np.ceil(np.log10(ssd_max)))
+        ax.set_ylim(ssd_min, ssd_max)
 
         if hist:
-            self._2d_hist_bsd_mw(fig, ax, nbins)
+            self._2d_hist_ssd_mw(fig, ax, nbins)
         else:
-            self._scatter_bsd_mw(fig, ax)
+            self._scatter_ssd_mw(fig, ax)
         if fit:
-            raise NotImplementedError('Fit not implemented yet for bsd_mw')
+            raise NotImplementedError('Fit not implemented yet for ssd_mw')
 
         self._set_plot_title(ax)
         self._add_grid(ax_Mo)
-        ax_Mo.set_ylabel('bsd (MPa)')
+        ax_Mo.set_ylabel('ssd (MPa)')
         plt.show()
 
-    def plot_hist(self, param_name, nbins=None):
+    def plot_hist(self, param_name, nbins=None, wave_type='S'):
+        """Plot a histogram of the given parameter."""
         parameters = {
             'fc': ('Corner Frequency', 'Hz', 'log'),
-            'bsd': ('Brune Stress Drop', 'MPa', 'log'),
+            'ssd': ('Static Stress Drop', 'MPa', 'log'),
             'ra': ('Source Radius', 'm', 'lin'),
             'Mo': ('Seismic Moment', 'N·m', 'log'),
             't_star': ('T star', 's', 'lin'),
             'Qo': ('Qo', None, 'lin'),
-            'Er': ('Radiated Energy', 'J', 'log'),
+            'Er': ('Radiated Energy', 'N·m', 'log'),
+            'sigma_a': ('Apparent Stress', 'MPa', 'log'),
         }
         description, unit, log = parameters[param_name]
-        log = (log == 'log')
+        log = log == 'log'
         values = getattr(self, param_name)
+        if param_name == 'fc':
+            values = values[self.wave_type == wave_type]
+            if len(values) == 0:
+                raise ValueError(
+                    f'No events found for wave type "{wave_type}"')
+        values = values[~np.isnan(values)]
         nvalues = len(values)
+        if nvalues < 2:
+            raise ValueError(f'Not enough values to plot histogram: {nvalues}')
         if nbins is None:
             # find the number of bins as the closest power of 10 to the
             # number of values divided by 10
-            nbins_exp = int(np.ceil(np.log10(nvalues/10)))
+            nbins_exp = int(np.ceil(np.log10(nvalues / 10)))
             nbins = int(10**nbins_exp)
             # reduce the number of bins if there are too few values per bin
-            if nvalues/nbins < 2:
+            if nvalues / nbins < 2:
                 nbins //= 2
         if log:
             values_mean = 10**(np.mean(np.log10(values)))
             min_exp = np.floor(np.min(np.log10(values)))
             max_exp = np.ceil(np.max(np.log10(values)))
-            bins = np.logspace(min_exp, max_exp, nbins+1)
+            bins = np.logspace(min_exp, max_exp, nbins + 1)
         else:
             values_mean = np.mean(values)
             maxval = np.max(np.abs(values))
             bins = np.linspace(0, maxval, nbins)
-        fig, ax = plt.subplots()
+        _fig, ax = plt.subplots()
         ax.hist(values, bins=bins)
         ax.axvline(values_mean, color='red')
         txt = (
-            f'  mean: {values_mean:.1f}' if log
-            else
-            f'  mean: {values_mean:.4f}')
+            f'  mean: {values_mean:.1e}'
+            if log else
+            f'  mean: {values_mean:.4f}'
+        )
         if unit is not None:
             txt += f' {unit}'
         ax.text(
             values_mean, 0.95, txt, color='red',
             transform=ax.get_xaxis_transform())
         if log:
             ax.set_xscale('log')
@@ -649,33 +863,38 @@
         if self.runid is not None:
             title += f' - runid {self.runid}'
         ax.set_title(title)
         plt.show()
 
 
 def run():
+    """Run the script."""
     args = parse_args()
-    params = Params(args.sqlite_file, args.runid, args.statistics)
+    params = Params(args)
 
     if os.path.exists('problems.txt'):
         _skip_events(params)
     params.filter(
         stamin=args.stamin, stamax=args.stamax,
         magmin=args.magmin, magmax=args.magmax,
-        bsdmin=args.bsdmin, bsdmax=args.bsdmax
+        ssdmin=args.ssdmin, ssdmax=args.ssdmax,
+        sigmaamin=args.sigmaamin, sigmaamax=args.sigmaamax,
     )
+    if len(params.evids) == 0:
+        raise ValueError('No events found')
 
     if args.plot_type == 'fc_mw':
-        params.plot_fc_mw(args.hist, args.fit, args.slope, args.nbins)
+        params.plot_fc_mw(
+            args.hist, args.fit, args.slope, args.nbins, args.wave_type)
     elif args.plot_type == 'Er_mw':
-        params.plot_Er_mw(args.hist, args.fit, args.slope, args.nbins)
-    elif args.plot_type == 'bsd_mw':
-        params.plot_bsd_mw(args.hist, args.fit, args.slope, args.nbins)
+        params.plot_Er_mw(args.hist, args.fit, args.nbins)
+    elif args.plot_type == 'ssd_mw':
+        params.plot_ssd_mw(args.hist, args.fit, args.nbins)
     elif args.plot_type in valid_plot_types:
-        params.plot_hist(args.plot_type, args.nbins)
+        params.plot_hist(args.plot_type, args.nbins, args.wave_type)
 
 
 def _skip_events(params):
     evid_skip = np.loadtxt('problems.txt', usecols=(0,), dtype=str)
     # case in which there is only one evid:
     if not evid_skip.shape:
         evid_skip = evid_skip[None]
@@ -685,14 +904,15 @@
             skip_idx.append(np.where(params.evids == evid)[0][0])
     skipped_evid_str = ' '.join(params.evids[skip_idx])
     print(f'Skipping events: {skipped_evid_str}')
     params.skip_events(skip_idx)
 
 
 def main():
+    """Main function."""
     try:
         run()
     except KeyboardInterrupt:
         sys.exit(0)
     except Exception as msg:
         sys.exit(msg)
```

### Comparing `sourcespec-1.7/sourcespec/savefig.py` & `sourcespec-1.8/sourcespec/savefig.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # -*- coding: utf8 -*-
 # SPDX-License-Identifier: CECILL-2.1
 """
 Save Matplotlib figure. Optimize PNG format using PIL.
 
 :copyright:
-    2022-2023 Claudio Satriano <satriano@ipgp.fr>
+    2022-2024 Claudio Satriano <satriano@ipgp.fr>
 :license:
     CeCILL Free Software License Agreement v2.1
     (http://www.cecill.info/licences.en.html)
 """
 import io
-import PIL
 import logging
 import warnings
+from PIL import Image
 # Reduce logging level for PIL to avoid DEBUG messages
 pil_logger = logging.getLogger('PIL')
 pil_logger.setLevel(logging.WARNING)
 # Reduce logging level for fontTools to avoid DEBUG messages
 mpl_logger = logging.getLogger('fontTools')
 mpl_logger.setLevel(logging.WARNING)
 # Silence PIL warnings about transparency needing RGBA, since we remove the
@@ -26,17 +26,18 @@
 
 def savefig(fig, figfile, fmt, quantize_colors=True, **kwargs):
     """Save Matplotlib figure. Optimize PNG format using PIL."""
     if fmt == 'png':
         buf = io.BytesIO()
         fig.savefig(buf, format='png', **kwargs)
         buf.seek(0)
-        img = PIL.Image.open(buf)
+        img = Image.open(buf)
         if quantize_colors:
-            img = img.convert('P', palette=PIL.Image.ADAPTIVE, colors=256)
+            # pylint: disable=maybe-no-member
+            img = img.convert('P', palette=Image.ADAPTIVE, colors=256)
         else:
             # just remove the alpha channel
             img = img.convert('RGB')
         img.save(figfile, optimize=True)
         img.close()
     else:
         fig.savefig(figfile, **kwargs)
```

### Comparing `sourcespec-1.7/sourcespec/source_spec.py` & `sourcespec-1.8/sourcespec/source_spec.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,24 @@
 :copyright:
     2012 Claudio Satriano <satriano@ipgp.fr>
 
     2013-2014 Claudio Satriano <satriano@ipgp.fr>,
               Emanuela Matrullo <matrullo@geologie.ens.fr>,
               Agnes Chounet <chounet@ipgp.fr>
 
-    2015-2023 Claudio Satriano <satriano@ipgp.fr>
+    2015-2024 Claudio Satriano <satriano@ipgp.fr>
 :license:
     CeCILL Free Software License Agreement v2.1
     (http://www.cecill.info/licences.en.html)
 """
 
 
 def main():
     """Main routine for source_spec."""
+    # pylint: disable=import-outside-toplevel
     # Lazy-import modules for speed
     from sourcespec.ssp_parse_arguments import parse_args
     options = parse_args(progname='source_spec')
 
     # Setup stage
     from sourcespec.ssp_setup import (
         configure, move_outdir, remove_old_outdir, setup_logging,
@@ -31,15 +32,15 @@
     setup_logging(config)
 
     from sourcespec.ssp_read_traces import read_traces
     st = read_traces(config)
 
     # Now that we have an evid, we can rename the outdir and the log file
     move_outdir(config)
-    setup_logging(config, config.hypo.evid)
+    setup_logging(config, config.event.event_id)
     remove_old_outdir(config)
 
     # Save config to out dir
     save_config(config)
 
     # Deconvolve, filter, cut traces:
     from sourcespec.ssp_process_traces import process_traces
@@ -52,30 +53,33 @@
     from sourcespec.ssp_plot_traces import plot_traces
     plot_traces(config, proc_st)
 
     # Spectral inversion
     from sourcespec.ssp_inversion import spectral_inversion
     sspec_output = spectral_inversion(config, spec_st, weight_st)
 
-    # Radiated energy
-    from sourcespec.ssp_radiated_energy import radiated_energy
-    radiated_energy(config, spec_st, specnoise_st, sspec_output)
+    # Radiated energy and apparent stress
+    from sourcespec.ssp_radiated_energy import (
+        radiated_energy_and_apparent_stress)
+    radiated_energy_and_apparent_stress(
+        config, spec_st, specnoise_st, sspec_output)
 
     # Local magnitude
     if config.compute_local_magnitude:
         from sourcespec.ssp_local_magnitude import local_magnitude
         local_magnitude(config, st, proc_st, sspec_output)
 
     # Compute summary statistics from station spectral parameters
     from sourcespec.ssp_summary_statistics import compute_summary_statistics
     compute_summary_statistics(config, sspec_output)
 
     # Save output
-    from sourcespec.ssp_output import write_output
+    from sourcespec.ssp_output import write_output, save_spectra
     write_output(config, sspec_output)
+    save_spectra(config, spec_st)
 
     # Save residuals
     from sourcespec.ssp_residuals import spectral_residuals
     spectral_residuals(config, spec_st, sspec_output)
 
     # Plotting
     from sourcespec.ssp_plot_spectra import plot_spectra
```

### Comparing `sourcespec-1.7/sourcespec/ssp_build_spectra.py` & `sourcespec-1.8/sourcespec/ssp_build_spectra.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,35 +6,38 @@
 :copyright:
     2012 Claudio Satriano <satriano@ipgp.fr>
 
     2013-2014 Claudio Satriano <satriano@ipgp.fr>,
               Emanuela Matrullo <matrullo@geologie.ens.fr>,
               Agnes Chounet <chounet@ipgp.fr>
 
-    2015-2023 Claudio Satriano <satriano@ipgp.fr>
+    2015-2024 Claudio Satriano <satriano@ipgp.fr>
 :license:
     CeCILL Free Software License Agreement v2.1
     (http://www.cecill.info/licences.en.html)
 """
 import logging
-import numpy as np
 import math
+import numpy as np
 from scipy.integrate import cumtrapz
 from scipy.interpolate import interp1d
 from obspy.core import Stream
-from sourcespec import spectrum
+from sourcespec.spectrum import Spectrum, SpectrumStream
 from sourcespec.ssp_setup import ssp_exit
-from sourcespec.ssp_util import smooth, cosine_taper, moment_to_mag, get_vel
+from sourcespec.ssp_util import (
+    smooth, cosine_taper, moment_to_mag, MediumProperties,
+    geom_spread_r_power_n, geom_spread_boatwright, geom_spread_teleseismic)
 from sourcespec.ssp_process_traces import filter_trace
 from sourcespec.ssp_correction import station_correction
 from sourcespec.ssp_radiation_pattern import get_radiation_pattern_coefficient
-logger = logging.getLogger(__name__.split('.')[-1])
+logger = logging.getLogger(__name__.rsplit('.', maxsplit=1)[-1])
 
 
 class SpectrumIgnored(Exception):
+    """Spectrum ignored exception"""
     def __init__(self, message, reason):
         # Call the base class constructor with the parameters it needs
         super().__init__(message)
         # Now for your custom code...
         self.reason = reason
 
 
@@ -63,15 +66,15 @@
         trace.stats.npts -= 1
         filter_trace(config, trace)
 
 
 def _frequency_integrate(config, spec):
     nint = _get_nint(config, spec)
     for _ in range(nint):
-        spec.data /= (2 * math.pi * spec.get_freq())
+        spec.data /= (2 * math.pi * spec.freq)
 
 
 def _cut_spectrum(config, spec):
     # see if there is a station-specific frequency range
     station = spec.stats.station
     try:
         freq1 = float(config[f'freq1_{station}'])
@@ -94,44 +97,40 @@
     Compute the component 'H' from geometric mean of the stream components.
 
     (which can also be all three components)
     """
     if vertical_channel_codes is None:
         vertical_channel_codes = ['Z']
     spec_h = None
-    for spec in spec_st.traces:
+    for spec in spec_st:
         # this avoids taking a component from co-located station:
         # ('code' is band+instrument code)
         channel = spec.stats.channel
         if channel[:-1] != code:
             continue
         # avoid reusing a previous 'H' channel
         if channel[-1] == 'H':
             continue
         # only use transverse component for SH
         if wave_type == 'SH' and channel[-1] != 'T':
             continue
         # do not use transverse component for SV
-        # (only raidal and, optionally, vertical)
         if wave_type == 'SV' and channel[-1] == 'T':
             continue
-        # only use vertical component for P
-        if wave_type == 'P' and channel[-1] not in vertical_channel_codes:
-            continue
         if spec_h is None:
             spec_h = spec.copy()
             spec_h.data = np.power(spec_h.data, 2)
-            spec_h.data_log = np.power(spec_h.data_log, 2)
+            spec_h.data_logspaced = np.power(spec_h.data_logspaced, 2)
             spec_h.stats.channel = f'{code}H'
         else:
             spec_h.data += np.power(spec.data, 2)
-            spec_h.data_log += np.power(spec.data_log, 2)
+            spec_h.data_logspaced += np.power(spec.data_logspaced, 2)
     if spec_h is not None:
         spec_h.data = np.sqrt(spec_h.data)
-        spec_h.data_log = np.sqrt(spec_h.data_log)
+        spec_h.data_logspaced = np.sqrt(spec_h.data_logspaced)
     return spec_h
 
 
 def _check_data_len(config, trace):
     traceId = trace.get_id()
     trace_cut = trace.copy()
     if config.wave_type[0] == 'S':
@@ -143,15 +142,15 @@
     trace_cut.trim(starttime=t1, endtime=t2, pad=True, fill_value=0)
     npts = len(trace_cut.data)
     if npts == 0:
         raise RuntimeError(
             f'{traceId}: No data for the selected cut interval: '
             'skipping trace')
     nzeros = len(np.where(trace_cut.data == 0)[0])
-    if nzeros > npts/4:
+    if nzeros > npts / 4:
         raise RuntimeError(
             f'{traceId}: Signal window is zero for more than 25%: '
             'skipping trace')
 
 
 def _cut_signal_noise(config, trace):
     trace_signal = trace.copy()
@@ -189,236 +188,279 @@
         trace_noise.data = trace_noise.data[:npts]
     else:
         tr_noise_id = trace_noise.get_id()[:-1]
         if config.weighting == 'noise':
             msg = f'{tr_noise_id}: truncating signal window to noise length!'
             trace_signal.data = trace_signal.data[:npts]
             # recompute signal window end time, so that it's plotted correctly
-            _recompute_time_window(trace, config.wave_type[0], npts)
+            _recompute_time_window(
+                trace, config.wave_type[0], npts, keep='start')
         else:
             msg = f'{tr_noise_id}: zero-padding noise window to signal length'
             # Notes:
             # 1. no risk of ringing, as noise has been tapered
             # 2. we use np.pad instead of obspy trim method
             #    to avoid potential rounding errors with start/end times
             # 3. we just pad at the end for simplicity (no changes
             #    in trace headers required) and it is identical to
             #    symmetric padding (tested)
             pad_len = len(trace_signal) - len(trace_noise)
             trace_noise.data = np.pad(trace_noise.data, (0, pad_len))
             # recompute noise window start time, so that it's plotted correctly
-            _recompute_time_window(
-                trace, 'N', len(trace_signal), from_start=True)
+            _recompute_time_window(trace, 'N', len(trace_signal), keep='end')
         logger.warning(msg)
-
-    # ...and zero pad to spectral_win_length
-    if config.spectral_win_length is not None:
-        trace_signal.trim(starttime=t1,
-                          endtime=t1+config.spectral_win_length,
-                          pad=True,
-                          fill_value=0)
-        trace_noise.trim(starttime=noise_t1,
-                         endtime=noise_t1+config.spectral_win_length,
-                         pad=True,
-                         fill_value=0)
-
     return trace_signal, trace_noise
 
 
-def _recompute_time_window(trace, wave_type, npts, from_start=False):
+def _recompute_time_window(trace, wave_type, npts, keep='start'):
     """Recompute start or end time of signal or noise window,
     based on new number of points"""
     length = npts * trace.stats.delta
-    if from_start:
+    if keep == 'end':
         label, _ = trace.stats.arrivals[f'{wave_type}1']
         t1 = trace.stats.arrivals[f'{wave_type}2'][1] - length
         trace.stats.arrivals[f'{wave_type}1'] = (label, t1)
-    else:
+    elif keep == 'start':
         label, _ = trace.stats.arrivals[f'{wave_type}2']
         t2 = trace.stats.arrivals[f'{wave_type}1'][1] + length
         trace.stats.arrivals[f'{wave_type}2'] = (label, t2)
+    else:
+        raise ValueError('keep must be "start" or "end"')
 
 
 def _check_noise_level(trace_signal, trace_noise, config):
     traceId = trace_signal.get_id()
     trace_signal_rms = ((trace_signal.data**2).sum())**0.5
     # Scale trace_noise_rms to length of signal window,
     # based on length of non-zero noise window
     try:
         scale_factor = float(len(trace_signal)) / len(trace_noise.data != 0)
     except ZeroDivisionError:
         scale_factor = 1
     trace_noise_rms = ((trace_noise.data**2 * scale_factor).sum())**0.5
-    if trace_noise_rms/trace_signal_rms < 1e-6 and config.weighting == 'noise':
+    if (
+        trace_noise_rms / trace_signal_rms < 1e-6 and
+        config.weighting == 'noise'
+    ):
         # Skip trace if noise level is too low and if noise weighting is used
         raise RuntimeError(
             f'{traceId}: Noise level is too low or zero: '
             'station will be skipped')
 
 
-def _geom_spread_r_power_n(hypo_dist_in_km, exponent):
-    """rⁿ geometrical spreading coefficient."""
-    dist = hypo_dist_in_km * 1e3
-    return dist**exponent
-
-
-def _geom_spread_boatwright(hypo_dist_in_km, cutoff_dist_in_km, freqs):
-    """"
-    Geometrical spreading coefficient from Boatwright et al. (2002), eq. 8.
-
-    Except that we take the square root of eq. 8, since we correct amplitude
-    and not energy.
-    """
-    dist = hypo_dist_in_km * 1e3
-    cutoff_dist = cutoff_dist_in_km * 1e3
-    if dist <= cutoff_dist:
-        return dist
-    else:
-        return _boatwright_above_cutoff_dist(freqs, cutoff_dist, dist)
-
-
-def _boatwright_above_cutoff_dist(freqs, cutoff_dist, dist):
-    exponent = np.ones_like(freqs)
-    low_freq = freqs <= 0.2
-    mid_freq = np.logical_and(freqs > 0.2, freqs <= 0.25)
-    high_freq = freqs >= 0.25
-    exponent[low_freq] = 0.5
-    exponent[mid_freq] = 0.5 + 2*np.log(5*freqs[mid_freq])
-    exponent[high_freq] = 0.7
-    return cutoff_dist * (dist/cutoff_dist)**exponent
-
-
 def _geometrical_spreading_coefficient(config, spec):
+    """
+    Return the geometrical spreading coefficient for the given spectrum.
+    """
     hypo_dist_in_km = spec.stats.hypo_dist
+    epi_dist_in_km = spec.stats.epi_dist
+    # set geometrical spreading distance to a very large value if it is None
+    geom_spread_min_dist = config.geom_spread_min_teleseismic_distance or 1e99
+    geom_spread_model =\
+        'teleseismic' if epi_dist_in_km >= geom_spread_min_dist\
+        else config.geom_spread_model
+    logger.info(f'{spec.id}: geometrical spreading model: {geom_spread_model}')
+    if geom_spread_model == 'teleseismic':
+        angular_distance = spec.stats.gcarc
+        source_depth_in_km = spec.stats.event.hypocenter.depth.value_in_km
+        station_depth_in_km = -spec.stats.coords.elevation
+        phase = config.wave_type[0]
+        return geom_spread_teleseismic(
+            angular_distance, source_depth_in_km, station_depth_in_km, phase)
     if config.geom_spread_model == 'r_power_n':
         exponent = config.geom_spread_n_exponent
-        return _geom_spread_r_power_n(hypo_dist_in_km, exponent)
-    elif config.geom_spread_model == 'boatwright':
+        return geom_spread_r_power_n(hypo_dist_in_km, exponent)
+    if config.geom_spread_model == 'boatwright':
         cutoff_dist_in_km = config.geom_spread_cutoff_distance
-        return _geom_spread_boatwright(
-            hypo_dist_in_km, cutoff_dist_in_km, spec.get_freq())
+        return geom_spread_boatwright(
+            hypo_dist_in_km, cutoff_dist_in_km, spec.freq)
+    raise ValueError(
+        f'Unknown geometrical spreading model: {config.geom_spread_model}')
 
 
 # store log messages to avoid duplicates
-velocity_log_messages = []
+PROPERTY_LOG_MESSAGES = []
 
 
 def _displacement_to_moment(stats, config):
     """
     Return the coefficient for converting displacement to seismic moment.
 
     From Aki&Richards,1980
     """
     phase = config.wave_type[0]
-    if phase == 'P':
-        v_hypo = config.hypo.vp
-    elif phase == 'S':
-        v_hypo = config.hypo.vs
-    v_station = get_vel(
-        stats.coords.longitude, stats.coords.latitude, -stats.coords.elevation,
-        phase, config)
+    lon = stats.coords.longitude
+    lat = stats.coords.latitude
+    depth = -stats.coords.elevation
+    medium_properties = MediumProperties(lon, lat, depth, config)
+    depth_string = medium_properties.to_string('station depth', depth)
+    v_name = f'v{phase.lower()}'
+    v_source = config.event.hypocenter[v_name]
+    v_source_string = medium_properties.to_string(f'{v_name}_source', v_source)
+    v_station = medium_properties.get(mproperty=v_name, where='stations')
+    stats.v_station = v_station
+    stats.v_station_type = phase
+    v_station_string = medium_properties.to_string(
+        f'{v_name}_station', v_station)
+    rho_source = config.event.hypocenter.rho
+    rho_source_string = medium_properties.to_string('rho_source', rho_source)
+    rho_station = medium_properties.get(mproperty='rho', where='stations')
+    stats.rho_station = rho_station
+    rho_station_string = medium_properties.to_string(
+        'rho_station', rho_station)
     specid = '.'.join((
         stats.network, stats.station, stats.location, stats.channel))
     msg = (
-        f'{specid}: V{phase.lower()}_hypo: {v_hypo:.2f} km/s, '
-        f'V{phase.lower()}_station: {v_station:.2f} km/s')
-    global velocity_log_messages
-    if msg not in velocity_log_messages:
+        f'{specid}: {depth_string}, '
+        f'{v_source_string}, {v_station_string}'
+    )
+    if msg not in PROPERTY_LOG_MESSAGES:
         logger.info(msg)
-        velocity_log_messages.append(msg)
-    v_hypo *= 1000.
+        PROPERTY_LOG_MESSAGES.append(msg)
+    msg = (
+        f'{specid}: {depth_string}, '
+        f'{rho_source_string}, {rho_station_string}'
+    )
+    if msg not in PROPERTY_LOG_MESSAGES:
+        logger.info(msg)
+        PROPERTY_LOG_MESSAGES.append(msg)
+    v_source *= 1000.
     v_station *= 1000.
-    v3 = v_hypo**(5./2) * v_station**(1./2)
-    rp = get_radiation_pattern_coefficient(stats, config)
-    return 4 * math.pi * v3 * config.rho / (2 * rp)
+    v3 = v_source**(5. / 2) * v_station**(1. / 2)
+    rho = rho_source**0.5 * rho_station**0.5
+    fsa = config.free_surface_amplification
+    return 4 * math.pi * v3 * rho / (fsa * stats.radiation_pattern)
 
 
 def _smooth_spectrum(spec, smooth_width_decades=0.2):
     """Smooth spectrum in a log10-freq space."""
     # 1. Generate log10-spaced frequencies
-    freq = spec.get_freq()
+    freq = spec.freq
     _log_freq = np.log10(freq)
     # frequencies in logarithmic spacing
     log_df = _log_freq[-1] - _log_freq[-2]
-    freq_logspace =\
-        10**(np.arange(_log_freq[0], _log_freq[-1]+log_df, log_df))
+    freq_logspaced =\
+        10**(np.arange(_log_freq[0], _log_freq[-1] + log_df, log_df))
     # 2. Reinterpolate data using log10 frequencies
     # make sure that extrapolation does not create negative values
     f = interp1d(freq, spec.data, fill_value='extrapolate')
-    data_logspace = f(freq_logspace)
-    data_logspace[data_logspace <= 0] = np.min(spec.data)
+    data_logspaced = f(freq_logspaced)
+    data_logspaced[data_logspaced <= 0] = np.min(spec.data)
     # 3. Smooth log10-spaced data points
-    npts = max(1, int(round(smooth_width_decades/log_df)))
-    data_logspace = smooth(data_logspace, window_len=npts)
+    npts = max(1, int(round(smooth_width_decades / log_df)))
+    data_logspaced = smooth(data_logspaced, window_len=npts)
     # 4. Reinterpolate to linear frequencies
     # make sure that extrapolation does not create negative values
-    f = interp1d(freq_logspace, data_logspace, fill_value='extrapolate')
+    f = interp1d(freq_logspaced, data_logspaced, fill_value='extrapolate')
     data = f(freq)
     data[data <= 0] = np.min(spec.data)
     spec.data = data
     # 5. Optimize the sampling rate of log spectrum,
     #    based on the width of the smoothing window
     # make sure that extrapolation does not create negative values
-    log_df = smooth_width_decades/5
-    freq_logspace =\
-        10**(np.arange(_log_freq[0], _log_freq[-1]+log_df, log_df))
-    spec.freq_log = freq_logspace
-    data_logspace = f(freq_logspace)
-    data_logspace[data_logspace <= 0] = np.min(spec.data)
-    spec.data_log = data_logspace
+    log_df = smooth_width_decades / 5
+    freq_logspaced =\
+        10**(np.arange(_log_freq[0], _log_freq[-1] + log_df, log_df))
+    spec.freq_logspaced = freq_logspaced
+    data_logspaced = f(freq_logspaced)
+    data_logspaced[data_logspaced <= 0] = np.min(spec.data)
+    spec.data_logspaced = data_logspaced
 
 
 def _build_spectrum(config, trace):
-    spec = spectrum.do_spectrum(trace)
-    stats = trace.stats
-    spec.stats.instrtype = stats.instrtype
-    spec.stats.coords = stats.coords
-    spec.stats.hypo = stats.hypo
-    spec.stats.hypo_dist = stats.hypo_dist
-    spec.stats.epi_dist = stats.epi_dist
-    spec.stats.ignore = stats.ignore
-    spec.stats.travel_times = stats.travel_times
+    spec = Spectrum(obspy_trace=trace)
+    spec.stats.instrtype = trace.stats.instrtype
+    spec.stats.coords = trace.stats.coords
+    spec.stats.event = trace.stats.event
+    spec.stats.hypo_dist = trace.stats.hypo_dist
+    spec.stats.epi_dist = trace.stats.epi_dist
+    spec.stats.gcarc = trace.stats.gcarc
+    spec.stats.azimuth = trace.stats.azimuth
+    spec.stats.travel_times = trace.stats.travel_times
+    spec.stats.takeoff_angles = trace.stats.takeoff_angles
+    spec.stats.ignore = trace.stats.ignore
     # Integrate in frequency domain, if no time-domain
     # integration has been performed
     if not config.time_domain_int:
         _frequency_integrate(config, spec)
     # cut the spectrum
     spec = _cut_spectrum(config, spec)
     # correct geometrical spreading
-    geom_spread = _geometrical_spreading_coefficient(config, spec)
+    try:
+        geom_spread = _geometrical_spreading_coefficient(config, spec)
+    except Exception as e:
+        raise RuntimeError(
+            f'{spec.id}: Error computing geometrical spreading: '
+            f'skipping spectrum\n{str(e)}'
+        ) from e
     spec.data *= geom_spread
+    # store the radiation pattern coefficient in the spectrum stats
+    spec.stats.radiation_pattern =\
+        get_radiation_pattern_coefficient(spec.stats, config)
     # convert to seismic moment
-    coeff = _displacement_to_moment(stats, config)
+    coeff = _displacement_to_moment(spec.stats, config)
     spec.data *= coeff
     # store coeff to correct back data in displacement units
     # for radiated_energy()
-    spec.coeff = coeff
+    spec.stats.coeff = coeff
     # smooth
     _smooth_spectrum(spec, config.spectral_smooth_width_decades)
     return spec
 
 
 def _build_uniform_weight(spec):
     weight = spec.copy()
     weight.snratio = None
     weight.data = np.ones_like(weight.data)
-    weight.data_log = np.ones_like(weight.data_log)
+    weight.data_logspaced = np.ones_like(weight.data_logspaced)
     return weight
 
 
 def _build_weight_from_frequency(config, spec):
     weight = spec.copy()
-    freq = weight.get_freq()
+    freq = weight.freq
     weight.data = np.ones_like(weight.data)
     weight.data[freq <= config.f_weight] = config.weight
     weight.data /= np.max(weight.data)
-    freq_log = weight.freq_log
-    weight.data_log = np.ones_like(weight.data_log)
-    weight.data_log[freq_log <= config.f_weight] = config.weight
-    weight.data_log /= np.max(weight.data_log)
+    freq_logspaced = weight.freq_logspaced
+    weight.data_logspaced = np.ones_like(weight.data_logspaced)
+    weight.data_logspaced[freq_logspaced <= config.f_weight] = config.weight
+    weight.data_logspaced /= np.max(weight.data_logspaced)
+    return weight
+
+
+def _build_weight_from_inv_frequency(spec, power=0.25):
+    """
+    Build spectral weights from inverse frequency (raised to a power < 1)
+    """
+    if power >= 1:
+        raise ValueError('pow must be < 1')
+    # Note: weight.data is used for plotting,
+    #       weight.data_logspaced for actual weighting
+    weight = spec.copy()
+    freq = weight.freq
+    weight.data *= 0
+    # Limit non-zero weights to fmin/fmax from spectral_snratio if available
+    snr_fmin = getattr(spec.stats, 'spectral_snratio_fmin', None)
+    snr_fmax = getattr(spec.stats, 'spectral_snratio_fmax', None)
+    i0 = np.where(freq >= snr_fmin)[0][0] if snr_fmin else 0
+    i1 = np.where(freq <= snr_fmax)[0][-1] if snr_fmax else len(freq) - 1
+    # Build weights as if frequencies always start from 0.25 Hz
+    # to obtain similar curves regardless of fmin
+    # and to avoid too much weight for very low frequencies
+    weight.data[i0: i1 + 1] = 1. / (freq[i0: i1 + 1] - freq[i0] + 0.25)**power
+    weight.data /= np.max(weight.data)
+    freq_logspaced = weight.freq_logspaced
+    weight.data_logspaced *= 0
+    i0 = np.where(freq_logspaced >= snr_fmin)[0][0] if snr_fmin else 0
+    i1 = np.where(freq_logspaced <= snr_fmax)[0][-1] if snr_fmax\
+        else len(freq_logspaced) - 1
+    weight.data_logspaced[i0: i1 + 1] =\
+        1. / (freq_logspaced[i0: i1 + 1] - freq_logspaced[i0] + 0.25)**power
+    weight.data_logspaced /= np.max(weight.data_logspaced)
     return weight
 
 
 def _build_weight_from_ratio(spec, specnoise, smooth_width_decades):
     weight = spec.copy()
     weight.data /= specnoise.data
     # save signal-to-noise ratio before log10, smoothing, and normalization
@@ -427,67 +469,73 @@
     # so let's take log10 of weight
     weight.data = np.log10(weight.data)
     # Weight spectrum is smoothed once more
     _smooth_spectrum(weight, smooth_width_decades)
     weight.data /= np.max(weight.data)
     # slightly taper weight at low frequencies, to avoid overestimating
     # weight at low frequencies, in cases where noise is underestimated
-    cosine_taper(weight.data, weight.stats.delta/4, left_taper=True)
-    # Make sure weight is positive
-    weight.data[weight.data <= 0] = 0.001
+    cosine_taper(
+        weight.data,
+        min(0.25, weight.stats.delta / 4),
+        left_taper=True)
+    # Zero out weight below 0.2 Hz, so that it does not affect the fit
+    weight.data[weight.data <= 0.2] = 1e-9
     return weight
 
 
 def _build_weight_from_noise(config, spec, specnoise):
     if specnoise is None or np.all(specnoise.data == 0):
         spec_id = spec.get_id()[:-1]
         logger.warning(
             f'{spec_id}: No available noise window: '
             'a uniform weight will be applied')
         weight = _build_uniform_weight(spec)
     else:
         weight = _build_weight_from_ratio(
             spec, specnoise, config.spectral_smooth_width_decades)
     # interpolate to log-frequencies
-    f = interp1d(weight.get_freq(), weight.data, fill_value='extrapolate')
-    weight.data_log = f(weight.freq_log)
-    weight.data_log /= np.max(weight.data_log)
+    f = interp1d(weight.freq, weight.data, fill_value='extrapolate')
+    weight.data_logspaced = f(weight.freq_logspaced)
+    weight.data_logspaced /= np.max(weight.data_logspaced)
     # Make sure weight is positive
-    weight.data_log[weight.data_log <= 0] = 0.001
+    weight.data_logspaced[weight.data_logspaced <= 0] = 0.001
     return weight
 
 
 def _build_weight_spectral_stream(config, spec_st, specnoise_st):
     """Build a stream of weights from a stream of spectra and a stream of
     noise spectra."""
-    weight_st = Stream()
+    weight_st = SpectrumStream()
     spec_ids = {sp.id[:-1] for sp in spec_st if not sp.stats.ignore}
     for specid in spec_ids:
         try:
             spec_h = _select_spectra(spec_st, f'{specid}H')[0]
             specnoise_h = _select_spectra(specnoise_st, f'{specid}H')[0]
         except Exception:
             continue
         if config.weighting == 'noise':
             weight = _build_weight_from_noise(config, spec_h, specnoise_h)
         elif config.weighting == 'frequency':
             weight = _build_weight_from_frequency(config, spec_h)
+        elif config.weighting == 'inv_frequency':
+            weight = _build_weight_from_inv_frequency(spec_h)
         elif config.weighting == 'no_weight':
             weight = _build_uniform_weight(spec_h)
         weight_st.append(weight)
     return weight_st
 
 
 def _select_spectra(spec_st, specid):
     """Select spectra from stream, based on specid."""
     network, station, location, channel = specid.split('.')
-    channel = channel + '?'*(3-len(channel))
+    channel = channel + '?' * (3 - len(channel))
     spec_st_sel = spec_st.select(
         network=network, station=station, location=location, channel=channel)
-    spec_st_sel = Stream(sp for sp in spec_st_sel if not sp.stats.ignore)
+    spec_st_sel = SpectrumStream(
+        sp for sp in spec_st_sel if not sp.stats.ignore)
     return spec_st_sel
 
 
 def _build_H(spec_st, specnoise_st=None, vertical_channel_codes=None,
              wave_type='S'):
     """
     Add to spec_st and specnoise_st the "H" component.
@@ -509,52 +557,73 @@
             specnoise_h = _compute_h(
                 specnoise_st_sel, code, vertical_channel_codes, wave_type)
             if specnoise_h is not None:
                 specnoise_st.append(specnoise_h)
 
 
 def _check_spectral_sn_ratio(config, spec, specnoise):
+    spec_id = spec.get_id()
     weight = _build_weight_from_noise(config, spec, specnoise)
+    freqs = weight.freq
     # if no noise window is available, snratio is not computed
     if weight.snratio is None:
         spec.stats.spectral_snratio = None
         return
     if config.spectral_sn_freq_range is not None:
-        sn_fmin, sn_fmax = config.spectral_sn_freq_range
-        freqs = weight.get_freq()
-        idx = np.where((sn_fmin <= freqs)*(freqs <= sn_fmax))
+        sn_fmin, sn_fmax = config.spectral_sn_freq_range[:2]
+        valid_freqs_idx = np.where((sn_fmin <= freqs) * (freqs <= sn_fmax))
+        valid_snratio = weight.snratio[valid_freqs_idx]
     else:
-        idx = range(len(weight.snratio))
-    spectral_snratio =\
-        weight.snratio[idx].sum()/len(weight.snratio[idx])
+        valid_snratio = weight.snratio
+    if len(valid_snratio) == 0:
+        spec.stats.spectral_snratio = np.nan
+        msg = (
+            f'{spec_id}: no valid frequency to compute spectral S/N: '
+            'ignoring spectrum'
+        )
+        reason = 'no valid frequency'
+        raise SpectrumIgnored(msg, reason)
+    spectral_snratio = valid_snratio.mean()
     spec.stats.spectral_snratio = spectral_snratio
-    spec_id = spec.get_id()
-    logger.info(
-        f'{spec_id}: spectral S/N: {spectral_snratio:.2f}')
-    if config.spectral_sn_min:
-        ssnmin = config.spectral_sn_min
-        if spectral_snratio < ssnmin:
-            msg = (
-                f'{spec_id}: spectral S/N smaller than {ssnmin:.2f}: '
-                'ignoring spectrum')
-            reason = 'low spectral S/N'
-            raise SpectrumIgnored(msg, reason)
+    # Save frequency range where SNR > 3 so it can be used for building weights
+    # Note: not sure if we could use config.spectral_sn_min here instead of 3
+    snr_valid_freqs = freqs[weight.snratio >= 3]
+    try:
+        spec.stats.spectral_snratio_fmin = snr_valid_freqs[0]
+        spec.stats.spectral_snratio_fmax = snr_valid_freqs[-1]
+    except IndexError:
+        spec.stats.spectral_snratio_fmin = None
+        spec.stats.spectral_snratio_fmax = None
+    logger.info(f'{spec_id}: average spectral S/N: {spectral_snratio:.2f}')
+    ssnmin = config.spectral_sn_min or -np.inf
+    if spectral_snratio < ssnmin:
+        msg = (
+            f'{spec_id}: spectral S/N smaller than {ssnmin:.2f}: '
+            'ignoring spectrum')
+        reason = 'low spectral S/N'
+        raise SpectrumIgnored(msg, reason)
 
 
-def _ignore_spectrum(msg, trace, spec, specnoise):
+def _ignore_spectrum(msg, spec, specnoise):
     """Ignore spectrum. Set ignore flag and reason."""
     logger.warning(msg)
-    trace.stats.ignore = True
-    trace.stats.ignore_reason = msg.reason
     spec.stats.ignore = True
     spec.stats.ignore_reason = msg.reason
     specnoise.stats.ignore = True
     specnoise.stats.ignore_reason = msg.reason
 
 
+def _ignore_trace(msg, trace):
+    """Ignore trace. Set ignore flag and reason."""
+    # NOTE: no logger.warning here, because it is already done in
+    # _ignore_spectrum()
+    trace.stats.ignore = True
+    trace.stats.ignore_reason = msg.reason
+
+
 def _build_signal_and_noise_streams(config, st):
     """Build signal and noise streams."""
     # remove traces with ignore flag
     traces = Stream([tr for tr in st if not tr.stats.ignore])
     signal_st = Stream()
     noise_st = Stream()
     for trace in sorted(traces, key=lambda tr: tr.id):
@@ -564,78 +633,111 @@
             _check_noise_level(trace_signal, trace_noise, config)
             signal_st.append(trace_signal)
             noise_st.append(trace_noise)
         except RuntimeError as msg:
             # RuntimeError is for skipped traces
             logger.warning(msg)
             continue
-    # trim components of the same instrument to the same number of samples
-    for id in sorted({tr.id[:-1] for tr in signal_st}):
-        st_sel = signal_st.select(id=f'{id}*') + noise_st.select(id=f'{id}*')
+    return signal_st, noise_st
+
+
+def _trim_components(config, signal_st, noise_st, st):
+    """
+    Trim components of the same instrument to the same number of samples.
+
+    Recompute time window of the signal and noise traces for correct plotting.
+    """
+    for traceid in sorted({tr.id[:-1] for tr in signal_st}):
+        st_sel = signal_st.select(id=f'{traceid}*') +\
+            noise_st.select(id=f'{traceid}*')
         all_npts = {tr.stats.npts for tr in st_sel}
         if len(all_npts) == 1:
             continue
         logger.warning(
-            f'{id}: components have different window lengths. '
+            f'{traceid}: components have different window lengths. '
             'Trimming signal and noise windows to the shortest one')
         npts = min(all_npts)
         for tr in st_sel:
             if tr.stats.type == 'signal':
                 tr.data = tr.data[:npts]
             elif tr.stats.type == 'noise':
                 tr.data = tr.data[-npts:]
-        for tr in st.select(id=f'{id}*'):
-            _recompute_time_window(tr, config.wave_type[0], npts)
-            _recompute_time_window(tr, 'N', npts, from_start=True)
-    return signal_st, noise_st
+        for tr in st.select(id=f'{traceid}*'):
+            _recompute_time_window(tr, config.wave_type[0], npts, keep='start')
+            _recompute_time_window(tr, 'N', npts, keep='end')
 
 
-def _build_signal_and_noise_spectral_streams(config, signal_st, noise_st):
-    """Build signal and noise spectral streams."""
-    spec_st = Stream()
-    specnoise_st = Stream()
+def _build_signal_and_noise_spectral_streams(
+        config, signal_st, noise_st, original_st):
+    """
+    Build signal and noise spectral streams.
+
+    Note: original_st is only used to keep track of ignored traces.
+    """
+    spec_st = SpectrumStream()
+    specnoise_st = SpectrumStream()
     for trace_signal in sorted(signal_st, key=lambda tr: tr.id):
         trace_noise = noise_st.select(id=trace_signal.id)[0]
         try:
             spec = _build_spectrum(config, trace_signal)
             specnoise = _build_spectrum(config, trace_noise)
             _check_spectral_sn_ratio(config, spec, specnoise)
         except RuntimeError as msg:
             # RuntimeError is for skipped spectra
             logger.warning(msg)
             continue
         except SpectrumIgnored as msg:
-            _ignore_spectrum(msg, trace_signal, spec, specnoise)
+            _ignore_spectrum(msg, spec, specnoise)
+            trace_original = original_st.select(id=trace_signal.id)[0]
+            _ignore_trace(msg, trace_original)
         spec_st.append(spec)
         specnoise_st.append(specnoise)
     if not spec_st:
         logger.error('No spectra left! Exiting.')
         ssp_exit()
     # build H component
     _build_H(
         spec_st, specnoise_st, config.vertical_channel_codes, config.wave_type)
     # convert the spectral amplitudes to moment magnitude
     for spec in spec_st:
         spec.data_mag = moment_to_mag(spec.data)
-        spec.data_log_mag = moment_to_mag(spec.data_log)
+        spec.data_mag_logspaced = moment_to_mag(spec.data_logspaced)
     for specnoise in specnoise_st:
         specnoise.data_mag = moment_to_mag(specnoise.data)
     # apply station correction if a residual file is specified in config
     spec_st = station_correction(spec_st, config)
     return spec_st, specnoise_st
 
 
+def _zero_pad(config, trace):
+    """Zero-pad trace to spectral_win_length"""
+    spec_win_len = config.spectral_win_length
+    if spec_win_len is None:
+        return
+    wtype = config.wave_type[0]
+    if trace.stats.type == 'signal':
+        t1 = trace.stats.arrivals[f'{wtype}1'][1]
+    elif trace.stats.type == 'noise':
+        t1 = trace.stats.arrivals['N1'][1]
+    trace.trim(starttime=t1, endtime=t1 + spec_win_len, pad=True, fill_value=0)
+
+
 def build_spectra(config, st):
     """
     Build spectra and the ``spec_st`` object.
 
     Computes P- or S-wave (displacement) spectra from
     accelerometers and velocimeters, uncorrected for anelastic attenuation,
     corrected for instrumental constants, normalized by geometrical spreading.
     """
-    logger.info('Building spectra...')
+    wave_type = config.wave_type
+    logger.info(f'Building {wave_type}-wave spectra...')
     signal_st, noise_st = _build_signal_and_noise_streams(config, st)
-    spec_st, specnoise_st = \
-        _build_signal_and_noise_spectral_streams(config, signal_st, noise_st)
+    _trim_components(config, signal_st, noise_st, st)
+    for trace in signal_st + noise_st:
+        _zero_pad(config, trace)
+    spec_st, specnoise_st = _build_signal_and_noise_spectral_streams(
+        config, signal_st, noise_st, st)
     weight_st = _build_weight_spectral_stream(config, spec_st, specnoise_st)
-    logger.info('Building spectra: done')
+    logger.info(f'Building {wave_type}-wave spectra: done')
+    logger.info('---------------------------------------------------')
     return spec_st, specnoise_st, weight_st
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `sourcespec-1.7/sourcespec/ssp_correction.py` & `sourcespec-1.8/sourcespec/ssp_correction.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,62 +3,61 @@
 """
 Spectral station correction calculated from ssp_residuals.
 
 :copyright:
     2013-2014 Claudio Satriano <satriano@ipgp.fr>,
               Agnes Chounet <chounet@ipgp.fr>
 
-    2015-2023 Claudio Satriano <satriano@ipgp.fr>
+    2015-2024 Claudio Satriano <satriano@ipgp.fr>
 :license:
     CeCILL Free Software License Agreement v2.1
     (http://www.cecill.info/licences.en.html)
 """
-import pickle
 import logging
+from scipy.interpolate import interp1d
+from sourcespec.spectrum import read_spectra
 from sourcespec.ssp_util import moment_to_mag, mag_to_moment
 from sourcespec.ssp_setup import ssp_exit
-from scipy.interpolate import interp1d
-logger = logging.getLogger(__name__.split('.')[-1])
+logger = logging.getLogger(__name__.rsplit('.', maxsplit=1)[-1])
 
 
 def station_correction(spec_st, config):
     """
     Correct spectra using station-average residuals.
 
     Residuals are obtained from a previous run.
     """
     res_filepath = config.residuals_filepath
     if res_filepath is None:
         return spec_st
     try:
-        with open(res_filepath, 'rb') as fp:
-            residual = pickle.load(fp)
+        residual = read_spectra(res_filepath)
     except Exception as msg:
         logger.error(msg)
         ssp_exit(1)
 
-    H_specs = [spec for spec in spec_st if (spec.stats.channel[-1] == 'H')]
+    H_specs = [spec for spec in spec_st if spec.stats.channel[-1] == 'H']
     for spec in H_specs:
         try:
             corr = residual.select(id=spec.id)[0]
         except IndexError:
             continue
-        freq = spec.get_freq()
+        freq = spec.freq
         fmin = freq.min()
         fmax = freq.max()
         corr = corr.slice(fmin, fmax)
         corr.data_mag = moment_to_mag(corr.data)
         spec_corr = spec.copy()
         # uncorrected spectrum will have component name 'h'
         spec.stats.channel = f'{spec.stats.channel[:-1]}h'
         spec_corr.data_mag -= corr.data_mag
-        # interpolate the corrected data_mag to log frequencies
+        # interpolate the corrected data_mag to logspaced frequencies
         f = interp1d(freq, spec_corr.data_mag, fill_value='extrapolate')
-        spec_corr.data_log_mag = f(spec_corr.freq_log)
+        spec_corr.data_mag_logspaced = f(spec_corr.freq_logspaced)
         # convert mag to moment
         spec_corr.data = mag_to_moment(spec_corr.data_mag)
-        spec_corr.data_log = mag_to_moment(spec_corr.data_log_mag)
+        spec_corr.data_logspaced = mag_to_moment(spec_corr.data_mag_logspaced)
         spec_st.append(spec_corr)
         logger.info(
             f'{spec_corr.id} corrected, frequency range is: '
             f'{fmin:.2f} {fmax:.2f} Hz')
     return spec_st
```

### Comparing `sourcespec-1.7/sourcespec/ssp_data_types.py` & `sourcespec-1.8/sourcespec/ssp_data_types.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # -*- coding: utf8 -*-
 # SPDX-License-Identifier: CECILL-2.1
 """
 Classes for spectral inversion routines.
 
 :copyright:
-    2017-2023 Claudio Satriano <satriano@ipgp.fr>
+    2017-2024 Claudio Satriano <satriano@ipgp.fr>
 :license:
     CeCILL Free Software License Agreement v2.1
     (http://www.cecill.info/licences.en.html)
 """
 import logging
-import numpy as np
 from collections import OrderedDict
-logger = logging.getLogger(__name__.split('.')[-1])
+import numpy as np
+logger = logging.getLogger(__name__.rsplit('.', maxsplit=1)[-1])
 
 
 class InitialValues():
     """Initial values for spectral inversion."""
 
     def __init__(self, Mw_0=None, fc_0=None, t_star_0=None):
         self.Mw_0 = Mw_0
@@ -28,18 +28,19 @@
         return (
             f'Mw_0: {round(self.Mw_0, 4)}; '
             f'fc_0: {round(self.fc_0, 4)}; '
             f't_star_0: {round(self.t_star_0, 4)}'
         )
 
     def get_params0(self):
+        """Get initial values as a tuple."""
         return (self.Mw_0, self.fc_0, self.t_star_0)
 
 
-class Bounds(object):
+class Bounds():
     """Bounds for bounded spectral inversion."""
 
     def __init__(self, config, spec, initial_values):
         self.config = config
         self.spec = spec
         self.hd = spec.stats.hypo_dist
         self.ini_values = initial_values
@@ -50,29 +51,30 @@
                 self._check_minmax(config.t_star_min_max)
         else:
             self.t_star_min, self.t_star_max = self._Qo_to_t_star()
         self._fix_initial_values_t_star()
 
     def __str__(self):
         """String representation."""
+        # pylint: disable=consider-using-f-string
         s = 'Mw: {}, {}; '.format(
             *[round(x, 4) if x is not None else x for x in self.bounds[0]])
         s += 'fc: {}, {}; '.format(
             *[round(x, 4) if x is not None else x for x in self.bounds[1]])
         s += 't_star: {}, {}'.format(
             *[round(x, 4) if x is not None else x for x in self.bounds[2]])
         return s
 
     def _set_fc_min_max(self, config):
         fc_0 = self.ini_values.fc_0
         if config.fc_min_max is None:
             # If no bound is given, set it to fc_0 +/- a decade
             scale = 10.  # a decade
-            self.fc_min = fc_0/scale
-            self.fc_max = fc_0*scale
+            self.fc_min = fc_0 / scale
+            self.fc_max = fc_0 * scale
         else:
             self.fc_min, self.fc_max = config.fc_min_max
         if self.fc_min > fc_0:
             logger.warning(
                 f'{self.spec.id} {self.spec.stats.instrtype}: '
                 f'fc_min ({self.fc_min}) larger than '
                 f'fc_0 ({round(fc_0, 4)}). '
@@ -90,19 +92,19 @@
 
     def _check_minmax(self, minmax):
         return (None, None) if minmax is None else minmax
 
     def _Qo_to_t_star(self):
         phase = self.config.wave_type[0]
         travel_time = self.spec.stats.travel_times[phase]
-        t_star_bounds = travel_time/self.config.Qo_min_max
+        t_star_bounds = travel_time / np.array(self.config.Qo_min_max)
         return sorted(t_star_bounds)
 
     def _fix_initial_values_t_star(self):
-        if self.ini_values.t_star_0 is not None:
+        if self.ini_values.t_star_0 is None:
             return
         if None in self.bounds[2]:
             return
         if self.t_star_min < self.ini_values.t_star_0 < self.t_star_max:
             return
         t_star_0 = (self.t_star_max + self.t_star_min) / 2.
         logger.warning(
@@ -164,110 +166,96 @@
     def __setattr__(self, attr, value):
         self[attr] = value
 
 
 class SpectralParameter(OrderedAttribDict):
     """A spectral parameter measured at one station."""
 
-    def __init__(self, id, name=None, units=None, value=None, uncertainty=None,
+    def __init__(self, param_id, name=None, units=None, value=None,
+                 uncertainty=None,
                  lower_uncertainty=None, upper_uncertainty=None,
-                 confidence_level=None, format=None):
-        self._id = id
-        self._format = format
+                 confidence_level=None, format_spec=None):
+        self.param_id = param_id
+        self._format_spec = format_spec
         self.name = name
         self.units = units
         self.value = value
         self.uncertainty = uncertainty
         if (lower_uncertainty is not None and
                 lower_uncertainty == upper_uncertainty):
             self.uncertainty = lower_uncertainty
             self.lower_uncertainty = self.upper_uncertainty = None
         else:
             self.lower_uncertainty = lower_uncertainty
             self.upper_uncertainty = upper_uncertainty
         self.confidence_level = confidence_level
         self.outlier = False
 
-    def value_uncertainty(self):
-        """Return value and uncertainty as 3-element tuple."""
+    def compact_uncertainty(self):
+        """Return uncertainty in a compact form."""
         if self.lower_uncertainty is not None:
-            uncertainty = (self.lower_uncertainty, self.upper_uncertainty)
-        else:
-            uncertainty = (self.uncertainty, self.uncertainty)
-        return (self.value, *uncertainty)
+            return (self.lower_uncertainty, self.upper_uncertainty)
+        if self.uncertainty is not None:
+            return (self.uncertainty, self.uncertainty)
+        return (np.nan, np.nan)
 
 
 class StationParameters(OrderedAttribDict):
     """
     The parameters describing a given station (e.g., its id and location) and
     the spectral parameters measured at that station.
 
     Spectral parameters are provided as attributes, using SpectralParameter()
     objects.
     """
 
-    def __init__(self, id, instrument_type=None, latitude=None, longitude=None,
+    def __init__(self, station_id, instrument_type=None,
+                 latitude=None, longitude=None,
                  hypo_dist_in_km=None, epi_dist_in_km=None, azimuth=None):
-        self._id = id
+        self.station_id = station_id
         self.instrument_type = instrument_type
         self.latitude = latitude
         self.longitude = longitude
         self.hypo_dist_in_km = hypo_dist_in_km
         self.epi_dist_in_km = epi_dist_in_km
         self.azimuth = azimuth
-        self._params = {}
-        self._params_err = {}
-        self._is_outlier = {}
-
-    def __setattr__(self, attr, value):
-        if isinstance(value, SpectralParameter):
-            parname = attr
-            par = value
-            self._params[parname] = par.value
-            if par.uncertainty is not None:
-                self._params_err[parname] = (par.uncertainty, par.uncertainty)
-            else:
-                self._params_err[parname] = (
-                    par.lower_uncertainty, par.upper_uncertainty
-                )
-            self._is_outlier[parname] = par.outlier
-        self[attr] = value
+        self.Mw = None
+        self.fc = None
+        self.t_star = None
+        self.Mo = None
+        self.radius = None
+        self.ssd = None
+        self.Qo = None
+        self.Er = None
+        self.sigma_a = None
+        self.Ml = None
 
-    def rebuild_dictionaries(self):
-        for key, value in self.items():
-            if not isinstance(value, SpectralParameter):
-                continue
-            parname = key
-            par = value
-            self._params[parname] = par.value
-            if par.uncertainty is not None:
-                self._params_err[parname] = (par.uncertainty, par.uncertainty)
-            elif par.lower_uncertainty is not None:
-                self._params_err[parname] = (
-                    par.lower_uncertainty, par.upper_uncertainty
-                )
-            else:
-                self._params_err[parname] = (np.nan, np.nan)
-            self._is_outlier[parname] = par.outlier
+    def get_spectral_parameters(self):
+        """Return a dictionary of spectral parameters."""
+        return {
+            key: value
+            for key, value in self.items()
+            if isinstance(value, SpectralParameter)
+        }
 
 
 class SummaryStatistics(OrderedAttribDict):
     """
     A summary statistics (e.g., mean, weighted_mean, percentile), along with
     its uncertainty.
     """
 
-    def __init__(self, type, value=None, uncertainty=None,
+    def __init__(self, stat_type, value=None, uncertainty=None,
                  lower_uncertainty=None, upper_uncertainty=None,
                  confidence_level=None, lower_percentage=None,
                  mid_percentage=None, upper_percentage=None,
                  nobs=None, message=None,
-                 format=None):
+                 format_spec=None):
         # type of statistics: e.g., mean, median
-        self._type = type
+        self._stat_type = stat_type
         self.value = value
         self.uncertainty = uncertainty
         if (lower_uncertainty is not None and
                 lower_uncertainty == upper_uncertainty):
             self.uncertainty = lower_uncertainty
             self.lower_uncertainty = self.upper_uncertainty = None
         else:
@@ -275,90 +263,102 @@
             self.upper_uncertainty = upper_uncertainty
         self.confidence_level = confidence_level
         self.lower_percentage = lower_percentage
         self.mid_percentage = mid_percentage
         self.upper_percentage = upper_percentage
         self.nobs = nobs
         self.message = message
-        self._format = format
+        self._format_spec = format_spec
 
     def compact_uncertainty(self):
         """Return uncertainty in a compact form."""
         if self.lower_uncertainty is not None:
             return (self.lower_uncertainty, self.upper_uncertainty)
-        else:
+        if self.uncertainty is not None:
             return (self.uncertainty, self.uncertainty)
+        return (np.nan, np.nan)
 
 
 class SummarySpectralParameter(OrderedAttribDict):
     """
     A summary spectral parameter comprising one ore more summary statistics.
     """
 
-    def __init__(self, id, name=None, units=None, format=None):
-        self._id = id
+    def __init__(self, param_id, name=None, units=None, format_spec=None):
+        self.param_id = param_id
         self.name = name
         self.units = units
         # number formatting string
-        self._format = format
+        self._format_spec = format_spec
 
     def __setattr__(self, attr, value):
         if isinstance(value, SummaryStatistics):
-            value._format = self._format
+            value._format_spec = self._format_spec
         self[attr] = value
 
 
 class SourceSpecOutput(OrderedAttribDict):
     """The output of SourceSpec."""
 
     def __init__(self):
         self.run_info = OrderedAttribDict()
         self.event_info = OrderedAttribDict()
         self.inversion_info = OrderedAttribDict()
         self.summary_spectral_parameters = OrderedAttribDict()
         self.station_parameters = OrderedAttribDict()
+        # comments for each section
+        # do not remove the underscore from the attribute name!
         self._comments = {
             'begin': 'SourceSpec output in YAML format',
             'run_info': 'Information on the SourceSpec run',
             'event_info': 'Information on the event',
             'inversion_info': 'Information on the inversion procedure',
             'summary_spectral_parameters':
                 'Summary spectral parameters, computed using different '
                 'statistics',
             'station_parameters':
                 'Parameters describing each station and spectral '
                 'measurements\nperformed at that station'
         }
 
     def value_array(self, key, filter_outliers=False):
+        """Return an array of values for the given key."""
         vals = np.array([
-            x._params.get(key, np.nan)
-            for x in self.station_parameters.values()
+            stat_par[key].value
+            if key in stat_par and stat_par[key] is not None
+            else np.nan
+            for stat_par in self.station_parameters.values()
         ])
         if filter_outliers:
             outliers = self.outlier_array(key)
             vals = vals[~outliers]
         return vals
 
     def error_array(self, key, filter_outliers=False):
+        """Return an array of errors (two columns) for the given key."""
         errs = np.array([
-            x._params_err.get(key, np.nan)
-            for x in self.station_parameters.values()
+            stat_par[key].compact_uncertainty()
+            if key in stat_par and stat_par[key] is not None
+            else (np.nan, np.nan)
+            for stat_par in self.station_parameters.values()
         ])
         if filter_outliers:
             outliers = self.outlier_array(key)
             errs = errs[~outliers]
         return errs
 
     def outlier_array(self, key):
+        """Return an array of outliers for the given key."""
         return np.array(
             [
+                stat_par[key].outlier
+                if key in stat_par
                 # if we cannot find the given key, we assume outlier=True
-                x._is_outlier.get(key, True)
-                for x in self.station_parameters.values()
+                else True
+                for stat_par in self.station_parameters.values()
             ]
         )
 
     def find_outliers(self, key, n):
         """
         Find outliers using the IQR method.
 
@@ -371,28 +371,34 @@
             outlier         <----------->            outliers
                                  IQR
 
         If ``n`` is ``None``, then the above check is skipped.
         ``Nan`` and ``inf`` values are also marked as outliers.
         """
         values = self.value_array(key)
-        station_ids = np.array(list(self.station_parameters.keys()))
         naninf = np.logical_or(np.isnan(values), np.isinf(values))
         _values = values[~naninf]
-        if n is not None and len(_values) > 0:
+        # cases for which outliers cannot be computed
+        if (
+            n is None or
+            len(_values) == 0 or
+            # _values are all the same within 0.01 %
+            np.ptp(_values) < 0.0001 * np.mean(_values)
+        ):
+            outliers = naninf
+        else:
             Q1, _, Q3 = np.percentile(_values, [25, 50, 75])
-            IQR = Q3-Q1
-            outliers = np.logical_or(values < Q1 - n*IQR, values > Q3 + n*IQR)
+            IQR = Q3 - Q1
+            outliers = np.logical_or(
+                values < Q1 - n * IQR, values > Q3 + n * IQR)
             outliers = np.logical_or(outliers, naninf)
-        else:
-            outliers = naninf
+        station_ids = np.array(list(self.station_parameters.keys()))
         for stat_id, outl in zip(station_ids, outliers):
             stat_par = self.station_parameters[stat_id]
             stat_par[key].outlier = outl
-            stat_par.rebuild_dictionaries()
 
     def mean_values(self):
         """Return a dictionary of mean values."""
         return {
             parname: par.mean.value
             for parname, par in self.summary_spectral_parameters.items()
             if isinstance(par, SummarySpectralParameter)
@@ -404,14 +410,25 @@
         return {
             parname: par.mean.compact_uncertainty()
             for parname, par in self.summary_spectral_parameters.items()
             if isinstance(par, SummarySpectralParameter)
             and 'mean' in par
         }
 
+    def mean_nobs(self):
+        """
+        Return a dictionary of number of observations used for computing mean.
+        """
+        return {
+            parname: par.mean.nobs
+            for parname, par in self.summary_spectral_parameters.items()
+            if isinstance(par, SummarySpectralParameter)
+            and 'mean' in par
+        }
+
     def weighted_mean_values(self):
         """Return a dictionary of weighted mean values."""
         return {
             parname: par.weighted_mean.value
             for parname, par in self.summary_spectral_parameters.items()
             if isinstance(par, SummarySpectralParameter)
             and 'weighted_mean' in par
@@ -422,14 +439,26 @@
         return {
             parname: par.weighted_mean.compact_uncertainty()
             for parname, par in self.summary_spectral_parameters.items()
             if isinstance(par, SummarySpectralParameter)
             and 'weighted_mean' in par
         }
 
+    def weighted_mean_nobs(self):
+        """
+        Return a dictionary of number of observations used for computing
+        weighted mean.
+        """
+        return {
+            parname: par.weighted_mean.nobs
+            for parname, par in self.summary_spectral_parameters.items()
+            if isinstance(par, SummarySpectralParameter)
+            and 'weighted_mean' in par
+        }
+
     def percentiles_values(self):
         """Return a dictionary of percentile values."""
         return {
             parname: par.percentiles.value
             for parname, par in self.summary_spectral_parameters.items()
             if isinstance(par, SummarySpectralParameter)
             and 'percentiles' in par
@@ -440,45 +469,55 @@
         return {
             parname: par.percentiles.compact_uncertainty()
             for parname, par in self.summary_spectral_parameters.items()
             if isinstance(par, SummarySpectralParameter)
             and 'percentiles' in par
         }
 
+    def percentiles_nobs(self):
+        """
+        Return a dictionary of number of observations used for computing
+        percentiles.
+        """
+        return {
+            parname: par.percentiles.nobs
+            for parname, par in self.summary_spectral_parameters.items()
+            if isinstance(par, SummarySpectralParameter)
+            and 'percentiles' in par
+        }
+
     def reference_values(self):
         """Return a dictionary of reference values."""
         try:
             ref_stat = self.summary_spectral_parameters.reference_statistics
         except KeyError as e:
             raise ValueError('No reference statistics defined') from e
         if ref_stat == 'mean':
             return self.mean_values()
-        elif ref_stat == 'percentiles':
+        if ref_stat == 'percentiles':
             return self.percentiles_values()
-        elif ref_stat == 'weighted_mean':
+        if ref_stat == 'weighted_mean':
             return self.weighted_mean_values()
-        else:
-            msg = f'Invalid reference statistics: {ref_stat}'
-            raise ValueError(msg)
+        msg = f'Invalid reference statistics: {ref_stat}'
+        raise ValueError(msg)
 
     def reference_uncertainties(self):
         """Return a dictionary of reference uncertainties."""
         try:
             ref_stat = self.summary_spectral_parameters.reference_statistics
         except KeyError as e:
             raise ValueError('No reference statistics defined') from e
         if ref_stat == 'mean':
             return self.mean_uncertainties()
-        elif ref_stat == 'percentiles':
+        if ref_stat == 'percentiles':
             return self.percentiles_uncertainties()
-        elif ref_stat == 'weighted_mean':
+        if ref_stat == 'weighted_mean':
             return self.weighted_mean_uncertainties()
-        else:
-            msg = f'Invalid reference statistics: {ref_stat}'
-            raise ValueError(msg)
+        msg = f'Invalid reference statistics: {ref_stat}'
+        raise ValueError(msg)
 
     def reference_summary_parameters(self):
         """
         Return a dictionary of reference summary parameters,
         each being a SummaryStatistics() object.
         """
         try:
```

### Comparing `sourcespec-1.7/sourcespec/ssp_grid_sampling.py` & `sourcespec-1.8/sourcespec/ssp_grid_sampling.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,56 +4,57 @@
 """
 A class for sampling a parameter space over a grid.
 
 Sampling can be performed by several approaches.
 The class provides optimal solutions, uncertainties and plotting methods.
 
 :copyright:
-    2022-2023 Claudio Satriano <satriano@ipgp.fr>
+    2022-2024 Claudio Satriano <satriano@ipgp.fr>
 :license:
     CeCILL Free Software License Agreement v2.1
     (http://www.cecill.info/licences.en.html)
 """
 import os
+import warnings
+import logging
 import numpy as np
-from sourcespec.kdtree import KDTree
-from sourcespec.savefig import savefig
-from scipy.signal import peak_widths
+from scipy.signal import peak_widths as find_peak_widths
+# pylint: disable=no-name-in-module
 from scipy.signal._peak_finding_utils import PeakPropertyWarning
 import matplotlib.pyplot as plt
-import warnings
-import logging
-logger = logging.getLogger(__name__.split('.')[-1])
+from sourcespec.kdtree import KDTree
+from sourcespec.savefig import savefig
+logger = logging.getLogger(__name__.rsplit('.', maxsplit=1)[-1])
 
 
-def peak_width(x, peak_idx, rel_height, negative=False):
+def find_peak_width(x, peak_idx, rel_height, negative=False):
     """
     Find width of a single peak at a given relative height.
 
     rel_height: float parameter between 0 and 1
                 0 means the base of the curve and 1 the peak value
                 (Note: this is the opposite of scipy.peak_widths)
     """
     if rel_height < 0 or rel_height > 1:
         msg = 'rel_height must be between 0 and 1'
         raise ValueError(msg)
     sign = -1 if negative else 1
     with warnings.catch_warnings():
         warnings.filterwarnings('ignore', category=PeakPropertyWarning)
-        _, width_height, idx_left, idx_right = peak_widths(
-            sign*x, [peak_idx, ], 1-rel_height)
+        _, width_height, idx_left, idx_right =\
+            find_peak_widths(sign * x, [peak_idx, ], 1 - rel_height)
     idx_left = int(idx_left)
     idx_right = int(idx_right)
-    width_height = sign*width_height[0]
+    width_height = sign * width_height[0]
     # fall back approach if the previous one fails
     if idx_left == idx_right:
         height = x.max() - x.min()
         if not negative:
             rel_height = 1 - rel_height
-        width_height = x.max() - rel_height*height
+        width_height = x.max() - rel_height * height
         # Search for the indexes of the misfit curve points which are
         # closest to width_height, on the left and on the right
         #   Note: This assumes that the misfit function is monotonic.
         #         A safer but less precise approach is the commented one,
         #         based on "iii"
         # iii = np.where(np.isclose(x, width_height, rtol=0.1))
         try:
@@ -106,42 +107,44 @@
         self.truebounds = []
         for bds, ns, mode in zip(self.bounds, self.nsteps, self.sampling_mode):
             if None in bds:
                 msg = 'All parameters must be bounded for grid sampling'
                 raise RuntimeError(msg)
             if mode == 'log':
                 if bds[0] == 0:
-                    bds = (bds[1]/ns, bds[1])
+                    bds = (bds[1] / ns, bds[1])
                 bds = tuple(np.log10(bds))
             self.truebounds.append(bds)
         self.kdt = None
+        self.extent = None
 
     @property
     def values(self):
+        """Return a meshgrid of parameter values."""
         if self._values is not None:
             return self._values
         values = []
         for bds, ns, mode in zip(
                 self.truebounds, self.nsteps, self.sampling_mode):
             if mode == 'log':
                 values.append(np.logspace(*bds, ns))
             else:
                 values.append(np.linspace(*bds, ns))
         self._values = np.meshgrid(*values, indexing='ij')
         return self._values
 
     @property
     def min_idx(self):
+        """Find the index of the minimum of the misfit function."""
         if self.misfit is None:
             return None
         if self._min_idx is None:
             return np.unravel_index(
                 np.nanargmin(self.misfit), self.misfit.shape)
-        else:
-            return self._min_idx
+        return self._min_idx
 
     @property
     def values_1d(self):
         """Extract a 1D array of parameter values along one dimension."""
         # same thing for values: we extract a 1d array of values along dim
         ndim = len(self.values)
         values_1d = []
@@ -175,41 +178,43 @@
             mm = mm[idx]
             cond_misfit.append(mm)
         self._conditional_misfit = tuple(cond_misfit)
         return self._conditional_misfit
 
     @property
     def params_opt(self):
+        """Return optimal parameters."""
         if self.misfit is None:
             return None
         return np.array([v[self.min_idx] for v in self.values])
 
     @property
     def params_err(self):
+        """Return optimal parameters uncertainties."""
         if self.misfit is None:
             return None
         error = []
         for p, w in zip(self.params_opt, self.conditional_peak_widths):
-            err_left = p-w[1]
-            err_right = w[2]-p
+            err_left = p - w[1]
+            err_right = w[2] - p
             error.append((err_left, err_right))
         return tuple(error)
 
     @property
     def conditional_peak_widths(self):
         """Find width of conditional misfit around its minimum."""
         if self.misfit is None:
             return None
         if self._conditional_peak_widths is not None:
             return self._conditional_peak_widths
         peak_widths = []
         rel_height = np.exp(-0.5)  # height of a gaussian for x=sigma
         for mm, idx, values in zip(
                 self.conditional_misfit, self.min_idx, self.values_1d):
-            width_height, idx_left, idx_right = peak_width(
+            width_height, idx_left, idx_right = find_peak_width(
                 mm, idx, rel_height, negative=True)
             peak_widths.append(
                 (width_height, values[idx_left], values[idx_right]))
         self._conditional_peak_widths = tuple(peak_widths)
         return self._conditional_peak_widths
 
     def grid_search(self):
@@ -217,14 +222,15 @@
         # small helper function to transform args into a tuple
         def mf(*args):
             return self.misfit_func(args)
         mf = np.vectorize(mf)
         self.misfit = mf(*self.values)
 
     def kdtree_search(self):
+        """Sample the misfit function using kdtree search."""
         # small helper function to transform misfit to pdf and manage logscale
         def mf(args):
             newargs = []
             for a, mode in zip(args, self.sampling_mode):
                 if mode == 'log':
                     a = 10**a
                 newargs.append(a)
@@ -235,15 +241,15 @@
         while kdt.ncells <= np.prod(maxdiv):
             oldn = kdt.ncells
             kdt.divide()
             if kdt.ncells == oldn:
                 break
         deltas = []
         for bds, ns in zip(self.truebounds, self.nsteps):
-            deltas.append((bds[1] - bds[0])/ns)
+            deltas.append((bds[1] - bds[0]) / ns)
         pdf, extent = kdt.get_pdf(deltas)
         self.kdt = kdt
         self.misfit = -np.log(pdf)
         self.nsteps = self.misfit.shape
         self.extent = extent
 
     def plot_conditional_misfit(self, config, label):
@@ -268,14 +274,22 @@
                 popt, 0.9, text, color='red', ha=ha, va='top',
                 transform=ax[dim].get_xaxis_transform())
             if self.sampling_mode[dim] == 'log':
                 ax[dim].set_xscale('log')
             xlabel = self.params_name[dim]
             if self.params_unit[dim]:
                 xlabel += f' ({self.params_unit[dim]})'
+            # add some margin if values are too close
+            tolerance = 1e-3
+            if np.isclose(v.min(), v.max(), rtol=tolerance):
+                vmean = np.mean(v)
+                vmin = vmean - tolerance * np.abs(vmean)
+                vmax = vmean + tolerance * np.abs(vmean)
+                ax[dim].set_xlim(vmin, vmax)
+                ax[dim].set_ylim(0, 1)
             ax[dim].set_xlabel(xlabel)
             ax[dim].set_ylabel('misfit')
         ax[0].set_title(label)
         plt.tight_layout()
         figfile_base = self._get_figfile_base(config)
         figfile_base += f".cond_misfit_{label.replace(' ', '_')}."
         fmt = config.plot_save_format
@@ -323,19 +337,30 @@
         params_opt = np.take(params_opt_all, plot_par_idx)
         params_name = np.take(self.params_name, plot_par_idx)
         params_unit = np.take(self.params_unit, plot_par_idx)
         sampling_mode = np.take(self.sampling_mode, plot_par_idx)
         fig, ax = plt.subplots(1, 1, figsize=(5, 4), dpi=300)
         # imshow: saturate scale at 2 times the minimum
         mmap = ax.imshow(
-            mm, vmax=2*mm.min(), origin='lower', cmap='viridis',
+            mm, vmax=2 * mm.min(), origin='lower', cmap='viridis',
             extent=extent, aspect='auto'
         )
-        ax.set_xlim(extent[0], extent[1])
-        ax.set_ylim(extent[2], extent[3])
+        xmin, xmax, ymin, ymax = extent
+        # add some margin if values are too close
+        tolerance = 1e-3
+        if np.isclose(xmin, xmax, rtol=tolerance):
+            xmean = np.mean((xmin, xmax))
+            xmin = xmean - tolerance * np.abs(xmean)
+            xmax = xmean + tolerance * np.abs(xmean)
+        if np.isclose(ymin, ymax, rtol=tolerance):
+            ymean = np.mean((ymin, ymax))
+            ymin = ymean - tolerance * np.abs(ymean)
+            ymax = ymean + tolerance * np.abs(ymean)
+        ax.set_xlim(xmin, xmax)
+        ax.set_ylim(ymin, ymax)
         if self.kdt is not None:
             self._plot_kdtree_structure(ax, plot_par_idx, params_opt_all)
         ax.scatter(*params_opt, facecolors='none', edgecolors='w')
         ax.set_title(label)
         xlabel = params_name[0]
         if params_unit[0]:
             xlabel += f' ({params_unit[0]})'
@@ -368,15 +393,15 @@
             logger.info(f'{label}: conditional misfit map saved to: {figfile}')
             config.figures[f'misfit_{params_string}'].append(figfile)
 
     def _get_figfile_base(self, config):
         outdir = os.path.join(config.options.outdir, 'misfit')
         if not os.path.exists(outdir):
             os.makedirs(outdir)
-        evid = config.hypo.evid
+        evid = config.event.event_id
         return os.path.join(outdir, evid)
 
     def _set_ylogscale(self, ax, extent, ylabel):
         # the grid is plotted by imshow() in linear scale,
         # so we create a fake yaxis with logscale
         ax.yaxis.set_visible(False)
         ax2 = ax.twinx()
```

### Comparing `sourcespec-1.7/sourcespec/ssp_html_report.py` & `sourcespec-1.8/sourcespec/ssp_html_report.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # -*- coding: utf-8 -*-
 # SPDX-License-Identifier: CECILL-2.1
 """
 Generate an HTML report for source_spec.
 
 :copyright:
-    2021-2023 Claudio Satriano <satriano@ipgp.fr>
+    2021-2024 Claudio Satriano <satriano@ipgp.fr>
 :license:
     CeCILL Free Software License Agreement v2.1
     (http://www.cecill.info/licences.en.html)
 """
 import os
 import logging
 import shutil
 import re
 import contextlib
-import numpy as np
 from urllib.parse import urlparse
+import numpy as np
 from sourcespec._version import get_versions
 from sourcespec.ssp_data_types import SpectralParameter
-logger = logging.getLogger(__name__.split('.')[-1])
+logger = logging.getLogger(__name__.rsplit('.', maxsplit=1)[-1])
 VALID_FIGURE_FORMATS = ('.png', '.svg')
 
 
 def _multireplace(string, replacements, ignore_case=False):
     """
     Given a string and a replacement map, it returns the replaced string.
 
@@ -93,18 +93,18 @@
         agency_logo_path = bname
     return agency_logo_path
 
 
 def _agency_logo(config):
     agency_logo_path = _agency_logo_path(config)
     if agency_logo_path is None:
-        return ""
+        return ''
     agency_logo_img = f'<img class="logo" src="{agency_logo_path}"/>'
-    indent5 = 5*'  '
-    indent6 = 6*'  '
+    indent5 = 5 * '  '
+    indent6 = 6 * '  '
     if config.agency_url is not None:
         agency_logo_html = (
             f'{indent5}<a href="{config.agency_url}" target="_blank">\n'
             f'{indent6}{agency_logo_img}\n'
             f'{indent5}</a>'
         )
     else:
@@ -117,15 +117,15 @@
     cdn_baseurl = 'https://cdn.jsdelivr.net/gh/SeismicSource/sourcespec@1.6'
     return f'{cdn_baseurl}/imgs/SourceSpec_logo.svg'
 
 
 def _version_and_run_completed(config):
     ssp_version = get_versions()['version']
     run_completed = (
-        f'{config.end_of_run.strftime("%Y-%m-%d %H:%M:%S")}'
+        f'{config.end_of_run.strftime("%Y-%m-%d %H:%M:%S")} '
         f'{config.end_of_run_tz}'
     )
     return ssp_version, run_completed
 
 
 def _author_html(config):
     author = ''
@@ -149,30 +149,28 @@
     elif config.agency_url is not None:
         agency = config.agency_url
     if config.agency_url is not None:
         agency = f'<a href="{config.agency_url}" target="_blank">{agency}</a>'
     return agency
 
 
-def _author_and_agency(config):
-    author = _author_html(config)
-    agency = _agency_html(config)
+def _author_and_agency_html(author, agency):
     if author != '':
         author = f'<br/><br/>{author}'
     if author == '' and agency != '':
         agency = f'<br/><br/>{agency}'
     if author != '' and agency != '':
         agency = f'<br/>{agency}'
-    return author, agency
+    return author + agency
 
 
 def _page_footer(config):
     footer_html = ''
-    indent3 = 3*'  '
-    indent4 = 4*'  '
+    indent3 = 3 * '  '
+    indent4 = 4 * '  '
     footer_html += f'{indent3}<div class="text_footer">\n'
     author = _author_html(config)
     agency = _agency_html(config)
     auth_agen_text = ''
     if author != '':
         if agency != '':
             auth_agen_text +=\
@@ -221,17 +219,18 @@
         text = f'{fmt}<br>-{fmt}<br>+{fmt}'
         text = text.format(value, error[0], error[1])
     return text
 
 
 def _station_value_and_err_text(par, key, fmt):
     """Format station value and error text."""
-    try:
-        _par = par[key]
-    except KeyError:
+    # par[key] can be None even if key is in par (e.g., if key is 'Ml' and
+    # local magnitude is not computed)
+    _par = par[key] if key in par else None
+    if _par is None:
         return '', ''
     if isinstance(_par, SpectralParameter):
         value = _par.value
         outlier = _par.outlier
     else:
         value = _par
         outlier = False
@@ -256,29 +255,32 @@
 def _misfit_table_rows(misfit_plot_files):
     template_dir = os.path.join(
         os.path.dirname(os.path.realpath(__file__)),
         'html_report_template'
     )
     misfit_table_column_html = os.path.join(
         template_dir, 'misfit_table_column.html')
-    misfit_table_column = open(misfit_table_column_html).read()
+    with open(
+        misfit_table_column_html, encoding='utf-8'
+    ) as fp:
+        misfit_table_column = fp.read()
     misfit_table_rows = ''
     for n, misfit_plot_file in enumerate(sorted(misfit_plot_files)):
         if n % 3 == 0:
             misfit_table_rows += '<tr>\n'
         misfit_plot_file = os.path.join(
             'misfit', os.path.basename(misfit_plot_file))
         misfit_table_rows += misfit_table_column.replace(
             '{MISFIT_PLOT}', misfit_plot_file)
         misfit_table_rows += '\n'
         if n % 3 == 2:
-            misfit_table_rows += 10*' '
+            misfit_table_rows += 10 * ' '
             misfit_table_rows += '</tr>\n'
-            misfit_table_rows += 10*' '
-    misfit_table_rows += 10*' '
+            misfit_table_rows += 10 * ' '
+    misfit_table_rows += 10 * ' '
     misfit_table_rows += '</tr>'
     return misfit_table_rows
 
 
 def _misfit_page(config):
     """Generate an HTML page with misfit plots."""
     # Read template files
@@ -292,19 +294,17 @@
     # Logo file
     logo_file = _logo_file_url()
 
     # Version and run completed
     ssp_version, run_completed = _version_and_run_completed(config)
 
     # Author and agency
-    author, agency = _author_and_agency(config)
-
-    # event info
-    hypo = config.hypo
-    evid = hypo.evid
+    author = _author_html(config)
+    agency = _agency_html(config)
+    author_and_agency = _author_and_agency_html(author, agency)
 
     # 1d conditional misfit plots
     misfit_plot_files = config.figures['misfit_1d']
     one_d_misfit_table_rows = _misfit_table_rows(misfit_plot_files)
 
     # 2d conditional misfit plots: fc-Mw
     misfit_plot_files = config.figures['misfit_fc-Mw']
@@ -319,57 +319,80 @@
     two_d_misfit_table_rows_tstar_mw = _misfit_table_rows(misfit_plot_files)
 
     # Main HTML page
     replacements = {
         '{LOGO_FILE}': logo_file,
         '{VERSION}': ssp_version,
         '{RUN_COMPLETED}': run_completed,
-        '{AUTHOR}': author,
-        '{AGENCY}': agency,
-        '{EVENTID}': evid,
+        '{AUTHOR_AND_AGENCY}': author_and_agency,
+        '{EVENTID}': config.event.event_id,
         '{1D_MISFIT_TABLE_ROWS}': one_d_misfit_table_rows,
         '{2D_MISFIT_TABLE_ROWS_FC_MW}': two_d_misfit_table_rows_fc_mw,
         '{2D_MISFIT_TABLE_ROWS_FC_TSTAR}': two_d_misfit_table_rows_fc_tstar,
         '{2D_MISFIT_TABLE_ROWS_TSTAR_MW}': two_d_misfit_table_rows_tstar_mw
     }
-    misfit = open(misfit_html).read()
+    with open(misfit_html, encoding='utf-8') as fp:
+        misfit = fp.read()
     misfit = _multireplace(misfit, replacements)
-    with open(misfit_html_out, 'w') as fp:
+    with open(misfit_html_out, 'w', encoding='utf-8') as fp:
         fp.write(misfit)
 
 
 def _add_run_info_to_html(config, replacements):
     """Add run info to HTML report."""
+    ssp_url = 'https://sourcespec.seismicsource.org'
     logo_file = _logo_file_url()
     agency_logo = _agency_logo(config)
     ssp_version, run_completed = _version_and_run_completed(config)
-    author, agency = _author_and_agency(config)
+    author = _author_html(config)
+    if not author:
+        author_comment_begin = '<!--'
+        author_comment_end = '-->'
+    else:
+        author_comment_begin = ''
+        author_comment_end = ''
+    agency = _agency_html(config)
+    if not agency:
+        agency_comment_begin = '<!--'
+        agency_comment_end = '-->'
+    else:
+        agency_comment_begin = ''
+        agency_comment_end = ''
+    author_and_agency = _author_and_agency_html(author, agency)
     page_footer = _page_footer(config)
     replacements.update({
         '{AGENCY_LOGO}': agency_logo,
         '{LOGO_FILE}': logo_file,
         '{VERSION}': ssp_version,
+        '{SSP_URL}': ssp_url,
         '{RUN_COMPLETED}': run_completed,
         '{AUTHOR}': author,
+        '{AUTHOR_COMMENT_BEGIN}': author_comment_begin,
+        '{AUTHOR_COMMENT_END}': author_comment_end,
         '{AGENCY}': agency,
+        '{AGENCY_COMMENT_BEGIN}': agency_comment_begin,
+        '{AGENCY_COMMENT_END}': agency_comment_end,
+        '{AUTHOR_AND_AGENCY}': author_and_agency,
         '{PAGE_FOOTER}': page_footer,
     })
 
 
 def _add_event_info_to_html(config, replacements):
     """Add event info to HTML report."""
-    hypo = config.hypo
-    evid = hypo.evid
+    evid = config.event.event_id
+    evname = config.event.name
+    hypo = config.event.hypocenter
     run_id = config.options.run_id
     replacements.update({
         '{EVENTID}': evid,
+        '{EVENT_NAME}': evname,
         '{RUNID}': run_id,
-        '{EVENT_LONGITUDE}': f'{hypo.longitude:8.3f}',
-        '{EVENT_LATITUDE}': f'{hypo.latitude:7.3f}',
-        '{EVENT_DEPTH}': f'{hypo.depth:5.1f}',
+        '{EVENT_LONGITUDE}': f'{hypo.longitude.value_in_deg:8.3f}',
+        '{EVENT_LATITUDE}': f'{hypo.latitude.value_in_deg:7.3f}',
+        '{EVENT_DEPTH}': f'{hypo.depth.value_in_km:5.1f}',
         '{ORIGIN_TIME}': f'{hypo.origin_time}',
     })
     # Link to event page, if defined
     event_url = config.event_url
     if event_url is not None:
         event_url = event_url.replace('$EVENTID', evid)
         parsed_url = urlparse(event_url)
@@ -385,29 +408,38 @@
         event_url_comment_begin = '<!--'
         event_url_comment_end = '-->'
     replacements.update({
         '{EVENT_URL}': event_url,
         '{EVENT_URL_COMMENT_BEGIN}': event_url_comment_begin,
         '{EVENT_URL_COMMENT_END}': event_url_comment_end
     })
+    # Only show Event Name if it is not empty
+    if evname:
+        evname_comment_begin = evname_comment_end = ''
+    else:
+        evname_comment_begin = '<!--'
+        evname_comment_end = '-->'
+    replacements.update({
+        '{EVENT_NAME_COMMENT_BEGIN}': evname_comment_begin,
+        '{EVENT_NAME_COMMENT_END}': evname_comment_end
+    })
     # Only show Run ID if it is not empty
     if run_id:
         run_id_comment_begin = run_id_comment_end = ''
     else:
         run_id_comment_begin = '<!--'
         run_id_comment_end = '-->'
     replacements.update({
         '{RUNID_COMMENT_BEGIN}': run_id_comment_begin,
         '{RUNID_COMMENT_END}': run_id_comment_end
     })
 
 
 def _add_maps_to_html(config, replacements):
     """Add maps to HTML report."""
-    global VALID_FIGURE_FORMATS
     try:
         station_maps = [
             m for m in config.figures['station_maps']
             if m.endswith(VALID_FIGURE_FORMATS)]
     except KeyError:
         station_maps = []
     map_mag = ''
@@ -438,16 +470,16 @@
         '{MAP_FC_COMMENT_BEGIN}': map_fc_comment_begin,
         '{MAP_FC_COMMENT_END}': map_fc_comment_end
     })
 
 
 def _add_traces_plots_to_html(config, templates, replacements):
     """Add trace plots to HTML report."""
-    global VALID_FIGURE_FORMATS
-    traces_plot = open(templates.traces_plot_html).read()
+    with open(templates.traces_plot_html, encoding='utf-8') as fp:
+        traces_plot = fp.read()
     traces_plot_files = [
         t for t in config.figures['traces']
         if t.endswith(VALID_FIGURE_FORMATS)]
     traces_plots = ''
     traces_plot_class = ''
     n_traces_plot_files = len(traces_plot_files)
     for n, traces_plot_file in enumerate(sorted(traces_plot_files)):
@@ -474,16 +506,16 @@
         '{TRACES_PLOTS_COMMENT_BEGIN}': traces_plots_comment_begin,
         '{TRACES_PLOTS_COMMENT_END}': traces_plots_comment_end
     })
 
 
 def _add_spectra_plots_to_html(config, templates, replacements):
     """Add spectra plots to HTML report."""
-    global VALID_FIGURE_FORMATS
-    spectra_plot = open(templates.spectra_plot_html).read()
+    with open(templates.spectra_plot_html, encoding='utf-8') as fp:
+        spectra_plot = fp.read()
     spectra_plot_files = [
         s for s in config.figures['spectra_regular']
         if s.endswith(VALID_FIGURE_FORMATS)]
     spectra_plots = ''
     spectra_plot_class = ''
     n_spectra_plot_files = len(spectra_plot_files)
     for n, spectra_plot_file in enumerate(sorted(spectra_plot_files)):
@@ -520,18 +552,20 @@
         'BH': 'Basin-hopping',
         'GS': 'Grid search',
         'IS': 'K-d tree importance sampling',
     }
     weightings = {
         'noise': 'Noise weighting',
         'frequency': 'Frequency weighting',
+        'inv_frequency': 'Inverse frequency weighting',
         'no_weight': 'No weighting',
     }
     inversion_algorithm = inversion_algorithms[
         sspec_output.inversion_info.algorithm]
+    inversion_wave_type = sspec_output.inversion_info.wave_type
     inversion_weighting = weightings[sspec_output.inversion_info.weighting]
     inversion_t_star_0 = f'{sspec_output.inversion_info.t_star_0} s'
     inversion_invert_t_star_0 =\
         str(sspec_output.inversion_info.invert_t_star_0)
     inversion_t_star_0_variability =\
         f'{sspec_output.inversion_info.t_star_0_variability * 100:.1f} %'
     if sspec_output.inversion_info.t_star_min_max == 'null':
@@ -547,14 +581,15 @@
     if sspec_output.inversion_info.Qo_min_max == 'null':
         inversion_Qo_min_max = '-'
     else:
         inversion_Qo_min_max =\
             str(sspec_output.inversion_info.Qo_min_max)
     replacements.update({
         '{INVERSION_ALGORITHM}': inversion_algorithm,
+        '{INVERSION_WAVE_TYPE}': inversion_wave_type,
         '{INVERSION_WEIGHTING}': inversion_weighting,
         '{INVERSION_T_STAR_0}': inversion_t_star_0,
         '{INVERSION_INVERT_T_STAR_0}': inversion_invert_t_star_0,
         '{INVERSION_T_STAR_0_VARIABILITY}': inversion_t_star_0_variability,
         '{INVERSION_T_STAR_MIN_MAX}': inversion_t_star_min_max,
         '{INVERSION_FC_MIN_MAX}': inversion_fc_min_max,
         '{INVERSION_Q0_MIN_MAX}': inversion_Qo_min_max,
@@ -608,21 +643,21 @@
     mean_errors = sspec_output.mean_uncertainties()
     wmeans = sspec_output.weighted_mean_values()
     wmean_errors = sspec_output.weighted_mean_uncertainties()
     percentiles = sspec_output.percentiles_values()
     percentile_errors = sspec_output.percentiles_uncertainties()
 
     n_sigma = config.n_sigma
-    n_sigma = int(n_sigma) if n_sigma.is_integer() else n_sigma
+    n_sigma = int(n_sigma) if float(n_sigma).is_integer() else n_sigma
     n_sigma = f'{n_sigma} sigma'
     mid_pct, lower_pct, upper_pct =\
         config.mid_percentage, config.lower_percentage, config.upper_percentage
-    mid_pct = int(mid_pct) if mid_pct.is_integer() else mid_pct
-    lower_pct = int(lower_pct) if lower_pct.is_integer() else lower_pct
-    upper_pct = int(upper_pct) if upper_pct.is_integer() else upper_pct
+    mid_pct = int(mid_pct) if float(mid_pct).is_integer() else mid_pct
+    lower_pct = int(lower_pct) if float(lower_pct).is_integer() else lower_pct
+    upper_pct = int(upper_pct) if float(upper_pct).is_integer() else upper_pct
     percentages = f'{mid_pct}%, [{lower_pct}%, {upper_pct}%]'
     replacements.update({
         '{N_SIGMA}': n_sigma,
         '{PERCENTAGES}': percentages
     })
 
     Mw_mean = means['Mw']
@@ -705,64 +740,85 @@
         '{RADIUS_MEAN_AND_ERR}': _summary_value_and_err_text(
             ra_mean, ra_mean_error, '{:.3f}'),
         '{RADIUS_WMEAN_AND_ERR}': _summary_value_and_err_text(
             ra_wmean, ra_wmean_error, '{:.3f}'),
         '{RADIUS_PERC_AND_ERR}': _summary_value_and_err_text(
             ra_perc, ra_perc_error, '{:.3f}'),
     })
-    bsd_mean = means['bsd']
-    bsd_mean_error = mean_errors['bsd']
-    bsd_wmean = wmeans['bsd']
-    bsd_wmean_error = wmean_errors['bsd']
-    bsd_perc = percentiles['bsd']
-    bsd_perc_error = percentile_errors['bsd']
-    replacements.update({
-        '{BSD_MEAN_AND_ERR}': _summary_value_and_err_text(
-            bsd_mean, bsd_mean_error, '{:.3e}'),
-        '{BSD_WMEAN_AND_ERR}': _summary_value_and_err_text(
-            bsd_wmean, bsd_wmean_error, '{:.3e}'),
-        '{BSD_PERC_AND_ERR}': _summary_value_and_err_text(
-            bsd_perc, bsd_perc_error, '{:.3e}'),
+    ssd_mean = means['ssd']
+    ssd_mean_error = mean_errors['ssd']
+    ssd_wmean = wmeans['ssd']
+    ssd_wmean_error = wmean_errors['ssd']
+    ssd_perc = percentiles['ssd']
+    ssd_perc_error = percentile_errors['ssd']
+    replacements.update({
+        '{SSD_MEAN_AND_ERR}': _summary_value_and_err_text(
+            ssd_mean, ssd_mean_error, '{:.3e}'),
+        '{SSD_WMEAN_AND_ERR}': _summary_value_and_err_text(
+            ssd_wmean, ssd_wmean_error, '{:.3e}'),
+        '{SSD_PERC_AND_ERR}': _summary_value_and_err_text(
+            ssd_perc, ssd_perc_error, '{:.3e}'),
     })
     Er_mean = means['Er']
     Er_mean_error = mean_errors['Er']
+    Er_wmean = wmeans['Er']
+    Er_wmean_error = wmean_errors['Er']
     Er_perc = percentiles['Er']
     Er_perc_error = percentile_errors['Er']
     replacements.update({
         '{ER_MEAN_AND_ERR}': _summary_value_and_err_text(
             Er_mean, Er_mean_error, '{:.3e}'),
+        '{ER_WMEAN_AND_ERR}': _summary_value_and_err_text(
+            Er_wmean, Er_wmean_error, '{:.3e}'),
         '{ER_PERC_AND_ERR}': _summary_value_and_err_text(
             Er_perc, Er_perc_error, '{:.3e}'),
     })
+    sigma_a_mean = means['sigma_a']
+    sigma_a_mean_error = mean_errors['sigma_a']
+    sigma_a_wmean = wmeans['sigma_a']
+    sigma_a_wmean_error = wmean_errors['sigma_a']
+    sigma_a_perc = percentiles['sigma_a']
+    sigma_a_perc_error = percentile_errors['sigma_a']
+    replacements.update({
+        '{SIGMA_A_MEAN_AND_ERR}': _summary_value_and_err_text(
+            sigma_a_mean, sigma_a_mean_error, '{:.3e}'),
+        '{SIGMA_A_WMEAN_AND_ERR}': _summary_value_and_err_text(
+            sigma_a_wmean, sigma_a_wmean_error, '{:.3e}'),
+        '{SIGMA_A_PERC_AND_ERR}': _summary_value_and_err_text(
+            sigma_a_perc, sigma_a_perc_error, '{:.3e}'),
+    })
     # Local magnitude, if computed
     if config.compute_local_magnitude:
         Ml_mean = means['Ml']
         Ml_mean_error = mean_errors['Ml']
+        Ml_wmean = wmeans['Ml']
+        Ml_wmean_error = wmean_errors['Ml']
         Ml_perc = percentiles['Ml']
         Ml_perc_error = percentile_errors['Ml']
         Ml_comment_begin = ''
         Ml_comment_end = ''
     else:
-        Ml_mean = Ml_perc = np.nan
-        Ml_mean_error = Ml_perc_error = (np.nan, np.nan)
+        Ml_mean = Ml_wmean = Ml_perc = np.nan
+        Ml_mean_error = Ml_wmean_error = Ml_perc_error = (np.nan, np.nan)
         Ml_comment_begin = '<!--'
         Ml_comment_end = '-->'
     replacements.update({
         '{ML_MEAN_AND_ERR}': _summary_value_and_err_text(
             Ml_mean, Ml_mean_error, '{:.2f}'),
+        '{ML_WMEAN_AND_ERR}': _summary_value_and_err_text(
+            Ml_wmean, Ml_wmean_error, '{:.2f}'),
         '{ML_PERC_AND_ERR}': _summary_value_and_err_text(
             Ml_perc, Ml_perc_error, '{:.2f}'),
         '{ML_COMMENT_BEGIN}': Ml_comment_begin,
         '{ML_COMMENT_END}': Ml_comment_end,
     })
 
 
 def _add_box_plots_to_html(config, replacements):
     """Add box plots to HTML report."""
-    global VALID_FIGURE_FORMATS
     box_plots = ''
     with contextlib.suppress(KeyError, IndexError):
         box_plots = [
             b for b in config.figures['boxplots']
             if b.endswith(VALID_FIGURE_FORMATS)][0]
         box_plots = os.path.basename(box_plots)
     if box_plots:
@@ -775,15 +831,14 @@
         '{BOX_PLOTS_COMMENT_BEGIN}': box_plots_comment_begin,
         '{BOX_PLOTS_COMMENT_END}': box_plots_comment_end,
     })
 
 
 def _add_stacked_spectra_to_html(config, replacements):
     """Add stacked spectra to HTML report."""
-    global VALID_FIGURE_FORMATS
     stacked_spectra = ''
     with contextlib.suppress(KeyError, IndexError):
         stacked_spectra = [
             s for s in config.figures['stacked_spectra']
             if s.endswith(VALID_FIGURE_FORMATS)][0]
         stacked_spectra = os.path.basename(stacked_spectra)
     if stacked_spectra:
@@ -796,31 +851,34 @@
         '{STACKED_SPECTRA_COMMENT_BEGIN}': stacked_spectra_comment_begin,
         '{STACKED_SPECTRA_COMMENT_END}': stacked_spectra_comment_end,
     })
 
 
 def _add_station_table_to_html(config, sspec_output, templates, replacements):
     """Add station table to HTML report."""
-    station_table_row = open(templates.station_table_row_html).read()
+    with open(templates.station_table_row_html, encoding='utf-8') as fp:
+        station_table_row = fp.read()
     station_table_rows = ''
     stationpar = sspec_output.station_parameters
     for statId in sorted(stationpar.keys()):
         par = stationpar[statId]
         instrument_type = par.instrument_type
         Mw_text, Mw_err_text = _station_value_and_err_text(par, 'Mw', '{:.3f}')
         fc_text, fc_err_text = _station_value_and_err_text(par, 'fc', '{:.3f}')
         t_star_text, t_star_err_text =\
             _station_value_and_err_text(par, 't_star', '{:.3f}')
         Qo_text, Qo_err_text = _station_value_and_err_text(par, 'Qo', '{:.1f}')
         Mo_text, Mo_err_text = _station_value_and_err_text(par, 'Mo', '{:.3e}')
-        bsd_text, bsd_err_text =\
-            _station_value_and_err_text(par, 'bsd', '{:.3e}')
+        ssd_text, ssd_err_text =\
+            _station_value_and_err_text(par, 'ssd', '{:.3e}')
         ra_text, ra_err_text =\
             _station_value_and_err_text(par, 'radius', '{:.3f}')
         Er_text, _ = _station_value_and_err_text(par, 'Er', '{:.3e}')
+        sigma_a_text, sigma_a_err_text =\
+            _station_value_and_err_text(par, 'sigma_a', '{:.3e}')
         Ml_text, _ = _station_value_and_err_text(par, 'Ml', '{:.3f}')
         hyp_dist_text, _ =\
             _station_value_and_err_text(par, 'hypo_dist_in_km', '{:.3f}')
         az_text, _ = _station_value_and_err_text(par, 'azimuth', '{:.3f}')
         row_replacements = {
             '{STATION_ID}': statId,
             '{STATION_TYPE}': instrument_type,
@@ -830,18 +888,20 @@
             '{STATION_FC_ERR}': fc_err_text,
             '{STATION_TSTAR}': t_star_text,
             '{STATION_TSTAR_ERR}': t_star_err_text,
             '{STATION_Q0}': Qo_text,
             '{STATION_Q0_ERR}': Qo_err_text,
             '{STATION_M0}': Mo_text,
             '{STATION_M0_ERR}': Mo_err_text,
-            '{STATION_BSD}': bsd_text,
-            '{STATION_BSD_ERR}': bsd_err_text,
+            '{STATION_SSD}': ssd_text,
+            '{STATION_SSD_ERR}': ssd_err_text,
             '{STATION_RA}': ra_text,
             '{STATION_RA_ERR}': ra_err_text,
+            '{STATION_SIGMA_A}': sigma_a_text,
+            '{STATION_SIGMA_A_ERR}': sigma_a_err_text,
             '{STATION_ER}': Er_text,
             '{STATION_ML}': Ml_text,
             '{STATION_DIST}': hyp_dist_text,
             '{STATION_AZ}': az_text,
         }
         # Local magnitude, if computed
         if config.compute_local_magnitude:
@@ -872,44 +932,50 @@
         misfit_plot_comment_end = '-->'
     replacements.update({
         '{MISFIT_PLOT_COMMENT_BEGIN}': misfit_plot_comment_begin,
         '{MISFIT_PLOT_COMMENT_END}': misfit_plot_comment_end
     })
 
 
-def _add_output_files_to_html(config, templates, replacements):
-    evid = config.hypo.evid
+def _add_downloadable_files_to_html(config, templates, replacements):
+    """Add links to downloadable files to HTML report."""
+    # symlink to input files (not supported on Windows)
+    input_files = '' if os.name == 'nt' else 'input_files'
+    evid = config.event.event_id
     config_file = f'{evid}.ssp.conf'
     yaml_file = f'{evid}.ssp.yaml'
     log_file = f'{evid}.ssp.log'
 
     replacements.update({
+        '{INPUT_FILES}': input_files,
         '{CONF_FILE_BNAME}': config_file,
         '{CONF_FILE}': config_file,
         '{YAML_FILE_BNAME}': yaml_file,
         '{YAML_FILE}': yaml_file,
         '{LOG_FILE_BNAME}': log_file,
         '{LOG_FILE}': log_file,
     })
 
     # QuakeML file (if produced)
     if config.qml_file_out is not None:
         quakeml_file = os.path.basename(config.qml_file_out)
-        quakeml_file_link = open(templates.quakeml_file_link_html).read()
+        with open(templates.quakeml_file_link_html, encoding='utf-8') as fp:
+            quakeml_file_link = fp.read()
         quakeml_file_link = quakeml_file_link\
             .replace('{QUAKEML_FILE}', quakeml_file)\
             .replace('{QUAKEML_FILE_BNAME}', quakeml_file)
     else:
         quakeml_file_link = ''
     replacements.update({
         '{QUAKEML_FILE_LINK}': quakeml_file_link
     })
 
 
 class HTMLtemplates:
+    """Class to hold paths to HTML templates."""
     def __init__(self):
         template_dir = os.path.join(
             os.path.dirname(os.path.realpath(__file__)),
             'html_report_template'
         )
         self.style_css = os.path.join(template_dir, 'style.css')
         self.index_html = os.path.join(template_dir, 'index.html')
@@ -946,17 +1012,18 @@
     _add_spectra_plots_to_html(config, templates, replacements)
     _add_inversion_info_to_html(sspec_output, replacements)
     _add_summary_spectral_params_to_html(config, sspec_output, replacements)
     _add_box_plots_to_html(config, replacements)
     _add_stacked_spectra_to_html(config, replacements)
     _add_station_table_to_html(config, sspec_output, templates, replacements)
     _add_misfit_plots_to_html(config, replacements)
-    _add_output_files_to_html(config, templates, replacements)
+    _add_downloadable_files_to_html(config, templates, replacements)
 
-    index = open(templates.index_html).read()
+    with open(templates.index_html, encoding='utf-8') as fp:
+        index = fp.read()
     index = _multireplace(index, replacements)
     index = _cleanup_html(index)
     shutil.copy(templates.style_css, config.options.outdir)
     index_html_out = os.path.join(config.options.outdir, 'index.html')
-    with open(index_html_out, 'w') as fp:
+    with open(index_html_out, 'w', encoding='utf-8') as fp:
         fp.write(index)
     logger.info(f'HTML report written to file: {index_html_out}')
```

### Comparing `sourcespec-1.7/sourcespec/ssp_inversion.py` & `sourcespec-1.8/sourcespec/ssp_inversion.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,95 +6,99 @@
 :copyright:
     2012 Claudio Satriano <satriano@ipgp.fr>
 
     2013-2014 Claudio Satriano <satriano@ipgp.fr>,
               Emanuela Matrullo <matrullo@geologie.ens.fr>,
               Agnes Chounet <chounet@ipgp.fr>
 
-    2015-2023 Claudio Satriano <satriano@ipgp.fr>
+    2015-2024 Claudio Satriano <satriano@ipgp.fr>
 :license:
     CeCILL Free Software License Agreement v2.1
     (http://www.cecill.info/licences.en.html)
 """
 import logging
 import numpy as np
 from scipy.optimize import curve_fit, minimize, basinhopping
 from scipy.signal import argrelmax
-from obspy import Stream
 from obspy.geodetics import gps2dist_azimuth
+from sourcespec.spectrum import SpectrumStream
 from sourcespec.ssp_spectral_model import (
     spectral_model, objective_func, callback)
 from sourcespec.ssp_util import (
-    mag_to_moment, source_radius, bsd, quality_factor, select_trace, smooth)
+    mag_to_moment, source_radius, static_stress_drop, quality_factor,
+    select_trace, smooth)
 from sourcespec.ssp_data_types import (
     InitialValues, Bounds, SpectralParameter, StationParameters,
     SourceSpecOutput)
 from sourcespec.ssp_grid_sampling import GridSampling
-logger = logging.getLogger(__name__.split('.')[-1])
+logger = logging.getLogger(__name__.rsplit('.', maxsplit=1)[-1])
 
 
 def _curve_fit(config, spec, weight, yerr, initial_values, bounds):
     """
     Curve fitting.
 
     Available algorithms:
       - Levenberg-Marquardt (LM, via `curve_fit()`). Automatically switches to
         Trust Region Reflective algorithm if bounds are provided.
       - Truncated Newton algorithm (TNC) with bounds.
       - Basin-hopping (BH)
       - Grid search (GS)
     """
-    freq_log = spec.freq_log
-    ydata = spec.data_log_mag
-    minimize_func = objective_func(freq_log, ydata, weight)
+    freq_logspaced = spec.freq_logspaced
+    ydata = spec.data_mag_logspaced
+    minimize_func = objective_func(freq_logspaced, ydata, weight)
     if config.inv_algorithm == 'TNC':
         res = minimize(
             minimize_func,
             x0=initial_values.get_params0(), method='TNC',
             callback=callback, bounds=bounds.bounds
         )
         params_opt = res.x
         # trick: use curve_fit() bounded to params_opt
         # to get the covariance
+        # pylint: disable=unbalanced-tuple-unpacking
         _, params_cov = curve_fit(
-            spectral_model, freq_log, ydata,
+            spectral_model, freq_logspaced, ydata,
             p0=params_opt, sigma=yerr,
-            bounds=(params_opt-(1e-10), params_opt+(1e-10))
+            bounds=(params_opt - (1e-10), params_opt + (1e-10))
         )
         err = np.sqrt(params_cov.diagonal())
         # symmetric error
         params_err = ((e, e) for e in err)
     elif config.inv_algorithm == 'LM':
         bnds = bounds.get_bounds_curve_fit()
         if bnds is not None:
             logger.info(
                 'Trying to use using Levenberg-Marquardt '
                 'algorithm with bounds. Switching to the '
                 'Trust Region Reflective algorithm.'
             )
+        # pylint: disable=unbalanced-tuple-unpacking
         params_opt, params_cov = curve_fit(
-            spectral_model, freq_log, ydata,
+            spectral_model, freq_logspaced, ydata,
             p0=initial_values.get_params0(), sigma=yerr,
             bounds=bnds
         )
         err = np.sqrt(params_cov.diagonal())
         # symmetric error
         params_err = ((e, e) for e in err)
     elif config.inv_algorithm == 'BH':
         res = basinhopping(
             minimize_func, x0=initial_values.get_params0(), niter=100,
             accept_test=bounds
         )
         params_opt = res.x
         # trick: use curve_fit() bounded to params_opt
         # to get the covariance
+        # pylint: disable=unbalanced-tuple-unpacking
         _, params_cov = curve_fit(
-            spectral_model, freq_log, ydata,
+            spectral_model, freq_logspaced, ydata,
             p0=params_opt, sigma=yerr,
-            bounds=(params_opt-(1e-10), params_opt+(1e-10))
+            bounds=(params_opt - (1e-10), params_opt + (1e-10))
         )
         err = np.sqrt(params_cov.diagonal())
         # symmetric error
         params_err = ((e, e) for e in err)
     elif config.inv_algorithm in ['GS', 'IS']:
         nsteps = (20, 150, 150)  # we do fewer steps in magnitude
         sampling_mode = ('lin', 'log', 'lin')
@@ -120,15 +124,15 @@
         # tstar-Mw
         plot_par_idx = (2, 0)
         grid_sampling.plot_misfit_2d(config, plot_par_idx, spec_label)
     misfit = minimize_func(params_opt)
     return params_opt, params_err, misfit
 
 
-def _freq_ranges_for_Mw0_and_tstar0(config, weight, freq_log, statId):
+def _freq_ranges_for_Mw0_and_tstar0(config, weight, freq_logspaced, statId):
     """Find the frequency range to compute Mw_0 and, possibly, t_star_0."""
     if config.weighting == 'noise':
         # we start where signal-to-noise becomes strong
         idx0 = np.where(weight > 0.5)[0][0]
         # we stop at the first max of signal-to-noise (proxy for fc)
         idx_max = argrelmax(weight)[0]
         # just keep the indexes for maxima > 0.5
@@ -143,81 +147,106 @@
             )
         idx1 = idx_max[0]
         if idx1 == idx0:
             try:
                 idx1 = idx_max[1]
             except IndexError:
                 # if there are no other maxima, just take 5 points
-                idx1 = idx0+5
+                idx1 = idx0 + 5
     elif config.weighting == 'frequency':
         idx0 = 0
         # the closest index to f_weight:
-        idx1 = np.where(freq_log <= config.f_weight)[0][-1]
+        idx1 = np.where(freq_logspaced <= config.f_weight)[0][-1]
+    elif config.weighting == 'inv_frequency':
+        weight_idxs = np.where(weight >= 0.7)[0]
+        try:
+            idx0 = weight_idxs[0]
+        except IndexError:
+            idx0 = 0
+        try:
+            idx1 = weight_idxs[-1]
+        except IndexError:
+            idx1 = len(weight) - 1
     else:
         idx0 = 0
         idx1 = len(weight) // 2
     return idx0, idx1
 
 
 def _spec_inversion(config, spec, spec_weight):
     """Invert one spectrum, return a StationParameters() object."""
     # azimuth computation
     coords = spec.stats.coords
-    hypo = spec.stats.hypo
     stla = coords.latitude
     stlo = coords.longitude
-    evla = hypo.latitude
-    evlo = hypo.longitude
+    hypo = spec.stats.event.hypocenter
+    magnitude = spec.stats.event.magnitude
+    evla = hypo.latitude.value_in_deg
+    evlo = hypo.longitude.value_in_deg
     geod = gps2dist_azimuth(evla, evlo, stla, stlo)
     az = geod[1]
 
-    freq_log = spec.freq_log
-    ydata = spec.data_log_mag
+    freq_logspaced = spec.freq_logspaced
+    ydata = spec.data_mag_logspaced
     statId = f'{spec.id} {spec.stats.instrtype}'
-    weight = spec_weight.data_log
+    weight = spec_weight.data_logspaced
 
     # 'curve_fit' interprets 'yerr' as standard deviation array
     # and calculates weights as 1/yerr^2 .
     # Therefore we build yerr as:
-    yerr = 1./np.sqrt(weight)
+    yerr = 1. / np.sqrt(weight)
 
     # Find frequency range (indexes) to compute Mw_0 and t_star_0
     # When using noise weighting, idx1 is the first maximum in
     # signal-to-noise ratio
     idx0, idx1 = _freq_ranges_for_Mw0_and_tstar0(
-        config, weight, freq_log, statId)
+        config, weight, freq_logspaced, statId)
 
     # first maximum is a proxy for fc, we use it for fc_0:
-    fc_0 = freq_log[idx1]
+    fc_0 = freq_logspaced[idx1]
 
     t_star_min = t_star_max = None
     if config.invert_t_star_0:
         # fit t_star_0 and Mw on the initial part of the spectrum,
         # corrected for the effect of fc
-        ydata_corr = ydata - spectral_model(freq_log, Mw=0, fc=fc_0, t_star=0)
+        ydata_corr =\
+            ydata - spectral_model(freq_logspaced, Mw=0, fc=fc_0, t_star=0)
         ydata_corr = smooth(ydata_corr, window_len=18)
         slope, Mw_0 = np.polyfit(
-            freq_log[idx0: idx1], ydata_corr[idx0: idx1], deg=1)
-        t_star_0 = -3./2 * slope / (np.pi * np.log10(np.e))
+            freq_logspaced[idx0: idx1], ydata_corr[idx0: idx1], deg=1)
+        t_star_0 = -3. / 2 * slope / (np.pi * np.log10(np.e))
         t_star_min = t_star_0 * (1 - config.t_star_0_variability)
         t_star_max = t_star_0 * (1 + config.t_star_0_variability)
     if not config.invert_t_star_0 or t_star_0 < 0:
         # we calculate the initial value for Mw as an average
         Mw_0 = np.nanmean(ydata[idx0: idx1])
         t_star_0 = config.t_star_0
+    # Mw_0_min and Mw_0_max are used to set the bounds for Mw
+    # (see below)
+    Mw_0_min = np.nanmin(ydata[idx0: idx1])
+    Mw_0_max = np.nanmax(ydata[idx0: idx1])
+
+    if config.Mw_0_from_event_file and magnitude.value is not None:
+        Mw_0 = magnitude.value
+        # If Mw_0 is provided in the event file, we will set the inversion
+        # bounds around it (see below)
+        Mw_0_min = Mw_0_max = Mw_0
 
     initial_values = InitialValues(Mw_0, fc_0, t_star_0)
-    logger.info(f'{statId}: initial values: {initial_values}')
     bounds = Bounds(config, spec, initial_values)
-    bounds.Mw_min = np.nanmin(ydata[idx0: idx1]) * 0.9
-    bounds.Mw_max = np.nanmax(ydata[idx0: idx1]) * 1.1
+    Mw_0_variability =\
+        config.Mw_0_variability if config.Mw_0_variability > 0 else 1e-6
+    bounds.Mw_min = Mw_0_min * (1 - Mw_0_variability)
+    bounds.Mw_max = Mw_0_max * (1 + Mw_0_variability)
     if t_star_min is not None:
         bounds.t_star_min = t_star_min
     if t_star_max is not None:
         bounds.t_star_max = t_star_max
+    # Initial values need to be printed here because Bounds can modify them
+    logger.info(f'{statId}: initial values: {initial_values}')
     logger.info(f'{statId}: bounds: {bounds}')
     try:
         params_opt, params_err, misfit = _curve_fit(
             config, spec, weight, yerr, initial_values, bounds)
     except (RuntimeError, ValueError) as m:
         raise RuntimeError(
             f'{m}\n{statId}: unable to fit spectral model'
@@ -247,69 +276,77 @@
             f'{statId}: misfit larger than pi_misfit_max: '
             f'{misfit:.3f} > {misfit_max:.3f}: ignoring inversion results'
         )
 
     # Check post-inversion bounds for t_star and fc
     pi_t_star_min, pi_t_star_max =\
         config.pi_t_star_min_max or (-np.inf, np.inf)
+    # pylint: disable=superfluous-parens
     if not (pi_t_star_min <= t_star <= pi_t_star_max):
         raise ValueError(
             f'{statId}: t_star: {t_star:.3f} not in allowed range '
             f'[{pi_t_star_min:.3f}, {pi_t_star_max:.3f}]: '
             'ignoring inversion results'
         )
     pi_fc_min, pi_fc_max = config.pi_fc_min_max or (-np.inf, np.inf)
     if not (pi_fc_min <= fc <= pi_fc_max):
         raise ValueError(
             f'{statId}: fc: {fc:.3f} not in allowed range '
             f'[{pi_fc_min:.3f}, {pi_fc_max:.3f}]: ignoring inversion results'
         )
 
     station_pars = StationParameters(
-        id=spec.id, instrument_type=spec.stats.instrtype,
+        station_id=spec.id, instrument_type=spec.stats.instrtype,
         latitude=stla, longitude=stlo,
         hypo_dist_in_km=spec.stats.hypo_dist,
         epi_dist_in_km=spec.stats.epi_dist,
         azimuth=az)
     station_pars.Mw = SpectralParameter(
-        id='Mw', value=Mw,
+        param_id='Mw', value=Mw,
         lower_uncertainty=Mw_err[0], upper_uncertainty=Mw_err[1],
-        confidence_level=68.2, format='{:.2f}')
+        confidence_level=68.2, format_spec='{:.2f}')
     station_pars.fc = SpectralParameter(
-        id='fc', value=fc,
+        param_id='fc', value=fc,
         lower_uncertainty=fc_err[0], upper_uncertainty=fc_err[1],
-        confidence_level=68.2, format='{:.3f}')
+        confidence_level=68.2, format_spec='{:.3f}')
     station_pars.t_star = SpectralParameter(
-        id='t_star', value=t_star,
+        param_id='t_star', value=t_star,
         lower_uncertainty=t_star_err[0], upper_uncertainty=t_star_err[1],
-        confidence_level=68.2, format='{:.3f}')
+        confidence_level=68.2, format_spec='{:.3f}')
 
     # additional parameters, computed from fc, Mw and t_star
-    vs = config.hypo.vs
+    k_coeff = config.kp if config.wave_type == 'P' else config.ks
+    beta = config.event.hypocenter.vs * 1e3  # shear wave velocity in m/s
     travel_time = spec.stats.travel_times[config.wave_type[0]]
     # seismic moment
     station_pars.Mo = SpectralParameter(
-        id='Mw', value=mag_to_moment(Mw), format='{:.3e}')
+        param_id='Mo', value=mag_to_moment(Mw), format_spec='{:.3e}')
     # source radius in meters
     station_pars.radius = SpectralParameter(
-        id='radius', value=source_radius(fc, vs*1e3), format='{:.3f}')
-    # Brune stress drop in MPa
-    station_pars.bsd = SpectralParameter(
-        id='bsd', value=bsd(station_pars.Mo.value, station_pars.radius.value),
-        format='{:.3e}')
+        param_id='radius', value=source_radius(fc, beta, k_coeff),
+        format_spec='{:.3f}')
+    # Static stress drop in MPa
+    station_pars.ssd = SpectralParameter(
+        param_id='ssd',
+        value=static_stress_drop(
+            station_pars.Mo.value, station_pars.radius.value
+        ),
+        format_spec='{:.3e}'
+    )
     # quality factor
     station_pars.Qo = SpectralParameter(
-        id='Qo', value=quality_factor(travel_time, t_star), format='{:.1f}')
+        param_id='Qo', value=quality_factor(travel_time, t_star),
+        format_spec='{:.1f}')
 
-    # Check post-inversion bounds for bsd
-    pi_bsd_min, pi_bsd_max = config.pi_bsd_min_max or (-np.inf, np.inf)
-    if not (pi_bsd_min <= station_pars.bsd.value <= pi_bsd_max):
+    # Check post-inversion bounds for ssd
+    pi_ssd_min, pi_ssd_max = config.pi_ssd_min_max or (-np.inf, np.inf)
+    if not (pi_ssd_min <= station_pars.ssd.value <= pi_ssd_max):
         raise ValueError(
-            f'{statId}: bsd: {station_pars.bsd.value:.3e} '
-            f'not in allowed range [{pi_bsd_min:.3e}, {pi_bsd_max:.3e}]: '
+            f'{statId}: ssd: {station_pars.ssd.value:.3e} '
+            f'not in allowed range [{pi_ssd_min:.3e}, {pi_ssd_max:.3e}]: '
             'ignoring inversion results'
         )
 
     # additional parameter errors, computed from fc, Mw and t_star
     # seismic moment
     Mw_min = Mw - Mw_err[0]
     Mw_max = Mw + Mw_err[1]
@@ -317,29 +354,29 @@
     Mo_max = mag_to_moment(Mw_max)
     station_pars.Mo.lower_uncertainty = station_pars.Mo.value - Mo_min
     station_pars.Mo.upper_uncertainty = Mo_max - station_pars.Mo.value
     station_pars.Mo.confidence_level = 68.2
     # source radius in meters
     fc_min = fc - fc_err[0]
     if fc_min <= 0:
-        fc_min = freq_log[0]
+        fc_min = freq_logspaced[0]
     fc_max = fc + fc_err[1]
-    radius_min = source_radius(fc_max, vs*1e3)
-    radius_max = source_radius(fc_min, vs*1e3)
+    radius_min = source_radius(fc_max, beta, k_coeff)
+    radius_max = source_radius(fc_min, beta, k_coeff)
     station_pars.radius.lower_uncertainty =\
         station_pars.radius.value - radius_min
     station_pars.radius.upper_uncertainty =\
         radius_max - station_pars.radius.value
     station_pars.radius.confidence_level = 68.2
-    # Brune stress drop in MPa
-    bsd_min = bsd(Mo_min, radius_max)
-    bsd_max = bsd(Mo_max, radius_min)
-    station_pars.bsd.lower_uncertainty = station_pars.bsd.value - bsd_min
-    station_pars.bsd.upper_uncertainty = bsd_max - station_pars.bsd.value
-    station_pars.bsd.confidence_level = 68.2
+    # static stress drop in MPa
+    ssd_min = static_stress_drop(Mo_min, radius_max)
+    ssd_max = static_stress_drop(Mo_max, radius_min)
+    station_pars.ssd.lower_uncertainty = station_pars.ssd.value - ssd_min
+    station_pars.ssd.upper_uncertainty = ssd_max - station_pars.ssd.value
+    station_pars.ssd.confidence_level = 68.2
     # quality factor
     t_star_min = t_star - t_star_err[0]
     if t_star_min <= 0:
         t_star_min = 0.001
     t_star_max = t_star + t_star_err[1]
     Qo_min = quality_factor(travel_time, t_star_max)
     Qo_max = quality_factor(travel_time, t_star_min)
@@ -348,65 +385,75 @@
     station_pars.Qo.confidence_level = 68.2
 
     return station_pars
 
 
 def _synth_spec(config, spec, station_pars):
     """Return a stream with one or more synthetic spectra."""
-    par = station_pars._params
-    par_err = station_pars._params_err
-    spec_st = Stream()
+    par = {
+        x.param_id: x.value
+        for x in station_pars.get_spectral_parameters().values()
+    }
+    par_err = {
+        x.param_id: x.compact_uncertainty()
+        for x in station_pars.get_spectral_parameters().values()
+    }
     params_opt = [par[key] for key in ('Mw', 'fc', 't_star')]
-
     chan_no_orientation = spec.stats.channel[:-1]
+    spec_st = SpectrumStream()
 
-    freq = spec.get_freq()
-    freq_log = spec.freq_log
+    freq = spec.freq
+    freq_logspaced = spec.freq_logspaced
     spec_synth = spec.copy()
     spec_synth.stats.channel = f'{chan_no_orientation}S'
     spec_synth.stats.par = par
     spec_synth.stats.par_err = par_err
     spec_synth.data_mag = spectral_model(freq, *params_opt)
     spec_synth.data = mag_to_moment(spec_synth.data_mag)
-    spec_synth.data_log_mag = spectral_model(freq_log, *params_opt)
-    spec_synth.data_log = mag_to_moment(spec_synth.data_log_mag)
+    spec_synth.data_mag_logspaced = spectral_model(freq_logspaced, *params_opt)
+    spec_synth.data_logspaced = mag_to_moment(spec_synth.data_mag_logspaced)
     spec_st.append(spec_synth)
 
     # Add an extra spectrum with no attenuation
     if config.plot_spectra_no_attenuation:
         spec_synth = spec.copy()
         spec_synth.stats.channel = f'{chan_no_orientation}s'
         _params = list(params_opt)
         _params[-1] = 0
         spec_synth.data_mag = spectral_model(freq, *_params)
         spec_synth.data = mag_to_moment(spec_synth.data_mag)
-        spec_synth.data_log_mag = spectral_model(freq_log, *_params)
-        spec_synth.data_log = mag_to_moment(spec_synth.data_log_mag)
+        spec_synth.data_mag_logspaced =\
+            spectral_model(freq_logspaced, *_params)
+        spec_synth.data_logspaced =\
+            mag_to_moment(spec_synth.data_mag_logspaced)
         spec_st.append(spec_synth)
 
     # Add an extra spectrum with no corner frequency
     if config.plot_spectra_no_fc:
         spec_synth = spec.copy()
         spec_synth.stats.channel = f'{chan_no_orientation}t'
         _params = list(params_opt)
         _params[1] = 1e999
         spec_synth.data_mag = spectral_model(freq, *_params)
         spec_synth.data = mag_to_moment(spec_synth.data_mag)
-        spec_synth.data_log_mag = spectral_model(freq_log, *_params)
-        spec_synth.data_log = mag_to_moment(spec_synth.data_log_mag)
+        spec_synth.data_mag_logspaced =\
+            spectral_model(freq_logspaced, *_params)
+        spec_synth.data_logspaced =\
+            mag_to_moment(spec_synth.data_mag_logspaced)
         spec_st.append(spec_synth)
     return spec_st
 
 
 def spectral_inversion(config, spec_st, weight_st):
     """Inversion of displacement spectra."""
     logger.info('Inverting spectra...')
     weighting_messages = {
         'noise': 'Using noise weighting for inversion.',
         'frequency': 'Using frequency weighting for inversion.',
+        'inv_frequency': 'Using inverse frequency weighting for inversion.',
         'no_weight': 'Using no weighting for inversion.'
     }
     logger.info(weighting_messages[config.weighting])
     algorithm_messages = {
         'TNC': 'Using truncated Newton algorithm for inversion.',
         'LM': 'Using Levenberg-Marquardt algorithm for inversion.',
         'BH': 'Using basin-hopping algorithm for inversion.',
@@ -415,39 +462,56 @@
     }
     logger.info(algorithm_messages[config.inv_algorithm])
 
     stations = {x.stats.station for x in spec_st}
     spectra = [sp for sta in stations for sp in spec_st.select(station=sta)]
 
     sspec_output = SourceSpecOutput()
+    sspec_output.inversion_info.wave_type = config.wave_type
     sspec_output.inversion_info.algorithm = config.inv_algorithm
     sspec_output.inversion_info.weighting = config.weighting
     sspec_output.inversion_info.t_star_0 = config.t_star_0
     sspec_output.inversion_info.invert_t_star_0 = config.invert_t_star_0
     sspec_output.inversion_info.t_star_0_variability =\
         config.t_star_0_variability
     sspec_output.inversion_info.t_star_min_max =\
         config.t_star_min_max or 'null'
     sspec_output.inversion_info.fc_min_max = config.fc_min_max or 'null'
     sspec_output.inversion_info.Qo_min_max = config.Qo_min_max or 'null'
-    hypo = config.hypo
-    sspec_output.event_info.event_id = hypo.evid
-    sspec_output.event_info.longitude = hypo.longitude
-    sspec_output.event_info.latitude = hypo.latitude
-    sspec_output.event_info.depth_in_km = hypo.depth
-    sspec_output.event_info.origin_time = hypo.origin_time
+    event = config.event
+    sspec_output.event_info.event_id = event.event_id
+    if event.name is not None:
+        sspec_output.event_info.event_name = event.name
+    sspec_output.event_info.longitude = event.hypocenter.longitude.value_in_deg
+    sspec_output.event_info.latitude = event.hypocenter.latitude.value_in_deg
+    sspec_output.event_info.depth_in_km = event.hypocenter.depth.value_in_km
+    sspec_output.event_info.origin_time = event.hypocenter.origin_time
+    sspec_output.event_info.vp_in_km_s = event.hypocenter.vp
+    sspec_output.event_info.vs_in_km_s = event.hypocenter.vs
+    sspec_output.event_info.rho_in_kg_m3 = event.hypocenter.rho
+    sspec_output.event_info.kp = config.kp
+    sspec_output.event_info.ks = config.ks
+    if config.Mw_0_from_event_file and event.magnitude.value is not None:
+        msg = (
+            f'Setting Mw_0 to the value provided in the event file: '
+            f'{event.magnitude.mag_type} '
+            f'{event.magnitude.value:.4f}')
+        if event.magnitude.computed:
+            msg += ' (computed from scalar moment)'
+        logger.info(msg)
     for spec in sorted(spectra, key=lambda sp: sp.id):
         if spec.stats.channel[-1] != 'H':
             continue
         if spec.stats.ignore:
             continue
         spec_weight = select_trace(weight_st, spec.id, spec.stats.instrtype)
         try:
             station_pars = _spec_inversion(config, spec, spec_weight)
         except (RuntimeError, ValueError) as msg:
             logger.warning(msg)
             continue
         spec_st += _synth_spec(config, spec, station_pars)
-        sspec_output.station_parameters[station_pars._id] = station_pars
+        sspec_output.station_parameters[station_pars.station_id] = station_pars
 
     logger.info('Inverting spectra: done')
+    logger.info('---------------------------------------------------')
     return sspec_output
```

### Comparing `sourcespec-1.7/sourcespec/ssp_local_magnitude.py` & `sourcespec-1.8/sourcespec/ssp_local_magnitude.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,36 +5,37 @@
 
 :copyright:
     2012 Claudio Satriano <satriano@ipgp.fr>
 
     2013-2014 Claudio Satriano <satriano@ipgp.fr>,
               Emanuela Matrullo <matrullo@geologie.ens.fr>
 
-    2015-2023 Claudio Satriano <satriano@ipgp.fr>
+    2015-2024 Claudio Satriano <satriano@ipgp.fr>
 :license:
     CeCILL Free Software License Agreement v2.1
     (http://www.cecill.info/licences.en.html)
 """
 import contextlib
 import logging
-import numpy as np
 from copy import deepcopy
+import numpy as np
+# pylint: disable=no-name-in-module
 from obspy.signal.filter import envelope
 from obspy.signal.invsim import WOODANDERSON
 from obspy.signal.util import smooth
 from obspy.signal.trigger import trigger_onset
 from sourcespec.ssp_data_types import SpectralParameter
 from sourcespec.ssp_util import cosine_taper
 from sourcespec.ssp_util import remove_instr_response
-logger = logging.getLogger(__name__.split('.')[-1])
+logger = logging.getLogger(__name__.rsplit('.', maxsplit=1)[-1])
 
 
 def _check_nyquist(freqmax, trace):
     """Check if freqmax is smaller than Nyquist frequency."""
-    nyquist = 1./(2. * trace.stats.delta)
+    nyquist = 1. / (2. * trace.stats.delta)
     if freqmax >= nyquist:
         freqmax = nyquist * 0.999
         msg = (
             f'{trace.id}: maximum frequency for bandpass filtering in '
             'local magnitude computation is larger than or equal '
             f'to Nyquist. Setting it to {freqmax} Hz'
         )
@@ -100,15 +101,15 @@
     tr_process.trim(starttime=t0, endtime=t1, pad=True, fill_value=0)
     npts = len(tr_process.data)
     if npts == 0:
         raise RuntimeError(
             f'{tr.id}: No data for the selected cut interval: skipping trace'
         )
     nzeros = len(np.where(tr_process.data == 0)[0])
-    if nzeros > npts/4:
+    if nzeros > npts / 4:
         raise RuntimeError(
             f'{tr.id}: Too many gaps for the selected cut interval: '
             'skipping trace'
         )
 
     # If the check is ok, recover the full trace
     # (it will be cut later on)
@@ -116,15 +117,15 @@
     # remove the mean...
     tr_process.detrend(type='constant')
     # ...and the linear trend...
     tr_process.detrend(type='linear')
     freqmin = config.ml_bp_freqmin
     freqmax = _check_nyquist(freqmax=config.ml_bp_freqmax, trace=tr)
     # ...remove response...
-    pre_filt = (freqmin, freqmin*1.1, freqmax*0.9, freqmax)
+    pre_filt = (freqmin, freqmin * 1.1, freqmax * 0.9, freqmax)
     if config.correct_instrumental_response:
         remove_instr_response(tr_process, pre_filt)
     # ...filter
     tr_process.filter(type='bandpass', freqmin=freqmin, freqmax=freqmax)
     # Convert to Wood-Anderson
     # note: conversion to Wood-Anderson integrates the signal once
     if tr.stats.instrtype == 'acc':
@@ -166,19 +167,18 @@
         try:
             station_pars = station_parameters[key]
         except KeyError:
             continue
 
         # Make sure that the param_Ml object is always defined, even when Ml
         # is not computed (i.e., "continue" below)
-        try:
-            param_Ml = station_pars.Ml
-        except KeyError:
+        param_Ml = station_pars.Ml
+        if param_Ml is None:
             param_Ml = SpectralParameter(
-                id='Ml', value=np.nan, format='{:.2f}')
+                param_id='Ml', value=np.nan, format_spec='{:.2f}')
             station_pars.Ml = param_Ml
 
         # only compute Ml for horizontal components
         comp = tr.stats.channel
         if comp[-1] in ['Z', 'H']:
             continue
 
@@ -187,15 +187,15 @@
             tr_process = _process_trace(config, tr, t0, t1)
         except RuntimeError as msg:
             logger.warning(msg)
             continue
 
         # Local magnitude
         # amp must be in millimeters for local magnitude computation
-        amp = np.abs(tr_process.max())*1000.
+        amp = np.abs(tr_process.max()) * 1e3
         h_dist = tr_process.stats.hypo_dist
         ml = _compute_local_magnitude(config, amp, h_dist)
         statId = f'{tr_id} {tr.stats.instrtype}'
         logger.info(f'{statId}: Ml {ml:.1f}')
         # compute average with the other component, if available
         with contextlib.suppress(KeyError):
             old_ml = param_Ml.value
```

### Comparing `sourcespec-1.7/sourcespec/ssp_output.py` & `sourcespec-1.8/sourcespec/ssp_output.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,30 +5,31 @@
 
 :copyright:
     2012 Claudio Satriano <satriano@ipgp.fr>
 
     2013-2014 Claudio Satriano <satriano@ipgp.fr>,
               Emanuela Matrullo <matrullo@geologie.ens.fr>
 
-    2015-2023 Claudio Satriano <satriano@ipgp.fr>
+    2015-2024 Claudio Satriano <satriano@ipgp.fr>
 :license:
     CeCILL Free Software License Agreement v2.1
     (http://www.cecill.info/licences.en.html)
 """
 import os
+import shutil
 import contextlib
 import logging
-import numpy as np
 from collections.abc import Mapping
 from datetime import datetime
 from tzlocal import get_localzone
+import numpy as np
 from sourcespec.ssp_qml_output import write_qml
 from sourcespec.ssp_sqlite_output import write_sqlite
 from sourcespec._version import get_versions
-logger = logging.getLogger(__name__.split('.')[-1])
+logger = logging.getLogger(__name__.rsplit('.', maxsplit=1)[-1])
 
 
 def _write_author_and_agency_to_parfile(config, parfile):
     author_str = empty_author_str = '\n*** Author:'
     if config.author_name is not None:
         author_str += f' {config.author_name}'
     if config.author_email is not None:
@@ -69,63 +70,67 @@
     Write station source parameters to file.
 
     Note: this format is deprecated and will not evolve anymore
     (e.g., including new parameters or new way of computing statistics).
     """
     if not os.path.exists(config.options.outdir):
         os.makedirs(config.options.outdir)
-    evid = config.hypo.evid
+    evid = config.event.event_id
     parfilename = os.path.join(
         config.options.outdir, f'{evid}.ssp.out')
-    with open(parfilename, 'w') as parfile:
+    with open(parfilename, 'w', encoding='utf-8') as parfile:
         parfile.write(
             '*** Note: this file is deprecated and might not contain all the '
             'output information. ***\n')
         parfile.write(
             '*** It will be removed in future versions of SourceSpec. ***\n')
         parfile.write(
             '*** Please look at the YAML file in this directory. ***\n')
 
-        hypo = config.hypo
+        evid = config.event.event_id
+        hypo = config.event.hypocenter
+        evlo = hypo.longitude.value_in_deg
+        evla = hypo.latitude.value_in_deg
+        evdp = hypo.depth.value_in_km
         parfile.write(
-            f'{hypo.evid} lon {hypo.longitude:8.3f} lat {hypo.latitude:7.3f} '
-            f'depth {hypo.depth:5.1f} km orig_time {hypo.origin_time}\n\n')
+            f'{evid} lon {evlo:8.3f} lat {evla:7.3f} depth {evdp:5.1f} km '
+            f'orig_time {hypo.origin_time}\n\n')
         parfile.write('*** Station source parameters ***\n')
         parfile.write(
             '*** Note: outliers are prepended by a star (*) symbol ***\n')
         parkeys = (
             'Mw', 'fc', 't_star', 'Qo', 'Mo',
-            'bsd', 'ra', 'hyp_dist', 'az', 'Er'
-        )
-        formats = dict(
-            Mo='{:.3e} ',
-            Er='{:.3e} ',
-            hyp_dist='{:7.3f} ',
-            az='{:7.3f} ',
-            Mw='{:6.3f} ',
-            fc='{:6.3f} ',
-            bsd='{:.3e} ',
-            ra='{:8.3f} ',
-            t_star='{:6.3f} ',
-            Qo='{:7.1f} ',
-            Ml='{:6.3f} '
-        )
-        formats_none = dict(
-            Mo='{:>9} ',
-            Er='{:>9} ',
-            hyp_dist='{:>7} ',
-            az='{:>7} ',
-            Mw='{:>6} ',
-            fc='{:>6} ',
-            bsd='{:>9} ',
-            ra='{:>8} ',
-            t_star='{:>6} ',
-            Qo='{:>7} ',
-            Ml='{:>6} '
+            'ssd', 'ra', 'hyp_dist', 'az', 'Er'
         )
+        formats = {
+            'Mo': '{:.3e} ',
+            'Er': '{:.3e} ',
+            'hyp_dist': '{:7.3f} ',
+            'az': '{:7.3f} ',
+            'Mw': '{:6.3f} ',
+            'fc': '{:6.3f} ',
+            'ssd': '{:.3e} ',
+            'ra': '{:8.3f} ',
+            't_star': '{:6.3f} ',
+            'Qo': '{:7.1f} ',
+            'Ml': '{:6.3f} '
+        }
+        formats_none = {
+            'Mo': '{:>9} ',
+            'Er': '{:>9} ',
+            'hyp_dist': '{:>7} ',
+            'az': '{:>7} ',
+            'Mw': '{:>6} ',
+            'fc': '{:>6} ',
+            'ssd': '{:>9} ',
+            'ra': '{:>8} ',
+            't_star': '{:>6} ',
+            'Qo': '{:>7} ',
+            'Ml': '{:>6} '
+        }
         stationpar = sspec_output.station_parameters
         for statId in sorted(stationpar.keys()):
             par = stationpar[statId]
             parfile.write(f'{statId:>15} {par.instrument_type:>6}\t')
             for key in parkeys:
                 if key == 'az':
                     _pkey = key
@@ -251,37 +256,38 @@
         s = _value_error_str(ra_mean, ra_error, '{:.3f}')
         parfile.write(f'Source radius: {s} m\n')
         ra_mean_weight = means_weight['radius']
         ra_error_weight = errors_weight['radius']
         s = _value_error_str(ra_mean_weight, ra_error_weight, '{:.3f}')
         parfile.write(f'Source radius (weighted): {s} m\n')
 
-        bsd_mean = means['bsd']
-        bsd_error = errors['bsd']
-        s = _value_error_str(bsd_mean, bsd_error, '{:.3e}')
-        parfile.write(f'Brune stress drop: {s} MPa\n')
-        bsd_mean_weight = means_weight['bsd']
-        bsd_error_weight = errors_weight['bsd']
-        s = _value_error_str(bsd_mean_weight, bsd_error_weight, '{:.3e}')
-        parfile.write(f'Brune stress drop (weighted): {s} MPa\n')
+        ssd_mean = means['ssd']
+        ssd_error = errors['ssd']
+        s = _value_error_str(ssd_mean, ssd_error, '{:.3e}')
+        parfile.write(f'Static stress drop: {s} MPa\n')
+        ssd_mean_weight = means_weight['ssd']
+        ssd_error_weight = errors_weight['ssd']
+        s = _value_error_str(ssd_mean_weight, ssd_error_weight, '{:.3e}')
+        parfile.write(f'Static stress drop (weighted): {s} MPa\n')
 
         Ml_mean = means.get('Ml', None)
         Ml_error = errors.get('Ml', None)
         if Ml_mean is not None:
             s = _value_error_str(Ml_mean, Ml_error, '{:.3f}')
             parfile.write(f'Ml: {s}\n')
 
         Er_mean = means['Er']
         Er_error = errors['Er']
         s = _value_error_str(Er_mean, Er_error, '{:.3e}')
         parfile.write(f'Er: {s} N·m\n')
 
         parfile.write(f'\n*** SourceSpec: {get_versions()["version"]}')
         parfile.write(
-            f'\n*** Run completed on: {config.end_of_run} {config.end_of_run_tz}')
+            f'\n*** Run completed on: {config.end_of_run} '
+            f'{config.end_of_run_tz}')
         if config.options.run_id:
             parfile.write(f'\n*** Run ID: {config.options.run_id}')
         _write_author_and_agency_to_parfile(config, parfile)
 
     logger.info(f'Output written to file: {parfilename}')
 
 
@@ -296,15 +302,15 @@
     target_dict = {
         key: (fmt.format(value)
               if fmt is not None and key in value_uncertainty_keys
               else value)
         for key, value in dict_like.items()
         if not key.startswith('_') and value is not None
     }
-    indent = ' '*2*level
+    indent = ' ' * 2 * level
     # use oneliners for dict-like objects containing value and uncertainty keys
     if set(target_dict.keys()).intersection(set(value_uncertainty_keys)):
         oneliner = str(target_dict).replace("'", "")
         return f'{indent}{oneliner}\n'
     lines = ''
     for key, value in target_dict.items():
         if key.startswith('_') or value is None:
@@ -313,64 +319,97 @@
             if level == 0:
                 lines += '\n'
             with contextlib.suppress(KeyError):
                 comment = comments[key]
                 for line in comment.split('\n'):
                     lines += f'# {line}\n'
             lines += f'{indent}{key}:\n'
-            lines += _dict2yaml(value, level+1)
+            lines += _dict2yaml(value, level + 1)
         else:
             lines += f'{indent}{key}: {value}\n'
     return lines
 
 
 def _write_yaml(config, sspec_output):
     """Write sspec output in a YAML file."""
     if not os.path.exists(config.options.outdir):
         os.makedirs(config.options.outdir)
-    evid = config.hypo.evid
+    evid = config.event.event_id
     yamlfilename = os.path.join(config.options.outdir, f'{evid}.ssp.yaml')
     lines = _dict2yaml(sspec_output)
-    with open(yamlfilename, 'w') as fp:
-        comment = sspec_output._comments['begin']
-        for line in comment.split('\n'):
-            fp.write(f'# {line}\n')
+    comments = sspec_output.get('_comments', {})
+    with open(yamlfilename, 'w', encoding='utf-8') as fp:
+        begin_comment = comments.get('begin', None)
+        if begin_comment is not None:
+            for line in begin_comment.split('\n'):
+                fp.write(f'# {line}\n')
         fp.write(lines)
     logger.info(f'Output written to file: {yamlfilename}')
 
 
-def _write_hypo(config, sspec_output):
+def _write_hypo71(config, sspec_output):
     if not config.options.hypo_file:
         return
-    with open(config.options.hypo_file, 'r') as fp:
+    if config.hypo_file_format != 'hypo71':
+        return
+    with open(config.options.hypo_file, 'r', encoding='ascii') as fp:
         line = fp.readline()
         # Check if first 10 digits of the line contain characters
         if any(c.isalpha() for c in line[:10]):
             line1 = line
             line = fp.readline()
         line = list(line)
-
     summary_values = sspec_output.reference_values()
     mw_str = f'{summary_values["Mw"]:03.2f}'
     Ml = summary_values.get('Ml', None)
-    ml_str = f'{Ml:03.2f}' if Ml is not None and ~np.isnan(Ml) else ' '*4
+    ml_str = f'{Ml:03.2f}' if Ml is not None and ~np.isnan(Ml) else ' ' * 4
     for i in range(4):
-        line[49+i] = mw_str[0+i]
-        # line[45+i] = mw_str[0+i]
-        line[69+i] = ml_str[0+i]
+        line[49 + i] = mw_str[0 + i]
+        # line[45 + i] = mw_str[0 + i]
+        line[69 + i] = ml_str[0 + i]
     outline = ''.join(line)
-    evid = config.hypo.evid
+    evid = config.event.event_id
     hypo_file_out = os.path.join(config.options.outdir, f'{evid}.ssp.h')
-    with open(hypo_file_out, 'w') as fp:
+    with open(hypo_file_out, 'w', encoding='ascii') as fp:
         with contextlib.suppress(Exception):
             fp.write(line1)
         fp.write(outline)
     logger.info(f'Hypo file written to: {hypo_file_out}')
 
 
+def _make_symlinks(config):
+    """Make symlinks to input files into output directory."""
+    # Windows does not support symlinks
+    if os.name == 'nt':
+        return
+    outdir = config.options.outdir
+    out_data_dir = os.path.join(outdir, 'input_files')
+    rel_path = os.path.relpath(config.workdir, out_data_dir)
+    os.makedirs(out_data_dir, exist_ok=True)
+    filelist =\
+        list(config.options.trace_path) +\
+        [
+            config.options.station_metadata,
+            config.options.hypo_file,
+            config.options.pick_file,
+            config.options.qml_file,
+        ]
+    for filename in filelist:
+        if filename is None or not os.path.exists(filename):
+            continue
+        basename = os.path.basename(filename)
+        linkname = os.path.join(out_data_dir, basename)
+        if os.path.isfile(linkname) or os.path.islink(linkname):
+            os.remove(linkname)
+        elif os.path.isdir(linkname):
+            shutil.rmtree(linkname, ignore_errors=True)
+        filename = os.path.join(rel_path, filename)
+        os.symlink(filename, linkname)
+
+
 def write_output(config, sspec_output):
     """Write results into different formats."""
     # Add run info to output object
     run_info = sspec_output.run_info
     run_info.SourceSpec_version = get_versions()['version']
     config.end_of_run = datetime.now()
     tz = get_localzone()
@@ -379,17 +418,35 @@
     if config.options.run_id:
         run_info.run_id = config.options.run_id
     run_info.author_name = config.author_name
     run_info.author_email = config.author_email
     run_info.agency_full_name = config.agency_full_name
     run_info.agency_short_name = config.agency_short_name
     run_info.agency_url = config.agency_url
+    # Symlink input files into output directory
+    _make_symlinks(config)
     # Write to parfile (deprecated)
     _write_parfile(config, sspec_output)
     # Write to YAML file
     _write_yaml(config, sspec_output)
     # Write to SQLite database, if requested
     write_sqlite(config, sspec_output)
     # Write to hypo file, if requested
-    _write_hypo(config, sspec_output)
+    _write_hypo71(config, sspec_output)
     # Write to quakeml file, if requested
     write_qml(config, sspec_output)
+
+
+def save_spectra(config, spec_st):
+    """Save spectra to file."""
+    if not config.save_spectra:
+        return
+    outfile = os.path.join(
+        config.options.outdir,
+        f'{config.event.event_id}.spectra.hdf5'
+    )
+    spec_st.sort()
+    for spec in spec_st:
+        spec.stats.software = 'SourceSpec'
+        spec.stats.software_version = get_versions()['version']
+    spec_st.write(outfile)
+    logger.info(f'Spectra saved to: {outfile}')
```

### Comparing `sourcespec-1.7/sourcespec/ssp_parse_arguments.py` & `sourcespec-1.8/sourcespec/ssp_parse_arguments.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 # -*- coding: utf-8 -*-
 # SPDX-License-Identifier: CECILL-2.1
 """
 Argument parser for sourcespec.
 
 :copyright:
-    2021-2023 Claudio Satriano <satriano@ipgp.fr>
+    2021-2024 Claudio Satriano <satriano@ipgp.fr>
 :license:
     CeCILL Free Software License Agreement v2.1
     (http://www.cecill.info/licences.en.html)
 """
 import sys
 from argparse import ArgumentParser, RawTextHelpFormatter
 from itertools import zip_longest
 from sourcespec._version import get_versions
 
 
 def _parse_values(value_str):
     # Lazy-import for speed
+    # pylint: disable=import-outside-toplevel
     import numpy as np
     if value_str[0] == 'i':
         value_str = value_str[1:]
         val_min, val_max, val_step =\
             tuple(map(float, value_str.rstrip(',').split(',')))
         # we add a small number to val_max to make sure
         # it is included by np.arange()
@@ -83,35 +84,50 @@
     )
     group.add_argument(
         '-U', '--updateconf', dest='updateconf',
         action='store', default=None,
         help='update an existing config file from a previous version',
         metavar='FILE'
     )
+    group.add_argument(
+        '-u', '--updatedb', dest='updatedb',
+        action='store', default=None,
+        help='update an existing SourceSpec database from a previous version',
+        metavar='DATABASE_FILE'
+    )
+    group.add_argument(
+        '-y', '--samplesspevent', dest='samplesspevent',
+        action='store_true', default=False,
+        help='write sample SourceSpec Event File and exit'
+    )
     parser.add_argument(
         '-c', '--configfile', dest='config_file',
         action='store', default='source_spec.conf',
         help='load configuration from FILE (default: source_spec.conf)',
         metavar='FILE'
     )
     group.add_argument(
         '-t', '--trace_path', nargs=nargs,
-        help='path to trace file(s) or trace dir'
+        help='path to trace file(s) or trace dir. It can be any format\n'
+             'supported by ObsPy (e.g. miniSEED, SAC, etc.), a directory\n'
+             'containing such files, or a TAR(GZ) or ZIP archive containing\n'
+             'such files'
     )
     parser.add_argument(
         '-q', '--qmlfile', dest='qml_file',
         action='store', default=None,
         help='get picks and hypocenter information from QuakeML FILE',
         metavar='FILE'
     )
     parser.add_argument(
         '-H', '--hypocenter', dest='hypo_file',
         action='store', default=None,
         help='get hypocenter information from FILE.\n'
-             'Supported formats: HYPO71, HYPOINVERSE-2000.\n'
+             'Supported formats: SourceSpec Event File, HYPO71,\n'
+             'HYPOINVERSE-2000.\n'
              'If this file contains picks, they will be parsed as well.',
         metavar='FILE'
     )
     parser.add_argument(
         '-p', '--pickfile', dest='pick_file',
         action='store', default=None,
         help='get picks from FILE. Supported formats: HYPO71',
@@ -131,15 +147,16 @@
         action='store', default=None,
         help='event name (used for plots and output files) ',
         metavar='NAME'
     )
     parser.add_argument(
         '-e', '--evid', dest='evid',
         action='store', default=None,
-        help='get evid from catalog', metavar='EVID'
+        help='select this EVID from QuakeML or SourceSpec Event File',
+        metavar='EVID'
     )
     parser.add_argument(
         '-s', '--station', dest='station',
         action='store', default=None,
         help='only use this station', metavar='STATION'
     )
     return parser
@@ -156,23 +173,34 @@
     )
 
 
 def _update_parser_for_source_spec(parser):
     parser.add_argument(
         '-o', '--outdir', dest='outdir',
         action='store', default='sspec_out',
-        help='save output to OUTDIR (default: sspec_out)',
+        help='save output to OUTDIR (default: sspec_out).\n'
+             'The results are further organized in event subdirectories\n'
+             'named after the event id',
         metavar='OUTDIR'
     )
     parser.add_argument(
         '-r', '--run_id', dest='run_id',
         action='store', default='',
-        help='string identifying current run (default: "")',
+        help='string identifying current run (default: none)\n'
+             'If specified, it will be appended to the event directory name\n'
+             'unless the option "-R" is used, in which case it will be used\n'
+             'as a subdirectory of the event directory.',
         metavar='RUN_ID'
     )
+    parser.add_argument(
+        '-R', '--run_id_subdir', dest='run_id_subdir',
+        action='store_true', default=False,
+        help='use run_id as a subdirectory of the event directory\n'
+             '(default: False)'
+    )
 
 
 def _update_parser_for_source_model(parser):
     parser.add_argument(
         '-f', '--fmin', dest='fmin', action='store',
         type=float, default='0.01',
         help='minimum frequency (Hz, default 0.01)',
@@ -247,15 +275,15 @@
                   options.t_star, options.alpha]
         oplist = list(zip_longest(*oplist))
         # Unzip and convert tuple to lists:
         oplist = list(map(list, zip(*oplist)))
         for opt in oplist:
             for n, x in enumerate(opt):
                 if x is None:
-                    opt[n] = opt[n-1]
+                    opt[n] = opt[n - 1]
 
     options.fc, options.mag, options.Mo, options.t_star, options.alpha = \
         oplist
     # Add unused options (required by source_spec):
     options.correction = False
     options.outdir = '.'
```

### Comparing `sourcespec-1.7/sourcespec/ssp_plot_params_stats.py` & `sourcespec-1.8/sourcespec/ssp_plot_params_stats.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 # -*- coding: utf-8 -*-
 # SPDX-License-Identifier: CECILL-2.1
 """
 Plot parameter statistics.
 
 :copyright:
-    2022-2023 Claudio Satriano <satriano@ipgp.fr>
+    2022-2024 Claudio Satriano <satriano@ipgp.fr>
 :license:
     CeCILL Free Software License Agreement v2.1
     (http://www.cecill.info/licences.en.html)
 """
 import os
 import contextlib
+import logging
 import numpy as np
 import matplotlib
 import matplotlib.pyplot as plt
 import matplotlib.patheffects as mpe
-import logging
 
 from sourcespec._version import get_versions
 from sourcespec.savefig import savefig
-logger = logging.getLogger(__name__.split('.')[-1])
+logger = logging.getLogger(__name__.rsplit('.', maxsplit=1)[-1])
 # Reduce logging level for Matplotlib to avoid DEBUG messages
 mpl_logger = logging.getLogger('matplotlib')
 mpl_logger.setLevel(logging.WARNING)
 
 
 class PlotParam():
+    """A plot parameter."""
     def __init__(self, name, unit, color):
         self.name = name
         self.unit = unit
         self.color = color
 
 
 def box_plots(config, sspec_output):
@@ -40,28 +41,29 @@
     matplotlib.rcParams['pdf.fonttype'] = 42  # to edit text in Illustrator
 
     plot_params = {
         'Mw': PlotParam('Mw', None, '#EE5835'),
         'fc': PlotParam('Corner Frequency', 'Hz', '#6FBA6C'),
         't_star': PlotParam('t-star', 's', '#9EBAE2'),
         'radius': PlotParam('Source Radius', 'm', '#FAAC64'),
-        'bsd': PlotParam('Brune Stress Drop', 'MPa', '#D4ADD2'),
+        'ssd': PlotParam('Static Stress Drop', 'MPa', '#D4ADD2'),
         'Qo': PlotParam('Quality Factor', None, '#C07131'),
         'Er': PlotParam('Radiated Energy', 'N·m', '#00E3E9'),
+        'sigma_a': PlotParam('Apparent Stress', 'MPa', '#943B99'),
         'Ml': PlotParam('Ml', None, '#FC8384')
     }
     npars = len(plot_params)
 
     path_effect = [
         mpe.Stroke(linewidth=5, foreground='black'),
         mpe.Stroke(foreground='white', alpha=1),
         mpe.Normal()
     ]
 
-    fig, axes = plt.subplots(npars, 1, figsize=(8, 9), dpi=300)
+    fig, axes = plt.subplots(npars, 1, figsize=(8, 10), dpi=300)
     fig.set_tight_layout(True)
     # Create an invisible axis and use it for title and footer
     ax0 = fig.add_subplot(111, label='ax0')
     ax0.set_axis_off()
     for ax, param in zip(axes, plot_params.keys()):
         plot_param = plot_params[param]
         values = sspec_output.value_array(param)
@@ -70,49 +72,63 @@
         values = values[~np.isinf(values)]
         if len(values) == 0:
             ax.set_visible(False)
             continue
         vmean = np.mean(values)
         # remove values that are very far from the mean
         # (otherwise plot is too compressed)
-        _newvalues = values[np.abs(values-vmean)/vmean < 10]
+        _newvalues = values[np.abs(values - vmean) / vmean < 10]
         if len(_newvalues) > 0:
             values = _newvalues
+        min_values = np.min(values)
+        max_values = np.max(values)
         # use logscale if values span a large interval, avoid zero values
-        min_values = np.min(values) or 1e-10
-        if max(values)/min_values > 50:
+        if max_values / min_values > 50:
+            if min_values == 0:
+                min_values = 1e-10
             values = values[values != 0]
             ax.set_xscale('log')
         whiskers = config.nIQR
         if whiskers is None:
             whiskers = (0, 100)
         bplot = ax.boxplot(
             values, vert=False, whis=whiskers,
             widths=0.7, patch_artist=True)
         ax.scatter(
             values, np.ones_like(values), color='dimgray', edgecolor='white',
             zorder=10)
+        # if values are very close to each other, add some margin
+        margin = 0.001 * vmean
+        if max_values - min_values < margin:
+            min_values -= margin
+            max_values += margin
+            ax.set_xlim(min_values, max_values)
         for box in bplot['boxes']:
             box.set_facecolor(plot_param.color)
         for line in bplot['medians']:
             line.set_color('white')
             line.set_linewidth(2)
             line.set_path_effects(path_effect)
         if plot_param.unit is None:
             ax.set_xlabel(f'{plot_param.name}')
         else:
             ax.set_xlabel(f'{plot_param.name} ({plot_param.unit})')
         ax.tick_params(left=False, labelleft=False)
         ax.minorticks_on()
 
     # Add event information as a title
-    hypo = config.hypo
-    textstr = (
-        f'evid: {hypo.evid}\nlon: {hypo.longitude:.3f} '
-        f'lat: {hypo.latitude:.3f} depth: {hypo.depth:.1f} km'
+    evid = config.event.event_id
+    hypo = config.event.hypocenter
+    ev_lon = hypo.longitude.value_in_deg
+    ev_lat = hypo.latitude.value_in_deg
+    ev_depth = hypo.depth.value_in_km
+    textstr = f'{config.options.evname} — ' if config.options.evname else ''
+    textstr += (
+        f'evid: {evid}\n'
+        f'lon: {ev_lon:.3f} lat: {ev_lat:.3f} depth: {ev_depth:.1f} km'
     )
     with contextlib.suppress(AttributeError):
         textstr += f' time: {hypo.origin_time.format_iris_web_service()}'
     ax0.text(
         0., 1.08, textstr, fontsize=10, linespacing=1.5,
         ha='left', va='top', transform=ax0.transAxes)
     textstr = (
@@ -143,15 +159,15 @@
     if config.plot_show:
         plt.show()
     if config.plot_save:
         _savefig(config, fig)
 
 
 def _savefig(config, fig):
-    evid = config.hypo.evid
+    evid = config.event.event_id
     figfile_base = os.path.join(config.options.outdir, f'{evid}.boxplot.')
     fmt = config.plot_save_format
     if fmt == 'pdf_multipage':
         fmt = 'pdf'
     figfile = f'{figfile_base}{fmt}'
     savefig(fig, figfile, fmt, bbox_inches='tight')
     config.figures['boxplots'].append(figfile)
```

### Comparing `sourcespec-1.7/sourcespec/ssp_plot_spectra.py` & `sourcespec-1.8/sourcespec/ssp_plot_spectra.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,60 +5,66 @@
 
 :copyright:
     2012 Claudio Satriano <satriano@ipgp.fr>
 
     2013-2014 Claudio Satriano <satriano@ipgp.fr>,
               Emanuela Matrullo <matrullo@geologie.ens.fr>
 
-    2015-2023 Claudio Satriano <satriano@ipgp.fr>
+    2015-2024 Claudio Satriano <satriano@ipgp.fr>
 :license:
     CeCILL Free Software License Agreement v2.1
     (http://www.cecill.info/licences.en.html)
 """
 import os
 import math
 import logging
 import warnings
 import contextlib
 from collections import defaultdict
 from obspy import Stream
-from sourcespec.ssp_util import spec_minmax, moment_to_mag, mag_to_moment
-from sourcespec.savefig import savefig
-from sourcespec._version import get_versions
 import matplotlib
 import matplotlib.pyplot as plt
 from matplotlib.backends.backend_pdf import PdfPages
 import matplotlib.patheffects as PathEffects
-logger = logging.getLogger(__name__.split('.')[-1])
+from sourcespec.ssp_util import spec_minmax, moment_to_mag, mag_to_moment
+from sourcespec.savefig import savefig
+from sourcespec._version import get_versions
+logger = logging.getLogger(__name__.rsplit('.', maxsplit=1)[-1])
 # Reduce logging level for Matplotlib to avoid DEBUG messages
 mpl_logger = logging.getLogger('matplotlib')
 mpl_logger.setLevel(logging.WARNING)
 
 
 synth_colors = [
     '#201F1F',
     '#94F75B',
     '#3EC2AA',
     '#FECC38',
     '#FC4384',
 ]
 
+STATION_TEXT_YPOS = None
+SNRATIO_TEXT_YPOS = None
+
 
 class PlotParams():
-    plot_type = None
-    stack_plots = False
-    nlines = 0
-    ncols = 0
-    freq_minmax = None
-    moment_minmax = None
-    mag_minmax = None
-    plotn = 0
-    figures = []
-    axes = None
-    ax0 = None
+    """Parameters for plotting spectra."""
+
+    def __init__(self):
+        self.plot_type = None
+        self.stack_plots = False
+        self.nlines = 0
+        self.ncols = 0
+        self.freq_minmax = None
+        self.moment_minmax = None
+        self.mag_minmax = None
+        self.plotn = 0
+        self.figures = []
+        self.axes = []
+        self.ax0 = None
 
     def set_plot_params(self, config, spec_st, specnoise_st):
         """Determine the number of plots and axes min and max."""
         nplots = 0
         moment_minmax = None
         freq_minmax = None
         _spec_st = (
@@ -74,19 +80,19 @@
             if specnoise_st:
                 specnoise_sel = specnoise_st.select(
                     network=network, station=station, location=location)
                 if specnoise_sel[0].data.sum() != 0:
                     spec_st_sel += specnoise_sel
             for spec in spec_st_sel:
                 moment_minmax, freq_minmax = spec_minmax(
-                    spec.data, spec.get_freq(), moment_minmax, freq_minmax)
+                    spec.data, spec.freq, moment_minmax, freq_minmax)
             # increment the number of plots,
             # based on the number of uniqs band+instrument codes
             nplots += len({x.stats.channel[:-1] for x in spec_st_sel})
-        nlines = int(math.ceil(nplots/self.ncols))
+        nlines = int(math.ceil(nplots / self.ncols))
         maxlines = config.plot_spectra_maxrows
         self.nlines = min(nlines, maxlines)
         if self.plot_type != 'weight':
             moment_minmax[1] *= 10
             self.mag_minmax = moment_to_mag(moment_minmax)
         self.freq_minmax = freq_minmax
         self.moment_minmax = moment_minmax
@@ -99,29 +105,29 @@
     figsize = (16, 9) if nlines <= 3 or stack_plots else (16, 18)
     dpi = 100 if config.plot_show else 300
     fig = plt.figure(figsize=figsize, dpi=dpi)
     # Create an invisible axis and use it for title and footer
     ax0 = fig.add_subplot(111, label='ax0')
     ax0.set_axis_off()
     # Add event information as a title
-    hypo = config.hypo
-    textstr = (
-        f'evid: {hypo.evid} lon: {hypo.longitude:.3f} '
-        f'lat: {hypo.latitude:.3f} depth: {hypo.depth:.1f} km'
+    evid = config.event.event_id
+    hypo = config.event.hypocenter
+    ev_lon = hypo.longitude.value_in_deg
+    ev_lat = hypo.latitude.value_in_deg
+    ev_depth = hypo.depth.value_in_km
+    textstr = f'{config.options.evname} — ' if config.options.evname else ''
+    textstr += (
+        f'evid: {evid} '
+        f'lon: {ev_lon:.3f} lat: {ev_lat:.3f} depth: {ev_depth:.1f} km'
     )
     with contextlib.suppress(AttributeError):
         textstr += f' time: {hypo.origin_time.format_iris_web_service()}'
     ax0.text(
         0., 1.06, textstr, fontsize=12,
         ha='left', va='top', transform=ax0.transAxes)
-    if config.options.evname is not None:
-        textstr = config.options.evname
-        ax0.text(
-            0., 1.1, textstr, fontsize=14,
-            ha='left', va='top', transform=ax0.transAxes)
     # Add code and author information at the figure bottom
     textstr = f'SourceSpec v{get_versions()["version"]} '
     if not stack_plots:
         textstr += (
             f'- {config.end_of_run.strftime("%Y-%m-%d %H:%M:%S")} '
             f'{config.end_of_run_tz} '
         )
@@ -140,16 +146,16 @@
         textstr2 += config.agency_full_name
     if textstr2 != '':
         textstr = f'{textstr}\n{textstr2} '
     ax0.text(
         1., -0.1, textstr, fontsize=10, linespacing=1.5,
         ha='right', va='top', transform=ax0.transAxes)
     axes = []
-    for n in range(nlines*ncols):
-        plotn = n+1
+    for n in range(nlines * ncols):
+        plotn = n + 1
         # ax1 has moment units (or weight)
         if plotn == 1:
             ax = (
                 fig.add_subplot(1, 1, 1, label='ax')
                 if stack_plots
                 else fig.add_subplot(nlines, ncols, plotn)
             )
@@ -181,47 +187,60 @@
     fig.subplots_adjust(hspace=.025, wspace=.03)
     plot_params.figures.append(fig)
     plot_params.axes = axes
     plot_params.ax0 = ax0
     plot_params.plotn = 0
 
 
-def _savefig(config, plottype, figures):
-    evid = config.hypo.evid
+# Keep track of saved figure codes to avoid saving the same figure twice
+SAVED_FIGURE_CODES = []
+# Bounding box for saving figures
+BBOX = None
+
+
+def _savefig(config, plottype, figures, force_numbering=False):
+    global BBOX  # pylint: disable=global-statement
+    evid = config.event.event_id
     if plottype == 'regular':
         suffix = '.ssp.'
         message = 'Spectral'
     elif plottype == 'weight':
         suffix = '.sspweight.'
         message = 'Weight'
     figfile_base = os.path.join(config.options.outdir, evid + suffix)
     fmt = config.plot_save_format
-    pad_inches = matplotlib.rcParams['savefig.pad_inches']
-    bbox = figures[0].get_tightbbox(figures[0].canvas.get_renderer())
-    bbox = bbox.padded(pad_inches)
+    if BBOX is None:
+        pad_inches = matplotlib.rcParams['savefig.pad_inches']
+        BBOX = figures[0].get_tightbbox(figures[0].canvas.get_renderer())
+        BBOX = BBOX.padded(pad_inches)
     nfigures = len(figures)
-    if nfigures == 1 or fmt == 'pdf_multipage':
+    if (nfigures == 1 or fmt == 'pdf_multipage') and not force_numbering:
         if fmt == 'pdf_multipage':
             figfile = f'{figfile_base}pdf'
             pdf = PdfPages(figfile)
         else:
             figfile = figfile_base + fmt
         figfiles = [figfile, ]
     else:
         figfiles = [f'{figfile_base}{n:02d}.{fmt}' for n in range(nfigures)]
     for n in range(nfigures):
+        figcode = f'{plottype}_{n}'
+        if figcode in SAVED_FIGURE_CODES:
+            continue
         if fmt == 'pdf_multipage':
-            pdf.savefig(figures[n], bbox_inches=bbox)
+            pdf.savefig(figures[n], bbox_inches=BBOX)
         else:
-            savefig(figures[n], figfiles[n], fmt, bbox_inches=bbox)
+            savefig(figures[n], figfiles[n], fmt, bbox_inches=BBOX)
         if not config.plot_show:
             plt.close(figures[n])
-    for figfile in figfiles:
-        logger.info(f'{message} plots saved to: {figfile}')
-    config.figures[f'spectra_{plottype}'] += figfiles
+            # dereference the figure to free up memory
+            figures[n] = None
+        SAVED_FIGURE_CODES.append(figcode)
+        config.figures[f'spectra_{plottype}'].append(figfiles[n])
+        logger.info(f'{message} plots saved to: {figfiles[n]}')
     if fmt == 'pdf_multipage':
         pdf.close()
 
 
 def _add_labels(plot_params):
     """
     Add xlabels to the last row plots.
@@ -229,39 +248,39 @@
     Add ylabels to the first and last columns.
     """
     plotn = plot_params.plotn
     ncols = plot_params.ncols
     plot_type = plot_params.plot_type
     axes = plot_params.axes
     # A row has "ncols" plots: the last row is from `plotn-ncols` to `plotn`
-    n0 = max(plotn-ncols, 0)
+    n0 = max(plotn - ncols, 0)
     for ax, ax2 in axes[n0:plotn]:
         ax.xaxis.set_tick_params(which='both', labelbottom=True)
         ax.set_xlabel('Frequency (Hz)')
     # Show the y-labels only for the first column
-    for i in range(0, len(axes)+ncols, ncols):
+    for i in range(0, len(axes) + ncols, ncols):
         try:
             ax = axes[i][0]
         except IndexError:
             continue
         try:
             # for ax2 we take the last column
-            ax2 = axes[i-1][1]
+            ax2 = axes[i - 1][1]
         except IndexError:
             continue
         ax.yaxis.set_tick_params(which='both', labelleft=True)
         ax.set_ylabel('Weight')
         if plot_type != 'weight':
             ax.set_ylabel('Seismic moment (N·m)')
             if ax2:
                 ax2.yaxis.set_tick_params(
                     which='both', labelright=True, pad=0, width=2)
                 ax2.set_ylabel('Magnitude')
     # still some work to do on the last plot
-    ax, ax2 = axes[plotn-1]
+    ax, ax2 = axes[plotn - 1]
     if ax2:
         ax2.yaxis.set_tick_params(
             which='both', labelright=True, pad=0, width=2)
         ax2.set_ylabel('Magnitude')
 
 
 def _color_lines(config, orientation, plotn, stack_plots):
@@ -281,15 +300,15 @@
         # root sum of squares spectrum, corrected
         color = 'red'
         linestyle = 'solid'
         linewidth = 2
     elif orientation == 'S':
         # synthetic spectrum
         color = (
-            synth_colors[(plotn-1) % len(synth_colors)]
+            synth_colors[(plotn - 1) % len(synth_colors)]
             if stack_plots
             else 'black'
         )
         linestyle = 'solid'
         linewidth = 2
     elif orientation == 'h':
         # root sum of squares spectrum, uncorrected
@@ -433,60 +452,65 @@
                    loc='lower left', borderaxespad=0, ncol=ncol1)
     # Make lines invisible
     for h in handles0 + handles1:
         h.set_visible(False)
 
 
 def _snratio_text(spec, ax, color, path_effects):
-    global snratio_text_ypos
+    global SNRATIO_TEXT_YPOS  # pylint: disable=global-statement
     if spec.stats.spectral_snratio is None:
         return
     snratio_text = f'S/N: {spec.stats.spectral_snratio:.1f}'
     ax.text(
-        0.95, snratio_text_ypos, snratio_text, ha='right', va='top',
+        0.95, SNRATIO_TEXT_YPOS, snratio_text, ha='right', va='top',
         fontsize=8, color=color, path_effects=path_effects,
         transform=ax.transAxes, zorder=20)
-    snratio_text_ypos -= 0.05
+    SNRATIO_TEXT_YPOS -= 0.05
 
 
 def _station_text(spec, ax, color, path_effects, stack_plots):
-    global station_text_ypos
     station_text = f'{spec.id[:-1]} {spec.stats.instrtype}'
     if not stack_plots:
         color = 'black'
     station_text += (
         f'\n{spec.stats.hypo_dist:.1f} km ({spec.stats.epi_dist:.1f} km)')
     if not ax.has_station_text or stack_plots:
         ax.text(
-            0.05, station_text_ypos, station_text,
+            0.05, STATION_TEXT_YPOS, station_text,
             horizontalalignment='left',
             verticalalignment='bottom',
             color=color,
             transform=ax.transAxes,
             zorder=50,
             path_effects=path_effects)
         ax.has_station_text = True
 
 
 def _params_text(spec, ax, color, path_effects, stack_plots):
-    global station_text_ypos
+    global STATION_TEXT_YPOS  # pylint: disable=global-statement
     if stack_plots:
-        params_text_ypos = station_text_ypos - 0.04
+        params_text_ypos = STATION_TEXT_YPOS - 0.04
     else:
-        params_text_ypos = 0.03
+        params_text_ypos = 0.02
         color = 'black'
     fc = spec.stats.par['fc']
     Mw = spec.stats.par['Mw']
     Mo = mag_to_moment(Mw)
     t_star = spec.stats.par['t_star']
+    try:
+        Er = spec.stats.par['Er']
+    except KeyError:
+        # Er might not be computed for noisy spectra
+        Er = None
     if 'par_err' in spec.stats.keys():
         fc_err_left, fc_err_right = spec.stats.par_err['fc']
         Mw_err_left, Mw_err_right = spec.stats.par_err['Mw']
         t_star_err_left, t_star_err_right =\
             spec.stats.par_err['t_star']
+        # Er has no error
     else:
         fc_err_left = fc_err_right = 0.
         Mw_err_left = Mw_err_right = 0.
         t_star_err_left = t_star_err_right = 0.
     Mo_text = f'Mo: {Mo:.2g}N·m'
     Mw_err_text = (
         f'±{Mw_err_left:.2f}'
@@ -502,21 +526,27 @@
     fc_text = f'fc: {fc:.2f}{fc_err_text}'
     t_star_err_text = (
         f'±{t_star_err_left:.2f}s'
         if round(t_star_err_left, 2) == round(t_star_err_right, 2)
         else f'[-{t_star_err_left:.2f},+{t_star_err_right:.2f}]s'
     )
     t_star_text = f't*: {t_star:.2f}{t_star_err_text}'
-    if len(fc_text+t_star_text) > 38:
+    Er_text = f'Er: {Er:.1e}N·m' if Er else ''
+    if len(fc_text + t_star_text) > 38:
         sep = '\n'
         params_text_ypos -= 0.01
-        station_text_ypos += 0.06
+        STATION_TEXT_YPOS += 0.06
     else:
         sep = ' '
-    params_text = f'{Mo_text} {Mw_text}\n{fc_text}{sep}{t_star_text}'
+    params_text = (
+        f'{Mo_text} {Mw_text}\n'
+        f'{fc_text}{sep}{t_star_text}'
+    )
+    if Er_text:
+        params_text += f'\n{Er_text}'
     ax.text(
         0.05, params_text_ypos, params_text,
         horizontalalignment='left',
         verticalalignment='bottom',
         color=color,
         fontsize=9,
         transform=ax.transAxes,
@@ -525,63 +555,62 @@
 
 
 def _plot_fc_and_mw(spec, ax, ax2):
     fc = spec.stats.par['fc']
     Mw = spec.stats.par['Mw']
     if 'par_err' in spec.stats.keys():
         fc_err_left, fc_err_right = spec.stats.par_err['fc']
-        fc_min = fc-fc_err_left
+        fc_min = fc - fc_err_left
         if fc_min < 0:
             fc_min = 0.01
         ax.axvspan(
-            fc_min, fc+fc_err_right, color='#bbbbbb', alpha=0.3, zorder=1)
+            fc_min, fc + fc_err_right, color='#bbbbbb', alpha=0.3, zorder=1)
         Mw_err_left, Mw_err_right = spec.stats.par_err['Mw']
         ax2.axhspan(
-            Mw-Mw_err_left, Mw+Mw_err_right, color='#bbbbbb',
+            Mw - Mw_err_left, Mw + Mw_err_right, color='#bbbbbb',
             alpha=0.3, zorder=1)
     ax.axvline(fc, color='#999999', linewidth=2., zorder=1)
 
 
 def _plot_spec(config, plot_params, spec, spec_noise):
     """Plot one spectrum (and its associated noise)."""
     plotn = plot_params.plotn
     plot_type = plot_params.plot_type
     stack_plots = plot_params.stack_plots
     axes = plot_params.axes
-    ax, ax2 = axes[plotn-1]
+    ax, ax2 = axes[plotn - 1]
     orientation = spec.stats.channel[-1]
     # Path effect to contour text in white
     path_effects = [PathEffects.withStroke(linewidth=3, foreground='white')]
     color, linestyle, linewidth =\
         _color_lines(config, orientation, plotn, stack_plots)
     # dim out ignored spectra
     alpha = 0.3 if spec.stats.ignore else 1.0
     if plot_type == 'regular':
         zorder = defaultdict(lambda: 20, {'S': 21, 'H': 22})
         ax.loglog(
-            spec.freq_log, spec.data_log, color=color, alpha=alpha,
+            spec.freq_logspaced, spec.data_logspaced, color=color, alpha=alpha,
             linestyle=linestyle, linewidth=linewidth,
             zorder=zorder[orientation])
         special_orientations = ['S', 's', 't', 'H', 'h']
         # Write spectral S/N for regular Z,N,E components
         if orientation not in special_orientations:
             _snratio_text(spec, ax, color, path_effects)
         # Plot fc and Mw if a synthetic spectrum S is available
         if orientation == 'S':
             _plot_fc_and_mw(spec, ax, ax2)
     elif plot_type == 'weight':
         ax.semilogx(
-            spec.get_freq(), spec.data, color=color, alpha=alpha,
-            zorder=20)
+            spec.freq, spec.data, color=color, alpha=alpha, zorder=20)
     else:
         raise ValueError(f'Unknown plot type: {plot_type}')
 
     if spec_noise:
         ax.loglog(
-            spec_noise.get_freq(), spec_noise.data,
+            spec_noise.freq, spec_noise.data,
             linestyle=':', linewidth=linewidth,
             color=color, alpha=alpha, zorder=20)
     if orientation == 'S':
         _params_text(spec, ax, color, path_effects, stack_plots)
     # station_text must be written after params_text, since it might move up
     # if params_text is too tall
     _station_text(spec, ax, color, path_effects, stack_plots)
@@ -592,33 +621,42 @@
     plotn = plot_params.plotn + 1
     nlines = plot_params.nlines
     ncols = plot_params.ncols
     # 'code' is band+instrument code
     network, station, location, code = specid.split('.')
     spec_st_sel = spec_st.select(
         network=network, station=station, location=location)
-    if plotn > nlines*ncols:
+    if plotn > nlines * ncols:
         # Add labels and legend before making a new figure
         _add_labels(plot_params)
         _add_legend(config, plot_params, spec_st, specnoise_st)
+        if (
+            config.plot_save_asap and
+            config.plot_save and not config.plot_show and
+            config.plot_save_format != 'pdf_multipage'
+        ):
+            # save figure here to free up memory
+            _savefig(
+                config, plot_params.plot_type, plot_params.figures,
+                force_numbering=True)
         _make_fig(config, plot_params)
         plotn = 1
     plot_params.plotn = plotn
     special_orientations = ['S', 's', 't', 'H', 'h']
     orientations = [sp.stats.channel[-1] for sp in spec_st_sel]
     # compute the number of instrument components (N, Z, E, 1, 2, ...)
     ncomponents = len(
         [o for o in orientations if o not in special_orientations])
-    global snratio_text_ypos
-    global station_text_ypos
-    snratio_text_ypos = 0.95
+    global SNRATIO_TEXT_YPOS  # pylint: disable=global-statement
+    global STATION_TEXT_YPOS  # pylint: disable=global-statement
+    SNRATIO_TEXT_YPOS = 0.95
     if plot_params.stack_plots:
-        station_text_ypos = 0.05 + 0.10*(plotn-1)
+        STATION_TEXT_YPOS = 0.05 + 0.10 * (plotn - 1)
     else:
-        station_text_ypos = 0.15
+        STATION_TEXT_YPOS = 0.20
     # sort specs by orientation letter, so that synthetic is plotted first
     # sort_order[...] gives 10 if the key is not present
     sort_order = defaultdict(lambda: 10, {'S': 0, 's': 1, 't': 2, 'H': 99})
     spec_st_sel_sort = sorted(
         spec_st_sel, key=lambda s: sort_order[s.stats.channel[-1]])
     for spec in spec_st_sel_sort:
         if spec.stats.channel[:-1] != code:
```

### Comparing `sourcespec-1.7/sourcespec/ssp_plot_stacked_spectra.py` & `sourcespec-1.8/sourcespec/ssp_plot_stacked_spectra.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 # -*- coding: utf-8 -*-
 # SPDX-License-Identifier: CECILL-2.1
 """
 Plot stacked spectra, along with summary inverted spectrum.
 
 :copyright:
-    2023 Claudio Satriano <satriano@ipgp.fr>
+    2023-2024 Claudio Satriano <satriano@ipgp.fr>
 :license:
     CeCILL Free Software License Agreement v2.1
     (http://www.cecill.info/licences.en.html)
 """
 import os
 import contextlib
 import logging
 import numpy as np
+import matplotlib
+import matplotlib.pyplot as plt
+import matplotlib.patheffects as PathEffects
 from sourcespec.ssp_util import moment_to_mag, mag_to_moment
 from sourcespec.ssp_spectral_model import spectral_model
 from sourcespec.savefig import savefig
 from sourcespec._version import get_versions
-import matplotlib
-import matplotlib.pyplot as plt
-import matplotlib.patheffects as PathEffects
-logger = logging.getLogger(__name__.split('.')[-1])
+logger = logging.getLogger(__name__.rsplit('.', maxsplit=1)[-1])
 # Reduce logging level for Matplotlib to avoid DEBUG messages
 mpl_logger = logging.getLogger('matplotlib')
 mpl_logger.setLevel(logging.WARNING)
 
 
 def _spectral_model_moment(freq, Mw, fc, t_star):
     return mag_to_moment(spectral_model(freq, Mw=Mw, fc=fc, t_star=t_star))
@@ -60,20 +60,20 @@
 def _plot_fc_and_mw(sspec_output, ax, ax2):
     fc = sspec_output.reference_values()['fc']
     fc_err_left, fc_err_right = sspec_output.reference_uncertainties()['fc']
     fc_min = fc - fc_err_left
     if fc_min < 0:
         fc_min = 0.01
     ax.axvspan(
-        fc_min, fc+fc_err_right, color='#bbbbbb', alpha=0.3, zorder=9)
+        fc_min, fc + fc_err_right, color='#bbbbbb', alpha=0.3, zorder=9)
     ax.axvline(fc, color='#999999', linewidth=2., zorder=10)
     Mw = sspec_output.reference_values()['Mw']
     Mw_err_left, Mw_err_right = sspec_output.reference_uncertainties()['Mw']
     ax2.axhspan(
-        Mw-Mw_err_left, Mw+Mw_err_right, color='#bbbbbb',
+        Mw - Mw_err_left, Mw + Mw_err_right, color='#bbbbbb',
         alpha=0.3, zorder=8)
 
 
 def _make_ax2(ax):
     ax2 = ax.twinx()
     # Move ax2 below ax
     ax.zorder = 2
@@ -113,16 +113,21 @@
     fc_text = (
         f'fc: {fc_value:.2f} [- {fc_err_left:.2f}, + {fc_err_right:.2f}] Hz')
     t_star_value = summary_values['t_star']
     t_star_err_left, t_star_err_right = summary_uncertainties['t_star']
     t_star_text = (
         f't*: {t_star_value:.2f} '
         f'[- {t_star_err_left:.2f}, + {t_star_err_right:.2f}] s')
+    Er_value = summary_values['Er']
+    Er_err_left, Er_err_right = summary_uncertainties['Er']
+    Er_text = (
+        f'Er: {Er_value:.1e} [- {Er_err_left:.1e}, + {Er_err_right:.1e}] N·m')
     params_text = (
-        f'Summary parameters:\n{Mo_text}\n{Mw_text}\n{fc_text}\n{t_star_text}'
+        'Summary parameters:\n'
+        f'{Mo_text}\n{Mw_text}\n{fc_text}\n{t_star_text}\n{Er_text}'
     )
     color = 'black'
     # Path effect to contour text in white
     path_effects = [PathEffects.withStroke(linewidth=3, foreground='white')]
     ax.text(
         0.05, 0.02, params_text,
         horizontalalignment='left',
@@ -133,22 +138,28 @@
         transform=ax.transAxes,
         zorder=50,
         path_effects=path_effects)
 
 
 def _add_title(config, ax):
     # Add event information as a title
-    hypo = config.hypo
-    textstr = (
-        f'evid: {hypo.evid}\nlon: {hypo.longitude:.3f} '
-        f'lat: {hypo.latitude:.3f} depth: {hypo.depth:.1f} km')
+    evid = config.event.event_id
+    hypo = config.event.hypocenter
+    ev_lon = hypo.longitude.value_in_deg
+    ev_lat = hypo.latitude.value_in_deg
+    ev_depth = hypo.depth.value_in_km
+    textstr = f'{config.options.evname} — ' if config.options.evname else ''
+    textstr += (
+        f'evid: {evid}\n'
+        f'lon: {ev_lon:.3f} lat: {ev_lat:.3f} depth: {ev_depth:.1f} km'
+    )
     with contextlib.suppress(AttributeError):
-        textstr += f'\ntime: {hypo.origin_time.format_iris_web_service()}'
+        textstr += f' time: {hypo.origin_time.format_iris_web_service()}'
     ax.text(
-        0., 1.15, textstr, fontsize=10, linespacing=1.5,
+        0., 1.10, textstr, fontsize=10, linespacing=1.5,
         ha='left', va='top', transform=ax.transAxes)
 
 
 def _add_code_author(config, ax):
     # Add code and author information to the figure bottom
     textstr = (
         f'SourceSpec v{get_versions()["version"]} '
@@ -173,15 +184,15 @@
     ypos = -0.15
     ax.text(
         1., ypos, textstr, fontsize=8, linespacing=1.5,
         ha='right', va='top', transform=ax.transAxes)
 
 
 def _savefig(config, fig):
-    evid = config.hypo.evid
+    evid = config.event.event_id
     figfile_base = os.path.join(config.options.outdir, evid)
     figfile_base += '.stacked_spectra.'
     fmt = config.plot_save_format
     if fmt == 'pdf_multipage':
         fmt = 'pdf'
     figfile = figfile_base + fmt
     if config.plot_show:
@@ -207,15 +218,15 @@
     fig, ax = _make_fig(config)
     color = 'red'
     alpha = 0.5
     linewidth = 2
     fmins = []
     fmaxs = []
     for spec in selected_specs:
-        freqs = spec.get_freq()
+        freqs = spec.freq
         spec_handle, = ax.loglog(
             freqs, spec.data, color=color, lw=linewidth,
             alpha=alpha, zorder=20)
         fmins.append(freqs.min())
         fmaxs.append(freqs.max())
     fmin = min(fmins)
     fmax = max(fmaxs)
```

### Comparing `sourcespec-1.7/sourcespec/ssp_plot_traces.py` & `sourcespec-1.8/sourcespec/ssp_plot_traces.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 # -*- coding: utf-8 -*-
 # SPDX-License-Identifier: CECILL-2.1
 """
 Trace plotting routine.
 
 :copyright:
-    2015-2023 Claudio Satriano <satriano@ipgp.fr>
+    2015-2024 Claudio Satriano <satriano@ipgp.fr>
 :license:
     CeCILL Free Software License Agreement v2.1
     (http://www.cecill.info/licences.en.html)
 """
 import os
 import contextlib
-import numpy as np
 import logging
+import numpy as np
 from obspy.core import Stream
-from sourcespec.savefig import savefig
-from sourcespec._version import get_versions
 import matplotlib
 import matplotlib.pyplot as plt
 from matplotlib.backends.backend_pdf import PdfPages
-import matplotlib.transforms as transforms
-import matplotlib.patches as patches
+from matplotlib import transforms
+from matplotlib import patches
 import matplotlib.patheffects as PathEffects
 from matplotlib.ticker import ScalarFormatter as sf
-logger = logging.getLogger(__name__.split('.')[-1])
+from sourcespec.savefig import savefig
+from sourcespec._version import get_versions
+logger = logging.getLogger(__name__.rsplit('.', maxsplit=1)[-1])
 # Reduce logging level for Matplotlib to avoid DEBUG messages
 mpl_logger = logging.getLogger('matplotlib')
 mpl_logger.setLevel(logging.WARNING)
 
 
-class ScalarFormatter(sf):  #NOQA
+class ScalarFormatter(sf):
+    """A ScalarFormatter with a custom format."""
     def _set_format(self, vmin=None, vmax=None):
+        # pylint: disable=unused-argument
         self.format = '%1.1f'
 
 
 phase_label_pos = {'P': 0.9, 'S': 0.93}
 phase_label_color = {'P': 'black', 'S': 'black'}
 
 
@@ -42,15 +44,15 @@
     """Determine the number of lines and columns of the plot."""
     # Remove the channel letter to determine the number of plots
     if config.plot_traces_ignored:
         nplots = len({tr.id[:-1] for tr in st})
     else:
         nplots = len({tr.id[:-1] for tr in st if not tr.stats.ignore})
     nplots = len({tr.id[:-1] for tr in st})
-    nlines = int(np.ceil(nplots/ncols))
+    nlines = int(np.ceil(nplots / ncols))
     nlines = min(nlines, maxlines)
     if nplots < ncols:
         ncols = 1
     return nlines, ncols
 
 
 def _make_fig(config, nlines, ncols):
@@ -59,27 +61,28 @@
     # vector formats (pdf, svg) do not have rasters
     dpi = 300 if config.plot_save_format == 'png' else 72
     fig = plt.figure(figsize=figsize, dpi=dpi)
     # Create an invisible axis and use it for title and footer
     ax0 = fig.add_subplot(111, label='ax0')
     ax0.set_axis_off()
     # Add event information as a title
-    hypo = config.hypo
-    textstr = (
-        f'evid: {hypo.evid} lon: {hypo.longitude:.3f} '
-        f'lat: {hypo.latitude:.3f} depth: {hypo.depth:.1f} km'
+    evid = config.event.event_id
+    hypo = config.event.hypocenter
+    ev_lon = hypo.longitude.value_in_deg
+    ev_lat = hypo.latitude.value_in_deg
+    ev_depth = hypo.depth.value_in_km
+    textstr = f'{config.options.evname} — ' if config.options.evname else ''
+    textstr += (
+        f'evid: {evid} '
+        f'lon: {ev_lon:.3f} lat: {ev_lat:.3f} depth: {ev_depth:.1f} km'
     )
     with contextlib.suppress(AttributeError):
         textstr += f' time: {hypo.origin_time.format_iris_web_service()}'
     ax0.text(0., 1.06, textstr, fontsize=12,
              ha='left', va='top', transform=ax0.transAxes)
-    if config.options.evname is not None:
-        textstr = config.options.evname
-        ax0.text(0., 1.1, textstr, fontsize=14,
-                 ha='left', va='top', transform=ax0.transAxes)
     # Add code and author information at the figure bottom
     textstr = f'SourceSpec v{get_versions()["version"]} '
     textstr2 = ''
     if config.author_name is not None:
         textstr2 += config.author_name
     elif config.author_email is not None:
         textstr2 += config.author_email
@@ -92,16 +95,16 @@
             textstr2 += ' - '
         textstr2 += config.agency_full_name
     if textstr2 != '':
         textstr = f'{textstr}\n{textstr2} '
     ax0.text(1., -0.1, textstr, fontsize=10, linespacing=1.5,
              ha='right', va='top', transform=ax0.transAxes)
     axes = []
-    for n in range(nlines*ncols):
-        plotn = n+1
+    for n in range(nlines * ncols):
+        plotn = n + 1
         if plotn == 1:
             ax = fig.add_subplot(nlines, ncols, plotn)
         else:
             ax = fig.add_subplot(nlines, ncols, plotn, sharex=axes[0])
         ax.grid(True, which='both', linestyle='solid', color='#DDDDDD',
                 zorder=0)
         ax.set_axisbelow(True)
@@ -114,113 +117,124 @@
         yfmt.set_powerlimits((-1, 1))
         ax.yaxis.set_major_formatter(yfmt)
         axes.append(ax)
     fig.subplots_adjust(hspace=.1, wspace=.20)
     return fig, axes
 
 
-def _savefig(config, figures):
-    evid = config.hypo.evid
+# Keep track of saved figure numbers to avoid saving the same figure twice
+SAVED_FIGURE_NUMBERS = []
+# Bounding box for saving figures
+BBOX = None
+
+
+def _savefig(config, figures, force_numbering=False):
+    global BBOX  # pylint: disable=global-statement
+    evid = config.event.event_id
     figfile_base = os.path.join(config.options.outdir, f'{evid}.traces.')
     fmt = config.plot_save_format
-    pad_inches = matplotlib.rcParams['savefig.pad_inches']
-    bbox = figures[0].get_tightbbox(figures[0].canvas.get_renderer())
-    bbox = bbox.padded(pad_inches)
+    if BBOX is None:
+        pad_inches = matplotlib.rcParams['savefig.pad_inches']
+        BBOX = figures[0].get_tightbbox(figures[0].canvas.get_renderer())
+        BBOX = BBOX.padded(pad_inches)
     nfigures = len(figures)
-    if nfigures == 1 or fmt == 'pdf_multipage':
+    if (nfigures == 1 or fmt == 'pdf_multipage') and not force_numbering:
         if fmt == 'pdf_multipage':
             figfile = f'{figfile_base}pdf'
             pdf = PdfPages(figfile)
         else:
             figfile = figfile_base + fmt
         figfiles = [figfile, ]
     else:
         figfiles = [f'{figfile_base}{n:02d}.{fmt}' for n in range(nfigures)]
     for n in range(nfigures):
+        if n in SAVED_FIGURE_NUMBERS:
+            continue
         if fmt == 'pdf_multipage':
-            pdf.savefig(figures[n], bbox_inches=bbox)
+            pdf.savefig(figures[n], bbox_inches=BBOX)
         else:
-            savefig(figures[n], figfiles[n], fmt, bbox_inches=bbox)
+            savefig(figures[n], figfiles[n], fmt, bbox_inches=BBOX)
         if not config.plot_show:
             plt.close(figures[n])
-    for figfile in figfiles:
-        logger.info(f'Trace plots saved to: {figfile}')
-    config.figures['traces'] += figfiles
+            # dereference the figure to free up memory
+            figures[n] = None
+        SAVED_FIGURE_NUMBERS.append(n)
+        config.figures['traces'].append(figfiles[n])
+        logger.info(f'Trace plots saved to: {figfiles[n]}')
     if fmt == 'pdf_multipage':
         pdf.close()
 
 
 def _plot_min_max(ax, x_vals, y_vals, linewidth, color, alpha, zorder):
     """Quick and dirty plot using less points. Useful for vector plotting."""
     ax_width_in_pixels = int(np.ceil(ax.bbox.width))
     nsamples = len(x_vals)
-    samples_per_pixel = int(np.ceil(nsamples/ax_width_in_pixels))
+    samples_per_pixel = int(np.ceil(nsamples / ax_width_in_pixels))
     # find the closest multiple of samples_per_pixel (rounded down)
     nsamples -= nsamples % samples_per_pixel
     # resample x_vals
     x_vals = x_vals[:nsamples:samples_per_pixel]
     # reshape y_vals so that each row has a number of elements equal to
     # samples_per_pixel
     y_vals = y_vals[:nsamples].reshape(-1, samples_per_pixel)
     # find min and max for each row
     y_min = y_vals.min(axis=1)
     y_max = y_vals.max(axis=1)
     # double the number of elements in x_vals
     dx = x_vals[1] - x_vals[0]
-    x_vals = np.column_stack((x_vals, x_vals+dx/2)).flatten()
+    x_vals = np.column_stack((x_vals, x_vals + dx / 2)).flatten()
     # alternate mins and maxs in y_vals
     y_vals = np.column_stack((y_min, y_max)).flatten()
     ax.plot(
         x_vals, y_vals, linewidth=linewidth, color=color, alpha=alpha,
         zorder=zorder)
 
 
 def _freq_string(freq):
     """Return a string representing the rounded frequency."""
+    # int or float notation for frequencies between 0.01 and 100
     if 1e-2 <= freq <= 1e2:
-        # int or float notation for frequencies between 0.01 and 100
         int_freq = int(round(freq))
         return (
             f'{int_freq}' if np.abs(int_freq - freq) < 1e-1
             else f'{freq:.1f}'
         )
-    else:
-        # scientific notation for frequencies outside of 0.01 and 100
-        freq_str = f'{freq:.1e}'
-        m, n = map(float, freq_str.split('e'))
-        n = int(n)
-        int_m = int(round(m))
-        return (
-            f'{int_m}e{n}' if np.abs(int_m - m) < 1e-1
-            else f'{m:.1f}e{n}'
-        )
+    # scientific notation for frequencies outside of 0.01 and 100
+    freq_str = f'{freq:.1e}'
+    m, n = map(float, freq_str.split('e'))
+    n = int(n)
+    int_m = int(round(m))
+    return (
+        f'{int_m}e{n}' if np.abs(int_m - m) < 1e-1
+        else f'{m:.1f}e{n}'
+    )
 
 
 def _plot_trace(config, trace, ntraces, tmax, ax, trans, trans3, path_effects):
     # Origin and height to draw vertical patches for noise and signal windows
     rectangle_patch_origin = 0
     rectangle_patch_height = 1
     orientation = trace.stats.channel[-1]
     if orientation in config.vertical_channel_codes:
         color = 'purple'
         if ntraces > 1:
-            rectangle_patch_origin = 1./3
-            rectangle_patch_height = 1./3
+            rectangle_patch_origin = 1. / 3
+            rectangle_patch_height = 1. / 3
     if orientation in config.horizontal_channel_codes_1:
         color = 'green'
         if ntraces > 1:
             trace.data = (trace.data / tmax - 1) * tmax
             rectangle_patch_origin = 0
-            rectangle_patch_height = 1./3
+            rectangle_patch_height = 1. / 3
     if orientation in config.horizontal_channel_codes_2:
         color = 'blue'
         if ntraces > 1:
             trace.data = (trace.data / tmax + 1) * tmax
-            rectangle_patch_origin = 2./3
-            rectangle_patch_height = 1./3
+            rectangle_patch_origin = 2. / 3
+            rectangle_patch_height = 1. / 3
     # dim out ignored traces
     alpha = 0.3 if trace.stats.ignore else 1.0
     times = trace.times() + trace.stats.time_offset
     if config.plot_save_format == 'png':
         ax.plot(
             times, trace.data, linewidth=1, color=color,
             alpha=alpha, zorder=20, rasterized=True)
@@ -247,28 +261,28 @@
                 zorder=22, path_effects=path_effects)
     # Noise window
     with contextlib.suppress(KeyError):
         N1 = trace.stats.arrivals['N1'][1] - starttime
         N2 = trace.stats.arrivals['N2'][1] - starttime
         rect = patches.Rectangle(
             (N1, rectangle_patch_origin),
-            width=N2-N1, height=rectangle_patch_height,
+            width=(N2 - N1), height=rectangle_patch_height,
             transform=trans, color='#eeeeee',
             zorder=-1)
         ax.add_patch(rect)
     # Signal window
     if config.wave_type[0] == 'S':
         t1 = trace.stats.arrivals['S1'][1] - starttime
         t2 = trace.stats.arrivals['S2'][1] - starttime
     elif config.wave_type[0] == 'P':
         t1 = trace.stats.arrivals['P1'][1] - starttime
         t2 = trace.stats.arrivals['P2'][1] - starttime
     rect = patches.Rectangle(
         (t1, rectangle_patch_origin),
-        width=t2-t1, height=rectangle_patch_height,
+        width=(t2 - t1), height=rectangle_patch_height,
         transform=trans, color='yellow',
         alpha=0.5, zorder=-1)
     ax.add_patch(rect)
     # Reason why trace is ignored
     if trace.stats.ignore:
         _text = trace.stats.ignore_reason
         color = 'black'
@@ -299,15 +313,15 @@
         transform=ax.transAxes, zorder=50, path_effects=path_effects)
     ax.has_station_info_text = True
 
 
 def _add_labels(axes, plotn, ncols):
     """Add xlabels to the last row of plots."""
     # A row has "ncols" plots: the last row is from `plotn-ncols` to `plotn`
-    n0 = max(plotn-ncols, 0)
+    n0 = max(plotn - ncols, 0)
     for ax in axes[n0:plotn]:
         ax.xaxis.set_tick_params(which='both', labelbottom=True)
         ax.set_xlabel('Time (s)', fontsize=8)
 
 
 def _set_ylim(axes):
     """Set symmetric ylim."""
@@ -315,16 +329,16 @@
         ylim = ax.get_ylim()
         ymax = np.max(np.abs(ylim))
         ax.set_ylim(-ymax, ymax)
 
 
 def _trim_traces(config, st):
     for trace in st:
-        t1 = (trace.stats.arrivals['P'][1] - config.noise_pre_time)
-        t2 = (trace.stats.arrivals['S'][1] + 3 * config.win_length)
+        t1 = trace.stats.arrivals['N1'][1]
+        t2 = trace.stats.arrivals['S2'][1] + 2 * config.win_length
         trace.trim(starttime=t1, endtime=t2)
     # compute time offset for correctly aligning traces when plotting
     min_starttime = min(tr.stats.starttime for tr in st)
     for trace in st:
         trace.stats.time_offset = trace.stats.starttime - min_starttime
 
 
@@ -367,29 +381,36 @@
             network=network, station=station, location=location,
             channel=f'{code}*')
         if not config.plot_traces_ignored:
             st_sel = Stream(tr for tr in st_sel if not tr.stats.ignore)
         if not st_sel:
             continue
         plotn += 1
-        if plotn > nlines*ncols:
+        if plotn > nlines * ncols:
             _set_ylim(axes)
-            _add_labels(axes, plotn-1, ncols)
+            _add_labels(axes, plotn - 1, ncols)
+            if (
+                config.plot_save_asap and
+                config.plot_save and not config.plot_show and
+                config.plot_save_format != 'pdf_multipage'
+            ):
+                # save figure here to free up memory
+                _savefig(config, figures, force_numbering=True)
             fig, axes = _make_fig(config, nlines, ncols)
             figures.append(fig)
             plotn = 1
-        ax = axes[plotn-1]
+        ax = axes[plotn - 1]
         if config.trace_units == 'auto':
             instrtype = [
                 t.stats.instrtype for t in st_sel.traces
                 if t.stats.channel[:-1] == code][0]
         else:
             instrtype = config.trace_units
         if instrtype in ['acc']:
-            ax.set_ylabel(u'Acceleration (m/s²)', fontsize=8, labelpad=0)
+            ax.set_ylabel('Acceleration (m/s²)', fontsize=8, labelpad=0)
         elif instrtype in ['broadb', 'shortp', 'vel']:
             ax.set_ylabel('Velocity (m/s)', fontsize=8, labelpad=0)
         elif instrtype in ['disp']:
             ax.set_ylabel('Displacement (m)', fontsize=8, labelpad=0)
         # Custom transformation for plotting phase labels:
         # x coords are data, y coords are axes
         trans =\
```

### Comparing `sourcespec-1.7/sourcespec/ssp_process_traces.py` & `sourcespec-1.8/sourcespec/ssp_process_traces.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,30 +5,32 @@
 
 :copyright:
     2012 Claudio Satriano <satriano@ipgp.fr>
 
     2013-2014 Claudio Satriano <satriano@ipgp.fr>,
               Emanuela Matrullo <matrullo@geologie.ens.fr>
 
-    2015-2023 Claudio Satriano <satriano@ipgp.fr>
+    2015-2024 Claudio Satriano <satriano@ipgp.fr>
 :license:
     CeCILL Free Software License Agreement v2.1
     (http://www.cecill.info/licences.en.html)
 """
 import logging
+import re
 import numpy as np
 from scipy.signal import savgol_filter
-import re
 from obspy.core import Stream
 from obspy.core.util import AttribDict
 from sourcespec.ssp_setup import ssp_exit
-from sourcespec.ssp_util import remove_instr_response, hypo_dist
-from sourcespec.ssp_wave_arrival import add_arrivals_to_trace
-from sourcespec.clipping_detection import clipping_score, clipping_peaks
-logger = logging.getLogger(__name__.split('.')[-1])
+from sourcespec.ssp_util import (
+    remove_instr_response, station_to_event_position)
+from sourcespec.ssp_wave_arrival import add_arrival_to_trace
+from sourcespec.clipping_detection import (
+    compute_clipping_score, clipping_peaks)
+logger = logging.getLogger(__name__.rsplit('.', maxsplit=1)[-1])
 
 
 def _get_bandpass_frequencies(config, trace):
     """Get frequencies for bandpass filter."""
     # see if there is a station-specific filter
     station = trace.stats.station
     try:
@@ -44,23 +46,27 @@
                 f'{trace.id}: Unknown instrument type: {instrtype}: '
                 'skipping trace'
             ) from e
     return bp_freqmin, bp_freqmax
 
 
 def filter_trace(config, trace):
+    """Filter trace."""
     bp_freqmin, bp_freqmax = _get_bandpass_frequencies(config, trace)
-    nyquist = 1./(2. * trace.stats.delta)
+    nyquist = 1. / (2. * trace.stats.delta)
     if bp_freqmax >= nyquist:
         bp_freqmax = nyquist * 0.999
         logger.warning(
             f'{trace.id}: maximum frequency for bandpass filtering '
             f'is larger or equal to Nyquist. Setting it to {bp_freqmax} Hz')
-    filter_options = dict(
-        type='bandpass', freqmin=bp_freqmin, freqmax=bp_freqmax)
+    filter_options = {
+        'type': 'bandpass',
+        'freqmin': bp_freqmin,
+        'freqmax': bp_freqmax
+    }
     trace.filter(**filter_options)
     # save filter info to trace stats
     trace.stats.filter = AttribDict(filter_options)
 
 
 def _check_signal_level(config, trace):
     rms2 = np.power(trace.data, 2).sum()
@@ -81,15 +87,15 @@
     t1 = trace.stats.arrivals['N1'][1]
     if config.wave_type[0] == 'S':
         t2 = trace.stats.arrivals['S2'][1]
     elif config.wave_type[0] == 'P':
         t2 = trace.stats.arrivals['P2'][1]
     tr = trace.copy().trim(t1, t2)
     if config.clipping_detection_algorithm == 'clipping_score':
-        score = clipping_score(
+        score = compute_clipping_score(
             tr, config.remove_baseline, config.clipping_debug_plot)
         logger.info(f'{tr.stats.info}: clipping score: {score:.1f}%')
         if score > config.clipping_score_threshold:
             trace.stats.clipped = True
             trace.stats.ignore = True
             trace.stats.ignore_reason = f'clipping: {score:.1f}%'
     elif config.clipping_detection_algorithm == 'clipping_peaks':
@@ -130,15 +136,15 @@
     rmsS = np.sqrt(rmsS2)
     if rmsnoise == 0:
         if config.weighting == 'noise':
             raise RuntimeError(
                 f'{trace.stats.info}: empty noise window: skipping trace')
         logger.warning(f'{trace.stats.info}: empty noise window!')
         rmsnoise = 1.
-    sn_ratio = rmsS/rmsnoise
+    sn_ratio = rmsS / rmsnoise
     logger.info(f'{trace.stats.info}: S/N: {sn_ratio:.1f}')
     trace.stats.sn_ratio = sn_ratio
     # stop here if trace is already ignored
     if trace.stats.ignore:
         return
     snratio_min = config.sn_min
     if sn_ratio < snratio_min:
@@ -192,57 +198,155 @@
     _check_signal_level(config, trace_process)
     # check if trace is clipped
     _check_clipping(config, trace_process)
     # Remove instrument response
     bp_freqmin, bp_freqmax = _get_bandpass_frequencies(config, trace)
     if config.correct_instrumental_response:
         try:
-            pre_filt = (bp_freqmin, bp_freqmin*1.1, bp_freqmax*0.9, bp_freqmax)
+            pre_filt = (
+                bp_freqmin, bp_freqmin * 1.1,
+                bp_freqmax * 0.9, bp_freqmax)
             remove_instr_response(trace_process, pre_filt)
         except Exception as e:
             raise RuntimeError(
                 f'{e}\n'
                 f'{trace.stats.info}: Unable to remove instrument response: '
                 'skipping trace') from e
     _remove_baseline(config, trace_process)
     filter_trace(config, trace_process)
     # Check if the trace has significant signal to noise ratio
     _check_sn_ratio(config, trace_process)
     return trace_process
 
 
-def _merge_stream(config, st):
+def _add_station_to_event_position(trace):
     """
-    Check for gaps and overlaps; remove mean; merge stream.
+    Add to ``trace.stats`` station-to-event distance (hypocentral and
+    epicentral), great-circle distance, azimuth and backazimuth.
+    Raise RuntimeError if unable to compute distances.
     """
-    traceid = st[0].id
-    # First, compute gap/overlap statistics for the whole trace.
-    gaps_olaps = st.get_gaps()
-    gaps = [g for g in gaps_olaps if g[6] >= 0]
-    overlaps = [g for g in gaps_olaps if g[6] < 0]
-    gap_duration = sum(g[6] for g in gaps)
-    if gap_duration > 0:
-        logger.info(
-            f'{traceid}: trace has {gap_duration:.3f} seconds of gaps.')
-        gap_max = config.gap_max
-        if gap_max is not None and gap_duration > gap_max:
-            raise RuntimeError(
-                f'{traceid}: Gap duration larger than gap_max '
-                f'({gap_max:.1f} s): skipping trace')
-    overlap_duration = -1 * sum(g[6] for g in overlaps)
-    if overlap_duration > 0:
-        logger.info(
-            f'{traceid}: trace has {overlap_duration:.3f} seconds of '
-            'overlaps.')
-        overlap_max = config.overlap_max
-        if overlap_max is not None and overlap_duration > overlap_max:
+    try:
+        station_to_event_position(trace)
+    except Exception as e:
+        raise RuntimeError(
+            f'{trace.id}: Unable to compute hypocentral distance: {e}. '
+            'Skipping trace'
+        ) from e
+
+
+def _check_epicentral_distance(config, trace):
+    """
+    Reject traces with hypocentral distance outside the range specified
+    in the configuration file.
+    """
+    if config.epi_dist_ranges is None:
+        return
+    # transform integers to true integers, for better string representation
+    edr = [
+        int(r) if float(r).is_integer() else r for r in config.epi_dist_ranges]
+    # if edr has an odd number of elements, add one last element
+    if len(edr) % 2 == 1:
+        edr.append(999999)
+    # reshape edr to a list of pairs
+    edr = [[edr[i], edr[i+1]] for i in range(0, len(edr), 2)]
+    # string representation of edr
+    edr_str = ', '.join(f'{ed[0]}-{ed[1]} km' for ed in edr)
+    epi_dist = trace.stats.epi_dist
+    # check if epi_dist is in one of the ranges
+    if not any(ed[0] <= epi_dist <= ed[1] for ed in edr):
+        raise RuntimeError(
+            f'{trace.id}: Epicentral distance ({epi_dist:.1f} km) '
+            f'not in the selected range ({edr_str}): skipping trace')
+
+
+def _add_arrivals(config, trace):
+    """Add to trace P and S arrival times, travel times and angles."""
+    for phase in 'P', 'S':
+        try:
+            add_arrival_to_trace(trace, phase, config)
+        except Exception as e:
+            for line in str(e).splitlines():
+                logger.warning(line)
             raise RuntimeError(
-                f'{traceid}: overlap duration larger than overlap_max '
-                f'({overlap_max:.1f} s): skipping trace')
-    # Then, compute the same statisics for the signal window.
+                f'{trace.id}: Unable to get {phase} arrival time: '
+                'skipping trace'
+            ) from e
+
+
+def _define_signal_and_noise_windows(config, trace):
+    """Define signal and noise windows for spectral analysis."""
+    p_arrival_time = trace.stats.arrivals['P'][1]
+    if config.wave_type[0] == 'P' and p_arrival_time < trace.stats.starttime:
+        raise RuntimeError(f'{trace.id}: P-window incomplete: skipping trace')
+    s_arrival_time = trace.stats.arrivals['S'][1]
+    if config.wave_type[0] == 'S' and s_arrival_time < trace.stats.starttime:
+        raise RuntimeError(f'{trace.id}: S-window incomplete: skipping trace')
+    # Signal window for spectral analysis (S phase)
+    s_minus_p = s_arrival_time - p_arrival_time
+    s_pre_time = config.signal_pre_time
+    if s_minus_p / 2 < s_pre_time:
+        # use (Ts-Tp)/2 if it is smaller than signal_pre_time
+        # (for short-distance records with short S-P interval)
+        s_pre_time = s_minus_p / 2
+        logger.warning(
+            f'{trace.id}: signal_pre_time is larger than (Ts-Tp)/2. '
+            'Using (Ts-Tp)/2 instead')
+    t1 = s_arrival_time - s_pre_time
+    t1 = max(trace.stats.starttime, t1)
+    tt_s = trace.stats.travel_times['S']
+    # manage case where variable_win_length_factor is None:
+    variable_win_length_factor = config.variable_win_length_factor or 0
+    win_length_s = max(config.win_length, variable_win_length_factor * tt_s)
+    t2 = t1 + win_length_s
+    t2 = min(trace.stats.endtime, t2)
+    win_length_s = t2 - t1
+    trace.stats.arrivals['S1'] = ('S1', t1)
+    trace.stats.arrivals['S2'] = ('S2', t2)
+    # Signal window for spectral analysis (P phase)
+    t1 = p_arrival_time - config.signal_pre_time
+    t1 = max(trace.stats.starttime, t1)
+    tt_p = trace.stats.travel_times['P']
+    win_length_p = max(config.win_length, variable_win_length_factor * tt_p)
+    t2 = t1 + min(win_length_p, s_minus_p + s_pre_time)
+    t2 = min(trace.stats.endtime, t2)
+    win_length_p = t2 - t1
+    trace.stats.arrivals['P1'] = ('P1', t1)
+    trace.stats.arrivals['P2'] = ('P2', t2)
+    # Noise window for spectral analysis
+    if config.wave_type[0] == 'P':
+        win_length = win_length_p
+    elif config.wave_type[0] == 'S':
+        win_length = win_length_s
+    if config.variable_win_length_factor:
+        logger.info(f'{trace.id}: window length {win_length:.3f} seconds')
+    if config.noise_pre_time is None:
+        noise_pre_time = win_length + config.signal_pre_time
+    else:
+        noise_pre_time = config.noise_pre_time
+    t1 = max(
+        trace.stats.starttime,
+        p_arrival_time - noise_pre_time
+    )
+    t2 = t1 + win_length
+    if t2 > (p_arrival_time - config.signal_pre_time):
+        logger.warning(f'{trace.id}: noise window ends after P-window start')
+        t2 = p_arrival_time - config.signal_pre_time
+        t1 = min(t1, t2)
+    trace.stats.arrivals['N1'] = ('N1', t1)
+    trace.stats.arrivals['N2'] = ('N2', t2)
+
+
+def _check_signal_window(config, st):
+    """
+    Check if the signal window has sufficient amount of signal
+    (i.e., not too many gaps).
+
+    This is done on the stream, before merging.
+    """
+    traceid = st[0].id
     st_cut = st.copy()
     if config.wave_type[0] == 'S':
         t1 = st[0].stats.arrivals['S1'][1]
         t2 = st[0].stats.arrivals['S2'][1]
     elif config.wave_type[0] == 'P':
         t1 = st[0].stats.arrivals['P1'][1]
         t2 = st[0].stats.arrivals['P2'][1]
@@ -253,23 +357,53 @@
             f'{config.wave_type[0]}-wave cut interval: skipping trace >\n'
             f'> Cut interval: {t1} - {t2}')
     gaps_olaps = st_cut.get_gaps()
     gaps = [g for g in gaps_olaps if g[6] >= 0]
     overlaps = [g for g in gaps_olaps if g[6] < 0]
     duration = st_cut[-1].stats.endtime - st_cut[0].stats.starttime
     gap_duration = sum(g[6] for g in gaps)
-    if gap_duration > duration/4:
+    if gap_duration > duration / 4:
         raise RuntimeError(
             f'{traceid}: too many gaps for the selected cut interval: '
             'skipping trace')
     overlap_duration = -1 * sum(g[6] for g in overlaps)
     if overlap_duration > 0:
         logger.info(
             f'{traceid}: signal window has {overlap_duration:.3f} seconds '
             'of overlaps.')
+
+
+def _merge_stream(config, st):
+    """
+    Check for gaps and overlaps; remove mean; merge stream.
+    """
+    traceid = st[0].id
+    # First, compute gap/overlap statistics for the whole trace.
+    gaps_olaps = st.get_gaps()
+    gaps = [g for g in gaps_olaps if g[6] >= 0]
+    overlaps = [g for g in gaps_olaps if g[6] < 0]
+    gap_duration = sum(g[6] for g in gaps)
+    if gap_duration > 0:
+        logger.info(
+            f'{traceid}: trace has {gap_duration:.3f} seconds of gaps.')
+        gap_max = config.gap_max
+        if gap_max is not None and gap_duration > gap_max:
+            raise RuntimeError(
+                f'{traceid}: Gap duration larger than gap_max '
+                f'({gap_max:.1f} s): skipping trace')
+    overlap_duration = -1 * sum(g[6] for g in overlaps)
+    if overlap_duration > 0:
+        logger.info(
+            f'{traceid}: trace has {overlap_duration:.3f} seconds of '
+            'overlaps.')
+        overlap_max = config.overlap_max
+        if overlap_max is not None and overlap_duration > overlap_max:
+            raise RuntimeError(
+                f'{traceid}: overlap duration larger than overlap_max '
+                f'({overlap_max:.1f} s): skipping trace')
     # Finally, demean (only if trace has not be already preprocessed)
     if config.trace_units == 'auto':
         # Since the count value is generally huge, we need to demean twice
         # to take into account for the rounding error
         st.detrend(type='constant')
         st.detrend(type='constant')
     # Merge stream to remove gaps and overlaps
@@ -280,136 +414,74 @@
     except Exception as e:
         raise RuntimeError(
             f'{traceid}: unable to fill gaps: skipping trace'
         ) from e
     return st[0]
 
 
-def _add_hypo_dist_and_arrivals(config, st):
-    for trace in st:
-        if hypo_dist(trace) is None:
-            raise RuntimeError(
-                f'{trace.id}: Unable to compute hypocentral distance: '
-                'skipping trace')
-        if config.max_epi_dist is not None and \
-                trace.stats.epi_dist > config.max_epi_dist:
-            raise RuntimeError(
-                f'{trace.id}: Epicentral distance '
-                f'({trace.stats.epi_dist:.1f} km) '
-                f'larger than max_epi_dist ({config.max_epi_dist:.1f} km): '
-                'skipping trace')
-        add_arrivals_to_trace(trace, config)
-        try:
-            p_arrival_time = trace.stats.arrivals['P'][1]
-        except KeyError as e:
-            raise RuntimeError(
-                f'{trace.id}: Unable to get P arrival time: skipping trace'
-            ) from e
-        if (config.wave_type[0] == 'P' and
-                p_arrival_time < trace.stats.starttime):
-            raise RuntimeError(
-                f'{trace.id}: P-window incomplete: skipping trace')
-        try:
-            s_arrival_time = trace.stats.arrivals['S'][1]
-        except KeyError as e:
-            raise RuntimeError(
-                f'{trace.id}: Unable to get S arrival time: skipping trace'
-            ) from e
-        if (config.wave_type[0] == 'S' and
-                s_arrival_time < trace.stats.starttime):
-            raise RuntimeError(
-                f'{trace.id}: S-window incomplete: skipping trace')
-        # Signal window for spectral analysis (S phase)
-        s_minus_p = s_arrival_time-p_arrival_time
-        s_pre_time = config.signal_pre_time
-        if s_minus_p/2 < s_pre_time:
-            # use (Ts-Tp)/2 if it is smaller than signal_pre_time
-            # (for short-distance records with short S-P interval)
-            s_pre_time = s_minus_p/2
-            logger.warning(
-                f'{trace.id}: signal_pre_time is larger than (Ts-Tp)/2. '
-                'Using (Ts-Tp)/2 instead')
-        t1 = s_arrival_time - s_pre_time
-        t1 = max(trace.stats.starttime, t1)
-        t2 = t1 + config.win_length
-        trace.stats.arrivals['S1'] = ('S1', t1)
-        trace.stats.arrivals['S2'] = ('S2', t2)
-        # Signal window for spectral analysis (P phase)
-        t1 = p_arrival_time - config.signal_pre_time
-        t1 = max(trace.stats.starttime, t1)
-        t2 = t1 + min(config.win_length, s_minus_p)
-        trace.stats.arrivals['P1'] = ('P1', t1)
-        trace.stats.arrivals['P2'] = ('P2', t2)
-        # Noise window for spectral analysis
-        t1 = max(trace.stats.starttime, p_arrival_time - config.noise_pre_time)
-        t2 = t1 + config.win_length
-        if t2 >= p_arrival_time:
-            logger.warning(
-                f'{trace.id}: noise window ends after P-wave arrival')
-            # Note: maybe we should also take into account signal_pre_time here
-            t2 = p_arrival_time
-            t1 = min(t1, t2)
-        trace.stats.arrivals['N1'] = ('N1', t1)
-        trace.stats.arrivals['N2'] = ('N2', t2)
-
-
-def _skip_ignored(config, id):
+def _skip_ignored(config, traceid):
     """Skip traces ignored from config."""
-    network, station, location, channel = id.split('.')
+    network, station, location, channel = traceid.split('.')
     # build a list of all possible ids, from station only
     # to full net.sta.loc.chan
     ss = [
         station,
         '.'.join((network, station)),
         '.'.join((network, station, location)),
         '.'.join((network, station, location, channel)),
     ]
     if config.use_traceids is not None:
         combined = (
             "(" + ")|(".join(config.use_traceids) + ")"
-            ).replace('.', r'\.')
+        ).replace('.', r'\.')
         if not any(re.match(combined, s) for s in ss):
-            raise RuntimeError(f'{id}: ignored from config file')
+            raise RuntimeError(f'{traceid}: ignored from config file')
     if config.ignore_traceids is not None:
         combined = (
             "(" + ")|(".join(config.ignore_traceids) + ")"
-            ).replace('.', r'\.')
+        ).replace('.', r'\.')
         if any(re.match(combined, s) for s in ss):
-            raise RuntimeError(f'{id}: ignored from config file')
+            raise RuntimeError(f'{traceid}: ignored from config file')
 
 
 def process_traces(config, st):
     """Remove mean, deconvolve and ignore unwanted components."""
     logger.info('Processing traces...')
     out_st = Stream()
-    for id in sorted({tr.id for tr in st}):
-        # We still use a stream, since the trace can have gaps or overlaps
-        st_sel = st.select(id=id)
+    for traceid in sorted({tr.id for tr in st}):
         try:
-            _skip_ignored(config, id)
-            _add_hypo_dist_and_arrivals(config, st_sel)
+            _skip_ignored(config, traceid)
+            # We still use a stream, since the trace can have gaps or overlaps
+            st_sel = st.select(id=traceid)
+            for _trace in st_sel:
+                _add_station_to_event_position(_trace)
+                _check_epicentral_distance(config, _trace)
+                _add_arrivals(config, _trace)
+                _define_signal_and_noise_windows(config, _trace)
+            _check_signal_window(config, st_sel)
             trace = _merge_stream(config, st_sel)
             trace.stats.ignore = False
             trace_process = _process_trace(config, trace)
             out_st.append(trace_process)
         except (ValueError, RuntimeError) as msg:
             logger.warning(msg)
             continue
 
     if len(out_st) == 0:
         logger.error('No traces left! Exiting.')
         ssp_exit()
 
     # Rotate traces, if SH or SV is requested
     if config.wave_type in ['SH', 'SV']:
-        for id in sorted({tr.id[:-1] for tr in out_st}):
-            net, sta, loc, chan = id.split('.')
+        for traceid in sorted({tr.id[:-1] for tr in out_st}):
+            net, sta, loc, chan = traceid.split('.')
             st_sel = out_st.select(
                 network=net, station=sta, location=loc, channel=f'{chan}?'
             )
             t0 = max(tr.stats.starttime for tr in st_sel)
             t1 = min(tr.stats.endtime for tr in st_sel)
             st_sel.trim(t0, t1)
             st_sel.rotate('NE->RT')
 
     logger.info('Processing traces: done')
+    logger.info('---------------------------------------------------')
     return out_st
```

### Comparing `sourcespec-1.7/sourcespec/ssp_qml_output.py` & `sourcespec-1.8/sourcespec/ssp_qml_output.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 # SPDX-License-Identifier: CECILL-2.1
 """
 QuakeML output for source_spec.
 
 :copyright:
-    2016-2023 Claudio Satriano <satriano@ipgp.fr>
+    2016-2024 Claudio Satriano <satriano@ipgp.fr>
 
 :license:
     CeCILL Free Software License Agreement, Version 2.1
     (http://www.cecill.info/index.en.html)
 """
 import os
 import logging
@@ -16,15 +16,15 @@
 from obspy import read_events, UTCDateTime
 from obspy.core import AttribDict
 from obspy.core.event import (CreationInfo, FocalMechanism, Magnitude,
                               MomentTensor, QuantityError, ResourceIdentifier,
                               StationMagnitude, StationMagnitudeContribution,
                               WaveformStreamID)
 from sourcespec._version import get_versions
-logger = logging.getLogger(__name__.split('.')[-1])
+logger = logging.getLogger(__name__.rsplit('.', maxsplit=1)[-1])
 
 
 def _to_camel_case(snake_str):
     # source: http://stackoverflow.com/q/19053707
     components = snake_str.split('_')
     # We capitalize the first letter of each component except the first one
     # with the 'title' method and join them together.
@@ -35,43 +35,46 @@
     """Container for custom tags."""
 
     def __setattr__(self, key, value):
         """Set class attribute."""
         key = _to_camel_case(key)
         return super(AttribDict, self).__setattr__(key, value)
 
-    def __getattr__(self, key):
+    def __getattr__(self, key, default=None):
         """Get class attribute."""
         key = _to_camel_case(key)
-        return self.__dict__[key]
+        return super(AttribDict, self).__getattr__(key, default)
 
 
 class SSPContainerTag(AttribDict):
     """Container for nested custom tags."""
 
     def __init__(self):
+        super().__init__()
         self.namespace = 'https://sourcespec.seismicsource.org'
         self.value = SSPExtra()
 
 
 class SSPTag(AttribDict):
     """Custom tag object."""
 
     def __init__(self, value=None):
+        super().__init__()
         self.namespace = 'https://sourcespec.seismicsource.org'
         self.value = value
 
 
 def write_qml(config, sspec_output):
+    """Write QuakeML output."""
     if not config.options.qml_file:
         config.qml_file_out = None
         return
     qml_file = config.options.qml_file
     cat = read_events(qml_file)
-    evid = config.hypo.evid
+    evid = config.event.event_id
     try:
         ev = [e for e in cat if evid in str(e.resource_id)][0]
     except Exception:
         logger.warning(
             f'Unable to find evid "{evid}" in QuakeML file. '
             'QuakeML output will not be written.')
         config.qml_file_out = None
@@ -179,15 +182,20 @@
     # Write other summary parameters as custom tags
     ev.extra = SSPExtra()
     ev.extra.corner_frequency = _summary_parameter_tag(
         summary_parameters['fc'])
     ev.extra.t_star = _summary_parameter_tag(summary_parameters['t_star'])
     ev.extra.source_radius = _summary_parameter_tag(
         summary_parameters['radius'])
-    ev.extra.stress_drop = _summary_parameter_tag(summary_parameters['bsd'])
+    ev.extra.static_stress_drop = _summary_parameter_tag(
+        summary_parameters['ssd'])
+    ev.extra.radiated_energy = _summary_parameter_tag(
+        summary_parameters['Er'])
+    ev.extra.apparent_stress = _summary_parameter_tag(
+        summary_parameters['sigma_a'])
     if config.set_preferred_magnitude:
         ev.preferred_magnitude_id = mag.resource_id.id
 
     qml_file_out = os.path.join(config.options.outdir, f'{evid}.xml')
     with warnings.catch_warnings(record=True) as warns:
         ev.write(qml_file_out, format='QUAKEML')
         for w in warns:
```

### Comparing `sourcespec-1.7/sourcespec/ssp_radiation_pattern.py` & `sourcespec-1.8/sourcespec/ssp_radiation_pattern.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 # -*- coding: utf-8 -*-
 # SPDX-License-Identifier: CECILL-2.1
 """
 Compute radiation pattern.
 
 :copyright:
-    2021-2023 Claudio Satriano <satriano@ipgp.fr>
+    2021-2024 Claudio Satriano <satriano@ipgp.fr>
 :license:
     CeCILL Free Software License Agreement v2.1
     (http://www.cecill.info/licences.en.html)
 """
 import contextlib
 import logging
 from math import pi, sin, cos
 from obspy.taup import TauPyModel
-logger = logging.getLogger(__name__.split('.')[-1])
+logger = logging.getLogger(__name__.rsplit('.', maxsplit=1)[-1])
 model = TauPyModel(model='iasp91')
 
 
 def toRad(angle):
-    return angle/180. * pi
+    """Convert angle from degrees to radians."""
+    return angle / 180. * pi
 
 
 def radiation_pattern(strike, dip, rake, takeoff_angle, azimuth, wave):
     """
     Body wave radiation pattern.
 
     From Lay-Wallace, page 340.
@@ -45,94 +46,95 @@
     else:
         raise ValueError(f'Unknown wave type: {wave}')
     return R
 
 
 def _rad_patt_P(phi, dip, rake, takeoff):
     return (
-        cos(rake) * sin(dip) * sin(takeoff)**2 * sin(2*phi) -
-        cos(rake) * cos(dip) * sin(2*takeoff) * cos(phi) +
-        sin(rake) * sin(2*dip) *
+        cos(rake) * sin(dip) * sin(takeoff)**2 * sin(2 * phi) -
+        cos(rake) * cos(dip) * sin(2 * takeoff) * cos(phi) +
+        sin(rake) * sin(2 * dip) *
         (cos(takeoff)**2 - sin(takeoff)**2 * sin(phi)**2) +
-        sin(rake) * cos(2*dip) * sin(2*takeoff) * sin(phi)
+        sin(rake) * cos(2 * dip) * sin(2 * takeoff) * sin(phi)
     )
 
 
 def _rad_patt_S(phi, dip, rake, takeoff):
     RSV = _rad_patt_SV(phi, dip, rake, takeoff)
     RSH = _rad_patt_SH(phi, dip, rake, takeoff)
-    return (RSV**2. + RSH**2.)**(1./2)
+    return (RSV**2. + RSH**2.)**(1. / 2)
 
 
 def _rad_patt_SV(phi, dip, rake, takeoff):
     return (
-        sin(rake) * cos(2*dip) * cos(2*takeoff) * sin(phi) -
-        cos(rake) * cos(dip) * cos(2*takeoff) * cos(phi) +
-        0.5 * cos(rake) * sin(dip) * sin(2*takeoff) * sin(2*phi) -
-        0.5 * sin(rake) * sin(2*dip) * sin(2*takeoff) *
+        sin(rake) * cos(2 * dip) * cos(2 * takeoff) * sin(phi) -
+        cos(rake) * cos(dip) * cos(2 * takeoff) * cos(phi) +
+        0.5 * cos(rake) * sin(dip) * sin(2 * takeoff) * sin(2 * phi) -
+        0.5 * sin(rake) * sin(2 * dip) * sin(2 * takeoff) *
         (1 + sin(phi)**2)
     )
 
 
 def _rad_patt_SH(phi, dip, rake, takeoff):
     return (
         cos(rake) * cos(dip) * cos(takeoff) * sin(phi) +
-        cos(rake) * sin(dip) * sin(takeoff) * cos(2*phi) +
-        sin(rake) * cos(2*dip) * cos(takeoff) * cos(phi) -
-        0.5 * sin(rake) * sin(2*dip) * sin(takeoff) * sin(2*phi)
+        cos(rake) * sin(dip) * sin(takeoff) * cos(2 * phi) +
+        sin(rake) * cos(2 * dip) * cos(takeoff) * cos(phi) -
+        0.5 * sin(rake) * sin(2 * dip) * sin(takeoff) * sin(2 * phi)
     )
 
 
 # Cache radiation patterns
-rp_cache = {}
+RP_CACHE = {}
 # Cache messages to avoid duplication
-rp_msg_cache = []
+RP_MSG_CACHE = []
 
 
 def get_radiation_pattern_coefficient(stats, config):
-    global rp_cache
-    global rp_msg_cache
+    """Get radiation pattern coefficient."""
     wave_type = config.wave_type  # P, S, SV, SH
     simple_wave_type = wave_type[0].lower()  # p or s
     if not config.rp_from_focal_mechanism:
         return config[f'rp{simple_wave_type}']
     try:
-        strike = stats.hypo.strike
-        dip = stats.hypo.dip
-        rake = stats.hypo.rake
+        fm = stats.event.focal_mechanism
+        # will raise an Exception if any of these is None
+        strike = float(fm.strike)
+        dip = float(fm.dip)
+        rake = float(fm.rake)
     except Exception:
         msg = (
             f'Cannot find focal mechanism. Using "rp{simple_wave_type}" '
             'value from config file'
         )
-        if msg not in rp_msg_cache:
+        if msg not in RP_MSG_CACHE:
             logger.warning(msg)
-            rp_msg_cache.append(msg)
+            RP_MSG_CACHE.append(msg)
         return config[f'rp{simple_wave_type}']
     traceid = '.'.join(
         (stats.network, stats.station, stats.location, stats.channel))
     key = f'{traceid}_{wave_type}'
     # try to get radiation pattern from cache
     with contextlib.suppress(KeyError):
-        return rp_cache[key]
+        return RP_CACHE[key]
     try:
         takeoff_angle = stats.takeoff_angles[simple_wave_type.upper()]
-    except Exception:
+    except KeyError:
         msg = (
             f'{traceid}: Cannot find takeoff angle. '
             f'Using "rp{simple_wave_type}" value from config file'
         )
-        if msg not in rp_msg_cache:
+        if msg not in RP_MSG_CACHE:
             logger.warning(msg)
-            rp_msg_cache.append(msg)
+            RP_MSG_CACHE.append(msg)
         return config[f'rp{simple_wave_type}']
     rp = radiation_pattern(
         strike, dip, rake, takeoff_angle, stats.azimuth, wave_type)
     # we are interested only in amplitude
     # (P, SV and SH radiation patterns have a sign)
     rp = abs(rp)
     logger.info(
         f'{traceid}: {wave_type} radiation pattern from focal mechanism: '
         f'{rp:.2f}'
     )
-    rp_cache[key] = rp
+    RP_CACHE[key] = rp
     return rp
```

### Comparing `sourcespec-1.7/sourcespec/ssp_read_sac_header.py` & `sourcespec-1.8/sourcespec/ssp_read_sac_header.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 # -*- coding: utf-8 -*-
 # SPDX-License-Identifier: CECILL-2.1
 """
 Read metadata from SAC file headers.
 
 :copyright:
-    2023 Claudio Satriano <satriano@ipgp.fr>
+    2023-2024 Claudio Satriano <satriano@ipgp.fr>
 :license:
     CeCILL Free Software License Agreement v2.1
     (http://www.cecill.info/licences.en.html)
 """
 import re
 import logging
 import contextlib
 from obspy.core.util import AttribDict
 from sourcespec.ssp_setup import ssp_exit
-from sourcespec.ssp_read_event_metadata import Pick
-logger = logging.getLogger(__name__.split('.')[-1])
+from sourcespec.ssp_event import SSPEvent
+from sourcespec.ssp_pick import SSPPick
+logger = logging.getLogger(__name__.rsplit('.', maxsplit=1)[-1])
 
 
 def compute_sensitivity_from_SAC(trace, config):
     """Compute sensitivity from SAC header fields."""
     # Securize the string before calling eval()
     # see https://stackoverflow.com/a/25437733/2021880
     inp = re.sub(r'\.(?![0-9])', '', config.sensitivity)
@@ -28,15 +29,15 @@
     namespace = None
     if re.search(r'[a-zA-Z]', inp):
         try:
             namespace = trace.stats.sac
         except Exception as e:
             raise TypeError(f'{trace.id}: trace must be in SAC format') from e
     try:
-        sensitivity = eval(inp, {}, namespace)
+        sensitivity = eval(inp, {}, namespace)  # pylint: disable=eval-used
     except NameError as msg:
         hdr_field = str(msg).split()[1]
         logger.error(f'SAC header field {hdr_field} does not exist')
         ssp_exit(1)
     return sensitivity
 
 
@@ -81,16 +82,16 @@
         coords = AttribDict(latitude=stla, longitude=stlo, elevation=stel)
         logger.info(
             f'{trace.id}: station coordinates read from SAC header')
         return coords
     return None
 
 
-def get_hypocenter_from_SAC(trace):
-    """Get hypocenter information from SAC header."""
+def get_event_from_SAC(trace):
+    """Get event information from SAC header."""
     try:
         sac_hdr = trace.stats.sac
     except AttributeError as e:
         raise RuntimeError(
             f'{trace.id}: not a SAC trace: cannot get hypocenter from header'
         ) from e
     evla = sac_hdr['evla']
@@ -117,17 +118,22 @@
     # (if it has spaces, then kevnm is probably not an evid)
     kevnm = sac_hdr.get('kevnm', '').strip()
     if kevnm and ' ' not in kevnm:
         evid = kevnm
     else:
         # create evid from origin time
         evid = evid_time.strftime('%Y%m%d_%H%M%S')
-    return AttribDict(
-        latitude=evla, longitude=evlo, depth=evdp, origin_time=origin_time,
-        evid=evid)
+    ssp_event = SSPEvent()
+    ssp_event.event_id = evid
+    ssp_event.hypocenter.latitude.value_in_deg = evla
+    ssp_event.hypocenter.longitude.value_in_deg = evlo
+    ssp_event.hypocenter.depth.value = evdp
+    ssp_event.hypocenter.depth.units = 'km'
+    ssp_event.hypocenter.origin_time = origin_time
+    return ssp_event
 
 
 def get_picks_from_SAC(trace):
     """Get picks from SAC header."""
     try:
         sac_hdr = trace.stats.sac
     except AttributeError as e:
@@ -139,28 +145,30 @@
         'a', 't0', 't1', 't2', 't3', 't4', 't5', 't6', 't7', 't8', 't9')
     for field in pick_fields:
         try:
             time = sac_hdr[field]
             begin = sac_hdr['b']
         except KeyError:
             continue
-        pick = Pick()
+        pick = SSPPick()
         pick.station = trace.stats.station
         pick.time = trace.stats.starttime + time - begin
+        # we will try to get the phase from the label later
+        pick.phase = 'X'
         # now look at labels (ka, kt0, ...)
         label = ''
         with contextlib.suppress(Exception):
             label = sac_hdr[f'k{field}'].strip()
         if len(label) == 4:
             # label is something like 'IPU0' or 'ES 2'
             pick.flag = label[0]
             pick.phase = label[1]
             pick.polarity = label[2]
             pick.quality = label[3]
-        elif len(label) > 0:
+        if pick.phase.upper() not in 'PS' and len(label) > 0:
             # we assume that label starts with 'P' or 'S'
             pick.phase = label[0]
         else:
             # no label, use default phase for field
             default_phases = {'a': 'P', 't0': 'S'}
             pick.phase = default_phases.get(field, 'X')
         trace_picks.append(pick)
```

### Comparing `sourcespec-1.7/sourcespec/ssp_read_station_metadata.py` & `sourcespec-1.8/sourcespec/ssp_read_station_metadata.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 # -*- coding: utf-8 -*-
 # SPDX-License-Identifier: CECILL-2.1
 """
 Read station metadata in StationXML, dataless SEED, SEED RESP,
 PAZ (SAC polezero format).
 
 :copyright:
-    2012-2023 Claudio Satriano <satriano@ipgp.fr>
+    2012-2024 Claudio Satriano <satriano@ipgp.fr>
 :license:
     CeCILL Free Software License Agreement v2.1
     (http://www.cecill.info/licences.en.html)
 """
 import os
 import re
 import logging
 from obspy import read_inventory
 from obspy.core.inventory import Inventory, Network, Station, Channel, Response
-from sourcespec.ssp_setup import instr_codes_vel, instr_codes_acc
-logger = logging.getLogger(__name__.split('.')[-1])
+from sourcespec.ssp_setup import INSTR_CODES_VEL, INSTR_CODES_ACC
+logger = logging.getLogger(__name__.rsplit('.', maxsplit=1)[-1])
 
 
 class PAZ():
     """Instrument response defined through poles and zeros."""
     zeros = []
     poles = []
     sensitivity = 1.
     _seedID = None
     network = None
     station = None
     location = None
     channel = None
     input_units = None
+    linenum = None
 
     def __init__(self, file=None):
         """
         Init PAZ object.
 
         :param file: path to the PAZ file
         :type file: str
@@ -48,14 +49,15 @@
             f'  poles: {self.poles}'
             f'  sensitivity: {self.sensitivity}'
             f'  input_units: {self.input_units}'
         )
 
     @property
     def seedID(self):
+        """Return the seedID."""
         return self._seedID
 
     @seedID.setter
     def seedID(self, seedID):
         try:
             self.network, self.station, self.location, self.channel =\
                 seedID.split('.')
@@ -71,26 +73,27 @@
         """
         Guess the input units from the seedID.
         """
         if len(self.channel) < 3:
             return
         instr_code = self.channel[1]
         self.input_units = None
-        if instr_code in instr_codes_vel:
+        if instr_code in INSTR_CODES_VEL:
             band_code = self.channel[0]
             # SEED standard band codes for velocity channels
             # https://ds.iris.edu/ds/nodes/dmc/data/formats/seed-channel-naming
             if band_code in ['B', 'C', 'D', 'E', 'F', 'G', 'H', 'S']:
                 self.input_units = 'M/S'
-        elif instr_code in instr_codes_acc:
+        elif instr_code in INSTR_CODES_ACC:
             self.input_units = 'M/S**2'
 
     def _read(self, file):
         """Read a PAZ file."""
-        self.lines = enumerate(open(file, 'r'), start=1)
+        with open(file, 'r', encoding='ascii') as fp:
+            self.lines = enumerate(fp, start=1)
         while True:
             try:
                 self._parse_paz_file_lines()
             except StopIteration:
                 break
             except Exception as e:
                 raise TypeError(
@@ -108,15 +111,15 @@
         if what in ['poles', 'zeros']:
             nvalues = int(word[1])
             poles_zeros = []
             for _ in range(nvalues):
                 self.linenum, line = next(self.lines)
                 value = complex(*map(float, line.split()))
                 poles_zeros.append(value)
-            self.__setattr__(what, poles_zeros)
+            setattr(self, what, poles_zeros)
         elif what == 'constant':
             self.sensitivity = float(word[1])
 
     def to_inventory(self):
         """
         Convert PAZ object to an Inventory object.
         """
@@ -140,15 +143,15 @@
     Read a paz file into an ``Inventory`` object.
 
     :note:
     - paz file must have ".pz" or ".paz" suffix (or no suffix)
     - paz file name (without prefix and suffix) can have
       the trace_id (NET.STA.LOC.CHAN) of the corresponding trace in the last
       part of his name (e.g., 20110208_1600.NOW.IV.CRAC.00.EHZ.paz),
-      otherwhise it will be treaten as a generic paz.
+      otherwise it will be treaten as a generic paz.
 
     :param file: path to the PAZ file
     :type file: str
 
     :return: inventory
     :rtype: :class:`~obspy.core.inventory.inventory.Inventory`
     """
@@ -204,8 +207,9 @@
             try:
                 inventory += _read_paz_file(file)
             except Exception as msg2:
                 logger.warning(msg1)
                 logger.warning(msg2)
                 continue
     logger.info('Reading station metadata: done')
+    logger.info('---------------------------------------------------')
     return inventory
```

### Comparing `sourcespec-1.7/sourcespec/ssp_read_traces.py` & `sourcespec-1.8/sourcespec/ssp_read_traces.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,50 +5,51 @@
 
 :copyright:
     2012 Claudio Satriano <satriano@ipgp.fr>
 
     2013-2014 Claudio Satriano <satriano@ipgp.fr>,
               Emanuela Matrullo <matrullo@geologie.ens.fr>
 
-    2015-2023 Claudio Satriano <satriano@ipgp.fr>,
+    2015-2024 Claudio Satriano <satriano@ipgp.fr>,
               Sophie Lambotte <sophie.lambotte@unistra.fr>
 :license:
     CeCILL Free Software License Agreement v2.1
     (http://www.cecill.info/licences.en.html)
 """
 import sys
 import os
 import logging
 import shutil
 import tarfile
+import zipfile
 import tempfile
 import contextlib
 from obspy import read
 from obspy.core import Stream
 from obspy.core.util import AttribDict
 from sourcespec.ssp_setup import (
-    ssp_exit, instr_codes_vel, instr_codes_acc, traceid_map)
-from sourcespec.ssp_util import get_vel
+    ssp_exit, INSTR_CODES_VEL, INSTR_CODES_ACC, TRACEID_MAP)
+from sourcespec.ssp_util import MediumProperties
 from sourcespec.ssp_read_station_metadata import (
     read_station_metadata, PAZ)
 from sourcespec.ssp_read_event_metadata import (
     parse_qml, parse_hypo_file, parse_hypo71_picks)
 from sourcespec.ssp_read_sac_header import (
     compute_sensitivity_from_SAC,
     get_instrument_from_SAC, get_station_coordinates_from_SAC,
-    get_hypocenter_from_SAC, get_picks_from_SAC)
-logger = logging.getLogger(__name__.split('.')[-1])
+    get_event_from_SAC, get_picks_from_SAC)
+logger = logging.getLogger(__name__.rsplit('.', maxsplit=1)[-1])
 
 
 # TRACE MANIPULATION ----------------------------------------------------------
 def _correct_traceid(trace):
-    if traceid_map is None:
+    if TRACEID_MAP is None:
         return
     with contextlib.suppress(KeyError):
-        traceid = traceid_map[trace.get_id()]
+        traceid = TRACEID_MAP[trace.get_id()]
         net, sta, loc, chan = traceid.split('.')
         trace.stats.network = net
         trace.stats.station = sta
         trace.stats.location = loc
         trace.stats.channel = chan
 
 
@@ -59,22 +60,22 @@
     instr_code = None
     trace.stats.instrtype = None
     # First, try to get the instrtype from channel name
     chan = trace.stats.channel
     if len(chan) > 2:
         band_code = chan[0]
         instr_code = chan[1]
-    if instr_code in instr_codes_vel:
+    if instr_code in INSTR_CODES_VEL:
         # SEED standard band codes from higher to lower sampling rate
         # https://ds.iris.edu/ds/nodes/dmc/data/formats/seed-channel-naming/
         if band_code in ['G', 'D', 'E', 'S']:
             instrtype = 'shortp'
         if band_code in ['F', 'C', 'H', 'B']:
             instrtype = 'broadb'
-    if instr_code in instr_codes_acc:
+    if instr_code in INSTR_CODES_ACC:
         instrtype = 'acc'
     if instrtype is None:
         # Let's see if there is an instrument name in SAC header (ISNet format)
         # In this case, we define band and instrument codes a posteriori
         instrtype, band_code, instr_code = get_instrument_from_SAC(trace)
         orientation = trace.stats.channel[-1]
         trace.stats.channel = ''.join((band_code, instr_code, orientation))
@@ -166,17 +167,22 @@
 def _add_coords(trace):
     """Add coordinates to trace."""
     # If we already know that traceid is skipped, raise a silent exception
     if trace.id in _add_coords.skipped:
         raise RuntimeError()
     coords = None
     with contextlib.suppress(Exception):
-        coords = AttribDict(
-            trace.stats.inventory.get_coordinates(
-                trace.id, trace.stats.starttime))
+        # Inventory.get_coordinates() raises a generic Exception
+        # if coordinates are not found
+        coords = trace.stats.inventory.get_coordinates(
+                    trace.id, trace.stats.starttime)
+    if coords is not None:
+        # Build an AttribDict and make sure that coordinates are floats
+        coords = AttribDict({
+            key: float(value) for key, value in coords.items()})
         coords = (
             None if (
                 coords.longitude == 0 and coords.latitude == 0 and
                 coords.local_depth == 123456 and coords.elevation == 123456)
             else coords)
     if coords is None:
         # If we still don't have trace coordinates,
@@ -190,26 +196,26 @@
     if coords.latitude == coords.longitude == 0:
         logger.warning(
             f'{trace.id}: trace has latitude and longitude equal to zero!')
     # elevation is in meters in StationXML or SAC header
     coords.elevation /= 1e3
     trace.stats.coords = coords
 # list to keep track of skipped traces
-_add_coords.skipped = []  #noqa
+_add_coords.skipped = []  # noqa
 
 
-def _add_hypocenter(trace, hypo=None):
-    """Add hypocenter information to trace."""
-    if hypo is None:
+def _add_event(trace, ssp_event=None):
+    """Add ssp_event object to trace."""
+    if ssp_event is None:
         # Try to get hypocenter information from the SAC header
         try:
-            hypo = get_hypocenter_from_SAC(trace)
+            ssp_event = get_event_from_SAC(trace)
         except Exception:
             return
-    trace.stats.hypo = hypo
+    trace.stats.event = ssp_event
 
 
 def _add_picks(trace, picks=None):
     """Add picks to trace."""
     if picks is None:
         picks = []
     trace_picks = []
@@ -246,60 +252,63 @@
                 if not [p for p in tr.stats.picks if p.phase == 'S']:
                     tr.stats.picks += default_S_pick
 # -----------------------------------------------------------------------------
 
 
 # FILE PARSING ----------------------------------------------------------------
 def _hypo_vel(hypo, config):
-    hypo.vp = get_vel(hypo.longitude, hypo.latitude, hypo.depth, 'P', config)
-    hypo.vs = get_vel(hypo.longitude, hypo.latitude, hypo.depth, 'S', config)
-    logger.info(f'Vp_hypo: {hypo.vp:.2f} km/s, Vs_hypo: {hypo.vs:.2f} km/s')
+    medium_properties = MediumProperties(
+        hypo.longitude, hypo.latitude, hypo.depth.value_in_km, config)
+    hypo.vp = medium_properties.get(mproperty='vp', where='source')
+    hypo.vs = medium_properties.get(mproperty='vs', where='source')
+    hypo.rho = medium_properties.get(mproperty='rho', where='source')
+    depth_string = medium_properties.to_string(
+        'source depth', hypo.depth.value_in_km)
+    vp_string = medium_properties.to_string('vp_source', hypo.vp)
+    vs_string = medium_properties.to_string('vs_source', hypo.vs)
+    rho_string = medium_properties.to_string('rho_source', hypo.rho)
+    logger.info(f'{depth_string}, {vp_string}, {vs_string}, {rho_string}')
 
 
 def _build_filelist(path, filelist, tmpdir):
     if os.path.isdir(path):
         listing = os.listdir(path)
         for filename in listing:
             fullpath = os.path.join(path, filename)
             _build_filelist(fullpath, filelist, tmpdir)
     else:
         try:
+            # pylint: disable=unspecified-encoding consider-using-with
             open(path)
         except IOError as err:
             logger.error(err)
             return
         if tarfile.is_tarfile(path) and tmpdir is not None:
-            tar = tarfile.open(path)
-            tar.extractall(path=tmpdir)
-            tar.close()
+            with tarfile.open(path) as tar:
+                try:
+                    tar.extractall(path=tmpdir)
+                except Exception as msg:
+                    logger.warning(
+                        f'{path}: Unable to fully extract tar archive: {msg}')
+        elif zipfile.is_zipfile(path) and tmpdir is not None:
+            with zipfile.ZipFile(path) as zipf:
+                try:
+                    zipf.extractall(path=tmpdir)
+                except Exception as msg:
+                    logger.warning(
+                        f'{path}: Unable to fully extract zip archive: {msg}')
         else:
             filelist.append(path)
-# -----------------------------------------------------------------------------
 
 
-# Public interface:
-def read_traces(config):
-    """Read traces, store waveforms and metadata."""
-    # read station metadata into an ObsPy ``Inventory`` object
-    inventory = read_station_metadata(config.station_metadata)
-
-    picks = []
-    hypo = None
-    # parse hypocenter file
-    if config.options.hypo_file is not None:
-        hypo, picks = parse_hypo_file(config.options.hypo_file)
-    # parse pick file
-    if config.options.pick_file is not None:
-        picks = parse_hypo71_picks(config)
-    # parse QML file
-    if config.options.qml_file is not None:
-        hypo, picks = parse_qml(config.options.qml_file, config.options.evid)
-
-    # finally, read traces
-    logger.info('Reading traces...')
+def _read_trace_files(config, inventory, ssp_event, picks):
+    """
+    Read trace files from a given path. Complete trace metadata and
+    return a stream object.
+    """
     # phase 1: build a file list
     # ph 1.1: create a temporary dir and run '_build_filelist()'
     #         to move files to it and extract all tar archives
     tmpdir = tempfile.mkdtemp()
     filelist = []
     for trace_path in config.options.trace_path:
         _build_filelist(trace_path, filelist, tmpdir)
@@ -336,43 +345,89 @@
                 continue
             _correct_traceid(trace)
             try:
                 _add_instrtype(trace)
                 _add_inventory(trace, inventory, config)
                 _check_instrtype(trace)
                 _add_coords(trace)
-                _add_hypocenter(trace, hypo)
+                _add_event(trace, ssp_event)
                 _add_picks(trace, picks)
             except Exception as err:
                 for line in str(err).splitlines():
                     logger.warning(line)
                 continue
             st.append(trace)
     shutil.rmtree(tmpdir)
+    return st
+# -----------------------------------------------------------------------------
 
-    logger.info('Reading traces: done')
-    if len(st.traces) == 0:
-        logger.info('No trace loaded')
-        ssp_exit()
 
+def _log_event_info(ssp_event):
+    for line in str(ssp_event).splitlines():
+        logger.info(line)
+    logger.info('---------------------------------------------------')
+
+
+# Public interface:
+def read_traces(config):
+    """Read traces, store waveforms and metadata."""
+    # read station metadata into an ObsPy ``Inventory`` object
+    inventory = read_station_metadata(config.station_metadata)
+
+    picks = []
+    ssp_event = None
+    # parse hypocenter file
+    if config.options.hypo_file is not None:
+        ssp_event, picks, file_format = parse_hypo_file(
+            config.options.hypo_file, config.options.evid)
+        config.hypo_file_format = file_format
+    # parse pick file
+    if config.options.pick_file is not None:
+        picks = parse_hypo71_picks(config)
+    # parse QML file
+    if config.options.qml_file is not None:
+        ssp_event, picks = parse_qml(config)
+    if ssp_event is not None:
+        _log_event_info(ssp_event)
+
+    # finally, read trace files
+    logger.info('Reading traces...')
+    st = _read_trace_files(config, inventory, ssp_event, picks)
+    logger.info('Reading traces: done')
+    logger.info('---------------------------------------------------')
+    if len(st) == 0:
+        logger.error('No trace loaded')
+        ssp_exit(1)
     _complete_picks(st)
 
-    # if hypo is still None, get it from first trace
-    if hypo is None:
+    # if ssp_event is still None, get it from first trace
+    if ssp_event is None:
         try:
-            hypo = st[0].stats.hypo
+            ssp_event = st[0].stats.event
+            _log_event_info(ssp_event)
         except AttributeError:
             logger.error('No hypocenter information found.')
             sys.stderr.write(
                 '\n'
                 'Use "-q" or "-H" options to provide hypocenter information\n'
                 'or add hypocenter information to the SAC file header\n'
                 '(if you use the SAC format).\n'
             )
-            ssp_exit()
-    # add vs to hypo
-    _hypo_vel(hypo, config)
-    # add hypo to config file
-    config.hypo = hypo
+            ssp_exit(1)
+    # add velocity info to hypocenter
+    try:
+        _hypo_vel(ssp_event.hypocenter, config)
+    except Exception as e:
+        logger.error(
+            f'Unable to compute velocity at hypocenter: {e}\n')
+        ssp_exit(1)
+    if config.options.evname is not None:
+        # add evname from command line, if any, overriding the one in ssp_event
+        ssp_event.name = config.options.evname
+    else:
+        # add evname from ssp_event, if any, to config file
+        config.options.evname = ssp_event.name
+    # add event to config file
+    config.event = ssp_event
 
     st.sort()
     return st
```

### Comparing `sourcespec-1.7/sourcespec/ssp_residuals.py` & `sourcespec-1.8/sourcespec/ssp_residuals.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,52 +3,56 @@
 """
 Spectral residual routine for sourcespec.
 
 :copyright:
     2013-2014 Claudio Satriano <satriano@ipgp.fr>,
               Agnes Chounet <chounet@ipgp.fr>
 
-    2015-2023 Claudio Satriano <satriano@ipgp.fr>
+    2015-2024 Claudio Satriano <satriano@ipgp.fr>
 :license:
     CeCILL Free Software License Agreement v2.1
     (http://www.cecill.info/licences.en.html)
 """
 import os
 import logging
-import pickle
-from obspy.core import Stream
+from sourcespec._version import get_versions
+from sourcespec.spectrum import SpectrumStream
 from sourcespec.ssp_spectral_model import spectral_model
 from sourcespec.ssp_util import mag_to_moment
-logger = logging.getLogger(__name__.split('.')[-1])
+logger = logging.getLogger(__name__.rsplit('.', maxsplit=1)[-1])
 
 
 def spectral_residuals(config, spec_st, sspec_output):
     """
     Compute spectral residuals with respect to an average spectral model.
+    Saves a stream of residuals to disk in HDF5 format.
 
-    Saves a stream of residuals to disk using pickle.
+    :param config: Configuration object
+    :type config: :class:`~sourcespec.config.Config`
+    :param spec_st: Stream of spectra
+    :type spec_st: :class:`~sourcespec.spectrum.SpectrumStream`
+    :param sspec_output: Output of the source spectral parameter estimation
+    :type sspec_output: :class:`~sourcespec.ssp_data_types.SourceSpecOutput`
     """
     # get reference summary values
     summary_values = sspec_output.reference_values()
     params_name = ('Mw', 'fc', 't_star')
     sourcepar_summary = {p: summary_values[p] for p in params_name}
-    residuals = Stream()
-    for station in {x.stats.station for x in spec_st.traces}:
+    residuals = SpectrumStream()
+    for station in {x.stats.station for x in spec_st}:
         spec_st_sel = spec_st.select(station=station)
-        for spec in spec_st_sel.traces:
+        for spec in spec_st_sel:
             if spec.stats.channel[-1] != 'H':
                 continue
-
-            xdata = spec.get_freq()
+            xdata = spec.freq
             synth_mean_mag = spectral_model(xdata, **sourcepar_summary)
-
             res = spec.copy()
             res.data_mag = spec.data_mag - synth_mean_mag
             res.data = mag_to_moment(res.data_mag)
+            res.stats.software = 'SourceSpec'
+            res.stats.software_version = get_versions()['version']
             residuals.append(res)
-
-    # Save residuals as pickle file
-    evid = config.hypo.evid
-    res_file = os.path.join(config.options.outdir, f'{evid}-residuals.pickle')
-    with open(res_file, 'wb') as fp:
-        pickle.dump(residuals, fp)
+    # Save residuals to HDF5 file
+    evid = config.event.event_id
+    res_file = os.path.join(config.options.outdir, f'{evid}.residuals.hdf5')
+    residuals.write(res_file, format='HDF5')
     logger.info(f'Spectral residuals saved to: {res_file}')
```

### Comparing `sourcespec-1.7/sourcespec/ssp_setup.py` & `sourcespec-1.8/sourcespec/ssp_setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,93 +6,96 @@
 :copyright:
     2012 Claudio Satriano <satriano@ipgp.fr>
 
     2013-2014 Claudio Satriano <satriano@ipgp.fr>,
               Emanuela Matrullo <matrullo@geologie.ens.fr>,
               Agnes Chounet <chounet@ipgp.fr>
 
-    2015-2023 Claudio Satriano <satriano@ipgp.fr>
+    2015-2024 Claudio Satriano <satriano@ipgp.fr>
 :license:
     CeCILL Free Software License Agreement v2.1
     (http://www.cecill.info/licences.en.html)
 """
 import sys
 import os
 import platform
 import shutil
 import logging
 import signal
 import uuid
 import json
 import contextlib
 import warnings
+from copy import copy
 from datetime import datetime
 from collections import defaultdict
+from sourcespec import __version__, __banner__
 from sourcespec.configobj import ConfigObj
 from sourcespec.configobj.validate import Validator
 from sourcespec.config import Config
-from sourcespec._version import get_versions
+from sourcespec.ssp_update_db import update_db_file
 
 # define ipshell(), if possible
 # note: ANSI colors do not work on Windows standard terminal
 if sys.stdout.isatty() and sys.platform != 'win32':
     try:
         from IPython.terminal.embed import InteractiveShellEmbed
-        ipshell = InteractiveShellEmbed()
+        IPSHELL = InteractiveShellEmbed.instance()
     except ImportError:
-        ipshell = None
+        IPSHELL = None
 else:
-    ipshell = None
+    IPSHELL = None
 
 # global variables
 OS = os.name
-oldlogfile = None
-logger = None
-ssp_exit_called = False
-traceid_map = None
+OLDLOGFILE = None
+LOGGER = None
+SSP_EXIT_CALLED = False
+TRACEID_MAP = None
 # SEED standard instrument codes:
 # https://ds.iris.edu/ds/nodes/dmc/data/formats/seed-channel-naming/
-instr_codes_vel = ['H', 'L']
-instr_codes_acc = ['N', ]
+INSTR_CODES_VEL = ['H', 'L']
+INSTR_CODES_ACC = ['N', ]
 OBSPY_VERSION = None
 OBSPY_VERSION_STR = None
 NUMPY_VERSION_STR = None
 SCIPY_VERSION_STR = None
 MATPLOTLIB_VERSION_STR = None
 CARTOPY_VERSION_STR = None
 PYTHON_VERSION_STR = None
 
 
 def _check_obspy_version():
-    global OBSPY_VERSION, OBSPY_VERSION_STR
+    global OBSPY_VERSION, OBSPY_VERSION_STR  # pylint: disable=global-statement
     # check ObsPy version
+    # pylint: disable=import-outside-toplevel
     import obspy
     MIN_OBSPY_VERSION = (1, 2, 0)
     OBSPY_VERSION_STR = obspy.__version__
     OBSPY_VERSION = OBSPY_VERSION_STR.split('.')[:3]
     # special case for "rc" versions:
     OBSPY_VERSION[2] = OBSPY_VERSION[2].split('rc')[0]
     OBSPY_VERSION = tuple(map(int, OBSPY_VERSION))
     with contextlib.suppress(IndexError):
         # add half version number for development versions
         # check if there is a fourth field in version string:
-        OBSPY_VERSION_STR.split('.')[3]
         OBSPY_VERSION = OBSPY_VERSION[:2] + (OBSPY_VERSION[2] + 0.5,)
     if OBSPY_VERSION < MIN_OBSPY_VERSION:
         MIN_OBSPY_VERSION_STR = '.'.join(map(str, MIN_OBSPY_VERSION))
         sys.stderr.write(
             f'ERROR: ObsPy >= {MIN_OBSPY_VERSION_STR} is required. '
             f'You have version: {OBSPY_VERSION_STR}\n')
         sys.exit(1)
 
 
 def _cartopy_download_gshhs():
     """
     Download GSHHS data for cartopy.
     """
+    # pylint: disable=import-outside-toplevel
     from cartopy.io.shapereader import GSHHSShpDownloader as Downloader
     from cartopy import config as cartopy_config
     from pathlib import Path
     gshhs_downloader = Downloader.from_config(('shapefiles', 'gshhs'))
     format_dict = {'config': cartopy_config, 'scale': 'f', 'level': 1}
     target_path = gshhs_downloader.target_path(format_dict)
     if not os.path.exists(target_path):
@@ -116,14 +119,15 @@
 def _cartopy_download_borders():
     """
     Download borders data for cartopy.
 
     Inspired from
     https://github.com/SciTools/cartopy/blob/main/tools/cartopy_feature_download.py
     """
+    # pylint: disable=import-outside-toplevel
     from cartopy.io import Downloader
     from cartopy import config as cartopy_config
     from pathlib import Path
     category = 'cultural'
     name = 'admin_0_boundary_lines_land'
     scales = ('10m', '50m')
     for scale in scales:
@@ -147,52 +151,54 @@
                         'Check your internet connection.\n')
                     sys.exit(1)
             sys.stdout.write(
                 f'Done! Data cached to {Path(path).parents[0]}\n\n')
 
 
 def _check_cartopy_version():
-    cartopy_min_ver = (0, 18, 0)
+    cartopy_min_ver = (0, 21, 0)
     try:
         cartopy_ver = None
-        import cartopy  #NOQA
-        global CARTOPY_VERSION_STR
+        import cartopy  # NOQA pylint: disable=import-outside-toplevel
+        global CARTOPY_VERSION_STR  # pylint: disable=global-statement
         CARTOPY_VERSION_STR = cartopy.__version__
         cartopy_ver = tuple(map(int, cartopy.__version__.split('.')[:3]))
         if cartopy_ver < cartopy_min_ver:
             raise ImportError
         _cartopy_download_gshhs()
         _cartopy_download_borders()
     except ImportError as e:
         cartopy_min_ver_str = '.'.join(map(str, cartopy_min_ver))
         msg = (
             f'\nPlease install cartopy >= {cartopy_min_ver_str} to plot maps.'
             '\nHow to install: '
             'https://scitools.org.uk/cartopy/docs/latest/installing.html\n\n'
-            'Alternatively, set "plot_station_map" and "html_report" to '
-            '"False" in config file.\n'
+            'Alternatively, set "plot_station_map" to "False" '
+            'in config file.\n'
         )
         if cartopy_ver is not None:
             msg += f'Installed cartopy version: {CARTOPY_VERSION_STR}.\n'
         raise ImportError(msg) from e
 
 
 def _check_pyproj_version():
+    # pylint: disable=import-outside-toplevel
     try:
-        import pyproj  #NOQA
+        import pyproj # noqa pylint: disable=unused-import
     except ImportError as e:
         msg = '\nPlease install pyproj to plot maps.\n'
         raise ImportError(msg) from e
 
 
 def _check_nllgrid_version():
+    # pylint: disable=import-outside-toplevel
     nllgrid_min_ver = (1, 4, 2)
     try:
         nllgrid_ver = None
-        import nllgrid  #NOQA
+        import nllgrid  # NOQA
         nllgrid_ver_str = nllgrid.__version__.split('+')[0]
         nllgrid_ver = tuple(map(int, nllgrid_ver_str.split('.')))
         # nllgrid versions are sometimes X.Y, other times X.Y.Z
         while len(nllgrid_ver) < 3:
             nllgrid_ver = (*nllgrid_ver, 0)
         if nllgrid_ver < nllgrid_min_ver:
             raise ImportError
@@ -205,14 +211,16 @@
         )
         if nllgrid_ver is not None:
             msg += f'Installed nllgrid version: {nllgrid.__version__}\n'
         raise ImportError(msg) from e
 
 
 def _check_library_versions():
+    # pylint: disable=import-outside-toplevel
+    # pylint: disable=global-statement
     global PYTHON_VERSION_STR
     global NUMPY_VERSION_STR
     global SCIPY_VERSION_STR
     global MATPLOTLIB_VERSION_STR
     PYTHON_VERSION_STR = '.'.join(map(str, sys.version_info[:3]))
     import numpy
     NUMPY_VERSION_STR = numpy.__version__
@@ -220,44 +228,49 @@
     SCIPY_VERSION_STR = scipy.__version__
     import matplotlib
     MATPLOTLIB_VERSION_STR = matplotlib.__version__
     MATPLOTLIB_VERSION = MATPLOTLIB_VERSION_STR.split('.')[:3]
     MATPLOTLIB_VERSION = tuple(map(int, MATPLOTLIB_VERSION))
     MAX_MATPLOTLIB_VERSION = (3, 9, 0)
     if MATPLOTLIB_VERSION >= MAX_MATPLOTLIB_VERSION:
-        MAX_MATPLOTLIB_VERSION_STR = '.'.join(
-            map(str, MAX_MATPLOTLIB_VERSION))
+        MAX_MATPLOTLIB_VERSION_STR = '.'.join(map(str, MAX_MATPLOTLIB_VERSION))
         sys.stderr.write(
             f'ERROR: Matplotlib >= {MAX_MATPLOTLIB_VERSION_STR}'
             'is not yet supported. Please use a less recent version'
             f' You have version: {MATPLOTLIB_VERSION_STR}\n'
         )
         sys.exit(1)
 
 
 def _read_config(config_file, configspec=None):
-    kwargs = dict(
-        configspec=configspec, file_error=True, default_encoding='utf8')
+    kwargs = {
+        'configspec': configspec,
+        'file_error': True,
+        'default_encoding': 'utf8'
+    }
     if configspec is None:
-        kwargs.update(
-            dict(interpolation=False, list_values=False, _inspec=True))
+        kwargs.update({
+            'interpolation': False,
+            'list_values': False,
+            '_inspec': True
+        })
     try:
         config_obj = ConfigObj(config_file, **kwargs)
     except IOError as err:
         sys.stderr.write(f'{err}\n')
         sys.exit(1)
     except Exception as err:
         sys.stderr.write(f'Unable to read "{config_file}": {err}\n')
         sys.exit(1)
     return config_obj
 
 
 def _parse_configspec():
     configspec_file = os.path.join(
-        os.path.dirname(__file__), 'configspec.conf')
+        os.path.dirname(__file__), 'config_files', 'configspec.conf')
     return _read_config(configspec_file)
 
 
 def _write_sample_config(configspec, progname):
     c = ConfigObj(configspec=configspec, default_encoding='utf8')
     val = Validator()
     c.validate(val)
@@ -319,37 +332,47 @@
         'dataless': 'station_metadata',
         'clip_nmax': 'clip_max_percent',
         'PLOT_SHOW': 'plot_show',
         'PLOT_SAVE': 'plot_save',
         'PLOT_SAVE_FORMAT': 'plot_save_format',
         'vp': 'vp_source',
         'vs': 'vs_source',
+        'rho': 'rho_source',
         'pre_p_time': 'noise_pre_time',
         'pre_s_time': 'signal_pre_time',
         'rps_from_focal_mechanism': 'rp_from_focal_mechanism',
         'paz': 'station_metadata',
+        'pi_bsd_min_max': 'pi_ssd_min_max',
+        'max_epi_dist': 'epi_dist_ranges'
     }
     for old_opt, new_opt in migrate_options.items():
         if old_opt in config_obj and config_obj[old_opt] != 'None':
-            config_new[new_opt] = config_obj[old_opt]
+            # max_epi_dist needs to be converted to a list
+            if old_opt == 'max_epi_dist':
+                config_new[new_opt] = [0, config_obj[old_opt]]
+            else:
+                config_new[new_opt] = config_obj[old_opt]
     shutil.copyfile(config_file, config_file_old)
     with open(config_file, 'wb') as fp:
         config_new.write(fp)
         print(f'{config_file}: updated')
 
 
 def _write_config(config_obj, progname, outdir):
     if progname != 'source_spec':
         return
     configfile = f'{progname}.conf'
     configfile = os.path.join(outdir, configfile)
     if not os.path.exists(outdir):
         os.makedirs(outdir)
     with open(configfile, 'wb') as fp:
-        config_obj.write(fp)
+        # create a copy of config_obj and remove the basemap API key
+        _tmp_config_obj = copy(config_obj)
+        _tmp_config_obj['plot_map_api_key'] = None
+        _tmp_config_obj.write(fp)
 
 
 def _check_deprecated_config_options(config_obj):
     deprecation_msgs = []
     if 's_win_length' in config_obj or 'noise_win_length' in config_obj:
         deprecation_msgs.append(
             '> "s_win_length" and "noise_win_length" config parameters '
@@ -402,14 +425,18 @@
         deprecation_msgs.append(
             '> "vp" config parameter has been renamed to "vp_source".\n'
         )
     if 'vs' in config_obj:
         deprecation_msgs.append(
             '> "vs" config parameter has been renamed to "vs_source".\n'
         )
+    if 'rho' in config_obj:
+        deprecation_msgs.append(
+            '> "rho" config parameter has been renamed to "rho_source".\n'
+        )
     if 'pre_p_time' in config_obj:
         deprecation_msgs.append(
             '> "pre_p_time" config parameter has been renamed to '
             '"noise_pre_time".\n'
         )
     if 'pre_s_time' in config_obj:
         deprecation_msgs.append(
@@ -422,28 +449,39 @@
             'to "rp_from_focal_mechanism".\n'
         )
     if 'paz' in config_obj:
         deprecation_msgs.append(
             '> "paz" config parameter has been removed and merged with '
             '"station_metadata".\n'
         )
+    if 'max_epi_dist' in config_obj:
+        deprecation_msgs.append(
+            '> "max_epi_dist" config parameter has been removed and replaced '
+            'by "epi_dist_ranges".\n'
+        )
+    if 'max_freq_Er' in config_obj:
+        deprecation_msgs.append(
+            '> "max_freq_Er" config parameter has been removed and replaced '
+            'by "Er_freq_min_max".\n'
+        )
     if deprecation_msgs:
         sys.stderr.write(
             'Error: your config file contains deprecated parameters:\n\n')
     for msg in deprecation_msgs:
         sys.stderr.write(msg)
     if deprecation_msgs:
         sys.stderr.write(
             '\nPlease upgrade your config file manually or '
             'via the "-U" option.\n'
         )
         sys.exit(1)
 
 
 def _init_plotting(plot_show):
+    # pylint: disable=import-outside-toplevel
     import matplotlib.pyplot as plt
     if not plot_show:
         plt.switch_backend('Agg')
 
 
 def _check_mandatory_config_params(config_obj):
     mandatory_params = [
@@ -465,15 +503,14 @@
         'freq1_shortp',
         'freq2_shortp',
         'freq1_broadb',
         'freq2_broadb',
         'rmsmin',
         'sn_min',
         'spectral_sn_min',
-        'rho',
         'rpp',
         'rps',
         'geom_spread_n_exponent',
         'geom_spread_cutoff_distance',
         'f_weight',
         'weight',
         't_star_0',
@@ -501,49 +538,115 @@
         ssp_exit(1)
 
 
 def _init_instrument_codes(config):
     """
     Initialize instrument codes from config file.
     """
-    global instr_codes_vel
-    global instr_codes_acc
     # User-defined instrument codes:
     instr_code_acc_user = config.instrument_code_acceleration
     instr_code_vel_user = config.instrument_code_velocity
     # Remove user-defined instrument codes if they conflict
     # with another instrument
     with contextlib.suppress(ValueError):
-        instr_codes_vel.remove(instr_code_acc_user)
+        INSTR_CODES_VEL.remove(instr_code_acc_user)
     with contextlib.suppress(ValueError):
-        instr_codes_acc.remove(instr_code_vel_user)
+        INSTR_CODES_ACC.remove(instr_code_vel_user)
     # Add user-defined instrument codes
     if instr_code_vel_user is not None:
-        instr_codes_vel.append(instr_code_vel_user)
+        INSTR_CODES_VEL.append(instr_code_vel_user)
     if instr_code_acc_user is not None:
-        instr_codes_acc.append(instr_code_acc_user)
+        INSTR_CODES_ACC.append(instr_code_acc_user)
 
 
 def _init_traceid_map(traceid_map_file):
     """
     Initialize trace ID map from file.
     """
-    global traceid_map
+    global TRACEID_MAP  # pylint: disable=global-statement
     if traceid_map_file is None:
         return
     try:
-        with open(traceid_map_file, 'r') as fp:
-            traceid_map = json.loads(fp.read())
+        with open(traceid_map_file, 'r', encoding='utf-8') as fp:
+            TRACEID_MAP = json.loads(fp.read())
     except Exception:
         sys.stderr.write(
             f'traceid mapping file "{traceid_map_file}" not found '
             'or not in json format.\n')
         ssp_exit(1)
 
 
+def _write_sample_ssp_event_file():
+    ssp_event_file = 'ssp_event.yaml'
+    src_path = os.path.join(
+        os.path.dirname(__file__), 'config_files', 'ssp_event.yaml')
+    dest_path = os.path.join('.', ssp_event_file)
+    write_file = True
+    if os.path.exists(dest_path):
+        ans = input(
+            f'{ssp_event_file} already exists. '
+            'Do you want to overwrite it? [y/N] '
+        )
+        write_file = ans in ['y', 'Y']
+    if write_file:
+        shutil.copyfile(src_path, dest_path)
+        print(f'Sample SourceSpec Event File written to: {ssp_event_file}')
+
+
+def _fix_and_expand_path(path):
+    """
+    Fix any path issues and expand it.
+
+    :param str path: Path specification
+    :return: The fixed and expanded path
+    :rtype: str
+    """
+    fixed_path = os.path.normpath(path).split(os.sep)
+    fixed_path = os.path.join(*fixed_path)
+    if path.startswith(os.sep):
+        fixed_path = os.path.join(os.sep, fixed_path)
+    elif path.startswith('~'):
+        fixed_path = os.path.expanduser(fixed_path)
+    return fixed_path
+
+
+def _float_list(input_list, max_length=None, accepted_values=None):
+    """
+    Convert an input list to a list of floats.
+
+    :param list input_list: Input list or None
+    :return: A list of floats or None
+    :rtype: list
+    """
+    if input_list is None:
+        return None
+    if accepted_values is None:
+        accepted_values = []
+
+    def _parse_float(val):
+        val = None if val == 'None' else val
+        return val if val in accepted_values else float(val)
+
+    try:
+        return [_parse_float(val) for val in input_list[:max_length]]
+    except ValueError as e:
+        raise ValueError('Cannot parse all values in list') from e
+
+
+def _none_lenght(input_list):
+    """
+    Return the length of input list, or 1 if input list is None
+
+    :param list input_list: Input list or None
+    :return: List length or 1
+    :rtype: int
+    """
+    return 1 if input_list is None else len(input_list)
+
+
 def configure(options, progname, config_overrides=None):
     """
     Parse command line arguments and read config file.
 
     :param object options: An object containing command line options
     :param str progname: The name of the program
     :param dict config_overrides: A dictionary with parameters that override or
@@ -556,15 +659,23 @@
     configspec = _parse_configspec()
     if options.sampleconf:
         _write_sample_config(configspec, progname)
         sys.exit(0)
     if options.updateconf:
         _update_config_file(options.updateconf, configspec)
         sys.exit(0)
+    if options.updatedb:
+        update_db_file(options.updatedb)
+        sys.exit(0)
+    if options.samplesspevent:
+        _write_sample_ssp_event_file()
+        sys.exit(0)
 
+    if options.config_file:
+        options.config_file = _fix_and_expand_path(options.config_file)
     config_obj = _read_config(options.config_file, configspec)
 
     # Apply overrides
     if config_overrides is not None:
         try:
             for key, value in config_overrides.items():
                 config_obj[key] = value
@@ -574,27 +685,43 @@
     # Set to None all the 'None' strings
     for key, value in config_obj.dict().items():
         if value == 'None':
             config_obj[key] = None
 
     val = Validator()
     test = config_obj.validate(val)
+    # test is:
+    # - True if everything is ok
+    # - False if no config value is provided
+    # - A dict if invalid values are present, with the invalid values as False
     if isinstance(test, dict):
-        for entry in test:
-            if not test[entry]:
-                sys.stderr.write(
-                    f'Invalid value for "{entry}": "{config_obj[entry]}"\n')
+        for entry in [e for e in test if not test[e]]:
+            sys.stderr.write(
+                f'Invalid value for "{entry}": "{config_obj[entry]}"\n')
         sys.exit(1)
     if not test:
         sys.stderr.write('No configuration value present!\n')
         sys.exit(1)
 
     _check_deprecated_config_options(config_obj)
     _check_mandatory_config_params(config_obj)
 
+    # Fix and expand paths in options
+    options.outdir = _fix_and_expand_path(options.outdir)
+    if options.trace_path:
+        # trace_path is a list
+        options.trace_path = [
+            _fix_and_expand_path(path) for path in options.trace_path]
+    if options.qml_file:
+        options.qml_file = _fix_and_expand_path(options.qml_file)
+    if options.hypo_file:
+        options.hypo_file = _fix_and_expand_path(options.hypo_file)
+    if options.pick_file:
+        options.pick_file = _fix_and_expand_path(options.pick_file)
+
     # Create a 'no_evid_' subdir into outdir.
     # The random hex string will make it sure that this name is unique
     # It will be then renamed once an evid is available
     hexstr = uuid.uuid4().hex
     options.outdir = os.path.join(options.outdir, f'no_evid_{hexstr}')
     _write_config(config_obj, progname, options.outdir)
 
@@ -614,14 +741,55 @@
     config.horizontal_channel_codes_2 = ['E', 'T']
     msc = config.mis_oriented_channels
     if msc is not None:
         config.vertical_channel_codes.append(msc[0])
         config.horizontal_channel_codes_1.append(msc[1])
         config.horizontal_channel_codes_2.append(msc[2])
 
+    # Fix and expand paths in config
+    if config.database_file:
+        config.database_file = _fix_and_expand_path(config.database_file)
+    if config.traceid_mapping_file:
+        config.traceid_mapping_file = _fix_and_expand_path(
+            config.traceid_mapping_file)
+    if config.station_metadata:
+        config.station_metadata = _fix_and_expand_path(config.station_metadata)
+    if config.residuals_filepath:
+        config.residuals_filepath = _fix_and_expand_path(
+            config.residuals_filepath)
+
+    # Parse force_list options into lists of float
+    try:
+        for param in [
+                'vp_source', 'vs_source', 'rho_source', 'layer_top_depths']:
+            config[param] = _float_list(config[param])
+    except ValueError as msg:
+        sys.exit(f'Error parsing parameter "{param}": {msg}')
+    n_vp_source = _none_lenght(config.vp_source)
+    n_vs_source = _none_lenght(config.vs_source)
+    n_rho_source = _none_lenght(config.rho_source)
+    n_layer_top_depths = _none_lenght(config.layer_top_depths)
+    try:
+        assert n_vp_source == n_vs_source == n_rho_source == n_layer_top_depths
+    except AssertionError:
+        sys.exit(
+            'Error: "vp_source", "vs_source", "rho_source", and '
+            '"layer_top_depths" must have the same length.'
+        )
+
+    # Check the Er_freq_range parameter
+    if config.Er_freq_range is None:
+        config.Er_freq_range = [None, None]
+    try:
+        config.Er_freq_range = _float_list(
+            config.Er_freq_range, max_length=2,
+            accepted_values=[None, 'noise'])
+    except ValueError as msg:
+        sys.exit(f'Error parsing parameter "Er_freq_range": {msg}')
+
     # A list of warnings to be issued when logger is set up
     config.warnings = []
 
     if config.html_report:
         if not config.plot_save:
             msg = (
                 'The "html_report" option is selected but "plot_save" '
@@ -651,40 +819,45 @@
             sys.exit(1)
 
     _init_instrument_codes(config)
     _init_traceid_map(config.traceid_mapping_file)
     _init_plotting(config.plot_show)
     # Create a dict to store figure paths
     config.figures = defaultdict(list)
+    # store the absolute path of the current working directory
+    config.workdir = os.getcwd()
     return config
 
 
 def save_config(config):
     """Save config file to output dir."""
     # Actually, it renames the file already existing.
     src = os.path.join(config.options.outdir, 'source_spec.conf')
-    evid = config.hypo.evid
+    evid = config.event.event_id
     dst = os.path.join(config.options.outdir, f'{evid}.ssp.conf')
     # On Windows, dst file must not exist
     with contextlib.suppress(Exception):
         os.remove(dst)
     os.rename(src, dst)
 
 
 def move_outdir(config):
     """Move outdir to a new dir named from evid (and optional run_id)."""
     try:
-        evid = config.hypo.evid
+        evid = config.event.event_id
     except Exception:
         return
     src = config.options.outdir
     run_id = config.options.run_id
-    path = os.path.normpath(config.options.outdir).split(os.sep)
-    dst = os.path.join(*path[:-1], str(evid))
-    if run_id:
+    run_id_subdir = config.options.run_id_subdir
+    dst = os.path.split(src)[0]
+    dst = os.path.join(dst, str(evid))
+    if run_id and run_id_subdir:
+        dst = os.path.join(dst, str(run_id))
+    elif run_id:
         dst += f'_{run_id}'
     # Create destination
     if not os.path.exists(dst):
         os.makedirs(dst)
     # Copy all files into destination
     file_names = os.listdir(src)
     for file_name in file_names:
@@ -710,24 +883,24 @@
     """
     Add color-coding to the logging handler emitter.
 
     Source: https://stackoverflow.com/a/20707569/2021880
     """
     def new(*args):
         levelno = args[0].levelno
-        if(levelno >= logging.CRITICAL):
+        if levelno >= logging.CRITICAL:
             color = '\x1b[31;1m'  # red
-        elif(levelno >= logging.ERROR):
+        elif levelno >= logging.ERROR:
             color = '\x1b[31;1m'  # red
-        elif(levelno >= logging.WARNING):
+        elif levelno >= logging.WARNING:
             color = '\x1b[33;1m'  # yellow
-        elif(levelno >= logging.INFO):
+        elif levelno >= logging.INFO:
             # color = '\x1b[32;1m'  # green
             color = '\x1b[0m'  # no color
-        elif(levelno >= logging.DEBUG):
+        elif levelno >= logging.DEBUG:
             color = '\x1b[35;1m'  # purple
         else:
             color = '\x1b[0m'  # no color
         # Color-code the message
         args[0].msg = f'{color}{args[0].msg}\x1b[0m'
         return fn(*args)
     return new
@@ -738,46 +911,41 @@
     Set up the logging infrastructure.
 
     This function is typically called twice: the first time without basename
     and a second time with a basename (typically the eventid).
     When called the second time, the previous logfile is renamed using the
     given basename.
     """
-    global oldlogfile
-    global logger
-    global PYTHON_VERSION_STR
-    global OBSPY_VERSION_STR
-    global NUMPY_VERSION_STR
-    global SCIPY_VERSION_STR
-    global MATPLOTLIB_VERSION_STR
-    global CARTOPY_VERSION_STR
+    # pylint: disable=global-statement
+    global OLDLOGFILE
+    global LOGGER
     # Create outdir
     if not os.path.exists(config.options.outdir):
         os.makedirs(config.options.outdir)
 
     if basename:
         logfile = os.path.join(config.options.outdir, f'{basename}.ssp.log')
     else:
         datestring = datetime.now().strftime('%Y%m%d_%H%M%S')
         logfile = os.path.join(config.options.outdir, f'{datestring}.ssp.log')
 
     logger_root = logging.getLogger()
-    if oldlogfile:
+    if OLDLOGFILE:
         hdlrs = logger_root.handlers[:]
         for hdlr in hdlrs:
             hdlr.flush()
             hdlr.close()
             logger_root.removeHandler(hdlr)
         # Copy old logfile to new
-        shutil.copyfile(oldlogfile, logfile)
+        shutil.copyfile(OLDLOGFILE, logfile)
         # Remove old logfile from old and new dir
-        os.remove(oldlogfile)
-        oldlogfile = os.path.join(
-            config.options.outdir, os.path.basename(oldlogfile))
-        os.remove(oldlogfile)
+        os.remove(OLDLOGFILE)
+        OLDLOGFILE = os.path.join(
+            config.options.outdir, os.path.basename(OLDLOGFILE))
+        os.remove(OLDLOGFILE)
         filemode = 'a'
     else:
         filemode = 'w'
 
     # captureWarnings is not supported in old versions of python
     with contextlib.suppress(Exception):
         logging.captureWarnings(True)
@@ -793,54 +961,63 @@
     console.setLevel(logging.INFO)
 
     # Add logger color coding on all platforms but win32
     if sys.platform != 'win32' and sys.stdout.isatty():
         console.emit = _color_handler_emit(console.emit)
     logger_root.addHandler(console)
 
-    logger = logging.getLogger(progname)
+    LOGGER = logging.getLogger(progname)
 
     # Only write these debug infos for a new logfile
-    if not oldlogfile:
-        logger.debug('source_spec START')
-        logger.debug('SourceSpec version: ' + get_versions()['version'])
-        uname = platform.uname()
-        uname_str = f'{uname[0]} {uname[2]} {uname[4]}'
-        logger.debug(f'Platform: {uname_str}')
-        logger.debug(f'Python version: {PYTHON_VERSION_STR}')
-        logger.debug(f'ObsPy version: {OBSPY_VERSION_STR}')
-        logger.debug(f'NumPy version: {NUMPY_VERSION_STR}')
-        logger.debug(f'SciPy version: {SCIPY_VERSION_STR}')
-        logger.debug(f'Matplotlib version: {MATPLOTLIB_VERSION_STR}')
-        if CARTOPY_VERSION_STR is not None:
-            logger.debug(f'Cartopy version: {CARTOPY_VERSION_STR}')
-        logger.debug('Running arguments:')
-        logger.debug(' '.join(sys.argv))
-    oldlogfile = logfile
+    if not OLDLOGFILE:
+        _log_debug_information()
+    OLDLOGFILE = logfile
 
     # See if there are warnings to deliver
     for _ in range(len(config.warnings)):
         msg = config.warnings.pop(0)
-        logger.warning(msg)
+        LOGGER.warning(msg)
+
+
+def _log_debug_information():
+    banner = f'\n{__banner__}\nThis is SourceSpec v{__version__}.\n'
+    LOGGER.info(banner)
+    LOGGER.debug('source_spec START')
+    LOGGER.debug(f'SourceSpec version: {__version__}')
+    uname = platform.uname()
+    uname_str = f'{uname[0]} {uname[2]} {uname[4]}'
+    LOGGER.debug(f'Platform: {uname_str}')
+    LOGGER.debug(f'Python version: {PYTHON_VERSION_STR}')
+    LOGGER.debug(f'ObsPy version: {OBSPY_VERSION_STR}')
+    LOGGER.debug(f'NumPy version: {NUMPY_VERSION_STR}')
+    LOGGER.debug(f'SciPy version: {SCIPY_VERSION_STR}')
+    LOGGER.debug(f'Matplotlib version: {MATPLOTLIB_VERSION_STR}')
+    if CARTOPY_VERSION_STR is not None:
+        LOGGER.debug(f'Cartopy version: {CARTOPY_VERSION_STR}')
+    LOGGER.debug('Running arguments:')
+    LOGGER.debug(' '.join(sys.argv))
 
 
 def ssp_exit(retval=0, abort=False):
+    """Exit the program."""
     # ssp_exit might have already been called if multiprocessing
-    global ssp_exit_called
-    if ssp_exit_called:
+    global SSP_EXIT_CALLED  # pylint: disable=global-statement
+    if SSP_EXIT_CALLED:
         return
-    ssp_exit_called = True
+    SSP_EXIT_CALLED = True
     if abort:
         print('\nAborting.')
-        if logger is not None:
-            logger.debug('source_spec ABORTED')
-    elif logger is not None:
-        logger.debug('source_spec END')
+        if LOGGER is not None:
+            LOGGER.debug('source_spec ABORTED')
+    elif LOGGER is not None:
+        LOGGER.debug('source_spec END')
     logging.shutdown()
     sys.exit(retval)
 
 
 def sigint_handler(sig, frame):
+    """Handle SIGINT signal."""
+    # pylint: disable=unused-argument
     ssp_exit(1, abort=True)
 
 
 signal.signal(signal.SIGINT, sigint_handler)
```

### Comparing `sourcespec-1.7/sourcespec/ssp_spectral_model.py` & `sourcespec-1.8/sourcespec/ssp_spectral_model.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 :copyright:
     2012 Claudio Satriano <satriano@ipgp.fr>
 
     2013-2014 Claudio Satriano <satriano@ipgp.fr>,
               Emanuela Matrullo <matrullo@geologie.ens.fr>,
               Agnes Chounet <chounet@ipgp.fr>
 
-    2015-2023 Claudio Satriano <satriano@ipgp.fr>
+    2015-2024 Claudio Satriano <satriano@ipgp.fr>
 :license:
     CeCILL Free Software License Agreement v2.1
     (http://www.cecill.info/licences.en.html)
 """
 import math
 import numpy as np
 
@@ -32,17 +32,19 @@
     see :ref:`Theoretical Background <theoretical_background>`
     for a detailed derivation of this model.
     """
     # log S(w)= log(coeff*Mo) + log((1/(1+(w/wc)^2)) + \
     #           log (exp (- w *t_star/2))
     # attenuation model: exp[-pi t* f] with t*=T /Q
     loge = math.log10(math.e)
-    return (Mw -
-            (2./3.)*np.log10(1. + np.power((freq/fc), 2)) -
-            (2./3.)*loge * (math.pi * np.power(freq, alpha) * t_star))
+    return (
+        Mw -
+        (2. / 3.) * np.log10(1. + np.power((freq / fc), 2)) -
+        (2. / 3.) * loge * (math.pi * np.power(freq, alpha) * t_star)
+    )
 
 
 def objective_func(xdata, ydata, weight):
     """Objective function generator for bounded inversion."""
     errsum = np.sum(weight)
 
     def _objective_func(params):
@@ -51,14 +53,13 @@
             model = spectral_model(xdata, params[0], params[1],
                                    params[2], params[3])
         else:
             model = spectral_model(xdata, params[0], params[1], params[2])
         res = np.array(ydata) - np.array(model)
         res2 = np.power(res, 2)
         wres = np.array(weight) * np.array(res2)
-        return np.sqrt(np.sum(wres)/errsum)
+        return np.sqrt(np.sum(wres) / errsum)
     return _objective_func
 
 
-def callback(x):
-    pass
-    # print 'parameters:', x
+def callback(_):
+    """Empty callback function for bounded inversion."""
```

### Comparing `sourcespec-1.7/sourcespec/ssp_summary_statistics.py` & `sourcespec-1.8/sourcespec/ssp_summary_statistics.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- coding: utf-8 -*-
 # SPDX-License-Identifier: CECILL-2.1
 """
 Post processing of station source parameters.
 
 :copyright:
-    2012-2023 Claudio Satriano <satriano@ipgp.fr>
+    2012-2024 Claudio Satriano <satriano@ipgp.fr>
 :license:
     CeCILL Free Software License Agreement v2.1
     (http://www.cecill.info/licences.en.html)
 """
 import logging
 import numpy as np
 from scipy.stats import norm
 from scipy.integrate import quad
 from sourcespec.ssp_setup import ssp_exit
 from sourcespec.ssp_data_types import (
     SummarySpectralParameter, SummaryStatistics)
-logger = logging.getLogger(__name__.split('.')[-1])
+logger = logging.getLogger(__name__.rsplit('.', maxsplit=1)[-1])
 
 
 def _avg_and_std(values, errors=None, logarithmic=False):
     """
     Return the average and standard deviation.
 
     Optionally:
@@ -39,208 +39,226 @@
         values = np.log10(values)
     notnan = ~np.isnan(values)
     if weights is not None:
         notnan = np.logical_and(notnan, ~np.isnan(weights))
         weights = weights[notnan]
     values = values[notnan]
     average = np.average(values, weights=weights)
-    variance = np.average((values-average)**2, weights=weights)
+    variance = np.average((values - average)**2, weights=weights)
     std = np.sqrt(variance)
     if not logarithmic:
         return average, np.array((std, std))
     log_average = 10.**average
-    minus = log_average - 10.**(average-std)
-    plus = 10.**(average+std) - log_average
+    minus = log_average - 10.**(average - std)
+    plus = 10.**(average + std) - log_average
     return log_average, np.array((minus, plus))
 
 
 def _weights(values, errors=None, logarithmic=False):
     """Compute weights for weighted statistics."""
     if errors is None:
         return None
     # negative errors should not happen
     errors[errors < 0] = 0
     values_minus = values - errors[:, 0]
     values_plus = values + errors[:, 1]
     if logarithmic:
         # compute the width of the error bar in log10 units
         # replace negative left values with 1/10 of the central value
-        values_minus[values_minus <= 0] = values[values_minus <= 0]/10
+        values_minus[values_minus <= 0] = values[values_minus <= 0] / 10
         values_log_minus = np.log10(values_minus)
         values_log_plus = np.log10(values_plus)
         errors_width = values_log_plus - values_log_minus
     else:
         # compute the width of the error bar in linear units
         errors_width = values_plus - values_minus
     # fix for infinite weight (zero error width)
     errors_width[errors_width == 0] =\
         np.nanmin(errors_width[errors_width > 0])
-    return 1./(errors_width**2.)
+    return 1. / (errors_width**2.)
 
 
 def _normal_confidence_level(n_sigma):
     """
     Compute the confidence level of a normal (Gaussian) distribution
     between -n_sigma and +n_sigma.
     """
     def gauss(x):
         return norm.pdf(x, 0, 1)
     confidence, _ = quad(gauss, -n_sigma, n_sigma)
-    return np.round(confidence*100, 2)
+    return np.round(confidence * 100, 2)
 
 
 def _percentiles(
         values, low_percentage=25, mid_percentage=50, up_percentage=75):
     """Compute lower, mid and upper percentiles."""
     if len(values) == 0:
         return np.nan, np.nan, np.nan
     low_percentile, mid_percentile, up_percentile =\
         np.nanpercentile(
             values, (low_percentage, mid_percentage, up_percentage))
     return low_percentile, mid_percentile, up_percentile
 
 
 def _param_summary_statistics(
-        config, sspec_output, id, name, format, units=None, logarithmic=False):
+        config, sspec_output, param_id, name, format_spec, units=None,
+        logarithmic=False):
     """Compute summary statistics for one spectral parameter."""
     nIQR = config.nIQR
     summary = SummarySpectralParameter(
-        id=id, name=name, format=format, units=units)
-    sspec_output.find_outliers(id, n=nIQR)
-    values = sspec_output.value_array(id, filter_outliers=True)
-    errors = sspec_output.error_array(id, filter_outliers=True)
+        param_id=param_id, name=name, format_spec=format_spec, units=units)
+    sspec_output.find_outliers(param_id, n=nIQR)
+    values = sspec_output.value_array(param_id, filter_outliers=True)
+    errors = sspec_output.error_array(param_id, filter_outliers=True)
     # put to NaN infinite values and values whose errors are infinite
     values[np.isinf(values)] = np.nan
     _cond_err = np.logical_or(np.isinf(errors[:, 0]), np.isinf(errors[:, 1]))
     values[_cond_err] = np.nan
     errors[_cond_err] = np.nan
     # only count non-NaN values
     nobs = len(values[~np.isnan(values)])
     # mean
     mean_value, mean_error = _avg_and_std(values, logarithmic=logarithmic)
     mean_error *= config.n_sigma
     conf_level = _normal_confidence_level(config.n_sigma)
     summary.mean = SummaryStatistics(
-        type='mean', value=mean_value,
+        stat_type='mean', value=mean_value,
         lower_uncertainty=mean_error[0],
         upper_uncertainty=mean_error[1],
         confidence_level=conf_level, nobs=nobs)
-    # weighted mean (only if errors are defined)
     if not np.all(np.isnan(errors)):
+        # weighted mean (only if errors are defined)
         wmean_value, wmean_error = _avg_and_std(
             values, errors, logarithmic=logarithmic)
-        wmean_error *= config.n_sigma
-        summary.weighted_mean = SummaryStatistics(
-            type='weighted_mean', value=wmean_value,
-            lower_uncertainty=wmean_error[0],
-            upper_uncertainty=wmean_error[1],
-            confidence_level=conf_level, nobs=nobs)
+    else:
+        # else use an unweighted mean
+        logger.info(
+            f'{param_id} values have no uncertainty: weighted mean cannot be '
+            'computed. Using unweighted mean instead.')
+        wmean_value, wmean_error = mean_value, mean_error
+    summary.weighted_mean = SummaryStatistics(
+        stat_type='weighted_mean', value=wmean_value,
+        lower_uncertainty=wmean_error[0],
+        upper_uncertainty=wmean_error[1],
+        confidence_level=conf_level, nobs=nobs)
     # percentiles
     low_pctl, mid_pctl, up_pctl = _percentiles(
         values, config.lower_percentage, config.mid_percentage,
         config.upper_percentage)
     conf_level = round(
         (config.upper_percentage - config.lower_percentage), 2)
     summary.percentiles = SummaryStatistics(
-        type='percentiles', value=mid_pctl,
-        lower_uncertainty=mid_pctl-low_pctl,
-        upper_uncertainty=up_pctl-mid_pctl,
+        stat_type='percentiles', value=mid_pctl,
+        lower_uncertainty=mid_pctl - low_pctl,
+        upper_uncertainty=up_pctl - mid_pctl,
         confidence_level=conf_level,
         lower_percentage=config.lower_percentage,
         mid_percentage=config.mid_percentage,
         upper_percentage=config.upper_percentage,
         nobs=nobs)
     return summary
 
 
 def compute_summary_statistics(config, sspec_output):
     """Compute summary statistics from station spectral parameters."""
+    logger.info('Computing summary statistics...')
     if len(sspec_output.station_parameters) == 0:
         logger.info('No source parameter calculated')
         ssp_exit()
 
     sspec_output.summary_spectral_parameters.reference_statistics =\
         config.reference_statistics
 
     # Mw
     sspec_output.summary_spectral_parameters.Mw =\
         _param_summary_statistics(
             config, sspec_output,
-            id='Mw', name='moment magnitude', format='{:.2f}',
+            param_id='Mw', name='moment magnitude', format_spec='{:.2f}',
             logarithmic=False
         )
 
     # Mo (N·m)
     sspec_output.summary_spectral_parameters.Mo =\
         _param_summary_statistics(
             config, sspec_output,
-            id='Mo', name='seismic moment', units='N·m', format='{:.3e}',
-            logarithmic=True
+            param_id='Mo', name='seismic moment', units='N·m',
+            format_spec='{:.3e}', logarithmic=True
         )
 
     # fc (Hz)
     sspec_output.summary_spectral_parameters.fc =\
         _param_summary_statistics(
             config, sspec_output,
-            id='fc', name='corner frequency', units='Hz', format='{:.3f}',
-            logarithmic=True
+            param_id='fc', name='corner frequency', units='Hz',
+            format_spec='{:.3f}', logarithmic=True
         )
 
     # t_star (s)
     sspec_output.summary_spectral_parameters.t_star =\
         _param_summary_statistics(
             config, sspec_output,
-            id='t_star', name='t-star', units='s', format='{:.3f}',
+            param_id='t_star', name='t-star', units='s', format_spec='{:.3f}',
             logarithmic=False
         )
 
     # radius (meters)
     sspec_output.summary_spectral_parameters.radius =\
         _param_summary_statistics(
             config, sspec_output,
-            id='radius', name='source radius', units='m', format='{:.3f}',
-            logarithmic=True
+            param_id='radius', name='source radius', units='m',
+            format_spec='{:.3f}', logarithmic=True
         )
 
-    # bsd, Brune stress drop (MPa)
-    sspec_output.summary_spectral_parameters.bsd =\
+    # static stress drop (MPa)
+    sspec_output.summary_spectral_parameters.ssd =\
         _param_summary_statistics(
             config, sspec_output,
-            id='bsd', name='Brune stress drop', units='MPa', format='{:.3e}',
+            param_id='ssd', name='static stress drop',
+            units='MPa', format_spec='{:.3e}',
             logarithmic=True
         )
 
     # Quality factor
     sspec_output.summary_spectral_parameters.Qo =\
         _param_summary_statistics(
             config, sspec_output,
-            id='Qo', name='quality factor', format='{:.1f}',
+            param_id='Qo', name='quality factor', format_spec='{:.1f}',
             logarithmic=False
         )
 
     # Er (N·m)
     sspec_output.summary_spectral_parameters.Er =\
         _param_summary_statistics(
             config, sspec_output,
-            id='Er', name='radiated energy', units='N·m', format='{:.3e}',
-            logarithmic=True
+            param_id='Er', name='radiated energy', units='N·m',
+            format_spec='{:.3e}', logarithmic=True
+        )
+
+    # Apparent stress (MPa)
+    sspec_output.summary_spectral_parameters.sigma_a =\
+        _param_summary_statistics(
+            config, sspec_output,
+            param_id='sigma_a', name='apparent stress', units='MPa',
+            format_spec='{:.3e}', logarithmic=True
         )
 
     # Ml
     if config.compute_local_magnitude:
         sspec_output.summary_spectral_parameters.Ml =\
             _param_summary_statistics(
                 config, sspec_output,
-                id='Ml', name='local magnitude', format='{:.2f}',
+                param_id='Ml', name='local magnitude', format_spec='{:.2f}',
                 logarithmic=False
             )
 
     params_name = ('Mw', 'fc', 't_star')
     means = sspec_output.mean_values()
     sourcepar_mean = {par: means[par] for par in params_name}
     logger.info(f'params_mean: {sourcepar_mean}')
     means_weight = sspec_output.weighted_mean_values()
     sourcepar_mean_weight = {par: means_weight[par] for par in params_name}
     logger.info(f'params_mean_weighted: {sourcepar_mean_weight}')
     percentiles = sspec_output.percentiles_values()
     sourcepar_percentiles = {par: percentiles[par] for par in params_name}
     logger.info(f'params_percentiles: {sourcepar_percentiles}')
+    logger.info('Computing summary statistics: done')
+    logger.info('---------------------------------------------------')
```

### Comparing `sourcespec-1.7/sourcespec/ssp_wave_arrival.py` & `sourcespec-1.8/sourcespec/ssp_wave_arrival.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,104 +1,108 @@
 # -*- coding: utf-8 -*-
 # SPDX-License-Identifier: CECILL-2.1
 """
 Arrival time calculation for sourcespec.
 
 :copyright:
-    2012-2023 Claudio Satriano <satriano@ipgp.fr>
+    2012-2024 Claudio Satriano <satriano@ipgp.fr>
 :license:
     CeCILL Free Software License Agreement v2.1
     (http://www.cecill.info/licences.en.html)
 """
 import os
 import contextlib
 from glob import glob
 import logging
 import warnings
 from math import asin, degrees
 from obspy.taup import TauPyModel
 model = TauPyModel(model='iasp91')
-logger = logging.getLogger(__name__.split('.')[-1])
+logger = logging.getLogger(__name__.rsplit('.', maxsplit=1)[-1])
 
 
-def _get_nll_grd(phase, station, type, NLL_time_dir):
+def _get_nll_grd(phase, station, grd_type, NLL_time_dir):
     # Lazy-import here, since nllgrid is not an installation requirement
+    # pylint: disable=import-outside-toplevel
     from nllgrid import NLLGrid
     for _station in station, 'DEFAULT':
-        key = f'{phase}_{_station}_{type}'
+        key = f'{phase}_{_station}_{grd_type}'
         with contextlib.suppress(KeyError):
             return _get_nll_grd.grds[key]
         with contextlib.suppress(IndexError):
-            grdfile = f'*.{phase}.{_station}.{type}.hdr'
+            grdfile = f'*.{phase}.{_station}.{grd_type}.hdr'
             grdfile = os.path.join(NLL_time_dir, grdfile)
             grdfile = glob(grdfile)[0]
             grd = NLLGrid(grdfile)
             # cache NLL grid
             _get_nll_grd.grds[key] = grd
             return grd
     raise RuntimeError
 # dictionary to cache NLL grids
-_get_nll_grd.grds = {}  #noqa
+_get_nll_grd.grds = {}  # noqa
 
 
 def _wave_arrival_nll(trace, phase, NLL_time_dir, focmec):
     """Travel time and takeoff angle using a NLL grid."""
     if NLL_time_dir is None:
         raise RuntimeError
     station = trace.stats.station
     travel_time = takeoff_angle = None
-    grdtypes = ['time']
+    grd_types = ['time']
     if focmec:
-        grdtypes.append('angle')
-    for type in grdtypes:
+        grd_types.append('angle')
+    for grd_type in grd_types:
         try:
-            grd = _get_nll_grd(phase, station, type, NLL_time_dir)
+            grd = _get_nll_grd(phase, station, grd_type, NLL_time_dir)
         except RuntimeError as e:
             logger.warning(
-                f'{trace.id}: Cannot find NLL {type} grid. '
+                f'{trace.id}: Cannot find NLL {grd_type} grid. '
                 'Falling back to another method')
             raise RuntimeError from e
         if grd.station == 'DEFAULT':
             sta_x, sta_y = grd.project(
                 trace.stats.coords.longitude, trace.stats.coords.latitude)
             grd.sta_x, grd.sta_y = sta_x, sta_y
-        hypo_x, hypo_y = grd.project(
-            trace.stats.hypo.longitude, trace.stats.hypo.latitude)
-        hypo_z = trace.stats.hypo.depth
-        if type == 'time':
+        lon = trace.stats.event.hypocenter.longitude
+        lat = trace.stats.event.hypocenter.latitude
+        hypo_x, hypo_y = grd.project(lon, lat)
+        hypo_z = trace.stats.event.hypocenter.depth.value_in_km
+        if grd_type == 'time':
             travel_time = grd.get_value(hypo_x, hypo_y, hypo_z)
-        elif type == 'angle':
-            azimuth, takeoff_angle, quality = grd.get_value(
+        elif grd_type == 'angle':
+            _azimuth, takeoff_angle, _quality = grd.get_value(
                 hypo_x, hypo_y, hypo_z)
     return travel_time, takeoff_angle
 
 
 def _wave_arrival_vel(trace, vel):
     """Travel time and takeoff angle using a constant velocity (in km/s)."""
     if vel is None:
         raise RuntimeError
     travel_time = trace.stats.hypo_dist / vel
-    takeoff_angle = degrees(asin(trace.stats.epi_dist/trace.stats.hypo_dist))
+    takeoff_angle = degrees(asin(trace.stats.epi_dist / trace.stats.hypo_dist))
     # takeoff angle is 180° upwards and 0° downwards
     takeoff_angle = 180. - takeoff_angle
     return travel_time, takeoff_angle
 
 
 def _wave_arrival_taup(trace, phase):
     """Travel time and takeoff angle using taup."""
     phase_list = [phase.lower(), phase]
-    kwargs = dict(
-        source_depth_in_km=trace.stats.hypo.depth,
-        distance_in_degree=trace.stats.gcarc,
-        phase_list=phase_list)
+    hypo_depth = trace.stats.event.hypocenter.depth.value_in_km
+    kwargs = {
+        'source_depth_in_km': hypo_depth,
+        'distance_in_degree': trace.stats.gcarc,
+        'phase_list': phase_list
+    }
     with warnings.catch_warnings(record=True) as warns:
         try:
             arrivals = model.get_travel_times(**kwargs)
         except Exception:
-            trace.stats.hypo.depth = 0.
+            trace.stats.event.hypocenter.depth = 0.
             kwargs['source_depth_in_km'] = 0.
             arrivals = model.get_travel_times(**kwargs)
         for w in warns:
             message = str(w.message)
             # Ignore a specific obspy.taup warning we do not care about
             if '#2280' in message:
                 continue
@@ -121,113 +125,109 @@
         method = 'NonLinLoc grid'
         return travel_time, takeoff_angle, method
     with contextlib.suppress(RuntimeError):
         travel_time, takeoff_angle =\
             _wave_arrival_vel(trace, vel[phase])
         method = f'constant V{phase.lower()}: {vel[phase]:.1f} km/s'
         return travel_time, takeoff_angle, method
-    try:
-        travel_time, takeoff_angle = _wave_arrival_taup(trace, phase)
-        method = 'global velocity model (iasp91)'
-        return travel_time, takeoff_angle, method
-    except RuntimeError:
-        raise
+    # if _wave_arrival_taup() fails, it will raise a RuntimeError
+    travel_time, takeoff_angle = _wave_arrival_taup(trace, phase)
+    method = 'global velocity model (iasp91)'
+    # make sure returned values are float
+    return float(travel_time), float(takeoff_angle), method
 
 
 def _validate_pick(pick, theo_pick_time, tolerance, trace_id):
     """Check if a pick is valid, i.e., close enough to theoretical one."""
     if theo_pick_time is None:
         return True
     delta_t = pick.time - theo_pick_time
     if abs(delta_t) > tolerance:  # seconds
         logger.warning(
             f'{trace_id}: measured {pick.phase} pick time - theoretical time '
-            f'= {delta_t:.1f} s')
+            f'= {delta_t:.1f} s, above tolerance of {tolerance:.1f} s')
         return False
     return True
 
 
 def _get_theo_pick_time(trace, travel_time):
-    if trace.stats.hypo.origin_time is None:
+    if trace.stats.event.hypocenter.origin_time is None:
         msg = (
             f'{trace.id}: hypocenter origin time not set: '
             'unable to compute theoretical pick time')
         if msg not in _get_theo_pick_time.msg_cache:
             _get_theo_pick_time.msg_cache.append(msg)
             logger.warning(msg)
         return None
-    return trace.stats.hypo.origin_time + travel_time
+    return trace.stats.event.hypocenter.origin_time + travel_time
 _get_theo_pick_time.msg_cache = [] # noqa
 
 
 def _travel_time_from_pick(trace, pick_time):
     try:
-        travel_time = pick_time - trace.stats.hypo.origin_time
+        travel_time = pick_time - trace.stats.event.hypocenter.origin_time
     except TypeError:
         travel_time = None
     return travel_time
 
 
 def _find_picks(trace, phase, theo_pick_time, tolerance):
     """Search for valid picks in trace stats. Return pick time if found."""
-    for pick in (p for p in trace.stats.picks if p.phase == phase):
+    for pick in (p for p in trace.stats.picks if p.phase.upper() == phase):
         if _validate_pick(pick, theo_pick_time, tolerance, trace.id):
             trace.stats.arrivals[phase] = (phase, pick.time)
             return pick.time
     return None
 
 
-def add_arrivals_to_trace(trace, config):
+def add_arrival_to_trace(trace, phase, config):
     """
-    Add P and S arrival times and takeoff angles to trace.
+    Add arrival time, travel time and takeoff angle to trace for the
+    given phase.
 
     Uses the theoretical arrival time if no pick is available
     or if the pick is too different from the theoretical arrival.
     """
-    tolerance = config.p_arrival_tolerance
-    for phase in 'P', 'S':
-        key = f'{trace.id}_{phase}'
-        # First, see if there are cached values
-        with contextlib.suppress(KeyError):
-            trace.stats.arrivals[phase] =\
-                add_arrivals_to_trace.pick_cache[key]
-            trace.stats.travel_times[phase] =\
-                add_arrivals_to_trace.travel_time_cache[key]
-            trace.stats.takeoff_angles[phase] =\
-                add_arrivals_to_trace.angle_cache[key]
-            continue
-        # If no cache is available, compute travel_time and takeoff_angle
-        try:
-            travel_time, takeoff_angle, method =\
-                _wave_arrival(trace, phase, config)
-            theo_pick_time = _get_theo_pick_time(trace, travel_time)
-            pick_time = _find_picks(trace, phase, theo_pick_time, tolerance)
-        except Exception as msg:
-            for line in str(msg).splitlines():
-                logger.warning(line)
-            continue
-        if pick_time is not None:
-            logger.info(f'{trace.id}: found {phase} pick')
-            travel_time = \
-                _travel_time_from_pick(trace, pick_time) or travel_time
-            pick_phase = phase
-        else:
-            logger.info(f'{trace.id}: no {phase} pick found')
-            if theo_pick_time is None:
-                continue
-            logger.info(
-                f'{trace.id}: using theoretical {phase} pick from {method}')
-            pick_time = theo_pick_time
-            pick_phase = f'{phase}theo'
-        if config.rp_from_focal_mechanism:
-            logger.info(
-                f'{trace.id}: {phase} takeoff angle: {takeoff_angle:.1f} '
-                f'computed from {method}')
-        add_arrivals_to_trace.pick_cache[key] =\
-            trace.stats.arrivals[phase] = (pick_phase, pick_time)
-        add_arrivals_to_trace.travel_time_cache[key] =\
-            trace.stats.travel_times[phase] = travel_time
-        add_arrivals_to_trace.angle_cache[key] =\
-            trace.stats.takeoff_angles[phase] = takeoff_angle
-add_arrivals_to_trace.pick_cache = {}  #noqa
-add_arrivals_to_trace.travel_time_cache = {}  #noqa
-add_arrivals_to_trace.angle_cache = {}  #noqa
+    tolerance = (
+        config.p_arrival_tolerance
+        if phase == 'P' else
+        config.s_arrival_tolerance
+    )
+    key = f'{trace.id}_{phase}'
+    trst = trace.stats
+    # First, see if there are cached values
+    with contextlib.suppress(KeyError):
+        trst.arrivals[phase] = add_arrival_to_trace.pick_cache[key]
+        trst.travel_times[phase] = add_arrival_to_trace.travel_time_cache[key]
+        trst.takeoff_angles[phase] = add_arrival_to_trace.angle_cache[key]
+        return
+    # If no cache is available, compute travel_time and takeoff_angle
+    travel_time, takeoff_angle, method = _wave_arrival(trace, phase, config)
+    theo_pick_time = _get_theo_pick_time(trace, travel_time)
+    pick_time = _find_picks(trace, phase, theo_pick_time, tolerance)
+    if pick_time is not None:
+        logger.info(f'{trace.id}: found {phase} pick')
+        travel_time = \
+            _travel_time_from_pick(trace, pick_time) or travel_time
+        pick_phase = phase
+    else:
+        logger.info(f'{trace.id}: no {phase} pick found')
+        if theo_pick_time is None:
+            raise ValueError(
+                f'{trace.id}: no theoretical {phase} pick time available')
+        logger.info(
+            f'{trace.id}: using theoretical {phase} pick from {method}')
+        pick_time = theo_pick_time
+        pick_phase = f'{phase}theo'
+    if config.rp_from_focal_mechanism:
+        logger.info(
+            f'{trace.id}: {phase} takeoff angle: {takeoff_angle:.1f} '
+            f'computed from {method}')
+    add_arrival_to_trace.pick_cache[key] =\
+        trst.arrivals[phase] = (pick_phase, pick_time)
+    add_arrival_to_trace.travel_time_cache[key] =\
+        trst.travel_times[phase] = travel_time
+    add_arrival_to_trace.angle_cache[key] =\
+        trst.takeoff_angles[phase] = takeoff_angle
+add_arrival_to_trace.pick_cache = {}  # noqa
+add_arrival_to_trace.travel_time_cache = {}  # noqa
+add_arrival_to_trace.angle_cache = {}  # noqa
```

### Comparing `sourcespec-1.7/sourcespec.egg-info/PKG-INFO` & `sourcespec-1.8/sourcespec.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sourcespec
-Version: 1.7
+Version: 1.8
 Summary: Earthquake source parameters from P- or S-wave displacement spectra
 Home-page: https://sourcespec.seismicsource.org
 Author: Claudio Satriano
 Author-email: satriano@ipgp.fr
 License: CeCILL Free Software License Agreement, Version 2.1
 Project-URL: Homepage, https://sourcespec.seismicsource.org
 Project-URL: Source, https://github.com/SeismicSource/sourcespec
@@ -13,44 +13,53 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: CEA CNRS Inria Logiciel Libre License, version 2.1 (CeCILL-2.1)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: numpy>=1.10
+Requires-Dist: scipy>=0.17
+Requires-Dist: matplotlib>=3.2
+Requires-Dist: pillow>=4.0.0
+Requires-Dist: obspy>=1.2.0
+Requires-Dist: pyproj
+Requires-Dist: tzlocal
+Requires-Dist: pyyaml>=5.1
+Requires-Dist: h5py
 
-<img src="https://cdn.jsdelivr.net/gh/SeismicSource/sourcespec@14da5bf21ed6aa82da902d06d019487604c47ea2/imgs/SourceSpec_logo.svg" width="600">
+<img src="https://cdn.jsdelivr.net/gh/SeismicSource/sourcespec@721d460561daa0f48f7d4addb409ef11c6e98865/imgs/SourceSpec_logo.svg" width="600">
 
 # SourceSpec
 
 Earthquake source parameters from P- or S-wave displacement spectra
 
+[![changelog-badge]][changelog-link]
 [![PyPI-badge]][PyPI-link]
 [![license-badge]][license-link]
 [![docs-badge]][docs-link]
 [![DOI-badge]][DOI-link]
 
-Copyright (c) 2011-2023 Claudio Satriano <satriano@ipgp.fr>
+Copyright (c) 2011-2024 Claudio Satriano <satriano@ipgp.fr>
 
 ## Description
 
 SourceSpec is a collection of command line tools to compute earthquake source
 parameters (seismic moment, corner frequency, radiated energy, source size,
-stress drop) from the inversion of P-wave and S-wave displacement spectra
-recorded at one or more seismic stations.
+static stress drop, apparent stress) from the inversion of P-wave and S-wave
+displacement spectra recorded at one or more seismic stations.
 SourceSpec also computes attenuation parameters (t-star, quality factor) and,
 as a bonus, local magnitude.
 
 See [Madariaga (2011)][Madariaga2011] for a primer on earthquake source
 parameters and scaling laws.
 
 Go to section [Theoretical background](#theoretical-background) below to get
@@ -72,27 +81,43 @@
 - `plot_sourcepars`: 1D or 2D plot of source parameters from a sqlite
   parameter file.
 
 ## Getting Started
 
 ### For the impatient
 
+> Note that the default config parameters are suited for a M<5 earthquake
+> recorded within ~100 km. Adjust `win_length`, `noise_pre_time`, the
+> frequency bands (`bp_freqmin_*`, `bp_freqmax_*`, `freq1_*`, `freq2_*`),
+> and the bounds on `fc` and `t_star`, according to your problem.
+
+#### Use case: miniSEED + StationXML + QuakeML
+
 If you have seismic recordings in [miniSEED] format (e.g., `traces.mseed`),
 metadata in [StationXML] format (e.g., `station.xml`) and event information in
 [QuakeML] format (e.g., `event.xml`), then:
 
 1. Generate a config file via `source_spec -S`;
 2. Edit the config file variable `station_metadata` to point to `station.xml`
    file;
 3. Run `source_spec -t traces.mseed -q event.xml`.
 
-> Note that the default config parameters are suited for a M<5 earthquake
-> recorded within ~100 km. Adjust `win_length`, `noise_pre_time`, and the
-> frequency bands (`bp_freqmin_*`, `bp_freqmax_*`, `freq1_*`, `freq2_*`)
-> according to your setup.
+#### Use case: SAC + PAZ + SourceSpec Event File
+
+If you have seismic recordings in [SAC] format (e.g., in a directory named
+`sac_data`), metadata as [SAC polezero (PAZ)] (e.g., in a directory named
+`paz`) and event information in any format, then:
+
+1. Generate a config file via `source_spec -S`;
+2. Edit the config file variable `station_metadata` to point to the `paz`
+   directory;
+3. Generate a sample [SourceSpec Event File] using `source_spec -y`; this
+   will create a file named `ssp_event.yaml`;
+4. Edit the file `ssp_event.yaml` with your event information;
+5. Run `source_spec -t sac_data -H ssp_event.yaml`.
 
 ### Command line arguments
 
 After successfully installed SourceSpec (see [Installation](#installation)
 below), you can get help on the command line arguments used by each code by
 typing from your terminal:
 
@@ -101,18 +126,19 @@
 (or `source_model -h`, or `source_residuals -h`).
 
 `source_spec` and `source_model` require you to provide the path to seismic
 traces via the `--trace_path` command line argument (see
 [File formats](#file-formats) below).
 
 Information on the seismic event can be stored in the trace header ([SAC]
-format), or provided through a [QuakeML] file (`--qmlfile`) or a [HYPO71] or
-[HYPOINVERSE-2000] file (`--hypocenter`). See
-[File formats](#file-formats) below for more information on the supported file
-formats.
+format), or provided through a [QuakeML] file (`--qmlfile`) or
+or, alternatively (`--hypocenter`), through a [SourceSpec Event File],
+a [HYPO71] file, or a [HYPOINVERSE-2000] file.
+See [File formats](#file-formats) below for more information on the supported
+file formats.
 
 ### Configuration file
 
 `source_spec` and `source_model` require a configuration file. The default file
 name is `source_spec.conf`, other file names can be specified via the
 `--configfile` command line argument.
 
@@ -135,37 +161,51 @@
 
 - [miniSEED]
 - [SAC]
 
 The SAC format can carry additional information in its header, like event
 location and origin time, phase picks, instrument sensitivity.
 
+Input trace files can be provided --through the `-t` option-- as a list of
+files, as a directory containing the files, or as a TAR(GZ) or ZIP archive
+containing the files.
+
 ### Event formats
 
 SourceSpec can read event information (event ID, location, origin time) in the
 following formats:
 
-- [QuakeML]: SourceSpec will also read phase picks and
-  focal mechanism, if available
+- [SourceSpec Event File]: this file can contain additional event information,
+  such as magnitude, moment tensor or focal mechanism
+- [QuakeML]: this file can contain additional event information, such as
+  magnitude, moment tensor or focal mechanism. If phase picks are available,
+  they will be read as well
 - [HYPO71]
-- [HYPOINVERSE-2000]: SourceSpec will also read phase picks, if available
+- [HYPOINVERSE-2000]: if phase picks are available, they will be read as well
 
-Event information can also be stored in the SAC file headers (header fields:
+Event information can also be stored in the [SAC file header] (header fields:
 `EVLA`, `EVLO`, `EVDP`, `O`, `KEVNM`).
 
 ### Phase pick formats
 
 Phase picks for P and S waves can be read from one of the following formats:
 
 - [QuakeML]
 - [HYPO71]
 - [HYPOINVERSE-2000]
 
-Phase picks can also be stored in the SAC file headers (header fields: `A` and
-`T0`).
+Phase picks can also be stored in the [SAC file header], using the header
+fields `A` and `T0` through `T9`. A pick label can be specified (header fields
+`KA` and `KT0` through `KT9`) to identify the pick; the pick label can be a
+standard 4-characters SAC label (e.g., `"IPU0"`, `" S 1"`) or a label starting
+with `"P"` or `"S"` (lowercase or uppercase, e.g., `"P"`, `"pP"`, `"Pg"`,
+`"S"`, `"Sn"`).
+Picks with labels that cannot be parsed by SourceSpec will be ignored.
+If no label is specified, then SourceSpec will assume that `A` is the P-pick
+and `T0` is the S-pick.
 
 ### Station metadata formats
 
 Station metadata (coordinates, instrumental response) can be provided in one of
 the following formats:
 
 - [StationXML]
@@ -191,16 +231,16 @@
 - `EVID.ssp.yaml`: [YAML] file containing the estimated spectral parameters
   (summary values and per station values)
 - `EVID.ssp.out` (*deprecated*): text file containing the estimated spectral
   parameters (summary values and per station values)
 - `EVID.ssp.log`: log file in text format (including the command line arguments,
   for [reproducibility])
 - `EVID.ssp.conf`: the input config file (for [reproducibility])
-- `EVID-residuals.pickle`: station residuals in
-  [Python pickle format][pickle]
+- `EVID.residuals.hdf5`: station residuals in [HDF5] format
+- `EVID.spectra.hdf5`: (optional) spectra in [HDF5] format
 - `EVID.ssp.h`: hypocenter file in [HYPO71] format with the estimated moment
   magnitude (only if an input HYPO71 file is provided)
 - `EVID.xml`: updated [QuakeML] file with the results of the SourceSpec
   inversion (only if an input QuakeML file is provided)
 
 The following plots will be created, in png, pdf or svg format:
 
@@ -262,57 +302,84 @@
 - LM: [Levenberg-Marquardt algorithm]
   (warning: [Trust Region Reflective algorithm] will be used instead if
    bounds are provided)
 - BH: [basin-hopping algorithm]
 - GS: [grid search]
 - IS: [importance sampling] of misfit grid, using [k-d tree]
 
-Starting from the inverted parameters $M_0$ ( $M_w$ ), $fc$, $t^*$ and following
-the equations in [Madariaga (2011)][Madariaga2011], other quantities are
-computed for each station:
-
-- the Brune stress drop
-- the source radius
+Starting from the inverted parameters $M_0$ ( $M_w$ ), $fc$, $t^*$ and
+following the equations in [Madariaga (2011)][Madariaga2011] and
+[Lancieri (2012)][Lancieri2012], other quantities are computed for each
+station:
+
+- the static stress drop $\Delta \sigma$
+- the source radius $a$
+- the radiated energy $E_r$
+- the apparent stress $\sigma_a$
 - the quality factor $Q_0$ of P- or S-waves
 
-Finally, the radiated energy $E_r$ can be measured from the displacement
-spectra, following the approach described in [Lancieri et al.
-(2012)][Lancieri2012].
-
 As a bonus, local magnitude $M_l$ can be computed as well.
 
 Event summaries (mean, weighted mean, percentiles) are computed from single
 station estimates. For mean and weighted mean estimation, outliers are rejected
 based on the [interquartile range] rule.
 
 See the official [documentation] for more details.
 
-![Example Trace](https://cdn.jsdelivr.net/gh/SeismicSource/sourcespec@14da5bf21ed6aa82da902d06d019487604c47ea2/imgs/example_trace.svg) **Example three-component trace plot
+![Example Trace](https://cdn.jsdelivr.net/gh/SeismicSource/sourcespec@721d460561daa0f48f7d4addb409ef11c6e98865/imgs/example_trace.svg) **Example three-component trace plot
 (in velocity), showing noise and S-wave windows**
 
-![Example Spectrum](https://cdn.jsdelivr.net/gh/SeismicSource/sourcespec@14da5bf21ed6aa82da902d06d019487604c47ea2/imgs/example_spectrum.svg)
+![Example Spectrum](https://cdn.jsdelivr.net/gh/SeismicSource/sourcespec@721d460561daa0f48f7d4addb409ef11c6e98865/imgs/example_spectrum.svg)
 **Example displacement spectrum for noise and S-wave, including inversion
 results**
 
 ## Installation
 
-SourceSpec requires at least Python 3.6. All the required dependencies will be
+SourceSpec requires at least Python 3.7. All the required dependencies will be
 downloaded and installed during the setup process.
 
 ### Installing the latest release
 
-#### Using pip and PyPI (preferred method)
+### Using Anaconda
+
+The following command will automatically create an [Anaconda] environment
+named `sourcespec`, install the required packages and install the latest
+version of SourceSpec via `pip`:
+
+    conda env create --file https://raw.githubusercontent.com/SeismicSource/sourcespec/main/sourcespec_conda_env.yml
+
+If you want a different name for your environment, use:
+
+    conda env create -n YOUR_ENV_NAME --file https://raw.githubusercontent.com/SeismicSource/sourcespec/main/sourcespec_conda_env.yml
+
+Activate the environment with:
+
+    conda activate sourcespec
+
+(or `conda activate YOUR_ENV_NAME`)
+
+To keep SourceSpec updated run:
+
+    pip install --upgrade sourcespec
+
+from within your environment.
+
+#### Using pip and PyPI
 
 The latest release of SourceSpec is available on the
 [Python Package Index](https://pypi.org/project/sourcespec/).
 
 You can install it easily through `pip`:
 
     pip install sourcespec
 
+To upgrade from a previously installed version:
+
+    pip install --upgrade sourcespec
+
 #### From SourceSpec GitHub releases
 
 Download the latest release from the
 [releases page](https://github.com/SeismicSource/sourcespec/releases),
 in `zip` or `tar.gz` format, then:
 
     pip install sourcespec-X.Y.zip
@@ -323,19 +390,19 @@
 
 Where, `X.Y` is the version number (e.g., `1.2`).
 You don't need to uncompress the release files yourself.
 
 ### Installing a developer snapshot
 
 If you need a recent feature that is not in the latest release (see the
-`unreleased` section in [CHANGELOG](https://cdn.jsdelivr.net/gh/SeismicSource/sourcespec@14da5bf21ed6aa82da902d06d019487604c47ea2/CHANGELOG.md)), you want to use the more
+`unreleased` section in [CHANGELOG](https://cdn.jsdelivr.net/gh/SeismicSource/sourcespec@721d460561daa0f48f7d4addb409ef11c6e98865/CHANGELOG.md)), you want to use the more
 recent development snapshot from the
 [SourceSpec GitHub repository](https://github.com/SeismicSource/sourcespec).
 
-#### Using pip (preferred method)
+#### Using pip
 
 The easiest way to install the most recent development snapshot is to download
 and install it through `pip`, using its builtin `git` client:
 
     pip install git+https://github.com/SeismicSource/sourcespec.git
 
 Run this command again, from times to times, to keep SourceSpec updated with
@@ -391,66 +458,78 @@
 [Issue][Issues].
 Don't hesitate sending me pull requests with new features and/or bugfixes!
 
 ## How to Cite
 
 If you used SourceSpec for a scientific paper, please cite it as:
 
-> Satriano, C. (2023). SourceSpec – Earthquake source parameters from
+> Satriano, C. (2024). SourceSpec – Earthquake source parameters from
 > P- or S-wave displacement spectra (X.Y).
 > [doi: 10.5281/ZENODO.3688587]
 
 Please replace `X.Y` with the SourceSpec version number you used.
 
 You can also cite the following abstract presented at the
 2016 AGU Fall Meeting:
 
 > Satriano, C., Mejia Uquiche, A. R., & Saurel, J. M. (2016). Spectral
 > estimation of seismic moment, corner frequency and radiated energy for
 > earthquakes in the Lesser Antilles. In AGU Fall Meeting Abstracts
 > (Vol. 2016, pp. S13A-2518), [bibcode: 2016AGUFM.S13A2518S]
 
-
 ## References
 
 - Brune, J. N. (1970). Tectonic stress and the spectra of seismic shear waves
   from earthquakes, J. Geophys. Res., 75 (26), 4997– 5009,
   [doi: 10.1029/JB075i026p04997]
 - Lancieri, M., Madariaga, R., Bonilla, F. (2012). Spectral scaling of the
   aftershocks of the Tocopilla 2007 earthquake in northern Chile, Geophys. J.
   Int., 189 (1), 469–480, [doi: 10.1111/j.1365-246X.2011.05327.x]
 - Madariaga, R. (2011). Earthquake Scaling Laws. In "Extreme Environmental
   Events", pp. 364–383, [doi: 10.1007/978-1-4419-7695-6_22]. Available on
   [ResearchGate][Madariaga2011].
 
+## Citing literature
+
+A, probably incomplete, list of papers that used SourceSpec can be found in
+the [Citing Literature][citing_literature] section of the documentation.
+If you have used SourceSpec in a publication and would like to have it listed,
+please let me know.
+
 <!-- Badges and project links -->
 [PyPI-badge]: http://img.shields.io/pypi/v/sourcespec.svg
 [PyPI-link]: https://pypi.python.org/pypi/sourcespec
 [license-badge]: https://img.shields.io/badge/license-CeCILL--2.1-green.svg
 [license-link]: http://www.cecill.info/licences.en.html
 [docs-badge]: https://readthedocs.org/projects/sourcespec/badge/?version=latest
 [docs-link]: https://sourcespec.readthedocs.io/en/latest/?badge=latest
+[changelog-badge]: https://img.shields.io/badge/Changelog-136CB6.svg
+[changelog-link]: https://github.com/SeismicSource/sourcespec/blob/main/CHANGELOG.md
 [DOI-badge]: https://zenodo.org/badge/DOI/10.5281/zenodo.3688587.svg
 [DOI-link]: https://doi.org/10.5281/zenodo.3688587
 [documentation]: https://sourcespec.readthedocs.io
 [Discussions]: https://github.com/SeismicSource/sourcespec/discussions
 [Issues]: https://github.com/SeismicSource/sourcespec/issues
+[Anaconda]: https://www.anaconda.com/products/individual
+[citing_literature]: https://sourcespec.readthedocs.io/en/latest/citing_literature.html
 
 <!-- File formats -->
 [obspy_trace_formats]: https://docs.obspy.org/packages/autogen/obspy.core.stream.read.html
 [miniSEED]: http://ds.iris.edu/ds/nodes/dmc/data/formats/miniseed/
 [SAC]: https://ds.iris.edu/ds/support/faq/17/sac-file-format/
+[SAC file header]: https://ds.iris.edu/files/sac-manual/manual/file_format.html
+[SourceSpec Event File]: https://sourcespec.readthedocs.io/en/latest/source_spec_event_file.html
 [QuakeML]: https://quake.ethz.ch/quakeml/
 [HYPO71]: https://pubs.er.usgs.gov/publication/ofr72224
 [HYPOINVERSE-2000]: https://pubs.er.usgs.gov/publication/ofr02171
 [StationXML]: http://docs.fdsn.org/projects/stationxml/en/latest/
 [Dataless SEED]: https://ds.iris.edu/ds/nodes/dmc/data/formats/dataless-seed/
 [SEED resp]: https://ds.iris.edu/ds/nodes/dmc/data/formats/resp/
 [SAC polezero (PAZ)]: https://www.jakewalter.net/sacresponse.html
-[pickle]: https://docs.python.org/3/library/pickle.html
+[HDF5]: https://en.wikipedia.org/wiki/Hierarchical_Data_Format
 [Cartopy]: https://scitools.org.uk/cartopy/docs/latest
 [SQLite]: https://www.sqlite.org
 [YAML]: https://yaml.org
 
 <!-- Methods -->
 [reproducibility]: https://en.wikipedia.org/wiki/Reproducibility
 [box_plot]: https://en.wikipedia.org/wiki/Box_plot
```

### Comparing `sourcespec-1.7/versioneer.py` & `sourcespec-1.8/versioneer.py`

 * *Files identical despite different names*

