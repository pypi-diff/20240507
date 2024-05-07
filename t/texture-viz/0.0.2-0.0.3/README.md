# Comparing `tmp/texture_viz-0.0.2.tar.gz` & `tmp/texture_viz-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "texture_viz-0.0.2.tar", max compression
+gzip compressed data, was "texture_viz-0.0.3.tar", max compression
```

## Comparing `texture_viz-0.0.2.tar` & `texture_viz-0.0.3.tar`

### file list

```diff
@@ -1,117 +1,118 @@
--rw-r--r--   0        0        0     1076 2024-05-05 01:33:23.268126 texture_viz-0.0.2/README.md
--rw-r--r--   0        0        0      972 2024-05-06 21:09:20.876534 texture_viz-0.0.2/pyproject.toml
--rw-r--r--   0        0        0       62 2024-05-05 01:31:21.484411 texture_viz-0.0.2/texture/__init__.py
--rw-r--r--   0        0        0      118 2024-05-05 01:31:21.485088 texture_viz-0.0.2/texture/database/__init__.py
--rw-r--r--   0        0        0    11042 2024-05-06 19:36:30.468050 texture_viz-0.0.2/texture/database/connection.py
--rw-r--r--   0        0        0     6816 2024-05-06 16:46:57.768411 texture_viz-0.0.2/texture/database/example_data.py
--rw-r--r--   0        0        0    14409 2024-05-06 20:39:38.171724 texture_viz-0.0.2/texture/frontend/assets/abap-ad6e811d.js
--rw-r--r--   0        0        0     4198 2024-05-06 20:39:38.170735 texture_viz-0.0.2/texture/frontend/assets/apex-992ba105.js
--rw-r--r--   0        0        0     1094 2024-05-06 20:39:38.170386 texture_viz-0.0.2/texture/frontend/assets/azcli-2ae42e71.js
--rw-r--r--   0        0        0     2091 2024-05-06 20:39:38.170464 texture_viz-0.0.2/texture/frontend/assets/bat-638cac0f.js
--rw-r--r--   0        0        0     2782 2024-05-06 20:39:38.170728 texture_viz-0.0.2/texture/frontend/assets/bicep-389290ac.js
--rw-r--r--   0        0        0     2431 2024-05-06 20:39:38.170487 texture_viz-0.0.2/texture/frontend/assets/cameligo-e2b87a47.js
--rw-r--r--   0        0        0     9889 2024-05-06 20:39:38.171484 texture_viz-0.0.2/texture/frontend/assets/clojure-9f651a27.js
--rw-r--r--   0        0        0    79568 2024-05-06 20:39:38.170454 texture_viz-0.0.2/texture/frontend/assets/codicon-a3faa755.ttf
--rw-r--r--   0        0        0     3836 2024-05-06 20:39:38.170936 texture_viz-0.0.2/texture/frontend/assets/coffee-4e075114.js
--rw-r--r--   0        0        0     5680 2024-05-06 20:39:38.171510 texture_viz-0.0.2/texture/frontend/assets/cpp-8ffe77ae.js
--rw-r--r--   0        0        0     4770 2024-05-06 20:39:38.171506 texture_viz-0.0.2/texture/frontend/assets/csharp-0b267c6b.js
--rw-r--r--   0        0        0     1665 2024-05-06 20:39:38.170711 texture_viz-0.0.2/texture/frontend/assets/csp-c23415e1.js
--rw-r--r--   0        0        0     4756 2024-05-06 20:39:38.170915 texture_viz-0.0.2/texture/frontend/assets/css-c62f5578.js
--rw-r--r--   0        0        0   985422 2024-05-06 20:39:38.337449 texture_viz-0.0.2/texture/frontend/assets/css.worker-68e7a658.js
--rw-r--r--   0        0        0    33636 2024-05-06 20:39:38.336670 texture_viz-0.0.2/texture/frontend/assets/cssMode-199f294b.js
--rw-r--r--   0        0        0     3631 2024-05-06 20:39:38.170906 texture_viz-0.0.2/texture/frontend/assets/cypher-16871f29.js
--rw-r--r--   0        0        0     4496 2024-05-06 20:39:38.170742 texture_viz-0.0.2/texture/frontend/assets/dart-20618e99.js
--rw-r--r--   0        0        0     2115 2024-05-06 20:39:38.171133 texture_viz-0.0.2/texture/frontend/assets/dockerfile-13942c6d.js
--rw-r--r--   0        0        0     5588 2024-05-06 20:39:38.171491 texture_viz-0.0.2/texture/frontend/assets/ecl-82a13cc7.js
--rw-r--r--   0        0        0   210313 2024-05-06 20:39:38.336854 texture_viz-0.0.2/texture/frontend/assets/editor.worker-01431e3b.js
--rw-r--r--   0        0        0    10503 2024-05-06 20:39:38.187900 texture_viz-0.0.2/texture/frontend/assets/elixir-941d33da.js
--rw-r--r--   0        0        0     2056 2024-05-06 20:39:38.188338 texture_viz-0.0.2/texture/frontend/assets/flow9-82e25a0d.js
--rw-r--r--   0        0        0    16401 2024-05-06 20:39:38.206251 texture_viz-0.0.2/texture/frontend/assets/freemarker2-a4b4bb19.js
--rw-r--r--   0        0        0     3229 2024-05-06 20:39:38.188846 texture_viz-0.0.2/texture/frontend/assets/fsharp-930eb6d7.js
--rw-r--r--   0        0        0     2903 2024-05-06 20:39:38.204534 texture_viz-0.0.2/texture/frontend/assets/go-ace823b2.js
--rw-r--r--   0        0        0     2506 2024-05-06 20:39:38.204736 texture_viz-0.0.2/texture/frontend/assets/graphql-9395e6dd.js
--rw-r--r--   0        0        0     7079 2024-05-06 20:39:38.204747 texture_viz-0.0.2/texture/frontend/assets/handlebars-b3ff6f90.js
--rw-r--r--   0        0        0     3836 2024-05-06 20:39:38.200230 texture_viz-0.0.2/texture/frontend/assets/hcl-4160620f.js
--rw-r--r--   0        0        0     5319 2024-05-06 20:39:38.199734 texture_viz-0.0.2/texture/frontend/assets/html-5fb69d41.js
--rw-r--r--   0        0        0   648414 2024-05-06 20:39:38.337370 texture_viz-0.0.2/texture/frontend/assets/html.worker-507844cb.js
--rw-r--r--   0        0        0    34187 2024-05-06 20:39:38.336719 texture_viz-0.0.2/texture/frontend/assets/htmlMode-7bc37b7a.js
--rw-r--r--   0        0        0  1094289 2024-05-06 20:39:38.337815 texture_viz-0.0.2/texture/frontend/assets/index-12b44d82.js
--rw-r--r--   0        0        0   130080 2024-05-06 20:39:38.169365 texture_viz-0.0.2/texture/frontend/assets/index-9845c041.css
--rw-r--r--   0        0        0     1347 2024-05-06 20:39:38.188467 texture_viz-0.0.2/texture/frontend/assets/ini-1cc2fa96.js
--rw-r--r--   0        0        0     3467 2024-05-06 20:39:38.188755 texture_viz-0.0.2/texture/frontend/assets/java-fe979474.js
--rw-r--r--   0        0        0     1215 2024-05-06 20:39:38.199556 texture_viz-0.0.2/texture/frontend/assets/javascript-25a81c5f.js
--rw-r--r--   0        0        0   339128 2024-05-06 20:39:38.337067 texture_viz-0.0.2/texture/frontend/assets/json.worker-d3a373c5.js
--rw-r--r--   0        0        0    39713 2024-05-06 20:39:38.336706 texture_viz-0.0.2/texture/frontend/assets/jsonMode-be458bae.js
--rw-r--r--   0        0        0     7395 2024-05-06 20:39:38.199484 texture_viz-0.0.2/texture/frontend/assets/julia-1a2d9387.js
--rw-r--r--   0        0        0     3685 2024-05-06 20:39:38.187443 texture_viz-0.0.2/texture/frontend/assets/kotlin-45b3a4f3.js
--rw-r--r--   0        0        0     4144 2024-05-06 20:39:38.171730 texture_viz-0.0.2/texture/frontend/assets/less-a184ed1c.js
--rw-r--r--   0        0        0     2683 2024-05-06 20:39:38.187252 texture_viz-0.0.2/texture/frontend/assets/lexon-ebf376fd.js
--rw-r--r--   0        0        0     4265 2024-05-06 20:39:38.188141 texture_viz-0.0.2/texture/frontend/assets/liquid-752bf567.js
--rw-r--r--   0        0        0     2369 2024-05-06 20:39:38.188089 texture_viz-0.0.2/texture/frontend/assets/lua-666d20d5.js
--rw-r--r--   0        0        0     3063 2024-05-06 20:39:38.200173 texture_viz-0.0.2/texture/frontend/assets/m3-bbbbbca9.js
--rw-r--r--   0        0        0     4034 2024-05-06 20:39:38.188447 texture_viz-0.0.2/texture/frontend/assets/markdown-5de2301d.js
--rw-r--r--   0        0        0     5170 2024-05-06 20:39:38.188353 texture_viz-0.0.2/texture/frontend/assets/mdx-778b6fcd.js
--rw-r--r--   0        0        0     2825 2024-05-06 20:39:38.187802 texture_viz-0.0.2/texture/frontend/assets/mips-7b46d093.js
--rw-r--r--   0        0        0   125064 2024-05-06 20:39:38.170485 texture_viz-0.0.2/texture/frontend/assets/monaco-9a20ab81.css
--rw-r--r--   0        0        0  3213363 2024-05-06 20:39:38.338776 texture_viz-0.0.2/texture/frontend/assets/monaco-c2479957.js
--rw-r--r--   0        0        0     5158 2024-05-06 20:39:38.200143 texture_viz-0.0.2/texture/frontend/assets/msdax-295c0d3c.js
--rw-r--r--   0        0        0    11520 2024-05-06 20:39:38.200213 texture_viz-0.0.2/texture/frontend/assets/mysql-28fc43b5.js
--rw-r--r--   0        0        0     2648 2024-05-06 20:39:38.188829 texture_viz-0.0.2/texture/frontend/assets/objective-c-5f7f7623.js
--rw-r--r--   0        0        0     3241 2024-05-06 20:39:38.199502 texture_viz-0.0.2/texture/frontend/assets/pascal-830d8a16.js
--rw-r--r--   0        0        0     2246 2024-05-06 20:39:38.188845 texture_viz-0.0.2/texture/frontend/assets/pascaligo-ff6a611d.js
--rw-r--r--   0        0        0     8501 2024-05-06 20:39:38.188751 texture_viz-0.0.2/texture/frontend/assets/perl-0c4cf450.js
--rw-r--r--   0        0        0    13710 2024-05-06 20:39:38.188775 texture_viz-0.0.2/texture/frontend/assets/pgsql-85eb1e14.js
--rw-r--r--   0        0        0     8273 2024-05-06 20:39:38.188426 texture_viz-0.0.2/texture/frontend/assets/php-571f6521.js
--rw-r--r--   0        0        0     1929 2024-05-06 20:39:38.187869 texture_viz-0.0.2/texture/frontend/assets/pla-5e6cd4d5.js
--rw-r--r--   0        0        0     8102 2024-05-06 20:39:38.187820 texture_viz-0.0.2/texture/frontend/assets/postiats-4d02d044.js
--rw-r--r--   0        0        0    17185 2024-05-06 20:39:38.205708 texture_viz-0.0.2/texture/frontend/assets/powerquery-c6baddff.js
--rw-r--r--   0        0        0     3515 2024-05-06 20:39:38.206090 texture_viz-0.0.2/texture/frontend/assets/powershell-8bfccb2f.js
--rw-r--r--   0        0        0     9292 2024-05-06 20:39:38.206260 texture_viz-0.0.2/texture/frontend/assets/protobuf-7c245adb.js
--rw-r--r--   0        0        0     5074 2024-05-06 20:39:38.206280 texture_viz-0.0.2/texture/frontend/assets/pug-e0d77a81.js
--rw-r--r--   0        0        0     3929 2024-05-06 20:39:38.206455 texture_viz-0.0.2/texture/frontend/assets/python-a93e07ff.js
--rw-r--r--   0        0        0     3181 2024-05-06 20:39:38.206358 texture_viz-0.0.2/texture/frontend/assets/qsharp-560af9ec.js
--rw-r--r--   0        0        0     3377 2024-05-06 20:39:38.206473 texture_viz-0.0.2/texture/frontend/assets/r-96b98db0.js
--rw-r--r--   0        0        0     9083 2024-05-06 20:39:38.218370 texture_viz-0.0.2/texture/frontend/assets/razor-555b0b96.js
--rw-r--r--   0        0        0     3802 2024-05-06 20:39:38.206466 texture_viz-0.0.2/texture/frontend/assets/redis-2313a258.js
--rw-r--r--   0        0        0    12046 2024-05-06 20:39:38.217855 texture_viz-0.0.2/texture/frontend/assets/redshift-e81279f9.js
--rw-r--r--   0        0        0     4139 2024-05-06 20:39:38.217471 texture_viz-0.0.2/texture/frontend/assets/restructuredtext-23e36e2c.js
--rw-r--r--   0        0        0     8750 2024-05-06 20:39:38.218835 texture_viz-0.0.2/texture/frontend/assets/ruby-6e5b4752.js
--rw-r--r--   0        0        0     4406 2024-05-06 20:39:38.218375 texture_viz-0.0.2/texture/frontend/assets/rust-c4e1d9a9.js
--rw-r--r--   0        0        0     2075 2024-05-06 20:39:38.217477 texture_viz-0.0.2/texture/frontend/assets/sb-095651a8.js
--rw-r--r--   0        0        0     7564 2024-05-06 20:39:38.218819 texture_viz-0.0.2/texture/frontend/assets/scala-dfd2c035.js
--rw-r--r--   0        0        0     2013 2024-05-06 20:39:38.218389 texture_viz-0.0.2/texture/frontend/assets/scheme-4bd59040.js
--rw-r--r--   0        0        0     6655 2024-05-06 20:39:38.222783 texture_viz-0.0.2/texture/frontend/assets/scss-0b769ec8.js
--rw-r--r--   0        0        0     3319 2024-05-06 20:39:38.218880 texture_viz-0.0.2/texture/frontend/assets/shell-5fa60225.js
--rw-r--r--   0        0        0    18843 2024-05-06 20:39:38.224434 texture_viz-0.0.2/texture/frontend/assets/solidity-3efd84d4.js
--rw-r--r--   0        0        0     3010 2024-05-06 20:39:38.218838 texture_viz-0.0.2/texture/frontend/assets/sophia-156a057a.js
--rw-r--r--   0        0        0     2798 2024-05-06 20:39:38.224049 texture_viz-0.0.2/texture/frontend/assets/sparql-25a61c8a.js
--rw-r--r--   0        0        0    10543 2024-05-06 20:39:38.225079 texture_viz-0.0.2/texture/frontend/assets/sql-ef431720.js
--rw-r--r--   0        0        0     7645 2024-05-06 20:39:38.224446 texture_viz-0.0.2/texture/frontend/assets/st-06071006.js
--rw-r--r--   0        0        0     5417 2024-05-06 20:39:38.224404 texture_viz-0.0.2/texture/frontend/assets/swift-941c2e3c.js
--rw-r--r--   0        0        0     7849 2024-05-06 20:39:38.224716 texture_viz-0.0.2/texture/frontend/assets/systemverilog-dc0c3813.js
--rw-r--r--   0        0        0     3817 2024-05-06 20:39:38.224412 texture_viz-0.0.2/texture/frontend/assets/tcl-cc963d5c.js
--rw-r--r--   0        0        0  4847902 2024-05-06 20:39:38.339588 texture_viz-0.0.2/texture/frontend/assets/ts.worker-ac912115.js
--rw-r--r--   0        0        0    22568 2024-05-06 20:39:38.336710 texture_viz-0.0.2/texture/frontend/assets/tsMode-ed5a3878.js
--rw-r--r--   0        0        0     6219 2024-05-06 20:39:38.225252 texture_viz-0.0.2/texture/frontend/assets/twig-cdf47909.js
--rw-r--r--   0        0        0     5712 2024-05-06 20:39:38.187624 texture_viz-0.0.2/texture/frontend/assets/typescript-a3afb5cc.js
--rw-r--r--   0        0        0     6037 2024-05-06 20:39:38.224744 texture_viz-0.0.2/texture/frontend/assets/vb-3ff3c116.js
--rw-r--r--   0        0        0     7575 2024-05-06 20:39:38.324432 texture_viz-0.0.2/texture/frontend/assets/wgsl-7be617f0.js
--rw-r--r--   0        0        0     2713 2024-05-06 20:39:38.324262 texture_viz-0.0.2/texture/frontend/assets/xml-0a37659d.js
--rw-r--r--   0        0        0     4320 2024-05-06 20:39:38.324442 texture_viz-0.0.2/texture/frontend/assets/yaml-be9b69da.js
--rw-r--r--   0        0        0    14836 2024-05-06 20:39:36.703118 texture_viz-0.0.2/texture/frontend/icon.svg
--rw-r--r--   0        0        0      473 2024-05-06 20:39:38.337164 texture_viz-0.0.2/texture/frontend/index.html
--rw-r--r--   0        0        0     3651 2024-05-06 18:57:02.093384 texture_viz-0.0.2/texture/models.py
--rw-r--r--   0        0        0      341 2024-05-05 01:31:21.487096 texture_viz-0.0.2/texture/preprocess/__init__.py
--rw-r--r--   0        0        0     1855 2024-05-05 01:31:21.487702 texture_viz-0.0.2/texture/preprocess/embeddings.py
--rw-r--r--   0        0        0     4415 2024-05-06 19:34:47.411132 texture_viz-0.0.2/texture/preprocess/pipeline.py
--rw-r--r--   0        0        0     1156 2024-05-05 01:31:21.488691 texture_viz-0.0.2/texture/preprocess/tokenize.py
--rw-r--r--   0        0        0     1273 2024-05-06 19:22:20.530556 texture_viz-0.0.2/texture/preprocess/utils.py
--rw-r--r--   0        0        0     2139 2024-05-06 19:33:42.623331 texture_viz-0.0.2/texture/runner.py
--rw-r--r--   0        0        0      609 2024-05-06 13:53:24.922182 texture_viz-0.0.2/texture/runner_dev.py
--rw-r--r--   0        0        0    12074 2024-05-06 19:38:34.075786 texture_viz-0.0.2/texture/server.py
--rw-r--r--   0        0        0        0 2024-05-05 01:31:21.490444 texture_viz-0.0.2/texture/userTransformCode/__init__.py
--rw-r--r--   0        0        0      647 2024-05-05 01:31:21.490646 texture_viz-0.0.2/texture/userTransformCode/transform.py
--rw-r--r--   0        0        0        0 2024-05-05 01:31:21.490726 texture_viz-0.0.2/texture/userTransformLLM/__init__.py
--rw-r--r--   0        0        0    20500 2024-05-06 19:35:40.244819 texture_viz-0.0.2/texture/userTransformLLM/client.py
--rw-r--r--   0        0        0     1492 2024-05-05 01:31:21.492274 texture_viz-0.0.2/texture/utils.py
--rw-r--r--   0        0        0     2233 1970-01-01 00:00:00.000000 texture_viz-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1061 2024-05-07 04:29:57.908676 texture_viz-0.0.3/LICENSE.md
+-rw-r--r--   0        0        0     2983 2024-05-07 21:28:45.793022 texture_viz-0.0.3/README.md
+-rw-r--r--   0        0        0      998 2024-05-07 21:30:08.083080 texture_viz-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0       62 2024-05-05 01:31:21.484411 texture_viz-0.0.3/texture/__init__.py
+-rw-r--r--   0        0        0      118 2024-05-05 01:31:21.485088 texture_viz-0.0.3/texture/database/__init__.py
+-rw-r--r--   0        0        0    11042 2024-05-06 19:36:30.468050 texture_viz-0.0.3/texture/database/connection.py
+-rw-r--r--   0        0        0     6816 2024-05-06 16:46:57.768411 texture_viz-0.0.3/texture/database/example_data.py
+-rw-r--r--   0        0        0    14409 2024-05-07 21:31:16.001777 texture_viz-0.0.3/texture/frontend/assets/abap-ad6e811d.js
+-rw-r--r--   0        0        0     4198 2024-05-07 21:31:16.001638 texture_viz-0.0.3/texture/frontend/assets/apex-992ba105.js
+-rw-r--r--   0        0        0     1094 2024-05-07 21:31:16.000409 texture_viz-0.0.3/texture/frontend/assets/azcli-2ae42e71.js
+-rw-r--r--   0        0        0     2091 2024-05-07 21:31:16.000415 texture_viz-0.0.3/texture/frontend/assets/bat-638cac0f.js
+-rw-r--r--   0        0        0     2782 2024-05-07 21:31:16.000485 texture_viz-0.0.3/texture/frontend/assets/bicep-389290ac.js
+-rw-r--r--   0        0        0     2431 2024-05-07 21:31:16.001698 texture_viz-0.0.3/texture/frontend/assets/cameligo-e2b87a47.js
+-rw-r--r--   0        0        0     9889 2024-05-07 21:31:16.001626 texture_viz-0.0.3/texture/frontend/assets/clojure-9f651a27.js
+-rw-r--r--   0        0        0    79568 2024-05-07 21:31:15.989466 texture_viz-0.0.3/texture/frontend/assets/codicon-a3faa755.ttf
+-rw-r--r--   0        0        0     3836 2024-05-07 21:31:16.001783 texture_viz-0.0.3/texture/frontend/assets/coffee-4e075114.js
+-rw-r--r--   0        0        0     5680 2024-05-07 21:31:16.001537 texture_viz-0.0.3/texture/frontend/assets/cpp-8ffe77ae.js
+-rw-r--r--   0        0        0     4770 2024-05-07 21:31:16.001082 texture_viz-0.0.3/texture/frontend/assets/csharp-0b267c6b.js
+-rw-r--r--   0        0        0     1665 2024-05-07 21:31:16.000693 texture_viz-0.0.3/texture/frontend/assets/csp-c23415e1.js
+-rw-r--r--   0        0        0     4756 2024-05-07 21:31:16.000993 texture_viz-0.0.3/texture/frontend/assets/css-c62f5578.js
+-rw-r--r--   0        0        0   985422 2024-05-07 21:31:16.078686 texture_viz-0.0.3/texture/frontend/assets/css.worker-68e7a658.js
+-rw-r--r--   0        0        0    33636 2024-05-07 21:31:16.057143 texture_viz-0.0.3/texture/frontend/assets/cssMode-199f294b.js
+-rw-r--r--   0        0        0     3631 2024-05-07 21:31:16.000809 texture_viz-0.0.3/texture/frontend/assets/cypher-16871f29.js
+-rw-r--r--   0        0        0     4496 2024-05-07 21:31:16.001092 texture_viz-0.0.3/texture/frontend/assets/dart-20618e99.js
+-rw-r--r--   0        0        0     2115 2024-05-07 21:31:16.000567 texture_viz-0.0.3/texture/frontend/assets/dockerfile-13942c6d.js
+-rw-r--r--   0        0        0     5588 2024-05-07 21:31:16.004817 texture_viz-0.0.3/texture/frontend/assets/ecl-82a13cc7.js
+-rw-r--r--   0        0        0   210313 2024-05-07 21:31:16.077441 texture_viz-0.0.3/texture/frontend/assets/editor.worker-01431e3b.js
+-rw-r--r--   0        0        0    10503 2024-05-07 21:31:16.007578 texture_viz-0.0.3/texture/frontend/assets/elixir-941d33da.js
+-rw-r--r--   0        0        0     2056 2024-05-07 21:31:16.007266 texture_viz-0.0.3/texture/frontend/assets/flow9-82e25a0d.js
+-rw-r--r--   0        0        0    16401 2024-05-07 21:31:16.007787 texture_viz-0.0.3/texture/frontend/assets/freemarker2-a4b4bb19.js
+-rw-r--r--   0        0        0     3229 2024-05-07 21:31:16.007144 texture_viz-0.0.3/texture/frontend/assets/fsharp-930eb6d7.js
+-rw-r--r--   0        0        0     2903 2024-05-07 21:31:16.004444 texture_viz-0.0.3/texture/frontend/assets/go-ace823b2.js
+-rw-r--r--   0        0        0     2506 2024-05-07 21:31:16.005025 texture_viz-0.0.3/texture/frontend/assets/graphql-9395e6dd.js
+-rw-r--r--   0        0        0     7079 2024-05-07 21:31:16.001962 texture_viz-0.0.3/texture/frontend/assets/handlebars-b3ff6f90.js
+-rw-r--r--   0        0        0     3836 2024-05-07 21:31:16.004819 texture_viz-0.0.3/texture/frontend/assets/hcl-4160620f.js
+-rw-r--r--   0        0        0     5319 2024-05-07 21:31:16.004062 texture_viz-0.0.3/texture/frontend/assets/html-5fb69d41.js
+-rw-r--r--   0        0        0   648414 2024-05-07 21:31:16.078496 texture_viz-0.0.3/texture/frontend/assets/html.worker-507844cb.js
+-rw-r--r--   0        0        0    34187 2024-05-07 21:31:16.057118 texture_viz-0.0.3/texture/frontend/assets/htmlMode-7bc37b7a.js
+-rw-r--r--   0        0        0  1094289 2024-05-07 21:31:16.078562 texture_viz-0.0.3/texture/frontend/assets/index-12b44d82.js
+-rw-r--r--   0        0        0   130080 2024-05-07 21:31:16.000477 texture_viz-0.0.3/texture/frontend/assets/index-9845c041.css
+-rw-r--r--   0        0        0     1347 2024-05-07 21:31:16.004252 texture_viz-0.0.3/texture/frontend/assets/ini-1cc2fa96.js
+-rw-r--r--   0        0        0     3467 2024-05-07 21:31:16.003947 texture_viz-0.0.3/texture/frontend/assets/java-fe979474.js
+-rw-r--r--   0        0        0     1215 2024-05-07 21:31:16.001790 texture_viz-0.0.3/texture/frontend/assets/javascript-25a81c5f.js
+-rw-r--r--   0        0        0   339128 2024-05-07 21:31:16.077758 texture_viz-0.0.3/texture/frontend/assets/json.worker-d3a373c5.js
+-rw-r--r--   0        0        0    39713 2024-05-07 21:31:16.057170 texture_viz-0.0.3/texture/frontend/assets/jsonMode-be458bae.js
+-rw-r--r--   0        0        0     7395 2024-05-07 21:31:16.004487 texture_viz-0.0.3/texture/frontend/assets/julia-1a2d9387.js
+-rw-r--r--   0        0        0     3685 2024-05-07 21:31:16.004460 texture_viz-0.0.3/texture/frontend/assets/kotlin-45b3a4f3.js
+-rw-r--r--   0        0        0     4144 2024-05-07 21:31:16.004873 texture_viz-0.0.3/texture/frontend/assets/less-a184ed1c.js
+-rw-r--r--   0        0        0     2683 2024-05-07 21:31:16.005194 texture_viz-0.0.3/texture/frontend/assets/lexon-ebf376fd.js
+-rw-r--r--   0        0        0     4265 2024-05-07 21:31:16.008278 texture_viz-0.0.3/texture/frontend/assets/liquid-752bf567.js
+-rw-r--r--   0        0        0     2369 2024-05-07 21:31:16.007545 texture_viz-0.0.3/texture/frontend/assets/lua-666d20d5.js
+-rw-r--r--   0        0        0     3063 2024-05-07 21:31:16.005509 texture_viz-0.0.3/texture/frontend/assets/m3-bbbbbca9.js
+-rw-r--r--   0        0        0     4034 2024-05-07 21:31:16.005097 texture_viz-0.0.3/texture/frontend/assets/markdown-5de2301d.js
+-rw-r--r--   0        0        0     5170 2024-05-07 21:31:16.005241 texture_viz-0.0.3/texture/frontend/assets/mdx-778b6fcd.js
+-rw-r--r--   0        0        0     2825 2024-05-07 21:31:16.005059 texture_viz-0.0.3/texture/frontend/assets/mips-7b46d093.js
+-rw-r--r--   0        0        0   125064 2024-05-07 21:31:16.001383 texture_viz-0.0.3/texture/frontend/assets/monaco-9a20ab81.css
+-rw-r--r--   0        0        0  3213363 2024-05-07 21:31:16.080333 texture_viz-0.0.3/texture/frontend/assets/monaco-c2479957.js
+-rw-r--r--   0        0        0     5158 2024-05-07 21:31:16.004120 texture_viz-0.0.3/texture/frontend/assets/msdax-295c0d3c.js
+-rw-r--r--   0        0        0    11520 2024-05-07 21:31:16.005424 texture_viz-0.0.3/texture/frontend/assets/mysql-28fc43b5.js
+-rw-r--r--   0        0        0     2648 2024-05-07 21:31:16.005083 texture_viz-0.0.3/texture/frontend/assets/objective-c-5f7f7623.js
+-rw-r--r--   0        0        0     3241 2024-05-07 21:31:16.004215 texture_viz-0.0.3/texture/frontend/assets/pascal-830d8a16.js
+-rw-r--r--   0        0        0     2246 2024-05-07 21:31:16.011139 texture_viz-0.0.3/texture/frontend/assets/pascaligo-ff6a611d.js
+-rw-r--r--   0        0        0     8501 2024-05-07 21:31:16.011551 texture_viz-0.0.3/texture/frontend/assets/perl-0c4cf450.js
+-rw-r--r--   0        0        0    13710 2024-05-07 21:31:16.012021 texture_viz-0.0.3/texture/frontend/assets/pgsql-85eb1e14.js
+-rw-r--r--   0        0        0     8273 2024-05-07 21:31:16.011572 texture_viz-0.0.3/texture/frontend/assets/php-571f6521.js
+-rw-r--r--   0        0        0     1929 2024-05-07 21:31:16.008428 texture_viz-0.0.3/texture/frontend/assets/pla-5e6cd4d5.js
+-rw-r--r--   0        0        0     8102 2024-05-07 21:31:16.008855 texture_viz-0.0.3/texture/frontend/assets/postiats-4d02d044.js
+-rw-r--r--   0        0        0    17185 2024-05-07 21:31:16.008834 texture_viz-0.0.3/texture/frontend/assets/powerquery-c6baddff.js
+-rw-r--r--   0        0        0     3515 2024-05-07 21:31:16.008381 texture_viz-0.0.3/texture/frontend/assets/powershell-8bfccb2f.js
+-rw-r--r--   0        0        0     9292 2024-05-07 21:31:16.009289 texture_viz-0.0.3/texture/frontend/assets/protobuf-7c245adb.js
+-rw-r--r--   0        0        0     5074 2024-05-07 21:31:16.008262 texture_viz-0.0.3/texture/frontend/assets/pug-e0d77a81.js
+-rw-r--r--   0        0        0     3929 2024-05-07 21:31:16.008448 texture_viz-0.0.3/texture/frontend/assets/python-a93e07ff.js
+-rw-r--r--   0        0        0     3181 2024-05-07 21:31:16.007811 texture_viz-0.0.3/texture/frontend/assets/qsharp-560af9ec.js
+-rw-r--r--   0        0        0     3377 2024-05-07 21:31:16.007257 texture_viz-0.0.3/texture/frontend/assets/r-96b98db0.js
+-rw-r--r--   0        0        0     9083 2024-05-07 21:31:16.009320 texture_viz-0.0.3/texture/frontend/assets/razor-555b0b96.js
+-rw-r--r--   0        0        0     3802 2024-05-07 21:31:16.008878 texture_viz-0.0.3/texture/frontend/assets/redis-2313a258.js
+-rw-r--r--   0        0        0    12046 2024-05-07 21:31:16.011935 texture_viz-0.0.3/texture/frontend/assets/redshift-e81279f9.js
+-rw-r--r--   0        0        0     4139 2024-05-07 21:31:16.010858 texture_viz-0.0.3/texture/frontend/assets/restructuredtext-23e36e2c.js
+-rw-r--r--   0        0        0     8750 2024-05-07 21:31:16.011122 texture_viz-0.0.3/texture/frontend/assets/ruby-6e5b4752.js
+-rw-r--r--   0        0        0     4406 2024-05-07 21:31:16.008235 texture_viz-0.0.3/texture/frontend/assets/rust-c4e1d9a9.js
+-rw-r--r--   0        0        0     2075 2024-05-07 21:31:16.008559 texture_viz-0.0.3/texture/frontend/assets/sb-095651a8.js
+-rw-r--r--   0        0        0     7564 2024-05-07 21:31:16.010615 texture_viz-0.0.3/texture/frontend/assets/scala-dfd2c035.js
+-rw-r--r--   0        0        0     2013 2024-05-07 21:31:16.010684 texture_viz-0.0.3/texture/frontend/assets/scheme-4bd59040.js
+-rw-r--r--   0        0        0     6655 2024-05-07 21:31:16.009530 texture_viz-0.0.3/texture/frontend/assets/scss-0b769ec8.js
+-rw-r--r--   0        0        0     3319 2024-05-07 21:31:16.010875 texture_viz-0.0.3/texture/frontend/assets/shell-5fa60225.js
+-rw-r--r--   0        0        0    18843 2024-05-07 21:31:16.012749 texture_viz-0.0.3/texture/frontend/assets/solidity-3efd84d4.js
+-rw-r--r--   0        0        0     3010 2024-05-07 21:31:16.012149 texture_viz-0.0.3/texture/frontend/assets/sophia-156a057a.js
+-rw-r--r--   0        0        0     2798 2024-05-07 21:31:16.012214 texture_viz-0.0.3/texture/frontend/assets/sparql-25a61c8a.js
+-rw-r--r--   0        0        0    10543 2024-05-07 21:31:16.013213 texture_viz-0.0.3/texture/frontend/assets/sql-ef431720.js
+-rw-r--r--   0        0        0     7645 2024-05-07 21:31:16.012784 texture_viz-0.0.3/texture/frontend/assets/st-06071006.js
+-rw-r--r--   0        0        0     5417 2024-05-07 21:31:16.012386 texture_viz-0.0.3/texture/frontend/assets/swift-941c2e3c.js
+-rw-r--r--   0        0        0     7849 2024-05-07 21:31:16.013214 texture_viz-0.0.3/texture/frontend/assets/systemverilog-dc0c3813.js
+-rw-r--r--   0        0        0     3817 2024-05-07 21:31:16.012843 texture_viz-0.0.3/texture/frontend/assets/tcl-cc963d5c.js
+-rw-r--r--   0        0        0  4847902 2024-05-07 21:31:16.081835 texture_viz-0.0.3/texture/frontend/assets/ts.worker-ac912115.js
+-rw-r--r--   0        0        0    22568 2024-05-07 21:31:16.054321 texture_viz-0.0.3/texture/frontend/assets/tsMode-ed5a3878.js
+-rw-r--r--   0        0        0     6219 2024-05-07 21:31:16.013426 texture_viz-0.0.3/texture/frontend/assets/twig-cdf47909.js
+-rw-r--r--   0        0        0     5712 2024-05-07 21:31:16.004869 texture_viz-0.0.3/texture/frontend/assets/typescript-a3afb5cc.js
+-rw-r--r--   0        0        0     6037 2024-05-07 21:31:16.013603 texture_viz-0.0.3/texture/frontend/assets/vb-3ff3c116.js
+-rw-r--r--   0        0        0     7575 2024-05-07 21:31:16.051982 texture_viz-0.0.3/texture/frontend/assets/wgsl-7be617f0.js
+-rw-r--r--   0        0        0     2713 2024-05-07 21:31:16.054318 texture_viz-0.0.3/texture/frontend/assets/xml-0a37659d.js
+-rw-r--r--   0        0        0     4320 2024-05-07 21:31:16.057101 texture_viz-0.0.3/texture/frontend/assets/yaml-be9b69da.js
+-rw-r--r--   0        0        0    14836 2024-05-07 21:31:14.463506 texture_viz-0.0.3/texture/frontend/icon.svg
+-rw-r--r--   0        0        0      473 2024-05-07 21:31:16.077900 texture_viz-0.0.3/texture/frontend/index.html
+-rw-r--r--   0        0        0     3651 2024-05-06 18:57:02.093384 texture_viz-0.0.3/texture/models.py
+-rw-r--r--   0        0        0      341 2024-05-07 21:05:04.668821 texture_viz-0.0.3/texture/preprocess/__init__.py
+-rw-r--r--   0        0        0     1855 2024-05-05 01:31:21.487702 texture_viz-0.0.3/texture/preprocess/embeddings.py
+-rw-r--r--   0        0        0     4389 2024-05-07 21:02:39.767332 texture_viz-0.0.3/texture/preprocess/pipeline.py
+-rw-r--r--   0        0        0     1156 2024-05-05 01:31:21.488691 texture_viz-0.0.3/texture/preprocess/tokenize.py
+-rw-r--r--   0        0        0     1273 2024-05-06 19:22:20.530556 texture_viz-0.0.3/texture/preprocess/utils.py
+-rw-r--r--   0        0        0     2366 2024-05-07 21:03:32.082781 texture_viz-0.0.3/texture/runner.py
+-rw-r--r--   0        0        0      609 2024-05-07 20:52:32.388201 texture_viz-0.0.3/texture/runner_dev.py
+-rw-r--r--   0        0        0    12074 2024-05-07 21:04:43.605693 texture_viz-0.0.3/texture/server.py
+-rw-r--r--   0        0        0        0 2024-05-05 01:31:21.490444 texture_viz-0.0.3/texture/userTransformCode/__init__.py
+-rw-r--r--   0        0        0      647 2024-05-05 01:31:21.490646 texture_viz-0.0.3/texture/userTransformCode/transform.py
+-rw-r--r--   0        0        0        0 2024-05-05 01:31:21.490726 texture_viz-0.0.3/texture/userTransformLLM/__init__.py
+-rw-r--r--   0        0        0    20500 2024-05-06 19:35:40.244819 texture_viz-0.0.3/texture/userTransformLLM/client.py
+-rw-r--r--   0        0        0     1492 2024-05-05 01:31:21.492274 texture_viz-0.0.3/texture/utils.py
+-rw-r--r--   0        0        0     4188 1970-01-01 00:00:00.000000 texture_viz-0.0.3/PKG-INFO
```

### Comparing `texture_viz-0.0.2/pyproject.toml` & `texture_viz-0.0.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "texture-viz"
-version = "0.0.2"
+version = "0.0.3"
 description = "Process and profile text datasets interactively"
 authors = ["Will Epperson <willepp@live.com>"]
 readme = "README.md"
 repository = "https://github.com/cmudig/Texture"
 homepage = "https://github.com/cmudig/Texture"
 keywords = ["text", "nlp", "data profiling", "llm"]
 packages = [{ include = "texture" }]
