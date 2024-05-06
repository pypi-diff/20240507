# Comparing `tmp/mimllearning-0.2.82.tar.gz` & `tmp/mimllearning-0.3.1.tar.gz`

## Comparing `mimllearning-0.2.82.tar` & `mimllearning-0.3.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 mimllearning-0.2.82/readme.md
--rw-r--r--   0        0        0   258069 2020-02-02 00:00:00.000000 mimllearning-0.2.82/documentation/AnteproyectoDamianTFG.pdf
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 mimllearning-0.2.82/src/miml/__init__.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 mimllearning-0.2.82/src/miml/classifier/__init__.py
--rw-r--r--   0        0        0     2841 2020-02-02 00:00:00.000000 mimllearning-0.2.82/src/miml/classifier/miml_classifier.py
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 mimllearning-0.2.82/src/miml/classifier/mi/__init__.py
--rw-r--r--   0        0        0     2984 2020-02-02 00:00:00.000000 mimllearning-0.2.82/src/miml/classifier/mi/all_positive_apr_classifier.py
--rw-r--r--   0        0        0     2389 2020-02-02 00:00:00.000000 mimllearning-0.2.82/src/miml/classifier/mi/apr_classifier.py
--rw-r--r--   0        0        0     2499 2020-02-02 00:00:00.000000 mimllearning-0.2.82/src/miml/classifier/mi/miles_classifier.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 mimllearning-0.2.82/src/miml/classifier/mimlTOmi/__init__.py
--rw-r--r--   0        0        0     3646 2020-02-02 00:00:00.000000 mimllearning-0.2.82/src/miml/classifier/mimlTOmi/miml_to_mi_br_classifier.py
--rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 mimllearning-0.2.82/src/miml/classifier/mimlTOmi/miml_to_mi_classifier.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 mimllearning-0.2.82/src/miml/classifier/mimlTOml/__init__.py
--rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 mimllearning-0.2.82/src/miml/classifier/mimlTOml/miml_to_ml_classifier.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 mimllearning-0.2.82/src/miml/data/__init__.py
--rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 mimllearning-0.2.82/src/miml/data/arff_to_csv.py
--rw-r--r--   0        0        0     8990 2020-02-02 00:00:00.000000 mimllearning-0.2.82/src/miml/data/bag.py
--rw-r--r--   0        0        0     6840 2020-02-02 00:00:00.000000 mimllearning-0.2.82/src/miml/data/instance.py
--rw-r--r--   0        0        0     4591 2020-02-02 00:00:00.000000 mimllearning-0.2.82/src/miml/data/load_datasets.py
--rw-r--r--   0        0        0    15553 2020-02-02 00:00:00.000000 mimllearning-0.2.82/src/miml/data/miml_dataset.py
--rw-r--r--   0        0        0   735908 2020-02-02 00:00:00.000000 mimllearning-0.2.82/src/miml/datasets/miml_birds.arff
--rw-r--r--   0        0        0   842801 2020-02-02 00:00:00.000000 mimllearning-0.2.82/src/miml/datasets/miml_birds.csv
--rw-r--r--   0        0        0   134841 2020-02-02 00:00:00.000000 mimllearning-0.2.82/src/miml/datasets/miml_birds_random_20test.arff
--rw-r--r--   0        0        0   498562 2020-02-02 00:00:00.000000 mimllearning-0.2.82/src/miml/datasets/miml_birds_random_80train.arff
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 mimllearning-0.2.82/src/miml/datasets/toy.arff
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 mimllearning-0.2.82/src/miml/datasets/toy.csv
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 mimllearning-0.2.82/src/miml/report/__init__.py
--rw-r--r--   0        0        0     6770 2020-02-02 00:00:00.000000 mimllearning-0.2.82/src/miml/report/report.py
--rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 mimllearning-0.2.82/src/miml/test/data_test.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 mimllearning-0.2.82/src/miml/transformation/__init__.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 mimllearning-0.2.82/src/miml/transformation/mimlTOmi/__init__.py
--rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 mimllearning-0.2.82/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 mimllearning-0.2.82/src/miml/transformation/mimlTOml/__init__.py
--rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 mimllearning-0.2.82/src/miml/transformation/mimlTOml/arithmetic.py
--rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 mimllearning-0.2.82/src/miml/transformation/mimlTOml/geometric.py
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 mimllearning-0.2.82/src/miml/transformation/mimlTOml/miml_to_ml_transformation.py
--rw-r--r--   0        0        0     2826 2020-02-02 00:00:00.000000 mimllearning-0.2.82/src/miml/transformation/mimlTOml/minmax.py
--rw-r--r--   0        0        0     9910 2020-02-02 00:00:00.000000 mimllearning-0.2.82/src/miml/tutorial/demo.ipynb
--rw-r--r--   0        0        0    13016 2020-02-02 00:00:00.000000 mimllearning-0.2.82/src/miml/tutorial/miml_transformations.ipynb
--rw-r--r--   0        0        0    11077 2020-02-02 00:00:00.000000 mimllearning-0.2.82/src/miml/tutorial/mimltoml_classifiers.ipynb
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 mimllearning-0.2.82/.gitignore
--rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 mimllearning-0.2.82/README.md
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 mimllearning-0.2.82/pyproject.toml
--rw-r--r--   0        0        0     2387 2020-02-02 00:00:00.000000 mimllearning-0.2.82/PKG-INFO
+-rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 mimllearning-0.3.1/readme.md
+-rw-r--r--   0        0        0   258069 2020-02-02 00:00:00.000000 mimllearning-0.3.1/documentation/AnteproyectoDamianTFG.pdf
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 mimllearning-0.3.1/src/miml/__init__.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 mimllearning-0.3.1/src/miml/classifier/__init__.py
+-rw-r--r--   0        0        0     2841 2020-02-02 00:00:00.000000 mimllearning-0.3.1/src/miml/classifier/miml_classifier.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 mimllearning-0.3.1/src/miml/classifier/mi/__init__.py
+-rw-r--r--   0        0        0     2984 2020-02-02 00:00:00.000000 mimllearning-0.3.1/src/miml/classifier/mi/all_positive_apr_classifier.py
+-rw-r--r--   0        0        0     2389 2020-02-02 00:00:00.000000 mimllearning-0.3.1/src/miml/classifier/mi/apr_classifier.py
+-rw-r--r--   0        0        0     2499 2020-02-02 00:00:00.000000 mimllearning-0.3.1/src/miml/classifier/mi/miles_classifier.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 mimllearning-0.3.1/src/miml/classifier/mimlTOmi/__init__.py
+-rw-r--r--   0        0        0     3646 2020-02-02 00:00:00.000000 mimllearning-0.3.1/src/miml/classifier/mimlTOmi/miml_to_mi_br_classifier.py
+-rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 mimllearning-0.3.1/src/miml/classifier/mimlTOmi/miml_to_mi_classifier.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 mimllearning-0.3.1/src/miml/classifier/mimlTOml/__init__.py
+-rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 mimllearning-0.3.1/src/miml/classifier/mimlTOml/miml_to_ml_classifier.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 mimllearning-0.3.1/src/miml/data/__init__.py
+-rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 mimllearning-0.3.1/src/miml/data/arff_to_csv.py
+-rw-r--r--   0        0        0     8990 2020-02-02 00:00:00.000000 mimllearning-0.3.1/src/miml/data/bag.py
+-rw-r--r--   0        0        0     6840 2020-02-02 00:00:00.000000 mimllearning-0.3.1/src/miml/data/instance.py
+-rw-r--r--   0        0        0     4591 2020-02-02 00:00:00.000000 mimllearning-0.3.1/src/miml/data/load_datasets.py
+-rw-r--r--   0        0        0    15553 2020-02-02 00:00:00.000000 mimllearning-0.3.1/src/miml/data/miml_dataset.py
+-rw-r--r--   0        0        0   735908 2020-02-02 00:00:00.000000 mimllearning-0.3.1/src/miml/datasets/miml_birds.arff
+-rw-r--r--   0        0        0   842801 2020-02-02 00:00:00.000000 mimllearning-0.3.1/src/miml/datasets/miml_birds.csv
+-rw-r--r--   0        0        0   134841 2020-02-02 00:00:00.000000 mimllearning-0.3.1/src/miml/datasets/miml_birds_random_20test.arff
+-rw-r--r--   0        0        0   498562 2020-02-02 00:00:00.000000 mimllearning-0.3.1/src/miml/datasets/miml_birds_random_80train.arff
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 mimllearning-0.3.1/src/miml/datasets/toy.arff
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 mimllearning-0.3.1/src/miml/datasets/toy.csv
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 mimllearning-0.3.1/src/miml/report/__init__.py
+-rw-r--r--   0        0        0     7092 2020-02-02 00:00:00.000000 mimllearning-0.3.1/src/miml/report/report.py
+-rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 mimllearning-0.3.1/src/miml/test/data_test.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 mimllearning-0.3.1/src/miml/transformation/__init__.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 mimllearning-0.3.1/src/miml/transformation/mimlTOmi/__init__.py
+-rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 mimllearning-0.3.1/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 mimllearning-0.3.1/src/miml/transformation/mimlTOml/__init__.py
+-rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 mimllearning-0.3.1/src/miml/transformation/mimlTOml/arithmetic.py
+-rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 mimllearning-0.3.1/src/miml/transformation/mimlTOml/geometric.py
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 mimllearning-0.3.1/src/miml/transformation/mimlTOml/miml_to_ml_transformation.py
+-rw-r--r--   0        0        0     2826 2020-02-02 00:00:00.000000 mimllearning-0.3.1/src/miml/transformation/mimlTOml/minmax.py
+-rw-r--r--   0        0        0     9910 2020-02-02 00:00:00.000000 mimllearning-0.3.1/src/miml/tutorial/demo.ipynb
+-rw-r--r--   0        0        0    13016 2020-02-02 00:00:00.000000 mimllearning-0.3.1/src/miml/tutorial/miml_transformations.ipynb
+-rw-r--r--   0        0        0    11077 2020-02-02 00:00:00.000000 mimllearning-0.3.1/src/miml/tutorial/mimltoml_classifiers.ipynb
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 mimllearning-0.3.1/.gitignore
+-rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 mimllearning-0.3.1/README.md
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 mimllearning-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2386 2020-02-02 00:00:00.000000 mimllearning-0.3.1/PKG-INFO
```

### Comparing `mimllearning-0.2.82/readme.md` & `mimllearning-0.3.1/readme.md`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.82/documentation/AnteproyectoDamianTFG.pdf` & `mimllearning-0.3.1/documentation/AnteproyectoDamianTFG.pdf`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.82/src/miml/classifier/miml_classifier.py` & `mimllearning-0.3.1/src/miml/classifier/miml_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.82/src/miml/classifier/mi/all_positive_apr_classifier.py` & `mimllearning-0.3.1/src/miml/classifier/mi/all_positive_apr_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.82/src/miml/classifier/mi/apr_classifier.py` & `mimllearning-0.3.1/src/miml/classifier/mi/apr_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.82/src/miml/classifier/mi/miles_classifier.py` & `mimllearning-0.3.1/src/miml/classifier/mi/miles_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.82/src/miml/classifier/mimlTOmi/miml_to_mi_br_classifier.py` & `mimllearning-0.3.1/src/miml/classifier/mimlTOmi/miml_to_mi_br_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.82/src/miml/classifier/mimlTOmi/miml_to_mi_classifier.py` & `mimllearning-0.3.1/src/miml/classifier/mimlTOmi/miml_to_mi_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.82/src/miml/classifier/mimlTOml/miml_to_ml_classifier.py` & `mimllearning-0.3.1/src/miml/classifier/mimlTOml/miml_to_ml_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.82/src/miml/data/arff_to_csv.py` & `mimllearning-0.3.1/src/miml/data/arff_to_csv.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.82/src/miml/data/bag.py` & `mimllearning-0.3.1/src/miml/data/bag.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.82/src/miml/data/instance.py` & `mimllearning-0.3.1/src/miml/data/instance.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.82/src/miml/data/load_datasets.py` & `mimllearning-0.3.1/src/miml/data/load_datasets.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.82/src/miml/data/miml_dataset.py` & `mimllearning-0.3.1/src/miml/data/miml_dataset.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.82/src/miml/datasets/miml_birds.arff` & `mimllearning-0.3.1/src/miml/datasets/miml_birds.arff`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.82/src/miml/datasets/miml_birds.csv` & `mimllearning-0.3.1/src/miml/datasets/miml_birds.csv`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.82/src/miml/datasets/miml_birds_random_20test.arff` & `mimllearning-0.3.1/src/miml/datasets/miml_birds_random_20test.arff`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.82/src/miml/datasets/miml_birds_random_80train.arff` & `mimllearning-0.3.1/src/miml/datasets/miml_birds_random_80train.arff`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.82/src/miml/report/report.py` & `mimllearning-0.3.1/src/miml/report/report.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import warnings
 from sklearn.metrics import hamming_loss, accuracy_score, fbeta_score, jaccard_score, log_loss, \
     roc_auc_score, f1_score, precision_score, recall_score, average_precision_score
 from ..classifier import MIMLClassifier
 from ..data import MIMLDataset
 
 
 class Report:
