# Comparing `tmp/proksee_batch-0.5.9.tar.gz` & `tmp/proksee_batch-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proksee_batch-0.5.9.tar", max compression
+gzip compressed data, was "proksee_batch-0.6.0.tar", max compression
```

## Comparing `proksee_batch-0.5.9.tar` & `proksee_batch-0.6.0.tar`

### file list

```diff
@@ -1,42 +1,43 @@
--rw-r--r--   0        0        0     1089 2024-04-18 15:56:28.918512 proksee_batch-0.5.9/LICENSE
--rw-r--r--   0        0        0     3861 2024-04-18 15:56:28.918512 proksee_batch-0.5.9/README.md
--rw-r--r--   0        0        0     1797 2024-04-18 15:56:40.294520 proksee_batch-0.5.9/pyproject.toml
--rw-r--r--   0        0        0       21 2024-04-18 15:56:28.922512 proksee_batch-0.5.9/src/proksee_batch/__init__.py
--rw-r--r--   0        0        0    15177 2024-04-18 15:56:28.922512 proksee_batch-0.5.9/src/proksee_batch/__main__.py
--rw-r--r--   0        0        0     2330 2024-04-18 15:56:28.922512 proksee_batch-0.5.9/src/proksee_batch/data/assets/images/GitHub-Mark-Light-64px.png
--rw-r--r--   0        0        0    22591 2024-04-18 15:56:28.922512 proksee_batch-0.5.9/src/proksee_batch/data/assets/scripts/batch.js
--rw-r--r--   0        0        0   208923 2024-04-18 15:56:28.926512 proksee_batch-0.5.9/src/proksee_batch/data/assets/scripts/cgview.min.js
--rw-r--r--   0        0        0     1843 2024-04-18 15:56:28.926512 proksee_batch-0.5.9/src/proksee_batch/data/assets/scripts/controls.js
--rw-r--r--   0        0        0   274269 2024-04-18 15:56:28.926512 proksee_batch-0.5.9/src/proksee_batch/data/assets/scripts/d3.min.js
--rw-r--r--   0        0        0    61938 2024-04-18 15:56:28.926512 proksee_batch-0.5.9/src/proksee_batch/data/assets/scripts/svgcanvas.iife.js
--rw-r--r--   0        0        0    14980 2024-04-18 15:56:28.926512 proksee_batch-0.5.9/src/proksee_batch/data/assets/styles/cgview.css
--rw-r--r--   0        0        0     5696 2024-04-18 15:56:28.926512 proksee_batch-0.5.9/src/proksee_batch/data/assets/styles/controls.css
--rw-r--r--   0        0        0    12170 2024-04-18 15:56:28.926512 proksee_batch-0.5.9/src/proksee_batch/data/assets/styles/style.css
--rw-r--r--   0        0        0  5809583 2024-04-18 15:56:28.954512 proksee_batch-0.5.9/src/proksee_batch/data/data.example/genome_maps/genome_1.js
--rw-r--r--   0        0        0  5469891 2024-04-18 15:56:28.962512 proksee_batch-0.5.9/src/proksee_batch/data/data.example/genome_maps/genome_2.js
--rw-r--r--   0        0        0  6164597 2024-04-18 15:56:28.986512 proksee_batch-0.5.9/src/proksee_batch/data/data.example/genome_maps/genome_3.js
--rw-r--r--   0        0        0  7518134 2024-04-18 15:56:29.010512 proksee_batch-0.5.9/src/proksee_batch/data/data.example/genome_maps/genome_4.js
--rw-r--r--   0        0        0     3605 2024-04-18 15:56:29.010512 proksee_batch-0.5.9/src/proksee_batch/data/data.example/table_data.js
--rw-r--r--   0        0        0   221376 2024-04-18 15:56:29.010512 proksee_batch-0.5.9/src/proksee_batch/data/default_proksee_template.json
--rw-r--r--   0        0        0      158 2024-04-18 15:56:29.010512 proksee_batch-0.5.9/src/proksee_batch/data/example_input_dir/Escherichia_coli_str._K-12_substr._MG1655/bed/e_coli_features.bed
--rw-r--r--   0        0        0      269 2024-04-18 15:56:29.010512 proksee_batch-0.5.9/src/proksee_batch/data/example_input_dir/Escherichia_coli_str._K-12_substr._MG1655/blast/blast_against_e_coli.txt
--rw-r--r--   0        0        0      180 2024-04-18 15:56:29.010512 proksee_batch-0.5.9/src/proksee_batch/data/example_input_dir/Escherichia_coli_str._K-12_substr._MG1655/vcf/e_coli_variants.vcf
--rw-r--r--   0        0        0       79 2024-04-18 15:56:29.010512 proksee_batch-0.5.9/src/proksee_batch/data/example_input_dir/Klebsiella_aerogenes/bed/k_aerogenes_features.bed
--rw-r--r--   0        0        0      134 2024-04-18 15:56:29.010512 proksee_batch-0.5.9/src/proksee_batch/data/example_input_dir/Klebsiella_aerogenes/blast/blast_against_k_aerogenes.txt
--rw-r--r--   0        0        0       75 2024-04-18 15:56:29.010512 proksee_batch-0.5.9/src/proksee_batch/data/example_input_dir/Salmonella_enterica_subsp._enterica_serovar_Typhimurium_str._LT2/bed/s_enterica_features.bed
--rw-r--r--   0        0        0      130 2024-04-18 15:56:29.010512 proksee_batch-0.5.9/src/proksee_batch/data/example_input_dir/Salmonella_enterica_subsp._enterica_serovar_Typhimurium_str._LT2/blast/blast_against_s_enterica.txt
--rw-r--r--   0        0        0       75 2024-04-18 15:56:29.010512 proksee_batch-0.5.9/src/proksee_batch/data/example_input_dir/Shigella_flexneri_2a_str._301/bed/s_flexneri_features.bed
--rw-r--r--   0        0        0      130 2024-04-18 15:56:29.010512 proksee_batch-0.5.9/src/proksee_batch/data/example_input_dir/Shigella_flexneri_2a_str._301/blast/blast_against_s_flexneri.txt
--rw-r--r--   0        0        0     5127 2024-04-18 15:56:29.010512 proksee_batch-0.5.9/src/proksee_batch/data/report.html
--rw-r--r--   0        0        0     6474 2024-04-18 15:56:29.010512 proksee_batch-0.5.9/src/proksee_batch/download_example_input.py
--rw-r--r--   0        0        0      895 2024-04-18 15:56:29.010512 proksee_batch-0.5.9/src/proksee_batch/generate_proksee_link.py
--rw-r--r--   0        0        0     5311 2024-04-18 15:56:29.010512 proksee_batch-0.5.9/src/proksee_batch/generate_report_html.py
--rw-r--r--   0        0        0     1037 2024-04-18 15:56:29.010512 proksee_batch-0.5.9/src/proksee_batch/get_stats_from_seq_file.py
--rw-r--r--   0        0        0     1952 2024-04-18 15:56:29.010512 proksee_batch-0.5.9/src/proksee_batch/merge_cgview_json_with_template.py
--rw-r--r--   0        0        0    21812 2024-04-18 15:56:29.010512 proksee_batch-0.5.9/src/proksee_batch/parse_additional_features.py
--rw-r--r--   0        0        0        0 2024-04-18 15:56:29.010512 proksee_batch-0.5.9/src/proksee_batch/py.typed
--rw-r--r--   0        0        0     1163 2024-04-18 15:56:29.010512 proksee_batch-0.5.9/src/proksee_batch/remove_covered_features.py
--rw-r--r--   0        0        0     2658 2024-04-18 15:56:29.010512 proksee_batch-0.5.9/src/proksee_batch/scrape_proksee_image.py
--rw-r--r--   0        0        0    11471 2024-04-18 15:56:29.010512 proksee_batch-0.5.9/src/proksee_batch/seq_file_to_cgview_json.py
--rw-r--r--   0        0        0    24047 2024-04-18 15:56:29.010512 proksee_batch-0.5.9/src/proksee_batch/validate_input_data.py
--rw-r--r--   0        0        0     5058 1970-01-01 00:00:00.000000 proksee_batch-0.5.9/PKG-INFO
+-rw-r--r--   0        0        0     1089 2024-05-07 05:12:50.063781 proksee_batch-0.6.0/LICENSE
+-rw-r--r--   0        0        0     3861 2024-05-07 05:12:50.063781 proksee_batch-0.6.0/README.md
+-rw-r--r--   0        0        0     1797 2024-05-07 05:13:00.135968 proksee_batch-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0       21 2024-05-07 05:12:50.067781 proksee_batch-0.6.0/src/proksee_batch/__init__.py
+-rw-r--r--   0        0        0    16864 2024-05-07 05:12:50.067781 proksee_batch-0.6.0/src/proksee_batch/__main__.py
+-rw-r--r--   0        0        0     2330 2024-05-07 05:12:50.067781 proksee_batch-0.6.0/src/proksee_batch/data/assets/images/GitHub-Mark-Light-64px.png
+-rw-r--r--   0        0        0    22591 2024-05-07 05:12:50.067781 proksee_batch-0.6.0/src/proksee_batch/data/assets/scripts/batch.js
+-rw-r--r--   0        0        0   208377 2024-05-07 05:12:50.071781 proksee_batch-0.6.0/src/proksee_batch/data/assets/scripts/cgview.min.js
+-rw-r--r--   0        0        0     1843 2024-05-07 05:12:50.071781 proksee_batch-0.6.0/src/proksee_batch/data/assets/scripts/controls.js
+-rw-r--r--   0        0        0   274269 2024-05-07 05:12:50.071781 proksee_batch-0.6.0/src/proksee_batch/data/assets/scripts/d3.min.js
+-rw-r--r--   0        0        0    61938 2024-05-07 05:12:50.071781 proksee_batch-0.6.0/src/proksee_batch/data/assets/scripts/svgcanvas.iife.js
+-rw-r--r--   0        0        0    14980 2024-05-07 05:12:50.071781 proksee_batch-0.6.0/src/proksee_batch/data/assets/styles/cgview.css
+-rw-r--r--   0        0        0     5696 2024-05-07 05:12:50.071781 proksee_batch-0.6.0/src/proksee_batch/data/assets/styles/controls.css
+-rw-r--r--   0        0        0    12170 2024-05-07 05:12:50.071781 proksee_batch-0.6.0/src/proksee_batch/data/assets/styles/style.css
+-rw-r--r--   0        0        0  8699885 2024-05-07 05:12:50.115782 proksee_batch-0.6.0/src/proksee_batch/data/data.example/genome_maps/genome_1.js
+-rw-r--r--   0        0        0  8356605 2024-05-07 05:12:50.123782 proksee_batch-0.6.0/src/proksee_batch/data/data.example/genome_maps/genome_2.js
+-rw-r--r--   0        0        0  9930491 2024-05-07 05:12:50.155783 proksee_batch-0.6.0/src/proksee_batch/data/data.example/genome_maps/genome_3.js
+-rw-r--r--   0        0        0 12137099 2024-05-07 05:12:50.191784 proksee_batch-0.6.0/src/proksee_batch/data/data.example/genome_maps/genome_4.js
+-rw-r--r--   0        0        0     3874 2024-05-07 05:12:50.191784 proksee_batch-0.6.0/src/proksee_batch/data/data.example/table_data.js
+-rw-r--r--   0        0        0   221376 2024-05-07 05:12:50.191784 proksee_batch-0.6.0/src/proksee_batch/data/default_proksee_template.json
+-rw-r--r--   0        0        0      158 2024-05-07 05:12:50.191784 proksee_batch-0.6.0/src/proksee_batch/data/example_input_dir/Escherichia_coli_str._K-12_substr._MG1655/bed/e_coli_features.bed
+-rw-r--r--   0        0        0      269 2024-05-07 05:12:50.191784 proksee_batch-0.6.0/src/proksee_batch/data/example_input_dir/Escherichia_coli_str._K-12_substr._MG1655/blast/blast_against_e_coli.txt
+-rw-r--r--   0        0        0      180 2024-05-07 05:12:50.195784 proksee_batch-0.6.0/src/proksee_batch/data/example_input_dir/Escherichia_coli_str._K-12_substr._MG1655/vcf/e_coli_variants.vcf
+-rw-r--r--   0        0        0       79 2024-05-07 05:12:50.195784 proksee_batch-0.6.0/src/proksee_batch/data/example_input_dir/Klebsiella_aerogenes/bed/k_aerogenes_features.bed
+-rw-r--r--   0        0        0      134 2024-05-07 05:12:50.195784 proksee_batch-0.6.0/src/proksee_batch/data/example_input_dir/Klebsiella_aerogenes/blast/blast_against_k_aerogenes.txt
+-rw-r--r--   0        0        0       75 2024-05-07 05:12:50.195784 proksee_batch-0.6.0/src/proksee_batch/data/example_input_dir/Salmonella_enterica_subsp._enterica_serovar_Typhimurium_str._LT2/bed/s_enterica_features.bed
+-rw-r--r--   0        0        0      130 2024-05-07 05:12:50.195784 proksee_batch-0.6.0/src/proksee_batch/data/example_input_dir/Salmonella_enterica_subsp._enterica_serovar_Typhimurium_str._LT2/blast/blast_against_s_enterica.txt
+-rw-r--r--   0        0        0       75 2024-05-07 05:12:50.195784 proksee_batch-0.6.0/src/proksee_batch/data/example_input_dir/Shigella_flexneri_2a_str._301/bed/s_flexneri_features.bed
+-rw-r--r--   0        0        0      130 2024-05-07 05:12:50.195784 proksee_batch-0.6.0/src/proksee_batch/data/example_input_dir/Shigella_flexneri_2a_str._301/blast/blast_against_s_flexneri.txt
+-rw-r--r--   0        0        0     5127 2024-05-07 05:12:50.195784 proksee_batch-0.6.0/src/proksee_batch/data/report.html
+-rw-r--r--   0        0        0     6474 2024-05-07 05:12:50.195784 proksee_batch-0.6.0/src/proksee_batch/download_example_input.py
+-rw-r--r--   0        0        0      895 2024-05-07 05:12:50.195784 proksee_batch-0.6.0/src/proksee_batch/generate_proksee_link.py
+-rw-r--r--   0        0        0     5311 2024-05-07 05:12:50.195784 proksee_batch-0.6.0/src/proksee_batch/generate_report_html.py
+-rw-r--r--   0        0        0     1037 2024-05-07 05:12:50.195784 proksee_batch-0.6.0/src/proksee_batch/get_stats_from_seq_file.py
+-rw-r--r--   0        0        0     1952 2024-05-07 05:12:50.195784 proksee_batch-0.6.0/src/proksee_batch/merge_cgview_json_with_template.py
+-rw-r--r--   0        0        0    24085 2024-05-07 05:12:50.195784 proksee_batch-0.6.0/src/proksee_batch/parse_additional_features.py
+-rw-r--r--   0        0        0        0 2024-05-07 05:12:50.195784 proksee_batch-0.6.0/src/proksee_batch/py.typed
+-rw-r--r--   0        0        0     1165 2024-05-07 05:12:50.195784 proksee_batch-0.6.0/src/proksee_batch/remove_covered_features.py
+-rw-r--r--   0        0        0     2658 2024-05-07 05:12:50.195784 proksee_batch-0.6.0/src/proksee_batch/scrape_proksee_image.py
+-rw-r--r--   0        0        0    11471 2024-05-07 05:12:50.195784 proksee_batch-0.6.0/src/proksee_batch/seq_file_to_cgview_json.py
+-rw-r--r--   0        0        0     1927 2024-05-07 05:12:50.195784 proksee_batch-0.6.0/src/proksee_batch/update_legend.py
+-rw-r--r--   0        0        0    26801 2024-05-07 05:12:50.195784 proksee_batch-0.6.0/src/proksee_batch/validate_input_data.py
+-rw-r--r--   0        0        0     5058 1970-01-01 00:00:00.000000 proksee_batch-0.6.0/PKG-INFO
```

### Comparing `proksee_batch-0.5.9/LICENSE` & `proksee_batch-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.5.9/README.md` & `proksee_batch-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.5.9/pyproject.toml` & `proksee_batch-0.6.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "proksee-batch"
-version = "0.5.9"
+version = "0.6.0"
 description = "Proksee Batch"
 authors = ["Lael D. Barlow"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/stothard-group/proksee-batch"
 repository = "https://github.com/stothard-group/proksee-batch"
 documentation = "https://proksee-batch.readthedocs.io"
```

### Comparing `proksee_batch-0.5.9/src/proksee_batch/__main__.py` & `proksee_batch-0.6.0/src/proksee_batch/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 import sys
 from importlib import resources
 from importlib.metadata import version
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Optional
+from typing import Tuple
 
 import click
 import toml
 
 from .download_example_input import download_example_input
 
 # from .generate_proksee_link import generate_proksee_link
@@ -28,14 +29,15 @@
 from .merge_cgview_json_with_template import merge_cgview_json_with_template
 from .parse_additional_features import add_bed_features_and_tracks
 from .parse_additional_features import add_blast_features_and_tracks
 from .parse_additional_features import add_gff_features_and_tracks
 from .parse_additional_features import add_vcf_features_and_tracks
 from .seq_file_to_cgview_json import fasta_to_cgview_json
 from .seq_file_to_cgview_json import genbank_to_cgview_json
+from .update_legend import update_legend
 
 # from .scrape_proksee_image import scrape_proksee_image
 from .validate_input_data import get_data_files
 from .validate_input_data import validate_input_directory_contents
 
 
 @click.command()
@@ -127,24 +129,28 @@
         )
         fasta_paths = get_data_files(os.path.join(input_dir_path, genome_dir), "fasta")
         json_paths = get_data_files(os.path.join(input_dir_path, genome_dir), "json")
         blast_paths = get_data_files(os.path.join(input_dir_path, genome_dir), "blast")
         bed_paths = get_data_files(os.path.join(input_dir_path, genome_dir), "bed")
         vcf_paths = get_data_files(os.path.join(input_dir_path, genome_dir), "vcf")
         gff_paths = get_data_files(os.path.join(input_dir_path, genome_dir), "gff")