@@ -24,14 +24,15 @@
 uvicorn = { extras = ["standard"], version = "^0.24.0.post1" }
 python-multipart = "^0.0.6"
 nltk = "^3.8.1"
 tiktoken = "^0.5.2"
 lancedb = "^0.5.1"
 umap-learn = "^0.5.5"
 openai = "^1.20.0"
+multiprocess = "^0.70.16"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
```

### Comparing `texture_viz-0.0.2/texture/database/connection.py` & `texture_viz-0.0.3/texture/database/connection.py`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/database/example_data.py` & `texture_viz-0.0.3/texture/database/example_data.py`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/abap-ad6e811d.js` & `texture_viz-0.0.3/texture/frontend/assets/abap-ad6e811d.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/apex-992ba105.js` & `texture_viz-0.0.3/texture/frontend/assets/apex-992ba105.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/azcli-2ae42e71.js` & `texture_viz-0.0.3/texture/frontend/assets/azcli-2ae42e71.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/bat-638cac0f.js` & `texture_viz-0.0.3/texture/frontend/assets/bat-638cac0f.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/bicep-389290ac.js` & `texture_viz-0.0.3/texture/frontend/assets/bicep-389290ac.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/cameligo-e2b87a47.js` & `texture_viz-0.0.3/texture/frontend/assets/cameligo-e2b87a47.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/clojure-9f651a27.js` & `texture_viz-0.0.3/texture/frontend/assets/clojure-9f651a27.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/codicon-a3faa755.ttf` & `texture_viz-0.0.3/texture/frontend/assets/codicon-a3faa755.ttf`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/coffee-4e075114.js` & `texture_viz-0.0.3/texture/frontend/assets/coffee-4e075114.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/cpp-8ffe77ae.js` & `texture_viz-0.0.3/texture/frontend/assets/cpp-8ffe77ae.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/csharp-0b267c6b.js` & `texture_viz-0.0.3/texture/frontend/assets/csharp-0b267c6b.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/csp-c23415e1.js` & `texture_viz-0.0.3/texture/frontend/assets/csp-c23415e1.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/css-c62f5578.js` & `texture_viz-0.0.3/texture/frontend/assets/css-c62f5578.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/css.worker-68e7a658.js` & `texture_viz-0.0.3/texture/frontend/assets/css.worker-68e7a658.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/cssMode-199f294b.js` & `texture_viz-0.0.3/texture/frontend/assets/cssMode-199f294b.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/cypher-16871f29.js` & `texture_viz-0.0.3/texture/frontend/assets/cypher-16871f29.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/dart-20618e99.js` & `texture_viz-0.0.3/texture/frontend/assets/dart-20618e99.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/dockerfile-13942c6d.js` & `texture_viz-0.0.3/texture/frontend/assets/dockerfile-13942c6d.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/ecl-82a13cc7.js` & `texture_viz-0.0.3/texture/frontend/assets/ecl-82a13cc7.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/editor.worker-01431e3b.js` & `texture_viz-0.0.3/texture/frontend/assets/editor.worker-01431e3b.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/elixir-941d33da.js` & `texture_viz-0.0.3/texture/frontend/assets/elixir-941d33da.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/flow9-82e25a0d.js` & `texture_viz-0.0.3/texture/frontend/assets/flow9-82e25a0d.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/freemarker2-a4b4bb19.js` & `texture_viz-0.0.3/texture/frontend/assets/freemarker2-a4b4bb19.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/fsharp-930eb6d7.js` & `texture_viz-0.0.3/texture/frontend/assets/fsharp-930eb6d7.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/go-ace823b2.js` & `texture_viz-0.0.3/texture/frontend/assets/go-ace823b2.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/graphql-9395e6dd.js` & `texture_viz-0.0.3/texture/frontend/assets/graphql-9395e6dd.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/handlebars-b3ff6f90.js` & `texture_viz-0.0.3/texture/frontend/assets/handlebars-b3ff6f90.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/hcl-4160620f.js` & `texture_viz-0.0.3/texture/frontend/assets/hcl-4160620f.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/html-5fb69d41.js` & `texture_viz-0.0.3/texture/frontend/assets/html-5fb69d41.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/html.worker-507844cb.js` & `texture_viz-0.0.3/texture/frontend/assets/html.worker-507844cb.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/htmlMode-7bc37b7a.js` & `texture_viz-0.0.3/texture/frontend/assets/htmlMode-7bc37b7a.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/index-12b44d82.js` & `texture_viz-0.0.3/texture/frontend/assets/index-12b44d82.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/index-9845c041.css` & `texture_viz-0.0.3/texture/frontend/assets/index-9845c041.css`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/ini-1cc2fa96.js` & `texture_viz-0.0.3/texture/frontend/assets/ini-1cc2fa96.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/java-fe979474.js` & `texture_viz-0.0.3/texture/frontend/assets/java-fe979474.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/javascript-25a81c5f.js` & `texture_viz-0.0.3/texture/frontend/assets/javascript-25a81c5f.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/json.worker-d3a373c5.js` & `texture_viz-0.0.3/texture/frontend/assets/json.worker-d3a373c5.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/jsonMode-be458bae.js` & `texture_viz-0.0.3/texture/frontend/assets/jsonMode-be458bae.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/julia-1a2d9387.js` & `texture_viz-0.0.3/texture/frontend/assets/julia-1a2d9387.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/kotlin-45b3a4f3.js` & `texture_viz-0.0.3/texture/frontend/assets/kotlin-45b3a4f3.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/less-a184ed1c.js` & `texture_viz-0.0.3/texture/frontend/assets/less-a184ed1c.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/lexon-ebf376fd.js` & `texture_viz-0.0.3/texture/frontend/assets/lexon-ebf376fd.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/liquid-752bf567.js` & `texture_viz-0.0.3/texture/frontend/assets/liquid-752bf567.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/lua-666d20d5.js` & `texture_viz-0.0.3/texture/frontend/assets/lua-666d20d5.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/m3-bbbbbca9.js` & `texture_viz-0.0.3/texture/frontend/assets/m3-bbbbbca9.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/markdown-5de2301d.js` & `texture_viz-0.0.3/texture/frontend/assets/markdown-5de2301d.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/mdx-778b6fcd.js` & `texture_viz-0.0.3/texture/frontend/assets/mdx-778b6fcd.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/mips-7b46d093.js` & `texture_viz-0.0.3/texture/frontend/assets/mips-7b46d093.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/monaco-9a20ab81.css` & `texture_viz-0.0.3/texture/frontend/assets/monaco-9a20ab81.css`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/monaco-c2479957.js` & `texture_viz-0.0.3/texture/frontend/assets/monaco-c2479957.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/msdax-295c0d3c.js` & `texture_viz-0.0.3/texture/frontend/assets/msdax-295c0d3c.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/mysql-28fc43b5.js` & `texture_viz-0.0.3/texture/frontend/assets/mysql-28fc43b5.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/objective-c-5f7f7623.js` & `texture_viz-0.0.3/texture/frontend/assets/objective-c-5f7f7623.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/pascal-830d8a16.js` & `texture_viz-0.0.3/texture/frontend/assets/pascal-830d8a16.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/pascaligo-ff6a611d.js` & `texture_viz-0.0.3/texture/frontend/assets/pascaligo-ff6a611d.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/perl-0c4cf450.js` & `texture_viz-0.0.3/texture/frontend/assets/perl-0c4cf450.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/pgsql-85eb1e14.js` & `texture_viz-0.0.3/texture/frontend/assets/pgsql-85eb1e14.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/php-571f6521.js` & `texture_viz-0.0.3/texture/frontend/assets/php-571f6521.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/pla-5e6cd4d5.js` & `texture_viz-0.0.3/texture/frontend/assets/pla-5e6cd4d5.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/postiats-4d02d044.js` & `texture_viz-0.0.3/texture/frontend/assets/postiats-4d02d044.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/powerquery-c6baddff.js` & `texture_viz-0.0.3/texture/frontend/assets/powerquery-c6baddff.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/powershell-8bfccb2f.js` & `texture_viz-0.0.3/texture/frontend/assets/powershell-8bfccb2f.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/protobuf-7c245adb.js` & `texture_viz-0.0.3/texture/frontend/assets/protobuf-7c245adb.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/pug-e0d77a81.js` & `texture_viz-0.0.3/texture/frontend/assets/pug-e0d77a81.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/python-a93e07ff.js` & `texture_viz-0.0.3/texture/frontend/assets/python-a93e07ff.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/qsharp-560af9ec.js` & `texture_viz-0.0.3/texture/frontend/assets/qsharp-560af9ec.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/r-96b98db0.js` & `texture_viz-0.0.3/texture/frontend/assets/r-96b98db0.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/razor-555b0b96.js` & `texture_viz-0.0.3/texture/frontend/assets/razor-555b0b96.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/redis-2313a258.js` & `texture_viz-0.0.3/texture/frontend/assets/redis-2313a258.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/redshift-e81279f9.js` & `texture_viz-0.0.3/texture/frontend/assets/redshift-e81279f9.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/restructuredtext-23e36e2c.js` & `texture_viz-0.0.3/texture/frontend/assets/restructuredtext-23e36e2c.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/ruby-6e5b4752.js` & `texture_viz-0.0.3/texture/frontend/assets/ruby-6e5b4752.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/rust-c4e1d9a9.js` & `texture_viz-0.0.3/texture/frontend/assets/rust-c4e1d9a9.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/sb-095651a8.js` & `texture_viz-0.0.3/texture/frontend/assets/sb-095651a8.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/scala-dfd2c035.js` & `texture_viz-0.0.3/texture/frontend/assets/scala-dfd2c035.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/scheme-4bd59040.js` & `texture_viz-0.0.3/texture/frontend/assets/scheme-4bd59040.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/scss-0b769ec8.js` & `texture_viz-0.0.3/texture/frontend/assets/scss-0b769ec8.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/shell-5fa60225.js` & `texture_viz-0.0.3/texture/frontend/assets/shell-5fa60225.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/solidity-3efd84d4.js` & `texture_viz-0.0.3/texture/frontend/assets/solidity-3efd84d4.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/sophia-156a057a.js` & `texture_viz-0.0.3/texture/frontend/assets/sophia-156a057a.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/sparql-25a61c8a.js` & `texture_viz-0.0.3/texture/frontend/assets/sparql-25a61c8a.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/sql-ef431720.js` & `texture_viz-0.0.3/texture/frontend/assets/sql-ef431720.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/st-06071006.js` & `texture_viz-0.0.3/texture/frontend/assets/st-06071006.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/swift-941c2e3c.js` & `texture_viz-0.0.3/texture/frontend/assets/swift-941c2e3c.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/systemverilog-dc0c3813.js` & `texture_viz-0.0.3/texture/frontend/assets/systemverilog-dc0c3813.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/tcl-cc963d5c.js` & `texture_viz-0.0.3/texture/frontend/assets/tcl-cc963d5c.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/ts.worker-ac912115.js` & `texture_viz-0.0.3/texture/frontend/assets/ts.worker-ac912115.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/tsMode-ed5a3878.js` & `texture_viz-0.0.3/texture/frontend/assets/tsMode-ed5a3878.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/twig-cdf47909.js` & `texture_viz-0.0.3/texture/frontend/assets/twig-cdf47909.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/typescript-a3afb5cc.js` & `texture_viz-0.0.3/texture/frontend/assets/typescript-a3afb5cc.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/vb-3ff3c116.js` & `texture_viz-0.0.3/texture/frontend/assets/vb-3ff3c116.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/wgsl-7be617f0.js` & `texture_viz-0.0.3/texture/frontend/assets/wgsl-7be617f0.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/xml-0a37659d.js` & `texture_viz-0.0.3/texture/frontend/assets/xml-0a37659d.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/assets/yaml-be9b69da.js` & `texture_viz-0.0.3/texture/frontend/assets/yaml-be9b69da.js`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/frontend/icon.svg` & `texture_viz-0.0.3/texture/frontend/icon.svg`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/models.py` & `texture_viz-0.0.3/texture/models.py`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/preprocess/embeddings.py` & `texture_viz-0.0.3/texture/preprocess/embeddings.py`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/preprocess/pipeline.py` & `texture_viz-0.0.3/texture/preprocess/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import numpy as np
 from typing import List
 
 from texture import preprocess
 from texture.models import TextureInitArgs, DatasetInfo, Column, ColumnInputInfo
 
 
-def validate_and_run_preprocess(args: TextureInitArgs):  # -> (DatasetInfo, Dict)
+def validate_and_run_preprocess(args: TextureInitArgs):
     df = args.data
     name = args.name
     column_info = args.column_info
     sanitized_embeddings = None
     has_embeddings = False
     has_projection = False
```

