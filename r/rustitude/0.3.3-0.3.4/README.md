# Comparing `tmp/rustitude-0.3.3.tar.gz` & `tmp/rustitude-0.3.4.tar.gz`

## Comparing `rustitude-0.3.3.tar` & `rustitude-0.3.4.tar`

### file list

```diff
@@ -1,13 +1,25 @@
--rw-r--r--   0        0        0      928 1970-01-01 00:00:00.000000 rustitude-0.3.3/Cargo.toml
--rw-r--r--   0     1001      127     3471 2024-05-03 02:26:30.000000 rustitude-0.3.3/.github/workflows/maturin.yml
--rw-r--r--   0     1001      127      316 2024-05-03 02:26:30.000000 rustitude-0.3.3/.github/workflows/rust.yml
--rw-r--r--   0     1001      127       56 2024-05-03 02:26:30.000000 rustitude-0.3.3/.gitignore
--rw-r--r--   0     1001      127    11390 2024-05-03 02:26:30.000000 rustitude-0.3.3/CHANGELOG.md
--rw-r--r--   0     1001      127     1507 2024-05-03 02:26:30.000000 rustitude-0.3.3/LICENSE
--rw-r--r--   0     1001      127     9722 2024-05-03 02:26:30.000000 rustitude-0.3.3/README.md
--rw-r--r--   0     1001      127     2846 2024-05-03 02:26:30.000000 rustitude-0.3.3/bacon.toml
--rw-r--r--   0     1001      127    32108 2024-05-03 02:26:30.000000 rustitude-0.3.3/media/logo.png
--rw-r--r--   0     1001      127      386 2024-05-03 02:26:30.000000 rustitude-0.3.3/src/lib.rs
--rw-r--r--   0     1001      127    37972 2024-05-03 02:26:30.000000 rustitude-0.3.3/Cargo.lock
--rw-r--r--   0     1001      127      857 2024-05-03 02:26:30.000000 rustitude-0.3.3/pyproject.toml
--rw-r--r--   0        0        0    10462 1970-01-01 00:00:00.000000 rustitude-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0      928 1970-01-01 00:00:00.000000 rustitude-0.3.4/Cargo.toml
+-rw-r--r--   0     1001      127     3469 2024-05-06 23:06:20.000000 rustitude-0.3.4/.github/workflows/maturin.yml
+-rw-r--r--   0     1001      127      316 2024-05-06 23:06:20.000000 rustitude-0.3.4/.github/workflows/rust.yml
+-rw-r--r--   0     1001      127     3136 2024-05-06 23:06:20.000000 rustitude-0.3.4/.gitignore
+-rw-r--r--   0     1001      127    15705 2024-05-06 23:06:20.000000 rustitude-0.3.4/CHANGELOG.md
+-rw-r--r--   0     1001      127     1507 2024-05-06 23:06:20.000000 rustitude-0.3.4/LICENSE
+-rw-r--r--   0     1001      127    11361 2024-05-06 23:06:20.000000 rustitude-0.3.4/README.md
+-rw-r--r--   0     1001      127     2846 2024-05-06 23:06:20.000000 rustitude-0.3.4/bacon.toml
+-rw-r--r--   0     1001      127    32108 2024-05-06 23:06:20.000000 rustitude-0.3.4/media/logo.png
+-rw-r--r--   0     1001      127     1723 2024-05-06 23:06:20.000000 rustitude-0.3.4/rustitude/__init__.py
+-rw-r--r--   0     1001      127     4264 2024-05-06 23:06:20.000000 rustitude-0.3.4/rustitude/__init__.pyi
+-rw-r--r--   0     1001      127      145 2024-05-06 23:06:20.000000 rustitude-0.3.4/rustitude/amplitude.pyi
+-rw-r--r--   0     1001      127      840 2024-05-06 23:06:20.000000 rustitude-0.3.4/rustitude/dataset.pyi
+-rw-r--r--   0     1001      127      535 2024-05-06 23:06:20.000000 rustitude-0.3.4/rustitude/four_momentum.pyi
+-rw-r--r--   0     1001      127       90 2024-05-06 23:06:20.000000 rustitude-0.3.4/rustitude/gluex/__init__.pyi
+-rw-r--r--   0     1001      127       83 2024-05-06 23:06:20.000000 rustitude-0.3.4/rustitude/gluex/dalitz.pyi
+-rw-r--r--   0     1001      127     4632 2024-05-06 23:06:20.000000 rustitude-0.3.4/rustitude/gluex/harmonics.pyi
+-rw-r--r--   0     1001      127      566 2024-05-06 23:06:20.000000 rustitude-0.3.4/rustitude/gluex/resonances.pyi
+-rw-r--r--   0     1001      127      347 2024-05-06 23:06:20.000000 rustitude-0.3.4/rustitude/gluex/sdmes.pyi
+-rw-r--r--   0     1001      127     3275 2024-05-06 23:06:20.000000 rustitude-0.3.4/rustitude/manager.pyi
+-rw-r--r--   0     1001      127        0 2024-05-06 23:06:20.000000 rustitude-0.3.4/rustitude/py.typed
+-rw-r--r--   0     1001      127     1650 2024-05-06 23:06:20.000000 rustitude-0.3.4/src/lib.rs
+-rw-r--r--   0     1001      127    37972 2024-05-06 23:06:20.000000 rustitude-0.3.4/Cargo.lock
+-rw-r--r--   0     1001      127      911 2024-05-06 23:06:20.000000 rustitude-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0    12144 1970-01-01 00:00:00.000000 rustitude-0.3.4/PKG-INFO
```

### Comparing `rustitude-0.3.3/Cargo.toml` & `rustitude-0.3.4/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [package]
 exclude = ["convert", "resources"]
 name = "rustitude"
-version = "0.3.3"
+version = "0.3.4"
 edition = "2021"
 authors = ["Nathaniel Dene Hoffman <dene@cmu.edu>"]
 description = "A library to create and operate models for particle physics amplitude analyses"
 repository = "https://github.com/denehoffman/rustitude/"
 homepage = "https://github.com/denehoffman/rustitude/"
 license = "BSD-3-Clause"
 readme = "README.md"
```

### Comparing `rustitude-0.3.3/.github/workflows/maturin.yml` & `rustitude-0.3.4/.github/workflows/maturin.yml`

 * *Files 0% similar despite different names*

```diff
@@ -121,15 +121,15 @@
         with:
           name: wheels-sdist
           path: dist
 
   release:
     name: Release
     runs-on: ubuntu-latest
