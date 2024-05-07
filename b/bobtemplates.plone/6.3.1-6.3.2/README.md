# Comparing `tmp/bobtemplates.plone-6.3.1.tar.gz` & `tmp/bobtemplates.plone-6.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bobtemplates.plone-6.3.1.tar", last modified: Tue Oct 31 10:04:07 2023, max compression
+gzip compressed data, was "bobtemplates.plone-6.3.2.tar", last modified: Tue May  7 17:22:09 2024, max compression
```

## Comparing `bobtemplates.plone-6.3.1.tar` & `bobtemplates.plone-6.3.2.tar`

### file list

```diff
@@ -1,483 +1,493 @@
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.621396 bobtemplates.plone-6.3.1/
--rw-r--r--   0 maik      (1000) maik      (1000)    34484 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/CHANGES.rst
--rw-r--r--   0 maik      (1000) maik      (1000)      720 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/CONTRIBUTORS.rst
--rw-r--r--   0 maik      (1000) maik      (1000)    18092 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/LICENSE.GPL
--rw-r--r--   0 maik      (1000) maik      (1000)      665 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/LICENSE.rst
--rw-r--r--   0 maik      (1000) maik      (1000)      299 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/MANIFEST.in
--rw-r--r--   0 maik      (1000) maik      (1000)    42428 2023-10-31 10:04:07.625396 bobtemplates.plone-6.3.1/PKG-INFO
--rw-r--r--   0 maik      (1000) maik      (1000)     5751 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/README.rst
--rw-r--r--   0 maik      (1000) maik      (1000)      980 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/TODO.rst
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.525394 bobtemplates.plone-6.3.1/bobtemplates/
--rw-r--r--   0 maik      (1000) maik      (1000)       80 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/__init__.py
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.533394 bobtemplates.plone-6.3.1/bobtemplates/plone/
--rw-r--r--   0 maik      (1000) maik      (1000)       80 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/__init__.py
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.541394 bobtemplates.plone-6.3.1/bobtemplates/plone/addon/
--rw-r--r--   0 maik      (1000) maik      (1000)       91 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/addon/.coveragerc.bob
--rw-r--r--   0 maik      (1000) maik      (1000)      245 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/addon/.editorconfig
--rw-r--r--   0 maik      (1000) maik      (1000)       23 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/addon/.gitattributes
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.541394 bobtemplates.plone-6.3.1/bobtemplates/plone/addon/.github/
--rw-r--r--   0 maik      (1000) maik      (1000)      366 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/addon/.github/ISSUE_TEMPLATE.md.bob
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.541394 bobtemplates.plone-6.3.1/bobtemplates/plone/addon/.github/workflows/
--rw-r--r--   0 maik      (1000) maik      (1000)     2578 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/addon/.github/workflows/plone-package.yml.bob
--rw-r--r--   0 maik      (1000) maik      (1000)      380 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/addon/.gitignore.bob
--rw-r--r--   0 maik      (1000) maik      (1000)     1880 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/addon/.gitlab-ci.yml
--rw-r--r--   0 maik      (1000) maik      (1000)     2233 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/addon/.mrbob.ini
--rw-r--r--   0 maik      (1000) maik      (1000)     1651 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/addon/.travis.yml.bob
--rw-r--r--   0 maik      (1000) maik      (1000)      111 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/addon/CHANGES.rst.bob
--rw-r--r--   0 maik      (1000) maik      (1000)       71 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/addon/CONTRIBUTORS.rst.bob
--rw-r--r--   0 maik      (1000) maik      (1000)     1338 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/addon/DEVELOP.rst
--rw-r--r--   0 maik      (1000) maik      (1000)    18092 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/addon/LICENSE.GPL.bob
--rw-r--r--   0 maik      (1000) maik      (1000)      690 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/addon/LICENSE.rst.bob
--rw-r--r--   0 maik      (1000) maik      (1000)      140 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/addon/MANIFEST.in.bob
--rw-r--r--   0 maik      (1000) maik      (1000)     3026 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/addon/README.rst.bob
--rw-r--r--   0 maik      (1000) maik      (1000)     2167 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/addon/base.cfg.bob
--rw-r--r--   0 maik      (1000) maik      (1000)      130 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/addon/bobtemplate.cfg.bob
--rw-r--r--   0 maik      (1000) maik      (1000)      215 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/addon/buildout.cfg
--rw-r--r--   0 maik      (1000) maik      (1000)       27 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/addon/constraints.txt
--rw-r--r--   0 maik      (1000) maik      (1000)      155 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/addon/constraints_plone52.txt
--rw-r--r--   0 maik      (1000) maik      (1000)      424 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/addon/constraints_plone60.txt
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.541394 bobtemplates.plone-6.3.1/bobtemplates/plone/addon/docs/
--rw-r--r--   0 maik      (1000) maik      (1000)     7997 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/addon/docs/conf.py.bob
--rw-r--r--   0 maik      (1000) maik      (1000)      169 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/addon/docs/index.rst.bob
--rw-r--r--   0 maik      (1000) maik      (1000)       28 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/addon/requirements.txt
--rw-r--r--   0 maik      (1000) maik      (1000)       50 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/addon/requirements_plone52.txt
--rw-r--r--   0 maik      (1000) maik      (1000)       50 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/addon/requirements_plone60.txt
--rw-r--r--   0 maik      (1000) maik      (1000)      408 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/addon/setup.cfg.bob
--rw-r--r--   0 maik      (1000) maik      (1000)     2589 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/addon/setup.py.bob
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.501393 bobtemplates.plone-6.3.1/bobtemplates/plone/addon/src/
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.541394 bobtemplates.plone-6.3.1/bobtemplates/plone/addon/src/+package.namespace+/
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.545394 bobtemplates.plone-6.3.1/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/
--rw-r--r--   0 maik      (1000) maik      (1000)      143 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/__init__.py.bob
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.545394 bobtemplates.plone-6.3.1/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/browser/
--rw-r--r--   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/browser/__init__.py
--rw-r--r--   0 maik      (1000) maik      (1000)      620 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/browser/configure.zcml.bob
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.545394 bobtemplates.plone-6.3.1/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/browser/overrides/
--rw-r--r--   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/browser/overrides/.gitkeep
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.545394 bobtemplates.plone-6.3.1/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/browser/static/
--rw-r--r--   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/browser/static/.gitkeep
--rw-r--r--   0 maik      (1000) maik      (1000)     1521 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/configure.zcml.bob
--rw-r--r--   0 maik      (1000) maik      (1000)      273 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/interfaces.py.bob
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.545394 bobtemplates.plone-6.3.1/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/locales/
--rw-r--r--   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/locales/+package.dottedname+.pot
--rw-r--r--   0 maik      (1000) maik      (1000)      611 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/locales/README.rst.bob
--rw-r--r--   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/locales/__init__.py
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.501393 bobtemplates.plone-6.3.1/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/locales/en/
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.545394 bobtemplates.plone-6.3.1/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/locales/en/LC_MESSAGES/
--rw-r--r--   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/locales/en/LC_MESSAGES/+package.dottedname+.po.bob
--rw-r--r--   0 maik      (1000) maik      (1000)     1806 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/locales/update.py.bob
--rwxr-xr-x   0 maik      (1000) maik      (1000)      515 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/locales/update.sh.bob
--rw-r--r--   0 maik      (1000) maik      (1000)      260 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/permissions.zcml.bob
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.501393 bobtemplates.plone-6.3.1/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/profiles/
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.549394 bobtemplates.plone-6.3.1/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/profiles/default/
--rw-r--r--   0 maik      (1000) maik      (1000)      202 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/profiles/default/browserlayer.xml.bob
--rw-r--r--   0 maik      (1000) maik      (1000)      105 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/profiles/default/catalog.xml.bob
--rw-r--r--   0 maik      (1000) maik      (1000)      195 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/profiles/default/metadata.xml.bob
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.549394 bobtemplates.plone-6.3.1/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/profiles/default/registry/
--rw-r--r--   0 maik      (1000) maik      (1000)      184 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/profiles/default/registry/main.xml.bob
--rw-r--r--   0 maik      (1000) maik      (1000)      118 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/profiles/default/rolemap.xml.bob
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.549394 bobtemplates.plone-6.3.1/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/profiles/uninstall/
--rw-r--r--   0 maik      (1000) maik      (1000)      136 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/profiles/uninstall/browserlayer.xml.bob
--rw-r--r--   0 maik      (1000) maik      (1000)      803 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/setuphandlers.py.bob
--rw-r--r--   0 maik      (1000) maik      (1000)     1973 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/testing.py.bob
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.549394 bobtemplates.plone-6.3.1/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/tests/
--rw-r--r--   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/tests/__init__.py
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.549394 bobtemplates.plone-6.3.1/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/tests/robot/
--rw-r--r--   0 maik      (1000) maik      (1000)     2037 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/tests/robot/test_example.robot.bob
--rw-r--r--   0 maik      (1000) maik      (1000)      916 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/tests/test_robot.py.bob
--rw-r--r--   0 maik      (1000) maik      (1000)     2596 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/tests/test_setup.py.bob
--rw-r--r--   0 maik      (1000) maik      (1000)       80 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/addon/src/+package.namespace+/__init__.py
--rw-r--r--   0 maik      (1000) maik      (1000)      344 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/addon/test_plone52.cfg
--rw-r--r--   0 maik      (1000) maik      (1000)      298 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/addon/test_plone60.cfg
--rw-r--r--   0 maik      (1000) maik      (1000)     3733 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/addon/tox.ini
--rw-r--r--   0 maik      (1000) maik      (1000)     4404 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/addon.py
--rw-r--r--   0 maik      (1000) maik      (1000)    16854 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/base.py
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.549394 bobtemplates.plone-6.3.1/bobtemplates/plone/behavior/
--rw-r--r--   0 maik      (1000) maik      (1000)     1195 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/behavior/.mrbob.ini
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.549394 bobtemplates.plone-6.3.1/bobtemplates/plone/behavior/behaviors/
--rw-r--r--   0 maik      (1000) maik      (1000)     1103 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/behavior/behaviors/+behavior_name_normalized+.py.bob
--rw-r--r--   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/behavior/behaviors/__init__.py
--rw-r--r--   0 maik      (1000) maik      (1000)      342 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/behavior/behaviors/configure.zcml.example.bob
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.549394 bobtemplates.plone-6.3.1/bobtemplates/plone/behavior/tests/
--rw-r--r--   0 maik      (1000) maik      (1000)     1008 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/behavior/tests/test_behavior_+behavior_name_normalized+.py.bob
--rw-r--r--   0 maik      (1000) maik      (1000)     4830 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/behavior.py
--rw-r--r--   0 maik      (1000) maik      (1000)     3630 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/bobregistry.py
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.553394 bobtemplates.plone-6.3.1/bobtemplates/plone/buildout/
--rw-r--r--   0 maik      (1000) maik      (1000)      422 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/buildout/.gitignore
--rw-r--r--   0 maik      (1000) maik      (1000)     1743 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/buildout/.mrbob.ini
--rw-r--r--   0 maik      (1000) maik      (1000)     8167 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/buildout/base.cfg.bob
--rw-r--r--   0 maik      (1000) maik      (1000)       91 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/buildout/bobtemplate.cfg.bob
--rw-r--r--   0 maik      (1000) maik      (1000)      777 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/buildout/buildout.cfg.bob
--rw-r--r--   0 maik      (1000) maik      (1000)       73 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/buildout/constraints.txt.bob
--rw-r--r--   0 maik      (1000) maik      (1000)       42 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/buildout/requirements.txt
--rw-r--r--   0 maik      (1000) maik      (1000)      163 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/buildout.py
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.553394 bobtemplates.plone-6.3.1/bobtemplates/plone/content_type/
--rw-r--r--   0 maik      (1000) maik      (1000)     4940 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/content_type/.mrbob.ini
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.553394 bobtemplates.plone-6.3.1/bobtemplates/plone/content_type/content/
--rw-r--r--   0 maik      (1000) maik      (1000)     2498 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/content_type/content/+dexterity_type_name_normalized+.py.bob
--rw-r--r--   0 maik      (1000) maik      (1000)      326 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/content_type/content/+dexterity_type_name_normalized+.xml.bob
--rw-r--r--   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/content_type/content/__init__.py
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.501393 bobtemplates.plone-6.3.1/bobtemplates/plone/content_type/profiles/
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.553394 bobtemplates.plone-6.3.1/bobtemplates/plone/content_type/profiles/default/
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.553394 bobtemplates.plone-6.3.1/bobtemplates/plone/content_type/profiles/default/types/
--rw-r--r--   0 maik      (1000) maik      (1000)     5305 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/content_type/profiles/default/types/+dexterity_type_fti_file_name+.xml.bob
--rw-r--r--   0 maik      (1000) maik      (1000)      238 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/content_type/profiles/default/types.xml.example.bob
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.553394 bobtemplates.plone-6.3.1/bobtemplates/plone/content_type/tests/
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.553394 bobtemplates.plone-6.3.1/bobtemplates/plone/content_type/tests/robot/
--rw-r--r--   0 maik      (1000) maik      (1000)     3840 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/content_type/tests/robot/test_ct_+dexterity_type_name_normalized+.robot.bob
--rw-r--r--   0 maik      (1000) maik      (1000)     7810 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/content_type/tests/test_ct_+dexterity_type_name_normalized+.py.bob
--rw-r--r--   0 maik      (1000) maik      (1000)    10184 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/content_type.py
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.553394 bobtemplates.plone-6.3.1/bobtemplates/plone/controlpanel/
--rw-r--r--   0 maik      (1000) maik      (1000)     1040 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/controlpanel/.mrbob.ini
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.557395 bobtemplates.plone-6.3.1/bobtemplates/plone/controlpanel/controlpanels/
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.557395 bobtemplates.plone-6.3.1/bobtemplates/plone/controlpanel/controlpanels/+controlpanel_name_normalized+/
--rw-r--r--   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/controlpanel/controlpanels/+controlpanel_name_normalized+/__init__.py.bob
--rw-r--r--   0 maik      (1000) maik      (1000)      759 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/controlpanel/controlpanels/+controlpanel_name_normalized+/configure.zcml.bob
--rw-r--r--   0 maik      (1000) maik      (1000)     1625 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/controlpanel/controlpanels/+controlpanel_name_normalized+/controlpanel.py.bob
--rw-r--r--   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/controlpanel/controlpanels/__init__.py.bob
--rw-r--r--   0 maik      (1000) maik      (1000)      264 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/controlpanel/controlpanels/configure.zcml.example.bob
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.505393 bobtemplates.plone-6.3.1/bobtemplates/plone/controlpanel/profiles/
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.557395 bobtemplates.plone-6.3.1/bobtemplates/plone/controlpanel/profiles/default/
--rw-r--r--   0 maik      (1000) maik      (1000)      207 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/controlpanel/profiles/default/controlpanel.xml.example.bob
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.557395 bobtemplates.plone-6.3.1/bobtemplates/plone/controlpanel/profiles/default/registry/
--rw-r--r--   0 maik      (1000) maik      (1000)      420 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/controlpanel/profiles/default/registry/+controlpanel_name_normalized+.xml.bob
--rw-r--r--   0 maik      (1000) maik      (1000)     5516 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/controlpanel.py
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.557395 bobtemplates.plone-6.3.1/bobtemplates/plone/form/
--rw-r--r--   0 maik      (1000) maik      (1000)     1570 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/form/.mrbob.ini
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.557395 bobtemplates.plone-6.3.1/bobtemplates/plone/form/forms/
--rw-r--r--   0 maik      (1000) maik      (1000)     1280 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/form/forms/+form_python_file_name+.py.bob
--rw-r--r--   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/form/forms/__init__.py
--rw-r--r--   0 maik      (1000) maik      (1000)      263 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/form/forms/configure.zcml.example.bob
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.557395 bobtemplates.plone-6.3.1/bobtemplates/plone/form/tests/
--rw-r--r--   0 maik      (1000) maik      (1000)     1568 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/form/tests/test_form_+form_name_normalized+.py.bob
--rw-r--r--   0 maik      (1000) maik      (1000)     6386 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/form.py
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.557395 bobtemplates.plone-6.3.1/bobtemplates/plone/indexer/
--rw-r--r--   0 maik      (1000) maik      (1000)      876 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/indexer/.mrbob.ini
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.561395 bobtemplates.plone-6.3.1/bobtemplates/plone/indexer/indexers/
--rw-r--r--   0 maik      (1000) maik      (1000)      513 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/indexer/indexers/+indexer_file_name+.py.bob
--rw-r--r--   0 maik      (1000) maik      (1000)      261 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/indexer/indexers/+indexer_file_name+.zcml.bob
--rw-r--r--   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/indexer/indexers/__init__.py
--rw-r--r--   0 maik      (1000) maik      (1000)      157 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/indexer/indexers/configure.zcml.example.bob
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.561395 bobtemplates.plone-6.3.1/bobtemplates/plone/indexer/tests/
--rw-r--r--   0 maik      (1000) maik      (1000)      888 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/indexer/tests/test_indexer_+indexer_file_name+.py.bob
--rw-r--r--   0 maik      (1000) maik      (1000)     2838 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/indexer.py
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.561395 bobtemplates.plone-6.3.1/bobtemplates/plone/mockup_pattern/
--rw-r--r--   0 maik      (1000) maik      (1000)       59 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/mockup_pattern/.eslintrc.js
--rw-r--r--   0 maik      (1000) maik      (1000)      610 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/mockup_pattern/.mrbob.ini
--rw-r--r--   0 maik      (1000) maik      (1000)       28 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/mockup_pattern/.prettierignore
--rw-r--r--   0 maik      (1000) maik      (1000)       61 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/mockup_pattern/.release-it.js
--rw-r--r--   0 maik      (1000) maik      (1000)       62 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/mockup_pattern/babel.config.js
--rw-r--r--   0 maik      (1000) maik      (1000)      132 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/mockup_pattern/jest.config.js
--rw-r--r--   0 maik      (1000) maik      (1000)      702 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/mockup_pattern/package.json.bob
--rw-r--r--   0 maik      (1000) maik      (1000)       65 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/mockup_pattern/prettier.config.js
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.561395 bobtemplates.plone-6.3.1/bobtemplates/plone/mockup_pattern/resources/
--rw-r--r--   0 maik      (1000) maik      (1000)      169 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/mockup_pattern/resources/bundle.js.bob
--rw-r--r--   0 maik      (1000) maik      (1000)      252 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/mockup_pattern/resources/index.html.bob
--rw-r--r--   0 maik      (1000) maik      (1000)      113 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/mockup_pattern/resources/index.js
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.565395 bobtemplates.plone-6.3.1/bobtemplates/plone/mockup_pattern/resources/pat-+pattern.name+/
--rw-r--r--   0 maik      (1000) maik      (1000)     1356 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/mockup_pattern/resources/pat-+pattern.name+/+pattern.name+.js.bob
--rw-r--r--   0 maik      (1000) maik      (1000)      117 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/mockup_pattern/resources/pat-+pattern.name+/+pattern.name+.scss.bob
--rw-r--r--   0 maik      (1000) maik      (1000)     1277 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/mockup_pattern/resources/pat-+pattern.name+/+pattern.name+.test.js.bob
--rw-r--r--   0 maik      (1000) maik      (1000)      481 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/mockup_pattern/resources/pat-+pattern.name+/documentation.md.bob
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.505393 bobtemplates.plone-6.3.1/bobtemplates/plone/mockup_pattern/src/
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.505393 bobtemplates.plone-6.3.1/bobtemplates/plone/mockup_pattern/src/+package.namespace+/
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.505393 bobtemplates.plone-6.3.1/bobtemplates/plone/mockup_pattern/src/+package.namespace+/+package.name+/
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.565395 bobtemplates.plone-6.3.1/bobtemplates/plone/mockup_pattern/src/+package.namespace+/+package.name+/browser/
--rw-r--r--   0 maik      (1000) maik      (1000)      199 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/mockup_pattern/src/+package.namespace+/+package.name+/browser/configure.zcml.bob
--rw-r--r--   0 maik      (1000) maik      (1000)      560 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/mockup_pattern/src/+package.namespace+/+package.name+/browser/pattern-demo.pt.bob
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.505393 bobtemplates.plone-6.3.1/bobtemplates/plone/mockup_pattern/src/+package.namespace+/+package.name+/browser/static/
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.565395 bobtemplates.plone-6.3.1/bobtemplates/plone/mockup_pattern/src/+package.namespace+/+package.name+/browser/static/bundles/
--rw-r--r--   0 maik      (1000) maik      (1000)       68 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/mockup_pattern/src/+package.namespace+/+package.name+/browser/static/bundles/.gitkeep
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.509393 bobtemplates.plone-6.3.1/bobtemplates/plone/mockup_pattern/src/+package.namespace+/+package.name+/profiles/
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.505393 bobtemplates.plone-6.3.1/bobtemplates/plone/mockup_pattern/src/+package.namespace+/+package.name+/profiles/default/
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.565395 bobtemplates.plone-6.3.1/bobtemplates/plone/mockup_pattern/src/+package.namespace+/+package.name+/profiles/default/registry/
--rw-r--r--   0 maik      (1000) maik      (1000)      361 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/mockup_pattern/src/+package.namespace+/+package.name+/profiles/default/registry/bundles.xml.bob
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.509393 bobtemplates.plone-6.3.1/bobtemplates/plone/mockup_pattern/src/+package.namespace+/+package.name+/profiles/uninstall/
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.565395 bobtemplates.plone-6.3.1/bobtemplates/plone/mockup_pattern/src/+package.namespace+/+package.name+/profiles/uninstall/registry/
--rw-r--r--   0 maik      (1000) maik      (1000)      198 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/mockup_pattern/src/+package.namespace+/+package.name+/profiles/uninstall/registry/bundles.xml.bob
--rw-r--r--   0 maik      (1000) maik      (1000)     1495 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/mockup_pattern/webpack.config.js.bob
--rw-r--r--   0 maik      (1000) maik      (1000)     3836 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/mockup_pattern.py
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.565395 bobtemplates.plone-6.3.1/bobtemplates/plone/portlet/
--rw-r--r--   0 maik      (1000) maik      (1000)      916 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/portlet/.mrbob.ini
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.565395 bobtemplates.plone-6.3.1/bobtemplates/plone/portlet/portlets/
--rw-r--r--   0 maik      (1000) maik      (1000)      265 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/portlet/portlets/+portlet_name_normalized+.pt.bob
--rw-r--r--   0 maik      (1000) maik      (1000)     3583 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/portlet/portlets/+portlet_name_normalized+.py.bob
--rw-r--r--   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/portlet/portlets/__init__.py
--rw-r--r--   0 maik      (1000) maik      (1000)      259 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/portlet/portlets/configure.zcml.example.bob
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.509393 bobtemplates.plone-6.3.1/bobtemplates/plone/portlet/profiles/
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.565395 bobtemplates.plone-6.3.1/bobtemplates/plone/portlet/profiles/default/
--rw-r--r--   0 maik      (1000) maik      (1000)      159 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/portlet/profiles/default/portlets.xml.example.bob
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.565395 bobtemplates.plone-6.3.1/bobtemplates/plone/portlet/tests/
--rw-r--r--   0 maik      (1000) maik      (1000)     1202 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/portlet/tests/test_+portlet_name_normalized+.py.bob
--rw-r--r--   0 maik      (1000) maik      (1000)     7462 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/portlet.py
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.565395 bobtemplates.plone-6.3.1/bobtemplates/plone/restapi_service/
--rw-r--r--   0 maik      (1000) maik      (1000)     1236 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/restapi_service/.mrbob.ini
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.569395 bobtemplates.plone-6.3.1/bobtemplates/plone/restapi_service/api/
--rw-r--r--   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/restapi_service/api/__init__.py
--rw-r--r--   0 maik      (1000) maik      (1000)      265 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/restapi_service/api/configure.zcml.example.bob
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.569395 bobtemplates.plone-6.3.1/bobtemplates/plone/restapi_service/api/services/
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.569395 bobtemplates.plone-6.3.1/bobtemplates/plone/restapi_service/api/services/+service_class_name_normalized+/
--rw-r--r--   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/restapi_service/api/services/+service_class_name_normalized+/__init__.py
--rw-r--r--   0 maik      (1000) maik      (1000)      417 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/restapi_service/api/services/+service_class_name_normalized+/configure.zcml.bob
--rw-r--r--   0 maik      (1000) maik      (1000)     1845 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/restapi_service/api/services/+service_class_name_normalized+/get.py.bob
--rw-r--r--   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/restapi_service/api/services/__init__.py
--rw-r--r--   0 maik      (1000) maik      (1000)      265 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/restapi_service/api/services/configure.zcml.example.bob
--rw-r--r--   0 maik      (1000) maik      (1000)     5585 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/restapi_service.py
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.569395 bobtemplates.plone-6.3.1/bobtemplates/plone/subscriber/
--rw-r--r--   0 maik      (1000) maik      (1000)     1097 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/subscriber/.mrbob.ini
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.569395 bobtemplates.plone-6.3.1/bobtemplates/plone/subscriber/subscribers/
--rw-r--r--   0 maik      (1000) maik      (1000)      157 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/subscriber/subscribers/+subscriber_handler_file_name+.py.bob
--rw-r--r--   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/subscriber/subscribers/__init__.py
--rw-r--r--   0 maik      (1000) maik      (1000)      157 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/subscriber/subscribers/configure.zcml.example.bob
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.569395 bobtemplates.plone-6.3.1/bobtemplates/plone/subscriber/tests/
--rw-r--r--   0 maik      (1000) maik      (1000)      780 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/subscriber/tests/test_subscriber_+subscriber_handler_file_name+.py.bob
--rw-r--r--   0 maik      (1000) maik      (1000)     3010 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/subscriber.py
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.569395 bobtemplates.plone-6.3.1/bobtemplates/plone/svelte_app/
--rw-r--r--   0 maik      (1000) maik      (1000)     1533 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/svelte_app/.mrbob.ini
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.509393 bobtemplates.plone-6.3.1/bobtemplates/plone/svelte_app/src/
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.509393 bobtemplates.plone-6.3.1/bobtemplates/plone/svelte_app/src/+package.namespace+/
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.513393 bobtemplates.plone-6.3.1/bobtemplates/plone/svelte_app/src/+package.namespace+/+package.name+/
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.509393 bobtemplates.plone-6.3.1/bobtemplates/plone/svelte_app/src/+package.namespace+/+package.name+/profiles/
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.509393 bobtemplates.plone-6.3.1/bobtemplates/plone/svelte_app/src/+package.namespace+/+package.name+/profiles/default/
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.569395 bobtemplates.plone-6.3.1/bobtemplates/plone/svelte_app/src/+package.namespace+/+package.name+/profiles/default/registry/
--rw-r--r--   0 maik      (1000) maik      (1000)     1468 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/svelte_app/src/+package.namespace+/+package.name+/profiles/default/registry/+svelte_app_file_name+.xml.bob
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.509393 bobtemplates.plone-6.3.1/bobtemplates/plone/svelte_app/src/+package.namespace+/+package.name+/profiles/uninstall/
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.569395 bobtemplates.plone-6.3.1/bobtemplates/plone/svelte_app/src/+package.namespace+/+package.name+/profiles/uninstall/registry/
--rw-r--r--   0 maik      (1000) maik      (1000)      539 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/svelte_app/src/+package.namespace+/+package.name+/profiles/uninstall/registry/+svelte_app_file_name+.xml.bob
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.513393 bobtemplates.plone-6.3.1/bobtemplates/plone/svelte_app/src/+package.namespace+/+package.name+/svelte_apps/
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.573395 bobtemplates.plone-6.3.1/bobtemplates/plone/svelte_app/src/+package.namespace+/+package.name+/svelte_apps/+svelte_app_name_dashed+/
--rw-r--r--   0 maik      (1000) maik      (1000)      315 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/svelte_app/src/+package.namespace+/+package.name+/svelte_apps/+svelte_app_name_dashed+/README.md.bob
--rw-r--r--   0 maik      (1000) maik      (1000)     3127 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/svelte_app/src/+package.namespace+/+package.name+/svelte_apps/+svelte_app_name_dashed+/favicon.png
--rw-r--r--   0 maik      (1000) maik      (1000)      890 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/svelte_app/src/+package.namespace+/+package.name+/svelte_apps/+svelte_app_name_dashed+/global.css
--rw-r--r--   0 maik      (1000) maik      (1000)      531 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/svelte_app/src/+package.namespace+/+package.name+/svelte_apps/+svelte_app_name_dashed+/index.html.bob
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.513393 bobtemplates.plone-6.3.1/bobtemplates/plone/svelte_app/svelte_src/
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.573395 bobtemplates.plone-6.3.1/bobtemplates/plone/svelte_app/svelte_src/+svelte_app_name_dashed+/
--rw-r--r--   0 maik      (1000) maik      (1000)       41 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/svelte_app/svelte_src/+svelte_app_name_dashed+/.gitignore
--rw-r--r--   0 maik      (1000) maik      (1000)     2270 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/svelte_app/svelte_src/+svelte_app_name_dashed+/README.md.bob
--rw-r--r--   0 maik      (1000) maik      (1000)      516 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/svelte_app/svelte_src/+svelte_app_name_dashed+/package.json
--rw-r--r--   0 maik      (1000) maik      (1000)     2397 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/svelte_app/svelte_src/+svelte_app_name_dashed+/rollup.config.js.bob
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.573395 bobtemplates.plone-6.3.1/bobtemplates/plone/svelte_app/svelte_src/+svelte_app_name_dashed+/scripts/
--rw-r--r--   0 maik      (1000) maik      (1000)     4292 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/svelte_app/svelte_src/+svelte_app_name_dashed+/scripts/setupTypeScript.js
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.573395 bobtemplates.plone-6.3.1/bobtemplates/plone/svelte_app/svelte_src/+svelte_app_name_dashed+/src/
--rw-r--r--   0 maik      (1000) maik      (1000)      826 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/svelte_app/svelte_src/+svelte_app_name_dashed+/src/App.svelte.bob
--rw-r--r--   0 maik      (1000) maik      (1000)      613 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/svelte_app/svelte_src/+svelte_app_name_dashed+/src/main.js.bob
--rw-r--r--   0 maik      (1000) maik      (1000)     2979 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/svelte_app.py
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.573395 bobtemplates.plone-6.3.1/bobtemplates/plone/theme/
--rw-r--r--   0 maik      (1000) maik      (1000)     1020 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/theme/.mrbob.ini
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.513393 bobtemplates.plone-6.3.1/bobtemplates/plone/theme/profiles/
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.573395 bobtemplates.plone-6.3.1/bobtemplates/plone/theme/profiles/default/
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.573395 bobtemplates.plone-6.3.1/bobtemplates/plone/theme/profiles/default/registry/
--rw-r--r--   0 maik      (1000) maik      (1000)      387 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/theme/profiles/default/registry/displayed_types.xml
--rw-r--r--   0 maik      (1000) maik      (1000)      460 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/theme/profiles/default/registry/email_from.xml
--rw-r--r--   0 maik      (1000) maik      (1000)     2320 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/theme/profiles/default/registry/main.xml
--rw-r--r--   0 maik      (1000) maik      (1000)      309 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/theme/profiles/default/registry/nonfolderish_tabs.xml
--rw-r--r--   0 maik      (1000) maik      (1000)     2263 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/theme/profiles/default/registry/tinymce.xml
--rw-r--r--   0 maik      (1000) maik      (1000)      127 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/theme/profiles/default/theme.xml.bob
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.573395 bobtemplates.plone-6.3.1/bobtemplates/plone/theme/profiles/uninstall/
--rw-r--r--   0 maik      (1000) maik      (1000)      109 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/theme/profiles/uninstall/theme.xml.bob
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.577395 bobtemplates.plone-6.3.1/bobtemplates/plone/theme/theme/
--rw-r--r--   0 maik      (1000) maik      (1000)     3008 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/theme/theme/README.rst.bob
--rw-r--r--   0 maik      (1000) maik      (1000)      174 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/theme/theme/index.html
--rw-r--r--   0 maik      (1000) maik      (1000)      529 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/theme/theme/manifest.cfg.bob
--rw-r--r--   0 maik      (1000) maik      (1000)     1620 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/theme/theme/package.json.bob
--rw-r--r--   0 maik      (1000) maik      (1000)     6091 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/theme/theme/rules.xml.bob
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.577395 bobtemplates.plone-6.3.1/bobtemplates/plone/theme/theme/styles/
--rw-r--r--   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/theme/theme/styles/theme.min.css
--rw-r--r--   0 maik      (1000) maik      (1000)      638 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/theme/theme/styles/theme.scss
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.577395 bobtemplates.plone-6.3.1/bobtemplates/plone/theme/theme/tinymce-templates/
--rw-r--r--   0 maik      (1000) maik      (1000)      808 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/theme/theme/tinymce-templates/bs-dark-hero.html
--rw-r--r--   0 maik      (1000) maik      (1000)      951 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/theme/theme/tinymce-templates/bs-hero-left.html
--rw-r--r--   0 maik      (1000) maik      (1000)     2049 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/theme/theme/tinymce-templates/bs-pricing.html
--rw-r--r--   0 maik      (1000) maik      (1000)     5141 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/theme.py
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.577395 bobtemplates.plone-6.3.1/bobtemplates/plone/theme_barceloneta/
--rw-r--r--   0 maik      (1000) maik      (1000)     1056 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/theme_barceloneta/.mrbob.ini
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.513393 bobtemplates.plone-6.3.1/bobtemplates/plone/theme_barceloneta/src/
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.513393 bobtemplates.plone-6.3.1/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.513393 bobtemplates.plone-6.3.1/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.513393 bobtemplates.plone-6.3.1/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/profiles/
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.577395 bobtemplates.plone-6.3.1/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/profiles/default/
--rw-r--r--   0 maik      (1000) maik      (1000)      127 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/profiles/default/theme.xml.bob
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.577395 bobtemplates.plone-6.3.1/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/profiles/uninstall/
--rw-r--r--   0 maik      (1000) maik      (1000)      109 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/profiles/uninstall/theme.xml
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.581395 bobtemplates.plone-6.3.1/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/
--rw-r--r--   0 maik      (1000) maik      (1000)     2769 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/README.rst.bob
--rw-r--r--   0 maik      (1000) maik      (1000)     2112 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/barceloneta-apple-touch-icon-114x114-precomposed.png
--rw-r--r--   0 maik      (1000) maik      (1000)     2382 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/barceloneta-apple-touch-icon-144x144-precomposed.png
--rw-r--r--   0 maik      (1000) maik      (1000)     1090 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/barceloneta-apple-touch-icon-57x57-precomposed.png
--rw-r--r--   0 maik      (1000) maik      (1000)     1414 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/barceloneta-apple-touch-icon-72x72-precomposed.png
--rw-r--r--   0 maik      (1000) maik      (1000)     1090 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/barceloneta-apple-touch-icon-precomposed.png
--rw-r--r--   0 maik      (1000) maik      (1000)     4303 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/barceloneta-apple-touch-icon.png
--rw-r--r--   0 maik      (1000) maik      (1000)     5430 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/barceloneta-favicon.ico
--rw-r--r--   0 maik      (1000) maik      (1000)     3854 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/index.html
--rw-r--r--   0 maik      (1000) maik      (1000)      647 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/manifest.cfg.bob
--rw-r--r--   0 maik      (1000) maik      (1000)     1356 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/package.json.bob
--rw-r--r--   0 maik      (1000) maik      (1000)    89929 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/preview.png
--rw-r--r--   0 maik      (1000) maik      (1000)     7236 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/rules.xml
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.585395 bobtemplates.plone-6.3.1/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/scss/
--rw-r--r--   0 maik      (1000) maik      (1000)      120 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/scss/_custom.scss
--rw-r--r--   0 maik      (1000) maik      (1000)      273 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/scss/_maps.scss
--rw-r--r--   0 maik      (1000) maik      (1000)       60 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/scss/_variables.scss
--rw-r--r--   0 maik      (1000) maik      (1000)     3996 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/scss/theme.scss
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.585395 bobtemplates.plone-6.3.1/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/styles/
--rw-r--r--   0 maik      (1000) maik      (1000)   708963 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/styles/theme.css
--rw-r--r--   0 maik      (1000) maik      (1000)   242413 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/styles/theme.min.css
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.589395 bobtemplates.plone-6.3.1/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/tinymce-templates/
--rw-r--r--   0 maik      (1000) maik      (1000)      732 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/tinymce-templates/README.rst.bob
--rw-r--r--   0 maik      (1000) maik      (1000)     1352 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/tinymce-templates/card-group.html
--rw-r--r--   0 maik      (1000) maik      (1000)      313 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/tinymce-templates/list.html
--rw-r--r--   0 maik      (1000) maik      (1000)     5104 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/theme_barceloneta.py
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.589395 bobtemplates.plone-6.3.1/bobtemplates/plone/theme_basic/
--rw-r--r--   0 maik      (1000) maik      (1000)     1038 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/theme_basic/.mrbob.ini
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.517393 bobtemplates.plone-6.3.1/bobtemplates/plone/theme_basic/src/
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.517393 bobtemplates.plone-6.3.1/bobtemplates/plone/theme_basic/src/+package.namespace+/
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.517393 bobtemplates.plone-6.3.1/bobtemplates/plone/theme_basic/src/+package.namespace+/+package.name+/
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.517393 bobtemplates.plone-6.3.1/bobtemplates/plone/theme_basic/src/+package.namespace+/+package.name+/browser/
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.589395 bobtemplates.plone-6.3.1/bobtemplates/plone/theme_basic/src/+package.namespace+/+package.name+/browser/overrides/
--rw-r--r--   0 maik      (1000) maik      (1000)     1380 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/theme_basic/src/+package.namespace+/+package.name+/browser/overrides/plone.app.layout.viewlets.sections.pt
--rw-r--r--   0 maik      (1000) maik      (1000)      145 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/theme_basic/src/+package.namespace+/+package.name+/browser/overrides/plone.app.portlets.browser.templates.footer.pt
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.517393 bobtemplates.plone-6.3.1/bobtemplates/plone/theme_basic/src/+package.namespace+/+package.name+/profiles/
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.589395 bobtemplates.plone-6.3.1/bobtemplates/plone/theme_basic/src/+package.namespace+/+package.name+/profiles/default/
--rw-r--r--   0 maik      (1000) maik      (1000)      127 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/theme_basic/src/+package.namespace+/+package.name+/profiles/default/theme.xml.bob
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.589395 bobtemplates.plone-6.3.1/bobtemplates/plone/theme_basic/src/+package.namespace+/+package.name+/profiles/uninstall/
--rw-r--r--   0 maik      (1000) maik      (1000)      111 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/theme_basic/src/+package.namespace+/+package.name+/profiles/uninstall/theme.xml
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.589395 bobtemplates.plone-6.3.1/bobtemplates/plone/theme_basic/src/+package.namespace+/+package.name+/theme/
--rw-r--r--   0 maik      (1000) maik      (1000)     2287 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/theme_basic/src/+package.namespace+/+package.name+/theme/README.rst.bob
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.597396 bobtemplates.plone-6.3.1/bobtemplates/plone/theme_basic/src/+package.namespace+/+package.name+/theme/css/
--rw-r--r--   0 maik      (1000) maik      (1000)   896711 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/theme_basic/src/+package.namespace+/+package.name+/theme/css/theme.css
--rw-r--r--   0 maik      (1000) maik      (1000)   284809 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/theme_basic/src/+package.namespace+/+package.name+/theme/css/theme.css.map
--rw-r--r--   0 maik      (1000) maik      (1000)   153028 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/theme_basic/src/+package.namespace+/+package.name+/theme/css/theme.min.css
--rw-r--r--   0 maik      (1000) maik      (1000)  1139991 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/theme_basic/src/+package.namespace+/+package.name+/theme/css/theme.min.css.map
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.601396 bobtemplates.plone-6.3.1/bobtemplates/plone/theme_basic/src/+package.namespace+/+package.name+/theme/js/
--rw-r--r--   0 maik      (1000) maik      (1000)      192 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/theme_basic/src/+package.namespace+/+package.name+/theme/js/theme.js
--rw-r--r--   0 maik      (1000) maik      (1000)       65 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/theme_basic/src/+package.namespace+/+package.name+/theme/js/theme.min.js
--rw-r--r--   0 maik      (1000) maik      (1000)      476 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/theme_basic/src/+package.namespace+/+package.name+/theme/manifest.cfg.bob
--rw-r--r--   0 maik      (1000) maik      (1000)     1585 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/theme_basic/src/+package.namespace+/+package.name+/theme/package.json.bob
--rw-r--r--   0 maik      (1000) maik      (1000)     2852 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/theme_basic/src/+package.namespace+/+package.name+/theme/preview.png
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.601396 bobtemplates.plone-6.3.1/bobtemplates/plone/theme_basic/src/+package.namespace+/+package.name+/theme/scss/
--rw-r--r--   0 maik      (1000) maik      (1000)      285 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/theme_basic/src/+package.namespace+/+package.name+/theme/scss/_base.scss
--rw-r--r--   0 maik      (1000) maik      (1000)      704 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/theme_basic/src/+package.namespace+/+package.name+/theme/scss/theme.scss
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.605396 bobtemplates.plone-6.3.1/bobtemplates/plone/theme_basic/src/+package.namespace+/+package.name+/theme/tinymce-templates/
--rw-r--r--   0 maik      (1000) maik      (1000)     1240 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/theme_basic/src/+package.namespace+/+package.name+/theme/tinymce-templates/README.rst.bob
--rw-r--r--   0 maik      (1000) maik      (1000)     1352 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/theme_basic/src/+package.namespace+/+package.name+/theme/tinymce-templates/card-group.html
--rw-r--r--   0 maik      (1000) maik      (1000)      313 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/theme_basic/src/+package.namespace+/+package.name+/theme/tinymce-templates/list.html
--rw-r--r--   0 maik      (1000) maik      (1000)     4400 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/theme_basic.py
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.605396 bobtemplates.plone-6.3.1/bobtemplates/plone/upgrade_step/
--rw-r--r--   0 maik      (1000) maik      (1000)     1063 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/upgrade_step/.mrbob.ini
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.605396 bobtemplates.plone-6.3.1/bobtemplates/plone/upgrade_step/tests/
--rw-r--r--   0 maik      (1000) maik      (1000)      892 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/upgrade_step/tests/test_upgrade_step_+upgrade_step_id+.py.bob
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.605396 bobtemplates.plone-6.3.1/bobtemplates/plone/upgrade_step/upgrades/
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.605396 bobtemplates.plone-6.3.1/bobtemplates/plone/upgrade_step/upgrades/+upgrade_step_id+/
--rw-r--r--   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/upgrade_step/upgrades/+upgrade_step_id+/.gitkeep
--rw-r--r--   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/upgrade_step/upgrades/+upgrade_step_id+/metadata.txt
--rw-r--r--   0 maik      (1000) maik      (1000)     1056 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/upgrade_step/upgrades/+upgrade_step_id+.zcml.bob
--rw-r--r--   0 maik      (1000) maik      (1000)       98 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/upgrade_step/upgrades/__init__.py.bob
--rw-r--r--   0 maik      (1000) maik      (1000)      218 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/upgrade_step/upgrades/base.py.bob
--rw-r--r--   0 maik      (1000) maik      (1000)      156 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/upgrade_step/upgrades/configure.zcml.example.bob
--rw-r--r--   0 maik      (1000) maik      (1000)      262 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/upgrade_step/upgrades/v+upgrade_step_id+.py.bob
--rw-r--r--   0 maik      (1000) maik      (1000)     4448 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/upgrade_step.py
--rw-r--r--   0 maik      (1000) maik      (1000)     3251 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/utils.py
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.605396 bobtemplates.plone-6.3.1/bobtemplates/plone/view/
--rw-r--r--   0 maik      (1000) maik      (1000)     3329 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/view/.mrbob.ini
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.605396 bobtemplates.plone-6.3.1/bobtemplates/plone/view/tests/
--rw-r--r--   0 maik      (1000) maik      (1000)     1868 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/view/tests/test_view_+view_python_file_name+.py.bob
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.609396 bobtemplates.plone-6.3.1/bobtemplates/plone/view/views/
--rw-r--r--   0 maik      (1000) maik      (1000)     1443 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/view/views/+view_python_file_name+.py.bob
--rw-r--r--   0 maik      (1000) maik      (1000)     1058 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/view/views/+view_template_name+.pt.bob
--rw-r--r--   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/view/views/__init__.py
--rw-r--r--   0 maik      (1000) maik      (1000)      263 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/view/views/configure.zcml.example.bob
--rw-r--r--   0 maik      (1000) maik      (1000)     9202 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/view.py
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.609396 bobtemplates.plone-6.3.1/bobtemplates/plone/viewlet/
--rw-r--r--   0 maik      (1000) maik      (1000)     1964 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/viewlet/.mrbob.ini
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.609396 bobtemplates.plone-6.3.1/bobtemplates/plone/viewlet/tests/
--rw-r--r--   0 maik      (1000) maik      (1000)     2631 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/viewlet/tests/test_viewlet_+viewlet_name_normalized+.py.bob
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.609396 bobtemplates.plone-6.3.1/bobtemplates/plone/viewlet/viewlets/
--rw-r--r--   0 maik      (1000) maik      (1000)      585 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/viewlet/viewlets/+viewlet_python_file_name+.py.bob
--rw-r--r--   0 maik      (1000) maik      (1000)       54 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/viewlet/viewlets/+viewlet_template_name+.pt.bob
--rw-r--r--   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/viewlet/viewlets/__init__.py.bob
--rw-r--r--   0 maik      (1000) maik      (1000)      264 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/viewlet/viewlets/configure.zcml.example.bob
--rw-r--r--   0 maik      (1000) maik      (1000)     6626 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/viewlet.py
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.609396 bobtemplates.plone-6.3.1/bobtemplates/plone/vocabulary/
--rw-r--r--   0 maik      (1000) maik      (1000)      941 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/vocabulary/.mrbob.ini
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.609396 bobtemplates.plone-6.3.1/bobtemplates/plone/vocabulary/tests/
--rw-r--r--   0 maik      (1000) maik      (1000)     1230 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/vocabulary/tests/test_vocab_+vocabulary_name_normalized+.py.bob
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.609396 bobtemplates.plone-6.3.1/bobtemplates/plone/vocabulary/vocabularies/
--rw-r--r--   0 maik      (1000) maik      (1000)     1696 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/vocabulary/vocabularies/+vocabulary_name_normalized+.py.bob
--rw-r--r--   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/vocabulary/vocabularies/__init__.py
--rw-r--r--   0 maik      (1000) maik      (1000)      159 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/vocabulary/vocabularies/configure.zcml.example.bob
--rw-r--r--   0 maik      (1000) maik      (1000)     3995 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/bobtemplates/plone/vocabulary.py
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.529394 bobtemplates.plone-6.3.1/bobtemplates.plone.egg-info/
--rw-r--r--   0 maik      (1000) maik      (1000)    42428 2023-10-31 10:04:07.000000 bobtemplates.plone-6.3.1/bobtemplates.plone.egg-info/PKG-INFO
--rw-r--r--   0 maik      (1000) maik      (1000)    20407 2023-10-31 10:04:07.000000 bobtemplates.plone-6.3.1/bobtemplates.plone.egg-info/SOURCES.txt
--rw-r--r--   0 maik      (1000) maik      (1000)        1 2023-10-31 10:04:07.000000 bobtemplates.plone-6.3.1/bobtemplates.plone.egg-info/dependency_links.txt
--rw-r--r--   0 maik      (1000) maik      (1000)     1267 2023-10-31 10:04:07.000000 bobtemplates.plone-6.3.1/bobtemplates.plone.egg-info/entry_points.txt
--rw-r--r--   0 maik      (1000) maik      (1000)       13 2023-10-31 10:04:07.000000 bobtemplates.plone-6.3.1/bobtemplates.plone.egg-info/namespace_packages.txt
--rw-r--r--   0 maik      (1000) maik      (1000)        1 2023-10-31 10:04:07.000000 bobtemplates.plone-6.3.1/bobtemplates.plone.egg-info/not-zip-safe
--rw-r--r--   0 maik      (1000) maik      (1000)       64 2023-10-31 10:04:07.000000 bobtemplates.plone-6.3.1/bobtemplates.plone.egg-info/requires.txt
--rw-r--r--   0 maik      (1000) maik      (1000)       27 2023-10-31 10:04:07.000000 bobtemplates.plone-6.3.1/bobtemplates.plone.egg-info/top_level.txt
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.613396 bobtemplates.plone-6.3.1/docs/
--rw-r--r--   0 maik      (1000) maik      (1000)     8108 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/docs/Makefile
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.613396 bobtemplates.plone-6.3.1/docs/_static/
--rw-r--r--   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/docs/_static/dummy
--rw-r--r--   0 maik      (1000) maik      (1000)     9479 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/docs/conf.py
--rw-r--r--   0 maik      (1000) maik      (1000)     8939 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/docs/develop.rst
--rw-r--r--   0 maik      (1000) maik      (1000)     1934 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/docs/git-support.rst
--rw-r--r--   0 maik      (1000) maik      (1000)      381 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/docs/index.rst
--rw-r--r--   0 maik      (1000) maik      (1000)     7754 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/docs/make.bat
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.613396 bobtemplates.plone-6.3.1/docs/templates/
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.613396 bobtemplates.plone-6.3.1/docs/templates/addon/
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.613396 bobtemplates.plone-6.3.1/docs/templates/addon/behavior/
--rw-r--r--   0 maik      (1000) maik      (1000)      734 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/docs/templates/addon/behavior/index.rst
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.613396 bobtemplates.plone-6.3.1/docs/templates/addon/content_type/
--rw-r--r--   0 maik      (1000) maik      (1000)     5111 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/docs/templates/addon/content_type/index.rst
--rw-r--r--   0 maik      (1000) maik      (1000)     4328 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/docs/templates/addon/index.rst
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.613396 bobtemplates.plone-6.3.1/docs/templates/addon/indexer/
--rw-r--r--   0 maik      (1000) maik      (1000)     1987 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/docs/templates/addon/indexer/index.rst
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.613396 bobtemplates.plone-6.3.1/docs/templates/addon/portlet/
--rw-r--r--   0 maik      (1000) maik      (1000)     2300 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/docs/templates/addon/portlet/index.rst
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.613396 bobtemplates.plone-6.3.1/docs/templates/addon/restapi_service/
--rw-r--r--   0 maik      (1000) maik      (1000)      690 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/docs/templates/addon/restapi_service/index.rst
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.613396 bobtemplates.plone-6.3.1/docs/templates/addon/subscriber/
--rw-r--r--   0 maik      (1000) maik      (1000)     2043 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/docs/templates/addon/subscriber/index.rst
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.617396 bobtemplates.plone-6.3.1/docs/templates/addon/svelte_app/
--rw-r--r--   0 maik      (1000) maik      (1000)    55910 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/docs/templates/addon/svelte_app/html-filter-settings.png
--rw-r--r--   0 maik      (1000) maik      (1000)     4716 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/docs/templates/addon/svelte_app/index.rst
--rw-r--r--   0 maik      (1000) maik      (1000)    27390 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/docs/templates/addon/svelte_app/tinymce-advanced-settings.png
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.617396 bobtemplates.plone-6.3.1/docs/templates/addon/theme/
--rw-r--r--   0 maik      (1000) maik      (1000)     1697 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/docs/templates/addon/theme/index.rst
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.617396 bobtemplates.plone-6.3.1/docs/templates/addon/theme_barceloneta/
--rw-r--r--   0 maik      (1000) maik      (1000)     2175 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/docs/templates/addon/theme_barceloneta/index.rst
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.617396 bobtemplates.plone-6.3.1/docs/templates/addon/view/
--rw-r--r--   0 maik      (1000) maik      (1000)     2482 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/docs/templates/addon/view/index.rst
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.617396 bobtemplates.plone-6.3.1/docs/templates/addon/viewlet/
--rw-r--r--   0 maik      (1000) maik      (1000)     2462 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/docs/templates/addon/viewlet/index.rst
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.617396 bobtemplates.plone-6.3.1/docs/templates/addon/vocabulary/
--rw-r--r--   0 maik      (1000) maik      (1000)     1052 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/docs/templates/addon/vocabulary/index.rst
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.617396 bobtemplates.plone-6.3.1/docs/templates/buildout/
--rw-r--r--   0 maik      (1000) maik      (1000)     1107 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/docs/templates/buildout/index.rst
--rw-r--r--   0 maik      (1000) maik      (1000)      280 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/docs/templates/index.rst
--rw-r--r--   0 maik      (1000) maik      (1000)     1453 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/docs/upgrade-packages.rst
-drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:07.621396 bobtemplates.plone-6.3.1/package_tests/
--rw-r--r--   0 maik      (1000) maik      (1000)        0 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/package_tests/__init__.py
--rw-r--r--   0 maik      (1000) maik      (1000)     2034 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/package_tests/base.py
--rw-r--r--   0 maik      (1000) maik      (1000)     3388 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/package_tests/test_addon.py
--rw-r--r--   0 maik      (1000) maik      (1000)    13675 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/package_tests/test_base.py
--rw-r--r--   0 maik      (1000) maik      (1000)     2250 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/package_tests/test_behavior.py
--rw-r--r--   0 maik      (1000) maik      (1000)     1332 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/package_tests/test_bobregistry.py
--rw-r--r--   0 maik      (1000) maik      (1000)      438 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/package_tests/test_buildout.py
--rw-r--r--   0 maik      (1000) maik      (1000)    13395 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/package_tests/test_content_type.py
--rw-r--r--   0 maik      (1000) maik      (1000)     5794 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/package_tests/test_form.py
--rw-r--r--   0 maik      (1000) maik      (1000)     3198 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/package_tests/test_indexer.py
--rw-r--r--   0 maik      (1000) maik      (1000)     2194 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/package_tests/test_mockup_pattern.py
--rw-r--r--   0 maik      (1000) maik      (1000)    16782 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/package_tests/test_portlet.py
--rw-r--r--   0 maik      (1000) maik      (1000)     7526 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/package_tests/test_restapi_service.py
--rw-r--r--   0 maik      (1000) maik      (1000)     1743 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/package_tests/test_subscriber.py
--rw-r--r--   0 maik      (1000) maik      (1000)     3944 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/package_tests/test_svelte_app.py
--rw-r--r--   0 maik      (1000) maik      (1000)     3162 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/package_tests/test_theme.py
--rw-r--r--   0 maik      (1000) maik      (1000)     2247 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/package_tests/test_theme_barceloneta.py
--rw-r--r--   0 maik      (1000) maik      (1000)     2181 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/package_tests/test_theme_basic.py
--rw-r--r--   0 maik      (1000) maik      (1000)     5439 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/package_tests/test_upgrade_step.py
--rw-r--r--   0 maik      (1000) maik      (1000)    15448 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/package_tests/test_view.py
--rw-r--r--   0 maik      (1000) maik      (1000)    14572 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/package_tests/test_viewlet.py
--rw-r--r--   0 maik      (1000) maik      (1000)     2247 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/package_tests/test_vocabulary.py
--rw-r--r--   0 maik      (1000) maik      (1000)      732 2023-10-31 10:04:07.625396 bobtemplates.plone-6.3.1/setup.cfg
--rw-r--r--   0 maik      (1000) maik      (1000)     3831 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/setup.py
--rw-r--r--   0 maik      (1000) maik      (1000)     4807 2023-10-31 10:04:06.000000 bobtemplates.plone-6.3.1/tox.ini
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:09.020470 bobtemplates.plone-6.3.2/
+-rw-r--r--   0 maik      (1000) maik      (1000)    34676 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/CHANGES.rst
+-rw-r--r--   0 maik      (1000) maik      (1000)      720 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/CONTRIBUTORS.rst
+-rw-r--r--   0 maik      (1000) maik      (1000)    18092 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/LICENSE.GPL
+-rw-r--r--   0 maik      (1000) maik      (1000)      665 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/LICENSE.rst
+-rw-r--r--   0 maik      (1000) maik      (1000)      299 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/MANIFEST.in
+-rw-r--r--   0 maik      (1000) maik      (1000)    42804 2024-05-07 17:22:09.020470 bobtemplates.plone-6.3.2/PKG-INFO
+-rw-r--r--   0 maik      (1000) maik      (1000)     5751 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/README.rst
+-rw-r--r--   0 maik      (1000) maik      (1000)      980 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/TODO.rst
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.976469 bobtemplates.plone-6.3.2/bobtemplates/
+-rw-r--r--   0 maik      (1000) maik      (1000)       80 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/__init__.py
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.980469 bobtemplates.plone-6.3.2/bobtemplates/plone/
+-rw-r--r--   0 maik      (1000) maik      (1000)       80 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/__init__.py
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.984470 bobtemplates.plone-6.3.2/bobtemplates/plone/addon/
+-rw-r--r--   0 maik      (1000) maik      (1000)       91 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/addon/.coveragerc.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)      245 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/addon/.editorconfig
+-rw-r--r--   0 maik      (1000) maik      (1000)       23 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/addon/.gitattributes
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.984470 bobtemplates.plone-6.3.2/bobtemplates/plone/addon/.github/
+-rw-r--r--   0 maik      (1000) maik      (1000)      366 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/addon/.github/ISSUE_TEMPLATE.md.bob
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.984470 bobtemplates.plone-6.3.2/bobtemplates/plone/addon/.github/workflows/
+-rw-r--r--   0 maik      (1000) maik      (1000)     2578 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/addon/.github/workflows/plone-package.yml.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)      380 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/addon/.gitignore.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)     1880 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/addon/.gitlab-ci.yml
+-rw-r--r--   0 maik      (1000) maik      (1000)     2233 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/addon/.mrbob.ini
+-rw-r--r--   0 maik      (1000) maik      (1000)     1651 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/addon/.travis.yml.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)      111 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/addon/CHANGES.rst.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)       71 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/addon/CONTRIBUTORS.rst.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)     1338 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/addon/DEVELOP.rst
+-rw-r--r--   0 maik      (1000) maik      (1000)    18092 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/addon/LICENSE.GPL.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)      690 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/addon/LICENSE.rst.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)      140 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/addon/MANIFEST.in.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)     3026 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/addon/README.rst.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)     2167 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/addon/base.cfg.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)      130 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/addon/bobtemplate.cfg.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)      215 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/addon/buildout.cfg
+-rw-r--r--   0 maik      (1000) maik      (1000)       27 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/addon/constraints.txt
+-rw-r--r--   0 maik      (1000) maik      (1000)      155 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/addon/constraints_plone52.txt
+-rw-r--r--   0 maik      (1000) maik      (1000)      424 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/addon/constraints_plone60.txt
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.984470 bobtemplates.plone-6.3.2/bobtemplates/plone/addon/docs/
+-rw-r--r--   0 maik      (1000) maik      (1000)     7997 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/addon/docs/conf.py.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)      169 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/addon/docs/index.rst.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)       28 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/addon/requirements.txt
+-rw-r--r--   0 maik      (1000) maik      (1000)       50 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/addon/requirements_plone52.txt
+-rw-r--r--   0 maik      (1000) maik      (1000)       50 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/addon/requirements_plone60.txt
+-rw-r--r--   0 maik      (1000) maik      (1000)      408 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/addon/setup.cfg.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)     2589 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/addon/setup.py.bob
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.968469 bobtemplates.plone-6.3.2/bobtemplates/plone/addon/src/
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.984470 bobtemplates.plone-6.3.2/bobtemplates/plone/addon/src/+package.namespace+/
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.984470 bobtemplates.plone-6.3.2/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/
+-rw-r--r--   0 maik      (1000) maik      (1000)      143 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/__init__.py.bob
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.984470 bobtemplates.plone-6.3.2/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/browser/
+-rw-r--r--   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/browser/__init__.py
+-rw-r--r--   0 maik      (1000) maik      (1000)      620 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/browser/configure.zcml.bob
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.984470 bobtemplates.plone-6.3.2/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/browser/overrides/
+-rw-r--r--   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/browser/overrides/.gitkeep
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.984470 bobtemplates.plone-6.3.2/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/browser/static/
+-rw-r--r--   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/browser/static/.gitkeep
+-rw-r--r--   0 maik      (1000) maik      (1000)     1521 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/configure.zcml.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)      273 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/interfaces.py.bob
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.984470 bobtemplates.plone-6.3.2/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/locales/
+-rw-r--r--   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/locales/+package.dottedname+.pot
+-rw-r--r--   0 maik      (1000) maik      (1000)      611 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/locales/README.rst.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/locales/__init__.py
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.968469 bobtemplates.plone-6.3.2/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/locales/en/
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.984470 bobtemplates.plone-6.3.2/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/locales/en/LC_MESSAGES/
+-rw-r--r--   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/locales/en/LC_MESSAGES/+package.dottedname+.po.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)     1806 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/locales/update.py.bob
+-rwxr-xr-x   0 maik      (1000) maik      (1000)      515 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/locales/update.sh.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)      260 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/permissions.zcml.bob
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.968469 bobtemplates.plone-6.3.2/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/profiles/
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.988469 bobtemplates.plone-6.3.2/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/profiles/default/
+-rw-r--r--   0 maik      (1000) maik      (1000)      202 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/profiles/default/browserlayer.xml.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)      105 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/profiles/default/catalog.xml.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)      195 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/profiles/default/metadata.xml.bob
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.988469 bobtemplates.plone-6.3.2/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/profiles/default/registry/
+-rw-r--r--   0 maik      (1000) maik      (1000)      184 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/profiles/default/registry/main.xml.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)      118 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/profiles/default/rolemap.xml.bob
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.988469 bobtemplates.plone-6.3.2/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/profiles/uninstall/
+-rw-r--r--   0 maik      (1000) maik      (1000)      136 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/profiles/uninstall/browserlayer.xml.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)      803 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/setuphandlers.py.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)     1973 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/testing.py.bob
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.988469 bobtemplates.plone-6.3.2/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/tests/
+-rw-r--r--   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/tests/__init__.py
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.988469 bobtemplates.plone-6.3.2/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/tests/robot/
+-rw-r--r--   0 maik      (1000) maik      (1000)     2037 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/tests/robot/test_example.robot.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)      916 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/tests/test_robot.py.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)     2596 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/tests/test_setup.py.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)       80 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/addon/src/+package.namespace+/__init__.py
+-rw-r--r--   0 maik      (1000) maik      (1000)      344 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/addon/test_plone52.cfg
+-rw-r--r--   0 maik      (1000) maik      (1000)      298 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/addon/test_plone60.cfg
+-rw-r--r--   0 maik      (1000) maik      (1000)     3756 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/addon/tox.ini
+-rw-r--r--   0 maik      (1000) maik      (1000)     4404 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/addon.py
+-rw-r--r--   0 maik      (1000) maik      (1000)    16854 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/base.py
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.988469 bobtemplates.plone-6.3.2/bobtemplates/plone/behavior/
+-rw-r--r--   0 maik      (1000) maik      (1000)     1195 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/behavior/.mrbob.ini
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.988469 bobtemplates.plone-6.3.2/bobtemplates/plone/behavior/behaviors/
+-rw-r--r--   0 maik      (1000) maik      (1000)     1103 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/behavior/behaviors/+behavior_name_normalized+.py.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/behavior/behaviors/__init__.py
+-rw-r--r--   0 maik      (1000) maik      (1000)      342 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/behavior/behaviors/configure.zcml.example.bob
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.988469 bobtemplates.plone-6.3.2/bobtemplates/plone/behavior/tests/
+-rw-r--r--   0 maik      (1000) maik      (1000)     1008 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/behavior/tests/test_behavior_+behavior_name_normalized+.py.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)     4830 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/behavior.py
+-rw-r--r--   0 maik      (1000) maik      (1000)     3842 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/bobregistry.py
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.988469 bobtemplates.plone-6.3.2/bobtemplates/plone/buildout/
+-rw-r--r--   0 maik      (1000) maik      (1000)      422 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/buildout/.gitignore
+-rw-r--r--   0 maik      (1000) maik      (1000)     1743 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/buildout/.mrbob.ini
+-rw-r--r--   0 maik      (1000) maik      (1000)     8167 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/buildout/base.cfg.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)       91 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/buildout/bobtemplate.cfg.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)      777 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/buildout/buildout.cfg.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)       73 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/buildout/constraints.txt.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)       42 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/buildout/requirements.txt
+-rw-r--r--   0 maik      (1000) maik      (1000)      163 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/buildout.py
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.988469 bobtemplates.plone-6.3.2/bobtemplates/plone/content_type/
+-rw-r--r--   0 maik      (1000) maik      (1000)     4940 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/content_type/.mrbob.ini
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.988469 bobtemplates.plone-6.3.2/bobtemplates/plone/content_type/content/
+-rw-r--r--   0 maik      (1000) maik      (1000)     2498 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/content_type/content/+dexterity_type_name_normalized+.py.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)      326 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/content_type/content/+dexterity_type_name_normalized+.xml.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/content_type/content/__init__.py
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.968469 bobtemplates.plone-6.3.2/bobtemplates/plone/content_type/profiles/
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.988469 bobtemplates.plone-6.3.2/bobtemplates/plone/content_type/profiles/default/
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.988469 bobtemplates.plone-6.3.2/bobtemplates/plone/content_type/profiles/default/types/
+-rw-r--r--   0 maik      (1000) maik      (1000)     5305 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/content_type/profiles/default/types/+dexterity_type_fti_file_name+.xml.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)      238 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/content_type/profiles/default/types.xml.example.bob
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.988469 bobtemplates.plone-6.3.2/bobtemplates/plone/content_type/tests/
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.988469 bobtemplates.plone-6.3.2/bobtemplates/plone/content_type/tests/robot/
+-rw-r--r--   0 maik      (1000) maik      (1000)     3840 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/content_type/tests/robot/test_ct_+dexterity_type_name_normalized+.robot.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)     7810 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/content_type/tests/test_ct_+dexterity_type_name_normalized+.py.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)    10184 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/content_type.py
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.988469 bobtemplates.plone-6.3.2/bobtemplates/plone/controlpanel/
+-rw-r--r--   0 maik      (1000) maik      (1000)     1040 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/controlpanel/.mrbob.ini
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.988469 bobtemplates.plone-6.3.2/bobtemplates/plone/controlpanel/controlpanels/
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.988469 bobtemplates.plone-6.3.2/bobtemplates/plone/controlpanel/controlpanels/+controlpanel_name_normalized+/
+-rw-r--r--   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/controlpanel/controlpanels/+controlpanel_name_normalized+/__init__.py.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)      759 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/controlpanel/controlpanels/+controlpanel_name_normalized+/configure.zcml.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)     1625 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/controlpanel/controlpanels/+controlpanel_name_normalized+/controlpanel.py.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/controlpanel/controlpanels/__init__.py.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)      264 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/controlpanel/controlpanels/configure.zcml.example.bob
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.968469 bobtemplates.plone-6.3.2/bobtemplates/plone/controlpanel/profiles/
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.988469 bobtemplates.plone-6.3.2/bobtemplates/plone/controlpanel/profiles/default/
+-rw-r--r--   0 maik      (1000) maik      (1000)      207 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/controlpanel/profiles/default/controlpanel.xml.example.bob
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.992469 bobtemplates.plone-6.3.2/bobtemplates/plone/controlpanel/profiles/default/registry/
+-rw-r--r--   0 maik      (1000) maik      (1000)      420 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/controlpanel/profiles/default/registry/+controlpanel_name_normalized+.xml.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)     5516 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/controlpanel.py
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.992469 bobtemplates.plone-6.3.2/bobtemplates/plone/form/
+-rw-r--r--   0 maik      (1000) maik      (1000)     1570 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/form/.mrbob.ini
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.992469 bobtemplates.plone-6.3.2/bobtemplates/plone/form/forms/
+-rw-r--r--   0 maik      (1000) maik      (1000)     1280 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/form/forms/+form_python_file_name+.py.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/form/forms/__init__.py
+-rw-r--r--   0 maik      (1000) maik      (1000)      263 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/form/forms/configure.zcml.example.bob
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.992469 bobtemplates.plone-6.3.2/bobtemplates/plone/form/tests/
+-rw-r--r--   0 maik      (1000) maik      (1000)     1568 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/form/tests/test_form_+form_name_normalized+.py.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)     6386 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/form.py
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.992469 bobtemplates.plone-6.3.2/bobtemplates/plone/indexer/
+-rw-r--r--   0 maik      (1000) maik      (1000)      876 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/indexer/.mrbob.ini
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.992469 bobtemplates.plone-6.3.2/bobtemplates/plone/indexer/indexers/
+-rw-r--r--   0 maik      (1000) maik      (1000)      513 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/indexer/indexers/+indexer_file_name+.py.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)      261 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/indexer/indexers/+indexer_file_name+.zcml.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/indexer/indexers/__init__.py
+-rw-r--r--   0 maik      (1000) maik      (1000)      157 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/indexer/indexers/configure.zcml.example.bob
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.992469 bobtemplates.plone-6.3.2/bobtemplates/plone/indexer/tests/
+-rw-r--r--   0 maik      (1000) maik      (1000)      888 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/indexer/tests/test_indexer_+indexer_file_name+.py.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)     2838 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/indexer.py
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.992469 bobtemplates.plone-6.3.2/bobtemplates/plone/mockup_pattern/
+-rw-r--r--   0 maik      (1000) maik      (1000)       59 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/mockup_pattern/.eslintrc.js
+-rw-r--r--   0 maik      (1000) maik      (1000)      610 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/mockup_pattern/.mrbob.ini
+-rw-r--r--   0 maik      (1000) maik      (1000)       28 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/mockup_pattern/.prettierignore
+-rw-r--r--   0 maik      (1000) maik      (1000)       61 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/mockup_pattern/.release-it.js
+-rw-r--r--   0 maik      (1000) maik      (1000)       62 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/mockup_pattern/babel.config.js
+-rw-r--r--   0 maik      (1000) maik      (1000)      132 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/mockup_pattern/jest.config.js
+-rw-r--r--   0 maik      (1000) maik      (1000)      702 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/mockup_pattern/package.json.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)       65 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/mockup_pattern/prettier.config.js
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.992469 bobtemplates.plone-6.3.2/bobtemplates/plone/mockup_pattern/resources/
+-rw-r--r--   0 maik      (1000) maik      (1000)      169 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/mockup_pattern/resources/bundle.js.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)      252 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/mockup_pattern/resources/index.html.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)      113 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/mockup_pattern/resources/index.js
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.992469 bobtemplates.plone-6.3.2/bobtemplates/plone/mockup_pattern/resources/pat-+pattern.name+/
+-rw-r--r--   0 maik      (1000) maik      (1000)     1356 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/mockup_pattern/resources/pat-+pattern.name+/+pattern.name+.js.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)      117 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/mockup_pattern/resources/pat-+pattern.name+/+pattern.name+.scss.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)     1277 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/mockup_pattern/resources/pat-+pattern.name+/+pattern.name+.test.js.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)      481 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/mockup_pattern/resources/pat-+pattern.name+/documentation.md.bob
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.968469 bobtemplates.plone-6.3.2/bobtemplates/plone/mockup_pattern/src/
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.968469 bobtemplates.plone-6.3.2/bobtemplates/plone/mockup_pattern/src/+package.namespace+/
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.968469 bobtemplates.plone-6.3.2/bobtemplates/plone/mockup_pattern/src/+package.namespace+/+package.name+/
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.992469 bobtemplates.plone-6.3.2/bobtemplates/plone/mockup_pattern/src/+package.namespace+/+package.name+/browser/
+-rw-r--r--   0 maik      (1000) maik      (1000)      199 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/mockup_pattern/src/+package.namespace+/+package.name+/browser/configure.zcml.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)      560 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/mockup_pattern/src/+package.namespace+/+package.name+/browser/pattern-demo.pt.bob
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.968469 bobtemplates.plone-6.3.2/bobtemplates/plone/mockup_pattern/src/+package.namespace+/+package.name+/browser/static/
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.992469 bobtemplates.plone-6.3.2/bobtemplates/plone/mockup_pattern/src/+package.namespace+/+package.name+/browser/static/bundles/
+-rw-r--r--   0 maik      (1000) maik      (1000)       68 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/mockup_pattern/src/+package.namespace+/+package.name+/browser/static/bundles/.gitkeep
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.968469 bobtemplates.plone-6.3.2/bobtemplates/plone/mockup_pattern/src/+package.namespace+/+package.name+/profiles/
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.968469 bobtemplates.plone-6.3.2/bobtemplates/plone/mockup_pattern/src/+package.namespace+/+package.name+/profiles/default/
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.992469 bobtemplates.plone-6.3.2/bobtemplates/plone/mockup_pattern/src/+package.namespace+/+package.name+/profiles/default/registry/
+-rw-r--r--   0 maik      (1000) maik      (1000)      361 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/mockup_pattern/src/+package.namespace+/+package.name+/profiles/default/registry/bundles.xml.bob
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.968469 bobtemplates.plone-6.3.2/bobtemplates/plone/mockup_pattern/src/+package.namespace+/+package.name+/profiles/uninstall/
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.992469 bobtemplates.plone-6.3.2/bobtemplates/plone/mockup_pattern/src/+package.namespace+/+package.name+/profiles/uninstall/registry/
+-rw-r--r--   0 maik      (1000) maik      (1000)      198 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/mockup_pattern/src/+package.namespace+/+package.name+/profiles/uninstall/registry/bundles.xml.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)     1495 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/mockup_pattern/webpack.config.js.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)     3836 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/mockup_pattern.py
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.992469 bobtemplates.plone-6.3.2/bobtemplates/plone/portlet/
+-rw-r--r--   0 maik      (1000) maik      (1000)      916 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/portlet/.mrbob.ini
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.996469 bobtemplates.plone-6.3.2/bobtemplates/plone/portlet/portlets/
+-rw-r--r--   0 maik      (1000) maik      (1000)      265 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/portlet/portlets/+portlet_name_normalized+.pt.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)     3583 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/portlet/portlets/+portlet_name_normalized+.py.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/portlet/portlets/__init__.py
+-rw-r--r--   0 maik      (1000) maik      (1000)      259 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/portlet/portlets/configure.zcml.example.bob
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.968469 bobtemplates.plone-6.3.2/bobtemplates/plone/portlet/profiles/
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.996469 bobtemplates.plone-6.3.2/bobtemplates/plone/portlet/profiles/default/
+-rw-r--r--   0 maik      (1000) maik      (1000)      159 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/portlet/profiles/default/portlets.xml.example.bob
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.996469 bobtemplates.plone-6.3.2/bobtemplates/plone/portlet/tests/
+-rw-r--r--   0 maik      (1000) maik      (1000)     1202 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/portlet/tests/test_+portlet_name_normalized+.py.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)     7462 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/portlet.py
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.996469 bobtemplates.plone-6.3.2/bobtemplates/plone/restapi_service/
+-rw-r--r--   0 maik      (1000) maik      (1000)     1236 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/restapi_service/.mrbob.ini
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.996469 bobtemplates.plone-6.3.2/bobtemplates/plone/restapi_service/api/
+-rw-r--r--   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/restapi_service/api/__init__.py
+-rw-r--r--   0 maik      (1000) maik      (1000)      265 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/restapi_service/api/configure.zcml.example.bob
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.996469 bobtemplates.plone-6.3.2/bobtemplates/plone/restapi_service/api/services/
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.996469 bobtemplates.plone-6.3.2/bobtemplates/plone/restapi_service/api/services/+service_class_name_normalized+/
+-rw-r--r--   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/restapi_service/api/services/+service_class_name_normalized+/__init__.py
+-rw-r--r--   0 maik      (1000) maik      (1000)      417 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/restapi_service/api/services/+service_class_name_normalized+/configure.zcml.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)     1845 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/restapi_service/api/services/+service_class_name_normalized+/get.py.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/restapi_service/api/services/__init__.py
+-rw-r--r--   0 maik      (1000) maik      (1000)      265 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/restapi_service/api/services/configure.zcml.example.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)     5585 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/restapi_service.py
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.996469 bobtemplates.plone-6.3.2/bobtemplates/plone/site_initialization/
+-rw-r--r--   0 maik      (1000) maik      (1000)     1008 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/site_initialization/.mrbob.ini
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.972469 bobtemplates.plone-6.3.2/bobtemplates/plone/site_initialization/profiles/
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.972469 bobtemplates.plone-6.3.2/bobtemplates/plone/site_initialization/profiles/default/
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.996469 bobtemplates.plone-6.3.2/bobtemplates/plone/site_initialization/profiles/default/registry/
+-rw-r--r--   0 maik      (1000) maik      (1000)      234 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/site_initialization/profiles/default/registry/plone.base.interfaces.controlpanel.IMailSchema.xml.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)      229 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/site_initialization/profiles/default/registry/plone.base.interfaces.controlpanel.ISiteSchema.xml.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)      318 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/site_initialization/profiles/default/registry/plone.i18n.interfaces.ILanguageSchema.xml.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)      528 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/site_initialization.py
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.996469 bobtemplates.plone-6.3.2/bobtemplates/plone/subscriber/
+-rw-r--r--   0 maik      (1000) maik      (1000)     1097 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/subscriber/.mrbob.ini
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.996469 bobtemplates.plone-6.3.2/bobtemplates/plone/subscriber/subscribers/
+-rw-r--r--   0 maik      (1000) maik      (1000)      157 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/subscriber/subscribers/+subscriber_handler_file_name+.py.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/subscriber/subscribers/__init__.py
+-rw-r--r--   0 maik      (1000) maik      (1000)      157 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/subscriber/subscribers/configure.zcml.example.bob
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.996469 bobtemplates.plone-6.3.2/bobtemplates/plone/subscriber/tests/
+-rw-r--r--   0 maik      (1000) maik      (1000)      780 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/subscriber/tests/test_subscriber_+subscriber_handler_file_name+.py.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)     3010 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/subscriber.py
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.996469 bobtemplates.plone-6.3.2/bobtemplates/plone/svelte_app/
+-rw-r--r--   0 maik      (1000) maik      (1000)     1533 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/svelte_app/.mrbob.ini
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.972469 bobtemplates.plone-6.3.2/bobtemplates/plone/svelte_app/src/
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.972469 bobtemplates.plone-6.3.2/bobtemplates/plone/svelte_app/src/+package.namespace+/
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.972469 bobtemplates.plone-6.3.2/bobtemplates/plone/svelte_app/src/+package.namespace+/+package.name+/
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.972469 bobtemplates.plone-6.3.2/bobtemplates/plone/svelte_app/src/+package.namespace+/+package.name+/profiles/
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.972469 bobtemplates.plone-6.3.2/bobtemplates/plone/svelte_app/src/+package.namespace+/+package.name+/profiles/default/
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.996469 bobtemplates.plone-6.3.2/bobtemplates/plone/svelte_app/src/+package.namespace+/+package.name+/profiles/default/registry/
+-rw-r--r--   0 maik      (1000) maik      (1000)     1468 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/svelte_app/src/+package.namespace+/+package.name+/profiles/default/registry/+svelte_app_file_name+.xml.bob
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.972469 bobtemplates.plone-6.3.2/bobtemplates/plone/svelte_app/src/+package.namespace+/+package.name+/profiles/uninstall/
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.996469 bobtemplates.plone-6.3.2/bobtemplates/plone/svelte_app/src/+package.namespace+/+package.name+/profiles/uninstall/registry/
+-rw-r--r--   0 maik      (1000) maik      (1000)      539 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/svelte_app/src/+package.namespace+/+package.name+/profiles/uninstall/registry/+svelte_app_file_name+.xml.bob
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.972469 bobtemplates.plone-6.3.2/bobtemplates/plone/svelte_app/src/+package.namespace+/+package.name+/svelte_apps/
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.996469 bobtemplates.plone-6.3.2/bobtemplates/plone/svelte_app/src/+package.namespace+/+package.name+/svelte_apps/+svelte_app_name_dashed+/
+-rw-r--r--   0 maik      (1000) maik      (1000)      315 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/svelte_app/src/+package.namespace+/+package.name+/svelte_apps/+svelte_app_name_dashed+/README.md.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)     3127 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/svelte_app/src/+package.namespace+/+package.name+/svelte_apps/+svelte_app_name_dashed+/favicon.png
+-rw-r--r--   0 maik      (1000) maik      (1000)      890 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/svelte_app/src/+package.namespace+/+package.name+/svelte_apps/+svelte_app_name_dashed+/global.css
+-rw-r--r--   0 maik      (1000) maik      (1000)      531 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/svelte_app/src/+package.namespace+/+package.name+/svelte_apps/+svelte_app_name_dashed+/index.html.bob
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.972469 bobtemplates.plone-6.3.2/bobtemplates/plone/svelte_app/svelte_src/
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.996469 bobtemplates.plone-6.3.2/bobtemplates/plone/svelte_app/svelte_src/+svelte_app_name_dashed+/
+-rw-r--r--   0 maik      (1000) maik      (1000)       41 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/svelte_app/svelte_src/+svelte_app_name_dashed+/.gitignore
+-rw-r--r--   0 maik      (1000) maik      (1000)     2270 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/svelte_app/svelte_src/+svelte_app_name_dashed+/README.md.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)      516 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/svelte_app/svelte_src/+svelte_app_name_dashed+/package.json
+-rw-r--r--   0 maik      (1000) maik      (1000)     2397 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/svelte_app/svelte_src/+svelte_app_name_dashed+/rollup.config.js.bob
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.996469 bobtemplates.plone-6.3.2/bobtemplates/plone/svelte_app/svelte_src/+svelte_app_name_dashed+/scripts/
+-rw-r--r--   0 maik      (1000) maik      (1000)     4292 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/svelte_app/svelte_src/+svelte_app_name_dashed+/scripts/setupTypeScript.js
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.996469 bobtemplates.plone-6.3.2/bobtemplates/plone/svelte_app/svelte_src/+svelte_app_name_dashed+/src/
+-rw-r--r--   0 maik      (1000) maik      (1000)      826 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/svelte_app/svelte_src/+svelte_app_name_dashed+/src/App.svelte.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)      613 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/svelte_app/svelte_src/+svelte_app_name_dashed+/src/main.js.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)     2979 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/svelte_app.py
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:09.000469 bobtemplates.plone-6.3.2/bobtemplates/plone/theme/
+-rw-r--r--   0 maik      (1000) maik      (1000)     1020 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/theme/.mrbob.ini
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.972469 bobtemplates.plone-6.3.2/bobtemplates/plone/theme/profiles/
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:09.000469 bobtemplates.plone-6.3.2/bobtemplates/plone/theme/profiles/default/
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:09.000469 bobtemplates.plone-6.3.2/bobtemplates/plone/theme/profiles/default/registry/
+-rw-r--r--   0 maik      (1000) maik      (1000)      387 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/theme/profiles/default/registry/displayed_types.xml
+-rw-r--r--   0 maik      (1000) maik      (1000)      460 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/theme/profiles/default/registry/email_from.xml
+-rw-r--r--   0 maik      (1000) maik      (1000)     2320 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/theme/profiles/default/registry/main.xml
+-rw-r--r--   0 maik      (1000) maik      (1000)      309 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/theme/profiles/default/registry/nonfolderish_tabs.xml
+-rw-r--r--   0 maik      (1000) maik      (1000)     2263 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/theme/profiles/default/registry/tinymce.xml
+-rw-r--r--   0 maik      (1000) maik      (1000)      127 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/theme/profiles/default/theme.xml.bob
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:09.000469 bobtemplates.plone-6.3.2/bobtemplates/plone/theme/profiles/uninstall/
+-rw-r--r--   0 maik      (1000) maik      (1000)      109 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/theme/profiles/uninstall/theme.xml.bob
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:09.000469 bobtemplates.plone-6.3.2/bobtemplates/plone/theme/theme/
+-rw-r--r--   0 maik      (1000) maik      (1000)     3008 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/theme/theme/README.rst.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)      174 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/theme/theme/index.html
+-rw-r--r--   0 maik      (1000) maik      (1000)      529 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/theme/theme/manifest.cfg.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)     1620 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/theme/theme/package.json.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)     6091 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/theme/theme/rules.xml.bob
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:09.000469 bobtemplates.plone-6.3.2/bobtemplates/plone/theme/theme/styles/
+-rw-r--r--   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/theme/theme/styles/theme.min.css
+-rw-r--r--   0 maik      (1000) maik      (1000)      638 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/theme/theme/styles/theme.scss
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:09.000469 bobtemplates.plone-6.3.2/bobtemplates/plone/theme/theme/tinymce-templates/
+-rw-r--r--   0 maik      (1000) maik      (1000)      808 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/theme/theme/tinymce-templates/bs-dark-hero.html
+-rw-r--r--   0 maik      (1000) maik      (1000)      951 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/theme/theme/tinymce-templates/bs-hero-left.html
+-rw-r--r--   0 maik      (1000) maik      (1000)     2049 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/theme/theme/tinymce-templates/bs-pricing.html
+-rw-r--r--   0 maik      (1000) maik      (1000)     5141 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/theme.py
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:09.000469 bobtemplates.plone-6.3.2/bobtemplates/plone/theme_barceloneta/
+-rw-r--r--   0 maik      (1000) maik      (1000)     1056 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/theme_barceloneta/.mrbob.ini
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.972469 bobtemplates.plone-6.3.2/bobtemplates/plone/theme_barceloneta/src/
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.972469 bobtemplates.plone-6.3.2/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.972469 bobtemplates.plone-6.3.2/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.972469 bobtemplates.plone-6.3.2/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/profiles/
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:09.000469 bobtemplates.plone-6.3.2/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/profiles/default/
+-rw-r--r--   0 maik      (1000) maik      (1000)      127 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/profiles/default/theme.xml.bob
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:09.000469 bobtemplates.plone-6.3.2/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/profiles/uninstall/
+-rw-r--r--   0 maik      (1000) maik      (1000)      109 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/profiles/uninstall/theme.xml
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:09.004469 bobtemplates.plone-6.3.2/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/
+-rw-r--r--   0 maik      (1000) maik      (1000)     2769 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/README.rst.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)     2112 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/barceloneta-apple-touch-icon-114x114-precomposed.png
+-rw-r--r--   0 maik      (1000) maik      (1000)     2382 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/barceloneta-apple-touch-icon-144x144-precomposed.png
+-rw-r--r--   0 maik      (1000) maik      (1000)     1090 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/barceloneta-apple-touch-icon-57x57-precomposed.png
+-rw-r--r--   0 maik      (1000) maik      (1000)     1414 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/barceloneta-apple-touch-icon-72x72-precomposed.png
+-rw-r--r--   0 maik      (1000) maik      (1000)     1090 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/barceloneta-apple-touch-icon-precomposed.png
+-rw-r--r--   0 maik      (1000) maik      (1000)     4303 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/barceloneta-apple-touch-icon.png
+-rw-r--r--   0 maik      (1000) maik      (1000)     5430 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/barceloneta-favicon.ico
+-rw-r--r--   0 maik      (1000) maik      (1000)     3854 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/index.html
+-rw-r--r--   0 maik      (1000) maik      (1000)      647 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/manifest.cfg.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)     1356 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/package.json.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)    89929 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/preview.png
+-rw-r--r--   0 maik      (1000) maik      (1000)     7236 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/rules.xml
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:09.004469 bobtemplates.plone-6.3.2/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/scss/
+-rw-r--r--   0 maik      (1000) maik      (1000)      120 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/scss/_custom.scss
+-rw-r--r--   0 maik      (1000) maik      (1000)      273 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/scss/_maps.scss
+-rw-r--r--   0 maik      (1000) maik      (1000)       60 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/scss/_variables.scss
+-rw-r--r--   0 maik      (1000) maik      (1000)     3996 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/scss/theme.scss
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:09.004469 bobtemplates.plone-6.3.2/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/styles/
+-rw-r--r--   0 maik      (1000) maik      (1000)   708963 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/styles/theme.css
+-rw-r--r--   0 maik      (1000) maik      (1000)   242413 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/styles/theme.min.css
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:09.004469 bobtemplates.plone-6.3.2/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/tinymce-templates/
+-rw-r--r--   0 maik      (1000) maik      (1000)      732 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/tinymce-templates/README.rst.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)     1352 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/tinymce-templates/card-group.html
+-rw-r--r--   0 maik      (1000) maik      (1000)      313 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/tinymce-templates/list.html
+-rw-r--r--   0 maik      (1000) maik      (1000)     5104 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/theme_barceloneta.py
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:09.004469 bobtemplates.plone-6.3.2/bobtemplates/plone/theme_basic/
+-rw-r--r--   0 maik      (1000) maik      (1000)     1038 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/theme_basic/.mrbob.ini
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.972469 bobtemplates.plone-6.3.2/bobtemplates/plone/theme_basic/src/
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.972469 bobtemplates.plone-6.3.2/bobtemplates/plone/theme_basic/src/+package.namespace+/
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.972469 bobtemplates.plone-6.3.2/bobtemplates/plone/theme_basic/src/+package.namespace+/+package.name+/
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.972469 bobtemplates.plone-6.3.2/bobtemplates/plone/theme_basic/src/+package.namespace+/+package.name+/browser/
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:09.004469 bobtemplates.plone-6.3.2/bobtemplates/plone/theme_basic/src/+package.namespace+/+package.name+/browser/overrides/
+-rw-r--r--   0 maik      (1000) maik      (1000)     1380 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/theme_basic/src/+package.namespace+/+package.name+/browser/overrides/plone.app.layout.viewlets.sections.pt
+-rw-r--r--   0 maik      (1000) maik      (1000)      145 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/theme_basic/src/+package.namespace+/+package.name+/browser/overrides/plone.app.portlets.browser.templates.footer.pt
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.972469 bobtemplates.plone-6.3.2/bobtemplates/plone/theme_basic/src/+package.namespace+/+package.name+/profiles/
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:09.004469 bobtemplates.plone-6.3.2/bobtemplates/plone/theme_basic/src/+package.namespace+/+package.name+/profiles/default/
+-rw-r--r--   0 maik      (1000) maik      (1000)      127 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/theme_basic/src/+package.namespace+/+package.name+/profiles/default/theme.xml.bob
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:09.004469 bobtemplates.plone-6.3.2/bobtemplates/plone/theme_basic/src/+package.namespace+/+package.name+/profiles/uninstall/
+-rw-r--r--   0 maik      (1000) maik      (1000)      111 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/theme_basic/src/+package.namespace+/+package.name+/profiles/uninstall/theme.xml
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:09.008469 bobtemplates.plone-6.3.2/bobtemplates/plone/theme_basic/src/+package.namespace+/+package.name+/theme/
+-rw-r--r--   0 maik      (1000) maik      (1000)     2287 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/theme_basic/src/+package.namespace+/+package.name+/theme/README.rst.bob
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:09.008469 bobtemplates.plone-6.3.2/bobtemplates/plone/theme_basic/src/+package.namespace+/+package.name+/theme/css/
+-rw-r--r--   0 maik      (1000) maik      (1000)   896711 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/theme_basic/src/+package.namespace+/+package.name+/theme/css/theme.css
+-rw-r--r--   0 maik      (1000) maik      (1000)   284809 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/theme_basic/src/+package.namespace+/+package.name+/theme/css/theme.css.map
+-rw-r--r--   0 maik      (1000) maik      (1000)   153028 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/theme_basic/src/+package.namespace+/+package.name+/theme/css/theme.min.css
+-rw-r--r--   0 maik      (1000) maik      (1000)  1139991 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/theme_basic/src/+package.namespace+/+package.name+/theme/css/theme.min.css.map
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:09.012469 bobtemplates.plone-6.3.2/bobtemplates/plone/theme_basic/src/+package.namespace+/+package.name+/theme/js/
+-rw-r--r--   0 maik      (1000) maik      (1000)      192 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/theme_basic/src/+package.namespace+/+package.name+/theme/js/theme.js
+-rw-r--r--   0 maik      (1000) maik      (1000)       65 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/theme_basic/src/+package.namespace+/+package.name+/theme/js/theme.min.js
+-rw-r--r--   0 maik      (1000) maik      (1000)      476 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/theme_basic/src/+package.namespace+/+package.name+/theme/manifest.cfg.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)     1585 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/theme_basic/src/+package.namespace+/+package.name+/theme/package.json.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)     2852 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/theme_basic/src/+package.namespace+/+package.name+/theme/preview.png
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:09.012469 bobtemplates.plone-6.3.2/bobtemplates/plone/theme_basic/src/+package.namespace+/+package.name+/theme/scss/
+-rw-r--r--   0 maik      (1000) maik      (1000)      285 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/theme_basic/src/+package.namespace+/+package.name+/theme/scss/_base.scss
+-rw-r--r--   0 maik      (1000) maik      (1000)      704 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/theme_basic/src/+package.namespace+/+package.name+/theme/scss/theme.scss
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:09.012469 bobtemplates.plone-6.3.2/bobtemplates/plone/theme_basic/src/+package.namespace+/+package.name+/theme/tinymce-templates/
+-rw-r--r--   0 maik      (1000) maik      (1000)     1240 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/theme_basic/src/+package.namespace+/+package.name+/theme/tinymce-templates/README.rst.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)     1352 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/theme_basic/src/+package.namespace+/+package.name+/theme/tinymce-templates/card-group.html
+-rw-r--r--   0 maik      (1000) maik      (1000)      313 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/theme_basic/src/+package.namespace+/+package.name+/theme/tinymce-templates/list.html
+-rw-r--r--   0 maik      (1000) maik      (1000)     4400 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/theme_basic.py
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:09.012469 bobtemplates.plone-6.3.2/bobtemplates/plone/upgrade_step/
+-rw-r--r--   0 maik      (1000) maik      (1000)     1063 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/upgrade_step/.mrbob.ini
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:09.012469 bobtemplates.plone-6.3.2/bobtemplates/plone/upgrade_step/tests/
+-rw-r--r--   0 maik      (1000) maik      (1000)      892 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/upgrade_step/tests/test_upgrade_step_+upgrade_step_id+.py.bob
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:09.012469 bobtemplates.plone-6.3.2/bobtemplates/plone/upgrade_step/upgrades/
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:09.012469 bobtemplates.plone-6.3.2/bobtemplates/plone/upgrade_step/upgrades/+upgrade_step_id+/
+-rw-r--r--   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/upgrade_step/upgrades/+upgrade_step_id+/.gitkeep
+-rw-r--r--   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/upgrade_step/upgrades/+upgrade_step_id+/metadata.txt
+-rw-r--r--   0 maik      (1000) maik      (1000)     1056 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/upgrade_step/upgrades/+upgrade_step_id+.zcml.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)       98 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/upgrade_step/upgrades/__init__.py.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)      218 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/upgrade_step/upgrades/base.py.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)      156 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/upgrade_step/upgrades/configure.zcml.example.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)      262 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/upgrade_step/upgrades/v+upgrade_step_id+.py.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)     4448 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/upgrade_step.py
+-rw-r--r--   0 maik      (1000) maik      (1000)     3251 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/utils.py
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:09.012469 bobtemplates.plone-6.3.2/bobtemplates/plone/view/
+-rw-r--r--   0 maik      (1000) maik      (1000)     3329 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/view/.mrbob.ini
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:09.012469 bobtemplates.plone-6.3.2/bobtemplates/plone/view/tests/
+-rw-r--r--   0 maik      (1000) maik      (1000)     1868 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/view/tests/test_view_+view_python_file_name+.py.bob
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:09.012469 bobtemplates.plone-6.3.2/bobtemplates/plone/view/views/
+-rw-r--r--   0 maik      (1000) maik      (1000)     1443 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/view/views/+view_python_file_name+.py.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)     1058 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/view/views/+view_template_name+.pt.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/view/views/__init__.py
+-rw-r--r--   0 maik      (1000) maik      (1000)      263 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/view/views/configure.zcml.example.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)     9202 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/view.py
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:09.012469 bobtemplates.plone-6.3.2/bobtemplates/plone/viewlet/
+-rw-r--r--   0 maik      (1000) maik      (1000)     1964 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/viewlet/.mrbob.ini
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:09.012469 bobtemplates.plone-6.3.2/bobtemplates/plone/viewlet/tests/
+-rw-r--r--   0 maik      (1000) maik      (1000)     2631 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/viewlet/tests/test_viewlet_+viewlet_name_normalized+.py.bob
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:09.012469 bobtemplates.plone-6.3.2/bobtemplates/plone/viewlet/viewlets/
+-rw-r--r--   0 maik      (1000) maik      (1000)      585 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/viewlet/viewlets/+viewlet_python_file_name+.py.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)       54 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/viewlet/viewlets/+viewlet_template_name+.pt.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/viewlet/viewlets/__init__.py.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)      264 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/viewlet/viewlets/configure.zcml.example.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)     6626 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/viewlet.py
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:09.012469 bobtemplates.plone-6.3.2/bobtemplates/plone/vocabulary/
+-rw-r--r--   0 maik      (1000) maik      (1000)      941 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/vocabulary/.mrbob.ini
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:09.012469 bobtemplates.plone-6.3.2/bobtemplates/plone/vocabulary/tests/
+-rw-r--r--   0 maik      (1000) maik      (1000)     1230 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/vocabulary/tests/test_vocab_+vocabulary_name_normalized+.py.bob
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:09.016469 bobtemplates.plone-6.3.2/bobtemplates/plone/vocabulary/vocabularies/
+-rw-r--r--   0 maik      (1000) maik      (1000)     1696 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/vocabulary/vocabularies/+vocabulary_name_normalized+.py.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/vocabulary/vocabularies/__init__.py
+-rw-r--r--   0 maik      (1000) maik      (1000)      159 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/vocabulary/vocabularies/configure.zcml.example.bob
+-rw-r--r--   0 maik      (1000) maik      (1000)     3995 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates/plone/vocabulary.py
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:09.020470 bobtemplates.plone-6.3.2/bobtemplates.plone.egg-info/
+-rw-r--r--   0 maik      (1000) maik      (1000)    42804 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates.plone.egg-info/PKG-INFO
+-rw-r--r--   0 maik      (1000) maik      (1000)    20892 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates.plone.egg-info/SOURCES.txt
+-rw-r--r--   0 maik      (1000) maik      (1000)        1 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates.plone.egg-info/dependency_links.txt
+-rw-r--r--   0 maik      (1000) maik      (1000)     1352 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates.plone.egg-info/entry_points.txt
+-rw-r--r--   0 maik      (1000) maik      (1000)       13 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates.plone.egg-info/namespace_packages.txt
+-rw-r--r--   0 maik      (1000) maik      (1000)        1 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates.plone.egg-info/not-zip-safe
+-rw-r--r--   0 maik      (1000) maik      (1000)       64 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates.plone.egg-info/requires.txt
+-rw-r--r--   0 maik      (1000) maik      (1000)       27 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/bobtemplates.plone.egg-info/top_level.txt
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:09.016469 bobtemplates.plone-6.3.2/docs/
+-rw-r--r--   0 maik      (1000) maik      (1000)     8108 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/docs/Makefile
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:09.016469 bobtemplates.plone-6.3.2/docs/_static/
+-rw-r--r--   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/docs/_static/dummy
+-rw-r--r--   0 maik      (1000) maik      (1000)     9479 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/docs/conf.py
+-rw-r--r--   0 maik      (1000) maik      (1000)     8939 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/docs/develop.rst
+-rw-r--r--   0 maik      (1000) maik      (1000)     1934 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/docs/git-support.rst
+-rw-r--r--   0 maik      (1000) maik      (1000)      381 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/docs/index.rst
+-rw-r--r--   0 maik      (1000) maik      (1000)     7754 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/docs/make.bat
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:09.016469 bobtemplates.plone-6.3.2/docs/templates/
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:09.016469 bobtemplates.plone-6.3.2/docs/templates/addon/
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:09.016469 bobtemplates.plone-6.3.2/docs/templates/addon/behavior/
+-rw-r--r--   0 maik      (1000) maik      (1000)      734 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/docs/templates/addon/behavior/index.rst
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:09.016469 bobtemplates.plone-6.3.2/docs/templates/addon/content_type/
+-rw-r--r--   0 maik      (1000) maik      (1000)     5111 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/docs/templates/addon/content_type/index.rst
+-rw-r--r--   0 maik      (1000) maik      (1000)     4328 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/docs/templates/addon/index.rst
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:09.016469 bobtemplates.plone-6.3.2/docs/templates/addon/indexer/
+-rw-r--r--   0 maik      (1000) maik      (1000)     1987 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/docs/templates/addon/indexer/index.rst
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:09.016469 bobtemplates.plone-6.3.2/docs/templates/addon/portlet/
+-rw-r--r--   0 maik      (1000) maik      (1000)     2300 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/docs/templates/addon/portlet/index.rst
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:09.016469 bobtemplates.plone-6.3.2/docs/templates/addon/restapi_service/
+-rw-r--r--   0 maik      (1000) maik      (1000)      690 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/docs/templates/addon/restapi_service/index.rst
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:09.016469 bobtemplates.plone-6.3.2/docs/templates/addon/subscriber/
+-rw-r--r--   0 maik      (1000) maik      (1000)     2043 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/docs/templates/addon/subscriber/index.rst
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:09.016469 bobtemplates.plone-6.3.2/docs/templates/addon/svelte_app/
+-rw-r--r--   0 maik      (1000) maik      (1000)    55910 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/docs/templates/addon/svelte_app/html-filter-settings.png
+-rw-r--r--   0 maik      (1000) maik      (1000)     4716 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/docs/templates/addon/svelte_app/index.rst
+-rw-r--r--   0 maik      (1000) maik      (1000)    27390 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/docs/templates/addon/svelte_app/tinymce-advanced-settings.png
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:09.016469 bobtemplates.plone-6.3.2/docs/templates/addon/theme/
+-rw-r--r--   0 maik      (1000) maik      (1000)     1697 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/docs/templates/addon/theme/index.rst
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:09.016469 bobtemplates.plone-6.3.2/docs/templates/addon/theme_barceloneta/
+-rw-r--r--   0 maik      (1000) maik      (1000)     2175 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/docs/templates/addon/theme_barceloneta/index.rst
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:09.016469 bobtemplates.plone-6.3.2/docs/templates/addon/view/
+-rw-r--r--   0 maik      (1000) maik      (1000)     2482 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/docs/templates/addon/view/index.rst
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:09.016469 bobtemplates.plone-6.3.2/docs/templates/addon/viewlet/
+-rw-r--r--   0 maik      (1000) maik      (1000)     2462 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/docs/templates/addon/viewlet/index.rst
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:09.016469 bobtemplates.plone-6.3.2/docs/templates/addon/vocabulary/
+-rw-r--r--   0 maik      (1000) maik      (1000)     1052 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/docs/templates/addon/vocabulary/index.rst
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:09.016469 bobtemplates.plone-6.3.2/docs/templates/buildout/
+-rw-r--r--   0 maik      (1000) maik      (1000)     1107 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/docs/templates/buildout/index.rst
+-rw-r--r--   0 maik      (1000) maik      (1000)      280 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/docs/templates/index.rst
+-rw-r--r--   0 maik      (1000) maik      (1000)     1453 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/docs/upgrade-packages.rst
+drwxr-xr-x   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:09.020470 bobtemplates.plone-6.3.2/package_tests/
+-rw-r--r--   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/package_tests/__init__.py
+-rw-r--r--   0 maik      (1000) maik      (1000)     2034 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/package_tests/base.py
+-rw-r--r--   0 maik      (1000) maik      (1000)     3388 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/package_tests/test_addon.py
+-rw-r--r--   0 maik      (1000) maik      (1000)    13675 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/package_tests/test_base.py
+-rw-r--r--   0 maik      (1000) maik      (1000)     2250 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/package_tests/test_behavior.py
+-rw-r--r--   0 maik      (1000) maik      (1000)     1332 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/package_tests/test_bobregistry.py
+-rw-r--r--   0 maik      (1000) maik      (1000)      438 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/package_tests/test_buildout.py
+-rw-r--r--   0 maik      (1000) maik      (1000)    13395 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/package_tests/test_content_type.py
+-rw-r--r--   0 maik      (1000) maik      (1000)     5794 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/package_tests/test_form.py
+-rw-r--r--   0 maik      (1000) maik      (1000)     3198 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/package_tests/test_indexer.py
+-rw-r--r--   0 maik      (1000) maik      (1000)     2194 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/package_tests/test_mockup_pattern.py
+-rw-r--r--   0 maik      (1000) maik      (1000)    16782 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/package_tests/test_portlet.py
+-rw-r--r--   0 maik      (1000) maik      (1000)     7526 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/package_tests/test_restapi_service.py
+-rw-r--r--   0 maik      (1000) maik      (1000)        0 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/package_tests/test_site_initialization.py
+-rw-r--r--   0 maik      (1000) maik      (1000)     1743 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/package_tests/test_subscriber.py
+-rw-r--r--   0 maik      (1000) maik      (1000)     3944 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/package_tests/test_svelte_app.py
+-rw-r--r--   0 maik      (1000) maik      (1000)     3162 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/package_tests/test_theme.py
+-rw-r--r--   0 maik      (1000) maik      (1000)     2247 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/package_tests/test_theme_barceloneta.py
+-rw-r--r--   0 maik      (1000) maik      (1000)     2181 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/package_tests/test_theme_basic.py
+-rw-r--r--   0 maik      (1000) maik      (1000)     5439 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/package_tests/test_upgrade_step.py
+-rw-r--r--   0 maik      (1000) maik      (1000)    15448 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/package_tests/test_view.py
+-rw-r--r--   0 maik      (1000) maik      (1000)    14572 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/package_tests/test_viewlet.py
+-rw-r--r--   0 maik      (1000) maik      (1000)     2247 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/package_tests/test_vocabulary.py
+-rw-r--r--   0 maik      (1000) maik      (1000)      732 2024-05-07 17:22:09.020470 bobtemplates.plone-6.3.2/setup.cfg
+-rw-r--r--   0 maik      (1000) maik      (1000)     3931 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/setup.py
+-rw-r--r--   0 maik      (1000) maik      (1000)     4807 2024-05-07 17:22:08.000000 bobtemplates.plone-6.3.2/tox.ini
```

### Comparing `bobtemplates.plone-6.3.1/CHANGES.rst` & `bobtemplates.plone-6.3.2/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,27 @@
 Changelog
 =========
 
