# Comparing `tmp/Aianalytics-1.0.80.tar.gz` & `tmp/Aianalytics-1.0.82.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Aianalytics-1.0.80.tar", last modified: Tue May  7 14:53:04 2024, max compression
+gzip compressed data, was "Aianalytics-1.0.82.tar", last modified: Tue May  7 14:55:40 2024, max compression
```

## Comparing `Aianalytics-1.0.80.tar` & `Aianalytics-1.0.82.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 14:53:04.350286 Aianalytics-1.0.80/
-drwxrwxrwx   0        0        0        0 2024-05-07 14:53:04.317400 Aianalytics-1.0.80/Aianalytics/
--rw-rw-rw-   0        0        0    86147 2024-05-07 14:52:06.000000 Aianalytics-1.0.80/Aianalytics/__init__.py
--rw-rw-rw-   0        0        0    86147 2024-05-07 14:52:21.000000 Aianalytics-1.0.80/Aianalytics/a.py
-drwxrwxrwx   0        0        0        0 2024-05-07 14:53:04.345299 Aianalytics-1.0.80/Aianalytics.egg-info/
--rw-rw-rw-   0        0        0      579 2024-05-07 14:53:03.000000 Aianalytics-1.0.80/Aianalytics.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2024-05-07 14:53:03.000000 Aianalytics-1.0.80/Aianalytics.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 14:53:03.000000 Aianalytics-1.0.80/Aianalytics.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      143 2024-05-07 14:53:03.000000 Aianalytics-1.0.80/Aianalytics.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-07 14:53:03.000000 Aianalytics-1.0.80/Aianalytics.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1477 2023-07-11 09:07:10.000000 Aianalytics-1.0.80/LICENSE.txt
--rw-rw-rw-   0        0        0      579 2024-05-07 14:53:04.347293 Aianalytics-1.0.80/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-07 14:53:04.350286 Aianalytics-1.0.80/setup.cfg
--rw-rw-rw-   0        0        0     1078 2024-05-07 14:52:52.000000 Aianalytics-1.0.80/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 14:55:40.215205 Aianalytics-1.0.82/
+drwxrwxrwx   0        0        0        0 2024-05-07 14:55:40.195095 Aianalytics-1.0.82/Aianalytics/
+-rw-rw-rw-   0        0        0    90351 2024-05-07 14:54:39.000000 Aianalytics-1.0.82/Aianalytics/__init__.py
+-rw-rw-rw-   0        0        0    90351 2024-05-07 14:54:44.000000 Aianalytics-1.0.82/Aianalytics/a.py
+drwxrwxrwx   0        0        0        0 2024-05-07 14:55:40.214204 Aianalytics-1.0.82/Aianalytics.egg-info/
+-rw-rw-rw-   0        0        0      579 2024-05-07 14:55:40.000000 Aianalytics-1.0.82/Aianalytics.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2024-05-07 14:55:40.000000 Aianalytics-1.0.82/Aianalytics.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 14:55:40.000000 Aianalytics-1.0.82/Aianalytics.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      143 2024-05-07 14:55:40.000000 Aianalytics-1.0.82/Aianalytics.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-07 14:55:40.000000 Aianalytics-1.0.82/Aianalytics.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1477 2023-07-11 09:07:10.000000 Aianalytics-1.0.82/LICENSE.txt
+-rw-rw-rw-   0        0        0      579 2024-05-07 14:55:40.215205 Aianalytics-1.0.82/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-07 14:55:40.216202 Aianalytics-1.0.82/setup.cfg
+-rw-rw-rw-   0        0        0     1078 2024-05-07 14:55:35.000000 Aianalytics-1.0.82/setup.py
```

### Comparing `Aianalytics-1.0.80/Aianalytics/__init__.py` & `Aianalytics-1.0.82/Aianalytics/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -2551,8 +2551,129 @@
     </application>
 
 </manifest>
 OUTPUT :
  
 .
 