@@ -37,52 +38,57 @@
         self.metrics_value = dict()
 
     def calculate_metrics(self):
         self.metrics_value["precision-score-macro"] = precision_score(self.y_true, self.y_pred, average="macro",
                                                                       zero_division=0)
         self.metrics_value["precision-score-micro"] = precision_score(self.y_true, self.y_pred, average="micro",
                                                                       zero_division=0)
-        # TODO: UserWarning: No positive class found in y_true, recall is set to one for all thresholds.
-        self.metrics_value["average-precision-score-macro"] = average_precision_score(self.y_true, self.probs,
-                                                                                      average="macro")
-        # TODO: UserWarning: No positive class found in y_true, recall is set to one for all thresholds.
-        self.metrics_value["average-precision-score-micro"] = average_precision_score(self.y_true, self.probs,
-                                                                                      average="micro")
+        with warnings.catch_warnings():
+            warnings.filterwarnings("ignore", category=UserWarning)
+            # When average_precision_score called raise this warming:
+            # UserWarning: No positive class found in y_true, recall is set to one for all thresholds.
+            self.metrics_value["average-precision-score-macro"] = average_precision_score(self.y_true, self.probs,
+                                                                                          average="macro")
+            self.metrics_value["average-precision-score-micro"] = average_precision_score(self.y_true, self.probs,
+                                                                                          average="micro")
         self.metrics_value["recall-score-macro"] = recall_score(self.y_true, self.y_pred, average="macro",
                                                                 zero_division=0)
         self.metrics_value["recall-score-micro"] = recall_score(self.y_true, self.y_pred, average="micro",
                                                                 zero_division=0)
         self.metrics_value["f1-score-macro"] = f1_score(self.y_true, self.y_pred, average="macro", zero_division=0)
         self.metrics_value["f1-score-micro"] = f1_score(self.y_true, self.y_pred, average="micro", zero_division=0)
         self.metrics_value["fbeta-score-macro"] = fbeta_score(self.y_true, self.y_pred, beta=1, average="macro",
                                                               zero_division=0)
         self.metrics_value["fbeta-score-micro"] = fbeta_score(self.y_true, self.y_pred, beta=1, average="micro",
                                                               zero_division=0)
         # TODO: ValueError: Only one class present in y_true. ROC AUC score is not defined in that case.