-6.3.1 (2023-10-31)
+6.3.2 (2024-05-07)
 ------------------
 
-Breaking changes:
+New features:
+
+- Add a starter subtemplate to initialize a Plone site with some sane default values
+  [erral]
+
+
+Bug fixes:
+
+- add min_version = 4.11.0 to addon tempalte tox.ini
+  [MrTango]
+
 
-- *add item here*
+6.3.1 (2023-10-31)
+------------------
 
 New features:
 
 - Add `icon_expr` for `content_type`` view/edit actions and ask for "Content type icon" when adding a `content_type`.
   [petschki]
 
 Bug fixes:
```

### Comparing `bobtemplates.plone-6.3.1/CONTRIBUTORS.rst` & `bobtemplates.plone-6.3.2/CONTRIBUTORS.rst`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/LICENSE.GPL` & `bobtemplates.plone-6.3.2/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/LICENSE.rst` & `bobtemplates.plone-6.3.2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/PKG-INFO` & `bobtemplates.plone-6.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bobtemplates.plone
-Version: 6.3.1
+Version: 6.3.2
 Summary: Templates for Plone projects.
 Home-page: https://github.com/plone/bobtemplates.plone/
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/bobtemplates.plone
 Project-URL: Documentation, https://bobtemplatesplone.readthedocs.io/en/latest/
