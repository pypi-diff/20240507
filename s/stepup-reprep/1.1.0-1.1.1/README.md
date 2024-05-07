# Comparing `tmp/stepup_reprep-1.1.0.tar.gz` & `tmp/stepup_reprep-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stepup_reprep-1.1.0.tar", last modified: Thu May  2 09:38:23 2024, max compression
+gzip compressed data, was "stepup_reprep-1.1.1.tar", last modified: Tue May  7 17:50:13 2024, max compression
```

## Comparing `stepup_reprep-1.1.0.tar` & `stepup_reprep-1.1.1.tar`

### file list

```diff
@@ -1,333 +1,366 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:23.020955 stepup_reprep-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:22.968955 stepup_reprep-1.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:22.972955 stepup_reprep-1.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/.github/workflows/mkdocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/.github/workflows/pytest.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-05-02 09:38:23.020955 stepup_reprep-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:22.972955 stepup_reprep-1.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/docs/clean_stdout.sed
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/docs/development.md
--rw-r--r--   0 runner    (1001) docker     (127)     4140 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/docs/license.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:22.976955 stepup_reprep-1.1.0/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/docs/reference/stepup.reprep.api.md
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/docs/reference/stepup.reprep.tile_pdf.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:22.976955 stepup_reprep-1.1.0/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)     4171 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/docs/tutorials/before_you_begin.md
--rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/docs/tutorials/create_or_clone_a_project.md
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/docs/tutorials/manifest_files.md
--rw-r--r--   0 runner    (1001) docker     (127)     6754 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/docs/tutorials/template_conventions.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:22.976955 stepup_reprep-1.1.0/docs/tutorials/tiling_pdfs/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/docs/tutorials/tiling_pdfs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    22692 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/docs/tutorials/tiling_pdfs/figure.png
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/docs/tutorials/tiling_pdfs/hexagon.svg
--rwxr-xr-x   0 runner    (1001) docker     (127)      114 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/docs/tutorials/tiling_pdfs/main.sh
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/docs/tutorials/tiling_pdfs/pentagon.svg
--rwxr-xr-x   0 runner    (1001) docker     (127)      278 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/docs/tutorials/tiling_pdfs/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/docs/tutorials/tiling_pdfs/square.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/docs/tutorials/tiling_pdfs/stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      413 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/docs/tutorials/tiling_pdfs/tile.py
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/docs/tutorials/tiling_pdfs/triangle.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/docs/tutorials/tiling_pdfs.md
--rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/docs/tutorials/working_on_a_project.md
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 09:38:23.020955 stepup_reprep-1.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:22.968955 stepup_reprep-1.1.0/stepup/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:22.980955 stepup_reprep-1.1.0/stepup/reprep/
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/stepup/reprep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-02 09:38:22.000000 stepup_reprep-1.1.0/stepup/reprep/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/stepup/reprep/add_notes_pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)    25206 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/stepup/reprep/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/stepup/reprep/bibtex_log.py
--rw-r--r--   0 runner    (1001) docker     (127)     5286 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/stepup/reprep/check_hrefs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/stepup/reprep/check_manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4426 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/stepup/reprep/convert_inkscape.py
--rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/stepup/reprep/convert_markdown.py
--rw-r--r--   0 runner    (1001) docker     (127)     7521 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/stepup/reprep/latex.py
--rw-r--r--   0 runner    (1001) docker     (127)     4783 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/stepup/reprep/latex_deps.py
--rw-r--r--   0 runner    (1001) docker     (127)     7040 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/stepup/reprep/latex_flat.py
--rw-r--r--   0 runner    (1001) docker     (127)     5575 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/stepup/reprep/latex_log.py
--rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/stepup/reprep/make_manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/stepup/reprep/normalize_pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/stepup/reprep/nup_pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/stepup/reprep/pytest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/stepup/reprep/raster_pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     5081 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/stepup/reprep/render.py
--rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/stepup/reprep/tile_pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4415 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/stepup/reprep/zip_manifest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:23.016955 stepup_reprep-1.1.0/stepup_reprep.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-05-02 09:38:22.000000 stepup_reprep-1.1.0/stepup_reprep.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10550 2024-05-02 09:38:22.000000 stepup_reprep-1.1.0/stepup_reprep.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 09:38:22.000000 stepup_reprep-1.1.0/stepup_reprep.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-02 09:38:22.000000 stepup_reprep-1.1.0/stepup_reprep.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-02 09:38:22.000000 stepup_reprep-1.1.0/stepup_reprep.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 09:38:22.000000 stepup_reprep-1.1.0/stepup_reprep.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:22.984955 stepup_reprep-1.1.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:22.972955 stepup_reprep-1.1.0/tests/cases/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:22.984955 stepup_reprep-1.1.0/tests/cases/add_notes_pdf/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/add_notes_pdf/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/add_notes_pdf/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/add_notes_pdf/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/add_notes_pdf/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      955 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/add_notes_pdf/main.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/add_notes_pdf/notes.pdf
--rwxr-xr-x   0 runner    (1001) docker     (127)      182 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/add_notes_pdf/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     8616 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/add_notes_pdf/src.pdf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:22.984955 stepup_reprep-1.1.0/tests/cases/cat_pdf/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/cat_pdf/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/cat_pdf/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4820 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/cat_pdf/doc1.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     4956 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/cat_pdf/doc2.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/cat_pdf/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/cat_pdf/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      955 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/cat_pdf/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      172 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/cat_pdf/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:22.988955 stepup_reprep-1.1.0/tests/cases/check_hrefs_html/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/check_hrefs_html/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/check_hrefs_html/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/check_hrefs_html/check_hrefs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/check_hrefs_html/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/check_hrefs_html/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      596 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/check_hrefs_html/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      178 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/check_hrefs_html/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/check_hrefs_html/test.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:22.988955 stepup_reprep-1.1.0/tests/cases/check_hrefs_md/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/check_hrefs_md/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/check_hrefs_md/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/check_hrefs_md/check_hrefs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/check_hrefs_md/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/check_hrefs_md/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      596 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/check_hrefs_md/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      174 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/check_hrefs_md/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/check_hrefs_md/test.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:22.988955 stepup_reprep-1.1.0/tests/cases/check_hrefs_pdf/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/check_hrefs_pdf/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/check_hrefs_pdf/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/check_hrefs_pdf/check_hrefs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5718 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/check_hrefs_pdf/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/check_hrefs_pdf/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      728 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/check_hrefs_pdf/main.sh
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/check_hrefs_pdf/main.tex
--rwxr-xr-x   0 runner    (1001) docker     (127)      202 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/check_hrefs_pdf/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:22.992955 stepup_reprep-1.1.0/tests/cases/convert_inkscape/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/convert_inkscape/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/convert_inkscape/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4983 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/convert_inkscape/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/convert_inkscape/expected_stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/convert_inkscape/glasses.svg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1179 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/convert_inkscape/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      244 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/convert_inkscape/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/convert_inkscape/smile.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:22.992955 stepup_reprep-1.1.0/tests/cases/convert_libreoffice/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/convert_libreoffice/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/convert_libreoffice/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/convert_libreoffice/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/convert_libreoffice/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      988 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/convert_libreoffice/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      153 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/convert_libreoffice/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)    13660 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/convert_libreoffice/slide.odp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:22.992955 stepup_reprep-1.1.0/tests/cases/convert_markdown/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/convert_markdown/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/convert_markdown/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/convert_markdown/demo.md
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/convert_markdown/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/convert_markdown/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      976 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/convert_markdown/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      151 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/convert_markdown/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:22.992955 stepup_reprep-1.1.0/tests/cases/convert_mutool/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/convert_mutool/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/convert_mutool/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/convert_mutool/example.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/convert_mutool/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/convert_mutool/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      957 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/convert_mutool/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      173 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/convert_mutool/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:22.996955 stepup_reprep-1.1.0/tests/cases/convert_weasyprint/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/convert_weasyprint/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/convert_weasyprint/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/convert_weasyprint/doc.html
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/convert_weasyprint/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/convert_weasyprint/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      963 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/convert_weasyprint/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      157 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/convert_weasyprint/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:22.996955 stepup_reprep-1.1.0/tests/cases/latex_diff/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/latex_diff/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/latex_diff/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/latex_diff/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/latex_diff/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      904 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/latex_diff/main.sh
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/latex_diff/new.tex
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/latex_diff/old.tex
--rwxr-xr-x   0 runner    (1001) docker     (127)      173 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/latex_diff/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:22.996955 stepup_reprep-1.1.0/tests/cases/latex_flat/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/latex_flat/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/latex_flat/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/latex_flat/article_structured.tex
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/latex_flat/expected_article.tex
--rw-r--r--   0 runner    (1001) docker     (127)     3316 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/latex_flat/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/latex_flat/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/latex_flat/expected_stdout_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/latex_flat/expected_stdout_02.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1117 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/latex_flat/main.sh
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/latex_flat/part1.tex
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/latex_flat/part2.tex
--rwxr-xr-x   0 runner    (1001) docker     (127)      210 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/latex_flat/plan_01.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      249 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/latex_flat/plan_02.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:23.000955 stepup_reprep-1.1.0/tests/cases/latex_flat/sub/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/latex_flat/sub/original.tex
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:23.000955 stepup_reprep-1.1.0/tests/cases/latex_flat_subdir/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/latex_flat_subdir/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/latex_flat_subdir/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/latex_flat_subdir/expected_article.tex
--rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/latex_flat_subdir/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/latex_flat_subdir/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      724 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/latex_flat_subdir/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      238 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/latex_flat_subdir/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:23.000955 stepup_reprep-1.1.0/tests/cases/latex_flat_subdir/sub/
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/latex_flat_subdir/sub/article_structured.tex
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/latex_flat_subdir/sub/part1.tex
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/latex_flat_subdir/sub/part2.tex
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:23.000955 stepup_reprep-1.1.0/tests/cases/lualatex_simple/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/lualatex_simple/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/lualatex_simple/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/lualatex_simple/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1103 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/lualatex_simple/main.sh
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/lualatex_simple/paper.tex
--rwxr-xr-x   0 runner    (1001) docker     (127)      134 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/lualatex_simple/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:23.000955 stepup_reprep-1.1.0/tests/cases/make_manifest_in/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/make_manifest_in/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/make_manifest_in/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/make_manifest_in/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/make_manifest_in/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/make_manifest_in/expected_stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/make_manifest_in/hello.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      634 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/make_manifest_in/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      180 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/make_manifest_in/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:23.004955 stepup_reprep-1.1.0/tests/cases/make_manifest_in_sub/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/make_manifest_in_sub/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/make_manifest_in_sub/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/make_manifest_in_sub/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/make_manifest_in_sub/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      685 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/make_manifest_in_sub/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      187 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/make_manifest_in_sub/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:23.004955 stepup_reprep-1.1.0/tests/cases/make_manifest_in_sub/sub/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/make_manifest_in_sub/sub/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/make_manifest_in_sub/sub/hello.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:23.004955 stepup_reprep-1.1.0/tests/cases/make_manifest_list/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/make_manifest_list/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/make_manifest_list/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/make_manifest_list/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/make_manifest_list/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      634 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/make_manifest_list/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      166 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/make_manifest_list/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:23.004955 stepup_reprep-1.1.0/tests/cases/nup_pdf/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/nup_pdf/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/nup_pdf/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/nup_pdf/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/nup_pdf/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      925 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/nup_pdf/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      162 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/nup_pdf/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     9122 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/nup_pdf/src.pdf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:23.008955 stepup_reprep-1.1.0/tests/cases/pdflatex_bbl/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/pdflatex_bbl/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/pdflatex_bbl/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/pdflatex_bbl/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1071 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/pdflatex_bbl/main.sh
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/pdflatex_bbl/paper.bbl
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/pdflatex_bbl/paper.tex
--rwxr-xr-x   0 runner    (1001) docker     (127)      172 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/pdflatex_bbl/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:23.008955 stepup_reprep-1.1.0/tests/cases/pdflatex_bibtex/
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/pdflatex_bibtex/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/pdflatex_bibtex/bibsane.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4953 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/pdflatex_bibtex/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/pdflatex_bibtex/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1350 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/pdflatex_bibtex/main.sh
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/pdflatex_bibtex/paper.tex
--rwxr-xr-x   0 runner    (1001) docker     (127)      190 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/pdflatex_bibtex/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/pdflatex_bibtex/references.bib
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:23.008955 stepup_reprep-1.1.0/tests/cases/pdflatex_input/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/pdflatex_input/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     4368 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/pdflatex_input/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/pdflatex_input/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1116 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/pdflatex_input/main.sh
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/pdflatex_input/paper.tex
--rwxr-xr-x   0 runner    (1001) docker     (127)      224 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/pdflatex_input/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/pdflatex_input/smile.pdf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:23.008955 stepup_reprep-1.1.0/tests/cases/raster_pdf/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/raster_pdf/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/raster_pdf/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/raster_pdf/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/raster_pdf/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1004 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/raster_pdf/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      181 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/raster_pdf/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/raster_pdf/smile.pdf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:23.012955 stepup_reprep-1.1.0/tests/cases/render_basic/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/render_basic/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/render_basic/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/render_basic/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/render_basic/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      696 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/render_basic/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      188 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/render_basic/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/render_basic/template.md
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/render_basic/variables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:23.012955 stepup_reprep-1.1.0/tests/cases/render_relpath/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/render_relpath/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     9195 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/render_relpath/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/render_relpath/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      931 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/render_relpath/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      270 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/render_relpath/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:23.012955 stepup_reprep-1.1.0/tests/cases/render_relpath/static/
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/render_relpath/static/main.tex
--rwxr-xr-x   0 runner    (1001) docker     (127)      213 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/render_relpath/static/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/render_relpath/static/preamble.inc.tex
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/render_relpath/static/variables.py
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/render_relpath/variables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:23.016955 stepup_reprep-1.1.0/tests/cases/tile_pdf/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/tile_pdf/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/tile_pdf/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    15363 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/tile_pdf/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/tile_pdf/expected_stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/tile_pdf/hexagon.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/tile_pdf/horizontal.svg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1373 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/tile_pdf/main.sh
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/tile_pdf/pentagon.svg
--rwxr-xr-x   0 runner    (1001) docker     (127)      227 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/tile_pdf/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/tile_pdf/square.svg
--rwxr-xr-x   0 runner    (1001) docker     (127)      674 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/tile_pdf/tile.py
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/tile_pdf/triangle.svg
--rw-r--r--   0 runner    (1001) docker     (127)    65932 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/tile_pdf/vera.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/tile_pdf/vertical.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:23.016955 stepup_reprep-1.1.0/tests/cases/xelatex_input/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/xelatex_input/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     6384 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/xelatex_input/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/xelatex_input/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1217 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/xelatex_input/main.sh
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/xelatex_input/paper.tex
--rwxr-xr-x   0 runner    (1001) docker     (127)      348 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/xelatex_input/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/xelatex_input/smile.pdf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:23.016955 stepup_reprep-1.1.0/tests/cases/zip_manifest/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/zip_manifest/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/zip_manifest/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/zip_manifest/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/zip_manifest/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      994 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/zip_manifest/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      290 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/zip_manifest/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/zip_manifest/static.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/reprep_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     4395 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/test_bibtex_log.py
--rw-r--r--   0 runner    (1001) docker     (127)     3652 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/test_cases.py
--rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/test_latex_deps.py
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/test_latex_flat.py
--rw-r--r--   0 runner    (1001) docker     (127)    14002 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/test_latex_log.py
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/test_manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/test_zip.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.201306 stepup_reprep-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.145305 stepup_reprep-1.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.153305 stepup_reprep-1.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/.github/workflows/mkdocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/.github/workflows/pytest.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-05-07 17:50:13.201306 stepup_reprep-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.153305 stepup_reprep-1.1.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.153305 stepup_reprep-1.1.1/docs/advanced_topics/
+-rw-r--r--   0 runner    (1001) docker     (127)     6818 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/docs/advanced_topics/good_practices.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/docs/advanced_topics/manifest_files.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.157306 stepup_reprep-1.1.1/docs/advanced_topics/tiling_pdfs/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/docs/advanced_topics/tiling_pdfs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    22692 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/docs/advanced_topics/tiling_pdfs/figure.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/docs/advanced_topics/tiling_pdfs/hexagon.svg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      114 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/docs/advanced_topics/tiling_pdfs/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/docs/advanced_topics/tiling_pdfs/pentagon.svg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      278 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/docs/advanced_topics/tiling_pdfs/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/docs/advanced_topics/tiling_pdfs/square.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/docs/advanced_topics/tiling_pdfs/stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      413 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/docs/advanced_topics/tiling_pdfs/tile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/docs/advanced_topics/tiling_pdfs/triangle.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/docs/advanced_topics/tiling_pdfs.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/docs/clean_stdout.sed
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/docs/development.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.157306 stepup_reprep-1.1.1/docs/from_scratch/
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/docs/from_scratch/introduction.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.157306 stepup_reprep-1.1.1/docs/from_template/
+-rw-r--r--   0 runner    (1001) docker     (127)     4171 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/docs/from_template/before_you_begin.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/docs/from_template/create_or_clone_a_project.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/docs/from_template/introduction.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/docs/from_template/working_on_a_project.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/docs/license.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.157306 stepup_reprep-1.1.1/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/docs/reference/stepup.reprep.api.md
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/docs/reference/stepup.reprep.tile_pdf.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 17:50:13.201306 stepup_reprep-1.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.149305 stepup_reprep-1.1.1/stepup/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.161306 stepup_reprep-1.1.1/stepup/reprep/
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/stepup/reprep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/stepup/reprep/add_notes_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25407 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/stepup/reprep/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/stepup/reprep/bibtex_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5286 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/stepup/reprep/check_hrefs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/stepup/reprep/check_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4370 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/stepup/reprep/convert_inkscape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4076 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/stepup/reprep/convert_markdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7521 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/stepup/reprep/latex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4737 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/stepup/reprep/latex_deps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7006 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/stepup/reprep/latex_flat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5574 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/stepup/reprep/latex_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/stepup/reprep/make_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/stepup/reprep/normalize_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/stepup/reprep/nup_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/stepup/reprep/pytest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/stepup/reprep/raster_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5080 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/stepup/reprep/render.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/stepup/reprep/tile_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/stepup/reprep/zip_manifest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.201306 stepup_reprep-1.1.1/stepup_reprep.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-05-07 17:50:13.000000 stepup_reprep-1.1.1/stepup_reprep.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12175 2024-05-07 17:50:13.000000 stepup_reprep-1.1.1/stepup_reprep.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 17:50:13.000000 stepup_reprep-1.1.1/stepup_reprep.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-07 17:50:13.000000 stepup_reprep-1.1.1/stepup_reprep.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-07 17:50:13.000000 stepup_reprep-1.1.1/stepup_reprep.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-07 17:50:13.000000 stepup_reprep-1.1.1/stepup_reprep.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.161306 stepup_reprep-1.1.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.149305 stepup_reprep-1.1.1/tests/cases/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.161306 stepup_reprep-1.1.1/tests/cases/add_notes_pdf/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/add_notes_pdf/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/add_notes_pdf/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/add_notes_pdf/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/add_notes_pdf/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      955 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/add_notes_pdf/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/add_notes_pdf/notes.pdf
+-rwxr-xr-x   0 runner    (1001) docker     (127)      182 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/add_notes_pdf/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8616 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/add_notes_pdf/src.pdf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.165305 stepup_reprep-1.1.1/tests/cases/cat_pdf/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/cat_pdf/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/cat_pdf/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4820 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/cat_pdf/doc1.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     4956 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/cat_pdf/doc2.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/cat_pdf/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/cat_pdf/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      955 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/cat_pdf/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      172 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/cat_pdf/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.165305 stepup_reprep-1.1.1/tests/cases/check_hrefs_html/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/check_hrefs_html/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/check_hrefs_html/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/check_hrefs_html/check_hrefs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/check_hrefs_html/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/check_hrefs_html/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      596 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/check_hrefs_html/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      178 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/check_hrefs_html/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/check_hrefs_html/test.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.165305 stepup_reprep-1.1.1/tests/cases/check_hrefs_md/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/check_hrefs_md/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/check_hrefs_md/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/check_hrefs_md/check_hrefs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/check_hrefs_md/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/check_hrefs_md/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      596 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/check_hrefs_md/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      174 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/check_hrefs_md/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/check_hrefs_md/test.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.169306 stepup_reprep-1.1.1/tests/cases/check_hrefs_pdf/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/check_hrefs_pdf/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/check_hrefs_pdf/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/check_hrefs_pdf/check_hrefs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5718 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/check_hrefs_pdf/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/check_hrefs_pdf/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      728 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/check_hrefs_pdf/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/check_hrefs_pdf/main.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)      202 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/check_hrefs_pdf/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.169306 stepup_reprep-1.1.1/tests/cases/convert_inkscape/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_inkscape/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_inkscape/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5144 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_inkscape/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_inkscape/expected_stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_inkscape/glasses.svg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1179 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_inkscape/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      244 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_inkscape/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_inkscape/smile.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.173306 stepup_reprep-1.1.1/tests/cases/convert_inkscape_concurrency/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_inkscape_concurrency/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_inkscape_concurrency/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_inkscape_concurrency/dots_050.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_inkscape_concurrency/dots_055.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_inkscape_concurrency/dots_060.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_inkscape_concurrency/dots_065.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3399 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_inkscape_concurrency/dots_070.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3629 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_inkscape_concurrency/dots_075.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_inkscape_concurrency/dots_080.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4088 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_inkscape_concurrency/dots_085.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4308 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_inkscape_concurrency/dots_090.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4535 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_inkscape_concurrency/dots_095.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4774 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_inkscape_concurrency/dots_100.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4990 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_inkscape_concurrency/dots_105.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_inkscape_concurrency/dots_110.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5453 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_inkscape_concurrency/dots_115.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5674 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_inkscape_concurrency/dots_120.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5907 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_inkscape_concurrency/dots_125.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6110 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_inkscape_concurrency/dots_130.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6355 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_inkscape_concurrency/dots_135.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6586 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_inkscape_concurrency/dots_140.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6821 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_inkscape_concurrency/dots_145.svg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1892 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_inkscape_concurrency/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      163 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_inkscape_concurrency/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.173306 stepup_reprep-1.1.1/tests/cases/convert_libreoffice/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_libreoffice/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_libreoffice/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_libreoffice/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_libreoffice/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      988 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_libreoffice/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      153 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_libreoffice/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13660 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_libreoffice/slide.odp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.173306 stepup_reprep-1.1.1/tests/cases/convert_libreoffice_concurrency/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_libreoffice_concurrency/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1886 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_libreoffice_concurrency/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      242 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_libreoffice_concurrency/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10286 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_libreoffice_concurrency/something.odt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.173306 stepup_reprep-1.1.1/tests/cases/convert_markdown/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_markdown/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_markdown/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_markdown/demo.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_markdown/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_markdown/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      976 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_markdown/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      151 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_markdown/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.177306 stepup_reprep-1.1.1/tests/cases/convert_mutool/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_mutool/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_mutool/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_mutool/example.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_mutool/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_mutool/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      957 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_mutool/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      173 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_mutool/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.177306 stepup_reprep-1.1.1/tests/cases/convert_weasyprint/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_weasyprint/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_weasyprint/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_weasyprint/doc.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_weasyprint/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_weasyprint/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      963 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_weasyprint/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      157 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_weasyprint/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.177306 stepup_reprep-1.1.1/tests/cases/latex_diff/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/latex_diff/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/latex_diff/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/latex_diff/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/latex_diff/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      904 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/latex_diff/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/latex_diff/new.tex
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/latex_diff/old.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)      173 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/latex_diff/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.181306 stepup_reprep-1.1.1/tests/cases/latex_flat/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/latex_flat/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/latex_flat/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/latex_flat/article_structured.tex
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/latex_flat/expected_article.tex
+-rw-r--r--   0 runner    (1001) docker     (127)     3316 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/latex_flat/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/latex_flat/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/latex_flat/expected_stdout_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/latex_flat/expected_stdout_02.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1117 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/latex_flat/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/latex_flat/part1.tex
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/latex_flat/part2.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)      210 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/latex_flat/plan_01.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      249 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/latex_flat/plan_02.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.181306 stepup_reprep-1.1.1/tests/cases/latex_flat/sub/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/latex_flat/sub/original.tex
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.181306 stepup_reprep-1.1.1/tests/cases/latex_flat_subdir/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/latex_flat_subdir/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/latex_flat_subdir/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/latex_flat_subdir/expected_article.tex
+-rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/latex_flat_subdir/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/latex_flat_subdir/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      724 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/latex_flat_subdir/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      238 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/latex_flat_subdir/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.181306 stepup_reprep-1.1.1/tests/cases/latex_flat_subdir/sub/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/latex_flat_subdir/sub/article_structured.tex
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/latex_flat_subdir/sub/part1.tex
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/latex_flat_subdir/sub/part2.tex
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.185306 stepup_reprep-1.1.1/tests/cases/lualatex_simple/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/lualatex_simple/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/lualatex_simple/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/lualatex_simple/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1103 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/lualatex_simple/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/lualatex_simple/paper.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)      134 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/lualatex_simple/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.185306 stepup_reprep-1.1.1/tests/cases/make_manifest_in/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/make_manifest_in/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/make_manifest_in/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/make_manifest_in/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/make_manifest_in/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/make_manifest_in/expected_stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/make_manifest_in/hello.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      634 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/make_manifest_in/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      180 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/make_manifest_in/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.185306 stepup_reprep-1.1.1/tests/cases/make_manifest_in_sub/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/make_manifest_in_sub/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/make_manifest_in_sub/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/make_manifest_in_sub/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/make_manifest_in_sub/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      685 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/make_manifest_in_sub/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      187 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/make_manifest_in_sub/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.185306 stepup_reprep-1.1.1/tests/cases/make_manifest_in_sub/sub/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/make_manifest_in_sub/sub/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/make_manifest_in_sub/sub/hello.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.185306 stepup_reprep-1.1.1/tests/cases/make_manifest_list/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/make_manifest_list/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/make_manifest_list/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/make_manifest_list/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/make_manifest_list/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      634 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/make_manifest_list/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      166 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/make_manifest_list/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.189306 stepup_reprep-1.1.1/tests/cases/nup_pdf/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/nup_pdf/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/nup_pdf/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/nup_pdf/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/nup_pdf/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      925 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/nup_pdf/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      162 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/nup_pdf/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9122 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/nup_pdf/src.pdf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.189306 stepup_reprep-1.1.1/tests/cases/pdflatex_bbl/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/pdflatex_bbl/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/pdflatex_bbl/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/pdflatex_bbl/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1071 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/pdflatex_bbl/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/pdflatex_bbl/paper.bbl
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/pdflatex_bbl/paper.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)      172 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/pdflatex_bbl/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.189306 stepup_reprep-1.1.1/tests/cases/pdflatex_bibtex/
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/pdflatex_bibtex/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/pdflatex_bibtex/bibsane.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4953 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/pdflatex_bibtex/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/pdflatex_bibtex/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1350 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/pdflatex_bibtex/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/pdflatex_bibtex/paper.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)      190 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/pdflatex_bibtex/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/pdflatex_bibtex/references.bib
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.193306 stepup_reprep-1.1.1/tests/cases/pdflatex_input/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/pdflatex_input/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     4368 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/pdflatex_input/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/pdflatex_input/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1116 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/pdflatex_input/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/pdflatex_input/paper.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)      224 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/pdflatex_input/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/pdflatex_input/smile.pdf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.193306 stepup_reprep-1.1.1/tests/cases/raster_pdf/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/raster_pdf/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/raster_pdf/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/raster_pdf/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/raster_pdf/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1004 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/raster_pdf/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      181 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/raster_pdf/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/raster_pdf/smile.pdf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.193306 stepup_reprep-1.1.1/tests/cases/render_basic/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/render_basic/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/render_basic/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/render_basic/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/render_basic/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      696 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/render_basic/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      188 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/render_basic/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/render_basic/template.md
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/render_basic/variables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.193306 stepup_reprep-1.1.1/tests/cases/render_relpath/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/render_relpath/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     9195 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/render_relpath/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/render_relpath/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      931 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/render_relpath/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      270 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/render_relpath/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.193306 stepup_reprep-1.1.1/tests/cases/render_relpath/static/
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/render_relpath/static/main.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)      213 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/render_relpath/static/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/render_relpath/static/preamble.inc.tex
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/render_relpath/static/variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/render_relpath/variables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.197306 stepup_reprep-1.1.1/tests/cases/tile_pdf/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/tile_pdf/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/tile_pdf/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    15801 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/tile_pdf/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/tile_pdf/expected_stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/tile_pdf/hexagon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/tile_pdf/horizontal.svg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1373 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/tile_pdf/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/tile_pdf/pentagon.svg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      227 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/tile_pdf/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/tile_pdf/square.svg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      674 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/tile_pdf/tile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/tile_pdf/triangle.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    65932 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/tile_pdf/vera.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/tile_pdf/vertical.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.197306 stepup_reprep-1.1.1/tests/cases/xelatex_input/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/xelatex_input/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     6384 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/xelatex_input/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/xelatex_input/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1217 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/xelatex_input/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/xelatex_input/paper.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)      348 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/xelatex_input/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/xelatex_input/smile.pdf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.201306 stepup_reprep-1.1.1/tests/cases/zip_manifest/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/zip_manifest/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/zip_manifest/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/zip_manifest/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/zip_manifest/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      994 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/zip_manifest/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      290 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/zip_manifest/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/zip_manifest/static.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/reprep_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4394 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/test_bibtex_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3719 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/test_cases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/test_latex_deps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/test_latex_flat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14002 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/test_latex_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/test_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/test_zip.py
```

### Comparing `stepup_reprep-1.1.0/.github/workflows/release.yaml` & `stepup_reprep-1.1.1/.github/workflows/release.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     name: Publish Python distribution to PyPI
     if: startsWith(github.ref, 'refs/tags/')  # only publish to PyPI on tag pushes
     needs:
     - build
     runs-on: ubuntu-latest
     environment:
       name: pypi
