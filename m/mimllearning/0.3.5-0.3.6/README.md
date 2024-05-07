# Comparing `tmp/mimllearning-0.3.5.tar.gz` & `tmp/mimllearning-0.3.6.tar.gz`

## Comparing `mimllearning-0.3.5.tar` & `mimllearning-0.3.6.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 mimllearning-0.3.5/readme.md
--rw-r--r--   0        0        0   258069 2020-02-02 00:00:00.000000 mimllearning-0.3.5/documentation/AnteproyectoDamianTFG.pdf
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 mimllearning-0.3.5/src/miml/__init__.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 mimllearning-0.3.5/src/miml/classifier/__init__.py
--rw-r--r--   0        0        0     2841 2020-02-02 00:00:00.000000 mimllearning-0.3.5/src/miml/classifier/miml_classifier.py
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 mimllearning-0.3.5/src/miml/classifier/mi/__init__.py
--rw-r--r--   0        0        0     2984 2020-02-02 00:00:00.000000 mimllearning-0.3.5/src/miml/classifier/mi/all_positive_apr_classifier.py
--rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 mimllearning-0.3.5/src/miml/classifier/mi/apr_classifier.py
--rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 mimllearning-0.3.5/src/miml/classifier/mi/miles_classifier.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 mimllearning-0.3.5/src/miml/classifier/mimlTOmi/__init__.py
--rw-r--r--   0        0        0     3646 2020-02-02 00:00:00.000000 mimllearning-0.3.5/src/miml/classifier/mimlTOmi/miml_to_mi_br_classifier.py
--rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 mimllearning-0.3.5/src/miml/classifier/mimlTOmi/miml_to_mi_classifier.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 mimllearning-0.3.5/src/miml/classifier/mimlTOml/__init__.py
--rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 mimllearning-0.3.5/src/miml/classifier/mimlTOml/miml_to_ml_classifier.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 mimllearning-0.3.5/src/miml/data/__init__.py
--rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 mimllearning-0.3.5/src/miml/data/arff_to_csv.py
--rw-r--r--   0        0        0     8990 2020-02-02 00:00:00.000000 mimllearning-0.3.5/src/miml/data/bag.py
--rw-r--r--   0        0        0     6840 2020-02-02 00:00:00.000000 mimllearning-0.3.5/src/miml/data/instance.py
--rw-r--r--   0        0        0     5341 2020-02-02 00:00:00.000000 mimllearning-0.3.5/src/miml/data/load_datasets.py
--rw-r--r--   0        0        0    15894 2020-02-02 00:00:00.000000 mimllearning-0.3.5/src/miml/data/miml_dataset.py
--rw-r--r--   0        0        0   735908 2020-02-02 00:00:00.000000 mimllearning-0.3.5/src/miml/datasets/miml_birds.arff
--rw-r--r--   0        0        0   842801 2020-02-02 00:00:00.000000 mimllearning-0.3.5/src/miml/datasets/miml_birds.csv
--rw-r--r--   0        0        0   134841 2020-02-02 00:00:00.000000 mimllearning-0.3.5/src/miml/datasets/miml_birds_random_20test.arff
--rw-r--r--   0        0        0   498562 2020-02-02 00:00:00.000000 mimllearning-0.3.5/src/miml/datasets/miml_birds_random_80train.arff
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 mimllearning-0.3.5/src/miml/datasets/toy.arff
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 mimllearning-0.3.5/src/miml/datasets/toy.csv
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 mimllearning-0.3.5/src/miml/report/__init__.py
--rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 mimllearning-0.3.5/src/miml/report/report.py
--rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 mimllearning-0.3.5/src/miml/test/data_test.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 mimllearning-0.3.5/src/miml/transformation/__init__.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 mimllearning-0.3.5/src/miml/transformation/mimlTOmi/__init__.py
--rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 mimllearning-0.3.5/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 mimllearning-0.3.5/src/miml/transformation/mimlTOml/__init__.py
--rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 mimllearning-0.3.5/src/miml/transformation/mimlTOml/arithmetic.py
--rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 mimllearning-0.3.5/src/miml/transformation/mimlTOml/geometric.py
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 mimllearning-0.3.5/src/miml/transformation/mimlTOml/miml_to_ml_transformation.py
--rw-r--r--   0        0        0     3036 2020-02-02 00:00:00.000000 mimllearning-0.3.5/src/miml/transformation/mimlTOml/minmax.py
--rw-r--r--   0        0        0     9910 2020-02-02 00:00:00.000000 mimllearning-0.3.5/src/miml/tutorial/demo.ipynb
--rw-r--r--   0        0        0     6472 2020-02-02 00:00:00.000000 mimllearning-0.3.5/src/miml/tutorial/miml_data.ipynb
--rw-r--r--   0        0        0    13016 2020-02-02 00:00:00.000000 mimllearning-0.3.5/src/miml/tutorial/miml_transformations.ipynb
--rw-r--r--   0        0        0    11077 2020-02-02 00:00:00.000000 mimllearning-0.3.5/src/miml/tutorial/mimltoml_classifiers.ipynb
--rw-r--r--   0        0        0    16340 2020-02-02 00:00:00.000000 mimllearning-0.3.5/src/miml/tutorial/new_demo.ipynb
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 mimllearning-0.3.5/.gitignore
--rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 mimllearning-0.3.5/README.md
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 mimllearning-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     2386 2020-02-02 00:00:00.000000 mimllearning-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 mimllearning-0.3.6/readme.md
+-rw-r--r--   0        0        0   258069 2020-02-02 00:00:00.000000 mimllearning-0.3.6/documentation/AnteproyectoDamianTFG.pdf
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 mimllearning-0.3.6/src/miml/__init__.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 mimllearning-0.3.6/src/miml/classifier/__init__.py
+-rw-r--r--   0        0        0     2841 2020-02-02 00:00:00.000000 mimllearning-0.3.6/src/miml/classifier/miml_classifier.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 mimllearning-0.3.6/src/miml/classifier/mi/__init__.py
+-rw-r--r--   0        0        0     2984 2020-02-02 00:00:00.000000 mimllearning-0.3.6/src/miml/classifier/mi/all_positive_apr_classifier.py
+-rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 mimllearning-0.3.6/src/miml/classifier/mi/apr_classifier.py
+-rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 mimllearning-0.3.6/src/miml/classifier/mi/miles_classifier.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 mimllearning-0.3.6/src/miml/classifier/mimlTOmi/__init__.py
+-rw-r--r--   0        0        0     3646 2020-02-02 00:00:00.000000 mimllearning-0.3.6/src/miml/classifier/mimlTOmi/miml_to_mi_br_classifier.py
+-rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 mimllearning-0.3.6/src/miml/classifier/mimlTOmi/miml_to_mi_classifier.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 mimllearning-0.3.6/src/miml/classifier/mimlTOml/__init__.py
+-rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 mimllearning-0.3.6/src/miml/classifier/mimlTOml/miml_to_ml_classifier.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 mimllearning-0.3.6/src/miml/data/__init__.py
+-rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 mimllearning-0.3.6/src/miml/data/arff_to_csv.py
+-rw-r--r--   0        0        0     8990 2020-02-02 00:00:00.000000 mimllearning-0.3.6/src/miml/data/bag.py
+-rw-r--r--   0        0        0     6840 2020-02-02 00:00:00.000000 mimllearning-0.3.6/src/miml/data/instance.py
+-rw-r--r--   0        0        0     5341 2020-02-02 00:00:00.000000 mimllearning-0.3.6/src/miml/data/load_datasets.py
+-rw-r--r--   0        0        0    15871 2020-02-02 00:00:00.000000 mimllearning-0.3.6/src/miml/data/miml_dataset.py
+-rw-r--r--   0        0        0   735908 2020-02-02 00:00:00.000000 mimllearning-0.3.6/src/miml/datasets/miml_birds.arff
+-rw-r--r--   0        0        0   842801 2020-02-02 00:00:00.000000 mimllearning-0.3.6/src/miml/datasets/miml_birds.csv
+-rw-r--r--   0        0        0   134841 2020-02-02 00:00:00.000000 mimllearning-0.3.6/src/miml/datasets/miml_birds_random_20test.arff
+-rw-r--r--   0        0        0   498562 2020-02-02 00:00:00.000000 mimllearning-0.3.6/src/miml/datasets/miml_birds_random_80train.arff
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 mimllearning-0.3.6/src/miml/datasets/toy.arff
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 mimllearning-0.3.6/src/miml/datasets/toy.csv
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 mimllearning-0.3.6/src/miml/report/__init__.py
+-rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 mimllearning-0.3.6/src/miml/report/report.py
+-rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 mimllearning-0.3.6/src/miml/test/data_test.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 mimllearning-0.3.6/src/miml/transformation/__init__.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 mimllearning-0.3.6/src/miml/transformation/mimlTOmi/__init__.py
+-rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 mimllearning-0.3.6/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 mimllearning-0.3.6/src/miml/transformation/mimlTOml/__init__.py
+-rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 mimllearning-0.3.6/src/miml/transformation/mimlTOml/arithmetic.py
+-rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 mimllearning-0.3.6/src/miml/transformation/mimlTOml/geometric.py
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 mimllearning-0.3.6/src/miml/transformation/mimlTOml/miml_to_ml_transformation.py
+-rw-r--r--   0        0        0     3036 2020-02-02 00:00:00.000000 mimllearning-0.3.6/src/miml/transformation/mimlTOml/minmax.py
+-rw-r--r--   0        0        0     9910 2020-02-02 00:00:00.000000 mimllearning-0.3.6/src/miml/tutorial/demo.ipynb
+-rw-r--r--   0        0        0     6472 2020-02-02 00:00:00.000000 mimllearning-0.3.6/src/miml/tutorial/miml_data.ipynb
+-rw-r--r--   0        0        0    13016 2020-02-02 00:00:00.000000 mimllearning-0.3.6/src/miml/tutorial/miml_transformations.ipynb
+-rw-r--r--   0        0        0    11077 2020-02-02 00:00:00.000000 mimllearning-0.3.6/src/miml/tutorial/mimltoml_classifiers.ipynb
+-rw-r--r--   0        0        0    16340 2020-02-02 00:00:00.000000 mimllearning-0.3.6/src/miml/tutorial/new_demo.ipynb
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 mimllearning-0.3.6/.gitignore
+-rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 mimllearning-0.3.6/README.md
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 mimllearning-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0     2386 2020-02-02 00:00:00.000000 mimllearning-0.3.6/PKG-INFO
```

### Comparing `mimllearning-0.3.5/readme.md` & `mimllearning-0.3.6/readme.md`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.5/documentation/AnteproyectoDamianTFG.pdf` & `mimllearning-0.3.6/documentation/AnteproyectoDamianTFG.pdf`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.5/src/miml/classifier/miml_classifier.py` & `mimllearning-0.3.6/src/miml/classifier/miml_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.5/src/miml/classifier/mi/all_positive_apr_classifier.py` & `mimllearning-0.3.6/src/miml/classifier/mi/all_positive_apr_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.5/src/miml/classifier/mi/apr_classifier.py` & `mimllearning-0.3.6/src/miml/classifier/mi/apr_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.5/src/miml/classifier/mi/miles_classifier.py` & `mimllearning-0.3.6/src/miml/classifier/mi/miles_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.5/src/miml/classifier/mimlTOmi/miml_to_mi_br_classifier.py` & `mimllearning-0.3.6/src/miml/classifier/mimlTOmi/miml_to_mi_br_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.5/src/miml/classifier/mimlTOmi/miml_to_mi_classifier.py` & `mimllearning-0.3.6/src/miml/classifier/mimlTOmi/miml_to_mi_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.5/src/miml/classifier/mimlTOml/miml_to_ml_classifier.py` & `mimllearning-0.3.6/src/miml/classifier/mimlTOml/miml_to_ml_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.5/src/miml/data/arff_to_csv.py` & `mimllearning-0.3.6/src/miml/data/arff_to_csv.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.5/src/miml/data/bag.py` & `mimllearning-0.3.6/src/miml/data/bag.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.5/src/miml/data/instance.py` & `mimllearning-0.3.6/src/miml/data/instance.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.5/src/miml/data/load_datasets.py` & `mimllearning-0.3.6/src/miml/data/load_datasets.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.5/src/miml/data/miml_dataset.py` & `mimllearning-0.3.6/src/miml/data/miml_dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -524,10 +524,10 @@
         print("Nº of bags: ", self.get_number_bags())
         print("Total instances: ", n_instances)
         print("Average Instances per bag: ", n_instances / self.get_number_bags())
         print("Min Instances per bag: ", min_instances)
         print("Max Instances per bag: ", max_instances)
         print("Attributes per bag: ", self.get_number_attributes())
         # TODO: Implementarlo