@@ -27,14 +27,22 @@
 Classifier: Framework :: Plone :: 6.0
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Requires-Python: >=3.7
 License-File: LICENSE.GPL
 License-File: LICENSE.rst
+Requires-Dist: setuptools
+Requires-Dist: mr.bob
+Requires-Dist: lxml
+Requires-Dist: case-conversion
+Requires-Dist: colorama
+Requires-Dist: tox
+Requires-Dist: isort
+Requires-Dist: black
 
 .. image:: https://github.com/plone/bobtemplates.plone/actions/workflows/python-package.yml/badge.svg
     :target: https://github.com/plone/bobtemplates.plone/actions/workflows/python-package.yml
 
 .. image:: https://codecov.io/gh/plone/plone.bobtemplates/branch/main/graph/badge.svg
     :target: https://codecov.io/gh/plone/plone.bobtemplates
 
@@ -268,20 +276,31 @@
 - Peter Holzer [agitator]
 - Manuel Reinhardt [reinhardt]
 
 
 Changelog
 =========
 
-6.3.1 (2023-10-31)
+6.3.2 (2024-05-07)
 ------------------
 
-Breaking changes:
+New features:
+
+- Add a starter subtemplate to initialize a Plone site with some sane default values
+  [erral]
+
+
+Bug fixes:
+
+- add min_version = 4.11.0 to addon tempalte tox.ini
+  [MrTango]
+
 
