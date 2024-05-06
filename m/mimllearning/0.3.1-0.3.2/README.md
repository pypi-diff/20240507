# Comparing `tmp/mimllearning-0.3.1.tar.gz` & `tmp/mimllearning-0.3.2.tar.gz`

## Comparing `mimllearning-0.3.1.tar` & `mimllearning-0.3.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 mimllearning-0.3.1/readme.md
--rw-r--r--   0        0        0   258069 2020-02-02 00:00:00.000000 mimllearning-0.3.1/documentation/AnteproyectoDamianTFG.pdf
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 mimllearning-0.3.1/src/miml/__init__.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 mimllearning-0.3.1/src/miml/classifier/__init__.py
--rw-r--r--   0        0        0     2841 2020-02-02 00:00:00.000000 mimllearning-0.3.1/src/miml/classifier/miml_classifier.py
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 mimllearning-0.3.1/src/miml/classifier/mi/__init__.py
--rw-r--r--   0        0        0     2984 2020-02-02 00:00:00.000000 mimllearning-0.3.1/src/miml/classifier/mi/all_positive_apr_classifier.py
--rw-r--r--   0        0        0     2389 2020-02-02 00:00:00.000000 mimllearning-0.3.1/src/miml/classifier/mi/apr_classifier.py
--rw-r--r--   0        0        0     2499 2020-02-02 00:00:00.000000 mimllearning-0.3.1/src/miml/classifier/mi/miles_classifier.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 mimllearning-0.3.1/src/miml/classifier/mimlTOmi/__init__.py
--rw-r--r--   0        0        0     3646 2020-02-02 00:00:00.000000 mimllearning-0.3.1/src/miml/classifier/mimlTOmi/miml_to_mi_br_classifier.py
--rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 mimllearning-0.3.1/src/miml/classifier/mimlTOmi/miml_to_mi_classifier.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 mimllearning-0.3.1/src/miml/classifier/mimlTOml/__init__.py
--rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 mimllearning-0.3.1/src/miml/classifier/mimlTOml/miml_to_ml_classifier.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 mimllearning-0.3.1/src/miml/data/__init__.py
--rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 mimllearning-0.3.1/src/miml/data/arff_to_csv.py
--rw-r--r--   0        0        0     8990 2020-02-02 00:00:00.000000 mimllearning-0.3.1/src/miml/data/bag.py
--rw-r--r--   0        0        0     6840 2020-02-02 00:00:00.000000 mimllearning-0.3.1/src/miml/data/instance.py
--rw-r--r--   0        0        0     4591 2020-02-02 00:00:00.000000 mimllearning-0.3.1/src/miml/data/load_datasets.py
--rw-r--r--   0        0        0    15553 2020-02-02 00:00:00.000000 mimllearning-0.3.1/src/miml/data/miml_dataset.py
--rw-r--r--   0        0        0   735908 2020-02-02 00:00:00.000000 mimllearning-0.3.1/src/miml/datasets/miml_birds.arff
--rw-r--r--   0        0        0   842801 2020-02-02 00:00:00.000000 mimllearning-0.3.1/src/miml/datasets/miml_birds.csv
--rw-r--r--   0        0        0   134841 2020-02-02 00:00:00.000000 mimllearning-0.3.1/src/miml/datasets/miml_birds_random_20test.arff
--rw-r--r--   0        0        0   498562 2020-02-02 00:00:00.000000 mimllearning-0.3.1/src/miml/datasets/miml_birds_random_80train.arff
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 mimllearning-0.3.1/src/miml/datasets/toy.arff
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 mimllearning-0.3.1/src/miml/datasets/toy.csv
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 mimllearning-0.3.1/src/miml/report/__init__.py
--rw-r--r--   0        0        0     7092 2020-02-02 00:00:00.000000 mimllearning-0.3.1/src/miml/report/report.py
--rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 mimllearning-0.3.1/src/miml/test/data_test.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 mimllearning-0.3.1/src/miml/transformation/__init__.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 mimllearning-0.3.1/src/miml/transformation/mimlTOmi/__init__.py
--rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 mimllearning-0.3.1/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 mimllearning-0.3.1/src/miml/transformation/mimlTOml/__init__.py
--rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 mimllearning-0.3.1/src/miml/transformation/mimlTOml/arithmetic.py
--rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 mimllearning-0.3.1/src/miml/transformation/mimlTOml/geometric.py
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 mimllearning-0.3.1/src/miml/transformation/mimlTOml/miml_to_ml_transformation.py
--rw-r--r--   0        0        0     2826 2020-02-02 00:00:00.000000 mimllearning-0.3.1/src/miml/transformation/mimlTOml/minmax.py
--rw-r--r--   0        0        0     9910 2020-02-02 00:00:00.000000 mimllearning-0.3.1/src/miml/tutorial/demo.ipynb
--rw-r--r--   0        0        0    13016 2020-02-02 00:00:00.000000 mimllearning-0.3.1/src/miml/tutorial/miml_transformations.ipynb
--rw-r--r--   0        0        0    11077 2020-02-02 00:00:00.000000 mimllearning-0.3.1/src/miml/tutorial/mimltoml_classifiers.ipynb
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 mimllearning-0.3.1/.gitignore
--rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 mimllearning-0.3.1/README.md
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 mimllearning-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     2386 2020-02-02 00:00:00.000000 mimllearning-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 mimllearning-0.3.2/readme.md
+-rw-r--r--   0        0        0   258069 2020-02-02 00:00:00.000000 mimllearning-0.3.2/documentation/AnteproyectoDamianTFG.pdf
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 mimllearning-0.3.2/src/miml/__init__.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 mimllearning-0.3.2/src/miml/classifier/__init__.py
+-rw-r--r--   0        0        0     2841 2020-02-02 00:00:00.000000 mimllearning-0.3.2/src/miml/classifier/miml_classifier.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 mimllearning-0.3.2/src/miml/classifier/mi/__init__.py
+-rw-r--r--   0        0        0     2984 2020-02-02 00:00:00.000000 mimllearning-0.3.2/src/miml/classifier/mi/all_positive_apr_classifier.py
+-rw-r--r--   0        0        0     2389 2020-02-02 00:00:00.000000 mimllearning-0.3.2/src/miml/classifier/mi/apr_classifier.py
+-rw-r--r--   0        0        0     2499 2020-02-02 00:00:00.000000 mimllearning-0.3.2/src/miml/classifier/mi/miles_classifier.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 mimllearning-0.3.2/src/miml/classifier/mimlTOmi/__init__.py
+-rw-r--r--   0        0        0     3646 2020-02-02 00:00:00.000000 mimllearning-0.3.2/src/miml/classifier/mimlTOmi/miml_to_mi_br_classifier.py
+-rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 mimllearning-0.3.2/src/miml/classifier/mimlTOmi/miml_to_mi_classifier.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 mimllearning-0.3.2/src/miml/classifier/mimlTOml/__init__.py
+-rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 mimllearning-0.3.2/src/miml/classifier/mimlTOml/miml_to_ml_classifier.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 mimllearning-0.3.2/src/miml/data/__init__.py
+-rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 mimllearning-0.3.2/src/miml/data/arff_to_csv.py
+-rw-r--r--   0        0        0     8990 2020-02-02 00:00:00.000000 mimllearning-0.3.2/src/miml/data/bag.py
+-rw-r--r--   0        0        0     6840 2020-02-02 00:00:00.000000 mimllearning-0.3.2/src/miml/data/instance.py
+-rw-r--r--   0        0        0     5145 2020-02-02 00:00:00.000000 mimllearning-0.3.2/src/miml/data/load_datasets.py
+-rw-r--r--   0        0        0    15737 2020-02-02 00:00:00.000000 mimllearning-0.3.2/src/miml/data/miml_dataset.py
+-rw-r--r--   0        0        0   735908 2020-02-02 00:00:00.000000 mimllearning-0.3.2/src/miml/datasets/miml_birds.arff
+-rw-r--r--   0        0        0   842801 2020-02-02 00:00:00.000000 mimllearning-0.3.2/src/miml/datasets/miml_birds.csv
+-rw-r--r--   0        0        0   134841 2020-02-02 00:00:00.000000 mimllearning-0.3.2/src/miml/datasets/miml_birds_random_20test.arff
+-rw-r--r--   0        0        0   498562 2020-02-02 00:00:00.000000 mimllearning-0.3.2/src/miml/datasets/miml_birds_random_80train.arff
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 mimllearning-0.3.2/src/miml/datasets/toy.arff
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 mimllearning-0.3.2/src/miml/datasets/toy.csv
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 mimllearning-0.3.2/src/miml/report/__init__.py
+-rw-r--r--   0        0        0     7299 2020-02-02 00:00:00.000000 mimllearning-0.3.2/src/miml/report/report.py
+-rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 mimllearning-0.3.2/src/miml/test/data_test.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 mimllearning-0.3.2/src/miml/transformation/__init__.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 mimllearning-0.3.2/src/miml/transformation/mimlTOmi/__init__.py
+-rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 mimllearning-0.3.2/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 mimllearning-0.3.2/src/miml/transformation/mimlTOml/__init__.py
+-rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 mimllearning-0.3.2/src/miml/transformation/mimlTOml/arithmetic.py
+-rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 mimllearning-0.3.2/src/miml/transformation/mimlTOml/geometric.py
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 mimllearning-0.3.2/src/miml/transformation/mimlTOml/miml_to_ml_transformation.py
+-rw-r--r--   0        0        0     2826 2020-02-02 00:00:00.000000 mimllearning-0.3.2/src/miml/transformation/mimlTOml/minmax.py
+-rw-r--r--   0        0        0     9910 2020-02-02 00:00:00.000000 mimllearning-0.3.2/src/miml/tutorial/demo.ipynb
+-rw-r--r--   0        0        0    13016 2020-02-02 00:00:00.000000 mimllearning-0.3.2/src/miml/tutorial/miml_transformations.ipynb
+-rw-r--r--   0        0        0    11077 2020-02-02 00:00:00.000000 mimllearning-0.3.2/src/miml/tutorial/mimltoml_classifiers.ipynb
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 mimllearning-0.3.2/.gitignore
+-rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 mimllearning-0.3.2/README.md
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 mimllearning-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     2386 2020-02-02 00:00:00.000000 mimllearning-0.3.2/PKG-INFO
```

### Comparing `mimllearning-0.3.1/readme.md` & `mimllearning-0.3.2/readme.md`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.1/documentation/AnteproyectoDamianTFG.pdf` & `mimllearning-0.3.2/documentation/AnteproyectoDamianTFG.pdf`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.1/src/miml/classifier/miml_classifier.py` & `mimllearning-0.3.2/src/miml/classifier/miml_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.1/src/miml/classifier/mi/all_positive_apr_classifier.py` & `mimllearning-0.3.2/src/miml/classifier/mi/all_positive_apr_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.1/src/miml/classifier/mi/apr_classifier.py` & `mimllearning-0.3.2/src/miml/classifier/mi/apr_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.1/src/miml/classifier/mi/miles_classifier.py` & `mimllearning-0.3.2/src/miml/classifier/mi/miles_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.1/src/miml/classifier/mimlTOmi/miml_to_mi_br_classifier.py` & `mimllearning-0.3.2/src/miml/classifier/mimlTOmi/miml_to_mi_br_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.1/src/miml/classifier/mimlTOmi/miml_to_mi_classifier.py` & `mimllearning-0.3.2/src/miml/classifier/mimlTOmi/miml_to_mi_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.1/src/miml/classifier/mimlTOml/miml_to_ml_classifier.py` & `mimllearning-0.3.2/src/miml/classifier/mimlTOml/miml_to_ml_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.1/src/miml/data/arff_to_csv.py` & `mimllearning-0.3.2/src/miml/data/arff_to_csv.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.1/src/miml/data/bag.py` & `mimllearning-0.3.2/src/miml/data/bag.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.1/src/miml/data/instance.py` & `mimllearning-0.3.2/src/miml/data/instance.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.1/src/miml/data/load_datasets.py` & `mimllearning-0.3.2/src/miml/data/load_datasets.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import numpy as np
 import os
 