-"""
+"""
+    print(code)
+
+
+def intent():
+    code="""
+ Intent
+To create a program to implement intent (Implicit and Explicit).
+
+Activity_main.xml
+<?xml version="1.0" encoding="utf-8"?>
+<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
+    xmlns:app="http://schemas.android.com/apk/res-auto"
+    xmlns:tools="http://schemas.android.com/tools"
+    android:layout_width="match_parent"
+    android:layout_height="match_parent"
+    tools:context=".MainActivity">
+
+    <TextView
+        android:id="@+id/textView5"
+        android:layout_width="wrap_content"
+        android:layout_height="wrap_content"
+        android:layout_marginTop="37dp"
+        android:layout_marginBottom="42dp"
+        android:text="My Name is"
+        app:layout_constraintBottom_toTopOf="@+id/button2"
+        app:layout_constraintEnd_toEndOf="parent"
+        app:layout_constraintHorizontal_bias="0.498"
+        app:layout_constraintStart_toStartOf="parent"
+        app:layout_constraintTop_toBottomOf="@+id/textView6" />
+
+    <TextView
+        android:id="@+id/textView6"
+        android:layout_width="wrap_content"
+        android:layout_height="wrap_content"
+        android:layout_marginTop="44dp"
+        android:layout_marginBottom="36dp"
+        android:text="Enter your name"
+        app:layout_constraintBottom_toTopOf="@+id/textView5"
+        app:layout_constraintEnd_toEndOf="parent"
+        app:layout_constraintHorizontal_bias="0.498"
+        app:layout_constraintStart_toStartOf="parent"
+        app:layout_constraintTop_toBottomOf="@+id/editText" />
+
+    <Button
+        android:id="@+id/button2"
+        android:layout_width="183dp"
+        android:layout_height="39dp"
+        android:layout_marginTop="23dp"
+        android:layout_marginBottom="430dp"
+        android:text="Click here to pop-up"
+        app:layout_constraintBottom_toBottomOf="parent"
+        app:layout_constraintEnd_toEndOf="parent"
+        app:layout_constraintHorizontal_bias="0.442"
+        app:layout_constraintStart_toStartOf="parent"
+        app:layout_constraintTop_toBottomOf="@+id/textView5" />
+
+    <EditText
+        android:id="@+id/editText"
+        android:layout_width="357dp"
+        android:layout_height="87dp"
+        android:layout_marginTop="6dp"
+        android:layout_marginEnd="36dp"
+        android:layout_marginBottom="14dp"
+        android:ems="10"
+        android:inputType="textPersonName"
+        android:text="Intent In Android"
+        app:layout_constraintBottom_toTopOf="@+id/textView6"
+        app:layout_constraintEnd_toEndOf="parent"
+        app:layout_constraintHorizontal_bias="1.0"
+        app:layout_constraintStart_toStartOf="parent"
+        app:layout_constraintTop_toTopOf="parent"
+        tools:text="Enter Name" />
+
+
+</androidx.constraintlayout.widget.ConstraintLayout>
+
+MainActivity.kt
+package com.example.trial5
+
+import androidx.appcompat.app.AppCompatActivity
+import android.os.Bundle
+import android.text.Editable
+import android.text.TextWatcher
+import android.widget.Button
+import android.widget.EditText
+import android.widget.TextView
+import android.widget.Toast
+
+class MainActivity : AppCompatActivity() {
+    override fun onCreate(savedInstanceState: Bundle?) {
+        super.onCreate(savedInstanceState)
+        setContentView(R.layout.activity_main)
+
+        val clickme = findViewById<Button>(R.id.button2)
+        clickme.setOnClickListener {
+            Toast.makeText(this,"Button Clicked", Toast.LENGTH_SHORT).show()
+        }
+
+        val display = findViewById<TextView>(R.id.textView5)
+        val enteredName  = findViewById<EditText>(R.id.editText)
+        enteredName.addTextChangedListener(object : TextWatcher {
+            override fun beforeTextChanged(p0: CharSequence?, p1: Int, p2: Int, p3: Int) {
+
+            }
+
+            override fun afterTextChanged(p0: Editable?) {
+
+            }
+
+            override fun onTextChanged(p0: CharSequence?, p1: Int, p2: Int, p3: Int) {
+                display.setText("Your Name in Edit Text is : "+p0)
+
+            }
+
+        })
+
+    }
+}
+
+"""
+    print(code)
```

### Comparing `Aianalytics-1.0.80/Aianalytics/a.py` & `Aianalytics-1.0.82/Aianalytics/a.py`

 * *Files 4% similar despite different names*

```diff
@@ -2551,8 +2551,129 @@
     </application>
 
 </manifest>
 OUTPUT :
  
 .
 
