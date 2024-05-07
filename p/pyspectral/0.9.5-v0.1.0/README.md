# Comparing `tmp/pyspectral-0.9.5.tar.gz` & `tmp/pyspectral-v0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyspectral-0.9.5.tar", last modified: Tue Feb  4 15:35:08 2020, max compression
+gzip compressed data, was "pyspectral-v0.1.0.tar", last modified: Tue Jun 17 09:47:11 2014, max compression, from Unix
```

## Comparing `pyspectral-0.9.5.tar` & `pyspectral-v0.1.0.tar`

### file list

```diff
@@ -1,239 +1,31 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-04 15:35:08.000000 pyspectral-0.9.5/
--rw-rw-r--   0 travis    (2000) travis    (2000)      106 2020-02-04 15:29:50.000000 pyspectral-0.9.5/.bumpversion.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)    36207 2020-02-04 15:29:50.000000 pyspectral-0.9.5/changelog.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-04 15:35:08.000000 pyspectral-0.9.5/.github/
--rw-rw-r--   0 travis    (2000) travis    (2000)      604 2020-02-04 15:29:50.000000 pyspectral-0.9.5/.github/PULL_REQUEST_TEMPLATE.md
--rw-rw-r--   0 travis    (2000) travis    (2000)      420 2020-02-04 15:29:50.000000 pyspectral-0.9.5/.github/ISSUE_TEMPLATE.md
--rw-rw-r--   0 travis    (2000) travis    (2000)      208 2020-02-04 15:29:50.000000 pyspectral-0.9.5/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)    35147 2020-02-04 15:29:50.000000 pyspectral-0.9.5/LICENSE.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       66 2020-02-04 15:29:50.000000 pyspectral-0.9.5/requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      869 2020-02-04 15:35:08.000000 pyspectral-0.9.5/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     2012 2020-02-04 15:29:50.000000 pyspectral-0.9.5/compare2rsrfiles.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1476 2020-02-04 15:29:50.000000 pyspectral-0.9.5/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)     2594 2020-02-04 15:29:50.000000 pyspectral-0.9.5/plot_some_band.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-04 15:35:08.000000 pyspectral-0.9.5/pyspectral/
--rw-rw-r--   0 travis    (2000) travis    (2000)    11499 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/near_infrared_reflectance.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8342 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/blackbody.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-04 15:35:08.000000 pyspectral-0.9.5/pyspectral/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)   744960 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/MSG_SEVIRI_Spectral_Response_Characterisation.XLS
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-04 15:35:08.000000 pyspectral-0.9.5/pyspectral/data/modis/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-04 15:35:08.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Aqua/
--rw-rw-r--   0 travis    (2000) travis    (2000)    13564 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Aqua/07.tv.1pct.det
--rw-rw-r--   0 travis    (2000) travis    (2000)     8910 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Aqua/33.tv.1pct.det
--rw-rw-r--   0 travis    (2000) travis    (2000)     9898 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Aqua/20.tv.1pct.det
--rw-rw-r--   0 travis    (2000) travis    (2000)    11120 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Aqua/24.tv.1pct.det
--rw-rw-r--   0 travis    (2000) travis    (2000)     9768 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Aqua/34.tv.1pct.det
--rw-rw-r--   0 travis    (2000) travis    (2000)    21598 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Aqua/05.tv.1pct.det
--rw-rw-r--   0 travis    (2000) travis    (2000)     8026 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Aqua/29.tv.1pct.det
--rw-rw-r--   0 travis    (2000) travis    (2000)     9326 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Aqua/32.tv.1pct.det
--rw-rw-r--   0 travis    (2000) travis    (2000)    35638 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Aqua/02.amb.1pct.det
--rw-rw-r--   0 travis    (2000) travis    (2000)    10314 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Aqua/21.tv.1pct.det
--rw-rw-r--   0 travis    (2000) travis    (2000)     6518 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Aqua/12.amb.1pct.det
--rw-rw-r--   0 travis    (2000) travis    (2000)     6570 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Aqua/15.amb.1pct.det
--rw-rw-r--   0 travis    (2000) travis    (2000)     5530 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Aqua/08.amb.1pct.det
--rw-rw-r--   0 travis    (2000) travis    (2000)     9118 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Aqua/36.tv.1pct.det
--rw-rw-r--   0 travis    (2000) travis    (2000)    10132 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Aqua/22.tv.1pct.det
--rw-rw-r--   0 travis    (2000) travis    (2000)     7064 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Aqua/17.amb.1pct.det
--rw-rw-r--   0 travis    (2000) travis    (2000)    13044 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Aqua/28.tv.1pct.det
--rw-rw-r--   0 travis    (2000) travis    (2000)     7012 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Aqua/30.tv.1pct.det
--rw-rw-r--   0 travis    (2000) travis    (2000)    12576 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Aqua/26.tv.1pct.det
--rw-rw-r--   0 travis    (2000) travis    (2000)     9924 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Aqua/19.amb.1pct.det
--rw-rw-r--   0 travis    (2000) travis    (2000)     5660 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Aqua/09.amb.1pct.det
--rw-rw-r--   0 travis    (2000) travis    (2000)    11042 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Aqua/25.tv.1pct.det
--rw-rw-r--   0 travis    (2000) travis    (2000)    17178 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Aqua/03.amb.1pct.det
--rw-rw-r--   0 travis    (2000) travis    (2000)     8000 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Aqua/18.amb.1pct.det
--rw-rw-r--   0 travis    (2000) travis    (2000)    17230 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Aqua/04.amb.1pct.det
--rw-rw-r--   0 travis    (2000) travis    (2000)    18530 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Aqua/06.tv.1pct.det
--rw-rw-r--   0 travis    (2000) travis    (2000)     5920 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Aqua/13.amb.1pct.det
--rw-rw-r--   0 travis    (2000) travis    (2000)     8702 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Aqua/10.amb.1pct.det
--rw-rw-r--   0 travis    (2000) travis    (2000)     9170 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Aqua/16.amb.1pct.det
--rw-rw-r--   0 travis    (2000) travis    (2000)    11952 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Aqua/31.tv.1pct.det
--rw-rw-r--   0 travis    (2000) travis    (2000)    12264 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Aqua/27.tv.1pct.det
--rw-rw-r--   0 travis    (2000) travis    (2000)    10184 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Aqua/11.amb.1pct.det
--rw-rw-r--   0 travis    (2000) travis    (2000)    17542 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Aqua/35.tv.1pct.det
--rw-rw-r--   0 travis    (2000) travis    (2000)    30724 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Aqua/01.amb.1pct.det
--rw-rw-r--   0 travis    (2000) travis    (2000)     9768 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Aqua/14.amb.1pct.det
--rw-rw-r--   0 travis    (2000) travis    (2000)    10158 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Aqua/23.tv.1pct.det
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-04 15:35:08.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Terra/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-04 15:35:08.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Terra/L1B_RSR_LUT/
--rw-rw-r--   0 travis    (2000) travis    (2000)    20584 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Terra/L1B_RSR_LUT/rsr.6.inb.final
--rw-rw-r--   0 travis    (2000) travis    (2000)    10614 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Terra/L1B_RSR_LUT/rsr.32.inb.final
--rw-rw-r--   0 travis    (2000) travis    (2000)     5364 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Terra/L1B_RSR_LUT/rsr.10.inb.final
--rw-rw-r--   0 travis    (2000) travis    (2000)    11169 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Terra/L1B_RSR_LUT/rsr.22.inb.final
--rw-rw-r--   0 travis    (2000) travis    (2000)    15636 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Terra/L1B_RSR_LUT/rsr.4.inb.final
--rw-rw-r--   0 travis    (2000) travis    (2000)    10644 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Terra/L1B_RSR_LUT/rsr.34.inb.final
--rw-rw-r--   0 travis    (2000) travis    (2000)    10404 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Terra/L1B_RSR_LUT/rsr.33.inb.final
--rw-rw-r--   0 travis    (2000) travis    (2000)    11139 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Terra/L1B_RSR_LUT/rsr.21.inb.final
--rw-rw-r--   0 travis    (2000) travis    (2000)    12744 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Terra/L1B_RSR_LUT/rsr.31.inb.final
--rw-rw-r--   0 travis    (2000) travis    (2000)     8364 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Terra/L1B_RSR_LUT/rsr.16.inb.final
--rw-rw-r--   0 travis    (2000) travis    (2000)    23424 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Terra/L1B_RSR_LUT/rsr.5.inb.final
--rw-rw-r--   0 travis    (2000) travis    (2000)    10854 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Terra/L1B_RSR_LUT/rsr.35.inb.final
--rw-rw-r--   0 travis    (2000) travis    (2000)    13949 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Terra/L1B_RSR_LUT/rsr.27.inb.final
--rw-rw-r--   0 travis    (2000) travis    (2000)    10859 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Terra/L1B_RSR_LUT/rsr.20.inb.final
--rw-rw-r--   0 travis    (2000) travis    (2000)     7249 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Terra/L1B_RSR_LUT/rsr.15.inb.final
--rw-rw-r--   0 travis    (2000) travis    (2000)     7564 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Terra/L1B_RSR_LUT/rsr.17.inb.final
--rw-rw-r--   0 travis    (2000) travis    (2000)    14204 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Terra/L1B_RSR_LUT/rsr.28.inb.final
--rw-rw-r--   0 travis    (2000) travis    (2000)    15024 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Terra/L1B_RSR_LUT/rsr.7.inb.final
--rw-rw-r--   0 travis    (2000) travis    (2000)     6384 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Terra/L1B_RSR_LUT/rsr.8.inb.final
--rw-rw-r--   0 travis    (2000) travis    (2000)     3204 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Terra/L1B_RSR_LUT/rsr.13.inb.final
--rw-rw-r--   0 travis    (2000) travis    (2000)    11144 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Terra/L1B_RSR_LUT/rsr.24.inb.final
--rw-rw-r--   0 travis    (2000) travis    (2000)    38609 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Terra/L1B_RSR_LUT/rsr.2.inb.final
--rw-rw-r--   0 travis    (2000) travis    (2000)    11189 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Terra/L1B_RSR_LUT/rsr.25.inb.final
--rw-rw-r--   0 travis    (2000) travis    (2000)    24344 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Terra/L1B_RSR_LUT/rsr.26.inb.final
--rw-rw-r--   0 travis    (2000) travis    (2000)     8214 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Terra/L1B_RSR_LUT/rsr.30.inb.final
--rw-rw-r--   0 travis    (2000) travis    (2000)    33024 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Terra/L1B_RSR_LUT/rsr.1.inb.final
--rw-rw-r--   0 travis    (2000) travis    (2000)    10599 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Terra/L1B_RSR_LUT/rsr.19.inb.final
--rw-rw-r--   0 travis    (2000) travis    (2000)    10899 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Terra/L1B_RSR_LUT/rsr.23.inb.final
--rw-rw-r--   0 travis    (2000) travis    (2000)    10554 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Terra/L1B_RSR_LUT/rsr.36.inb.final
--rw-rw-r--   0 travis    (2000) travis    (2000)     8404 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Terra/L1B_RSR_LUT/rsr.18.inb.final
--rw-rw-r--   0 travis    (2000) travis    (2000)     6084 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Terra/L1B_RSR_LUT/rsr.11.inb.final
--rw-rw-r--   0 travis    (2000) travis    (2000)     9174 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Terra/L1B_RSR_LUT/rsr.29.inb.final
--rw-rw-r--   0 travis    (2000) travis    (2000)     6384 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Terra/L1B_RSR_LUT/rsr.9.inb.final
--rw-rw-r--   0 travis    (2000) travis    (2000)  1425745 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Terra/L1B_RSR_LUT/pfm-in-band-rsr.pdf
--rw-rw-r--   0 travis    (2000) travis    (2000)     6348 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Terra/L1B_RSR_LUT/rsr.14.inb.final
--rw-rw-r--   0 travis    (2000) travis    (2000)    18389 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Terra/L1B_RSR_LUT/rsr.3.inb.final
--rw-rw-r--   0 travis    (2000) travis    (2000)     5484 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Terra/L1B_RSR_LUT/rsr.12.inb.final
--rw-rw-r--   0 travis    (2000) travis    (2000)    11400 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Terra/RSR_Readme_File.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-04 15:35:08.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Terra/Reference_RSR_Dataset/
--rw-rw-r--   0 travis    (2000) travis    (2000)    83465 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Terra/Reference_RSR_Dataset/rsr.29.oobd.det
--rw-rw-r--   0 travis    (2000) travis    (2000)    33345 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Terra/Reference_RSR_Dataset/rsr.13.oobd.det
--rw-rw-r--   0 travis    (2000) travis    (2000)    33429 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Terra/Reference_RSR_Dataset/rsr.21.oobd.det
--rw-rw-r--   0 travis    (2000) travis    (2000)    30545 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Terra/Reference_RSR_Dataset/rsr.12.oobd.det
--rw-rw-r--   0 travis    (2000) travis    (2000)    30545 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Terra/Reference_RSR_Dataset/rsr.25.oobd.det
--rw-rw-r--   0 travis    (2000) travis    (2000)    33345 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Terra/Reference_RSR_Dataset/rsr.22.oobd.det
--rw-rw-r--   0 travis    (2000) travis    (2000)    85369 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Terra/Reference_RSR_Dataset/rsr.31.oobd.det
--rw-rw-r--   0 travis    (2000) travis    (2000)    33737 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Terra/Reference_RSR_Dataset/rsr.20.oobd.det
--rw-rw-r--   0 travis    (2000) travis    (2000)    35025 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Terra/Reference_RSR_Dataset/rsr.28.oobd.det
--rw-rw-r--   0 travis    (2000) travis    (2000)    29425 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Terra/Reference_RSR_Dataset/rsr.15.oobd.det
--rw-rw-r--   0 travis    (2000) travis    (2000)    33065 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Terra/Reference_RSR_Dataset/rsr.16.oobd.det
--rw-rw-r--   0 travis    (2000) travis    (2000)    82177 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Terra/Reference_RSR_Dataset/rsr.30.oobd.det
--rw-rw-r--   0 travis    (2000) travis    (2000)    73105 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Terra/Reference_RSR_Dataset/rsr.4.oobd.det
--rw-rw-r--   0 travis    (2000) travis    (2000)    30265 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Terra/Reference_RSR_Dataset/rsr.23.oobd.det
--rw-rw-r--   0 travis    (2000) travis    (2000)    30433 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Terra/Reference_RSR_Dataset/rsr.8.oobd.det
--rw-rw-r--   0 travis    (2000) travis    (2000)    86713 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Terra/Reference_RSR_Dataset/rsr.34.oobd.det
--rw-rw-r--   0 travis    (2000) travis    (2000)    73245 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Terra/Reference_RSR_Dataset/rsr.3.oobd.det
--rw-rw-r--   0 travis    (2000) travis    (2000)    29425 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Terra/Reference_RSR_Dataset/rsr.18.oobd.det
--rw-rw-r--   0 travis    (2000) travis    (2000)    33065 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Terra/Reference_RSR_Dataset/rsr.14.oobd.det
--rw-rw-r--   0 travis    (2000) travis    (2000)    85901 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Terra/Reference_RSR_Dataset/rsr.35.oobd.det
--rw-rw-r--   0 travis    (2000) travis    (2000)    38021 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Terra/Reference_RSR_Dataset/rsr.27.oobd.det
--rw-rw-r--   0 travis    (2000) travis    (2000)    59385 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Terra/Reference_RSR_Dataset/rsr.5.oobd.det
--rw-rw-r--   0 travis    (2000) travis    (2000)    47625 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Terra/Reference_RSR_Dataset/rsr.7.oobd.det
--rw-rw-r--   0 travis    (2000) travis    (2000)    58825 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Terra/Reference_RSR_Dataset/rsr.6.oobd.det
--rw-rw-r--   0 travis    (2000) travis    (2000)    40905 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Terra/Reference_RSR_Dataset/rsr.26.oobd.det
--rw-rw-r--   0 travis    (2000) travis    (2000)    27745 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Terra/Reference_RSR_Dataset/rsr.17.oobd.det
--rw-rw-r--   0 travis    (2000) travis    (2000)    83045 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Terra/Reference_RSR_Dataset/rsr.32.oobd.det
--rw-rw-r--   0 travis    (2000) travis    (2000)    80693 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Terra/Reference_RSR_Dataset/rsr.36.oobd.det
--rw-rw-r--   0 travis    (2000) travis    (2000)    29397 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Terra/Reference_RSR_Dataset/rsr.9.oobd.det
--rw-rw-r--   0 travis    (2000) travis    (2000)   135321 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Terra/Reference_RSR_Dataset/rsr.1.oobd.det
--rw-rw-r--   0 travis    (2000) travis    (2000)   119305 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Terra/Reference_RSR_Dataset/rsr.2.oobd.det
--rw-rw-r--   0 travis    (2000) travis    (2000)    29985 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Terra/Reference_RSR_Dataset/rsr.24.oobd.det
--rw-rw-r--   0 travis    (2000) travis    (2000)    34997 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Terra/Reference_RSR_Dataset/rsr.10.oobd.det
--rw-rw-r--   0 travis    (2000) travis    (2000)    84753 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Terra/Reference_RSR_Dataset/rsr.33.oobd.det
--rw-rw-r--   0 travis    (2000) travis    (2000)    35025 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Terra/Reference_RSR_Dataset/rsr.11.oobd.det
--rw-rw-r--   0 travis    (2000) travis    (2000)    31665 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/modis/EOS-Terra/Reference_RSR_Dataset/rsr.19.oobd.det
--rw-rw-r--   0 travis    (2000) travis    (2000)    20766 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/data/e490_00a.dat
--rw-rw-r--   0 travis    (2000) travis    (2000)    12624 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/radiance_tb_conversion.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18901 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/utils.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-04 15:35:08.000000 pyspectral-0.9.5/pyspectral/etc/
--rw-rw-r--   0 travis    (2000) travis    (2000)    12589 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/etc/pyspectral.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)     2740 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/config.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14615 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/rayleigh.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2805 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/raw_reader.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1048 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10554 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/solar.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5188 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/atm_correction_ir.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11897 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/rsr_reader.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-04 15:35:08.000000 pyspectral-0.9.5/pyspectral/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3581 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/tests/test_solarflux.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18897 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/tests/test_rad_tb_conversions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6894 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/tests/test_atm_correction_ir.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6105 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/tests/test_blackbody.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1109 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/tests/unittest_helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7824 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/tests/test_reflectance.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7496 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/tests/test_rsr_reader.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    17208 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/tests/data.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14380 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/tests/test_rayleigh.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1936 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6440 2020-02-04 15:29:50.000000 pyspectral-0.9.5/pyspectral/tests/test_utils.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-04 15:35:08.000000 pyspectral-0.9.5/pyspectral.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)      869 2020-02-04 15:35:08.000000 pyspectral-0.9.5/pyspectral.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-02-04 15:35:08.000000 pyspectral-0.9.5/pyspectral.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       11 2020-02-04 15:35:08.000000 pyspectral-0.9.5/pyspectral.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-02-04 15:35:08.000000 pyspectral-0.9.5/pyspectral.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)     9826 2020-02-04 15:35:08.000000 pyspectral-0.9.5/pyspectral.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      215 2020-02-04 15:35:08.000000 pyspectral-0.9.5/pyspectral.egg-info/requires.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-04 15:35:08.000000 pyspectral-0.9.5/doc/
--rw-rw-r--   0 travis    (2000) travis    (2000)      948 2020-02-04 15:29:50.000000 pyspectral-0.9.5/doc/api.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)    11297 2020-02-04 15:29:50.000000 pyspectral-0.9.5/doc/37_reflectance.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     4606 2020-02-04 15:29:50.000000 pyspectral-0.9.5/doc/Makefile
--rw-rw-r--   0 travis    (2000) travis    (2000)     8863 2020-02-04 15:29:50.000000 pyspectral-0.9.5/doc/conf.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1633 2020-02-04 15:29:50.000000 pyspectral-0.9.5/doc/rsr_plotting.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     3037 2020-02-04 15:29:50.000000 pyspectral-0.9.5/doc/usage.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     6470 2020-02-04 15:29:50.000000 pyspectral-0.9.5/doc/installation.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1665 2020-02-04 15:29:50.000000 pyspectral-0.9.5/doc/seviri_example.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)    15464 2020-02-04 15:29:50.000000 pyspectral-0.9.5/doc/rad_definitions.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     2241 2020-02-04 15:29:50.000000 pyspectral-0.9.5/doc/index.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      251 2020-02-04 15:29:50.000000 pyspectral-0.9.5/doc/rsr_formatting.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-04 15:35:08.000000 pyspectral-0.9.5/doc/_static/
--rw-rw-r--   0 travis    (2000) travis    (2000)    36583 2020-02-04 15:29:50.000000 pyspectral-0.9.5/doc/_static/sun-satellite-viewing.png
--rw-rw-r--   0 travis    (2000) travis    (2000)    90988 2020-02-04 15:29:50.000000 pyspectral-0.9.5/doc/_static/rsr_band_1080.png
--rw-rw-r--   0 travis    (2000) travis    (2000)    28100 2020-02-04 15:29:50.000000 pyspectral-0.9.5/doc/_static/solar_irradiance.png
--rw-rw-r--   0 travis    (2000) travis    (2000)  1062046 2020-02-04 15:29:50.000000 pyspectral-0.9.5/doc/_static/msg_daysolar_rgb_20131129_1100_overlay_small.png
--rw-rw-r--   0 travis    (2000) travis    (2000)    37718 2020-02-04 15:29:50.000000 pyspectral-0.9.5/doc/_static/solar_irradiance_wnum.png
--rw-rw-r--   0 travis    (2000) travis    (2000)    96588 2020-02-04 15:29:50.000000 pyspectral-0.9.5/doc/_static/truecolor_composite_20170518_nrk_reception_cropped_thumb.png
--rw-rw-r--   0 travis    (2000) travis    (2000)    23076 2020-02-04 15:29:50.000000 pyspectral-0.9.5/doc/_static/olci_ch1.png
--rw-rw-r--   0 travis    (2000) travis    (2000)    88229 2020-02-04 15:29:50.000000 pyspectral-0.9.5/doc/_static/msg_daysolar_rgb_20131129_1100_overlay_small_thumb.png
--rw-rw-r--   0 travis    (2000) travis    (2000)    95408 2020-02-04 15:29:50.000000 pyspectral-0.9.5/doc/_static/refl_subarctic_winter_lambda_0500_ssa_090.png
--rw-rw-r--   0 travis    (2000) travis    (2000)    71568 2020-02-04 15:29:50.000000 pyspectral-0.9.5/doc/_static/mersi2_rsr_band_0040_0070.png
--rw-rw-r--   0 travis    (2000) travis    (2000)   368893 2020-02-04 15:29:50.000000 pyspectral-0.9.5/doc/_static/mpop_germ_day_snow_thumb.png
--rw-rw-r--   0 travis    (2000) travis    (2000)    49093 2020-02-04 15:29:50.000000 pyspectral-0.9.5/doc/_static/rsr_band_M10.png
--rw-rw-r--   0 travis    (2000) travis    (2000)   263339 2020-02-04 15:29:50.000000 pyspectral-0.9.5/doc/_static/pyspectral_header_montage.png
--rw-rw-r--   0 travis    (2000) travis    (2000)    47183 2020-02-04 15:29:50.000000 pyspectral-0.9.5/doc/_static/mersi2_rsr_band_0040_0070_missingbands.png
--rw-rw-r--   0 travis    (2000) travis    (2000)   980761 2020-02-04 15:29:50.000000 pyspectral-0.9.5/doc/_static/msg_day_microphysics_summer_rgb_20131129_1100_overlay_small.png
--rw-rw-r--   0 travis    (2000) travis    (2000)    83313 2020-02-04 15:29:50.000000 pyspectral-0.9.5/doc/_static/msg_day_microphysics_summer_rgb_20131129_1100_overlay_small_thumb.png
--rw-rw-r--   0 travis    (2000) travis    (2000)    96316 2020-02-04 15:29:50.000000 pyspectral-0.9.5/doc/_static/refl_subarctic_winter_lambda_0400_ssa_000.png
--rw-rw-r--   0 travis    (2000) travis    (2000)      100 2020-02-04 15:29:50.000000 pyspectral-0.9.5/doc/rtd_requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     3696 2020-02-04 15:29:50.000000 pyspectral-0.9.5/doc/platforms_supported.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     5134 2020-02-04 15:29:50.000000 pyspectral-0.9.5/doc/rayleigh_correction.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       46 2020-02-04 15:29:50.000000 pyspectral-0.9.5/.stickler.yml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-04 15:35:08.000000 pyspectral-0.9.5/rsr_convert_scripts/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2411 2020-02-04 15:29:50.000000 pyspectral-0.9.5/rsr_convert_scripts/convert_avhrr_old2star.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2911 2020-02-04 15:29:50.000000 pyspectral-0.9.5/rsr_convert_scripts/abi_rsr.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2818 2020-02-04 15:29:50.000000 pyspectral-0.9.5/rsr_convert_scripts/cocts_rsr.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5380 2020-02-04 15:29:50.000000 pyspectral-0.9.5/rsr_convert_scripts/ahi_reader.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2588 2020-02-04 15:29:50.000000 pyspectral-0.9.5/rsr_convert_scripts/split_metop_avhrr_rsrfile.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6077 2020-02-04 15:29:50.000000 pyspectral-0.9.5/rsr_convert_scripts/metimage_rsr.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10470 2020-02-04 15:29:50.000000 pyspectral-0.9.5/rsr_convert_scripts/seviri_rsr.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8029 2020-02-04 15:29:50.000000 pyspectral-0.9.5/rsr_convert_scripts/modis_rsr.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2535 2020-02-04 15:29:50.000000 pyspectral-0.9.5/rsr_convert_scripts/aatsr_reader.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9663 2020-02-04 15:29:50.000000 pyspectral-0.9.5/rsr_convert_scripts/viirs_rsr.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3827 2020-02-04 15:29:50.000000 pyspectral-0.9.5/rsr_convert_scripts/agri_rsr.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2940 2020-02-04 15:29:50.000000 pyspectral-0.9.5/rsr_convert_scripts/mersi2_rsr.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3591 2020-02-04 15:29:50.000000 pyspectral-0.9.5/rsr_convert_scripts/ami_reader.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4254 2020-02-04 15:29:50.000000 pyspectral-0.9.5/rsr_convert_scripts/olci_rsr.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2789 2020-02-04 15:29:50.000000 pyspectral-0.9.5/rsr_convert_scripts/oli_reader.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3374 2020-02-04 15:29:50.000000 pyspectral-0.9.5/rsr_convert_scripts/avhrr_rsr.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2652 2020-02-04 15:29:50.000000 pyspectral-0.9.5/rsr_convert_scripts/slstr_rsr.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5484 2020-02-04 15:29:50.000000 pyspectral-0.9.5/rsr_convert_scripts/README.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     4998 2020-02-04 15:29:50.000000 pyspectral-0.9.5/rsr_convert_scripts/msi_reader.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2883 2020-02-04 15:29:50.000000 pyspectral-0.9.5/rsr_convert_scripts/virr_rsr.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-04 15:35:08.000000 pyspectral-0.9.5/bin/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1879 2020-02-04 15:29:50.000000 pyspectral-0.9.5/bin/download_atm_correction_luts.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8191 2020-02-04 15:29:50.000000 pyspectral-0.9.5/bin/composite_rsr_plot.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3223 2020-02-04 15:29:50.000000 pyspectral-0.9.5/bin/plot_rsr.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1851 2020-02-04 15:29:50.000000 pyspectral-0.9.5/bin/download_rsr.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-04 15:35:08.000000 pyspectral-0.9.5/appveyor/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2255 2020-02-04 15:29:50.000000 pyspectral-0.9.5/appveyor/run_with_compiler.cmd
--rw-rw-r--   0 travis    (2000) travis    (2000)     2327 2020-02-04 15:29:50.000000 pyspectral-0.9.5/appveyor/install.ps1
--rw-rw-r--   0 travis    (2000) travis    (2000)      174 2020-02-04 15:29:50.000000 pyspectral-0.9.5/.gitattributes
--rw-rw-r--   0 travis    (2000) travis    (2000)      189 2020-02-04 15:29:50.000000 pyspectral-0.9.5/.landscape.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      350 2020-02-04 15:29:50.000000 pyspectral-0.9.5/.gitignore
--rw-rw-r--   0 travis    (2000) travis    (2000)     6408 2020-02-04 15:29:50.000000 pyspectral-0.9.5/.gitchangelog.rc
--rw-rw-r--   0 travis    (2000) travis    (2000)      374 2020-02-04 15:35:08.000000 pyspectral-0.9.5/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1526 2020-02-04 15:29:50.000000 pyspectral-0.9.5/.travis.yml
--rw-rw-r--   0 travis    (2000) travis    (2000)      673 2020-02-04 15:29:50.000000 pyspectral-0.9.5/RELEASING.md
--rw-rw-r--   0 travis    (2000) travis    (2000)       22 2020-02-04 15:29:50.000000 pyspectral-0.9.5/.git_archival.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1405 2020-02-04 15:29:50.000000 pyspectral-0.9.5/appveyor.yml
--rw-rw-r--   0 travis    (2000) travis    (2000)     9230 2020-02-04 15:29:50.000000 pyspectral-0.9.5/CHANGELOG.md
--rw-rw-r--   0 travis    (2000) travis    (2000)     3978 2020-02-04 15:29:50.000000 pyspectral-0.9.5/setup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      223 2020-02-04 15:29:50.000000 pyspectral-0.9.5/.pre-commit-config.yaml
+drwxrwxr-x   0 a000680    (964) users      (100)        0 2014-06-17 09:47:11.000000 pyspectral-v0.1.0/
+drwxrwxr-x   0 a000680    (964) users      (100)        0 2014-06-17 09:47:11.000000 pyspectral-v0.1.0/etc/
+-rw-rw-r--   0 a000680    (964) users      (100)     1051 2014-06-17 09:16:17.000000 pyspectral-v0.1.0/etc/pyspectral.cfg_template
+-rw-rw-r--   0 a000680    (964) users      (100)       59 2014-06-17 09:47:11.000000 pyspectral-v0.1.0/setup.cfg
+-rw-rw-r--   0 a000680    (964) users      (100)       15 2013-10-14 21:15:51.000000 pyspectral-v0.1.0/MANIFEST.in
+-rw-rw-r--   0 a000680    (964) users      (100)     2517 2014-06-17 09:16:17.000000 pyspectral-v0.1.0/setup.py
+-rw-rw-r--   0 a000680    (964) users      (100)      600 2014-06-17 09:47:11.000000 pyspectral-v0.1.0/PKG-INFO
+drwxrwxr-x   0 a000680    (964) users      (100)        0 2014-06-17 09:47:11.000000 pyspectral-v0.1.0/pyspectral.egg-info/
+-rw-rw-r--   0 a000680    (964) users      (100)        1 2013-10-15 11:52:50.000000 pyspectral-v0.1.0/pyspectral.egg-info/not-zip-safe
+-rw-rw-r--   0 a000680    (964) users      (100)        1 2014-06-17 09:47:11.000000 pyspectral-v0.1.0/pyspectral.egg-info/dependency_links.txt
+-rw-rw-r--   0 a000680    (964) users      (100)      600 2014-06-17 09:47:11.000000 pyspectral-v0.1.0/pyspectral.egg-info/PKG-INFO
+-rw-rw-r--   0 a000680    (964) users      (100)      653 2014-06-17 09:47:11.000000 pyspectral-v0.1.0/pyspectral.egg-info/SOURCES.txt
+-rw-rw-r--   0 a000680    (964) users      (100)       11 2014-06-17 09:47:11.000000 pyspectral-v0.1.0/pyspectral.egg-info/top_level.txt
+-rw-rw-r--   0 a000680    (964) users      (100)       52 2014-06-17 09:47:11.000000 pyspectral-v0.1.0/pyspectral.egg-info/requires.txt
+drwxrwxr-x   0 a000680    (964) users      (100)        0 2014-06-17 09:47:11.000000 pyspectral-v0.1.0/pyspectral/
+-rw-rw-r--   0 a000680    (964) users      (100)     3193 2014-06-17 09:16:17.000000 pyspectral-v0.1.0/pyspectral/utils.py
+-rw-rw-r--   0 a000680    (964) users      (100)    10540 2014-06-17 09:16:17.000000 pyspectral-v0.1.0/pyspectral/seviri_rsr.py
+-rw-rw-r--   0 a000680    (964) users      (100)     9273 2014-06-17 09:16:17.000000 pyspectral-v0.1.0/pyspectral/radiance_tb_conversion.py
+-rw-rw-r--   0 a000680    (964) users      (100)     1160 2014-06-15 18:58:27.000000 pyspectral-v0.1.0/pyspectral/myrefl.py
+-rw-rw-r--   0 a000680    (964) users      (100)     5332 2014-06-17 09:16:17.000000 pyspectral-v0.1.0/pyspectral/blackbody.py
+-rw-rw-r--   0 a000680    (964) users      (100)     6613 2014-06-17 09:16:17.000000 pyspectral-v0.1.0/pyspectral/near_infrared_reflectance.py
+-rw-rw-r--   0 a000680    (964) users      (100)     2104 2014-06-12 13:23:09.000000 pyspectral-v0.1.0/pyspectral/mytest.py
+-rw-rw-r--   0 a000680    (964) users      (100)      896 2014-06-12 13:23:10.000000 pyspectral-v0.1.0/pyspectral/__init__.py
+-rw-rw-r--   0 a000680    (964) users      (100)     8403 2014-06-17 09:16:17.000000 pyspectral-v0.1.0/pyspectral/modis_rsr.py
+-rw-rw-r--   0 a000680    (964) users      (100)     2059 2014-06-12 13:23:09.000000 pyspectral-v0.1.0/pyspectral/myoldtest.py
+-rw-rw-r--   0 a000680    (964) users      (100)    10225 2014-06-17 09:16:17.000000 pyspectral-v0.1.0/pyspectral/solar.py
+-rw-rw-r--   0 a000680    (964) users      (100)     1703 2014-06-15 18:49:42.000000 pyspectral-v0.1.0/pyspectral/plot_tb_vs_rad.py
+-rw-rw-r--   0 a000680    (964) users      (100)     4747 2014-06-17 09:16:17.000000 pyspectral-v0.1.0/pyspectral/rsr_reader.py
+-rw-rw-r--   0 a000680    (964) users      (100)     9198 2014-06-17 09:16:17.000000 pyspectral-v0.1.0/pyspectral/viirs_rsr.py
+-rw-rw-r--   0 a000680    (964) users      (100)     5300 2014-06-17 09:16:17.000000 pyspectral-v0.1.0/pyspectral/avhrr_rsr.py
+-rw-rw-r--   0 a000680    (964) users      (100)      806 2014-06-12 13:23:09.000000 pyspectral-v0.1.0/pyspectral/version.py
```

### Comparing `pyspectral-0.9.5/pyspectral/near_infrared_reflectance.py` & `pyspectral-v0.1.0/pyspectral/solar.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
-# Copyright (c) 2014-2019 Adam.Dybbroe
+# Copyright (c) 2013, 2014 Adam.Dybbroe
 
 # Author(s):
 