### Comparing `texture_viz-0.0.2/texture/preprocess/tokenize.py` & `texture_viz-0.0.3/texture/preprocess/tokenize.py`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/preprocess/utils.py` & `texture_viz-0.0.3/texture/preprocess/utils.py`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/runner.py` & `texture_viz-0.0.3/texture/runner.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 import uvicorn
-from typing import Dict, Union, Any, List
-from multiprocessing import Process
+from typing import Dict, Any, List
+import multiprocess
 import pandas as pd
 
 from texture.models import (
     TextureInitArgs,
     DatasetInitArgs,
     ColumnInputInfo,
+    DatasetInfo,
 )
 from texture.server import get_server
 from texture.utils import is_notebook
 from texture import preprocess
 
 TEXTURE_SERVER_PROCESS = None
 
+try:
+    multiprocess.set_start_method("spawn", force=True)
+except RuntimeError as e:
+    pass
+
 
 def run(
     data: pd.DataFrame,
     name: str = None,
     embeddings: Any = None,
     primary_key: str = None,
     column_info: List[ColumnInputInfo] = None,
@@ -34,47 +40,53 @@
         column_info=column_info,
         host=host,
         port=port,
         load_example_data=load_example_data,
         api_key=api_key,
     )
 
+    dsInfo, load_tables, load_embeddings = preprocess.validate_and_run_preprocess(args)
+
     if is_notebook():
         print("Running from a notebook, starting a new process")
 
         global TEXTURE_SERVER_PROCESS
         if TEXTURE_SERVER_PROCESS is not None:
             print("Terminating existing server process")
             TEXTURE_SERVER_PROCESS.terminate()
 