-- *add item here*
+6.3.1 (2023-10-31)
+------------------
 
 New features:
 
 - Add `icon_expr` for `content_type`` view/edit actions and ask for "Content type icon" when adding a `content_type`.
   [petschki]
 
 Bug fixes:
```

### Comparing `bobtemplates.plone-6.3.1/README.rst` & `bobtemplates.plone-6.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/TODO.rst` & `bobtemplates.plone-6.3.2/TODO.rst`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/addon/.github/workflows/plone-package.yml.bob` & `bobtemplates.plone-6.3.2/bobtemplates/plone/addon/.github/workflows/plone-package.yml.bob`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/addon/.gitlab-ci.yml` & `bobtemplates.plone-6.3.2/bobtemplates/plone/addon/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/addon/.mrbob.ini` & `bobtemplates.plone-6.3.2/bobtemplates/plone/addon/.mrbob.ini`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/addon/.travis.yml.bob` & `bobtemplates.plone-6.3.2/bobtemplates/plone/addon/.travis.yml.bob`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/addon/DEVELOP.rst` & `bobtemplates.plone-6.3.2/bobtemplates/plone/addon/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/addon/LICENSE.GPL.bob` & `bobtemplates.plone-6.3.2/bobtemplates/plone/addon/LICENSE.GPL.bob`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/addon/LICENSE.rst.bob` & `bobtemplates.plone-6.3.2/bobtemplates/plone/addon/LICENSE.rst.bob`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/addon/README.rst.bob` & `bobtemplates.plone-6.3.2/bobtemplates/plone/addon/README.rst.bob`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/addon/base.cfg.bob` & `bobtemplates.plone-6.3.2/bobtemplates/plone/addon/base.cfg.bob`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/addon/docs/conf.py.bob` & `bobtemplates.plone-6.3.2/bobtemplates/plone/addon/docs/conf.py.bob`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/addon/setup.py.bob` & `bobtemplates.plone-6.3.2/bobtemplates/plone/addon/setup.py.bob`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/browser/configure.zcml.bob` & `bobtemplates.plone-6.3.2/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/browser/configure.zcml.bob`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/configure.zcml.bob` & `bobtemplates.plone-6.3.2/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/configure.zcml.bob`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/locales/README.rst.bob` & `bobtemplates.plone-6.3.2/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/locales/README.rst.bob`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/locales/update.py.bob` & `bobtemplates.plone-6.3.2/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/locales/update.py.bob`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/locales/update.sh.bob` & `bobtemplates.plone-6.3.2/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/locales/update.sh.bob`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/setuphandlers.py.bob` & `bobtemplates.plone-6.3.2/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/setuphandlers.py.bob`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/testing.py.bob` & `bobtemplates.plone-6.3.2/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/testing.py.bob`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/tests/robot/test_example.robot.bob` & `bobtemplates.plone-6.3.2/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/tests/robot/test_example.robot.bob`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/tests/test_robot.py.bob` & `bobtemplates.plone-6.3.2/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/tests/test_robot.py.bob`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/tests/test_setup.py.bob` & `bobtemplates.plone-6.3.2/bobtemplates/plone/addon/src/+package.namespace+/+package.name+/tests/test_setup.py.bob`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/addon/tox.ini` & `bobtemplates.plone-6.3.2/bobtemplates/plone/addon/tox.ini`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 [tox]
+
+min_version = 4.11.0
+
 envlist =
     py37-lint,
     py38-lint,
     py39-lint,
     py310-lint,
     black-check,
     py{38,37}-Plone{52},