-        #self.metrics_value["roc-auc-score-macro"] = roc_auc_score(self.y_true, self.probs, average="macro")
-        #self.metrics_value["roc-auc-score-micro"] = roc_auc_score(self.y_true, self.probs, average="micro")
+        # self.metrics_value["roc-auc-score-macro"] = roc_auc_score(self.y_true, self.probs, average="macro")
+        # self.metrics_value["roc-auc-score-micro"] = roc_auc_score(self.y_true, self.probs, average="micro")
         self.metrics_value["accuracy-score"] = accuracy_score(self.y_true, self.y_pred)
         self.metrics_value["hamming-loss"] = hamming_loss(self.y_true, self.y_pred)
         self.metrics_value["jaccard-score-macro"] = jaccard_score(self.y_true, self.y_pred, average="macro",
                                                                   zero_division=0)
         self.metrics_value["jaccard-score-micro"] = jaccard_score(self.y_true, self.y_pred, average="micro",
                                                                   zero_division=0)
-        # TODO: UserWarning: The y_pred values do not sum to one. Starting from 1.5 thiswill result in an error.
-        self.metrics_value["log-loss"] = log_loss(self.y_true, self.probs)
+        with warnings.catch_warnings():
+            warnings.filterwarnings("ignore", category=UserWarning)
+            # When log_loss called raise this warning, it is not true for multilabel classification
+            # UserWarning: The y_pred values do not sum to one. Starting from 1.5 thiswill result in an error.
+            self.metrics_value["log-loss"] = log_loss(self.y_true, self.probs)
 
         if self.per_label:
             self.metrics_value["precision-score-per-label"] = list(precision_score(self.y_true, self.y_pred,
                                                                                    average=None, zero_division=0))
             self.metrics_value["recall-score-per-label"] = list(recall_score(self.y_true, self.y_pred, average=None,
                                                                              zero_division=0))
             self.metrics_value["f1-score-per-label"] = list(f1_score(self.y_true, self.y_pred, average=None,
                                                                      zero_division=0))
             self.metrics_value["fbeta-score-per-label"] = list(fbeta_score(self.y_true, self.y_pred, beta=1,
                                                                            average=None, zero_division=0))