-"""
+"""
+    print(code)
+
+
+def intent():
+    code="""
+ Intent
+To create a program to implement intent (Implicit and Explicit).
+
+Activity_main.xml
+<?xml version="1.0" encoding="utf-8"?>
+<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
+    xmlns:app="http://schemas.android.com/apk/res-auto"
+    xmlns:tools="http://schemas.android.com/tools"
+    android:layout_width="match_parent"
+    android:layout_height="match_parent"
+    tools:context=".MainActivity">
+
+    <TextView
+        android:id="@+id/textView5"
+        android:layout_width="wrap_content"
+        android:layout_height="wrap_content"
+        android:layout_marginTop="37dp"
+        android:layout_marginBottom="42dp"
+        android:text="My Name is"
+        app:layout_constraintBottom_toTopOf="@+id/button2"
+        app:layout_constraintEnd_toEndOf="parent"
+        app:layout_constraintHorizontal_bias="0.498"
+        app:layout_constraintStart_toStartOf="parent"
+        app:layout_constraintTop_toBottomOf="@+id/textView6" />
+
+    <TextView
+        android:id="@+id/textView6"
+        android:layout_width="wrap_content"
+        android:layout_height="wrap_content"
+        android:layout_marginTop="44dp"
+        android:layout_marginBottom="36dp"
+        android:text="Enter your name"
+        app:layout_constraintBottom_toTopOf="@+id/textView5"
+        app:layout_constraintEnd_toEndOf="parent"
+        app:layout_constraintHorizontal_bias="0.498"
+        app:layout_constraintStart_toStartOf="parent"
+        app:layout_constraintTop_toBottomOf="@+id/editText" />
+
+    <Button
+        android:id="@+id/button2"
+        android:layout_width="183dp"
+        android:layout_height="39dp"
+        android:layout_marginTop="23dp"
+        android:layout_marginBottom="430dp"
+        android:text="Click here to pop-up"
+        app:layout_constraintBottom_toBottomOf="parent"
+        app:layout_constraintEnd_toEndOf="parent"
+        app:layout_constraintHorizontal_bias="0.442"
+        app:layout_constraintStart_toStartOf="parent"
+        app:layout_constraintTop_toBottomOf="@+id/textView5" />
+
+    <EditText
+        android:id="@+id/editText"
+        android:layout_width="357dp"
+        android:layout_height="87dp"
+        android:layout_marginTop="6dp"
+        android:layout_marginEnd="36dp"
+        android:layout_marginBottom="14dp"
+        android:ems="10"
+        android:inputType="textPersonName"
+        android:text="Intent In Android"
+        app:layout_constraintBottom_toTopOf="@+id/textView6"
+        app:layout_constraintEnd_toEndOf="parent"
+        app:layout_constraintHorizontal_bias="1.0"
+        app:layout_constraintStart_toStartOf="parent"
+        app:layout_constraintTop_toTopOf="parent"
+        tools:text="Enter Name" />
+
+
+</androidx.constraintlayout.widget.ConstraintLayout>
+
+MainActivity.kt
+package com.example.trial5
+
+import androidx.appcompat.app.AppCompatActivity
+import android.os.Bundle
+import android.text.Editable
+import android.text.TextWatcher
+import android.widget.Button
+import android.widget.EditText
+import android.widget.TextView
+import android.widget.Toast
+
+class MainActivity : AppCompatActivity() {
+    override fun onCreate(savedInstanceState: Bundle?) {
+        super.onCreate(savedInstanceState)
+        setContentView(R.layout.activity_main)
+
+        val clickme = findViewById<Button>(R.id.button2)
+        clickme.setOnClickListener {
+            Toast.makeText(this,"Button Clicked", Toast.LENGTH_SHORT).show()
+        }
+
+        val display = findViewById<TextView>(R.id.textView5)
+        val enteredName  = findViewById<EditText>(R.id.editText)
+        enteredName.addTextChangedListener(object : TextWatcher {
+            override fun beforeTextChanged(p0: CharSequence?, p1: Int, p2: Int, p3: Int) {
+
+            }
+
+            override fun afterTextChanged(p0: Editable?) {
+
+            }
+
+            override fun onTextChanged(p0: CharSequence?, p1: Int, p2: Int, p3: Int) {
+                display.setText("Your Name in Edit Text is : "+p0)
+
+            }
+
+        })
+
+    }
+}
+
+"""
+    print(code)
```

### Comparing `Aianalytics-1.0.80/Aianalytics.egg-info/PKG-INFO` & `Aianalytics-1.0.82/Aianalytics.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Aianalytics
-Version: 1.0.80
+Version: 1.0.82
 Summary: A module for image processing
 Author: Armankhanvsit
 Author-email: armanpconly@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `Aianalytics-1.0.80/LICENSE.txt` & `Aianalytics-1.0.82/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Aianalytics-1.0.80/PKG-INFO` & `Aianalytics-1.0.82/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Aianalytics
-Version: 1.0.80
+Version: 1.0.82
 Summary: A module for image processing
 Author: Armankhanvsit
 Author-email: armanpconly@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `Aianalytics-1.0.80/setup.py` & `Aianalytics-1.0.82/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='Aianalytics',
-    version='1.0.80',
+    version='1.0.82',
     author='Armankhanvsit',
     author_email='armanpconly@gmail.com',
     description='A module for image processing',
     long_description='A module for image processing using numpy, PIL, scipy, and matplotlib.',
     packages=['Aianalytics'],
   install_requires=[
     'numpy',
```