```

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/addon.py` & `bobtemplates.plone-6.3.2/bobtemplates/plone/addon.py`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/base.py` & `bobtemplates.plone-6.3.2/bobtemplates/plone/base.py`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/behavior/.mrbob.ini` & `bobtemplates.plone-6.3.2/bobtemplates/plone/behavior/.mrbob.ini`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/behavior/behaviors/+behavior_name_normalized+.py.bob` & `bobtemplates.plone-6.3.2/bobtemplates/plone/behavior/behaviors/+behavior_name_normalized+.py.bob`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/behavior/tests/test_behavior_+behavior_name_normalized+.py.bob` & `bobtemplates.plone-6.3.2/bobtemplates/plone/behavior/tests/test_behavior_+behavior_name_normalized+.py.bob`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/behavior.py` & `bobtemplates.plone-6.3.2/bobtemplates/plone/behavior.py`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/bobregistry.py` & `bobtemplates.plone-6.3.2/bobtemplates/plone/bobregistry.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,7 +154,15 @@
 
 def plone_form():
     reg = RegEntry()
     reg.template = "bobtemplates.plone:form"
     reg.plonecli_alias = "form"
     reg.depend_on = "plone_addon"
     return reg
+
+
+def plone_site_initialization():
+    reg = RegEntry()
+    reg.template = "bobtemplates.plone:site_initialization"
+    reg.plonecli_alias = "site_initialization"
+    reg.depend_on = "plone_addon"
+    return reg
```

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/buildout/.mrbob.ini` & `bobtemplates.plone-6.3.2/bobtemplates/plone/buildout/.mrbob.ini`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/buildout/base.cfg.bob` & `bobtemplates.plone-6.3.2/bobtemplates/plone/buildout/base.cfg.bob`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/buildout/buildout.cfg.bob` & `bobtemplates.plone-6.3.2/bobtemplates/plone/buildout/buildout.cfg.bob`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/content_type/.mrbob.ini` & `bobtemplates.plone-6.3.2/bobtemplates/plone/content_type/.mrbob.ini`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/content_type/content/+dexterity_type_name_normalized+.py.bob` & `bobtemplates.plone-6.3.2/bobtemplates/plone/content_type/content/+dexterity_type_name_normalized+.py.bob`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/content_type/profiles/default/types/+dexterity_type_fti_file_name+.xml.bob` & `bobtemplates.plone-6.3.2/bobtemplates/plone/content_type/profiles/default/types/+dexterity_type_fti_file_name+.xml.bob`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/content_type/tests/robot/test_ct_+dexterity_type_name_normalized+.robot.bob` & `bobtemplates.plone-6.3.2/bobtemplates/plone/content_type/tests/robot/test_ct_+dexterity_type_name_normalized+.robot.bob`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/content_type/tests/test_ct_+dexterity_type_name_normalized+.py.bob` & `bobtemplates.plone-6.3.2/bobtemplates/plone/content_type/tests/test_ct_+dexterity_type_name_normalized+.py.bob`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/content_type.py` & `bobtemplates.plone-6.3.2/bobtemplates/plone/content_type.py`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/controlpanel/.mrbob.ini` & `bobtemplates.plone-6.3.2/bobtemplates/plone/controlpanel/.mrbob.ini`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/controlpanel/controlpanels/+controlpanel_name_normalized+/configure.zcml.bob` & `bobtemplates.plone-6.3.2/bobtemplates/plone/controlpanel/controlpanels/+controlpanel_name_normalized+/configure.zcml.bob`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/controlpanel/controlpanels/+controlpanel_name_normalized+/controlpanel.py.bob` & `bobtemplates.plone-6.3.2/bobtemplates/plone/controlpanel/controlpanels/+controlpanel_name_normalized+/controlpanel.py.bob`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/controlpanel.py` & `bobtemplates.plone-6.3.2/bobtemplates/plone/controlpanel.py`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/form/.mrbob.ini` & `bobtemplates.plone-6.3.2/bobtemplates/plone/form/.mrbob.ini`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/form/forms/+form_python_file_name+.py.bob` & `bobtemplates.plone-6.3.2/bobtemplates/plone/form/forms/+form_python_file_name+.py.bob`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/form/tests/test_form_+form_name_normalized+.py.bob` & `bobtemplates.plone-6.3.2/bobtemplates/plone/form/tests/test_form_+form_name_normalized+.py.bob`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/form.py` & `bobtemplates.plone-6.3.2/bobtemplates/plone/form.py`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/indexer/.mrbob.ini` & `bobtemplates.plone-6.3.2/bobtemplates/plone/indexer/.mrbob.ini`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/indexer/indexers/+indexer_file_name+.py.bob` & `bobtemplates.plone-6.3.2/bobtemplates/plone/indexer/indexers/+indexer_file_name+.py.bob`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/indexer/tests/test_indexer_+indexer_file_name+.py.bob` & `bobtemplates.plone-6.3.2/bobtemplates/plone/indexer/tests/test_indexer_+indexer_file_name+.py.bob`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/indexer.py` & `bobtemplates.plone-6.3.2/bobtemplates/plone/indexer.py`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/mockup_pattern/.mrbob.ini` & `bobtemplates.plone-6.3.2/bobtemplates/plone/mockup_pattern/.mrbob.ini`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/mockup_pattern/package.json.bob` & `bobtemplates.plone-6.3.2/bobtemplates/plone/mockup_pattern/package.json.bob`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/mockup_pattern/resources/pat-+pattern.name+/+pattern.name+.js.bob` & `bobtemplates.plone-6.3.2/bobtemplates/plone/mockup_pattern/resources/pat-+pattern.name+/+pattern.name+.js.bob`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/mockup_pattern/resources/pat-+pattern.name+/+pattern.name+.test.js.bob` & `bobtemplates.plone-6.3.2/bobtemplates/plone/mockup_pattern/resources/pat-+pattern.name+/+pattern.name+.test.js.bob`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/mockup_pattern/src/+package.namespace+/+package.name+/browser/pattern-demo.pt.bob` & `bobtemplates.plone-6.3.2/bobtemplates/plone/mockup_pattern/src/+package.namespace+/+package.name+/browser/pattern-demo.pt.bob`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/mockup_pattern/webpack.config.js.bob` & `bobtemplates.plone-6.3.2/bobtemplates/plone/mockup_pattern/webpack.config.js.bob`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/mockup_pattern.py` & `bobtemplates.plone-6.3.2/bobtemplates/plone/mockup_pattern.py`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/portlet/.mrbob.ini` & `bobtemplates.plone-6.3.2/bobtemplates/plone/portlet/.mrbob.ini`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/portlet/portlets/+portlet_name_normalized+.py.bob` & `bobtemplates.plone-6.3.2/bobtemplates/plone/portlet/portlets/+portlet_name_normalized+.py.bob`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/portlet/tests/test_+portlet_name_normalized+.py.bob` & `bobtemplates.plone-6.3.2/bobtemplates/plone/portlet/tests/test_+portlet_name_normalized+.py.bob`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/portlet.py` & `bobtemplates.plone-6.3.2/bobtemplates/plone/portlet.py`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/restapi_service/.mrbob.ini` & `bobtemplates.plone-6.3.2/bobtemplates/plone/restapi_service/.mrbob.ini`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/restapi_service/api/services/+service_class_name_normalized+/get.py.bob` & `bobtemplates.plone-6.3.2/bobtemplates/plone/restapi_service/api/services/+service_class_name_normalized+/get.py.bob`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/restapi_service.py` & `bobtemplates.plone-6.3.2/bobtemplates/plone/restapi_service.py`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/subscriber/.mrbob.ini` & `bobtemplates.plone-6.3.2/bobtemplates/plone/subscriber/.mrbob.ini`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/subscriber/tests/test_subscriber_+subscriber_handler_file_name+.py.bob` & `bobtemplates.plone-6.3.2/bobtemplates/plone/subscriber/tests/test_subscriber_+subscriber_handler_file_name+.py.bob`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/subscriber.py` & `bobtemplates.plone-6.3.2/bobtemplates/plone/subscriber.py`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/svelte_app/.mrbob.ini` & `bobtemplates.plone-6.3.2/bobtemplates/plone/svelte_app/.mrbob.ini`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/svelte_app/src/+package.namespace+/+package.name+/profiles/default/registry/+svelte_app_file_name+.xml.bob` & `bobtemplates.plone-6.3.2/bobtemplates/plone/svelte_app/src/+package.namespace+/+package.name+/profiles/default/registry/+svelte_app_file_name+.xml.bob`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/svelte_app/src/+package.namespace+/+package.name+/profiles/uninstall/registry/+svelte_app_file_name+.xml.bob` & `bobtemplates.plone-6.3.2/bobtemplates/plone/svelte_app/src/+package.namespace+/+package.name+/profiles/uninstall/registry/+svelte_app_file_name+.xml.bob`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/svelte_app/src/+package.namespace+/+package.name+/svelte_apps/+svelte_app_name_dashed+/favicon.png` & `bobtemplates.plone-6.3.2/bobtemplates/plone/svelte_app/src/+package.namespace+/+package.name+/svelte_apps/+svelte_app_name_dashed+/favicon.png`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/svelte_app/src/+package.namespace+/+package.name+/svelte_apps/+svelte_app_name_dashed+/global.css` & `bobtemplates.plone-6.3.2/bobtemplates/plone/svelte_app/src/+package.namespace+/+package.name+/svelte_apps/+svelte_app_name_dashed+/global.css`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/svelte_app/src/+package.namespace+/+package.name+/svelte_apps/+svelte_app_name_dashed+/index.html.bob` & `bobtemplates.plone-6.3.2/bobtemplates/plone/svelte_app/src/+package.namespace+/+package.name+/svelte_apps/+svelte_app_name_dashed+/index.html.bob`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/svelte_app/svelte_src/+svelte_app_name_dashed+/README.md.bob` & `bobtemplates.plone-6.3.2/bobtemplates/plone/svelte_app/svelte_src/+svelte_app_name_dashed+/README.md.bob`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/svelte_app/svelte_src/+svelte_app_name_dashed+/package.json` & `bobtemplates.plone-6.3.2/bobtemplates/plone/svelte_app/svelte_src/+svelte_app_name_dashed+/package.json`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/svelte_app/svelte_src/+svelte_app_name_dashed+/rollup.config.js.bob` & `bobtemplates.plone-6.3.2/bobtemplates/plone/svelte_app/svelte_src/+svelte_app_name_dashed+/rollup.config.js.bob`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/svelte_app/svelte_src/+svelte_app_name_dashed+/scripts/setupTypeScript.js` & `bobtemplates.plone-6.3.2/bobtemplates/plone/svelte_app/svelte_src/+svelte_app_name_dashed+/scripts/setupTypeScript.js`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/svelte_app/svelte_src/+svelte_app_name_dashed+/src/App.svelte.bob` & `bobtemplates.plone-6.3.2/bobtemplates/plone/svelte_app/svelte_src/+svelte_app_name_dashed+/src/App.svelte.bob`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/svelte_app/svelte_src/+svelte_app_name_dashed+/src/main.js.bob` & `bobtemplates.plone-6.3.2/bobtemplates/plone/svelte_app/svelte_src/+svelte_app_name_dashed+/src/main.js.bob`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/svelte_app.py` & `bobtemplates.plone-6.3.2/bobtemplates/plone/svelte_app.py`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/theme/.mrbob.ini` & `bobtemplates.plone-6.3.2/bobtemplates/plone/theme/.mrbob.ini`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/theme/profiles/default/registry/main.xml` & `bobtemplates.plone-6.3.2/bobtemplates/plone/theme/profiles/default/registry/main.xml`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/theme/profiles/default/registry/tinymce.xml` & `bobtemplates.plone-6.3.2/bobtemplates/plone/theme/profiles/default/registry/tinymce.xml`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/theme/theme/README.rst.bob` & `bobtemplates.plone-6.3.2/bobtemplates/plone/theme/theme/README.rst.bob`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/theme/theme/manifest.cfg.bob` & `bobtemplates.plone-6.3.2/bobtemplates/plone/theme/theme/manifest.cfg.bob`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/theme/theme/package.json.bob` & `bobtemplates.plone-6.3.2/bobtemplates/plone/theme/theme/package.json.bob`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/theme/theme/rules.xml.bob` & `bobtemplates.plone-6.3.2/bobtemplates/plone/theme/theme/rules.xml.bob`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/theme/theme/styles/theme.scss` & `bobtemplates.plone-6.3.2/bobtemplates/plone/theme/theme/styles/theme.scss`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/theme/theme/tinymce-templates/bs-dark-hero.html` & `bobtemplates.plone-6.3.2/bobtemplates/plone/theme/theme/tinymce-templates/bs-dark-hero.html`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/theme/theme/tinymce-templates/bs-hero-left.html` & `bobtemplates.plone-6.3.2/bobtemplates/plone/theme/theme/tinymce-templates/bs-hero-left.html`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/theme/theme/tinymce-templates/bs-pricing.html` & `bobtemplates.plone-6.3.2/bobtemplates/plone/theme/theme/tinymce-templates/bs-pricing.html`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/theme.py` & `bobtemplates.plone-6.3.2/bobtemplates/plone/theme.py`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/theme_barceloneta/.mrbob.ini` & `bobtemplates.plone-6.3.2/bobtemplates/plone/theme_barceloneta/.mrbob.ini`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/README.rst.bob` & `bobtemplates.plone-6.3.2/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/README.rst.bob`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/barceloneta-apple-touch-icon-114x114-precomposed.png` & `bobtemplates.plone-6.3.2/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/barceloneta-apple-touch-icon-114x114-precomposed.png`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/barceloneta-apple-touch-icon-144x144-precomposed.png` & `bobtemplates.plone-6.3.2/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/barceloneta-apple-touch-icon-144x144-precomposed.png`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/barceloneta-apple-touch-icon-57x57-precomposed.png` & `bobtemplates.plone-6.3.2/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/barceloneta-apple-touch-icon-57x57-precomposed.png`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/barceloneta-apple-touch-icon-72x72-precomposed.png` & `bobtemplates.plone-6.3.2/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/barceloneta-apple-touch-icon-72x72-precomposed.png`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/barceloneta-apple-touch-icon-precomposed.png` & `bobtemplates.plone-6.3.2/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/barceloneta-apple-touch-icon-precomposed.png`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/barceloneta-apple-touch-icon.png` & `bobtemplates.plone-6.3.2/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/barceloneta-apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/barceloneta-favicon.ico` & `bobtemplates.plone-6.3.2/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/barceloneta-favicon.ico`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/index.html` & `bobtemplates.plone-6.3.2/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/index.html`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/manifest.cfg.bob` & `bobtemplates.plone-6.3.2/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/manifest.cfg.bob`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/package.json.bob` & `bobtemplates.plone-6.3.2/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/package.json.bob`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/preview.png` & `bobtemplates.plone-6.3.2/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/preview.png`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/rules.xml` & `bobtemplates.plone-6.3.2/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/rules.xml`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/scss/theme.scss` & `bobtemplates.plone-6.3.2/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/scss/theme.scss`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/styles/theme.css` & `bobtemplates.plone-6.3.2/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/styles/theme.css`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/styles/theme.min.css` & `bobtemplates.plone-6.3.2/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/styles/theme.min.css`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/tinymce-templates/README.rst.bob` & `bobtemplates.plone-6.3.2/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/tinymce-templates/README.rst.bob`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/tinymce-templates/card-group.html` & `bobtemplates.plone-6.3.2/bobtemplates/plone/theme_barceloneta/src/+package.namespace+/+package.name+/theme/tinymce-templates/card-group.html`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/theme_barceloneta.py` & `bobtemplates.plone-6.3.2/bobtemplates/plone/theme_barceloneta.py`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/theme_basic/.mrbob.ini` & `bobtemplates.plone-6.3.2/bobtemplates/plone/theme_basic/.mrbob.ini`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/theme_basic/src/+package.namespace+/+package.name+/browser/overrides/plone.app.layout.viewlets.sections.pt` & `bobtemplates.plone-6.3.2/bobtemplates/plone/theme_basic/src/+package.namespace+/+package.name+/browser/overrides/plone.app.layout.viewlets.sections.pt`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/theme_basic/src/+package.namespace+/+package.name+/theme/README.rst.bob` & `bobtemplates.plone-6.3.2/bobtemplates/plone/theme_basic/src/+package.namespace+/+package.name+/theme/README.rst.bob`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/theme_basic/src/+package.namespace+/+package.name+/theme/css/theme.css` & `bobtemplates.plone-6.3.2/bobtemplates/plone/theme_basic/src/+package.namespace+/+package.name+/theme/css/theme.css`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/theme_basic/src/+package.namespace+/+package.name+/theme/css/theme.css.map` & `bobtemplates.plone-6.3.2/bobtemplates/plone/theme_basic/src/+package.namespace+/+package.name+/theme/css/theme.css.map`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/theme_basic/src/+package.namespace+/+package.name+/theme/css/theme.min.css` & `bobtemplates.plone-6.3.2/bobtemplates/plone/theme_basic/src/+package.namespace+/+package.name+/theme/css/theme.min.css`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/theme_basic/src/+package.namespace+/+package.name+/theme/css/theme.min.css.map` & `bobtemplates.plone-6.3.2/bobtemplates/plone/theme_basic/src/+package.namespace+/+package.name+/theme/css/theme.min.css.map`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/theme_basic/src/+package.namespace+/+package.name+/theme/package.json.bob` & `bobtemplates.plone-6.3.2/bobtemplates/plone/theme_basic/src/+package.namespace+/+package.name+/theme/package.json.bob`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/theme_basic/src/+package.namespace+/+package.name+/theme/preview.png` & `bobtemplates.plone-6.3.2/bobtemplates/plone/theme_basic/src/+package.namespace+/+package.name+/theme/preview.png`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/theme_basic/src/+package.namespace+/+package.name+/theme/scss/theme.scss` & `bobtemplates.plone-6.3.2/bobtemplates/plone/theme_basic/src/+package.namespace+/+package.name+/theme/scss/theme.scss`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/theme_basic/src/+package.namespace+/+package.name+/theme/tinymce-templates/README.rst.bob` & `bobtemplates.plone-6.3.2/bobtemplates/plone/theme_basic/src/+package.namespace+/+package.name+/theme/tinymce-templates/README.rst.bob`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/theme_basic/src/+package.namespace+/+package.name+/theme/tinymce-templates/card-group.html` & `bobtemplates.plone-6.3.2/bobtemplates/plone/theme_basic/src/+package.namespace+/+package.name+/theme/tinymce-templates/card-group.html`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/theme_basic.py` & `bobtemplates.plone-6.3.2/bobtemplates/plone/theme_basic.py`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/upgrade_step/.mrbob.ini` & `bobtemplates.plone-6.3.2/bobtemplates/plone/upgrade_step/.mrbob.ini`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/upgrade_step/tests/test_upgrade_step_+upgrade_step_id+.py.bob` & `bobtemplates.plone-6.3.2/bobtemplates/plone/upgrade_step/tests/test_upgrade_step_+upgrade_step_id+.py.bob`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/upgrade_step/upgrades/+upgrade_step_id+.zcml.bob` & `bobtemplates.plone-6.3.2/bobtemplates/plone/upgrade_step/upgrades/+upgrade_step_id+.zcml.bob`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/upgrade_step.py` & `bobtemplates.plone-6.3.2/bobtemplates/plone/upgrade_step.py`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/utils.py` & `bobtemplates.plone-6.3.2/bobtemplates/plone/utils.py`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/view/.mrbob.ini` & `bobtemplates.plone-6.3.2/bobtemplates/plone/view/.mrbob.ini`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/view/tests/test_view_+view_python_file_name+.py.bob` & `bobtemplates.plone-6.3.2/bobtemplates/plone/view/tests/test_view_+view_python_file_name+.py.bob`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/view/views/+view_python_file_name+.py.bob` & `bobtemplates.plone-6.3.2/bobtemplates/plone/view/views/+view_python_file_name+.py.bob`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/view/views/+view_template_name+.pt.bob` & `bobtemplates.plone-6.3.2/bobtemplates/plone/view/views/+view_template_name+.pt.bob`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/view.py` & `bobtemplates.plone-6.3.2/bobtemplates/plone/view.py`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/viewlet/.mrbob.ini` & `bobtemplates.plone-6.3.2/bobtemplates/plone/viewlet/.mrbob.ini`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/viewlet/tests/test_viewlet_+viewlet_name_normalized+.py.bob` & `bobtemplates.plone-6.3.2/bobtemplates/plone/viewlet/tests/test_viewlet_+viewlet_name_normalized+.py.bob`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/viewlet/viewlets/+viewlet_python_file_name+.py.bob` & `bobtemplates.plone-6.3.2/bobtemplates/plone/viewlet/viewlets/+viewlet_python_file_name+.py.bob`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/viewlet.py` & `bobtemplates.plone-6.3.2/bobtemplates/plone/viewlet.py`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/vocabulary/.mrbob.ini` & `bobtemplates.plone-6.3.2/bobtemplates/plone/vocabulary/.mrbob.ini`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/vocabulary/tests/test_vocab_+vocabulary_name_normalized+.py.bob` & `bobtemplates.plone-6.3.2/bobtemplates/plone/vocabulary/tests/test_vocab_+vocabulary_name_normalized+.py.bob`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/vocabulary/vocabularies/+vocabulary_name_normalized+.py.bob` & `bobtemplates.plone-6.3.2/bobtemplates/plone/vocabulary/vocabularies/+vocabulary_name_normalized+.py.bob`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates/plone/vocabulary.py` & `bobtemplates.plone-6.3.2/bobtemplates/plone/vocabulary.py`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/bobtemplates.plone.egg-info/PKG-INFO` & `bobtemplates.plone-6.3.2/bobtemplates.plone.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bobtemplates.plone
-Version: 6.3.1
+Version: 6.3.2
 Summary: Templates for Plone projects.
 Home-page: https://github.com/plone/bobtemplates.plone/
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/bobtemplates.plone
 Project-URL: Documentation, https://bobtemplatesplone.readthedocs.io/en/latest/
@@ -27,14 +27,22 @@
 Classifier: Framework :: Plone :: 6.0
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Requires-Python: >=3.7
 License-File: LICENSE.GPL
 License-File: LICENSE.rst
+Requires-Dist: setuptools
+Requires-Dist: mr.bob
+Requires-Dist: lxml
+Requires-Dist: case-conversion
+Requires-Dist: colorama
+Requires-Dist: tox
+Requires-Dist: isort
+Requires-Dist: black
 
 .. image:: https://github.com/plone/bobtemplates.plone/actions/workflows/python-package.yml/badge.svg
     :target: https://github.com/plone/bobtemplates.plone/actions/workflows/python-package.yml
 
 .. image:: https://codecov.io/gh/plone/plone.bobtemplates/branch/main/graph/badge.svg
     :target: https://codecov.io/gh/plone/plone.bobtemplates
 
@@ -268,20 +276,31 @@
 - Peter Holzer [agitator]
 - Manuel Reinhardt [reinhardt]
 
 
 Changelog
 =========
 
-6.3.1 (2023-10-31)
+6.3.2 (2024-05-07)
 ------------------
 
-Breaking changes:
+New features:
+
+- Add a starter subtemplate to initialize a Plone site with some sane default values
+  [erral]
+
+
+Bug fixes:
+
+- add min_version = 4.11.0 to addon tempalte tox.ini
+  [MrTango]
+
 
-- *add item here*
+6.3.1 (2023-10-31)
+------------------
 
 New features:
 
 - Add `icon_expr` for `content_type`` view/edit actions and ask for "Content type icon" when adding a `content_type`.
   [petschki]
 
 Bug fixes:
```

### Comparing `bobtemplates.plone-6.3.1/bobtemplates.plone.egg-info/SOURCES.txt` & `bobtemplates.plone-6.3.2/bobtemplates.plone.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 bobtemplates/plone/content_type.py
 bobtemplates/plone/controlpanel.py
 bobtemplates/plone/form.py
 bobtemplates/plone/indexer.py
 bobtemplates/plone/mockup_pattern.py
 bobtemplates/plone/portlet.py
 bobtemplates/plone/restapi_service.py
+bobtemplates/plone/site_initialization.py
 bobtemplates/plone/subscriber.py
 bobtemplates/plone/svelte_app.py
 bobtemplates/plone/theme.py
 bobtemplates/plone/theme_barceloneta.py
 bobtemplates/plone/theme_basic.py
 bobtemplates/plone/upgrade_step.py
 bobtemplates/plone/utils.py
@@ -170,14 +171,18 @@
 bobtemplates/plone/restapi_service/api/__init__.py
 bobtemplates/plone/restapi_service/api/configure.zcml.example.bob
 bobtemplates/plone/restapi_service/api/services/__init__.py
 bobtemplates/plone/restapi_service/api/services/configure.zcml.example.bob
 bobtemplates/plone/restapi_service/api/services/+service_class_name_normalized+/__init__.py
 bobtemplates/plone/restapi_service/api/services/+service_class_name_normalized+/configure.zcml.bob
 bobtemplates/plone/restapi_service/api/services/+service_class_name_normalized+/get.py.bob