+import pkg_resources
+
 from .bag import Bag
 from .instance import Instance
 from .miml_dataset import MIMLDataset
 
 
 def load_dataset(file: str, delimiter: str = "\"") -> MIMLDataset:
     """
@@ -139,18 +141,35 @@
             labels = line[line.find(delimiter, 2) + 2:]
             labels_values = [int(i) for i in labels.split(",")]
             # print("Labels: ", labels)
 
             values_list = []
             for v in values:
                 values_instance = [float(i) for i in v.split(',')]
-                instance = Instance(values_instance+labels_values)
+                instance = Instance(values_instance + labels_values)
                 if key not in dataset.data:
                     bag = Bag(key)
                     bag.add_instance(instance)
                     dataset.add_bag(bag)
                 else:
                     dataset.add_instance(key, instance)
 
     dataset.set_features_name(features_name)
     dataset.set_labels_name(labels_name)
     return dataset
+
+
+def load_toy():
+    # TODO: Doc
+    return load_dataset(pkg_resources.resource_filename('miml', 'datasets/toy.arff'), delimiter="'")
+
+
+def load_birds_train():
+    # TODO: Doc
+    return load_dataset(pkg_resources.resource_filename('miml', 'datasets/miml_birds_random_80train.arff'),
+                        delimiter="'")
+
+
+def load_birds_test():
+    # TODO: Doc
+    return load_dataset(pkg_resources.resource_filename('miml', 'datasets/miml_birds_random_20test.arff'),
+                        delimiter="'")
```

### Comparing `mimllearning-0.3.1/src/miml/data/miml_dataset.py` & `mimllearning-0.3.2/src/miml/data/miml_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -243,16 +243,19 @@
         Add a bag to the dataset
 
         Parameters
         ----------
         bag : Bag
             Instance of Bag class to be added
         """