-#   Adam.Dybbroe <adam.dybbroe@smhi.se>
-#   Panu Lahtinen <panu.lahtinen@fmi.fi>
+#   Adam.Dybbroe <a000680@c14526.ad.smhi.se>
 
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 
 # This program is distributed in the hope that it will be useful,
@@ -18,281 +17,265 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 """
-Derive NIR reflectances of a a band in the 3-4 micron window region.
-
-Derive the Near-Infrared reflectance of a given band in the solar and
-thermal range (usually the 3.7-3.9 micron band) using a thermal atmospheric
-window channel (usually around 11-12 microns).
+Module to read solar irradiance spectra and calculate the solar flux over
+various instrument bands given their relative spectral response functions
 """
 
-import os
-import numpy as np
-try:
-    from dask.array import where, logical_or, asanyarray, array
-except ImportError:
-    from numpy import where, logical_or, asanyarray, array
-
-from pyspectral.solar import (SolarIrradianceSpectrum,
-                              TOTAL_IRRADIANCE_SPECTRUM_2000ASTM)
-from pyspectral.utils import BANDNAMES, get_bandname_from_wavelength
-from pyspectral.utils import TB2RAD_DIR
-from pyspectral.radiance_tb_conversion import RadTbConverter
-from pyspectral.config import get_config
-
 import logging
 LOG = logging.getLogger(__name__)
 