+        metadata_paths = get_data_files(
+            os.path.join(input_dir_path, genome_dir), "metadata"
+        )
 
         # Generate a dict with file types as keys and lists of file paths as values.
         file_names_dict = {
             "genbank": [os.path.basename(x) for x in genbank_paths],
             "fasta": [os.path.basename(x) for x in fasta_paths],
             "json": [os.path.basename(x) for x in json_paths],
             "blast": [os.path.basename(x) for x in blast_paths],
             "bed": [os.path.basename(x) for x in bed_paths],
             "vcf": [os.path.basename(x) for x in vcf_paths],
             "gff": [os.path.basename(x) for x in gff_paths],
+            "metadata": [os.path.basename(x) for x in metadata_paths],
         }
 
         # If the genome directory contains one or more GenBank files, remove the
         # list of FASTA files from the dict (because they won't be used).
         if genbank_paths:
             del file_names_dict["fasta"]
 
@@ -159,14 +165,20 @@
                 genbank_accession,
                 genbank_description,
                 genbank_total_size,
                 genbank_number_of_contigs,
                 genbank_gc_content,
             ) = get_stats_from_seq_file(genbank_path, "genbank")
 
+            # If metadata is provided, use it to update the genbank_description
+            # (may be putative species assignment, and evidence, etc., for local
+            # assemblies rather than genbank info)
+            if metadata_paths:
+                genbank_description = get_description_from_metadata(metadata_paths[0])
+
             genome_info.append(
                 {
                     "code_name": genome_code_name,
                     "name": genome_dir,
                     "accession": genbank_accession,
                     "description": genbank_description,
                     "total_size": genbank_total_size,
@@ -321,22 +333,33 @@
                         "dataMethod": "sequence",
                         "dataKeys": "gc-skew",
                     },
                 ]
             )
             json.dump(merged_json, merged_json_file_with_gc_tracks_fh)
 