-        bag.set_dataset(self)
-        self.data[bag.key] = bag
+        if bag.get_number_attributes() == self.get_number_attributes():
+            bag.set_dataset(self)
+            self.data[bag.key] = bag
+        else:
+            raise Exception("The bag doesn't have the same attributes as the dataset")
 
     def delete_bag(self, key_bag: str) -> None:
         """
         Delete a bag of the dataset
 
         Parameters
         ----------
```

### Comparing `mimllearning-0.3.1/src/miml/datasets/miml_birds.arff` & `mimllearning-0.3.2/src/miml/datasets/miml_birds.arff`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.1/src/miml/datasets/miml_birds.csv` & `mimllearning-0.3.2/src/miml/datasets/miml_birds.csv`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.1/src/miml/datasets/miml_birds_random_20test.arff` & `mimllearning-0.3.2/src/miml/datasets/miml_birds_random_20test.arff`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.1/src/miml/datasets/miml_birds_random_80train.arff` & `mimllearning-0.3.2/src/miml/datasets/miml_birds_random_80train.arff`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.1/src/miml/report/report.py` & `mimllearning-0.3.2/src/miml/report/report.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,28 +7,30 @@
 
 class Report:
     """
     Class to generate a report
     """
 
     def __init__(self, classifier: MIMLClassifier, dataset_test: MIMLDataset, metrics: list[str] = None,
-                 header: bool = True, per_label: bool = False):
+                 header: bool = True, per_label: bool = True):
 
+        self.dataset = dataset_test
         self.y_true = dataset_test.get_labels_by_bag()
         self.y_pred = classifier.evaluate(dataset_test)
         self.probs = classifier.predict_proba(dataset_test)
 
         all_metrics = ["precision-score-macro", "precision-score-micro", "average-precision-score-macro",
                        "average-precision-score-micro", "recall-score-macro", "recall-score-micro", "f1-score-macro",
                        "f1-score-micro", "fbeta-score-macro", "fbeta-score-micro", "accuracy-score", "hamming-loss",
                        "jaccard-score-macro", "jaccard-score-micro", "log-loss"]
-
         if per_label:
-            all_metrics += ["precision-score-per-label", "recall-score-per-label", "f1-score-per-label",
-                            "fbeta-score-per-label", "jaccard-score-per-label"]
+            per_label_metrics = ["precision-score", "recall-score", "f1-score", "fbeta-score", "jaccard-score"]
+            for metric in per_label_metrics:
+                for label in dataset_test.get_labels_name():
+                    all_metrics.append(metric+"-"+label)
 
         if metrics is None:
             metrics = all_metrics
         else:
             for metric in metrics:
                 if metric not in all_metrics:
                     raise Exception("Metric ", metric, "is not valid\n", "Metrics availables: ", all_metrics)
@@ -72,25 +74,27 @@
         with warnings.catch_warnings():
             warnings.filterwarnings("ignore", category=UserWarning)
             # When log_loss called raise this warning, it is not true for multilabel classification
             # UserWarning: The y_pred values do not sum to one. Starting from 1.5 thiswill result in an error.
             self.metrics_value["log-loss"] = log_loss(self.y_true, self.probs)
 
         if self.per_label:
-            self.metrics_value["precision-score-per-label"] = list(precision_score(self.y_true, self.y_pred,
-                                                                                   average=None, zero_division=0))
-            self.metrics_value["recall-score-per-label"] = list(recall_score(self.y_true, self.y_pred, average=None,
-                                                                             zero_division=0))
-            self.metrics_value["f1-score-per-label"] = list(f1_score(self.y_true, self.y_pred, average=None,
-                                                                     zero_division=0))
-            self.metrics_value["fbeta-score-per-label"] = list(fbeta_score(self.y_true, self.y_pred, beta=1,
-                                                                           average=None, zero_division=0))
-            # self.metrics_value["roc-auc-score-per-label"] = roc_auc_score(self.y_true, self.probs, average="None")
-            self.metrics_value["jaccard-score-per-label"] = list(jaccard_score(self.y_true, self.y_pred, average=None,
-                                                                               zero_division=0))
+            precision_score_per_label = list(precision_score(self.y_true, self.y_pred, average=None, zero_division=0))
+            recall_score_per_label = list(recall_score(self.y_true, self.y_pred, average=None, zero_division=0))
+            f1_score_per_label = list(f1_score(self.y_true, self.y_pred, average=None, zero_division=0))
+            fbeta_score_per_label = list(fbeta_score(self.y_true, self.y_pred, beta=1, average=None, zero_division=0))
+            #roc_auc_score_per_label = list(roc_auc_score(self.y_true, self.probs, average="None"))
+            jaccard_score_per_label = list(jaccard_score(self.y_true, self.y_pred, average=None, zero_division=0))
+            for i, label in enumerate(self.dataset.get_labels_name()):
+                self.metrics_value["precision-score-"+label] = precision_score_per_label[i]
+                self.metrics_value["recall-score-"+label] = recall_score_per_label[i]
+                self.metrics_value["f1-score-"+label] = f1_score_per_label[i]
+                self.metrics_value["fbeta-score-"+label] = fbeta_score_per_label[i]
+                # self.metrics_value["roc-auc-score-"+label] = roc_auc_score_per_label[i]
+                self.metrics_value["jaccard-score-"+label] = jaccard_score_per_label[i]
 
     def to_csv(self, path=None):
         self.calculate_metrics()
         header = ""
         if self.header:
             header = ",".join(str(metric) for metric in self.metrics_name)
         values = ",".join(str(self.metrics_value[metric]) for metric in self.metrics_name)
```

### Comparing `mimllearning-0.3.1/src/miml/test/data_test.py` & `mimllearning-0.3.2/src/miml/test/data_test.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.1/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py` & `mimllearning-0.3.2/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.1/src/miml/transformation/mimlTOml/arithmetic.py` & `mimllearning-0.3.2/src/miml/transformation/mimlTOml/arithmetic.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.1/src/miml/transformation/mimlTOml/geometric.py` & `mimllearning-0.3.2/src/miml/transformation/mimlTOml/geometric.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.1/src/miml/transformation/mimlTOml/minmax.py` & `mimllearning-0.3.2/src/miml/transformation/mimlTOml/minmax.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.1/src/miml/tutorial/demo.ipynb` & `mimllearning-0.3.2/src/miml/tutorial/demo.ipynb`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.1/src/miml/tutorial/miml_transformations.ipynb` & `mimllearning-0.3.2/src/miml/tutorial/miml_transformations.ipynb`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.1/src/miml/tutorial/mimltoml_classifiers.ipynb` & `mimllearning-0.3.2/src/miml/tutorial/mimltoml_classifiers.ipynb`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.1/README.md` & `mimllearning-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.1/pyproject.toml` & `mimllearning-0.3.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 requires = ["hatchling", "pkginfo >= 1.10"]
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/miml", "src/miml/*"]
 
 [metadata]
-version = "0.3.1"
+version = "0.3.2"
 name = "mimllearning"
 
 [project]
 name = "mimllearning"
-version = "0.3.1"
+version = "0.3.2"
 authors = [
   { name="Damian Martinez", email="damianmartinezavila@gmail.com" },
 ]
 description = "MIML Learning Library"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `mimllearning-0.3.1/PKG-INFO` & `mimllearning-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: mimllearning
-Version: 0.3.1
+Version: 0.3.2
 Summary: MIML Learning Library
 Project-URL: Homepage, https://github.com/p82maavd/miml
 Author-email: Damian Martinez <damianmartinezavila@gmail.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