+from pkg_resources import resource_filename
 
-EPSILON = 0.005
-TB_MIN = 150.
-TB_MAX = 360.
+# STANDARD SPECTRA from Air Mass Zero: http://rredc.nrel.gov/solar/spectra/am0/
+#    * 2000 ASTM Standard Extraterrestrial Spectrum Reference E-490-00
+#      (119.5 - 1,000,000.0 nm)
+TOTAL_IRRADIANCE_SPECTRUM_2000ASTM = resource_filename(__name__,
+                                                       'data/e490_00a.dat')
 
 
-class Calculator(RadTbConverter):
-    """
-    A thermal near-infrared (~3.7 micron) band reflectance calculator.
-
-    Given the relative spectral response of the NIR band, the solar zenith
-    angle, and the brightness temperatures of the NIR and the Thermal bands,
-    derive the solar reflectance for the NIR band removing the thermal
-    (terrestrial) part. The in-band solar flux over the NIR band is
-    optional. If not provided, it will be calculated here!
+class SolarIrradianceSpectrum(object):
 
-    The relfectance calculated is without units and should be between 0 and 1.
+    """Total Top of Atmosphere (TOA) Solar Irradiance Spectrum
+    Wavelength is in units of microns (10^-6 m).
+    The spectral Irradiance in the file TOTAL_IRRADIANCE_SPECTRUM_2000ASTM is
+    in units of W/m^2/micron
     """
 
-    def __init__(self, platform_name, instrument, band, **kwargs):
-        """Initialize the Class instance."""
-        super(Calculator, self).__init__(platform_name, instrument, band, **kwargs)
-
-        from numbers import Number
-        self.bandname = None
-        self.bandwavelength = None
-
-        if isinstance(band, str):
-            self.bandname = BANDNAMES.get(self.instrument, BANDNAMES['generic']).get(band, band)
-            self.bandwavelength = self.rsr[self.bandname][
-                'det-1']['central_wavelength']
-        elif isinstance(band, Number):
-            self.bandwavelength = band
-            self.bandname = get_bandname_from_wavelength(self.instrument, band, self.rsr)
-
-        if self.bandwavelength > 3.95 or self.bandwavelength < 3.5:
-            raise NotImplementedError('NIR reflectance is not supported outside ' +
-                                      'the 3.5-3.95 micron interval')
-
-        options = get_config()
-
-        self.solar_flux = kwargs.get('solar_flux', None)
-        if self.solar_flux is None:
-            self._get_solarflux()
-
-        self._rad3x = None
-        self._rad3x_t11 = None
-        self._solar_radiance = None
-        self._rad3x_correction = 1.0
-        self._r3x = None
-        self._e3x = None
-        self.lutfile = None
-
-        if 'detector' in kwargs:
-            self.detector = kwargs['detector']
-        else:
-            self.detector = 'det-1'
-
-        platform_sensor = platform_name + '-' + instrument
-        if platform_sensor in options and 'tb2rad_lut_filename' in options[platform_sensor]:
-            if isinstance(options[platform_sensor]['tb2rad_lut_filename'], dict):
-                for item in options[platform_sensor]['tb2rad_lut_filename']:
-                    if item == self.bandname or item == self.bandname.lower():
-                        self.lutfile = options[platform_sensor]['tb2rad_lut_filename'][item]
-                        break
-                if self.lutfile is None:
-                    LOG.warning("Failed determine LUT filename from config: %s", str(
-                        options[platform_sensor]['tb2rad_lut_filename']))
+    def __init__(self, filename, **options):
+        """
+        Input:
+        filename: Filename of the solar irradiance spectrum
+        dlambda:
+        Delta wavelength: the step in wavelength defining the resolution on
+        which to integrate/convolute.
+        """
+        self.wavelength = None
+        self.wavenumber = None
+        self.irradiance = None
+        self.filename = filename
+        self.ipol_wavelength = None
+        self.ipol_irradiance = None
+        self.ipol_channel_response = None
+        # Delta wavelength used when resampling the
+        # spectrum to an evenly spaced grid (using interpolation)
+        if 'wavespace' in options:
+            self.wavespace = options['wavespace']
+        else:
+            self.wavespace = 'wavelength'
+        if 'dlambda' in options:
+            self._dlambda = options['dlambda']
+        else:
+            if self.wavespace == 'wavelength':
+                self._dlambda = 0.005
             else:
-                self.lutfile = options[platform_sensor]['tb2rad_lut_filename']
+                self._dlambda = 1. / (0.005 * 100.)
 
-            if self.lutfile and not self.lutfile.endswith('.npz'):
-                self.lutfile = self.lutfile + '.npz'
+        self._load()
 
-            if self.lutfile and not os.path.exists(os.path.dirname(self.lutfile)):
-                LOG.warning(
-                    "Directory %s does not exist! Check config file", os.path.dirname(self.lutfile))
-                self.lutfile = os.path.join(TB2RAD_DIR, os.path.basename(self.lutfile))
-
-        if self.lutfile is None:
-            LOG.info("No lut filename available in config file. "
-                     "Will generate filename automatically")
-            lutname = 'tb2rad_lut_{0}_{1}_{band}'.format(
-                self.platform_name.lower(), self.instrument.lower(), band=self.bandname.lower())
-            self.lutfile = os.path.join(TB2RAD_DIR, lutname + '.npz')
-
-        LOG.info("lut filename: " + str(self.lutfile))
-        if not os.path.exists(self.lutfile):
-            self.make_tb2rad_lut(self.lutfile)
-            self.lut = self.read_tb2rad_lut(self.lutfile)
-            LOG.info("LUT file created")
-        else:
-            self.lut = self.read_tb2rad_lut(self.lutfile)
-            LOG.info("File was there and has been read!")
-
-    def derive_rad39_corr(self, bt11, bt13, method='rosenfeld'):
-        """Derive the CO2 correction to be applied to the 3.9 channel.
-
-        Derive the 3.9 radiance correction factor to account for the
-        attenuation of the emitted 3.9 radiance by CO2
-        absorption. Requires the 11 micron window band and the 13.4
-        CO2 absorption band, as e.g. available on SEVIRI. Currently
-        only supports the Rosenfeld method
+        if self.wavespace == 'wavenumber':
+            self.convert2wavenumber()
+            self.units = {'irradiance': 'mW/m^2 (cm^{-1})^{-1}',
+                          'flux': 'mW/m^2'}
+        else:
+            self.units = {'irradiance': '$W/m^2 (1e-6*m)^{-1})',
+                          'flux': 'W/m^2'}
 
