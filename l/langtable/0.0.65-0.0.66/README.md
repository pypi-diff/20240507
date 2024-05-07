# Comparing `tmp/langtable-0.0.65.tar.gz` & `tmp/langtable-0.0.66.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langtable-0.0.65.tar", last modified: Thu Feb  8 18:04:34 2024, max compression
+gzip compressed data, was "langtable-0.0.66.tar", last modified: Tue May  7 16:51:53 2024, max compression
```

## Comparing `langtable-0.0.65.tar` & `langtable-0.0.66.tar`

### file list

```diff
@@ -1,36 +1,38 @@
-drwxr-xr-x   0 mfabian  (10030) mfabian  (10030)        0 2024-02-08 18:04:34.808354 langtable-0.0.65/
--rw-r--r--   0 mfabian  (10030) mfabian  (10030)    35147 2013-05-08 14:51:39.000000 langtable-0.0.65/COPYING
--rw-r--r--   0 mfabian  (10030) mfabian  (10030)    19067 2024-02-08 17:27:27.000000 langtable-0.0.65/ChangeLog
--rw-r--r--   0 mfabian  (10030) mfabian  (10030)      163 2019-09-04 14:23:21.000000 langtable-0.0.65/MANIFEST.in
--rw-r--r--   0 mfabian  (10030) mfabian  (10030)     2750 2024-02-08 18:04:32.000000 langtable-0.0.65/Makefile
--rw-r--r--   0 mfabian  (10030) mfabian  (10030)     2549 2024-02-08 18:04:34.808354 langtable-0.0.65/PKG-INFO
--rw-r--r--   0 mfabian  (10030) mfabian  (10030)     1915 2024-02-08 17:27:27.000000 langtable-0.0.65/README
-drwxr-xr-x   0 mfabian  (10030) mfabian  (10030)        0 2024-02-08 18:04:34.806354 langtable-0.0.65/langtable/
--rw-r--r--   0 mfabian  (10030) mfabian  (10030)      526 2024-02-08 17:27:27.000000 langtable-0.0.65/langtable/__init__.py
-drwxr-xr-x   0 mfabian  (10030) mfabian  (10030)        0 2024-02-08 18:04:34.807354 langtable-0.0.65/langtable/data/
--rw-r--r--   0 mfabian  (10030) mfabian  (10030)     5888 2023-05-02 13:29:52.000000 langtable-0.0.65/langtable/data/keyboards.xml.gz
--rw-r--r--   0 mfabian  (10030) mfabian  (10030)   407980 2024-02-08 17:27:27.000000 langtable-0.0.65/langtable/data/languages.xml.gz
--rw-r--r--   0 mfabian  (10030) mfabian  (10030)   494333 2024-02-08 17:27:27.000000 langtable-0.0.65/langtable/data/territories.xml.gz
--rw-r--r--   0 mfabian  (10030) mfabian  (10030)   378548 2024-02-08 17:27:27.000000 langtable-0.0.65/langtable/data/timezoneidparts.xml.gz
--rw-r--r--   0 mfabian  (10030) mfabian  (10030)     3542 2022-01-25 07:22:23.000000 langtable-0.0.65/langtable/data/timezones.xml.gz
--rw-r--r--   0 mfabian  (10030) mfabian  (10030)   107347 2024-02-08 17:27:27.000000 langtable-0.0.65/langtable/langtable.py
-drwxr-xr-x   0 mfabian  (10030) mfabian  (10030)        0 2024-02-08 18:04:34.807354 langtable-0.0.65/langtable/schemas/
--rw-r--r--   0 mfabian  (10030) mfabian  (10030)     1301 2019-09-04 14:23:21.000000 langtable-0.0.65/langtable/schemas/keyboards.rng
--rw-r--r--   0 mfabian  (10030) mfabian  (10030)     4153 2019-09-04 14:23:21.000000 langtable-0.0.65/langtable/schemas/languages.rng
--rw-r--r--   0 mfabian  (10030) mfabian  (10030)     3482 2019-09-04 14:23:21.000000 langtable-0.0.65/langtable/schemas/territories.rng
--rw-r--r--   0 mfabian  (10030) mfabian  (10030)      683 2019-09-04 14:23:21.000000 langtable-0.0.65/langtable/schemas/timezoneidparts.rng
--rw-r--r--   0 mfabian  (10030) mfabian  (10030)      665 2019-09-04 14:23:21.000000 langtable-0.0.65/langtable/schemas/timezones.rng
-drwxr-xr-x   0 mfabian  (10030) mfabian  (10030)        0 2024-02-08 18:04:34.806354 langtable-0.0.65/langtable.egg-info/
--rw-r--r--   0 mfabian  (10030) mfabian  (10030)     2549 2024-02-08 18:04:34.000000 langtable-0.0.65/langtable.egg-info/PKG-INFO
--rw-r--r--   0 mfabian  (10030) mfabian  (10030)      719 2024-02-08 18:04:34.000000 langtable-0.0.65/langtable.egg-info/SOURCES.txt
--rw-r--r--   0 mfabian  (10030) mfabian  (10030)        1 2024-02-08 18:04:34.000000 langtable-0.0.65/langtable.egg-info/dependency_links.txt
--rw-r--r--   0 mfabian  (10030) mfabian  (10030)        1 2024-02-08 17:02:48.000000 langtable-0.0.65/langtable.egg-info/not-zip-safe
--rw-r--r--   0 mfabian  (10030) mfabian  (10030)       10 2024-02-08 18:04:34.000000 langtable-0.0.65/langtable.egg-info/top_level.txt
--rwxr-xr-x   0 mfabian  (10030) mfabian  (10030)    16310 2023-08-27 07:15:11.000000 langtable-0.0.65/main.py
--rw-r--r--   0 mfabian  (10030) mfabian  (10030)       38 2024-02-08 18:04:34.808354 langtable-0.0.65/setup.cfg
--rwxr-xr-x   0 mfabian  (10030) mfabian  (10030)     1811 2024-02-08 17:27:27.000000 langtable-0.0.65/setup.py
--rw-r--r--   0 mfabian  (10030) mfabian  (10030)   135787 2024-02-08 17:27:27.000000 langtable-0.0.65/test_cases.py
-drwxr-xr-x   0 mfabian  (10030) mfabian  (10030)        0 2024-02-08 18:04:34.808354 langtable-0.0.65/tools/
--rwxr-xr-x   0 mfabian  (10030) mfabian  (10030)     5005 2019-12-20 16:08:11.000000 langtable-0.0.65/tools/compare_with_glib_source.py
--rwxr-xr-x   0 mfabian  (10030) mfabian  (10030)     2931 2024-02-08 17:27:27.000000 langtable-0.0.65/tools/list-missing-regions-and-languages.sh
--rw-r--r--   0 mfabian  (10030) mfabian  (10030)     2933 2013-05-08 14:51:39.000000 langtable-0.0.65/unicode-license.txt
+drwxr-xr-x   0 mfabian  (10030) mfabian  (10030)        0 2024-05-07 16:51:53.230448 langtable-0.0.66/
+-rw-r--r--   0 mfabian  (10030) mfabian  (10030)    35147 2013-05-08 14:51:39.000000 langtable-0.0.66/COPYING
+-rw-r--r--   0 mfabian  (10030) mfabian  (10030)    19845 2024-05-07 16:25:07.000000 langtable-0.0.66/ChangeLog
+-rw-r--r--   0 mfabian  (10030) mfabian  (10030)      216 2024-05-07 16:25:07.000000 langtable-0.0.66/MANIFEST.in
+-rw-r--r--   0 mfabian  (10030) mfabian  (10030)     3037 2024-05-07 16:14:59.000000 langtable-0.0.66/Makefile
+-rw-r--r--   0 mfabian  (10030) mfabian  (10030)     2622 2024-05-07 16:51:53.230448 langtable-0.0.66/PKG-INFO
+-rw-r--r--   0 mfabian  (10030) mfabian  (10030)     1984 2024-02-22 09:53:02.000000 langtable-0.0.66/README
+-rw-r--r--   0 mfabian  (10030) mfabian  (10030)    37909 2024-02-22 09:52:49.000000 langtable-0.0.66/README.html
+-rw-r--r--   0 mfabian  (10030) mfabian  (10030)     1948 2024-02-22 09:52:44.000000 langtable-0.0.66/README.md
+drwxr-xr-x   0 mfabian  (10030) mfabian  (10030)        0 2024-05-07 16:51:53.228448 langtable-0.0.66/langtable/
+-rw-r--r--   0 mfabian  (10030) mfabian  (10030)      526 2024-02-08 17:27:27.000000 langtable-0.0.66/langtable/__init__.py
+drwxr-xr-x   0 mfabian  (10030) mfabian  (10030)        0 2024-05-07 16:51:53.229448 langtable-0.0.66/langtable/data/
+-rw-r--r--   0 mfabian  (10030) mfabian  (10030)     5888 2023-05-02 13:29:52.000000 langtable-0.0.66/langtable/data/keyboards.xml.gz
+-rw-r--r--   0 mfabian  (10030) mfabian  (10030)   409136 2024-05-07 16:25:07.000000 langtable-0.0.66/langtable/data/languages.xml.gz
+-rw-r--r--   0 mfabian  (10030) mfabian  (10030)   494566 2024-05-07 16:25:07.000000 langtable-0.0.66/langtable/data/territories.xml.gz
+-rw-r--r--   0 mfabian  (10030) mfabian  (10030)   378548 2024-02-08 17:27:27.000000 langtable-0.0.66/langtable/data/timezoneidparts.xml.gz
+-rw-r--r--   0 mfabian  (10030) mfabian  (10030)     3542 2022-01-25 07:22:23.000000 langtable-0.0.66/langtable/data/timezones.xml.gz
+-rw-r--r--   0 mfabian  (10030) mfabian  (10030)   107558 2024-02-13 16:18:42.000000 langtable-0.0.66/langtable/langtable.py
+drwxr-xr-x   0 mfabian  (10030) mfabian  (10030)        0 2024-05-07 16:51:53.230448 langtable-0.0.66/langtable/schemas/
+-rw-r--r--   0 mfabian  (10030) mfabian  (10030)     1301 2019-09-04 14:23:21.000000 langtable-0.0.66/langtable/schemas/keyboards.rng
+-rw-r--r--   0 mfabian  (10030) mfabian  (10030)     4153 2019-09-04 14:23:21.000000 langtable-0.0.66/langtable/schemas/languages.rng
+-rw-r--r--   0 mfabian  (10030) mfabian  (10030)     3482 2019-09-04 14:23:21.000000 langtable-0.0.66/langtable/schemas/territories.rng
+-rw-r--r--   0 mfabian  (10030) mfabian  (10030)      683 2019-09-04 14:23:21.000000 langtable-0.0.66/langtable/schemas/timezoneidparts.rng
+-rw-r--r--   0 mfabian  (10030) mfabian  (10030)      665 2019-09-04 14:23:21.000000 langtable-0.0.66/langtable/schemas/timezones.rng
+drwxr-xr-x   0 mfabian  (10030) mfabian  (10030)        0 2024-05-07 16:51:53.230448 langtable-0.0.66/langtable.egg-info/
+-rw-r--r--   0 mfabian  (10030) mfabian  (10030)     2622 2024-05-07 16:51:53.000000 langtable-0.0.66/langtable.egg-info/PKG-INFO
+-rw-r--r--   0 mfabian  (10030) mfabian  (10030)      741 2024-05-07 16:51:53.000000 langtable-0.0.66/langtable.egg-info/SOURCES.txt
+-rw-r--r--   0 mfabian  (10030) mfabian  (10030)        1 2024-05-07 16:51:53.000000 langtable-0.0.66/langtable.egg-info/dependency_links.txt
+-rw-r--r--   0 mfabian  (10030) mfabian  (10030)        1 2024-05-07 16:27:26.000000 langtable-0.0.66/langtable.egg-info/not-zip-safe
+-rw-r--r--   0 mfabian  (10030) mfabian  (10030)       10 2024-05-07 16:51:53.000000 langtable-0.0.66/langtable.egg-info/top_level.txt
+-rwxr-xr-x   0 mfabian  (10030) mfabian  (10030)    16575 2024-05-07 16:25:07.000000 langtable-0.0.66/main.py
+-rw-r--r--   0 mfabian  (10030) mfabian  (10030)       38 2024-05-07 16:51:53.230448 langtable-0.0.66/setup.cfg
+-rwxr-xr-x   0 mfabian  (10030) mfabian  (10030)     1865 2024-05-07 16:25:07.000000 langtable-0.0.66/setup.py
+-rw-r--r--   0 mfabian  (10030) mfabian  (10030)   135886 2024-05-07 16:25:07.000000 langtable-0.0.66/test_cases.py
+drwxr-xr-x   0 mfabian  (10030) mfabian  (10030)        0 2024-05-07 16:51:53.230448 langtable-0.0.66/tools/
+-rwxr-xr-x   0 mfabian  (10030) mfabian  (10030)     5005 2019-12-20 16:08:11.000000 langtable-0.0.66/tools/compare_with_glib_source.py
+-rwxr-xr-x   0 mfabian  (10030) mfabian  (10030)     2931 2024-02-08 17:27:27.000000 langtable-0.0.66/tools/list-missing-regions-and-languages.sh
+-rw-r--r--   0 mfabian  (10030) mfabian  (10030)     2933 2013-05-08 14:51:39.000000 langtable-0.0.66/unicode-license.txt
```

### Comparing `langtable-0.0.65/COPYING` & `langtable-0.0.66/COPYING`

 * *Files identical despite different names*

### Comparing `langtable-0.0.65/ChangeLog` & `langtable-0.0.66/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+2024-05-07  Mike FABIAN  <mfabian@redhat.com>
+
+	* Fix syntax error in a keyboard layout name for th
+	(Resolves: https://github.com/mike-fabian/langtable/issues/21xs)
+	* Add mdf
+	* Use “in(eng)” keyboard layout instead of “us” for BD to get AltGr enabled
+	* Get translation changes from CLDR
+	* Add option to include changed translations as well to the script getting translations from CLDR
+	* Add reference to the the PyPI package to the README.md.
+	And add a README.html and README generated from the README.md.
+	* Make test outputs somewhat more verbose, even when all tests pass
+	(Resolves: https://github.com/mike-fabian/langtable/pull/20).
+	Thanks to Sebastian <seb128@ubuntu.com> for the pull request.
+	* Fix Makefile twine-upload target for new authentification
+
 2024-02-08  Mike FABIAN  <mfabian@redhat.com>
 
 	* Add wuu, tok, glk, gbm, ssy
 	* Remove aa_ER.UTF-8@saaho
 	* Add kv_RU.UTF-8, chr_RU.UTF-8
 	* Add EU, EZ
 	* Improve README and Makefile (Resolves: https://github.com/mike-fabian/langtable/issues/19)
```

### Comparing `langtable-0.0.65/Makefile` & `langtable-0.0.66/Makefile`

 * *Files 11% similar despite different names*

```diff
@@ -5,35 +5,39 @@
 SRCDIR=$(PWD)
 
 .PHONY: gzip
 gzip: langtable/data/keyboards.xml.gz langtable/data/languages.xml.gz langtable/data/territories.xml.gz langtable/data/timezones.xml.gz langtable/data/timezoneidparts.xml.gz
 
 .PHONY: test
 test: gzip
-	(cd langtable; python3 langtable.py)
+	python3 langtable/langtable.py
 	python3 test_cases.py
-	(cd langtable; xmllint --noout --relaxng schemas/keyboards.rng data/keyboards.xml.gz)
-	(cd langtable; xmllint --noout --relaxng schemas/languages.rng data/languages.xml.gz)
-	(cd langtable; xmllint --noout --relaxng schemas/territories.rng data/territories.xml.gz)
-	(cd langtable; xmllint --noout --relaxng schemas/timezones.rng data/timezones.xml.gz)
-	(cd langtable; xmllint --noout --relaxng schemas/timezoneidparts.rng data/timezoneidparts.xml.gz)
+	xmllint --noout --relaxng langtable/schemas/keyboards.rng langtable/data/keyboards.xml.gz
+	xmllint --noout --relaxng langtable/schemas/languages.rng langtable/data/languages.xml.gz
+	xmllint --noout --relaxng langtable/schemas/territories.rng langtable/data/territories.xml.gz
+	xmllint --noout --relaxng langtable/schemas/timezones.rng langtable/data/timezones.xml.gz
+	xmllint --noout --relaxng langtable/schemas/timezoneidparts.rng langtable/data/timezoneidparts.xml.gz
 
 .PHONY: check
 check: test
 
 .PHONY: dist
 dist: gzip
 	DISTUTILS_DEBUG=$(DEBUG) python3 ./setup.py sdist bdist_wheel
 
 .PHONY: install
 install: dist
 	perl -pi -e "s,_datadir = '(.*)',_DATADIR = '$(DATADIR)'," langtable/langtable.py
 	DISTUTILS_DEBUG=$(DEBUG) python3 ./setup.py install --prefix=$(DESTDIR)
 #	DISTUTILS_DEBUG=$(DEBUG) python3 ./setup.py install_data --install-dir=$(DATADIR)
 
+.PHONY: twine-check
+twine-check: dist
+	twine check dist/*
+
 # check it here: https://test.pypi.org/manage/project/langtable/releases/
 .PHONY: twine-upload-test
 twine-upload-test: dist
 	python3 -m twine upload --verbose --repository testpypi dist/*
 
 # check it here: https://pypi.org/manage/project/langtable/releases/
 .PHONY: twine-upload
@@ -72,7 +76,13 @@
 # .rnc files for editing with Emacs
 # https://fedoraproject.org/wiki/How_to_use_Emacs_for_XML_editing
 %.rnc: %.rng
 	trang $< $@
 
 rnc: schemas/keyboards.rnc schemas/languages.rnc schemas/territories.rnc schemas/timezones.rnc schemas/timezoneidparts.rnc
 	cp schemas/*.rnc data/
+
+README: README.html
+	w3m -cols 78 -o display_borders=1 -o display_link_number=1 $< > $@
+
+README.html: README.md
+	pandoc -f gfm -t html --standalone --self-contained --metadata pagetitle="langtable README" $< > $@
```

### Comparing `langtable-0.0.65/PKG-INFO` & `langtable-0.0.66/README`

 * *Files 12% similar despite different names*

```diff
@@ -1,66 +1,47 @@
-Metadata-Version: 2.1
-Name: langtable
-Version: 0.0.65
-Summary: guess reasonable defaults for locale, keyboard, territory, ...
-Home-page: https://github.com/mike-fabian/langtable
-Author: Mike FABIAN
-Author-email: mfabian@redhat.com
-License: GPL-3.0-or-later
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python
-Classifier: Topic :: System :: Installation/Setup
-License-File: COPYING
-
-======================================================================
 langtable
-======================================================================
+
+[1]PyPI version
+
+Guessing reasonable defaults for locale, keyboard layout, territory, and
+language.
 
 Purpose of this package
-=======================
 
 langtable is used to guess reasonable defaults for locale, keyboard,
-territory, …, if part of that information is already known. For
-example, guess the territory and the keyboard layout if the language
-is known or guess the language and keyboard layout if the territory is
-already known.
+territory, …, if part of that information is already known. For example,
+guess the territory and the keyboard layout if the language is known or guess
+the language and keyboard layout if the territory is already known.
 
 License
-=======
 
 GPLv3+, see the included file “COPYING”.
 
 Translations for languages and territory names are from CLDR which is
 governed by the Unicode Terms of Use, see the included file
-“unicode-license.txt”. The short name for this Unicode license is
-“MIT”. See:
+“unicode-license.txt”. The short name for this Unicode license is “MIT”. See:
 
-https://fedoraproject.org/wiki/Licensing:MIT?rd=Licensing/MIT#Modern_Style_without_sublicense_.28Unicode.29
+[2]https://fedoraproject.org/wiki/Licensing:MIT?rd=Licensing/MIT#
+Modern_Style_without_sublicense_.28Unicode.29
 
 Installation
-============
 
 To install langtable, run
 
      make install DESTDIR=/usr
 
 To create a distribution tarball run
 
      make dist
 
 To run the test cases in the source directory:
 
-     make test
+     make check
 
 How to use it
-=============
 
 import langtable
 
 Functions in the public API:
 
      parse_locale()
      list_locales()
@@ -83,11 +64,17 @@
      list_all_keyboards()
      list_all_territories()
      list_all_timezones()
      list_all_scripts()
      list_all_input_methods()
      list_all_console_fonts()
 
-Some examples to show the usage are found in the documentation
-of the public functions in langtable.py.
+Some examples to show the usage are found in the documentation of the public
+functions in langtable.py.
+
+Some more examples are in the test cases in the file test_cases.py.
+
+
+References:
 
-(Some more examples are in the test cases in the file test_cases.py):
+[1] https://badge.fury.io/py/langtable
+[2] https://fedoraproject.org/wiki/Licensing:MIT?rd=Licensing/MIT#Modern_Style_without_sublicense_.28Unicode.29
```

### Comparing `langtable-0.0.65/langtable/__init__.py` & `langtable-0.0.66/langtable/__init__.py`

 * *Files identical despite different names*

### Comparing `langtable-0.0.65/langtable/data/keyboards.xml.gz` & `langtable-0.0.66/langtable/data/keyboards.xml.gz`

 * *Files identical despite different names*

### Comparing `langtable-0.0.65/langtable/data/timezoneidparts.xml.gz` & `langtable-0.0.66/langtable/data/timezoneidparts.xml.gz`

 * *Files identical despite different names*

### Comparing `langtable-0.0.65/langtable/data/timezones.xml.gz` & `langtable-0.0.66/langtable/data/timezones.xml.gz`

 * *Files identical despite different names*

### Comparing `langtable-0.0.65/langtable/langtable.py` & `langtable-0.0.66/langtable/langtable.py`

 * *Files 0% similar despite different names*

```diff
@@ -2715,9 +2715,15 @@
     def __del__(self):
         return
 
 __module_init = __ModuleInitializer()
 
 if __name__ == "__main__":
     import doctest
+    import sys
     _init()
-    doctest.testmod()
+    (FAILED, ATTEMPTED) = doctest.testmod()
+    print(f'{ATTEMPTED} tests run. {ATTEMPTED - FAILED} passed and {FAILED} failed.')
+    if FAILED:
+        sys.exit(FAILED)
+    print(f'All tests passed.')
+    sys.exit(0)
```

### Comparing `langtable-0.0.65/langtable/schemas/keyboards.rng` & `langtable-0.0.66/langtable/schemas/keyboards.rng`

 * *Files identical despite different names*

### Comparing `langtable-0.0.65/langtable/schemas/languages.rng` & `langtable-0.0.66/langtable/schemas/languages.rng`

 * *Files identical despite different names*

### Comparing `langtable-0.0.65/langtable/schemas/territories.rng` & `langtable-0.0.66/langtable/schemas/territories.rng`

 * *Files identical despite different names*

### Comparing `langtable-0.0.65/langtable/schemas/timezoneidparts.rng` & `langtable-0.0.66/langtable/schemas/timezoneidparts.rng`

 * *Files identical despite different names*

### Comparing `langtable-0.0.65/langtable/schemas/timezones.rng` & `langtable-0.0.66/langtable/schemas/timezones.rng`

 * *Files identical despite different names*

### Comparing `langtable-0.0.65/langtable.egg-info/PKG-INFO` & `langtable-0.0.66/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,71 +1,50 @@
-Metadata-Version: 2.1
-Name: langtable
-Version: 0.0.65
-Summary: guess reasonable defaults for locale, keyboard, territory, ...
-Home-page: https://github.com/mike-fabian/langtable
-Author: Mike FABIAN
-Author-email: mfabian@redhat.com
-License: GPL-3.0-or-later
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python
-Classifier: Topic :: System :: Installation/Setup
-License-File: COPYING
-
-======================================================================
-langtable
-======================================================================
-
-Purpose of this package
-=======================
-
-langtable is used to guess reasonable defaults for locale, keyboard,
-territory, …, if part of that information is already known. For
-example, guess the territory and the keyboard layout if the language
-is known or guess the language and keyboard layout if the territory is
-already known.
+# langtable
 
-License
-=======
+[![PyPI version](https://badge.fury.io/py/langtable.svg)](https://badge.fury.io/py/langtable)
+
+Guessing reasonable defaults for locale, keyboard layout, territory, and language.
+
+## Purpose of this package
+_langtable_ is used to guess reasonable defaults for locale, keyboard, territory, …, if part of that information is already known. For example, guess the territory and the keyboard layout if the language is known or guess the language and keyboard layout if the territory is already known.
+
+## License
 
 GPLv3+, see the included file “COPYING”.
 
-Translations for languages and territory names are from CLDR which is
-governed by the Unicode Terms of Use, see the included file
-“unicode-license.txt”. The short name for this Unicode license is
-“MIT”. See:
+Translations for languages and territory names are from CLDR which is governed by the Unicode Terms of Use, see the included file “unicode-license.txt”. The short name for this Unicode license is “MIT”. See:
 
 https://fedoraproject.org/wiki/Licensing:MIT?rd=Licensing/MIT#Modern_Style_without_sublicense_.28Unicode.29
 
-Installation
-============
+## Installation
 
 To install langtable, run
 
+```
      make install DESTDIR=/usr
+```
 
 To create a distribution tarball run
-
+```
      make dist
-
+```
 To run the test cases in the source directory:
+```
+     make check
+```
 
-     make test
-
-How to use it
-=============
+## How to use it
 
+```
 import langtable
+```
 
 Functions in the public API:
 
+```
      parse_locale()
      list_locales()
      list_keyboards()
      list_common_languages()
      list_common_locales()
      list_common_keyboards()
      list_consolefonts()
@@ -82,12 +61,12 @@
      list_all_locales()
      list_all_keyboards()
      list_all_territories()
      list_all_timezones()
      list_all_scripts()
      list_all_input_methods()
      list_all_console_fonts()
+```
 
-Some examples to show the usage are found in the documentation
-of the public functions in langtable.py.
+Some examples to show the usage are found in the documentation of the public functions in `langtable.py`.
 
-(Some more examples are in the test cases in the file test_cases.py):
+Some more examples are in the test cases in the file `test_cases.py`.
```

### Comparing `langtable-0.0.65/langtable.egg-info/SOURCES.txt` & `langtable-0.0.66/langtable.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 COPYING
 ChangeLog
 MANIFEST.in
 Makefile
 README
+README.html
+README.md
 main.py
 setup.py
 test_cases.py
 unicode-license.txt
 langtable/__init__.py
 langtable/langtable.py
 langtable.egg-info/PKG-INFO
```

### Comparing `langtable-0.0.65/main.py` & `langtable-0.0.66/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,14 +57,18 @@
                         default='./langtable/data/timezoneidparts.xml.new',
                         help='timezoneidparts output file, default is %(default)s')
     parser.add_argument('-l', '--logfilename',
                         nargs='?',
                         type=str,
                         default='./langtable.log',
                         help='log file, default is %(default)s')
+    parser.add_argument('-c', '--include_changes',
+                        action='store_true',
+                        default=False,
+                        help='Also write changed translations, not only new translations, default is %(default)s.')
     parser.add_argument('-d', '--debug',
                         action='store_true',
                         help='print debugging output')
     return parser.parse_args()
 
 translations_languages = {}
 translations_territories = {}
@@ -129,15 +133,15 @@
                                                     cityTranslation = element.text
                                                     translations_timezone_cities[idPart] = cityTranslation
     for alias in timezone_city_aliases:
         if alias in translations_timezone_cities:
             translations_timezone_cities[timezone_city_aliases[alias]] = translations_timezone_cities[alias]
     return
 
-def get_translations_from_cldr(main_cldr_dir = None):
+def get_translations_from_cldr(main_cldr_dir = None, include_changes=False):
     for target_language in sorted(langtable._languages_db):
         cldr_file = main_cldr_dir+'/'+target_language+'.xml'
         if not os.path.exists(cldr_file):
             continue
         read_translations_from_cldr_file(cldr_file)
         for language_to_translate in translations_languages:
             if translations_languages[language_to_translate] in ('↑↑↑', 'Tagalog'):
@@ -161,16 +165,16 @@
                         'language_to_translate': language_to_translate,
                         'target_language': target_language,
                         'tr': langtable._languages_db[language_to_translate].names[target_language]})
                     print("+ %(language_to_translate)s → %(target_language)s = %(tr)s" %{
                         'language_to_translate': language_to_translate,
                         'target_language': target_language,
                         'tr': translations_languages[language_to_translate]})
-                    # Uncomment this to really make the change:
-                    #langtable._languages_db[language_to_translate].names[target_language] = translations_languages[language_to_translate]
+                    if include_changes:
+                        langtable._languages_db[language_to_translate].names[target_language] = translations_languages[language_to_translate]
             else:
                 if opts['debug']:
                     print("Not in langtable: %(language_to_translate)s" %{
                         'language_to_translate': language_to_translate})
         for territory_to_translate in translations_territories:
             if translations_territories[territory_to_translate] in ('↑↑↑',):
                 continue
@@ -190,16 +194,16 @@
                     print("- %(territory_to_translate)s → %(target_language)s = %(tr)s" %{
                         'territory_to_translate': territory_to_translate,
                         'target_language': target_language,
                         'tr': langtable._territories_db[territory_to_translate].names[target_language]})
                     print("+ %(territory_to_translate)s → %(target_language)s = %(tr)s" %{'territory_to_translate': territory_to_translate,
                                                                                            'target_language': target_language,
                                                                                            'tr': translations_territories[territory_to_translate]})
-                    # Uncomment this to really make the change:
-                    #langtable._territories_db[territory_to_translate].names[target_language] = translations_territories[territory_to_translate]
+                    if include_changes:
+                        langtable._territories_db[territory_to_translate].names[target_language] = translations_territories[territory_to_translate]
             else:
                 if opts['debug']:
                     print("Not in langtable: %(territory_to_translate)s" %{
                         'territory_to_translate': territory_to_translate})
         for timezone_city_to_translate in translations_timezone_cities:
             if translations_timezone_cities[timezone_city_to_translate] in ('↑↑↑',):
                 continue
@@ -224,16 +228,16 @@
                             'timezone_city_to_translate': timezone_city_to_translate,
                             'target_language': target_language,
                             'tr': langtable._timezoneIdParts_db[timezone_city_to_translate].names[target_language]})
                         print("+ %(timezone_city_to_translate)s → %(target_language)s = %(tr)s" %{
                             'timezone_city_to_translate': timezone_city_to_translate,
                             'target_language': target_language,
                             'tr': translations_timezone_cities[timezone_city_to_translate]})
-                        # Uncomment this to really make the change:
-                        #langtable._timezoneIdParts_db[timezone_city_to_translate].names[target_language] = translations_timezone_cities[timezone_city_to_translate]
+                        if include_changes:
+                            langtable._timezoneIdParts_db[timezone_city_to_translate].names[target_language] = translations_timezone_cities[timezone_city_to_translate]
     return
 
 def _test_timezone_names():
     from pytz import common_timezones
     languages_supported_by_anaconda = ['af', 'am', 'ar', 'as', 'ast', 'bal', 'be', 'bg', 'bn', 'bn_IN', 'bs', 'ca', 'cs', 'cy', 'da', 'de', 'de_CH', 'el', 'en', 'en_GB', 'es', 'et', 'eu', 'eu_ES', 'fa', 'fi', 'fr', 'gl', 'gu', 'he', 'hi', 'hr', 'hu', 'hy', 'ia', 'id', 'ilo', 'is', 'it', 'ja', 'ka', 'kk', 'kn', 'ko', 'lt', 'lv', 'mai', 'mk', 'ml', 'mr', 'ms', 'nb', 'nds', 'ne', 'nl', 'nn', 'nso', 'or', 'pa', 'pl', 'pt', 'pt_BR', 'ro', 'ru', 'si', 'sk', 'sl', 'sq', 'sr', 'sr_Latn', 'sv', 'ta', 'te', 'tg', 'th', 'tr', 'uk', 'ur', 'vi', 'zh_CN', 'zh_TW', 'zu']
     for icuLocaleId in languages_supported_by_anaconda:
         for timezoneId in common_timezones:
@@ -247,20 +251,21 @@
         opts['debug'] = True
     else:
         opts['debug'] = False
 
     langtable._init(debug = True,
                     logfilename = args.logfilename)
 
-    get_translations_from_cldr(main_cldr_dir='/local/mfabian/src/cldr/common/main')
+    get_translations_from_cldr(
+        main_cldr_dir='/local/mfabian/src/cldr/common/main',
+        include_changes=args.include_changes)
 
     #_test_timezone_names()
 
     langtable._write_files(territoriesfilename = args.territoriesoutputfile,
                            languagesfilename = args.languagesoutputfile,
                            keyboardsfilename = args.keyboardsoutputfile,
                            timezonesfilename = args.timezonesoutputfile,
                            timezoneidpartsfilename = args.timezoneidpartsoutputfile)
 
-
 if __name__ == '__main__':
     main()
```

### Comparing `langtable-0.0.65/setup.py` & `langtable-0.0.66/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,18 +4,19 @@
 import codecs
 
 setuptools.setup(
     # do not zip the egg file to be able to access the *.xml.gz files
     # within the egg directory easily:
     zip_safe=False,
     name='langtable',
-    version='0.0.65',
+    version='0.0.66',
     packages=setuptools.find_packages(),
     description='guess reasonable defaults for locale, keyboard, territory, ...',
-    long_description=codecs.open('README', encoding='UTF-8').read(),
+    long_description=codecs.open('README.md', encoding='UTF-8').read(),
+    long_description_content_type='text/markdown',
     license="GPL-3.0-or-later",
     author='Mike FABIAN',
     author_email='mfabian@redhat.com',
     url='https://github.com/mike-fabian/langtable',
     py_modules=['langtable'],
     package_data={
         'langtable': ['data/*.xml.gz', 'schemas/*.rng'],
```

### Comparing `langtable-0.0.65/test_cases.py` & `langtable-0.0.66/test_cases.py`

 * *Files 0% similar despite different names*

```diff
@@ -757,16 +757,16 @@
          +: ['in(eng)']
 
     >>> _test_language_territory(show_weights=False, languageId="bn", territoryId="BD") # doctest: +NORMALIZE_WHITESPACE
         bn: ['bn_BD.UTF-8', 'bn_IN.UTF-8']
         BD: ['bn_BD.UTF-8']
          +: ['bn_BD.UTF-8']
         bn: ['in(eng)']
-        BD: ['us']
-         +: ['us', 'in(eng)']
+        BD: ['in(eng)']
+         +: ['in(eng)']
 
     >>> _test_language_territory(show_weights=False, languageId="bn", territoryId="IN") # doctest: +NORMALIZE_WHITESPACE
         bn: ['bn_BD.UTF-8', 'bn_IN.UTF-8']
         IN: ['hi_IN.UTF-8', 'en_IN.UTF-8', 'bn_IN.UTF-8', 'te_IN.UTF-8', 'mr_IN.UTF-8', 'ta_IN.UTF-8', 'ur_IN.UTF-8', 'gu_IN.UTF-8', 'kn_IN.UTF-8', 'ml_IN.UTF-8', 'or_IN.UTF-8', 'pa_IN.UTF-8', 'as_IN.UTF-8', 'mai_IN.UTF-8', 'sat_IN.UTF-8', 'ks_IN.UTF-8', 'ks_IN.UTF-8@devanagari', 'kok_IN.UTF-8', 'sd_IN.UTF-8', 'sd_IN.UTF-8@devanagari', 'doi_IN.UTF-8', 'mni_IN.UTF-8', 'brx_IN.UTF-8', 'raj_IN.UTF-8', 'mjw_IN.UTF-8', 'anp_IN.UTF-8', 'bhb_IN.UTF-8', 'bho_IN.UTF-8', 'bo_IN.UTF-8', 'hne_IN.UTF-8', 'mag_IN.UTF-8', 'tcy_IN.UTF-8', 'ar_IN.UTF-8', 'gbm_IN.UTF-8']
          +: ['bn_IN.UTF-8']
         bn: ['in(eng)']
         IN: ['in(eng)', 'ara']
@@ -2151,17 +2151,17 @@
         ['cn']
     >>> print(list_common_keyboards(languageId='zh', scriptId='Hans', territoryId='TW'))   # doctest: +NORMALIZE_WHITESPACE
         ['tw']
     >>> print(list_common_languages())   # doctest: +NORMALIZE_WHITESPACE
         ['ar', 'en', 'fr', 'de', 'ja', 'zh', 'ru', 'es']
 
     >>> print(list_all_languages())    # doctest: +NORMALIZE_WHITESPACE
-    ['aa', 'ab', 'af', 'agq', 'agr', 'ak', 'am', 'an', 'anp', 'ar', 'as', 'asa', 'ast', 'av', 'ay', 'ayc', 'ayr', 'az', 'ba', 'bas', 'be', 'bem', 'ber', 'bez', 'bg', 'bhb', 'bho', 'bi', 'bih', 'bin', 'bm', 'bn', 'bo', 'br', 'brx', 'bs', 'bua', 'byn', 'ca', 'ca_ES_VALENCIA', 'ccp', 'ce', 'cgg', 'ch', 'chm', 'chr', 'ckb', 'cmn', 'co', 'cop', 'crh', 'cs', 'csb', 'cu', 'cv', 'cy', 'da', 'dav', 'de', 'dje', 'doi', 'dsb', 'dua', 'dv', 'dyo', 'dz', 'ebu', 'ee', 'el', 'en', 'eo', 'es', 'et', 'eu', 'ewo', 'fa', 'fat', 'ff', 'fi', 'fil', 'fj', 'fo', 'fr', 'fur', 'fy', 'ga', 'gbm', 'gd', 'gez', 'gl', 'glk', 'gn', 'grc', 'gsw', 'gu', 'guz', 'gv', 'ha', 'hak', 'haw', 'he', 'hi', 'hif', 'hil', 'hne', 'ho', 'hr', 'hsb', 'ht', 'hu', 'hy', 'hz', 'ia', 'id', 'ie', 'ig', 'ii', 'ik', 'ilo', 'io', 'is', 'it', 'iu', 'iw', 'ja', 'jgo', 'jmc', 'jv', 'ka', 'kaa', 'kab', 'kam', 'kde', 'kea', 'kg', 'khb', 'khq', 'ki', 'kj', 'kk', 'kkj', 'kl', 'kln', 'km', 'kn', 'ko', 'kok', 'kr', 'ks', 'ks_Arab', 'ks_Deva', 'ksb', 'ksf', 'ksh', 'ku', 'kum', 'kv', 'kw', 'kwm', 'ky', 'la', 'lag', 'lah', 'lb', 'lez', 'lg', 'li', 'lij', 'lkt', 'ln', 'lo', 'lrc', 'lt', 'lu', 'luo', 'luy', 'lv', 'lzh', 'mag', 'mai', 'mas', 'mer', 'mfe', 'mg', 'mgh', 'mgo', 'mh', 'mhr', 'mi', 'miq', 'mjw', 'mk', 'ml', 'mn', 'mni', 'mnw', 'mo', 'mos', 'mr', 'ms', 'mt', 'mua', 'my', 'mzn', 'na', 'nan', 'naq', 'nb', 'nd', 'nds', 'ne', 'new', 'ng', 'nhn', 'niu', 'nl', 'nmg', 'nn', 'nnh', 'no', 'nqo', 'nr', 'nso', 'nus', 'nv', 'ny', 'nyn', 'oc', 'om', 'or', 'os', 'osa', 'ota', 'pa', 'pap', 'pl', 'prg', 'ps', 'pt', 'qu', 'quh', 'quz', 'raj', 'rif', 'rm', 'rn', 'ro', 'rof', 'ru', 'rw', 'rwk', 'sa', 'sah', 'saq', 'sat', 'sbp', 'sc', 'sco', 'sd', 'sd_Arab', 'sd_Deva', 'se', 'seh', 'sel', 'ses', 'sg', 'sgs', 'sh', 'shi', 'shn', 'shs', 'si', 'sid', 'sk', 'sl', 'sm', 'sma', 'smj', 'smn', 'sms', 'sn', 'so', 'sq', 'sr', 'sr_Cyrl', 'sr_Latn', 'ss', 'ssy', 'st', 'su', 'sv', 'sw', 'syc', 'syr', 'szl', 'ta', 'tcy', 'te', 'teo', 'tet', 'tg', 'th', 'the', 'ti', 'tig', 'tk', 'tl', 'tn', 'to', 'tok', 'tpi', 'tr', 'ts', 'tt', 'tt_Cyrl', 'tt_Latn', 'tw', 'twq', 'txg', 'ty', 'tyv', 'tzm', 'udm', 'ug', 'uk', 'unm', 'ur', 'uz', 'vai', 've', 'vi', 'vo', 'vot', 'vun', 'wa', 'wae', 'wal', 'wen', 'wo', 'wuu', 'xal', 'xh', 'xog', 'xzh', 'yap', 'yav', 'yi', 'yo', 'yue', 'yuw', 'za', 'zgh', 'zh', 'zh_Hans', 'zh_Hans_CN', 'zh_Hans_SG', 'zh_Hant', 'zh_Hant_HK', 'zh_Hant_MO', 'zh_Hant_TW', 'zu']
+    ['aa', 'ab', 'af', 'agq', 'agr', 'ak', 'am', 'an', 'anp', 'ar', 'as', 'asa', 'ast', 'av', 'ay', 'ayc', 'ayr', 'az', 'ba', 'bas', 'be', 'bem', 'ber', 'bez', 'bg', 'bhb', 'bho', 'bi', 'bih', 'bin', 'bm', 'bn', 'bo', 'br', 'brx', 'bs', 'bua', 'byn', 'ca', 'ca_ES_VALENCIA', 'ccp', 'ce', 'cgg', 'ch', 'chm', 'chr', 'ckb', 'cmn', 'co', 'cop', 'crh', 'cs', 'csb', 'cu', 'cv', 'cy', 'da', 'dav', 'de', 'dje', 'doi', 'dsb', 'dua', 'dv', 'dyo', 'dz', 'ebu', 'ee', 'el', 'en', 'eo', 'es', 'et', 'eu', 'ewo', 'fa', 'fat', 'ff', 'fi', 'fil', 'fj', 'fo', 'fr', 'fur', 'fy', 'ga', 'gbm', 'gd', 'gez', 'gl', 'glk', 'gn', 'grc', 'gsw', 'gu', 'guz', 'gv', 'ha', 'hak', 'haw', 'he', 'hi', 'hif', 'hil', 'hne', 'ho', 'hr', 'hsb', 'ht', 'hu', 'hy', 'hz', 'ia', 'id', 'ie', 'ig', 'ii', 'ik', 'ilo', 'io', 'is', 'it', 'iu', 'iw', 'ja', 'jgo', 'jmc', 'jv', 'ka', 'kaa', 'kab', 'kam', 'kde', 'kea', 'kg', 'khb', 'khq', 'ki', 'kj', 'kk', 'kkj', 'kl', 'kln', 'km', 'kn', 'ko', 'kok', 'kr', 'ks', 'ks_Arab', 'ks_Deva', 'ksb', 'ksf', 'ksh', 'ku', 'kum', 'kv', 'kw', 'kwm', 'ky', 'la', 'lag', 'lah', 'lb', 'lez', 'lg', 'li', 'lij', 'lkt', 'ln', 'lo', 'lrc', 'lt', 'lu', 'luo', 'luy', 'lv', 'lzh', 'mag', 'mai', 'mas', 'mdf', 'mer', 'mfe', 'mg', 'mgh', 'mgo', 'mh', 'mhr', 'mi', 'miq', 'mjw', 'mk', 'ml', 'mn', 'mni', 'mnw', 'mo', 'mos', 'mr', 'ms', 'mt', 'mua', 'my', 'mzn', 'na', 'nan', 'naq', 'nb', 'nd', 'nds', 'ne', 'new', 'ng', 'nhn', 'niu', 'nl', 'nmg', 'nn', 'nnh', 'no', 'nqo', 'nr', 'nso', 'nus', 'nv', 'ny', 'nyn', 'oc', 'om', 'or', 'os', 'osa', 'ota', 'pa', 'pap', 'pl', 'prg', 'ps', 'pt', 'qu', 'quh', 'quz', 'raj', 'rif', 'rm', 'rn', 'ro', 'rof', 'ru', 'rw', 'rwk', 'sa', 'sah', 'saq', 'sat', 'sbp', 'sc', 'sco', 'sd', 'sd_Arab', 'sd_Deva', 'se', 'seh', 'sel', 'ses', 'sg', 'sgs', 'sh', 'shi', 'shn', 'shs', 'si', 'sid', 'sk', 'sl', 'sm', 'sma', 'smj', 'smn', 'sms', 'sn', 'so', 'sq', 'sr', 'sr_Cyrl', 'sr_Latn', 'ss', 'ssy', 'st', 'su', 'sv', 'sw', 'syc', 'syr', 'szl', 'ta', 'tcy', 'te', 'teo', 'tet', 'tg', 'th', 'the', 'ti', 'tig', 'tk', 'tl', 'tn', 'to', 'tok', 'tpi', 'tr', 'ts', 'tt', 'tt_Cyrl', 'tt_Latn', 'tw', 'twq', 'txg', 'ty', 'tyv', 'tzm', 'udm', 'ug', 'uk', 'unm', 'ur', 'uz', 'vai', 've', 'vi', 'vo', 'vot', 'vun', 'wa', 'wae', 'wal', 'wen', 'wo', 'wuu', 'xal', 'xh', 'xog', 'xzh', 'yap', 'yav', 'yi', 'yo', 'yue', 'yuw', 'za', 'zgh', 'zh', 'zh_Hans', 'zh_Hans_CN', 'zh_Hans_SG', 'zh_Hant', 'zh_Hant_HK', 'zh_Hant_MO', 'zh_Hant_TW', 'zu']
     >>> print(list_all_locales())    # doctest: +NORMALIZE_WHITESPACE
-    ['aa_DJ.UTF-8', 'aa_ER.UTF-8', 'aa_ET.UTF-8', 'ab_GE.UTF-8', 'af_ZA.UTF-8', 'agr_PE.UTF-8', 'ak_GH.UTF-8', 'am_ET.UTF-8', 'an_ES.UTF-8', 'anp_IN.UTF-8', 'ar_AE.UTF-8', 'ar_BH.UTF-8', 'ar_DZ.UTF-8', 'ar_EG.UTF-8', 'ar_IN.UTF-8', 'ar_IQ.UTF-8', 'ar_JO.UTF-8', 'ar_KW.UTF-8', 'ar_LB.UTF-8', 'ar_LY.UTF-8', 'ar_MA.UTF-8', 'ar_OM.UTF-8', 'ar_QA.UTF-8', 'ar_SA.UTF-8', 'ar_SD.UTF-8', 'ar_SS.UTF-8', 'ar_SY.UTF-8', 'ar_TN.UTF-8', 'ar_YE.UTF-8', 'as_IN.UTF-8', 'ast_ES.UTF-8', 'ayc_PE.UTF-8', 'az_AZ.UTF-8', 'az_IR.UTF-8', 'be_BY.UTF-8', 'be_BY.UTF-8@latin', 'bem_ZM.UTF-8', 'ber_DZ.UTF-8', 'ber_MA.UTF-8', 'bg_BG.UTF-8', 'bhb_IN.UTF-8', 'bho_IN.UTF-8', 'bho_NP.UTF-8', 'bi_VU.UTF-8', 'bn_BD.UTF-8', 'bn_IN.UTF-8', 'bo_CN.UTF-8', 'bo_IN.UTF-8', 'br_FR.UTF-8', 'brx_IN.UTF-8', 'bs_BA.UTF-8', 'byn_ER.UTF-8', 'ca_AD.UTF-8', 'ca_ES.UTF-8', 'ca_ES.UTF-8@valencia', 'ca_FR.UTF-8', 'ca_IT.UTF-8', 'ce_RU.UTF-8', 'chr_US.UTF-8', 'ckb_IQ.UTF-8', 'cmn_TW.UTF-8', 'crh_RU.UTF-8', 'crh_UA.UTF-8', 'cs_CZ.UTF-8', 'csb_PL.UTF-8', 'cv_RU.UTF-8', 'cy_GB.UTF-8', 'da_DK.UTF-8', 'de_AT.UTF-8', 'de_BE.UTF-8', 'de_CH.UTF-8', 'de_DE.UTF-8', 'de_IT.UTF-8', 'de_LI.UTF-8', 'de_LU.UTF-8', 'doi_IN.UTF-8', 'dsb_DE.UTF-8', 'dv_MV.UTF-8', 'dz_BT.UTF-8', 'el_CY.UTF-8', 'el_GR.UTF-8', 'en_AG.UTF-8', 'en_AU.UTF-8', 'en_BW.UTF-8', 'en_CA.UTF-8', 'en_DK.UTF-8', 'en_GB.UTF-8', 'en_HK.UTF-8', 'en_IE.UTF-8', 'en_IL.UTF-8', 'en_IN.UTF-8', 'en_NG.UTF-8', 'en_NZ.UTF-8', 'en_PH.UTF-8', 'en_SC.UTF-8', 'en_SG.UTF-8', 'en_US.UTF-8', 'en_ZA.UTF-8', 'en_ZM.UTF-8', 'en_ZW.UTF-8', 'eo.UTF-8', 'es_AR.UTF-8', 'es_BO.UTF-8', 'es_CL.UTF-8', 'es_CO.UTF-8', 'es_CR.UTF-8', 'es_CU.UTF-8', 'es_DO.UTF-8', 'es_EC.UTF-8', 'es_ES.UTF-8', 'es_GT.UTF-8', 'es_HN.UTF-8', 'es_MX.UTF-8', 'es_NI.UTF-8', 'es_PA.UTF-8', 'es_PE.UTF-8', 'es_PR.UTF-8', 'es_PY.UTF-8', 'es_SV.UTF-8', 'es_US.UTF-8', 'es_UY.UTF-8', 'es_VE.UTF-8', 'et_EE.UTF-8', 'eu_ES.UTF-8', 'fa_IR.UTF-8', 'ff_SN.UTF-8', 'fi_FI.UTF-8', 'fil_PH.UTF-8', 'fo_FO.UTF-8', 'fr_BE.UTF-8', 'fr_CA.UTF-8', 'fr_CH.UTF-8', 'fr_FR.UTF-8', 'fr_HT.UTF-8', 'fr_LU.UTF-8', 'fur_IT.UTF-8', 'fy_DE.UTF-8', 'fy_NL.UTF-8', 'ga_IE.UTF-8', 'gbm_IN.UTF-8', 'gd_GB.UTF-8', 'gez_ER.UTF-8', 'gez_ER.UTF-8@abegede', 'gez_ET.UTF-8', 'gez_ET.UTF-8@abegede', 'gl_ES.UTF-8', 'glk_IR.UTF-8', 'gu_IN.UTF-8', 'gv_GB.UTF-8', 'ha_NG.UTF-8', 'hak_TW.UTF-8', 'he_IL.UTF-8', 'hi_IN.UTF-8', 'hif_FJ.UTF-8', 'hne_IN.UTF-8', 'hr_HR.UTF-8', 'hsb_DE.UTF-8', 'ht_HT.UTF-8', 'hu_HU.UTF-8', 'hy_AM.UTF-8', 'ia_FR.UTF-8', 'id_ID.UTF-8', 'ig_NG.UTF-8', 'ik_CA.UTF-8', 'ilo_PH.UTF-8', 'is_IS.UTF-8', 'it_CH.UTF-8', 'it_IT.UTF-8', 'iu_CA.UTF-8', 'iw_IL.UTF-8', 'ja_JP.UTF-8', 'ka_GE.UTF-8', 'kab_DZ.UTF-8', 'kk_KZ.UTF-8', 'kl_GL.UTF-8', 'km_KH.UTF-8', 'kn_IN.UTF-8', 'ko_KR.UTF-8', 'kok_IN.UTF-8', 'ks_IN.UTF-8', 'ks_IN.UTF-8@devanagari', 'ku_TR.UTF-8', 'kv_RU.UTF-8', 'kw_GB.UTF-8', 'ky_KG.UTF-8', 'lb_LU.UTF-8', 'lg_UG.UTF-8', 'li_BE.UTF-8', 'li_NL.UTF-8', 'lij_IT.UTF-8', 'ln_CD.UTF-8', 'lo_LA.UTF-8', 'lt_LT.UTF-8', 'lv_LV.UTF-8', 'lzh_TW.UTF-8', 'mag_IN.UTF-8', 'mai_IN.UTF-8', 'mai_NP.UTF-8', 'mfe_MU.UTF-8', 'mg_MG.UTF-8', 'mhr_RU.UTF-8', 'mi_NZ.UTF-8', 'miq_NI.UTF-8', 'mjw_IN.UTF-8', 'mk_MK.UTF-8', 'ml_IN.UTF-8', 'mn_MN.UTF-8', 'mni_IN.UTF-8', 'mnw_MM.UTF-8', 'mr_IN.UTF-8', 'ms_MY.UTF-8', 'mt_MT.UTF-8', 'my_MM.UTF-8', 'nan_TW.UTF-8', 'nan_TW.UTF-8@latin', 'nb_NO.UTF-8', 'nds_DE.UTF-8', 'nds_NL.UTF-8', 'ne_NP.UTF-8', 'nhn_MX.UTF-8', 'niu_NU.UTF-8', 'niu_NZ.UTF-8', 'nl_AW.UTF-8', 'nl_BE.UTF-8', 'nl_NL.UTF-8', 'nn_NO.UTF-8', 'no_NO.UTF-8', 'nr_ZA.UTF-8', 'nso_ZA.UTF-8', 'oc_FR.UTF-8', 'om_ET.UTF-8', 'om_KE.UTF-8', 'or_IN.UTF-8', 'os_RU.UTF-8', 'pa_IN.UTF-8', 'pa_PK.UTF-8', 'pap_AN.UTF-8', 'pap_AW.UTF-8', 'pap_CW.UTF-8', 'pl_PL.UTF-8', 'ps_AF.UTF-8', 'pt_BR.UTF-8', 'pt_PT.UTF-8', 'quz_PE.UTF-8', 'raj_IN.UTF-8', 'rif_MA.UTF-8', 'ro_RO.UTF-8', 'ru_RU.UTF-8', 'ru_UA.UTF-8', 'rw_RW.UTF-8', 'sa_IN.UTF-8', 'sah_RU.UTF-8', 'sat_IN.UTF-8', 'sc_IT.UTF-8', 'sd_IN.UTF-8', 'sd_IN.UTF-8@devanagari', 'se_NO.UTF-8', 'sgs_LT.UTF-8', 'shn_MM.UTF-8', 'shs_CA.UTF-8', 'si_LK.UTF-8', 'sid_ET.UTF-8', 'sk_SK.UTF-8', 'sl_SI.UTF-8', 'sm_WS.UTF-8', 'so_DJ.UTF-8', 'so_ET.UTF-8', 'so_KE.UTF-8', 'so_SO.UTF-8', 'sq_AL.UTF-8', 'sq_MK.UTF-8', 'sr_ME.UTF-8', 'sr_ME.UTF-8@latin', 'sr_RS.UTF-8', 'sr_RS.UTF-8@latin', 'ss_ZA.UTF-8', 'ssy_ER.UTF-8', 'st_ZA.UTF-8', 'sv_FI.UTF-8', 'sv_SE.UTF-8', 'sw_KE.UTF-8', 'sw_TZ.UTF-8', 'syr.UTF-8', 'szl_PL.UTF-8', 'ta_IN.UTF-8', 'ta_LK.UTF-8', 'ta_SG.UTF-8', 'tcy_IN.UTF-8', 'te_IN.UTF-8', 'tg_TJ.UTF-8', 'th_TH.UTF-8', 'the_NP.UTF-8', 'ti_ER.UTF-8', 'ti_ET.UTF-8', 'tig_ER.UTF-8', 'tk_TM.UTF-8', 'tl_PH.UTF-8', 'tn_BW.UTF-8', 'tn_ZA.UTF-8', 'to_TO.UTF-8', 'tok.UTF-8', 'tpi_PG.UTF-8', 'tr_CY.UTF-8', 'tr_TR.UTF-8', 'ts_ZA.UTF-8', 'tt_RU.UTF-8', 'tt_RU.UTF-8@iqtelif', 'ug_CN.UTF-8', 'uk_UA.UTF-8', 'unm_US.UTF-8', 'ur_IN.UTF-8', 'ur_PK.UTF-8', 'uz_UZ.UTF-8', 'uz_UZ.UTF-8@cyrillic', 've_ZA.UTF-8', 'vi_VN.UTF-8', 'wa_BE.UTF-8', 'wae_CH.UTF-8', 'wal_ET.UTF-8', 'wo_SN.UTF-8', 'xh_ZA.UTF-8', 'yi_US.UTF-8', 'yo_NG.UTF-8', 'yue_HK.UTF-8', 'yuw_PG.UTF-8', 'zh_CN.UTF-8', 'zh_HK.UTF-8', 'zh_MO.UTF-8', 'zh_SG.UTF-8', 'zh_TW.UTF-8', 'zu_ZA.UTF-8']
+    ['aa_DJ.UTF-8', 'aa_ER.UTF-8', 'aa_ET.UTF-8', 'ab_GE.UTF-8', 'af_ZA.UTF-8', 'agr_PE.UTF-8', 'ak_GH.UTF-8', 'am_ET.UTF-8', 'an_ES.UTF-8', 'anp_IN.UTF-8', 'ar_AE.UTF-8', 'ar_BH.UTF-8', 'ar_DZ.UTF-8', 'ar_EG.UTF-8', 'ar_IN.UTF-8', 'ar_IQ.UTF-8', 'ar_JO.UTF-8', 'ar_KW.UTF-8', 'ar_LB.UTF-8', 'ar_LY.UTF-8', 'ar_MA.UTF-8', 'ar_OM.UTF-8', 'ar_QA.UTF-8', 'ar_SA.UTF-8', 'ar_SD.UTF-8', 'ar_SS.UTF-8', 'ar_SY.UTF-8', 'ar_TN.UTF-8', 'ar_YE.UTF-8', 'as_IN.UTF-8', 'ast_ES.UTF-8', 'ayc_PE.UTF-8', 'az_AZ.UTF-8', 'az_IR.UTF-8', 'be_BY.UTF-8', 'be_BY.UTF-8@latin', 'bem_ZM.UTF-8', 'ber_DZ.UTF-8', 'ber_MA.UTF-8', 'bg_BG.UTF-8', 'bhb_IN.UTF-8', 'bho_IN.UTF-8', 'bho_NP.UTF-8', 'bi_VU.UTF-8', 'bn_BD.UTF-8', 'bn_IN.UTF-8', 'bo_CN.UTF-8', 'bo_IN.UTF-8', 'br_FR.UTF-8', 'brx_IN.UTF-8', 'bs_BA.UTF-8', 'byn_ER.UTF-8', 'ca_AD.UTF-8', 'ca_ES.UTF-8', 'ca_ES.UTF-8@valencia', 'ca_FR.UTF-8', 'ca_IT.UTF-8', 'ce_RU.UTF-8', 'chr_US.UTF-8', 'ckb_IQ.UTF-8', 'cmn_TW.UTF-8', 'crh_RU.UTF-8', 'crh_UA.UTF-8', 'cs_CZ.UTF-8', 'csb_PL.UTF-8', 'cv_RU.UTF-8', 'cy_GB.UTF-8', 'da_DK.UTF-8', 'de_AT.UTF-8', 'de_BE.UTF-8', 'de_CH.UTF-8', 'de_DE.UTF-8', 'de_IT.UTF-8', 'de_LI.UTF-8', 'de_LU.UTF-8', 'doi_IN.UTF-8', 'dsb_DE.UTF-8', 'dv_MV.UTF-8', 'dz_BT.UTF-8', 'el_CY.UTF-8', 'el_GR.UTF-8', 'en_AG.UTF-8', 'en_AU.UTF-8', 'en_BW.UTF-8', 'en_CA.UTF-8', 'en_DK.UTF-8', 'en_GB.UTF-8', 'en_HK.UTF-8', 'en_IE.UTF-8', 'en_IL.UTF-8', 'en_IN.UTF-8', 'en_NG.UTF-8', 'en_NZ.UTF-8', 'en_PH.UTF-8', 'en_SC.UTF-8', 'en_SG.UTF-8', 'en_US.UTF-8', 'en_ZA.UTF-8', 'en_ZM.UTF-8', 'en_ZW.UTF-8', 'eo.UTF-8', 'es_AR.UTF-8', 'es_BO.UTF-8', 'es_CL.UTF-8', 'es_CO.UTF-8', 'es_CR.UTF-8', 'es_CU.UTF-8', 'es_DO.UTF-8', 'es_EC.UTF-8', 'es_ES.UTF-8', 'es_GT.UTF-8', 'es_HN.UTF-8', 'es_MX.UTF-8', 'es_NI.UTF-8', 'es_PA.UTF-8', 'es_PE.UTF-8', 'es_PR.UTF-8', 'es_PY.UTF-8', 'es_SV.UTF-8', 'es_US.UTF-8', 'es_UY.UTF-8', 'es_VE.UTF-8', 'et_EE.UTF-8', 'eu_ES.UTF-8', 'fa_IR.UTF-8', 'ff_SN.UTF-8', 'fi_FI.UTF-8', 'fil_PH.UTF-8', 'fo_FO.UTF-8', 'fr_BE.UTF-8', 'fr_CA.UTF-8', 'fr_CH.UTF-8', 'fr_FR.UTF-8', 'fr_HT.UTF-8', 'fr_LU.UTF-8', 'fur_IT.UTF-8', 'fy_DE.UTF-8', 'fy_NL.UTF-8', 'ga_IE.UTF-8', 'gbm_IN.UTF-8', 'gd_GB.UTF-8', 'gez_ER.UTF-8', 'gez_ER.UTF-8@abegede', 'gez_ET.UTF-8', 'gez_ET.UTF-8@abegede', 'gl_ES.UTF-8', 'glk_IR.UTF-8', 'gu_IN.UTF-8', 'gv_GB.UTF-8', 'ha_NG.UTF-8', 'hak_TW.UTF-8', 'he_IL.UTF-8', 'hi_IN.UTF-8', 'hif_FJ.UTF-8', 'hne_IN.UTF-8', 'hr_HR.UTF-8', 'hsb_DE.UTF-8', 'ht_HT.UTF-8', 'hu_HU.UTF-8', 'hy_AM.UTF-8', 'ia_FR.UTF-8', 'id_ID.UTF-8', 'ig_NG.UTF-8', 'ik_CA.UTF-8', 'ilo_PH.UTF-8', 'is_IS.UTF-8', 'it_CH.UTF-8', 'it_IT.UTF-8', 'iu_CA.UTF-8', 'iw_IL.UTF-8', 'ja_JP.UTF-8', 'ka_GE.UTF-8', 'kab_DZ.UTF-8', 'kk_KZ.UTF-8', 'kl_GL.UTF-8', 'km_KH.UTF-8', 'kn_IN.UTF-8', 'ko_KR.UTF-8', 'kok_IN.UTF-8', 'ks_IN.UTF-8', 'ks_IN.UTF-8@devanagari', 'ku_TR.UTF-8', 'kv_RU.UTF-8', 'kw_GB.UTF-8', 'ky_KG.UTF-8', 'lb_LU.UTF-8', 'lg_UG.UTF-8', 'li_BE.UTF-8', 'li_NL.UTF-8', 'lij_IT.UTF-8', 'ln_CD.UTF-8', 'lo_LA.UTF-8', 'lt_LT.UTF-8', 'lv_LV.UTF-8', 'lzh_TW.UTF-8', 'mag_IN.UTF-8', 'mai_IN.UTF-8', 'mai_NP.UTF-8', 'mdf_RU.UTF-8', 'mfe_MU.UTF-8', 'mg_MG.UTF-8', 'mhr_RU.UTF-8', 'mi_NZ.UTF-8', 'miq_NI.UTF-8', 'mjw_IN.UTF-8', 'mk_MK.UTF-8', 'ml_IN.UTF-8', 'mn_MN.UTF-8', 'mni_IN.UTF-8', 'mnw_MM.UTF-8', 'mr_IN.UTF-8', 'ms_MY.UTF-8', 'mt_MT.UTF-8', 'my_MM.UTF-8', 'nan_TW.UTF-8', 'nan_TW.UTF-8@latin', 'nb_NO.UTF-8', 'nds_DE.UTF-8', 'nds_NL.UTF-8', 'ne_NP.UTF-8', 'nhn_MX.UTF-8', 'niu_NU.UTF-8', 'niu_NZ.UTF-8', 'nl_AW.UTF-8', 'nl_BE.UTF-8', 'nl_NL.UTF-8', 'nn_NO.UTF-8', 'no_NO.UTF-8', 'nr_ZA.UTF-8', 'nso_ZA.UTF-8', 'oc_FR.UTF-8', 'om_ET.UTF-8', 'om_KE.UTF-8', 'or_IN.UTF-8', 'os_RU.UTF-8', 'pa_IN.UTF-8', 'pa_PK.UTF-8', 'pap_AN.UTF-8', 'pap_AW.UTF-8', 'pap_CW.UTF-8', 'pl_PL.UTF-8', 'ps_AF.UTF-8', 'pt_BR.UTF-8', 'pt_PT.UTF-8', 'quz_PE.UTF-8', 'raj_IN.UTF-8', 'rif_MA.UTF-8', 'ro_RO.UTF-8', 'ru_RU.UTF-8', 'ru_UA.UTF-8', 'rw_RW.UTF-8', 'sa_IN.UTF-8', 'sah_RU.UTF-8', 'sat_IN.UTF-8', 'sc_IT.UTF-8', 'sd_IN.UTF-8', 'sd_IN.UTF-8@devanagari', 'se_NO.UTF-8', 'sgs_LT.UTF-8', 'shn_MM.UTF-8', 'shs_CA.UTF-8', 'si_LK.UTF-8', 'sid_ET.UTF-8', 'sk_SK.UTF-8', 'sl_SI.UTF-8', 'sm_WS.UTF-8', 'so_DJ.UTF-8', 'so_ET.UTF-8', 'so_KE.UTF-8', 'so_SO.UTF-8', 'sq_AL.UTF-8', 'sq_MK.UTF-8', 'sr_ME.UTF-8', 'sr_ME.UTF-8@latin', 'sr_RS.UTF-8', 'sr_RS.UTF-8@latin', 'ss_ZA.UTF-8', 'ssy_ER.UTF-8', 'st_ZA.UTF-8', 'sv_FI.UTF-8', 'sv_SE.UTF-8', 'sw_KE.UTF-8', 'sw_TZ.UTF-8', 'syr.UTF-8', 'szl_PL.UTF-8', 'ta_IN.UTF-8', 'ta_LK.UTF-8', 'ta_SG.UTF-8', 'tcy_IN.UTF-8', 'te_IN.UTF-8', 'tg_TJ.UTF-8', 'th_TH.UTF-8', 'the_NP.UTF-8', 'ti_ER.UTF-8', 'ti_ET.UTF-8', 'tig_ER.UTF-8', 'tk_TM.UTF-8', 'tl_PH.UTF-8', 'tn_BW.UTF-8', 'tn_ZA.UTF-8', 'to_TO.UTF-8', 'tok.UTF-8', 'tpi_PG.UTF-8', 'tr_CY.UTF-8', 'tr_TR.UTF-8', 'ts_ZA.UTF-8', 'tt_RU.UTF-8', 'tt_RU.UTF-8@iqtelif', 'ug_CN.UTF-8', 'uk_UA.UTF-8', 'unm_US.UTF-8', 'ur_IN.UTF-8', 'ur_PK.UTF-8', 'uz_UZ.UTF-8', 'uz_UZ.UTF-8@cyrillic', 've_ZA.UTF-8', 'vi_VN.UTF-8', 'wa_BE.UTF-8', 'wae_CH.UTF-8', 'wal_ET.UTF-8', 'wo_SN.UTF-8', 'xh_ZA.UTF-8', 'yi_US.UTF-8', 'yo_NG.UTF-8', 'yue_HK.UTF-8', 'yuw_PG.UTF-8', 'zh_CN.UTF-8', 'zh_HK.UTF-8', 'zh_MO.UTF-8', 'zh_SG.UTF-8', 'zh_TW.UTF-8', 'zu_ZA.UTF-8']
     >>> print(list_all_keyboards())    # doctest: +NORMALIZE_WHITESPACE
     ['ad', 'af', 'af(fa-olpc)', 'af(ps)', 'af(ps-olpc)', 'af(uz)', 'af(uz-olpc)', 'al', 'am', 'am(eastern)', 'am(eastern-alt)', 'am(phonetic)', 'am(phonetic-alt)', 'am(western)', 'ara', 'ara(azerty)', 'ara(azerty_digits)', 'ara(buckwalter)', 'ara(digits)', 'ara(qwerty)', 'ara(qwerty_digits)', 'at(nodeadkeys)', 'az', 'az(cyrillic)', 'ba', 'bd', 'bd(probhat)', 'be', 'be(oss)', 'bg', 'bg(bas_phonetic)', 'bg(phonetic)', 'br', 'brai', 'brai(left_hand)', 'brai(right_hand)', 'bt', 'by', 'by(legacy)', 'ca', 'ca(eng)', 'ca(ike)', 'ca(multi)', 'ca(multi-2gr)', 'ca(shs)', 'ch', 'ch(fr)', 'cn', 'cn(tib)', 'cn(tib_asciinum)', 'cn(ug)', 'cz', 'cz(ucw)', 'de', 'de(deadacute)', 'de(nodeadkeys)', 'de(ru)', 'dk', 'ee', 'es', 'es(ast)', 'es(cat)', 'et', 'fi', 'fi(classic)', 'fi(nodeadkeys)', 'fo', 'fr', 'fr(geo)', 'fr(latin9)', 'fr(oss)', 'gb', 'ge', 'ge(os)', 'gr', 'gr(extended)', 'gr(nodeadkeys)', 'gr(polytonic)', 'gr(simple)', 'hr', 'hu', 'ie', 'ie(CloGaelach)', 'ie(ogam)', 'il', 'il(biblical)', 'il(lyx)', 'il(phonetic)', 'in', 'in(ben)', 'in(ben_baishakhi)', 'in(ben_bornona)', 'in(ben_gitanjali)', 'in(ben_inscript)', 'in(ben_probhat)', 'in(bolnagri)', 'in(deva)', 'in(eng)', 'in(guj)', 'in(guru)', 'in(hin-kagapa)', 'in(hin-wx)', 'in(jhelum)', 'in(kan)', 'in(kan-kagapa)', 'in(mal)', 'in(mal_enhanced)', 'in(mal_lalitha)', 'in(mar-kagapa)', 'in(ori)', 'in(san-kagapa)', 'in(tam)', 'in(tam_tamilnet)', 'in(tam_tamilnet_TAB)', 'in(tam_tamilnet_TSCII)', 'in(tam_tamilnet_with_tam_nums)', 'in(tel)', 'in(tel-kagapa)', 'in(urd-phonetic)', 'in(urd-phonetic3)', 'in(urd-winkeys)', 'iq', 'ir', 'ir(pes_keypad)', 'it', 'jp', 'jp(kana)', 'jp(mac)', 'ke', 'kg', 'kg(phonetic)', 'kh', 'kr', 'kz', 'kz(kazrus)', 'kz(ruskaz)', 'la', 'la(stea)', 'latam', 'lk', 'lk(tam_TAB)', 'lk(tam_unicode)', 'lt', 'lv', 'ma', 'ma(french)', 'ma(tifinagh)', 'ma(tifinagh-alt)', 'ma(tifinagh-alt-phonetic)', 'ma(tifinagh-extended)', 'ma(tifinagh-extended-phonetic)', 'ma(tifinagh-phonetic)', 'me', 'me(cyrillic)', 'me(cyrillicalternatequotes)', 'me(cyrillicyz)', 'mk', 'mk(nodeadkeys)', 'mm', 'mn', 'mt', 'mt(us)', 'mv', 'ng', 'ng(hausa)', 'ng(igbo)', 'ng(yoruba)', 'nl', 'no', 'np', 'ph', 'ph(capewell-dvorak-bay)', 'ph(capewell-qwerf2k6-bay)', 'ph(colemak-bay)', 'ph(dvorak-bay)', 'ph(qwerty-bay)', 'pk', 'pk(ara)', 'pk(snd)', 'pk(urd-crulp)', 'pk(urd-nla)', 'pl', 'pl(ru_phonetic_dvorak)', 'pt', 'ro', 'rs', 'rs(alternatequotes)', 'rs(latin)', 'rs(rue)', 'rs(yz)', 'ru', 'ru(bak)', 'ru(chm)', 'ru(cv)', 'ru(dos)', 'ru(kom)', 'ru(legacy)', 'ru(mac)', 'ru(os_legacy)', 'ru(os_winkeys)', 'ru(phonetic)', 'ru(phonetic_winkeys)', 'ru(sah)', 'ru(srp)', 'ru(tt)', 'ru(typewriter)', 'ru(typewriter-legacy)', 'ru(udm)', 'ru(xal)', 'se', 'se(nodeadkeys)', 'se(rus)', 'se(rus_nodeadkeys)', 'se(swl)', 'si', 'sk', 'sn', 'sy', 'sy(syc)', 'sy(syc_phonetic)', 'th', 'th(pat)', 'th(tis)', 'tj', 'tj(legacy)', 'tm', 'tr', 'tr(crh)', 'tr(ku)', 'tz', 'ua', 'ua(homophonic)', 'ua(legacy)', 'ua(phonetic)', 'ua(rstu)', 'ua(rstu_ru)', 'ua(typewriter)', 'ua(winkeys)', 'us', 'us(altgr-intl)', 'us(chr)', 'us(euro)', 'us(intl)', 'us(rus)', 'uz', 'uz(latin)', 'vn', 'za']
     >>> print(list_all_territories())    # doctest: +NORMALIZE_WHITESPACE
     ['001', '002', '019', '142', '150', '419', 'AD', 'AE', 'AF', 'AG', 'AI', 'AL', 'AM', 'AN', 'AO', 'AQ', 'AR', 'AS', 'AT', 'AU', 'AW', 'AX', 'AZ', 'BA', 'BB', 'BD', 'BE', 'BF', 'BG', 'BH', 'BI', 'BJ', 'BL', 'BM', 'BN', 'BO', 'BQ', 'BR', 'BS', 'BT', 'BW', 'BY', 'BZ', 'CA', 'CC', 'CD', 'CF', 'CG', 'CH', 'CI', 'CK', 'CL', 'CM', 'CN', 'CO', 'CR', 'CU', 'CV', 'CW', 'CX', 'CY', 'CZ', 'DE', 'DG', 'DJ', 'DK', 'DM', 'DO', 'DZ', 'EA', 'EC', 'EE', 'EG', 'EH', 'ER', 'ES', 'ET', 'EU', 'EZ', 'FI', 'FJ', 'FK', 'FM', 'FO', 'FR', 'GA', 'GB', 'GD', 'GE', 'GF', 'GG', 'GH', 'GI', 'GL', 'GM', 'GN', 'GP', 'GQ', 'GR', 'GT', 'GU', 'GW', 'GY', 'HK', 'HN', 'HR', 'HT', 'HU', 'IC', 'ID', 'IE', 'IL', 'IM', 'IN', 'IO', 'IQ', 'IR', 'IS', 'IT', 'JE', 'JM', 'JO', 'JP', 'KE', 'KG', 'KH', 'KI', 'KM', 'KN', 'KP', 'KR', 'KW', 'KY', 'KZ', 'LA', 'LB', 'LC', 'LI', 'LK', 'LR', 'LS', 'LT', 'LU', 'LV', 'LY', 'MA', 'MC', 'MD', 'ME', 'MF', 'MG', 'MH', 'MK', 'ML', 'MM', 'MN', 'MO', 'MP', 'MQ', 'MR', 'MS', 'MT', 'MU', 'MV', 'MW', 'MX', 'MY', 'MZ', 'NA', 'NC', 'NE', 'NF', 'NG', 'NI', 'NL', 'NO', 'NP', 'NR', 'NU', 'NZ', 'OM', 'PA', 'PE', 'PF', 'PG', 'PH', 'PK', 'PL', 'PM', 'PN', 'PR', 'PS', 'PT', 'PW', 'PY', 'QA', 'RE', 'RO', 'RS', 'RU', 'RW', 'SA', 'SB', 'SC', 'SD', 'SE', 'SG', 'SH', 'SI', 'SJ', 'SK', 'SL', 'SM', 'SN', 'SO', 'SR', 'SS', 'ST', 'SV', 'SX', 'SY', 'SZ', 'TC', 'TD', 'TG', 'TH', 'TJ', 'TK', 'TL', 'TM', 'TN', 'TO', 'TR', 'TT', 'TV', 'TW', 'TZ', 'UA', 'UG', 'UM', 'US', 'UY', 'UZ', 'VA', 'VC', 'VE', 'VG', 'VI', 'VN', 'VU', 'WF', 'WS', 'XK', 'YE', 'YT', 'YU', 'ZA', 'ZM', 'ZW']
     >>> print(list_all_timezones())    # doctest: +NORMALIZE_WHITESPACE
     ['Africa/Abidjan', 'Africa/Accra', 'Africa/Addis_Ababa', 'Africa/Algiers', 'Africa/Asmara', 'Africa/Bamako', 'Africa/Bangui', 'Africa/Banjul', 'Africa/Bissau', 'Africa/Blantyre', 'Africa/Brazzaville', 'Africa/Bujumbura', 'Africa/Cairo', 'Africa/Casablanca', 'Africa/Ceuta', 'Africa/Conakry', 'Africa/Dakar', 'Africa/Dar_es_Salaam', 'Africa/Djibouti', 'Africa/Douala', 'Africa/El_Aaiun', 'Africa/Freetown', 'Africa/Gaborone', 'Africa/Harare', 'Africa/Johannesburg', 'Africa/Juba', 'Africa/Kampala', 'Africa/Khartoum', 'Africa/Kigali', 'Africa/Kinshasa', 'Africa/Lagos', 'Africa/Libreville', 'Africa/Lome', 'Africa/Luanda', 'Africa/Lubumbashi', 'Africa/Lusaka', 'Africa/Malabo', 'Africa/Maputo', 'Africa/Maseru', 'Africa/Mbabane', 'Africa/Mogadishu', 'Africa/Monrovia', 'Africa/Nairobi', 'Africa/Ndjamena', 'Africa/Niamey', 'Africa/Nouakchott', 'Africa/Ouagadougou', 'Africa/Porto-Novo', 'Africa/Sao_Tome', 'Africa/Tripoli', 'Africa/Tunis', 'Africa/Windhoek', 'America/Adak', 'America/Anchorage', 'America/Anguilla', 'America/Antigua', 'America/Araguaina', 'America/Argentina/Buenos_Aires', 'America/Argentina/Catamarca', 'America/Argentina/Cordoba', 'America/Argentina/Jujuy', 'America/Argentina/La_Rioja', 'America/Argentina/Mendoza', 'America/Argentina/Rio_Gallegos', 'America/Argentina/Salta', 'America/Argentina/San_Juan', 'America/Argentina/San_Luis', 'America/Argentina/Tucuman', 'America/Argentina/Ushuaia', 'America/Aruba', 'America/Asuncion', 'America/Atikokan', 'America/Bahia', 'America/Bahia_Banderas', 'America/Barbados', 'America/Belem', 'America/Belize', 'America/Blanc-Sablon', 'America/Boa_Vista', 'America/Bogota', 'America/Boise', 'America/Cambridge_Bay', 'America/Campo_Grande', 'America/Cancun', 'America/Caracas', 'America/Cayenne', 'America/Cayman', 'America/Chicago', 'America/Chihuahua', 'America/Costa_Rica', 'America/Creston', 'America/Cuiaba', 'America/Curacao', 'America/Danmarkshavn', 'America/Dawson', 'America/Dawson_Creek', 'America/Denver', 'America/Detroit', 'America/Dominica', 'America/Edmonton', 'America/Eirunepe', 'America/El_Salvador', 'America/Fortaleza', 'America/Galapagos', 'America/Glace_Bay', 'America/Godthab', 'America/Goose_Bay', 'America/Grand_Turk', 'America/Grenada', 'America/Guadeloupe', 'America/Guatemala', 'America/Guayaquil', 'America/Guyana', 'America/Halifax', 'America/Havana', 'America/Hermosillo', 'America/Indiana/Indianapolis', 'America/Indiana/Knox', 'America/Indiana/Marengo', 'America/Indiana/Petersburg', 'America/Indiana/Tell_City', 'America/Indiana/Vevay', 'America/Indiana/Vincennes', 'America/Indiana/Winamac', 'America/Inuvik', 'America/Iqaluit', 'America/Jamaica', 'America/Juneau', 'America/Kentucky/Louisville', 'America/Kentucky/Monticello', 'America/Kralendijk', 'America/La_Paz', 'America/Lima', 'America/Los_Angeles', 'America/Lower_Princes', 'America/Maceio', 'America/Managua', 'America/Manaus', 'America/Marigot', 'America/Martinique', 'America/Matamoros', 'America/Mazatlan', 'America/Menominee', 'America/Merida', 'America/Metlakatla', 'America/Mexico_City', 'America/Miquelon', 'America/Moncton', 'America/Monterrey', 'America/Montevideo', 'America/Montreal', 'America/Montserrat', 'America/Nassau', 'America/New_York', 'America/Nipigon', 'America/Nome', 'America/Noronha', 'America/North_Dakota/Beulah', 'America/North_Dakota/Center', 'America/North_Dakota/New_Salem', 'America/Ojinaga', 'America/Panama', 'America/Pangnirtung', 'America/Paramaribo', 'America/Phoenix', 'America/Port-au-Prince', 'America/Port_of_Spain', 'America/Porto_Velho', 'America/Puerto_Rico', 'America/Rainy_River', 'America/Rankin_Inlet', 'America/Recife', 'America/Regina', 'America/Resolute', 'America/Rio_Branco', 'America/Santa_Isabel', 'America/Santarem', 'America/Santiago', 'America/Santo_Domingo', 'America/Sao_Paulo', 'America/Scoresbysund', 'America/Shiprock', 'America/Sitka', 'America/St_Barthelemy', 'America/St_Johns', 'America/St_Kitts', 'America/St_Lucia', 'America/St_Thomas', 'America/St_Vincent', 'America/Swift_Current', 'America/Tegucigalpa', 'America/Thule', 'America/Thunder_Bay', 'America/Tijuana', 'America/Toronto', 'America/Tortola', 'America/Vancouver', 'America/Whitehorse', 'America/Winnipeg', 'America/Yakutat', 'America/Yellowknife', 'Arctic/Longyearbyen', 'Asia/Aden', 'Asia/Amman', 'Asia/Anadyr', 'Asia/Ashgabat', 'Asia/Baghdad', 'Asia/Bahrain', 'Asia/Baku', 'Asia/Bangkok', 'Asia/Beirut', 'Asia/Bishkek', 'Asia/Brunei', 'Asia/Choibalsan', 'Asia/Colombo', 'Asia/Damascus', 'Asia/Dhaka', 'Asia/Dili', 'Asia/Dubai', 'Asia/Dushanbe', 'Asia/Famagusta', 'Asia/Gaza', 'Asia/Ho_Chi_Minh', 'Asia/Hong_Kong', 'Asia/Hovd', 'Asia/Irkutsk', 'Asia/Jakarta', 'Asia/Jayapura', 'Asia/Jerusalem', 'Asia/Kabul', 'Asia/Kamchatka', 'Asia/Karachi', 'Asia/Kathmandu', 'Asia/Khandyga', 'Asia/Kolkata', 'Asia/Krasnoyarsk', 'Asia/Kuala_Lumpur', 'Asia/Kuching', 'Asia/Kuwait', 'Asia/Macau', 'Asia/Magadan', 'Asia/Manila', 'Asia/Muscat', 'Asia/Nicosia', 'Asia/Novokuznetsk', 'Asia/Novosibirsk', 'Asia/Omsk', 'Asia/Oral', 'Asia/Phnom_Penh', 'Asia/Pyongyang', 'Asia/Qatar', 'Asia/Rangoon', 'Asia/Riyadh', 'Asia/Sakhalin', 'Asia/Samarkand', 'Asia/Seoul', 'Asia/Shanghai', 'Asia/Singapore', 'Asia/Taipei', 'Asia/Tashkent', 'Asia/Tbilisi', 'Asia/Tehran', 'Asia/Thimphu', 'Asia/Tokyo', 'Asia/Ulaanbaatar', 'Asia/Ust-Nera', 'Asia/Vientiane', 'Asia/Vladivostok', 'Asia/Yakutsk', 'Asia/Yangon', 'Asia/Yekaterinburg', 'Asia/Yerevan', 'Atlantic/Azores', 'Atlantic/Bermuda', 'Atlantic/Canary', 'Atlantic/Cape_Verde', 'Atlantic/Faroe', 'Atlantic/Madeira', 'Atlantic/Reykjavik', 'Atlantic/St_Helena', 'Atlantic/Stanley', 'Australia/Adelaide', 'Australia/Brisbane', 'Australia/Broken_Hill', 'Australia/Currie', 'Australia/Darwin', 'Australia/Eucla', 'Australia/Hobart', 'Australia/Lindeman', 'Australia/Lord_Howe', 'Australia/Melbourne', 'Australia/Perth', 'Australia/Sydney', 'Europe/Amsterdam', 'Europe/Andorra', 'Europe/Athens', 'Europe/Belgrade', 'Europe/Berlin', 'Europe/Bratislava', 'Europe/Brussels', 'Europe/Bucharest', 'Europe/Budapest', 'Europe/Busingen', 'Europe/Chisinau', 'Europe/Copenhagen', 'Europe/Dublin', 'Europe/Gibraltar', 'Europe/Guernsey', 'Europe/Helsinki', 'Europe/Isle_of_Man', 'Europe/Istanbul', 'Europe/Jersey', 'Europe/Kaliningrad', 'Europe/Kiev', 'Europe/Lisbon', 'Europe/Ljubljana', 'Europe/London', 'Europe/Luxembourg', 'Europe/Madrid', 'Europe/Malta', 'Europe/Mariehamn', 'Europe/Minsk', 'Europe/Monaco', 'Europe/Moscow', 'Europe/Oslo', 'Europe/Paris', 'Europe/Podgorica', 'Europe/Prague', 'Europe/Riga', 'Europe/Rome', 'Europe/Samara', 'Europe/San_Marino', 'Europe/Sarajevo', 'Europe/Simferopol', 'Europe/Skopje', 'Europe/Sofia', 'Europe/Stockholm', 'Europe/Tallinn', 'Europe/Tirane', 'Europe/Uzhgorod', 'Europe/Vaduz', 'Europe/Vatican', 'Europe/Vienna', 'Europe/Vilnius', 'Europe/Volgograd', 'Europe/Warsaw', 'Europe/Zagreb', 'Europe/Zaporozhye', 'Europe/Zurich', 'Indian/Antananarivo', 'Indian/Chagos', 'Indian/Christmas', 'Indian/Cocos', 'Indian/Comoro', 'Indian/Mahe', 'Indian/Maldives', 'Indian/Mauritius', 'Indian/Mayotte', 'Indian/Reunion', 'Pacific/Apia', 'Pacific/Auckland', 'Pacific/Chatham', 'Pacific/Chuuk', 'Pacific/Easter', 'Pacific/Efate', 'Pacific/Fakaofo', 'Pacific/Fiji', 'Pacific/Funafuti', 'Pacific/Guadalcanal', 'Pacific/Guam', 'Pacific/Honolulu', 'Pacific/Kiritimati', 'Pacific/Kwajalein', 'Pacific/Majuro', 'Pacific/Midway', 'Pacific/Nauru', 'Pacific/Niue', 'Pacific/Norfolk', 'Pacific/Noumea', 'Pacific/Pago_Pago', 'Pacific/Palau', 'Pacific/Pitcairn', 'Pacific/Port_Moresby', 'Pacific/Rarotonga', 'Pacific/Saipan', 'Pacific/Tahiti', 'Pacific/Tongatapu', 'Pacific/Wake', 'Pacific/Wallis', 'US/Pacific']
     >>> print(list_all_scripts())    # doctest: +NORMALIZE_WHITESPACE
@@ -2172,11 +2172,12 @@
     ['LatGrkCyr-8x16', 'eurlatgr', 'iso07u-16', 'latarcyrheb-sun16']
     '''
 
 
 if __name__ == "__main__":
     import doctest
     (FAILED, ATTEMPTED) = doctest.testmod()
+    print(f'{ATTEMPTED} tests run. {ATTEMPTED - FAILED} passed and {FAILED} failed.')
     if FAILED:
-        # Return number of failed tests:
         sys.exit(FAILED)
+    print(f'All tests passed.')
     sys.exit(0)
```

### Comparing `langtable-0.0.65/tools/compare_with_glib_source.py` & `langtable-0.0.66/tools/compare_with_glib_source.py`

 * *Files identical despite different names*

### Comparing `langtable-0.0.65/tools/list-missing-regions-and-languages.sh` & `langtable-0.0.66/tools/list-missing-regions-and-languages.sh`

 * *Files identical despite different names*

### Comparing `langtable-0.0.65/unicode-license.txt` & `langtable-0.0.66/unicode-license.txt`

 * *Files identical despite different names*