+        # Update the legend, if necessary.
+        json_data = json.load(open(merged_json_file_with_gc_tracks))
+        json_data_with_updated_legend = update_legend(json_data)
+        json_file_with_updated_legend = os.path.join(
+            temp_output,
+            genome_code_name + ".merged_with_gc_tracks_with_updated_legend.json",
+        )
+        with open(json_file_with_updated_legend, "w") as file:
+            json.dump(json_data_with_updated_legend, file)
+
         # Convert the merged JSON file to .js file by wrapping it in a variable assignment.
         js_file = os.path.join(
             output_path, "data", "genome_maps", genome_code_name + ".js"
         )
         with open(js_file, "w") as file:
             # Get the JSON data from the merged JSON file as a string.
             json_data = None
-            with open(merged_json_file_with_gc_tracks) as json_file:
+            # with open(merged_json_file_with_gc_tracks) as json_file:
+            with open(json_file_with_updated_legend) as json_file:
                 json_data = json_file.read()
             # Write the variable assignment.
             file.write(f"json = {json_data};")
 
         # Generate a .js file with the contents of the genome_info dictionary.
         generate_js_data(output_path, genome_info, run_date, input_dir_path)
 
@@ -374,14 +397,32 @@
     js_content = "const tableData = " + json.dumps(all_info, indent=4) + ";"
 
     # Save the data to a .js file
     with open(output_file, "w") as file:
         file.write(js_content)
 
 