+    def convert2wavenumber(self):
         """
-        if method != 'rosenfeld':
-            raise AttributeError("Only CO2 correction for SEVIRI using "
-                                 "the Rosenfeld equation is supported!")
-
-        LOG.debug("Derive the 3.9 micron radiance CO2 correction coefficent")
-        self._rad3x_correction = (bt11 - 0.25 * (bt11 - bt13)) ** 4 / bt11 ** 4
-
-    def _get_solarflux(self):
-        """Derive the in-band solar flux from rsr over the Near IR band (3.7 or 3.9 microns)."""
-        solar_spectrum = \
-            SolarIrradianceSpectrum(TOTAL_IRRADIANCE_SPECTRUM_2000ASTM,
-                                    dlambda=0.0005,
-                                    wavespace=self.wavespace)
-        self.solar_flux = solar_spectrum.inband_solarflux(self.rsr[self.bandname])
-
-    def emissive_part_3x(self, tb=True):
-        """Get the emissive part of the 3.x band."""
-        try:
-            # Emissive part:
-            self._e3x = self._rad3x_t11 * (1 - self._r3x)
-            # Unsure how much sense it makes to apply the co2 correction term here!?
-            # FIXME!
-            # self._e3x *= self._rad3x_correction
-
-        except TypeError:
-            LOG.warning(
-                "Couldn't derive the emissive part \n" +
-                "Please derive the relfectance prior to requesting the emissive part")
-
-        if tb:
-            return self.radiance2tb(self._e3x)
-        else:
-            return self._e3x
-
-    def reflectance_from_tbs(self, sun_zenith, tb_near_ir, tb_thermal, **kwargs):
-        """Derive reflectances from Tb's in the 3.x band.
-
-        The relfectance calculated is without units and should be between 0 and 1.
-
-        Inputs:
-
-          sun_zenith: Sun zenith angle for every pixel - in degrees
-
-          tb_near_ir: The 3.7 (or 3.9 or equivalent) IR Tb's at every pixel
-                      (Kelvin)
-
-          tb_thermal: The 10.8 (or 11 or 12 or equivalent) IR Tb's at every
-                      pixel (Kelvin)
-
-          tb_ir_co2: The 13.4 micron channel (or similar - co2 absorption band)
-                     brightness temperatures at every pixel. If None, no CO2
-                     absorption correction will be applied.
+        Convert from wavelengths to wavenumber. 
 