+bobtemplates/plone/site_initialization/.mrbob.ini
+bobtemplates/plone/site_initialization/profiles/default/registry/plone.base.interfaces.controlpanel.IMailSchema.xml.bob
+bobtemplates/plone/site_initialization/profiles/default/registry/plone.base.interfaces.controlpanel.ISiteSchema.xml.bob
+bobtemplates/plone/site_initialization/profiles/default/registry/plone.i18n.interfaces.ILanguageSchema.xml.bob
 bobtemplates/plone/subscriber/.mrbob.ini
 bobtemplates/plone/subscriber/subscribers/+subscriber_handler_file_name+.py.bob
 bobtemplates/plone/subscriber/subscribers/__init__.py
 bobtemplates/plone/subscriber/subscribers/configure.zcml.example.bob
 bobtemplates/plone/subscriber/tests/test_subscriber_+subscriber_handler_file_name+.py.bob
 bobtemplates/plone/svelte_app/.mrbob.ini
 bobtemplates/plone/svelte_app/src/+package.namespace+/+package.name+/profiles/default/registry/+svelte_app_file_name+.xml.bob
@@ -316,14 +321,15 @@
 package_tests/test_buildout.py
 package_tests/test_content_type.py
 package_tests/test_form.py
 package_tests/test_indexer.py
 package_tests/test_mockup_pattern.py
 package_tests/test_portlet.py
 package_tests/test_restapi_service.py
