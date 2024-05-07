# Comparing `tmp/vegafusion-1.6.7.tar.gz` & `tmp/vegafusion-1.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vegafusion-1.6.7.tar", last modified: Thu Apr 11 21:27:01 2024, max compression
+gzip compressed data, was "vegafusion-1.6.8.tar", last modified: Tue May  7 14:03:45 2024, max compression
```

## Comparing `vegafusion-1.6.7.tar` & `vegafusion-1.6.8.tar`

### file list

```diff
@@ -1,403 +1,403 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.118775 vegafusion-1.6.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-11 21:26:35.000000 vegafusion-1.6.7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-11 21:27:01.118775 vegafusion-1.6.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-11 21:26:35.000000 vegafusion-1.6.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.086775 vegafusion-1.6.7/proto/
--rw-r--r--   0 runner    (1001) docker     (127)    38178 2024-04-11 21:26:35.000000 vegafusion-1.6.7/proto/datafusion.proto
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-11 21:26:35.000000 vegafusion-1.6.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-11 21:26:35.000000 vegafusion-1.6.7/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-11 21:27:01.118775 vegafusion-1.6.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 21:26:35.000000 vegafusion-1.6.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.086775 vegafusion-1.6.7/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.082775 vegafusion-1.6.7/tests/altair_mocks/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.070775 vegafusion-1.6.7/tests/altair_mocks/area/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.086775 vegafusion-1.6.7/tests/altair_mocks/area/cumulative_count/
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/area/cumulative_count/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.090775 vegafusion-1.6.7/tests/altair_mocks/area/density_facet/
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/area/density_facet/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.090775 vegafusion-1.6.7/tests/altair_mocks/area/density_stack/
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/area/density_stack/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.090775 vegafusion-1.6.7/tests/altair_mocks/area/gradient/
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/area/gradient/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.090775 vegafusion-1.6.7/tests/altair_mocks/area/horizon_graph/
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/area/horizon_graph/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.090775 vegafusion-1.6.7/tests/altair_mocks/area/layered/
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/area/layered/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.090775 vegafusion-1.6.7/tests/altair_mocks/area/normalized_stacked/
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/area/normalized_stacked/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.090775 vegafusion-1.6.7/tests/altair_mocks/area/streamgraph/
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/area/streamgraph/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.090775 vegafusion-1.6.7/tests/altair_mocks/area/trellis/
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/area/trellis/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.090775 vegafusion-1.6.7/tests/altair_mocks/area/trellis_sort_array/
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/area/trellis_sort_array/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.070775 vegafusion-1.6.7/tests/altair_mocks/bar/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.090775 vegafusion-1.6.7/tests/altair_mocks/bar/and_tick_chart/
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/bar/and_tick_chart/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.090775 vegafusion-1.6.7/tests/altair_mocks/bar/diverging_stacked/
--rw-r--r--   0 runner    (1001) docker     (127)     8391 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/bar/diverging_stacked/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.090775 vegafusion-1.6.7/tests/altair_mocks/bar/grouped/
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/bar/grouped/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.090775 vegafusion-1.6.7/tests/altair_mocks/bar/horizontal/
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/bar/horizontal/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.090775 vegafusion-1.6.7/tests/altair_mocks/bar/horizontal_grouped/
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/bar/horizontal_grouped/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.090775 vegafusion-1.6.7/tests/altair_mocks/bar/horizontal_stacked/
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/bar/horizontal_stacked/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.090775 vegafusion-1.6.7/tests/altair_mocks/bar/layered/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/bar/layered/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.090775 vegafusion-1.6.7/tests/altair_mocks/bar/normalized_stacked/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/bar/normalized_stacked/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.090775 vegafusion-1.6.7/tests/altair_mocks/bar/percentage_of_total/
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/bar/percentage_of_total/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.090775 vegafusion-1.6.7/tests/altair_mocks/bar/sorted/
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/bar/sorted/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.090775 vegafusion-1.6.7/tests/altair_mocks/bar/stacked/
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/bar/stacked/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.090775 vegafusion-1.6.7/tests/altair_mocks/bar/stacked_with_sorted_segments/
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/bar/stacked_with_sorted_segments/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.090775 vegafusion-1.6.7/tests/altair_mocks/bar/stacked_with_text_overlay/
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/bar/stacked_with_text_overlay/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.090775 vegafusion-1.6.7/tests/altair_mocks/bar/trellis_compact/
--rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/bar/trellis_compact/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.090775 vegafusion-1.6.7/tests/altair_mocks/bar/trellis_stacked/
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/bar/trellis_stacked/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.090775 vegafusion-1.6.7/tests/altair_mocks/bar/with_error_bars/
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/bar/with_error_bars/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.090775 vegafusion-1.6.7/tests/altair_mocks/bar/with_highlighted_bar/
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/bar/with_highlighted_bar/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.090775 vegafusion-1.6.7/tests/altair_mocks/bar/with_labels/
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/bar/with_labels/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.090775 vegafusion-1.6.7/tests/altair_mocks/bar/with_line_at_mean/
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/bar/with_line_at_mean/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.090775 vegafusion-1.6.7/tests/altair_mocks/bar/with_line_on_dual_axis/
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/bar/with_line_on_dual_axis/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.094776 vegafusion-1.6.7/tests/altair_mocks/bar/with_negative_values/
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/bar/with_negative_values/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.094776 vegafusion-1.6.7/tests/altair_mocks/bar/with_rolling_mean/
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/bar/with_rolling_mean/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.094776 vegafusion-1.6.7/tests/altair_mocks/bar/with_rounded_edges/
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/bar/with_rounded_edges/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.074776 vegafusion-1.6.7/tests/altair_mocks/casestudy/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.094776 vegafusion-1.6.7/tests/altair_mocks/casestudy/airports/
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/casestudy/airports/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.094776 vegafusion-1.6.7/tests/altair_mocks/casestudy/anscombe_plot/
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/casestudy/anscombe_plot/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.094776 vegafusion-1.6.7/tests/altair_mocks/casestudy/beckers_barley_trellis_plot/
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/casestudy/beckers_barley_trellis_plot/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.094776 vegafusion-1.6.7/tests/altair_mocks/casestudy/co2_concentration/
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/casestudy/co2_concentration/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.094776 vegafusion-1.6.7/tests/altair_mocks/casestudy/falkensee/
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/casestudy/falkensee/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.094776 vegafusion-1.6.7/tests/altair_mocks/casestudy/gapminder_bubble_plot/
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/casestudy/gapminder_bubble_plot/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.094776 vegafusion-1.6.7/tests/altair_mocks/casestudy/iowa_electricity/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/casestudy/iowa_electricity/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.094776 vegafusion-1.6.7/tests/altair_mocks/casestudy/isotype/
--rw-r--r--   0 runner    (1001) docker     (127)     5881 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/casestudy/isotype/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.094776 vegafusion-1.6.7/tests/altair_mocks/casestudy/isotype_emoji/
--rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/casestudy/isotype_emoji/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.094776 vegafusion-1.6.7/tests/altair_mocks/casestudy/london_tube/
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/casestudy/london_tube/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.094776 vegafusion-1.6.7/tests/altair_mocks/casestudy/natural_disasters/
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/casestudy/natural_disasters/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.094776 vegafusion-1.6.7/tests/altair_mocks/casestudy/one_dot_per_zipcode/
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/casestudy/one_dot_per_zipcode/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.094776 vegafusion-1.6.7/tests/altair_mocks/casestudy/top_k_items/
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/casestudy/top_k_items/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.094776 vegafusion-1.6.7/tests/altair_mocks/casestudy/top_k_letters/
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/casestudy/top_k_letters/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.094776 vegafusion-1.6.7/tests/altair_mocks/casestudy/top_k_with_others/
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/casestudy/top_k_with_others/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.094776 vegafusion-1.6.7/tests/altair_mocks/casestudy/us_employment/
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/casestudy/us_employment/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.094776 vegafusion-1.6.7/tests/altair_mocks/casestudy/us_population_over_time_facet/
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/casestudy/us_population_over_time_facet/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.094776 vegafusion-1.6.7/tests/altair_mocks/casestudy/us_state_capitals/
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/casestudy/us_state_capitals/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.094776 vegafusion-1.6.7/tests/altair_mocks/casestudy/wheat_wages/
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/casestudy/wheat_wages/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.094776 vegafusion-1.6.7/tests/altair_mocks/casestudy/window_rank/
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/casestudy/window_rank/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.074776 vegafusion-1.6.7/tests/altair_mocks/circular/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.094776 vegafusion-1.6.7/tests/altair_mocks/circular/donut/
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/circular/donut/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.094776 vegafusion-1.6.7/tests/altair_mocks/circular/pacman/
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/circular/pacman/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.094776 vegafusion-1.6.7/tests/altair_mocks/circular/pie/
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/circular/pie/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.094776 vegafusion-1.6.7/tests/altair_mocks/circular/pie_with_labels/
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/circular/pie_with_labels/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.094776 vegafusion-1.6.7/tests/altair_mocks/circular/radial/
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/circular/radial/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.074776 vegafusion-1.6.7/tests/altair_mocks/histogram/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.094776 vegafusion-1.6.7/tests/altair_mocks/histogram/layered/
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/histogram/layered/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.098775 vegafusion-1.6.7/tests/altair_mocks/histogram/trellis/
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/histogram/trellis/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.098775 vegafusion-1.6.7/tests/altair_mocks/histogram/with_a_global_mean_overlay/
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/histogram/with_a_global_mean_overlay/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.078776 vegafusion-1.6.7/tests/altair_mocks/interactive/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.098775 vegafusion-1.6.7/tests/altair_mocks/interactive/area-interval_selection/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/interactive/area-interval_selection/actions.json
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/interactive/area-interval_selection/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.098775 vegafusion-1.6.7/tests/altair_mocks/interactive/brush/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/interactive/brush/actions.json
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/interactive/brush/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.098775 vegafusion-1.6.7/tests/altair_mocks/interactive/casestudy-airport_connections/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/interactive/casestudy-airport_connections/actions.json
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/interactive/casestudy-airport_connections/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.098775 vegafusion-1.6.7/tests/altair_mocks/interactive/casestudy-seattle_weather_interactive/
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/interactive/casestudy-seattle_weather_interactive/actions.json
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/interactive/casestudy-seattle_weather_interactive/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.098775 vegafusion-1.6.7/tests/altair_mocks/interactive/casestudy-us_population_over_time/
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/interactive/casestudy-us_population_over_time/actions.json
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/interactive/casestudy-us_population_over_time/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.098775 vegafusion-1.6.7/tests/altair_mocks/interactive/casestudy-us_population_pyramid_over_time/
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/interactive/casestudy-us_population_pyramid_over_time/actions.json
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/interactive/casestudy-us_population_pyramid_over_time/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.098775 vegafusion-1.6.7/tests/altair_mocks/interactive/casestudy-weather_heatmap/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/interactive/casestudy-weather_heatmap/actions.json
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/interactive/casestudy-weather_heatmap/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.098775 vegafusion-1.6.7/tests/altair_mocks/interactive/cross_highlight/
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/interactive/cross_highlight/actions.json
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/interactive/cross_highlight/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.098775 vegafusion-1.6.7/tests/altair_mocks/interactive/histogram-responsive/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/interactive/histogram-responsive/actions.json
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/interactive/histogram-responsive/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.098775 vegafusion-1.6.7/tests/altair_mocks/interactive/layered_crossfilter/
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/interactive/layered_crossfilter/actions.json
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/interactive/layered_crossfilter/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.098775 vegafusion-1.6.7/tests/altair_mocks/interactive/legend/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/interactive/legend/actions.json
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/interactive/legend/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.098775 vegafusion-1.6.7/tests/altair_mocks/interactive/multiline_highlight/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/interactive/multiline_highlight/actions.json
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/interactive/multiline_highlight/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.098775 vegafusion-1.6.7/tests/altair_mocks/interactive/multiline_tooltip/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/interactive/multiline_tooltip/actions.json
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/interactive/multiline_tooltip/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.098775 vegafusion-1.6.7/tests/altair_mocks/interactive/other-image_tooltip/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/interactive/other-image_tooltip/actions.json
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/interactive/other-image_tooltip/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.102775 vegafusion-1.6.7/tests/altair_mocks/interactive/scatter-href/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/interactive/scatter-href/actions.json
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/interactive/scatter-href/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.102775 vegafusion-1.6.7/tests/altair_mocks/interactive/scatter-with_linked_table/
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/interactive/scatter-with_linked_table/actions.json
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/interactive/scatter-with_linked_table/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.102775 vegafusion-1.6.7/tests/altair_mocks/interactive/scatter-with_minimap/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/interactive/scatter-with_minimap/actions.json
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/interactive/scatter-with_minimap/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.102775 vegafusion-1.6.7/tests/altair_mocks/interactive/scatter_linked_brush/
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/interactive/scatter_linked_brush/actions.json
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/interactive/scatter_linked_brush/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.102775 vegafusion-1.6.7/tests/altair_mocks/interactive/scatter_plot/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/interactive/scatter_plot/actions.json
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/interactive/scatter_plot/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.102775 vegafusion-1.6.7/tests/altair_mocks/interactive/scatter_with_histogram/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/interactive/scatter_with_histogram/actions.json
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/interactive/scatter_with_histogram/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.102775 vegafusion-1.6.7/tests/altair_mocks/interactive/scatter_with_layered_histogram/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/interactive/scatter_with_layered_histogram/actions.json
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/interactive/scatter_with_layered_histogram/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.102775 vegafusion-1.6.7/tests/altair_mocks/interactive/select_detail/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/interactive/select_detail/actions.json
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/interactive/select_detail/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.102775 vegafusion-1.6.7/tests/altair_mocks/interactive/select_mark_area/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/interactive/select_mark_area/actions.json
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/interactive/select_mark_area/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.102775 vegafusion-1.6.7/tests/altair_mocks/interactive/selection_histogram/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/interactive/selection_histogram/actions.json
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/interactive/selection_histogram/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.102775 vegafusion-1.6.7/tests/altair_mocks/interactive/selection_layer_bar_month/
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/interactive/selection_layer_bar_month/actions.json
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/interactive/selection_layer_bar_month/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.078776 vegafusion-1.6.7/tests/altair_mocks/line/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.102775 vegafusion-1.6.7/tests/altair_mocks/line/bump_chart/
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/line/bump_chart/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.102775 vegafusion-1.6.7/tests/altair_mocks/line/filled_step_chart/
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/line/filled_step_chart/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.102775 vegafusion-1.6.7/tests/altair_mocks/line/layer_line_color_rule/
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/line/layer_line_color_rule/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.102775 vegafusion-1.6.7/tests/altair_mocks/line/multi_series/
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/line/multi_series/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.102775 vegafusion-1.6.7/tests/altair_mocks/line/percent_axis/
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/line/percent_axis/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.102775 vegafusion-1.6.7/tests/altair_mocks/line/slope_graph/
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/line/slope_graph/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.102775 vegafusion-1.6.7/tests/altair_mocks/line/slope_graph2/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/line/slope_graph2/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.106775 vegafusion-1.6.7/tests/altair_mocks/line/step_chart/
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/line/step_chart/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.106775 vegafusion-1.6.7/tests/altair_mocks/line/trail_marker/
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/line/trail_marker/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.106775 vegafusion-1.6.7/tests/altair_mocks/line/with_ci/
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/line/with_ci/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.106775 vegafusion-1.6.7/tests/altair_mocks/line/with_color_datum/
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/line/with_color_datum/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.106775 vegafusion-1.6.7/tests/altair_mocks/line/with_cumsum/
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/line/with_cumsum/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.106775 vegafusion-1.6.7/tests/altair_mocks/line/with_datum/
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/line/with_datum/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.106775 vegafusion-1.6.7/tests/altair_mocks/line/with_generator/
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/line/with_generator/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.106775 vegafusion-1.6.7/tests/altair_mocks/line/with_logarithmic_scale/
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/line/with_logarithmic_scale/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.106775 vegafusion-1.6.7/tests/altair_mocks/line/with_points/
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/line/with_points/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.078776 vegafusion-1.6.7/tests/altair_mocks/maps/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.106775 vegafusion-1.6.7/tests/altair_mocks/maps/airports_count/
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/maps/airports_count/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.106775 vegafusion-1.6.7/tests/altair_mocks/maps/choropleth/
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/maps/choropleth/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.106775 vegafusion-1.6.7/tests/altair_mocks/maps/choropleth_repeat/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/maps/choropleth_repeat/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.106775 vegafusion-1.6.7/tests/altair_mocks/maps/us_incomebrackets_by_state_facet/
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/maps/us_incomebrackets_by_state_facet/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.106775 vegafusion-1.6.7/tests/altair_mocks/maps/world/
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/maps/world/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.106775 vegafusion-1.6.7/tests/altair_mocks/maps/world_projections/
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/maps/world_projections/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.082775 vegafusion-1.6.7/tests/altair_mocks/other/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.106775 vegafusion-1.6.7/tests/altair_mocks/other/bar_chart_with_highlighted_segment/
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/other/bar_chart_with_highlighted_segment/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.106775 vegafusion-1.6.7/tests/altair_mocks/other/beckers_barley_wrapped_facet/
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/other/beckers_barley_wrapped_facet/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.106775 vegafusion-1.6.7/tests/altair_mocks/other/binned_heatmap/
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/other/binned_heatmap/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.106775 vegafusion-1.6.7/tests/altair_mocks/other/boxplot/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/other/boxplot/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.106775 vegafusion-1.6.7/tests/altair_mocks/other/candlestick_chart/
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/other/candlestick_chart/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.106775 vegafusion-1.6.7/tests/altair_mocks/other/comet_chart/
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/other/comet_chart/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.106775 vegafusion-1.6.7/tests/altair_mocks/other/errorbars_with_ci/
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/other/errorbars_with_ci/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.106775 vegafusion-1.6.7/tests/altair_mocks/other/errorbars_with_std/
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/other/errorbars_with_std/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.106775 vegafusion-1.6.7/tests/altair_mocks/other/gantt_chart/
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/other/gantt_chart/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.106775 vegafusion-1.6.7/tests/altair_mocks/other/hexbins/
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/other/hexbins/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.106775 vegafusion-1.6.7/tests/altair_mocks/other/isotype_grid/
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/other/isotype_grid/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.106775 vegafusion-1.6.7/tests/altair_mocks/other/layered_chart_with_dual_axis/
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/other/layered_chart_with_dual_axis/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.106775 vegafusion-1.6.7/tests/altair_mocks/other/layered_heatmap_text/
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/other/layered_heatmap_text/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.106775 vegafusion-1.6.7/tests/altair_mocks/other/multiple_marks/
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/other/multiple_marks/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.106775 vegafusion-1.6.7/tests/altair_mocks/other/normed_parallel_coordinates/
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/other/normed_parallel_coordinates/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.110775 vegafusion-1.6.7/tests/altair_mocks/other/parallel_coordinates/
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/other/parallel_coordinates/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.110775 vegafusion-1.6.7/tests/altair_mocks/other/ranged_dot_plot/
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/other/ranged_dot_plot/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.110775 vegafusion-1.6.7/tests/altair_mocks/other/ridgeline_plot/
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/other/ridgeline_plot/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.110775 vegafusion-1.6.7/tests/altair_mocks/other/scatter_marginal_hist/
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/other/scatter_marginal_hist/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.110775 vegafusion-1.6.7/tests/altair_mocks/other/sorted_error_bars_with_ci/
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/other/sorted_error_bars_with_ci/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.110775 vegafusion-1.6.7/tests/altair_mocks/other/stem_and_leaf/
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/other/stem_and_leaf/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.110775 vegafusion-1.6.7/tests/altair_mocks/other/violin_plot/
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/other/violin_plot/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.110775 vegafusion-1.6.7/tests/altair_mocks/other/wilkinson_dot_plot/
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/other/wilkinson_dot_plot/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.082775 vegafusion-1.6.7/tests/altair_mocks/scatter/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.110775 vegafusion-1.6.7/tests/altair_mocks/scatter/binned/
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/scatter/binned/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.110775 vegafusion-1.6.7/tests/altair_mocks/scatter/bubble_plot/
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/scatter/bubble_plot/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.110775 vegafusion-1.6.7/tests/altair_mocks/scatter/connected/
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/scatter/connected/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.110775 vegafusion-1.6.7/tests/altair_mocks/scatter/dot_dash_plot/
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/scatter/dot_dash_plot/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.110775 vegafusion-1.6.7/tests/altair_mocks/scatter/matrix/
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/scatter/matrix/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.110775 vegafusion-1.6.7/tests/altair_mocks/scatter/multifeature/
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/scatter/multifeature/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.110775 vegafusion-1.6.7/tests/altair_mocks/scatter/poly_fit_regression/
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/scatter/poly_fit_regression/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.110775 vegafusion-1.6.7/tests/altair_mocks/scatter/qq/
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/scatter/qq/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.110775 vegafusion-1.6.7/tests/altair_mocks/scatter/stripplot/
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/scatter/stripplot/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.110775 vegafusion-1.6.7/tests/altair_mocks/scatter/table_bubble_plot_github/
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/scatter/table_bubble_plot_github/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.110775 vegafusion-1.6.7/tests/altair_mocks/scatter/trellis/
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/scatter/trellis/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.110775 vegafusion-1.6.7/tests/altair_mocks/scatter/wind_vector_map/
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/scatter/wind_vector_map/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.110775 vegafusion-1.6.7/tests/altair_mocks/scatter/with_errorbars/
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/scatter/with_errorbars/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.110775 vegafusion-1.6.7/tests/altair_mocks/scatter/with_labels/
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/scatter/with_labels/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.110775 vegafusion-1.6.7/tests/altair_mocks/scatter/with_lowess/
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/scatter/with_lowess/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.110775 vegafusion-1.6.7/tests/altair_mocks/scatter/with_rolling_mean/
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/scatter/with_rolling_mean/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.086775 vegafusion-1.6.7/tests/altair_mocks/simple/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.110775 vegafusion-1.6.7/tests/altair_mocks/simple/bar_chart/
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/simple/bar_chart/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.110775 vegafusion-1.6.7/tests/altair_mocks/simple/heatmap/
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/simple/heatmap/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.110775 vegafusion-1.6.7/tests/altair_mocks/simple/line_chart/
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/simple/line_chart/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.110775 vegafusion-1.6.7/tests/altair_mocks/simple/scatter_tooltips/
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/simple/scatter_tooltips/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.114776 vegafusion-1.6.7/tests/altair_mocks/simple/stacked_bar_chart/
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/simple/stacked_bar_chart/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.114776 vegafusion-1.6.7/tests/altair_mocks/simple/strip_chart/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/altair_mocks/simple/strip_chart/mock.py
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/test_conext_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/test_datasource.py
--rw-r--r--   0 runner    (1001) docker     (127)    16868 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/test_input_utc.py
--rw-r--r--   0 runner    (1001) docker     (127)    50706 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/test_pretransform.py
--rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/test_pretransform_specs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/test_row_limit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/test_save.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/test_sql_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    14052 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/test_transformed_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-04-11 21:26:35.000000 vegafusion-1.6.7/tests/test_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.114776 vegafusion-1.6.7/vegafusion/
--rw-r--r--   0 runner    (1001) docker     (127)     3930 2024-04-11 21:26:35.000000 vegafusion-1.6.7/vegafusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-11 21:26:35.000000 vegafusion-1.6.7/vegafusion/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-11 21:26:35.000000 vegafusion-1.6.7/vegafusion/compilers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.114776 vegafusion-1.6.7/vegafusion/connection/
--rw-r--r--   0 runner    (1001) docker     (127)     5518 2024-04-11 21:26:35.000000 vegafusion-1.6.7/vegafusion/connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13181 2024-04-11 21:26:35.000000 vegafusion-1.6.7/vegafusion/connection/duckdb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.114776 vegafusion-1.6.7/vegafusion/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-11 21:26:35.000000 vegafusion-1.6.7/vegafusion/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6071 2024-04-11 21:26:35.000000 vegafusion-1.6.7/vegafusion/dataset/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)     5326 2024-04-11 21:26:35.000000 vegafusion-1.6.7/vegafusion/dataset/dfi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-11 21:26:35.000000 vegafusion-1.6.7/vegafusion/dataset/duckdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-04-11 21:26:35.000000 vegafusion-1.6.7/vegafusion/dataset/snowpark.py
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-04-11 21:26:35.000000 vegafusion-1.6.7/vegafusion/dataset/sql.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.118775 vegafusion-1.6.7/vegafusion/datasource/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-11 21:26:35.000000 vegafusion-1.6.7/vegafusion/datasource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17414 2024-04-11 21:26:35.000000 vegafusion-1.6.7/vegafusion/datasource/_dfi_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-11 21:26:35.000000 vegafusion-1.6.7/vegafusion/datasource/datasource.py
--rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-04-11 21:26:35.000000 vegafusion-1.6.7/vegafusion/datasource/dfi_datasource.py
--rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-04-11 21:26:35.000000 vegafusion-1.6.7/vegafusion/datasource/pandas_datasource.py
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-11 21:26:35.000000 vegafusion-1.6.7/vegafusion/datasource/pyarrow_datasource.py
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-11 21:26:35.000000 vegafusion-1.6.7/vegafusion/embed.py
--rw-r--r--   0 runner    (1001) docker     (127)     7992 2024-04-11 21:26:35.000000 vegafusion-1.6.7/vegafusion/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-11 21:26:35.000000 vegafusion-1.6.7/vegafusion/jupyter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-11 21:26:35.000000 vegafusion-1.6.7/vegafusion/local_tz.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.118775 vegafusion-1.6.7/vegafusion/proto/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 21:26:35.000000 vegafusion-1.6.7/vegafusion/proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    85200 2024-04-11 21:26:35.000000 vegafusion-1.6.7/vegafusion/proto/datafusion_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-04-11 21:26:35.000000 vegafusion-1.6.7/vegafusion/renderer.py
--rw-r--r--   0 runner    (1001) docker     (127)    33884 2024-04-11 21:26:35.000000 vegafusion-1.6.7/vegafusion/runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)     4267 2024-04-11 21:26:35.000000 vegafusion-1.6.7/vegafusion/save.py
--rw-r--r--   0 runner    (1001) docker     (127)     8401 2024-04-11 21:26:35.000000 vegafusion-1.6.7/vegafusion/transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-11 21:26:35.000000 vegafusion-1.6.7/vegafusion/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:27:01.118775 vegafusion-1.6.7/vegafusion.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-11 21:27:00.000000 vegafusion-1.6.7/vegafusion.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10742 2024-04-11 21:27:01.000000 vegafusion-1.6.7/vegafusion.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 21:27:00.000000 vegafusion-1.6.7/vegafusion.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-11 21:27:00.000000 vegafusion-1.6.7/vegafusion.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-11 21:27:00.000000 vegafusion-1.6.7/vegafusion.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.500220 vegafusion-1.6.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-07 14:03:06.000000 vegafusion-1.6.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-07 14:03:45.500220 vegafusion-1.6.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-07 14:03:06.000000 vegafusion-1.6.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.472220 vegafusion-1.6.8/proto/
+-rw-r--r--   0 runner    (1001) docker     (127)    38178 2024-05-07 14:03:06.000000 vegafusion-1.6.8/proto/datafusion.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-07 14:03:06.000000 vegafusion-1.6.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-07 14:03:06.000000 vegafusion-1.6.8/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-07 14:03:45.500220 vegafusion-1.6.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 14:03:06.000000 vegafusion-1.6.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.472220 vegafusion-1.6.8/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.468220 vegafusion-1.6.8/tests/altair_mocks/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.456219 vegafusion-1.6.8/tests/altair_mocks/area/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.472220 vegafusion-1.6.8/tests/altair_mocks/area/cumulative_count/
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/area/cumulative_count/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.472220 vegafusion-1.6.8/tests/altair_mocks/area/density_facet/
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/area/density_facet/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.472220 vegafusion-1.6.8/tests/altair_mocks/area/density_stack/
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/area/density_stack/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.472220 vegafusion-1.6.8/tests/altair_mocks/area/gradient/
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/area/gradient/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.472220 vegafusion-1.6.8/tests/altair_mocks/area/horizon_graph/
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/area/horizon_graph/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.472220 vegafusion-1.6.8/tests/altair_mocks/area/layered/
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/area/layered/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.472220 vegafusion-1.6.8/tests/altair_mocks/area/normalized_stacked/
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/area/normalized_stacked/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.472220 vegafusion-1.6.8/tests/altair_mocks/area/streamgraph/
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/area/streamgraph/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.472220 vegafusion-1.6.8/tests/altair_mocks/area/trellis/
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/area/trellis/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.472220 vegafusion-1.6.8/tests/altair_mocks/area/trellis_sort_array/
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/area/trellis_sort_array/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.456219 vegafusion-1.6.8/tests/altair_mocks/bar/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.472220 vegafusion-1.6.8/tests/altair_mocks/bar/and_tick_chart/
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/bar/and_tick_chart/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.476220 vegafusion-1.6.8/tests/altair_mocks/bar/diverging_stacked/
+-rw-r--r--   0 runner    (1001) docker     (127)     8391 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/bar/diverging_stacked/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.476220 vegafusion-1.6.8/tests/altair_mocks/bar/grouped/
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/bar/grouped/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.476220 vegafusion-1.6.8/tests/altair_mocks/bar/horizontal/
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/bar/horizontal/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.476220 vegafusion-1.6.8/tests/altair_mocks/bar/horizontal_grouped/
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/bar/horizontal_grouped/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.476220 vegafusion-1.6.8/tests/altair_mocks/bar/horizontal_stacked/
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/bar/horizontal_stacked/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.476220 vegafusion-1.6.8/tests/altair_mocks/bar/layered/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/bar/layered/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.476220 vegafusion-1.6.8/tests/altair_mocks/bar/normalized_stacked/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/bar/normalized_stacked/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.476220 vegafusion-1.6.8/tests/altair_mocks/bar/percentage_of_total/
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/bar/percentage_of_total/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.476220 vegafusion-1.6.8/tests/altair_mocks/bar/sorted/
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/bar/sorted/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.476220 vegafusion-1.6.8/tests/altair_mocks/bar/stacked/
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/bar/stacked/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.476220 vegafusion-1.6.8/tests/altair_mocks/bar/stacked_with_sorted_segments/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/bar/stacked_with_sorted_segments/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.476220 vegafusion-1.6.8/tests/altair_mocks/bar/stacked_with_text_overlay/
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/bar/stacked_with_text_overlay/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.476220 vegafusion-1.6.8/tests/altair_mocks/bar/trellis_compact/
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/bar/trellis_compact/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.476220 vegafusion-1.6.8/tests/altair_mocks/bar/trellis_stacked/
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/bar/trellis_stacked/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.476220 vegafusion-1.6.8/tests/altair_mocks/bar/with_error_bars/
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/bar/with_error_bars/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.476220 vegafusion-1.6.8/tests/altair_mocks/bar/with_highlighted_bar/
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/bar/with_highlighted_bar/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.476220 vegafusion-1.6.8/tests/altair_mocks/bar/with_labels/
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/bar/with_labels/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.476220 vegafusion-1.6.8/tests/altair_mocks/bar/with_line_at_mean/
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/bar/with_line_at_mean/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.476220 vegafusion-1.6.8/tests/altair_mocks/bar/with_line_on_dual_axis/
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/bar/with_line_on_dual_axis/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.476220 vegafusion-1.6.8/tests/altair_mocks/bar/with_negative_values/
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/bar/with_negative_values/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.476220 vegafusion-1.6.8/tests/altair_mocks/bar/with_rolling_mean/
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/bar/with_rolling_mean/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.476220 vegafusion-1.6.8/tests/altair_mocks/bar/with_rounded_edges/
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/bar/with_rounded_edges/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.460219 vegafusion-1.6.8/tests/altair_mocks/casestudy/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.476220 vegafusion-1.6.8/tests/altair_mocks/casestudy/airports/
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/casestudy/airports/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.476220 vegafusion-1.6.8/tests/altair_mocks/casestudy/anscombe_plot/
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/casestudy/anscombe_plot/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.476220 vegafusion-1.6.8/tests/altair_mocks/casestudy/beckers_barley_trellis_plot/
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/casestudy/beckers_barley_trellis_plot/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.476220 vegafusion-1.6.8/tests/altair_mocks/casestudy/co2_concentration/
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/casestudy/co2_concentration/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.476220 vegafusion-1.6.8/tests/altair_mocks/casestudy/falkensee/
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/casestudy/falkensee/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.476220 vegafusion-1.6.8/tests/altair_mocks/casestudy/gapminder_bubble_plot/
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/casestudy/gapminder_bubble_plot/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.476220 vegafusion-1.6.8/tests/altair_mocks/casestudy/iowa_electricity/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/casestudy/iowa_electricity/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.476220 vegafusion-1.6.8/tests/altair_mocks/casestudy/isotype/
+-rw-r--r--   0 runner    (1001) docker     (127)     5881 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/casestudy/isotype/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.476220 vegafusion-1.6.8/tests/altair_mocks/casestudy/isotype_emoji/
+-rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/casestudy/isotype_emoji/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.480220 vegafusion-1.6.8/tests/altair_mocks/casestudy/london_tube/
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/casestudy/london_tube/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.480220 vegafusion-1.6.8/tests/altair_mocks/casestudy/natural_disasters/
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/casestudy/natural_disasters/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.480220 vegafusion-1.6.8/tests/altair_mocks/casestudy/one_dot_per_zipcode/
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/casestudy/one_dot_per_zipcode/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.480220 vegafusion-1.6.8/tests/altair_mocks/casestudy/top_k_items/
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/casestudy/top_k_items/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.480220 vegafusion-1.6.8/tests/altair_mocks/casestudy/top_k_letters/
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/casestudy/top_k_letters/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.480220 vegafusion-1.6.8/tests/altair_mocks/casestudy/top_k_with_others/
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/casestudy/top_k_with_others/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.480220 vegafusion-1.6.8/tests/altair_mocks/casestudy/us_employment/
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/casestudy/us_employment/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.480220 vegafusion-1.6.8/tests/altair_mocks/casestudy/us_population_over_time_facet/
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/casestudy/us_population_over_time_facet/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.480220 vegafusion-1.6.8/tests/altair_mocks/casestudy/us_state_capitals/
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/casestudy/us_state_capitals/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.480220 vegafusion-1.6.8/tests/altair_mocks/casestudy/wheat_wages/
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/casestudy/wheat_wages/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.480220 vegafusion-1.6.8/tests/altair_mocks/casestudy/window_rank/
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/casestudy/window_rank/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.460219 vegafusion-1.6.8/tests/altair_mocks/circular/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.480220 vegafusion-1.6.8/tests/altair_mocks/circular/donut/
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/circular/donut/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.480220 vegafusion-1.6.8/tests/altair_mocks/circular/pacman/
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/circular/pacman/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.480220 vegafusion-1.6.8/tests/altair_mocks/circular/pie/
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/circular/pie/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.480220 vegafusion-1.6.8/tests/altair_mocks/circular/pie_with_labels/
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/circular/pie_with_labels/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.480220 vegafusion-1.6.8/tests/altair_mocks/circular/radial/
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/circular/radial/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.460219 vegafusion-1.6.8/tests/altair_mocks/histogram/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.480220 vegafusion-1.6.8/tests/altair_mocks/histogram/layered/
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/histogram/layered/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.480220 vegafusion-1.6.8/tests/altair_mocks/histogram/trellis/
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/histogram/trellis/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.480220 vegafusion-1.6.8/tests/altair_mocks/histogram/with_a_global_mean_overlay/
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/histogram/with_a_global_mean_overlay/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.464219 vegafusion-1.6.8/tests/altair_mocks/interactive/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.480220 vegafusion-1.6.8/tests/altair_mocks/interactive/area-interval_selection/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/area-interval_selection/actions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/area-interval_selection/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.480220 vegafusion-1.6.8/tests/altair_mocks/interactive/brush/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/brush/actions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/brush/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.480220 vegafusion-1.6.8/tests/altair_mocks/interactive/casestudy-airport_connections/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/casestudy-airport_connections/actions.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/casestudy-airport_connections/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.480220 vegafusion-1.6.8/tests/altair_mocks/interactive/casestudy-seattle_weather_interactive/
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/casestudy-seattle_weather_interactive/actions.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/casestudy-seattle_weather_interactive/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.480220 vegafusion-1.6.8/tests/altair_mocks/interactive/casestudy-us_population_over_time/
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/casestudy-us_population_over_time/actions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/casestudy-us_population_over_time/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.480220 vegafusion-1.6.8/tests/altair_mocks/interactive/casestudy-us_population_pyramid_over_time/
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/casestudy-us_population_pyramid_over_time/actions.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/casestudy-us_population_pyramid_over_time/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.480220 vegafusion-1.6.8/tests/altair_mocks/interactive/casestudy-weather_heatmap/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/casestudy-weather_heatmap/actions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/casestudy-weather_heatmap/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.484220 vegafusion-1.6.8/tests/altair_mocks/interactive/cross_highlight/
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/cross_highlight/actions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/cross_highlight/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.484220 vegafusion-1.6.8/tests/altair_mocks/interactive/histogram-responsive/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/histogram-responsive/actions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/histogram-responsive/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.484220 vegafusion-1.6.8/tests/altair_mocks/interactive/layered_crossfilter/
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/layered_crossfilter/actions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/layered_crossfilter/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.484220 vegafusion-1.6.8/tests/altair_mocks/interactive/legend/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/legend/actions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/legend/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.484220 vegafusion-1.6.8/tests/altair_mocks/interactive/multiline_highlight/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/multiline_highlight/actions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/multiline_highlight/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.484220 vegafusion-1.6.8/tests/altair_mocks/interactive/multiline_tooltip/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/multiline_tooltip/actions.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/multiline_tooltip/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.484220 vegafusion-1.6.8/tests/altair_mocks/interactive/other-image_tooltip/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/other-image_tooltip/actions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/other-image_tooltip/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.484220 vegafusion-1.6.8/tests/altair_mocks/interactive/scatter-href/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/scatter-href/actions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/scatter-href/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.484220 vegafusion-1.6.8/tests/altair_mocks/interactive/scatter-with_linked_table/
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/scatter-with_linked_table/actions.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/scatter-with_linked_table/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.484220 vegafusion-1.6.8/tests/altair_mocks/interactive/scatter-with_minimap/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/scatter-with_minimap/actions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/scatter-with_minimap/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.484220 vegafusion-1.6.8/tests/altair_mocks/interactive/scatter_linked_brush/
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/scatter_linked_brush/actions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/scatter_linked_brush/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.484220 vegafusion-1.6.8/tests/altair_mocks/interactive/scatter_plot/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/scatter_plot/actions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/scatter_plot/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.484220 vegafusion-1.6.8/tests/altair_mocks/interactive/scatter_with_histogram/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/scatter_with_histogram/actions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/scatter_with_histogram/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.484220 vegafusion-1.6.8/tests/altair_mocks/interactive/scatter_with_layered_histogram/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/scatter_with_layered_histogram/actions.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/scatter_with_layered_histogram/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.484220 vegafusion-1.6.8/tests/altair_mocks/interactive/select_detail/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/select_detail/actions.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/select_detail/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.484220 vegafusion-1.6.8/tests/altair_mocks/interactive/select_mark_area/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/select_mark_area/actions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/select_mark_area/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.488220 vegafusion-1.6.8/tests/altair_mocks/interactive/selection_histogram/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/selection_histogram/actions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/selection_histogram/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.488220 vegafusion-1.6.8/tests/altair_mocks/interactive/selection_layer_bar_month/
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/selection_layer_bar_month/actions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/selection_layer_bar_month/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.464219 vegafusion-1.6.8/tests/altair_mocks/line/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.488220 vegafusion-1.6.8/tests/altair_mocks/line/bump_chart/
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/line/bump_chart/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.488220 vegafusion-1.6.8/tests/altair_mocks/line/filled_step_chart/
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/line/filled_step_chart/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.488220 vegafusion-1.6.8/tests/altair_mocks/line/layer_line_color_rule/
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/line/layer_line_color_rule/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.488220 vegafusion-1.6.8/tests/altair_mocks/line/multi_series/
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/line/multi_series/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.488220 vegafusion-1.6.8/tests/altair_mocks/line/percent_axis/
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/line/percent_axis/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.488220 vegafusion-1.6.8/tests/altair_mocks/line/slope_graph/
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/line/slope_graph/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.488220 vegafusion-1.6.8/tests/altair_mocks/line/slope_graph2/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/line/slope_graph2/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.488220 vegafusion-1.6.8/tests/altair_mocks/line/step_chart/
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/line/step_chart/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.488220 vegafusion-1.6.8/tests/altair_mocks/line/trail_marker/
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/line/trail_marker/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.488220 vegafusion-1.6.8/tests/altair_mocks/line/with_ci/
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/line/with_ci/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.488220 vegafusion-1.6.8/tests/altair_mocks/line/with_color_datum/
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/line/with_color_datum/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.488220 vegafusion-1.6.8/tests/altair_mocks/line/with_cumsum/
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/line/with_cumsum/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.488220 vegafusion-1.6.8/tests/altair_mocks/line/with_datum/
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/line/with_datum/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.488220 vegafusion-1.6.8/tests/altair_mocks/line/with_generator/
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/line/with_generator/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.488220 vegafusion-1.6.8/tests/altair_mocks/line/with_logarithmic_scale/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/line/with_logarithmic_scale/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.488220 vegafusion-1.6.8/tests/altair_mocks/line/with_points/
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/line/with_points/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.464219 vegafusion-1.6.8/tests/altair_mocks/maps/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.488220 vegafusion-1.6.8/tests/altair_mocks/maps/airports_count/
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/maps/airports_count/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.488220 vegafusion-1.6.8/tests/altair_mocks/maps/choropleth/
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/maps/choropleth/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.488220 vegafusion-1.6.8/tests/altair_mocks/maps/choropleth_repeat/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/maps/choropleth_repeat/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.488220 vegafusion-1.6.8/tests/altair_mocks/maps/us_incomebrackets_by_state_facet/
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/maps/us_incomebrackets_by_state_facet/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.488220 vegafusion-1.6.8/tests/altair_mocks/maps/world/
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/maps/world/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.488220 vegafusion-1.6.8/tests/altair_mocks/maps/world_projections/
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/maps/world_projections/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.468220 vegafusion-1.6.8/tests/altair_mocks/other/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.488220 vegafusion-1.6.8/tests/altair_mocks/other/bar_chart_with_highlighted_segment/
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/other/bar_chart_with_highlighted_segment/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.488220 vegafusion-1.6.8/tests/altair_mocks/other/beckers_barley_wrapped_facet/
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/other/beckers_barley_wrapped_facet/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.488220 vegafusion-1.6.8/tests/altair_mocks/other/binned_heatmap/
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/other/binned_heatmap/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.488220 vegafusion-1.6.8/tests/altair_mocks/other/boxplot/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/other/boxplot/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.488220 vegafusion-1.6.8/tests/altair_mocks/other/candlestick_chart/
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/other/candlestick_chart/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.492220 vegafusion-1.6.8/tests/altair_mocks/other/comet_chart/
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/other/comet_chart/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.492220 vegafusion-1.6.8/tests/altair_mocks/other/errorbars_with_ci/
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/other/errorbars_with_ci/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.492220 vegafusion-1.6.8/tests/altair_mocks/other/errorbars_with_std/
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/other/errorbars_with_std/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.492220 vegafusion-1.6.8/tests/altair_mocks/other/gantt_chart/
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/other/gantt_chart/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.492220 vegafusion-1.6.8/tests/altair_mocks/other/hexbins/
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/other/hexbins/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.492220 vegafusion-1.6.8/tests/altair_mocks/other/isotype_grid/
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/other/isotype_grid/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.492220 vegafusion-1.6.8/tests/altair_mocks/other/layered_chart_with_dual_axis/
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/other/layered_chart_with_dual_axis/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.492220 vegafusion-1.6.8/tests/altair_mocks/other/layered_heatmap_text/
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/other/layered_heatmap_text/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.492220 vegafusion-1.6.8/tests/altair_mocks/other/multiple_marks/
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/other/multiple_marks/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.492220 vegafusion-1.6.8/tests/altair_mocks/other/normed_parallel_coordinates/
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/other/normed_parallel_coordinates/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.492220 vegafusion-1.6.8/tests/altair_mocks/other/parallel_coordinates/
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/other/parallel_coordinates/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.492220 vegafusion-1.6.8/tests/altair_mocks/other/ranged_dot_plot/
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/other/ranged_dot_plot/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.492220 vegafusion-1.6.8/tests/altair_mocks/other/ridgeline_plot/
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/other/ridgeline_plot/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.492220 vegafusion-1.6.8/tests/altair_mocks/other/scatter_marginal_hist/
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/other/scatter_marginal_hist/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.492220 vegafusion-1.6.8/tests/altair_mocks/other/sorted_error_bars_with_ci/
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/other/sorted_error_bars_with_ci/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.492220 vegafusion-1.6.8/tests/altair_mocks/other/stem_and_leaf/
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/other/stem_and_leaf/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.492220 vegafusion-1.6.8/tests/altair_mocks/other/violin_plot/
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/other/violin_plot/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.492220 vegafusion-1.6.8/tests/altair_mocks/other/wilkinson_dot_plot/
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/other/wilkinson_dot_plot/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.468220 vegafusion-1.6.8/tests/altair_mocks/scatter/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.492220 vegafusion-1.6.8/tests/altair_mocks/scatter/binned/
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/scatter/binned/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.492220 vegafusion-1.6.8/tests/altair_mocks/scatter/bubble_plot/
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/scatter/bubble_plot/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.492220 vegafusion-1.6.8/tests/altair_mocks/scatter/connected/
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/scatter/connected/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.492220 vegafusion-1.6.8/tests/altair_mocks/scatter/dot_dash_plot/
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/scatter/dot_dash_plot/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.492220 vegafusion-1.6.8/tests/altair_mocks/scatter/matrix/
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/scatter/matrix/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.492220 vegafusion-1.6.8/tests/altair_mocks/scatter/multifeature/
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/scatter/multifeature/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.492220 vegafusion-1.6.8/tests/altair_mocks/scatter/poly_fit_regression/
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/scatter/poly_fit_regression/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.492220 vegafusion-1.6.8/tests/altair_mocks/scatter/qq/
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/scatter/qq/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.492220 vegafusion-1.6.8/tests/altair_mocks/scatter/stripplot/
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/scatter/stripplot/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.492220 vegafusion-1.6.8/tests/altair_mocks/scatter/table_bubble_plot_github/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/scatter/table_bubble_plot_github/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.492220 vegafusion-1.6.8/tests/altair_mocks/scatter/trellis/
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/scatter/trellis/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.492220 vegafusion-1.6.8/tests/altair_mocks/scatter/wind_vector_map/
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/scatter/wind_vector_map/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.492220 vegafusion-1.6.8/tests/altair_mocks/scatter/with_errorbars/
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/scatter/with_errorbars/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.492220 vegafusion-1.6.8/tests/altair_mocks/scatter/with_labels/
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/scatter/with_labels/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.496220 vegafusion-1.6.8/tests/altair_mocks/scatter/with_lowess/
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/scatter/with_lowess/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.496220 vegafusion-1.6.8/tests/altair_mocks/scatter/with_rolling_mean/
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/scatter/with_rolling_mean/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.468220 vegafusion-1.6.8/tests/altair_mocks/simple/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.496220 vegafusion-1.6.8/tests/altair_mocks/simple/bar_chart/
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/simple/bar_chart/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.496220 vegafusion-1.6.8/tests/altair_mocks/simple/heatmap/
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/simple/heatmap/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.496220 vegafusion-1.6.8/tests/altair_mocks/simple/line_chart/
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/simple/line_chart/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.496220 vegafusion-1.6.8/tests/altair_mocks/simple/scatter_tooltips/
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/simple/scatter_tooltips/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.496220 vegafusion-1.6.8/tests/altair_mocks/simple/stacked_bar_chart/
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/simple/stacked_bar_chart/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.496220 vegafusion-1.6.8/tests/altair_mocks/simple/strip_chart/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/simple/strip_chart/mock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/test_conext_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/test_datasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16868 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/test_input_utc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50706 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/test_pretransform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/test_pretransform_specs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/test_row_limit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/test_save.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/test_sql_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14052 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/test_transformed_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/test_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.496220 vegafusion-1.6.8/vegafusion/
+-rw-r--r--   0 runner    (1001) docker     (127)     3930 2024-05-07 14:03:06.000000 vegafusion-1.6.8/vegafusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-07 14:03:06.000000 vegafusion-1.6.8/vegafusion/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-07 14:03:06.000000 vegafusion-1.6.8/vegafusion/compilers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.496220 vegafusion-1.6.8/vegafusion/connection/
+-rw-r--r--   0 runner    (1001) docker     (127)     5518 2024-05-07 14:03:06.000000 vegafusion-1.6.8/vegafusion/connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13181 2024-05-07 14:03:06.000000 vegafusion-1.6.8/vegafusion/connection/duckdb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.500220 vegafusion-1.6.8/vegafusion/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-07 14:03:06.000000 vegafusion-1.6.8/vegafusion/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6071 2024-05-07 14:03:06.000000 vegafusion-1.6.8/vegafusion/dataset/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5326 2024-05-07 14:03:06.000000 vegafusion-1.6.8/vegafusion/dataset/dfi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-07 14:03:06.000000 vegafusion-1.6.8/vegafusion/dataset/duckdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-05-07 14:03:06.000000 vegafusion-1.6.8/vegafusion/dataset/snowpark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-05-07 14:03:06.000000 vegafusion-1.6.8/vegafusion/dataset/sql.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.500220 vegafusion-1.6.8/vegafusion/datasource/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-07 14:03:06.000000 vegafusion-1.6.8/vegafusion/datasource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17414 2024-05-07 14:03:06.000000 vegafusion-1.6.8/vegafusion/datasource/_dfi_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-07 14:03:06.000000 vegafusion-1.6.8/vegafusion/datasource/datasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-05-07 14:03:06.000000 vegafusion-1.6.8/vegafusion/datasource/dfi_datasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-05-07 14:03:06.000000 vegafusion-1.6.8/vegafusion/datasource/pandas_datasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-07 14:03:06.000000 vegafusion-1.6.8/vegafusion/datasource/pyarrow_datasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-07 14:03:06.000000 vegafusion-1.6.8/vegafusion/embed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7992 2024-05-07 14:03:06.000000 vegafusion-1.6.8/vegafusion/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-07 14:03:06.000000 vegafusion-1.6.8/vegafusion/jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-05-07 14:03:06.000000 vegafusion-1.6.8/vegafusion/local_tz.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.500220 vegafusion-1.6.8/vegafusion/proto/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:06.000000 vegafusion-1.6.8/vegafusion/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    85200 2024-05-07 14:03:06.000000 vegafusion-1.6.8/vegafusion/proto/datafusion_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-05-07 14:03:06.000000 vegafusion-1.6.8/vegafusion/renderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33884 2024-05-07 14:03:06.000000 vegafusion-1.6.8/vegafusion/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4267 2024-05-07 14:03:06.000000 vegafusion-1.6.8/vegafusion/save.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8401 2024-05-07 14:03:06.000000 vegafusion-1.6.8/vegafusion/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-07 14:03:06.000000 vegafusion-1.6.8/vegafusion/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.500220 vegafusion-1.6.8/vegafusion.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-07 14:03:45.000000 vegafusion-1.6.8/vegafusion.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10742 2024-05-07 14:03:45.000000 vegafusion-1.6.8/vegafusion.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 14:03:45.000000 vegafusion-1.6.8/vegafusion.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-07 14:03:45.000000 vegafusion-1.6.8/vegafusion.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-07 14:03:45.000000 vegafusion-1.6.8/vegafusion.egg-info/top_level.txt
```

### Comparing `vegafusion-1.6.7/LICENSE.txt` & `vegafusion-1.6.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/PKG-INFO` & `vegafusion-1.6.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vegafusion
-Version: 1.6.7
+Version: 1.6.8
 Summary: Core tools for using VegaFusion from Python
 License: BSD-3-Clause
 Keywords: vega,altair,vegafusion,arrow
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -14,14 +14,14 @@
 Description-Content-Type: text/markdown
 Requires-Dist: altair>=4.2.0
 Requires-Dist: pyarrow>=5
 Requires-Dist: pandas
 Requires-Dist: psutil
 Requires-Dist: protobuf
 Provides-Extra: embed