+def get_description_from_metadata(metadata_path: str) -> str:
+    """
+    Extracts the accession and description from a metadata file.
+
+    Args:
+        metadata_path (str): Path to the metadata file.
+
+    Returns:
+        str: The description extracted from the metadata file.
+    """
+    description = ""
+    with open(metadata_path) as metadata_file:
+        metadata = json.load(metadata_file)
+        if "metadata" in metadata and "description" in metadata["metadata"]:
+            description = metadata["metadata"]["description"]
+    return description
+
+
 def handle_error_exit(error_message: str, exit_code: int = 1) -> None:
     """
     Handles errors by printing a message to sys.stderr and exiting the program.
 
     Args:
         error_message (str): The error message to be printed.
         exit_code (int): The exit code to be used for sys.exit. Defaults to 1.
```

### Comparing `proksee_batch-0.5.9/src/proksee_batch/data/assets/images/GitHub-Mark-Light-64px.png` & `proksee_batch-0.6.0/src/proksee_batch/data/assets/images/GitHub-Mark-Light-64px.png`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.5.9/src/proksee_batch/data/assets/scripts/batch.js` & `proksee_batch-0.6.0/src/proksee_batch/data/assets/scripts/batch.js`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.5.9/src/proksee_batch/data/assets/scripts/cgview.min.js` & `proksee_batch-0.6.0/src/proksee_batch/data/assets/scripts/cgview.min.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,31 +1,11 @@
-/*
-   Copyright 2018 Jason R. Grant
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
-
-
-   See the source repository for more information:
-   https://github.com/stothard-group/cgview-js
-*/
 var CGV = function(t, e) {
     "use strict";
 
     function s(t) {
-        if (t && t.__esModule) return t;
         var e = Object.create(null);
         return t && Object.keys(t).forEach((function(s) {
             if ("default" !== s) {
                 var i = Object.getOwnPropertyDescriptor(t, s);
                 Object.defineProperty(e, s, i.get ? i : {
                     enumerable: !0,
                     get: function() {
@@ -4220,15 +4200,15 @@
                 font: this.font.string,
                 color: this.color.rgbString,
                 contigs: this._contigs.map((e => e.toJSON(t)))
             };
             return this.visible && !t.includeDefaults || (e.visible = this.visible), e
         }
     }
-    class D extends c {
+    var D = class extends c {
         constructor(t, e = {}, s = {}) {
             super(t.viewer, e, s), this._sequence = t, this._viewer = t.viewer, this.name = o.defaultFor(e.name, "Unknown"), this.orientation = o.defaultFor(e.orientation, "+"), this.seq = e.seq, this.color = e.color, this._features = new n, this._updateLengthOffset(0), this.seq || (this.length = e.length), this.length || console.error(`Contig '${this.name}'  has no sequence or length set!`)
         }
         static removeFeatures(t) {
             if (0 === (t = n.arrayerize(t)).length) return;
             const e = t[0].viewer,
                 s = {};
@@ -4370,15 +4350,15 @@
                 name: this.name,
                 orientation: this.orientation,
                 length: this.length,
                 color: this.color && this.color.rgbaString
             };
             return this.hasSeq && (e.seq = this.seq), this.visible && !t.includeDefaults || (e.visible = this.visible), e
         }
-    }
+    };
     class $ {
         constructor(t, e = {}) {
             this.viewer = t, this._data = {}, this._sections = o.defaultFor(e.sections, []);
             for (const t of this.sections) this.data[t] = {}
         }
         get sections() {
             return this._sections
@@ -5094,30 +5074,34 @@
             let e = `<div class='track-data'>Map: ${o.commaNumber(t.bp)} bp</div>`;
             if ("contig" === t.elementType) {
                 const s = t.element;
                 e = `<div class='track-data'>Contig: ${o.commaNumber(t.bp-s.lengthOffset)} bp</div>` + e
             }
             return e
         }
+        getMetaDivs(t) {
+            if (!t) return "";
+            let e = "";
+            const s = Object.keys(t);
+            return this.showMetaData && s.length > 0 && (e = s.map((e => `<div class='meta-data'><span class='meta-data-key'>${e}</span>: <span class='meta-data-value'>${t[e]}</span></div>`)).join(""), e = `<div class='meta-data-container'>${e}</div>`), e
+        }
         featurePopoverContentsDefault(t) {
-            const e = t.element,
-                s = Object.keys(e.meta);
-            let i = "";
-            return this.showMetaData && s.length > 0 && (i = s.map((t => `<div class='meta-data'><span class='meta-data-key'>${t}</span>: <span class='meta-data-value'>${e.meta[t]}</span></div>`)).join(""), i = `<div class='meta-data-container'>${i}</div>`), `\n      <div style='margin: 0 5px; font-size: 14px'>\n        <div>${e.type}: ${e.name}<div>\n        <div class='track-data'>Length: ${o.commaNumber(e.length)} bp</div>\n        ${i}\n        ${this.getTrackDiv(t)}\n      </div>\n    `
+            const e = t.element;
+            return `\n      <div style='margin: 0 5px; font-size: 14px'>\n        <div>${e.type}: ${e.name}<div>\n        <div class='track-data'>Length: ${o.commaNumber(e.length)} bp</div>\n        ${this.getMetaDivs(e.meta)}\n        ${this.getTrackDiv(t)}\n      </div>\n    `
         }
         plotPopoverContentsDefault(t) {
             return `\n      <div style='margin: 0 5px; font-size: 14px'>\n        <div>Score: ${t.element.scoreForPosition(t.bp).toFixed(2)}</div>\n        ${this.getTrackDiv(t)}\n      </div>\n    `
         }
         backbonePopoverContentsDefault(t) {
-            return `\n      <div style='margin: 0 5px; font-size: 14px'>\n        <div>Backbone: ${o.commaNumber(this.sequence.length)} bp</div>\n        ${this.getPositionDiv(t)}\n      </div>\n    `
+            return `\n      <div style='margin: 0 5px; font-size: 14px'>\n        <div>Backbone: ${o.commaNumber(this.sequence.length)} bp</div>\n        ${this.getPositionDiv(t)}\n        ${this.getMetaDivs(this.viewer.backbone.meta)}\n      </div>\n    `
         }
         contigPopoverContentsDefault(t) {
             const e = t.element,
                 s = o.commaNumber(e.length);
-            return `\n      <div style='margin: 0 5px; font-size: 14px'>\n        <div>Contig ${e.index}/${this.sequence.contigs().length} [${s} bp]: ${e.name}</div>\n        ${this.getPositionDiv(t)}\n      </div>\n    `
+            return `\n      <div style='margin: 0 5px; font-size: 14px'>\n        <div>Contig ${e.index}/${this.sequence.contigs().length} [${s} bp]: ${e.name}</div>\n        ${this.getPositionDiv(t)}\n        ${this.getMetaDivs(e.meta)}\n      </div>\n    `
         }
         highlightFeature(t) {
             t.element.highlight(t.slot)
         }
         highlightPlot(t) {
             const e = this.viewer,
                 s = t.element,
@@ -5317,15 +5301,15 @@
             return this._minorTickStep
         }
         get tickFormater() {
             return this._tickFormater
         }
         _createTickFormatter(t) {
             let e, s;
-            return t <= 50 ? e = i.formatPrefix(",.0", 1) : t <= 5e4 ? (s = i.precisionPrefix(t, 1e3), e = i.formatPrefix(`.${s}`, 1e3)) : t <= 5e7 && (s = i.precisionPrefix(t, 1e6), e = i.formatPrefix(`.${s}`, 1e6)), e
+            return t <= 50 ? e = i.formatPrefix(",.0", 1) : t <= 5e4 ? (s = i.precisionPrefix(t, 1e3), e = i.formatPrefix(`.${s}`, 1e3)) : t <= 5e7 ? (s = i.precisionPrefix(t, 1e6), e = i.formatPrefix(`.${s}`, 1e6)) : t <= 5e10 && (s = i.precisionPrefix(t, 1e9), e = i.formatPrefix(`.${s}`, 1e9)), e
         }
         _updateTicks(t, e) {
             const s = this.sequence.length;
             let r = 0,
                 n = 0,
                 o = [],
                 a = 0,
@@ -5884,15 +5868,14 @@
                 i = {
                     cgview: {
                         version: r,
                         created: s.created || this.formatDate(new Date),
                         updated: this.formatDate(new Date),
                         id: e.id,
                         name: e.name,
-                        format: e.format,
                         settings: e.settings.toJSON(t),
                         backbone: e.backbone.toJSON(t),
                         ruler: e.ruler.toJSON(t),
                         annotation: e.annotation.toJSON(t),
                         dividers: e.dividers.toJSON(t),
                         highlighter: e.highlighter.toJSON(t),
                         captions: [],
@@ -5933,17 +5916,17 @@
             const s = this._viewer;
             s.clear("all"), s._objects = {}, s.trigger("cgv-json-load", e), s.update({
                 id: e.id,
                 name: e.name
             }), s._jsonInfo = {
                 version: e.version,
                 created: e.created
-            }, s._features = new n, s._tracks = new n, s._plots = new n, s._captions = new n, s._bookmarks = new n, s._loading = !0, s._sequence = new j(s, e.sequence), s._settings = new J(s, e.settings), s._ruler = new Y(s, e.ruler), s._backbone = new S(s, e.backbone), s._annotation = new k(s, e.annotation), s._dividers = new z(s, e.dividers), s._highlighter = new H(s, e.highlighter), e.bookmarks && s.addBookmarks(e.bookmarks), e.captions && s.addCaptions(e.captions), s._legend = new Q(s, e.legend), e.features && s.addFeatures(e.features), e.plots && s.addPlots(e.plots), e.tracks && s.addTracks(e.tracks), e.meta && (s.meta = e.meta), s.annotation.refresh(), s._loading = !1, s.update({
+            }, s._features = new n, s._tracks = new n, s._plots = new n, s._captions = new n, s._bookmarks = new n, s._loading = !0, s._sequence = new j(s, e.sequence), s.format = o.defaultFor(e.format, "circular"), s._settings = new J(s, e.settings), s._ruler = new Y(s, e.ruler), s._backbone = new S(s, e.backbone), s._annotation = new k(s, e.annotation), s._dividers = new z(s, e.dividers), s._highlighter = new H(s, e.highlighter), e.bookmarks && s.addBookmarks(e.bookmarks), e.captions && s.addCaptions(e.captions), s._legend = new Q(s, e.legend), e.features && s.addFeatures(e.features), e.plots && s.addPlots(e.plots), e.tracks && s.addTracks(e.tracks), e.meta && (s.meta = e.meta), s.annotation.refresh(), s._loading = !1, s.update({
                 dataHasChanged: !1
-            }), s.format = o.defaultFor(e.format, "circular"), s.zoomTo(0, 1, {
+            }), s.zoomTo(0, 1, {
                 duration: 0
             })
         }
         updateJSON(t) {
             if (!(t = t && t.cgview)) throw new Error("No 'cgview' property found in JSON.");
 
             function e(t) {
@@ -6580,15 +6563,15 @@
             let n = this._nonSlotSpace("outside"),
                 o = this._nonSlotSpace("inside");
             this.visibleSlots().each(((t, e) => {
                 e.proportionOfMap = e.thicknessRatio / r;
                 const s = i * e.proportionOfMap;
                 e.inside ? o += s : n += s
             })), this._updateSlotProportionStats(e), this.updateInitialBackboneCenterOffset(o, n), this._calculateMaxMapThickness(), this.updateLayout(!0), t.zoomFactor > 2 && t.moveTo(void 0, void 0, {
-                duration: 0
+                duration: 500
             })
         }
         _calculateMaxMapThickness() {
             const t = this.viewer,
                 e = t.zoomFactor;
             t._zoomFactor = 1, this.updateLayout(!0), this.bbOutsideOffset, this.bbInsideOffset;
             let s = 0;
@@ -7435,15 +7418,15 @@
             const s = t => {
                 t.shiftKey && console.log(t)
             };
             this._wrapper.on("mouseover", (() => {
                 this.shiftSet || (document.addEventListener("keydown", s), this.shiftSet = !0)
             })).on("mouseout", (() => {
                 this.shiftSet && (document.removeEventListener("keydown", s), this.shiftSet = !1)
-            })), this._loading = !1, this.draw()
+            })), this._loading = !1, this.resize(), this.draw()
         }
         static get debugSections() {
             return ["time", "zoom", "position", "n"]
         }
         get version() {
             return r
         }
@@ -8058,11 +8041,9 @@
                 }
                 this.update({
                     dataHasChanged: !0
                 })
             }
         }
     }
-    return t.Anchor = h, t.Annotation = k, t.Backbone = S, t.Bookmark = F, t.Box = C, t.CGArray = n, t.CGObject = c, t.CGRange = M, t.Canvas = P, t.Caption = L, t.CodonTable = T, t.CodonTables = O, t.Color = y, t.ColorPicker = I, t.Contig = D, t.Debug = $, t.Divider = E, t.Dividers = z, t.EventMonitor = G, t.Events = f, t.Feature = V, t.Font = _, t.Highlighter = H, t.HighlighterElement = K, t.IO = X, t.Label = W, t.Layout = et, t.LayoutCircular = Z, t.LayoutLinear = tt, t.Legend = Q, t.LegendItem = U, t.Messenger = st, t.NCList = x, t.Plot = it, t.Position = a, t.Rect = d, t.Ruler = Y, t.Sequence = j, t.SequenceExtractor = q, t.Settings = J, t.Slot = rt, t.Track = nt, t.Viewer = ot, t.utils = o, t.version = r, Object.defineProperty(t, "__esModule", {
-        value: !0
-    }), t
+    return t.Anchor = h, t.Annotation = k, t.Backbone = S, t.Bookmark = F, t.Box = C, t.CGArray = n, t.CGObject = c, t.CGRange = M, t.Canvas = P, t.Caption = L, t.CodonTable = T, t.CodonTables = O, t.Color = y, t.ColorPicker = I, t.Contig = D, t.Debug = $, t.Divider = E, t.Dividers = z, t.EventMonitor = G, t.Events = f, t.Feature = V, t.Font = _, t.Highlighter = H, t.HighlighterElement = K, t.IO = X, t.Label = W, t.Layout = et, t.LayoutCircular = Z, t.LayoutLinear = tt, t.Legend = Q, t.LegendItem = U, t.Messenger = st, t.NCList = x, t.Plot = it, t.Position = a, t.Rect = d, t.Ruler = Y, t.Sequence = j, t.SequenceExtractor = q, t.Settings = J, t.Slot = rt, t.Track = nt, t.Viewer = ot, t.utils = o, t.version = r, t
 }({}, d3);
```

### Comparing `proksee_batch-0.5.9/src/proksee_batch/data/assets/scripts/controls.js` & `proksee_batch-0.6.0/src/proksee_batch/data/assets/scripts/controls.js`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.5.9/src/proksee_batch/data/assets/scripts/d3.min.js` & `proksee_batch-0.6.0/src/proksee_batch/data/assets/scripts/d3.min.js`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.5.9/src/proksee_batch/data/assets/scripts/svgcanvas.iife.js` & `proksee_batch-0.6.0/src/proksee_batch/data/assets/scripts/svgcanvas.iife.js`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.5.9/src/proksee_batch/data/assets/styles/cgview.css` & `proksee_batch-0.6.0/src/proksee_batch/data/assets/styles/cgview.css`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.5.9/src/proksee_batch/data/assets/styles/controls.css` & `proksee_batch-0.6.0/src/proksee_batch/data/assets/styles/controls.css`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.5.9/src/proksee_batch/data/assets/styles/style.css` & `proksee_batch-0.6.0/src/proksee_batch/data/assets/styles/style.css`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.5.9/src/proksee_batch/data/data.example/table_data.js` & `proksee_batch-0.6.0/src/proksee_batch/data/data.example/table_data.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 const tableData = {
-    "proksee-batch_version": "0.5.1",
-    "run_date": "2024-03-11 20:12:32 UTC",
-    "input_dir": "/path/to/example_data",
+    "proksee-batch_version": "0.0.1a1",
+    "run_date": "2024-05-07 02:57:01 UTC",
+    "input_dir": "/Users/laelbarlow/Documents/Projects_current/Read_searching_projects/231218_proksee-batch/tests/example_input_dir6",
     "genomes": [{
         "code_name": "genome_1",
         "name": "Shigella_flexneri_2a_str._301",
         "accession": "NC_004337.2",
         "description": "Shigella flexneri 2a str. 301 chromosome, complete genome",
         "total_size": 4828820,
         "num_contigs": 2,
@@ -20,15 +20,16 @@
             ],
             "bed": [
                 "s_flexneri_features.bed"
             ],
             "vcf": [],
             "gff": [
                 "GCF_000006925.2_ASM692v2_genomic.gff"
-            ]
+            ],
+            "metadata": []
         }
     }, {
         "code_name": "genome_2",
         "name": "Escherichia_coli_str._K-12_substr._MG1655",
         "accession": "NC_000913.3",
         "description": "Escherichia coli str. K-12 substr. MG1655, complete genome",
         "total_size": 4641652,
@@ -46,21 +47,22 @@
                 "e_coli_features.bed"
             ],
             "vcf": [
                 "e_coli_variants.vcf"
             ],
             "gff": [
                 "GCF_000005845.2_ASM584v2_genomic.gff"
-            ]
+            ],
+            "metadata": []
         }
     }, {
         "code_name": "genome_3",
         "name": "Klebsiella_aerogenes",
         "accession": "NZ_CP041925.1",
-        "description": "Klebsiella aerogenes strain Ka37751 chromosome, complete genome",
+        "description": "Custom description here (not from GenBank file).",
         "total_size": 5249267,
         "num_contigs": 2,
         "gc_content": 0.5491,
         "files": {
             "genbank": [
                 "GCF_007632255.1_ASM763225v1_genomic.gbff"
             ],
@@ -70,14 +72,17 @@
             ],
             "bed": [
                 "k_aerogenes_features.bed"
             ],
             "vcf": [],
             "gff": [
                 "GCF_007632255.1_ASM763225v1_genomic.gff"
+            ],
+            "metadata": [
+                "example_metadata.json"
             ]
         }
     }, {
         "code_name": "genome_4",
         "name": "Salmonella_enterica_subsp._enterica_serovar_Typhimurium_str._LT2",
         "accession": "NC_003197.2",
         "description": "Salmonella enterica subsp. enterica serovar Typhimurium str. LT2, complete genome",
@@ -94,11 +99,12 @@
             ],
             "bed": [
                 "s_enterica_features.bed"
             ],
             "vcf": [],
             "gff": [
                 "GCF_000006945.2_ASM694v2_genomic.gff"
-            ]
+            ],
+            "metadata": []
         }
     }]
 };
```

### Comparing `proksee_batch-0.5.9/src/proksee_batch/data/default_proksee_template.json` & `proksee_batch-0.6.0/src/proksee_batch/data/default_proksee_template.json`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.5.9/src/proksee_batch/data/report.html` & `proksee_batch-0.6.0/src/proksee_batch/data/report.html`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.5.9/src/proksee_batch/download_example_input.py` & `proksee_batch-0.6.0/src/proksee_batch/download_example_input.py`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.5.9/src/proksee_batch/generate_proksee_link.py` & `proksee_batch-0.6.0/src/proksee_batch/generate_proksee_link.py`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.5.9/src/proksee_batch/generate_report_html.py` & `proksee_batch-0.6.0/src/proksee_batch/generate_report_html.py`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.5.9/src/proksee_batch/get_stats_from_seq_file.py` & `proksee_batch-0.6.0/src/proksee_batch/get_stats_from_seq_file.py`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.5.9/src/proksee_batch/merge_cgview_json_with_template.py` & `proksee_batch-0.6.0/src/proksee_batch/merge_cgview_json_with_template.py`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.5.9/src/proksee_batch/parse_additional_features.py` & `proksee_batch-0.6.0/src/proksee_batch/parse_additional_features.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     blast_files (list): A list of paths to BLAST result files.
 
     Returns:
     tuple: A tuple containing a list of parsed BLAST features and a list of parsed BLAST tracks.
     """
     blast_features = []
     blast_tracks = []
