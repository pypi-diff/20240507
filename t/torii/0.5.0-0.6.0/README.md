# Comparing `tmp/torii-0.5.0.tar.gz` & `tmp/torii-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torii-0.5.0.tar", last modified: Wed Oct 11 20:15:15 2023, max compression
+gzip compressed data, was "torii-0.6.0.tar", last modified: Tue May  7 05:48:01 2024, max compression
```

## Comparing `torii-0.5.0.tar` & `torii-0.6.0.tar`

### file list

```diff
@@ -1,302 +1,300 @@
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-11 20:15:15.639087 torii-0.5.0/
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-11 11:34:43.000000 torii-0.5.0/.gitattributes
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-11 20:15:15.579087 torii-0.5.0/.github/
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-11 20:15:15.579087 torii-0.5.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1406 2023-10-11 11:34:43.000000 torii-0.5.0/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)       99 2023-10-11 11:34:43.000000 torii-0.5.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      674 2023-10-11 11:34:43.000000 torii-0.5.0/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)       54 2023-10-11 11:34:43.000000 torii-0.5.0/.github/codecov.yml
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-11 20:15:15.579087 torii-0.5.0/.github/workflows/
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      845 2023-10-11 11:34:43.000000 torii-0.5.0/.github/workflows/codeql.yml
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      982 2023-10-11 11:34:43.000000 torii-0.5.0/.github/workflows/docs.yaml
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1348 2023-10-11 11:34:43.000000 torii-0.5.0/.github/workflows/pr.yaml
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1306 2023-10-11 11:34:43.000000 torii-0.5.0/.github/workflows/tests.yaml
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      219 2023-10-11 11:34:43.000000 torii-0.5.0/.gitignore
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)    11676 2023-10-11 20:11:31.000000 torii-0.5.0/CHANGELOG.md
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     5222 2023-10-11 11:34:43.000000 torii-0.5.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      922 2023-10-11 11:34:43.000000 torii-0.5.0/CONTRIBUTING.md
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1405 2023-10-11 11:34:43.000000 torii-0.5.0/LICENSE
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     4286 2023-10-11 20:15:15.635754 torii-0.5.0/PKG-INFO
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     2704 2023-10-11 11:34:43.000000 torii-0.5.0/README.md
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-11 20:15:15.582420 torii-0.5.0/contrib/
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      298 2023-10-11 11:34:43.000000 torii-0.5.0/contrib/.flake8
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)       30 2023-10-11 11:34:43.000000 torii-0.5.0/contrib/.mypy.ini
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)       85 2023-10-11 11:34:43.000000 torii-0.5.0/contrib/coveragerc
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-11 20:15:15.582420 torii-0.5.0/docs/
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)        8 2022-11-08 04:43:46.000000 torii-0.5.0/docs/.gitignore
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-11 20:15:15.585754 torii-0.5.0/docs/_code/
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      566 2023-10-11 11:34:43.000000 torii-0.5.0/docs/_code/led_blinker.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1773 2023-10-11 11:34:43.000000 torii-0.5.0/docs/_code/up_counter.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1358 2023-10-11 11:34:43.000000 torii-0.5.0/docs/_code/up_counter.v
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-11 20:15:15.585754 torii-0.5.0/docs/_images/
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)    16425 2023-10-11 11:34:43.000000 torii-0.5.0/docs/_images/up_counter_gtkwave.png
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-11 20:15:15.565754 torii-0.5.0/docs/_static/
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-11 20:15:15.585754 torii-0.5.0/docs/_static/css/
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     5062 2023-10-11 11:34:43.000000 torii-0.5.0/docs/_static/css/styles.css
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-11 20:15:15.585754 torii-0.5.0/docs/_static/js/
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)   181781 2023-10-11 11:34:43.000000 torii-0.5.0/docs/_static/js/wavedrom.min.js
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)    40815 2023-10-11 11:34:43.000000 torii-0.5.0/docs/_static/js/wavedrom.skin.js
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-11 20:15:15.585754 torii-0.5.0/docs/_templates/
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1135 2023-10-11 11:34:43.000000 torii-0.5.0/docs/_templates/versions.html
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-11 20:15:15.585754 torii-0.5.0/docs/api/
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-11 20:15:15.589087 torii-0.5.0/docs/api/backend/
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      242 2023-10-11 11:34:43.000000 torii-0.5.0/docs/api/backend/cxxrtl.md
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      309 2023-10-11 11:34:43.000000 torii-0.5.0/docs/api/backend/index.md
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      240 2023-10-11 11:34:43.000000 torii-0.5.0/docs/api/backend/rtlil.md
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      244 2023-10-11 11:34:43.000000 torii-0.5.0/docs/api/backend/verilog.md
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-11 20:15:15.589087 torii-0.5.0/docs/api/hdl/
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      244 2023-10-11 11:34:43.000000 torii-0.5.0/docs/api/hdl/ast.md
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      235 2023-10-11 11:34:43.000000 torii-0.5.0/docs/api/hdl/cd.md
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      227 2023-10-11 11:34:43.000000 torii-0.5.0/docs/api/hdl/dsl.md
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      241 2023-10-11 11:34:43.000000 torii-0.5.0/docs/api/hdl/index.md
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      225 2023-10-11 11:34:43.000000 torii-0.5.0/docs/api/hdl/ir.md
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      230 2023-10-11 11:34:43.000000 torii-0.5.0/docs/api/hdl/mem.md
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      231 2023-10-11 11:34:43.000000 torii-0.5.0/docs/api/hdl/rec.md
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      229 2023-10-11 11:34:43.000000 torii-0.5.0/docs/api/hdl/xfrm.md
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      232 2023-10-11 11:34:43.000000 torii-0.5.0/docs/api/index.md
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)       33 2023-10-11 11:34:43.000000 torii-0.5.0/docs/changelog.md
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     2060 2023-10-11 11:34:43.000000 torii-0.5.0/docs/conf.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     5607 2023-10-11 11:34:43.000000 torii-0.5.0/docs/getting_started.md
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1640 2023-10-11 11:34:43.000000 torii-0.5.0/docs/index.md
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)    12464 2023-10-11 11:34:43.000000 torii-0.5.0/docs/install.md
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     7919 2023-10-11 11:34:43.000000 torii-0.5.0/docs/intro.md
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-11 20:15:15.589087 torii-0.5.0/docs/language/
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)    38527 2023-10-11 11:34:43.000000 torii-0.5.0/docs/language/index.md
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-11 20:15:15.592420 torii-0.5.0/docs/library/
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      338 2023-10-11 11:34:43.000000 torii-0.5.0/docs/library/cdc.md
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-11 20:15:15.592420 torii-0.5.0/docs/library/coding/
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      524 2023-10-11 11:34:43.000000 torii-0.5.0/docs/library/coding/index.md
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      518 2023-10-11 11:34:43.000000 torii-0.5.0/docs/library/fifo.md
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      373 2023-10-11 11:34:43.000000 torii-0.5.0/docs/library/index.md
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-11 20:15:15.592420 torii-0.5.0/docs/library/soc/
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-11 20:15:15.592420 torii-0.5.0/docs/library/soc/csr/
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      400 2023-10-11 11:34:43.000000 torii-0.5.0/docs/library/soc/csr/index.md
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      159 2023-10-11 11:34:43.000000 torii-0.5.0/docs/library/soc/event.md
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      200 2023-10-11 11:34:43.000000 torii-0.5.0/docs/library/soc/index.md
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      129 2023-10-11 11:34:43.000000 torii-0.5.0/docs/library/soc/memory.md
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      281 2023-10-11 11:34:43.000000 torii-0.5.0/docs/library/soc/periph.md
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-11 20:15:15.592420 torii-0.5.0/docs/library/soc/wishbone/
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      295 2023-10-11 11:34:43.000000 torii-0.5.0/docs/library/soc/wishbone/index.md
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-11 20:15:15.592420 torii-0.5.0/docs/library/stdio/
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      292 2023-10-11 11:34:43.000000 torii-0.5.0/docs/library/stdio/index.md
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-11 20:15:15.592420 torii-0.5.0/docs/library/vendor/
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      196 2023-10-11 11:34:43.000000 torii-0.5.0/docs/library/vendor/index.md
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-11 20:15:15.592420 torii-0.5.0/docs/library/vendor/lattice/
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      227 2023-10-11 11:34:43.000000 torii-0.5.0/docs/library/vendor/lattice/index.md
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-11 20:15:15.592420 torii-0.5.0/docs/library/vendor/xilinx/
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      126 2023-10-11 11:34:43.000000 torii-0.5.0/docs/library/vendor/xilinx/index.md
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-11 20:15:15.595754 torii-0.5.0/docs/platforms/
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-11 20:15:15.595754 torii-0.5.0/docs/platforms/fpga/
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      326 2023-10-11 11:34:43.000000 torii-0.5.0/docs/platforms/fpga/gowin.md
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      258 2023-10-11 11:34:43.000000 torii-0.5.0/docs/platforms/fpga/index.md
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      396 2023-10-11 11:34:43.000000 torii-0.5.0/docs/platforms/fpga/intel.md
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      362 2023-10-11 11:34:43.000000 torii-0.5.0/docs/platforms/fpga/lattice-ecp5.md
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      363 2023-10-11 11:34:43.000000 torii-0.5.0/docs/platforms/fpga/lattice-ice40.md
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      664 2023-10-11 11:34:43.000000 torii-0.5.0/docs/platforms/fpga/lattice-machxo-2-3l.md
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      313 2023-10-11 11:34:43.000000 torii-0.5.0/docs/platforms/fpga/quicklogic.md
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      464 2023-10-11 11:34:43.000000 torii-0.5.0/docs/platforms/fpga/xilinx.md
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      180 2023-10-11 11:34:43.000000 torii-0.5.0/docs/platforms/index.md
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      515 2023-10-11 11:34:43.000000 torii-0.5.0/docs/projects.md
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      112 2023-10-11 11:34:43.000000 torii-0.5.0/docs/requirements.txt
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-11 20:15:15.595754 torii-0.5.0/docs/sim/
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)       52 2023-10-11 11:34:43.000000 torii-0.5.0/docs/sim/index.md
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-11 20:15:15.595754 torii-0.5.0/docs/tutorials/
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     3335 2023-10-11 11:34:43.000000 torii-0.5.0/docs/tutorials/external_modules.md
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      724 2023-10-11 11:34:43.000000 torii-0.5.0/docs/tutorials/index.md
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-11 20:15:15.569087 torii-0.5.0/examples/
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-11 20:15:15.599087 torii-0.5.0/examples/basic/
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      810 2023-10-11 11:34:43.000000 torii-0.5.0/examples/basic/alu.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1342 2023-10-11 11:34:43.000000 torii-0.5.0/examples/basic/alu_hier.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      608 2023-10-11 11:34:43.000000 torii-0.5.0/examples/basic/arst.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      326 2023-10-11 11:34:43.000000 torii-0.5.0/examples/basic/cdc.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      495 2023-10-11 11:34:43.000000 torii-0.5.0/examples/basic/ctr.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      904 2023-10-11 11:34:43.000000 torii-0.5.0/examples/basic/ctr_en.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1429 2023-10-11 11:34:43.000000 torii-0.5.0/examples/basic/fsm.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      705 2023-10-11 11:34:43.000000 torii-0.5.0/examples/basic/gpio.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      664 2023-10-11 11:34:43.000000 torii-0.5.0/examples/basic/inst.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      822 2023-10-11 11:34:43.000000 torii-0.5.0/examples/basic/mem.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      752 2023-10-11 11:34:43.000000 torii-0.5.0/examples/basic/pmux.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      508 2023-10-11 11:34:43.000000 torii-0.5.0/examples/basic/por.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      751 2023-10-11 11:34:43.000000 torii-0.5.0/examples/basic/sel.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     3731 2023-10-11 11:34:43.000000 torii-0.5.0/examples/basic/uart.py
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-11 20:15:15.602420 torii-0.5.0/examples/board/
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      701 2023-10-11 11:34:43.000000 torii-0.5.0/examples/board/01_blinky.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      956 2023-10-11 11:34:43.000000 torii-0.5.0/examples/board/02_domain.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     3034 2023-10-11 11:34:43.000000 torii-0.5.0/noxfile.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)       38 2023-10-11 20:15:15.639087 torii-0.5.0/setup.cfg
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     2714 2023-10-11 11:34:43.000000 torii-0.5.0/setup.py
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-11 20:15:15.602420 torii-0.5.0/tests/
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)       40 2023-10-11 11:34:43.000000 torii-0.5.0/tests/__init__.py
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-11 20:15:15.602420 torii-0.5.0/tests/back/
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)       40 2023-10-11 11:34:43.000000 torii-0.5.0/tests/back/__init__.py
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-11 20:15:15.602420 torii-0.5.0/tests/build/
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)       40 2023-10-11 11:34:43.000000 torii-0.5.0/tests/build/__init__.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)    11304 2023-10-11 11:34:43.000000 torii-0.5.0/tests/build/test_dsl.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1993 2023-10-11 11:34:43.000000 torii-0.5.0/tests/build/test_plat.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)    10692 2023-10-11 11:34:43.000000 torii-0.5.0/tests/build/test_res.py
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-11 20:15:15.605754 torii-0.5.0/tests/hdl/
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)       40 2023-10-11 11:34:43.000000 torii-0.5.0/tests/hdl/__init__.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)    42073 2023-10-11 11:34:43.000000 torii-0.5.0/tests/hdl/test_ast.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     2507 2023-10-11 11:34:43.000000 torii-0.5.0/tests/hdl/test_cd.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)    20805 2023-10-11 11:34:43.000000 torii-0.5.0/tests/hdl/test_dsl.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)    21317 2023-10-11 11:34:43.000000 torii-0.5.0/tests/hdl/test_ir.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     5042 2023-10-11 11:34:43.000000 torii-0.5.0/tests/hdl/test_mem.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)    15964 2023-10-11 11:34:43.000000 torii-0.5.0/tests/hdl/test_rec.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)    12392 2023-10-11 11:34:43.000000 torii-0.5.0/tests/hdl/test_xfrm.py
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-11 20:15:15.605754 torii-0.5.0/tests/lib/
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)       40 2023-10-11 11:34:43.000000 torii-0.5.0/tests/lib/__init__.py
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-11 20:15:15.609087 torii-0.5.0/tests/lib/coding/
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)       40 2023-10-11 11:34:43.000000 torii-0.5.0/tests/lib/coding/__init__.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1511 2023-10-11 11:34:43.000000 torii-0.5.0/tests/lib/coding/test_gray.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1362 2023-10-11 11:34:43.000000 torii-0.5.0/tests/lib/coding/test_one_hot.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      911 2023-10-11 11:34:43.000000 torii-0.5.0/tests/lib/coding/test_priotity.py
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-11 20:15:15.609087 torii-0.5.0/tests/lib/soc/
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)       40 2023-10-11 11:34:43.000000 torii-0.5.0/tests/lib/soc/__init__.py
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-11 20:15:15.609087 torii-0.5.0/tests/lib/soc/csr/
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)       40 2023-10-11 11:34:43.000000 torii-0.5.0/tests/lib/soc/csr/__init__.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)    12496 2023-10-11 11:34:43.000000 torii-0.5.0/tests/lib/soc/csr/test_bus.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     3951 2023-10-11 11:34:43.000000 torii-0.5.0/tests/lib/soc/csr/test_event.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     6457 2023-10-11 11:34:43.000000 torii-0.5.0/tests/lib/soc/csr/test_wishbone.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     5828 2023-10-11 11:34:43.000000 torii-0.5.0/tests/lib/soc/test_event.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)    21141 2023-10-11 11:34:43.000000 torii-0.5.0/tests/lib/soc/test_memory.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     5557 2023-10-11 11:34:43.000000 torii-0.5.0/tests/lib/soc/test_periph.py
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-11 20:15:15.609087 torii-0.5.0/tests/lib/soc/wishbone/
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)       40 2023-10-11 11:34:43.000000 torii-0.5.0/tests/lib/soc/wishbone/__init__.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)    22508 2023-10-11 11:34:43.000000 torii-0.5.0/tests/lib/soc/wishbone/test_bus.py
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-11 20:15:15.609087 torii-0.5.0/tests/lib/stdio/
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)       40 2023-10-11 11:34:43.000000 torii-0.5.0/tests/lib/stdio/__init__.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     8234 2023-10-11 11:34:43.000000 torii-0.5.0/tests/lib/stdio/test_serial.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     7076 2023-10-11 11:34:43.000000 torii-0.5.0/tests/lib/test_cdc.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)    12742 2023-10-11 11:34:43.000000 torii-0.5.0/tests/lib/test_fifo.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     5940 2023-10-11 11:34:43.000000 torii-0.5.0/tests/lib/test_io.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     2745 2023-10-11 11:34:43.000000 torii-0.5.0/tests/lib/test_scheduler.py
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-11 20:15:15.612420 torii-0.5.0/tests/platform/
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)       40 2023-10-11 11:34:43.000000 torii-0.5.0/tests/platform/__init__.py
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-11 20:15:15.612420 torii-0.5.0/tests/sim/
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)       40 2023-10-11 11:34:43.000000 torii-0.5.0/tests/sim/__init__.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)    39389 2023-10-11 11:34:43.000000 torii-0.5.0/tests/sim/test_sim.py
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-11 20:15:15.612420 torii-0.5.0/tests/test/
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)       40 2023-10-11 11:34:43.000000 torii-0.5.0/tests/test/__init__.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1797 2023-10-11 11:34:43.000000 torii-0.5.0/tests/test/test_test.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1129 2023-10-11 11:34:43.000000 torii-0.5.0/tests/test_examples.py
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-11 20:15:15.612420 torii-0.5.0/tests/tools/
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)       40 2023-10-11 11:34:43.000000 torii-0.5.0/tests/tools/__init__.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1917 2023-10-11 11:34:43.000000 torii-0.5.0/tests/tools/test_cxx.py
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-11 20:15:15.612420 torii-0.5.0/tests/util/
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)       40 2023-10-11 11:34:43.000000 torii-0.5.0/tests/util/__init__.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1109 2023-10-11 11:34:43.000000 torii-0.5.0/tests/util/test_string.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     2024 2023-10-11 11:34:43.000000 torii-0.5.0/tests/util/test_tracer.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1180 2023-10-11 11:34:43.000000 torii-0.5.0/tests/util/test_units.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     2506 2023-10-11 11:34:43.000000 torii-0.5.0/tests/utils.py
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-11 20:15:15.615754 torii-0.5.0/torii/
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1005 2023-10-11 11:34:43.000000 torii-0.5.0/torii/__init__.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      264 2023-10-11 11:34:43.000000 torii-0.5.0/torii/asserts.py
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-11 20:15:15.615754 torii-0.5.0/torii/back/
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      564 2023-10-11 11:34:43.000000 torii-0.5.0/torii/back/__init__.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1630 2023-10-11 11:34:43.000000 torii-0.5.0/torii/back/cxxrtl.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)    35046 2023-10-11 11:34:43.000000 torii-0.5.0/torii/back/rtlil.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     2105 2023-10-11 11:34:43.000000 torii-0.5.0/torii/back/verilog.py
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-11 20:15:15.619087 torii-0.5.0/torii/build/
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      401 2023-10-11 11:34:43.000000 torii-0.5.0/torii/build/__init__.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     8757 2023-10-11 11:34:43.000000 torii-0.5.0/torii/build/dsl.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)    18485 2023-10-11 11:34:43.000000 torii-0.5.0/torii/build/plat.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)    10227 2023-10-11 11:34:43.000000 torii-0.5.0/torii/build/res.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     6603 2023-10-11 11:34:43.000000 torii-0.5.0/torii/build/run.py
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-11 20:15:15.619087 torii-0.5.0/torii/hdl/
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      673 2023-10-11 11:34:43.000000 torii-0.5.0/torii/hdl/__init__.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1536 2023-10-11 11:34:43.000000 torii-0.5.0/torii/hdl/_unused.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)    58255 2023-10-11 11:34:43.000000 torii-0.5.0/torii/hdl/ast.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     2725 2023-10-11 11:34:43.000000 torii-0.5.0/torii/hdl/cd.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)    17834 2023-10-11 11:34:43.000000 torii-0.5.0/torii/hdl/dsl.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)    20885 2023-10-11 11:34:43.000000 torii-0.5.0/torii/hdl/ir.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)    12881 2023-10-11 11:34:43.000000 torii-0.5.0/torii/hdl/mem.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     9142 2023-10-11 11:34:43.000000 torii-0.5.0/torii/hdl/rec.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)    21387 2023-10-11 11:34:43.000000 torii-0.5.0/torii/hdl/xfrm.py
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-11 20:15:15.622420 torii-0.5.0/torii/lib/
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)       56 2023-10-11 11:34:43.000000 torii-0.5.0/torii/lib/__init__.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     9919 2023-10-11 11:34:43.000000 torii-0.5.0/torii/lib/cdc.py
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-11 20:15:15.622420 torii-0.5.0/torii/lib/coding/
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      337 2023-10-11 11:34:43.000000 torii-0.5.0/torii/lib/coding/__init__.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1135 2023-10-11 11:34:43.000000 torii-0.5.0/torii/lib/coding/gray.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1733 2023-10-11 11:34:43.000000 torii-0.5.0/torii/lib/coding/one_hot.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1130 2023-10-11 11:34:43.000000 torii-0.5.0/torii/lib/coding/priority.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)    18102 2023-10-11 11:34:43.000000 torii-0.5.0/torii/lib/fifo.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     4489 2023-10-11 11:34:43.000000 torii-0.5.0/torii/lib/io.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1635 2023-10-11 11:34:43.000000 torii-0.5.0/torii/lib/scheduler.py
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-11 20:15:15.622420 torii-0.5.0/torii/lib/soc/
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)       56 2023-10-11 11:34:43.000000 torii-0.5.0/torii/lib/soc/__init__.py
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-11 20:15:15.625754 torii-0.5.0/torii/lib/soc/csr/
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      219 2023-10-11 11:34:43.000000 torii-0.5.0/torii/lib/soc/csr/__init__.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)    14824 2023-10-11 11:34:43.000000 torii-0.5.0/torii/lib/soc/csr/bus.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     3053 2023-10-11 11:34:43.000000 torii-0.5.0/torii/lib/soc/csr/event.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     3311 2023-10-11 11:34:43.000000 torii-0.5.0/torii/lib/soc/csr/wishbone.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     5468 2023-10-11 11:34:43.000000 torii-0.5.0/torii/lib/soc/event.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)    23039 2023-10-11 11:34:43.000000 torii-0.5.0/torii/lib/soc/memory.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     5259 2023-10-11 11:34:43.000000 torii-0.5.0/torii/lib/soc/periph.py
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-11 20:15:15.625754 torii-0.5.0/torii/lib/soc/wishbone/
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      195 2023-10-11 11:34:43.000000 torii-0.5.0/torii/lib/soc/wishbone/__init__.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)    16868 2023-10-11 11:34:43.000000 torii-0.5.0/torii/lib/soc/wishbone/bus.py
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-11 20:15:15.625754 torii-0.5.0/torii/lib/stdio/
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)       56 2023-10-11 11:34:43.000000 torii-0.5.0/torii/lib/stdio/__init__.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     8094 2023-10-11 11:34:43.000000 torii-0.5.0/torii/lib/stdio/serial.py
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-11 20:15:15.625754 torii-0.5.0/torii/lib/vendor/
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)       56 2023-10-11 11:34:43.000000 torii-0.5.0/torii/lib/vendor/__init__.py
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-11 20:15:15.625754 torii-0.5.0/torii/lib/vendor/lattice/
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)       56 2023-10-11 11:34:43.000000 torii-0.5.0/torii/lib/vendor/lattice/__init__.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      631 2023-10-11 11:34:43.000000 torii-0.5.0/torii/lib/vendor/lattice/ice40.py
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-11 20:15:15.625754 torii-0.5.0/torii/lib/vendor/xilinx/
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)       56 2023-10-11 11:34:43.000000 torii-0.5.0/torii/lib/vendor/xilinx/__init__.py
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-11 20:15:15.625754 torii-0.5.0/torii/platform/
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)       56 2023-10-11 11:34:43.000000 torii-0.5.0/torii/platform/__init__.py
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-11 20:15:15.629087 torii-0.5.0/torii/platform/resources/
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1399 2023-10-11 11:34:43.000000 torii-0.5.0/torii/platform/resources/__init__.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     2977 2023-10-11 11:34:43.000000 torii-0.5.0/torii/platform/resources/display.py
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-11 20:15:15.629087 torii-0.5.0/torii/platform/resources/extensions/
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      493 2023-10-11 11:34:43.000000 torii-0.5.0/torii/platform/resources/extensions/__init__.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     3522 2023-10-11 11:34:43.000000 torii-0.5.0/torii/platform/resources/extensions/pmod.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)    11031 2023-10-11 11:34:43.000000 torii-0.5.0/torii/platform/resources/interface.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)    12158 2023-10-11 11:34:43.000000 torii-0.5.0/torii/platform/resources/memory.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1987 2023-10-11 11:34:43.000000 torii-0.5.0/torii/platform/resources/user.py
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-11 20:15:15.632420 torii-0.5.0/torii/platform/vendor/
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      520 2023-10-11 11:34:43.000000 torii-0.5.0/torii/platform/vendor/__init__.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)    17075 2023-10-11 11:34:43.000000 torii-0.5.0/torii/platform/vendor/gowin.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)    18703 2023-10-11 11:34:43.000000 torii-0.5.0/torii/platform/vendor/intel.py
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-11 20:15:15.632420 torii-0.5.0/torii/platform/vendor/lattice/
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      547 2023-10-11 11:34:43.000000 torii-0.5.0/torii/platform/vendor/lattice/__init__.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)    23143 2023-10-11 11:34:43.000000 torii-0.5.0/torii/platform/vendor/lattice/ecp5.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)    22651 2023-10-11 11:34:43.000000 torii-0.5.0/torii/platform/vendor/lattice/ice40.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)    16580 2023-10-11 11:34:43.000000 torii-0.5.0/torii/platform/vendor/lattice/machxo_2_3l.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      309 2023-10-11 11:34:43.000000 torii-0.5.0/torii/platform/vendor/lattice_ecp5.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      316 2023-10-11 11:34:43.000000 torii-0.5.0/torii/platform/vendor/lattice_ice40.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      573 2023-10-11 11:34:43.000000 torii-0.5.0/torii/platform/vendor/lattice_machxo_2_3l.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     5683 2023-10-11 11:34:43.000000 torii-0.5.0/torii/platform/vendor/quicklogic.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)    41698 2023-10-11 11:34:43.000000 torii-0.5.0/torii/platform/vendor/xilinx.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-11 11:34:43.000000 torii-0.5.0/torii/py.typed
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-11 20:15:15.635754 torii-0.5.0/torii/sim/
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      189 2023-10-11 11:34:43.000000 torii-0.5.0/torii/sim/__init__.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1532 2023-10-11 11:34:43.000000 torii-0.5.0/torii/sim/_base.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      712 2023-10-11 11:34:43.000000 torii-0.5.0/torii/sim/_pyclock.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     4640 2023-10-11 11:34:43.000000 torii-0.5.0/torii/sim/_pycoro.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)    15259 2023-10-11 11:34:43.000000 torii-0.5.0/torii/sim/_pyrtl.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     7883 2023-10-11 11:34:43.000000 torii-0.5.0/torii/sim/core.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     9427 2023-10-11 11:34:43.000000 torii-0.5.0/torii/sim/pysim.py
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-11 20:15:15.635754 torii-0.5.0/torii/test/
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     8477 2023-10-11 11:34:43.000000 torii-0.5.0/torii/test/__init__.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     2365 2023-10-11 11:34:43.000000 torii-0.5.0/torii/test/mock.py
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-11 20:15:15.635754 torii-0.5.0/torii/tools/
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1819 2023-10-11 11:34:43.000000 torii-0.5.0/torii/tools/__init__.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     2479 2023-10-11 11:34:43.000000 torii-0.5.0/torii/tools/cxx.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     4635 2023-10-11 11:34:43.000000 torii-0.5.0/torii/tools/yosys.py
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-11 20:15:15.635754 torii-0.5.0/torii/util/
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1483 2023-10-11 11:34:43.000000 torii-0.5.0/torii/util/__init__.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      922 2023-10-11 11:34:43.000000 torii-0.5.0/torii/util/decorators.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1257 2023-10-11 11:34:43.000000 torii-0.5.0/torii/util/string.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     2174 2023-10-11 11:34:43.000000 torii-0.5.0/torii/util/tracer.py
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     2192 2023-10-11 11:34:43.000000 torii-0.5.0/torii/util/units.py
-drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-11 20:15:15.615754 torii-0.5.0/torii.egg-info/
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     4286 2023-10-11 20:15:15.000000 torii-0.5.0/torii.egg-info/PKG-INFO
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     5815 2023-10-11 20:15:15.000000 torii-0.5.0/torii.egg-info/SOURCES.txt
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)        1 2023-10-11 20:15:15.000000 torii-0.5.0/torii.egg-info/dependency_links.txt
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)       60 2023-10-11 20:15:15.000000 torii-0.5.0/torii.egg-info/requires.txt
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)        6 2023-10-11 20:15:15.000000 torii-0.5.0/torii.egg-info/top_level.txt
--rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)        1 2022-11-30 20:07:38.000000 torii-0.5.0/torii.egg-info/zip-safe
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 05:48:01.086859 torii-0.6.0/
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-11 11:34:43.000000 torii-0.6.0/.gitattributes
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 05:48:01.036859 torii-0.6.0/.github/
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 05:48:01.036859 torii-0.6.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1406 2023-10-11 11:34:43.000000 torii-0.6.0/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)       99 2023-10-11 11:34:43.000000 torii-0.6.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      674 2023-10-11 11:34:43.000000 torii-0.6.0/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)       54 2023-10-11 11:34:43.000000 torii-0.6.0/.github/codecov.yml
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 05:48:01.036859 torii-0.6.0/.github/workflows/
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      845 2024-02-07 16:58:19.000000 torii-0.6.0/.github/workflows/codeql.yml
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      985 2024-03-14 08:29:00.000000 torii-0.6.0/.github/workflows/docs.yaml
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1465 2024-03-14 08:29:00.000000 torii-0.6.0/.github/workflows/pr.yaml
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1340 2024-04-25 14:50:19.000000 torii-0.6.0/.github/workflows/tests.yaml
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      219 2023-10-11 11:34:43.000000 torii-0.6.0/.gitignore
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)    15952 2024-05-07 05:40:53.000000 torii-0.6.0/CHANGELOG.md
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     5222 2023-10-11 11:34:43.000000 torii-0.6.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      922 2023-10-11 11:34:43.000000 torii-0.6.0/CONTRIBUTING.md
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1405 2023-10-11 11:34:43.000000 torii-0.6.0/LICENSE
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     4280 2024-05-07 05:48:01.086859 torii-0.6.0/PKG-INFO
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     2704 2024-04-25 14:50:19.000000 torii-0.6.0/README.md
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 05:48:01.036859 torii-0.6.0/contrib/
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      298 2023-10-11 11:34:43.000000 torii-0.6.0/contrib/.flake8
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)       30 2023-10-11 11:34:43.000000 torii-0.6.0/contrib/.mypy.ini
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)       85 2023-10-11 11:34:43.000000 torii-0.6.0/contrib/coveragerc
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 05:48:01.040193 torii-0.6.0/docs/
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)        8 2022-11-08 04:43:46.000000 torii-0.6.0/docs/.gitignore
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 05:48:01.040193 torii-0.6.0/docs/_code/
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      566 2023-10-11 11:34:43.000000 torii-0.6.0/docs/_code/led_blinker.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1773 2023-10-11 11:34:43.000000 torii-0.6.0/docs/_code/up_counter.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1358 2023-10-11 11:34:43.000000 torii-0.6.0/docs/_code/up_counter.v
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 05:48:01.040193 torii-0.6.0/docs/_images/
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)    16425 2023-10-11 11:34:43.000000 torii-0.6.0/docs/_images/up_counter_gtkwave.png
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 05:48:01.023526 torii-0.6.0/docs/_static/
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 05:48:01.040193 torii-0.6.0/docs/_static/css/
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     5062 2023-10-11 11:34:43.000000 torii-0.6.0/docs/_static/css/styles.css
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 05:48:01.040193 torii-0.6.0/docs/_static/js/
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)   181781 2023-10-11 11:34:43.000000 torii-0.6.0/docs/_static/js/wavedrom.min.js
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)    40815 2023-10-11 11:34:43.000000 torii-0.6.0/docs/_static/js/wavedrom.skin.js
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 05:48:01.040193 torii-0.6.0/docs/_templates/
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1135 2023-10-11 11:34:43.000000 torii-0.6.0/docs/_templates/versions.html
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 05:48:01.043526 torii-0.6.0/docs/api/
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 05:48:01.043526 torii-0.6.0/docs/api/backend/
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      242 2023-10-11 11:34:43.000000 torii-0.6.0/docs/api/backend/cxxrtl.md
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      309 2023-10-11 11:34:43.000000 torii-0.6.0/docs/api/backend/index.md
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      240 2023-10-11 11:34:43.000000 torii-0.6.0/docs/api/backend/rtlil.md
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      244 2023-10-11 11:34:43.000000 torii-0.6.0/docs/api/backend/verilog.md
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 05:48:01.043526 torii-0.6.0/docs/api/hdl/
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      244 2023-10-11 11:34:43.000000 torii-0.6.0/docs/api/hdl/ast.md
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      235 2023-10-11 11:34:43.000000 torii-0.6.0/docs/api/hdl/cd.md
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      227 2023-10-11 11:34:43.000000 torii-0.6.0/docs/api/hdl/dsl.md
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      241 2023-10-11 11:34:43.000000 torii-0.6.0/docs/api/hdl/index.md
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      225 2023-10-11 11:34:43.000000 torii-0.6.0/docs/api/hdl/ir.md
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      230 2023-10-11 11:34:43.000000 torii-0.6.0/docs/api/hdl/mem.md
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      231 2023-10-11 11:34:43.000000 torii-0.6.0/docs/api/hdl/rec.md
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      229 2023-10-11 11:34:43.000000 torii-0.6.0/docs/api/hdl/xfrm.md
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      232 2023-10-11 11:34:43.000000 torii-0.6.0/docs/api/index.md
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)       33 2023-10-11 11:34:43.000000 torii-0.6.0/docs/changelog.md
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     2060 2023-10-11 20:23:40.000000 torii-0.6.0/docs/conf.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     5607 2023-10-11 11:34:43.000000 torii-0.6.0/docs/getting_started.md
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1640 2023-10-11 11:34:43.000000 torii-0.6.0/docs/index.md
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)    12520 2024-05-05 06:18:05.000000 torii-0.6.0/docs/install.md
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     7919 2023-10-11 11:34:43.000000 torii-0.6.0/docs/intro.md
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 05:48:01.043526 torii-0.6.0/docs/language/
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)    39334 2024-05-05 05:51:20.000000 torii-0.6.0/docs/language/index.md
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 05:48:01.046859 torii-0.6.0/docs/library/
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      338 2023-10-11 11:34:43.000000 torii-0.6.0/docs/library/cdc.md
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 05:48:01.046859 torii-0.6.0/docs/library/coding/
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      524 2023-10-11 11:34:43.000000 torii-0.6.0/docs/library/coding/index.md
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      518 2023-10-11 11:34:43.000000 torii-0.6.0/docs/library/fifo.md
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      373 2023-10-11 11:34:43.000000 torii-0.6.0/docs/library/index.md
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 05:48:01.046859 torii-0.6.0/docs/library/soc/
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 05:48:01.046859 torii-0.6.0/docs/library/soc/csr/
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      400 2023-10-11 11:34:43.000000 torii-0.6.0/docs/library/soc/csr/index.md
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      159 2023-10-11 11:34:43.000000 torii-0.6.0/docs/library/soc/event.md
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      200 2023-10-11 11:34:43.000000 torii-0.6.0/docs/library/soc/index.md
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      129 2023-10-11 11:34:43.000000 torii-0.6.0/docs/library/soc/memory.md
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      281 2023-10-11 11:34:43.000000 torii-0.6.0/docs/library/soc/periph.md
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 05:48:01.046859 torii-0.6.0/docs/library/soc/wishbone/
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      295 2023-10-11 11:34:43.000000 torii-0.6.0/docs/library/soc/wishbone/index.md
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 05:48:01.046859 torii-0.6.0/docs/library/stdio/
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      292 2023-10-11 11:34:43.000000 torii-0.6.0/docs/library/stdio/index.md
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 05:48:01.046859 torii-0.6.0/docs/library/vendor/
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      196 2023-10-11 11:34:43.000000 torii-0.6.0/docs/library/vendor/index.md
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 05:48:01.046859 torii-0.6.0/docs/library/vendor/lattice/
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      227 2023-10-11 11:34:43.000000 torii-0.6.0/docs/library/vendor/lattice/index.md
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 05:48:01.050193 torii-0.6.0/docs/library/vendor/xilinx/
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      126 2023-10-11 11:34:43.000000 torii-0.6.0/docs/library/vendor/xilinx/index.md
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 05:48:01.050193 torii-0.6.0/docs/platforms/
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 05:48:01.050193 torii-0.6.0/docs/platforms/fpga/
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      400 2024-03-14 09:15:42.000000 torii-0.6.0/docs/platforms/fpga/altera.md
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      326 2023-10-11 11:34:43.000000 torii-0.6.0/docs/platforms/fpga/gowin.md
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      259 2024-03-14 09:15:42.000000 torii-0.6.0/docs/platforms/fpga/index.md
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      362 2023-10-11 11:34:43.000000 torii-0.6.0/docs/platforms/fpga/lattice-ecp5.md
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      363 2023-10-11 11:34:43.000000 torii-0.6.0/docs/platforms/fpga/lattice-ice40.md
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      664 2023-10-11 11:34:43.000000 torii-0.6.0/docs/platforms/fpga/lattice-machxo-2-3l.md
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      313 2023-10-11 11:34:43.000000 torii-0.6.0/docs/platforms/fpga/quicklogic.md
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      464 2023-10-11 11:34:43.000000 torii-0.6.0/docs/platforms/fpga/xilinx.md
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      180 2023-10-11 11:34:43.000000 torii-0.6.0/docs/platforms/index.md
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      515 2023-10-11 11:34:43.000000 torii-0.6.0/docs/projects.md
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      112 2023-10-11 11:34:43.000000 torii-0.6.0/docs/requirements.txt
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 05:48:01.050193 torii-0.6.0/docs/sim/
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)       52 2023-10-11 11:34:43.000000 torii-0.6.0/docs/sim/index.md
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 05:48:01.050193 torii-0.6.0/docs/tutorials/
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     3335 2023-10-11 11:34:43.000000 torii-0.6.0/docs/tutorials/external_modules.md
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      724 2023-10-11 11:34:43.000000 torii-0.6.0/docs/tutorials/index.md
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 05:48:01.026859 torii-0.6.0/examples/
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 05:48:01.053526 torii-0.6.0/examples/basic/
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      810 2023-10-11 11:34:43.000000 torii-0.6.0/examples/basic/alu.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1342 2023-10-11 11:34:43.000000 torii-0.6.0/examples/basic/alu_hier.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      608 2023-10-11 11:34:43.000000 torii-0.6.0/examples/basic/arst.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      326 2023-10-11 11:34:43.000000 torii-0.6.0/examples/basic/cdc.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      495 2023-10-11 11:34:43.000000 torii-0.6.0/examples/basic/ctr.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      904 2023-10-11 11:34:43.000000 torii-0.6.0/examples/basic/ctr_en.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1429 2023-10-11 11:34:43.000000 torii-0.6.0/examples/basic/fsm.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      705 2023-10-11 11:34:43.000000 torii-0.6.0/examples/basic/gpio.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      664 2023-10-11 11:34:43.000000 torii-0.6.0/examples/basic/inst.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      822 2023-10-11 11:34:43.000000 torii-0.6.0/examples/basic/mem.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      755 2024-05-05 04:32:28.000000 torii-0.6.0/examples/basic/pmux.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      508 2023-10-11 11:34:43.000000 torii-0.6.0/examples/basic/por.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      751 2023-10-11 11:34:43.000000 torii-0.6.0/examples/basic/sel.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     3731 2023-10-11 11:34:43.000000 torii-0.6.0/examples/basic/uart.py
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 05:48:01.056859 torii-0.6.0/examples/board/
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      701 2023-10-11 11:34:43.000000 torii-0.6.0/examples/board/01_blinky.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      956 2023-10-11 11:34:43.000000 torii-0.6.0/examples/board/02_domain.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     3034 2024-04-25 14:50:19.000000 torii-0.6.0/noxfile.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)       38 2024-05-07 05:48:01.086859 torii-0.6.0/setup.cfg
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     2708 2024-05-07 04:51:27.000000 torii-0.6.0/setup.py
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 05:48:01.056859 torii-0.6.0/tests/
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)       40 2023-10-11 11:34:43.000000 torii-0.6.0/tests/__init__.py
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 05:48:01.056859 torii-0.6.0/tests/back/
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)       40 2023-10-11 11:34:43.000000 torii-0.6.0/tests/back/__init__.py
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 05:48:01.056859 torii-0.6.0/tests/build/
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)       40 2023-10-11 11:34:43.000000 torii-0.6.0/tests/build/__init__.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)    11304 2023-10-11 11:34:43.000000 torii-0.6.0/tests/build/test_dsl.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1993 2023-10-11 11:34:43.000000 torii-0.6.0/tests/build/test_plat.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)    10692 2023-10-11 11:34:43.000000 torii-0.6.0/tests/build/test_res.py
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 05:48:01.060193 torii-0.6.0/tests/hdl/
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)       40 2023-10-11 11:34:43.000000 torii-0.6.0/tests/hdl/__init__.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)    48739 2024-05-07 05:09:07.000000 torii-0.6.0/tests/hdl/test_ast.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     2507 2023-10-11 11:34:43.000000 torii-0.6.0/tests/hdl/test_cd.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)    22424 2024-05-07 01:46:36.000000 torii-0.6.0/tests/hdl/test_dsl.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)    23068 2024-05-05 01:34:33.000000 torii-0.6.0/tests/hdl/test_ir.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     5042 2023-10-11 11:34:43.000000 torii-0.6.0/tests/hdl/test_mem.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)    15964 2024-05-05 01:01:58.000000 torii-0.6.0/tests/hdl/test_rec.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)    12683 2024-05-06 08:40:39.000000 torii-0.6.0/tests/hdl/test_xfrm.py
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 05:48:01.060193 torii-0.6.0/tests/lib/
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)       40 2023-10-11 11:34:43.000000 torii-0.6.0/tests/lib/__init__.py
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 05:48:01.060193 torii-0.6.0/tests/lib/coding/
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)       40 2023-10-11 11:34:43.000000 torii-0.6.0/tests/lib/coding/__init__.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1511 2023-10-11 11:34:43.000000 torii-0.6.0/tests/lib/coding/test_gray.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1362 2023-10-11 11:34:43.000000 torii-0.6.0/tests/lib/coding/test_one_hot.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      911 2023-10-11 11:34:43.000000 torii-0.6.0/tests/lib/coding/test_priotity.py
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 05:48:01.063526 torii-0.6.0/tests/lib/soc/
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)       40 2023-10-11 11:34:43.000000 torii-0.6.0/tests/lib/soc/__init__.py
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 05:48:01.063526 torii-0.6.0/tests/lib/soc/csr/
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)       40 2023-10-11 11:34:43.000000 torii-0.6.0/tests/lib/soc/csr/__init__.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)    13590 2024-05-05 07:30:42.000000 torii-0.6.0/tests/lib/soc/csr/test_bus.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     3929 2024-05-05 07:31:05.000000 torii-0.6.0/tests/lib/soc/csr/test_event.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     6413 2024-05-05 07:31:23.000000 torii-0.6.0/tests/lib/soc/csr/test_wishbone.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     5806 2024-05-05 07:30:22.000000 torii-0.6.0/tests/lib/soc/test_event.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)    21206 2023-10-23 18:11:51.000000 torii-0.6.0/tests/lib/soc/test_memory.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     5557 2023-10-11 11:34:43.000000 torii-0.6.0/tests/lib/soc/test_periph.py
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 05:48:01.063526 torii-0.6.0/tests/lib/soc/wishbone/
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)       40 2023-10-11 11:34:43.000000 torii-0.6.0/tests/lib/soc/wishbone/__init__.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)    22332 2024-05-05 07:31:36.000000 torii-0.6.0/tests/lib/soc/wishbone/test_bus.py
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 05:48:01.063526 torii-0.6.0/tests/lib/stdio/
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)       40 2023-10-11 11:34:43.000000 torii-0.6.0/tests/lib/stdio/__init__.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     8234 2023-10-11 11:34:43.000000 torii-0.6.0/tests/lib/stdio/test_serial.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     7076 2023-10-11 11:34:43.000000 torii-0.6.0/tests/lib/test_cdc.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)    12742 2024-03-11 21:19:45.000000 torii-0.6.0/tests/lib/test_fifo.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     5940 2023-10-11 11:34:43.000000 torii-0.6.0/tests/lib/test_io.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     2745 2023-10-11 11:34:43.000000 torii-0.6.0/tests/lib/test_scheduler.py
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 05:48:01.063526 torii-0.6.0/tests/platform/
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)       40 2023-10-11 11:34:43.000000 torii-0.6.0/tests/platform/__init__.py
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 05:48:01.066859 torii-0.6.0/tests/sim/
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)       40 2023-10-11 11:34:43.000000 torii-0.6.0/tests/sim/__init__.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)    40092 2024-05-07 03:46:29.000000 torii-0.6.0/tests/sim/test_sim.py
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 05:48:01.066859 torii-0.6.0/tests/test/
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)       40 2023-10-11 11:34:43.000000 torii-0.6.0/tests/test/__init__.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1797 2023-10-11 11:34:43.000000 torii-0.6.0/tests/test/test_test.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1129 2023-10-11 11:34:43.000000 torii-0.6.0/tests/test_examples.py
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 05:48:01.066859 torii-0.6.0/tests/tools/
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)       40 2023-10-11 11:34:43.000000 torii-0.6.0/tests/tools/__init__.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1917 2023-10-11 11:34:43.000000 torii-0.6.0/tests/tools/test_cxx.py
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 05:48:01.066859 torii-0.6.0/tests/util/
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)       40 2023-10-11 11:34:43.000000 torii-0.6.0/tests/util/__init__.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1109 2023-10-11 11:34:43.000000 torii-0.6.0/tests/util/test_string.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     2069 2024-05-05 07:20:07.000000 torii-0.6.0/tests/util/test_tracer.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     3889 2024-05-06 04:30:41.000000 torii-0.6.0/tests/util/test_units.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     2506 2024-05-06 22:21:55.000000 torii-0.6.0/tests/utils.py
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 05:48:01.066859 torii-0.6.0/torii/
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      990 2024-05-07 05:08:05.000000 torii-0.6.0/torii/__init__.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      264 2024-04-25 14:49:41.000000 torii-0.6.0/torii/asserts.py
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 05:48:01.070193 torii-0.6.0/torii/back/
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      564 2023-10-11 11:34:43.000000 torii-0.6.0/torii/back/__init__.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1630 2024-04-21 08:21:56.000000 torii-0.6.0/torii/back/cxxrtl.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)    37681 2024-05-07 02:38:01.000000 torii-0.6.0/torii/back/rtlil.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     2004 2024-05-05 01:08:47.000000 torii-0.6.0/torii/back/verilog.py
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 05:48:01.073526 torii-0.6.0/torii/build/
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      401 2023-10-11 11:34:43.000000 torii-0.6.0/torii/build/__init__.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     8757 2024-04-21 08:21:56.000000 torii-0.6.0/torii/build/dsl.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)    18775 2024-05-05 20:50:11.000000 torii-0.6.0/torii/build/plat.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)    10655 2024-04-21 08:21:56.000000 torii-0.6.0/torii/build/res.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     8711 2024-05-05 21:48:46.000000 torii-0.6.0/torii/build/run.py
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 05:48:01.073526 torii-0.6.0/torii/hdl/
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      658 2024-05-07 05:07:56.000000 torii-0.6.0/torii/hdl/__init__.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1582 2024-04-21 08:21:56.000000 torii-0.6.0/torii/hdl/_unused.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)    65023 2024-05-07 05:07:46.000000 torii-0.6.0/torii/hdl/ast.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     2725 2024-04-21 08:21:56.000000 torii-0.6.0/torii/hdl/cd.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)    21404 2024-05-07 02:56:04.000000 torii-0.6.0/torii/hdl/dsl.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)    24326 2024-05-06 04:47:21.000000 torii-0.6.0/torii/hdl/ir.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)    10133 2024-05-06 07:59:42.000000 torii-0.6.0/torii/hdl/mem.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     9322 2024-04-25 14:51:19.000000 torii-0.6.0/torii/hdl/rec.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)    22097 2024-05-07 03:03:47.000000 torii-0.6.0/torii/hdl/xfrm.py
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 05:48:01.073526 torii-0.6.0/torii/lib/
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)       56 2023-10-11 11:34:43.000000 torii-0.6.0/torii/lib/__init__.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     9919 2024-04-21 08:21:56.000000 torii-0.6.0/torii/lib/cdc.py
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 05:48:01.076859 torii-0.6.0/torii/lib/coding/
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      337 2023-10-11 11:34:43.000000 torii-0.6.0/torii/lib/coding/__init__.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1135 2023-10-11 11:34:43.000000 torii-0.6.0/torii/lib/coding/gray.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1736 2024-05-05 04:32:12.000000 torii-0.6.0/torii/lib/coding/one_hot.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1130 2023-10-11 11:34:43.000000 torii-0.6.0/torii/lib/coding/priority.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)    18016 2024-05-06 04:18:24.000000 torii-0.6.0/torii/lib/fifo.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     4489 2024-04-21 08:21:56.000000 torii-0.6.0/torii/lib/io.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1635 2023-10-11 11:34:43.000000 torii-0.6.0/torii/lib/scheduler.py
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 05:48:01.076859 torii-0.6.0/torii/lib/soc/
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)       56 2023-10-11 11:34:43.000000 torii-0.6.0/torii/lib/soc/__init__.py
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 05:48:01.076859 torii-0.6.0/torii/lib/soc/csr/
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      219 2023-10-11 11:34:43.000000 torii-0.6.0/torii/lib/soc/csr/__init__.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)    22321 2024-05-06 04:18:24.000000 torii-0.6.0/torii/lib/soc/csr/bus.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     3053 2023-10-11 11:34:43.000000 torii-0.6.0/torii/lib/soc/csr/event.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     3317 2024-05-06 04:18:38.000000 torii-0.6.0/torii/lib/soc/csr/wishbone.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     5534 2024-04-21 08:21:56.000000 torii-0.6.0/torii/lib/soc/event.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)    23615 2024-04-21 08:21:56.000000 torii-0.6.0/torii/lib/soc/memory.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     5259 2024-04-21 08:21:56.000000 torii-0.6.0/torii/lib/soc/periph.py
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 05:48:01.076859 torii-0.6.0/torii/lib/soc/wishbone/
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      195 2023-10-11 11:34:43.000000 torii-0.6.0/torii/lib/soc/wishbone/__init__.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)    16885 2024-05-06 04:18:38.000000 torii-0.6.0/torii/lib/soc/wishbone/bus.py
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 05:48:01.076859 torii-0.6.0/torii/lib/stdio/
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)       56 2023-10-11 11:34:43.000000 torii-0.6.0/torii/lib/stdio/__init__.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     8256 2024-04-21 08:21:56.000000 torii-0.6.0/torii/lib/stdio/serial.py
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 05:48:01.076859 torii-0.6.0/torii/lib/vendor/
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)       56 2023-10-11 11:34:43.000000 torii-0.6.0/torii/lib/vendor/__init__.py
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 05:48:01.076859 torii-0.6.0/torii/lib/vendor/lattice/
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)       56 2023-10-11 11:34:43.000000 torii-0.6.0/torii/lib/vendor/lattice/__init__.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      631 2023-10-11 11:34:43.000000 torii-0.6.0/torii/lib/vendor/lattice/ice40.py
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 05:48:01.080193 torii-0.6.0/torii/lib/vendor/xilinx/
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)       56 2023-10-11 11:34:43.000000 torii-0.6.0/torii/lib/vendor/xilinx/__init__.py
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 05:48:01.080193 torii-0.6.0/torii/platform/
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)       56 2023-10-11 11:34:43.000000 torii-0.6.0/torii/platform/__init__.py
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 05:48:01.080193 torii-0.6.0/torii/platform/resources/
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1438 2023-10-16 06:39:33.000000 torii-0.6.0/torii/platform/resources/__init__.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     2977 2024-04-21 08:21:56.000000 torii-0.6.0/torii/platform/resources/display.py
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 05:48:01.080193 torii-0.6.0/torii/platform/resources/extensions/
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      493 2023-10-11 11:34:43.000000 torii-0.6.0/torii/platform/resources/extensions/__init__.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     3522 2023-10-11 11:34:43.000000 torii-0.6.0/torii/platform/resources/extensions/pmod.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)    13010 2024-04-21 08:21:56.000000 torii-0.6.0/torii/platform/resources/interface.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)    12500 2024-04-21 08:21:56.000000 torii-0.6.0/torii/platform/resources/memory.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1987 2024-04-21 08:21:56.000000 torii-0.6.0/torii/platform/resources/user.py
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 05:48:01.080193 torii-0.6.0/torii/platform/vendor/
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      522 2024-03-14 09:15:42.000000 torii-0.6.0/torii/platform/vendor/__init__.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)    19666 2024-05-05 20:52:11.000000 torii-0.6.0/torii/platform/vendor/altera.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)    18445 2024-05-05 01:56:56.000000 torii-0.6.0/torii/platform/vendor/gowin.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      274 2024-03-14 09:15:42.000000 torii-0.6.0/torii/platform/vendor/intel.py
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 05:48:01.083526 torii-0.6.0/torii/platform/vendor/lattice/
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      547 2023-10-11 11:34:43.000000 torii-0.6.0/torii/platform/vendor/lattice/__init__.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)    23747 2024-05-05 20:53:41.000000 torii-0.6.0/torii/platform/vendor/lattice/ecp5.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)    23840 2024-05-05 20:51:28.000000 torii-0.6.0/torii/platform/vendor/lattice/ice40.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)    16827 2024-05-05 20:52:01.000000 torii-0.6.0/torii/platform/vendor/lattice/machxo_2_3l.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     5683 2024-04-21 08:21:56.000000 torii-0.6.0/torii/platform/vendor/quicklogic.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)    42806 2024-05-05 20:54:24.000000 torii-0.6.0/torii/platform/vendor/xilinx.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)        0 2023-10-11 11:34:43.000000 torii-0.6.0/torii/py.typed
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 05:48:01.083526 torii-0.6.0/torii/sim/
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      189 2023-10-11 11:34:43.000000 torii-0.6.0/torii/sim/__init__.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1532 2024-04-21 08:21:56.000000 torii-0.6.0/torii/sim/_base.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      787 2023-10-23 18:11:51.000000 torii-0.6.0/torii/sim/_pyclock.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     3896 2024-05-07 03:47:40.000000 torii-0.6.0/torii/sim/_pycoro.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)    15152 2024-05-07 03:05:01.000000 torii-0.6.0/torii/sim/_pyrtl.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     8050 2024-04-21 08:21:56.000000 torii-0.6.0/torii/sim/core.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     9612 2024-05-05 07:10:07.000000 torii-0.6.0/torii/sim/pysim.py
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 05:48:01.083526 torii-0.6.0/torii/test/
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     8514 2024-04-21 08:21:56.000000 torii-0.6.0/torii/test/__init__.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     2365 2023-10-11 11:34:43.000000 torii-0.6.0/torii/test/mock.py
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 05:48:01.083526 torii-0.6.0/torii/tools/
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1819 2023-10-11 11:34:43.000000 torii-0.6.0/torii/tools/__init__.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     2479 2023-10-11 11:34:43.000000 torii-0.6.0/torii/tools/cxx.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     4671 2024-05-05 06:17:18.000000 torii-0.6.0/torii/tools/yosys.py
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 05:48:01.086859 torii-0.6.0/torii/util/
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1586 2024-04-21 08:21:56.000000 torii-0.6.0/torii/util/__init__.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)      922 2024-05-06 04:17:08.000000 torii-0.6.0/torii/util/decorators.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     1257 2024-04-21 08:21:50.000000 torii-0.6.0/torii/util/string.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     2208 2024-05-05 07:21:58.000000 torii-0.6.0/torii/util/tracer.py
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     3184 2024-05-06 04:23:58.000000 torii-0.6.0/torii/util/units.py
+drwxr-xr-x   0 lethalbit  (1000) lethalbit  (1000)        0 2024-05-07 05:48:01.086859 torii-0.6.0/torii.egg-info/
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     4280 2024-05-07 05:48:00.000000 torii-0.6.0/torii.egg-info/PKG-INFO
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)     5726 2024-05-07 05:48:01.000000 torii-0.6.0/torii.egg-info/SOURCES.txt
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)        1 2024-05-07 05:48:00.000000 torii-0.6.0/torii.egg-info/dependency_links.txt
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)       52 2024-05-07 05:48:00.000000 torii-0.6.0/torii.egg-info/requires.txt
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)        6 2024-05-07 05:48:00.000000 torii-0.6.0/torii.egg-info/top_level.txt
+-rw-r--r--   0 lethalbit  (1000) lethalbit  (1000)        1 2022-11-30 20:07:38.000000 torii-0.6.0/torii.egg-info/zip-safe
```

### Comparing `torii-0.5.0/.github/ISSUE_TEMPLATE/bug_report.yml` & `torii-0.6.0/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `torii-0.5.0/.github/ISSUE_TEMPLATE/feature_request.yml` & `torii-0.6.0/.github/ISSUE_TEMPLATE/feature_request.yml`

 * *Files identical despite different names*

### Comparing `torii-0.5.0/.github/workflows/codeql.yml` & `torii-0.6.0/.github/workflows/codeql.yml`

 * *Files 26% similar despite different names*

```diff
@@ -19,26 +19,26 @@
     strategy:
       fail-fast: false
       matrix:
         language: [ 'python' ]
 
     steps:
     - name: Setup Python
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: 3.11
 
     - name: Checkout repository
-      uses: actions/checkout@v3
+      uses: actions/checkout@v4
 
     - name: Initialize CodeQL
-      uses: github/codeql-action/init@v2
+      uses: github/codeql-action/init@v3
       with:
         languages: ${{ matrix.language }}
 
     - name: Autobuild
-      uses: github/codeql-action/autobuild@v2
+      uses: github/codeql-action/autobuild@v3
 
     - name: Perform CodeQL Analysis
-      uses: github/codeql-action/analyze@v2
+      uses: github/codeql-action/analyze@v3
       with:
         category: "/language:${{matrix.language}}"
```

### Comparing `torii-0.5.0/.github/workflows/docs.yaml` & `torii-0.6.0/.github/workflows/docs.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 jobs:
   build-docs:
     name: Build Torii Docs
     runs-on: ubuntu-latest
     steps:
       - name: Setup Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
-          python-version: 3.9
+          python-version: '3.10'
 
       - name: Initialize Env
         shell: bash
         env:
           WORKSPACE: ${{ github.workspace }}
         run: |
           echo "$HOME/.local/bin:$PATH" >> $GITHUB_PATH
           echo "GITHUB_WORKSPACE=\"`pwd`\"" >> $GITHUB_ENV
 
       - name: Checkout
-        uses: actions/checkout@v3
+        uses: actions/checkout@v4
 
       - name: Setup
         shell: bash
         run: |
           sudo apt-get update
           python -m pip install --user --upgrade pip setuptools wheel setuptools_scm nox
 
@@ -35,10 +35,10 @@
         shell: bash
         run: |
           nox -s docs
 
       - name: Deploy
         uses: JamesIves/github-pages-deploy-action@v4
         with:
-          BRANCH: gh-pages
-          FOLDER: build/docs/
-          CLEAN: true
+          branch: gh-pages
+          folder: build/docs/
+          clean: true
```

### Comparing `torii-0.5.0/.github/workflows/pr.yaml` & `torii-0.6.0/.github/workflows/pr.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -4,36 +4,36 @@
 
 jobs:
   test-torii:
     name: Torii PR Tests (Python ${{ matrix.python-version }})
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: [ '3.9', '3.10', '3.11', '3.12-dev', 'pypy-3.9-v7.3.11']
+        python-version: [ '3.10', '3.11', '3.12', 'pypy3.10-v7.3.15']
       fail-fast: true
 
     steps:
       - name: Setup Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: Initialize Env
         shell: bash
         env:
           WORKSPACE: ${{ github.workspace }}
         run: |
           echo "$HOME/.local/bin:$PATH" >> $GITHUB_PATH
           echo "GITHUB_WORKSPACE=\"`pwd`\"" >> $GITHUB_ENV
 
       - name: Checkout
-        uses: actions/checkout@v3
+        uses: actions/checkout@v4
 
       - name: Setup OSS CAD Suite
-        uses: YosysHQ/setup-oss-cad-suite@v2
+        uses: YosysHQ/setup-oss-cad-suite@v3
         with:
           github-token: ${{ secrets.GITHUB_TOKEN }}
 
       - name: Setup
         shell: bash
         run: |
           python -m pip install --user --upgrade pip setuptools wheel setuptools_scm nox
@@ -47,8 +47,12 @@
       - name: Run Tests
         shell: bash
         run: |
           nox -s test
 
       - name: Codecov
         if: success() && github.repository == 'shrine-maiden-heavy-industries/torii-hdl'
-        uses: codecov/codecov-action@v3
+        uses: codecov/codecov-action@v4
+        with:
+          verbose: true
+          files: ./build/tests/coverage.xml
+          token: ${{ secrets.CODECOV_TOKEN }}
```

### Comparing `torii-0.5.0/.github/workflows/tests.yaml` & `torii-0.6.0/.github/workflows/tests.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -7,36 +7,36 @@
 
 jobs:
   test-torii:
     name: Torii Tests (Python ${{ matrix.python-version }})
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: [ '3.9', '3.10', '3.11', '3.12-dev', 'pypy-3.9-v7.3.11']
+        python-version: ['3.10', '3.11', '3.12', 'pypy3.10-v7.3.15']
       fail-fast: false
 
     steps:
       - name: Setup Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: Initialize Env
         shell: bash
         env:
           WORKSPACE: ${{ github.workspace }}
         run: |
           echo "$HOME/.local/bin:$PATH" >> $GITHUB_PATH
           echo "GITHUB_WORKSPACE=\"`pwd`\"" >> $GITHUB_ENV
 
       - name: Checkout
-        uses: actions/checkout@v3
+        uses: actions/checkout@v4
 
       - name: Setup OSS CAD Suite
-        uses: YosysHQ/setup-oss-cad-suite@v2
+        uses: YosysHQ/setup-oss-cad-suite@v3
         with:
           github-token: ${{ secrets.GITHUB_TOKEN }}
 
       - name: Setup
         shell: bash
         run: |
           python -m pip install --user --upgrade pip setuptools wheel setuptools_scm nox
@@ -44,11 +44,12 @@
 
       - name: Run Tests
         shell: bash
         run: |
           nox -s test -- --coverage
 
       - name: Codecov Upload
-        uses: codecov/codecov-action@v3
+        uses: codecov/codecov-action@v4
         with:
           verbose: true
           files: ./build/tests/coverage.xml
+          token: ${{ secrets.CODECOV_TOKEN }}
```

### Comparing `torii-0.5.0/CHANGELOG.md` & `torii-0.6.0/CHANGELOG.md`

 * *Files 15% similar despite different names*

```diff
@@ -15,14 +15,95 @@
 ### Removed
 ### Fixed
 ### Security
 -->
 
 ## [Unreleased]
 
+### Added
+
+
+### Changed
+
+
+### Deprecated
+
+
+### Removed
+
+
+### Fixed
+
+## [0.6.0]
+
+### Added
+
+ - Rough initial type annotations to `torii.hdl.mem`
+ - Added the ability to specify `tar` for the `torii.build.run.BuildPlan.archive` call.
+ - Added check inside `Record`s to ensure they're properly constructed prior to accessing their fields.
+ - Added the ability to override a Value's operators.
+ - Added the ability to put non-signals into `write_vcd`'s `traces` parameter.
+ - Added name disambiguation for traced signals where they share the same name.
+ - Added `ValueLike` and `ShapeLike`, mainly for additional typing and instance checking assistance.
+ - Added the ability for `Cat` and `Slice`, statements to be cast as a `Const` value.
+ - Added `#!/bin/sh` to the top of build shell scripts.
+ - Added `BuildPlan.extract` to extract files from the build plan without having to run it, this replaces the functionality that occurred when `BuildPlan.execute_local` was passed with `run_script = False`.
+ - Added `BuildPlan.execute_docker` to allow for invoking a build inside a specified docker container.
+ - Added `log2_ceil` and `log2_exact` to replace `log2_int` with the `False` and `True` params respectively.
+ - `ShapeCastable` objects can now be const initialized.
+
+### Changed
+
+ - Improved Oscillator frequency diagnostics for `torii.vendor.GowinPlatform`.
+ - Fixed `torii.lib.fifo` FIFOs to use the new memory semantics correctly.
+ - `torii.lib.soc.csr` Multiplexer shadow registers have been re-designed.
+ - Bumped minimum Python version from 3.9 to 3.10.
+ - Renamed `IntelPlatform` to `AlteraPlatform`.
+ - FWFT mode is default for all FIFOs now.
+ - Bumped the minimum version of Yosys to 0.30.
+ - Empty `Case` blocks now throw an exception when being used in place of a `Default` block
+ - Behavioral change warning in empty `Value.matches()` where currently it returns `Const(1)` but will return `Const(0)` in the future.
+ - We now only close a VCD or GTKW file in the simulator if it was opened by the simulator.
+ - Build shell scripts will now be marked as executable on unix-like hosts.
+ - `Instance` objects know collect source location information.
+ - Memories have been turned into a first-class IR representation.
+ - Out-of-range rests now error, not just warn.
+ - A warning is now generated when a `Case()` falls after a `Default()`, and an error is raised when there are multiple `Default()`'s in a `Switch`
+ - Shape casting a `range(1)` now resolves to an `unsigned(0)`
+
+### Deprecated
+
+ - Deprecated `torii.vendor.intel` and `torii.vendor.intel.IntelPlatform` in favor of `torii.vendor.altera` and `torii.vendor.altera.AlteraPlatform`.
+ - Deprecated `execute_local()`'s `run_script` param in favor of `extract`
+ - Deprecated use of `log2_int` in favor of `log2_ceil` and `log2_exact` where appropriate.
+
+### Removed
+
+ - Removed deprecated `torii.platform.vendor.lattice_*` modules.
+ - Removed deprecated `Repl` call in favor of `Value.replicate`.
+ - Removed `set -x` if the `verbose` param is set for platform builds.
+ - Removed the last little bit of `$verilog_initial_trigger` traces.
+ - Removed sub-classing of `AnyValue` and `Property`
+
+### Fixed
+
+ - Fixed `ToriiTestCase.settle` to handle "0" count settles.
+ - Fixed `torii.hdl.dsl.Module`'s constructor to properly use `super()` rather than a parent class name call.
+ - Load of typing annotation fixes.
+ - Cleaned up a load of blank `asserts`, they should now have more clear error diagnostics.
+ - Fixed a handful of typos throughout the library and documentation.
+ - Fixed tracer calls for Python 3.13
+ - Fixed `Array` not being indexable by a `ValueCastable`.
+ - Fixed `ValueCastable` not being accepted as a simulation coroutine command.
+ - Fixed handling of redundant `Case` branches.
+ - Fixed `Value.shift_right` and `Value.as_signed` edge cases.
+ - Fixed using 0-width `Switch`'s with integer keys.
+ - Trying to use the Python `in` operator on a `Value` now raises a sensible error.
+ - When indexing or slicing a Value with another Value, it now raises an error and suggests to use `Value.bit_select` or `Value.word_select` instead.
+ - Fixed simulation look when process catches an injected exception.
 
 ## [0.5.0]
 
 ### Added
 
  - Added some minor comments to the `torii.sim.core` module about the function of some of the objects.
  - Added `torii.vendor.gowin.GowinPlatform`.
@@ -43,14 +124,15 @@
  - Ensured `Part` offsets are always unsigned.
  - Disallowed `signed(0)` values.
 
 ### Deprecated
 
  - Old Lattice platform names have been deprecated in favor of the new platform location.
  - Deprecated `Repl` in favor of `Value.replicate`.
+
 ### Removed
 
  - Removed the `torii.cli` module
  - Removed the `remote-build` category from the `setup.py` `extra_requires` due to removal of remote builds.
 ### Fixed
 
  - Fixed an issue where the `IrDAResource` was not imported into the `torii.platform.resources` `__init__.py`
@@ -231,15 +313,16 @@
 - Fixed docstring formatting.
 
 ## [0.1.0] - [0.3.0]
 
 No changelog is provided for these versions as they are all older tagged releases of [Amaranth](https://github.com/amaranth-lang/amaranth) from before the fork.
 
 
-[unreleased]: https://github.com/shrine-maiden-heavy-industries/torii-hdl/compare/v0.5.0...main
+[unreleased]: https://github.com/shrine-maiden-heavy-industries/torii-hdl/compare/v0.6.0...main
+[0.6.0]: https://github.com/shrine-maiden-heavy-industries/torii-hdl/compare/v0.5.0...v0.6.0
 [0.5.0]: https://github.com/shrine-maiden-heavy-industries/torii-hdl/compare/v0.4.5...v0.5.0
 [0.4.5]: https://github.com/shrine-maiden-heavy-industries/torii-hdl/compare/v0.4.4...v0.4.5
 [0.4.4]: https://github.com/shrine-maiden-heavy-industries/torii-hdl/compare/v0.4.3...v0.4.4
 [0.4.3]: https://github.com/shrine-maiden-heavy-industries/torii-hdl/compare/v0.4.2...v0.4.3
 [0.4.2]: https://github.com/shrine-maiden-heavy-industries/torii-hdl/compare/v0.4.1...v0.4.2
 [0.4.1]: https://github.com/shrine-maiden-heavy-industries/torii-hdl/compare/v0.4.0...v0.4.1
 [0.4.0]: https://github.com/shrine-maiden-heavy-industries/torii-hdl/compare/amaranth-fork...v0.4.0
```

### Comparing `torii-0.5.0/CODE_OF_CONDUCT.md` & `torii-0.6.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `torii-0.5.0/CONTRIBUTING.md` & `torii-0.6.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `torii-0.5.0/LICENSE` & `torii-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `torii-0.5.0/PKG-INFO` & `torii-0.6.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torii
-Version: 0.5.0
+Version: 0.6.0
 Summary: Torii hardware definition language
 Home-page: https://torii.shmdn.link/
 Author: Aki Van Ness, Rachel Mant
 Author-email: aki@lethalbit.net, git@dragonmux.network
 License: BSD-2-Clause
 Project-URL: Documentation, https://torii.shmdn.link/
 Project-URL: Source Code, https://github.com/shrine-maiden-heavy-industries/torii-hdl
@@ -13,30 +13,30 @@
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Typing :: Typed
-Requires-Python: ~=3.9
+Requires-Python: ~=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: setuptools
 Requires-Dist: pyvcd>=0.2.2
 Requires-Dist: Jinja2~=3.0
-Requires-Dist: rich>=12.6.0
+Requires-Dist: rich
 Provides-Extra: dev
 Requires-Dist: nox; extra == "dev"
 
 # Torii-HDL
 
 Torii is a fork of [Amaranth HDL](https://github.com/amaranth-lang) that has been modified for use at [Shrine Maiden Heavy Industries](https://shrine-maiden-heavy.industries/). It has merged several of the components that were separate into a single package, and also adds new functionality, as well as some internal changes for better integration into tooling.
```

#### html2text {}

```diff
@@ -1,34 +1,34 @@
-Metadata-Version: 2.1 Name: torii Version: 0.5.0 Summary: Torii hardware
+Metadata-Version: 2.1 Name: torii Version: 0.6.0 Summary: Torii hardware
 definition language Home-page: https://torii.shmdn.link/ Author: Aki Van Ness,
 Rachel Mant Author-email: aki@lethalbit.net, git@dragonmux.network License:
 BSD-2-Clause Project-URL: Documentation, https://torii.shmdn.link/ Project-URL:
 Source Code, https://github.com/shrine-maiden-heavy-industries/torii-hdl
 Project-URL: Bug Tracker, https://github.com/shrine-maiden-heavy-industries/
 torii-hdl/issues Classifier: Development Status :: 4 - Beta Classifier:
 Intended Audience :: Developers Classifier: Intended Audience :: Information
 Technology Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: BSD License Classifier: Operating System :: MacOS ::
 MacOS X Classifier: Operating System :: Microsoft :: Windows Classifier:
 Operating System :: POSIX :: Linux Classifier: Programming Language :: Python
-:: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Classifier: Topic :: Scientific/
+:: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Programming Language :: Python :: 3.12 Classifier: Topic :: Scientific/
 Engineering Classifier: Topic :: Scientific/Engineering :: Electronic Design
 Automation (EDA) Classifier: Topic :: Software Development Classifier: Topic ::
 Software Development :: Embedded Systems Classifier: Topic :: Software
-Development :: Libraries Classifier: Typing :: Typed Requires-Python: ~=3.9
+Development :: Libraries Classifier: Typing :: Typed Requires-Python: ~=3.10
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 setuptools Requires-Dist: pyvcd>=0.2.2 Requires-Dist: Jinja2~=3.0 Requires-
-Dist: rich>=12.6.0 Provides-Extra: dev Requires-Dist: nox; extra == "dev" #
-Torii-HDL Torii is a fork of [Amaranth HDL](https://github.com/amaranth-lang)
-that has been modified for use at [Shrine Maiden Heavy Industries](https://
-shrine-maiden-heavy.industries/). It has merged several of the components that
-were separate into a single package, and also adds new functionality, as well
-as some internal changes for better integration into tooling. The evaluation
-board definitions have also been migrated and are located in the [torii-boards]
+Dist: rich Provides-Extra: dev Requires-Dist: nox; extra == "dev" # Torii-HDL
+Torii is a fork of [Amaranth HDL](https://github.com/amaranth-lang) that has
+been modified for use at [Shrine Maiden Heavy Industries](https://shrine-
+maiden-heavy.industries/). It has merged several of the components that were
+separate into a single package, and also adds new functionality, as well as
+some internal changes for better integration into tooling. The evaluation board
+definitions have also been migrated and are located in the [torii-boards]
 (https://github.com/shrine-maiden-heavy-industries/torii-boards) repository.
 There is also a list of [projects using Torii](https://torii.shmdn.link/
 projects.html) that are using Torii, and we'd love to add yours too! ##
 Introduction Please see the [Torii Introduction](https://shrine-maiden-heavy-
 industries.github.io/torii-hdl/intro.html) on the [online documentation](https:
 //shrine-maiden-heavy-industries.github.io/torii-hdl/) ## Installation Please
 see the [installation instructions](https://shrine-maiden-heavy-
```

### Comparing `torii-0.5.0/README.md` & `torii-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `torii-0.5.0/docs/_code/led_blinker.py` & `torii-0.6.0/docs/_code/led_blinker.py`

 * *Files identical despite different names*

### Comparing `torii-0.5.0/docs/_code/up_counter.py` & `torii-0.6.0/docs/_code/up_counter.py`

 * *Files identical despite different names*

### Comparing `torii-0.5.0/docs/_code/up_counter.v` & `torii-0.6.0/docs/_code/up_counter.v`

 * *Files identical despite different names*

### Comparing `torii-0.5.0/docs/_images/up_counter_gtkwave.png` & `torii-0.6.0/docs/_images/up_counter_gtkwave.png`

 * *Files identical despite different names*

### Comparing `torii-0.5.0/docs/_static/css/styles.css` & `torii-0.6.0/docs/_static/css/styles.css`

 * *Files identical despite different names*

### Comparing `torii-0.5.0/docs/_static/js/wavedrom.min.js` & `torii-0.6.0/docs/_static/js/wavedrom.min.js`

 * *Files identical despite different names*

### Comparing `torii-0.5.0/docs/_static/js/wavedrom.skin.js` & `torii-0.6.0/docs/_static/js/wavedrom.skin.js`

 * *Files identical despite different names*

### Comparing `torii-0.5.0/docs/_templates/versions.html` & `torii-0.6.0/docs/_templates/versions.html`

 * *Files identical despite different names*

### Comparing `torii-0.5.0/docs/conf.py` & `torii-0.6.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `torii-0.5.0/docs/getting_started.md` & `torii-0.6.0/docs/getting_started.md`

 * *Files identical despite different names*

### Comparing `torii-0.5.0/docs/index.md` & `torii-0.6.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `torii-0.5.0/docs/install.md` & `torii-0.6.0/docs/install.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ```{warning}
 The following instructions are a work-in-progress and may not be entirely up to date.
 ```
 
 
 ## System requirements
 
-Torii requires Python >= 3.9, and [Yosys](https://github.com/YosysHQ/yosys) >= 0.20. Torii has been tested with [CPython](https://www.python.org/), but might possibly run under [PyPy](https://www.pypy.org/).
+Torii requires Python >= 3.10, and [Yosys](https://github.com/YosysHQ/yosys) >= 0.30 except Yosys version 0.37 due to a Verilog backend bug. Torii has been tested with [CPython](https://www.python.org/), but might possibly run under [PyPy](https://www.pypy.org/).
 
 
 Simulating Torii code requires no additional software. However, a waveform viewer like [GTKWave](http://gtkwave.sourceforge.net/) is invaluable for debugging.
 
 Synthesizing, placing and routing an Torii design for an FPGA requires the FPGA family specific toolchain. See the [platform](./platforms/index.md) specific documentation for more information regarding vendor toolchains.
 
 
@@ -104,30 +104,30 @@
 
 		With other Linux distributions, it is recommended to use the `OSS Cad Suite <https://github.com/YosysHQ/oss-cad-suite-build>`_ nightly build. It provides a full environment of all the tools needed built on a nightly basis. This includes Yosys and GTKWave
 
 		Simply download the latest `release <https://github.com/YosysHQ/oss-cad-suite-build/releases>`_ for your architecture, extract it to a good home, and then add it to your ``$PATH``
 
 		.. code-block:: console
 
-		  $ curl -LOJ https://github.com/YosysHQ/oss-cad-suite-build/releases/download/2022-04-26/oss-cad-suite-linux-x64-20220426.tgz
-		  $ tar xfv oss-cad-suite-linux-x64-20220426.tgz
+		  $ curl -LOJ https://github.com/YosysHQ/oss-cad-suite-build/releases/download/2024-05-04/oss-cad-suite-linux-x64-20240504.tgz
+		  $ tar xfv oss-cad-suite-linux-x64-20240504.tgz
 		  $ export PATH="`pwd`/oss-cad-suite/bin:$PATH"
 
 
 	.. platform-choice:: macos
 		:title: macOS
 
 		For macOS systems, it is recommended to use the YoWASP distribution of the toolchain. However if you want to use the native tools, and you are using an Intel based Mac, then the `OSS Cad Suite <https://github.com/YosysHQ/oss-cad-suite-build>`_ has nightly builds for x86_64 versions of Darwin. This includes Yosys and GTKWave
 
 		Simply download the latest `release <https://github.com/YosysHQ/oss-cad-suite-build/releases>`_ for your architecture, extract it to a good home, and then add it to your ``$PATH``
 
 		.. code-block:: console
 
-		  $ curl -LOJ https://github.com/YosysHQ/oss-cad-suite-build/releases/download/2022-04-26/oss-cad-suite-darwin-x64-20220426.tgz
-		  $ tar xfv oss-cad-suite-darwin-x64-20220426.tgz
+		  $ curl -LOJ https://github.com/YosysHQ/oss-cad-suite-build/releases/download/2024-05-04/oss-cad-suite-darwin-x64-20240504.tgz
+		  $ tar xfv oss-cad-suite-darwin-x64-20240504.tgz
 		  $ export PATH="`pwd`/oss-cad-suite/bin:$PATH"
 
 	.. platform-choice:: windows
 		:title: Windows
 
 		.. warning:: These instructions may be incorrect or incomplete!
```

### Comparing `torii-0.5.0/docs/intro.md` & `torii-0.6.0/docs/intro.md`

 * *Files identical despite different names*

### Comparing `torii-0.5.0/docs/language/index.md` & `torii-0.6.0/docs/language/index.md`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,51 @@
 ```{eval-rst}
 .. testsetup::
 
    from torii import *
 
 ```
 
+## Shapes
+
+A `Shape` is an object with two attributes, `.width` and `.signed`. It can be constructed directly:
+
+```{eval-rst}
+.. doctest::
+
+   >>> Shape(width=5, signed=False)
+   unsigned(5)
+   >>> Shape(width=12, signed=True)
+   signed(12)
+```
+
+However, in most cases, the shape is always constructed with the same signedness, and the aliases `signed` and `unsigned` are more convenient:
+
+```{eval-rst}
+.. doctest::
+
+   >>> unsigned(5) == Shape(width=5, signed=False)
+   True
+   >>> signed(12) == Shape(width=12, signed=True)
+   True
+```
+
+## Shapes of values
+
+All values have a `.shape()` method that computes their shape. The width of a value `v`, `v.shape().width`, can also be retrieved with `len(v)`.
+
+```{eval-rst}
+.. doctest::
+
+   >>> Const(5).shape()
+   unsigned(3)
+   >>> len(Const(5))
+   3
+```
+
 ## Values
 
 The basic building block of the Torii language is a *value*, which is a term for a binary number that is computed or stored anywhere in the design. Each value has a *width*---the amount of bits used to represent the value---and a *signedness*---the interpretation of the value by arithmetic operations---collectively called its *shape*. Signed values always use [two's complement] representation.
 
 
 ## Constants
 
@@ -75,55 +112,14 @@
    >>> Const(129, signed(8)).value
    -127
    >>> Const(1, unsigned(0)).value
    0
 
 ```
 
-
-## Shapes
-
-A `Shape` is an object with two attributes, `.width` and `.signed`. It can be constructed directly:
-
-```{eval-rst}
-.. doctest::
-
-   >>> Shape(width = 5, signed = False)
-   unsigned(5)
-   >>> Shape(width = 12, signed = True)
-
-   signed(12)
-```
-
-However, in most cases, the shape is always constructed with the same signedness, and the aliases `signed` and `unsigned` are more convenient:
-
-```{eval-rst}
-.. doctest::
-
-   >>> unsigned(5) == Shape(width = 5, signed = False)
-   True
-   >>> signed(12) == Shape(width = 12, signed = True)
-   True
-
-```
-
-### Shapes of values
-
-All values have a `.shape()` method that computes their shape. The width of a value `v`, `v.shape().width`, can also be retrieved with `len(v)`.
-
-```{eval-rst}
-.. doctest::
-
-   >>> Const(5).shape()
-   unsigned(3)
-   >>> len(Const(5))
-   3
-```
-
-
 ## Shape casting
 
 Shapes can be *cast* from other objects, which are called *shape-castable*. Casting is a convenient way to specify a shape indirectly, for example, by a range of numbers representable by values with that shape.
 
 Casting to a shape can be done explicitly with `Shape.cast`, but is usually implicit, since shape-castable objects are accepted anywhere shapes are.
 
 
@@ -209,25 +205,25 @@
 
 ```{note}
 The enumeration does not have to subclass {class}`enum.IntEnum`; it only needs to have integers as values of every member. Using enumerations based on {class}`enum.Enum` rather than {class}`enum.IntEnum` prevents unwanted implicit conversion of enum members to integers.
 ```
 
 ## Value casting
 
-Like shapes, values may be *cast* from other objects, which are called *value-castable*. Casting allows objects that are not provided by Torii, such as integers or enumeration members, to be used in Torii expressions directly.
+Like shapes, values may be *cast* from other objects, which are called *value-castable*. Casting to values allows objects that are not provided by Torii, such as integers or enumeration members, to be used in Torii expressions directly.
 
 <!-- TODO: link to ValueCastable -->
 
 Casting to a value can be done explicitly with `Value.cast`, but is usually implicit, since value-castable objects are accepted anywhere values are.
 
 
 ### Values from integers
 
 
-Casting a value from an integer `i` is a shorthand for `Const(i)`:
+Casting a value from an integer `i` is equivalent to `Const(i)`:
 
 ```{eval-rst}
 .. doctest::
 
    >>> Value.cast(5)
    (const 3'd5)
 
@@ -235,28 +231,55 @@
 
 ```{note}
 If a value subclasses :class:`enum.IntEnum` or its class otherwise inherits from both :class:`int` and :class:`Enum`, it is treated as an enumeration.
 ```
 
 ### Values from enumeration members
 
-Casting a value from an enumeration member `m` is a shorthand for `Const(m.value, type(m))`:
+Casting a value from an enumeration member `m` is equivalent to `Const(m.value, type(m))`:
 
 ```{eval-rst}
 .. doctest::
 
    >>> Value.cast(Direction.LEFT)
    (const 2'd1)
 
 ```
 
 ```{note}
 If a value subclasses :class:`enum.IntEnum` or its class otherwise inherits from both :class:`int` and :class:`Enum`, it is treated as an enumeration.
 ```
 
+# Constant casting
+
+A subset of [values](#values) are *constant-castable*. If a value is constant-castable and all of its operands are also constant-castable, it can be converted to a `Const`, the numeric value of which can then be read by Python code. This provides a way to perform computation on Torii values while constructing the design.
+
+```{todo}
+link to m.Case and v.matches() below
+```
+
+Constant-castable objects are accepted anywhere a constant integer is accepted. Casting to a constant can also be done explicitly with `Const.cast`:
+
+```{eval-rst}
+.. doctest::
+
+   >>> Const.cast(Cat(Direction.TOP, Direction.LEFT))
+   (const 4'd4)
+
+```
+
+```{note}
+   At the moment, only the following expressions are constant-castable:
+
+   * :class:`Const`
+   * :class:`Cat`
+
+   This list will be expanded in the future.
+```
+
 ## Signals
 
 
 A *signal* is a value representing a (potentially) varying number. Signals can be [*assigned*](#assigning-to-signals) in a [combinatorial](#combinatorial-evaluation) or [synchronous](#synchronous-evaluation) domain, in which case they are generated as wires or registers, respectively. Signals always have a well-defined value; they cannot be uninitialized or undefined.
 
 ### Signal shapes
```

### Comparing `torii-0.5.0/docs/library/coding/index.md` & `torii-0.6.0/docs/library/coding/index.md`

 * *Files identical despite different names*

### Comparing `torii-0.5.0/docs/library/fifo.md` & `torii-0.6.0/docs/library/fifo.md`

 * *Files identical despite different names*

### Comparing `torii-0.5.0/docs/platforms/fpga/lattice-machxo-2-3l.md` & `torii-0.6.0/docs/platforms/fpga/lattice-machxo-2-3l.md`

 * *Files identical despite different names*

### Comparing `torii-0.5.0/docs/projects.md` & `torii-0.6.0/docs/projects.md`

 * *Files identical despite different names*

### Comparing `torii-0.5.0/docs/tutorials/external_modules.md` & `torii-0.6.0/docs/tutorials/external_modules.md`

 * *Files identical despite different names*

### Comparing `torii-0.5.0/docs/tutorials/index.md` & `torii-0.6.0/docs/tutorials/index.md`

 * *Files identical despite different names*

### Comparing `torii-0.5.0/examples/basic/alu.py` & `torii-0.6.0/examples/basic/alu.py`

 * *Files identical despite different names*

### Comparing `torii-0.5.0/examples/basic/alu_hier.py` & `torii-0.6.0/examples/basic/alu_hier.py`

 * *Files identical despite different names*

### Comparing `torii-0.5.0/examples/basic/arst.py` & `torii-0.6.0/examples/basic/arst.py`

 * *Files identical despite different names*

### Comparing `torii-0.5.0/examples/basic/ctr_en.py` & `torii-0.6.0/examples/basic/ctr_en.py`

 * *Files identical despite different names*

### Comparing `torii-0.5.0/examples/basic/fsm.py` & `torii-0.6.0/examples/basic/fsm.py`

 * *Files identical despite different names*

### Comparing `torii-0.5.0/examples/basic/gpio.py` & `torii-0.6.0/examples/basic/gpio.py`

 * *Files identical despite different names*

### Comparing `torii-0.5.0/examples/basic/inst.py` & `torii-0.6.0/examples/basic/inst.py`

 * *Files identical despite different names*

### Comparing `torii-0.5.0/examples/basic/mem.py` & `torii-0.6.0/examples/basic/mem.py`

 * *Files identical despite different names*

### Comparing `torii-0.5.0/examples/basic/pmux.py` & `torii-0.6.0/examples/basic/pmux.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 		with m.Switch(self.s):
 			with m.Case('--1'):
 				m.d.comb += self.o.eq(self.a)
 			with m.Case('-1-'):
 				m.d.comb += self.o.eq(self.b)
 			with m.Case('1--'):
 				m.d.comb += self.o.eq(self.c)
-			with m.Case():
+			with m.Default():
 				m.d.comb += self.o.eq(0)
 		return m
 
 
 if __name__ == '__main__':
 	pmux = ParMux(width = 16)
```

### Comparing `torii-0.5.0/examples/basic/sel.py` & `torii-0.6.0/examples/basic/sel.py`

 * *Files identical despite different names*

### Comparing `torii-0.5.0/examples/basic/uart.py` & `torii-0.6.0/examples/basic/uart.py`

 * *Files identical despite different names*

### Comparing `torii-0.5.0/examples/board/01_blinky.py` & `torii-0.6.0/examples/board/01_blinky.py`

 * *Files identical despite different names*

### Comparing `torii-0.5.0/examples/board/02_domain.py` & `torii-0.6.0/examples/board/02_domain.py`

 * *Files identical despite different names*

### Comparing `torii-0.5.0/noxfile.py` & `torii-0.6.0/noxfile.py`

 * *Files identical despite different names*

### Comparing `torii-0.5.0/setup.py` & `torii-0.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 	]),
 	author_email     = ', '.join([
 		'aki@lethalbit.net',
 		'git@dragonmux.network',
 	]),
 	description      = 'Torii hardware definition language',
 	license          = 'BSD-2-Clause',
-	python_requires  = '~=3.9',
+	python_requires  = '~=3.10',
 	zip_safe         = True,
 	url              = 'https://torii.shmdn.link/',
 
 	long_description = README_FILE.read_text(),
 	long_description_content_type = 'text/markdown',
 
 	setup_requires   = [
@@ -61,15 +61,15 @@
 		'setuptools_scm'
 	],
 
 	install_requires = [
 		'setuptools',
 		'pyvcd>=0.2.2',
 		'Jinja2~=3.0',
-		'rich>=12.6.0',
+		'rich',
 	],
 
 	extras_require   = {
 		'dev': [
 			'nox'
 		],
 	},
@@ -98,17 +98,17 @@
 
 		'License :: OSI Approved :: BSD License',
 
 		'Operating System :: MacOS :: MacOS X',
 		'Operating System :: Microsoft :: Windows',
 		'Operating System :: POSIX :: Linux',
 
-		'Programming Language :: Python :: 3.9',
 		'Programming Language :: Python :: 3.10',
 		'Programming Language :: Python :: 3.11',
+		'Programming Language :: Python :: 3.12',
 
 		'Topic :: Scientific/Engineering',
 		'Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)',
 		'Topic :: Software Development',
 		'Topic :: Software Development :: Embedded Systems',
 		'Topic :: Software Development :: Libraries',
```

### Comparing `torii-0.5.0/tests/build/test_dsl.py` & `torii-0.6.0/tests/build/test_dsl.py`

 * *Files identical despite different names*

### Comparing `torii-0.5.0/tests/build/test_plat.py` & `torii-0.6.0/tests/build/test_plat.py`

 * *Files identical despite different names*

### Comparing `torii-0.5.0/tests/build/test_res.py` & `torii-0.6.0/tests/build/test_res.py`

 * *Files identical despite different names*

### Comparing `torii-0.5.0/tests/hdl/test_ast.py` & `torii-0.6.0/tests/hdl/test_ast.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # SPDX-License-Identifier: BSD-2-Clause
 
 import warnings
-from enum          import Enum
+from enum          import Enum, EnumMeta
 
 from torii.hdl.ast import *
 
 from ..utils       import ToriiTestSuiteCase
 
 
 class UnsignedEnum(Enum):
@@ -134,28 +134,31 @@
 		s2 = Shape.cast(range(0, 9))
 		self.assertEqual(s2.width, 4)
 		self.assertEqual(s2.signed, False)
 		s3 = Shape.cast(range(-7, 8))
 		self.assertEqual(s3.width, 4)
 		self.assertEqual(s3.signed, True)
 		s4 = Shape.cast(range(0, 1))
-		self.assertEqual(s4.width, 1)
+		self.assertEqual(s4.width, 0)
 		self.assertEqual(s4.signed, False)
 		s5 = Shape.cast(range(-1, 0))
 		self.assertEqual(s5.width, 1)
 		self.assertEqual(s5.signed, True)
 		s6 = Shape.cast(range(0, 0))
 		self.assertEqual(s6.width, 0)
 		self.assertEqual(s6.signed, False)
 		s7 = Shape.cast(range(-1, -1))
 		self.assertEqual(s7.width, 0)
 		self.assertEqual(s7.signed, False)
 		s8 = Shape.cast(range(0, 10, 3))
 		self.assertEqual(s8.width, 4)
 		self.assertEqual(s8.signed, False)
+		s9 = Shape.cast(range(0, 3, 3))
+		self.assertEqual(s9.width, 0)
+		self.assertEqual(s9.signed, False)
 
 	def test_cast_enum(self):
 		s1 = Shape.cast(UnsignedEnum)
 		self.assertEqual(s1.width, 2)
 		self.assertEqual(s1.signed, False)
 		s2 = Shape.cast(SignedEnum)
 		self.assertEqual(s2.width, 2)
@@ -179,14 +182,17 @@
 class MockShapeCastable(ShapeCastable):
 	def __init__(self, dest):
 		self.dest = dest
 
 	def as_shape(self):
 		return self.dest
 
+	def const(self, obj):
+		return Const(obj, self.dest)
+
 
 class ShapeCastableTestCase(ToriiTestSuiteCase):
 	def test_no_override(self):
 		with self.assertRaisesRegex(
 			TypeError,
 			r'^Class \'MockShapeCastableNoOverride\' deriving from `ShapeCastable` must '
 			r'override the `as_shape` method$'
@@ -209,14 +215,55 @@
 			Shape.cast(sc)
 
 	def test_recurse(self):
 		sc = MockShapeCastable(MockShapeCastable(unsigned(1)))
 		self.assertEqual(Shape.cast(sc), unsigned(1))
 
 
+class ShapeLikeTestCase(ToriiTestSuiteCase):
+	def test_construct(self):
+		with self.assertRaises(TypeError):
+			ShapeLike()
+
+	def test_subclass(self):
+		self.assertTrue(issubclass(Shape, ShapeLike))
+		self.assertTrue(issubclass(MockShapeCastable, ShapeLike))
+		self.assertTrue(issubclass(int, ShapeLike))
+		self.assertTrue(issubclass(range, ShapeLike))
+		self.assertTrue(issubclass(EnumMeta, ShapeLike))
+		self.assertFalse(issubclass(Enum, ShapeLike))
+		self.assertFalse(issubclass(str, ShapeLike))
+		self.assertTrue(issubclass(ShapeLike, ShapeLike))
+
+	def test_isinstance(self):
+		self.assertTrue(isinstance(unsigned(2), ShapeLike))
+		self.assertTrue(isinstance(MockShapeCastable(unsigned(2)), ShapeLike))
+		self.assertTrue(isinstance(2, ShapeLike))
+		self.assertTrue(isinstance(0, ShapeLike))
+		self.assertFalse(isinstance(-1, ShapeLike))
+		self.assertTrue(isinstance(range(10), ShapeLike))
+		self.assertFalse(isinstance('abc', ShapeLike))
+
+	def test_isinstance_enum(self):
+		class EnumA(Enum):
+			A = 1
+			B = 2
+
+		class EnumB(Enum):
+			A = 'a'
+			B = 'b'
+
+		class EnumC(Enum):
+			A = Cat(Const(1, 2), Const(0, 2))
+
+		self.assertTrue(isinstance(EnumA, ShapeLike))
+		self.assertFalse(isinstance(EnumB, ShapeLike))
+		self.assertTrue(isinstance(EnumC, ShapeLike))
+
+
 class ValueTestCase(ToriiTestSuiteCase):
 	def test_cast(self):
 		self.assertIsInstance(Value.cast(0), Const)
 		self.assertIsInstance(Value.cast(True), Const)
 		c = Const(0)
 		self.assertIs(Value.cast(c), c)
 		with self.assertRaisesRegex(
@@ -295,14 +342,28 @@
 	def test_getitem_wrong(self):
 		with self.assertRaisesRegex(
 			TypeError,
 			r'^Cannot index value with \'str\'$'
 		):
 			Const(31)['str']
 
+		with self.assertRaises(
+			SyntaxError,
+			msg = 'Slicing a value with a Value is unsupported, '
+				'use `Value.bit_select()` or `Value.word_select()` instead.'
+		):
+			Const(31)[Signal(3)]
+
+		s = Signal(3)
+		with self.assertRaises(
+			SyntaxError,
+			msg = 'Indexing a value with another value is not supported, use `Value.bit_select()` instead.'
+		):
+			Const(31)[s:s+3]
+
 	def test_shift_left(self):
 		self.assertRepr(
 			Const(256, unsigned(9)).shift_left(0),
 			'(cat (const 0\'d0) (const 9\'d256))'
 		)
 
 		self.assertRepr(
@@ -336,15 +397,15 @@
 		)
 		self.assertRepr(
 			Const(256, signed(9)).shift_left(-5),
 			'(s (slice (const 9\'sd-256) 5:9))'
 		)
 		self.assertRepr(
 			Const(256, signed(9)).shift_left(-15),
-			'(s (slice (const 9\'sd-256) 9:9))'
+			'(s (slice (const 9\'sd-256) 8:9))'
 		)
 
 	def test_shift_left_wrong(self):
 		with self.assertRaisesRegex(
 			TypeError,
 			r'^Shift amount must be an integer, not \'str\'$'
 		):
@@ -378,24 +439,40 @@
 			'(slice (const 9\'d256) 1:9)'
 		)
 		self.assertRepr(
 			Const(256, unsigned(9)).shift_right(5),
 			'(slice (const 9\'d256) 5:9)'
 		)
 		self.assertRepr(
+			Const(256, unsigned(9)).shift_right(15),
+			'(slice (const 9\'d256) 9:9)'
+		)
+		self.assertRepr(
 			Const(256, signed(9)).shift_right(1),
 			'(s (slice (const 9\'sd-256) 1:9))'
 		)
 		self.assertRepr(
 			Const(256, signed(9)).shift_right(5),
 			'(s (slice (const 9\'sd-256) 5:9))'
 		)
 		self.assertRepr(
+			Const(256, signed(9)).shift_right(7),
+			'(s (slice (const 9\'sd-256) 7:9))'
+		)
+		self.assertRepr(
+			Const(256, signed(9)).shift_right(8),
+			'(s (slice (const 9\'sd-256) 8:9))'
+		)
+		self.assertRepr(
+			Const(256, signed(9)).shift_right(9),
+			'(s (slice (const 9\'sd-256) 8:9))'
+		)
+		self.assertRepr(
 			Const(256, signed(9)).shift_right(15),
-			'(s (slice (const 9\'sd-256) 9:9))'
+			'(s (slice (const 9\'sd-256) 8:9))'
 		)
 
 	def test_shift_right_wrong(self):
 		with self.assertRaisesRegex(
 			TypeError,
 			r'^Shift amount must be an integer, not \'str\'$'
 		):
@@ -527,14 +604,32 @@
 		self.assertEqual(repr(Const(10)),  '(const 4\'d10)')
 		self.assertEqual(repr(Const(-10)), '(const 5\'sd-10)')
 
 	def test_hash(self):
 		with self.assertRaises(TypeError):
 			hash(Const(0))
 
+	def test_shape_castable(self):
+		class MockConstValue:
+			def __init__(self, value):
+				self.value = value
+
+		class MockConstShape(ShapeCastable):
+			def as_shape(self):
+				return unsigned(8)
+
+			def __call__(self, value):
+				return value
+
+			def const(self, init):
+				return MockConstValue(init)
+
+		s = Const(10, MockConstShape())
+		self.assertIsInstance(s, MockConstValue)
+		self.assertEqual(s.value, 10)
 
 class OperatorTestCase(ToriiTestSuiteCase):
 	def test_bool(self):
 		v = Const(0, 4).bool()
 		self.assertEqual(repr(v), '(b (const 4\'d0))')
 		self.assertEqual(v.shape(), unsigned(1))
 
@@ -549,14 +644,20 @@
 		self.assertEqual(v.shape(), unsigned(4))
 
 	def test_as_signed(self):
 		v = Const(1, unsigned(4)).as_signed()
 		self.assertEqual(repr(v), '(s (const 4\'d1))')
 		self.assertEqual(v.shape(), signed(4))
 
+	def test_as_signed_wrong(self):
+		with self.assertRaisesRegex(
+			ValueError, r'^Cannot create a 0-width signed value$'
+		):
+			Const(0, 0).as_signed()
+
 	def test_pos(self):
 		self.assertRepr(+Const(10), '(const 4\'d10)')
 
 	def test_neg(self):
 		v1 = -Const(0, unsigned(4))
 		self.assertEqual(repr(v1), '(- (const 4\'d0))')
 		self.assertEqual(v1.shape(), signed(5))
@@ -747,15 +848,19 @@
 
 	def test_xor_value(self):
 		v = Const(0b101).xor()
 		self.assertEqual(repr(v), '(r^ (const 3\'d5))')
 
 	def test_matches(self):
 		s = Signal(4)
-		self.assertRepr(s.matches(), '(const 1\'d1)')
+		with self.assertWarns(
+			SyntaxWarning,
+			msg = 'Value.matches() with an empty patterns clause will return `Const(0)` in a future release.'
+		):
+			self.assertRepr(s.matches(), '(const 1\'d1)')
 		self.assertRepr(s.matches(1), '''
 		(== (sig s) (const 1'd1))
 		''')
 		self.assertRepr(s.matches(0, 1), '''
 		(r| (cat (== (sig s) (const 1'd0)) (== (sig s) (const 1'd1))))
 		''')
 		self.assertRepr(s.matches('10--'), '''
@@ -764,47 +869,60 @@
 		self.assertRepr(s.matches('1 0--'), '''
 		(== (& (sig s) (const 4'd12)) (const 4'd8))
 		''')
 
 	def test_matches_enum(self):
 		s = Signal(SignedEnum)
 		self.assertRepr(s.matches(SignedEnum.FOO), '''
-		(== (sig s) (const 1'sd-1))
+		(== (sig s) (const 2'sd-1))
+		''')
+
+	def test_matches_const_castable(self):
+		s = Signal(4)
+		self.assertRepr(s.matches(Cat(Const(0b10, 2), Const(0b11, 2))), '''
+		(== (sig s) (const 4'd14))
 		''')
 
 	def test_matches_width_wrong(self):
 		s = Signal(4)
 		with self.assertRaisesRegex(
 			SyntaxError,
 			r'^Match pattern \'--\' must have the same width as match value \(which is 4\)$'
 		):
 			s.matches('--')
 		with self.assertWarnsRegex(
 			SyntaxWarning, (
-				r'^Match pattern \'10110\' is wider than match value \(which has width 4\); '
+				r'^Match pattern \'22\' \(5\'10110\) is wider than match value \(which has width 4\); '
 				r'comparison will never be true$'
 			)
 		):
 			s.matches(0b10110)
 
+		with self.assertWarns(
+			SyntaxWarning,
+			msg = 'Match pattern \'(cat (const 1\'d0) (const 4\'d11))\' (5\'10110) is wider '
+				'than match value (which has width 4); comparison will never be true'
+		):
+			s.matches(Cat(0, Const(0b1011, 4)))
+
 	def test_matches_bits_wrong(self):
 		s = Signal(4)
 		with self.assertRaisesRegex(
 			SyntaxError, (
 				r'^Match pattern \'abc\' must consist of 0, 1, and - \(don\'t care\) bits, '
 				r'and may include whitespace$'
 			)
 		):
 			s.matches('abc')
 
 	def test_matches_pattern_wrong(self):
 		s = Signal(4)
 		with self.assertRaisesRegex(
 			SyntaxError,
-			r'^Match pattern must be an integer, a string, or an enumeration, not 1\.0$'
+			r'^Match pattern must be a string or a const-castable expression, not 1\.0$'
 		):
 			s.matches(1.0)
 
 	def test_hash(self):
 		with self.assertRaises(TypeError):
 			hash(Const(0) + Const(0))
 
@@ -814,14 +932,18 @@
 		s = Signal(signed(4))
 		self.assertRepr(
 			abs(s),
 			'(slice (m (>= (sig s) (const 1\'d0)) (sig s) (- (sig s))) 0:4)'
 		)
 		self.assertEqual(abs(s).shape(), unsigned(4))
 
+	def test_contains(self):
+		with self.assertRaises(TypeError, msg = 'The python `in` operator is not supported on Torii values'):
+			1 in Signal(3)
+
 
 class SliceTestCase(ToriiTestSuiteCase):
 	def test_shape(self):
 		s1 = Const(10)[2]
 		self.assertEqual(s1.shape(), unsigned(1))
 		self.assertIsInstance(s1.shape(), Shape)
 		s2 = Const(-10)[0:2]
@@ -880,14 +1002,23 @@
 		):
 			Slice(c, 5, 9)
 
 	def test_repr(self):
 		s1 = Const(10)[2]
 		self.assertEqual(repr(s1), '(slice (const 4\'d10) 2:3)')
 
+	def test_const(self):
+		a = Const.cast(Const(0x1234, 16)[4:12])
+		self.assertEqual(a.value, 0x23)
+		self.assertEqual(a.width, 8)
+		self.assertEqual(a.signed, False)
+		a = Const.cast(Const(-4, signed(8))[1:6])
+		self.assertEqual(a.value, 0x1e)
+		self.assertEqual(a.width, 5)
+		self.assertEqual(a.signed, False)
 
 class BitSelectTestCase(ToriiTestSuiteCase):
 	def setUp(self):
 		self.c = Const(0, 8)
 		self.s = Signal(range(self.c.width))
 
 	def test_shape(self):
@@ -1021,34 +1152,23 @@
 		with self.assertWarnsRegex(
 			SyntaxWarning,
 			r'^Argument #1 of \'Cat\(\)\' is a bare integer 2 used in bit vector context; '
 			r'consider specifying the width explicitly using \'Const\(2, 2\)\' instead$'
 		):
 			Cat(2)
 
-
-class ReplTestCase(ToriiTestSuiteCase):
-	def test_cast(self):
-		r = Repl(0, 3)
-		self.assertEqual(repr(r), '(cat (const 1\'d0) (const 1\'d0) (const 1\'d0))')
-
-	def test_int_01(self):
-		with warnings.catch_warnings():
-			warnings.filterwarnings(action = 'error', category = SyntaxWarning)
-			Repl(0, 3)
-			Repl(1, 3)
-
-	def test_int_wrong(self):
-		with self.assertWarnsRegex(
-			SyntaxWarning,
-			r'^Value argument of Repl\(\) is a bare integer 2 used in bit vector context; '
-			r'consider specifying explicit width using Const\(2, 2\) instead$'
-		):
-			Repl(2, 3)
-
+	def test_const(self):
+		a = Const.cast(Cat(Const(1, 1), Const(0, 1), Const(3, 2), Const(2, 2)))
+		self.assertEqual(a.value, 0x2d)
+		self.assertEqual(a.width, 6)
+		self.assertEqual(a.signed, False)
+		a = Const.cast(Cat(Const(-4, 8), Const(-3, 8)))
+		self.assertEqual(a.value, 0xfdfc)
+		self.assertEqual(a.width, 16)
+		self.assertEqual(a.signed, False)
 
 class ArrayTestCase(ToriiTestSuiteCase):
 	def test_acts_like_array(self):
 		a = Array([1, 2, 3])
 		self.assertSequenceEqual(a, [1, 2, 3])
 		self.assertEqual(a[1], 2)
 		a[1] = 4
@@ -1076,14 +1196,26 @@
 			del a[1]
 		with self.assertRaisesRegex(
 			ValueError,
 			r'^Array can no longer be mutated after it was indexed with a value at '
 		):
 			a.insert(1, 2)
 
+	def test_index_value_castable(self):
+		class MyValue(ValueCastable):
+			@ValueCastable.lowermethod
+			def as_value(self):
+				return Signal()
+
+			def shape():
+				return unsigned(1)
+
+		a = Array([1,2,3])
+		a[MyValue()]
+
 	def test_repr(self):
 		a = Array([1, 2, 3])
 		self.assertEqual(repr(a), '(array mutable [1, 2, 3])')
 		s = Signal(range(len(a)))
 		a[s]
 		self.assertEqual(repr(a), '(array [1, 2, 3])')
 
@@ -1151,20 +1283,18 @@
 		self.assertEqual(s6.shape(), unsigned(4))
 		s7 = Signal(range(4, 16))
 		self.assertEqual(s7.shape(), unsigned(4))
 		s8 = Signal(range(-4, 16))
 		self.assertEqual(s8.shape(), signed(5))
 		s9 = Signal(range(-20, 16))
 		self.assertEqual(s9.shape(), signed(6))
-		with warnings.catch_warnings():
-			warnings.filterwarnings(action = 'ignore', category = SyntaxWarning)
-			s10 = Signal(range(0))
-			self.assertEqual(s10.shape(), unsigned(0))
+		s10 = Signal(range(0))
+		self.assertEqual(s10.shape(), unsigned(0))
 		s11 = Signal(range(1))
-		self.assertEqual(s11.shape(), unsigned(1))
+		self.assertEqual(s11.shape(), unsigned(0))
 
 	def test_shape_wrong(self):
 		with self.assertRaisesRegex(
 			ValueError,
 			r'^Width of an unsigned value must be zero or a positive integer, not -10$'
 		):
 			Signal(-10)
@@ -1186,14 +1316,32 @@
 		with self.assertRaisesRegex(
 			TypeError,
 			r'^Reset value must be a constant-castable expression, '
 			r'not <StringEnum\.FOO: \'a\'>$'
 		):
 			Signal(1, reset = StringEnum.FOO)
 
+	def test_reset_shape_castable_const(self):
+		class CastableFromHex(ShapeCastable):
+			def as_shape(self):
+				return unsigned(8)
+
+			def const(self, init):
+				return int(init, 16)
+
+		s1 = Signal(CastableFromHex(), reset = 'aa')
+		self.assertEqual(s1.reset, 0xaa)
+
+		with self.assertRaisesRegex(
+			ValueError,
+			r'^Constant returned by <.+?CastableFromHex.+?>\.const\(\) must have the shape '
+			r'that it casts to, unsigned\(8\), and not unsigned\(1\)$'
+		):
+			Signal(CastableFromHex(), reset="01")
+
 	def test_reset_signed_mismatch(self):
 		with self.assertWarnsRegex(
 			SyntaxWarning,
 			r'^Reset value -2 is signed, but the signal shape is unsigned\(2\)$'
 		):
 			Signal(unsigned(2), reset = -2)
 
@@ -1211,21 +1359,40 @@
 		with self.assertWarnsRegex(
 			SyntaxWarning,
 			r'^Reset value -2 will be truncated to the signal shape signed\(1\)$'
 		):
 			Signal(signed(1), reset = -2)
 
 	def test_reset_wrong_fencepost(self):
-		with self.assertWarnsRegex(
-			SyntaxWarning,
+		with self.assertRaisesRegex(
+			SyntaxError,
 			r'^Reset value 10 equals the non-inclusive end of the signal shape '
 			r'range\(0, 10\); this is likely an off-by-one error$'
 		):
-			Signal(range(0, 10), reset=10)
+			Signal(range(0, 10), reset = 10)
+
+		with self.assertRaisesRegex(
+			SyntaxError,
+			r'^Reset value 0 equals the non-inclusive end of the signal shape '
+			r'range\(0, 0\); this is likely an off-by-one error$'
+		):
+			Signal(range(0), reset = 0)
 
+	def test_reset_wrong_range(self):
+		with self.assertRaisesRegex(
+			SyntaxError,
+			r'^Reset value 11 is not within the signal shape range\(0, 10\)$'
+		):
+			Signal(range(0, 10), reset = 11)
+
+		with self.assertRaisesRegex(
+			SyntaxError,
+			r'^Reset value 0 is not within the signal shape range\(1, 10\)$'
+		):
+			Signal(range(1, 10), reset = 0)
 
 	def test_attrs(self):
 		s1 = Signal()
 		self.assertEqual(s1.attrs, {})
 		s2 = Signal(attrs = {'no_retiming': True})
 		self.assertEqual(s2.attrs, {'no_retiming': True})
 
@@ -1263,14 +1430,18 @@
 	def test_enum(self):
 		s1 = Signal(UnsignedEnum)
 		self.assertEqual(s1.shape(), unsigned(2))
 		s2 = Signal(SignedEnum)
 		self.assertEqual(s2.shape(), signed(2))
 		self.assertEqual(s2.decoder(SignedEnum.FOO), 'FOO/-1')
 
+	def test_const_wrong(self):
+		s1 = Signal()
+		with self.assertRaises(TypeError, msg = 'Value (sig s1) cannot be converted to a Torii constant'):
+			Const.cast(s1)
 
 class ClockSignalTestCase(ToriiTestSuiteCase):
 	def test_domain(self):
 		s1 = ClockSignal()
 		self.assertEqual(s1.domain, 'sync')
 		s2 = ClockSignal('pix')
 		self.assertEqual(s2.domain, 'pix')
@@ -1429,14 +1600,61 @@
 			Value.cast(vc)
 
 	def test_recurse(self):
 		vc = MockValueCastable(MockValueCastable(Signal()))
 		self.assertIsInstance(Value.cast(vc), Signal)
 
 
+class ValueLikeTestCase(ToriiTestSuiteCase):
+	def test_construct(self):
+		with self.assertRaises(TypeError):
+			ValueLike()
+
+	def test_subclass(self):
+		self.assertTrue(issubclass(Value, ValueLike))
+		self.assertTrue(issubclass(MockValueCastable, ValueLike))
+		self.assertTrue(issubclass(int, ValueLike))
+		self.assertFalse(issubclass(range, ValueLike))
+		self.assertFalse(issubclass(EnumMeta, ValueLike))
+		self.assertTrue(issubclass(Enum, ValueLike))
+		self.assertFalse(issubclass(str, ValueLike))
+		self.assertTrue(issubclass(ValueLike, ValueLike))
+
+	def test_isinstance(self):
+		self.assertTrue(isinstance(Const(0, 2), ValueLike))
+		self.assertTrue(isinstance(MockValueCastable(Const(0, 2)), ValueLike))
+		self.assertTrue(isinstance(2, ValueLike))
+		self.assertTrue(isinstance(-2, ValueLike))
+		self.assertFalse(isinstance(range(10), ValueLike))
+
+	def test_enum(self):
+		class EnumA(Enum):
+			A = 1
+			B = 2
+
+		class EnumB(Enum):
+			A = 'a'
+			B = 'b'
+
+		class EnumC(Enum):
+			A = Cat(Const(1, 2), Const(0, 2))
+
+		class EnumD(Enum):
+			A = 1
+			B = 'a'
+
+		self.assertTrue(issubclass(EnumA, ValueLike))
+		self.assertFalse(issubclass(EnumB, ValueLike))
+		self.assertTrue(issubclass(EnumC, ValueLike))
+		self.assertFalse(issubclass(EnumD, ValueLike))
+		self.assertTrue(isinstance(EnumA.A, ValueLike))
+		self.assertFalse(isinstance(EnumB.A, ValueLike))
+		self.assertTrue(isinstance(EnumC.A, ValueLike))
+		self.assertFalse(isinstance(EnumD.A, ValueLike))
+
 class SampleTestCase(ToriiTestSuiteCase):
 	def test_const(self):
 		s = Sample(1, 1, 'sync')
 		self.assertEqual(s.shape(), unsigned(1))
 
 	def test_signal(self):
 		s1 = Sample(Signal(2), 1, 'sync')
@@ -1484,14 +1702,25 @@
 		s = Switch(Const(0, 8), {10: []})
 		self.assertEqual(s.cases, {('00001010',): []})
 
 	def test_int_neg_case(self):
 		s = Switch(Const(0, 8), {-10: []})
 		self.assertEqual(s.cases, {('11110110',): []})
 
+	def test_int_zero_width(self):
+		s = Switch(Const(0, 0), {0: []})
+		self.assertEqual(s.cases, {('',): []})
+
+	def test_int_zero_width_enum(self):
+		class ZeroEnum(Enum):
+			A = 0
+
+		s = Switch(Const(0, 0), {ZeroEnum.A: []})
+		self.assertEqual(s.cases, {('',): []})
+
 	def test_enum_case(self):
 		s = Switch(Const(0, UnsignedEnum), {UnsignedEnum.FOO: []})
 		self.assertEqual(s.cases, {('01',): []})
 
 	def test_str_case(self):
 		s = Switch(Const(0, 8), {'0000 11\t01': []})
 		self.assertEqual(s.cases, {('00001101',): []})
```

### Comparing `torii-0.5.0/tests/hdl/test_cd.py` & `torii-0.6.0/tests/hdl/test_cd.py`

 * *Files identical despite different names*

### Comparing `torii-0.5.0/tests/hdl/test_dsl.py` & `torii-0.6.0/tests/hdl/test_dsl.py`

 * *Files 2% similar despite different names*

```diff
@@ -406,19 +406,25 @@
 				(case 10-- (eq (sig c2) (const 1'd1)))
 			)
 		)
 		''')
 
 	def test_Switch_default_Case(self):
 		m = Module()
-		with m.Switch(self.w1):
-			with m.Case(3):
-				m.d.comb += self.c1.eq(1)
-			with m.Case():
-				m.d.comb += self.c2.eq(1)
+		with self.assertRaises(
+			ValueError,
+			msg = 'Empty Case() clauses have been superseded by Default()'
+		):
+			with m.Switch(self.w1):
+				with m.Case(3):
+					m.d.comb += self.c1.eq(1)
+				with m.Default():
+					m.d.comb += self.c2.eq(1)
+				with m.Case():
+					m.d.comb += self.c2.eq(1)
 		m._flush()
 		self.assertRepr(m._statements, '''
 		(
 			(switch (sig w1)
 				(case 0011 (eq (sig c1) (const 1'd1)))
 				(default (eq (sig c2) (const 1'd1)))
 			)
@@ -457,59 +463,92 @@
 		''')
 
 	def test_Switch_enum(self):
 		class Color(Enum):
 			RED  = 1
 			BLUE = 2
 		m = Module()
-		se = Signal(Color)
+		se = Signal(Color, reset = Color.RED)
 		with m.Switch(se):
 			with m.Case(Color.RED):
 				m.d.comb += self.c1.eq(1)
 		self.assertRepr(m._statements, '''
 		(
 			(switch (sig se)
 				(case 01 (eq (sig c1) (const 1'd1)))
 			)
 		)
 		''')
 
+	def test_Switch_const_castable(self):
+		class Color(Enum):
+			RED  = 0
+			BLUE = 1
+
+		m = Module()
+		se = Signal(2)
+		with m.Switch(se):
+			with m.Case(Cat(Color.RED, Color.BLUE)):
+				m.d.comb += self.c1.eq(1)
+		self.assertRepr(m._statements, '''
+		(
+			(switch (sig se)
+				(case 10 (eq (sig c1) (const 1'd1)))
+			)
+		)
+		''')
+
 	def test_Case_width_wrong(self):
 		class Color(Enum):
 			RED = 0b10101010
 		m = Module()
 		with m.Switch(self.w1):
 			with self.assertRaisesRegex(
 				SyntaxError,
 				r'^Case pattern \'--\' must have the same width as switch value \(which is 4\)$'
 			):
 				with m.Case('--'):
 					pass
 			with self.assertWarnsRegex(
 				SyntaxWarning, (
-					r'^Case pattern \'10110\' is wider than switch value \(which has width 4\); '
+					r'^Case pattern \'22\' \(5\'10110\) is wider than switch value \(which has width 4\); '
 					r'comparison will never be true$'
 				)
 			):
 				with m.Case(0b10110):
 					pass
 			with self.assertWarnsRegex(
 				SyntaxWarning, (
-					r'^Case pattern \'10101010\' \(Color\.RED\) is wider than switch value '
+					r'^Case pattern \'<Color.RED: 170>\' \(8\'10101010\) is wider than switch value '
 					r'\(which has width 4\); comparison will never be true$'
 				)
 			):
 				with m.Case(Color.RED):
 					pass
 		self.assertRepr(m._statements, '''
 		(
 			(switch (sig w1) )
 		)
 		''')
 
+	def test_Switch_zero_width(self):
+		m = Module()
+		s = Signal(0)
+		with m.Switch(s):
+			with m.Case(0):
+				m.d.comb += self.c1.eq(1)
+		m._flush()
+		self.assertRepr(m._statements, '''
+		(
+			(switch (sig s)
+				(case (eq (sig c1) (const 1'd1)))
+			)
+		)
+		''')
+
 	def test_Case_bits_wrong(self):
 		m = Module()
 		with m.Switch(self.w1):
 			with self.assertRaisesRegex(
 				SyntaxError, (
 					r'^Case pattern \'abc\' must consist of 0, 1, and - \(don\'t care\) bits, '
 					r'and may include whitespace$'
@@ -519,27 +558,61 @@
 					pass
 
 	def test_Case_pattern_wrong(self):
 		m = Module()
 		with m.Switch(self.w1):
 			with self.assertRaisesRegex(
 				SyntaxError,
-				r'^Case pattern must be an integer, a string, or an enumeration, not 1\.0$'
+				r'^Case pattern must be a string or a const-castable expression, not 1\.0$'
 			):
 				with m.Case(1.0):
 					pass
 
 	def test_Case_outside_Switch_wrong(self):
 		m = Module()
 		with self.assertRaisesRegex(
 			SyntaxError,
 			r'^Case is not permitted outside of Switch$'
 		):
-			with m.Case():
+			with m.Case(1):
+				pass
+
+	def test_Default_outside_Switch_wrong(self):
+		m = Module()
+		with self.assertRaisesRegex(
+			SyntaxError,
+			r'^Default is not permitted outside of Switch$'
+		):
+			with m.Default():
+				pass
+
+	def test_Case_after_Default_wrong(self):
+		m = Module()
+		with m.Switch(self.w1):
+			with m.Default():
+				pass
+			with self.assertWarns(
+				SyntaxWarning,
+				msg = 'Case statements are order-dependant, any Case after a Default will be ignored'
+			):
+				with m.Case('101-'):
+					pass
+
+	def test_Default_after_Default_wrong(self):
+		m = Module()
+		with m.Switch(self.w1):
+			with m.Default():
 				pass
+			with self.assertRaises(
+				SyntaxError,
+				msg = 'Multiple Default statements within a switch are not allowed, '
+					'as only the first Default will ever be considered.'
+			):
+				with m.Default():
+					pass
 
 	def test_If_inside_Switch_wrong(self):
 		m = Module()
 		with m.Switch(self.s1):
 			with self.assertRaisesRegex(
 				SyntaxError, (
 					r'^If is not permitted directly inside of Switch; '
```

### Comparing `torii-0.5.0/tests/hdl/test_ir.py` & `torii-0.6.0/tests/hdl/test_ir.py`

 * *Files 2% similar despite different names*

```diff
@@ -874,7 +874,75 @@
 	def test_prepare_attrs(self):
 		self.setUp_cpu()
 		self.inst.attrs['ATTR'] = 1
 		f = self.inst.prepare()
 		self.assertEqual(f.attrs, OrderedDict([
 			('ATTR', 1),
 		]))
+
+	def test_assign_names_to_signals(self):
+		i = Signal()
+		rst = Signal()
+		o1 = Signal()
+		o2 = Signal()
+		o3 = Signal()
+		i1 = Signal(name = 'i')
+
+		f = Fragment()
+		f.add_domains(cd_sync := ClockDomain())
+		f.add_domains(cd_sync_norst := ClockDomain(reset_less = True))
+		f.add_ports((i, rst), dir = 'i')
+		f.add_ports((o1, o2, o3), dir = 'o')
+		f.add_statements([o1.eq(0)])
+		f.add_driver(o1, domain = None)
+		f.add_statements([o2.eq(i1)])
+		f.add_driver(o2, domain = 'sync')
+		f.add_statements([o3.eq(i1)])
+		f.add_driver(o3, domain = 'sync_norst')
+
+		names = f._assign_names_to_signals()
+		self.assertEqual(names, SignalDict([
+			(i, 'i'),
+			(rst, 'rst'),
+			(o1, 'o1'),
+			(o2, 'o2'),
+			(o3, 'o3'),
+			(cd_sync.clk, 'clk'),
+			(cd_sync.rst, 'rst$6'),
+			(cd_sync_norst.clk, 'sync_norst_clk'),
+			(i1, 'i$8'),
+		]))
+
+	def test_assign_names_to_fragments(self):
+		f = Fragment()
+		f.add_subfragment(a := Fragment())
+		f.add_subfragment(b := Fragment(), name = 'b')
+
+		names = f._assign_names_to_fragments()
+		self.assertEqual(names, {
+			f: ('top',),
+			a: ('top', 'U$0'),
+			b: ('top', 'b')
+		})
+
+	def test_assign_names_to_fragments_rename_top(self):
+		f = Fragment()
+		f.add_subfragment(a := Fragment())
+		f.add_subfragment(b := Fragment(), name = 'b')
+
+		names = f._assign_names_to_fragments(hierarchy = ('bench', 'cpu'))
+		self.assertEqual(names, {
+			f: ('bench', 'cpu',),
+			a: ('bench', 'cpu', 'U$0'),
+			b: ('bench', 'cpu', 'b')
+		})
+
+	def test_assign_names_to_fragments_collide_with_signal(self):
+		f = Fragment()
+		f.add_subfragment(a_f := Fragment(), name = 'a')
+		f.add_ports((a_s := Signal(name = 'a'),), dir = 'o')
+
+		names = f._assign_names_to_fragments()
+		self.assertEqual(names, {
+			f: ('top',),
+			a_f: ('top', 'a$U$0')
+		})
```

### Comparing `torii-0.5.0/tests/hdl/test_mem.py` & `torii-0.6.0/tests/hdl/test_mem.py`

 * *Files identical despite different names*

### Comparing `torii-0.5.0/tests/hdl/test_rec.py` & `torii-0.6.0/tests/hdl/test_rec.py`

 * *Files 2% similar despite different names*

```diff
@@ -304,30 +304,30 @@
 		self.assertEqual(repr(r1 | s1), '(| (cat (sig r1__a)) (sig s1))')
 		self.assertEqual(repr(1 | r1),  '(| (const 1\'d1) (cat (sig r1__a)))')
 		self.assertEqual(repr(s1 | r1), '(| (sig s1) (cat (sig r1__a)))')
 
 		# __eq__, __ne__, __lt__, __le__, __gt__, __ge__
 		self.assertEqual(repr(r1 == 1),  '(== (cat (sig r1__a)) (const 1\'d1))')
 		self.assertEqual(repr(r1 == s1), '(== (cat (sig r1__a)) (sig s1))')
-		self.assertEqual(repr(s1 == r1), '(== (sig s1) (cat (sig r1__a)))')
+		self.assertEqual(repr(s1 == r1), '(== (cat (sig r1__a)) (sig s1))')
 		self.assertEqual(repr(r1 != 1),  '(!= (cat (sig r1__a)) (const 1\'d1))')
 		self.assertEqual(repr(r1 != s1), '(!= (cat (sig r1__a)) (sig s1))')
-		self.assertEqual(repr(s1 != r1), '(!= (sig s1) (cat (sig r1__a)))')
+		self.assertEqual(repr(s1 != r1), '(!= (cat (sig r1__a)) (sig s1))')
 		self.assertEqual(repr(r1 < 1),   '(< (cat (sig r1__a)) (const 1\'d1))')
 		self.assertEqual(repr(r1 < s1),  '(< (cat (sig r1__a)) (sig s1))')
-		self.assertEqual(repr(s1 < r1),  '(< (sig s1) (cat (sig r1__a)))')
+		self.assertEqual(repr(s1 < r1),  '(> (cat (sig r1__a)) (sig s1))')
 		self.assertEqual(repr(r1 <= 1),  '(<= (cat (sig r1__a)) (const 1\'d1))')
 		self.assertEqual(repr(r1 <= s1), '(<= (cat (sig r1__a)) (sig s1))')
-		self.assertEqual(repr(s1 <= r1), '(<= (sig s1) (cat (sig r1__a)))')
+		self.assertEqual(repr(s1 <= r1), '(>= (cat (sig r1__a)) (sig s1))')
 		self.assertEqual(repr(r1 > 1),   '(> (cat (sig r1__a)) (const 1\'d1))')
 		self.assertEqual(repr(r1 > s1),  '(> (cat (sig r1__a)) (sig s1))')
-		self.assertEqual(repr(s1 > r1),  '(> (sig s1) (cat (sig r1__a)))')
+		self.assertEqual(repr(s1 > r1),  '(< (cat (sig r1__a)) (sig s1))')
 		self.assertEqual(repr(r1 >= 1),  '(>= (cat (sig r1__a)) (const 1\'d1))')
 		self.assertEqual(repr(r1 >= s1), '(>= (cat (sig r1__a)) (sig s1))')
-		self.assertEqual(repr(s1 >= r1), '(>= (sig s1) (cat (sig r1__a)))')
+		self.assertEqual(repr(s1 >= r1), '(<= (cat (sig r1__a)) (sig s1))')
 
 		# __abs__, __len__
 		self.assertEqual(repr(abs(r1)), '(cat (sig r1__a))')
 		self.assertEqual(len(r1), 1)
 
 		# as_unsigned, as_signed, bool, any, all, xor, implies
 		self.assertEqual(repr(r1.as_unsigned()), '(u (cat (sig r1__a)))')
```

### Comparing `torii-0.5.0/tests/hdl/test_xfrm.py` & `torii-0.6.0/tests/hdl/test_xfrm.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # SPDX-License-Identifier: BSD-2-Clause
 # torii: UnusedElaboratable=no
 
 from torii.hdl.ast  import *
 from torii.hdl.cd   import *
+from torii.hdl.dsl  import Module
 from torii.hdl.ir   import *
 from torii.hdl.xfrm import *
 from torii.hdl.mem  import *
+from torii.hdl.mem  import MemoryInstance
 
 from ..utils        import ToriiTestSuiteCase
 
 
 class DomainRenamerTestCase(ToriiTestSuiteCase):
 	def setUp(self):
 		self.s1 = Signal()
@@ -107,14 +109,31 @@
 		f1 = DomainRenamer('ext')(f1)
 		self.assertEqual(cd_sync.name, 'ext')
 		self.assertEqual(f1.domains, {
 			'ext': cd_sync,
 			'pix': cd_pix,
 		})
 
+	def test_rename_mem_ports(self):
+		m = Module()
+		mem = Memory(depth = 4, width = 16)
+		m.submodules.mem = mem
+		mem.read_port(domain = 'a')
+		mem.read_port(domain = 'b')
+		mem.write_port(domain = 'c')
+
+		f = Fragment.get(m, None)
+		f = DomainRenamer({'a': 'd', 'c': 'e'})(f)
+		mem = f.subfragments[0][0]
+		self.assertIsInstance(mem, MemoryInstance)
+		self.assertEqual(mem.read_ports[0].domain, 'd')
+		self.assertEqual(mem.read_ports[1].domain, 'b')
+		self.assertEqual(mem.write_ports[0].domain, 'e')
+
+
 	def test_rename_wrong_to_comb(self):
 		with self.assertRaisesRegex(
 			ValueError,
 			r'^Domain \'sync\' may not be renamed to \'comb\'$'
 		):
 			DomainRenamer('comb')
 
@@ -547,39 +566,28 @@
 		)
 		''')
 
 	def test_enable_read_port(self):
 		mem = Memory(width = 8, depth = 4)
 		mem.read_port(transparent = False)
 		f = EnableInserter(self.c1)(mem).elaborate(platform = None)
-		self.assertRepr(f.named_ports['RD_EN'][0], '''
-		(cat (m (sig c1) (sig mem_r_en) (const 1'd0)))
+		self.assertRepr(f.read_ports[0].en, '''
+		(& (sig mem_r_en) (sig c1))
 		''')
 
 	def test_enable_write_port(self):
 		mem = Memory(width = 8, depth = 4)
-		mem.write_port()
+		mem.write_port(granularity = 2)
 		f = EnableInserter(self.c1)(mem).elaborate(platform = None)
-		self.assertRepr(f.named_ports['WR_EN'][0], '''
-		(cat (m
+		self.assertRepr(f.write_ports[0].en, '''
+		(m
 			(sig c1)
-			(cat
-				(cat
-					(slice (sig mem_w_en) 0:1)
-					(slice (sig mem_w_en) 0:1)
-					(slice (sig mem_w_en) 0:1)
-					(slice (sig mem_w_en) 0:1)
-					(slice (sig mem_w_en) 0:1)
-					(slice (sig mem_w_en) 0:1)
-					(slice (sig mem_w_en) 0:1)
-					(slice (sig mem_w_en) 0:1)
-				)
-			)
-			(const 8'd0)
-		))
+			(sig mem_w_en)
+			(const 4'd0)
+		)
 		''')
 
 
 class _MockElaboratable(Elaboratable):
 	def __init__(self):
 		self.s1 = Signal()
```

### Comparing `torii-0.5.0/tests/lib/coding/test_gray.py` & `torii-0.6.0/tests/lib/coding/test_gray.py`

 * *Files identical despite different names*

### Comparing `torii-0.5.0/tests/lib/coding/test_one_hot.py` & `torii-0.6.0/tests/lib/coding/test_one_hot.py`

 * *Files identical despite different names*

### Comparing `torii-0.5.0/tests/lib/coding/test_priotity.py` & `torii-0.6.0/tests/lib/coding/test_priotity.py`

 * *Files identical despite different names*

### Comparing `torii-0.5.0/tests/lib/soc/csr/test_bus.py` & `torii-0.6.0/tests/lib/soc/csr/test_bus.py`

 * *Files 8% similar despite different names*

```diff
@@ -191,89 +191,111 @@
 			ValueError,
 			r'Address range 0x10000\.\.0x10001 out of bounds for memory map spanning '
 			r'range 0x0\.\.0x10000 \(16 address bits\)'
 		):
 			self.dut.add(elem, addr = 0x10000)
 
 	def test_sim(self):
-		elem_4_r = Element(4, 'r')
-		self.dut.add(elem_4_r)
-		elem_8_w = Element(8, 'w')
-		self.dut.add(elem_8_w)
-		elem_16_rw = Element(16, 'rw')
-		self.dut.add(elem_16_rw)
-
-		bus = self.dut.bus
-
-		def sim_test():
-			yield elem_4_r.r_data.eq(0xa)
-			yield elem_16_rw.r_data.eq(0x5aa5)
-
-			yield bus.addr.eq(0)
-			yield bus.r_stb.eq(1)
-			yield
-			yield bus.r_stb.eq(0)
-			self.assertEqual((yield elem_4_r.r_stb), 1)
-			self.assertEqual((yield elem_16_rw.r_stb), 0)
-			yield
-			self.assertEqual((yield bus.r_data), 0xa)
-
-			yield bus.addr.eq(2)
-			yield bus.r_stb.eq(1)
-			yield
-			yield bus.r_stb.eq(0)
-			self.assertEqual((yield elem_4_r.r_stb), 0)
-			self.assertEqual((yield elem_16_rw.r_stb), 1)
-			yield
-			yield bus.addr.eq(3) # pipeline a read
-			self.assertEqual((yield bus.r_data), 0xa5)
-
-			yield bus.r_stb.eq(1)
-			yield
-			yield bus.r_stb.eq(0)
-			self.assertEqual((yield elem_4_r.r_stb), 0)
-			self.assertEqual((yield elem_16_rw.r_stb), 0)
-			yield
-			self.assertEqual((yield bus.r_data), 0x5a)
-
-			yield bus.addr.eq(1)
-			yield bus.w_data.eq(0x3d)
-			yield bus.w_stb.eq(1)
-			yield
-			yield bus.w_stb.eq(0)
-			yield bus.addr.eq(2) # change address
-			yield
-			self.assertEqual((yield elem_8_w.w_stb), 1)
-			self.assertEqual((yield elem_8_w.w_data), 0x3d)
-			self.assertEqual((yield elem_16_rw.w_stb), 0)
-			yield
-			self.assertEqual((yield elem_8_w.w_stb), 0)
-
-			yield bus.addr.eq(2)
-			yield bus.w_data.eq(0x55)
-			yield bus.w_stb.eq(1)
-			yield
-			self.assertEqual((yield elem_8_w.w_stb), 0)
-			self.assertEqual((yield elem_16_rw.w_stb), 0)
-			yield bus.addr.eq(3) # pipeline a write
-			yield bus.w_data.eq(0xaa)
-			yield
-			self.assertEqual((yield elem_8_w.w_stb), 0)
-			self.assertEqual((yield elem_16_rw.w_stb), 0)
-			yield bus.w_stb.eq(0)
-			yield
-			self.assertEqual((yield elem_8_w.w_stb), 0)
-			self.assertEqual((yield elem_16_rw.w_stb), 1)
-			self.assertEqual((yield elem_16_rw.w_data), 0xaa55)
-
-		sim = Simulator(self.dut)
-		sim.add_clock(1e-6)
-		sim.add_sync_process(sim_test)
-		with sim.write_vcd(vcd_file = open('test.vcd', 'w')):
-			sim.run()
+		for shadow_overlaps in [None, 0, 1]:
+			with self.subTest(shadow_overlaps = shadow_overlaps):
+				dut = Multiplexer(addr_width = 16, data_width = 8, shadow_overlaps = shadow_overlaps)
+
+				elem_4_r = Element(4, 'r')
+				dut.add(elem_4_r)
+				elem_8_w = Element(8, 'w')
+				dut.add(elem_8_w)
+				elem_16_rw = Element(16, 'rw')
+				dut.add(elem_16_rw)
+
+				bus = dut.bus
+
+				def sim_test():
+					yield elem_4_r.r_data.eq(0xa)
+					yield elem_16_rw.r_data.eq(0x5aa5)
+
+					yield bus.addr.eq(0)
+					yield bus.r_stb.eq(1)
+					yield
+					yield bus.r_stb.eq(0)
+					self.assertEqual((yield elem_4_r.r_stb), 1)
+					self.assertEqual((yield elem_16_rw.r_stb), 0)
+					yield
+					self.assertEqual((yield bus.r_data), 0xa)
+
+					yield bus.addr.eq(2)
+					yield bus.r_stb.eq(1)
+					yield
+					yield bus.r_stb.eq(0)
+					self.assertEqual((yield elem_4_r.r_stb), 0)
+					self.assertEqual((yield elem_16_rw.r_stb), 1)
+					yield
+					yield bus.addr.eq(3) # pipeline a read
+					self.assertEqual((yield bus.r_data), 0xa5)
+
+					yield bus.r_stb.eq(1)
+					yield
+					yield bus.r_stb.eq(0)
+					self.assertEqual((yield elem_4_r.r_stb), 0)
+					self.assertEqual((yield elem_16_rw.r_stb), 0)
+					yield
+					self.assertEqual((yield bus.r_data), 0x5a)
+
+					yield bus.addr.eq(1)
+					yield bus.w_data.eq(0x3d)
+					yield bus.w_stb.eq(1)
+					yield
+					yield bus.w_stb.eq(0)
+					yield bus.addr.eq(2) # change address
+					yield
+					self.assertEqual((yield elem_8_w.w_stb), 1)
+					self.assertEqual((yield elem_8_w.w_data), 0x3d)
+					self.assertEqual((yield elem_16_rw.w_stb), 0)
+					yield
+					self.assertEqual((yield elem_8_w.w_stb), 0)
+
+					yield bus.addr.eq(2)
+					yield bus.w_data.eq(0x55)
+					yield bus.w_stb.eq(1)
+					yield
+					self.assertEqual((yield elem_8_w.w_stb), 0)
+					self.assertEqual((yield elem_16_rw.w_stb), 0)
+					yield bus.addr.eq(3) # pipeline a write
+					yield bus.w_data.eq(0xaa)
+					yield
+					self.assertEqual((yield elem_8_w.w_stb), 0)
+					self.assertEqual((yield elem_16_rw.w_stb), 0)
+					yield bus.w_stb.eq(0)
+					yield
+					self.assertEqual((yield elem_8_w.w_stb), 0)
+					self.assertEqual((yield elem_16_rw.w_stb), 1)
+					self.assertEqual((yield elem_16_rw.w_data), 0xaa55)
+
+					yield bus.addr.eq(2)
+					yield bus.r_stb.eq(1)
+					yield bus.w_data.eq(0x66)
+					yield bus.w_stb.eq(1)
+					yield
+					self.assertEqual((yield elem_16_rw.r_stb), 1)
+					self.assertEqual((yield elem_16_rw.w_stb), 0)
+					yield
+					yield bus.addr.eq(3) # pipeline a read and a write
+					yield bus.w_data.eq(0xbb)
+					self.assertEqual((yield bus.r_data), 0xa5)
+					yield
+					yield Delay()
+					self.assertEqual((yield bus.r_data), 0x5a)
+					self.assertEqual((yield elem_16_rw.r_stb), 0)
+					self.assertEqual((yield elem_16_rw.w_stb), 1)
+					self.assertEqual((yield elem_16_rw.w_data), 0xbb66)
+
+				sim = Simulator(dut)
+				sim.add_clock(1e-6)
+				sim.add_sync_process(sim_test)
+				with sim.write_vcd('test.vcd'):
+					sim.run()
 
 
 class MultiplexerAlignedTestCase(ToriiTestSuiteCase):
 	def setUp(self):
 		self.dut = Multiplexer(addr_width = 16, data_width = 8, alignment = 2)
 
 	def test_add_two(self):
@@ -293,47 +315,52 @@
 		elem_0 = Element(8, 'rw')
 		elem_1 = Element(8, 'rw')
 		self.assertEqual(self.dut.add(elem_0), (0, 4))
 		self.assertEqual(self.dut.align_to(alignment = 1), 4)
 		self.assertEqual(self.dut.add(elem_1), (4, 8))
 
 	def test_sim(self):
-		elem_20_rw = Element(20, 'rw')
-		self.dut.add(elem_20_rw)
-
-		bus = self.dut.bus
-
-		def sim_test():
-			yield bus.w_stb.eq(1)
-			yield bus.addr.eq(0)
-			yield bus.w_data.eq(0x55)
-			yield
-			self.assertEqual((yield elem_20_rw.w_stb), 0)
-			yield bus.addr.eq(1)
-			yield bus.w_data.eq(0xaa)
-			yield
-			self.assertEqual((yield elem_20_rw.w_stb), 0)
-			yield bus.addr.eq(2)
-			yield bus.w_data.eq(0x33)
-			yield
-			self.assertEqual((yield elem_20_rw.w_stb), 0)
-			yield bus.addr.eq(3)
-			yield bus.w_data.eq(0xdd)
-			yield
-			self.assertEqual((yield elem_20_rw.w_stb), 0)
-			yield bus.w_stb.eq(0)
-			yield
-			self.assertEqual((yield elem_20_rw.w_stb), 1)
-			self.assertEqual((yield elem_20_rw.w_data), 0x3aa55)
-
-		sim = Simulator(self.dut)
-		sim.add_clock(1e-6)
-		sim.add_sync_process(sim_test)
-		with sim.write_vcd(vcd_file = open('test.vcd', 'w')):
-			sim.run()
+		for shadow_overlaps in [None, 0, 1]:
+			with self.subTest(shadow_overlaps = shadow_overlaps):
+				dut = Multiplexer(addr_width = 16, data_width = 8, alignment = 2,
+									shadow_overlaps = shadow_overlaps)
+
+				elem_20_rw = Element(20, 'rw')
+				dut.add(elem_20_rw)
+
+				bus = dut.bus
+
+				def sim_test():
+					yield bus.w_stb.eq(1)
+					yield bus.addr.eq(0)
+					yield bus.w_data.eq(0x55)
+					yield
+					self.assertEqual((yield elem_20_rw.w_stb), 0)
+					yield bus.addr.eq(1)
+					yield bus.w_data.eq(0xaa)
+					yield
+					self.assertEqual((yield elem_20_rw.w_stb), 0)
+					yield bus.addr.eq(2)
+					yield bus.w_data.eq(0x33)
+					yield
+					self.assertEqual((yield elem_20_rw.w_stb), 0)
+					yield bus.addr.eq(3)
+					yield bus.w_data.eq(0xdd)
+					yield
+					self.assertEqual((yield elem_20_rw.w_stb), 0)
+					yield bus.w_stb.eq(0)
+					yield
+					self.assertEqual((yield elem_20_rw.w_stb), 1)
+					self.assertEqual((yield elem_20_rw.w_data), 0x3aa55)
+
+				sim = Simulator(dut)
+				sim.add_clock(1e-6)
+				sim.add_sync_process(sim_test)
+				with sim.write_vcd('test.vcd'):
+					sim.run()
 
 
 class DecoderTestCase(ToriiTestSuiteCase):
 	def setUp(self):
 		self.dut = Decoder(addr_width = 16, data_width = 8)
 
 	def test_align_to(self):
@@ -432,9 +459,9 @@
 			self.assertEqual((yield bus.r_data), 0xaa)
 
 		m = Module()
 		m.submodules += self.dut, mux_1, mux_2
 		sim = Simulator(m)
 		sim.add_clock(1e-6)
 		sim.add_sync_process(sim_test)
-		with sim.write_vcd(vcd_file = open('test.vcd', 'w')):
+		with sim.write_vcd('test.vcd'):
 			sim.run()
```

### Comparing `torii-0.5.0/tests/lib/soc/csr/test_event.py` & `torii-0.6.0/tests/lib/soc/csr/test_event.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from ....utils         import ToriiTestSuiteCase
 
 def simulation_test(dut, process):
 	sim = Simulator(dut)
 	sim.add_clock(1e-6)
 	sim.add_sync_process(process)
-	with sim.write_vcd(vcd_file = open('test.vcd', 'w')):
+	with sim.write_vcd('test.vcd'):
 		sim.run()
 
 
 class EventMonitorTestCase(ToriiTestSuiteCase):
 	def test_params(self):
 		monitor = EventMonitor(data_width = 16, alignment = 4, trigger = 'rise')
 		self.assertEqual(monitor.bus.data_width, 16)
```

### Comparing `torii-0.5.0/tests/lib/soc/csr/test_wishbone.py` & `torii-0.6.0/tests/lib/soc/csr/test_wishbone.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,15 +143,15 @@
 			self.assertEqual((yield reg_2.w_count), 1)
 
 		m = Module()
 		m.submodules += mux, reg_1, reg_2, dut
 		sim = Simulator(m)
 		sim.add_clock(1e-6)
 		sim.add_sync_process(sim_test)
-		with sim.write_vcd(vcd_file = open('test.vcd', 'w')):
+		with sim.write_vcd('test.vcd'):
 			sim.run()
 
 	def test_wide(self):
 		mux = csr.Multiplexer(addr_width = 10, data_width = 8)
 		reg = MockRegister(32, name = 'reg')
 		mux.add(reg.element)
 		dut = WishboneCSRBridge(mux.bus, data_width = 32)
@@ -235,9 +235,9 @@
 			self.assertEqual((yield reg.w_count), 1)
 
 		m = Module()
 		m.submodules += mux, reg, dut
 		sim = Simulator(m)
 		sim.add_clock(1e-6)
 		sim.add_sync_process(sim_test)
-		with sim.write_vcd(vcd_file = open('test.vcd', 'w')):
+		with sim.write_vcd('test.vcd'):
 			sim.run()
```

### Comparing `torii-0.5.0/tests/lib/soc/test_event.py` & `torii-0.6.0/tests/lib/soc/test_event.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from ...utils            import ToriiTestSuiteCase
 
 def simulation_test(dut, process):
 	sim = Simulator(dut)
 	sim.add_clock(1e-6)
 	sim.add_sync_process(process)
-	with sim.write_vcd(vcd_file = open('test.vcd', 'w')):
+	with sim.write_vcd('test.vcd'):
 		sim.run()
 
 
 class SourceTestCase(ToriiTestSuiteCase):
 	def test_level(self):
 		src = Source(trigger = 'level')
 		self.assertEqual(src.trigger, Source.Trigger.LEVEL)
```

### Comparing `torii-0.5.0/tests/lib/soc/test_memory.py` & `torii-0.6.0/tests/lib/soc/test_memory.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,18 @@
 		self.assertEqual(range_map.overlaps(range(0, 3)), [])
 		self.assertEqual(range_map.overlaps(range(0, 5)), [])
 		self.assertEqual(range_map.overlaps(range(25, 30)), [])
 
 	def test_insert_wrong_overlap(self):
 		range_map = _RangeMap()
 		range_map.insert(range(0, 10), 'a')
-		with self.assertRaises(AssertionError):
+		with self.assertRaisesRegex(
+			ValueError,
+			r'^Key range\(5, 15\) overlaps an existing region!$'
+		):
 			range_map.insert(range(5, 15), 'b')
 
 	def test_get(self):
 		range_map = _RangeMap()
 		range_map.insert(range(5, 15), 'a')
 		self.assertEqual(range_map.get(0), None)
 		self.assertEqual(range_map.get(5), 'a')
```

### Comparing `torii-0.5.0/tests/lib/soc/test_periph.py` & `torii-0.6.0/tests/lib/soc/test_periph.py`

 * *Files identical despite different names*

### Comparing `torii-0.5.0/tests/lib/soc/wishbone/test_bus.py` & `torii-0.6.0/tests/lib/soc/wishbone/test_bus.py`

 * *Files 7% similar despite different names*

```diff
@@ -283,15 +283,15 @@
 			self.assertEqual((yield dut.bus.err), 1)
 			self.assertEqual((yield dut.bus.rty), 1)
 			self.assertEqual((yield dut.bus.stall), 1)
 			self.assertEqual((yield dut.bus.dat_r), 0x5678abcd)
 
 		sim = Simulator(dut)
 		sim.add_process(sim_test)
-		with sim.write_vcd(vcd_file = open('test.vcd', 'w')):
+		with sim.write_vcd('test.vcd'):
 			sim.run()
 
 	def test_addr_translate(self):
 		class AddressLoopback(Elaboratable):
 			def __init__(self, **kwargs):
 				self.bus = Interface(**kwargs)
 
@@ -402,15 +402,15 @@
 			yield Delay(1e-6)
 			self.assertEqual((yield dut.bus.dat_r), 0x09)
 
 		m = Module()
 		m.submodules += dut, loop_1, loop_2, loop_3, loop_4
 		sim = Simulator(m)
 		sim.add_process(sim_test)
-		with sim.write_vcd(vcd_file = open('test.vcd', 'w')):
+		with sim.write_vcd('test.vcd'):
 			sim.run()
 
 	def test_coarse_granularity(self):
 		dut = Decoder(addr_width = 3, data_width = 32)
 		sub = Interface(addr_width = 2, data_width = 32)
 		sub.memory_map = MemoryMap(addr_width = 2, data_width = 32)
 		dut.add(sub)
@@ -424,15 +424,15 @@
 
 			yield dut.bus.adr.eq(0x4)
 			yield Delay(1e-6)
 			self.assertEqual((yield sub.cyc), 0)
 
 		sim = Simulator(dut)
 		sim.add_process(sim_test)
-		with sim.write_vcd(vcd_file = open('test.vcd', 'w')):
+		with sim.write_vcd('test.vcd'):
 			sim.run()
 
 
 class ArbiterTestCase(ToriiTestSuiteCase):
 	def setUp(self):
 		self.dut = Arbiter(
 			addr_width = 31, data_width = 32, granularity = 16,
@@ -550,15 +550,15 @@
 			self.assertEqual((yield intr_2.err), 1)
 			self.assertEqual((yield intr_2.rty), 1)
 			self.assertEqual((yield intr_2.stall), 0)
 
 		sim = Simulator(dut)
 		sim.add_clock(1e-6)
 		sim.add_sync_process(sim_test)
-		with sim.write_vcd(vcd_file = open('test.vcd', 'w')):
+		with sim.write_vcd('test.vcd'):
 			sim.run()
 
 	def test_lock(self):
 		dut = Arbiter(addr_width = 30, data_width = 32, features = {'lock'})
 		intr_1 = Interface(addr_width = 30, data_width = 32, features = {'lock'})
 		dut.add(intr_1)
 		intr_2 = Interface(addr_width = 30, data_width = 32, features = {'lock'})
@@ -602,15 +602,15 @@
 			yield Delay(1e-7)
 			self.assertEqual((yield intr_1.ack), 0)
 			self.assertEqual((yield intr_2.ack), 1)
 
 		sim = Simulator(dut)
 		sim.add_clock(1e-6)
 		sim.add_sync_process(sim_test)
-		with sim.write_vcd(vcd_file = open('test.vcd', 'w')):
+		with sim.write_vcd('test.vcd'):
 			sim.run()
 
 	def test_stall(self):
 		dut = Arbiter(addr_width = 30, data_width = 32, features = {'stall'})
 		intr_1 = Interface(addr_width = 30, data_width = 32, features = {'stall'})
 		dut.add(intr_1)
 		intr_2 = Interface(addr_width = 30, data_width = 32, features = {'stall'})
@@ -627,15 +627,15 @@
 			yield dut.bus.stall.eq(1)
 			yield Delay(1e-6)
 			self.assertEqual((yield intr_1.stall), 1)
 			self.assertEqual((yield intr_2.stall), 1)
 
 		sim = Simulator(dut)
 		sim.add_process(sim_test)
-		with sim.write_vcd(vcd_file = open('test.vcd', 'w')):
+		with sim.write_vcd('test.vcd'):
 			sim.run()
 
 	def test_stall_compat(self):
 		dut = Arbiter(addr_width = 30, data_width = 32)
 		intr_1 = Interface(addr_width = 30, data_width = 32, features = {'stall'})
 		dut.add(intr_1)
 		intr_2 = Interface(addr_width = 30, data_width = 32, features = {'stall'})
@@ -651,15 +651,15 @@
 			yield dut.bus.ack.eq(1)
 			yield Delay(1e-6)
 			self.assertEqual((yield intr_1.stall), 0)
 			self.assertEqual((yield intr_2.stall), 1)
 
 		sim = Simulator(dut)
 		sim.add_process(sim_test)
-		with sim.write_vcd(vcd_file = open('test.vcd', 'w')):
+		with sim.write_vcd('test.vcd'):
 			sim.run()
 
 	def test_roundrobin(self):
 		dut = Arbiter(addr_width = 30, data_width = 32)
 		intr_1 = Interface(addr_width = 30, data_width = 32)
 		dut.add(intr_1)
 		intr_2 = Interface(addr_width = 30, data_width = 32)
@@ -712,9 +712,9 @@
 			self.assertEqual((yield intr_1.ack), 0)
 			self.assertEqual((yield intr_2.ack), 0)
 			self.assertEqual((yield intr_3.ack), 1)
 
 		sim = Simulator(dut)
 		sim.add_clock(1e-6)
 		sim.add_sync_process(sim_test)
-		with sim.write_vcd(vcd_file = open('test.vcd', 'w')):
+		with sim.write_vcd('test.vcd'):
 			sim.run()
```

### Comparing `torii-0.5.0/tests/lib/stdio/test_serial.py` & `torii-0.6.0/tests/lib/stdio/test_serial.py`

 * *Files identical despite different names*

### Comparing `torii-0.5.0/tests/lib/test_cdc.py` & `torii-0.6.0/tests/lib/test_cdc.py`

 * *Files identical despite different names*

### Comparing `torii-0.5.0/tests/lib/test_fifo.py` & `torii-0.6.0/tests/lib/test_fifo.py`

 * *Files identical despite different names*

### Comparing `torii-0.5.0/tests/lib/test_io.py` & `torii-0.6.0/tests/lib/test_io.py`

 * *Files identical despite different names*

### Comparing `torii-0.5.0/tests/lib/test_scheduler.py` & `torii-0.6.0/tests/lib/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `torii-0.5.0/tests/sim/test_sim.py` & `torii-0.6.0/tests/sim/test_sim.py`

 * *Files 1% similar despite different names*

```diff
@@ -936,15 +936,15 @@
 		self.m = Module()
 		self.m.d.comb += self.x.eq(self.a ^ self.b)
 		with self.m.Switch(self.s):
 			with self.m.Case(0):
 				self.m.d.sync += self.o.eq(self.a + self.b)
 			with self.m.Case(1):
 				self.m.d.sync += self.o.eq(self.a - self.b)
-			with self.m.Case():
+			with self.m.Default():
 				self.m.d.sync += self.o.eq(0)
 		self.m.domains += self.sync
 
 	def test_alu(self):
 		self.setUp_alu()
 		with self.assertSimulation(self.m) as sim:
 			sim.add_clock(1e-6)
@@ -1129,15 +1129,36 @@
 				nonlocal survived
 
 				with self.assertRaisesRegex(
 					TypeError,
 					r'Received unsupported command 1 from process .+'
 				):
 					yield 1
-				yield Settle()
+				# yield Settle()
+				survived = True
+			sim.add_process(process)
+		self.assertTrue(survived)
+
+	def test_value_castable(self):
+		class MyValue(ValueCastable):
+			@ValueCastable.lowermethod
+			def as_value(self):
+				return Signal()
+
+			def shape():
+				return unsigned(1)
+
+		a = Array([1,2,3])
+		a[MyValue()]
+
+		survived = False
+		with self.assertSimulation(Module()) as sim:
+			def process():
+				nonlocal survived
+				yield MyValue()
 				survived = True
 			sim.add_process(process)
 		self.assertTrue(survived)
 
 	def setUp_memory(self, rd_synchronous = True, rd_transparent = True, wr_granularity = None):
 		self.m = Module()
 		self.memory = Memory(width = 8, depth = 4, init = [0xaa, 0x55])
@@ -1443,14 +1464,27 @@
 			op = (op ^ 1)
 
 		op = op & op
 
 		m.d.comb += a.eq(op)
 		Simulator(m)
 
+	def test_switch_zero(self):
+		m = Module()
+		a = Signal(0)
+		o = Signal()
+		with m.Switch(a):
+			with m.Case(''):
+				m.d.comb += o.eq(1)
+		with self.assertSimulation(m) as sim:
+			def process():
+				yield Settle()
+				self.assertEqual((yield o), 1)
+			sim.add_process(process)
+
 class SimulatorRegressionTestCase(ToriiTestSuiteCase):
 	def test_bug_325(self):
 		dut = Module()
 		dut.d.comb += Signal().eq(Cat())
 		Simulator(dut).run()
 
 	def test_bug_473(self):
```

### Comparing `torii-0.5.0/tests/test/test_test.py` & `torii-0.6.0/tests/test/test_test.py`

 * *Files identical despite different names*

### Comparing `torii-0.5.0/tests/test_examples.py` & `torii-0.6.0/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `torii-0.5.0/tests/tools/test_cxx.py` & `torii-0.6.0/tests/tools/test_cxx.py`

 * *Files identical despite different names*

### Comparing `torii-0.5.0/tests/util/test_string.py` & `torii-0.6.0/tests/util/test_string.py`

 * *Files identical despite different names*

### Comparing `torii-0.5.0/tests/utils.py` & `torii-0.6.0/tests/utils.py`

 * *Files identical despite different names*

### Comparing `torii-0.5.0/torii/__init__.py` & `torii-0.6.0/torii/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 	# `lib/pythonX.Y/site-packages`. Although not a recommended way, we still try to support it.
 	__version__ = 'unknown'
 
 
 from .hdl import (
 	Array, Cat, ClockDomain, ClockSignal, Const, DomainRenamer,
 	Elaboratable, EnableInserter, Fragment, Instance, Memory,
-	Module, Mux, Record, Repl, ResetInserter, ResetSignal, Shape,
+	Module, Mux, Record, ResetInserter, ResetSignal, Shape,
 	Signal, Value, signed, unsigned
 )
 
 __all__ = (
 	'Array',
 	'Cat',
 	'ClockDomain',
@@ -27,15 +27,14 @@
 	'EnableInserter',
 	'Fragment',
 	'Instance',
 	'Memory',
 	'Module',
 	'Mux',
 	'Record',
-	'Repl',
 	'ResetInserter',
 	'ResetSignal',
 	'Shape',
 	'Signal',
 	'Value',
 	'signed',
 	'unsigned',
```

### Comparing `torii-0.5.0/torii/back/__init__.py` & `torii-0.6.0/torii/back/__init__.py`

 * *Files identical despite different names*

### Comparing `torii-0.5.0/torii/back/cxxrtl.py` & `torii-0.6.0/torii/back/cxxrtl.py`

 * *Files identical despite different names*

### Comparing `torii-0.5.0/torii/back/rtlil.py` & `torii-0.6.0/torii/back/rtlil.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import io
 import re
 from collections  import OrderedDict
 from contextlib   import contextmanager
 from typing       import Literal, Optional, Union
 
-from ..hdl        import ast, ir, mem, xfrm
+from ..hdl        import ast, ir, xfrm, mem
 from ..util       import flatten
 from ..util.units import bits_for
 
 __all__ = (
 	'convert_fragment',
 	'convert',
 )
@@ -58,15 +58,18 @@
 		super().__init__()
 		self._anon  = 0
 		self._index = 0
 		self._names = set()
 
 	def anonymous(self) -> str:
 		name = f'U$${self._anon}'
-		assert name not in self._names
+
+		if name in self._names:
+			raise ValueError(f'Name \'{name}\' already exists!')
+
 		self._anon += 1
 		return name
 
 	def _make_name(self, name: Optional[str], local: bool) -> str:
 		if name is None:
 			self._index += 1
 			name = f'${self._index}'
@@ -229,17 +232,14 @@
 	def __exit__(self, *args) -> None:
 		self._append('  end\n')
 		self.rtlil._buffer.write(str(self))
 
 	def case(self) -> '_CaseBuilder':
 		return _CaseBuilder(self, indent = 2)
 
-	def sync(self, kind: Literal['i', 'o', 'io'], cond: Optional[str] = None) -> '_SyncBuilder':
-		return _SyncBuilder(self, kind, cond)
-
 
 class _CaseBuilder(_ProxiedBuilder):
 	def __init__(self, rtlil, indent: int):
 		self.rtlil  = rtlil
 		self.indent = indent
 
 	def __enter__(self) -> '_CaseBuilder':
@@ -285,34 +285,14 @@
 		else:
 			self._append(
 				'{}case {}\n', '  ' * (self.indent + 1), ', '.join(f'{len(value)}\'{value}'for value in values)
 			)
 		return _CaseBuilder(self.rtlil, self.indent + 2)
 
 
-class _SyncBuilder(_ProxiedBuilder):
-	def __init__(self, rtlil, kind: Literal['i', 'o', 'io'], cond: Optional[str]) -> None:
-		self.rtlil = rtlil
-		self.kind  = kind
-		self.cond  = cond
-
-	def __enter__(self) -> '_SyncBuilder':
-		if self.cond is None:
-			self._append('    sync {}\n', self.kind)
-		else:
-			self._append('    sync {} {}\n', self.kind, self.cond)
-		return self
-
-	def __exit__(self, *args) -> None:
-		pass
-
-	def update(self, lhs, rhs) -> None:
-		self._append('      update {} {}\n', lhs, rhs)
-
-
 def _src(src_loc: Optional[tuple[str, int]]) -> Optional[str]:
 	if src_loc is None:
 		return None
 	file, line = src_loc
 	return f'{file}:{line}'
 
 
@@ -396,15 +376,17 @@
 		if not self.expansions:
 			return value
 		return self.expansions.get(value, value)
 
 	@contextmanager
 	def expand_to(self, value, expansion):
 		try:
-			assert value not in self.expansions
+			if value in self.expansions:
+				raise ValueError(f'Value {value} expansion already exists!')
+
 			self.expansions[value] = expansion
 			yield
 		finally:
 			del self.expansions[value]
 
 
 class _ValueCompiler(xfrm.ValueVisitor):
@@ -492,35 +474,21 @@
 
 	def on_value(self, value):
 		return super().on_value(self.s.expand(value))
 
 	def on_Const(self, value):
 		return _const(value)
 
-	def on_AnyConst(self, value):
-		if value in self.s.anys:
-			return self.s.anys[value]
-
-		res_shape = value.shape()
-		res = self.s.rtlil.wire(width = res_shape.width, src = _src(value.src_loc))
-		self.s.rtlil.cell('$anyconst', ports = {
-			'\\Y': res,
-		}, params = {
-			'WIDTH': res_shape.width,
-		}, src = _src(value.src_loc))
-		self.s.anys[value] = res
-		return res
-
-	def on_AnySeq(self, value):
+	def on_AnyValue(self, value):
 		if value in self.s.anys:
 			return self.s.anys[value]
 
 		res_shape = value.shape()
 		res = self.s.rtlil.wire(width = res_shape.width, src = _src(value.src_loc))
-		self.s.rtlil.cell('$anyseq', ports = {
+		self.s.rtlil.cell(f'${value.kind.value}', ports = {
 			'\\Y': res,
 		}, params = {
 			'WIDTH': res_shape.width,
 		}, src = _src(value.src_loc))
 		self.s.anys[value] = res
 		return res
 
@@ -626,15 +594,17 @@
 
 	def on_Operator(self, value):
 		if len(value.operands) == 1:
 			return self.on_Operator_unary(value)
 		elif len(value.operands) == 2:
 			return self.on_Operator_binary(value)
 		elif len(value.operands) == 3:
-			assert value.operator == 'm'
+			if value.operator != 'm':
+				raise ValueError(f'Operator \'{value.operator}\' not applicable for 3 operands!')
+
 			return self.on_Operator_mux(value)
 		else:
 			raise TypeError # :nocov:
 
 	def _prepare_value_for_Slice(self, value):
 		if isinstance(value, (ast.Signal, ast.Slice, ast.Cat)):
 			sigspec = self(value)
@@ -668,18 +638,15 @@
 		return res
 
 
 class _LHSValueCompiler(_ValueCompiler):
 	def on_Const(self, value):
 		raise TypeError # :nocov:
 
-	def on_AnyConst(self, value):
-		raise TypeError # :nocov:
-
-	def on_AnySeq(self, value):
+	def on_AnyValue(self, value):
 		raise TypeError # :nocov:
 
 	def on_Operator(self, value):
 		if value.operator in ('u', 's'):
 			# These operators are transparent on the LHS.
 			arg, = value.operands
 			return self(arg)
@@ -700,15 +667,16 @@
 	def on_Signal(self, value):
 		if value not in self.s.driven:
 			raise ValueError(f'No LHS wire for non-driven signal {repr(value)}')
 		wire_curr, wire_next = self.s.resolve(value)
 		return wire_next or wire_curr
 
 	def _prepare_value_for_Slice(self, value):
-		assert isinstance(value, (ast.Signal, ast.Slice, ast.Cat, ast.Part))
+		if not isinstance(value, (ast.Signal, ast.Slice, ast.Cat, ast.Part)):
+			raise TypeError(f'value must be one of \'Signal\', \'Slice\', \'Cat\', or \'Part\', not \'{value!r}\'')
 		return self(value)
 
 	def on_Part(self, value):
 		offset = self.s.expand(value.offset)
 		if isinstance(offset, ast.Const):
 			start = offset.value * value.stride
 			stop  = start + value.width
@@ -769,29 +737,25 @@
 			# mismatch, we wrap all assigns following a switch in a dummy switch.
 			with self._case.switch('{ }') as wrap_switch:
 				with wrap_switch.case() as wrap_case:
 					wrap_case.assign(self.lhs_compiler(stmt.lhs), rhs_sigspec)
 		else:
 			self._case.assign(self.lhs_compiler(stmt.lhs), rhs_sigspec)
 
-	def on_property(self, stmt):
+	def on_Property(self, stmt):
 		self(stmt._check.eq(stmt.test))
 		self(stmt._en.eq(1))
 
 		en_wire = self.rhs_compiler(stmt._en)
 		check_wire = self.rhs_compiler(stmt._check)
-		self.state.rtlil.cell('$' + stmt._kind, ports = {
+		self.state.rtlil.cell(f'${stmt.kind.value}', ports = {
 			'\\A' : check_wire,
 			'\\EN': en_wire,
 		}, src = _src(stmt.src_loc), name = stmt.name)
 
-	on_Assert = on_property
-	on_Assume = on_property
-	on_Cover  = on_property
-
 	def on_Switch(self, stmt):
 		self._check_rhs(stmt.test)
 
 		if not self.state.expansions:
 			# We repeatedly translate the same switches over and over (see the LHSGroupAnalyzer
 			# related code below), and translating the switch test only once helps readability.
 			if stmt not in self._test_cache:
@@ -849,18 +813,97 @@
 
 def _convert_fragment(builder, fragment, name_map, hierarchy):
 	if isinstance(fragment, ir.Instance):
 		port_map = OrderedDict()
 		for port_name, (value, dir) in fragment.named_ports.items():
 			port_map[f'\\{port_name}'] = value
 
+		params = OrderedDict(fragment.parameters)
+
 		if fragment.type[0] == '$':
-			return fragment.type, port_map
+			return fragment.type, port_map, params
 		else:
-			return f'\\{fragment.type}', port_map
+			return f'\\{fragment.type}', port_map, params
+
+	if isinstance(fragment, mem.MemoryInstance):
+		memory = fragment.memory
+		init = ''.join(
+			format(
+				ast.Const(elem, ast.unsigned(memory.width)).value,
+				f'0{memory.width}b'
+			)
+			for elem in reversed(memory.init)
+		)
+		init = ast.Const(int(init or '0', 2), memory.depth * memory.width)
+
+		rd_clk = []
+		rd_clk_enable = 0
+		rd_clk_polarity = 0
+		rd_transparency_mask = 0
+		for index, port in enumerate(fragment.read_ports):
+			if port.domain != 'comb':
+				cd = fragment.domains[port.domain]
+				rd_clk.append(cd.clk)
+				if cd.clk_edge == 'pos':
+					rd_clk_polarity |= 1 << index
+				rd_clk_enable |= 1 << index
+				if port.transparent:
+					for write_index, write_port in enumerate(fragment.write_ports):
+						if port.domain == write_port.domain:
+							rd_transparency_mask |= 1 << (index * len(fragment.write_ports) + write_index)
+			else:
+				rd_clk.append(ast.Const(0, 1))
+
+		wr_clk = []
+		wr_clk_enable = 0
+		wr_clk_polarity = 0
+		for index, port in enumerate(fragment.write_ports):
+			cd = fragment.domains[port.domain]
+			wr_clk.append(cd.clk)
+			wr_clk_enable |= 1 << index
+			if cd.clk_edge == 'pos':
+				wr_clk_polarity |= 1 << index
+
+		params = {
+			'MEMID': builder._make_name(hierarchy[-1], local = False),
+			'SIZE': memory.depth,
+			'OFFSET': 0,
+			'ABITS': ast.Shape.cast(range(memory.depth)).width,
+			'WIDTH': memory.width,
+			'INIT': init,
+			'RD_PORTS': len(fragment.read_ports),
+			'RD_CLK_ENABLE': ast.Const(rd_clk_enable, max(1, len(fragment.read_ports))),
+			'RD_CLK_POLARITY': ast.Const(rd_clk_polarity, max(1, len(fragment.read_ports))),
+			'RD_TRANSPARENCY_MASK': ast.Const(rd_transparency_mask, max(1, len(fragment.read_ports) * len(fragment.write_ports))),
+			'RD_COLLISION_X_MASK': ast.Const(0, max(1, len(fragment.read_ports) * len(fragment.write_ports))),
+			'RD_WIDE_CONTINUATION': ast.Const(0, max(1, len(fragment.read_ports))),
+			'RD_CE_OVER_SRST': ast.Const(0, max(1, len(fragment.read_ports))),
+			'RD_ARST_VALUE': ast.Const(0, len(fragment.read_ports) * memory.width),
+			'RD_SRST_VALUE': ast.Const(0, len(fragment.read_ports) * memory.width),
+			'RD_INIT_VALUE': ast.Const(0, len(fragment.read_ports) * memory.width),
+			'WR_PORTS': len(fragment.write_ports),
+			'WR_CLK_ENABLE': ast.Const(wr_clk_enable, max(1, len(fragment.write_ports))),
+			'WR_CLK_POLARITY': ast.Const(wr_clk_polarity, max(1, len(fragment.write_ports))),
+			'WR_PRIORITY_MASK': ast.Const(0, max(1, len(fragment.write_ports) * len(fragment.write_ports))),
+			'WR_WIDE_CONTINUATION': ast.Const(0, max(1, len(fragment.write_ports))),
+		}
+
+		port_map = {
+			'\\RD_CLK': ast.Cat(rd_clk),
+			'\\RD_EN': ast.Cat(port.en for port in fragment.read_ports),
+			'\\RD_ARST': ast.Const(0, len(fragment.read_ports)),
+			'\\RD_SRST': ast.Const(0, len(fragment.read_ports)),
+			'\\RD_ADDR': ast.Cat(port.addr for port in fragment.read_ports),
+			'\\RD_DATA': ast.Cat(port.data for port in fragment.read_ports),
+			'\\WR_CLK': ast.Cat(wr_clk),
+			'\\WR_EN': ast.Cat(ast.Cat(en_bit.replicate(port.granularity) for en_bit in port.en) for port in fragment.write_ports),
+			'\\WR_ADDR': ast.Cat(port.addr for port in fragment.write_ports),
+			'\\WR_DATA': ast.Cat(port.data for port in fragment.write_ports),
+		}
+		return '$mem_v2', port_map, params
 
 	module_name  = '.'.join(name or 'anonymous' for name in hierarchy)
 	module_attrs = OrderedDict()
 	if len(hierarchy) == 1:
 		module_attrs['top'] = 1
 
 	with builder.module(module_name, attrs = module_attrs) as module:
@@ -888,43 +931,54 @@
 			if cd.rst is not None:
 				compiler_state.resolve_curr(cd.rst)
 
 		# Transform all subfragments to their respective cells. Transforming signals connected
 		# to their ports into wires eagerly makes sure they get sensible (prefixed with submodule
 		# name) names.
 		for subfragment, sub_name in fragment.subfragments:
-			if not (subfragment.ports or subfragment.statements or subfragment.subfragments):
+			if not (
+				subfragment.ports or subfragment.statements or
+				subfragment.subfragments or isinstance(subfragment, (ir.Instance, mem.MemoryInstance))
+			):
 				# If the fragment is completely empty, skip translating it, otherwise synthesis
 				# tools (including Yosys and Vivado) will treat it as a black box when it is
 				# loaded after conversion to Verilog.
 				continue
 
 			if sub_name is None:
 				sub_name = module.anonymous()
 
-			sub_params = OrderedDict(getattr(subfragment, 'parameters', {}))
-
-			sub_type, sub_port_map = _convert_fragment(
+			sub_type, sub_port_map, sub_params = _convert_fragment(
 				builder, subfragment, name_map,
 				hierarchy = hierarchy + (sub_name,)
 			)
 
-			if sub_type == '$mem_v2' and 'MEMID' not in sub_params:
-				sub_params['MEMID'] = builder._make_name(sub_name, local = False)
-
 			sub_ports = OrderedDict()
 			for port, value in sub_port_map.items():
-				if not isinstance(subfragment, ir.Instance):
+				if not isinstance(subfragment, (ir.Instance, mem.MemoryInstance)):
 					for signal in value._rhs_signals():
 						compiler_state.resolve_curr(signal, prefix = sub_name)
 				if len(value) > 0 or sub_type == '$mem_v2':
 					sub_ports[port] = rhs_compiler(value)
 
-			module.cell(sub_type, name = sub_name, ports = sub_ports, params = sub_params,
-						attrs = subfragment.attrs)
+			if isinstance(subfragment, ir.Instance):
+				src = _src(subfragment.src_loc)
+			if isinstance(subfragment, mem.MemoryInstance):
+				src = _src(subfragment.memory.src_loc)
+			else:
+				src = ''
+
+			module.cell(
+				sub_type,
+				name = sub_name,
+				ports = sub_ports,
+				params = sub_params,
+				attrs = subfragment.attrs,
+				src = src
+			)
 
 		# If we emit all of our combinatorial logic into a single RTLIL process, Verilog
 		# simulators will break horribly, because Yosys write_verilog transforms RTLIL processes
 		# into always @* blocks with blocking assignment, and that does not create delta cycles.
 		#
 		# Therefore, we translate the fragment as many times as there are independent groups
 		# of signals (a group is a transitive closure of signals that appear together on LHS),
@@ -1027,15 +1081,15 @@
 	# the caller, to allow manipulating them in the toolchain.
 	for signal in compiler_state.wires:
 		wire_name = compiler_state.resolve_curr(signal)
 		if wire_name.startswith('\\'):
 			wire_name = wire_name[1:]
 		name_map[signal] = hierarchy + (wire_name,)
 
-	return module.name, port_map
+	return module.name, port_map, {}
 
 
 def convert_fragment(
 	fragment: ir.Fragment, name: str = 'top', *, emit_src: bool = True
 ) -> tuple[str, ast.SignalDict]:
 	if not isinstance(fragment, ir.Fragment):
 		raise ValueError(f'Expected an ir.Fragment not a {fragment!r}')
```

### Comparing `torii-0.5.0/torii/back/verilog.py` & `torii-0.6.0/torii/back/verilog.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,22 +14,19 @@
 
 
 def _convert_rtlil_text(
 	rtlil_text: str, *, strip_internal_attrs: bool = False, write_verilog_opts: tuple[str] = ()
 ) -> str:
 
 	yosys = find_yosys()
-	yosys_version = yosys.version()
 
 	script = []
 	script.append(f'read_rtlil <<rtlil\n{rtlil_text}\nrtlil')
-	if yosys_version >= (0, 17):
-		script.append('proc -nomux -norom')
-	else:
-		script.append('proc -nomux')
+
+	script.append('proc -nomux -norom')
 	script.append('memory_collect')
 
 	if strip_internal_attrs:
 		attr_map = []
 		attr_map.append('-remove generator')
 		attr_map.append('-remove top')
 		attr_map.append('-remove src')
```

### Comparing `torii-0.5.0/torii/build/dsl.py` & `torii-0.6.0/torii/build/dsl.py`

 * *Files identical despite different names*

### Comparing `torii-0.5.0/torii/build/plat.py` & `torii-0.6.0/torii/build/plat.py`

 * *Files 3% similar despite different names*

```diff
@@ -151,15 +151,17 @@
 			m.d.comb += ClockSignal('sync').eq(clk_i)
 			m.submodules.reset_sync = ResetSynchronizer(rst_i, domain = 'sync')
 			return m
 
 	def prepare(
 		self, elaboratable: Union[Fragment, Elaboratable], name: str = 'top', **kwargs
 	) -> BuildPlan:
-		assert not self._prepared
+		if self._prepared:
+			raise RuntimeError(f'Design \'{name}\' is already prepared!')
+
 		self._prepared = True
 
 		fragment = Fragment.get(elaboratable, self)
 		fragment = SampleLowerer()(fragment)
 		fragment._propagate_domains(self.create_missing_domain, platform = self)
 		fragment = DomainLowerer()(fragment)
 
@@ -307,16 +309,17 @@
 	@property
 	@abstractmethod
 	def command_templates(self) -> list[str]:
 		raise NotImplementedError('Platform must implement this property')
 
 	build_script_templates = {
 		'build_{{name}}.sh': '''
+			#!/bin/sh
 			# {{autogenerated}}
-			set -e{{verbose("x")}}
+			set -e
 			[ -n "${{platform._toolchain_env_var}}" ] && . "${{platform._toolchain_env_var}}"
 			{{emit_commands("sh")}}
 		''',
 		'build_{{name}}.bat': '''
 			@rem {{autogenerated}}
 			{{quiet("@echo off")}}
 			if defined {{platform._toolchain_env_var}} call %{{platform._toolchain_env_var}}%
@@ -425,40 +428,40 @@
 				if syntax == 'sh':
 					template = ': ${{{env_var}:={name}}}'
 				elif syntax == 'bat':
 					template = \
 						'if [%{env_var}%] equ [\"\"] set {env_var}=\n' \
 						'if [%{env_var}%] equ [] set {env_var}={name}'
 				else:
-					assert False
+					raise ValueError(f'Shell syntax must be either \'bat\' or \'sh\', not \'{syntax}\'')
 				commands.append(template.format(env_var = env_var, name = name))
 
 			for index, command_tpl in enumerate(self.command_templates):
 				command = render(
 					command_tpl, origin = f'<command#{index + 1}>', syntax = syntax
 				)
 				command = re.sub(r'\s+', ' ', command)
 				if syntax == 'sh':
 					commands.append(command)
 				elif syntax == 'bat':
 					commands.append(command + ' || exit /b')
 				else:
-					assert False
+					raise ValueError(f'Shell syntax must be either \'bat\' or \'sh\', not \'{syntax}\'')
 
 			return '\n'.join(commands)
 
 		@jinja2.pass_context
 		def invoke_tool(context, name: str) -> str:
 			env_var = tool_env_var(name)
 			if context.parent['syntax'] == 'sh':
 				return f'"${env_var}"'
 			elif context.parent['syntax'] == 'bat':
 				return f'%{env_var}%'
 			else:
-				assert False
+				raise ValueError(f'Shell syntax must be either \'bat\' or \'sh\', not \'{context.parent["syntax"]}\'')
 
 		def options(opts: Union[str, Iterable[str]]) -> str:
 			if isinstance(opts, str):
 				return opts
 			else:
 				return ' '.join(opts)
```

### Comparing `torii-0.5.0/torii/build/res.py` & `torii-0.6.0/torii/build/res.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,20 +44,24 @@
 			self.resources[res.name, res.number] = res
 
 	def add_connectors(self, connectors: list[Connector]) -> None:
 		for conn in connectors:
 			if not isinstance(conn, Connector):
 				raise TypeError(f'Object {conn!r} is not a Connector')
 			if (conn.name, conn.number) in self.connectors:
-				raise NameError(f'Trying to add {conn!r}, but {self.connectors[conn.name, conn.number]!r} has the same name and number')
+				raise NameError(
+					f'Trying to add {conn!r}, but {self.connectors[conn.name, conn.number]!r} '
+					'has the same name and number'
+				)
 
 			self.connectors[conn.name, conn.number] = conn
 
 			for conn_pin, plat_pin in conn:
-				assert conn_pin not in self._conn_pins
+				if conn_pin in self._conn_pins:
+					raise ValueError(f'Connector pin {conn_pin!r} already in connector!')
 				self._conn_pins[conn_pin] = plat_pin
 
 	def lookup(self, name: str , number: int = 0) -> Resource:
 		if (name, number) not in self.resources:
 			raise ResourceError(f'Resource {name}#{number} does not exist')
 
 		return self.resources[name, number]
@@ -123,15 +127,17 @@
 			dir: Union[Literal['i', 'o', 'oe', 'io', '-'], dict[str, Literal['i', 'o', 'oe', 'io', '-']]],
 			xdr: Union[int, dict[str, int]],
 			name: str, attrs: Attrs
 		) -> Union[Record, Pin]:
 			for attr_key, attr_value in attrs.items():
 				if hasattr(attr_value, '__call__'):
 					attr_value = attr_value(self)
-					assert attr_value is None or isinstance(attr_value, str)
+					if attr_value is not None or not isinstance(attr_value, str):
+						raise TypeError(f'attr_value is expected to be either a str or None, not \'{attr_value!r}\'')
+
 				if attr_value is None:
 					del attrs[attr_key]
 				else:
 					attrs[attr_key] = attr_value
 
 			if isinstance(resource.ios[0], Subsignal):
 				fields = OrderedDict()
@@ -179,15 +185,15 @@
 
 				if pin is not None and resource.clock is not None:
 					self.add_clock_constraint(pin.i, resource.clock.frequency)
 
 				return pin if pin is not None else port
 
 			else:
-				assert False # :nocov:
+				raise TypeError(f'Expected a Subsignal, Pin, or DiffPairs, not a \'{resource.ios[0]!r}\'') # :nocov:
 
 		value = resolve(
 			resource,
 			*merge_options(resource, dir, xdr),
 			name = f'{resource.name}_{resource.number}',
 			attrs = resource.attrs
 		)
@@ -224,30 +230,30 @@
 					yield port.io
 			elif isinstance(res.ios[0], DiffPairs):
 				if not self.should_skip_port_component(port, attrs, 'p'):
 					yield port.p
 				if not self.should_skip_port_component(port, attrs, 'n'):
 					yield port.n
 			else:
-				assert False
+				raise TypeError(f'Expected either \'Pins\', or \'DiffPairs\', not \'{res.ios[0]!r}\'')
 
 	def iter_port_constraints(self) -> Generator[
 		tuple[str, str, Attrs], None, None
 	]:
 		for res, pin, port, attrs in self._ports:
 			if isinstance(res.ios[0], Pins):
 				if not self.should_skip_port_component(port, attrs, 'io'):
 					yield (port.io.name, res.ios[0].map_names(self._conn_pins, res), attrs)
 			elif isinstance(res.ios[0], DiffPairs):
 				if not self.should_skip_port_component(port, attrs, 'p'):
 					yield (port.p.name, res.ios[0].p.map_names(self._conn_pins, res), attrs)
 				if not self.should_skip_port_component(port, attrs, 'n'):
 					yield (port.n.name, res.ios[0].n.map_names(self._conn_pins, res), attrs)
 			else:
-				assert False
+				raise TypeError(f'Expected either \'Pins\', or \'DiffPairs\', not \'{res.ios[0]!r}\'')
 
 	def iter_port_constraints_bits(self) -> Generator[
 		tuple[str, str, Attrs], None, None
 	]:
 		for port_name, pin_names, attrs in self.iter_port_constraints():
 			if len(pin_names) == 1:
 				yield (port_name, pin_names[0], attrs)
@@ -258,15 +264,17 @@
 	def add_clock_constraint(self, clock: Signal, frequency: Union[int, float]) -> None:
 		if not isinstance(clock, Signal):
 			raise TypeError(f'Object {clock!r} is not a Signal')
 		if not isinstance(frequency, (int, float)):
 			raise TypeError(f'Frequency must be a number, not {frequency!r}')
 
 		if clock in self._clocks:
-			raise ValueError(f'Cannot add clock constraint on {clock!r}, which is already constrained to {self._clocks[clock]} Hz')
+			raise ValueError(
+				f'Cannot add clock constraint on {clock!r}, which is already constrained to {self._clocks[clock]} Hz'
+			)
 
 		else:
 			self._clocks[clock] = float(frequency)
 
 	def iter_clock_constraints(self) -> Generator[
 		tuple[str, Signal, float], None, None
 	]:
```

### Comparing `torii-0.5.0/torii/hdl/__init__.py` & `torii-0.6.0/torii/hdl/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # SPDX-License-Identifier: BSD-2-Clause
 
 from .ast  import (
-	Array, Cat, ClockSignal, Const, Mux, Repl, ResetSignal,
+	Array, Cat, ClockSignal, Const, Mux, ResetSignal,
 	Shape, Signal, Value, signed, unsigned
 )
 from .cd   import ClockDomain
 from .dsl  import Module
 from .ir   import Elaboratable, Fragment, Instance
 from .mem  import Memory
 from .rec  import Record
@@ -22,15 +22,14 @@
 	'EnableInserter',
 	'Fragment',
 	'Instance',
 	'Memory',
 	'Module',
 	'Mux',
 	'Record',
-	'Repl',
 	'ResetInserter',
 	'ResetSignal',
 	'Shape',
 	'Signal',
 	'signed',
 	'unsigned',
 	'Value',
```

### Comparing `torii-0.5.0/torii/hdl/_unused.py` & `torii-0.6.0/torii/hdl/_unused.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 # SPDX-License-Identifier: BSD-2-Clause
 
 from sys      import _getframe, excepthook
 from types    import TracebackType
-from typing   import Optional, Type
+from typing   import Optional, Type, TypeVar
 from warnings import warn_explicit
 
 from ..util   import get_linter_option
 
 __all__ = (
 	'MustUse',
 	'UnusedMustUse',
 )
 
 class UnusedMustUse(Warning):
 	pass
 
+Self = TypeVar('Self', bound = 'MustUse')
 
 class MustUse:
 	_MustUse__silence = False
 	_MustUse__warning = UnusedMustUse
 
-	def __new__(cls, *args, src_loc_at: int = 0, **kwargs) -> 'MustUse':
+	def __new__(cls, *args, src_loc_at: int = 0, **kwargs) -> Self:
 		frame = _getframe(1 + src_loc_at)
 		self = super().__new__(cls)
 		self._MustUse__used    = False
 		self._MustUse__context = dict(
 			filename = frame.f_code.co_filename,
 			lineno   = frame.f_lineno,
 			source   = self
```

### Comparing `torii-0.5.0/torii/hdl/ast.py` & `torii-0.6.0/torii/hdl/ast.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 # SPDX-License-Identifier: BSD-2-Clause
 
 import functools
 import warnings
+import operator
+
 from abc               import ABCMeta, abstractmethod
 from collections       import OrderedDict
 from collections.abc   import (
 	Iterable, MutableMapping, MutableSequence, MutableSet
 )
-from enum              import Enum
+from enum              import Enum, EnumMeta
 from itertools         import chain
 from typing            import Optional, Union
 
 from ..util            import flatten, tracer, union
-from ..util.decorators import final, deprecated
+from ..util.decorators import final
 from ..util.units      import bits_for
 from ._unused          import MustUse, UnusedMustUse
 
 __all__ = (
 	'AnyConst',
 	'AnySeq',
 	'Array',
@@ -31,32 +33,33 @@
 	'Fell',
 	'Initial',
 	'Mux',
 	'Operator',
 	'Part',
 	'Past',
 	'Property',
-	'Repl',
 	'ResetSignal',
 	'Rose',
 	'Sample',
 	'Shape',
 	'ShapeCastable',
+	'ShapeLike',
 	'Signal',
 	'SignalDict',
 	'SignalKey',
 	'SignalSet',
 	'signed',
 	'Slice',
 	'Stable',
 	'Statement',
 	'Switch',
 	'unsigned',
 	'Value',
 	'ValueCastable',
+	'ValueLike',
 	'ValueDict',
 	'ValueKey',
 	'ValueSet',
 )
 
 
 class DUID:
@@ -79,14 +82,16 @@
 
 	'''
 
 	def __init_subclass__(cls, **kwargs):
 		if not hasattr(cls, 'as_shape'):
 			raise TypeError(f'Class \'{cls.__name__}\' deriving from `ShapeCastable` must override the `as_shape` method')
 
+		if not hasattr(cls, 'const'):
+			raise TypeError(f'Class \'{cls.__name__}\' deriving from `ShapeCastable` must override the `const` method')
 
 
 class Shape:
 	'''
 	Bit width and signedness of a value.
 
 	A ``Shape`` can be constructed using:
@@ -163,14 +168,16 @@
 				if len(obj) == 0:
 					return Shape(0)
 				signed = obj[0] < 0 or obj[-1] < 0
 				width  = max(
 					bits_for(obj[0], signed),
 					bits_for(obj[-1], signed)
 				)
+				if obj[0] == obj[-1] == 0:
+					width = 0
 				return Shape(width, signed)
 			elif isinstance(obj, type) and issubclass(obj, Enum):
 				return Shape._cast_plain_enum(obj)
 			else:
 				raise TypeError(f'Object {obj!r} cannot be converted to a Torii shape')
 			if new_obj is obj:
 				raise RecursionError(f'Shape-castable object {obj!r} casts to itself')
@@ -186,39 +193,101 @@
 		if not isinstance(other, Shape):
 			try:
 				other = self.__class__.cast(other)
 			except TypeError as e:
 				raise TypeError(f'Shapes may be compared with shape-castable objects, not {other!r}') from e
 		return self.width == other.width and self.signed == other.signed
 
+class _ShapeLikeMeta(type):
+	def __subclasscheck__(cls, subclass):
+		return (
+			issubclass(subclass, (Shape, ShapeCastable, int, range, EnumMeta)) or
+			subclass is ShapeLike
+		)
+
+	def __instancecheck__(cls, instance):
+		if isinstance(instance, int):
+			return instance >= 0
+		if isinstance(instance, EnumMeta):
+			return all(isinstance(member.value, ValueLike) for member in instance)
+
+		return isinstance(instance, (Shape, ShapeCastable, range))
+
+@final
+class ShapeLike(metaclass = _ShapeLikeMeta):
+	'''
+	An abstract class representing all objects that can be cast to a :class:`Shape`.
+
+	``issubclass(cls, ShapeLike)`` returns ``True`` for:
+
+	- :class:`Shape`
+	- :class:`ShapeCastable` and its subclasses
+	- ``int`` and its subclasses
+	- ``range`` and its subclasses
+	- :class:`enum.EnumMeta` and its subclasses
+	- :class:`ShapeLike` itself
+
+	``isinstance(obj, ShapeLike)`` returns ``True`` for:
+
+	- :class:`Shape` instances
+	- :class:`ShapeCastable` instances
+	- non-negative ``int`` values
+	- ``range`` instances
+	- :class:`enum.Enum` subclasses where all values are :ref:`value-like <lang-valuelike>`
+
+	This class is only usable for the above checks — no instances and no (non-virtual)
+	subclasses can be created.
+	'''
+
+	def __new__(cls, *args, **kwargs):
+		raise TypeError('ShapeLike is an abstract class and cannot be constructed')
+
 
 def unsigned(width: int) -> Shape:
 	''' Shorthand for ``Shape(width, signed = False)``. '''
 	return Shape(width, signed = False)
 
 
 def signed(width: int) -> Shape:
 	''' Shorthand for ``Shape(width, signed = True)``. '''
 	return Shape(width, signed = True)
 
 
 ValueCastType = Union['Value', int, Enum, 'ValueCastable']
 
+def _overridable_by_swapping(method_name: str):
+	'''
+	Allow overriding the decorated method.
+
+	Allows :class:`ValueCastable` to override the decorated method by implementing
+	a reflected method named ``method_name``. Intended for operators, but
+	also usable for other methods that have a reflected counterpart.
+	'''
+	def decorator(f):
+		@functools.wraps(f)
+		def wrapper(self, other):
+			if isinstance(other, ValueCastable) and hasattr(other, method_name):
+				res = getattr(other, method_name)(self)
+				if res is not NotImplemented:
+					return res
+			return f(self, other)
+		return wrapper
+	return decorator
+
 class Value(metaclass = ABCMeta):
 	@staticmethod
-	def cast(obj: ValueCastType ) -> 'Value':
+	def cast(obj: ValueCastType) -> 'Value':
 		'''
 		Converts ``obj`` to an Torii value.
 
 		Booleans and integers are wrapped into a :class:`Const`. Enumerations whose members are
 		all integers are converted to a :class:`Const` with a shape that fits every member.
 		:class:`ValueCastable` objects are recursively cast to an Torii value.
 
 		'''
-
 		while True:
 			if isinstance(obj, Value):
 				return obj
 			elif isinstance(obj, ValueCastable):
 				new_obj = obj.as_value()
 			elif isinstance(obj, Enum):
 				return Const(obj.value, Shape.cast(type(obj)))
@@ -242,106 +311,121 @@
 
 	def __invert__(self) -> 'Operator':
 		return Operator('~', [self])
 
 	def __neg__(self) -> 'Operator':
 		return Operator('-', [self])
 
+	@_overridable_by_swapping('__radd__')
 	def __add__(self, other: ValueCastType) -> 'Operator':
-		return Operator('+', [self, other])
+		return Operator('+', [self, other], src_loc_at = 1)
 
 	def __radd__(self, other: ValueCastType) -> 'Operator':
 		return Operator('+', [other, self])
 
+	@_overridable_by_swapping('__rsub__')
 	def __sub__(self, other: ValueCastType) -> 'Operator':
-		return Operator('-', [self, other])
+		return Operator('-', [self, other], src_loc_at = 1)
 
 	def __rsub__(self, other: ValueCastType) -> 'Operator':
 		return Operator('-', [other, self])
 
-
+	@_overridable_by_swapping('__rmul__')
 	def __mul__(self, other: ValueCastType) -> 'Operator':
-		return Operator('*', [self, other])
+		return Operator('*', [self, other], src_loc_at = 1)
 
 	def __rmul__(self, other: ValueCastType) -> 'Operator':
 		return Operator('*', [other, self])
 
+	@_overridable_by_swapping('__rmod__')
 	def __mod__(self, other: ValueCastType) -> 'Operator':
-		return Operator('%', [self, other])
+		return Operator('%', [self, other], src_loc_at = 1)
 
 	def __rmod__(self, other: ValueCastType) -> 'Operator':
 		return Operator('%', [other, self])
 
+	@_overridable_by_swapping('__rfloordiv__')
 	def __floordiv__(self, other: ValueCastType) -> 'Operator':
-		return Operator('//', [self, other])
+		return Operator('//', [self, other], src_loc_at = 1)
 
 	def __rfloordiv__(self, other: ValueCastType) -> 'Operator':
 		return Operator('//', [other, self])
 
 
 	def __check_shamt(self) -> None:
 		if self.shape().signed:
 			# Neither Python nor HDLs implement shifts by negative values; prohibit any shifts
 			# by a signed value to make sure the shift amount can always be interpreted as
 			# an unsigned value.
 			raise TypeError('Shift amount must be unsigned')
 
+	@_overridable_by_swapping('__rlshift__')
 	def __lshift__(self, other: ValueCastType) -> 'Operator':
 		other = Value.cast(other)
 		other.__check_shamt()
-		return Operator('<<', [self, other])
+		return Operator('<<', [self, other], src_loc_at = 1)
 
 	def __rlshift__(self, other: ValueCastType) -> 'Operator':
 		self.__check_shamt()
 		return Operator('<<', [other, self])
 
+	@_overridable_by_swapping('__rrshift__')
 	def __rshift__(self, other: ValueCastType) -> 'Operator':
 		other = Value.cast(other)
 		other.__check_shamt()
-		return Operator('>>', [self, other])
+		return Operator('>>', [self, other], src_loc_at = 1)
 
 	def __rrshift__(self, other: ValueCastType) -> 'Operator':
 		self.__check_shamt()
 		return Operator('>>', [other, self])
 
+	@_overridable_by_swapping('__rand__')
 	def __and__(self, other: ValueCastType) -> 'Operator':
-		return Operator('&', [self, other])
+		return Operator('&', [self, other], src_loc_at = 1)
 
 	def __rand__(self, other: ValueCastType) -> 'Operator':
 		return Operator('&', [other, self])
 
+	@_overridable_by_swapping('__rxor__')
 	def __xor__(self, other: ValueCastType) -> 'Operator':
-		return Operator('^', [self, other])
+		return Operator('^', [self, other], src_loc_at = 1)
 
 	def __rxor__(self, other: ValueCastType) -> 'Operator':
 		return Operator('^', [other, self])
 
+	@_overridable_by_swapping('__ror__')
 	def __or__(self, other: ValueCastType) -> 'Operator':
-		return Operator('|', [self, other])
+		return Operator('|', [self, other], src_loc_at = 1)
 
 	def __ror__(self, other: ValueCastType) -> 'Operator':
 		return Operator('|', [other, self])
 
+	@_overridable_by_swapping('__eq__')
 	def __eq__(self, other: ValueCastType) -> 'Operator':
-		return Operator('==', [self, other])
+		return Operator('==', [self, other], src_loc_at = 1)
 
+	@_overridable_by_swapping('__ne__')
 	def __ne__(self, other: ValueCastType) -> 'Operator':
-		return Operator('!=', [self, other])
+		return Operator('!=', [self, other], src_loc_at = 1)
 
+	@_overridable_by_swapping('__gt__')
 	def __lt__(self, other: ValueCastType) -> 'Operator':
-		return Operator('<', [self, other])
+		return Operator('<', [self, other], src_loc_at = 1)
 
+	@_overridable_by_swapping('__ge__')
 	def __le__(self, other: ValueCastType) -> 'Operator':
-		return Operator('<=', [self, other])
+		return Operator('<=', [self, other], src_loc_at = 1)
 
+	@_overridable_by_swapping('__lt__')
 	def __gt__(self, other: ValueCastType) -> 'Operator':
-		return Operator('>', [self, other])
+		return Operator('>', [self, other], src_loc_at = 1)
 
+	@_overridable_by_swapping('__le__')
 	def __ge__(self, other: ValueCastType) -> 'Operator':
-		return Operator('>=', [self, other])
+		return Operator('>=', [self, other], src_loc_at = 1)
 
 	def __abs__(self) -> 'Value':
 		if self.shape().signed:
 			return Mux(self >= 0, self, -self)[:len(self)]
 		else:
 			return self
 
@@ -353,21 +437,31 @@
 		if isinstance(key, int):
 			if key not in range(-n, n):
 				raise IndexError(f'Index {key} is out of bounds for a {n}-bit value')
 			if key < 0:
 				key += n
 			return Slice(self, key, key + 1, src_loc_at = 1)
 		elif isinstance(key, slice):
+			if isinstance(key.start, Value) or isinstance(key.stop, Value):
+				raise SyntaxError(
+					'Slicing a value with a Value is unsupported, '
+					'use `Value.bit_select()` or `Value.word_select()` instead.'
+				)
 			start, stop, step = key.indices(n)
 			if step != 1:
 				return Cat(self[i] for i in range(start, stop, step))
 			return Slice(self, start, stop, src_loc_at = 1)
+		elif isinstance(key, Value):
+			raise SyntaxError('Indexing a value with another value is not supported, use `Value.bit_select()` instead.')
 		else:
 			raise TypeError(f'Cannot index value with {key!r}')
 
+	def __contains__(self, _):
+		raise TypeError('The python `in` operator is not supported on Torii values')
+
 	def as_unsigned(self)  -> 'Operator':
 		'''
 		Conversion to unsigned.
 
 		Returns
 		-------
 		Value, out
@@ -383,15 +477,16 @@
 
 		Returns
 		-------
 		Value, out
 			This ``Value`` reinterpreted as a signed integer.
 
 		'''
-
+		if len(self) == 0:
+			raise ValueError('Cannot create a 0-width signed value')
 		return Operator('s', [self])
 
 	def bool(self)  -> 'Operator':
 		'''
 		Conversion to boolean.
 
 		Returns
@@ -523,49 +618,56 @@
 		-------
 		Value, out
 			``1`` if any pattern matches the value, ``0`` otherwise.
 
 		'''
 
 		matches = []
+		# This code should accept exactly the same patterns as `with m.Case(...):`.
 		for pattern in patterns:
-			if not isinstance(pattern, (int, str, Enum)):
-				raise SyntaxError(
-					f'Match pattern must be an integer, a string, or an enumeration, not {pattern!r}'
-				)
-
 			if isinstance(pattern, str) and any(bit not in '01- \t' for bit in pattern):
 				raise SyntaxError(
 					f'Match pattern \'{pattern}\' must consist of 0, 1, and - (don\'t care) bits, and may include whitespace'
 				)
 
 			if (isinstance(pattern, str) and len(''.join(pattern.split())) != len(self)):
 				raise SyntaxError(
 					f'Match pattern \'{pattern}\' must have the same width as match value (which is {len(self)})'
 				)
 
-			if isinstance(pattern, int) and bits_for(pattern) > len(self):
-				warnings.warn(
-					f'Match pattern \'{pattern:b}\' is wider than match value (which has width {len(self)}); '
-					'comparison will never be true',
-					SyntaxWarning, stacklevel = 3
-				)
-				continue
 			if isinstance(pattern, str):
 				pattern = ''.join(pattern.split()) # remove whitespace
 				mask    = int(pattern.replace('0', '1').replace('-', '0'), 2)
 				pattern = int(pattern.replace('-', '0'), 2)
 				matches.append((self & mask) == pattern)
-			elif isinstance(pattern, int):
-				matches.append(self == pattern)
-			elif isinstance(pattern, Enum):
-				matches.append(self == pattern.value)
 			else:
-				assert False
+				orig_pattern = pattern
+				try:
+					pattern = Const.cast(pattern)
+				except TypeError as error:
+					raise SyntaxError(
+						'Match pattern must be a string or a const-castable expression, '
+						f'not {pattern!r}'
+					) from error
+
+				pattern_len = bits_for(pattern.value)
+				if pattern_len > len(self):
+					warnings.warn(
+						f'Match pattern \'{orig_pattern}\' ({pattern_len}\'{pattern.value:b}) is wider than '
+						f'match value (which has width {len(self)}); comparison will never be true',
+						SyntaxWarning, stacklevel = 2
+					)
+					continue
+				matches.append(self == pattern)
+
 		if not matches:
+			warnings.warn(
+				'Value.matches() with an empty patterns clause will return `Const(0)` in a future release.',
+				SyntaxWarning, stacklevel = 2
+			)
 			return Const(1)
 		elif len(matches) == 1:
 			return matches[0]
 		else:
 			return Cat(*matches).any()
 
 	def shift_left(self, amount: int) -> 'Value':
@@ -610,14 +712,16 @@
 		'''
 
 		if not isinstance(amount, int):
 			raise TypeError(f'Shift amount must be an integer, not {amount!r}')
 		if amount < 0:
 			return self.shift_left(-amount)
 		if self.shape().signed:
+			if amount >= len(self):
+				amount = len(self) - 1
 			return self[amount:].as_signed()
 		else:
 			return self[amount:] # unsigned
 
 	def rotate_left(self, amount: int) -> 'Value':
 		'''
 		Rotate left by constant amount.
@@ -681,15 +785,15 @@
 		Value, out
 			Replicated value.
 		'''
 		if not isinstance(count, int) or count < 0:
 			raise TypeError(f'Replication count must be a non-negative integer, not {count!r}')
 		return Cat(self for _ in range(count))
 
-	def eq(self, value: 'Value') -> 'Assign':
+	def eq(self, value: ValueCastType) -> 'Assign':
 		'''
 		Assignment.
 
 		Parameters
 		----------
 		value : Value, in
 			Value to be assigned.
@@ -727,20 +831,22 @@
 	def _lhs_signals(self):
 		raise TypeError(f'Value {self!r} cannot be used in assignments')
 
 	@abstractmethod
 	def _rhs_signals(self):
 		pass # :nocov:
 
-	def _as_const(self):
-		raise TypeError(f'Value {self!r} cannot be evaluated as constant')
-
+class _ConstMeta(ABCMeta):
+	def __call__(cls, value, shape = None, src_loc_at: int = 0, **kwargs):
+		if isinstance(shape, ShapeCastable):
+			return shape.const(value)
+		return super().__call__(value, shape, **kwargs, src_loc_at = src_loc_at + 1)
 
 @final
-class Const(Value):
+class Const(Value, metaclass = _ConstMeta):
 	'''
 	A constant, literal integer value.
 
 	Parameters
 	----------
 	value : int
 	shape : int or tuple or None
@@ -761,80 +867,76 @@
 	def normalize(value: int, shape: tuple[int, bool]):
 		mask = (1 << shape.width) - 1
 		value &= mask
 		if shape.signed and (value >> (shape.width - 1)) & 1:
 			value |= ~mask
 		return value
 
+	@staticmethod
+	def cast(obj):
+		'''
+		Converts ``obj`` to an Torii constant.
+
+		First, ``obj`` is converted to a value using :meth:`Value.cast`. If it is a constant, it
+		is returned. If it is a constant-castable expression, it is evaluated and returned.
+		Otherwise, :exn:`TypeError` is raised.
+		'''
+
+		obj = Value.cast(obj)
+		if type(obj) is Const:
+			return obj
+		elif type(obj) is Cat:
+			value = 0
+			width = 0
+			for part in obj.parts:
+				const  = Const.cast(part)
+				part_value = Const(const.value, unsigned(const.width)).value
+				value |= part_value << width
+				width += len(const)
+			return Const(value, width)
+		elif type(obj) is Slice:
+			value = Const.cast(obj.value)
+			return Const(value.value >> obj.start, unsigned(obj.stop - obj.start))
+		else:
+			raise TypeError(f'Value {obj!r} cannot be converted to an Torii constant')
+
+
 	def __init__(
 		self, value: int, shape: Optional[Union[int, tuple[int, bool]]] = None, *,
 		src_loc_at: int = 0
 	) -> None:
 		# We deliberately do not call Value.__init__ here.
-		self.value = int(value)
+		self.value = int(operator.index(value))
 		if shape is None:
 			shape = Shape(bits_for(self.value), signed = self.value < 0)
 		elif isinstance(shape, int):
 			shape = Shape(shape, signed = self.value < 0)
 		else:
 			if isinstance(shape, range) and self.value == shape.stop:
 				warnings.warn(
 					message =
 						f'Value {self.value!r} equals the non-inclusive end of the constant '
 						f'shape {shape!r}; this is likely an off-by-one error',
 					category = SyntaxWarning,
-					stacklevel = 2
+					stacklevel = 3
 				)
 			shape = Shape.cast(shape, src_loc_at = 1 + src_loc_at)
 		self.width  = shape.width
 		self.signed = shape.signed
 		self.value  = self.normalize(self.value, shape)
 
 	def shape(self) -> Shape:
 		return Shape(self.width, self.signed)
 
 	def _rhs_signals(self) -> 'SignalSet':
 		return SignalSet()
 
-	def _as_const(self) -> int:
-		return self.value
-
 	def __repr__(self) -> str:
 		return f'(const {self.width}\'{"s" if self.signed else ""}d{self.value})'
 
-
-class AnyValue(Value, DUID):
-	def __init__(
-		self, shape: Union[Shape, int, tuple[int, bool], range, type, ShapeCastable] , *,
-		src_loc_at: int = 0
-	) -> None:
-		super().__init__(src_loc_at = src_loc_at)
-		shape = Shape.cast(shape, src_loc_at = 1 + src_loc_at)
-		self.width  = shape.width
-		self.signed = shape.signed
-
-	def shape(self) -> Shape:
-		return Shape(self.width, self.signed)
-
-	def _rhs_signals(self) -> 'SignalSet':
-		return SignalSet()
-
-
-@final
-class AnyConst(AnyValue):
-	def __repr__(self) -> str:
-		return f'(anyconst {self.width}\'{"s" if self.signed else ""})'
-
-
-@final
-class AnySeq(AnyValue):
-	def __repr__(self) -> str:
-		return f'(anyseq {self.width}\'{"s" if self.signed else ""})'
-
-
 @final
 class Operator(Value):
 	def __init__(self, operator, operands , *, src_loc_at = 0) -> None:
 		super().__init__(src_loc_at = 1 + src_loc_at)
 		self.operator = operator
 		self.operands = [Value.cast(op) for op in operands]
 
@@ -881,18 +983,22 @@
 			if self.operator == '%':
 				return Shape(b_shape.width, b_shape.signed)
 			if self.operator in ('<', '<=', '==', '!=', '>', '>='):
 				return Shape(1, False)
 			if self.operator in ('&', '^', '|'):
 				return _bitwise_binary_shape(*op_shapes)
 			if self.operator == '<<':
-				assert not b_shape.signed
+				if b_shape.signed:
+					raise TypeError('Operator << operand must be unsigned!')
+
 				return Shape(a_shape.width + 2 ** b_shape.width - 1, a_shape.signed)
 			if self.operator == '>>':
-				assert not b_shape.signed
+				if b_shape.signed:
+					raise TypeError('Operator >> operand must be unsigned!')
+
 				return Shape(a_shape.width, a_shape.signed)
 		elif len(op_shapes) == 3:
 			if self.operator == 'm':
 				s_shape, a_shape, b_shape = op_shapes
 				return _bitwise_binary_shape(a_shape, b_shape)
 		raise NotImplementedError(f'Operator {self.operator}/{len(op_shapes)} not implemented') # :nocov:
 
@@ -951,16 +1057,16 @@
 		if stop < 0:
 			stop += n
 		if start > stop:
 			raise IndexError(f'Slice start {start} must be less than slice stop {stop}')
 
 		super().__init__(src_loc_at = src_loc_at)
 		self.value = value
-		self.start = int(start)
-		self.stop  = int(stop)
+		self.start = int(operator.index(start))
+		self.stop  = int(operator.index(stop))
 
 	def shape(self) -> Shape:
 		return Shape(self.stop - self.start)
 
 	def _lhs_signals(self):
 		return self.value._lhs_signals()
 
@@ -1030,15 +1136,15 @@
 	Returns
 	-------
 	Value, inout
 		Resulting ``Value`` obtained by concatenation.
 
 	'''
 
-	def __init__(self, *args: Iterable[Value], src_loc_at: int = 0) -> None:
+	def __init__(self, *args: ValueCastType, src_loc_at: int = 0) -> None:
 		super().__init__(src_loc_at = src_loc_at)
 		self.parts = []
 		for index, arg in enumerate(flatten(args)):
 			if isinstance(arg, Enum) and (not isinstance(type(arg), ShapeCastable) or
 				not hasattr(arg, '_torii_shape_')
 			):
 				warnings.warn(
@@ -1061,58 +1167,18 @@
 
 	def _lhs_signals(self):
 		return union((part._lhs_signals() for part in self.parts), start = SignalSet())
 
 	def _rhs_signals(self):
 		return union((part._rhs_signals() for part in self.parts), start = SignalSet())
 
-	def _as_const(self) -> int:
-		value = 0
-		for part in reversed(self.parts):
-			value <<= len(part)
-			value |= part._as_const()
-		return value
-
 	def __repr__(self) -> str:
 		return f'(cat {" ".join(map(repr, self.parts))})'
 
 
-@deprecated('instead of `Repl(value, count)`, use `value.replicate(count)`')
-def Repl(value: ValueCastType, count: int):
-	'''
-	Replicate a value
-
-	An input value is replicated (repeated) several times
-	to be used on the RHS of assignments::
-
-		len(Repl(s, n)) == len(s) * n
-
-	Parameters
-	----------
-	value : Value, in
-		Input value to be replicated.
-	count : int
-		Number of replications.
-
-	Returns
-	-------
-	Value, out
-		Replicated value.
-
-	'''
-	if isinstance(value, int) and value not in [0, 1]:
-		warnings.warn(
-			f'Value argument of Repl() is a bare integer {value} used in bit vector '
-			f'context; consider specifying explicit width using Const({value}, {bits_for(value)}) instead',
-			SyntaxWarning, stacklevel = 3
-		)
-
-	return Value.cast(value).replicate(count)
-
-
 # @final
 class Signal(Value, DUID):
 	'''
 	A varying integer value.
 
 	Parameters
 	----------
@@ -1150,15 +1216,15 @@
 	reset_less : bool
 	attrs : dict
 	decoder : function
 
 	'''
 
 	def __init__(
-		self, shape = None, *, name = None, reset = 0, reset_less = False,
+		self, shape = None, *, name = None, reset = None, reset_less = False,
 		attrs = None, decoder = None, src_loc_at = 0
 	):
 		super().__init__(src_loc_at = src_loc_at)
 
 		if name is not None and not isinstance(name, str):
 			raise TypeError(f'Name must be a string, not {name!r}')
 		self.name = name or tracer.get_var_name(depth = 2 + src_loc_at, default = '$signal')
@@ -1168,23 +1234,37 @@
 			shape = unsigned(1)
 		else:
 			shape = Shape.cast(shape, src_loc_at = 1 + src_loc_at)
 		self.width  = shape.width
 		self.signed = shape.signed
 
 		orig_reset = reset
-		try:
-			reset = Const.cast(reset)
-		except TypeError:
-			raise TypeError(
-				f'Reset value must be a constant-castable expression, not {orig_reset!r}'
-			)
+		if isinstance(orig_shape, ShapeCastable):
+			try:
+				reset = Const.cast(orig_shape.const(reset))
+			except Exception:
+				raise TypeError(
+					f'Reset value must be a constant initializer of {orig_shape!r}'
+				)
+
+			if reset.shape() != Shape.cast(orig_shape):
+				raise ValueError(
+					f'Constant returned by {orig_shape!r}.const() must have the shape that it casts '
+					f'to, {Shape.cast(orig_shape)!r}, and not {reset.shape()!r}'
+				)
+		else:
+			try:
+				reset = Const.cast(reset or 0)
+			except TypeError:
+				raise TypeError(
+					f'Reset value must be a constant-castable expression, not {orig_reset!r}'
+				)
 
 		# Avoid false positives for all-zeroes and all-ones
-		if orig_reset not in (0, -1):
+		if orig_reset not in (None, 0, -1):
 			if reset.shape().signed and not self.signed:
 				warnings.warn(
 					message = f'Reset value {orig_reset!r} is signed, but the signal shape is {shape!r}',
 					category = SyntaxWarning,
 					stacklevel = 2
 				)
 			elif (
@@ -1196,22 +1276,22 @@
 					message = f'Reset value {orig_reset!r} will be truncated to the signal shape {shape!r}',
 					category = SyntaxWarning,
 					stacklevel = 2
 				)
 		self.reset = reset.value
 		self.reset_less = bool(reset_less)
 
-		if isinstance(orig_shape, range) and self.reset == orig_shape.stop:
-			warnings.warn(
-				message =
-					f'Reset value {self.reset!r} equals the non-inclusive end of the signal '
+		if isinstance(orig_shape, range) and orig_reset is not None and orig_reset not in orig_shape:
+			if orig_reset == orig_shape.stop:
+				raise SyntaxError(
+					f'Reset value {orig_reset!r} equals the non-inclusive end of the signal '
 					f'shape {orig_shape!r}; this is likely an off-by-one error',
-				category = SyntaxWarning,
-				stacklevel = 2
-			)
+				)
+			else:
+				raise SyntaxError(f'Reset value {orig_reset!r} is not within the signal shape {orig_shape!r}')
 
 		self.attrs = OrderedDict(() if attrs is None else attrs)
 
 		if decoder is None and isinstance(orig_shape, type) and issubclass(orig_shape, Enum):
 			decoder = orig_shape
 		if isinstance(decoder, type) and issubclass(decoder, Enum):
 			def enum_decoder(value):
@@ -1344,14 +1424,46 @@
 	def _rhs_signals(self) -> None:
 		raise NotImplementedError('ResetSignal must be lowered to a concrete signal') # :nocov:
 
 	def __repr__(self) -> str:
 		return f'(rst {self.domain})'
 
 
+@final
+class AnyValue(Value, DUID):
+	class Kind(Enum):
+		AnyConst = 'anyconst'
+		AnySeq   = 'anyseq'
+
+	def __init__(self, kind: str, shape: ShapeCastable, *, src_loc_at: int = 0) -> None:
+		super().__init__(src_loc_at = src_loc_at)
+
+		self.kind   = self.Kind(kind)
+		# XXX(aki): Why the hecc are we not just caching the shape if we
+		# are re-creating it for the `shape()` call anyway???
+		shape       = Shape.cast(shape, src_loc_at = src_loc_at + 1)
+		self.width  = shape.width
+		self.signed = shape.signed
+
+	def shape(self):
+		return Shape(self.width, self.signed)
+
+	def _rhs_signals(self):
+		return SignalSet()
+
+	def __repr__(self) -> str:
+		return f'({self.kind.value} {self.width}\'{"s" if self.signed else ""})'
+
+
+def AnyConst(shape, *, src_loc_at: int = 0) -> AnyValue:
+	return AnyValue('anyconst', shape, src_loc_at = src_loc_at + 1)
+
+def AnySeq(shape, *, src_loc_at: int = 0) -> AnyValue:
+	return AnyValue('anyseq', shape, src_loc_at = src_loc_at + 1)
+
 class Array(MutableSequence):
 	'''
 	Addressable multiplexer.
 
 	An array is similar to a ``list`` that can also be indexed by ``Value``s;
 	indexing by an integer or a slice works the same as for Python lists,
 	but indexing by a ``Value`` results in a proxy.
@@ -1403,14 +1515,16 @@
 
 	def __init__(self, iterable = ()):
 		self._inner    = list(iterable)
 		self._proxy_at = None
 		self._mutable  = True
 
 	def __getitem__(self, index):
+		if isinstance(index, ValueCastable):
+			index = Value.cast(index)
 		if isinstance(index, Value):
 			if self._mutable:
 				self._proxy_at = tracer.get_src_loc()
 				self._mutable  = False
 			return ArrayProxy(self, index)
 		else:
 			return self._inner[index]
@@ -1545,14 +1659,50 @@
 			if '_ValueCastable__lowered_to' not in self.__dict__:
 				self.__lowered_to = func(self, *args, **kwargs)
 			return self.__lowered_to
 		wrapper_memoized.__memoized = True
 		return wrapper_memoized
 
 
+class _ValueLikeMeta(type):
+	'''
+	An abstract class representing all objects that can be cast to a :class:`Value`.
+
+	``issubclass(cls, ValueLike)`` returns ``True`` for:
+
+	- :class:`Value`
+	- :class:`ValueCastable` and its subclasses
+	- ``int`` and its subclasses
+	- :class:`enum.Enum` subclasses where all values are :ref:`value-like <lang-valuelike>`
+	- :class:`ValueLike` itself
+
+	``isinstance(obj, ValueLike)`` returns the same value as ``issubclass(type(obj), ValueLike)``.
+
+	This class is only usable for the above checks — no instances and no (non-virtual)
+	subclasses can be created.
+	'''
+
+	def __subclasscheck__(cls, subclass):
+		if issubclass(subclass, Enum):
+			return isinstance(subclass, ShapeLike)
+
+		return (
+			issubclass(subclass, (Value, ValueCastable, int)) or
+			subclass is ValueLike
+		)
+
+	def __instancecheck__(cls, instance):
+		return issubclass(type(instance), cls)
+
+
+@final
+class ValueLike(metaclass = _ValueLikeMeta):
+	def __new__(cls, *args, **kwargs):
+		raise TypeError('ValueLike is an abstract class and cannot be constructed')
+
 @final
 class Sample(Value):
 	'''
 	Value from the past.
 
 	A ``Sample`` of an expression is equal to the value of the expression ``clocks`` clock edges
 	of the ``domain`` clock back. If that moment is before the beginning of time, it is equal
@@ -1657,61 +1807,64 @@
 		return f'(eq {self.lhs!r} {self.rhs!r})'
 
 
 class UnusedProperty(UnusedMustUse):
 	pass
 
 
+@final
 class Property(Statement, MustUse):
 	_MustUse__warning = UnusedProperty
 
+	class Kind(Enum):
+		Assert = 'assert'
+		Assume = 'assume'
+		Cover  = 'cover'
+
+
 	def __init__(
-		self, test: ValueCastType, *, _check: Optional[Signal] = None, _en: Optional[Signal] = None,
+		self, kind: str, test: ValueCastType, *, _check: Optional[Signal] = None, _en: Optional[Signal] = None,
 		name: Optional[str] = None, src_loc_at: int = 0
 	) -> None:
 		super().__init__(src_loc_at = src_loc_at)
+		self.kind   = self.Kind(kind)
 		self.test   = Value.cast(test)
 		self._check = _check
 		self._en    = _en
 		self.name   = name
 		if not isinstance(self.name, str) and self.name is not None:
 			raise TypeError(f'Property name must be a string of None, not {self.name!r}')
 
 		if self._check is None:
-			self._check = Signal(reset_less = True, name = f'${self._kind}$check')
+			self._check = Signal(reset_less = True, name = f'${self.kind.value}$check')
 			self._check.src_loc = self.src_loc
 		if _en is None:
-			self._en = Signal(reset_less = True, name = f'${self._kind}$en')
+			self._en = Signal(reset_less = True, name = f'${self.kind.value}$en')
 			self._en.src_loc = self.src_loc
 
 	def _lhs_signals(self):
 		return SignalSet((self._en, self._check))
 
 	def _rhs_signals(self):
 		return self.test._rhs_signals()
 
 	def __repr__(self) -> str:
 		if self.name is not None:
-			return f'({self.name}: {self._kind} {self.test!r})'
-		return f'({self._kind} {self.test!r})'
+			return f'({self.name}: {self.kind.value} {self.test!r})'
+		return f'({self.kind.value} {self.test!r})'
 
 
-@final
-class Assert(Property):
-	_kind = 'assert'
+def Assert(test: ValueCastType, *, name: str | None = None, src_loc_at: int = 0) -> Property:
+	return Property('assert', test, name = name, src_loc_at = src_loc_at + 1)
 
+def Assume(test: ValueCastType, *, name: str | None = None, src_loc_at: int = 0) -> Property:
+	return Property('assume', test, name = name, src_loc_at = src_loc_at + 1)
 
-@final
-class Assume(Property):
-	_kind = 'assume'
-
-
-@final
-class Cover(Property):
-	_kind = 'cover'
+def Cover(test: ValueCastType, *, name: str | None = None, src_loc_at: int = 0) -> Property:
+	return Property('cover', test, name = name, src_loc_at = src_loc_at + 1)
 
 
 # @final
 class Switch(Statement):
 	def __init__(self, test, cases, *, src_loc = None, src_loc_at = 0, case_src_locs = {}):
 		if src_loc is None:
 			super().__init__(src_loc_at = src_loc_at)
@@ -1733,22 +1886,27 @@
 			if not isinstance(keys, tuple):
 				keys = (keys,)
 			# Map: 2 -> "0010"; "0010" -> "0010"
 			new_keys = ()
 			key_mask = (1 << len(self.test)) - 1
 			for key in keys:
 				if isinstance(key, str):
-					key = "".join(key.split()) # remove whitespace
+					key = ''.join(key.split()) # remove whitespace
 				elif isinstance(key, int):
 					key = format(key & key_mask, 'b').rjust(len(self.test), '0')
+					if key_mask == 0:
+						key = ''
 				elif isinstance(key, Enum):
 					key = format(key.value & key_mask, 'b').rjust(len(self.test), '0')
+					if key_mask == 0:
+						key = ''
 				else:
 					raise TypeError(f'Object {key!r} cannot be used as a switch key')
-				assert len(key) == len(self.test)
+				if len(key) != len(self.test):
+					raise ValueError(f'Length mismatch between switch key and test value {len(key)} != {len(self.test)}')
 				new_keys = (*new_keys, key)
 			if not isinstance(stmts, Iterable):
 				stmts = [stmts]
 			self.cases[new_keys] = Statement.cast(stmts)
 			if orig_keys in case_src_locs:
 				self.case_src_locs[new_keys] = case_src_locs[orig_keys]
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `torii-0.5.0/torii/hdl/cd.py` & `torii-0.6.0/torii/hdl/cd.py`

 * *Files identical despite different names*

### Comparing `torii-0.5.0/torii/hdl/dsl.py` & `torii-0.6.0/torii/hdl/dsl.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,20 +2,23 @@
 
 import warnings
 from collections  import OrderedDict
 from contextlib   import _GeneratorContextManager, contextmanager
 from enum         import Enum
 from functools    import wraps
 from sys          import version_info
+from typing       import (
+	Callable, Generator, ParamSpec, Any, Iterable, Optional, TypedDict, Union, TYPE_CHECKING
+)
 
 from ..util       import flatten, tracer
 from ..util.units import bits_for
 from .ast         import (
-	Assert, Assign, Assume, Cat, Cover, Operator, Signal, SignalDict,
-	Statement, Switch, Value
+	Assign, Cat, Const, Operator, Property, Signal, SignalDict, Statement, Switch, Value,
+	_StatementList, ValueCastType
 )
 from .cd          import ClockDomain
 from .ir          import Elaboratable, Fragment
 from .xfrm        import SampleDomainInjector
 
 __all__ = (
 	'Module',
@@ -29,31 +32,34 @@
 
 
 class SyntaxWarning(Warning):
 	pass
 
 
 class _ModuleBuilderProxy:
-	def __init__(self, builder, depth):
+	_builder: 'Module'
+	_depth: int
+
+	def __init__(self, builder: 'Module', depth: int):
 		object.__setattr__(self, '_builder', builder)
 		object.__setattr__(self, '_depth', depth)
 
 
 class _ModuleBuilderDomain(_ModuleBuilderProxy):
-	def __init__(self, builder, depth, domain):
+	def __init__(self, builder: 'Module', depth: int, domain: Optional[str]):
 		super().__init__(builder, depth)
 		self._domain = domain
 
 	def __iadd__(self, assigns):
 		self._builder._add_statement(assigns, domain = self._domain, depth = self._depth)
 		return self
 
 
 class _ModuleBuilderDomains(_ModuleBuilderProxy):
-	def __getattr__(self, name):
+	def __getattr__(self, name: str):
 		if name == 'submodules':
 			warnings.warn(
 				f'Using \'<module>.d.{name}\' would add statements to clock domain {name!r}; '
 				f'did you mean <module>.{name} instead?',
 				SyntaxWarning, stacklevel = 2
 			)
 		if name == 'comb':
@@ -72,26 +78,28 @@
 			raise AttributeError(f'Cannot assign \'d.{name}\' attribute; did you mean \'d.{name} +=\'?')
 
 	def __setitem__(self, name, value):
 		return self.__setattr__(name, value)
 
 
 class _ModuleBuilderRoot:
-	def __init__(self, builder, depth):
+	def __init__(self, builder: 'Module', depth: int):
 		self._builder = builder
 		self.domain = self.d = _ModuleBuilderDomains(builder, depth)
 
 	def __getattr__(self, name):
 		if name in ('comb', 'sync'):
 			raise AttributeError(f'\'{type(self).__name__}\' object has no attribute \'{name}\'; did you mean \'d.{name}\'?')
 		raise AttributeError(f'\'{type(self).__name__}\' object has no attribute \'{name}\'')
 
 
 class _ModuleBuilderSubmodules:
-	def __init__(self, builder):
+	_builder: 'Module'
+
+	def __init__(self, builder: 'Module'):
 		object.__setattr__(self, '_builder', builder)
 
 	def __iadd__(self, modules):
 		for module in flatten([modules]):
 			self._builder._add_submodule(module)
 		return self
 
@@ -105,80 +113,110 @@
 		return self._builder._get_submodule(name)
 
 	def __getitem__(self, name):
 		return self.__getattr__(name)
 
 
 class _ModuleBuilderDomainSet:
-	def __init__(self, builder):
+	_builder: 'Module'
+
+	def __init__(self, builder: 'Module'):
 		object.__setattr__(self, '_builder', builder)
 
-	def __iadd__(self, domains):
+	def __iadd__(self, domains: Iterable):
 		for domain in flatten([domains]):
 			if not isinstance(domain, ClockDomain):
 				raise TypeError(f'Only clock domains may be added to `m.domains`, not {domain!r}')
 			self._builder._add_domain(domain)
 		return self
 
 	def __setattr__(self, name, domain):
 		if not isinstance(domain, ClockDomain):
 			raise TypeError(f'Only clock domains may be added to `m.domains`, not {domain!r}')
 		if domain.name != name:
 			raise NameError(f'Clock domain name {domain.name!r} must match name in `m.domains.{name} += ...` syntax')
 		self._builder._add_domain(domain)
 
+Params = ParamSpec('Params')
 
 # It's not particularly clean to depend on an internal interface, but, unfortunately, __bool__
 # must be defined on a class to be called during implicit conversion.
 class _GuardedContextManager(_GeneratorContextManager):
-	def __init__(self, keyword, func, args, kwds):
+	def __init__(self, keyword: str, func: Callable[Params, Generator[Any, Any, None]], args: tuple, kwds: dict):
 		self.keyword = keyword
 		return super().__init__(func, args, kwds)
 
 	def __bool__(self):
 		raise SyntaxError(f'`if m.{self.keyword}(...):` does not work; use `with m.{self.keyword}(...)`')
 
-
-def _guardedcontextmanager(keyword):
-	def decorator(func):
+def _guardedcontextmanager(keyword: str):
+	def decorator(func: Callable[Params, Generator[Any, Any, None]]) -> Callable[Params, _GeneratorContextManager]:
 		@wraps(func)
-		def helper(*args, **kwds):
+		def helper(*args: Params.args, **kwds: Params.kwargs):
 			return _GuardedContextManager(keyword, func, args, kwds)
 		return helper
 	return decorator
 
-
 class FSM:
 	def __init__(self, state, encoding, decoding):
 		self.state    = state
 		self.encoding = encoding
 		self.decoding = decoding
 
 	def ongoing(self, name):
 		if name not in self.encoding:
 			self.encoding[name] = len(self.encoding)
 		return Operator('==', [ self.state, self.encoding[name] ], src_loc_at = 0)
 
+_SrcLoc = tuple[str, int]
+_Pattern = Union[int, str, Enum]
+_PatternTuple = tuple[_Pattern, ...]
+
+class _IfDict(TypedDict):
+	depth: int
+	tests: list
+	bodies: list
+	src_loc: _SrcLoc
+	src_locs: list[_SrcLoc]
+
+class _SwitchDict(TypedDict):
+	test: Value
+	cases: OrderedDict[_PatternTuple, _StatementList]
+	src_loc: _SrcLoc
+	case_src_locs: dict[_PatternTuple, _SrcLoc]
+
+class _FSMDict(TypedDict):
+	name: str
+	signal: Signal
+	reset: Optional[str]
+	domain: str
+	encoding: OrderedDict
+	decoding: OrderedDict
+	states: OrderedDict
+	src_loc: _SrcLoc
+	state_src_locs: dict[str, _SrcLoc]
+
+_CtrlEntry = Union[_IfDict, _SwitchDict, _FSMDict]
 
 class Module(_ModuleBuilderRoot, Elaboratable):
 	@classmethod
 	def __init_subclass__(cls):
 		raise SyntaxError(
 			'Instead of inheriting from `Module`, inherit from `Elaboratable` '
 			'and return a `Module` from the `elaborate(self, platform)` method'
 		)
 
 	def __init__(self):
-		_ModuleBuilderRoot.__init__(self, self, depth = 0)
+		super().__init__(builder = self, depth = 0)
 		self.submodules    = _ModuleBuilderSubmodules(self)
 		self.domains       = _ModuleBuilderDomainSet(self)
 
 		self._statements   = Statement.cast([])
 		self._ctrl_context = None
-		self._ctrl_stack   = []
+		self._ctrl_stack : list[tuple[str, _CtrlEntry]]  = []
 
 		self._driving      = SignalDict()
 		self._named_submodules = {}
 		self._anon_submodules  = []
 		self._domains      = {}
 		self._generated    = {}
 
@@ -192,76 +230,82 @@
 				if self._ctrl_context == 'FSM':
 					secondary_context = 'State'
 				raise SyntaxError(
 					f'{construct} is not permitted directly inside of {self._ctrl_context}; '
 					f'it is permitted inside of {self._ctrl_context} {secondary_context}'
 				)
 
-	def _get_ctrl(self, name):
+	def _get_ctrl(self, name: str):
 		if self._ctrl_stack:
 			top_name, top_data = self._ctrl_stack[-1]
 			if top_name == name:
 				return top_data
 
 	def _flush_ctrl(self):
 		while len(self._ctrl_stack) > self.domain._depth:
 			self._pop_ctrl()
 
-	def _set_ctrl(self, name, data):
+	def _set_ctrl(self, name: str, data: _CtrlEntry):
 		self._flush_ctrl()
 		self._ctrl_stack.append((name, data))
 		return data
 
-	def _check_signed_cond(self, cond):
+	def _check_signed_cond(self, cond: ValueCastType):
 		cond = Value.cast(cond)
 		if version_info < (3, 12, 0) and cond.shape().signed:
 			# TODO(py3.11): remove; ~True is a warning in 3.12+, finally!
 			warnings.warn(
 				'Signed values in If/Elif conditions usually result from inverting '
 				'Python booleans with ~, which leads to unexpected results. '
 				'Replace `~flag` with `not flag`. (If this is a false positive, '
 				'silence this warning with `m.If(x)` → `m.If(x.bool())`.)',
 				SyntaxWarning, stacklevel = 4
 			)
 		return cond
 
 	@_guardedcontextmanager('If')
-	def If(self, cond):
+	def If(self, cond: ValueCastType):
 		self._check_context('If', context = None)
 		cond = self._check_signed_cond(cond)
 		src_loc = tracer.get_src_loc(src_loc_at = 1)
 		if_data = self._set_ctrl('If', {
 			'depth'   : self.domain._depth,
 			'tests'   : [],
 			'bodies'  : [],
 			'src_loc' : src_loc,
 			'src_locs': [],
 		})
+		if TYPE_CHECKING:
+			assert isinstance(if_data, _IfDict)
+		_outer_case = self._statements
 		try:
-			_outer_case, self._statements = self._statements, []
+			self._statements = Statement.cast([])
 			self.domain._depth += 1
 			yield
 			self._flush_ctrl()
 			if_data['tests'].append(cond)
 			if_data['bodies'].append(self._statements)
 			if_data['src_locs'].append(src_loc)
 		finally:
 			self.domain._depth -= 1
 			self._statements = _outer_case
 
 	@_guardedcontextmanager('Elif')
-	def Elif(self, cond):
+	def Elif(self, cond: ValueCastType):
 		self._check_context('Elif', context = None)
 		cond = self._check_signed_cond(cond)
 		src_loc = tracer.get_src_loc(src_loc_at = 1)
 		if_data = self._get_ctrl('If')
+		if TYPE_CHECKING:
+			assert if_data is None or isinstance(if_data, _IfDict)
 		if if_data is None or if_data['depth'] != self.domain._depth:
 			raise SyntaxError('Elif without preceding If')
+		_outer_case = self._statements
 		try:
-			_outer_case, self._statements = self._statements, []
+			self._statements = Statement.cast([])
 			self.domain._depth += 1
 			yield
 			self._flush_ctrl()
 			if_data['tests'].append(cond)
 			if_data['bodies'].append(self._statements)
 			if_data['src_locs'].append(src_loc)
 		finally:
@@ -269,18 +313,21 @@
 			self._statements = _outer_case
 
 	@_guardedcontextmanager('Else')
 	def Else(self):
 		self._check_context('Else', context = None)
 		src_loc = tracer.get_src_loc(src_loc_at = 1)
 		if_data = self._get_ctrl('If')
+		if TYPE_CHECKING:
+			assert if_data is None or isinstance(if_data, _IfDict)
 		if if_data is None or if_data['depth'] != self.domain._depth:
 			raise SyntaxError('Else without preceding If/Elif')
+		_outer_case = self._statements
 		try:
-			_outer_case, self._statements = self._statements, []
+			self._statements = Statement.cast([])
 			self.domain._depth += 1
 			yield
 			self._flush_ctrl()
 			if_data['bodies'].append(self._statements)
 			if_data['src_locs'].append(src_loc)
 		finally:
 			self.domain._depth -= 1
@@ -303,80 +350,132 @@
 		finally:
 			self.domain._depth -= 1
 			self._ctrl_context = None
 		self._pop_ctrl()
 
 	@contextmanager
 	def Case(self, *patterns):
+		if not patterns:
+			raise ValueError('Empty Case() clauses have been superseded by Default()')
+
 		self._check_context('Case', context = 'Switch')
 		src_loc = tracer.get_src_loc(src_loc_at = 1)
 		switch_data = self._get_ctrl('Switch')
-		new_patterns = ()
+		if TYPE_CHECKING:
+			assert switch_data is None or isinstance(switch_data, _SwitchDict)
+		if switch_data is None:
+			raise SyntaxError('Case outside of Switch block')
+		new_patterns: _PatternTuple = ()
+		if () in switch_data['cases']:
+			warnings.warn(
+				'Case statements are order-dependant, any Case after a Default will be ignored',
+				SyntaxWarning, stacklevel = 3
+			)
+
+		# This code should accept exactly the same patterns as `v.matches(...)`.
 		for pattern in patterns:
-			if not isinstance(pattern, (int, str, Enum)):
-				raise SyntaxError(f'Case pattern must be an integer, a string, or an enumeration, not {pattern!r}')
 			if isinstance(pattern, str) and any(bit not in '01- \t' for bit in pattern):
 				raise SyntaxError(
 					f'Case pattern \'{pattern}\' must consist of 0, 1, and - (don\'t care) bits, and may '
 					'include whitespace'
 				)
 			if (isinstance(pattern, str) and
 					len("".join(pattern.split())) != len(switch_data['test'])):
 				raise SyntaxError(
 					f'Case pattern \'{pattern}\' must have the same width as switch value '
 					f'(which is {len(switch_data["test"])})'
 				)
-			if isinstance(pattern, int) and bits_for(pattern) > len(switch_data["test"]):
-				warnings.warn(
-					f'Case pattern \'{pattern:b}\' is wider than switch value (which has width {len(switch_data["test"])}); '
-					'comparison will never be true', SyntaxWarning, stacklevel = 3
-				)
-				continue
-			if isinstance(pattern, Enum) and bits_for(pattern.value) > len(switch_data["test"]):
-				warnings.warn(
-					f'Case pattern \'{pattern.value:b}\' ({ pattern.__class__.__name__}.{pattern.name}) is wider than switch value '
-					f'(which has width {len(switch_data["test"])}); comparison will never be true',
-					SyntaxWarning, stacklevel = 3
-				)
-				continue
-			new_patterns = (*new_patterns, pattern)
+			if isinstance(pattern, str):
+				new_patterns = (*new_patterns, pattern)
+			else:
+				orig_pattern = pattern
+				try:
+					pattern = Const.cast(pattern)
+				except TypeError as error:
+					raise SyntaxError(
+						'Case pattern must be a string or a const-castable expression, '
+						f'not {pattern!r}'
+					) from error
+
+				pattern_len = bits_for(pattern.value)
+				if pattern.value == 0:
+					pattern_len = 0
+				if pattern_len > len(switch_data['test']):
+					warnings.warn(
+						f'Case pattern \'{orig_pattern!r}\' ({pattern_len}\'{pattern.value:b}) is wider than '
+						f'switch value (which has width {len(switch_data["test"])}); comparison will never be true',
+						SyntaxWarning, stacklevel = 2
+					)
+					continue
+				new_patterns = (*new_patterns, pattern.value)
+		_outer_case = self._statements
 		try:
-			_outer_case, self._statements = self._statements, []
+			self._statements = Statement.cast([])
 			self._ctrl_context = None
 			yield
 			self._flush_ctrl()
 			# If none of the provided cases can possibly be true, omit this branch completely.
 			# This needs to be differentiated from no cases being provided in the first place,
 			# which means the branch will always match.
-			if not (patterns and not new_patterns):
+			# Likewise, omit this branch if another branch with this exact set of patterns already
+			# exists (since otherwise we'd overwrite the previous branch's slot in the dict).
+			if not (patterns and not new_patterns) and new_patterns not in switch_data['cases']:
 				switch_data['cases'][new_patterns] = self._statements
 				switch_data['case_src_locs'][new_patterns] = src_loc
 		finally:
 			self._ctrl_context = 'Switch'
 			self._statements = _outer_case
 
+	@contextmanager
 	def Default(self):
-		return self.Case()
+		self._check_context('Default', context = 'Switch')
+		src_loc = tracer.get_src_loc(src_loc_at = 1)
+		switch_data = self._get_ctrl('Switch')
+		if () in switch_data['cases']:
+			raise SyntaxError(
+				'Multiple Default statements within a switch are not allowed, '
+				'as only the first Default will ever be considered.',
+			)
+
+		if TYPE_CHECKING:
+			assert switch_data is None or isinstance(switch_data, _SwitchDict)
+		if switch_data is None:
+			raise SyntaxError('Default outside of Switch block')
+
+		_outer_case = self._statements
+		try:
+			self._statements = Statement.cast([])
+			self._ctrl_context = None
+			yield
+			self._flush_ctrl()
+			if () not in switch_data['cases']:
+				switch_data['cases'][()] = self._statements
+				switch_data['case_src_locs'][()] = src_loc
+		finally:
+			self._ctrl_context = 'Switch'
+			self._statements = _outer_case
 
 	@contextmanager
-	def FSM(self, reset = None, domain = 'sync', name = 'fsm'):
+	def FSM(self, reset: Optional[str] = None, domain = 'sync', name = 'fsm'):
 		self._check_context('FSM', context = None)
 		if domain == 'comb':
 			raise ValueError(f'FSM may not be driven by the \'{domain}\' domain')
 		fsm_data = self._set_ctrl('FSM', {
 			'name'          : name,
 			'signal'        : Signal(name = f'{name}_state', src_loc_at = 2),
 			'reset'         : reset,
 			'domain'        : domain,
 			'encoding'      : OrderedDict(),
 			'decoding'      : OrderedDict(),
 			'states'        : OrderedDict(),
 			'src_loc'       : tracer.get_src_loc(src_loc_at = 1),
 			'state_src_locs': {},
 		})
+		if TYPE_CHECKING:
+			assert isinstance(fsm_data, _FSMDict)
 		self._generated[name] = fsm = FSM(
 			fsm_data['signal'], fsm_data['encoding'], fsm_data['decoding']
 		)
 		try:
 			self._ctrl_context = 'FSM'
 			self.domain._depth += 1
 			yield fsm
@@ -385,24 +484,29 @@
 					raise NameError(f'FSM state \'{state_name}\' is referenced but not defined')
 		finally:
 			self.domain._depth -= 1
 			self._ctrl_context = None
 		self._pop_ctrl()
 
 	@contextmanager
-	def State(self, name):
+	def State(self, name: str):
 		self._check_context('FSM State', context = 'FSM')
 		src_loc = tracer.get_src_loc(src_loc_at = 1)
 		fsm_data = self._get_ctrl('FSM')
+		if TYPE_CHECKING:
+			assert fsm_data is None or isinstance(fsm_data, _FSMDict)
+		if fsm_data is None:
+			raise SyntaxError('State outside of FSM block')
 		if name in fsm_data['states']:
 			raise NameError(f'FSM state \'{name}\' is already defined')
 		if name not in fsm_data['encoding']:
 			fsm_data['encoding'][name] = len(fsm_data['encoding'])
+		_outer_case = self._statements
 		try:
-			_outer_case, self._statements = self._statements, []
+			self._statements = Statement.cast([])
 			self._ctrl_context = None
 			yield
 			self._flush_ctrl()
 			fsm_data['states'][name] = self._statements
 			fsm_data['state_src_locs'][name] = src_loc
 		finally:
 			self._ctrl_context = 'FSM'
@@ -413,14 +517,16 @@
 		raise SyntaxError('Only assignment to `m.next` is permitted')
 
 	@next.setter
 	def next(self, name):
 		if self._ctrl_context != 'FSM':
 			for level, (ctrl_name, ctrl_data) in enumerate(reversed(self._ctrl_stack)):
 				if ctrl_name == 'FSM':
+					if TYPE_CHECKING:
+						assert isinstance(ctrl_data, _FSMDict)
 					if name not in ctrl_data['encoding']:
 						ctrl_data['encoding'][name] = len(ctrl_data['encoding'])
 					self._add_statement(
 						assigns = [ ctrl_data['signal'].eq(ctrl_data['encoding'][name]) ],
 						domain  = ctrl_data['domain'],
 						depth   = len(self._ctrl_stack)
 					)
@@ -429,14 +535,16 @@
 		raise SyntaxError('`m.next = <...>` is only permitted inside an FSM state')
 
 	def _pop_ctrl(self):
 		name, data = self._ctrl_stack.pop()
 		src_loc = data['src_loc']
 
 		if name == 'If':
+			if TYPE_CHECKING:
+				assert isinstance(data, _IfDict)
 			if_tests, if_bodies = data['tests'], data['bodies']
 			if_src_locs = data['src_locs']
 
 			tests, cases = [], OrderedDict()
 			for if_test, if_case in zip(if_tests + [ None ], if_bodies):
 				if if_test is not None:
 					if len(if_test) != 1:
@@ -449,23 +557,30 @@
 					match = None
 				cases[match] = if_case
 
 			self._statements.append(Switch(Cat(tests), cases,
 				src_loc = src_loc, case_src_locs = dict(zip(cases, if_src_locs))))
 
 		if name == 'Switch':
+			if TYPE_CHECKING:
+				assert isinstance(data, _SwitchDict)
 			switch_test, switch_cases = data['test'], data['cases']
 			switch_case_src_locs = data['case_src_locs']
 
 			self._statements.append(Switch(switch_test, switch_cases,
 				src_loc = src_loc, case_src_locs = switch_case_src_locs))
 
 		if name == 'FSM':
-			fsm_signal, fsm_reset, fsm_encoding, fsm_decoding, fsm_states = \
-				data['signal'], data['reset'], data['encoding'], data['decoding'], data['states']
+			if TYPE_CHECKING:
+				assert isinstance(data, _FSMDict)
+			fsm_signal = data['signal']
+			fsm_reset = data['reset']
+			fsm_encoding = data['encoding']
+			fsm_decoding = data['decoding']
+			fsm_states = data['states']
 			fsm_state_src_locs = data['state_src_locs']
 			if not fsm_states:
 				return
 			fsm_signal.width = bits_for(len(fsm_encoding) - 1)
 			if fsm_reset is None:
 				fsm_signal.reset = fsm_encoding[next(iter(fsm_states))]
 			else:
@@ -485,15 +600,15 @@
 			else:
 				return domain
 
 		while len(self._ctrl_stack) > self.domain._depth:
 			self._pop_ctrl()
 
 		for stmt in Statement.cast(assigns):
-			if not compat_mode and not isinstance(stmt, (Assign, Assert, Assume, Cover)):
+			if not compat_mode and not isinstance(stmt, (Assign, Property)):
 				raise SyntaxError(f'Only assignments and property checks may be appended to d.{domain_name(domain)}')
 
 			stmt._MustUse__used = True
 			stmt = SampleDomainInjector(domain)(stmt)
 
 			for signal in stmt._lhs_signals():
 				if signal not in self._driving:
@@ -512,21 +627,21 @@
 		if name is None:
 			self._anon_submodules.append(submodule)
 		else:
 			if name in self._named_submodules:
 				raise NameError(f'Submodule named \'{name}\' already exists')
 			self._named_submodules[name] = submodule
 
-	def _get_submodule(self, name):
+	def _get_submodule(self, name: str):
 		if name in self._named_submodules:
 			return self._named_submodules[name]
 		else:
 			raise AttributeError(f'No submodule named \'{name}\' exists')
 
-	def _add_domain(self, cd):
+	def _add_domain(self, cd: ClockDomain):
 		if cd.name in self._domains:
 			raise NameError(f'Clock domain named \'{cd.name}\' already exists')
 		self._domains[cd.name] = cd
 
 	def _flush(self):
 		while self._ctrl_stack:
 			self._pop_ctrl()
```

### Comparing `torii-0.5.0/torii/hdl/ir.py` & `torii-0.6.0/torii/hdl/ir.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import warnings
 from abc               import ABCMeta, abstractmethod
 from collections       import OrderedDict, defaultdict
 from functools         import reduce
 from typing            import Any, Optional, Union
 
 from ..util            import flatten
+from ..util.tracer     import get_src_loc
 from ..util.decorators import memoize
 from ._unused          import MustUse, UnusedMustUse
 from .ast              import (
 	ClockSignal, ResetSignal, Signal, SignalDict, SignalSet, Statement,
 	Value
 )
 from .cd               import ClockDomain, DomainError
@@ -78,15 +79,17 @@
 		self.domains = OrderedDict()
 		self.subfragments = []
 		self.attrs = OrderedDict()
 		self.generated = OrderedDict()
 		self.flatten = False
 
 	def add_ports(self, *ports, dir):
-		assert dir in ('i', 'o', 'io')
+		if dir not in ('i', 'o', 'io'):
+			raise ValueError(f'Expected dir to be \'i\', \'o\', or \'io\', not \'{dir}\'')
+
 		for port in flatten(ports):
 			self.ports[port] = dir
 
 	def iter_ports(self, dir = None):
 		if dir is None:
 			yield from self.ports
 		else:
@@ -125,28 +128,33 @@
 				if cd.rst is not None:
 					signals.add(cd.rst)
 			signals |= domain_signals
 		return signals
 
 	def add_domains(self, *domains):
 		for domain in flatten(domains):
-			assert isinstance(domain, ClockDomain)
-			assert domain.name not in self.domains
+			if not isinstance(domain, ClockDomain):
+				raise TypeError(f'Domain must be a \'ClockDomain\', not a \'{domain!r}\'')
+
+			if domain.name in self.domains:
+				raise ValueError(f'Domain \'{domain.name}\' already in the list of domains')
+
 			self.domains[domain.name] = domain
 
 	def iter_domains(self):
 		yield from self.domains
 
 	def add_statements(self, *stmts):
 		for stmt in Statement.cast(stmts):
 			stmt._MustUse__used = True
 			self.statements.append(stmt)
 
 	def add_subfragment(self, subfragment, name = None):
-		assert isinstance(subfragment, Fragment)
+		if not isinstance(subfragment, Fragment):
+			raise TypeError(f'Unable to add subfragment that is of type \'{type(subfragment)}\', not \'Fragment\'')
 		self.subfragments.append((subfragment, name))
 
 	def find_subfragment(self, name_or_index):
 		if isinstance(name_or_index, int):
 			if name_or_index < len(self.subfragments):
 				subfragment, name = self.subfragments[name_or_index]
 				return subfragment
@@ -181,18 +189,20 @@
 		# Remove the merged subfragment.
 		found = False
 		for i, (check_subfrag, check_name) in enumerate(self.subfragments): # :nobr:
 			if subfragment == check_subfrag:
 				del self.subfragments[i]
 				found = True
 				break
-		assert found
+		if not found:
+			raise RuntimeError('Unable to find merged subfragment!')
 
 	def _resolve_hierarchy_conflicts(self, hierarchy = ('top',), mode = 'warn'):
-		assert mode in ('silent', 'warn', 'error')
+		if mode not in ('silent', 'warn', 'error'):
+			raise ValueError(f'Expected mode to be one of \'silent\', \'warn\', or \'error\', not \'{mode!r}\'')
 
 		driver_subfrags = SignalDict()
 
 		def add_subfrag(registry, entity, entry):
 			# Because of missing domain insertion, at the point when this code runs, we have
 			# a mixture of bound and unbound {Clock,Reset}Signals. Map the bound ones to
 			# the actual signals (because the signal itself can be driven as well); but leave
@@ -327,15 +337,19 @@
 				self.add_domains(domain)
 
 	def _propagate_domains_down(self):
 		# For each domain defined in this fragment, ensure it also exists in all subfragments.
 		for subfrag, name in self.subfragments:
 			for domain in self.iter_domains():
 				if domain in subfrag.domains:
-					assert self.domains[domain] is subfrag.domains[domain]
+					if self.domains[domain] is not subfrag.domains[domain]:
+						raise RuntimeError(
+							f'Subfragment domain propagation failure, mismatching domains: '
+							f'{self.domains[domain]!r} is not {subfrag.domains[domain]!r}'
+						)
 				else:
 					subfrag.add_domains(self.domains[domain])
 
 			subfrag._propagate_domains_down()
 
 	def _create_missing_domains(self, missing_domain, *, platform = None):
 		from .xfrm import DomainCollector
@@ -543,14 +557,95 @@
 			for cd in new_domains:
 				mapped_ports.append(cd.clk)
 				if cd.rst is not None:
 					mapped_ports.append(cd.rst)
 			fragment._propagate_ports(ports = mapped_ports, all_undef_as_ports = False)
 		return fragment
 
+	def _assign_names_to_signals(self):
+		'''
+		Assign names to signals used in this fragment.
+
+		Returns
+		-------
+		SignalDict of Signal to str
+			A mapping from signals used in this fragment to their local names. Because names are
+			deduplicated using local information only, the same signal used in a different fragment
+			may get a different name.
+		'''
+
+		signal_names   = SignalDict()
+		assigned_names = set()
+
+		def add_signal_name(signal):
+			if signal not in signal_names:
+				if signal.name not in assigned_names:
+					name = signal.name
+				else:
+					name = f'{signal.name}${len(assigned_names)}'
+					assert name not in assigned_names
+				signal_names[signal] = name
+				assigned_names.add(name)
+
+		for port in self.ports.keys():
+			add_signal_name(port)
+
+		for domain_name, domain_signals in self.drivers.items():
+			if domain_name is not None:
+				domain = self.domains[domain_name]
+				add_signal_name(domain.clk)
+				if domain.rst is not None:
+					add_signal_name(domain.rst)
+
+		for statement in self.statements:
+			for signal in statement._lhs_signals() | statement._rhs_signals():
+				if not isinstance(signal, (ClockSignal, ResetSignal)):
+					add_signal_name(signal)
+
+		return signal_names
+
+	def _assign_names_to_fragments(self, hierarchy = ('top',), *, _names = None):
+		'''
+		Assign names to this fragment and its subfragments.
+
+		Subfragments may not necessarily have a name. This method assigns every such subfragment
+		a name, ``U$<number>``, where ``<number>`` is based on its location in the hierarchy.
+
+		Subfragment names may collide with signal names safely in Torii, but this may confuse
+		backends. This method assigns every such subfragment a name, ``<name>$U$<number>``, where
+		``name`` is its original name, and ``<number>`` is based on its location in the hierarchy.
+
+		Arguments
+		---------
+		hierarchy : tuple of str
+			Name of this fragment.
+
+		Returns
+		-------
+		dict of Fragment to tuple of str
+			A mapping from this fragment and its subfragments to their full hierarchical names.
+		'''
+
+		if _names is None:
+			_names = dict()
+		_names[self] = hierarchy
+
+		signal_names = set(self._assign_names_to_signals().values())
+		for subfragment_index, (subfragment, subfragment_name) in enumerate(self.subfragments):
+			if subfragment_name is None:
+				subfragment_name = f'U${subfragment_index}'
+			elif subfragment_name in signal_names:
+				subfragment_name = f'{subfragment_name}$U${subfragment_index}'
+			assert subfragment_name not in signal_names
+			subfragment._assign_names_to_fragments(
+				hierarchy = (*hierarchy, subfragment_name), _names = _names
+			)
+
+		return _names
+
 
 class Instance(Fragment):
 	'''
 	Allows for the direct instantiation of external modules, cells, or primitives.
 
 	It accepts the name of the object to instantiate and a collection of keyword arguments
 	that define the ports, attributes, and parameters to it.
@@ -587,20 +682,21 @@
 	Parameters
 	----------
 	type: str
 		The name/type of object to instantiate
 
 	'''
 
-	def __init__(self, type, *args, **kwargs):
+	def __init__(self, type, *args, src_loc = None, src_loc_at = 0, **kwargs):
 		super().__init__()
 
 		self.type        = type
 		self.parameters  = OrderedDict()
 		self.named_ports = OrderedDict()
+		self.src_loc     = src_loc or get_src_loc(src_loc_at)
 
 		for (kind, name, value) in args:
 			if kind == 'a':
 				self.attrs[name] = value
 			elif kind == 'p':
 				self.parameters[name] = value
 			elif kind in ('i', 'o', 'io'):
```

### Comparing `torii-0.5.0/torii/hdl/mem.py` & `torii-0.6.0/torii/hdl/mem.py`

 * *Files 18% similar despite different names*

```diff
@@ -89,15 +89,15 @@
 				if addr < len(self._init):
 					self._array[addr].reset = operator.index(self._init[addr])
 				else:
 					self._array[addr].reset = 0
 		except TypeError as e:
 			raise TypeError(f'Memory initialization value at address {addr:x}: {e}') from None
 
-	def read_port(self, *, src_loc_at = 0, **kwargs):
+	def read_port(self, *, src_loc_at = 0, **kwargs) -> 'ReadPort':
 		'''
 		Get a read port.
 
 		See :class:`ReadPort` for details.
 
 		Arguments
 		---------
@@ -108,15 +108,15 @@
 		-------
 		An instance of :class:`ReadPort` associated with this memory.
 
 		'''
 
 		return ReadPort(self, src_loc_at = 1 + src_loc_at, **kwargs)
 
-	def write_port(self, *, src_loc_at = 0, **kwargs):
+	def write_port(self, *, src_loc_at = 0, **kwargs) -> 'WritePort':
 		'''
 		Get a write port.
 
 		See :class:`WritePort` for details.
 
 		Arguments
 		---------
@@ -132,68 +132,15 @@
 		return WritePort(self, src_loc_at = 1 + src_loc_at, **kwargs)
 
 	def __getitem__(self, index):
 		''' Simulation only. '''
 		return self._array[index]
 
 	def elaborate(self, platform):
-		init = ''.join(format(Const(elem, unsigned(self.width)).value, f'0{self.width}b') for elem in reversed(self.init))
-		init = Const(int(init or '0', 2), self.depth * self.width)
-		rd_clk = []
-		rd_clk_enable = 0
-		rd_transparency_mask = 0
-		for index, port in enumerate(self._read_ports):
-			if port.domain != 'comb':
-				rd_clk.append(ClockSignal(port.domain))
-				rd_clk_enable |= 1 << index
-				if port.transparent:
-					for write_index, write_port in enumerate(self._write_ports):
-						if port.domain == write_port.domain:
-							rd_transparency_mask |= 1 << (index * len(self._write_ports) + write_index)
-			else:
-				rd_clk.append(Const(0, 1))
-
-		f = Instance(
-			'$mem_v2',
-			*(('a', attr, value) for attr, value in self.attrs.items()),
-			p_SIZE                 = self.depth,
-			p_OFFSET               = 0,
-			p_ABITS                = Shape.cast(range(self.depth)).width,
-			p_WIDTH                = self.width,
-			p_INIT                 = init,
-			p_RD_PORTS             = len(self._read_ports),
-			p_RD_CLK_ENABLE        = Const(rd_clk_enable, len(self._read_ports)) if self._read_ports else Const(0, 1),
-			p_RD_CLK_POLARITY      = Const(-1, unsigned(len(self._read_ports))) if self._read_ports else Const(0, 1),
-			p_RD_TRANSPARENCY_MASK = Const(rd_transparency_mask, max(1, len(self._read_ports) * len(self._write_ports))),
-			p_RD_COLLISION_X_MASK  = Const(0, max(1, len(self._read_ports) * len(self._write_ports))),
-			p_RD_WIDE_CONTINUATION = Const(0, len(self._read_ports)) if self._read_ports else Const(0, 1),
-			p_RD_CE_OVER_SRST      = Const(0, len(self._read_ports)) if self._read_ports else Const(0, 1),
-			p_RD_ARST_VALUE        = Const(0, len(self._read_ports) * self.width),
-			p_RD_SRST_VALUE        = Const(0, len(self._read_ports) * self.width),
-			p_RD_INIT_VALUE        = Const(0, len(self._read_ports) * self.width),
-			p_WR_PORTS             = len(self._write_ports),
-			p_WR_CLK_ENABLE        = Const(-1, unsigned(len(self._write_ports))) if self._write_ports else Const(0, 1),
-			p_WR_CLK_POLARITY      = Const(-1, unsigned(len(self._write_ports))) if self._write_ports else Const(0, 1),
-			p_WR_PRIORITY_MASK     = Const(0, len(self._write_ports) * len(self._write_ports)) if self._write_ports else Const(0, 1),
-			p_WR_WIDE_CONTINUATION = Const(0, len(self._write_ports)) if self._write_ports else Const(0, 1),
-			i_RD_CLK               = Cat(rd_clk),
-			i_RD_EN                = Cat(port.en for port in self._read_ports),
-			i_RD_ARST              = Const(0, len(self._read_ports)),
-			i_RD_SRST              = Const(0, len(self._read_ports)),
-			i_RD_ADDR              = Cat(port.addr for port in self._read_ports),
-			o_RD_DATA              = Cat(port.data for port in self._read_ports),
-			i_WR_CLK               = Cat(ClockSignal(port.domain) for port in self._write_ports),
-			i_WR_EN                = Cat(
-				Cat(
-					en_bit.replicate(port.granularity) for en_bit in port.en
-				) for port in self._write_ports
-			),
-			i_WR_ADDR              = Cat(port.addr for port in self._write_ports),
-			i_WR_DATA              = Cat(port.data for port in self._write_ports),
-		)
+		f = MemoryInstance(self, self._read_ports, self._write_ports)
 
 		for port in self._read_ports:
 			port._MustUse__used = True
 			if port.domain == 'comb':
 				f.add_statements(port.data.eq(self._array[port.addr]))
 				f.add_driver(port.data)
 			else:
@@ -386,7 +333,15 @@
 			granularity = data_width
 		if name is None:
 			name = tracer.get_var_name(depth = 2, default = 'dummy')
 
 		self.addr = Signal(addr_width, name = f'{name}_addr', src_loc_at = 1)
 		self.data = Signal(data_width, name = f'{name}_data', src_loc_at = 1)
 		self.en   = Signal(data_width // granularity, name = f'{name}_en', src_loc_at = 1)
+
+class MemoryInstance(Fragment):
+	def __init__(self, memory: Memory, read_ports: list[ReadPort], write_ports: list[WritePort]):
+		super().__init__()
+		self.memory      = memory
+		self.read_ports  = read_ports
+		self.write_ports = write_ports
+		self.attrs       = memory.attrs
```

### Comparing `torii-0.5.0/torii/hdl/rec.py` & `torii-0.6.0/torii/hdl/rec.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,14 +153,17 @@
 				else:
 					self.fields[field_name] = Signal(
 						field_shape, name = concat(name, field_name),
 						src_loc_at = 1 + src_loc_at
 					)
 
 	def __getattr__(self, name):
+		# TODO: Add tests for this!
+		if name == 'fields' and name not in self.__dict__:
+			raise AssertionError('Record has not been properly constructed and does not have any fields')
 		return self[name]
 
 	def __getitem__(self, item):
 		if isinstance(item, str):
 			try:
 				return self.fields[item]
 			except KeyError:
```

### Comparing `torii-0.5.0/torii/hdl/xfrm.py` & `torii-0.6.0/torii/hdl/xfrm.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 # SPDX-License-Identifier: BSD-2-Clause
 
 from abc             import ABCMeta, abstractmethod
 from collections     import OrderedDict
 from collections.abc import Iterable
+from copy            import copy
 
 from ..util          import flatten, tracer
 from .ast            import (
-	AnyConst, AnySeq, ArrayProxy, Assert, Assign, Assume, Cat,
+	AnyConst, AnySeq, AnyValue, ArrayProxy, Assert, Assign, Assume, Cat,
 	ClockSignal, Const, Cover, Initial, Mux, Operator, Part,
 	Property, ResetSignal, Sample, Signal, SignalDict,
 	SignalSet, Slice, Statement, Switch, Value, ValueDict,
 	_StatementList
 )
 from .cd             import DomainError
 from .ir             import Elaboratable, Fragment, Instance
+from .mem            import MemoryInstance
 
 __all__ = (
 	'DomainCollector',
 	'DomainLowerer',
 	'DomainRenamer',
 	'EnableInserter',
 	'FragmentTransformer',
@@ -37,34 +39,30 @@
 
 class ValueVisitor(metaclass = ABCMeta):
 	@abstractmethod
 	def on_Const(self, value):
 		pass # :nocov:
 
 	@abstractmethod
-	def on_AnyConst(self, value):
-		pass # :nocov:
-
-	@abstractmethod
-	def on_AnySeq(self, value):
-		pass # :nocov:
-
-	@abstractmethod
 	def on_Signal(self, value):
 		pass # :nocov:
 
 	@abstractmethod
 	def on_ClockSignal(self, value):
 		pass # :nocov:
 
 	@abstractmethod
 	def on_ResetSignal(self, value):
 		pass # :nocov:
 
 	@abstractmethod
+	def on_AnyValue(self, value):
+		pass # :nocov:
+
+	@abstractmethod
 	def on_Operator(self, value):
 		pass # :nocov:
 
 	@abstractmethod
 	def on_Slice(self, value):
 		pass # :nocov:
 
@@ -93,24 +91,22 @@
 
 	def replace_value_src_loc(self, value, new_value):
 		return True
 
 	def on_value(self, value):
 		if type(value) is Const:
 			new_value = self.on_Const(value)
-		elif type(value) is AnyConst:
-			new_value = self.on_AnyConst(value)
-		elif type(value) is AnySeq:
-			new_value = self.on_AnySeq(value)
 		elif type(value) is Signal:
 			new_value = self.on_Signal(value)
 		elif type(value) is ClockSignal:
 			new_value = self.on_ClockSignal(value)
 		elif type(value) is ResetSignal:
 			new_value = self.on_ResetSignal(value)
+		elif type(value) is AnyValue:
+			new_value = self.on_AnyValue(value)
 		elif type(value) is Operator:
 			new_value = self.on_Operator(value)
 		elif type(value) is Slice:
 			new_value = self.on_Slice(value)
 		elif type(value) is Part:
 			new_value = self.on_Part(value)
 		elif type(value) is Cat:
@@ -131,29 +127,26 @@
 		return self.on_value(value)
 
 
 class ValueTransformer(ValueVisitor):
 	def on_Const(self, value):
 		return value
 
-	def on_AnyConst(self, value):
-		return value
-
-	def on_AnySeq(self, value):
-		return value
-
 	def on_Signal(self, value):
 		return value
 
 	def on_ClockSignal(self, value):
 		return value
 
 	def on_ResetSignal(self, value):
 		return value
 
+	def on_AnyValue(self, value):
+		return value
+
 	def on_Operator(self, value):
 		return Operator(value.operator, [ self.on_value(o) for o in value.operands ])
 
 	def on_Slice(self, value):
 		return Slice(self.on_value(value.value), value.start, value.stop)
 
 	def on_Part(self, value):
@@ -178,23 +171,15 @@
 
 class StatementVisitor(metaclass = ABCMeta):
 	@abstractmethod
 	def on_Assign(self, stmt):
 		pass # :nocov:
 
 	@abstractmethod
-	def on_Assert(self, stmt):
-		pass # :nocov:
-
-	@abstractmethod
-	def on_Assume(self, stmt):
-		pass # :nocov:
-
-	@abstractmethod
-	def on_Cover(self, stmt):
+	def on_Property(self, stmt):
 		pass # :nocov:
 
 	@abstractmethod
 	def on_Switch(self, stmt):
 		pass # :nocov:
 
 	@abstractmethod
@@ -206,20 +191,16 @@
 
 	def replace_statement_src_loc(self, stmt, new_stmt):
 		return True
 
 	def on_statement(self, stmt):
 		if type(stmt) is Assign:
 			new_stmt = self.on_Assign(stmt)
-		elif type(stmt) is Assert:
-			new_stmt = self.on_Assert(stmt)
-		elif type(stmt) is Assume:
-			new_stmt = self.on_Assume(stmt)
-		elif type(stmt) is Cover:
-			new_stmt = self.on_Cover(stmt)
+		elif type(stmt) is Property:
+			new_stmt = self.on_Property(stmt)
 		elif isinstance(stmt, Switch):
 			# Uses `isinstance()` and not `type() is` because amaranth.compat requires it.
 			new_stmt = self.on_Switch(stmt)
 		elif isinstance(stmt, Iterable):
 			new_stmt = self.on_statements(stmt)
 		else:
 			new_stmt = self.on_unknown_statement(stmt)
@@ -238,29 +219,18 @@
 class StatementTransformer(StatementVisitor):
 	def on_value(self, value):
 		return value
 
 	def on_Assign(self, stmt):
 		return Assign(self.on_value(stmt.lhs), self.on_value(stmt.rhs))
 
-	def on_Assert(self, stmt):
-		return Assert(
-			self.on_value(stmt.test), _check = stmt._check,
-			_en = stmt._en, name = stmt.name
-		)
-
-	def on_Assume(self, stmt):
-		return Assume(
-			self.on_value(stmt.test), _check = stmt._check,
-			_en = stmt._en, name = stmt.name
-		)
 
-	def on_Cover(self, stmt):
-		return Cover(
-			self.on_value(stmt.test), _check = stmt._check,
+	def on_Property(self, stmt):
+		return Property(
+			stmt.kind, self.on_value(stmt.test), _check = stmt._check,
 			_en = stmt._en, name = stmt.name
 		)
 
 	def on_Switch(self, stmt):
 		cases = OrderedDict((k, self.on_statement(s)) for k, s in stmt.cases.items())
 		return Switch(self.on_value(stmt.test), cases)
 
@@ -294,17 +264,40 @@
 		else:
 			new_fragment.add_statements(fragment.statements)
 
 	def map_drivers(self, fragment, new_fragment):
 		for domain, signal in fragment.iter_drivers():
 			new_fragment.add_driver(signal, domain)
 
+	def map_memory_ports(self, fragment, new_fragment):
+		new_fragment.read_ports = [
+			copy(port) for port in fragment.read_ports
+		]
+
+		new_fragment.write_ports = [
+			copy(port) for port in fragment.write_ports
+		]
+
+		if hasattr(self, 'on_value'):
+			for port in new_fragment.read_ports:
+				port.en   = self.on_value(port.en)
+				port.addr = self.on_value(port.addr)
+				port.data = self.on_value(port.data)
+
+			for port in new_fragment.write_ports:
+				port.en   = self.on_value(port.en)
+				port.addr = self.on_value(port.addr)
+				port.data = self.on_value(port.data)
+
 	def on_fragment(self, fragment):
-		if isinstance(fragment, Instance):
-			new_fragment = Instance(fragment.type)
+		if isinstance(fragment, MemoryInstance):
+			new_fragment = MemoryInstance(fragment.memory, [], [])
+			self.map_memory_ports(fragment, new_fragment)
+		elif isinstance(fragment, Instance):
+			new_fragment = Instance(fragment.type, src_loc = fragment.src_loc)
 			new_fragment.parameters = OrderedDict(fragment.parameters)
 			self.map_named_ports(fragment, new_fragment)
 		else:
 			new_fragment = Fragment()
 			new_fragment.flatten = fragment.flatten
 		new_fragment.attrs = OrderedDict(fragment.attrs)
 		self.map_ports(fragment, new_fragment)
@@ -326,15 +319,16 @@
 			return value
 		else:
 			raise AttributeError(f'Object {value!r} cannot be elaborated')
 
 
 class TransformedElaboratable(Elaboratable):
 	def __init__(self, elaboratable, *, src_loc_at = 0):
-		assert hasattr(elaboratable, 'elaborate')
+		if not hasattr(elaboratable, 'elaborate'):
+			raise TypeError(f'Unable to elaborate object of type \'{type(elaboratable)}\' which has no \'elaborate\' method')
 
 		# Fields prefixed and suffixed with underscore to avoid as many conflicts with the inner
 		# object as possible, since we're forwarding attribute requests to it.
 		self._elaboratable_ = elaboratable
 		self._transforms_   = []
 
 	def __getattr__(self, attr):
@@ -360,17 +354,16 @@
 			return
 		self.used_domains.add(domain_name)
 
 	def on_ignore(self, value):
 		pass
 
 	on_Const = on_ignore
-	on_AnyConst = on_ignore
-	on_AnySeq = on_ignore
 	on_Signal = on_ignore
+	on_AnyValue = on_ignore
 
 	def on_ClockSignal(self, value):
 		self._add_used_domain(value.domain)
 
 	def on_ResetSignal(self, value):
 		self._add_used_domain(value.domain)
 
@@ -400,31 +393,41 @@
 	def on_Initial(self, value):
 		pass
 
 	def on_Assign(self, stmt):
 		self.on_value(stmt.lhs)
 		self.on_value(stmt.rhs)
 
-	def on_property(self, stmt):
+	def on_Property(self, stmt):
 		self.on_value(stmt.test)
 
-	on_Assert = on_property
-	on_Assume = on_property
-	on_Cover  = on_property
-
 	def on_Switch(self, stmt):
 		self.on_value(stmt.test)
 		for stmts in stmt.cases.values():
 			self.on_statement(stmts)
 
 	def on_statements(self, stmts):
 		for stmt in stmts:
 			self.on_statement(stmt)
 
 	def on_fragment(self, fragment):
+		if isinstance(fragment, MemoryInstance):
+			for port in fragment.read_ports:
+				self.on_value(port.addr)
+				self.on_value(port.data)
+				self.on_value(port.en)
+				if port.domain != 'comb':
+					self._add_used_domain(port.domain)
+
+			for port in fragment.write_ports:
+				self.on_value(port.addr)
+				self.on_value(port.data)
+				self.on_value(port.en)
+				self._add_used_domain(port.domain)
+
 		if isinstance(fragment, Instance):
 			for name, (value, dir) in fragment.named_ports.items():
 				self.on_value(value)
 
 		old_local_domains, self._local_domains = self._local_domains, set(self._local_domains)
 		for domain_name, domain in fragment.domains.items():
 			if domain.local:
@@ -472,24 +475,36 @@
 		for domain in fragment.iter_domains():
 			cd = fragment.domains[domain]
 			if domain in self.domain_map:
 				if cd.name == domain:
 					# Rename the actual ClockDomain object.
 					cd.rename(self.domain_map[domain])
 				else:
-					assert cd.name == self.domain_map[domain]
+					if cd.name != self.domain_map[domain]:
+						raise ValueError(f'Clock domain mismatch! \'{cd.name}\' != \'{self.domain_map[domain]}\'')
 			new_fragment.add_domains(cd)
 
 	def map_drivers(self, fragment, new_fragment):
 		for domain, signals in fragment.drivers.items():
 			if domain in self.domain_map:
 				domain = self.domain_map[domain]
 			for signal in signals:
 				new_fragment.add_driver(self.on_value(signal), domain)
 
+	def map_memory_ports(self, fragment, new_fragment):
+		super().map_memory_ports(fragment, new_fragment)
+
+		for port in new_fragment.read_ports:
+			if port.domain in self.domain_map:
+				port.domain = self.domain_map[port.domain]
+
+		for port in new_fragment.write_ports:
+			if port.domain in self.domain_map:
+				port.domain = self.domain_map[port.domain]
+
 
 class DomainLowerer(FragmentTransformer, ValueTransformer, StatementTransformer):
 	def __init__(self, domains = None):
 		self.domains = domains
 
 	def _resolve(self, domain, context):
 		if domain not in self.domains:
@@ -573,15 +588,17 @@
 		if value in self.sample_cache:
 			return self.sample_cache[value]
 
 		sampled_value = self.on_value(value.value)
 		if value.clocks == 0:
 			sample = sampled_value
 		else:
-			assert value.domain is not None
+			if value.domain is None:
+				raise ValueError(f'Domain for value \'{value!r}\' is None!')
+
 			sampled_name, sampled_reset = self._name_reset(value.value)
 			name = f'$sample${sampled_name}${value.domain}${value.clocks}'
 			sample = Signal.like(value.value, name = name, reset_less = True, reset = sampled_reset)
 			sample.attrs['torii.sample_reg'] = True
 
 			prev_sample = self.on_Sample(Sample(sampled_value, value.clocks - 1, value.domain))
 			if value.domain not in self.sample_stmts:
@@ -610,17 +627,15 @@
 
 
 class SwitchCleaner(StatementVisitor):
 	def on_ignore(self, stmt):
 		return stmt
 
 	on_Assign = on_ignore
-	on_Assert = on_ignore
-	on_Assume = on_ignore
-	on_Cover  = on_ignore
+	on_Property = on_ignore
 
 	def on_Switch(self, stmt):
 		cases = OrderedDict((k, self.on_statement(s)) for k, s in stmt.cases.items())
 		if any(len(s) for s in cases.values()):
 			return Switch(stmt.test, cases)
 
 	def on_statements(self, stmts):
@@ -660,23 +675,19 @@
 		return groups
 
 	def on_Assign(self, stmt):
 		lhs_signals = stmt._lhs_signals()
 		if lhs_signals:
 			self.unify(*stmt._lhs_signals())
 
-	def on_property(self, stmt):
+	def on_Property(self, stmt):
 		lhs_signals = stmt._lhs_signals()
 		if lhs_signals:
 			self.unify(*stmt._lhs_signals())
 
-	on_Assert = on_property
-	on_Assume = on_property
-	on_Cover  = on_property
-
 	def on_Switch(self, stmt):
 		for case_stmts in stmt.cases.values():
 			self.on_statements(case_stmts)
 
 	def on_statements(self, stmts):
 		for stmt in stmts:
 			self.on_statement(stmt)
@@ -695,23 +706,19 @@
 		# on LHS are a part of the same group, so it is sufficient to check any of them.
 		lhs_signals = stmt.lhs._lhs_signals()
 		if lhs_signals:
 			any_lhs_signal = next(iter(lhs_signals))
 			if any_lhs_signal in self.signals:
 				return stmt
 
-	def on_property(self, stmt):
+	def on_Property(self, stmt):
 		any_lhs_signal = next(iter(stmt._lhs_signals()))
 		if any_lhs_signal in self.signals:
 			return stmt
 
-	on_Assert = on_property
-	on_Assume = on_property
-	on_Cover  = on_property
-
 
 class _ControlInserter(FragmentTransformer):
 	def __init__(self, controls):
 		self.src_loc = None
 		if isinstance(controls, Value):
 			controls = { 'sync': controls }
 		self.controls = OrderedDict(controls)
@@ -741,18 +748,16 @@
 class EnableInserter(_ControlInserter):
 	def _insert_control(self, fragment, domain, signals):
 		stmts = [s.eq(s) for s in signals]
 		fragment.add_statements(Switch(self.controls[domain], { 0: stmts }, src_loc = self.src_loc))
 
 	def on_fragment(self, fragment):
 		new_fragment = super().on_fragment(fragment)
-		if isinstance(new_fragment, Instance) and new_fragment.type == '$mem_v2':
-			for kind in ('RD', 'WR'):
-				clk_parts = new_fragment.named_ports[f'{kind}_CLK'][0].parts
-				en_parts  = new_fragment.named_ports[f'{kind}_EN'][0].parts
-				new_en = []
-				for clk, en in zip(clk_parts, en_parts):
-					if isinstance(clk, ClockSignal) and clk.domain in self.controls:
-						en = Mux(self.controls[clk.domain], en, Const(0, len(en)))
-					new_en.append(en)
-				new_fragment.named_ports[f'{kind}_EN'] = (Cat(new_en), 'i')
+		if isinstance(new_fragment, MemoryInstance):
+			for port in new_fragment.read_ports:
+				if port.domain in self.controls:
+					port.en = port.en & self.controls[port.domain]
+			for port in new_fragment.write_ports:
+				if port.domain in self.controls:
+					port.en = Mux(self.controls[port.domain], port.en, Const(0, len(port.en)))
+
 		return new_fragment
```

### Comparing `torii-0.5.0/torii/lib/cdc.py` & `torii-0.6.0/torii/lib/cdc.py`

 * *Files identical despite different names*

### Comparing `torii-0.5.0/torii/lib/coding/gray.py` & `torii-0.6.0/torii/lib/coding/gray.py`

 * *Files identical despite different names*

### Comparing `torii-0.5.0/torii/lib/coding/one_hot.py` & `torii-0.6.0/torii/lib/coding/one_hot.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 	def elaborate(self, platform) -> Module:
 		m = Module()
 		with m.Switch(self.i):
 			for j in range(self.width):
 				with m.Case(1 << j):
 					m.d.comb += self.o.eq(j)
-			with m.Case():
+			with m.Default():
 				m.d.comb += self.n.eq(1)
 		return m
 
 class Decoder(Elaboratable):
 	'''
 	Decode binary to one-hot.
```

### Comparing `torii-0.5.0/torii/lib/coding/priority.py` & `torii-0.6.0/torii/lib/coding/priority.py`

 * *Files identical despite different names*

### Comparing `torii-0.5.0/torii/lib/fifo.py` & `torii-0.6.0/torii/lib/fifo.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 ''' First-in first-out queues. '''
 
 from typing       import Union
 
 from ..           import Elaboratable, Memory, Module, Mux, ResetSignal, Signal
 from ..asserts    import Assert, Assume, Initial
-from ..util.units import log2_int
+from ..util.units import log2_ceil
 from .cdc         import AsyncFFSynchronizer, FFSynchronizer
 from .coding.gray import Decoder, Encoder
 
 __all__ = (
 	'AsyncFIFO',
 	'AsyncFIFOBuffered',
 	'FIFOInterface',
@@ -72,15 +72,15 @@
 		'''.strip(),
 		r_data_valid = 'The conditions in which ``r_data`` is valid depends on the type of the queue.',
 		attributes   = '',
 		w_attributes = '',
 		r_attributes = ''
 	)
 
-	def __init__(self, *, width: int, depth: int, fwft: bool) -> None:
+	def __init__(self, *, width: int, depth: int, fwft: bool = True) -> None:
 		if not isinstance(width, int) or width < 0:
 			raise TypeError(f'FIFO width must be a non-negative integer, not {width!r}')
 
 		if not isinstance(depth, int) or depth < 0:
 			raise TypeError(f'FIFO depth must be a non-negative integer, not {depth!r}')
 
 		self.width = width
@@ -149,17 +149,17 @@
 			self.w_level.eq(self.level),
 			self.r_level.eq(self.level),
 		]
 
 		do_read  = self.r_rdy & self.r_en
 		do_write = self.w_rdy & self.w_en
 
-		storage = Memory(width = self.width, depth = self.depth)
-		w_port  = m.submodules.w_port = storage.write_port()
-		r_port  = m.submodules.r_port = storage.read_port(
+		m.submodules.storage = storage = Memory(width = self.width, depth = self.depth)
+		w_port = storage.write_port()
+		r_port = storage.read_port(
 			domain = 'comb' if self.fwft else 'sync', transparent = self.fwft)
 		produce = Signal(range(self.depth))
 		consume = Signal(range(self.depth))
 
 		m.d.comb += [
 			w_port.addr.eq(produce),
 			w_port.data.eq(self.w_data),
@@ -231,15 +231,15 @@
 		'''.strip(),
 		r_data_valid = 'Valid if ``r_rdy`` is asserted.',
 		r_attributes = '',
 		w_attributes = ''
 	)
 
 	def __init__(self, *, width: int, depth: int):
-		super().__init__(width = width, depth = depth, fwft = True)
+		super().__init__(width = width, depth = depth)
 
 		self.level = Signal(range(depth + 1))
 
 	def elaborate(self, platform) -> Module:
 		m = Module()
 		if self.depth == 0:
 			m.d.comb += [
@@ -314,24 +314,23 @@
 	)
 
 	def __init__(
 		self, *, width: int, depth: int, r_domain: str = 'read', w_domain: str = 'write',
 		exact_depth: bool = False
 	) -> None:
 		if depth != 0:
-			try:
-				depth_bits = log2_int(depth, need_pow2 = exact_depth)
-				depth = 1 << depth_bits
-			except ValueError:
+			depth_bits = log2_ceil(depth)
+			if exact_depth and depth != 1 << depth_bits:
 				raise ValueError(
 					f'AsyncFIFO only supports depths that are powers of 2; requested exact depth {depth} is not'
 				) from None
+			depth = 1 << depth_bits
 		else:
 			depth_bits = 0
-		super().__init__(width = width, depth = depth, fwft = True)
+		super().__init__(width = width, depth = depth)
 
 		self.r_rst = Signal()
 		self._r_domain = r_domain
 		self._w_domain = w_domain
 		self._ctr_bits = depth_bits + 1
 
 	def elaborate(self, platform) -> Module:
@@ -400,17 +399,17 @@
 			),
 			r_empty.eq(consume_r_gry == produce_r_gry),
 		]
 
 		m.d[self._w_domain] += self.w_level.eq((produce_w_bin - consume_w_bin))
 		m.d.comb += self.r_level.eq((produce_r_bin - consume_r_bin))
 
-		storage = Memory(width = self.width, depth = self.depth)
-		w_port  = m.submodules.w_port = storage.write_port(domain = self._w_domain)
-		r_port  = m.submodules.r_port = storage.read_port(
+		m.submodules.storage = storage = Memory(width = self.width, depth = self.depth)
+		w_port = storage.write_port(domain = self._w_domain)
+		r_port = storage.read_port(
 			domain = self._r_domain, transparent = False
 		)
 		m.d.comb += [
 			w_port.addr.eq(produce_w_bin[:-1]),
 			w_port.data.eq(self.w_data),
 			w_port.en.eq(do_write),
 			self.w_rdy.eq(~w_full),
@@ -496,23 +495,23 @@
 	)
 
 	def __init__(
 		self, *, width: int, depth: int, r_domain: str = 'read', w_domain: str = 'write',
 		exact_depth: bool = False
 	) -> None:
 		if depth != 0:
-			try:
-				depth_bits = log2_int(max(0, depth - 1), need_pow2 = exact_depth)
-				depth = (1 << depth_bits) + 1
-			except ValueError:
+			depth_bits = log2_ceil(max(0, depth - 1))
+			if exact_depth and depth != (1 << depth_bits) + 1:
 				raise ValueError(
 					'AsyncFIFOBuffered only supports depths that are one higher than powers of 2; '
 					f'requested exact depth {depth} is not'
 				) from None
-		super().__init__(width = width, depth = depth, fwft = True)
+			depth = (1 << depth_bits) + 1
+
+		super().__init__(width = width, depth = depth)
 
 		self.r_rst = Signal()
 		self._r_domain = r_domain
 		self._w_domain = w_domain
 
 	def elaborate(self, platform) -> Module:
 		m = Module()
```

### Comparing `torii-0.5.0/torii/lib/io.py` & `torii-0.6.0/torii/lib/io.py`

 * *Files identical despite different names*

### Comparing `torii-0.5.0/torii/lib/scheduler.py` & `torii-0.6.0/torii/lib/scheduler.py`

 * *Files identical despite different names*

### Comparing `torii-0.5.0/torii/lib/soc/csr/bus.py` & `torii-0.6.0/torii/lib/soc/csr/bus.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # SPDX-License-Identifier: BSD-2-Clause
 
-from enum     import Enum
-from typing   import Optional
-
-from ....     import Elaboratable, Module, Mux, Record, Signal
-from ..memory import MemoryMap
+from collections    import defaultdict
+from enum           import Enum
+from typing         import Optional
+
+from ....           import Elaboratable, Module, Mux, Record, Signal
+from ....util.units import log2_ceil
+from ..memory       import MemoryMap
 
 __all__ = (
 	'Decoder',
 	'Element',
 	'Interface',
 	'Multiplexer',
 )
@@ -178,19 +180,198 @@
 				f'which is not the same as bus interface data width {self.data_width}'
 			)
 		memory_map.freeze()
 		self._map = memory_map
 
 
 class Multiplexer(Elaboratable):
+	class _Shadow:
+		class Chunk:
+			'''The interface between a CSR multiplexer and a shadow register chunk.'''
+			def __init__(self, shadow, offset, elements):
+				self.name = f'{shadow.name}__{offset}'
+				self.data = Signal(shadow.granularity, name = f'{self.name}__data')
+				self.r_en = Signal(name = f'{self.name}__r_en')
+				self.w_en = Signal(name = f'{self.name}__w_en')
+				self._elements = tuple(elements)
+
+			def elements(self):
+				'''Iterate the address ranges of CSR elements using this chunk.'''
+				yield from self._elements
+
+		'''
+		CSR multiplexer shadow register.
+
+		Attributes
+		----------
+		name : :class:`str`
+			Name of the shadow register.
+		granularity : :class:`int`
+			Amount of bits stored in a chunk of the shadow register.
+		overlaps : :class:`int`
+			Maximum number of CSR elements that can share a chunk of the shadow register. Optional.
+			If ``None``, it is implicitly set by :meth:`Multiplexer._Shadow.prepare`.
+		'''
+		def __init__(self, granularity, overlaps, *, name):
+			assert isinstance(name, str)
+			assert isinstance(granularity, int) and granularity >= 0
+			assert overlaps is None or isinstance(overlaps, int) and overlaps >= 0
+			self.name        = name
+			self.granularity = granularity
+			self.overlaps    = overlaps
+			self._ranges     = set()
+			self._size       = 1
+			self._chunks     = None
+
+		@property
+		def size(self):
+			'''
+			Size of the shadow register.
+
+			Returns
+			-------
+			:class:`int`
+				The amount of :class:`Multiplexer._Shadow.Chunk`s of the shadow. It can increase
+				by calling :meth:`Multiplexer._Shadow.add` or :meth:`Multiplexer._Shadow.prepare`.
+			'''
+			return self._size
+
+		def add(self, elem_range):
+			'''
+			Add a CSR element to the shadow.
+
+			Arguments
+			---------
+			elem_range : :class:`range`
+				Address range of a CSR :class:`Element`. It uses ``2 ** log2_ceil(elem_range.stop -
+				elem_range.start)`` chunks of the shadow register. If this amount is greater than
+				:attr:`~Multiplexer._Shadow.size`, it replaces the latter.
+			'''
+			assert isinstance(elem_range, range)
+			self._ranges.add(elem_range)
+			elem_size  = 2 ** log2_ceil(elem_range.stop - elem_range.start)
+			self._size = max(self._size, elem_size)
+
+		def decode_address(self, addr, elem_range):
+			'''
+			Decode a bus address into a shadow register offset.
+
+			Returns
+			-------
+			:class:`int`
+				The shadow register offset corresponding to the :class:`Multiplexer._Shadow.Chunk`
+				used by ``addr``.
+
+				The address decoding scheme is illustrated by the following example:
+					* ``addr`` is ``0x1c``;
+					* ``elem_range`` is ``range(0x1b, 0x1f)``;
+					* the :attr:`~Multiplexer._Shadow.size` of the shadow is ``16``.
+
+				The lower bits of the offset would be ``0b00``, extracted from ``addr``:
+
+				.. code-block::
+
+					+----+--+--+
+					|0001|11|00|
+					+----+--+--+
+							│  └─ 0
+							└──── log2_ceil(elem_range.stop - elem_range.start)
+
+				The upper bits of the offset would be ``0b10``, extracted from ``elem_range.start``:
+
+				.. code-block::
+
+					+----+--+--+
+					|0001|10|11|
+					+----+--+--+
+						 │  │
+						 │  └──── log2_ceil(elem_range.stop - elem_range.start)
+						 └─────── log2(self.size)
+
+
+				The decoded offset would therefore be ``8`` (i.e. ``0b1000``).
+			''' # noqa: E101
+			assert elem_range in self._ranges and addr in elem_range
+			elem_size = 2 ** log2_ceil(elem_range.stop - elem_range.start)
+			self_mask = self.size - 1
+			elem_mask = elem_size - 1
+			return elem_range.start & self_mask & ~elem_mask | addr & elem_mask
+
+		def encode_offset(self, offset, elem_range):
+			'''
+			Encode a shadow register offset into a bus address.
+
+			Returns
+			-------
+			:class:`int`
+				The bus address in ``elem_range`` using the :class:`Multiplexer._Shadow.Chunk`
+				located at ``offset``. See :meth:`~Multiplexer._Shadow.decode_address` for details.
+			'''
+			assert elem_range in self._ranges and isinstance(offset, int)
+			elem_size = 2 ** log2_ceil(elem_range.stop - elem_range.start)
+			return elem_range.start + ((offset - elem_range.start) % elem_size)
+
+		def prepare(self):
+			'''
+			Balance out and instantiate the shadow register chunks.
+
+			The scheme used by :meth:`~Multiplexer._Shadow.decode_address` allows multiple bus
+			addresses to be decoded to the same shadow register offset. Depending on the platform
+			and its toolchain, this may create nets with high fan-in (if the chunk is read from
+			the bus) or fan-out (if written), which may impact timing closure or resource usage.
+
+			If any shadow register offset is aliased to more bus addresses than permitted by the
+			:attr:`~Multiplexer._Shadow.overlaps` constraint, the :attr:`~Multiplexer._Shadow.size`
+			of the shadow is doubled. This increases the number of address bits used for decoding,
+			which effectively balances chunk usage across the shadow register.
+
+			This method is recursive until the overlap constraint is satisfied.
+			'''
+			if isinstance(self._ranges, frozenset):
+				return
+			if self.overlaps is None:
+				self.overlaps = len(self._ranges)
+
+			elements = defaultdict(list)
+			balanced = True
+
+			for elem_range in self._ranges:
+				for chunk_addr in elem_range:
+					chunk_offset = self.decode_address(chunk_addr, elem_range)
+					if len(elements[chunk_offset]) > self.overlaps:
+						balanced = False
+						break
+					elements[chunk_offset].append(elem_range)
+
+			if balanced:
+				self._ranges = frozenset(self._ranges)
+				self._chunks = dict()
+				for chunk_offset, chunk_elements in elements.items():
+					chunk = Multiplexer._Shadow.Chunk(self, chunk_offset, chunk_elements)
+					self._chunks[chunk_offset] = chunk
+			else:
+				self._size *= 2
+				self.prepare()
+
+		def chunks(self):
+			'''Iterate shadow register chunks used by at least one CSR element.'''
+			for chunk_offset, chunk in self._chunks.items():
+				yield chunk_offset, chunk
+
 	'''
 	CSR register multiplexer.
 
 	An address-based multiplexer for CSR registers implementing atomic updates.
 
+	This implementation assumes the following from the CSR bus:
+	* an initiator must have exclusive ownership over the multiplexer for the full duration of
+		a register transaction;
+	* an initiator must access a register in ascending order of addresses, but it may abort a
+		transaction after any bus cycle.
+
 	Latency
 	-------
 
 	Writes are registered, and are performed 1 cycle after ``w_stb`` is asserted.
 
 	Alignment
 	---------
@@ -224,29 +405,38 @@
 	data_width : int
 		Data width. See :class:`Interface`.
 	alignment : log2 of int
 		Register alignment. See :class:`..memory.MemoryMap`.
 	name : str
 		Window name. Optional.
 
+	shadow_overlaps : int
+		Maximum number of CSR registers that can share a chunk of a shadow register.
+		Optional. If ``None``, any number of CSR registers can share a shadow chunk.
+		See :class:`Multiplexer._Shadow` for details.
+
+
 	Attributes
 	----------
 	bus : :class:`Interface`
 		CSR bus providing access to registers.
 
 	''' # noqa: E101
 
 	def __init__(
-		self, *, addr_width: int, data_width: int, alignment: int = 0, name: Optional[str] = None
+		self, *, addr_width: int, data_width: int, alignment: int = 0, name: Optional[str] = None,
+		shadow_overlaps: Optional[int] = None
 	) -> None:
 		self._map = MemoryMap(
 			addr_width = addr_width, data_width = data_width,
 			alignment = alignment, name = name
 		)
 		self._bus = None
+		self._r_shadow = Multiplexer._Shadow(data_width, shadow_overlaps, name = 'r_shadow')
+		self._w_shadow = Multiplexer._Shadow(data_width, shadow_overlaps, name = 'w_shadow')
 
 	@property
 	def bus(self) -> Interface:
 		if self._bus is None:
 			self._map.freeze()
 			self._bus = Interface(
 				addr_width = self._map.addr_width,
@@ -285,61 +475,89 @@
 			element, size = size, addr = addr, alignment = alignment,
 			extend = extend, name = element.name
 		)
 
 	def elaborate(self, platform) -> Module:
 		m = Module()
 
+		for elem, _, (elem_start, elem_end) in self._map.resources():
+			elem_range = range(elem_start, elem_end)
+			if elem.access.readable():
+				self._r_shadow.add(elem_range)
+			if elem.access.writable():
+				self._w_shadow.add(elem_range)
+
+		self._r_shadow.prepare()
+		self._w_shadow.prepare()
+
 		# Instead of a straightforward multiplexer for reads, use a per-element address comparator,
 		# AND the shadow register chunk with the comparator output, and OR all of those together.
 		# If the toolchain doesn't already synthesize multiplexer trees this way, this trick can
 		# save a significant amount of logic, since e.g. one 4-LUT can pack one 2-MUX, but two
 		# 2-AND or 2-OR gates.
 		r_data_fanin = 0
 
-		for elem, _, (elem_start, elem_end) in self._map.resources():
-			shadow = Signal(elem.width, name = f'{elem.name}__shadow')
-			if elem.access.readable():
-				shadow_en = Signal(elem_end - elem_start, name = f'{elem.name}__shadow_en')
-				m.d.sync += shadow_en.eq(0)
-			if elem.access.writable():
-				m.d.comb += elem.w_data.eq(shadow)
-				m.d.sync += elem.w_stb.eq(0)
+		for chunk_offset, r_chunk, in self._r_shadow.chunks():
+			# Use the same trick to select which element is read into a shadow register chunk.
+			r_chunk_w_en_fanin = 0
+			r_chunk_data_fanin = 0
+
+			m.d.sync += r_chunk.r_en.eq(0)
 
-			# Enumerate every address used by the register explicitly, rather than using
-			# arithmetic comparisons, since some toolchains (e.g. Yosys) are too eager to infer
-			# carry chains for comparisons, even with a constant. (Register sizes don't have
-			# to be powers of 2.)
 			with m.Switch(self.bus.addr):
-				for chunk_offset, chunk_addr in enumerate(range(elem_start, elem_end)):
-					shadow_slice = shadow.word_select(chunk_offset, self.bus.data_width)
+				for elem_range in r_chunk.elements():
+					chunk_addr  = self._r_shadow.encode_offset(chunk_offset, elem_range)
+					elem        = self._map.decode_address(elem_range.start)
+					elem_offset = chunk_addr - elem_range.start
+					elem_slice  = elem.r_data.word_select(elem_offset, self.bus.data_width)
 
 					with m.Case(chunk_addr):
-						if elem.access.readable():
-							r_data_fanin |= Mux(shadow_en[chunk_offset], shadow_slice, 0)
-							if chunk_addr == elem_start:
-								m.d.comb += elem.r_stb.eq(self.bus.r_stb)
-								with m.If(self.bus.r_stb):
-									m.d.sync += shadow.eq(elem.r_data)
-							# Delay by 1 cycle, allowing reads to be pipelined.
-							m.d.sync += shadow_en.eq(self.bus.r_stb << chunk_offset)
-
-						if elem.access.writable():
-							if chunk_addr == elem_end - 1:
-								# Delay by 1 cycle, avoiding combinatorial paths through
-								# the CSR bus and into CSR registers.
-								m.d.sync += elem.w_stb.eq(self.bus.w_stb)
-							with m.If(self.bus.w_stb):
-								m.d.sync += shadow_slice.eq(self.bus.w_data)
+						if chunk_addr == elem_range.start:
+							m.d.comb += elem.r_stb.eq(self.bus.r_stb)
+						# Delay by 1 cycle, allowing reads to be pipelined.
+						m.d.sync += r_chunk.r_en.eq(self.bus.r_stb)
+
+					r_chunk_w_en_fanin |= elem.r_stb
+					r_chunk_data_fanin |= Mux(elem.r_stb, elem_slice, 0)
+
+			m.d.comb += r_chunk.w_en.eq(r_chunk_w_en_fanin)
+			with m.If(r_chunk.w_en):
+				m.d.sync += r_chunk.data.eq(r_chunk_data_fanin)
+
+			r_data_fanin |= Mux(r_chunk.r_en, r_chunk.data, 0)
 
 		m.d.comb += self.bus.r_data.eq(r_data_fanin)
 
+		for chunk_offset, w_chunk in self._w_shadow.chunks():
+			with m.Switch(self.bus.addr):
+				for elem_range in w_chunk.elements():
+					chunk_addr  = self._w_shadow.encode_offset(chunk_offset, elem_range)
+					elem        = self._map.decode_address(elem_range.start)
+					elem_offset = chunk_addr - elem_range.start
+					elem_slice  = elem.w_data.word_select(elem_offset, self.bus.data_width)
+
+					if chunk_addr == elem_range.stop - 1:
+						m.d.sync += elem.w_stb.eq(0)
+
+					with m.Case(chunk_addr):
+						if chunk_addr == elem_range.stop - 1:
+							# Delay by 1 cycle, avoiding combinatorial paths through
+							# the CSR bus and into CSR registers.
+							m.d.sync += elem.w_stb.eq(self.bus.w_stb)
+						m.d.comb += w_chunk.w_en.eq(self.bus.w_stb)
+
+					m.d.comb += elem_slice.eq(w_chunk.data)
+
+			with m.If(w_chunk.w_en):
+				m.d.sync += w_chunk.data.eq(self.bus.w_data)
+
 		return m
 
 
+
 class Decoder(Elaboratable):
 	'''
 	CSR bus decoder.
 
 	An address decoder for subordinate CSR buses.
 
 	Usage
@@ -428,15 +646,16 @@
 		m = Module()
 
 		# See Multiplexer.elaborate above.
 		r_data_fanin = 0
 
 		with m.Switch(self.bus.addr):
 			for sub_map, (sub_pat, sub_ratio) in self._map.window_patterns():
-				assert sub_ratio == 1
+				if sub_ratio != 1:
+					raise ValueError(f'sub_ratio must be exactly 1, not {sub_ratio}')
 
 				sub_bus = self._subs[sub_map]
 				m.d.comb += sub_bus.addr.eq(self.bus.addr[:sub_bus.addr_width])
 
 				# The CSR bus interface is defined to output zero when idle, allowing us to avoid
 				# adding a multiplexer here.
 				r_data_fanin |= sub_bus.r_data
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `torii-0.5.0/torii/lib/soc/csr/event.py` & `torii-0.6.0/torii/lib/soc/csr/event.py`

 * *Files identical despite different names*

### Comparing `torii-0.5.0/torii/lib/soc/csr/wishbone.py` & `torii-0.6.0/torii/lib/soc/csr/wishbone.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # SPDX-License-Identifier: BSD-2-Clause
 
 from typing         import Optional
 
 from ....           import Cat, Elaboratable, Module, Signal
-from ....util.units import log2_int
+from ....util.units import log2_exact
 from ..memory       import MemoryMap
 from ..wishbone     import Interface as WishboneInterface
 from .              import Interface as CSRInterface
 
 __all__ = (
 	'WishboneCSRBridge',
 )
@@ -49,15 +49,15 @@
 		if csr_bus.data_width not in (8, 16, 32, 64):
 			raise ValueError(f'CSR bus data width must be one of 8, 16, 32, 64, not {csr_bus.data_width!r}')
 		if data_width is None:
 			data_width = csr_bus.data_width
 
 		self.csr_bus = csr_bus
 		self.wb_bus  = WishboneInterface(
-			addr_width = max(0, csr_bus.addr_width - log2_int(data_width // csr_bus.data_width)),
+			addr_width = max(0, csr_bus.addr_width - log2_exact(data_width // csr_bus.data_width)),
 			data_width = data_width,
 			granularity = csr_bus.data_width,
 			name = 'wb'
 		)
 
 		wb_map = MemoryMap(
 			addr_width = csr_bus.addr_width,
@@ -72,15 +72,15 @@
 	def elaborate(self, platform) -> Module:
 		csr_bus = self.csr_bus
 		wb_bus  = self.wb_bus
 
 		m = Module()
 
 		cycle = Signal(range(len(wb_bus.sel) + 1))
-		m.d.comb += csr_bus.addr.eq(Cat(cycle[:log2_int(len(wb_bus.sel))], wb_bus.adr))
+		m.d.comb += csr_bus.addr.eq(Cat(cycle[:log2_exact(len(wb_bus.sel))], wb_bus.adr))
 
 		with m.If(wb_bus.cyc & wb_bus.stb):
 			with m.Switch(cycle):
 				def segment(index):
 					return slice(index * wb_bus.granularity, (index + 1) * wb_bus.granularity)
 
 				for index, sel_index in enumerate(wb_bus.sel):
```

### Comparing `torii-0.5.0/torii/lib/soc/event.py` & `torii-0.6.0/torii/lib/soc/event.py`

 * *Files 5% similar despite different names*

```diff
@@ -223,15 +223,15 @@
 			if sub.trigger == Source.Trigger.LEVEL:
 				m.d.comb += sub.trg.eq(sub.i)
 			elif sub.trigger == Source.Trigger.RISE:
 				m.d.comb += sub.trg.eq(~sub_i_r & sub.i)
 			elif sub.trigger == Source.Trigger.FALL:
 				m.d.comb += sub.trg.eq( sub_i_r & ~sub.i)
 			else:
-				assert False # :nocov:
+				raise ValueError(f'Trigger must be Level, Rise, or Fall, not {sub.trigger!r}') # :nocov:
 
 			with m.If(sub.trg):
 				m.d.sync += self.pending[index].eq(1)
 			with m.Elif(self.clear[index]):
 				m.d.sync += self.pending[index].eq(0)
 
 		m.d.comb += self.src.i.eq((self.enable & self.pending).any())
```

### Comparing `torii-0.5.0/torii/lib/soc/memory.py` & `torii-0.6.0/torii/lib/soc/memory.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,20 +21,24 @@
 	def __init__(self) -> None:
 		self._keys   = []
 		self._values = dict()
 		self._starts = []
 		self._stops  = []
 
 	def insert(self, key: range, value: object):
-		assert isinstance(key, range)
-		assert not self.overlaps(key)
+		if not isinstance(key, range):
+			raise TypeError(f'key must be of type \'range\', not \'{type(key)}\'')
+
+		if self.overlaps(key):
+			raise ValueError(f'Key {key} overlaps an existing region!')
 
 		start_idx = bisect_right(self._starts, key.start)
 		stop_idx  = bisect_left(self._stops, key.stop)
-		assert start_idx == stop_idx
+		if start_idx != stop_idx:
+			raise ValueError(f'Start and stop indices are not equivalent: {start_idx} != {stop_idx}')
 
 		self._starts.insert(start_idx, key.start)
 		self._stops.insert(stop_idx, key.stop)
 		self._keys.insert(start_idx, key)
 		self._values[key] = value
 
 	def get(self, point: int) -> object:
@@ -545,18 +549,23 @@
 			pattern = f'{const_pat}{"-" * window.addr_width}'
 			yield (window, (pattern, window_range.step))
 
 	@staticmethod
 	def _translate(
 		resource_info: ResourceInfo, window, window_range: range
 	) -> ResourceInfo:
-		assert (resource_info.end - resource_info.start) % window_range.step == 0
+		if (resource_info.end - resource_info.start) % window_range.step != 0:
+			raise ValueError('Resource range does not fit in the window range step')
+
 		# Accessing a resource through a dense and then a sparse window results in very strange
 		# layouts that cannot be easily represented, so reject those.
-		assert window_range.step == 1 or resource_info.width == window.data_width
+		if window_range.step != 1 and resource_info.width != window.data_width:
+			raise ValueError(
+				'Window range step must be 1 or the resource info width and window data width must be the same!'
+			)
 
 		name  = resource_info.name if window.name is None else (window.name, *resource_info.name)
 		size  = (resource_info.end - resource_info.start) // window_range.step
 		start = resource_info.start + window_range.start
 		width = resource_info.width * window_range.step
 		return ResourceInfo(resource_info.resource, name, start, start + size, width)
 
@@ -579,15 +588,15 @@
 				yield ResourceInfo(
 					assignment, resource_name, addr_range.start, addr_range.stop, self.data_width
 				)
 			elif id(assignment) in self._windows:
 				for resource_info in assignment.all_resources():
 					yield self._translate(resource_info, assignment, addr_range)
 			else:
-				assert False # :nocov:
+				raise ValueError(f'Assignment {assignment!r} not a known resource or in a known window') # :nocov:
 
 	def find_resource(self, resource: object) -> ResourceInfo:
 		'''
 		Find address range corresponding to a resource.
 
 		Recursively find the address range of a resource, performing address translation for
 		resources that are located behind a window.
@@ -641,8 +650,8 @@
 
 		if id(assignment) in self._resources:
 			return assignment
 		elif id(assignment) in self._windows:
 			_, addr_range = self._windows[id(assignment)]
 			return assignment.decode_address((address - addr_range.start) // addr_range.step)
 		else:
-			assert False # :nocov:
+			raise ValueError(f'Address {address} is not a known resource or in a valid address window') # :nocov:
```

### Comparing `torii-0.5.0/torii/lib/soc/periph.py` & `torii-0.6.0/torii/lib/soc/periph.py`

 * *Files identical despite different names*

### Comparing `torii-0.5.0/torii/lib/soc/wishbone/bus.py` & `torii-0.6.0/torii/lib/soc/wishbone/bus.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # SPDX-License-Identifier: BSD-2-Clause
 
 from enum           import Enum
 from typing         import Iterable, Literal, Optional
 
 from ....           import Cat, Elaboratable, Module, Record, Signal
 from ....hdl.rec    import Direction
-from ....util.units import log2_int
+from ....util.units import log2_exact
 from ..memory       import MemoryMap
 
 __all__ = (
 	'Arbiter',
 	'BurstTypeExt',
 	'CycleType',
 	'Decoder',
@@ -166,15 +166,15 @@
 		if not isinstance(memory_map, MemoryMap):
 			raise TypeError(f'Memory map must be an instance of MemoryMap, not {memory_map!r}')
 		if memory_map.data_width != self.granularity:
 			raise ValueError(
 				f'Memory map has data width {memory_map.data_width}, which is not the same as bus '
 				f'interface granularity {self.granularity}'
 			)
-		granularity_bits = log2_int(self.data_width // self.granularity)
+		granularity_bits = log2_exact(self.data_width // self.granularity)
 		if memory_map.addr_width != max(1, self.addr_width + granularity_bits):
 			raise ValueError(
 				f'Memory map has address width {memory_map.addr_width}, which is not the same as bus '
 				f'interface address width {self.addr_width + granularity_bits} ({self.addr_width} '
 				f'address bits + {granularity_bits} granularity bits)'
 			)
 
@@ -202,15 +202,15 @@
 		Window alignment. See :class:`..memory.MemoryMap`
 	name : str
 		Window name. Optional.
 
 	Attributes
 	----------
 	bus : :class:`Interface`
-		CSR bus providing access to subordinate buses.
+		Wishbone bus providing access to subordinate buses.
 
 	'''
 
 	def __init__(
 		self, *, addr_width: int, data_width: int, granularity: Optional[int] = None,
 		features: Iterable[Literal['rty', 'err', 'stall', 'lock', 'cti', 'bte']] = frozenset(),
 		alignment: int = 0, name: Optional[str] = None
@@ -221,28 +221,28 @@
 		_check_interface(addr_width, data_width, granularity, features)
 
 		self.data_width  = data_width
 		self.granularity = granularity
 		self.features    = set(features)
 		self.alignment   = alignment
 
-		granularity_bits = log2_int(data_width // granularity)
+		granularity_bits = log2_exact(data_width // granularity)
 		self._map        = MemoryMap(
 			addr_width = max(1, addr_width + granularity_bits),
 			data_width = granularity, alignment = alignment,
 			name = name
 		)
 		self._subs       = dict()
 		self._bus        = None
 
 	@property
 	def bus(self) -> Interface:
 		if self._bus is None:
 			self._map.freeze()
-			granularity_bits = log2_int(self.data_width // self.granularity)
+			granularity_bits = log2_exact(self.data_width // self.granularity)
 			self._bus = Interface(
 				addr_width = self._map.addr_width - granularity_bits,
 				data_width = self.data_width, granularity = self.granularity,
 				features = self.features
 			)
 			self._bus.memory_map = self._map
 		return self._bus
@@ -314,28 +314,28 @@
 		stall_fanin = 0
 
 		with m.Switch(self.bus.adr):
 			for sub_map, (sub_pat, sub_ratio) in self._map.window_patterns():
 				sub_bus = self._subs[sub_map]
 
 				m.d.comb += [
-					sub_bus.adr.eq(self.bus.adr << log2_int(sub_ratio)),
+					sub_bus.adr.eq(self.bus.adr << log2_exact(sub_ratio)),
 					sub_bus.dat_w.eq(self.bus.dat_w),
 					sub_bus.sel.eq(Cat(sel.replicate(sub_ratio) for sel in self.bus.sel)),
 					sub_bus.we.eq(self.bus.we),
 					sub_bus.stb.eq(self.bus.stb),
 				]
 				if hasattr(sub_bus, 'lock'):
 					m.d.comb += sub_bus.lock.eq(getattr(self.bus, 'lock', 0))
 				if hasattr(sub_bus, 'cti'):
 					m.d.comb += sub_bus.cti.eq(getattr(self.bus, 'cti', CycleType.CLASSIC))
 				if hasattr(sub_bus, 'bte'):
 					m.d.comb += sub_bus.bte.eq(getattr(self.bus, 'bte', BurstTypeExt.LINEAR))
 
-				granularity_bits = log2_int(self.bus.data_width // self.bus.granularity)
+				granularity_bits = log2_exact(self.bus.data_width // self.bus.granularity)
 				with m.Case(sub_pat[:-granularity_bits if granularity_bits > 0 else None]):
 					m.d.comb += [
 						sub_bus.cyc.eq(self.bus.cyc),
 						self.bus.dat_r.eq(sub_bus.dat_r),
 					]
 					ack_fanin |= sub_bus.ack
 					if hasattr(sub_bus, 'err'):
```

### Comparing `torii-0.5.0/torii/lib/stdio/serial.py` & `torii-0.6.0/torii/lib/stdio/serial.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,25 +24,27 @@
 	if parity not in choices:
 		raise ValueError(f'Invalid parity {parity!r}; must be one of {", ".join(choices)}')
 
 
 def _compute_parity_bit(
 	data: Record , parity: Literal['none', 'mark', 'space', 'even', 'odd']
 ) -> Union[Const, Record, bool]:
+	if parity not in ('none', 'mark', 'space', 'even', 'odd'):
+		raise ValueError(f'Parity must be one of \'none\', \'mark\', \'space\', \'even\', or \'odd\', not \'{parity}\'')
+
 	if parity == 'none':
 		return Const(0, 0)
 	if parity == 'mark':
 		return Const(1, 1)
 	if parity == 'space':
 		return Const(0, 1)
 	if parity == 'even':
 		return data.xor()
 	if parity == 'odd':
 		return ~data.xor()
-	assert False
 
 
 def _wire_layout(
 	data_bits: int, parity: Literal['none', 'mark', 'space', 'even', 'odd'] = 'none'
 ) -> list[tuple[str, int]]:
 	return [
 		('start',  1),
```

### Comparing `torii-0.5.0/torii/lib/vendor/lattice/ice40.py` & `torii-0.6.0/torii/lib/vendor/lattice/ice40.py`

 * *Files identical despite different names*

### Comparing `torii-0.5.0/torii/platform/resources/__init__.py` & `torii-0.6.0/torii/platform/resources/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 	PmodHBridgeType5Resource, PmodSPIType2AResource,
 	PmodSPIType2Resource, PmodUARTType3Resource,
 	PmodUARTType4AResource, PmodUARTType4Resource
 )
 from .interface  import (
 	CANResource, DirectUSBResource, I2CResource, IrDAResource,
 	JTAGResource, PS2Resource, SPIResource, UARTResource,
-	ULPIResource
+	ULPIResource, HyperBusResource
 )
 from .memory     import (
 	DDR3Resource, NORFlashResources, QSPIFlashResource,
 	SDCardResources, SDRAMResource, SPIFlashResources,
 	SRAMResource
 )
 from .user       import (
@@ -40,14 +40,15 @@
 	'I2CResource',
 	'IrDAResource',
 	'JTAGResource',
 	'PS2Resource',
 	'SPIResource',
 	'UARTResource',
 	'ULPIResource',
+	'HyperBusResource',
 
 	'DDR3Resource',
 	'NORFlashResources',
 	'QSPIFlashResource',
 	'SDCardResources',
 	'SDRAMResource',
 	'SPIFlashResources',
```

### Comparing `torii-0.5.0/torii/platform/resources/display.py` & `torii-0.6.0/torii/platform/resources/display.py`

 * *Files identical despite different names*

### Comparing `torii-0.5.0/torii/platform/resources/extensions/pmod.py` & `torii-0.6.0/torii/platform/resources/extensions/pmod.py`

 * *Files identical despite different names*

### Comparing `torii-0.5.0/torii/platform/resources/interface.py` & `torii-0.6.0/torii/platform/resources/interface.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 # SPDX-License-Identifier: BSD-2-Clause
 
 from typing   import Literal, Optional, Union
 
-from ...build import Attrs, Clock, Pins, PinsN, Resource, Subsignal
+from ...build import Attrs, Clock, Pins, PinsN, Resource, Subsignal, DiffPairs
 
 __all__ = (
 	'CANResource',
 	'DirectUSBResource',
 	'I2CResource',
 	'IrDAResource',
 	'JTAGResource',
 	'PS2Resource',
 	'SPIResource',
 	'UARTResource',
 	'ULPIResource',
+	'HyperBusResource',
 )
 
 def UARTResource(
 	*args,
 	rx: str, tx: str, rts: Optional[str] = None, cts: Optional[str] = None,
 	dtr: Optional[str] = None, dsr: Optional[str] = None, dcd: Optional[str] = None,
 	ri: Optional[str] = None, conn: Optional[Union[tuple[str, int], str]] = None,
 	attrs: Optional[Attrs] = None, role: Optional[str]  = None
 ) -> Resource:
 
 	if any(line is not None for line in (rts, cts, dtr, dsr, dcd, ri)):
-		assert role in ('dce', 'dte')
+		if role not in ('dce', 'dte'):
+			raise ValueError(f'Invalid role, expected \'dce\' or \'dte\', not \'{role}\'')
 
 	if role == 'dte':
 		dce_to_dte = 'i'
 		dte_to_dce = 'o'
 	else:
 		dce_to_dte = 'o'
 		dte_to_dce = 'i'
@@ -65,15 +67,16 @@
 
 def IrDAResource(
 	number: int, *, rx: str, tx: str, en: Optional[str] = None, sd: Optional[str] = None,
 	conn: Optional[Union[tuple[str, int], int]] = None, attrs: Optional[Attrs] = None
 ) -> Resource:
 	# Exactly one of en (active-high enable) or sd (shutdown, active-low enable) should
 	# be specified, and it is mapped to a logic level en subsignal.
-	assert (en is not None) ^ (sd is not None)
+	if not (en is not None) ^ (sd is not None):
+		raise ValueError('Only en or sd may be specified, not both!')
 
 	io = []
 
 	io.append(Subsignal('rx', Pins(rx, dir = 'i', conn = conn, assert_width = 1)))
 	io.append(Subsignal('tx', Pins(tx, dir = 'o', conn = conn, assert_width = 1)))
 
 	if en is not None:
@@ -94,15 +97,17 @@
 	conn: Optional[Union[tuple[str, int], int]] = None, attrs: Optional[Attrs] = None,
 	role: Literal['controller', 'peripheral'] = 'controller'
 ) -> Resource:
 
 	if role not in ('controller', 'peripheral'):
 		raise ValueError(f'role is expected to be \'controller\' or \'peripheral\', not {role!r}')
 
-	assert copi is not None or cipo is not None # support unidirectional SPI
+	# support unidirectional SPI
+	if copi is None and cipo is None:
+		raise ValueError('Either COPI or CIPO or both must be set, not none')
 
 	io = []
 
 	if role == 'controller':
 		io.append(Subsignal('cs', PinsN(cs_n, dir = 'o', conn = conn)))
 		io.append(Subsignal('clk', Pins(clk, dir = 'o', conn = conn, assert_width = 1)))
 		if copi is not None:
@@ -280,38 +285,97 @@
 		Subsignal('rx_clk', Pins(rxck, dir = 'i', conn = conn, assert_width = 1)),
 		Subsignal('rx_dat', Pins(rxd, dir = 'i', conn = conn)),
 		Subsignal('tx_clk', Pins(txck, dir = 'i', conn = conn, assert_width = 1)),
 		Subsignal('tx_dat', Pins(txd, dir = 'o', conn = conn)),
 	]
 
 	if rx_dv is not None and rx_err is not None:
-		assert rx_ctl is None
+		if rx_ctl is not None:
+			raise ValueError('rx_ctl must be None!')
 		ios.append(Subsignal('rx_dv', Pins(rx_dv, dir = 'i', conn = conn, assert_width = 1)))
 		ios.append(Subsignal('rx_err', Pins(rx_err, dir = 'i', conn = conn, assert_width = 1)))
 	elif rx_ctl is not None:
 		ios.append(Subsignal('rx_ctl', Pins(rx_ctl, dir = 'i', conn = conn, assert_width = 1)))
 	else:
 		raise AssertionError('Must specify either MII RXDV + RXER pins or RGMII RXCTL')
 
 	if tx_en is not None and tx_err is not None:
-		assert tx_ctl is None
+		if tx_ctl is not None:
+			raise ValueError('tx_ctl must be None')
 		ios.append(Subsignal('tx_en', Pins(tx_en, dir = 'o', conn = conn, assert_width = 1)))
 		ios.append(Subsignal('tx_err', Pins(tx_err, dir = 'o', conn = conn, assert_width = 1)))
 		if col is not None:
 			ios.append(Subsignal('col', Pins(col, dir = 'i', conn = conn, assert_width = 1)))
 		if crs is not None:
 			ios.append(Subsignal('crs', Pins(crs, dir = 'i', conn = conn, assert_width = 1)))
 	elif tx_ctl is not None:
-		assert col is None and crs is None
+		if col is not None and crs is not None:
+			raise ValueError('col and crs must not be specified if tx_ctl is')
 		ios.append(Subsignal('tx_ctl', Pins(tx_ctl, dir = 'o', conn = conn, assert_width = 1)))
 	else:
 		raise AssertionError('Must specify either MII TXDV + TXER pins or RGMII TXCTL')
 
 	assert (rx_dv is not None and rx_err is not None) == (tx_en is not None and tx_err is not None)
 	assert (rx_ctl is not None) == (tx_ctl is not None)
 
 	if mdc is not None and mdio is not None:
 		ios.append(Subsignal('mdc', Pins(mdc, dir = 'o', conn = conn, assert_width = 1), mdio_attrs))
 		ios.append(Subsignal('mdio', Pins(mdio, dir = 'io', conn = conn, assert_width = 1), mdio_attrs))
 	if attrs is not None:
 		ios.append(attrs)
 	return Resource.family(*args, default_name = 'eth', ios = ios)
+
+def HyperBusResource(
+	*args, bus_type: Literal['controller', 'peripheral'],
+	cs_n: str, clk_p: str, clk_n: Optional[str], dq: str, rwds: str, rst_n: Optional[str] = None,
+	rsto_n: Optional[str] = None, int_n: Optional[str] = None,
+	conn: Optional[Union[tuple[str, int], int]] = None, diff_attrs = None, attrs: Optional[Attrs] = None,
+):
+	ios = []
+
+
+	ios.append(
+		Subsignal('cs', PinsN(
+			cs_n, dir = 'o' if bus_type == 'controller' else 'i', conn = conn, assert_width = 1
+		)),
+		Subsignal('dq',   Pins(dq, dir = 'io', conn = conn, assert_width = 8)),
+		Subsignal('rwds', Pins(rwds, dir = 'io', conn = conn, assert_width = 1)),
+	)
+
+	if clk_n is None:
+		ios.append(
+			Subsignal('clk', Pins(
+				clk_p, dir = 'o' if bus_type == 'controller' else 'i', conn = conn, assert_width = 1
+			))
+		)
+	else:
+		ios.append(
+			Subsignal('clk', DiffPairs(
+				clk_p, clk_n, dir = 'o' if bus_type == 'controller' else 'i', conn = conn, assert_width = 1
+			), diff_attrs)
+		)
+
+	if rst_n is not None:
+		ios.append(
+			Subsignal('rst', PinsN(
+				rst_n, dir = 'o' if bus_type == 'controller' else 'i', conn = conn, assert_width = 1
+			))
+		)
+
+	if rsto_n is not None:
+		ios.append(
+			Subsignal('rsto', PinsN(
+				rst_n, dir = 'i' if bus_type == 'controller' else 'o', conn = conn, assert_width = 1
+			))
+		)
+
+	if int_n is not None:
+		ios.append(
+			Subsignal('int', PinsN(
+				int_n, dir = 'i' if bus_type == 'controller' else 'o', conn = conn, assert_width = 1
+			))
+		)
+
+	if attrs is not None:
+		ios.append(attrs)
+
+	return Resource.family(*args, default_name = 'hyperbus', ios = ios)
```

### Comparing `torii-0.5.0/torii/platform/resources/memory.py` & `torii-0.6.0/torii/platform/resources/memory.py`

 * *Files 4% similar despite different names*

```diff
@@ -98,28 +98,33 @@
 
 	ios = [
 		Subsignal('cs', PinsN(cs_n, dir = 'o', conn = conn, assert_width = cs_count)),
 		Subsignal('clk', Pins(clk, dir = 'o', conn = conn, assert_width = clk_count)),
 	]
 
 	if mode == QSPIMode.DualParallel:
-		assert dq is None and dq_a is not None and dq_b is not None
+		if dq is not None and (dq_a is None or dq_b is None):
+			raise ValueError(f'\'dq\' must be None and \'dq_a\' and \'dq_b\' must be specified for mode \'{mode}\'')
 		ios.append('dq_a', Pins(dq_a, dir = 'io', conn = conn, assert_width = 4))
 		ios.append('dq_b', Pins(dq_b, dir = 'io', conn = conn, assert_width = 4))
 	else:
-		assert dq is not None and dq_a is None and dq_b is None
+		if dq is None and (dq_a is not None or dq_b is not None):
+			raise ValueError(f'\'dq\' must be specified and \'dq_a\' and \'dq_b\' must be None for mode \'{mode}\'')
+
 		if data_mode == QSPIDataMode.x1:
 			dq = dq.split(' ')
-			assert len(dq) == 3
+			if len(dq) != 3:
+				raise ValueError(f'dq must have exactly 3 pins, not {len(dq)}')
 			ios.append('copi', Pins(dq[0], dir = 'o', conn = conn))
 			ios.append('cipo', Pins(dq[1], dir = 'i', conn = conn))
 			ios.append('hold', PinsN(dq[2], dir = 'io', conn = conn))
 		elif data_mode == QSPIDataMode.x2:
 			dq = dq.split(' ')
-			assert len(dq) == 3
+			if len(dq) != 3:
+				raise ValueError(f'dq must have exactly 3 pins not {len(dq)}')
 			ios.append('dq', Pins(f'{dq[0]} {dq[1]}', dir = 'io', conn = conn))
 			ios.append('hold', PinsN(dq[2], dir = 'io', conn = conn))
 		elif data_mode == QSPIDataMode.x4:
 			ios.append('dq', Pins(dq, dir = 'io', conn = conn, assert_width = 4))
 
 	if clk_fb is not None:
 		ios.append(Subsignal('clk_fb', Pins(clk_fb, dir = 'i', conn = conn, assert_width = 1)))
```

### Comparing `torii-0.5.0/torii/platform/resources/user.py` & `torii-0.6.0/torii/platform/resources/user.py`

 * *Files identical despite different names*

### Comparing `torii-0.5.0/torii/platform/vendor/__init__.py` & `torii-0.6.0/torii/platform/vendor/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # SPDX-License-Identifier: BSD-2-Clause
 
 from .gowin      import GowinPlatform
-from .intel      import IntelPlatform
+from .altera     import AlteraPlatform
 from .lattice    import (
 	LatticeECP5Platform, LatticeICE40Platform, LatticeMachXO2Platform, LatticeMachXO3LPlatform
 )
 from .quicklogic import QuicklogicPlatform
 from .xilinx     import XilinxPlatform
 
 __all__ = (
 	'GowinPlatform',
 
-	'IntelPlatform',
+	'AlteraPlatform',
 
 	'LatticeECP5Platform',
 	'LatticeICE40Platform',
 	'LatticeMachXO2Platform',
 	'LatticeMachXO3LPlatform',
 
 	'QuicklogicPlatform',
```

### Comparing `torii-0.5.0/torii/platform/vendor/gowin.py` & `torii-0.6.0/torii/platform/vendor/gowin.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # SPDX-License-Identifier: BSD-2-Clause
 
 from abc       import abstractproperty
 from fractions import Fraction
 import re
 
-from ...hdl     import *
+from ...hdl     import Const, Module, Instance, Signal, ClockDomain, ClockSignal
 from ...lib.cdc import ResetSynchronizer
-from ...build   import *
+from ...build   import TemplatedPlatform, Clock
 
 # Acknowledgments:
 #   Parts of this file originate from https://github.com/tcjie/Gowin
 
 
 __all__ = (
 	'GowinPlatform',
@@ -165,32 +165,42 @@
 			else:
 				return 250_000_000
 		elif osc in ('OSCF', 'OSCH'):
 			return 240_000_000
 		elif osc == 'OSCW':
 			return 200_000_000
 		else:
-			assert False
+			raise ValueError(
+				'Unknown oscillator, expected \'OSC\', \'OSCZ\', \'OSCO\', \'OSCF\','
+				f' \'OSCH\', or \'OSCW\', not \'{osc}\''
+			)
 
 	@property
 	def _osc_div(self):
-		div_min  = 2
-		div_max  = 128
-		div_step = 2
-		div_frac = Fraction(self._osc_base_freq, self.osc_frequency)
+		div_range = range(2, 130, 2)
+		div_frac  = Fraction(self._osc_base_freq, self.osc_frequency)
 
-		if div_frac.denominator != 1 or div_frac not in range(div_min, div_max, div_step):
+		# Check that the requested frequency is within 50 ppm. This takes care of small mismatches
+		# arising due to rounding. The tolerance of a typical crystal oscillator is 50 ppm.
+		if (abs(round(div_frac) - div_frac) > Fraction(50, 1_000_000) or int(div_frac) not in div_range):
+
+			achievable = (
+				min((frac for frac in div_range if frac > div_frac), default = None),
+				max((frac for frac in div_range if frac < div_frac), default = None)
+			)
 			raise ValueError(
-				'On-chip oscillator frequency (platform.osc_frequency) must be chosen such that '
-				f'the oscillator divider, calculated as ({div_frac.numerator}/{div_frac.denominator}), '
-				f'is an integer between {div_min} and {div_max} in '
-				f'steps of {div_step}'
+				f'On-chip oscillator frequency (platform.osc_frequency) must be chosen such that '
+				f'the base frequency of {self._osc_base_freq} Hz is divided by an integer factor '
+				f'between {div_range.start} and {div_range.stop} in steps of {div_range.step}; '
+				f'the divider for the requested frequency of {self.osc_frequency} Hz was '
+				f'calculated as ({div_frac.numerator}/{div_frac.denominator}), and the closest '
+				f'achievable frequencies are {", ".join(str(self._osc_base_freq // frac) for frac in achievable if frac)}'
 			)
 
-		return div_frac.numerator
+		return int(div_frac)
 
 	# Common templates
 
 	_common_file_templates = {
 		'{{name}}.cst': r'''
 			// {{autogenerated}}
 			{% for port_name, pin_name, attrs in platform.iter_port_constraints_bits() -%}
@@ -228,15 +238,14 @@
 			{% for file in platform.iter_files(".sv") -%}
 				read_verilog -sv {{get_override("read_verilog_opts")|options}} {{file}}
 			{% endfor %}
 			{% for file in platform.iter_files(".il") -%}
 				read_ilang {{file}}
 			{% endfor %}
 			read_ilang {{name}}.il
-			delete w:$verilog_initial_trigger
 			{{get_override("script_after_read")|default("# (script_after_read placeholder)")}}
 			synth_gowin {{get_override("synth_opts")|options}} -top {{name}} -json {{name}}.syn.json
 			{{get_override("script_after_synth")|default("# (script_after_synth placeholder)")}}
 		''',
 	}
 	_apicula_command_templates = [
 		r'''
@@ -293,54 +302,61 @@
 		''',
 		'{{name}}.sdc': r'''
 		// {{autogenerated}}
 		{% for net_signal,port_signal,frequency in platform.iter_clock_constraints() -%}
 			create_clock -name {{port_signal.name|tcl_escape}} -period {{1000000000/frequency}}  [get_ports {{port_signal.name|tcl_escape}}]
 		{% endfor %}
 		{{get_override("add_constraints")|default("# (add_constraints placeholder)")}}
-		''',
+		''', # noqa: E501
 	}
 	_gowin_command_templates = [
 		r'''
 		{{invoke_tool("gw_sh")}}
 			{{name}}.tcl
 		'''
 	]
 
 	def __init__(self, *, toolchain = 'Apicula'):
 		super().__init__()
 
-		assert toolchain in ('Apicula', 'Gowin')
+		if toolchain not in ('Apicula', 'Gowin'):
+			raise ValueError(f'Unknown toolchain \'{toolchain}\', expected \'Apicula\', or \'Gowin\'')
 		self.toolchain = toolchain
 
 		self.parse_part()
 
 	@property
 	def required_tools(self):
+		if self.toolchain not in ('Apicula', 'Gowin'):
+			raise ValueError(f'Unknown toolchain \'{self.toolchain}\', expected \'Apicula\', or \'Gowin\'')
+
 		if self.toolchain == 'Apicula':
 			return self._apicula_required_tools
 		elif self.toolchain == 'Gowin':
 			return self._gowin_required_tools
-		assert False
 
 	@property
 	def file_templates(self):
+		if self.toolchain not in ('Apicula', 'Gowin'):
+			raise ValueError(f'Unknown toolchain \'{self.toolchain}\', expected \'Apicula\', or \'Gowin\'')
+
 		if self.toolchain == 'Apicula':
 			return self._apicula_file_templates
 		elif self.toolchain == 'Gowin':
 			return self._gowin_file_templates
-		assert False
 
 	@property
 	def command_templates(self):
+		if self.toolchain not in ('Apicula', 'Gowin'):
+			raise ValueError(f'Unknown toolchain \'{self.toolchain}\', expected \'Apicula\', or \'Gowin\'')
+
 		if self.toolchain == 'Apicula':
 			return self._apicula_command_templates
 		elif self.toolchain == 'Gowin':
 			return self._gowin_command_templates
-		assert False
 
 	def add_clock_constraint(self, clock, frequency):
 		super().add_clock_constraint(clock, frequency)
 		clock.attrs['keep'] = 'true'
 
 	@property
 	def default_clk_constraint(self):
@@ -517,15 +533,15 @@
 			if 'i' in pin.dir:
 				get_iddr(pin.i_clk, i, pin_i0, pin_i1)
 			if pin.dir in ('o', ):
 				get_oddr(pin.o_clk, pin_o0, pin_o1, o, )
 			if pin.dir in ('oe', 'io'):
 				get_oeddr(pin.o_clk, pin_o0, pin_o1, ~pin.oe, o, t)
 		else:
-			assert False
+			raise ValueError(f'Invalid gearing {pin.xdr} for pin {pin.name}, must be 0, 1, or 2')
 
 		return (i, o, t)
 
 	def get_input(self, pin, port, attrs, invert):
 		self._check_feature(
 			'single-ended input', pin, attrs, valid_xdrs = (0, 1, 2), valid_attrs = True
 		)
@@ -586,15 +602,15 @@
 
 	def get_diff_input(self, pin, port, attrs, invert):
 		self._check_feature(
 			'differential input', pin, attrs, valid_xdrs = (0, 1, 2), valid_attrs = True
 		)
 		m = Module()
 		i, o, t = self._get_xdr_buffer(m, pin, i_invert = invert)
-		for bit in range(pin.wodth):
+		for bit in range(pin.width):
 			m.submodules[f'{pin.name}_{bit}'] = Instance(
 				'TLVDS_IBUF',
 				i_I  = port.p[bit],
 				i_IB = port.n[bit],
 				o_O  = i[bit]
 			)
 		return m
```

### Comparing `torii-0.5.0/torii/platform/vendor/intel.py` & `torii-0.6.0/torii/platform/vendor/altera.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 from ...build  import Attrs, Clock, TemplatedPlatform
 from ...hdl    import (
 	ClockDomain, ClockSignal, Const, Instance, Module, Record, Signal
 )
 from ...lib.io import Pin
 
 __all__ = (
-	'IntelPlatform',
+	'AlteraPlatform',
 )
 
-class IntelPlatform(TemplatedPlatform):
+class AlteraPlatform(TemplatedPlatform):
 	'''
 	.. rubric:: Quartus toolchain
 
 	Required tools:
 		* ``quartus_map``
 		* ``quartus_fit``
 		* ``quartus_asm``
@@ -82,15 +82,15 @@
 	# Quartus templates
 
 	quartus_suppressed_warnings = [
 		10264,  # All case item expressions in this case statement are onehot
 		10270,  # Incomplete Verilog case statement has no default case item
 		10335,  # Unrecognized synthesis attribute
 		10763,  # Verilog case statement has overlapping case item expressions with non-constant or don't care bits
-		10935,  # Verilog casex/casez overlaps with a previous casex/vasez item expression
+		10935,  # Verilog casex/casez overlaps with a previous casex/casez item expression
 		12125,  # Using design file which is not specified as a design file for the current project, but contains
 				# definitions used in project
 		18236,  # Number of processors not specified in QSF
 		292013, # Feature is only available with a valid subscription license
 	]
 
 	quartus_required_tools = [
@@ -99,14 +99,15 @@
 		'quartus_asm',
 		'quartus_sta',
 	]
 
 	quartus_file_templates = {
 		**TemplatedPlatform.build_script_templates,
 		'build_{{name}}.sh': r'''
+			#!/bin/bash
 			# {{autogenerated}}
 			if [ -n "${{platform._toolchain_env_var}}" ]; then
 				QUARTUS_ROOTDIR=$(dirname $(dirname "${{platform._toolchain_env_var}}"))
 				# Quartus' qenv.sh does not work with `set -e`.
 				. "${{platform._toolchain_env_var}}"
 			fi
 			set -e{{verbose("x")}}
@@ -214,15 +215,14 @@
 			{% for file in platform.iter_files(".sv") -%}
 				read_verilog -sv {{get_override("read_verilog_opts")|options}} {{file}}
 			{% endfor %}
 			{% for file in platform.iter_files(".il") -%}
 				read_rtlil {{file}}
 			{% endfor %}
 			read_rtlil {{name}}.il
-			delete w:$verilog_initial_trigger
 			{{get_override("script_after_read")|default("# (script_after_read placeholder)")}}
 			synth_intel_alm {{get_override("synth_opts")|options}} -top {{name}}
 			{{get_override("script_after_synth")|default("# (script_after_synth placeholder)")}}
 			write_json {{name}}.json
 		''',
 		'{{name}}.qsf': r'''
 			# {{autogenerated}}
@@ -258,61 +258,72 @@
 	# Common logic
 
 	def __init__(
 		self, *, toolchain: Literal['Quartus', 'Mistral'] = 'Quartus'
 	) -> None:
 		super().__init__()
 
-		assert toolchain in ('Quartus', 'Mistral')
+		if toolchain not in ('Quartus', 'Mistral'):
+			raise ValueError(f'Unknown toolchain {toolchain}, expected either \'Quartus\' or \'Mistral\'')
 		self.toolchain = toolchain
 
 	@property
 	def required_tools(self) -> list[str]:
+		if self.toolchain not in ('Quartus', 'Mistral'):
+			raise ValueError(f'Unknown toolchain {self.toolchain}, expected either \'Quartus\' or \'Mistral\'')
+
 		if self.toolchain == 'Quartus':
 			return self.quartus_required_tools
 		if self.toolchain == 'Mistral':
 			return self.mistral_required_tools
-		assert False
 
 	@property
 	def file_templates(self) -> dict[str, str]:
+		if self.toolchain not in ('Quartus', 'Mistral'):
+			raise ValueError(f'Unknown toolchain {self.toolchain}, expected either \'Quartus\' or \'Mistral\'')
+
 		if self.toolchain == 'Quartus':
 			return self.quartus_file_templates
 		if self.toolchain == 'Mistral':
 			return self.mistral_file_templates
-		assert False
 
 	@property
 	def command_templates(self) -> list[str]:
+		if self.toolchain not in ('Quartus', 'Mistral'):
+			raise ValueError(f'Unknown toolchain {self.toolchain}, expected either \'Quartus\' or \'Mistral\'')
+
 		if self.toolchain == 'Quartus':
 			return self.quartus_command_templates
 		if self.toolchain == 'Mistral':
 			return self.mistral_command_templates
-		assert False
 
 	def add_clock_constraint(self, clock: Signal, frequency: Union[int, float]) -> None:
 		super().add_clock_constraint(clock, frequency)
 		clock.attrs['keep'] = 'true'
 
 	@property
 	def default_clk_constraint(self) -> Clock:
 		# Internal high-speed oscillator on Cyclone V devices.
 		# It is specified to not be faster than 100MHz, but the actual
 		# frequency seems to vary a lot between devices. Measurements
 		# of 78 to 84 MHz have been observed.
 		if self.default_clk == 'cyclonev_oscillator':
-			assert self.device.startswith('5C')
+			if not self.device.startswith('5C'):
+				raise ValueError(f'Device {self.device} does not support the \'cyclonev_oscillator\' as a clock source')
+
 			return Clock(100e6)
 		# Otherwise, use the defined Clock resource.
 		return super().default_clk_constraint
 
 	def create_missing_domain(self, name: str) -> Module:
 		if name == 'sync' and self.default_clk == 'cyclonev_oscillator':
 			# Use the internal high-speed oscillator for Cyclone V devices
-			assert self.device.startswith('5C')
+			if not self.device.startswith('5C'):
+				raise ValueError(f'Device {self.device} does not support the \'cyclonev_oscillator\' as a clock source')
+
 			m = Module()
 			m.domains += ClockDomain('sync')
 			m.submodules += Instance(
 				'cyclonev_oscillator',
 				i_oscena = Const(1),
 				o_clkout = ClockSignal('sync')
 			)
@@ -356,15 +367,16 @@
 				p_width = pin.width,
 				i_datain = i_ddr,
 				i_inclock = pin.i_clk,
 				o_dataout_h = get_ineg(pin.i0),
 				o_dataout_l = get_ineg(pin.i1),
 			)
 			return i_ddr
-		assert False
+		raise ValueError(f'Invalid gearing {pin.xdr} for pin {pin.name}, must be either 0, 1, or 2')
+
 
 	@staticmethod
 	def _get_oreg(m: Module, pin: Pin, invert: bool) -> Signal:
 		def get_oneg(o: Signal):
 			if invert:
 				o_neg = Signal.like(o, name_suffix = '_neg')
 				m.d.comb += o_neg.eq(~o)
@@ -392,15 +404,16 @@
 				p_width = pin.width,
 				o_dataout = o_ddr,
 				i_outclock = pin.o_clk,
 				i_datain_h = get_oneg(pin.o0),
 				i_datain_l = get_oneg(pin.o1),
 			)
 			return o_ddr
-		assert False
+		raise ValueError(f'Invalid gearing {pin.xdr} for pin {pin.name}, must be either 0, 1, or 2')
+
 
 	@staticmethod
 	def _get_oereg(m: Module, pin: Pin) -> Signal:
 		# altiobuf_ requires an output enable signal for each pin, but pin.oe is 1 bit wide.
 		if pin.xdr == 0:
 			return pin.oe.replicate(pin.width)
 		elif pin.xdr in (1, 2):
@@ -411,15 +424,15 @@
 				p_CLK_POLARITY = 1,
 				p_WIDTH = pin.width,
 				i_CLK = pin.o_clk,
 				i_D = pin.oe,
 				o_Q = oe_reg,
 			)
 			return oe_reg
-		assert False
+		raise ValueError(f'Invalid gearing {pin.xdr} for pin {pin.name}, must be either 0, 1, or 2')
 
 	def get_input(self, pin: Pin, port: Record, attrs: Attrs, invert: bool) -> Module:
 		self._check_feature(
 			'single-ended input', pin, attrs, valid_xdrs = (0, 1, 2), valid_attrs = True
 		)
 
 		if pin.xdr == 1:
```

### Comparing `torii-0.5.0/torii/platform/vendor/lattice/__init__.py` & `torii-0.6.0/torii/platform/vendor/lattice/__init__.py`

 * *Files identical despite different names*

### Comparing `torii-0.5.0/torii/platform/vendor/lattice/ecp5.py` & `torii-0.6.0/torii/platform/vendor/lattice/ecp5.py`

 * *Files 4% similar despite different names*

```diff
@@ -135,15 +135,14 @@
 			{% for file in platform.iter_files(".sv") -%}
 				read_verilog -sv {{get_override("read_verilog_opts")|options}} {{file}}
 			{% endfor %}
 			{% for file in platform.iter_files(".il") -%}
 				read_rtlil {{file}}
 			{% endfor %}
 			read_rtlil {{name}}.il
-			delete w:$verilog_initial_trigger
 			{{get_override("script_after_read")|default("# (script_after_read placeholder)")}}
 			synth_ecp5 {{get_override("synth_opts")|options}} -top {{name}}
 			{{get_override("script_after_synth")|default("# (script_after_synth placeholder)")}}
 			write_json {{name}}.json
 		''',
 		'{{name}}.lpf': r'''
 			# {{autogenerated}}
@@ -201,14 +200,15 @@
 	_diamond_required_tools = [
 		'pnmainc',
 		'ddtcmd',
 	]
 	_diamond_file_templates = {
 		**TemplatedPlatform.build_script_templates,
 		'build_{{name}}.sh': r'''
+			#!/bin/sh
 			# {{autogenerated}}
 			set -e{{verbose("x")}}
 			if [ -z "$BASH" ] ; then exec /bin/bash "$0" "$@"; fi
 			if [ -n "${{platform._toolchain_env_var}}" ]; then
 				bindir=$(dirname "${{platform._toolchain_env_var}}")
 				. "${{platform._toolchain_env_var}}"
 			fi
@@ -287,40 +287,48 @@
 	# Common logic
 
 	def __init__(
 		self, *, toolchain: Literal['Trellis', 'Diamond'] = 'Trellis'
 	) -> None:
 		super().__init__()
 
-		assert toolchain in ('Trellis', 'Diamond')
+		if toolchain not in ('Trellis', 'Diamond'):
+			raise ValueError(f'Unknown toolchain \'{self.toolchain}\', must be either \'Trellis\', or \'Diamond\'')
+
 		self.toolchain = toolchain
 
 	@property
 	def required_tools(self) -> list[str]:
+		if self.toolchain not in ('Trellis', 'Diamond'):
+			raise ValueError(f'Unknown toolchain \'{self.toolchain}\', must be either \'Trellis\', or \'Diamond\'')
+
 		if self.toolchain == 'Trellis':
 			return self._trellis_required_tools
 		if self.toolchain == 'Diamond':
 			return self._diamond_required_tools
-		assert False
 
 	@property
 	def file_templates(self) -> dict[str, str]:
+		if self.toolchain not in ('Trellis', 'Diamond'):
+			raise ValueError(f'Unknown toolchain \'{self.toolchain}\', must be either \'Trellis\', or \'Diamond\'')
+
 		if self.toolchain == 'Trellis':
 			return self._trellis_file_templates
 		if self.toolchain == 'Diamond':
 			return self._diamond_file_templates
-		assert False
 
 	@property
 	def command_templates(self) -> list[str]:
+		if self.toolchain not in ('Trellis', 'Diamond'):
+			raise ValueError(f'Unknown toolchain \'{self.toolchain}\', must be either \'Trellis\', or \'Diamond\'')
+
 		if self.toolchain == 'Trellis':
 			return self._trellis_command_templates
 		if self.toolchain == 'Diamond':
 			return self._diamond_command_templates
-		assert False
 
 	@property
 	def default_clk_constraint(self) -> Clock:
 		if self.default_clk == 'OSCG':
 			return Clock(310e6 / self.oscg_div)
 		return super().default_clk_constraint
 
@@ -616,15 +624,15 @@
 			if 'i' in pin.dir:
 				get_iddr71b(pin.i_clk, pin.i_fclk, i, pin_i0, pin_i1, pin_i2, pin_i3, pin_i4, pin_i5, pin_i6)
 			if 'o' in pin.dir:
 				get_oddr71b(pin.o_clk, pin.o_fclk, pin_o0, pin_o1, pin_o2, pin_o3, pin_o4, pin_o5, pin_o6, o)
 			if pin.dir in ('oe', 'io'):
 				get_oereg(pin.o_clk, ~pin.oe, t)
 		else:
-			assert False
+			raise ValueError(f'Invalid gearing {pin.xdr} for pin {pin.name}, must be one of, 0, 1, 2, 4, or 7')
 
 		return (i, o, t)
 
 	def get_input(self, pin: Pin, port: Record, attrs: Attrs, invert: bool) -> Module:
 		self._check_feature(
 			'single-ended input', pin, attrs, valid_xdrs = (0, 1, 2, 4, 7), valid_attrs = True
 		)
```

### Comparing `torii-0.5.0/torii/platform/vendor/lattice/ice40.py` & `torii-0.6.0/torii/platform/vendor/lattice/ice40.py`

 * *Files 5% similar despite different names*

```diff
@@ -133,15 +133,14 @@
 			{% for file in platform.iter_files(".sv") -%}
 				read_verilog -sv {{get_override("read_verilog_opts")|options}} {{file}}
 			{% endfor %}
 			{% for file in platform.iter_files(".il") -%}
 				read_rtlil {{file}}
 			{% endfor %}
 			read_rtlil {{name}}.il
-			delete w:$verilog_initial_trigger
 			{{get_override("script_after_read")|default("# (script_after_read placeholder)")}}
 			synth_ice40 {{get_override("synth_opts")|options}} -top {{name}}
 			{{get_override("script_after_synth")|default("# (script_after_synth placeholder)")}}
 			write_json {{name}}.json
 		''',
 		'{{name}}.pcf': r'''
 			# {{autogenerated}}
@@ -190,14 +189,15 @@
 		'synthesis',
 		'synpwrap',
 		'tclsh',
 	]
 	_icecube2_file_templates = {
 		**TemplatedPlatform.build_script_templates,
 		'build_{{name}}.sh': r'''
+			#!/bin/sh
 			# {{autogenerated}}
 			set -e{{verbose("x")}}
 			if [ -n "${{platform._toolchain_env_var}}" ]; then
 				# LSE environment
 				export LD_LIBRARY_PATH=${{platform._toolchain_env_var}}/LSE/bin/lin64:$LD_LIBRARY_PATH
 				export PATH=${{platform._toolchain_env_var}}/LSE/bin/lin64:$PATH
 				export FOUNDRY=${{platform._toolchain_env_var}}/LSE
@@ -302,58 +302,87 @@
 	# Common logic
 
 	def __init__(
 		self, *, toolchain: Literal['IceStorm', 'LSE-iCECube2', 'Synplify-iCECube2'] = 'IceStorm'
 	) -> None:
 		super().__init__()
 
-		assert toolchain in ('IceStorm', 'LSE-iCECube2', 'Synplify-iCECube2')
+		if toolchain not in ('IceStorm', 'LSE-iCECube2', 'Synplify-iCECube2'):
+			raise ValueError(
+				f'Unknown toolchain \'{toolchain}\', must be either'
+				' \'IceStorm\', \'LSE-iCECube2\', or \'Synplify-iCECube2\''
+			)
+
 		self.toolchain = toolchain
 
 	@property
 	def family(self) -> str:
+		if not (self.device.startswith('iCE40') or self.device.startswith('iCE5')):
+			raise ValueError(f'Unknown iCE40 device \'{self.device}\'')
+
 		if self.device.startswith('iCE40'):
 			return 'iCE40'
 		if self.device.startswith('iCE5'):
 			return 'iCE5'
-		assert False
+
 
 	@property
 	def _toolchain_env_var(self) -> str:
+		if self.toolchain not in ('IceStorm', 'LSE-iCECube2', 'Synplify-iCECube2'):
+			raise ValueError(
+				f'Unknown toolchain \'{self.toolchain}\', must be either'
+				' \'IceStorm\', \'LSE-iCECube2\', or \'Synplify-iCECube2\''
+			)
+
 		if self.toolchain in ('LSE-iCECube2', 'Synplify-iCECube2'):
 			return 'TORII_ENV_iCECube2'
 		elif self.toolchain == 'IceStorm':
 			return super()._toolchain_env_var
-		assert False
 
 	@property
 	def required_tools(self) -> list[str]:
+		if self.toolchain not in ('IceStorm', 'LSE-iCECube2', 'Synplify-iCECube2'):
+			raise ValueError(
+				f'Unknown toolchain \'{self.toolchain}\', must be either'
+				' \'IceStorm\', \'LSE-iCECube2\', or \'Synplify-iCECube2\''
+			)
+
 		if self.toolchain == 'IceStorm':
 			return self._icestorm_required_tools
 		if self.toolchain in ('LSE-iCECube2', 'Synplify-iCECube2'):
 			return self._icecube2_required_tools
-		assert False
 
 	@property
 	def file_templates(self) -> dict[str, str]:
+		if self.toolchain not in ('IceStorm', 'LSE-iCECube2', 'Synplify-iCECube2'):
+			raise ValueError(
+				f'Unknown toolchain \'{self.toolchain}\', must be either'
+				' \'IceStorm\', \'LSE-iCECube2\', or \'Synplify-iCECube2\''
+			)
+
 		if self.toolchain == 'IceStorm':
 			return self._icestorm_file_templates
 		if self.toolchain in ('LSE-iCECube2', 'Synplify-iCECube2'):
 			return self._icecube2_file_templates
-		assert False
 
 	@property
 	def command_templates(self) -> list[str]:
+		if self.toolchain not in ('IceStorm', 'LSE-iCECube2', 'Synplify-iCECube2'):
+			raise ValueError(
+				f'Unknown toolchain \'{self.toolchain}\', must be either'
+				' \'IceStorm\', \'LSE-iCECube2\', or \'Synplify-iCECube2\''
+			)
+
 		if self.toolchain == 'IceStorm':
 			return self._icestorm_command_templates
 		if self.toolchain == 'LSE-iCECube2':
 			return self._lse_icecube2_command_templates
 		if self.toolchain == 'Synplify-iCECube2':
 			return self._synplify_icecube2_command_templates
-		assert False
+
 
 	@property
 	def default_clk_constraint(self) -> Clock:
 		# Internal high-speed oscillator: 48 MHz / (2 ^ div)
 		if self.default_clk == 'SB_HFOSC':
 			return Clock(48e6 / 2 ** self.hfosc_div)
 		# Internal low-speed oscillator: 10 KHz
@@ -509,15 +538,17 @@
 				return a
 
 		if 'GLOBAL' in attrs:
 			is_global_input = bool(attrs['GLOBAL'])
 			del attrs['GLOBAL']
 		else:
 			is_global_input = False
-		assert not (is_global_input and i_invert)
+
+		if is_global_input and i_invert:
+			raise ValueError(f'Pin {pin.name} must not be a global input and inverted')
 
 		if 'i' in pin.dir:
 			if pin.xdr < 2:
 				pin_i  = get_ineg(pin.i,  i_invert)
 			elif pin.xdr == 2:
 				pin_i0 = get_ineg(pin.i0, i_invert)
 				pin_i1 = get_ineg(pin.i1, i_invert)
```

### Comparing `torii-0.5.0/torii/platform/vendor/lattice/machxo_2_3l.py` & `torii-0.6.0/torii/platform/vendor/lattice/machxo_2_3l.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,14 +70,15 @@
 	required_tools = [
 		'pnmainc',
 		'ddtcmd'
 	]
 	file_templates = {
 		**TemplatedPlatform.build_script_templates,
 		'build_{{name}}.sh': r'''
+			#!/bin/bash
 			# {{autogenerated}}
 			set -e{{verbose("x")}}
 			if [ -z "$BASH" ] ; then exec /bin/bash "$0" "$@"; fi
 			if [ -n "${{platform._toolchain_env_var}}" ]; then
 				bindir=$(dirname "${{platform._toolchain_env_var}}")
 				. "${{platform._toolchain_env_var}}"
 			fi
@@ -177,15 +178,20 @@
 	]
 
 	@property
 	def default_clk_constraint(self) -> Clock:
 		# Internal high-speed oscillator on MachXO2/MachXO3L devices.
 		# It can have a range of frequencies.
 		if self.default_clk == 'OSCH':
-			assert self.osch_frequency in self._supported_osch_freqs
+			if self.osch_frequency not in self._supported_osch_freqs:
+				raise ValueError(
+					f'Invalid OSCH frequency \'{self.osch_frequency}\','
+					f' must be one of {", ".join(self._supported_osch_freqs)}'
+				)
+
 			return Clock(int(self.osch_frequency * 1e6))
 		# Otherwise, use the defined Clock resource.
 		return super().default_clk_constraint
 
 	def create_missing_domain(self, name: str) -> Module:
 		# Lattice MachXO2/MachXO3L devices have two global set/reset signals: PUR, which is driven at
 		# startup by the configuration logic and unconditionally resets every storage element,
@@ -369,15 +375,15 @@
 				get_oddr(pin.o_clk, pin_o0, pin_o1, o)
 			if pin.dir in ('oe', 'io'):
 				# It looks like Diamond will not pack an OREG as a tristate register in a DDR PIO.
 				# It is not clear what is the recommended set of primitives for this task.
 				# Similarly, nextpnr will not pack anything as a tristate register in a DDR PIO.
 				get_oreg(pin.o_clk, ~pin.oe, t)
 		else:
-			assert False
+			raise ValueError(f'Invalid gearing {pin.xdr} for pin {pin.name}, must be either 0, 1, or 2')
 
 		return (i, o, t)
 
 	def get_input(self, pin: Pin, port: Record, attrs: Attrs, invert: bool) -> Module:
 		self._check_feature(
 			'single-ended input', pin, attrs, valid_xdrs = (0, 1, 2), valid_attrs = True
 		)
```

### Comparing `torii-0.5.0/torii/platform/vendor/quicklogic.py` & `torii-0.6.0/torii/platform/vendor/quicklogic.py`

 * *Files identical despite different names*

### Comparing `torii-0.5.0/torii/platform/vendor/xilinx.py` & `torii-0.6.0/torii/platform/vendor/xilinx.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,14 +161,15 @@
 
 	# Vivado templates
 
 	_vivado_required_tools = [ 'vivado' ]
 	_vivado_file_templates = {
 		**TemplatedPlatform.build_script_templates,
 		'build_{{name}}.sh': r'''
+			#!/bin/sh
 			# {{autogenerated}}
 			set -e{{verbose("x")}}
 			if [ -z "$BASH" ] ; then exec /bin/bash "$0" "$@"; fi
 			[ -n "${{platform._toolchain_env_var}}" ] && . "${{platform._toolchain_env_var}}"
 			{{emit_commands("sh")}}
 		''',
 		'{{name}}.v': r'''
@@ -267,14 +268,15 @@
 		'map',
 		'par',
 		'bitgen',
 	]
 	_ise_file_templates = {
 		**TemplatedPlatform.build_script_templates,
 		'build_{{name}}.sh': r'''
+			#!/bin/sh
 			# {{autogenerated}}
 			set -e{{verbose("x")}}
 			if [ -z "$BASH" ] ; then exec /bin/bash "$0" "$@"; fi
 			[ -n "${{platform._toolchain_env_var}}" ] && . "${{platform._toolchain_env_var}}"
 			{{emit_commands("sh")}}
 		''',
 		'{{name}}.v': r'''
@@ -474,14 +476,15 @@
 		'fasm2frames',
 		'xc7frames2bit'
 	]
 
 	_yosys_nextpnr_file_templates = {
 		**TemplatedPlatform.build_script_templates,
 		'build_{{name}}.sh': r'''
+			#!/bin/sh
 			# {{autogenerated}}
 			set -e{{verbose("x")}}
 			if [ -z "$BASH" ] ; then exec /bin/bash "$0" "$@"; fi
 			[ -n "${{platform._toolchain_env_var}}" ] && . "${{platform._toolchain_env_var}}"
 			{{emit_commands("sh")}}
 		''',
 		'{{name}}.v': r'''
@@ -521,15 +524,15 @@
 	}
 
 	_yosys_nextpnr_command_templates = [
 		r'''
 		PRJXRAY_DB_DIR={{get_override("prjxray_db_dir")|default("/usr/share/nextpnr/prjxray-db")}}
 		''',
 		r'''
-		NEXPNR_CHIPDB_DIR={{get_override("nextpnr_db_dir")|default("/usr/share/nextpnr/xilinx-chipdb")}}
+		NEXTPNR_CHIPDB_DIR={{get_override("nextpnr_db_dir")|default("/usr/share/nextpnr/xilinx-chipdb")}}
 		''',
 		r'''
 		PART={{platform._yosys_nextpnr_part_map.get(platform._part, platform._part)}}
 		''',
 		r'''
 		FAMILY={{platform._yosys_nextpnr_family[platform.device[:4]]}}
 		''',
@@ -541,15 +544,15 @@
 			{{name}}.ys
 		''',
 		r'''
 		{{invoke_tool("nextpnr-xilinx")}}
 			{{quiet("--quiet")}}
 			{{get_override("nextpnr_xilinx_opts")|options}}
 			--log {{name}}.tim
-			--chipdb "$NEXPNR_CHIPDB_DIR/$PART.bin"
+			--chipdb "$NEXTPNR_CHIPDB_DIR/$PART.bin"
 			--xdc {{name}}.xdc
 			--json {{name}}.json
 			--write {{name}}_routed.json
 			--fasm {{name}}.fasm
 		''',
 		r'''
 		{{invoke_tool("fasm2frames")}}
@@ -636,15 +639,20 @@
 		}
 		if toolchain is None:
 			if self.family in ISE_FAMILIES:
 				toolchain = 'ISE'
 			else:
 				toolchain = 'Vivado'
 
-		assert toolchain in ('Vivado', 'ISE', 'Symbiflow', 'yosys_nextpnr')
+		if toolchain not in ('Vivado', 'ISE', 'Symbiflow', 'yosys_nextpnr'):
+			raise ValueError(
+				f'Unknown toolchain {toolchain}, must be one of '
+				'\'Vivado\', \'ISE\', \'Symbiflow\', or \'yosys_nextpnr\''
+			)
+
 		if toolchain == 'Vivado':
 			if self.family in ISE_FAMILIES:
 				raise ValueError(f'Family \'{self.family}\' is not supported by the Vivado toolchain, please use ISE instead')
 		elif toolchain == 'ISE':
 			if self.family not in ISE_FAMILIES and self.family != "series7":
 				raise ValueError(f'Family \'{self.family}\' is not supported by the ISE toolchain, please use Vivado instead')
 		elif toolchain == "Symbiflow":
@@ -653,47 +661,63 @@
 		elif toolchain == 'yosys_nextpnr':
 			if self.family != 'series7':
 				raise ValueError(f'Family \'{self.family}\' is not supported by the yosys nextpnr toolchain')
 		self.toolchain = toolchain
 
 	@property
 	def required_tools(self) -> list[str]:
+		if self.toolchain not in ('Vivado', 'ISE', 'Symbiflow', 'yosys_nextpnr'):
+			raise ValueError(
+				f'Unknown toolchain {self.toolchain}, must be one of '
+				'\'Vivado\', \'ISE\', \'Symbiflow\', or \'yosys_nextpnr\''
+			)
+
 		if self.toolchain == 'Vivado':
 			return self._vivado_required_tools
 		if self.toolchain == 'ISE':
 			return self._ise_required_tools
 		if self.toolchain == 'Symbiflow':
 			return self._symbiflow_required_tools
 		if self.toolchain == 'yosys_nextpnr':
 			return self._yosys_nextpnr_required_tools
-		assert False
+
 
 	@property
 	def file_templates(self) -> dict[str, str]:
+		if self.toolchain not in ('Vivado', 'ISE', 'Symbiflow', 'yosys_nextpnr'):
+			raise ValueError(
+				f'Unknown toolchain {self.toolchain}, must be one of '
+				'\'Vivado\', \'ISE\', \'Symbiflow\', or \'yosys_nextpnr\''
+			)
+
 		if self.toolchain == 'Vivado':
 			return self._vivado_file_templates
 		if self.toolchain == 'ISE':
 			return self._ise_file_templates
 		if self.toolchain == 'Symbiflow':
 			return self._symbiflow_file_templates
 		if self.toolchain == 'yosys_nextpnr':
 			return self._yosys_nextpnr_file_templates
-		assert False
 
 	@property
 	def command_templates(self) -> list[str]:
+		if self.toolchain not in ('Vivado', 'ISE', 'Symbiflow', 'yosys_nextpnr'):
+			raise ValueError(
+				f'Unknown toolchain {self.toolchain}, must be one of '
+				'\'Vivado\', \'ISE\', \'Symbiflow\', or \'yosys_nextpnr\''
+			)
+
 		if self.toolchain == 'Vivado':
 			return self._vivado_command_templates
 		if self.toolchain == 'ISE':
 			return self._ise_command_templates
 		if self.toolchain == 'Symbiflow':
 			return self._symbiflow_command_templates
 		if self.toolchain == 'yosys_nextpnr':
 			return self._yosys_nextpnr_command_templates
-		assert False
 
 	def create_missing_domain(self, name: str) -> Module:
 		# Xilinx devices have a global write enable (GWE) signal that asserted during configuration
 		# and de-asserted once it ends. Because it is an asynchronous signal (GWE is driven by logic
 		# synchronous to configuration clock, which is not used by most designs), even though it is
 		# a low-skew global network, its de-assertion may violate a setup/hold constraint with
 		# relation to a user clock. The recommended solution is to use a BUFGCE driven by the EOS
@@ -807,30 +831,34 @@
 					i_CE = Const(1),
 					i_CLR = Const(0),
 					i_D = d[bit],
 					o_Q = q[bit]
 				)
 
 		def get_ifddr(clk: Signal, io: Signal, q0: Signal, q1: Signal) -> None:
-			assert self.family in XFDDR_FAMILIES
+			if self.family not in XFDDR_FAMILIES:
+				raise ValueError(f'Family {self.family} is not IFDDR capable')
+
 			for bit in range(len(q0)):
 				m.submodules += Instance(
 					'IFDDRCPE',
 					i_C0 = clk,
 					i_C1 = ~clk,
 					i_CE = Const(1),
 					i_CLR = Const(0),
 					i_PRE = Const(0),
 					i_D = io[bit],
 					o_Q0 = q0[bit],
 					o_Q1 = q1[bit]
 				)
 
 		def get_iddr2(clk: Signal, d: Signal, q0: Signal, q1: Signal, alignment) -> None:
-			assert self.family in XDDR2_FAMILIES
+			if self.family not in XDDR2_FAMILIES:
+				raise ValueError(f'Family {self.family} is not IDDR2 capable')
+
 			for bit in range(len(q0)):
 				m.submodules += Instance(
 					'IDDR2',
 					p_DDR_ALIGNMENT = alignment,
 					p_SRTYPE = 'ASYNC',
 					p_INIT_Q0 = Const(0, 1),
 					p_INIT_Q1 = Const(0, 1),
@@ -841,15 +869,17 @@
 					i_R = Const(0),
 					i_D = d[bit],
 					o_Q0 = q0[bit],
 					o_Q1 = q1[bit]
 				)
 
 		def get_iddr(clk: Signal, d: Signal, q1: Signal, q2: Signal) -> None:
-			assert self.family in XDDR_FAMILIES or self.family in XDDRE1_FAMILIES
+			if self.family not in XDDR_FAMILIES or self.family not in XDDRE1_FAMILIES:
+				raise ValueError(f'Family {self.family} is not IDDR capable')
+
 			for bit in range(len(q1)):
 				if self.family in XDDR_FAMILIES:
 					m.submodules += Instance(
 						'IDDR',
 						p_DDR_CLK_EDGE = 'SAME_EDGE_PIPELINED',
 						p_SRTYPE = 'ASYNC',
 						p_INIT_Q1 = Const(0, 1),
@@ -1072,15 +1102,15 @@
 					get_oddr(pin.o_clk, pin_o0, pin_o1, o)
 			if pin.dir in ('oe', 'io'):
 				if self.family == 'spartan6':
 					get_oddr(pin.o_clk, ~pin.oe, ~pin.oe, t)
 				else:
 					get_iob_dff(pin.o_clk, ~pin.oe, t)
 		else:
-			assert False
+			raise ValueError(f'Invalid gearing {pin.xdr} for pin {pin.name}, must be one of, 0, 1, or 2')
 
 		return (i, o, t)
 
 	def _get_valid_xdrs(self) -> Union[
 		tuple[Literal[0], Literal[1]],
 		tuple[Literal[0], Literal[1], Literal[2]]
 	]:
```

### Comparing `torii-0.5.0/torii/sim/_base.py` & `torii-0.6.0/torii/sim/_base.py`

 * *Files identical despite different names*

### Comparing `torii-0.5.0/torii/sim/_pyrtl.py` & `torii-0.6.0/torii/sim/_pyrtl.py`

 * *Files 4% similar despite different names*

```diff
@@ -94,31 +94,29 @@
 
 	def on_ClockSignal(self, value):
 		raise NotImplementedError # :nocov:
 
 	def on_ResetSignal(self, value):
 		raise NotImplementedError # :nocov:
 
-	def on_AnyConst(self, value):
-		raise NotImplementedError # :nocov:
-
-	def on_AnySeq(self, value):
+	def on_AnyValue(self, value):
 		raise NotImplementedError # :nocov:
 
 	def on_Sample(self, value):
 		raise NotImplementedError # :nocov:
 
 	def on_Initial(self, value):
 		raise NotImplementedError # :nocov:
 
 
 class _RHSValueCompiler(_ValueCompiler):
 	def __init__(self, state, emitter, *, mode, inputs = None):
 		super().__init__(state, emitter)
-		assert mode in ('curr', 'next')
+		if mode not in ('curr', 'next'):
+			raise ValueError(f'Expected mode to be \'curr\', or \'next\', not \'{mode!r}\'')
 		self.mode = mode
 		# If not None, `inputs` gets populated with RHS signals.
 		self.inputs = inputs
 
 	def on_Const(self, value):
 		return f'{value.value}'
 
@@ -383,30 +381,24 @@
 			else:
 				for pattern in patterns:
 					if "-" in pattern:
 						mask  = int(''.join('0' if b == '-' else '1' for b in pattern), 2)
 						value = int(''.join('0' if b == '-' else b for b in pattern), 2)
 						gen_checks.append(f'{value} == ({mask} & {gen_test})')
 					else:
-						value = int(pattern, 2)
+						value = int(pattern or '0', 2)
 						gen_checks.append(f'{value} == {gen_test}')
 			if index == 0:
 				self.emitter.append(f'if {" or ".join(gen_checks)}:')
 			else:
 				self.emitter.append(f'elif {" or ".join(gen_checks)}:')
 			with self.emitter.indent():
 				self(stmts)
 
-	def on_Assert(self, stmt):
-		raise NotImplementedError # :nocov:
-
-	def on_Assume(self, stmt):
-		raise NotImplementedError # :nocov:
-
-	def on_Cover(self, stmt):
+	def on_Property(self, stmt):
 		raise NotImplementedError # :nocov:
 
 	@classmethod
 	def compile(cls, state, stmt):
 		output_indexes = [state.get_signal(signal) for signal in stmt._lhs_signals()]
 		emitter = _PythonEmitter()
 		for signal_index in output_indexes:
```

### Comparing `torii-0.5.0/torii/sim/core.py` & `torii-0.6.0/torii/sim/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,17 @@
 
 			This can cause things to appear out-of-step.
 
 	'''
 	def __init__(self, domain: Union[str, ClockDomain] = 'sync') -> None:
 		if not isinstance(domain, (str, ClockDomain)):
 			raise TypeError(f'Domain must be a string or a ClockDomain instance, not {domain!r}')
-		assert domain != 'comb'
+		if domain == 'comb':
+			raise ValueError('Unable to tick the combinatorial domain!')
+
 		self.domain = domain
 
 	def __repr__(self) -> str:
 		return f'(tick {self.domain})'
 
 
 class Passive(Command):
@@ -219,15 +221,18 @@
 
 		If the simulation stops advancing, this function will never return.
 
 		'''
 
 		# Convert deadline in seconds into internal 1 ps units
 		deadline = deadline * 1e12
-		assert self._engine.now <= deadline
+
+		if self._engine.now > deadline:
+			raise ValueError(f'Simulation engine time is ahead of given deadline! {self._engine.now} > {deadline}')
+
 		while (self.advance() or run_passive) and self._engine.now < deadline:
 			pass
 
 	def write_vcd(
 		self, vcd_file: Optional[Union[IO, str]], gtkw_file: Optional[Union[IO, str]] = None, *,
 		traces: Iterable[Signal] = ()
 	) -> None:
```

### Comparing `torii-0.5.0/torii/sim/pysim.py` & `torii-0.6.0/torii/sim/pysim.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,86 +4,80 @@
 from itertools  import chain
 from re         import search
 
 from vcd        import VCDWriter
 from vcd.gtkw   import GTKWSave
 
 from ..hdl      import ClockSignal, ResetSignal
-from ..hdl.ast  import SignalDict
+from ..hdl.ast  import SignalDict, Value
+from ..hdl.ir   import Fragment
 from ._base     import BaseEngine, BaseSignalState, BaseSimulation
 from ._pyclock  import PyClockProcess
 from ._pycoro   import PyCoroProcess
 from ._pyrtl    import _FragmentCompiler
 
 __all__ = (
 	'PySimEngine',
 )
 
-
-class _NameExtractor:
-	def __init__(self):
-		self.names = SignalDict()
-
-	def __call__(self, fragment, *, hierarchy = ('bench', 'top',)):
-		def add_signal_name(signal):
-			hierarchical_signal_name = (*hierarchy, signal.name)
-			if signal not in self.names:
-				self.names[signal] = {hierarchical_signal_name}
-			else:
-				self.names[signal].add(hierarchical_signal_name)
-
-		for domain_name, domain_signals in fragment.drivers.items():
-			if domain_name is not None:
-				domain = fragment.domains[domain_name]
-				add_signal_name(domain.clk)
-				if domain.rst is not None:
-					add_signal_name(domain.rst)
-
-		for statement in fragment.statements:
-			for signal in statement._lhs_signals() | statement._rhs_signals():
-				if not isinstance(signal, (ClockSignal, ResetSignal)):
-					add_signal_name(signal)
-
-		for subfragment_index, (subfragment, subfragment_name) in enumerate(fragment.subfragments):
-			if subfragment_name is None:
-				subfragment_name = f'U${subfragment_name}'
-			self(subfragment, hierarchy = (*hierarchy, subfragment_name))
-
-		return self.names
-
-
 class _VCDWriter:
 	@staticmethod
 	def decode_to_vcd(signal, value):
 		return signal.decoder(value).expandtabs().replace(' ', '_')
 
-	def __init__(self, fragment, *, vcd_file, gtkw_file = None, traces = ()):
+	def __init__(self, fragment: Fragment, *, vcd_file: str, gtkw_file: str | None = None, traces = ()):
+
+		self._close_vcd = False
+		self._close_gtkw = False
 		if isinstance(vcd_file, str):
 			vcd_file = open(vcd_file, 'wt')
+			self._close_vcd = True
+
 		if isinstance(gtkw_file, str):
 			gtkw_file = open(gtkw_file, 'wt')
+			self._close_gtkw = True
 
 		self.vcd_vars = SignalDict()
 		self.vcd_file = vcd_file
 		self.vcd_writer = vcd_file and VCDWriter(self.vcd_file,
 			timescale = '1 ps', comment = 'Generated by Torii')
 
 		self.gtkw_names = SignalDict()
 		self.gtkw_file = gtkw_file
 		self.gtkw_save = gtkw_file and GTKWSave(self.gtkw_file)
 
 		self.traces = []
 
-		signal_names = _NameExtractor()(fragment)
+		signal_names = SignalDict()
+		for subfragment, subfragment_name in fragment._assign_names_to_fragments(
+			hierarchy = ('bench', 'top', )
+		).items():
+			for signal, signal_name in subfragment._assign_names_to_signals().items():
+				if signal not in signal_names:
+					signal_names[signal] = set()
+				signal_names[signal].add((*subfragment_name, signal_name))
 
 		trace_names = SignalDict()
+		assigned_names = set()
 		for trace in traces:
-			if trace not in signal_names:
-				trace_names[trace] = { ('bench', trace.name) }
-			self.traces.append(trace)
+			trace = Value.cast(trace)
+			for trace_signal in trace._rhs_signals():
+				if trace_signal not in signal_names:
+					if trace_signal.name not in assigned_names:
+						name = trace_signal.name
+					else:
+						name = f'{trace_signal.name}${len(assigned_names)}'
+						if name in assigned_names:
+							raise RuntimeError(
+								f'Unable to create unique signal name for {trace_signal.name}. '
+								f'Tried {name}, but it already exists.'
+							)
+					trace_names[trace_signal] = { ('bench', name) }
+					assigned_names.add(name)
+				self.traces.append(trace_signal)
 
 		if self.vcd_writer is None:
 			return
 
 		for signal, names in chain(signal_names.items(), trace_names.items()):
 			if signal.decoder:
 				var_type = 'string'
@@ -144,31 +138,32 @@
 			for signal in self.traces:
 				if len(signal) > 1 and not signal.decoder:
 					suffix = f'[{len(signal) - 1}:0]'
 				else:
 					suffix = ''
 				self.gtkw_save.trace('.'.join(self.gtkw_names[signal]) + suffix)
 
-		if self.vcd_file is not None:
+		if self._close_vcd:
 			self.vcd_file.close()
-		if self.gtkw_file is not None:
+		if self._close_gtkw:
 			self.gtkw_file.close()
 
 
 class _Timeline:
 	def __init__(self):
 		self.now = 0
 		self.deadlines = dict()
 
 	def reset(self):
 		self.now = 0
 		self.deadlines.clear()
 
 	def at(self, run_at, process):
-		assert process not in self.deadlines
+		if process in self.deadlines:
+			raise ValueError(f'Process {process!r} already in deadline list')
 		self.deadlines[process] = run_at
 
 	def delay(self, delay_by, process):
 		if delay_by is None:
 			run_at = self.now
 		else:
 			run_at = self.now + delay_by
@@ -181,15 +176,17 @@
 			if deadline is None:
 				if nearest_deadline is not None:
 					nearest_processes.clear()
 				nearest_processes.add(process)
 				nearest_deadline = self.now
 				break
 			elif nearest_deadline is None or deadline <= nearest_deadline:
-				assert deadline >= self.now
+				if deadline < self.now:
+					raise ValueError(f'Deadline of {deadline} is behind our current state of {self.now}')
+
 				if nearest_deadline is not None and deadline < nearest_deadline:
 					nearest_processes.clear()
 				nearest_processes.add(process)
 				nearest_deadline = deadline
 
 		if not nearest_processes:
 			return False
@@ -249,21 +246,22 @@
 			index = len(self.slots)
 			self.slots.append(_PySignalState(signal, self.pending))
 			self.signals[signal] = index
 			return index
 
 	def add_trigger(self, process, signal, *, trigger = None):
 		index = self.get_signal(signal)
-		assert (process not in self.slots[index].waiters or
-				self.slots[index].waiters[process] == trigger)
+		if process in self.slots[index].waiters and self.slots[index].waiters[process] != trigger:
+			raise ValueError('Unable to add trigger for process!')
 		self.slots[index].waiters[process] = trigger
 
 	def remove_trigger(self, process, signal):
 		index = self.get_signal(signal)
-		assert process in self.slots[index].waiters
+		if process not in self.slots[index].waiters:
+			raise ValueError(f'Unable to remove trigger for process {process!r}, not in the slot list')
 		del self.slots[index].waiters[process]
 
 	def wait_interval(self, process, interval):
 		self.timeline.delay(interval, process)
 
 	def commit(self, changed = None):
 		converged = True
```

### Comparing `torii-0.5.0/torii/test/__init__.py` & `torii-0.6.0/torii/test/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -233,17 +233,18 @@
 		count : int
 			Number of settles to invoke in the simulator.
 
 		'''
 		for _ in range(count):
 			yield Settle()
 			yield
+		yield Settle()
 
 	@staticmethod
-	def wait_until_high(strobe: Signal, *, timeout: int = None):
+	def wait_until_high(strobe: Signal, *, timeout: Optional[int] = None):
 		'''
 		Run simulation until signal goes high.
 
 		Runs the simulation while checking for the positive edge of the `strobe`
 		signal.
 
 		Will run until a positive edge is seen, or if `timeout` is set, will run
@@ -266,15 +267,15 @@
 		while not (yield strobe):
 			yield
 			elapsed_cycles += 1
 			if timeout and elapsed_cycles > timeout:
 				raise RuntimeError(f'Timeout waiting for \'{strobe.name}\' to go high')
 
 	@staticmethod
-	def wait_until_low(strobe: Signal, *, timeout: int = None):
+	def wait_until_low(strobe: Signal, *, timeout: Optional[int] = None):
 		'''
 		Run simulation until signal goes low.
 
 		Runs the simulation while checking for the negative edge of the `strobe`
 		signal.
 
 		Will run until a negative edge is seen, or if `timeout` is set, will run
```

### Comparing `torii-0.5.0/torii/test/mock.py` & `torii-0.6.0/torii/test/mock.py`

 * *Files identical despite different names*

### Comparing `torii-0.5.0/torii/tools/__init__.py` & `torii-0.6.0/torii/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `torii-0.5.0/torii/tools/cxx.py` & `torii-0.6.0/torii/tools/cxx.py`

 * *Files identical despite different names*

### Comparing `torii-0.5.0/torii/tools/yosys.py` & `torii-0.6.0/torii/tools/yosys.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,19 +153,19 @@
 	----------
 	version: tuple[int, int, int]
 		The version of Yosys found on the system
 
 	Returns
 	-------
 	bool:
-		If the version meets the minimum requirement. (currently 0.15)
+		If the version meets the minimum requirement. (currently 0.30+ except 0.37)
 
 	'''
 
-	return version >= (0, 15)
+	return version >= (0, 30) and version != (0, 37)
 
 def find_yosys(
 	requirement: Callable[[Optional[tuple[int, int, int]]], bool] = min_yosys_version
 ) -> YosysBinary:
 	'''
 	Find an available Yosys executable of required version.
```

### Comparing `torii-0.5.0/torii/util/__init__.py` & `torii-0.6.0/torii/util/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,14 +41,17 @@
 			return dict(map(lambda s: s.strip().split('=', 2), matches[0].group(1).split(',')))
 	return dict()
 
 
 def get_linter_option(
 	filename: str , name: str, type: Union[type[bool], type[int]], default: Union[bool, int]
 ) -> Union[bool, int]:
+	if type not in (bool, int):
+		raise TypeError(f'Expected type to be either \'bool\' or \'int\', not \'{type!r}\'')
+
 	options = get_linter_options(filename)
 	if name not in options:
 		return default
 
 	option = options[name]
 	if type is bool:
 		if option in ('1', 'yes', 'enable'):
@@ -57,8 +60,7 @@
 			return False
 		return default
 	if type is int:
 		try:
 			return int(option, 0)
 		except ValueError:
 			return default
-	assert False
```

### Comparing `torii-0.5.0/torii/util/decorators.py` & `torii-0.6.0/torii/util/decorators.py`

 * *Files identical despite different names*

### Comparing `torii-0.5.0/torii/util/string.py` & `torii-0.6.0/torii/util/string.py`

 * *Files identical despite different names*

### Comparing `torii-0.5.0/torii/util/tracer.py` & `torii-0.6.0/torii/util/tracer.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,15 +24,17 @@
 		call_index -= 2
 	while True:
 		call_opc = opname[code.co_code[call_index]]
 		if call_opc in ('EXTENDED_ARG',):
 			call_index += 2
 		else:
 			break
-	if call_opc not in ('CALL_FUNCTION', 'CALL_FUNCTION_KW', 'CALL_FUNCTION_EX', 'CALL_METHOD', 'CALL'):
+	if call_opc not in (
+		'CALL_FUNCTION', 'CALL_FUNCTION_KW', 'CALL_FUNCTION_EX', 'CALL_METHOD', 'CALL_METHOD_KW', 'CALL', 'CALL_KW'
+	):
 		if default is _raise_exception:
 			raise NameNotFound
 		else:
 			return default
 
 	index = call_index + 2
 	imm = 0
```

### Comparing `torii-0.5.0/torii/util/units.py` & `torii-0.6.0/torii/util/units.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 # SPDX-License-Identifier: BSD-2-Clause
 
+import operator
+import warnings
+
 __all__ = (
 	'ps_to_sec',
 	'ns_to_sec',
 	'us_to_sec',
 	'ms_to_sec',
 	'sec_to_ps',
 	'sec_to_ns',
 	'sec_to_us',
 	'sec_to_ms',
 	'bits_for',
 	'iec_size',
 	'log2_int',
+	'log2_ceil',
+	'log2_exact',
 )
 
 PS = 1e-12
 NS = 1e-9
 US = 1e-6
 MS = 1e-3
 
@@ -72,29 +77,72 @@
 	if rem == 0 and dec == 0:
 		fixed = int(fixed)
 	else:
 		fixed = round(fixed, dec)
 
 	return f'{fixed}{suffixes[scale]}'
 
+def log2_ceil(n):
+	'''
+	Returns the integer log2 of the smallest power-of-2 greater than or equal to `n`.
+
+	Raises a `ValueError` for negative inputs.
+	'''
+
+	n = operator.index(n)
+	if n < 0:
+		raise ValueError(f'{n} is negative')
+	if n == 0:
+		return 0
+	return (n - 1).bit_length()
+
+
+def log2_exact(n):
+	'''
+	Returns the integer log2 of `n`, which must be an exact power of two.
+
+	Raises a `ValueError` if `n` is not a power of two.
+	'''
+
+	n = operator.index(n)
+	if n <= 0 or (n & (n - 1)):
+		raise ValueError(f'{n} is not a power of 2')
+	return (n - 1).bit_length()
+
 def log2_int(n: int, need_pow2: bool = True) -> int:
 	''' '''
+	if need_pow2:
+		warnings.warn(
+			'`log2_int` is deprecated, replace usage of `log2_int(n, True)` with `log2_exact(n)`',
+			DeprecationWarning,
+			stacklevel = 2
+		)
+	else:
+		warnings.warn(
+			'`log2_int` is deprecated, replace usage of `log2_int(n, False)` with `log2_ceil(n)`',
+			DeprecationWarning,
+			stacklevel = 2
+		)
+
 
+	n = operator.index(n)
 	if n == 0:
 		return 0
 	r = (n - 1).bit_length()
 	if need_pow2 and (1 << r) != n:
 		raise ValueError(f'{n} is not a power of 2')
 	return r
 
 
 def bits_for(n: int, require_sign_bit: bool = False) -> int:
 	''' Returns the number of bits needed to represent int ``n`` '''
 
+	n = operator.index(n)
+
 	if n > 0:
-		r = log2_int(n + 1, False)
+		r = log2_ceil(n + 1)
 	else:
 		require_sign_bit = True
-		r = log2_int(-n, False)
+		r = log2_ceil(-n)
 	if require_sign_bit:
 		r += 1
 	return r
```

### Comparing `torii-0.5.0/torii.egg-info/PKG-INFO` & `torii-0.6.0/torii.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torii
-Version: 0.5.0
+Version: 0.6.0
 Summary: Torii hardware definition language
 Home-page: https://torii.shmdn.link/
 Author: Aki Van Ness, Rachel Mant
 Author-email: aki@lethalbit.net, git@dragonmux.network
 License: BSD-2-Clause
 Project-URL: Documentation, https://torii.shmdn.link/
 Project-URL: Source Code, https://github.com/shrine-maiden-heavy-industries/torii-hdl
@@ -13,30 +13,30 @@
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Typing :: Typed
-Requires-Python: ~=3.9
+Requires-Python: ~=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: setuptools
 Requires-Dist: pyvcd>=0.2.2
 Requires-Dist: Jinja2~=3.0
-Requires-Dist: rich>=12.6.0
+Requires-Dist: rich
 Provides-Extra: dev
 Requires-Dist: nox; extra == "dev"
 
 # Torii-HDL
 
 Torii is a fork of [Amaranth HDL](https://github.com/amaranth-lang) that has been modified for use at [Shrine Maiden Heavy Industries](https://shrine-maiden-heavy.industries/). It has merged several of the components that were separate into a single package, and also adds new functionality, as well as some internal changes for better integration into tooling.
```

#### html2text {}

```diff
@@ -1,34 +1,34 @@
-Metadata-Version: 2.1 Name: torii Version: 0.5.0 Summary: Torii hardware
+Metadata-Version: 2.1 Name: torii Version: 0.6.0 Summary: Torii hardware
 definition language Home-page: https://torii.shmdn.link/ Author: Aki Van Ness,
 Rachel Mant Author-email: aki@lethalbit.net, git@dragonmux.network License:
 BSD-2-Clause Project-URL: Documentation, https://torii.shmdn.link/ Project-URL:
 Source Code, https://github.com/shrine-maiden-heavy-industries/torii-hdl
 Project-URL: Bug Tracker, https://github.com/shrine-maiden-heavy-industries/
 torii-hdl/issues Classifier: Development Status :: 4 - Beta Classifier:
 Intended Audience :: Developers Classifier: Intended Audience :: Information
 Technology Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: BSD License Classifier: Operating System :: MacOS ::
 MacOS X Classifier: Operating System :: Microsoft :: Windows Classifier:
 Operating System :: POSIX :: Linux Classifier: Programming Language :: Python
-:: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Classifier: Topic :: Scientific/
+:: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Programming Language :: Python :: 3.12 Classifier: Topic :: Scientific/
 Engineering Classifier: Topic :: Scientific/Engineering :: Electronic Design
 Automation (EDA) Classifier: Topic :: Software Development Classifier: Topic ::
 Software Development :: Embedded Systems Classifier: Topic :: Software
-Development :: Libraries Classifier: Typing :: Typed Requires-Python: ~=3.9
+Development :: Libraries Classifier: Typing :: Typed Requires-Python: ~=3.10
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 setuptools Requires-Dist: pyvcd>=0.2.2 Requires-Dist: Jinja2~=3.0 Requires-
-Dist: rich>=12.6.0 Provides-Extra: dev Requires-Dist: nox; extra == "dev" #
-Torii-HDL Torii is a fork of [Amaranth HDL](https://github.com/amaranth-lang)
-that has been modified for use at [Shrine Maiden Heavy Industries](https://
-shrine-maiden-heavy.industries/). It has merged several of the components that
-were separate into a single package, and also adds new functionality, as well
-as some internal changes for better integration into tooling. The evaluation
-board definitions have also been migrated and are located in the [torii-boards]
+Dist: rich Provides-Extra: dev Requires-Dist: nox; extra == "dev" # Torii-HDL
+Torii is a fork of [Amaranth HDL](https://github.com/amaranth-lang) that has
+been modified for use at [Shrine Maiden Heavy Industries](https://shrine-
+maiden-heavy.industries/). It has merged several of the components that were
+separate into a single package, and also adds new functionality, as well as
+some internal changes for better integration into tooling. The evaluation board
+definitions have also been migrated and are located in the [torii-boards]
 (https://github.com/shrine-maiden-heavy-industries/torii-boards) repository.
 There is also a list of [projects using Torii](https://torii.shmdn.link/
 projects.html) that are using Torii, and we'd love to add yours too! ##
 Introduction Please see the [Torii Introduction](https://shrine-maiden-heavy-
 industries.github.io/torii-hdl/intro.html) on the [online documentation](https:
 //shrine-maiden-heavy-industries.github.io/torii-hdl/) ## Installation Please
 see the [installation instructions](https://shrine-maiden-heavy-
```

### Comparing `torii-0.5.0/torii.egg-info/SOURCES.txt` & `torii-0.6.0/torii.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -60,17 +60,17 @@
 docs/library/soc/csr/index.md
 docs/library/soc/wishbone/index.md
 docs/library/stdio/index.md
 docs/library/vendor/index.md
 docs/library/vendor/lattice/index.md
 docs/library/vendor/xilinx/index.md
 docs/platforms/index.md
+docs/platforms/fpga/altera.md
 docs/platforms/fpga/gowin.md
 docs/platforms/fpga/index.md
-docs/platforms/fpga/intel.md
 docs/platforms/fpga/lattice-ecp5.md
 docs/platforms/fpga/lattice-ice40.md
 docs/platforms/fpga/lattice-machxo-2-3l.md
 docs/platforms/fpga/quicklogic.md
 docs/platforms/fpga/xilinx.md
 docs/sim/index.md
 docs/tutorials/external_modules.md
@@ -196,19 +196,17 @@
 torii/platform/resources/display.py
 torii/platform/resources/interface.py
 torii/platform/resources/memory.py
 torii/platform/resources/user.py
 torii/platform/resources/extensions/__init__.py
 torii/platform/resources/extensions/pmod.py
 torii/platform/vendor/__init__.py
+torii/platform/vendor/altera.py
 torii/platform/vendor/gowin.py
 torii/platform/vendor/intel.py
-torii/platform/vendor/lattice_ecp5.py
-torii/platform/vendor/lattice_ice40.py
-torii/platform/vendor/lattice_machxo_2_3l.py
 torii/platform/vendor/quicklogic.py
 torii/platform/vendor/xilinx.py
 torii/platform/vendor/lattice/__init__.py
 torii/platform/vendor/lattice/ecp5.py
 torii/platform/vendor/lattice/ice40.py
 torii/platform/vendor/lattice/machxo_2_3l.py
 torii/sim/__init__.py
```