-Requires-Dist: vegafusion-python-embed==1.6.7; extra == "embed"
+Requires-Dist: vegafusion-python-embed==1.6.8; extra == "embed"
 Requires-Dist: vl-convert-python>=0.7.0; extra == "embed"
 
 ## VegaFusion
 This package is part of the VegaFusion project: https://vegafusion.io.
 
 In particular, the `vegafusion` package provides a pure Python interface to a VegaFusion Runtime. Initially, the only runtime available is provided by the `vegafusion-python-embed` package. Eventually, the VegaFusion runtime will be available as a standalone gRPC server and this package will be updated to support communication with a VegaFusion Runtime over gRPC as an alternative to the Runtime provided by `vegafusion-python-embed`.
```

### Comparing `vegafusion-1.6.7/README.md` & `vegafusion-1.6.8/README.md`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/proto/datafusion.proto` & `vegafusion-1.6.8/proto/datafusion.proto`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/setup.cfg` & `vegafusion-1.6.8/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [bdist_wheel]
 universal = 0
 
 [metadata]
 name = vegafusion
 description = Core tools for using VegaFusion from Python
-version = 1.6.7
+version = 1.6.8
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = vega, altair, vegafusion, arrow
 license = BSD-3-Clause
 license_files = [LICENSE.txt]
 python = "^3.7"
 homepage = "https://vegafusion.io"
