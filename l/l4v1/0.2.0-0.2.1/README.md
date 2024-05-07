# Comparing `tmp/l4v1-0.2.0.tar.gz` & `tmp/l4v1-0.2.1.tar.gz`

## Comparing `l4v1-0.2.0.tar` & `l4v1-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 l4v1-0.2.0/.python-version
--rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 l4v1-0.2.0/TESTING.py
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 l4v1-0.2.0/requirements-dev.lock
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 l4v1-0.2.0/requirements.lock
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 l4v1-0.2.0/.github/workflows/python-tests.yml
--rw-r--r--   0        0        0    42532 2020-02-02 00:00:00.000000 l4v1-0.2.0/data/supermarket_sales.parquet
--rw-r--r--   0        0        0   172599 2020-02-02 00:00:00.000000 l4v1-0.2.0/docs/readme/example_excel_heatmap.png
--rw-r--r--   0        0        0   112382 2020-02-02 00:00:00.000000 l4v1-0.2.0/docs/readme/example_waterfall.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 l4v1-0.2.0/l4v1/__init__.py
--rw-r--r--   0        0        0    16815 2020-02-02 00:00:00.000000 l4v1-0.2.0/l4v1/price_volume_mix.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 l4v1-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 l4v1-0.2.0/tests/test_price_volume_mix.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 l4v1-0.2.0/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 l4v1-0.2.0/LICENSE
--rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 l4v1-0.2.0/README.md
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 l4v1-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2539 2020-02-02 00:00:00.000000 l4v1-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 l4v1-0.2.1/.python-version
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 l4v1-0.2.1/TESTING.py
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 l4v1-0.2.1/requirements-dev.lock
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 l4v1-0.2.1/requirements.lock
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 l4v1-0.2.1/.github/workflows/python-tests.yml
+-rw-r--r--   0        0        0    42532 2020-02-02 00:00:00.000000 l4v1-0.2.1/data/supermarket_sales.parquet
+-rw-r--r--   0        0        0   172599 2020-02-02 00:00:00.000000 l4v1-0.2.1/docs/readme/example_excel_heatmap.png
+-rw-r--r--   0        0        0   112382 2020-02-02 00:00:00.000000 l4v1-0.2.1/docs/readme/example_waterfall.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 l4v1-0.2.1/l4v1/__init__.py
+-rw-r--r--   0        0        0    15974 2020-02-02 00:00:00.000000 l4v1-0.2.1/l4v1/price_volume_mix.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 l4v1-0.2.1/tests/__init__.py
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 l4v1-0.2.1/tests/test_price_volume_mix.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 l4v1-0.2.1/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 l4v1-0.2.1/LICENSE
+-rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 l4v1-0.2.1/README.md
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 l4v1-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2539 2020-02-02 00:00:00.000000 l4v1-0.2.1/PKG-INFO
```

### Comparing `l4v1-0.2.0/TESTING.py` & `l4v1-0.2.1/TESTING.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from l4v1.price_volume_mix import PVM
 import polars as pl
 
 sales_week_1 = pl.read_parquet("data/supermarket_sales.parquet").filter(
     pl.col("Datetime").dt.week() == 1
 )
 sales_week_2 = pl.read_parquet("data/supermarket_sales.parquet").filter(
-    pl.col("Datetime").dt.week() == 2
+    pl.col("Datetime").dt.month() == 2
 )
 
 
 pvm = PVM(
     df_primary=sales_week_2,
     df_comparison=sales_week_1,
     group_by_columns=["Product line", "Customer type", "Gender"],
@@ -18,19 +18,9 @@
 )
 
 pvm.waterfall_plot(
     primary_total_label="Week 2 Sales",
     comparison_total_label="Week 1 Sales",
     format_data_labels="{:,.0f}€",
     title="Sales Week 2 vs 1",
-    color_total = "#F1F1F1",
+    color_total="#F1F1F1",
 )
-
-
-
-
-# pvm.get_table()
-
-
-# pvm.write_xlsx_table("/mnt/c/Users/mirol/Downloads/testing.xlsx")
-
-pvm.get_table().schema
```

### Comparing `l4v1-0.2.0/requirements-dev.lock` & `l4v1-0.2.1/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `l4v1-0.2.0/.github/workflows/python-tests.yml` & `l4v1-0.2.1/.github/workflows/python-tests.yml`

 * *Files identical despite different names*

### Comparing `l4v1-0.2.0/data/supermarket_sales.parquet` & `l4v1-0.2.1/data/supermarket_sales.parquet`

 * *Files identical despite different names*

### Comparing `l4v1-0.2.0/docs/readme/example_excel_heatmap.png` & `l4v1-0.2.1/docs/readme/example_excel_heatmap.png`

 * *Files identical despite different names*

### Comparing `l4v1-0.2.0/docs/readme/example_waterfall.png` & `l4v1-0.2.1/docs/readme/example_waterfall.png`

 * *Files identical despite different names*

### Comparing `l4v1-0.2.0/l4v1/price_volume_mix.py` & `l4v1-0.2.1/l4v1/price_volume_mix.py`

 * *Files 7% similar despite different names*