+        Units:
+          Wavelength: micro meters (1e-6 m)
+          Wavenumber: cm-1
         """
-        # Check for dask arrays
-        if hasattr(tb_near_ir, 'compute') or hasattr(tb_thermal, 'compute'):
-            compute = False
-        else:
-            compute = True
-        if hasattr(tb_near_ir, 'mask') or hasattr(tb_thermal, 'mask'):
-            is_masked = True
+
+        self.wavenumber = 1. / (1e-4 * self.wavelength[::-1])
+        self.irradiance = (self.irradiance[::-1] *
+                           self.wavelength[::-1] * self.wavelength[::-1] * 0.1)
+        self.wavelength = None
+
+    def _load(self):
+        """Read the tabulated spectral irradiance data from file"""
+        import numpy as np
+        self.wavelength, self.irradiance = np.genfromtxt(
+            self.filename, unpack=True)
+
+    def solar_constant(self):
+        """Calculate the solar constant"""
+        import numpy as np
+        if self.wavenumber != None:
+            return np.trapz(self.irradiance, self.wavenumber)
+        elif self.wavelength != None:
+            return np.trapz(self.irradiance, self.wavelength)
         else:
-            is_masked = False
+            raise TypeError('Neither wavelengths nor wavenumbers available!')
+
+    def inband_solarflux(self, rsr, scale=1.0, **options):
+        """Derive the inband solar flux for a given instrument relative
+        spectral response valid for an earth-sun distance of one AU."""
+
+        return self._band_calculations(rsr, True, scale, **options)
+
+    # def inband_solarirradiance(self, rsr, scale=1.0, **options):
+    #     """Derive the inband solar irradiance for a given instrument relative
+    #     spectral response valid for an earth-sun distance of one AU."""
+
+    #     return self._band_calculations(rsr, False, scale, **options)
+
+    def _band_calculations(self, rsr, flux, scale, **options):
+        """Derive the inband solar flux or inband solar irradiance for a given
+        instrument relative spectral response valid for an earth-sun distance
+        of one AU.
+
+        rsr: Relative Spectral Response (one detector only)
+        Dictionary with two members 'wavelength' and 'response'
+        options:
+        detector: Detector number (between 1 and N - N=number of detectors
+        for channel)
+        """
+        import numpy as np
+        from scipy.interpolate import InterpolatedUnivariateSpline
 
-        if np.isscalar(tb_near_ir):
-            tb_nir = array([tb_near_ir, ])
+        if 'detector' in options:
+            detector = options['detector']
         else:
-            tb_nir = asanyarray(tb_near_ir)
+            detector = 1
 
-        if np.isscalar(tb_thermal):
-            tb_therm = array([tb_thermal, ])
+        # Resample/Interpolate the response curve:
+        if self.wavespace == 'wavelength':
+            if 'response' in rsr:
+                wvl = rsr['wavelength'] * scale
+                resp = rsr['response']
+            else:
+                wvl = rsr['det-%d' % detector]['wavelength'] * scale
+                resp = rsr['det-%d' % detector]['response']
         else:
-            tb_therm = asanyarray(tb_thermal)
+            if 'response' in rsr:
+                wvl = rsr['wavenumber'] * scale
+                resp = rsr['response']
+            else:
+                wvl = rsr['det-%d' % detector]['wavenumber'] * scale
+                resp = rsr['det-%d' % detector]['response']
 
-        if tb_therm.shape != tb_nir.shape:
-            errmsg = 'Dimensions do not match! {0} and {1}'.format(
-                str(tb_therm.shape), str(tb_nir.shape))
-            raise ValueError(errmsg)
+        start = wvl[0]
+        end = wvl[-1]
+        # print "Start and end: ", start, end
+        LOG.debug("Begin and end wavelength/wavenumber: %f %f " % (start, end))
+        dlambda = self._dlambda
+        xspl = np.linspace(start, end, (end - start) / dlambda)
+
+        ius = InterpolatedUnivariateSpline(wvl, resp)
+        resp_ipol = ius(xspl)
+
+        # Interpolate solar spectrum to specified resolution and over specified
+        # Spectral interval:
+        self.interpolate(dlambda=dlambda, ival_wavelength=(start, end))
+
+        # Mask out outside the response curve:
+        maskidx = np.logical_and(np.greater_equal(self.ipol_wavelength, start),
+                                 np.less_equal(self.ipol_wavelength, end))
+        wvl = np.repeat(self.ipol_wavelength, maskidx)
+        irr = np.repeat(self.ipol_irradiance, maskidx)
+
+        # Calculate the solar-flux: (w/m2)
+        if flux:
+            return np.trapz(irr * resp_ipol, wvl)
+        else:
+            # Divide by the equivalent band width:
+            return np.trapz(irr * resp_ipol, wvl) / np.trapz(resp_ipol, wvl)
 
-        tb_ir_co2 = kwargs.get('tb_ir_co2')
-        lut = kwargs.get('lut', self.lut)
+    def interpolate(self, **options):
+        """Interpolate Irradiance to a specified evenly spaced resolution/grid
+        This is necessary to make integration and folding (with a channel
+        relative spectral response) straightforward.
+
+        dlambda = wavelength interval in microns
+        start = Start of the wavelength interval (left/lower)
+        end = End of the wavelength interval (right/upper end)
+        options:
+        dlambda: Delta wavelength used when interpolating/resampling
+        ival_wavelength: Tuple. The start and end interval in wavelength
+        space, defining where to integrate/convolute the spectral response
+        curve on the spectral irradiance data.
+        """
+        from numpy import linspace
+        from scipy.interpolate import InterpolatedUnivariateSpline
 
-        if tb_ir_co2 is None:
-            co2corr = False
-            tbco2 = None
+        # The user defined wavelength span is not yet used:
+        # FIXME!
+        if 'ival_wavelength' in options:
+            ival_wavelength = options['ival_wavelength']
         else:
-            co2corr = True
-            if np.isscalar(tb_ir_co2):
-                tbco2 = array([tb_ir_co2, ])
+            ival_wavelength = None
+
+        if 'dlambda' in options:
+            self._dlambda = options['dlambda']
+
+        if ival_wavelength == None:
+            if self.wavespace == 'wavelength':
+                start = self.wavelength[0]
+                end = self.wavelength[-1]
             else:
-                tbco2 = asanyarray(tb_ir_co2)
+                start = self.wavenumber[0]
+                end = self.wavenumber[-1]
+        else:
+            start, end = ival_wavelength
 
-        if not self.rsr:
-            raise NotImplementedError("Reflectance calculations without "
-                                      "rsr not yet supported!")
+        xspl = linspace(start, end, (end - start) / self._dlambda)
+        if self.wavespace == 'wavelength':
+            ius = InterpolatedUnivariateSpline(
+                self.wavelength, self.irradiance)
+        else:
+            ius = InterpolatedUnivariateSpline(
+                self.wavenumber, self.irradiance)
+        yspl = ius(xspl)
+
+        self.ipol_wavelength = xspl
+        self.ipol_irradiance = yspl
+
+    def plot(self, plotname=None, **options):
+        """Plot the data"""
+        if 'color' in options:
+            color = options['color']
+        else:
+            color = 'blue'
 
-        # Assume rsr is in microns!!!
-        # FIXME!
-        self._rad3x_t11 = self.tb2radiance(tb_therm, lut=lut)['radiance']
-        thermal_emiss_one = self._rad3x_t11 * self.rsr_integral
+        if self.wavespace == "wavelength":
+            xlabel = "Wavelength ($\mu m$)"
+            ylabel = "Irradiance ($W/(m^2 \mu m$))"
+            xlim = [0, 4.2]
+            xwl, yir = self.wavelength, self.irradiance
+        elif self.wavespace == "wavenumber":
+            xlabel = "Wavenumber ($cm^{-1}$)"
+            ylabel = "Irradiance ($mW/m^2 (cm^{-1})^{-1}$))"
+            xlim = [0, 35000]
+            xwl, yir = self.wavenumber, self.irradiance
+        else:
+            raise TypeError('Neither wavelengths nor wavenumbers available!')
 
-        l_nir = self.tb2radiance(tb_nir, lut=lut)['radiance'] * self.rsr_integral
+        import pylab
+        from matplotlib import rcParams
+        rcParams['text.usetex'] = True
+        rcParams['text.latex.unicode'] = True
+
+        fig = pylab.figure(figsize=(8, 4))
+        plot_title = "Solar Irradiance Spectrum"
+        pylab.title(plot_title)
+        ax = fig.add_subplot(111)
+
+        ax.plot(xwl, yir, '-', color=color)
+
+        pylab.xlabel(xlabel)
+        pylab.ylabel(ylabel)
+        pylab.xlim(xlim)
+        pylab.ylim([0, yir.max()])
+        ax.grid(True)
 
-        if thermal_emiss_one.ravel().shape[0] < 10:
-            LOG.info('thermal_emiss_one = %s', str(thermal_emiss_one))
-        if l_nir.ravel().shape[0] < 10:
-            LOG.info('l_nir = %s', str(l_nir))
-
-        sunzmask = (sun_zenith < 0.0) | (sun_zenith > 88.0)
-        sunz = sun_zenith.clip(0, 88.0)
-
-        mu0 = np.cos(np.deg2rad(sunz))
-        # mu0 = np.where(np.less(mu0, 0.1), 0.1, mu0)
-        self._rad3x = l_nir
-        self._solar_radiance = self.solar_flux * mu0 / np.pi
-
-        # CO2 correction to the 3.9 radiance, only if tbs of a co2 band around
-        # 13.4 micron is provided:
-        if co2corr:
-            self.derive_rad39_corr(tb_therm, tbco2)
-            LOG.info("CO2 correction applied...")
-        else:
-            self._rad3x_correction = 1.0
-
-        corrected_thermal_emiss_one = thermal_emiss_one * self._rad3x_correction
-        nomin = l_nir - corrected_thermal_emiss_one
-        denom = self._solar_radiance - corrected_thermal_emiss_one
-        data = nomin / denom
-        mask = denom < EPSILON
-
-        logical_or(sunzmask, mask, out=mask)
-        logical_or(mask, np.isnan(tb_nir), out=mask)
-
-        self._r3x = where(mask, np.nan, data)
-
-        # Reflectances should be between 0 and 1, but values above 1 is
-        # perfectly possible and okay! (Multiply by 100 to get reflectances
-        # in percent)
-        if hasattr(self._r3x, 'compute') and compute:
-            res = self._r3x.compute()
-        else:
-            res = self._r3x
-        if is_masked:
-            res = np.ma.masked_invalid(res)
-        return res
+        if plotname == None:
+            pylab.show()
+        else:
+            fig.savefig(plotname)
```

### Comparing `pyspectral-0.9.5/rsr_convert_scripts/seviri_rsr.py` & `pyspectral-v0.1.0/pyspectral/seviri_rsr.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 #!/usr/bin/env python
-
 # -*- coding: utf-8 -*-
 
-# Copyright (c) 2013-2018 Adam.Dybbroe
+# Copyright (c) 2013, 2014 Adam.Dybbroe
 
 # Author(s):
 
-#   Adam.Dybbroe <adam.dybbroe@smhi.se>
-#   Panu Lahtinen <panu.lahtinen@fmi.fi>
+#   Adam.Dybbroe <a000680@c14526.ad.smhi.se>
 
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 
 # This program is distributed in the hope that it will be useful,
@@ -22,46 +20,68 @@
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 """Interface to the SEVIRI spectral response functions for all four MSG
 satellites
 """
 
+import logging
+LOG = logging.getLogger(__name__)
+
+import ConfigParser
 import os
+
+try:
+    CONFIG_FILE = os.environ['PSP_CONFIG_FILE']
+except KeyError:
+    LOG.exception('Environment variable PSP_CONFIG_FILE not set!')
+    raise
+
+if not os.path.exists(CONFIG_FILE) or not os.path.isfile(CONFIG_FILE):
+    raise IOError(str(CONFIG_FILE) + " pointed to by the environment " +
+                  "variable PSP_CONFIG_FILE is not a file or does not exist!")
+
 from xlrd import open_workbook
 import numpy as np
-from pyspectral.config import get_config
-import pkg_resources
-import logging
 
-LOG = logging.getLogger(__name__)
-DATA_PATH = pkg_resources.resource_filename('pyspectral', 'data/')
+METEOSAT_SAT = {'meteosat10': 'met10',
+                'meteosat9': 'met9',
+                'meteosat8': 'met8',
+                'meteosat11': 'met11',
+                }
 
 
 class Seviri(object):
 
-    """Class for Seviri RSR"""
-
     def __init__(self, wavespace='wavelength'):
         """
         Read the seviri relative spectral responses for all channels and all
         MSG satellites.
 
         Optional input: 'wavespace'. Equals 'wavelength' (units of micron's) on
         default. Can be 'wavenumber' in which case the unit is in cm-1.
 
         """