-      url: https://pypi.org/p/stepup
+      url: https://pypi.org/p/stepup-reprep
     permissions:
       id-token: write
 
     steps:
     - name: Download all the dists
       uses: actions/download-artifact@v3
       with:
@@ -89,22 +89,22 @@
       run: >-
         gh release upload
         '${{ github.ref_name }}' dist/**
         --repo '${{ github.repository }}'
 
   publish-to-testpypi:
     name: Publish Python distribution to TestPyPI
-    if: ${{ ! startsWith(github.ref, 'refs/tags/') }}
+    if: ${{ github.ref == 'refs/heads/main' &&  github.repository_owner == 'reproducible-reporting'}}
     needs:
     - build
     runs-on: ubuntu-latest
 
     environment:
       name: testpypi
-      url: https://test.pypi.org/p/<package-name>
+      url: https://test.pypi.org/p/stepup-reprep
 
     permissions:
       id-token: write
 
     steps:
     - name: Download all the dists
       uses: actions/download-artifact@v3
```

### Comparing `stepup_reprep-1.1.0/.pre-commit-config.yaml` & `stepup_reprep-1.1.1/.pre-commit-config.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 repos:
 - repo: https://github.com/pre-commit/pre-commit-hooks
-  rev: v4.5.0
+  rev: v4.6.0
   hooks:
     - id: check-added-large-files
     - id: check-ast
     - id: check-case-conflict
     - id: check-executables-have-shebangs
     - id: check-json
     - id: check-merge-conflict
@@ -20,20 +20,17 @@
     - id: pretty-format-json
       args: ["--autofix", "--no-sort-keys"]
     - id: trailing-whitespace
 - repo: https://github.com/Lucas-C/pre-commit-hooks
   rev: v1.5.5
   hooks:
     - id: remove-crlf
-- repo: https://github.com/psf/black
-  rev: 24.3.0
-  hooks:
-    - id: black
 - repo: https://github.com/astral-sh/ruff-pre-commit
-  rev: 'v0.3.5'
+  rev: v0.4.3
   hooks:
+    - id: ruff-format
     - id: ruff
-      args: ["--fix"]
+      args: ["--fix", "--show-fixes"]
 - repo: https://github.com/python-jsonschema/check-jsonschema
-  rev: 0.28.1
+  rev: 0.28.2
   hooks:
     - id: check-github-workflows
```

### Comparing `stepup_reprep-1.1.0/LICENSE` & `stepup_reprep-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/PKG-INFO` & `stepup_reprep-1.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stepup-reprep
-Version: 1.1.0
+Version: 1.1.1
 Summary: StepUp RepRep is the StepUp extension for Reproducible Reporting
 Author-email: Toon Verstraelen <toon.verstraelen@ugent.be>
 Project-URL: Documentation, https://reproducible-reporting.github.io/stepup-reprep/
 Project-URL: Issues, https://github.com/reproducible-reporting/stepup-reprep/issues
 Project-URL: Source, https://github.com/reproducible-reporting/stepup-reprep/
 Project-URL: Changelog, https://reproducible-reporting.github.io/stepup-reprep/changelog/
 Classifier: Environment :: Console
@@ -37,14 +37,16 @@
 Requires-Dist: pytest-xdist; extra == "dev"
 Requires-Dist: mkdocs; extra == "dev"
 Requires-Dist: mkdocstrings[python]; extra == "dev"
 Requires-Dist: mkdocs-macros-plugin; extra == "dev"
 Requires-Dist: mkdocs-material; extra == "dev"
 
 [![release](https://github.com/reproducible-reporting/stepup-reprep/actions/workflows/release.yaml/badge.svg)](https://github.com/reproducible-reporting/stepup-reprep/actions/workflows/release.yaml)
+[![pytest](https://github.com/reproducible-reporting/stepup-reprep/actions/workflows/pytest.yaml/badge.svg)](https://github.com/reproducible-reporting/stepup-reprep/actions/workflows/pytest.yaml)
+[![mkdocs](https://github.com/reproducible-reporting/stepup-reprep/actions/workflows/mkdocs.yaml/badge.svg)](https://github.com/reproducible-reporting/stepup-reprep/actions/workflows/mkdocs.yaml)
 [![PyPI Version](https://img.shields.io/pypi/v/stepup-reprep)](https://pypi.org/project/stepup-reprep/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/stepup-reprep)
 ![GPL-3 License](https://img.shields.io/github/license/reproducible-reporting/stepup-reprep)
 
 
 # StepUp RepRep
```

### Comparing `stepup_reprep-1.1.0/README.md` & `stepup_reprep-1.1.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 [![release](https://github.com/reproducible-reporting/stepup-reprep/actions/workflows/release.yaml/badge.svg)](https://github.com/reproducible-reporting/stepup-reprep/actions/workflows/release.yaml)
+[![pytest](https://github.com/reproducible-reporting/stepup-reprep/actions/workflows/pytest.yaml/badge.svg)](https://github.com/reproducible-reporting/stepup-reprep/actions/workflows/pytest.yaml)
+[![mkdocs](https://github.com/reproducible-reporting/stepup-reprep/actions/workflows/mkdocs.yaml/badge.svg)](https://github.com/reproducible-reporting/stepup-reprep/actions/workflows/mkdocs.yaml)
 [![PyPI Version](https://img.shields.io/pypi/v/stepup-reprep)](https://pypi.org/project/stepup-reprep/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/stepup-reprep)
 ![GPL-3 License](https://img.shields.io/github/license/reproducible-reporting/stepup-reprep)
 
 
 # StepUp RepRep
```

### Comparing `stepup_reprep-1.1.0/docs/development.md` & `stepup_reprep-1.1.1/docs/development.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,26 @@
 # Developer Notes
 
 If you would like to contribute, please read [CONTRIBUTING.md](https://github.com/reproducible-reporting/.github/blob/main/CONTRIBUTING.md).
 
-## How to Make Releases
-
-- Mark the release in `changelog.md`.
-- Make a new commit and tag it with `vX.Y.Z`.
-- Trigger the PyPI GitHub Action: `git push origin main --tags`.
-
-
 ## Development Install and Unit Tests
 
 First, create a [StepUp Core development installation](https://reproducible-reporting.github.io/stepup-core/development/).
 The following commands assume you create `stepup-core` and `step-reprep` source trees as subdirectories of the same parent.
 
 ```bash
 git clone git@github.com:reproducible-reporting/stepup-reprep.git
 cd stepup-reprep
 pre-commit install
 python -m venv venv
 echo 'source venv/bin/activate' > .envrc
 direnv allow
 pip install -U pip
 pip install -e .[dev]
-pip install -e ../stepup-core
+pip install -e ../stepup-core  # optional
 pytest -vv
 ```
 
 ## Documentation
 
 The documentation is created with [MkDocs](https://www.mkdocs.org/).
 
@@ -35,7 +28,17 @@
 
 ```bash
 mkdocs serve --watch stepup/reprep/
 ```
 
 (Keep this running.)
 Then open the live preview in your browser: [http://127.0.0.1:8000/](http://127.0.0.1:8000/)
+and edit Markdown files in your IDE.
+
+Please, use [Semantic Line Breaks](https://sembr.org/)
+because it results in cleaner file diffs when editing documentation.
+
+## How to Make A Release
+
+- Mark the release in `changelog.md`.
+- Make a new commit and tag it with `vX.Y.Z`.
+- Trigger the PyPI GitHub Action: `git push origin main --tags`.
```

### Comparing `stepup_reprep-1.1.0/docs/index.md` & `stepup_reprep-1.1.1/docs/index.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,13 @@
 # Welcome to StepUp RepRep
 
 StepUp RepRep is the publication build tool for [Reproducible Reporting](https://github.com/reproducible-reporting).
 It is a domain-specific extension of a powerful universal build tool called [StepUp Core](https://reproducible-reporting.github.io/stepup-core/).
 
-To get started, follow the tutorials in this documentation:
-
-- [Before You Begin](tutorials/before_you_begin.md)
-- [Create or Clone a Project](tutorials/create_or_clone_a_project.md)
-- [Working on a Project](tutorials/working_on_a_project.md)
-
+To get started, we recommend to follow the [Template Tutorial](from_template/introduction.md) in this documentation.
 StepUp RepRep will be installed in your instance of the template, as part of the setup.
 
 If you want to gain a more in-depth understanding of how StepUp works, the [StepUp Core tutorials](https://reproducible-reporting.github.io/stepup-core/getting_started/introduction/) will take you through all the basics.
 
 
 ## Quick Demo
```

### Comparing `stepup_reprep-1.1.0/docs/installation.md` & `stepup_reprep-1.1.1/docs/installation.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,26 @@
 # Installation
 
-Requirements:
+!!! warning "The installation instructions are listed here for completeness."
+
+    If you are new to StepUp RepRep, we recommend that you follow the [Template Tutorial](from_template/introduction.md) instead.
+    One of the steps in that tutorial is to install StepUp RepRep in a suitable virtual environment.
+
+
+## Requirements
 
 - [POSIX](https://en.wikipedia.org/wiki/POSIX) operating system: Linux, macOS or WSL. StepUp cannot run natively on Windows.
 - [Python](https://www.python.org/) ≥ 3.11
 - [Pip](https://pip.pypa.io/)
 
 It is assumed you know how to use [Pip](https://pip.pypa.io/).
 We recommend performing the installation in a [Python virtual environment](https://docs.python.org/3/library/venv.html) and activating such environments with [direnv](https://direnv.net/).
 
+## Minimal installation
+
 The RepRep extension (for reproducible reporting) is installed with:
 
 ```bash
 pip install stepup-reprep
 ```
 
-(This will also install `stepup-core`.)
+(This will also install [StepUp Core](https://reproducible-reporting.github.io/stepup-core/).)
```

### Comparing `stepup_reprep-1.1.0/docs/license.md` & `stepup_reprep-1.1.1/docs/license.md`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/docs/tutorials/before_you_begin.md` & `stepup_reprep-1.1.1/docs/from_template/before_you_begin.md`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/docs/tutorials/create_or_clone_a_project.md` & `stepup_reprep-1.1.1/docs/from_template/create_or_clone_a_project.md`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/docs/tutorials/manifest_files.md` & `stepup_reprep-1.1.1/docs/advanced_topics/manifest_files.md`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/docs/tutorials/template_conventions.md` & `stepup_reprep-1.1.1/docs/advanced_topics/good_practices.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Template Conventions
+# Good Practices
 
 This tutorial lists some recommendations that facilitate data reuse and reproducibility.
 
 
 ## General Filename Conventions
 
 ### Must
@@ -122,21 +122,23 @@
 - Jupyter notebooks
 
 
 ## Data Sets
 
 ### Must
 
-- Use `dataset-{name}` directories for data that cannot be (easily) generated from scratch:
+- Use `dataset-{name}` directories for data that cannot be (easily) generated from scratch.
+  For example.
 
     - External data sets.
     - Expensive calculations done previously.
+    - (Large amounts of) experimental measurements.
     - Data generated with closed-source software.
       (Avoid closed-source software when you have the choice.)
-    - Data requiring specialized hardware not generally available.
+    - Data created with specialized hardware not generally available.
     - Manually curated data.
 
 - Add scripts and implementations to regenerate the data,
   integrating them as much as possible with StepUp RepRep.
 
 - Add a `README.md` file explaining:
```

### Comparing `stepup_reprep-1.1.0/docs/tutorials/tiling_pdfs/figure.png` & `stepup_reprep-1.1.1/docs/advanced_topics/tiling_pdfs/figure.png`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/docs/tutorials/tiling_pdfs/hexagon.svg` & `stepup_reprep-1.1.1/docs/advanced_topics/tiling_pdfs/hexagon.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/docs/tutorials/tiling_pdfs/pentagon.svg` & `stepup_reprep-1.1.1/docs/advanced_topics/tiling_pdfs/pentagon.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/docs/tutorials/tiling_pdfs/square.svg` & `stepup_reprep-1.1.1/docs/advanced_topics/tiling_pdfs/square.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/docs/tutorials/tiling_pdfs/stdout.txt` & `stepup_reprep-1.1.1/docs/advanced_topics/tiling_pdfs/stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/docs/tutorials/tiling_pdfs/triangle.svg` & `stepup_reprep-1.1.1/docs/advanced_topics/tiling_pdfs/triangle.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/docs/tutorials/tiling_pdfs.md` & `stepup_reprep-1.1.1/docs/advanced_topics/tiling_pdfs.md`

 * *Files 23% similar despite different names*

```diff
@@ -7,39 +7,39 @@
 
 This tutorial provides a simple example that you can use as a starting point.
 For a more advanced example, see the [`tild_pdf` test case](https://github.com/reproducible-reporting/stepup-reprep/tree/main/tests/cases/tile_pdf) in the StepUp RepRep unit test suite.
 
 
 ## Example
 
-Example source files: [tutorials/tiling_pdfs/](https://github.com/reproducible-reporting/stepup-reprep/tree/main/docs/tutorials/tiling_pdfs)
+Example source files: [tutorials/tiling_pdfs/](https://github.com/reproducible-reporting/stepup-reprep/tree/main/docs/advanced_topics/tiling_pdfs)
 
 Create a `tile.py` script with the following code:
 
 ```python
-{% include 'tutorials/tiling_pdfs/tile.py' %}
+{% include 'advanced_topics/tiling_pdfs/tile.py' %}
 ```
 
 Next, create a script `plan.py` as follows:
 
 ```python
-{% include 'tutorials/tiling_pdfs/plan.py' %}
+{% include 'advanced_topics/tiling_pdfs/plan.py' %}
 ```
 
 For this example to work, you also need to create four SVG figures of the same size: `triangle.svg`, `square.svg`, `pentagon.svg` and  `hexagon.svg`.
 
 To run the example, make the scripts executable and run StepUp:
 
 ```bash
 chmod +x plan.py tile.py
 stepup -n -w1
 ```
 
 You should see the following terminal output:
 
 ```
-{% include 'tutorials/tiling_pdfs/stdout.txt' %}
+{% include 'advanced_topics/tiling_pdfs/stdout.txt' %}
 ```
 
 This is the PNG conversion of the resulting PDF figure:
 
 ![figure](tiling_pdfs/figure.png)
```

### Comparing `stepup_reprep-1.1.0/docs/tutorials/working_on_a_project.md` & `stepup_reprep-1.1.1/docs/from_template/working_on_a_project.md`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/mkdocs.yml` & `stepup_reprep-1.1.1/mkdocs.yml`

 * *Files 24% similar despite different names*

```diff
@@ -34,21 +34,25 @@
     toggle:
       icon: material/toggle-switch-off
       name: Switch to system preference
 
 nav:
   - Home: index.md
   - installation.md
-  - Tutorials:
-    - tutorials/before_you_begin.md
-    - tutorials/create_or_clone_a_project.md
-    - tutorials/working_on_a_project.md
-    - tutorials/template_conventions.md
-    - tutorials/manifest_files.md
-    - tutorials/tiling_pdfs.md
+  - Template Tutorial:
+    - from_template/introduction.md
+    - from_template/before_you_begin.md
+    - from_template/create_or_clone_a_project.md
+    - from_template/working_on_a_project.md
+  - From Scratch:
+    - from_scratch/introduction.md
+  - Advanced Topics:
+    - advanced_topics/manifest_files.md
+    - advanced_topics/tiling_pdfs.md
+    - advanced_topics/good_practices.md
   - Reference:
     - reference/stepup.reprep.api.md
     - reference/stepup.reprep.tile_pdf.md
   - changelog.md
   - development.md
   - license.md
 
@@ -65,15 +69,18 @@
       python:
         paths: ["stepup-reprep"]
         options:
           docstring_style: numpy
           docstring_section_style: list
 
 markdown_extensions:
+  - admonition
   - smarty
   - pymdownx.highlight:
       anchor_linenums: true
       line_spans: __span
       pygments_lang_class: true
   - pymdownx.inlinehilite
   - pymdownx.snippets
   - pymdownx.superfences
+  - toc:
+      permalink: true
```

### Comparing `stepup_reprep-1.1.0/pyproject.toml` & `stepup_reprep-1.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -67,17 +67,17 @@
 target-version = ['py311']
 
 [tool.ruff]
 line-length = 100
 target-version = "py311"
 
 [tool.ruff.lint]
-select = ["E", "F", "UP", "B", "I", "PGH", "PL", "RUF", "C"]
+select = ["E", "F", "UP", "B", "SIM", "I", "PGH", "PL", "RUF", "C"]
 ignore = ["PLR0911", "PLR0912", "PLR0913", "PLR0915", "PLR2004", "PLW2901", "C901"]
 
 [tool.setuptools]
-packages = ["stepup.reprep"]
+packages = ["stepup"]
 
 [tool.setuptools_scm]
 write_to = "stepup/reprep/_version.py"
 version_scheme = "post-release"
 local_scheme = "no-local-version"
```

### Comparing `stepup_reprep-1.1.0/stepup/reprep/__init__.py` & `stepup_reprep-1.1.1/stepup/reprep/__init__.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/stepup/reprep/add_notes_pdf.py` & `stepup_reprep-1.1.1/stepup/reprep/add_notes_pdf.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/stepup/reprep/api.py` & `stepup_reprep-1.1.1/stepup/reprep/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -193,17 +193,14 @@
     if not path_html.endswith(".html"):
         raise ValueError("The HTML file must have extension .html")
     path_pdf = make_path_out(path_html, out, ".pdf")
     command = "weasyprint ${inp} ${out}"
     step(command, inp=path_html, out=path_pdf, optional=optional, block=block)
 
 
-pool("libreoffice", 1)
-
-
 def convert_odf_pdf(
     path_odf: str,
     out: str | None = None,
     *,
     libreoffice: str | None = None,
     optional: bool = False,
     block: bool = False,
@@ -234,20 +231,25 @@
     """
     with subs_env_vars() as subs:
         path_odf = subs(path_odf)
         out = subs(out)
     if libreoffice is None:
         libreoffice = getenv("REPREP_LIBREOFFICE", "libreoffice")
     command = (
-        # Hacky workaround for the poor CLI of libreoffice ...
-        f"WORK=`mktemp -d --suffix=reprep` && {libreoffice} --convert-to pdf "
-        "${inp} --outdir ${WORK} > /dev/null && cp ${WORK}/*.pdf ${out} && rm -r ${WORK}"
+        # Simple things should be simple! ;) See:
+        # https://bugs.documentfoundation.org/show_bug.cgi?id=106134
+        # https://bugs.documentfoundation.org/show_bug.cgi?id=152192
+        # Not solved yet:
+        # https://bugs.documentfoundation.org/show_bug.cgi?id=160033
+        f"WORK=`mktemp -d --suffix=reprep` && {libreoffice} "
+        "-env:UserInstallation=file://${WORK} --convert-to pdf ${inp} --outdir ${WORK} "
+        "> /dev/null && cp ${WORK}/*.pdf ${out} && rm -r ${WORK}"
     )
     path_pdf = make_path_out(path_odf, out, ".pdf")
-    step(command, inp=path_odf, out=path_pdf, pool="libreoffice", optional=optional, block=block)
+    step(command, inp=path_odf, out=path_pdf, optional=optional, block=block)
 
 
 def convert_pdf(
     path_pdf: str,
     path_out: str,
     *,
     resolution: int | None = None,
@@ -306,17 +308,14 @@
         raise ValueError("The PDF file must have extension .pdf")
     path_png = make_path_out(path_pdf, out, ".png")
     convert_pdf(
         path_pdf, path_png, resolution=resolution, mutool=mutool, optional=optional, block=block
     )
 
 
-pool("inkscape", 1)
-
-
 def convert_svg(
     path_svg: str,
     path_out: str,
     *,
     inkscape: str | None = None,
     inkscape_args: str | None = None,
     optional: bool = False,
```

### Comparing `stepup_reprep-1.1.0/stepup/reprep/bibtex_log.py` & `stepup_reprep-1.1.1/stepup/reprep/bibtex_log.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
 # --
 r"""Identification of errors in BibTeX logs."""
 
-
 from .latex_log import DEFAULT_MESSAGE, ErrorInfo
 
 
 def parse_bibtex_log(path_blg: str) -> ErrorInfo | None:
     """Parse a BibTeX log file.
 
     Parameters
```

### Comparing `stepup_reprep-1.1.0/stepup/reprep/check_hrefs.py` & `stepup_reprep-1.1.1/stepup/reprep/check_hrefs.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/stepup/reprep/check_manifest.py` & `stepup_reprep-1.1.1/stepup/reprep/check_manifest.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 There are two kinds of MANIFEST files:
 
 - ``MANIFEST.in`` contains rules to select or ignore files to be included into an archive.
 - ``MANIFEST.txt`` is the result of a processing a ``MANIFEST.in`` file with this script.
   It contains every individual file, together with its size in bytes and its blake2b hexdigest.
 """
 
-
 import argparse
 import sys
 from collections.abc import Iterator
 
 from path import Path
 
 from stepup.core.hash import compute_file_digest
```

### Comparing `stepup_reprep-1.1.0/stepup/reprep/convert_inkscape.py` & `stepup_reprep-1.1.1/stepup/reprep/convert_inkscape.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 #
 # --
 """Wrapper for SVG to PDF convrsion."""
 
 import argparse
 import re
 import sys
-from mmap import mmap
 
 from path import Path
 
 from stepup.core.api import getenv, step
 
 
 def main() -> int:
@@ -82,18 +81,18 @@
 
 def convert_svg_pdf(
     path_svg: str, path_out: Path, inkscape: str, inkscape_args: str, optional: bool
 ):
     inp_paths = search_svg_deps(path_svg)
     ffmt = path_out.suffix[1:]
     step(
-        f"{inkscape} {path_svg} {inkscape_args} --export-filename={path_out} --export-type={ffmt}",
+        f"unshare --user {inkscape} {path_svg} {inkscape_args} "
+        f"--export-filename={path_out} --export-type={ffmt}",
         inp=[path_svg, *inp_paths],
         out=path_out,
-        pool="inkscape",
         optional=optional,
     )
 
 
 RE_OPTIONS = re.MULTILINE | re.DOTALL
 RE_SVG_HREF = re.compile(rb"<image\s[^<]*?href=\"(?!#)(?!data:)(.*?)\"[^<]*?>", RE_OPTIONS)
 
@@ -103,17 +102,16 @@
     implicit = []
     todo = [src]
     idep = 0
     while idep < len(todo):
         path_svg = Path(todo[idep])
         # It is generally a poor practice to parse XML with a regular expression,
         # unless performance becomes an issue...
-        with open(path_svg, "rb+") as fh:
-            data = mmap(fh.fileno(), 0)
-            hrefs = re.findall(RE_SVG_HREF, data)
+        with open(path_svg, "rb") as fh:
+            hrefs = re.findall(RE_SVG_HREF, fh.read())
 
         # Process hrefs
         for href in hrefs:
             href = href.decode("utf-8")
             if href.startswith("file://"):
                 href = href[7:]
             if "://" not in href:
```

### Comparing `stepup_reprep-1.1.0/stepup/reprep/convert_markdown.py` & `stepup_reprep-1.1.1/stepup/reprep/convert_markdown.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
 # --
 """Markdown to HTML conversion."""
 
-
 import argparse
 import re
 import sys
 import tempfile
 
 import markdown
```

### Comparing `stepup_reprep-1.1.0/stepup/reprep/latex.py` & `stepup_reprep-1.1.1/stepup/reprep/latex.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/stepup/reprep/latex_deps.py` & `stepup_reprep-1.1.1/stepup/reprep/latex_deps.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
 # --
 r"""Identification of dependencies from LaTeX sources."""
 
-
 import re
 
 from path import Path
 
 RE_OPTIONS = re.MULTILINE | re.DOTALL
 RE_INPUT = re.compile(r"\\input\s*\{(.*?)}", RE_OPTIONS)
 RE_VERBATIMINPUT = re.compile(r"\\verbatiminput\s*\{(.*?)}", RE_OPTIONS)
@@ -106,18 +105,15 @@
         BibTeX files.
     """
     implicit = set()
     bib = set()
 
     path_tex = Path(path_tex)
     if path_tex.is_file():
-        if tex_root is None:
-            tex_root = path_tex.parent.normpath()
-        else:
-            tex_root = Path(tex_root)
+        tex_root = path_tex.parent.normpath() if tex_root is None else Path(tex_root)
         with open(path_tex) as fh:
             stripped = []
             for line in fh:
                 if "%REPREPBUILD ignore" in line:
                     pass
                 elif line.startswith("%REPREPBUILD input "):
                     implicit.add((tex_root / line[18:].strip()).normpath())
```

### Comparing `stepup_reprep-1.1.0/stepup/reprep/latex_flat.py` & `stepup_reprep-1.1.1/stepup/reprep/latex_flat.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,15 +33,14 @@
 This script is intentionally somewhat limited.
 It expects that ``\input`` and ``\import`` commands are the only ones present on their line,
 to avoid ambiguities. If this is not the case, the script will fail.
 The script also assumes the ``\includgraphics``, ``\thebibliography`` and ``\verbatiminput``
 commands are contained within a single line.
 """
 
-
 import argparse
 import re
 import sys
 import tempfile
 from typing import TextIO
 
 from path import Path
@@ -99,18 +98,15 @@
     returncode
         Zero when successful.
     inp_paths
         A list of additional inputs used.
     """
     inp_paths = []
     path_tex = Path(path_tex)
-    if tex_root is None:
-        tex_root = path_tex.parent.normpath()
-    else:
-        tex_root = Path(tex_root)
+    tex_root = path_tex.parent.normpath() if tex_root is None else Path(tex_root)
     with open(path_tex) as fh:
         for iline, line in enumerate(fh):
             # Reduce line to standard form
             stripped = line[: line.find("%")].strip()
             stripped = stripped.replace(" ", "").replace("\t", "")
 
             # Try to find input or import
```

### Comparing `stepup_reprep-1.1.0/stepup/reprep/latex_log.py` & `stepup_reprep-1.1.1/stepup/reprep/latex_log.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
 # --
 r"""Identification of errors in LaTeX logs."""
 
-
 import re
 import sys
 
 import attrs
 
 
 @attrs.define
```

### Comparing `stepup_reprep-1.1.0/stepup/reprep/make_manifest.py` & `stepup_reprep-1.1.1/stepup/reprep/make_manifest.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/stepup/reprep/normalize_pdf.py` & `stepup_reprep-1.1.1/stepup/reprep/normalize_pdf.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/stepup/reprep/nup_pdf.py` & `stepup_reprep-1.1.1/stepup/reprep/nup_pdf.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/stepup/reprep/pytest.py` & `stepup_reprep-1.1.1/stepup/reprep/pytest.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/stepup/reprep/raster_pdf.py` & `stepup_reprep-1.1.1/stepup/reprep/raster_pdf.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/stepup/reprep/render.py` & `stepup_reprep-1.1.1/stepup/reprep/render.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 # --
 """Rendering of template files with Jinja2.
 
 Parameters for the template can be defined in a "variables" Python file,
 from which all variables that are strings, integers or floats are imported.
 """
 
-
 import argparse
 import contextlib
 import sys
 
 import jinja2
 from path import Path
```

### Comparing `stepup_reprep-1.1.0/stepup/reprep/tile_pdf.py` & `stepup_reprep-1.1.1/stepup/reprep/tile_pdf.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/stepup/reprep/zip_manifest.py` & `stepup_reprep-1.1.1/stepup/reprep/zip_manifest.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
 # --
 """Create ZIP with all files listed in a MANIFEST.txt file."""
 
-
 import argparse
 import datetime
 import sys
 import tempfile
 import zipfile
 
 from path import Path
```

### Comparing `stepup_reprep-1.1.0/stepup_reprep.egg-info/PKG-INFO` & `stepup_reprep-1.1.1/stepup_reprep.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stepup-reprep
-Version: 1.1.0
+Version: 1.1.1
 Summary: StepUp RepRep is the StepUp extension for Reproducible Reporting
 Author-email: Toon Verstraelen <toon.verstraelen@ugent.be>
 Project-URL: Documentation, https://reproducible-reporting.github.io/stepup-reprep/
 Project-URL: Issues, https://github.com/reproducible-reporting/stepup-reprep/issues
 Project-URL: Source, https://github.com/reproducible-reporting/stepup-reprep/
 Project-URL: Changelog, https://reproducible-reporting.github.io/stepup-reprep/changelog/
 Classifier: Environment :: Console
@@ -37,14 +37,16 @@
 Requires-Dist: pytest-xdist; extra == "dev"
 Requires-Dist: mkdocs; extra == "dev"
 Requires-Dist: mkdocstrings[python]; extra == "dev"
 Requires-Dist: mkdocs-macros-plugin; extra == "dev"
 Requires-Dist: mkdocs-material; extra == "dev"
 
 [![release](https://github.com/reproducible-reporting/stepup-reprep/actions/workflows/release.yaml/badge.svg)](https://github.com/reproducible-reporting/stepup-reprep/actions/workflows/release.yaml)
+[![pytest](https://github.com/reproducible-reporting/stepup-reprep/actions/workflows/pytest.yaml/badge.svg)](https://github.com/reproducible-reporting/stepup-reprep/actions/workflows/pytest.yaml)
+[![mkdocs](https://github.com/reproducible-reporting/stepup-reprep/actions/workflows/mkdocs.yaml/badge.svg)](https://github.com/reproducible-reporting/stepup-reprep/actions/workflows/mkdocs.yaml)
 [![PyPI Version](https://img.shields.io/pypi/v/stepup-reprep)](https://pypi.org/project/stepup-reprep/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/stepup-reprep)
 ![GPL-3 License](https://img.shields.io/github/license/reproducible-reporting/stepup-reprep)
 
 
 # StepUp RepRep
```

### Comparing `stepup_reprep-1.1.0/stepup_reprep.egg-info/SOURCES.txt` & `stepup_reprep-1.1.1/stepup_reprep.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -10,34 +10,35 @@
 .github/workflows/release.yaml
 docs/changelog.md
 docs/clean_stdout.sed
 docs/development.md
 docs/index.md
 docs/installation.md
 docs/license.md
+docs/advanced_topics/good_practices.md
+docs/advanced_topics/manifest_files.md
+docs/advanced_topics/tiling_pdfs.md
+docs/advanced_topics/tiling_pdfs/.gitignore
+docs/advanced_topics/tiling_pdfs/figure.png
+docs/advanced_topics/tiling_pdfs/hexagon.svg
+docs/advanced_topics/tiling_pdfs/main.sh
+docs/advanced_topics/tiling_pdfs/pentagon.svg
+docs/advanced_topics/tiling_pdfs/plan.py
+docs/advanced_topics/tiling_pdfs/square.svg
+docs/advanced_topics/tiling_pdfs/stdout.txt
+docs/advanced_topics/tiling_pdfs/tile.py
+docs/advanced_topics/tiling_pdfs/triangle.svg
+docs/from_scratch/introduction.md
+docs/from_template/before_you_begin.md
+docs/from_template/create_or_clone_a_project.md
+docs/from_template/introduction.md
+docs/from_template/working_on_a_project.md
 docs/reference/stepup.reprep.api.md
 docs/reference/stepup.reprep.tile_pdf.md
-docs/tutorials/before_you_begin.md
-docs/tutorials/create_or_clone_a_project.md
-docs/tutorials/manifest_files.md
-docs/tutorials/template_conventions.md
-docs/tutorials/tiling_pdfs.md
-docs/tutorials/working_on_a_project.md
-docs/tutorials/tiling_pdfs/.gitignore
-docs/tutorials/tiling_pdfs/figure.png
-docs/tutorials/tiling_pdfs/hexagon.svg
-docs/tutorials/tiling_pdfs/main.sh
-docs/tutorials/tiling_pdfs/pentagon.svg
-docs/tutorials/tiling_pdfs/plan.py
-docs/tutorials/tiling_pdfs/square.svg
-docs/tutorials/tiling_pdfs/stdout.txt
-docs/tutorials/tiling_pdfs/tile.py
-docs/tutorials/tiling_pdfs/triangle.svg
 stepup/reprep/__init__.py
-stepup/reprep/_version.py
 stepup/reprep/add_notes_pdf.py
 stepup/reprep/api.py
 stepup/reprep/bibtex_log.py
 stepup/reprep/check_hrefs.py
 stepup/reprep/check_manifest.py
 stepup/reprep/convert_inkscape.py
 stepup/reprep/convert_markdown.py
@@ -112,21 +113,49 @@
 tests/cases/convert_inkscape/README.md
 tests/cases/convert_inkscape/expected_graph.txt
 tests/cases/convert_inkscape/expected_stdout.txt
 tests/cases/convert_inkscape/glasses.svg
 tests/cases/convert_inkscape/main.sh
 tests/cases/convert_inkscape/plan.py
 tests/cases/convert_inkscape/smile.svg
+tests/cases/convert_inkscape_concurrency/.gitignore
+tests/cases/convert_inkscape_concurrency/README.md
+tests/cases/convert_inkscape_concurrency/dots_050.svg
+tests/cases/convert_inkscape_concurrency/dots_055.svg
+tests/cases/convert_inkscape_concurrency/dots_060.svg
+tests/cases/convert_inkscape_concurrency/dots_065.svg
+tests/cases/convert_inkscape_concurrency/dots_070.svg
+tests/cases/convert_inkscape_concurrency/dots_075.svg
+tests/cases/convert_inkscape_concurrency/dots_080.svg
+tests/cases/convert_inkscape_concurrency/dots_085.svg
+tests/cases/convert_inkscape_concurrency/dots_090.svg
+tests/cases/convert_inkscape_concurrency/dots_095.svg
+tests/cases/convert_inkscape_concurrency/dots_100.svg
+tests/cases/convert_inkscape_concurrency/dots_105.svg
+tests/cases/convert_inkscape_concurrency/dots_110.svg
+tests/cases/convert_inkscape_concurrency/dots_115.svg
+tests/cases/convert_inkscape_concurrency/dots_120.svg
+tests/cases/convert_inkscape_concurrency/dots_125.svg
+tests/cases/convert_inkscape_concurrency/dots_130.svg
+tests/cases/convert_inkscape_concurrency/dots_135.svg
+tests/cases/convert_inkscape_concurrency/dots_140.svg
+tests/cases/convert_inkscape_concurrency/dots_145.svg
+tests/cases/convert_inkscape_concurrency/main.sh
+tests/cases/convert_inkscape_concurrency/plan.py
 tests/cases/convert_libreoffice/.gitignore
 tests/cases/convert_libreoffice/README.md
 tests/cases/convert_libreoffice/expected_graph.txt
 tests/cases/convert_libreoffice/expected_stdout.txt
 tests/cases/convert_libreoffice/main.sh
 tests/cases/convert_libreoffice/plan.py
 tests/cases/convert_libreoffice/slide.odp
+tests/cases/convert_libreoffice_concurrency/.gitignore
+tests/cases/convert_libreoffice_concurrency/main.sh
+tests/cases/convert_libreoffice_concurrency/plan.py
+tests/cases/convert_libreoffice_concurrency/something.odt
 tests/cases/convert_markdown/.gitignore
 tests/cases/convert_markdown/README.md
 tests/cases/convert_markdown/demo.md
 tests/cases/convert_markdown/expected_graph.txt
 tests/cases/convert_markdown/expected_stdout.txt
 tests/cases/convert_markdown/main.sh
 tests/cases/convert_markdown/plan.py
```

### Comparing `stepup_reprep-1.1.0/tests/cases/add_notes_pdf/expected_graph.txt` & `stepup_reprep-1.1.1/tests/cases/add_notes_pdf/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/add_notes_pdf/expected_stdout.txt` & `stepup_reprep-1.1.1/tests/cases/add_notes_pdf/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/add_notes_pdf/main.sh` & `stepup_reprep-1.1.1/tests/cases/add_notes_pdf/main.sh`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/add_notes_pdf/notes.pdf` & `stepup_reprep-1.1.1/tests/cases/add_notes_pdf/notes.pdf`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/add_notes_pdf/src.pdf` & `stepup_reprep-1.1.1/tests/cases/add_notes_pdf/src.pdf`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/cat_pdf/doc1.pdf` & `stepup_reprep-1.1.1/tests/cases/cat_pdf/doc1.pdf`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/cat_pdf/doc2.pdf` & `stepup_reprep-1.1.1/tests/cases/cat_pdf/doc2.pdf`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/cat_pdf/expected_graph.txt` & `stepup_reprep-1.1.1/tests/cases/cat_pdf/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/cat_pdf/expected_stdout.txt` & `stepup_reprep-1.1.1/tests/cases/cat_pdf/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/cat_pdf/main.sh` & `stepup_reprep-1.1.1/tests/cases/cat_pdf/main.sh`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/check_hrefs_html/expected_graph.txt` & `stepup_reprep-1.1.1/tests/cases/check_hrefs_html/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/check_hrefs_html/expected_stdout.txt` & `stepup_reprep-1.1.1/tests/cases/check_hrefs_html/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/check_hrefs_html/main.sh` & `stepup_reprep-1.1.1/tests/cases/check_hrefs_html/main.sh`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/check_hrefs_html/test.html` & `stepup_reprep-1.1.1/tests/cases/check_hrefs_html/test.html`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/check_hrefs_md/expected_graph.txt` & `stepup_reprep-1.1.1/tests/cases/check_hrefs_md/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/check_hrefs_md/expected_stdout.txt` & `stepup_reprep-1.1.1/tests/cases/check_hrefs_md/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/check_hrefs_md/main.sh` & `stepup_reprep-1.1.1/tests/cases/check_hrefs_md/main.sh`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/check_hrefs_pdf/expected_graph.txt` & `stepup_reprep-1.1.1/tests/cases/check_hrefs_pdf/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/check_hrefs_pdf/expected_stdout.txt` & `stepup_reprep-1.1.1/tests/cases/check_hrefs_pdf/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/check_hrefs_pdf/main.sh` & `stepup_reprep-1.1.1/tests/cases/check_hrefs_pdf/main.sh`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/check_hrefs_pdf/main.tex` & `stepup_reprep-1.1.1/tests/cases/check_hrefs_pdf/main.tex`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/convert_inkscape/expected_graph.txt` & `stepup_reprep-1.1.1/tests/cases/convert_inkscape/expected_graph.txt`

 * *Files 6% similar despite different names*

```diff
@@ -17,18 +17,18 @@
           created by   root:
             supplies   file:final.pdf
             supplies   file:glasses.png
             supplies   file:glasses.svg
             supplies   file:plan.py
             supplies   file:smile.svg
             supplies   step:./plan.py
-            supplies   step:inkscape glasses.svg  --export-filename=glasses.png --export-type=png
-            supplies   step:inkscape smile.svg  --export-filename=final.pdf --export-type=pdf
             supplies   step:python -m stepup.reprep.convert_inkscape glasses.svg glasses.png --optional
             supplies   step:python -m stepup.reprep.convert_inkscape smile.svg final.pdf
+            supplies   step:unshare --user inkscape glasses.svg  --export-filename=glasses.png --export-type=png
+            supplies   step:unshare --user inkscape smile.svg  --export-filename=final.pdf --export-type=pdf
 
 step:./plan.py
              workdir = ./
              command = ./plan.py
                state = SUCCEEDED
           created by   root:
             consumes   file:./
@@ -39,78 +39,76 @@
              creates   step:python -m stepup.reprep.convert_inkscape smile.svg final.pdf
 
 file:glasses.svg
                 path = glasses.svg
                state = STATIC
           created by   step:./plan.py
             consumes   file:./
-            supplies   step:inkscape glasses.svg  --export-filename=glasses.png --export-type=png
             supplies   step:python -m stepup.reprep.convert_inkscape glasses.svg glasses.png --optional
+            supplies   step:unshare --user inkscape glasses.svg  --export-filename=glasses.png --export-type=png
 
 file:smile.svg
                 path = smile.svg
                state = STATIC
           created by   step:./plan.py
             consumes   file:./
-            supplies   step:inkscape smile.svg  --export-filename=final.pdf --export-type=pdf
             supplies   step:python -m stepup.reprep.convert_inkscape smile.svg final.pdf
+            supplies   step:unshare --user inkscape smile.svg  --export-filename=final.pdf --export-type=pdf
 
 step:python -m stepup.reprep.convert_inkscape glasses.svg glasses.png --optional
              workdir = ./
              command = python -m stepup.reprep.convert_inkscape glasses.svg glasses.png --optional
                state = SUCCEEDED
    env_var (amended) = REPREP_INKSCAPE
                      = REPREP_INKSCAPE_PNG_ARGS
           created by   step:./plan.py
             consumes   file:./
             consumes   file:glasses.svg
-             creates   step:inkscape glasses.svg  --export-filename=glasses.png --export-type=png
+             creates   step:unshare --user inkscape glasses.svg  --export-filename=glasses.png --export-type=png
 
 step:python -m stepup.reprep.convert_inkscape smile.svg final.pdf
              workdir = ./
              command = python -m stepup.reprep.convert_inkscape smile.svg final.pdf
                state = SUCCEEDED
    env_var (amended) = REPREP_INKSCAPE
                      = REPREP_INKSCAPE_PDF_ARGS
           created by   step:./plan.py
             consumes   file:./
             consumes   file:smile.svg
-             creates   step:inkscape smile.svg  --export-filename=final.pdf --export-type=pdf
+             creates   step:unshare --user inkscape smile.svg  --export-filename=final.pdf --export-type=pdf
 
-step:inkscape glasses.svg  --export-filename=glasses.png --export-type=png
+step:unshare --user inkscape glasses.svg  --export-filename=glasses.png --export-type=png
              workdir = ./
-             command = inkscape glasses.svg  --export-filename=glasses.png --export-type=png
+             command = unshare --user inkscape glasses.svg  --export-filename=glasses.png --export-type=png
                state = SUCCEEDED
            mandatory = IMPLIED
-                pool = inkscape
           created by   step:python -m stepup.reprep.convert_inkscape glasses.svg glasses.png --optional
             consumes   file:./
             consumes   file:glasses.svg
              creates   file:glasses.png
             supplies   file:glasses.png
 
 file:glasses.png
                 path = glasses.png
                state = BUILT
-          created by   step:inkscape glasses.svg  --export-filename=glasses.png --export-type=png
+          created by   step:unshare --user inkscape glasses.svg  --export-filename=glasses.png --export-type=png
             consumes   file:./
-            consumes   step:inkscape glasses.svg  --export-filename=glasses.png --export-type=png
-            supplies   step:inkscape smile.svg  --export-filename=final.pdf --export-type=pdf
+            consumes   step:unshare --user inkscape glasses.svg  --export-filename=glasses.png --export-type=png
+            supplies   step:unshare --user inkscape smile.svg  --export-filename=final.pdf --export-type=pdf
 
-step:inkscape smile.svg  --export-filename=final.pdf --export-type=pdf
+step:unshare --user inkscape smile.svg  --export-filename=final.pdf --export-type=pdf
              workdir = ./
-             command = inkscape smile.svg  --export-filename=final.pdf --export-type=pdf
+             command = unshare --user inkscape smile.svg  --export-filename=final.pdf --export-type=pdf
                state = SUCCEEDED
-                pool = inkscape
           created by   step:python -m stepup.reprep.convert_inkscape smile.svg final.pdf
             consumes   file:./
             consumes   file:glasses.png
             consumes   file:smile.svg
              creates   file:final.pdf
             supplies   file:final.pdf
 
 file:final.pdf
                 path = final.pdf
                state = BUILT
-          created by   step:inkscape smile.svg  --export-filename=final.pdf --export-type=pdf
+          created by   step:unshare --user inkscape smile.svg  --export-filename=final.pdf --export-type=pdf
             consumes   file:./
-            consumes   step:inkscape smile.svg  --export-filename=final.pdf --export-type=pdf
+            consumes   step:unshare --user inkscape smile.svg  --export-filename=final.pdf --export-type=pdf
```

### Comparing `stepup_reprep-1.1.0/tests/cases/convert_inkscape/expected_stdout.txt` & `stepup_reprep-1.1.1/tests/cases/convert_inkscape/expected_stdout.txt`

 * *Files 12% similar despite different names*

```diff
@@ -2,28 +2,24 @@
      PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
      START │ python -m stepup.reprep.convert_inkscape glasses.svg glasses.png --optional
    SUCCESS │ python -m stepup.reprep.convert_inkscape glasses.svg glasses.png --optional
      START │ python -m stepup.reprep.convert_inkscape smile.svg final.pdf
    SUCCESS │ python -m stepup.reprep.convert_inkscape smile.svg final.pdf
-     START │ inkscape glasses.svg  --export-filename=glasses.png --export-type=png
-   SUCCESS │ inkscape glasses.svg  --export-filename=glasses.png --export-type=png
-     START │ inkscape smile.svg  --export-filename=final.pdf --export-type=pdf
-   SUCCESS │ inkscape smile.svg  --export-filename=final.pdf --export-type=pdf
+     START │ unshare --user inkscape glasses.svg  --export-filename=glasses.png --export-type=png
+   SUCCESS │ unshare --user inkscape glasses.svg  --export-filename=glasses.png --export-type=png
+     START │ unshare --user inkscape smile.svg  --export-filename=final.pdf --export-type=pdf
+   SUCCESS │ unshare --user inkscape smile.svg  --export-filename=final.pdf --export-type=pdf
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
-   UPDATED │ glasses.svg
-   UPDATED │ smile.svg
      PHASE │ watch
    DELETED │ final.pdf
    DELETED │ glasses.png
      PHASE │ run
-      SKIP │ python -m stepup.reprep.convert_inkscape glasses.svg glasses.png --optional
-      SKIP │ python -m stepup.reprep.convert_inkscape smile.svg final.pdf
-     START │ inkscape glasses.svg  --export-filename=glasses.png --export-type=png
-   SUCCESS │ inkscape glasses.svg  --export-filename=glasses.png --export-type=png
-     START │ inkscape smile.svg  --export-filename=final.pdf --export-type=pdf
-   SUCCESS │ inkscape smile.svg  --export-filename=final.pdf --export-type=pdf
+     START │ unshare --user inkscape glasses.svg  --export-filename=glasses.png --export-type=png
+   SUCCESS │ unshare --user inkscape glasses.svg  --export-filename=glasses.png --export-type=png
+     START │ unshare --user inkscape smile.svg  --export-filename=final.pdf --export-type=pdf
+   SUCCESS │ unshare --user inkscape smile.svg  --export-filename=final.pdf --export-type=pdf
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
      PHASE │ watch
   DIRECTOR │ Stopping workers.
   DIRECTOR │ See you!
```

### Comparing `stepup_reprep-1.1.0/tests/cases/convert_inkscape/glasses.svg` & `stepup_reprep-1.1.1/tests/cases/convert_inkscape/glasses.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/convert_inkscape/main.sh` & `stepup_reprep-1.1.1/tests/cases/convert_inkscape/main.sh`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/convert_inkscape/smile.svg` & `stepup_reprep-1.1.1/tests/cases/convert_inkscape/smile.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/convert_libreoffice/expected_graph.txt` & `stepup_reprep-1.1.1/tests/cases/convert_libreoffice/expected_graph.txt`

 * *Files 23% similar despite different names*

```diff
@@ -15,44 +15,43 @@
                 path = ./
                state = STATIC
           created by   root:
             supplies   file:plan.py
             supplies   file:slide.odp
             supplies   file:slide.pdf
             supplies   step:./plan.py
-            supplies   step:WORK=`mktemp -d --suffix=reprep` && libreoffice --convert-to pdf slide.odp --outdir ${WORK} > /dev/null && cp ${WORK}/*.pdf slide.pdf && rm -r ${WORK}
+            supplies   step:WORK=`mktemp -d --suffix=reprep` && libreoffice -env:UserInstallation=file://${WORK} --convert-to pdf slide.odp --outdir ${WORK} > /dev/null && cp ${WORK}/*.pdf slide.pdf && rm -r ${WORK}
 
 step:./plan.py
              workdir = ./
              command = ./plan.py
                state = SUCCEEDED
    env_var (amended) = REPREP_LIBREOFFICE
           created by   root:
             consumes   file:./
             consumes   file:plan.py
              creates   file:slide.odp
-             creates   step:WORK=`mktemp -d --suffix=reprep` && libreoffice --convert-to pdf slide.odp --outdir ${WORK} > /dev/null && cp ${WORK}/*.pdf slide.pdf && rm -r ${WORK}
+             creates   step:WORK=`mktemp -d --suffix=reprep` && libreoffice -env:UserInstallation=file://${WORK} --convert-to pdf slide.odp --outdir ${WORK} > /dev/null && cp ${WORK}/*.pdf slide.pdf && rm -r ${WORK}
 
 file:slide.odp
                 path = slide.odp
                state = STATIC
           created by   step:./plan.py
             consumes   file:./
-            supplies   step:WORK=`mktemp -d --suffix=reprep` && libreoffice --convert-to pdf slide.odp --outdir ${WORK} > /dev/null && cp ${WORK}/*.pdf slide.pdf && rm -r ${WORK}
+            supplies   step:WORK=`mktemp -d --suffix=reprep` && libreoffice -env:UserInstallation=file://${WORK} --convert-to pdf slide.odp --outdir ${WORK} > /dev/null && cp ${WORK}/*.pdf slide.pdf && rm -r ${WORK}
 
-step:WORK=`mktemp -d --suffix=reprep` && libreoffice --convert-to pdf slide.odp --outdir ${WORK} > /dev/null && cp ${WORK}/*.pdf slide.pdf && rm -r ${WORK}
+step:WORK=`mktemp -d --suffix=reprep` && libreoffice -env:UserInstallation=file://${WORK} --convert-to pdf slide.odp --outdir ${WORK} > /dev/null && cp ${WORK}/*.pdf slide.pdf && rm -r ${WORK}
              workdir = ./
-             command = WORK=`mktemp -d --suffix=reprep` && libreoffice --convert-to pdf slide.odp --outdir ${WORK} > /dev/null && cp ${WORK}/*.pdf slide.pdf && rm -r ${WORK}
+             command = WORK=`mktemp -d --suffix=reprep` && libreoffice -env:UserInstallation=file://${WORK} --convert-to pdf slide.odp --outdir ${WORK} > /dev/null && cp ${WORK}/*.pdf slide.pdf && rm -r ${WORK}
                state = SUCCEEDED
-                pool = libreoffice
           created by   step:./plan.py
             consumes   file:./
             consumes   file:slide.odp
              creates   file:slide.pdf
             supplies   file:slide.pdf
 
 file:slide.pdf
                 path = slide.pdf
                state = BUILT
-          created by   step:WORK=`mktemp -d --suffix=reprep` && libreoffice --convert-to pdf slide.odp --outdir ${WORK} > /dev/null && cp ${WORK}/*.pdf slide.pdf && rm -r ${WORK}
+          created by   step:WORK=`mktemp -d --suffix=reprep` && libreoffice -env:UserInstallation=file://${WORK} --convert-to pdf slide.odp --outdir ${WORK} > /dev/null && cp ${WORK}/*.pdf slide.pdf && rm -r ${WORK}
             consumes   file:./
-            consumes   step:WORK=`mktemp -d --suffix=reprep` && libreoffice --convert-to pdf slide.odp --outdir ${WORK} > /dev/null && cp ${WORK}/*.pdf slide.pdf && rm -r ${WORK}
+            consumes   step:WORK=`mktemp -d --suffix=reprep` && libreoffice -env:UserInstallation=file://${WORK} --convert-to pdf slide.odp --outdir ${WORK} > /dev/null && cp ${WORK}/*.pdf slide.pdf && rm -r ${WORK}
```

### Comparing `stepup_reprep-1.1.0/tests/cases/convert_libreoffice/expected_stdout.txt` & `stepup_reprep-1.1.1/tests/cases/raster_pdf/expected_stdout.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,18 @@
   DIRECTOR │ Launched worker 0
      PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
-     START │ WORK=`mktemp -d --suffix=reprep` && libreoffice --convert-to pdf slide.odp --outdir ${WORK} > /dev/null && cp ${WORK}/*.pdf slide.pdf && rm -r ${WORK}
-   SUCCESS │ WORK=`mktemp -d --suffix=reprep` && libreoffice --convert-to pdf slide.odp --outdir ${WORK} > /dev/null && cp ${WORK}/*.pdf slide.pdf && rm -r ${WORK}
+     START │ mkdir -p rastered/
+   SUCCESS │ mkdir -p rastered/
+     START │ python -m stepup.reprep.raster_pdf smile.pdf rastered/smile.pdf
+   SUCCESS │ python -m stepup.reprep.raster_pdf smile.pdf rastered/smile.pdf
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
      PHASE │ watch
-   DELETED │ slide.pdf
+   DELETED │ rastered/smile.pdf
      PHASE │ run
-     START │ WORK=`mktemp -d --suffix=reprep` && libreoffice --convert-to pdf slide.odp --outdir ${WORK} > /dev/null && cp ${WORK}/*.pdf slide.pdf && rm -r ${WORK}
-   SUCCESS │ WORK=`mktemp -d --suffix=reprep` && libreoffice --convert-to pdf slide.odp --outdir ${WORK} > /dev/null && cp ${WORK}/*.pdf slide.pdf && rm -r ${WORK}
+     START │ python -m stepup.reprep.raster_pdf smile.pdf rastered/smile.pdf
+   SUCCESS │ python -m stepup.reprep.raster_pdf smile.pdf rastered/smile.pdf
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
      PHASE │ watch
   DIRECTOR │ Stopping workers.
   DIRECTOR │ See you!
```

### Comparing `stepup_reprep-1.1.0/tests/cases/convert_libreoffice/main.sh` & `stepup_reprep-1.1.1/tests/cases/convert_libreoffice/main.sh`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/convert_libreoffice/slide.odp` & `stepup_reprep-1.1.1/tests/cases/convert_libreoffice/slide.odp`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/convert_markdown/expected_graph.txt` & `stepup_reprep-1.1.1/tests/cases/convert_markdown/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/convert_markdown/expected_stdout.txt` & `stepup_reprep-1.1.1/tests/cases/convert_markdown/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/convert_markdown/main.sh` & `stepup_reprep-1.1.1/tests/cases/convert_markdown/main.sh`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/convert_mutool/example.pdf` & `stepup_reprep-1.1.1/tests/cases/convert_mutool/example.pdf`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/convert_mutool/expected_graph.txt` & `stepup_reprep-1.1.1/tests/cases/convert_mutool/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/convert_mutool/expected_stdout.txt` & `stepup_reprep-1.1.1/tests/cases/convert_mutool/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/convert_mutool/main.sh` & `stepup_reprep-1.1.1/tests/cases/convert_mutool/main.sh`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/convert_weasyprint/expected_graph.txt` & `stepup_reprep-1.1.1/tests/cases/convert_weasyprint/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/convert_weasyprint/expected_stdout.txt` & `stepup_reprep-1.1.1/tests/cases/convert_weasyprint/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/convert_weasyprint/main.sh` & `stepup_reprep-1.1.1/tests/cases/convert_weasyprint/main.sh`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/latex_diff/expected_graph.txt` & `stepup_reprep-1.1.1/tests/cases/latex_diff/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/latex_diff/expected_stdout.txt` & `stepup_reprep-1.1.1/tests/cases/latex_diff/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/latex_diff/main.sh` & `stepup_reprep-1.1.1/tests/cases/latex_diff/main.sh`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/latex_flat/expected_graph_01.txt` & `stepup_reprep-1.1.1/tests/cases/latex_flat/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/latex_flat/expected_graph_02.txt` & `stepup_reprep-1.1.1/tests/cases/latex_flat/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/latex_flat/expected_stdout_01.txt` & `stepup_reprep-1.1.1/tests/cases/latex_flat/expected_stdout_01.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/latex_flat/main.sh` & `stepup_reprep-1.1.1/tests/cases/latex_flat/main.sh`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/latex_flat_subdir/expected_graph.txt` & `stepup_reprep-1.1.1/tests/cases/latex_flat_subdir/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/latex_flat_subdir/main.sh` & `stepup_reprep-1.1.1/tests/cases/latex_flat_subdir/main.sh`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/lualatex_simple/expected_graph.txt` & `stepup_reprep-1.1.1/tests/cases/lualatex_simple/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/lualatex_simple/expected_stdout.txt` & `stepup_reprep-1.1.1/tests/cases/lualatex_simple/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/lualatex_simple/main.sh` & `stepup_reprep-1.1.1/tests/cases/lualatex_simple/main.sh`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/make_manifest_in/expected_graph.txt` & `stepup_reprep-1.1.1/tests/cases/make_manifest_in/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/make_manifest_in/main.sh` & `stepup_reprep-1.1.1/tests/cases/make_manifest_in/main.sh`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/make_manifest_in_sub/expected_graph.txt` & `stepup_reprep-1.1.1/tests/cases/make_manifest_in_sub/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/make_manifest_in_sub/main.sh` & `stepup_reprep-1.1.1/tests/cases/make_manifest_in_sub/main.sh`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/make_manifest_list/expected_graph.txt` & `stepup_reprep-1.1.1/tests/cases/make_manifest_list/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/make_manifest_list/main.sh` & `stepup_reprep-1.1.1/tests/cases/make_manifest_list/main.sh`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/nup_pdf/expected_graph.txt` & `stepup_reprep-1.1.1/tests/cases/nup_pdf/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/nup_pdf/expected_stdout.txt` & `stepup_reprep-1.1.1/tests/cases/nup_pdf/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/nup_pdf/main.sh` & `stepup_reprep-1.1.1/tests/cases/nup_pdf/main.sh`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/nup_pdf/src.pdf` & `stepup_reprep-1.1.1/tests/cases/nup_pdf/src.pdf`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/pdflatex_bbl/expected_graph.txt` & `stepup_reprep-1.1.1/tests/cases/pdflatex_bbl/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/pdflatex_bbl/expected_stdout.txt` & `stepup_reprep-1.1.1/tests/cases/pdflatex_bbl/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/pdflatex_bbl/main.sh` & `stepup_reprep-1.1.1/tests/cases/pdflatex_bbl/main.sh`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/pdflatex_bibtex/expected_graph.txt` & `stepup_reprep-1.1.1/tests/cases/pdflatex_bibtex/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/pdflatex_bibtex/expected_stdout.txt` & `stepup_reprep-1.1.1/tests/cases/pdflatex_bibtex/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/pdflatex_bibtex/main.sh` & `stepup_reprep-1.1.1/tests/cases/pdflatex_bibtex/main.sh`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/pdflatex_input/expected_graph.txt` & `stepup_reprep-1.1.1/tests/cases/pdflatex_input/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/pdflatex_input/expected_stdout.txt` & `stepup_reprep-1.1.1/tests/cases/pdflatex_input/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/pdflatex_input/main.sh` & `stepup_reprep-1.1.1/tests/cases/pdflatex_input/main.sh`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/pdflatex_input/smile.pdf` & `stepup_reprep-1.1.1/tests/cases/pdflatex_input/smile.pdf`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/raster_pdf/expected_graph.txt` & `stepup_reprep-1.1.1/tests/cases/raster_pdf/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/raster_pdf/main.sh` & `stepup_reprep-1.1.1/tests/cases/raster_pdf/main.sh`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/raster_pdf/smile.pdf` & `stepup_reprep-1.1.1/tests/cases/raster_pdf/smile.pdf`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/render_basic/expected_graph.txt` & `stepup_reprep-1.1.1/tests/cases/render_basic/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/render_basic/main.sh` & `stepup_reprep-1.1.1/tests/cases/render_basic/main.sh`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/render_relpath/expected_graph.txt` & `stepup_reprep-1.1.1/tests/cases/render_relpath/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/render_relpath/expected_stdout.txt` & `stepup_reprep-1.1.1/tests/cases/render_relpath/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/render_relpath/main.sh` & `stepup_reprep-1.1.1/tests/cases/render_relpath/main.sh`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/tile_pdf/expected_graph.txt` & `stepup_reprep-1.1.1/tests/cases/tile_pdf/expected_graph.txt`

 * *Files 12% similar despite different names*

```diff
@@ -30,26 +30,26 @@
             supplies   file:triangle.svg
             supplies   file:vera.ttf
             supplies   file:vertical.pdf
             supplies   file:vertical.svg
             supplies   step:./plan.py
             supplies   step:./tile.py plan
             supplies   step:./tile.py run
-            supplies   step:inkscape hexagon.svg  --export-filename=hexagon.pdf --export-type=pdf
-            supplies   step:inkscape horizontal.svg  --export-filename=horizontal.pdf --export-type=pdf
-            supplies   step:inkscape pentagon.svg  --export-filename=pentagon.pdf --export-type=pdf
-            supplies   step:inkscape square.svg  --export-filename=square.pdf --export-type=pdf
-            supplies   step:inkscape triangle.svg  --export-filename=triangle.pdf --export-type=pdf
-            supplies   step:inkscape vertical.svg  --export-filename=vertical.pdf --export-type=pdf
             supplies   step:python -m stepup.reprep.convert_inkscape hexagon.svg hexagon.pdf
             supplies   step:python -m stepup.reprep.convert_inkscape horizontal.svg horizontal.pdf
             supplies   step:python -m stepup.reprep.convert_inkscape pentagon.svg pentagon.pdf
             supplies   step:python -m stepup.reprep.convert_inkscape square.svg square.pdf
             supplies   step:python -m stepup.reprep.convert_inkscape triangle.svg triangle.pdf
             supplies   step:python -m stepup.reprep.convert_inkscape vertical.svg vertical.pdf
+            supplies   step:unshare --user inkscape hexagon.svg  --export-filename=hexagon.pdf --export-type=pdf
+            supplies   step:unshare --user inkscape horizontal.svg  --export-filename=horizontal.pdf --export-type=pdf
+            supplies   step:unshare --user inkscape pentagon.svg  --export-filename=pentagon.pdf --export-type=pdf
+            supplies   step:unshare --user inkscape square.svg  --export-filename=square.pdf --export-type=pdf
+            supplies   step:unshare --user inkscape triangle.svg  --export-filename=triangle.pdf --export-type=pdf
+            supplies   step:unshare --user inkscape vertical.svg  --export-filename=vertical.pdf --export-type=pdf
 
 step:./plan.py
              workdir = ./
              command = ./plan.py
                state = SUCCEEDED
                  ngm = ['*.svg'] {}
           created by   root:
@@ -72,122 +72,122 @@
              creates   step:python -m stepup.reprep.convert_inkscape vertical.svg vertical.pdf
 
 file:hexagon.svg
                 path = hexagon.svg
                state = STATIC
           created by   step:./plan.py
             consumes   file:./
-            supplies   step:inkscape hexagon.svg  --export-filename=hexagon.pdf --export-type=pdf
             supplies   step:python -m stepup.reprep.convert_inkscape hexagon.svg hexagon.pdf
+            supplies   step:unshare --user inkscape hexagon.svg  --export-filename=hexagon.pdf --export-type=pdf
 
 file:horizontal.svg
                 path = horizontal.svg
                state = STATIC
           created by   step:./plan.py
             consumes   file:./
-            supplies   step:inkscape horizontal.svg  --export-filename=horizontal.pdf --export-type=pdf
             supplies   step:python -m stepup.reprep.convert_inkscape horizontal.svg horizontal.pdf
+            supplies   step:unshare --user inkscape horizontal.svg  --export-filename=horizontal.pdf --export-type=pdf
 
 file:pentagon.svg
                 path = pentagon.svg
                state = STATIC
           created by   step:./plan.py
             consumes   file:./
-            supplies   step:inkscape pentagon.svg  --export-filename=pentagon.pdf --export-type=pdf
             supplies   step:python -m stepup.reprep.convert_inkscape pentagon.svg pentagon.pdf
+            supplies   step:unshare --user inkscape pentagon.svg  --export-filename=pentagon.pdf --export-type=pdf
 
 file:square.svg
                 path = square.svg
                state = STATIC
           created by   step:./plan.py
             consumes   file:./
-            supplies   step:inkscape square.svg  --export-filename=square.pdf --export-type=pdf
             supplies   step:python -m stepup.reprep.convert_inkscape square.svg square.pdf
+            supplies   step:unshare --user inkscape square.svg  --export-filename=square.pdf --export-type=pdf
 
 file:triangle.svg
                 path = triangle.svg
                state = STATIC
           created by   step:./plan.py
             consumes   file:./
-            supplies   step:inkscape triangle.svg  --export-filename=triangle.pdf --export-type=pdf
             supplies   step:python -m stepup.reprep.convert_inkscape triangle.svg triangle.pdf
+            supplies   step:unshare --user inkscape triangle.svg  --export-filename=triangle.pdf --export-type=pdf
 
 file:vertical.svg
                 path = vertical.svg
                state = STATIC
           created by   step:./plan.py
             consumes   file:./
-            supplies   step:inkscape vertical.svg  --export-filename=vertical.pdf --export-type=pdf
             supplies   step:python -m stepup.reprep.convert_inkscape vertical.svg vertical.pdf
+            supplies   step:unshare --user inkscape vertical.svg  --export-filename=vertical.pdf --export-type=pdf
 
 step:python -m stepup.reprep.convert_inkscape hexagon.svg hexagon.pdf
              workdir = ./
              command = python -m stepup.reprep.convert_inkscape hexagon.svg hexagon.pdf
                state = SUCCEEDED
    env_var (amended) = REPREP_INKSCAPE
                      = REPREP_INKSCAPE_PDF_ARGS
           created by   step:./plan.py
             consumes   file:./
             consumes   file:hexagon.svg
-             creates   step:inkscape hexagon.svg  --export-filename=hexagon.pdf --export-type=pdf
+             creates   step:unshare --user inkscape hexagon.svg  --export-filename=hexagon.pdf --export-type=pdf
 
 step:python -m stepup.reprep.convert_inkscape horizontal.svg horizontal.pdf
              workdir = ./
              command = python -m stepup.reprep.convert_inkscape horizontal.svg horizontal.pdf
                state = SUCCEEDED
    env_var (amended) = REPREP_INKSCAPE
                      = REPREP_INKSCAPE_PDF_ARGS
           created by   step:./plan.py
             consumes   file:./
             consumes   file:horizontal.svg
-             creates   step:inkscape horizontal.svg  --export-filename=horizontal.pdf --export-type=pdf
+             creates   step:unshare --user inkscape horizontal.svg  --export-filename=horizontal.pdf --export-type=pdf
 
 step:python -m stepup.reprep.convert_inkscape pentagon.svg pentagon.pdf
              workdir = ./
              command = python -m stepup.reprep.convert_inkscape pentagon.svg pentagon.pdf
                state = SUCCEEDED
    env_var (amended) = REPREP_INKSCAPE
                      = REPREP_INKSCAPE_PDF_ARGS
           created by   step:./plan.py
             consumes   file:./
             consumes   file:pentagon.svg
-             creates   step:inkscape pentagon.svg  --export-filename=pentagon.pdf --export-type=pdf
+             creates   step:unshare --user inkscape pentagon.svg  --export-filename=pentagon.pdf --export-type=pdf
 
 step:python -m stepup.reprep.convert_inkscape square.svg square.pdf
              workdir = ./
              command = python -m stepup.reprep.convert_inkscape square.svg square.pdf
                state = SUCCEEDED
    env_var (amended) = REPREP_INKSCAPE
                      = REPREP_INKSCAPE_PDF_ARGS
           created by   step:./plan.py
             consumes   file:./
             consumes   file:square.svg
-             creates   step:inkscape square.svg  --export-filename=square.pdf --export-type=pdf
+             creates   step:unshare --user inkscape square.svg  --export-filename=square.pdf --export-type=pdf
 
 step:python -m stepup.reprep.convert_inkscape triangle.svg triangle.pdf
              workdir = ./
              command = python -m stepup.reprep.convert_inkscape triangle.svg triangle.pdf
                state = SUCCEEDED
    env_var (amended) = REPREP_INKSCAPE
                      = REPREP_INKSCAPE_PDF_ARGS
           created by   step:./plan.py
             consumes   file:./
             consumes   file:triangle.svg
-             creates   step:inkscape triangle.svg  --export-filename=triangle.pdf --export-type=pdf
+             creates   step:unshare --user inkscape triangle.svg  --export-filename=triangle.pdf --export-type=pdf
 
 step:python -m stepup.reprep.convert_inkscape vertical.svg vertical.pdf
              workdir = ./
              command = python -m stepup.reprep.convert_inkscape vertical.svg vertical.pdf
                state = SUCCEEDED
    env_var (amended) = REPREP_INKSCAPE
                      = REPREP_INKSCAPE_PDF_ARGS
           created by   step:./plan.py
             consumes   file:./
             consumes   file:vertical.svg
-             creates   step:inkscape vertical.svg  --export-filename=vertical.pdf --export-type=pdf
+             creates   step:unshare --user inkscape vertical.svg  --export-filename=vertical.pdf --export-type=pdf
 
 file:tile.py
                 path = tile.py
                state = STATIC
           created by   step:./plan.py
             consumes   file:./
             supplies   step:./tile.py plan
@@ -205,126 +205,120 @@
              command = ./tile.py plan
                state = SUCCEEDED
           created by   step:./plan.py
             consumes   file:./
             consumes   file:tile.py
              creates   step:./tile.py run
 
-step:inkscape hexagon.svg  --export-filename=hexagon.pdf --export-type=pdf
+step:unshare --user inkscape hexagon.svg  --export-filename=hexagon.pdf --export-type=pdf
              workdir = ./
-             command = inkscape hexagon.svg  --export-filename=hexagon.pdf --export-type=pdf
+             command = unshare --user inkscape hexagon.svg  --export-filename=hexagon.pdf --export-type=pdf
                state = SUCCEEDED
-                pool = inkscape
           created by   step:python -m stepup.reprep.convert_inkscape hexagon.svg hexagon.pdf
             consumes   file:./
             consumes   file:hexagon.svg
              creates   file:hexagon.pdf
             supplies   file:hexagon.pdf
 
 file:hexagon.pdf
                 path = hexagon.pdf
                state = BUILT
-          created by   step:inkscape hexagon.svg  --export-filename=hexagon.pdf --export-type=pdf
+          created by   step:unshare --user inkscape hexagon.svg  --export-filename=hexagon.pdf --export-type=pdf
             consumes   file:./
-            consumes   step:inkscape hexagon.svg  --export-filename=hexagon.pdf --export-type=pdf
+            consumes   step:unshare --user inkscape hexagon.svg  --export-filename=hexagon.pdf --export-type=pdf
             supplies   step:./tile.py run
 
-step:inkscape horizontal.svg  --export-filename=horizontal.pdf --export-type=pdf
+step:unshare --user inkscape horizontal.svg  --export-filename=horizontal.pdf --export-type=pdf
              workdir = ./
-             command = inkscape horizontal.svg  --export-filename=horizontal.pdf --export-type=pdf
+             command = unshare --user inkscape horizontal.svg  --export-filename=horizontal.pdf --export-type=pdf
                state = SUCCEEDED
-                pool = inkscape
           created by   step:python -m stepup.reprep.convert_inkscape horizontal.svg horizontal.pdf
             consumes   file:./
             consumes   file:horizontal.svg
              creates   file:horizontal.pdf
             supplies   file:horizontal.pdf
 
 file:horizontal.pdf
                 path = horizontal.pdf
                state = BUILT
-          created by   step:inkscape horizontal.svg  --export-filename=horizontal.pdf --export-type=pdf
+          created by   step:unshare --user inkscape horizontal.svg  --export-filename=horizontal.pdf --export-type=pdf
             consumes   file:./
-            consumes   step:inkscape horizontal.svg  --export-filename=horizontal.pdf --export-type=pdf
+            consumes   step:unshare --user inkscape horizontal.svg  --export-filename=horizontal.pdf --export-type=pdf
             supplies   step:./tile.py run
 
-step:inkscape pentagon.svg  --export-filename=pentagon.pdf --export-type=pdf
+step:unshare --user inkscape pentagon.svg  --export-filename=pentagon.pdf --export-type=pdf
              workdir = ./
-             command = inkscape pentagon.svg  --export-filename=pentagon.pdf --export-type=pdf
+             command = unshare --user inkscape pentagon.svg  --export-filename=pentagon.pdf --export-type=pdf
                state = SUCCEEDED
-                pool = inkscape
           created by   step:python -m stepup.reprep.convert_inkscape pentagon.svg pentagon.pdf
             consumes   file:./
             consumes   file:pentagon.svg
              creates   file:pentagon.pdf
             supplies   file:pentagon.pdf
 
 file:pentagon.pdf
                 path = pentagon.pdf
                state = BUILT
-          created by   step:inkscape pentagon.svg  --export-filename=pentagon.pdf --export-type=pdf
+          created by   step:unshare --user inkscape pentagon.svg  --export-filename=pentagon.pdf --export-type=pdf
             consumes   file:./
-            consumes   step:inkscape pentagon.svg  --export-filename=pentagon.pdf --export-type=pdf
+            consumes   step:unshare --user inkscape pentagon.svg  --export-filename=pentagon.pdf --export-type=pdf
             supplies   step:./tile.py run
 
-step:inkscape square.svg  --export-filename=square.pdf --export-type=pdf
+step:unshare --user inkscape square.svg  --export-filename=square.pdf --export-type=pdf
              workdir = ./
-             command = inkscape square.svg  --export-filename=square.pdf --export-type=pdf
+             command = unshare --user inkscape square.svg  --export-filename=square.pdf --export-type=pdf
                state = SUCCEEDED
-                pool = inkscape
           created by   step:python -m stepup.reprep.convert_inkscape square.svg square.pdf
             consumes   file:./
             consumes   file:square.svg
              creates   file:square.pdf
             supplies   file:square.pdf
 
 file:square.pdf
                 path = square.pdf
                state = BUILT
-          created by   step:inkscape square.svg  --export-filename=square.pdf --export-type=pdf
+          created by   step:unshare --user inkscape square.svg  --export-filename=square.pdf --export-type=pdf
             consumes   file:./
-            consumes   step:inkscape square.svg  --export-filename=square.pdf --export-type=pdf
+            consumes   step:unshare --user inkscape square.svg  --export-filename=square.pdf --export-type=pdf
             supplies   step:./tile.py run
 
-step:inkscape triangle.svg  --export-filename=triangle.pdf --export-type=pdf
+step:unshare --user inkscape triangle.svg  --export-filename=triangle.pdf --export-type=pdf
              workdir = ./
-             command = inkscape triangle.svg  --export-filename=triangle.pdf --export-type=pdf
+             command = unshare --user inkscape triangle.svg  --export-filename=triangle.pdf --export-type=pdf
                state = SUCCEEDED
-                pool = inkscape
           created by   step:python -m stepup.reprep.convert_inkscape triangle.svg triangle.pdf
             consumes   file:./
             consumes   file:triangle.svg
              creates   file:triangle.pdf
             supplies   file:triangle.pdf
 
 file:triangle.pdf
                 path = triangle.pdf
                state = BUILT
-          created by   step:inkscape triangle.svg  --export-filename=triangle.pdf --export-type=pdf
+          created by   step:unshare --user inkscape triangle.svg  --export-filename=triangle.pdf --export-type=pdf
             consumes   file:./
-            consumes   step:inkscape triangle.svg  --export-filename=triangle.pdf --export-type=pdf
+            consumes   step:unshare --user inkscape triangle.svg  --export-filename=triangle.pdf --export-type=pdf
             supplies   step:./tile.py run
 
-step:inkscape vertical.svg  --export-filename=vertical.pdf --export-type=pdf
+step:unshare --user inkscape vertical.svg  --export-filename=vertical.pdf --export-type=pdf
              workdir = ./
-             command = inkscape vertical.svg  --export-filename=vertical.pdf --export-type=pdf
+             command = unshare --user inkscape vertical.svg  --export-filename=vertical.pdf --export-type=pdf
                state = SUCCEEDED
-                pool = inkscape
           created by   step:python -m stepup.reprep.convert_inkscape vertical.svg vertical.pdf
             consumes   file:./
             consumes   file:vertical.svg
              creates   file:vertical.pdf
             supplies   file:vertical.pdf
 
 file:vertical.pdf
                 path = vertical.pdf
                state = BUILT
-          created by   step:inkscape vertical.svg  --export-filename=vertical.pdf --export-type=pdf
+          created by   step:unshare --user inkscape vertical.svg  --export-filename=vertical.pdf --export-type=pdf
             consumes   file:./
-            consumes   step:inkscape vertical.svg  --export-filename=vertical.pdf --export-type=pdf
+            consumes   step:unshare --user inkscape vertical.svg  --export-filename=vertical.pdf --export-type=pdf
             supplies   step:./tile.py run
 
 step:./tile.py run
              workdir = ./
              command = ./tile.py run
                state = SUCCEEDED
           created by   step:./tile.py plan
```

### Comparing `stepup_reprep-1.1.0/tests/cases/tile_pdf/expected_stdout.txt` & `stepup_reprep-1.1.1/tests/cases/tile_pdf/expected_stdout.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,60 +1,42 @@
   DIRECTOR │ Launched worker 0
      PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
      START │ python -m stepup.reprep.convert_inkscape hexagon.svg hexagon.pdf
    SUCCESS │ python -m stepup.reprep.convert_inkscape hexagon.svg hexagon.pdf
-     START │ inkscape hexagon.svg  --export-filename=hexagon.pdf --export-type=pdf
-   SUCCESS │ inkscape hexagon.svg  --export-filename=hexagon.pdf --export-type=pdf
      START │ python -m stepup.reprep.convert_inkscape horizontal.svg horizontal.pdf
    SUCCESS │ python -m stepup.reprep.convert_inkscape horizontal.svg horizontal.pdf
-     START │ inkscape horizontal.svg  --export-filename=horizontal.pdf --export-type=pdf
-   SUCCESS │ inkscape horizontal.svg  --export-filename=horizontal.pdf --export-type=pdf
      START │ python -m stepup.reprep.convert_inkscape pentagon.svg pentagon.pdf
    SUCCESS │ python -m stepup.reprep.convert_inkscape pentagon.svg pentagon.pdf
-     START │ inkscape pentagon.svg  --export-filename=pentagon.pdf --export-type=pdf
-   SUCCESS │ inkscape pentagon.svg  --export-filename=pentagon.pdf --export-type=pdf
      START │ python -m stepup.reprep.convert_inkscape square.svg square.pdf
    SUCCESS │ python -m stepup.reprep.convert_inkscape square.svg square.pdf
-     START │ inkscape square.svg  --export-filename=square.pdf --export-type=pdf
-   SUCCESS │ inkscape square.svg  --export-filename=square.pdf --export-type=pdf
      START │ python -m stepup.reprep.convert_inkscape triangle.svg triangle.pdf
    SUCCESS │ python -m stepup.reprep.convert_inkscape triangle.svg triangle.pdf
-     START │ inkscape triangle.svg  --export-filename=triangle.pdf --export-type=pdf
-   SUCCESS │ inkscape triangle.svg  --export-filename=triangle.pdf --export-type=pdf
      START │ python -m stepup.reprep.convert_inkscape vertical.svg vertical.pdf
    SUCCESS │ python -m stepup.reprep.convert_inkscape vertical.svg vertical.pdf
-     START │ inkscape vertical.svg  --export-filename=vertical.pdf --export-type=pdf
-   SUCCESS │ inkscape vertical.svg  --export-filename=vertical.pdf --export-type=pdf
      START │ ./tile.py plan
    SUCCESS │ ./tile.py plan
+     START │ unshare --user inkscape hexagon.svg  --export-filename=hexagon.pdf --export-type=pdf
+   SUCCESS │ unshare --user inkscape hexagon.svg  --export-filename=hexagon.pdf --export-type=pdf
+     START │ unshare --user inkscape horizontal.svg  --export-filename=horizontal.pdf --export-type=pdf
+   SUCCESS │ unshare --user inkscape horizontal.svg  --export-filename=horizontal.pdf --export-type=pdf
+     START │ unshare --user inkscape pentagon.svg  --export-filename=pentagon.pdf --export-type=pdf
+   SUCCESS │ unshare --user inkscape pentagon.svg  --export-filename=pentagon.pdf --export-type=pdf
+     START │ unshare --user inkscape square.svg  --export-filename=square.pdf --export-type=pdf
+   SUCCESS │ unshare --user inkscape square.svg  --export-filename=square.pdf --export-type=pdf
+     START │ unshare --user inkscape triangle.svg  --export-filename=triangle.pdf --export-type=pdf
+   SUCCESS │ unshare --user inkscape triangle.svg  --export-filename=triangle.pdf --export-type=pdf
+     START │ unshare --user inkscape vertical.svg  --export-filename=vertical.pdf --export-type=pdf
+   SUCCESS │ unshare --user inkscape vertical.svg  --export-filename=vertical.pdf --export-type=pdf
      START │ ./tile.py run
    SUCCESS │ ./tile.py run
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
-   UPDATED │ hexagon.svg
-   UPDATED │ horizontal.svg
-   UPDATED │ pentagon.svg
-   UPDATED │ square.svg
-   UPDATED │ triangle.svg
-   UPDATED │ vertical.svg
      PHASE │ watch
    DELETED │ figure.pdf
      PHASE │ run
-      SKIP │ python -m stepup.reprep.convert_inkscape hexagon.svg hexagon.pdf
-      SKIP │ python -m stepup.reprep.convert_inkscape horizontal.svg horizontal.pdf
-      SKIP │ python -m stepup.reprep.convert_inkscape pentagon.svg pentagon.pdf
-      SKIP │ python -m stepup.reprep.convert_inkscape square.svg square.pdf
-      SKIP │ python -m stepup.reprep.convert_inkscape triangle.svg triangle.pdf
-      SKIP │ python -m stepup.reprep.convert_inkscape vertical.svg vertical.pdf
-      SKIP │ inkscape hexagon.svg  --export-filename=hexagon.pdf --export-type=pdf
-      SKIP │ inkscape horizontal.svg  --export-filename=horizontal.pdf --export-type=pdf
-      SKIP │ inkscape pentagon.svg  --export-filename=pentagon.pdf --export-type=pdf
-      SKIP │ inkscape square.svg  --export-filename=square.pdf --export-type=pdf
-      SKIP │ inkscape triangle.svg  --export-filename=triangle.pdf --export-type=pdf
-      SKIP │ inkscape vertical.svg  --export-filename=vertical.pdf --export-type=pdf
      START │ ./tile.py run
    SUCCESS │ ./tile.py run
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
      PHASE │ watch
   DIRECTOR │ Stopping workers.
   DIRECTOR │ See you!
```

### Comparing `stepup_reprep-1.1.0/tests/cases/tile_pdf/hexagon.svg` & `stepup_reprep-1.1.1/tests/cases/tile_pdf/hexagon.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/tile_pdf/horizontal.svg` & `stepup_reprep-1.1.1/tests/cases/tile_pdf/horizontal.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/tile_pdf/main.sh` & `stepup_reprep-1.1.1/tests/cases/tile_pdf/main.sh`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/tile_pdf/pentagon.svg` & `stepup_reprep-1.1.1/tests/cases/tile_pdf/pentagon.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/tile_pdf/square.svg` & `stepup_reprep-1.1.1/tests/cases/tile_pdf/square.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/tile_pdf/tile.py` & `stepup_reprep-1.1.1/tests/cases/tile_pdf/tile.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/tile_pdf/triangle.svg` & `stepup_reprep-1.1.1/tests/cases/tile_pdf/triangle.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/tile_pdf/vera.ttf` & `stepup_reprep-1.1.1/tests/cases/tile_pdf/vera.ttf`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/tile_pdf/vertical.svg` & `stepup_reprep-1.1.1/tests/cases/tile_pdf/vertical.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/xelatex_input/expected_graph.txt` & `stepup_reprep-1.1.1/tests/cases/xelatex_input/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/xelatex_input/expected_stdout.txt` & `stepup_reprep-1.1.1/tests/cases/xelatex_input/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/xelatex_input/main.sh` & `stepup_reprep-1.1.1/tests/cases/xelatex_input/main.sh`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/xelatex_input/smile.pdf` & `stepup_reprep-1.1.1/tests/cases/xelatex_input/smile.pdf`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/zip_manifest/expected_graph.txt` & `stepup_reprep-1.1.1/tests/cases/zip_manifest/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/zip_manifest/expected_stdout.txt` & `stepup_reprep-1.1.1/tests/cases/zip_manifest/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/cases/zip_manifest/main.sh` & `stepup_reprep-1.1.1/tests/cases/zip_manifest/main.sh`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/conftest.py` & `stepup_reprep-1.1.1/tests/conftest.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,14 +18,13 @@
 #
 # --
 """Pytest configuration."""
 
 import pytest
 from path import Path
 
-pytest.register_assert_rewrite("stepup.core.pytest")
-pytest.register_assert_rewrite("stepup.reprep.pytest")
+pytest.register_assert_rewrite("stepup.core.pytest", "stepup.reprep.pytest")
 
 
 @pytest.fixture
 def path_tmp(tmpdir: str) -> Path:
     return Path(tmpdir)
```

### Comparing `stepup_reprep-1.1.0/tests/reprep_common.py` & `stepup_reprep-1.1.1/tests/reprep_common.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
 # --
 """Utilities shared by several unit test modules."""
 
-
 import contextlib
 
 
 @contextlib.contextmanager
 def local_file(contents, filename, tmpdir):
     """Change to a temporary directory and create a file with given contents."""
     with contextlib.chdir(tmpdir):
```

### Comparing `stepup_reprep-1.1.0/tests/test_bibtex_log.py` & `stepup_reprep-1.1.1/tests/test_bibtex_log.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
 # --
 """Unit tests for stepup.reprep.bibtex_log"""
 
-
 from reprep_common import local_file
 
 from stepup.reprep.bibtex_log import DEFAULT_MESSAGE, parse_bibtex_log
 
 BIBTEX_BLG1 = """\
 This is BibTeX, Version 0.99d (TeX Live 2022/CVE-2023-32700 patched)
 Capacity: max_strings=200000, hash_size=200000, hash_prime=170003
```

### Comparing `stepup_reprep-1.1.0/tests/test_cases.py` & `stepup_reprep-1.1.1/tests/test_cases.py`

 * *Files 4% similar despite different names*

```diff
@@ -101,15 +101,15 @@
 async def test_latex_example(tmpdir, name: str):
     await run_example(Path("tests/cases") / name, tmpdir, OVERWRITE_EXPECTED)
 
 
 @pytest.mark.skipif(not shutil.which("inkscape"), reason="No Inkscape")
 @pytest.mark.parametrize(
     "name",
-    ["convert_inkscape", "tile_pdf"],
+    ["convert_inkscape", "convert_inkscape_concurrency", "tile_pdf"],
 )
 @pytest.mark.asyncio
 async def test_inkscape_example(tmpdir, name: str):
     await run_example(Path("tests/cases") / name, tmpdir, OVERWRITE_EXPECTED)
 
 
 @pytest.mark.skipif(not shutil.which("mutool"), reason="No Mutool")
@@ -121,12 +121,12 @@
 async def test_mutool_example(tmpdir, name: str):
     await run_example(Path("tests/cases") / name, tmpdir, OVERWRITE_EXPECTED)
 
 
 @pytest.mark.skipif(not shutil.which("libreoffice"), reason="No LibreOffice")
 @pytest.mark.parametrize(
     "name",
-    ["convert_libreoffice"],
+    ["convert_libreoffice", "convert_libreoffice_concurrency"],
 )
 @pytest.mark.asyncio
 async def test_libreoffice_example(tmpdir, name: str):
     await run_example(Path("tests/cases") / name, tmpdir, OVERWRITE_EXPECTED)
```

### Comparing `stepup_reprep-1.1.0/tests/test_latex_deps.py` & `stepup_reprep-1.1.1/tests/test_latex_deps.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
 # --
 """Unit tests for stepup.reprep.latex_deps"""
 
-
 from stepup.reprep.latex_deps import scan_latex_deps
 
 SCAN_LATEX_DEPS_EXAMPLE = r"""
 \input{foo.tex}
 %\includegraphics{not.pdf}
 \includegraphics{figure}
 \includegraphics{\thepage.png} %REPREPBUILD ignore
```

### Comparing `stepup_reprep-1.1.0/tests/test_latex_flat.py` & `stepup_reprep-1.1.1/tests/test_latex_flat.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
 # --
 """Unit tests for stepup.reprep.latex_flat"""
 
-
 from stepup.reprep.latex_flat import flatten_latex
 
 MAIN_TEX = r"""
 \begin{document}
 \input{table}
 \includegraphics{smile}\cite{knuth:1984}
 \import{sub}{foo.tex}
```

### Comparing `stepup_reprep-1.1.0/tests/test_latex_log.py` & `stepup_reprep-1.1.1/tests/test_latex_log.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/test_manifest.py` & `stepup_reprep-1.1.1/tests/test_manifest.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.0/tests/test_zip.py` & `stepup_reprep-1.1.1/tests/test_zip.py`

 * *Files identical despite different names*