```diff
@@ -108,60 +108,38 @@
         )
         rate_diff_pct = (rate_diff / rate_comparison).alias(
             f"{self._rate_metric_name}_diff_%"
         )
         rate_avg_comparison = outcome_comparison.sum() / volume_comparison.sum()
 
         # Expressions for the bridge
-        rate = (rate_new - rate_comparison) * volume_new
-        volume = volume_diff * rate_avg_comparison
-        mix = (rate_comparison - rate_avg_comparison) * volume_diff
-
-        def effect_expression(expr: pl.Expr, name: str) -> pl.Expr:
-            return (
-                pl.when((outcome_comparison.is_null()) | (outcome_new.is_null()))
-                .then(pl.lit(0))
-                .otherwise(expr)
-            ).alias(f"{name}_effect")
-
-        rate_expr = effect_expression(rate, "rate")
-        volume_expr = effect_expression(volume, "volume")
-        mix_expr = effect_expression(mix, "mix")
-
-        new_expr = (
-            pl.when((outcome_comparison.is_null()) & (outcome_new.is_not_null()))
-            .then(outcome_new)
-            .otherwise(pl.lit(0))
-            .alias("new_effect")
-        )
-        old_expr = (
-            pl.when((outcome_new.is_null()) & (outcome_comparison.is_not_null()))
-            .then(outcome_comparison * -1)
-            .otherwise(pl.lit(0))
-            .alias("old_effect")
-        )
+        rate_effect = ((rate_new - rate_comparison) * volume_new).alias("rate_effect")
+        volume_effect = (volume_diff * rate_avg_comparison).alias("volume_effect")
+        mix_effect = (
+            pl.when(rate_comparison.is_null() | rate_comparison.is_nan())
+            .then((rate_new - rate_avg_comparison) * volume_diff)
+            .otherwise((rate_comparison - rate_avg_comparison) * volume_diff)
+        ).alias("mix_effect")
 
         return (
             volume_new,
             volume_comparison,
             volume_diff,
             volume_diff_pct,
             rate_new,
             rate_comparison,
             rate_diff,
             rate_diff_pct,
             outcome_new,
             outcome_comparison,
             outcome_diff,
             outcome_diff_pct,
-            volume_expr,
-            rate_expr,
-            mix_expr,
-            new_expr,
-            old_expr,
+            volume_effect,
+            rate_effect,
+            mix_effect,
         )
 
     def get_table(self) -> pl.DataFrame:
         """
         Generates a summary table for changes together with price, volume, and mix effects.
 
         Returns:
@@ -203,16 +181,16 @@
             workbook=file_path,
             table_style="Table Style Light 1",
             conditional_formats={
                 (
                     "volume_effect",
                     "rate_effect",
                     "mix_effect",
-                    "new_effect",
-                    "old_effect",
+                    # "new_effect",
+                    # "old_effect",
                 ): {
                     "type": "3_color_scale",
                     "min_color": "#ff0000",
                     "mid_color": "#ffffff",
                     "max_color": "#73e656",
                 }
             },
@@ -242,16 +220,16 @@
             },
             freeze_panes=(1, 0),
             column_widths={
                 "group_keys": 250,
                 "volume_effect": 100,
                 "rate_effect": 100,
                 "mix_effect": 100,
-                "new_effect": 100,
-                "old_effect": 100,
+                # "new_effect": 100,
+                # "old_effect": 100,
             },
         )
 
     def _create_data_label(
         self, value: float, previous_value: float, format_func: Callable
     ) -> str:
         formatted_value = format_func(value)
@@ -286,19 +264,15 @@
         y_values.append(outcome_comparison)
         data_labels.append(f"<b>{format_data_labels(outcome_comparison)}</b>")
         measure_list.append("absolute")
 
         cumulative_sum = outcome_comparison
         previous_value = outcome_comparison
 
-        impact_types = ["volume", "rate", "mix", "old", "new"]
-        if (impact_table.get_column("old_effect").sum() == 0) & (
-            impact_table.get_column("new_effect").sum() == 0
-        ):
-            impact_types = ["volume", "rate", "mix"]
+        impact_types = ["volume", "rate", "mix"]
 
         for impact_type in impact_types:
             for key in (
                 impact_table.get_column("group_keys").unique().sort(descending=True)
             ):
                 impact_value = (
                     impact_table.filter(pl.col("group_keys") == key)
```

### Comparing `l4v1-0.2.0/tests/test_price_volume_mix.py` & `l4v1-0.2.1/tests/test_price_volume_mix.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,16 +27,16 @@
     effect_sum = (
         summary_table.select(
             pl.sum_horizontal(
                 [
                     "volume_effect",
                     "rate_effect",
                     "mix_effect",
-                    "new_effect",
-                    "old_effect",
+                    # "new_effect",
+                    # "old_effect",
                 ]
             )
         )
         .sum()
         .item()
     )
```

### Comparing `l4v1-0.2.0/.gitignore` & `l4v1-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `l4v1-0.2.0/LICENSE` & `l4v1-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `l4v1-0.2.0/README.md` & `l4v1-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `l4v1-0.2.0/pyproject.toml` & `l4v1-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "l4v1"
-version = "0.2.0"
+version = "0.2.1"
 description = "A Python library to simplify data-analytics tasks"
 authors = [
     { name = "Miro Lavi", email = "info.l4v1@gmail.com" }
 ]
 dependencies = [
     "plotly>=5.20.0",
     "xlsxwriter>=3.2.0",
```

### Comparing `l4v1-0.2.0/PKG-INFO` & `l4v1-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: l4v1
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Python library to simplify data-analytics tasks
 Author-email: Miro Lavi <info.l4v1@gmail.com>
 License-File: LICENSE
 Requires-Python: >=3.10
 Requires-Dist: plotly>=5.20.0
 Requires-Dist: polars>=0.20.23
 Requires-Dist: xlsxwriter>=3.2.0
```

