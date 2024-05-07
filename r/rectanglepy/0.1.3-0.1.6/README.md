# Comparing `tmp/rectanglepy-0.1.3.tar.gz` & `tmp/rectanglepy-0.1.6.tar.gz`

## Comparing `rectanglepy-0.1.3.tar` & `rectanglepy-0.1.6.tar`

### file list

```diff
@@ -1,52 +1,53 @@
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 rectanglepy-0.1.3/.bumpversion.cfg
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 rectanglepy-0.1.3/.cruft.json
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 rectanglepy-0.1.3/.editorconfig
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 rectanglepy-0.1.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 rectanglepy-0.1.3/.readthedocs.yaml
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 rectanglepy-0.1.3/CHANGELOG.md
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 rectanglepy-0.1.3/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 rectanglepy-0.1.3/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 rectanglepy-0.1.3/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 rectanglepy-0.1.3/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 rectanglepy-0.1.3/.github/workflows/build.yaml
--rw-r--r--   0        0        0     2489 2020-02-02 00:00:00.000000 rectanglepy-0.1.3/.github/workflows/release.yaml
--rw-r--r--   0        0        0     1365 2020-02-02 00:00:00.000000 rectanglepy-0.1.3/.github/workflows/test.yaml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 rectanglepy-0.1.3/docs/Makefile
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 rectanglepy-0.1.3/docs/api.md
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 rectanglepy-0.1.3/docs/changelog.md
--rw-r--r--   0        0        0     4203 2020-02-02 00:00:00.000000 rectanglepy-0.1.3/docs/conf.py
--rw-r--r--   0        0        0     7832 2020-02-02 00:00:00.000000 rectanglepy-0.1.3/docs/contributing.md
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 rectanglepy-0.1.3/docs/index.md
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 rectanglepy-0.1.3/docs/make.bat
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 rectanglepy-0.1.3/docs/references.bib
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 rectanglepy-0.1.3/docs/references.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rectanglepy-0.1.3/docs/_static/.gitkeep
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rectanglepy-0.1.3/docs/_templates/.gitkeep
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 rectanglepy-0.1.3/docs/_templates/autosummary/class.rst
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 rectanglepy-0.1.3/docs/extensions/typed_returns.py
--rw-r--r--   0        0        0    14330 2020-02-02 00:00:00.000000 rectanglepy-0.1.3/docs/notebooks/example.ipynb
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 rectanglepy-0.1.3/src/rectanglepy/__init__.py
--rw-r--r--   0        0        0     4843 2020-02-02 00:00:00.000000 rectanglepy-0.1.3/src/rectanglepy/rectangle.py
--rw-r--r--   0        0        0    10478 2020-02-02 00:00:00.000000 rectanglepy-0.1.3/src/rectanglepy/data/hao1_annotations_small.zip
--rw-r--r--   0        0        0  1423449 2020-02-02 00:00:00.000000 rectanglepy-0.1.3/src/rectanglepy/data/hao1_counts_small.zip
--rw-r--r--   0        0        0   296709 2020-02-02 00:00:00.000000 rectanglepy-0.1.3/src/rectanglepy/data/small_fino_bulks.zip
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 rectanglepy-0.1.3/src/rectanglepy/pp/__init__.py
--rw-r--r--   0        0        0    19253 2020-02-02 00:00:00.000000 rectanglepy-0.1.3/src/rectanglepy/pp/create_signature.py
--rw-r--r--   0        0        0     3468 2020-02-02 00:00:00.000000 rectanglepy-0.1.3/src/rectanglepy/pp/rectangle_signature.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 rectanglepy-0.1.3/src/rectanglepy/tl/__init__.py
--rw-r--r--   0        0        0    14808 2020-02-02 00:00:00.000000 rectanglepy-0.1.3/src/rectanglepy/tl/deconvolution.py
--rw-r--r--   0        0        0     9140 2020-02-02 00:00:00.000000 rectanglepy-0.1.3/tests/test_pp.py
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 rectanglepy-0.1.3/tests/test_rectangle.py
--rw-r--r--   0        0        0     4628 2020-02-02 00:00:00.000000 rectanglepy-0.1.3/tests/test_tl.py
--rw-r--r--   0        0        0    28466 2020-02-02 00:00:00.000000 rectanglepy-0.1.3/tests/data/TIL10_signature.txt
--rw-r--r--   0        0        0   132044 2020-02-02 00:00:00.000000 rectanglepy-0.1.3/tests/data/bulk_small.csv
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 rectanglepy-0.1.3/tests/data/cell_annotations_small.txt
--rw-r--r--   0        0        0  2201267 2020-02-02 00:00:00.000000 rectanglepy-0.1.3/tests/data/quanTIseq_SimRNAseq_mixture_smaller.csv
--rw-r--r--   0        0        0     2537 2020-02-02 00:00:00.000000 rectanglepy-0.1.3/tests/data/quanTIseq_SimRNAseq_read_fractions_small.txt
--rw-r--r--   0        0        0   274597 2020-02-02 00:00:00.000000 rectanglepy-0.1.3/tests/data/sc_object_small.csv
--rw-r--r--   0        0        0   312634 2020-02-02 00:00:00.000000 rectanglepy-0.1.3/tests/data/signature_hao1.csv
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 rectanglepy-0.1.3/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 rectanglepy-0.1.3/LICENSE
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 rectanglepy-0.1.3/README.md
--rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 rectanglepy-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     4209 2020-02-02 00:00:00.000000 rectanglepy-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 rectanglepy-0.1.6/.bumpversion.cfg
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 rectanglepy-0.1.6/.cruft.json
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 rectanglepy-0.1.6/.editorconfig
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 rectanglepy-0.1.6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 rectanglepy-0.1.6/.readthedocs.yaml
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 rectanglepy-0.1.6/CHANGELOG.md
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 rectanglepy-0.1.6/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 rectanglepy-0.1.6/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 rectanglepy-0.1.6/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 rectanglepy-0.1.6/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 rectanglepy-0.1.6/.github/workflows/build.yaml
+-rw-r--r--   0        0        0     2489 2020-02-02 00:00:00.000000 rectanglepy-0.1.6/.github/workflows/release.yaml
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 rectanglepy-0.1.6/.github/workflows/release_testpypi.yaml
+-rw-r--r--   0        0        0     1365 2020-02-02 00:00:00.000000 rectanglepy-0.1.6/.github/workflows/test.yaml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 rectanglepy-0.1.6/docs/Makefile
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 rectanglepy-0.1.6/docs/api.md
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 rectanglepy-0.1.6/docs/changelog.md
+-rw-r--r--   0        0        0     4203 2020-02-02 00:00:00.000000 rectanglepy-0.1.6/docs/conf.py
+-rw-r--r--   0        0        0     7832 2020-02-02 00:00:00.000000 rectanglepy-0.1.6/docs/contributing.md
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 rectanglepy-0.1.6/docs/index.md
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 rectanglepy-0.1.6/docs/make.bat
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 rectanglepy-0.1.6/docs/references.bib
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 rectanglepy-0.1.6/docs/references.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rectanglepy-0.1.6/docs/_static/.gitkeep
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rectanglepy-0.1.6/docs/_templates/.gitkeep
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 rectanglepy-0.1.6/docs/_templates/autosummary/class.rst
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 rectanglepy-0.1.6/docs/extensions/typed_returns.py
+-rw-r--r--   0        0        0    14941 2020-02-02 00:00:00.000000 rectanglepy-0.1.6/docs/notebooks/example.ipynb
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 rectanglepy-0.1.6/src/rectanglepy/__init__.py
+-rw-r--r--   0        0        0     7909 2020-02-02 00:00:00.000000 rectanglepy-0.1.6/src/rectanglepy/rectangle.py
+-rw-r--r--   0        0        0    10478 2020-02-02 00:00:00.000000 rectanglepy-0.1.6/src/rectanglepy/data/hao1_annotations_small.zip
+-rw-r--r--   0        0        0  1423449 2020-02-02 00:00:00.000000 rectanglepy-0.1.6/src/rectanglepy/data/hao1_counts_small.zip
+-rw-r--r--   0        0        0   296709 2020-02-02 00:00:00.000000 rectanglepy-0.1.6/src/rectanglepy/data/small_fino_bulks.zip
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 rectanglepy-0.1.6/src/rectanglepy/pp/__init__.py
+-rw-r--r--   0        0        0    19348 2020-02-02 00:00:00.000000 rectanglepy-0.1.6/src/rectanglepy/pp/create_signature.py
+-rw-r--r--   0        0        0     3119 2020-02-02 00:00:00.000000 rectanglepy-0.1.6/src/rectanglepy/pp/rectangle_signature.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 rectanglepy-0.1.6/src/rectanglepy/tl/__init__.py
+-rw-r--r--   0        0        0    14955 2020-02-02 00:00:00.000000 rectanglepy-0.1.6/src/rectanglepy/tl/deconvolution.py
+-rw-r--r--   0        0        0     9140 2020-02-02 00:00:00.000000 rectanglepy-0.1.6/tests/test_pp.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 rectanglepy-0.1.6/tests/test_rectangle.py
+-rw-r--r--   0        0        0     4628 2020-02-02 00:00:00.000000 rectanglepy-0.1.6/tests/test_tl.py
+-rw-r--r--   0        0        0    28466 2020-02-02 00:00:00.000000 rectanglepy-0.1.6/tests/data/TIL10_signature.txt
+-rw-r--r--   0        0        0   132044 2020-02-02 00:00:00.000000 rectanglepy-0.1.6/tests/data/bulk_small.csv
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 rectanglepy-0.1.6/tests/data/cell_annotations_small.txt
+-rw-r--r--   0        0        0  2201267 2020-02-02 00:00:00.000000 rectanglepy-0.1.6/tests/data/quanTIseq_SimRNAseq_mixture_smaller.csv
+-rw-r--r--   0        0        0     2537 2020-02-02 00:00:00.000000 rectanglepy-0.1.6/tests/data/quanTIseq_SimRNAseq_read_fractions_small.txt
+-rw-r--r--   0        0        0   274597 2020-02-02 00:00:00.000000 rectanglepy-0.1.6/tests/data/sc_object_small.csv
+-rw-r--r--   0        0        0   312634 2020-02-02 00:00:00.000000 rectanglepy-0.1.6/tests/data/signature_hao1.csv
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 rectanglepy-0.1.6/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 rectanglepy-0.1.6/LICENSE
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 rectanglepy-0.1.6/README.md
+-rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 rectanglepy-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     4209 2020-02-02 00:00:00.000000 rectanglepy-0.1.6/PKG-INFO
```