-            #self.metrics_value["roc-auc-score-per-label"] = roc_auc_score(self.y_true, self.probs, average="None")
+            # self.metrics_value["roc-auc-score-per-label"] = roc_auc_score(self.y_true, self.probs, average="None")
             self.metrics_value["jaccard-score-per-label"] = list(jaccard_score(self.y_true, self.y_pred, average=None,
                                                                                zero_division=0))
 
     def to_csv(self, path=None):
         self.calculate_metrics()
         header = ""
         if self.header:
```

### Comparing `mimllearning-0.2.82/src/miml/test/data_test.py` & `mimllearning-0.3.1/src/miml/test/data_test.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.82/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py` & `mimllearning-0.3.1/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.82/src/miml/transformation/mimlTOml/arithmetic.py` & `mimllearning-0.3.1/src/miml/transformation/mimlTOml/arithmetic.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.82/src/miml/transformation/mimlTOml/geometric.py` & `mimllearning-0.3.1/src/miml/transformation/mimlTOml/geometric.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.82/src/miml/transformation/mimlTOml/minmax.py` & `mimllearning-0.3.1/src/miml/transformation/mimlTOml/minmax.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.82/src/miml/tutorial/demo.ipynb` & `mimllearning-0.3.1/src/miml/tutorial/demo.ipynb`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.82/src/miml/tutorial/miml_transformations.ipynb` & `mimllearning-0.3.1/src/miml/tutorial/miml_transformations.ipynb`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.82/src/miml/tutorial/mimltoml_classifiers.ipynb` & `mimllearning-0.3.1/src/miml/tutorial/mimltoml_classifiers.ipynb`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.82/README.md` & `mimllearning-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `mimllearning-0.2.82/pyproject.toml` & `mimllearning-0.3.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 requires = ["hatchling", "pkginfo >= 1.10"]
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/miml", "src/miml/*"]
 
 [metadata]
-version = "0.2.82"
+version = "0.3.1"
 name = "mimllearning"
 
 [project]
 name = "mimllearning"
-version = "0.2.82"
+version = "0.3.1"
 authors = [
   { name="Damian Martinez", email="damianmartinezavila@gmail.com" },
 ]
 description = "MIML Learning Library"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `mimllearning-0.2.82/PKG-INFO` & `mimllearning-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: mimllearning
-Version: 0.2.82
+Version: 0.3.1
 Summary: MIML Learning Library
 Project-URL: Homepage, https://github.com/p82maavd/miml
 Author-email: Damian Martinez <damianmartinezavila@gmail.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