+package_tests/test_site_initialization.py
 package_tests/test_subscriber.py
 package_tests/test_svelte_app.py
 package_tests/test_theme.py
 package_tests/test_theme_barceloneta.py
 package_tests/test_theme_basic.py
 package_tests/test_upgrade_step.py
 package_tests/test_view.py
```

### Comparing `bobtemplates.plone-6.3.1/bobtemplates.plone.egg-info/entry_points.txt` & `bobtemplates.plone-6.3.2/bobtemplates.plone.egg-info/entry_points.txt`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 plone_content_type = bobtemplates.plone.bobregistry:plone_content_type
 plone_controlpanel = bobtemplates.plone.bobregistry:plone_controlpanel
 plone_form = bobtemplates.plone.bobregistry:plone_form
 plone_indexer = bobtemplates.plone.bobregistry:plone_indexer
 plone_mockup_pattern = bobtemplates.plone.bobregistry:plone_mockup_pattern
 plone_portlet = bobtemplates.plone.bobregistry:plone_portlet
 plone_restapi_service = bobtemplates.plone.bobregistry:plone_restapi_service
+plone_site_initialization = bobtemplates.plone.bobregistry:plone_site_initialization
 plone_subscriber = bobtemplates.plone.bobregistry:plone_subscriber
 plone_svelte_app = bobtemplates.plone.bobregistry:plone_svelte_app
 plone_theme = bobtemplates.plone.bobregistry:plone_theme
 plone_theme_barceloneta = bobtemplates.plone.bobregistry:plone_theme_barceloneta
 plone_theme_basic = bobtemplates.plone.bobregistry:plone_theme_basic
 plone_upgrade_step = bobtemplates.plone.bobregistry:plone_upgrade_step
 plone_view = bobtemplates.plone.bobregistry:plone_view
```

### Comparing `bobtemplates.plone-6.3.1/docs/Makefile` & `bobtemplates.plone-6.3.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/docs/conf.py` & `bobtemplates.plone-6.3.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/docs/develop.rst` & `bobtemplates.plone-6.3.2/docs/develop.rst`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/docs/git-support.rst` & `bobtemplates.plone-6.3.2/docs/git-support.rst`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/docs/make.bat` & `bobtemplates.plone-6.3.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/docs/templates/addon/behavior/index.rst` & `bobtemplates.plone-6.3.2/docs/templates/addon/behavior/index.rst`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/docs/templates/addon/content_type/index.rst` & `bobtemplates.plone-6.3.2/docs/templates/addon/content_type/index.rst`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/docs/templates/addon/index.rst` & `bobtemplates.plone-6.3.2/docs/templates/addon/index.rst`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/docs/templates/addon/indexer/index.rst` & `bobtemplates.plone-6.3.2/docs/templates/addon/indexer/index.rst`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/docs/templates/addon/portlet/index.rst` & `bobtemplates.plone-6.3.2/docs/templates/addon/portlet/index.rst`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/docs/templates/addon/restapi_service/index.rst` & `bobtemplates.plone-6.3.2/docs/templates/addon/restapi_service/index.rst`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/docs/templates/addon/subscriber/index.rst` & `bobtemplates.plone-6.3.2/docs/templates/addon/subscriber/index.rst`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/docs/templates/addon/svelte_app/html-filter-settings.png` & `bobtemplates.plone-6.3.2/docs/templates/addon/svelte_app/html-filter-settings.png`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/docs/templates/addon/svelte_app/index.rst` & `bobtemplates.plone-6.3.2/docs/templates/addon/svelte_app/index.rst`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/docs/templates/addon/svelte_app/tinymce-advanced-settings.png` & `bobtemplates.plone-6.3.2/docs/templates/addon/svelte_app/tinymce-advanced-settings.png`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/docs/templates/addon/theme/index.rst` & `bobtemplates.plone-6.3.2/docs/templates/addon/theme/index.rst`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/docs/templates/addon/theme_barceloneta/index.rst` & `bobtemplates.plone-6.3.2/docs/templates/addon/theme_barceloneta/index.rst`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/docs/templates/addon/view/index.rst` & `bobtemplates.plone-6.3.2/docs/templates/addon/view/index.rst`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/docs/templates/addon/viewlet/index.rst` & `bobtemplates.plone-6.3.2/docs/templates/addon/viewlet/index.rst`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/docs/templates/addon/vocabulary/index.rst` & `bobtemplates.plone-6.3.2/docs/templates/addon/vocabulary/index.rst`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/docs/templates/buildout/index.rst` & `bobtemplates.plone-6.3.2/docs/templates/buildout/index.rst`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/docs/upgrade-packages.rst` & `bobtemplates.plone-6.3.2/docs/upgrade-packages.rst`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/package_tests/base.py` & `bobtemplates.plone-6.3.2/package_tests/base.py`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/package_tests/test_addon.py` & `bobtemplates.plone-6.3.2/package_tests/test_addon.py`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/package_tests/test_base.py` & `bobtemplates.plone-6.3.2/package_tests/test_base.py`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/package_tests/test_behavior.py` & `bobtemplates.plone-6.3.2/package_tests/test_behavior.py`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/package_tests/test_bobregistry.py` & `bobtemplates.plone-6.3.2/package_tests/test_bobregistry.py`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/package_tests/test_content_type.py` & `bobtemplates.plone-6.3.2/package_tests/test_content_type.py`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/package_tests/test_form.py` & `bobtemplates.plone-6.3.2/package_tests/test_form.py`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/package_tests/test_indexer.py` & `bobtemplates.plone-6.3.2/package_tests/test_indexer.py`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/package_tests/test_mockup_pattern.py` & `bobtemplates.plone-6.3.2/package_tests/test_mockup_pattern.py`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/package_tests/test_portlet.py` & `bobtemplates.plone-6.3.2/package_tests/test_portlet.py`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/package_tests/test_restapi_service.py` & `bobtemplates.plone-6.3.2/package_tests/test_restapi_service.py`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/package_tests/test_subscriber.py` & `bobtemplates.plone-6.3.2/package_tests/test_subscriber.py`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/package_tests/test_svelte_app.py` & `bobtemplates.plone-6.3.2/package_tests/test_svelte_app.py`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/package_tests/test_theme.py` & `bobtemplates.plone-6.3.2/package_tests/test_theme.py`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/package_tests/test_theme_barceloneta.py` & `bobtemplates.plone-6.3.2/package_tests/test_theme_barceloneta.py`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/package_tests/test_theme_basic.py` & `bobtemplates.plone-6.3.2/package_tests/test_theme_basic.py`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/package_tests/test_upgrade_step.py` & `bobtemplates.plone-6.3.2/package_tests/test_upgrade_step.py`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/package_tests/test_view.py` & `bobtemplates.plone-6.3.2/package_tests/test_view.py`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/package_tests/test_viewlet.py` & `bobtemplates.plone-6.3.2/package_tests/test_viewlet.py`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/package_tests/test_vocabulary.py` & `bobtemplates.plone-6.3.2/package_tests/test_vocabulary.py`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/setup.cfg` & `bobtemplates.plone-6.3.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `bobtemplates.plone-6.3.1/setup.py` & `bobtemplates.plone-6.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = "6.3.1"
+version = "6.3.2"
 
 
 long_description = "\n\n".join(
     [
         open("README.rst").read(),
         open("CONTRIBUTORS.rst").read(),
         open("CHANGES.rst").read(),
@@ -86,10 +86,11 @@
             "plone_theme_basic = bobtemplates.plone.bobregistry:plone_theme_basic",  # NOQA E501
             "plone_upgrade_step = bobtemplates.plone.bobregistry:plone_upgrade_step",
             "plone_view = bobtemplates.plone.bobregistry:plone_view",
             "plone_viewlet = bobtemplates.plone.bobregistry:plone_viewlet",
             "plone_vocabulary = bobtemplates.plone.bobregistry:plone_vocabulary",
             "plone_controlpanel = bobtemplates.plone.bobregistry:plone_controlpanel",
             "plone_form = bobtemplates.plone.bobregistry:plone_form",
+            "plone_site_initialization = bobtemplates.plone.bobregistry:plone_site_initialization",
         ]
     },
 )
```

### Comparing `bobtemplates.plone-6.3.1/tox.ini` & `bobtemplates.plone-6.3.2/tox.ini`

 * *Files identical despite different names*