-    # if: "startsWith(github.ref, 'refs/tags/')"
+    if: "startsWith(github.ref, 'refs/tags/')"
     needs: [linux, windows, macos, sdist]
     steps:
       - uses: actions/download-artifact@v4
       - name: Publish to PyPI
         uses: PyO3/maturin-action@v1
         env:
           MATURIN_PYPI_TOKEN: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `rustitude-0.3.3/CHANGELOG.md` & `rustitude-0.3.4/CHANGELOG.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,76 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
-## 0.3.3 (2024-05-03)
+## 0.3.4 (2024-05-06)
+
+### Chore
+
+ - <csr-id-475682fc30d7dc6a817030dd754cc4fb7dd295cc/> bump python library version
+
+### Documentation
+
+ - <csr-id-6d613a1c49ce065ffa4a50df09380f41359218be/> Update README.md
+ - <csr-id-48a73623f151336f198009097c028d000d3e43c5/> Update README.md
+ - <csr-id-2d548c4865b90043005b2aed7977612a28dad409/> fixed some links
+ - <csr-id-3dc627598be4f79ffc230f8bff813423d57491f2/> Update README.md
+
+### New Features
+
+ - <csr-id-6fc5c77477602403f3b892b240064de9f717d406/> add type checking and re-export rustitude-core and rustitude-gluex as their own submodules
+
+### Bug Fixes
+
+ - <csr-id-9735d57d039946cc7b5de57a9965c4fd01c2964f/> correct spelling
+
+### Other
+
+ - <csr-id-f64c86d2e21c17fe6bc5638240293a774185159a/> update Cargo.lock
+ - <csr-id-4a88e2b13fb01de2812f91ef4d55eea6b37fe7b2/> re-enable tag check
+ - <csr-id-1747d5dc4a63bf47f2f5cbc479f879459e900c4c/> temporarily disable tag check so we can push to pypi through an action
+ - <csr-id-42f29669736bb72ed4d85f4669df1a48288a2db8/> re-enable on-push and on-PR workflow conditions
+   A release only happens with a new tag
+ - <csr-id-d94179156007fd86b69b8efbfd2f1799d0bb71b8/> update pyproject.toml version
+
+### Commit Statistics
+
+<csr-read-only-do-not-edit/>
+
+ - 13 commits contributed to the release over the course of 3 calendar days.
+ - 3 days passed between releases.
+ - 12 commits were understood as [conventional](https://www.conventionalcommits.org).
+ - 0 issues like '(#ID)' were seen in commit messages
+
+### Commit Details
+
+<csr-read-only-do-not-edit/>
+
+<details><summary>view details</summary>
+
+ * **Uncategorized**
+    - Merge branch 'main' of https://github.com/denehoffman/rustitude ([`7a3806c`](https://github.com/denehoffman/rustitude/commit/7a3806caf8741dc55283deb803653d4b0f892a61))
+    - Bump python library version ([`475682f`](https://github.com/denehoffman/rustitude/commit/475682fc30d7dc6a817030dd754cc4fb7dd295cc))
+    - Update Cargo.lock ([`f64c86d`](https://github.com/denehoffman/rustitude/commit/f64c86d2e21c17fe6bc5638240293a774185159a))
+    - Update README.md ([`6d613a1`](https://github.com/denehoffman/rustitude/commit/6d613a1c49ce065ffa4a50df09380f41359218be))
+    - Correct spelling ([`9735d57`](https://github.com/denehoffman/rustitude/commit/9735d57d039946cc7b5de57a9965c4fd01c2964f))
+    - Update README.md ([`48a7362`](https://github.com/denehoffman/rustitude/commit/48a73623f151336f198009097c028d000d3e43c5))
+    - Fixed some links ([`2d548c4`](https://github.com/denehoffman/rustitude/commit/2d548c4865b90043005b2aed7977612a28dad409))
+    - Add type checking and re-export rustitude-core and rustitude-gluex as their own submodules ([`6fc5c77`](https://github.com/denehoffman/rustitude/commit/6fc5c77477602403f3b892b240064de9f717d406))
+    - Update README.md ([`3dc6275`](https://github.com/denehoffman/rustitude/commit/3dc627598be4f79ffc230f8bff813423d57491f2))
+    - Re-enable tag check ([`4a88e2b`](https://github.com/denehoffman/rustitude/commit/4a88e2b13fb01de2812f91ef4d55eea6b37fe7b2))
+    - Temporarily disable tag check so we can push to pypi through an action ([`1747d5d`](https://github.com/denehoffman/rustitude/commit/1747d5dc4a63bf47f2f5cbc479f879459e900c4c))
+    - Re-enable on-push and on-PR workflow conditions ([`42f2966`](https://github.com/denehoffman/rustitude/commit/42f29669736bb72ed4d85f4669df1a48288a2db8))
+    - Update pyproject.toml version ([`d941791`](https://github.com/denehoffman/rustitude/commit/d94179156007fd86b69b8efbfd2f1799d0bb71b8))
+</details>
+
+## 0.3.3-pypi (2024-05-03)
 
 ### Chore
 
  - <csr-id-e0c32f773b601e2703a0803849a1a2db130e2ffc/> update pyproject.toml info
 
 ### Other
 
@@ -18,31 +79,50 @@
    don't publish on every push, need to set up more for that
  - <csr-id-db8b1a32563700203f896c0d357ed96d1144d202/> add maturin github actions
 
 ### Commit Statistics
 
 <csr-read-only-do-not-edit/>
 
- - 4 commits contributed to the release.
+ - 5 commits contributed to the release.
  - 4 commits were understood as [conventional](https://www.conventionalcommits.org).
  - 0 issues like '(#ID)' were seen in commit messages
 
 ### Commit Details
 
 <csr-read-only-do-not-edit/>
 
 <details><summary>view details</summary>
 
  * **Uncategorized**
+    - Release rustitude v0.3.3 ([`b5748e4`](https://github.com/denehoffman/rustitude/commit/b5748e46a5bb8c19e74b71b10de3d6ba48edbf87))
     - Remove unused library in rustitude-gluex which prevented cross-compilation ([`158ddc2`](https://github.com/denehoffman/rustitude/commit/158ddc248dc8463e08eb14b7f633952fc28abcd6))
     - Update maturin.yml ([`f837054`](https://github.com/denehoffman/rustitude/commit/f8370544ef666930bfd5f3a1b555e34e53525b6f))
     - Add maturin github actions ([`db8b1a3`](https://github.com/denehoffman/rustitude/commit/db8b1a32563700203f896c0d357ed96d1144d202))
     - Update pyproject.toml info ([`e0c32f7`](https://github.com/denehoffman/rustitude/commit/e0c32f773b601e2703a0803849a1a2db130e2ffc))
 </details>
 
+## 0.3.3 (2024-05-03)
+
+<csr-id-e0c32f773b601e2703a0803849a1a2db130e2ffc/>
+<csr-id-158ddc248dc8463e08eb14b7f633952fc28abcd6/>
+<csr-id-f8370544ef666930bfd5f3a1b555e34e53525b6f/>
+<csr-id-db8b1a32563700203f896c0d357ed96d1144d202/>
+
+### Chore
+
+ - <csr-id-e0c32f773b601e2703a0803849a1a2db130e2ffc/> update pyproject.toml info
+
+### Other
+
+ - <csr-id-158ddc248dc8463e08eb14b7f633952fc28abcd6/> remove unused library in rustitude-gluex which prevented cross-compilation
+ - <csr-id-f8370544ef666930bfd5f3a1b555e34e53525b6f/> Update maturin.yml
+   don't publish on every push, need to set up more for that
+ - <csr-id-db8b1a32563700203f896c0d357ed96d1144d202/> add maturin github actions
+
 ## 0.3.2 (2024-05-02)
 
 <csr-id-023cfea357b0d6e5c12f724df32d4ed30c9f24c7/>
 <csr-id-7646b89c792c0f55b8898832abe6a743a052fc7a/>
 <csr-id-8bd07de2425e48f4489a59ce4c168eaa9df9cc42/>
 <csr-id-aaa07cd742e03461449269e8261e7f326600b2a0/>
 <csr-id-e2cb6e54946744299506a39a5d3559ee099378fb/>
```

### Comparing `rustitude-0.3.3/LICENSE` & `rustitude-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rustitude-0.3.3/bacon.toml` & `rustitude-0.3.4/bacon.toml`

 * *Files identical despite different names*

### Comparing `rustitude-0.3.3/media/logo.png` & `rustitude-0.3.4/media/logo.png`

 * *Files identical despite different names*

### Comparing `rustitude-0.3.3/Cargo.lock` & `rustitude-0.3.4/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -171,17 +171,17 @@
 checksum = "f28d99ec8bfea296261ca1af174f24225171fea9664ba9003cbebee704810528"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
 name = "autocfg"
-version = "1.2.0"
+version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f1fdabc7756949593fe60f30ec81974b613357de856987752631dea1e3394c80"
+checksum = "0c4b4d0bd25bd0b74681c0ad21497610ce1b7c91b1022cd21c80c6fbdd9476b0"
 
 [[package]]
 name = "base64"
 version = "0.22.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "72b3254f16251a8381aa12e40e3c4d2f0199f8c6508fbecb9d91f575e0fbb8c6"
 
@@ -240,17 +240,17 @@
 name = "bytes"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "514de17de45fdb8dc022b1a7975556c53c86f9f0aa5f534b98977b171857c2c9"
 
 [[package]]
 name = "cc"