-        options = get_config()
 
-        self.seviri_path = options['seviri'].get('path')
-        if not os.path.exists(self.seviri_path):
-            self.seviri_path = os.path.join(
-                DATA_PATH, options['seviri'].get('filename'))
+        conf = ConfigParser.ConfigParser()
+        try:
+            conf.read(CONFIG_FILE)
+        except ConfigParser.NoSectionError:
+            LOG.exception(
+                'Failed reading configuration file: ' + str(CONFIG_FILE))
+            raise
+
+        options = {}
+        for option, value in conf.items('seviri', raw=True):
+            options[option] = value
+
+        self.seviri_path = options.get('path')
 
-        LOG.debug("Original RSR file from EUMETSAT: {}".format(self.seviri_path))
+        for option, value in conf.items('general', raw=True):
+            options[option] = value
 
         self.output_dir = options.get('rsr_dir', './')
 
         self.rsr = None
         self._load()
         self.wavespace = wavespace
         if wavespace not in ['wavelength', 'wavenumber']:
@@ -76,49 +96,50 @@
         self.central_wavenumber = None
         self.central_wavelength = None
 
         self.get_centrals()
 
     def _load(self, filename=None):
         """Read the SEVIRI rsr data"""
+
         if not filename:
             filename = self.seviri_path
 
-        wb_ = open_workbook(filename)
+        wb = open_workbook(filename)
 
         self.rsr = {}
         sheet_names = []
-        for sheet in wb_.sheets():
+        for sheet in wb.sheets():
             if sheet.name in ['Info', 'Requirements']:
                 continue
             ch_name = sheet.name.strip()
             sheet_names.append(sheet.name.strip())
 
             self.rsr[ch_name] = {'wavelength': None,
-                                 'Meteosat-8': None,
-                                 'Meteosat-9': None,
-                                 'Meteosat-10': None,
-                                 'Meteosat-11': None}
+                                 'met8': None,
+                                 'met9': None,
+                                 'met10': None,
+                                 'met11': None}
 
             if ch_name.startswith('HRV'):
                 wvl = np.array(
                     sheet.col_values(0, start_rowx=37, end_rowx=137))
                 # TODO: Add the 'extended' responses as well!
                 met8 = np.array(
                     sheet.col_values(1, start_rowx=37, end_rowx=137))
                 met9 = np.array(
                     sheet.col_values(3, start_rowx=37, end_rowx=137))
                 met10 = np.array(
                     sheet.col_values(5, start_rowx=37, end_rowx=137))
                 met11 = np.array(
                     sheet.col_values(6, start_rowx=37, end_rowx=137))
-                self.rsr[ch_name]['Meteosat-8'] = met8
-                self.rsr[ch_name]['Meteosat-9'] = met9
-                self.rsr[ch_name]['Meteosat-10'] = met10
-                self.rsr[ch_name]['Meteosat-11'] = met11
+                self.rsr[ch_name]['met8'] = met8
+                self.rsr[ch_name]['met9'] = met9
+                self.rsr[ch_name]['met10'] = met10
+                self.rsr[ch_name]['met11'] = met11
             elif ch_name.startswith('IR'):
                 wvl = np.array(
                     sheet.col_values(0, start_rowx=13, end_rowx=113))
                 met8_95 = np.array(
                     sheet.col_values(1, start_rowx=13, end_rowx=113))
                 met9_95 = np.array(
                     sheet.col_values(3, start_rowx=13, end_rowx=113))
@@ -130,67 +151,60 @@
                     sheet.col_values(2, start_rowx=13, end_rowx=113))
                 met9_85 = np.array(
                     sheet.col_values(4, start_rowx=13, end_rowx=113))
                 met10_85 = np.array(
                     sheet.col_values(6, start_rowx=13, end_rowx=113))
                 met11_85 = np.array(
                     sheet.col_values(8, start_rowx=13, end_rowx=113))
-                self.rsr[ch_name]['Meteosat-8'] = {'95': met8_95,
-                                                   '85': met8_85}
-                self.rsr[ch_name]['Meteosat-9'] = {'95': met9_95,
-                                                   '85': met9_85}
-                self.rsr[ch_name]['Meteosat-10'] = {'95': met10_95,
-                                                    '85': met10_85}
-                self.rsr[ch_name]['Meteosat-11'] = {'95': met11_95,
-                                                    '85': met11_85}
+                self.rsr[ch_name]['met8'] = {'95': met8_95, '85': met8_85}
+                self.rsr[ch_name]['met9'] = {'95': met9_95, '85': met9_85}
+                self.rsr[ch_name]['met10'] = {'95': met10_95, '85': met10_85}
+                self.rsr[ch_name]['met11'] = {'95': met11_95, '85': met11_85}
             else:
                 wvl = np.array(
                     sheet.col_values(0, start_rowx=12, end_rowx=112))
                 met8 = np.array(
                     sheet.col_values(1, start_rowx=12, end_rowx=112))
                 met9 = np.array(
                     sheet.col_values(2, start_rowx=12, end_rowx=112))
                 met10 = np.array(
                     sheet.col_values(3, start_rowx=12, end_rowx=112))
                 met11 = np.array(
                     sheet.col_values(4, start_rowx=12, end_rowx=112))
-                self.rsr[ch_name]['Meteosat-8'] = met8
-                self.rsr[ch_name]['Meteosat-9'] = met9
-                self.rsr[ch_name]['Meteosat-10'] = met10
-                self.rsr[ch_name]['Meteosat-11'] = met11
+                self.rsr[ch_name]['met8'] = met8
+                self.rsr[ch_name]['met9'] = met9
+                self.rsr[ch_name]['met10'] = met10
+                self.rsr[ch_name]['met11'] = met11
 
             self.rsr[ch_name]['wavelength'] = wvl
 
     def convert2wavenumber(self):
         """Convert from wavelengths to wavenumber"""
+
         for chname in self.rsr.keys():
-            elems = [k for k in self.rsr[chname].keys()]
-            for sat in elems:
+            for sat in self.rsr[chname].keys():
                 if sat == "wavelength":
-                    LOG.debug("Get the wavenumber from the wavelength: sat=%s chname=%s", sat, chname)
-                    wnum = 1. / (1e-4 * self.rsr[chname][sat][:])  # microns to cm
+                    wnum = 1. / (1e-4 * self.rsr[chname][sat])  # microns to cm
                     self.rsr[chname]['wavenumber'] = wnum[::-1]
+                    del self.rsr[chname][sat]
                 else:
                     if type(self.rsr[chname][sat]) is dict:
                         for name in self.rsr[chname][sat].keys():
-                            resp = self.rsr[chname][sat][name][:]
+                            resp = self.rsr[chname][sat][name]
                             self.rsr[chname][sat][name] = resp[::-1]
                     else:
-                        resp = self.rsr[chname][sat][:]
+                        resp = self.rsr[chname][sat]
                         self.rsr[chname][sat] = resp[::-1]
 
-        for chname in self.rsr.keys():
-            del self.rsr[chname]['wavelength']
-
         self.unit = 'cm-1'
 
     def get_centrals(self):
         """Get the central wavenumbers or central wavelengths of all channels,
-        depending on the given 'wavespace'
-        """
+        depending on the given 'wavespace'"""
+
         result = {}
         for chname in self.rsr.keys():
             result[chname] = {}
             if self.wavespace == "wavelength":
                 x__ = self.rsr[chname]["wavelength"]
             else:
                 x__ = self.rsr[chname]["wavenumber"]
@@ -209,64 +223,58 @@
         if self.wavespace == "wavelength":
             self.central_wavelength = result
         else:
             self.central_wavenumber = result
 
 
 def get_central_wave(wavl, resp):
-    """Calculate the central wavelength or the central wavenumber,
-    depending on what is input
-    """
+    """Calculate the central wavelength or the central wavenumber, depending on
+    what is input"""
+
     return np.trapz(resp * wavl, wavl) / np.trapz(resp, wavl)
 
 
-def generate_seviri_file(seviri, platform_name):
+def generate_seviri_file(seviri, platform_id, sat_number):
     """Generate the pyspectral internal common format relative response
-    function file for one SEVIRI
-    """
-    import h5py
+    function file for one SEVIRI"""
 
-    filename = os.path.join(seviri.output_dir,
-                            "rsr_seviri_{0}.h5".format(platform_name))
+    filename = os.path.join(sevObj.output_dir,
+                            "rsr_seviri_%s%d.h5" % (platform_id, sat_number))
 
-    sat_name = platform_name
+    sat_name = METEOSAT_SAT['%s%d' % (platform_id, sat_number)]
     with h5py.File(filename, "w") as h5f:
 
         h5f.attrs['description'] = 'Relative Spectral Responses for SEVIRI'
-        h5f.attrs['platform_name'] = platform_name
+        h5f.attrs['platform'] = platform_id
+        h5f.attrs['sat_number'] = sat_number
         bandlist = [str(key) for key in seviri.rsr.keys()]
         h5f.attrs['band_names'] = bandlist
 
         for key in seviri.rsr.keys():
             grp = h5f.create_group(key)
             if isinstance(seviri.central_wavelength[key][sat_name], dict):
-                grp.attrs['central_wavelength'] = \
-                    seviri.central_wavelength[key][sat_name]['95']
+                grp.attrs['central_wavelength'] = seviri.central_wavelength[
+                    key][sat_name]['95']
             else:
-                grp.attrs['central_wavelength'] = \
-                    seviri.central_wavelength[key][sat_name]
+                grp.attrs['central_wavelength'] = seviri.central_wavelength[
+                    key][sat_name]
             arr = seviri.rsr[key]['wavelength']
             dset = grp.create_dataset('wavelength', arr.shape, dtype='f')
             dset.attrs['unit'] = 'm'
             dset.attrs['scale'] = 1e-06
             dset[...] = arr
             try:
                 arr = seviri.rsr[key][sat_name]['95']
             except ValueError:
                 arr = seviri.rsr[key][sat_name]
             dset = grp.create_dataset('response', arr.shape, dtype='f')
             dset[...] = arr
 
     return
 
+if __name__ == "__main__":
+    sevObj = Seviri()
 
-def main():
-    """Main"""
-    sev_obj = Seviri()
-
+    import h5py
     for satnum in [8, 9, 10, 11]:
-        generate_seviri_file(sev_obj, 'Meteosat-{0:d}'.format(satnum))
-        print("Meteosat-{0:d} done...".format(satnum))
-
-
-if __name__ == "__main__":
-    main()
+        generate_seviri_file(sevObj, 'meteosat', satnum)
+        print "meteosat%d done..." % satnum
```

### Comparing `pyspectral-0.9.5/rsr_convert_scripts/modis_rsr.py` & `pyspectral-v0.1.0/pyspectral/modis_rsr.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,186 +1,206 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
-# Copyright (c) 2014-2019 Adam.Dybbroe
+# Copyright (c) 2014 Adam.Dybbroe
 
 # Author(s):
 
 #   Adam.Dybbroe <a000680@c14526.ad.smhi.se>