### Comparing `rectanglepy-0.1.3/.cruft.json` & `rectanglepy-0.1.6/.cruft.json`

 * *Files identical despite different names*

### Comparing `rectanglepy-0.1.3/.pre-commit-config.yaml` & `rectanglepy-0.1.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `rectanglepy-0.1.3/.github/ISSUE_TEMPLATE/bug_report.yml` & `rectanglepy-0.1.6/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `rectanglepy-0.1.3/.github/workflows/build.yaml` & `rectanglepy-0.1.6/.github/workflows/build.yaml`

 * *Files identical despite different names*

### Comparing `rectanglepy-0.1.3/.github/workflows/release.yaml` & `rectanglepy-0.1.6/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `rectanglepy-0.1.3/.github/workflows/test.yaml` & `rectanglepy-0.1.6/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `rectanglepy-0.1.3/docs/Makefile` & `rectanglepy-0.1.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `rectanglepy-0.1.3/docs/conf.py` & `rectanglepy-0.1.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `rectanglepy-0.1.3/docs/contributing.md` & `rectanglepy-0.1.6/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `rectanglepy-0.1.3/docs/make.bat` & `rectanglepy-0.1.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `rectanglepy-0.1.3/docs/references.bib` & `rectanglepy-0.1.6/docs/references.bib`

 * *Files identical despite different names*