-version = "1.0.96"
+version = "1.0.97"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "065a29261d53ba54260972629f9ca6bffa69bac13cd1fed61420f7fa68b9f8bd"
+checksum = "099a5357d84c4c61eb35fc8eafa9a79a902c2f76911e5747ced4e032edd8d9b4"
 dependencies = [
  "jobserver",
  "libc",
  "once_cell",
 ]
 
 [[package]]
@@ -385,17 +385,17 @@
 dependencies = [
  "crc32fast",
  "miniz_oxide",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.14"
+version = "0.2.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "94b22e06ecb0110981051723910cbf0b5f5e09a2062dd7663334ee79a9d1286c"
+checksum = "c4567c8db10ae91089c99af84c68c38da3ec2f087c3f82960bcdbf3656b6f4d7"
 dependencies = [
  "cfg-if",
  "libc",
  "wasi",
 ]
 
 [[package]]
@@ -750,17 +750,17 @@
 checksum = "7969661fd2958a5cb096e56c8e1ad0444ac2bbcd0061bd28660485a44879858f"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
 name = "num-iter"
-version = "0.1.44"
+version = "0.1.45"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d869c01cc0c455284163fd0092f1f93835385ccab5a98a0dcc497b2f8bf055a9"
+checksum = "1429034a0490724d0075ebb2bc9e875d6503c3cf69e235a8941aa757d83ef5bf"
 dependencies = [
  "autocfg",
  "num-integer",
  "num-traits",
 ]
 
 [[package]]
@@ -773,17 +773,17 @@
  "num-bigint",
  "num-integer",
  "num-traits",
 ]
 
 [[package]]
 name = "num-traits"
-version = "0.2.18"
+version = "0.2.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da0df0e5185db44f69b44f26786fe401b6c293d1907744beaa7fa62b2e5a517a"
+checksum = "071dfc062690e90b734c0b2273ce72ad0ffa95f0c74596bc250dcfd960262841"
 dependencies = [
  "autocfg",
  "libm",
 ]
 
 [[package]]
 name = "once_cell"
@@ -1074,26 +1074,26 @@
 checksum = "bfa0f585226d2e68097d4f95d113b15b83a82e819ab25717ec0590d9584ef366"
 dependencies = [
  "semver",
 ]
 
 [[package]]
 name = "rustitude"
-version = "0.3.3"
+version = "0.3.4"
 dependencies = [
  "pyo3",
  "rayon",
  "rustitude-core",
  "rustitude-gluex",
 ]
 
 [[package]]
 name = "rustitude-core"
-version = "0.3.3"
-source = "git+https://github.com/denehoffman/rustitude-core.git#f35d785ac58b4266a308b8c9ea85f57ce476bf43"
+version = "0.3.4"
+source = "git+https://github.com/denehoffman/rustitude-core.git#c8943f2cec72300c0a0de4fb283367ac8df4f1e4"
 dependencies = [
  "approx",
  "indexmap",
  "itertools",
  "nalgebra",
  "num",
  "num-complex",
@@ -1103,16 +1103,16 @@
  "parquet",
  "pyo3",
  "rayon",
 ]
 
 [[package]]
 name = "rustitude-gluex"
-version = "0.1.4"
-source = "git+https://github.com/denehoffman/rustitude-gluex.git#45426dc7f88a8ff5e888cbd0c756adf1efbc94f9"
+version = "0.1.5"
+source = "git+https://github.com/denehoffman/rustitude-gluex.git#f2f72ff64a12806352534459cc3faa6ebdbdb449"
 dependencies = [
  "factorial",
  "nalgebra",
  "num-complex",
  "pyo3",
  "rayon",
  "rustitude-core",
@@ -1443,26 +1443,26 @@
 checksum = "388c44dc09d76f1536602ead6d325eb532f5c122f17782bd57fb47baeeb767e2"
 dependencies = [
  "lzma-sys",
 ]
 
 [[package]]
 name = "zerocopy"
-version = "0.7.32"
+version = "0.7.33"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "74d4d3961e53fa4c9a25a8637fc2bfaf2595b3d3ae34875568a5cf64787716be"
+checksum = "087eca3c1eaf8c47b94d02790dd086cd594b912d2043d4de4bfdd466b3befb7c"
 dependencies = [
  "zerocopy-derive",
 ]
 
 [[package]]
 name = "zerocopy-derive"
-version = "0.7.32"
+version = "0.7.33"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9ce1b18ccd8e73a9321186f97e46f9f04b778851177567b1975109d26a08d2a6"
+checksum = "6f4b6c273f496d8fd4eaf18853e6b448760225dc030ff2c485a786859aea6393"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 2.0.60",
 ]
 
 [[package]]
```

### Comparing `rustitude-0.3.3/pyproject.toml` & `rustitude-0.3.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 [build-system]
 requires = ["maturin>=1.0,<2.0"]
 build-backend = "maturin"
 
 [tool.maturin]
+module-name = "rustitude._rustitude"
 features = ["pyo3/extension-module"]
 
 [project]
 name = "rustitude"
-version = "0.3.3"
+version = "0.3.4"
 description = "Python bindings for the Rustitude library"
 readme = "README.md"
 requires-python = ">=3.7"
 license = { file = "LICENSE" }
 keywords = ["physics", "math", "rust"]
 authors = [{ email = "dene@cmu.edu" }, { name = "Nathaniel Dene Hoffman" }]
 maintainers = [{ name = "Nathaniel Dene Hoffman", email = "dene@cmu.edu" }]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python",
 ]
 
-dependencies = []
+dependencies = ["uproot", "numpy"]
 
 [project.urls]
 homepage = "https://github.com/denehoffman/rustitude"
 repository = "https://github.com/denehoffman/rustitude"
 changelog = "https://github.com/denehoffman/rustitude/blob/main/CHANGELOG.md"
 # TODO: documentation = "readthedocs.org"
```

### Comparing `rustitude-0.3.3/PKG-INFO` & `rustitude-0.3.4/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.3
-Name: rustitude
-Version: 0.3.3
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python
-License-File: LICENSE
-Summary: Python bindings for the Rustitude library
-Keywords: physics,math,rust
-Home-Page: https://github.com/denehoffman/rustitude/
-Author: Nathaniel Dene Hoffman
-Author-email: dene@cmu.edu
-Maintainer-email: Nathaniel Dene Hoffman <dene@cmu.edu>
-License: BSD-3-Clause
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: homepage, https://github.com/denehoffman/rustitude
-Project-URL: repository, https://github.com/denehoffman/rustitude
-Project-URL: changelog, https://github.com/denehoffman/rustitude/blob/main/CHANGELOG.md
-
 <p align="center">
   <img
     width="800"
     src="https://raw.githubusercontent.com/denehoffman/rustitude/main/media/logo.png"
   />
 </p>
 <p align="center">
@@ -32,176 +13,125 @@
     <img src="https://img.shields.io/github/last-commit/denehoffman/rustitude/main" /></a>
   <a href="https://github.com/denehoffman/rustitude/actions" alt="Build Status">
     <img src="https://img.shields.io/github/actions/workflow/status/denehoffman/rustitude/rust.yml" /></a>
   <a href="LICENSE" alt="License">
     <img src="https://img.shields.io/github/license/denehoffman/rustitude" /></a>
   <a href="https://crates.io/crates/rustitude" alt="Rustitude on crates.io">
     <img src="https://img.shields.io/crates/v/rustitude" /></a>
-  <a href="https://docs.rs/rustitude/latest/rustitude/" alt="Rustitude documentation on docs.rs">
+  <a href="https://docs.rs/rustitude" alt="Rustitude documentation on docs.rs">
     <img src="https://img.shields.io/docsrs/rustitude" /></a>
 </p>
 