-        print("\nDistribution of bags <nBags, nInstances>:");
-        for number_instances_in_bag, occurrences in distribution():
+        print("\nDistribution of bags:")
+        for number_instances_in_bag, occurrences in distribution:
             print("\tBags with ", number_instances_in_bag, " instances: ", occurrences)
```

### Comparing `mimllearning-0.3.5/src/miml/datasets/miml_birds.arff` & `mimllearning-0.3.6/src/miml/datasets/miml_birds.arff`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.5/src/miml/datasets/miml_birds.csv` & `mimllearning-0.3.6/src/miml/datasets/miml_birds.csv`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.5/src/miml/datasets/miml_birds_random_20test.arff` & `mimllearning-0.3.6/src/miml/datasets/miml_birds_random_20test.arff`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.5/src/miml/datasets/miml_birds_random_80train.arff` & `mimllearning-0.3.6/src/miml/datasets/miml_birds_random_80train.arff`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.5/src/miml/report/report.py` & `mimllearning-0.3.6/src/miml/report/report.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.5/src/miml/test/data_test.py` & `mimllearning-0.3.6/src/miml/test/data_test.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.5/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py` & `mimllearning-0.3.6/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.5/src/miml/transformation/mimlTOml/arithmetic.py` & `mimllearning-0.3.6/src/miml/transformation/mimlTOml/arithmetic.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.5/src/miml/transformation/mimlTOml/geometric.py` & `mimllearning-0.3.6/src/miml/transformation/mimlTOml/geometric.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.5/src/miml/transformation/mimlTOml/minmax.py` & `mimllearning-0.3.6/src/miml/transformation/mimlTOml/minmax.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.5/src/miml/tutorial/demo.ipynb` & `mimllearning-0.3.6/src/miml/tutorial/demo.ipynb`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.5/src/miml/tutorial/miml_data.ipynb` & `mimllearning-0.3.6/src/miml/tutorial/miml_data.ipynb`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.5/src/miml/tutorial/miml_transformations.ipynb` & `mimllearning-0.3.6/src/miml/tutorial/miml_transformations.ipynb`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.5/src/miml/tutorial/mimltoml_classifiers.ipynb` & `mimllearning-0.3.6/src/miml/tutorial/mimltoml_classifiers.ipynb`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.5/src/miml/tutorial/new_demo.ipynb` & `mimllearning-0.3.6/src/miml/tutorial/new_demo.ipynb`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.5/README.md` & `mimllearning-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `mimllearning-0.3.5/pyproject.toml` & `mimllearning-0.3.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 requires = ["hatchling", "pkginfo >= 1.10"]
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/miml", "src/miml/*"]
 
 [metadata]
-version = "0.3.5"
+version = "0.3.6"
 name = "mimllearning"
 
 [project]
 name = "mimllearning"
-version = "0.3.5"
+version = "0.3.6"
 authors = [
   { name="Damian Martinez", email="damianmartinezavila@gmail.com" },
 ]
 description = "MIML Learning Library"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `mimllearning-0.3.5/PKG-INFO` & `mimllearning-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: mimllearning
-Version: 0.3.5
+Version: 0.3.6
 Summary: MIML Learning Library
 Project-URL: Homepage, https://github.com/p82maavd/miml
 Author-email: Damian Martinez <damianmartinezavila@gmail.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