### Comparing `rectanglepy-0.1.3/docs/_templates/autosummary/class.rst` & `rectanglepy-0.1.6/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `rectanglepy-0.1.3/docs/extensions/typed_returns.py` & `rectanglepy-0.1.6/docs/extensions/typed_returns.py`

 * *Files identical despite different names*

### Comparing `rectanglepy-0.1.3/docs/notebooks/example.ipynb` & `rectanglepy-0.1.6/docs/notebooks/example.ipynb`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9883928571428572%*

 * *Differences: {"'cells'": "{14: {'source': 'signature_result is a "*

 * *            '[`RectangleSignatureResult`](../generated/rectanglepy.pp.RectangleSignatureResult.rst) '*

 * *            "object. '}, 15: {'source': '## Running Rectangle in Consensus mode'}, 16: {'source': "*

 * *            "'For some scRNA-seq datatasets it may be beneficial to run rectangle in consensus "*

 * *            'mode. In this function we run the rectangle algorithm multiple times '*

 * *            '(`consensus_runs`), where on each iteration we sample  `sample […]*

```diff
@@ -154,14 +154,19 @@
                 "collapsed": false
             },
             "source": [
                 "# Single step Rectangle workflow"
             ]
         },
         {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": "To deconvolute the bulk data in a single step, use the rectangle function. This function returns a tuple of the estimated cell type proportions and the signature result."
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "collapsed": false
             },
             "outputs": [],
             "source": [
@@ -194,47 +199,43 @@
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "collapsed": false
             },
-            "source": [
-                "signature_result is a [`RectangleSignatureResult`](../generated/rectanglepy.pp.RectangleSignatureResult.rst) object. Results of estimations vary slightly from machine to machine (due to difference in theunderlying linear algebra packages)"
-            ]
+            "source": "signature_result is a [`RectangleSignatureResult`](../generated/rectanglepy.pp.RectangleSignatureResult.rst) object. "
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "collapsed": false
             },
-            "source": [
-                "## Even sampling and consensus"
-            ]
+            "source": "## Running Rectangle in Consensus mode"
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "collapsed": false
             },
-            "source": [
-                "We recommend even subsampling of the sc data.\n",
-                "You can use the `sample_size` parameter to sample a fixed number of cells per cell type,  and run the consensus multiple times to get a more robust result."
-            ]
+            "source": "For some scRNA-seq datatasets it may be beneficial to run rectangle in consensus mode. In this function we run the rectangle algorithm multiple times (`consensus_runs`), where on each iteration we sample  `sample_size` cells of each cell type. The final cell type proportions are the median of the proportions estimated in each run."
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "collapsed": false
             },
             "outputs": [],
-            "source": [
-                "estimations, signature_result = rectangle.rectangle(sc_adata, bulks, consensus_runs=5, sample_size=1500)"
-            ]
+            "source": "estimations, signature_result, consensus_result = rectangle.rectangle_consens(sc_adata, bulks, consensus_runs=5, sample_size=1500)"
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": "signature_result holds the signature result([`RectangleSignatureResult`](../generated/rectanglepy.pp.RectangleSignatureResult.rst)) for the most recent consensus run, while consensus_result is a [`ConsensusResult`](../generated/rectanglepy.ConsensusResult.rst) object that holds the results of all the runs."
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "collapsed": false
             },
             "source": [
```

### Comparing `rectanglepy-0.1.3/src/rectanglepy/rectangle.py` & `rectanglepy-0.1.6/src/rectanglepy/rectangle.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,30 +4,46 @@
 from pandas import DataFrame
 from pkg_resources import resource_stream
 
 from .pp import RectangleSignatureResult, build_rectangle_signatures
 from .tl import deconvolution
 
 
-def rectangle(
+class ConsensusResult:
+    """A class used to represent the consensus result of the rectangle_consens function.
+
+    Parameters
+    ----------
+    estimations
+        A list of DataFrame objects representing the estimations from each consensus run.
+    rectangle_signature_results
+        A list of RectangleSignatureResult objects representing the rectangle signature results from each consensus run.
+    """
+
+    def __init__(self, estimations: list[DataFrame], rectangle_signature_results: list[RectangleSignatureResult]):
+        self.estimations = estimations
+        self.rectangle_signature_results = rectangle_signature_results
+
+
+def rectangle_consens(
     adata: AnnData,
     bulks: DataFrame,
     cell_type_col: str = "cell_type",
     *,
     layer: str = None,
     raw: bool = False,
-    subsample: bool = False,
+    subsample: bool = True,
     sample_size: int = 1500,
-    consensus_runs: int = 1,
+    consensus_runs: int = 5,
     correct_mrna_bias: bool = True,
     optimize_cutoffs=True,
     p=0.015,
     lfc=1.5,
     n_cpus: int = None,
-) -> tuple[DataFrame, RectangleSignatureResult]:
+) -> tuple[DataFrame, RectangleSignatureResult, ConsensusResult]:
     r"""All in one deconvolution method. Creates signatures and deconvolutes the bulk data. Has options for subsampling and consensus runs.
 
     Parameters
     ----------
     adata
         The single-cell count data as a DataFrame. DataFrame must have the genes as index and cell identifier as columns. Each entry should be in raw counts.
     bulks
@@ -35,34 +51,35 @@
     cell_type_col
         The annotations corresponding to the single-cell count data. Series data should have the cell identifier as index and the annotations as values.
     layer
         The Anndata layer to use for the single-cell data. Defaults to None.
     raw
         A flag indicating whether to use the raw Anndata data. Defaults to False.
     subsample : bool
-        A flag indicating whether to balance the single-cell data. Defaults to False.
+        A flag indicating whether to balance the single-cell data.
     sample_size : int
-        The number of cells to balance the single-cell data to. Defaults to 1500. If cell number is less than this number it takes the original number of cells.
+        The number of cells to balance the single-cell data to. If cell number is less than this number it takes the original number of cells.
     consensus_runs : int
-        The number of consensus runs to perform. Defaults to 1 for a singular deconvolution run. Consensus runs are performed by subsampling the single-cell data and running the analysis multiple times. The results are then aggregated.
+        The number of consensus runs to perform. Consensus runs are performed by subsampling the single-cell data and running the analysis multiple times. The results are then aggregated.
     optimize_cutoffs
-        Indicates whether to optimize the p-value and log fold change cutoffs using gridsearch. Defaults to True.
+        Indicates whether to optimize the p-value and log fold change cutoffs using gridsearch.
     p
         The p-value threshold for the DE analysis (only used if optimize_cutoffs is False).
     lfc
         The log fold change threshold for the DE analysis (only used if optimize_cutoffs is False).
     n_cpus
-        The number of cpus to use for the DE analysis. Defaults to the number of cpus available.
+        The number of cpus to use for the DE analysis. None value takes all cpus available.
     correct_mrna_bias : bool
         A flag indicating whether to correct for mRNA bias. Defaults to True.
 
     Returns
     -------
-    DataFrame : The estimated cell fractions.
-    RectangleSignatureResult : The result of the rectangle signature analysis.
+    DataFrame : The estimated cell fractions consens.
+    RectangleSignatureResult : The result of the last consensus run.
+    ConsensusResult : Estimations and rectangle signature results for each consensus run.
     """
     assert isinstance(adata, AnnData), "adata must be an AnnData object"
     assert isinstance(bulks, DataFrame), "bulks must be a DataFrame"
 
     if bulks is not None:
         genes = list(set(bulks.columns) & set(adata.var_names))
         genes = sorted(genes)
@@ -70,14 +87,15 @@
         bulks = bulks[genes]
 
     if consensus_runs > 1:
         logger.info(f"Running {consensus_runs} consensus runs with subsample size {sample_size}")
         subsample = True
 
     estimations = []
+    rectangle_signature_results = []
     most_recent_signatures = None
 
     for _i in range(consensus_runs):
         logger.info(f"Running consensus run {_i + 1} of {consensus_runs}")
         signatures = build_rectangle_signatures(
             adata,
             cell_type_col,
@@ -87,19 +105,82 @@
             raw=raw,
             p=p,
             lfc=lfc,
             n_cpus=n_cpus,
             subsample=subsample,
             sample_size=sample_size,
         )
+        rectangle_signature_results.append(signatures)
+        most_recent_signatures = signatures
         cell_fractions = deconvolution(signatures, bulks, correct_mrna_bias, n_cpus)
         estimations.append(cell_fractions)
-        most_recent_signatures = signatures
 
-    return pd.concat(estimations).groupby(level=0).median(), most_recent_signatures
+    consensus_results = ConsensusResult(estimations, rectangle_signature_results)
+    return pd.concat(estimations).groupby(level=0).median(), most_recent_signatures, consensus_results
+
+
+def rectangle(
+    adata: AnnData,
+    bulks: DataFrame,
+    cell_type_col: str = "cell_type",
+    *,
+    layer: str = None,
+    raw: bool = False,
+    correct_mrna_bias: bool = True,
+    optimize_cutoffs=True,
+    p=0.015,
+    lfc=1.5,
+    n_cpus: int = None,
+) -> tuple[DataFrame, RectangleSignatureResult]:
+    r"""All in one deconvolution method. Creates signatures and deconvolutes the bulk data. Has options for subsampling and consensus runs.
+
+    Parameters
+    ----------
+    adata
+        The single-cell count data as a DataFrame. DataFrame must have the genes as index and cell identifier as columns. Each entry should be in raw counts.
+    bulks
+        The bulk data as a DataFrame. DataFrame must have the bulk identifier as index and the genes as columns. Each entry should be in transcripts per million (TPM).
+    cell_type_col
+        The annotations corresponding to the single-cell count data. Series data should have the cell identifier as index and the annotations as values.
+    layer
+        The Anndata layer to use for the single-cell data.
+    raw
+        A flag indicating whether to use the raw Anndata data.
+    optimize_cutoffs
+        Indicates whether to optimize the p-value and log fold change cutoffs using gridsearch.
+    p
+        The p-value threshold for the DE analysis (only used if optimize_cutoffs is False).
+    lfc
+        The log fold change threshold for the DE analysis (only used if optimize_cutoffs is False).
+    n_cpus
+        The number of cpus to use for the DE analysis. None value takes all cpus available.
+    correct_mrna_bias : bool
+        A flag indicating whether to correct for mRNA bias. Defaults to True.
+
+    Returns
+    -------
+    DataFrame : The estimated cell fractions.
+    RectangleSignatureResult : The result of the rectangle signature analysis.
+    """
+    estimations, signatures, _ = rectangle_consens(
+        adata,
+        bulks,
+        cell_type_col,
+        layer=layer,
+        raw=raw,
+        subsample=False,
+        sample_size=-1,
+        consensus_runs=1,
+        correct_mrna_bias=correct_mrna_bias,
+        optimize_cutoffs=optimize_cutoffs,
+        p=p,
+        lfc=lfc,
+        n_cpus=n_cpus,
+    )
+    return estimations, signatures
 
 
 def load_tutorial_data() -> tuple[pd.DataFrame, pd.DataFrame, pd.DataFrame]:
     """Loads the single-cell count data, annotations, and bulk data from the tutorial.
 
     Returns
     -------
```

### Comparing `rectanglepy-0.1.3/src/rectanglepy/data/hao1_annotations_small.zip` & `rectanglepy-0.1.6/src/rectanglepy/data/hao1_annotations_small.zip`

 * *Files identical despite different names*

### Comparing `rectanglepy-0.1.3/src/rectanglepy/data/hao1_counts_small.zip` & `rectanglepy-0.1.6/src/rectanglepy/data/hao1_counts_small.zip`

 * *Files identical despite different names*

### Comparing `rectanglepy-0.1.3/src/rectanglepy/data/small_fino_bulks.zip` & `rectanglepy-0.1.6/src/rectanglepy/data/small_fino_bulks.zip`

 * *Files identical despite different names*

### Comparing `rectanglepy-0.1.3/src/rectanglepy/pp/create_signature.py` & `rectanglepy-0.1.6/src/rectanglepy/pp/create_signature.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,15 +151,15 @@
         results[cell_type] = stat_res.results_df
 
     return results
 
 
 def _de_analysis(
     pseudo_count_sig, sc_data, annotations, p, lfc, optimize_cutoffs: bool, n_cpus: int = None, genes=None
-) -> tuple[Series, dict[str, int] :, DataFrame | None]:
+) -> tuple[Series, dict[str, [str]] :, DataFrame | None]:
     logger.info("Starting DE analysis")
     deseq_results = _run_deseq2(pseudo_count_sig, n_cpus)
     optimization_results = None
 
     if optimize_cutoffs:
         logger.info("Optimizing cutoff parameters p and lfc")
         optimization_results = _optimize_parameters(sc_data, annotations, pseudo_count_sig, deseq_results, genes)
@@ -181,23 +181,23 @@
     optimal_condition_index = condition_numbers.index(min(condition_numbers))
 
     optimal_condition_number = optimal_condition_index + range_minimum
     logger.info(f"Optimal condition number: {optimal_condition_number}")
     optimal_condition_matrix = condition_number_matrices[optimal_condition_index]
 
     markers = optimal_condition_matrix.index
-    marker_genes_per_cell_type = _count_marker_genes_per_cell_type(de_analysis_adjusted, optimal_condition_number)
+    marker_genes_per_cell_type = _get_marker_genes_per_cell_type(de_analysis_adjusted, optimal_condition_number)
     return markers, marker_genes_per_cell_type
 
 
-def _count_marker_genes_per_cell_type(de_analysis_adjusted, optimal_condition_number: int) -> dict[str, int]:
+def _get_marker_genes_per_cell_type(de_analysis_adjusted, optimal_condition_number: int) -> dict[str, [str]]:
     marker_genes_per_cell_type = {}
     for annotation, result in de_analysis_adjusted.items():
-        marker_genes_per_cell_type[annotation] = min(len(result), optimal_condition_number)
-    logger.info(f"Number of marker genes per cell type: {str(marker_genes_per_cell_type)}")
+        number_of_genes = min(len(result), optimal_condition_number)
+        marker_genes_per_cell_type[annotation] = list(result.index[0:number_of_genes])
     return marker_genes_per_cell_type
 
 
 def _create_bias_factors(countsig: pd.DataFrame, sc_counts: pd.DataFrame | np.ndarray, annotations) -> pd.Series:
     number_of_expressed_genes = (sc_counts > 0).sum(axis=0)
     number_of_expressed_genes = np.squeeze(np.asarray(number_of_expressed_genes))
     bias_factors = [
@@ -319,26 +319,29 @@
             pseudobulk_sig_cpm=pseudo_sig_cpm,
             bias_factors=m_rna_biasfactors,
             marker_genes_per_cell_type=marker_genes_per_cell_type,
             optimization_result=optimization_result,
         )
 
     clustered_biasfact = _create_bias_factors(clustered_signature, sc_counts, clustered_annotations)
-    clustered_genes = _de_analysis(clustered_signature, sc_counts, clustered_annotations, p, lfc, False)[0]
+    clustered_genes, clustered_marker_genes_per_cell_type, _ = _de_analysis(
+        clustered_signature, sc_counts, clustered_annotations, p, lfc, False
+    )
     clustered_signature = _convert_to_cpm(clustered_signature)
     return RectangleSignatureResult(
         signature_genes=marker_genes,
         pseudobulk_sig_cpm=pseudo_sig_cpm,
         bias_factors=m_rna_biasfactors,
         marker_genes_per_cell_type=marker_genes_per_cell_type,
         optimization_result=optimization_result,
         clustered_pseudobulk_sig_cpm=clustered_signature,
         clustered_signature_genes=clustered_genes,
         clustered_bias_factors=clustered_biasfact,
         cluster_assignments=assignments,
+        marker_genes_per_cluster=clustered_marker_genes_per_cell_type,
     )
 
 
 def _create_pseudo_count_sig(sc_counts: np.ndarray, annotations: pd.Series, var_names) -> pd.DataFrame:
     unique_labels, label_indices = np.unique(annotations, return_inverse=True)
     grouped_sum = np.zeros((len(unique_labels), sc_counts.shape[0]))
     for i, _label in enumerate(unique_labels):
```

### Comparing `rectanglepy-0.1.3/src/rectanglepy/pp/rectangle_signature.py` & `rectanglepy-0.1.6/src/rectanglepy/pp/rectangle_signature.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,46 +25,33 @@
     """
 
     def __init__(
         self,
         signature_genes: pd.Series,
         bias_factors: pd.Series,
         pseudobulk_sig_cpm: pd.DataFrame,
-        marker_genes_per_cell_type: dict[str, int],
+        marker_genes_per_cell_type: dict[str, [str]],
         optimization_result: pd.DataFrame = None,
         clustered_pseudobulk_sig_cpm: pd.DataFrame = None,
         clustered_bias_factors: pd.Series = None,
+        marker_genes_per_cluster: dict[str, [str]] = None,
         clustered_signature_genes: pd.Series = None,
         cluster_assignments: list[int or str] = None,
     ):
         self.signature_genes = signature_genes
         self.bias_factors = bias_factors
         self.pseudobulk_sig_cpm = pseudobulk_sig_cpm
+        self.marker_genes_per_cluster = marker_genes_per_cluster
         self.marker_genes_per_cell_type = marker_genes_per_cell_type
         self.optimization_result = optimization_result
         self.clustered_pseudobulk_sig_cpm = clustered_pseudobulk_sig_cpm
         self.clustered_bias_factors = clustered_bias_factors
         self.clustered_signature_genes = clustered_signature_genes
         self.assignments = cluster_assignments
 
-    def cell_types_with_low_number_of_marker_genes(self) -> list[str]:
-        """Returns the cell types with less than threshold marker genes.
-
-        Returns
-        -------
-        list[str]: The cell types with less than threshold marker genes.
-
-        """
-        low_annotation_threshold = 30
-        return [
-            cell_type
-            for cell_type, count in self.marker_genes_per_cell_type.items()
-            if count < low_annotation_threshold
-        ]
-
     def get_signature_matrix(self, include_mrna_bias=True) -> pd.DataFrame:
         """Calculates the signature matrix by multiplying the pseudobulk_sig_cpm DataFrame subset by signature_genes and the bias_factors Series.
 
         Parameters
         ----------
         include_mrna_bias
             If True, the method includes mRNA bias in the calculation. Defaults to True.
```

### Comparing `rectanglepy-0.1.3/src/rectanglepy/tl/deconvolution.py` & `rectanglepy-0.1.6/src/rectanglepy/tl/deconvolution.py`

 * *Files 2% similar despite different names*

```diff
@@ -253,15 +253,22 @@
         return start_fractions
 
     union_direct_fraction = _calculate_dwls(union_direct_signature, bulk)
 
     averaged_start_fractions = (start_fractions + union_direct_fraction) / 2
 
     final_fractions = []
-    cell_types_with_low_number_of_marker_genes = signatures.cell_types_with_low_number_of_marker_genes()
+
+    low_number_threshold = 30
+    cell_types_with_low_number_of_marker_genes = [
+        cell_type
+        for cell_type, num_marker_genes in signatures.marker_genes_per_cell_type.items()
+        if len(num_marker_genes) < low_number_threshold
+    ]
+
     for cell_type in list(averaged_start_fractions.index):
         if cell_type in cell_types_with_low_number_of_marker_genes:
             final_fractions.append(recursive_fractions[cell_type])
         else:
             final_fractions.append(averaged_start_fractions[cell_type])
 
     final_fractions = pd.Series(final_fractions, index=averaged_start_fractions.index)
```

### Comparing `rectanglepy-0.1.3/tests/test_pp.py` & `rectanglepy-0.1.6/tests/test_pp.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,15 +142,15 @@
 
 def test_build_rectangle_signatures(small_data):
     sc_counts, annotations, bulk = small_data
     sc_counts = sc_counts.astype("int")
     adata = AnnData(sc_counts.T, obs=annotations.to_frame(name="cell_type"))
     results = build_rectangle_signatures(adata, "cell_type", bulks=bulk.T, p=0.5, lfc=0.1, optimize_cutoffs=False)
     assert results.assignments is None  # not enough cells to cluster
-    assert 10 < len(results.signature_genes) < 100
+    assert 10 < len(results.signature_genes) < 400
 
 
 def test_generate_pseudo_bulks(small_data):
     sc_counts, annotations, bulk = small_data
     sc_counts = sc_counts.astype("int")
     adata = AnnData(sc_counts.T, obs=annotations.to_frame(name="cell_type"))
     result, _ = _generate_pseudo_bulks(adata.X.T, annotations, adata.var_names)
```

### Comparing `rectanglepy-0.1.3/tests/test_rectangle.py` & `rectanglepy-0.1.6/tests/test_rectangle.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import pandas as pd
 from anndata import AnnData
 
 import rectanglepy.rectangle
+from rectanglepy import ConsensusResult
 from rectanglepy.pp import RectangleSignatureResult
 
 
 def test_load_tutorial_data():
     sc_data, annotations, bulks = rectanglepy.load_tutorial_data()
     assert isinstance(sc_data, pd.DataFrame)
     assert isinstance(annotations, pd.Series)
@@ -22,13 +23,14 @@
     assert isinstance(result[1], RectangleSignatureResult)
 
 
 def test_rectangle_consensus():
     sc_data, annotations, bulks = rectanglepy.load_tutorial_data()
     sc_data_adata = AnnData(sc_data, obs=annotations.to_frame(name="cell_type"))
 
-    result = rectanglepy.rectangle(
+    result = rectanglepy.rectangle_consens(
         sc_data_adata, bulks, optimize_cutoffs=False, p=0.5, lfc=0.0, consensus_runs=2, sample_size=50
     )
 
     assert isinstance(result[0], pd.DataFrame)
     assert isinstance(result[1], RectangleSignatureResult)
+    assert isinstance(result[2], ConsensusResult)
```

### Comparing `rectanglepy-0.1.3/tests/test_tl.py` & `rectanglepy-0.1.6/tests/test_tl.py`

 * *Files identical despite different names*

### Comparing `rectanglepy-0.1.3/tests/data/TIL10_signature.txt` & `rectanglepy-0.1.6/tests/data/TIL10_signature.txt`

 * *Files identical despite different names*

### Comparing `rectanglepy-0.1.3/tests/data/bulk_small.csv` & `rectanglepy-0.1.6/tests/data/bulk_small.csv`

 * *Files identical despite different names*

### Comparing `rectanglepy-0.1.3/tests/data/quanTIseq_SimRNAseq_mixture_smaller.csv` & `rectanglepy-0.1.6/tests/data/quanTIseq_SimRNAseq_mixture_smaller.csv`

 * *Files identical despite different names*

### Comparing `rectanglepy-0.1.3/tests/data/quanTIseq_SimRNAseq_read_fractions_small.txt` & `rectanglepy-0.1.6/tests/data/quanTIseq_SimRNAseq_read_fractions_small.txt`

 * *Files identical despite different names*

### Comparing `rectanglepy-0.1.3/tests/data/sc_object_small.csv` & `rectanglepy-0.1.6/tests/data/sc_object_small.csv`

 * *Files identical despite different names*

### Comparing `rectanglepy-0.1.3/tests/data/signature_hao1.csv` & `rectanglepy-0.1.6/tests/data/signature_hao1.csv`

 * *Files identical despite different names*

### Comparing `rectanglepy-0.1.3/LICENSE` & `rectanglepy-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `rectanglepy-0.1.3/README.md` & `rectanglepy-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `rectanglepy-0.1.3/pyproject.toml` & `rectanglepy-0.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "hatchling.build"
 requires = ["hatchling"]
 
 [project]
 name = "rectanglepy"
-version = "0.1.3"
+version = "0.1.6"
 description = "Hierarchical deconvolution of bulk  transcriptomics"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {file = "LICENSE"}
 authors = [
     {name = "Bernhard Eder"},
 ]
```

### Comparing `rectanglepy-0.1.3/PKG-INFO` & `rectanglepy-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: rectanglepy
-Version: 0.1.3
+Version: 0.1.6
 Summary: Hierarchical deconvolution of bulk  transcriptomics
 Project-URL: Documentation, https://rectanglepy.readthedocs.io/
 Project-URL: Source, https://github.com/ComputationalBiomedicineGroup/Rectangle
 Project-URL: Home-page, https://github.com/ComputationalBiomedicineGroup/Rectangle
 Author: Bernhard Eder
 Maintainer-email: Bernhard Eder <Bernhard.Eder@student.uibk.ac.at>
 License: MIT License
```