-
-### Note: This project is still very much under development and not recommended for use in actual research projects (yet)
-
-### Table of Contents
-- [Overview](#Overview)
+### Table of Contents:
+- [Introduction](#Introduction)
+- [Theory](#Theory)
 - [Installation](#Installation)
 - [Usage](#Usage)
+- [TODOs](#TODOs)
 
-## Overview
-Amplitude analysis is the scientific process of fitting models (amplitudes) to data in order to extract additional information. In particle physics, this is often synonymous with partial-wave analysis (PWA), a process commonly used to determine angular momentum quantum numbers for decaying particles. The goal of Rustitude is to establish a framework which is generic enough to fit almost any data to any model, but specific enough to be quick and easy to use in typical particle physics studies. There are three core ideas which this crate tries to follow to make fits fast and efficient:
+# Introduction
+This project began with a desire to make a fast but easy to use interface for fitting amplitudes to particle physics data. That being said, there are performant methods such as [`AmpTools`](https://github.com/mashephe/AmpTools), which is written in C++, but in my personal experience, it can be a bit tricky to use and extend, and it generally requires a lot of boilerplate code to generate new amplitudes or plotting scripts. On the other hand, there are also libraries like [`PyPWA`](https://github.com/JeffersonLab/PyPWA/) (written in Python) which seem like they could be easy to use, but often fail in this aspect due to Python's limiting syntax, speed issues, and a general lack of documentation and ongoing development. There have been attempts to bridge the gap between AmpTools and Python, most recently (and successfully) [`PyAmpTools`](https://github.com/lan13005/PyAmpTools). The difficulty with this method is that it relies on PyROOT, which also means you need ROOT installed (and built with your version of Python). For now, I'll spare you the anti-ROOT rant and just say that ROOT should be an opt-in, not a requirement. So where does that leave `rustitude`?
 
-1. Every function is automatically paralellized over the dataset using [rayon](https://github.com/rayon-rs/rayon).
-2. Model builders can separate their code efficiently into pieces which only need to be calculated once for the whole dataset and those which depend on parameters, which could change at every evaluation. Amplitudes implement `Node`, which is a trait containing all the required methods for an amplitude to be used in an analysis. By precalculating things which don't change, we trade RAM usage now for evaluation speed later.
-3. `Dataset` structs only allow `Event` structs to be stored, so there is a fixed format that implementers must agree on. As it stands, this format closely follows that of [AmpTools](https://github.com/mashephe/AmpTools), but with the addition of a polarization vector. This format can be added to in the future without breaking backwards compatibility, but members should probably not be removed or modified. Unfortunately, ROOT files do not yet have well-documented R/W libraries like Python's [uproot](https://pypi.org/project/uproot/) or Julia's [UpROOT.jl](https://github.com/JuliaHEP/UpROOT.jl), so the current recommendation is to convert files to a more versatile format like parquet. A ROOT-free Python conversion script is included [here](convert).
+As the name suggests, `rustitude` was written in Rust, so let's get the obvious downside out of the way: not many particle physicists know how to write Rust code. Hopefully, this will change over the next decade (and there has already been some [support](https://www.whitehouse.gov/oncd/briefing-room/2024/02/26/memory-safety-statements-of-support/) from the US government, of all places). While Rust carries the disadvantage of relative obscurity compared to C++, it also has many benefits. No `null` means no null references (Tony Hoare's ["billion dollar mistake"](https://web.archive.org/web/20090628071208/http://qconlondon.com/london-2009/speaker/Tony+Hoare)). Pointers (called references in Rust) are always valid, a guarantee made by a very helpful and only occasionally frustrating borrow checker. Rust "crates" are set up in a way which encourages documentation (see [`rustitude-core`'s documentation](https://docs.rs/rustitude-core/)), and the basic syntax is fairly easy to learn for people who have been using optional type checking in Python. Perhaps one of the biggest benefits of Rust is how easy it is to employ [parallelization](https://crates.io/crates/rayon), but the two reasons I like it most are that it's incredibly easy to write Python bindings (that's what this library is after all) and it has a package manager. This second point is important -- unlike C/C++, where a developer is swamped with some menagerie `Makefile`, `CMakeLists.txt`, or some `scons` monstrosity which may only work on "X" system and only if you install and use `make`, `cmake`, `g++`, or whatever (oh yeah, and you made sure all your external dependencies are linked correctly, right? Right?), Rust supports adding a package by simply adding a line to `Cargo.toml` (or using the `cargo add` command). In many ways, package management in Rust is actually simpler than Python, since there's only one prefered method of creating and managing projects, formatting, linting, and compiling.
 
-## Installation
+Now I've covered why I don't like some of the existing solutions, and why I chose to use Rust, but what does this project have that makes it stand out? Here are some reasons to entice you:
 
-Cargo provides the usual command for including this crate in a project:
-```sh
-cargo add rustitude
-```
+- `rustitude` will automatically parallelize amplitudes over the events in a dataset. There's no reason for a developer to ever write parallelized code themselves.
+- Implementing [`Node`](https://docs.rs/rustitude-core/latest/rustitude_core/amplitude/trait.Node.html) on a struct is all that is needed to use it as an amplitude. This means developers need only write two to three total methods to describe the entire functionality of their amplitude, and one of these just gives the names and order of the amplitude's input parameters.
+- A major goal of `rustitude` was to increase processing speed by sacrificing memory. This is done by precalculating parts of amplitudes which don't change when the free parameter inputs change. `AmpTools` supports a version of this, but only on the level of each general amplitude rather than on an individual basis. The simplest example of this is the `Ylm` amplitude (spherical harmonic), which can be entirely precalculated given the value of `l` and `m`. In `AmpTools`, different instances of `Ylm` with different `l`s and `m`s share precalculated data, whereas in `rustitude`, they don't. The `AmpTools` implementation of `Ylm` needs to calculate a spherical harmonic for every event on every function call, while `rustitude` just needs to look up a value in an array!
+- The majority of the library (the public interface) has Python bindings, so if there is no need for custom amplitudes, a developer never actually has to write any Rust code, and the resulting calculations will be as performant as if they were written in Rust.
 
-## Usage
-The basic usage pattern is as follows. We start by importing our data files, we create the amplitudes we want to use, we register them with a `Manager` struct that handles all the internal sums and parameters, and then we evaluate the resulting model. For example, we can generate a model which takes evaluates two spherical harmonics as follows (this uses some code from [another repo of mine](https://github.com/denehoffman/rustitude-gluex/) which contains the spherical harmonic struct):
-```rust
-use rustitude::prelude::*;
-use rustitude_gluex::harmonics::{Wave, Ylm};
-
-fn main() {
-    // Load Datasets:
-    let data = Dataset::from_parquet("path/to/data.parquet", false);
-    let mc = Dataset::from_parquet("path/to/mc.parquet", false);
-    // Create Manager:
-    let mut m = ExtendedLogLikelihood::new(&data, &mc);
-    // Create Amplitudes:
-    let s0 = amplitude!("S0", Ylm::new(Wave::S0));
-    let d2 = amplitude!("D2", Ylm::new(Wave::D2));
-    let s0_amp = scalar!("S0 amp");
-    let d2_amp = cscalar!("D2 amp");
-    // Register Amplitudes:
-    m.register("", "S0", &s0);
-    m.register("", "S0", &s0_amp);
-    m.register("", "D2", &d2);
-    m.register("", "D2", &d2_amp);
-    // You can check the names of the free parameters and how many there are:
-    dbg!(m.parameters());
-    // prints:
-    // m.parameters() = [
-    // ("", "S0", "S0 amp", "value"),
-    // ("", "D2", "D2 amp", "real"),
-    // ("", "D2", "D2 amp", "imag"),
-    // ]
-    // Compute the negative log-likelihood:
-    let nll = dbg!(m.compute(&[1.0, 2.0, 3.0]));
-    std::hint::black_box(nll);
-}
-```
-Amplitudes are registered into a named `sum` and `group`. The typical calculation for any event $e$ and list of parameters $\overrightarrow{p}$ will then be:
+# Theory
+
+Amplitudes are registered into a named `sum` and `group`. Similar to `AmpTools`, the typical calculation for any event $e$ and list of parameters $\overrightarrow{p}$ will then be:
 ```math
 I(\overrightarrow{p}, e) = \sum_{\text{groups} \in \text{sums}}\left|\sum_{\text{amplitudes} \in \text{groups}} \prod_{\text{amp} \in \text{amplitudes}} \text{amp}(\overrightarrow{p}, e)\right|^2
 ```
 
-This is the behavior of a `Manager` struct, but more complex `Manage`-implementing structs like `ExtendedLogLikelihood` can be used to run analyses over more than one dataset at a time (data and Monte Carlo in this case) and compute other values like a negative log-likelihood.
-
-## Implementing an Amplitude
+# Installation
+Adding `rustitude` to an existing Rust project is as simple as
+```shell
+cargo add rustitude
+```
 
-While typical usage might be to use premade amplitudes in various combinations, it is important to know how to design an amplitude which will work seamlessly with this crate. Let's write down the Rustitude version of the [OmegaDalitz](https://github.com/JeffersonLab/halld_sim/blob/6544f01ac1514b0b9a53ad241cf2e8a63e1d3dfa/src/libraries/AMPTOOLS_AMPS/OmegaDalitz.cc) amplitude:
+The Python installation is equally straightforward:
+```shell
+pip install rustitude
+```
 
-```rust
-use rayon::prelude::*;
-use rustitude::prelude::*;
-
-#[derive(Default)]
-struct OmegaDalitz {
-    dalitz_z: Vec<f64>,
-    dalitz_sin3theta: Vec<f64>,
-    lambda: Vec<f64>,
-}
-
-impl Node for OmegaDalitz {
-    fn precalculate(&mut self, dataset: &Dataset) {
-        (self.dalitz_z, (self.dalitz_sin3theta, self.lambda)) = dataset
-            .par_iter()
-            .map(|event| {
-                let pi0 = event.daughter_p4s[0];
-                let pip = event.daughter_p4s[1];
-                let pim = event.daughter_p4s[2];
-                let omega = pi0 + pip + pim;
-
-                let dalitz_s = (pip + pim).m2();
-                let dalitz_t = (pip + pi0).m2();
-                let dalitz_u = (pim + pi0).m2();
-                
-                let m3pi = (2.0 * pip.m()) + pi0.m();
-                let dalitz_d = 2.0 * omega.m() * (omega.m() - m3pi);
-                let dalitz_sc = (1.0 / 3.0) * (omega.m2() + pip.m2() + pim.m2() + pi0.m2());
-                let dalitz_x = f64::sqrt(3.0) * (dalitz_t - dalitz_u) / dalitz_d;
-                let dalitz_y = 3.0 * (dalitz_sc - dalitz_s) / dalitz_d;
-                
-                let dalitz_z = dalitz_x * dalitz_x + dalitz_y * dalitz_y;
-                let dalitz_sin3theta = f64::sin(3.0 * f64::asin(dalitz_y / f64::sqrt(dalitz_z)));
-                
-                let pip_omega = pip.boost_along(&omega);
-                let pim_omega = pim.boost_along(&omega);
-                let pi_cross = pip_omega.momentum().cross(&pim_omega.momentum());
-                
-                let lambda = (4.0 / 3.0) * f64::abs(pi_cross.dot(&pi_cross))
-                    / ((1.0 / 9.0) * (omega.m2() - (2.0 * pip.m() + pi0.m()).powi(2)).powi(2));
-                    
-                (dalitz_z, (dalitz_sin3theta, lambda))
-            })
-            .unzip();
-    }
-
-    fn calculate(&self, parameters: &[f64], event: &Event) -> Complex64 {
-        let dalitz_z = self.dalitz_z[event.index];
-        let dalitz_sin3theta = self.dalitz_sin3theta[event.index];
-        let lambda = self.lambda[event.index];
-        let alpha = parameters[0];
-        let beta = parameters[1];
-        let gamma = parameters[2];
-        let delta = parameters[3];
-        f64::sqrt(f64::abs(
-            lambda
-                * (1.0
-                    + 2.0 * alpha * dalitz_z
-                    + 2.0 * beta * dalitz_z.powf(3.0 / 2.0) * dalitz_sin3theta
-                    + 2.0 * gamma * dalitz_z.powi(2)
-                    + 2.0 * delta * dalitz_z.powf(5.0 / 2.0) * dalitz_sin3theta),
-        ))
-        .into()
-    }
-
-    fn parameters(&self) -> Option<Vec<String>> {
-        Some(vec![
-            "alpha".to_string(),
-            "beta".to_string(),
-            "gamma".to_string(),
-            "delta".to_string(),
-        ])
-    }
-}
-
-fn main() {
-    let data = Dataset::from_parquet("data.parquet", false);
-    let mut m = Manager::new(&data);
-    let dalitz = amplitude!("Omega Dalitz", OmegaDalitz::default())
-    m.register("", "", &dalitz);
-    let res: Vec<f64> = m.compute(&[1.1, 2.2, 3.3, 4.4]);
-    println!("First event result: {}", res[0]);
-}
+# Usage
+See the [`rustitude-core`](https://github.com/denehoffman/rustitude-core) crate for a more in-depth tutorial on writing custom amplitudes in Rust. This package is mostly focused on the Python side of things. Here is the setup for an example analysis:
+```python
+import rustitude as rt
+from rustitude import gluex
+import numpy as np
+
+# Load data files
+# This uses uproot under the hood
+ds = rt.open('data.root')
+ds_mc = rt.open('mc.root')
+
+# Create a new "manager" to handle the interface between data and amplitudes
+m = rt.ExtendedLogLikelihood(ds, ds_mc)
+
+# Register some amplitudes
+# We provide a sum name, group name, and a named amplitude
+# This function also runs the precalculation method over the datasets
+m.register('pos re', 'S', gluex.resonances.KMatrixF0('f0', channel=2))
+m.register('pos re', 'S', gluex.resonances.KMatrixA0('a0', channel=1))
+m.register('pos re', 'S', gluex.harmonics.Zlm('z00', 0, 0, reflectivity='+', part='real'))
+m.register('pos re', 'D', gluex.resonances.KMatrixF2('f2', channel=2))
+m.register('pos re', 'D', gluex.resonances.KMatrixA2('a2', channel=1))
+m.register('pos re', 'D', gluex.harmonics.Zlm('z22', 0, 0, reflectivity='+', part='real'))
+
+m.register('pos im', 'S', gluex.resonances.KMatrixF0('f0', channel=2))
+m.register('pos im', 'S', gluex.resonances.KMatrixA0('a0', channel=1))
+m.register('pos im', 'S', gluex.harmonics.Zlm('z00', 0, 0, reflectivity='+', part='imag'))
+m.register('pos im', 'D', gluex.resonances.KMatrixF2('f2', channel=2))
+m.register('pos im', 'D', gluex.resonances.KMatrixA2('a2', channel=1))
+m.register('pos im', 'D', gluex.harmonics.Zlm('z22', 0, 0, reflectivity='+', part='imag'))
+
+# We can constrain all the free parameters of one amplitude to be equal to those of another,
+# provided they have the same free parameters. To constrain an individual amplitude, we can use
+# m.constrain(('pos re', 'S', 'f0', 'f0_500 re'), ('pos re', 'S', 'f0', 'f0_500 im')) for example,
+# which would make the real and imaginary part of equal to each other in the calculation.
+# This step reduces the number of free parameters in the calculation.
+m.constrain_amplitude(('pos re', 'S', 'f0'), ('pos im', 'S', 'f0'))
+m.constrain_amplitude(('pos re', 'S', 'a0'), ('pos im', 'S', 'a0'))
+m.constrain_amplitude(('pos re', 'D', 'f2'), ('pos im', 'D', 'f2'))
+m.constrain_amplitude(('pos re', 'D', 'a2'), ('pos im', 'D', 'a2'))
+
+# Fix some parameters to a given value (zero in this case)
+m.fix(('pos re', 'S', 'f0', 'f0_500 re'), 0.0)
+m.fix(('pos re', 'S', 'f0', 'f0_500 im'), 0.0)
+m.fix(('pos re', 'S', 'f0', 'f0_980 im'), 0.0)
+
+m.register('neg re', 'S', gluex.resonances.KMatrixF0('f0', channel=2))
+m.register('neg re', 'S', gluex.resonances.KMatrixA0('a0', channel=1))
+m.register('neg re', 'S', gluex.harmonics.Zlm('z00', 0, 0, reflectivity='-', part='real'))
+
+m.register('neg im', 'S', gluex.resonances.KMatrixF0('f0', channel=2))
+m.register('neg im', 'S', gluex.resonances.KMatrixA0('a0', channel=1))
+m.register('neg im', 'S', gluex.harmonics.Zlm('z00', 0, 0, reflectivity='-', part='imag'))
+
+m.constrain_amplitude(('neg re', 'S', 'f0'), ('neg im', 'S', 'f0'))
+m.constrain_amplitude(('neg re', 'S', 'a0'), ('neg im', 'S', 'a0'))
+
+m.fix(('neg re', 'S', 'f0', 'f0_500 re'), 0.0)
+m.fix(('neg re', 'S', 'f0', 'f0_500 im'), 0.0)
+m.fix(('neg re', 'S', 'f0', 'f0_980 im'), 0.0)
+
+# Calculate the negative log-likelihood given some random input parameters:
+rng = np.random.default_rng()
+nll = m(rng.random(len(m.parameters())) * 100.0)
 ```
 
+See the [`rustitude-gluex`](https://github.com/denehoffman/rustitude-gluex) package for some of the currently implemented amplitudes (derived from GlueX's [halld_sim](https://github.com/JeffersonLab/halld_sim) repo). There are also some helper methods `scalar`, `cscalar`, and `pcscalar` to create amplitudes which represent a single free parameter, a single complex free parameter, and a single complex free parameter in polar coordinates respectively.
+
 # TODOs
 In no particular order, here is a list of what (probably) needs to be done before I will stop making any breaking changes:
-- [ ] Create convenience methods for binned fits
-- [x] Formalize parameters into their own struct for pretty-printing and ease of use
-- [x] Create alternate methods of including polarization
-- [ ] Read raw ROOT files
-- [ ] Add plotting methods
-- [ ] A way to check if the number of parameters matches the input at compile time would be nice, not sure if it's possible though
-- [ ] If the parameters are formalized, I could include upper and lower bounds somehow as well as preferred initial values or randomization
-- [ ] Lots of documentation
-- [ ] Lots of tests
-
+- Pure Rust parsing of ROOT files without the `uproot` backend (I have some moderate success with `oxyroot`, but there are still a few issues reading larger files)
+- Add plotting methods
+- A way to check if the number of parameters matches the input at compile time would be nice, not sure if it's possible though
+- Give managers a way to apply amplitudes to new datasets, like using the result from a fit to weight some generated Monte-Carlo for plotting the result. This is possible to do through Python, but a convenience method is probably needed
+- Lots of documentation
+- Lots of tests
```

#### html2text {}

```diff
@@ -1,120 +1,143 @@
-Metadata-Version: 2.3 Name: rustitude Version: 0.3.3 Classifier: Development
-Status :: 4 - Beta Classifier: Programming Language :: Python License-File:
-LICENSE Summary: Python bindings for the Rustitude library Keywords:
-physics,math,rust Home-Page: https://github.com/denehoffman/rustitude/ Author:
-Nathaniel Dene Hoffman Author-email: dene@cmu.edu Maintainer-email: Nathaniel
-Dene Hoffman
-cmu.edu> License: BSD-3-Clause Requires-Python: >=3.7 Description-Content-Type:
-text/markdown; charset=UTF-8; variant=GFM Project-URL: homepage, https://
-github.com/denehoffman/rustitude Project-URL: repository, https://github.com/
-denehoffman/rustitude Project-URL: changelog, https://github.com/denehoffman/
-rustitude/blob/main/CHANGELOG.md
  [https://raw.githubusercontent.com/denehoffman/rustitude/main/media/logo.png]
                  ************ DDeemmyyssttiiffyyiinngg AAmmpplliittuuddee AAnnaallyyssiiss ************
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_l_a_s_t_-_c_o_m_m_i_t_/_d_e_n_e_h_o_f_f_m_a_n_/_r_u_s_t_i_t_u_d_e_/_m_a_i_n_]_[_h_t_t_p_s_:_/_/
  _i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_/_s_t_a_t_u_s_/_d_e_n_e_h_o_f_f_m_a_n_/_r_u_s_t_i_t_u_d_e_/_r_u_s_t_._y_m_l_]
     _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_l_i_c_e_n_s_e_/_d_e_n_e_h_o_f_f_m_a_n_/_r_u_s_t_i_t_u_d_e_]_[_h_t_t_p_s_:_/_/
   _i_m_g_._s_h_i_e_l_d_s_._i_o_/_c_r_a_t_e_s_/_v_/_r_u_s_t_i_t_u_d_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_d_o_c_s_r_s_/_r_u_s_t_i_t_u_d_e_]
-### Note: This project is still very much under development and not recommended
-for use in actual research projects (yet) ### Table of Contents - [Overview]
-(#Overview) - [Installation](#Installation) - [Usage](#Usage) ## Overview
-Amplitude analysis is the scientific process of fitting models (amplitudes) to
-data in order to extract additional information. In particle physics, this is
-often synonymous with partial-wave analysis (PWA), a process commonly used to
-determine angular momentum quantum numbers for decaying particles. The goal of
-Rustitude is to establish a framework which is generic enough to fit almost any
-data to any model, but specific enough to be quick and easy to use in typical
-particle physics studies. There are three core ideas which this crate tries to
-follow to make fits fast and efficient: 1. Every function is automatically
-paralellized over the dataset using [rayon](https://github.com/rayon-rs/rayon).
-2. Model builders can separate their code efficiently into pieces which only
-need to be calculated once for the whole dataset and those which depend on
-parameters, which could change at every evaluation. Amplitudes implement
-`Node`, which is a trait containing all the required methods for an amplitude
-to be used in an analysis. By precalculating things which don't change, we
-trade RAM usage now for evaluation speed later. 3. `Dataset` structs only allow
-`Event` structs to be stored, so there is a fixed format that implementers must
-agree on. As it stands, this format closely follows that of [AmpTools](https://
-github.com/mashephe/AmpTools), but with the addition of a polarization vector.
-This format can be added to in the future without breaking backwards
-compatibility, but members should probably not be removed or modified.
-Unfortunately, ROOT files do not yet have well-documented R/W libraries like
-Python's [uproot](https://pypi.org/project/uproot/) or Julia's [UpROOT.jl]
-(https://github.com/JuliaHEP/UpROOT.jl), so the current recommendation is to
-convert files to a more versatile format like parquet. A ROOT-free Python
-conversion script is included [here](convert). ## Installation Cargo provides
-the usual command for including this crate in a project: ```sh cargo add
-rustitude ``` ## Usage The basic usage pattern is as follows. We start by
-importing our data files, we create the amplitudes we want to use, we register
-them with a `Manager` struct that handles all the internal sums and parameters,
-and then we evaluate the resulting model. For example, we can generate a model
-which takes evaluates two spherical harmonics as follows (this uses some code
-from [another repo of mine](https://github.com/denehoffman/rustitude-gluex/
-) which contains the spherical harmonic struct): ```rust use rustitude::
-prelude::*; use rustitude_gluex::harmonics::{Wave, Ylm}; fn main() { // Load
-Datasets: let data = Dataset::from_parquet("path/to/data.parquet", false); let
-mc = Dataset::from_parquet("path/to/mc.parquet", false); // Create Manager: let
-mut m = ExtendedLogLikelihood::new(&data, &mc); // Create Amplitudes: let s0 =
-amplitude!("S0", Ylm::new(Wave::S0)); let d2 = amplitude!("D2", Ylm::new(Wave::
-D2)); let s0_amp = scalar!("S0 amp"); let d2_amp = cscalar!("D2 amp"); /
-/ Register Amplitudes: m.register("", "S0", &s0); m.register("", "S0",
-&s0_amp); m.register("", "D2", &d2); m.register("", "D2", &d2_amp); // You can
-check the names of the free parameters and how many there are: dbg!
-(m.parameters()); // prints: // m.parameters() = [ // ("", "S0", "S0 amp",
-"value"), // ("", "D2", "D2 amp", "real"), // ("", "D2", "D2 amp", "imag"), /
-/ ] // Compute the negative log-likelihood: let nll = dbg!(m.compute(&[1.0,
-2.0, 3.0])); std::hint::black_box(nll); } ``` Amplitudes are registered into a
-named `sum` and `group`. The typical calculation for any event $e$ and list of
-parameters $\overrightarrow{p}$ will then be: ```math I(\overrightarrow{p}, e)
-= \sum_{\text{groups} \in \text{sums}}\left|\sum_{\text{amplitudes} \in \text
-{groups}} \prod_{\text{amp} \in \text{amplitudes}} \text{amp}(\overrightarrow
-{p}, e)\right|^2 ``` This is the behavior of a `Manager` struct, but more
-complex `Manage`-implementing structs like `ExtendedLogLikelihood` can be used
-to run analyses over more than one dataset at a time (data and Monte Carlo in
-this case) and compute other values like a negative log-likelihood. ##
-Implementing an Amplitude While typical usage might be to use premade
-amplitudes in various combinations, it is important to know how to design an
-amplitude which will work seamlessly with this crate. Let's write down the
-Rustitude version of the [OmegaDalitz](https://github.com/JeffersonLab/
-halld_sim/blob/6544f01ac1514b0b9a53ad241cf2e8a63e1d3dfa/src/libraries/
-AMPTOOLS_AMPS/OmegaDalitz.cc) amplitude: ```rust use rayon::prelude::*; use
-rustitude::prelude::*; #[derive(Default)] struct OmegaDalitz { dalitz_z: Vec,
-dalitz_sin3theta: Vec, lambda: Vec, } impl Node for OmegaDalitz { fn
-precalculate(&mut self, dataset: &Dataset) { (self.dalitz_z,
-(self.dalitz_sin3theta, self.lambda)) = dataset .par_iter() .map(|event| { let
-pi0 = event.daughter_p4s[0]; let pip = event.daughter_p4s[1]; let pim =
-event.daughter_p4s[2]; let omega = pi0 + pip + pim; let dalitz_s = (pip +
-pim).m2(); let dalitz_t = (pip + pi0).m2(); let dalitz_u = (pim + pi0).m2();
-let m3pi = (2.0 * pip.m()) + pi0.m(); let dalitz_d = 2.0 * omega.m() * (omega.m
-() - m3pi); let dalitz_sc = (1.0 / 3.0) * (omega.m2() + pip.m2() + pim.m2() +
-pi0.m2()); let dalitz_x = f64::sqrt(3.0) * (dalitz_t - dalitz_u) / dalitz_d;
-let dalitz_y = 3.0 * (dalitz_sc - dalitz_s) / dalitz_d; let dalitz_z = dalitz_x
-* dalitz_x + dalitz_y * dalitz_y; let dalitz_sin3theta = f64::sin(3.0 * f64::
-asin(dalitz_y / f64::sqrt(dalitz_z))); let pip_omega = pip.boost_along(ω); let
-pim_omega = pim.boost_along(ω); let pi_cross = pip_omega.momentum().cross
-(&pim_omega.momentum()); let lambda = (4.0 / 3.0) * f64::abs(pi_cross.dot
-(π_cross)) / ((1.0 / 9.0) * (omega.m2() - (2.0 * pip.m() + pi0.m()).powi
-(2)).powi(2)); (dalitz_z, (dalitz_sin3theta, lambda)) }) .unzip(); } fn
-calculate(&self, parameters: &[f64], event: &Event) -> Complex64 { let dalitz_z
-= self.dalitz_z[event.index]; let dalitz_sin3theta = self.dalitz_sin3theta
-[event.index]; let lambda = self.lambda[event.index]; let alpha = parameters
-[0]; let beta = parameters[1]; let gamma = parameters[2]; let delta =
-parameters[3]; f64::sqrt(f64::abs( lambda * (1.0 + 2.0 * alpha * dalitz_z + 2.0
-* beta * dalitz_z.powf(3.0 / 2.0) * dalitz_sin3theta + 2.0 * gamma *
-dalitz_z.powi(2) + 2.0 * delta * dalitz_z.powf(5.0 / 2.0) * dalitz_sin3theta),
-)) .into() } fn parameters(&self) -> Option
-String>> { Some(vec![ "alpha".to_string(), "beta".to_string(),
-"gamma".to_string(), "delta".to_string(), ]) } } fn main() { let data =
-Dataset::from_parquet("data.parquet", false); let mut m = Manager::new(&data);
-let dalitz = amplitude!("Omega Dalitz", OmegaDalitz::default()) m.register("",
-"", &dalitz); let res: Vec = m.compute(&[1.1, 2.2, 3.3, 4.4]); println!("First
-event result: {}", res[0]); } ``` # TODOs In no particular order, here is a
-list of what (probably) needs to be done before I will stop making any breaking
-changes: - [ ] Create convenience methods for binned fits - [x] Formalize
-parameters into their own struct for pretty-printing and ease of use - [x]
-Create alternate methods of including polarization - [ ] Read raw ROOT files -
-[ ] Add plotting methods - [ ] A way to check if the number of parameters
-matches the input at compile time would be nice, not sure if it's possible
-though - [ ] If the parameters are formalized, I could include upper and lower
-bounds somehow as well as preferred initial values or randomization - [ ] Lots
-of documentation - [ ] Lots of tests
+### Table of Contents: - [Introduction](#Introduction) - [Theory](#Theory) -
+[Installation](#Installation) - [Usage](#Usage) - [TODOs](#TODOs) #
+Introduction This project began with a desire to make a fast but easy to use
+interface for fitting amplitudes to particle physics data. That being said,
+there are performant methods such as [`AmpTools`](https://github.com/mashephe/
+AmpTools), which is written in C++, but in my personal experience, it can be a
+bit tricky to use and extend, and it generally requires a lot of boilerplate
+code to generate new amplitudes or plotting scripts. On the other hand, there
+are also libraries like [`PyPWA`](https://github.com/JeffersonLab/PyPWA/)
+(written in Python) which seem like they could be easy to use, but often fail
+in this aspect due to Python's limiting syntax, speed issues, and a general
+lack of documentation and ongoing development. There have been attempts to
+bridge the gap between AmpTools and Python, most recently (and successfully)
+[`PyAmpTools`](https://github.com/lan13005/PyAmpTools). The difficulty with
+this method is that it relies on PyROOT, which also means you need ROOT
+installed (and built with your version of Python). For now, I'll spare you the
+anti-ROOT rant and just say that ROOT should be an opt-in, not a requirement.
+So where does that leave `rustitude`? As the name suggests, `rustitude` was
+written in Rust, so let's get the obvious downside out of the way: not many
+particle physicists know how to write Rust code. Hopefully, this will change
+over the next decade (and there has already been some [support](https://
+www.whitehouse.gov/oncd/briefing-room/2024/02/26/memory-safety-statements-of-
+support/) from the US government, of all places). While Rust carries the
+disadvantage of relative obscurity compared to C++, it also has many benefits.
+No `null` means no null references (Tony Hoare's ["billion dollar mistake"]
+(https://web.archive.org/web/20090628071208/http://qconlondon.com/london-2009/
+speaker/Tony+Hoare)). Pointers (called references in Rust) are always valid, a
+guarantee made by a very helpful and only occasionally frustrating borrow
+checker. Rust "crates" are set up in a way which encourages documentation (see
+[`rustitude-core`'s documentation](https://docs.rs/rustitude-core/)), and the
+basic syntax is fairly easy to learn for people who have been using optional
+type checking in Python. Perhaps one of the biggest benefits of Rust is how
+easy it is to employ [parallelization](https://crates.io/crates/rayon), but the
+two reasons I like it most are that it's incredibly easy to write Python
+bindings (that's what this library is after all) and it has a package manager.
+This second point is important -- unlike C/C++, where a developer is swamped
+with some menagerie `Makefile`, `CMakeLists.txt`, or some `scons` monstrosity
+which may only work on "X" system and only if you install and use `make`,
+`cmake`, `g++`, or whatever (oh yeah, and you made sure all your external
+dependencies are linked correctly, right? Right?), Rust supports adding a
+package by simply adding a line to `Cargo.toml` (or using the `cargo add`
+command). In many ways, package management in Rust is actually simpler than
+Python, since there's only one prefered method of creating and managing
+projects, formatting, linting, and compiling. Now I've covered why I don't like
+some of the existing solutions, and why I chose to use Rust, but what does this
+project have that makes it stand out? Here are some reasons to entice you: -
+`rustitude` will automatically parallelize amplitudes over the events in a
+dataset. There's no reason for a developer to ever write parallelized code
+themselves. - Implementing [`Node`](https://docs.rs/rustitude-core/latest/
+rustitude_core/amplitude/trait.Node.html) on a struct is all that is needed to
+use it as an amplitude. This means developers need only write two to three
+total methods to describe the entire functionality of their amplitude, and one
+of these just gives the names and order of the amplitude's input parameters. -
+A major goal of `rustitude` was to increase processing speed by sacrificing
+memory. This is done by precalculating parts of amplitudes which don't change
+when the free parameter inputs change. `AmpTools` supports a version of this,
+but only on the level of each general amplitude rather than on an individual
+basis. The simplest example of this is the `Ylm` amplitude (spherical
+harmonic), which can be entirely precalculated given the value of `l` and `m`.
+In `AmpTools`, different instances of `Ylm` with different `l`s and `m`s share
+precalculated data, whereas in `rustitude`, they don't. The `AmpTools`
+implementation of `Ylm` needs to calculate a spherical harmonic for every event
+on every function call, while `rustitude` just needs to look up a value in an
+array! - The majority of the library (the public interface) has Python
+bindings, so if there is no need for custom amplitudes, a developer never
+actually has to write any Rust code, and the resulting calculations will be as
+performant as if they were written in Rust. # Theory Amplitudes are registered
+into a named `sum` and `group`. Similar to `AmpTools`, the typical calculation
+for any event $e$ and list of parameters $\overrightarrow{p}$ will then be:
+```math I(\overrightarrow{p}, e) = \sum_{\text{groups} \in \text
+{sums}}\left|\sum_{\text{amplitudes} \in \text{groups}} \prod_{\text{amp} \in
+\text{amplitudes}} \text{amp}(\overrightarrow{p}, e)\right|^2 ``` #
+Installation Adding `rustitude` to an existing Rust project is as simple as
+```shell cargo add rustitude ``` The Python installation is equally
+straightforward: ```shell pip install rustitude ``` # Usage See the
+[`rustitude-core`](https://github.com/denehoffman/rustitude-core) crate for a
+more in-depth tutorial on writing custom amplitudes in Rust. This package is
+mostly focused on the Python side of things. Here is the setup for an example
+analysis: ```python import rustitude as rt from rustitude import gluex import
+numpy as np # Load data files # This uses uproot under the hood ds = rt.open
+('data.root') ds_mc = rt.open('mc.root') # Create a new "manager" to handle the
+interface between data and amplitudes m = rt.ExtendedLogLikelihood(ds, ds_mc) #
+Register some amplitudes # We provide a sum name, group name, and a named
+amplitude # This function also runs the precalculation method over the datasets
+m.register('pos re', 'S', gluex.resonances.KMatrixF0('f0', channel=2))
+m.register('pos re', 'S', gluex.resonances.KMatrixA0('a0', channel=1))
+m.register('pos re', 'S', gluex.harmonics.Zlm('z00', 0, 0, reflectivity='+',
+part='real')) m.register('pos re', 'D', gluex.resonances.KMatrixF2('f2',
+channel=2)) m.register('pos re', 'D', gluex.resonances.KMatrixA2('a2',
+channel=1)) m.register('pos re', 'D', gluex.harmonics.Zlm('z22', 0, 0,
+reflectivity='+', part='real')) m.register('pos im', 'S',
+gluex.resonances.KMatrixF0('f0', channel=2)) m.register('pos im', 'S',
+gluex.resonances.KMatrixA0('a0', channel=1)) m.register('pos im', 'S',
+gluex.harmonics.Zlm('z00', 0, 0, reflectivity='+', part='imag')) m.register
+('pos im', 'D', gluex.resonances.KMatrixF2('f2', channel=2)) m.register('pos
+im', 'D', gluex.resonances.KMatrixA2('a2', channel=1)) m.register('pos im',
+'D', gluex.harmonics.Zlm('z22', 0, 0, reflectivity='+', part='imag')) # We can
+constrain all the free parameters of one amplitude to be equal to those of
+another, # provided they have the same free parameters. To constrain an
+individual amplitude, we can use # m.constrain(('pos re', 'S', 'f0', 'f0_500
+re'), ('pos re', 'S', 'f0', 'f0_500 im')) for example, # which would make the
+real and imaginary part of equal to each other in the calculation. # This step
+reduces the number of free parameters in the calculation. m.constrain_amplitude
+(('pos re', 'S', 'f0'), ('pos im', 'S', 'f0')) m.constrain_amplitude(('pos re',
+'S', 'a0'), ('pos im', 'S', 'a0')) m.constrain_amplitude(('pos re', 'D', 'f2'),
+('pos im', 'D', 'f2')) m.constrain_amplitude(('pos re', 'D', 'a2'), ('pos im',
+'D', 'a2')) # Fix some parameters to a given value (zero in this case) m.fix(
+('pos re', 'S', 'f0', 'f0_500 re'), 0.0) m.fix(('pos re', 'S', 'f0', 'f0_500
+im'), 0.0) m.fix(('pos re', 'S', 'f0', 'f0_980 im'), 0.0) m.register('neg re',
+'S', gluex.resonances.KMatrixF0('f0', channel=2)) m.register('neg re', 'S',
+gluex.resonances.KMatrixA0('a0', channel=1)) m.register('neg re', 'S',
+gluex.harmonics.Zlm('z00', 0, 0, reflectivity='-', part='real')) m.register
+('neg im', 'S', gluex.resonances.KMatrixF0('f0', channel=2)) m.register('neg
+im', 'S', gluex.resonances.KMatrixA0('a0', channel=1)) m.register('neg im',
+'S', gluex.harmonics.Zlm('z00', 0, 0, reflectivity='-', part='imag'))
+m.constrain_amplitude(('neg re', 'S', 'f0'), ('neg im', 'S', 'f0'))
+m.constrain_amplitude(('neg re', 'S', 'a0'), ('neg im', 'S', 'a0')) m.fix(('neg
+re', 'S', 'f0', 'f0_500 re'), 0.0) m.fix(('neg re', 'S', 'f0', 'f0_500 im'),
+0.0) m.fix(('neg re', 'S', 'f0', 'f0_980 im'), 0.0) # Calculate the negative
+log-likelihood given some random input parameters: rng = np.random.default_rng
+() nll = m(rng.random(len(m.parameters())) * 100.0) ``` See the [`rustitude-
+gluex`](https://github.com/denehoffman/rustitude-gluex) package for some of the
+currently implemented amplitudes (derived from GlueX's [halld_sim](https://
+github.com/JeffersonLab/halld_sim) repo). There are also some helper methods
+`scalar`, `cscalar`, and `pcscalar` to create amplitudes which represent a
+single free parameter, a single complex free parameter, and a single complex
+free parameter in polar coordinates respectively. # TODOs In no particular
+order, here is a list of what (probably) needs to be done before I will stop
+making any breaking changes: - Pure Rust parsing of ROOT files without the
+`uproot` backend (I have some moderate success with `oxyroot`, but there are
+still a few issues reading larger files) - Add plotting methods - A way to
+check if the number of parameters matches the input at compile time would be
+nice, not sure if it's possible though - Give managers a way to apply
+amplitudes to new datasets, like using the result from a fit to weight some
+generated Monte-Carlo for plotting the result. This is possible to do through
+Python, but a convenience method is probably needed - Lots of documentation -
+Lots of tests
```