-#   Panu Lahtinen <panu.lahtinen@fmi.fi>
 
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Read the Terra/Aqua MODIS relative spectral response functions."""
+"""Read the Terra/Aqua MODIS relative spectral response functions.
+"""
 
+import logging
+LOG = logging.getLogger(__name__)
+
+import ConfigParser
 import os
 import numpy as np
-import logging
+
 from pyspectral.utils import sort_data
 from pyspectral.utils import get_central_wave
-from pyspectral.config import get_config
 
-LOG = logging.getLogger(__name__)
+try:
+    CONFIG_FILE = os.environ['PSP_CONFIG_FILE']
+except KeyError:
+    LOG.exception('Environment variable PSP_CONFIG_FILE not set!')
+    raise
+
+if not os.path.exists(CONFIG_FILE) or not os.path.isfile(CONFIG_FILE):
+    raise IOError(str(CONFIG_FILE) + " pointed to by the environment " +
+                  "variable PSP_CONFIG_FILE is not a file or does not exist!")
 
 MODIS_BAND_NAMES = [str(i) for i in range(1, 37)]
-SHORTWAVE_BANDS = [str(i) for i in list(range(1, 20)) + [26]]
+SATELLITE_NAME = {'terra': 'eos1', 'aqua': 'eos2'}
+PLATFORM_NAME = {'terra': 'eos', 'aqua': 'eos'}
+SATELLITE_NUMBER = {'terra': 1, 'aqua': 2}
+SHORTWAVE_BANDS = [str(i) for i in range(1, 20) + [26]]
 
 
 class ModisRSR(object):
 
     """Container for the Terra/Aqua RSR data"""
 
-    def __init__(self, bandname, platform_name, sort=True):
-        """Init Modis RSR
+    def __init__(self, bandname, satname, sort=True):
+        """
         """
-        self.platform_name = platform_name
+        self.satname = satname
         self.bandname = bandname
         self.filenames = {}
         self.requested_band_filename = None
         self.is_sw = False
         if bandname in SHORTWAVE_BANDS:
             self.is_sw = True
         self.scales = {}
         for bname in MODIS_BAND_NAMES:
             self.filenames[bname] = None
 
         self.rsr = None
         self._sort = sort
+        conf = ConfigParser.ConfigParser()
+        try:
+            conf.read(CONFIG_FILE)
+        except ConfigParser.NoSectionError:
+            LOG.exception(
+                'Failed reading configuration file: ' + str(CONFIG_FILE))
+            raise
+
+        options = {}
+        for option, value in conf.items(self.satname + '-modis', raw=True):
+            options[option] = value
+
+        for option, value in conf.items('general', raw=True):
+            options[option] = value
 
-        options = get_config()
-        self.path = options[platform_name + '-modis'].get('path')
         self.output_dir = options.get('rsr_dir', './')
 
-        self._get_bandfilenames()
-        LOG.debug("Filenames: %s", str(self.filenames))
+        self._get_bandfilenames(**options)
+        LOG.debug("Filenames: " + str(self.filenames))
         if os.path.exists(self.filenames[bandname]):
             self.requested_band_filename = self.filenames[bandname]
             self._load()
         else:
             raise IOError("Couldn't find an existing file for this band: " +
                           str(self.bandname))
 
-    def _get_bandfilenames(self):
+    def _get_bandfilenames(self, **options):
         """Get the MODIS rsr filenames"""
-        path = self.path
+
+        path = options["path"]
 
         for band in MODIS_BAND_NAMES:
             bnum = int(band)
-            LOG.debug("Band = %s", str(band))
-            if self.platform_name == 'EOS-Terra':
+            LOG.debug("Band= " + str(band))
+            if self.satname == 'terra':
                 filename = os.path.join(path,
-                                        "rsr.{0:d}.inb.final".format(bnum))
+                                        "rsr.%d.oobd.det" % (bnum))
             else:
-                if bnum in [5, 6, 7] + list(range(20, 37)):
-                    filename = os.path.join(
-                        path, "{0:>02d}.tv.1pct.det".format(bnum))
+                if bnum in [5, 6, 7] + range(20, 37):
+                    filename = os.path.join(path, "%.2d.tv.1pct.det" % (bnum))
                 else:
-                    filename = os.path.join(
-                        path, "{0:>02d}.amb.1pct.det".format(bnum))
+                    filename = os.path.join(path, "%.2d.amb.1pct.det" % (bnum))
 
             self.filenames[band] = filename
 
     def _load(self):
-        """Load the MODIS RSR data for the band requested"""
-        if self.is_sw or self.platform_name == 'EOS-Aqua':
+        """Load the MODIS RSR data for the band requested
+        """
+
+        if self.is_sw or self.satname == 'aqua':
             scale = 0.001
         else:
             scale = 1.0
         detector = read_modis_response(self.requested_band_filename, scale)
         self.rsr = detector
         if self._sort:
             self.sort()
 
     def sort(self):
         """Sort the data so that x is monotonically increasing and contains
-        no duplicates.
-        """
+        no duplicates."""
         if 'wavelength' in self.rsr:
             # Only one detector apparently:
             self.rsr['wavelength'], self.rsr['response'] = \
                 sort_data(self.rsr['wavelength'], self.rsr['response'])
         else:
             for detector_name in self.rsr:
-                (self.rsr[detector_name]['wavelength'],
-                 self.rsr[detector_name]['response']) = \
-                    sort_data(self.rsr[detector_name]['wavelength'],
-                              self.rsr[detector_name]['response'])
+                self.rsr[detector_name]['wavelength'], self.rsr[detector_name]['response'] = \
+                    sort_data(
+                        self.rsr[detector_name]['wavelength'], self.rsr[detector_name]['response'])
 
 
 def read_modis_response(filename, scale=1.0):
     """Read the Terra/Aqua MODIS relative spectral responses. Be aware that
     MODIS has several detectors (more than one) compared to e.g. AVHRR which
     has always only one.
     """
-    with open(filename, "r") as fid:
-        lines = fid.readlines()
+    fd = open(filename, "r")
+    lines = fd.readlines()
+    fd.close()
 
-    nodata = -99.0
     # The IR channels seem to be in microns, whereas the short wave channels are
     # in nanometers! For VIS/NIR scale should be 0.001
     detectors = {}
     for line in lines:
         if line.find("#") == 0:
             continue
-        dummy, det_num, s_1, s_2 = line.split()
-        detector_name = 'det-{0:d}'.format(int(det_num))
+        dummy1, dummy2, s1, s2 = line.split()
+        detector_name = 'det-%d' % int(dummy2)
         if detector_name not in detectors:
             detectors[detector_name] = {'wavelength': [], 'response': []}
 
-        detectors[detector_name]['wavelength'].append(float(s_1) * scale)
-        detectors[detector_name]['response'].append(float(s_2))
+        detectors[detector_name]['wavelength'].append(float(s1) * scale)
+        detectors[detector_name]['response'].append(float(s2))
 
     for key in detectors:
-        mask = np.array(detectors[key]['response']) == nodata
-        detectors[key]['response'] = np.ma.masked_array(
-            detectors[key]['response'], mask=mask).compressed()
-        detectors[key]['wavelength'] = np.ma.masked_array(
-            detectors[key]['wavelength'], mask=mask).compressed()
+        detectors[key]['wavelength'] = np.array(detectors[key]['wavelength'])
+        detectors[key]['response'] = np.array(detectors[key]['response'])
 
     return detectors
 
 
-def convert2hdf5(platform_name):
+def convert2hdf5(platform):
     """Retrieve original RSR data and convert to internal hdf5 format"""
     import h5py
 
-    modis = ModisRSR('20', platform_name)
+    modis = ModisRSR('20', platform)
     mfile = os.path.join(modis.output_dir,
-                         "rsr_modis_{platform}.h5".format(platform=platform_name))
+                         "rsr_modis_%s.h5" % SATELLITE_NAME.get(platform, platform))
 
     with h5py.File(mfile, "w") as h5f:
         h5f.attrs['description'] = 'Relative Spectral Responses for MODIS'
-        h5f.attrs['platform_name'] = platform_name
+        h5f.attrs['platform'] = PLATFORM_NAME.get(platform, platform)
+        h5f.attrs['sat_number'] = SATELLITE_NUMBER.get(platform, 'unknown')
         h5f.attrs['band_names'] = MODIS_BAND_NAMES
 
         for chname in MODIS_BAND_NAMES:
-            modis = ModisRSR(chname, platform_name)
+            modis = ModisRSR(chname, platform)
             grp = h5f.create_group(chname)
             grp.attrs['number_of_detectors'] = len(modis.rsr.keys())
             # Loop over each detector to check if the sampling wavelengths are
             # identical:
-            det_names = [detector_name for detector_name in modis.rsr.keys()]
+            det_names = modis.rsr.keys()
             wvl = modis.rsr[det_names[0]]['wavelength']
             wvl_is_constant = True
             for det in det_names[1:]:
-                if wvl.shape != modis.rsr[det]['wavelength'].shape:
-                    wvl_is_constant = False
-                    break
-                elif not np.allclose(wvl, modis.rsr[det]['wavelength']):
+                if not np.alltrue(wvl == modis.rsr[det]['wavelength']):
                     wvl_is_constant = False
                     break
 
             if wvl_is_constant:
                 arr = modis.rsr[det_names[0]]['wavelength']
                 dset = grp.create_dataset('wavelength', arr.shape, dtype='f')
                 dset.attrs['unit'] = 'm'
@@ -205,15 +225,11 @@
                     dset[...] = arr
 
                 arr = modis.rsr[det]['response']
                 dset = det_grp.create_dataset('response', arr.shape, dtype='f')
                 dset[...] = arr
 
 
-def main():
-    """Main"""
-    for sat in ['EOS-Terra', 'EOS-Aqua']:
-        convert2hdf5(sat)
-
-
 if __name__ == "__main__":
-    main()
+
+    for sat in ['terra', 'aqua']:
+        convert2hdf5(sat)
```

### Comparing `pyspectral-0.9.5/rsr_convert_scripts/viirs_rsr.py` & `pyspectral-v0.1.0/pyspectral/viirs_rsr.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,267 +1,248 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
-# Copyright (c) 2013-2018 Adam.Dybbroe
+# Copyright (c) 2013, 2014 Adam.Dybbroe
 
 # Author(s):
 
-#   Adam.Dybbroe <adam.dybbroe@smhi.se>
-#   Panu Lahtinen <panu.lahtinen@fmi.fi>
+#   Adam.Dybbroe <a000680@c14526.ad.smhi.se>
 
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Interface to VIIRS relative spectral responses"""
+"""Interface to VIIRS relative spectral responses
+"""
 
+import logging
+LOG = logging.getLogger(__name__)
+
+import ConfigParser
 import os
+
+try:
+    CONFIG_FILE = os.environ['PSP_CONFIG_FILE']
+except KeyError:
+    LOG.exception('Environment variable PSP_CONFIG_FILE not set!')
+    raise
+
+if not os.path.exists(CONFIG_FILE) or not os.path.isfile(CONFIG_FILE):
+    raise IOError(str(CONFIG_FILE) + " pointed to by the environment " +
+                  "variable PSP_CONFIG_FILE is not a file or does not exist!")
+
 import numpy as np
 from pyspectral.utils import get_central_wave
-from pyspectral.config import get_config
-from trollsift.parser import compose
-import logging
-LOG = logging.getLogger(__name__)
 
 VIIRS_BAND_NAMES = ['M1', 'M2', 'M3', 'M4', 'M5',
                     'M6', 'M7', 'M8', 'M9', 'M10',
                     'M11', 'M12', 'M13', 'M14', 'M15', 'M16',
                     'I1', 'I2', 'I3', 'I4', 'I5',
                     'DNB']
 