@@ -31,14 +31,14 @@
 	pyarrow>=5
 	pandas
 	psutil
 	protobuf
 
 [options.extras_require]
 embed = 
-	vegafusion-python-embed==1.6.7
+	vegafusion-python-embed==1.6.8
 	vl-convert-python>=0.7.0
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `vegafusion-1.6.7/tests/altair_mocks/area/density_facet/mock.py` & `vegafusion-1.6.8/tests/altair_mocks/area/density_facet/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/tests/altair_mocks/area/density_stack/mock.py` & `vegafusion-1.6.8/tests/altair_mocks/area/density_stack/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/tests/altair_mocks/area/gradient/mock.py` & `vegafusion-1.6.8/tests/altair_mocks/area/gradient/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/tests/altair_mocks/area/horizon_graph/mock.py` & `vegafusion-1.6.8/tests/altair_mocks/area/horizon_graph/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/tests/altair_mocks/bar/and_tick_chart/mock.py` & `vegafusion-1.6.8/tests/altair_mocks/bar/and_tick_chart/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/tests/altair_mocks/bar/diverging_stacked/mock.py` & `vegafusion-1.6.8/tests/altair_mocks/bar/diverging_stacked/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/tests/altair_mocks/bar/stacked_with_text_overlay/mock.py` & `vegafusion-1.6.8/tests/altair_mocks/bar/stacked_with_text_overlay/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/tests/altair_mocks/bar/trellis_compact/mock.py` & `vegafusion-1.6.8/tests/altair_mocks/bar/trellis_compact/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/tests/altair_mocks/bar/with_highlighted_bar/mock.py` & `vegafusion-1.6.8/tests/altair_mocks/bar/with_highlighted_bar/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/tests/altair_mocks/bar/with_rolling_mean/mock.py` & `vegafusion-1.6.8/tests/altair_mocks/bar/with_rolling_mean/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/tests/altair_mocks/casestudy/airports/mock.py` & `vegafusion-1.6.8/tests/altair_mocks/casestudy/airports/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/tests/altair_mocks/casestudy/beckers_barley_trellis_plot/mock.py` & `vegafusion-1.6.8/tests/altair_mocks/casestudy/beckers_barley_trellis_plot/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/tests/altair_mocks/casestudy/co2_concentration/mock.py` & `vegafusion-1.6.8/tests/altair_mocks/casestudy/co2_concentration/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/tests/altair_mocks/casestudy/falkensee/mock.py` & `vegafusion-1.6.8/tests/altair_mocks/casestudy/falkensee/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/tests/altair_mocks/casestudy/iowa_electricity/mock.py` & `vegafusion-1.6.8/tests/altair_mocks/casestudy/iowa_electricity/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/tests/altair_mocks/casestudy/isotype/mock.py` & `vegafusion-1.6.8/tests/altair_mocks/casestudy/isotype/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/tests/altair_mocks/casestudy/isotype_emoji/mock.py` & `vegafusion-1.6.8/tests/altair_mocks/casestudy/isotype_emoji/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/tests/altair_mocks/casestudy/london_tube/mock.py` & `vegafusion-1.6.8/tests/altair_mocks/casestudy/london_tube/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/tests/altair_mocks/casestudy/natural_disasters/mock.py` & `vegafusion-1.6.8/tests/altair_mocks/casestudy/natural_disasters/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/tests/altair_mocks/casestudy/one_dot_per_zipcode/mock.py` & `vegafusion-1.6.8/tests/altair_mocks/casestudy/one_dot_per_zipcode/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/tests/altair_mocks/casestudy/top_k_items/mock.py` & `vegafusion-1.6.8/tests/altair_mocks/casestudy/top_k_items/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/tests/altair_mocks/casestudy/top_k_letters/mock.py` & `vegafusion-1.6.8/tests/altair_mocks/casestudy/top_k_letters/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/tests/altair_mocks/casestudy/top_k_with_others/mock.py` & `vegafusion-1.6.8/tests/altair_mocks/casestudy/top_k_with_others/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/tests/altair_mocks/casestudy/us_employment/mock.py` & `vegafusion-1.6.8/tests/altair_mocks/casestudy/us_employment/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/tests/altair_mocks/casestudy/us_state_capitals/mock.py` & `vegafusion-1.6.8/tests/altair_mocks/casestudy/us_state_capitals/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/tests/altair_mocks/casestudy/wheat_wages/mock.py` & `vegafusion-1.6.8/tests/altair_mocks/casestudy/wheat_wages/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/tests/altair_mocks/casestudy/window_rank/mock.py` & `vegafusion-1.6.8/tests/altair_mocks/casestudy/window_rank/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/tests/altair_mocks/histogram/layered/mock.py` & `vegafusion-1.6.8/tests/altair_mocks/histogram/layered/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/tests/altair_mocks/interactive/casestudy-airport_connections/mock.py` & `vegafusion-1.6.8/tests/altair_mocks/interactive/casestudy-airport_connections/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/tests/altair_mocks/interactive/casestudy-seattle_weather_interactive/mock.py` & `vegafusion-1.6.8/tests/altair_mocks/interactive/casestudy-seattle_weather_interactive/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/tests/altair_mocks/interactive/casestudy-us_population_over_time/mock.py` & `vegafusion-1.6.8/tests/altair_mocks/interactive/casestudy-us_population_over_time/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/tests/altair_mocks/interactive/casestudy-us_population_pyramid_over_time/mock.py` & `vegafusion-1.6.8/tests/altair_mocks/interactive/casestudy-us_population_pyramid_over_time/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/tests/altair_mocks/interactive/casestudy-weather_heatmap/mock.py` & `vegafusion-1.6.8/tests/altair_mocks/interactive/casestudy-weather_heatmap/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/tests/altair_mocks/interactive/cross_highlight/mock.py` & `vegafusion-1.6.8/tests/altair_mocks/interactive/cross_highlight/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/tests/altair_mocks/interactive/histogram-responsive/mock.py` & `vegafusion-1.6.8/tests/altair_mocks/interactive/histogram-responsive/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/tests/altair_mocks/interactive/layered_crossfilter/actions.json` & `vegafusion-1.6.8/tests/altair_mocks/interactive/layered_crossfilter/actions.json`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/tests/altair_mocks/interactive/layered_crossfilter/mock.py` & `vegafusion-1.6.8/tests/altair_mocks/interactive/layered_crossfilter/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/tests/altair_mocks/interactive/legend/mock.py` & `vegafusion-1.6.8/tests/altair_mocks/interactive/legend/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/tests/altair_mocks/interactive/multiline_highlight/mock.py` & `vegafusion-1.6.8/tests/altair_mocks/interactive/multiline_highlight/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/tests/altair_mocks/interactive/multiline_tooltip/mock.py` & `vegafusion-1.6.8/tests/altair_mocks/interactive/multiline_tooltip/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/tests/altair_mocks/interactive/scatter-with_linked_table/mock.py` & `vegafusion-1.6.8/tests/altair_mocks/interactive/scatter-with_linked_table/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/tests/altair_mocks/interactive/scatter-with_minimap/mock.py` & `vegafusion-1.6.8/tests/altair_mocks/interactive/scatter-with_minimap/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/tests/altair_mocks/interactive/scatter_with_histogram/mock.py` & `vegafusion-1.6.8/tests/altair_mocks/interactive/scatter_with_histogram/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/tests/altair_mocks/interactive/scatter_with_layered_histogram/mock.py` & `vegafusion-1.6.8/tests/altair_mocks/interactive/scatter_with_layered_histogram/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/tests/altair_mocks/interactive/select_detail/mock.py` & `vegafusion-1.6.8/tests/altair_mocks/interactive/select_detail/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/tests/altair_mocks/interactive/selection_layer_bar_month/mock.py` & `vegafusion-1.6.8/tests/altair_mocks/interactive/selection_layer_bar_month/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/tests/altair_mocks/line/bump_chart/mock.py` & `vegafusion-1.6.8/tests/altair_mocks/line/bump_chart/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/tests/altair_mocks/line/with_cumsum/mock.py` & `vegafusion-1.6.8/tests/altair_mocks/line/with_cumsum/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/tests/altair_mocks/line/with_datum/mock.py` & `vegafusion-1.6.8/tests/altair_mocks/line/with_datum/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/tests/altair_mocks/maps/airports_count/mock.py` & `vegafusion-1.6.8/tests/altair_mocks/maps/airports_count/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/tests/altair_mocks/maps/choropleth_repeat/mock.py` & `vegafusion-1.6.8/tests/altair_mocks/maps/choropleth_repeat/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/tests/altair_mocks/maps/us_incomebrackets_by_state_facet/mock.py` & `vegafusion-1.6.8/tests/altair_mocks/maps/us_incomebrackets_by_state_facet/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/tests/altair_mocks/maps/world/mock.py` & `vegafusion-1.6.8/tests/altair_mocks/maps/world/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/tests/altair_mocks/other/bar_chart_with_highlighted_segment/mock.py` & `vegafusion-1.6.8/tests/altair_mocks/other/bar_chart_with_highlighted_segment/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/tests/altair_mocks/other/candlestick_chart/mock.py` & `vegafusion-1.6.8/tests/altair_mocks/other/candlestick_chart/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/tests/altair_mocks/other/comet_chart/mock.py` & `vegafusion-1.6.8/tests/altair_mocks/other/comet_chart/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/tests/altair_mocks/other/errorbars_with_ci/mock.py` & `vegafusion-1.6.8/tests/altair_mocks/other/errorbars_with_ci/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/tests/altair_mocks/other/hexbins/mock.py` & `vegafusion-1.6.8/tests/altair_mocks/other/hexbins/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/tests/altair_mocks/other/isotype_grid/mock.py` & `vegafusion-1.6.8/tests/altair_mocks/other/isotype_grid/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/tests/altair_mocks/other/layered_chart_with_dual_axis/mock.py` & `vegafusion-1.6.8/tests/altair_mocks/other/layered_chart_with_dual_axis/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/tests/altair_mocks/other/layered_heatmap_text/mock.py` & `vegafusion-1.6.8/tests/altair_mocks/other/layered_heatmap_text/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/tests/altair_mocks/other/normed_parallel_coordinates/mock.py` & `vegafusion-1.6.8/tests/altair_mocks/other/normed_parallel_coordinates/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/tests/altair_mocks/other/ranged_dot_plot/mock.py` & `vegafusion-1.6.8/tests/altair_mocks/other/ranged_dot_plot/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/tests/altair_mocks/other/ridgeline_plot/mock.py` & `vegafusion-1.6.8/tests/altair_mocks/other/ridgeline_plot/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/tests/altair_mocks/other/scatter_marginal_hist/mock.py` & `vegafusion-1.6.8/tests/altair_mocks/other/scatter_marginal_hist/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/tests/altair_mocks/other/sorted_error_bars_with_ci/mock.py` & `vegafusion-1.6.8/tests/altair_mocks/other/sorted_error_bars_with_ci/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/tests/altair_mocks/other/stem_and_leaf/mock.py` & `vegafusion-1.6.8/tests/altair_mocks/other/stem_and_leaf/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/tests/altair_mocks/other/violin_plot/mock.py` & `vegafusion-1.6.8/tests/altair_mocks/other/violin_plot/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/tests/altair_mocks/scatter/dot_dash_plot/mock.py` & `vegafusion-1.6.8/tests/altair_mocks/scatter/dot_dash_plot/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/tests/altair_mocks/scatter/poly_fit_regression/mock.py` & `vegafusion-1.6.8/tests/altair_mocks/scatter/poly_fit_regression/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/tests/altair_mocks/scatter/stripplot/mock.py` & `vegafusion-1.6.8/tests/altair_mocks/scatter/stripplot/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/tests/altair_mocks/scatter/wind_vector_map/mock.py` & `vegafusion-1.6.8/tests/altair_mocks/scatter/wind_vector_map/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/tests/altair_mocks/scatter/with_errorbars/mock.py` & `vegafusion-1.6.8/tests/altair_mocks/scatter/with_errorbars/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/tests/altair_mocks/scatter/with_lowess/mock.py` & `vegafusion-1.6.8/tests/altair_mocks/scatter/with_lowess/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/tests/altair_mocks/scatter/with_rolling_mean/mock.py` & `vegafusion-1.6.8/tests/altair_mocks/scatter/with_rolling_mean/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/tests/test_conext_manager.py` & `vegafusion-1.6.8/tests/test_conext_manager.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/tests/test_datasource.py` & `vegafusion-1.6.8/tests/test_datasource.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/tests/test_input_utc.py` & `vegafusion-1.6.8/tests/test_input_utc.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/tests/test_pretransform.py` & `vegafusion-1.6.8/tests/test_pretransform.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/tests/test_pretransform_specs.py` & `vegafusion-1.6.8/tests/test_pretransform_specs.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/tests/test_row_limit.py` & `vegafusion-1.6.8/tests/test_row_limit.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/tests/test_save.py` & `vegafusion-1.6.8/tests/test_save.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/tests/test_transformed_data.py` & `vegafusion-1.6.8/tests/test_transformed_data.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/tests/test_transformer.py` & `vegafusion-1.6.8/tests/test_transformer.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/vegafusion/__init__.py` & `vegafusion-1.6.8/vegafusion/__init__.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/vegafusion/compilers.py` & `vegafusion-1.6.8/vegafusion/compilers.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/vegafusion/connection/__init__.py` & `vegafusion-1.6.8/vegafusion/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/vegafusion/connection/duckdb.py` & `vegafusion-1.6.8/vegafusion/connection/duckdb.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/vegafusion/dataset/dataframe.py` & `vegafusion-1.6.8/vegafusion/dataset/dataframe.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/vegafusion/dataset/dfi.py` & `vegafusion-1.6.8/vegafusion/dataset/dfi.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/vegafusion/dataset/duckdb.py` & `vegafusion-1.6.8/vegafusion/dataset/duckdb.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/vegafusion/dataset/snowpark.py` & `vegafusion-1.6.8/vegafusion/dataset/snowpark.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/vegafusion/dataset/sql.py` & `vegafusion-1.6.8/vegafusion/dataset/sql.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/vegafusion/datasource/_dfi_types.py` & `vegafusion-1.6.8/vegafusion/datasource/_dfi_types.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/vegafusion/datasource/dfi_datasource.py` & `vegafusion-1.6.8/vegafusion/datasource/dfi_datasource.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/vegafusion/datasource/pandas_datasource.py` & `vegafusion-1.6.8/vegafusion/datasource/pandas_datasource.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/vegafusion/evaluation.py` & `vegafusion-1.6.8/vegafusion/evaluation.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/vegafusion/local_tz.py` & `vegafusion-1.6.8/vegafusion/local_tz.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/vegafusion/proto/datafusion_pb2.py` & `vegafusion-1.6.8/vegafusion/proto/datafusion_pb2.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/vegafusion/renderer.py` & `vegafusion-1.6.8/vegafusion/renderer.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/vegafusion/runtime.py` & `vegafusion-1.6.8/vegafusion/runtime.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/vegafusion/save.py` & `vegafusion-1.6.8/vegafusion/save.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/vegafusion/transformer.py` & `vegafusion-1.6.8/vegafusion/transformer.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/vegafusion/utils.py` & `vegafusion-1.6.8/vegafusion/utils.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.7/vegafusion.egg-info/PKG-INFO` & `vegafusion-1.6.8/vegafusion.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vegafusion
-Version: 1.6.7
+Version: 1.6.8
 Summary: Core tools for using VegaFusion from Python
 License: BSD-3-Clause
 Keywords: vega,altair,vegafusion,arrow
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -14,14 +14,14 @@
 Description-Content-Type: text/markdown
 Requires-Dist: altair>=4.2.0
 Requires-Dist: pyarrow>=5
 Requires-Dist: pandas
 Requires-Dist: psutil
 Requires-Dist: protobuf
 Provides-Extra: embed
-Requires-Dist: vegafusion-python-embed==1.6.7; extra == "embed"
+Requires-Dist: vegafusion-python-embed==1.6.8; extra == "embed"
 Requires-Dist: vl-convert-python>=0.7.0; extra == "embed"
 
 ## VegaFusion
 This package is part of the VegaFusion project: https://vegafusion.io.
 
 In particular, the `vegafusion` package provides a pure Python interface to a VegaFusion Runtime. Initially, the only runtime available is provided by the `vegafusion-python-embed` package. Eventually, the VegaFusion runtime will be available as a standalone gRPC server and this package will be updated to support communication with a VegaFusion Runtime over gRPC as an alternative to the Runtime provided by `vegafusion-python-embed`.
```

### Comparing `vegafusion-1.6.7/vegafusion.egg-info/SOURCES.txt` & `vegafusion-1.6.8/vegafusion.egg-info/SOURCES.txt`

 * *Files identical despite different names*