-        TEXTURE_SERVER_PROCESS = Process(
+        TEXTURE_SERVER_PROCESS = multiprocess.Process(
             target=run_server,
-            args=(args,),
+            args=(args, dsInfo, load_tables, load_embeddings),
         )
         TEXTURE_SERVER_PROCESS.start()
         # below will block notebook from progressing past server cell
         # TEXTURE_SERVER_PROCESS.join()
     else:
-        run_server(args)
+        run_server(args, dsInfo, load_tables, load_embeddings)
 
 
-def run_server(args: Union[TextureInitArgs, Dict]):
-    args = TextureInitArgs(**args) if isinstance(args, dict) else args
-
-    dsInfo, load_tables, load_embeddings = preprocess.validate_and_run_preprocess(args)
+def run_server(
+    args: TextureInitArgs,
+    dsInfo: DatasetInfo,
+    load_tables: Dict,
+    load_embeddings: Dict | None,
+):
 
     app = get_server(
         DatasetInitArgs(
-            datasetInfo=dsInfo, load_tables=load_tables, load_embeddings=load_embeddings
+            datasetInfo=dsInfo,
+            load_tables=load_tables,
+            load_embeddings=load_embeddings,
         ),
         load_example_data=args.load_example_data,
         api_key=args.api_key,
     )
 
     print(f"\n\033[1mTexture\033[0m running on http://{args.host}:{args.port}\n")
     uvicorn.run(
         app,
         host=args.host,
         port=args.port,
-        log_level="warning",
+        log_level="warning",  # info or warning
         # reload=True,
     )
```

### Comparing `texture_viz-0.0.2/texture/runner_dev.py` & `texture_viz-0.0.3/texture/runner_dev.py`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/server.py` & `texture_viz-0.0.3/texture/server.py`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/userTransformCode/transform.py` & `texture_viz-0.0.3/texture/userTransformCode/transform.py`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/userTransformLLM/client.py` & `texture_viz-0.0.3/texture/userTransformLLM/client.py`

 * *Files identical despite different names*

### Comparing `texture_viz-0.0.2/texture/utils.py` & `texture_viz-0.0.3/texture/utils.py`

 * *Files identical despite different names*