+    file_specific_blast_features = []
     for i, blast_file in enumerate(blast_files):
         num = i + 1
 
         # Define the BLAST track.
         blast_track = {
             "name": os.path.basename(blast_file),
             "separateFeaturesBy": "none",
@@ -43,73 +44,94 @@
 
         # Parse the BLAST result file.
         with open(blast_file) as f:
             blast_results = f.readlines()
         # Parse the BLAST result file.
         for blast_result_line in blast_results:
             # Parse the BLAST result line.
-            blast_result = blast_result_line.split("\t")
+            blast_result = blast_result_line.strip().split("\t")
 
-            # Skip the header line(s), if present.
-            if blast_result[0] == "qseqid" or blast_result[0].startswith("#"):
+            # Skip the header line(s), or blank lines, if present.
+            if (
+                blast_result[0] == "qseqid"
+                or blast_result[0].startswith("#")
+                or blast_result[0].startswith("\n")
+            ):
                 continue
 
             # Define the BLAST feature.
             blast_feature = {
-                "name": blast_result[
+                "name": [
+                    blast_result[1] if len(blast_result[1]) <= 20 else "blast_hit"
+                ][
                     0
-                ],  # Here we assume that the query sequence is a sequence aligned to a contig in the genome/map.
+                ],  # "blast_hit" if the name is too long
                 "type": "blast",
                 "start": int(
-                    blast_result[8]
+                    # blast_result[8]
+                    min([int(blast_result[6]), int(blast_result[7])])
                 ),  # Here we assume that the subject sequence is a contig in the genome/map.
                 "stop": int(
-                    blast_result[9]
+                    # blast_result[9]
+                    max([int(blast_result[6]), int(blast_result[7])])
                 ),  # Here we assume that the subject sequence is a contig in the genome/map.
-                "strand": 1 if blast_result[8] < blast_result[9] else -1,
+                # "strand": 1 if blast_result[8] < blast_result[9] else -1,
+                "strand": ".",
                 "source": f"blast_{num}",
                 "contig": blast_result[
-                    1
+                    0
                 ],  # Here we assume that the subject sequence is a contig in the genome/map.
                 "legend": os.path.basename(blast_file),
                 "tags": [],
                 "meta": {
+                    "query": blast_result[0],
+                    "query_start": int(blast_result[6]),
+                    "query_stop": int(blast_result[7]),
+                    "subject": blast_result[1],
+                    "subject_start": int(blast_result[8]),
+                    "subject_stop": int(blast_result[9]),
+                    "alignment_length": int(blast_result[3]),
                     "identity": float(blast_result[2]),
                     "mismatches": int(blast_result[4]),
                     "evalue": float(blast_result[10]),
-                    "bit_score": int(blast_result[11]),
+                    "bit_score": float(blast_result[11]),
                 },
             }
             # Add the BLAST feature to the list of BLAST features.
-            blast_features.append(blast_feature)
+            file_specific_blast_features.append(blast_feature)
 
-    # Remove BLAST features that are completely covered by another BLAST feature
-    # with an equal or higher score.
-    blast_features = [
-        blast_feature
-        for blast_feature, is_not_covered in zip(
-            blast_features,
-            remove_covered_features(
-                get_feature_locations_and_scores_from_blast_features(blast_features)
-            ),
-        )
-        if is_not_covered
-    ]
+        # Remove BLAST features that are completely covered by another BLAST feature
+        # with an equal or higher score.
+        file_specific_blast_features = [
+            blast_feature
+            for blast_feature, is_not_covered in zip(
+                file_specific_blast_features,
+                remove_covered_features(
+                    get_feature_locations_and_scores_from_blast_features(
+                        file_specific_blast_features
+                    )
+                ),
+            )
+            if is_not_covered
+        ]
+
+        # Add the file-specific BLAST features to the list of BLAST features.
+        blast_features += file_specific_blast_features
 
     assert (
         len(blast_features) > 0 and len(blast_tracks) > 0
-    ), "No BLAST features or tracks were obtained from input file {}.".format(
+    ), "No BLAST features or tracks were obtained from input file {}. Please check that the query sequences are sequences (contigs, chromosomes, etc.) of the genome being mapped.".format(
         blast_file
     )
     return (blast_features, blast_tracks)
 
 
 def get_feature_locations_and_scores_from_blast_features(
     blast_features: List[Dict[str, Any]]
-) -> List[Tuple[int, int, int]]:
+) -> List[Tuple[int, int, float]]:
     """
     Gets feature locations and scores from BLAST features.
 
     Parameters:
     blast_features (list): A list of parsed BLAST features.
 
     Returns:
@@ -176,14 +198,15 @@
     bed_files (list): A list of paths to BED files.
 
     Returns:
     tuple: A tuple containing a list of parsed BED features and a list of parsed BED tracks.
     """
     bed_features = []
     bed_tracks = []