-N_HEADER_LINES = {'Suomi-NPP': 1, 'NOAA-20': 5}
-N_HEADER_LINES_DNB = {'Suomi-NPP': 1, 'NOAA-20': 6}
-
-# JPSS-1:  Band   det  SS      wvl_nm       RSR        SNR   SNR_Thresh QF
-# UAID/Swp
-NAMES1 = {'Suomi-NPP': ['bandname',
-                        'detector',
-                        'subsample',
-                        'wavelength',
-                        'band_avg_snr',
-                        'asr',
-                        'response',
-                        'quality_flag',
-                        'xtalk_flag'],
-          'NOAA-20': ['bandname',
-                      'detector',
-                      'subsample',
-                      'wavelength',
-                      'response',
-                      'snr',
-                      'snr_thresh',
-                      'qf',
-                      'uaid_swp']}
-
-DTYPE1 = {'Suomi-NPP': [('bandname', '|S3'),
-                        ('detector', '<i4'),
-                        ('subsample', '<i4'),
-                        ('wavelength', '<f8'),
-                        ('band_avg_snr', '<f8'),
-                        ('asr', '<f8'),
-                        ('response', '<f8'),
-                        ('quality_flag', '<i4'),
-                        ('xtalk_flag', '<i4')],
-          'NOAA-20': [('bandname', '|S3'),
-                      ('detector', '<i4'),
-                      ('subsample', '<i4'),
-                      ('wavelength', '<f8'),
-                      ('response', '<f8'),
-                      ('snr', '<f8'),
-                      ('snr_thresh', '<f8'),
-                      ('qf', '<i4'),
-                      ('uaid_swp', '<i4')]}
-
-
-NAMES2 = {'Suomi-NPP': ['bandname',
-                        'detector',
-                        'subsample',
-                        'wavelength',
-                        'response'],
-          'NOAA-20': []}
-
-DTYPE2 = {'Suomi-NPP': [('bandname', '|S3'),
-                        ('detector', '<i4'),
-                        ('subsample', '<i4'),
-                        ('wavelength', '<f8'),
-                        ('response', '<f8')],
-          'NOAA-20': []}
-
-
 #: Default time format
 _DEFAULT_TIME_FORMAT = '%Y-%m-%d %H:%M:%S'
 
 #: Default log format
 _DEFAULT_LOG_FORMAT = '[%(levelname)s: %(asctime)s : %(name)s] %(message)s'
 
 
 class ViirsRSR(object):
 
-    """Container for the (S-NPP/JPSS) VIIRS RSR data"""
+    """Container for the (S-NPP) VIIRS RSR data"""
 
-    def __init__(self, bandname, platform_name):
-        self.platform_name = platform_name
+    def __init__(self, bandname, satname='npp'):
+        """
+        """
+        self.satname = satname
         self.bandname = bandname
         self.filename = None
         self.rsr = None
 
-        options = get_config()
-        self.output_dir = options.get('rsr_dir', './')
+        conf = ConfigParser.ConfigParser()
+        try:
+            conf.read(CONFIG_FILE)
+        except ConfigParser.NoSectionError:
+            LOG.exception('Failed reading configuration file: ' +
+                          str(CONFIG_FILE))
+            raise
+
+        options = {}
+        for option, value in conf.items('viirs', raw=True):
+            options[option] = value
+
+        for option, value in conf.items('general', raw=True):
+            options[option] = value
 
-        self.bandfilenames = {}
+        self.output_dir = options.get('rsr_dir', './')
 
-        self._get_bandfilenames(**options)
         self._get_bandfile(**options)
-        LOG.debug("Filename: %s", str(self.filename))
+        LOG.debug("Filename: " + str(self.filename))
         self._load()
 
-    def _get_bandfilenames(self, **options):
-        """Get filename for each band"""
-        conf = options[self.platform_name + '-viirs']
-
-        rootdir = conf['rootdir']
-        for section in conf:
-            if not section.startswith('section'):
-                continue
-            bandnames = conf[section]['bands']
-            for band in bandnames:
-                filename = os.path.join(rootdir, conf[section]['filename'])
-                self.bandfilenames[band] = compose(
-                    filename, {'bandname': band})
-
     def _get_bandfile(self, **options):
         """Get the VIIRS rsr filename"""
 
+        band_file = None
+
         # Need to understand why there are A&B files for band M16. FIXME!
         # Anyway, the absolute response differences are small, below 0.05
+        if self.bandname == 'M16':
+            values = {"bandname": 'M16A'}
+        else:
+            values = {"bandname": self.bandname}
 
-        # LOG.debug("paths = %s", str(self.bandfilenames))
-
-        path = self.bandfilenames[self.bandname]
-        if not os.path.exists(path):
-            raise IOError("Couldn't find an existing file for this band ({band}): {path}".format(
-                band=self.bandname, path=path))
-
-        self.filename = path
-        return
+        paths = [options["iband_visnir_path"],
+                 options["iband_ir_path"],
+                 options["mband_visnir_path"],
+                 options["mband_ir_path"],
+                 options["dnb_path"]
+                 ]
+        fnames = [options["iband_visnir_names"] % values,
+                  options["iband_ir_names"] % values,
+                  options["mband_visnir_names"] % values,
+                  options["mband_ir_names"] % values,
+                  options["dnb_name"] % values
+                  ]
+
+        LOG.debug("paths = " + str(paths))
+        LOG.debug("fnames = " + str(fnames))
+
+        for path, fname in zip(paths, fnames):
+            band_file = os.path.join(path, fname)
+            if os.path.exists(band_file):
+                self.filename = band_file
+                return
+
+        if not band_file:
+            raise IOError("Couldn't find an existing file for this band: " +
+                          str(self.bandname))
 
     def _load(self, scale=0.001):
-        """Load the VIIRS RSR data for the band requested"""
-        if self.bandname == 'DNB':
-            header_lines_to_skip = N_HEADER_LINES_DNB[self.platform_name]
-        else:
-            header_lines_to_skip = N_HEADER_LINES[self.platform_name]
+        """Load the VIIRS RSR data for the band requested
+        """
+        import numpy as np
 
         try:
             data = np.genfromtxt(self.filename,
-                                 unpack=True, skip_header=header_lines_to_skip,
-                                 names=NAMES1[self.platform_name],
-                                 dtype=DTYPE1[self.platform_name])
+                                 unpack=True, skip_header=1,
+                                 names=['bandname',
+                                        'detector',
+                                        'subsample',
+                                        'wavelength',
+                                        'band_avg_snr',
+                                        'asr',
+                                        'response',
+                                        'quality_flag',
+                                        'xtalk_flag'],
+                                 dtype=[('bandname', '|S3'),
+                                        ('detector', '<i4'),
+                                        ('subsample', '<i4'),
+                                        ('wavelength', '<f8'),
+                                        ('band_avg_snr', '<f8'),
+                                        ('asr', '<f8'),
+                                        ('response', '<f8'),
+                                        ('quality_flag', '<i4'),
+                                        ('xtalk_flag', '<i4')])
         except ValueError:
             data = np.genfromtxt(self.filename,
-                                 unpack=True, skip_header=N_HEADER_LINES[
-                                     self.platform_name],
-                                 names=NAMES2[self.platform_name],
-                                 dtype=DTYPE2[self.platform_name])
-
+                                 unpack=True, skip_header=1,
+                                 names=['bandname',
+                                        'detector',
+                                        'subsample',
+                                        'wavelength',
+                                        'response'],
+                                 dtype=[('bandname', '|S3'),
+                                        ('detector', '<i4'),
+                                        ('subsample', '<i4'),
+                                        ('wavelength', '<f8'),
+                                        ('response', '<f8')])
         wavelength = data['wavelength'] * scale
         response = data['response']
         det = data['detector']
 
         detectors = {}
         for idx in range(int(max(det))):
-            detectors["det-{0:d}".format(idx + 1)] = {}
+            detectors["det-%d" % (idx + 1)] = {}
             detectors[
-                "det-{0:d}".format(idx + 1)]['wavelength'] = np.repeat(wavelength, np.equal(det, idx + 1))
+                "det-%d" % (idx + 1)]['wavelength'] = np.repeat(wavelength, np.equal(det, idx + 1))
             detectors[
-                "det-{0:d}".format(idx + 1)]['response'] = np.repeat(response, np.equal(det, idx + 1))
+                "det-%d" % (idx + 1)]['response'] = np.repeat(response, np.equal(det, idx + 1))
 
         self.rsr = detectors
 
 
-def main():
-    """Main"""
-    import sys
-    import h5py
+if __name__ == "__main__":
 
+    import sys
+    LOG = logging.getLogger('viirs_rsr')
     handler = logging.StreamHandler(sys.stderr)
 
     formatter = logging.Formatter(fmt=_DEFAULT_LOG_FORMAT,
                                   datefmt=_DEFAULT_TIME_FORMAT)
     handler.setFormatter(formatter)
     handler.setLevel(logging.DEBUG)
     LOG.setLevel(logging.DEBUG)
     LOG.addHandler(handler)
 
-    platform_name = "NOAA-20"
-    # platform_name = "Suomi-NPP"
-    viirs = ViirsRSR('M1', platform_name)
+    import h5py
+
+    platform_id = "npp"
+    viirs = ViirsRSR('M1', 'npp')
     filename = os.path.join(viirs.output_dir,
-                            "rsr_viirs_{0}.h5".format(platform_name))
+                            "rsr_viirs_%s.h5" % platform_id)
 
     with h5py.File(filename, "w") as h5f:
         h5f.attrs['description'] = 'Relative Spectral Responses for VIIRS'
-        h5f.attrs['platform_name'] = platform_name
-        h5f.attrs['sensor'] = 'viirs'
+        h5f.attrs['platform'] = platform_id
+        h5f.attrs['sat_number'] = np.nan
         h5f.attrs['band_names'] = VIIRS_BAND_NAMES
 
         for chname in VIIRS_BAND_NAMES:
-
-            viirs = ViirsRSR(chname, platform_name)
+            viirs = ViirsRSR(chname)
             grp = h5f.create_group(chname)
             grp.attrs['number_of_detectors'] = len(viirs.rsr.keys())
             # Loop over each detector to check if the sampling wavelengths are
             # identical:
             det_names = viirs.rsr.keys()
             wvl = viirs.rsr[det_names[0]]['wavelength']
-            wvl, idx = np.unique(wvl, return_index=True)
             wvl_is_constant = True
             for det in det_names[1:]:
-                det_wvl = np.unique(viirs.rsr[det]['wavelength'])
-                if not np.alltrue(wvl == det_wvl):
-                    LOG.warning(
-                        "Wavelngth arrays are not the same among detectors!")
+                if not np.alltrue(wvl == viirs.rsr[det_names[0]]['wavelength']):
                     wvl_is_constant = False
 
             if wvl_is_constant:
-                arr = wvl
+                arr = viirs.rsr[det_names[0]]['wavelength']
                 dset = grp.create_dataset('wavelength', arr.shape, dtype='f')
                 dset.attrs['unit'] = 'm'
                 dset.attrs['scale'] = 1e-06
                 dset[...] = arr
 
             # Loop over each detector:
             for det in viirs.rsr:
                 det_grp = grp.create_group(det)
                 wvl = viirs.rsr[det]['wavelength'][
                     ~np.isnan(viirs.rsr[det]['wavelength'])]
                 rsp = viirs.rsr[det]['response'][
                     ~np.isnan(viirs.rsr[det]['wavelength'])]
-                wvl, idx = np.unique(wvl, return_index=True)
-                rsp = np.take(rsp, idx)
-                LOG.debug("wvl.shape: %s", str(wvl.shape))
                 det_grp.attrs[
                     'central_wavelength'] = get_central_wave(wvl, rsp)
                 if not wvl_is_constant:
-                    arr = wvl
+                    arr = viirs.rsr[det]['wavelength']
                     dset = det_grp.create_dataset(
                         'wavelength', arr.shape, dtype='f')
                     dset.attrs['unit'] = 'm'
                     dset.attrs['scale'] = 1e-06
                     dset[...] = arr
 
-                dset = det_grp.create_dataset('response', rsp.shape, dtype='f')
-                dset[...] = rsp
-
-
-if __name__ == "__main__":
-    LOG = logging.getLogger('viirs_rsr')
-    main()
+                arr = viirs.rsr[det]['response']
+                dset = det_grp.create_dataset('response', arr.shape, dtype='f')
+                dset[...] = arr
```