+    file_specific_bed_features = []
     for i, bed_file in enumerate(bed_files):
         num = i + 1
 
         # Define the BED track.
         bed_track = {
             "name": os.path.basename(bed_file),
             "separateFeaturesBy": "none",
@@ -216,17 +239,17 @@
             assert (
                 len(bed_result) >= 3
             ), f"BED file {bed_file} is not in the correct format."
 
             name = ""
             if len(bed_result) >= 4:
                 name = bed_result[3]
-            score = 0
+            score = 0.0
             if len(bed_result) >= 5:
-                score = int(bed_result[4])
+                score = float(bed_result[4])
             strand = 1
             if len(bed_result) >= 6:
                 if bed_result[5] == "+":
                     strand = 1
                 elif bed_result[5] == "-":
                     strand = -1
                 else:
@@ -248,38 +271,43 @@
                 "legend": os.path.basename(bed_file),
                 "tags": [],
                 "meta": {
                     "score": score,
                 },
             }
             # Add the BED feature to the list of BED features.
-            bed_features.append(bed_feature)
+            file_specific_bed_features.append(bed_feature)
 
-    # Remove BED features that are completely covered by another BED feature
-    # with an equal or higher score.
-    bed_features = [
-        bed_feature
-        for bed_feature, is_not_covered in zip(
-            bed_features,
-            remove_covered_features(
-                get_feature_locations_and_scores_from_bed_features(bed_features)
-            ),
-        )
-        if is_not_covered
-    ]
+        # Remove BED features that are completely covered by another BED feature
+        # with an equal or higher score.
+        file_specific_bed_features = [
+            bed_feature
+            for bed_feature, is_not_covered in zip(
+                file_specific_bed_features,
+                remove_covered_features(
+                    get_feature_locations_and_scores_from_bed_features(
+                        file_specific_bed_features
+                    )
+                ),
+            )
+            if is_not_covered
+        ]
+
+        # Add the file-specific BED features to the list of BED features.
+        bed_features += file_specific_bed_features
 
     assert (
         len(bed_features) > 0 and len(bed_tracks) > 0
     ), f"No BED features or tracks were obtained from input file {bed_file}."
     return (bed_features, bed_tracks)
 
 
 def get_feature_locations_and_scores_from_bed_features(
     bed_features: List[Dict[str, Any]]
-) -> List[Tuple[int, int, int]]:
+) -> List[Tuple[int, int, float]]:
     """
     Gets feature locations and scores from BED features.
 
     Parameters:
     bed_features (list): A list of parsed BED features.
 
     Returns:
@@ -346,14 +374,15 @@
     vcf_files (list): A list of paths to VCF files.
 
     Returns:
     tuple: A tuple containing a list of parsed VCF features and a list of parsed VCF tracks.
     """
     vcf_features = []
     vcf_tracks = []
+    file_specific_vcf_features = []
     for i, vcf_file in enumerate(vcf_files):
         num = i + 1
 
         # Define the VCF track.
         vcf_track = {
             "name": os.path.basename(vcf_file),
             "separateFeaturesBy": "none",
@@ -403,38 +432,43 @@
                 "meta": {
                     "ref": vcf_result[3],
                     "alt": vcf_result[4],
                 },
             }
 
             # Add the VCF feature to the list of VCF features.
-            vcf_features.append(vcf_feature)
+            file_specific_vcf_features.append(vcf_feature)
 
-    # Remove VCF features that are completely covered by another VCF feature
-    # with an equal or higher score.
-    vcf_features = [
-        vcf_feature
-        for vcf_feature, is_not_covered in zip(
-            vcf_features,
-            remove_covered_features(
-                get_feature_locations_and_scores_from_vcf_features(vcf_features)
-            ),
-        )
-        if is_not_covered
-    ]
+        # Remove VCF features that are completely covered by another VCF feature
+        # with an equal or higher score.
+        file_specific_vcf_features = [
+            vcf_feature
+            for vcf_feature, is_not_covered in zip(
+                file_specific_vcf_features,
+                remove_covered_features(
+                    get_feature_locations_and_scores_from_vcf_features(
+                        file_specific_vcf_features
+                    )
+                ),
+            )
+            if is_not_covered
+        ]
+
+        # Add the file-specific VCF features to the list of VCF features.
+        vcf_features += file_specific_vcf_features
 
     assert (
         len(vcf_features) > 0 and len(vcf_tracks) > 0
     ), f"No VCF features or tracks were obtained from input file {vcf_file}."
     return (vcf_features, vcf_tracks)
 
 
 def get_feature_locations_and_scores_from_vcf_features(
     vcf_features: List[Dict[str, Any]]
-) -> List[Tuple[int, int, int]]:
+) -> List[Tuple[int, int, float]]:
     """
     Gets feature locations and scores from VCF features.
 
     Parameters:
     vcf_features (list): A list of parsed VCF features.
 
     Returns:
@@ -442,15 +476,15 @@
     """
     feature_locations_and_scores = []
     for vcf_feature in vcf_features:
         feature_locations_and_scores.append(
             (
                 vcf_feature["start"],
                 vcf_feature["stop"],
-                1,
+                1.0,
             )
         )
     return feature_locations_and_scores
 
 
 def add_vcf_features_and_tracks(
     vcf_files: List[str], json_file: str, output_file: str
@@ -502,14 +536,15 @@
     gff_files (list): A list of paths to GFF files.
 
     Returns:
     tuple: A tuple containing a list of parsed GFF features and a list of parsed GFF tracks.
     """
     gff_features = []
     gff_tracks = []
+    file_specific_gff_features = []
     for i, gff_file in enumerate(gff_files):
         num = i + 1
 
         # Define the GFF track.
         gff_track = {
             "name": os.path.basename(gff_file),
             "separateFeaturesBy": "none",
@@ -555,47 +590,53 @@
                 "stop": gff_result.stop,
                 "strand": gff_result.strand,
                 "source": f"gff_{num}",
                 "contig": gff_result.seqid,
                 "legend": os.path.basename(gff_file),
                 "tags": [],
                 "meta": {
-                    "score": "0",
+                    "score": 0.0,
                 },
             }
 
             # Add any additional metadata, if present.
             for attribute in gff_result.attributes:
-                gff_feature["meta"][attribute] = gff_result.attributes[attribute][0]
+                if len(gff_result.attributes[attribute]) > 0:
+                    gff_feature["meta"][attribute] = gff_result.attributes[attribute][0]
 
             # Add the GFF feature to the list of GFF features.
-            gff_features.append(gff_feature)
+            file_specific_gff_features.append(gff_feature)
 
-    # Remove GFF features that are completely covered by another GFF feature
-    # with an equal or higher score.
-    gff_features = [
-        gff_feature
-        for gff_feature, is_not_covered in zip(
-            gff_features,
-            remove_covered_features(
-                get_feature_locations_and_scores_from_gff_features(gff_features)
-            ),
-        )
-        if is_not_covered
-    ]
+        # Remove GFF features that are completely covered by another GFF feature
+        # with an equal or higher score.
+        file_specific_gff_features = [
+            gff_feature
+            for gff_feature, is_not_covered in zip(
+                file_specific_gff_features,
+                remove_covered_features(
+                    get_feature_locations_and_scores_from_gff_features(
+                        file_specific_gff_features
+                    )
+                ),
+            )
+            if is_not_covered
+        ]
+
+        # Add the file-specific GFF features to the list of GFF features.
+        gff_features += file_specific_gff_features
 
     assert (
         len(gff_features) > 0 and len(gff_tracks) > 0
     ), f"No GFF features or tracks were obtained from input file {gff_file}."
     return (gff_features, gff_tracks)
 
 
 def get_feature_locations_and_scores_from_gff_features(
     gff_features: List[Dict[str, Any]]
-) -> List[Tuple[int, int, int]]:
+) -> List[Tuple[int, int, float]]:
     """
     Gets feature locations and scores from GFF features.
 
     Parameters:
     gff_features (list): A list of parsed GFF features.
 
     Returns:
@@ -641,12 +682,14 @@
         assert (
             gff_feature["contig"] in contigs
         ), "The contig {} listed in the GFF file {} is not among the contigs in the genome being mapped.".format(
             gff_feature["contig"], gff_feature["legend"]
         )
 
     # Add the parsed GFF features and tracks to the cgview map JSON data structure.
+    for gff_feature in gff_features:
+        assert gff_feature not in json_data["cgview"]["features"]
     json_data["cgview"]["features"] += gff_features
     json_data["cgview"]["tracks"] += gff_tracks
     # Write the cgview map JSON data structure to a new file.
     with open(output_file, "w") as f:
         json.dump(json_data, f, indent=4)
```

### Comparing `proksee_batch-0.5.9/src/proksee_batch/remove_covered_features.py` & `proksee_batch-0.6.0/src/proksee_batch/remove_covered_features.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import List
 from typing import Tuple
 
 
-def remove_covered_features(features: List[Tuple[int, int, int]]) -> List[bool]:
+def remove_covered_features(features: List[Tuple[int, int, float]]) -> List[bool]:
     """
     Identifies features that are completely covered by another feature with an
     equal or higher score.
 
     Parameters:
     features (list of tuples): A list of tuples, each containing a start position,
                                an end position, and a score.
```

### Comparing `proksee_batch-0.5.9/src/proksee_batch/scrape_proksee_image.py` & `proksee_batch-0.6.0/src/proksee_batch/scrape_proksee_image.py`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.5.9/src/proksee_batch/seq_file_to_cgview_json.py` & `proksee_batch-0.6.0/src/proksee_batch/seq_file_to_cgview_json.py`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.5.9/src/proksee_batch/validate_input_data.py` & `proksee_batch-0.6.0/src/proksee_batch/validate_input_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -96,16 +96,19 @@
             "genbank",
             "fasta",
             "blast",
             "bed",
             "json",
             "vcf",
             "gff",
+            "metadata",
         ]
         for subdirectory in os.listdir(os.path.join(input, genome_dir)):
+            if subdirectory.startswith("."):
+                continue
             if subdirectory not in valid_subdirectories:
                 handle_error_exit(
                     f"The input directory contains an invalid subdirectory: {subdirectory}"
                 )
 
         # Check the contents of the subdirectories, if they exist.
         seq_file_path = ""
@@ -183,20 +186,21 @@
                 elif subdirectory == "blast":
                     blast_result_files = []
                     for file in os.listdir(subdirectory_path):
                         if file.endswith(".txt") or file.endswith(".tsv"):
                             blast_result_files.append(file)
                             # Validate the BLAST result file. It should be in tabular format (outfmt 6).
                             with open(os.path.join(subdirectory_path, file)) as f:
-                                for line in f:
-                                    if not line.startswith("#"):
+                                # for line in f:
+                                for i, line in enumerate(f):
+                                    if not line.startswith("#") and line.strip() != "":
                                         line_split = line.split("\t")
                                         if len(line_split) != 12:
                                             handle_error_exit(
-                                                f"The BLAST result file {file} does not have the correct number of columns. Please check that the file is in tabular format (outfmt 6)."
+                                                f"The BLAST result file {file} does not have the correct number of columns at line {i+1}. Please check that the file is in tabular format (outfmt 6)."
                                             )
                                         try:
                                             float(line_split[2])
                                             float(line_split[3])
                                             float(line_split[10])
                                             float(line_split[11])
                                         except ValueError:
@@ -327,14 +331,51 @@
                                             handle_error_exit(
                                                 f"The GFF file {file} does not have the correct format. Please check that the file is in GFF format."
                                             )
                     if len(gff_files) == 0:
                         handle_error_exit(
                             f"The input directory {subdirectory_path} does not contain any GFF files. Valid file extensions are .gff and .gff3."
                         )
+                elif subdirectory == "metadata":
+                    # Check that there is one and only one metadata file in the metadata directory, with a filename extension .json.
+                    metadata_files = [
+                        file
+                        for file in os.listdir(subdirectory_path)
+                        if file.endswith(".json")
+                    ]
+                    if len(metadata_files) == 0:
+                        handle_error_exit(
+                            f"The input directory {subdirectory_path} does not contain any metadata files. Valid file extension is .json."
+                        )
+                    elif len(metadata_files) > 1:
+                        handle_error_exit(
+                            f"The input directory {subdirectory_path} contains more than one metadata file. Please ensure that there is exactly one metadata file in the directory."
+                        )
+                    # Parse the metadata file with json.load to check if the file format is valid.
+                    with open(os.path.join(subdirectory_path, metadata_files[0])) as f:
+                        try:
+                            metadata = json.load(f)
+                        except Exception as e:
+                            handle_error_exit(
+                                f"Error parsing the metadata file {metadata_files[0]}: {e}. Please check that the file is in JSON format."
+                            )
+                        # Check that the metadata file contains the required keys.
+                        required_metadata_keys = {"metadata": {"description": None}}
+                        metadata_file = metadata_files[0]
+
+                        for main_key, sub_keys in required_metadata_keys.items():
+                            if main_key not in metadata:
+                                handle_error_exit(
+                                    f"{metadata_file} is missing the required key: {main_key}"
+                                )
+                            for sub_key in sub_keys:
+                                if sub_key not in metadata[main_key]:
+                                    handle_error_exit(
+                                        f"{metadata_file} is missing the required sub-key: {main_key}.{sub_key}"
+                                    )
 
 
 def get_data_files(input_subdir: str, data_type: str) -> List[str]:
     """
     Returns the paths to the data files of the specified type in the provided subdirectory.
 
     Args:
@@ -396,14 +437,20 @@
             ]
         elif data_type == "gff":
             return [
                 os.path.join(data_dir, file)
                 for file in os.listdir(data_dir)
                 if file.endswith(".gff") or file.endswith(".gff3")
             ]
+        elif data_type == "metadata":
+            return [
+                os.path.join(data_dir, file)
+                for file in os.listdir(data_dir)
+                if file.endswith(".json")
+            ]
         else:
             handle_error_exit(f"Invalid data type: {data_type}")
     return []
 
 
 def handle_error_exit(error_message: str, exit_code: int = 1) -> None:
     """
```

### Comparing `proksee_batch-0.5.9/PKG-INFO` & `proksee_batch-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proksee-batch
-Version: 0.5.9
+Version: 0.6.0
 Summary: Proksee Batch
 Home-page: https://github.com/stothard-group/proksee-batch
 License: MIT
 Author: Lael D. Barlow
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

