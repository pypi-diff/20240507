# Comparing `tmp/exchange_calendars-4.5.3.tar.gz` & `tmp/exchange_calendars-4.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exchange_calendars-4.5.3.tar", last modified: Thu Feb 15 17:42:08 2024, max compression
+gzip compressed data, was "exchange_calendars-4.5.4.tar", last modified: Tue May  7 14:26:00 2024, max compression
```

## Comparing `exchange_calendars-4.5.3.tar` & `exchange_calendars-4.5.4.tar`

### file list

```diff
@@ -1,238 +1,238 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 17:42:08.647751 exchange_calendars-4.5.3/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/.gitattributes
--rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    11347 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    37202 2024-02-15 17:42:08.647751 exchange_calendars-4.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    22633 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 17:42:08.579752 exchange_calendars-4.5.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/docs/changes_archive.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 17:42:08.579752 exchange_calendars-4.5.3/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)    90326 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/docs/tutorials/calendar_methods.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    37097 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/docs/tutorials/calendar_properties.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    29917 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/docs/tutorials/minutes.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    22137 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/docs/tutorials/sessions.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   149704 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/docs/tutorials/trading_index.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 17:42:08.583752 exchange_calendars-4.5.3/etc/
--rw-r--r--   0 runner    (1001) docker     (127)   141885 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/etc/NYSE-Historical-Closings.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/etc/bench.py
--rw-r--r--   0 runner    (1001) docker     (127)     5835 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/etc/check_holidays.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3711 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/etc/ecal
--rw-r--r--   0 runner    (1001) docker     (127)    12890 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/etc/factory_bounds.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    50220 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/etc/lunisolar
--rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/etc/make_exchange_calendar_test_csv.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/etc/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/etc/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/etc/requirements_lunisolar.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/etc/requirements_minpandas.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/etc/requirements_update_xkrx_holidays.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4397 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/etc/update_xkrx_holidays.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 17:42:08.591752 exchange_calendars-4.5.3/exchange_calendars/
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/exchange_calendars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-02-15 17:42:08.000000 exchange_calendars-4.5.3/exchange_calendars/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/exchange_calendars/always_open.py
--rw-r--r--   0 runner    (1001) docker     (127)    24842 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/exchange_calendars/calendar_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    20211 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/exchange_calendars/calendar_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10626 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/exchange_calendars/common_holidays.py
--rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/exchange_calendars/ecal.py
--rw-r--r--   0 runner    (1001) docker     (127)    10859 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/exchange_calendars/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)   105255 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/exchange_calendars/exchange_calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)     5977 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_aixk.py
--rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_asex.py
--rw-r--r--   0 runner    (1001) docker     (127)     5610 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_bvmf.py
--rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_cmes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_iepa.py
--rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xams.py
--rw-r--r--   0 runner    (1001) docker     (127)     6946 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xasx.py
--rw-r--r--   0 runner    (1001) docker     (127)     3391 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xbkk.py
--rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xbog.py
--rw-r--r--   0 runner    (1001) docker     (127)    10385 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xbom.py
--rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xbru.py
--rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xbse.py
--rw-r--r--   0 runner    (1001) docker     (127)     5962 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xbud.py
--rw-r--r--   0 runner    (1001) docker     (127)     9063 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xbue.py
--rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xcbf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xcse.py
--rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xdub.py
--rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xetr.py
--rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xfra.py
--rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xhel.py
--rw-r--r--   0 runner    (1001) docker     (127)    16783 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xhkg.py
--rw-r--r--   0 runner    (1001) docker     (127)     2904 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xice.py
--rw-r--r--   0 runner    (1001) docker     (127)    12605 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xidx.py
--rw-r--r--   0 runner    (1001) docker     (127)     5351 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xist.py
--rw-r--r--   0 runner    (1001) docker     (127)     5170 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xjse.py
--rw-r--r--   0 runner    (1001) docker     (127)    11007 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xkar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xkls.py
--rw-r--r--   0 runner    (1001) docker     (127)    13216 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xkrx.py
--rw-r--r--   0 runner    (1001) docker     (127)     3682 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xlim.py
--rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xlis.py
--rw-r--r--   0 runner    (1001) docker     (127)     7304 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xlon.py
--rw-r--r--   0 runner    (1001) docker     (127)     4134 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xmad.py
--rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xmex.py
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xmil.py
--rw-r--r--   0 runner    (1001) docker     (127)     7955 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xmos.py
--rw-r--r--   0 runner    (1001) docker     (127)     9349 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xnys.py
--rw-r--r--   0 runner    (1001) docker     (127)     6927 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xnze.py
--rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xosl.py
--rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xpar.py
--rw-r--r--   0 runner    (1001) docker     (127)    10772 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xphs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xpra.py
--rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xsau.py
--rw-r--r--   0 runner    (1001) docker     (127)    10693 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xses.py
--rw-r--r--   0 runner    (1001) docker     (127)     7496 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xsgo.py
--rw-r--r--   0 runner    (1001) docker     (127)    14023 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xshg.py
--rw-r--r--   0 runner    (1001) docker     (127)     3918 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xsto.py
--rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xswx.py
--rw-r--r--   0 runner    (1001) docker     (127)     4682 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xtae.py
--rw-r--r--   0 runner    (1001) docker     (127)    10203 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xtai.py
--rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xtks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xtse.py
--rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xwar.py
--rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xwbo.py
--rw-r--r--   0 runner    (1001) docker     (127)    13602 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/exchange_calendars/lunisolar_holidays.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 17:42:08.595752 exchange_calendars-4.5.3/exchange_calendars/pandas_extensions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/exchange_calendars/pandas_extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6316 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/exchange_calendars/pandas_extensions/holiday.py
--rw-r--r--   0 runner    (1001) docker     (127)     7810 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/exchange_calendars/pandas_extensions/korean_holiday.py
--rw-r--r--   0 runner    (1001) docker     (127)    10124 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/exchange_calendars/pandas_extensions/offsets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/exchange_calendars/precomputed_exchange_calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)    11751 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/exchange_calendars/tase_holidays.py
--rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/exchange_calendars/us_futures_calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)    10119 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/exchange_calendars/us_holidays.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 17:42:08.595752 exchange_calendars-4.5.3/exchange_calendars/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/exchange_calendars/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4756 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/exchange_calendars/utils/pandas_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/exchange_calendars/weekday_calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)     7748 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/exchange_calendars/xbkk_holidays.py
--rw-r--r--   0 runner    (1001) docker     (127)    12755 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/exchange_calendars/xkls_holidays.py
--rw-r--r--   0 runner    (1001) docker     (127)    35197 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/exchange_calendars/xkrx_holidays.py
--rw-r--r--   0 runner    (1001) docker     (127)     9305 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/exchange_calendars/xtks_holidays.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 17:42:08.647751 exchange_calendars-4.5.3/exchange_calendars.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    37202 2024-02-15 17:42:08.000000 exchange_calendars-4.5.3/exchange_calendars.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7318 2024-02-15 17:42:08.000000 exchange_calendars-4.5.3/exchange_calendars.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-15 17:42:08.000000 exchange_calendars-4.5.3/exchange_calendars.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-15 17:42:08.000000 exchange_calendars-4.5.3/exchange_calendars.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-02-15 17:42:08.000000 exchange_calendars-4.5.3/exchange_calendars.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-02-15 17:42:08.000000 exchange_calendars-4.5.3/exchange_calendars.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-02-15 17:42:08.647751 exchange_calendars-4.5.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 17:42:08.603752 exchange_calendars-4.5.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 17:42:08.643751 exchange_calendars-4.5.3/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (127)    16999 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/resources/24-5.csv
--rw-r--r--   0 runner    (1001) docker     (127)    23824 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/resources/24-7.csv
--rw-r--r--   0 runner    (1001) docker     (127)   110144 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/resources/aixk.csv
--rw-r--r--   0 runner    (1001) docker     (127)   496439 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/resources/asex.csv
--rw-r--r--   0 runner    (1001) docker     (127)   537779 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/resources/bvmf.csv
--rw-r--r--   0 runner    (1001) docker     (127)   461924 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/resources/cmes.csv
--rw-r--r--   0 runner    (1001) docker     (127)   461924 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/resources/iepa.csv
--rw-r--r--   0 runner    (1001) docker     (127)   114134 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/resources/test.csv
--rw-r--r--   0 runner    (1001) docker     (127)   492279 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/resources/xams.csv
--rw-r--r--   0 runner    (1001) docker     (127)   577884 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/resources/xasx.csv
--rw-r--r--   0 runner    (1001) docker     (127)   494164 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/resources/xbkk.csv
--rw-r--r--   0 runner    (1001) docker     (127)   486819 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/resources/xbog.csv
--rw-r--r--   0 runner    (1001) docker     (127)   450159 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/resources/xbom.csv
--rw-r--r--   0 runner    (1001) docker     (127)   492344 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/resources/xbru.csv
--rw-r--r--   0 runner    (1001) docker     (127)   560724 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/resources/xbse.csv
--rw-r--r--   0 runner    (1001) docker     (127)   499559 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/resources/xbud.csv
--rw-r--r--   0 runner    (1001) docker     (127)   498389 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/resources/xbue.csv
--rw-r--r--   0 runner    (1001) docker     (127)   547139 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/resources/xcbf.csv
--rw-r--r--   0 runner    (1001) docker     (127)   571384 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/resources/xcse.csv
--rw-r--r--   0 runner    (1001) docker     (127)   507099 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/resources/xdub.csv
--rw-r--r--   0 runner    (1001) docker     (127)   552404 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/resources/xetr.csv
--rw-r--r--   0 runner    (1001) docker     (127)   551104 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/resources/xfra.csv
--rw-r--r--   0 runner    (1001) docker     (127)   486559 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/resources/xhel.csv
--rw-r--r--   0 runner    (1001) docker     (127)   904219 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/resources/xhkg.csv
--rw-r--r--   0 runner    (1001) docker     (127)   145764 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/resources/xice.csv
--rw-r--r--   0 runner    (1001) docker     (127)   500014 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/resources/xidx.csv
--rw-r--r--   0 runner    (1001) docker     (127)   502614 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/resources/xist.csv
--rw-r--r--   0 runner    (1001) docker     (127)   499819 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/resources/xjse.csv
--rw-r--r--   0 runner    (1001) docker     (127)   504889 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/resources/xkar.csv
--rw-r--r--   0 runner    (1001) docker     (127)   499299 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/resources/xkls.csv
--rw-r--r--   0 runner    (1001) docker     (127)   826564 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/resources/xkrx.csv
--rw-r--r--   0 runner    (1001) docker     (127)   501444 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/resources/xlim.csv
--rw-r--r--   0 runner    (1001) docker     (127)   488119 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/resources/xlis.csv
--rw-r--r--   0 runner    (1001) docker     (127)   553509 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/resources/xlon.csv
--rw-r--r--   0 runner    (1001) docker     (127)   541224 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/resources/xmad.csv
--rw-r--r--   0 runner    (1001) docker     (127)   503979 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/resources/xmex.csv
--rw-r--r--   0 runner    (1001) docker     (127)   490784 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/resources/xmil.csv
--rw-r--r--   0 runner    (1001) docker     (127)   569434 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/resources/xmos.csv
--rw-r--r--   0 runner    (1001) docker     (127)   541094 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/resources/xnys.csv
--rw-r--r--   0 runner    (1001) docker     (127)   550909 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/resources/xnze.csv
--rw-r--r--   0 runner    (1001) docker     (127)   486299 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/resources/xosl.csv
--rw-r--r--   0 runner    (1001) docker     (127)   493059 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/resources/xpar.csv
--rw-r--r--   0 runner    (1001) docker     (127)   504694 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/resources/xphs.csv
--rw-r--r--   0 runner    (1001) docker     (127)   501184 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/resources/xpra.csv
--rw-r--r--   0 runner    (1001) docker     (127)    48654 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/resources/xsau.csv
--rw-r--r--   0 runner    (1001) docker     (127)   635344 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/resources/xses.csv
--rw-r--r--   0 runner    (1001) docker     (127)   498714 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/resources/xsgo.csv
--rw-r--r--   0 runner    (1001) docker     (127)   876784 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/resources/xshg.csv
--rw-r--r--   0 runner    (1001) docker     (127)   486494 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/resources/xsto.csv
--rw-r--r--   0 runner    (1001) docker     (127)   485129 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/resources/xswx.csv
--rw-r--r--   0 runner    (1001) docker     (127)    79204 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/resources/xtae.csv
--rw-r--r--   0 runner    (1001) docker     (127)   548374 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/resources/xtai.csv
--rw-r--r--   0 runner    (1001) docker     (127)   643474 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/resources/xtks.csv
--rw-r--r--   0 runner    (1001) docker     (127)   486494 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/resources/xtse.csv
--rw-r--r--   0 runner    (1001) docker     (127)   500989 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/resources/xwar.csv
--rw-r--r--   0 runner    (1001) docker     (127)   555134 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/resources/xwbo.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/test_aixk_calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/test_always_open.py
--rw-r--r--   0 runner    (1001) docker     (127)     5105 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/test_asex_calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/test_bvmf_calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)     5974 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/test_calendar_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (127)    70029 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/test_calendar_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/test_cmes_calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)   162607 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/test_exchange_calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/test_iepa_calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/test_weekday_calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/test_xams_calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/test_xasx_calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3729 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/test_xbkk_calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/test_xbog_calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/test_xbom_calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/test_xbru_calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/test_xbse_calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)     4823 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/test_xbud_calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3701 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/test_xbue_calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/test_xcbf_calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/test_xcse_calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/test_xdub_calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/test_xetr_calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/test_xfra_calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/test_xhel_calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)     9143 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/test_xhkg_calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/test_xice_calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)     4735 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/test_xidx_calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3657 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/test_xist_calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/test_xjse_calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/test_xkar_calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/test_xkls_calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)     4868 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/test_xkrx_calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/test_xlim_calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/test_xlis_calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/test_xlon_calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/test_xmad_calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)     4444 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/test_xmex_calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/test_xmil_calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/test_xmos_calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3701 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/test_xnys_calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3576 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/test_xnze_calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/test_xosl_calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/test_xpar_calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/test_xphs_calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/test_xpra_calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/test_xsau_calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/test_xses_calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)     8524 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/test_xsgo_calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/test_xshg_calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/test_xsto_calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/test_xswx_calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/test_xtae_calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/test_xtai_calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)    13389 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/test_xtks_calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/test_xtse_calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3334 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/test_xwar_calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-02-15 17:41:59.000000 exchange_calendars-4.5.3/tests/test_xwbo_calendar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:26:00.466529 exchange_calendars-4.5.4/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/.gitattributes
+-rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    11347 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    37202 2024-05-07 14:26:00.466529 exchange_calendars-4.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    22633 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:26:00.398529 exchange_calendars-4.5.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/docs/changes_archive.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:26:00.398529 exchange_calendars-4.5.4/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)    90326 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/docs/tutorials/calendar_methods.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    37097 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/docs/tutorials/calendar_properties.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    29917 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/docs/tutorials/minutes.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    22137 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/docs/tutorials/sessions.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   149704 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/docs/tutorials/trading_index.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:26:00.398529 exchange_calendars-4.5.4/etc/
+-rw-r--r--   0 runner    (1001) docker     (127)   141885 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/etc/NYSE-Historical-Closings.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/etc/bench.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5835 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/etc/check_holidays.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3711 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/etc/ecal
+-rw-r--r--   0 runner    (1001) docker     (127)    12890 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/etc/factory_bounds.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    50220 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/etc/lunisolar
+-rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/etc/make_exchange_calendar_test_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/etc/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/etc/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/etc/requirements_lunisolar.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/etc/requirements_minpandas.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/etc/requirements_update_xkrx_holidays.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4397 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/etc/update_xkrx_holidays.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:26:00.410529 exchange_calendars-4.5.4/exchange_calendars/
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/exchange_calendars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-07 14:26:00.000000 exchange_calendars-4.5.4/exchange_calendars/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/exchange_calendars/always_open.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24842 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/exchange_calendars/calendar_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20211 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/exchange_calendars/calendar_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10626 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/exchange_calendars/common_holidays.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/exchange_calendars/ecal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10859 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/exchange_calendars/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)   105255 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/exchange_calendars/exchange_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5977 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_aixk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_asex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5862 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_bvmf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_cmes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_iepa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xams.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6946 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xasx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3391 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xbkk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xbog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10385 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xbom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xbru.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xbse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5962 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xbud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9063 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xbue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xcbf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xcse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4353 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xdub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xetr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xfra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xhel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16783 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xhkg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2904 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xice.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12605 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xidx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5351 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5170 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xjse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11007 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xkar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xkls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13216 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xkrx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3682 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xlim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xlis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7304 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xlon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4134 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xmad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xmex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xmil.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12501 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xmos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9349 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xnys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6927 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xnze.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xosl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xpar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10772 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xphs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xpra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xsau.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10693 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7496 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xsgo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14023 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xshg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3918 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xsto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xswx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4682 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xtae.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10203 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xtai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xtks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xtse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xwar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xwbo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13602 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/exchange_calendars/lunisolar_holidays.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:26:00.414529 exchange_calendars-4.5.4/exchange_calendars/pandas_extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/exchange_calendars/pandas_extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6316 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/exchange_calendars/pandas_extensions/holiday.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7810 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/exchange_calendars/pandas_extensions/korean_holiday.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10188 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/exchange_calendars/pandas_extensions/offsets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/exchange_calendars/precomputed_exchange_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11751 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/exchange_calendars/tase_holidays.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/exchange_calendars/us_futures_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10119 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/exchange_calendars/us_holidays.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:26:00.414529 exchange_calendars-4.5.4/exchange_calendars/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/exchange_calendars/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4756 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/exchange_calendars/utils/pandas_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/exchange_calendars/weekday_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7748 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/exchange_calendars/xbkk_holidays.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12755 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/exchange_calendars/xkls_holidays.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35249 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/exchange_calendars/xkrx_holidays.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9305 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/exchange_calendars/xtks_holidays.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:26:00.462529 exchange_calendars-4.5.4/exchange_calendars.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    37202 2024-05-07 14:26:00.000000 exchange_calendars-4.5.4/exchange_calendars.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7318 2024-05-07 14:26:00.000000 exchange_calendars-4.5.4/exchange_calendars.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 14:26:00.000000 exchange_calendars-4.5.4/exchange_calendars.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-07 14:26:00.000000 exchange_calendars-4.5.4/exchange_calendars.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-07 14:26:00.000000 exchange_calendars-4.5.4/exchange_calendars.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-07 14:26:00.000000 exchange_calendars-4.5.4/exchange_calendars.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-07 14:26:00.466529 exchange_calendars-4.5.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:26:00.422529 exchange_calendars-4.5.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:26:00.462529 exchange_calendars-4.5.4/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)    16999 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/resources/24-5.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    23824 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/resources/24-7.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   110144 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/resources/aixk.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   496439 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/resources/asex.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   537779 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/resources/bvmf.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   461924 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/resources/cmes.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   461924 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/resources/iepa.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   114134 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/resources/test.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   492279 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/resources/xams.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   577884 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/resources/xasx.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   494164 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/resources/xbkk.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   486819 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/resources/xbog.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   450159 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/resources/xbom.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   492344 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/resources/xbru.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   560724 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/resources/xbse.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   499559 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/resources/xbud.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   498389 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/resources/xbue.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   547139 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/resources/xcbf.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   571384 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/resources/xcse.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   507099 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/resources/xdub.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   552404 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/resources/xetr.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   551104 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/resources/xfra.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   486559 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/resources/xhel.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   904219 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/resources/xhkg.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   145764 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/resources/xice.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   500014 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/resources/xidx.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   502614 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/resources/xist.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   499819 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/resources/xjse.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   504889 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/resources/xkar.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   499299 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/resources/xkls.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   832479 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/resources/xkrx.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   501444 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/resources/xlim.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   488119 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/resources/xlis.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   553509 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/resources/xlon.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   541224 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/resources/xmad.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   503979 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/resources/xmex.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   490784 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/resources/xmil.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   572034 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/resources/xmos.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   541094 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/resources/xnys.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   550909 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/resources/xnze.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   486299 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/resources/xosl.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   493059 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/resources/xpar.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   504694 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/resources/xphs.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   501184 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/resources/xpra.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    48654 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/resources/xsau.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   635344 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/resources/xses.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   498714 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/resources/xsgo.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   876784 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/resources/xshg.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   486494 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/resources/xsto.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   485129 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/resources/xswx.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    79204 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/resources/xtae.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   548374 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/resources/xtai.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   643474 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/resources/xtks.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   486494 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/resources/xtse.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   500989 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/resources/xwar.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   555134 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/resources/xwbo.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/test_aixk_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/test_always_open.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5105 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/test_asex_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/test_bvmf_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5974 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/test_calendar_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70029 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/test_calendar_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/test_cmes_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)   162688 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/test_exchange_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/test_iepa_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/test_weekday_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/test_xams_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/test_xasx_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3729 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/test_xbkk_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/test_xbog_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/test_xbom_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/test_xbru_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/test_xbse_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4823 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/test_xbud_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3701 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/test_xbue_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/test_xcbf_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/test_xcse_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/test_xdub_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/test_xetr_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/test_xfra_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/test_xhel_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9143 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/test_xhkg_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/test_xice_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4735 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/test_xidx_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3657 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/test_xist_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/test_xjse_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/test_xkar_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/test_xkls_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4868 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/test_xkrx_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/test_xlim_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/test_xlis_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/test_xlon_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/test_xmad_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4444 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/test_xmex_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/test_xmil_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/test_xmos_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3701 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/test_xnys_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3576 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/test_xnze_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/test_xosl_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/test_xpar_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/test_xphs_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/test_xpra_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/test_xsau_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/test_xses_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8524 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/test_xsgo_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/test_xshg_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/test_xsto_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/test_xswx_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/test_xtae_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/test_xtai_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13389 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/test_xtks_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/test_xtse_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3334 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/test_xwar_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-05-07 14:25:55.000000 exchange_calendars-4.5.4/tests/test_xwbo_calendar.py
```

### Comparing `exchange_calendars-4.5.3/.gitignore` & `exchange_calendars-4.5.4/.gitignore`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/LICENSE` & `exchange_calendars-4.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/PKG-INFO` & `exchange_calendars-4.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exchange_calendars
-Version: 4.5.3
+Version: 4.5.4
 Summary: Calendars for securities exchanges
 Author: Gerry Manoim
 Author-email: gerrymanoim@gmail.com
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `exchange_calendars-4.5.3/README.md` & `exchange_calendars-4.5.4/README.md`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/docs/changes_archive.md` & `exchange_calendars-4.5.4/docs/changes_archive.md`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/docs/tutorials/calendar_methods.ipynb` & `exchange_calendars-4.5.4/docs/tutorials/calendar_methods.ipynb`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/docs/tutorials/calendar_properties.ipynb` & `exchange_calendars-4.5.4/docs/tutorials/calendar_properties.ipynb`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/docs/tutorials/minutes.ipynb` & `exchange_calendars-4.5.4/docs/tutorials/minutes.ipynb`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/docs/tutorials/sessions.ipynb` & `exchange_calendars-4.5.4/docs/tutorials/sessions.ipynb`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/docs/tutorials/trading_index.ipynb` & `exchange_calendars-4.5.4/docs/tutorials/trading_index.ipynb`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/etc/NYSE-Historical-Closings.pdf` & `exchange_calendars-4.5.4/etc/NYSE-Historical-Closings.pdf`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/etc/bench.py` & `exchange_calendars-4.5.4/etc/bench.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/etc/check_holidays.py` & `exchange_calendars-4.5.4/etc/check_holidays.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/etc/ecal` & `exchange_calendars-4.5.4/etc/ecal`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/etc/factory_bounds.py` & `exchange_calendars-4.5.4/etc/factory_bounds.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/etc/lunisolar` & `exchange_calendars-4.5.4/etc/lunisolar`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/etc/make_exchange_calendar_test_csv.py` & `exchange_calendars-4.5.4/etc/make_exchange_calendar_test_csv.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/etc/requirements.txt` & `exchange_calendars-4.5.4/etc/requirements.txt`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/etc/requirements_dev.txt` & `exchange_calendars-4.5.4/etc/requirements_dev.txt`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/etc/requirements_minpandas.txt` & `exchange_calendars-4.5.4/etc/requirements_minpandas.txt`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/etc/update_xkrx_holidays.py` & `exchange_calendars-4.5.4/etc/update_xkrx_holidays.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/exchange_calendars/__init__.py` & `exchange_calendars-4.5.4/exchange_calendars/__init__.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/exchange_calendars/calendar_helpers.py` & `exchange_calendars-4.5.4/exchange_calendars/calendar_helpers.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/exchange_calendars/calendar_utils.py` & `exchange_calendars-4.5.4/exchange_calendars/calendar_utils.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/exchange_calendars/common_holidays.py` & `exchange_calendars-4.5.4/exchange_calendars/common_holidays.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/exchange_calendars/ecal.py` & `exchange_calendars-4.5.4/exchange_calendars/ecal.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/exchange_calendars/errors.py` & `exchange_calendars-4.5.4/exchange_calendars/errors.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/exchange_calendars/exchange_calendar.py` & `exchange_calendars-4.5.4/exchange_calendars/exchange_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_aixk.py` & `exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_aixk.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_asex.py` & `exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_asex.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_bvmf.py` & `exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_bvmf.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,14 +115,21 @@
 ConscienciaNegra = Holiday(
     "Dia da Consciencia Negra",
     month=11,
     day=20,
     start_date="2004-01-01",
     end_date="2022-01-01",
 )
+# Day of Black Awareness is now a national holiday, starting 2024
+ConscienciaNegraNacional = Holiday(
+    "Dia Nacional de Zumbi e da Consciencia Negra",
+    month=11,
+    day=20,
+    start_date="2024-01-01"
+)
 # Christmas Eve
 VesperaNatal = Holiday(
     "Vespera Natal",
     month=12,
     day=24,
 )
 # Christmas
@@ -205,14 +212,15 @@
                 Constitucionalista_prepandemic,
                 Constitucionalista_pospandemic,
                 Independencia,
                 Aparecida,
                 Finados,
                 ProclamacaoRepublica,
                 ConscienciaNegra,
+                ConscienciaNegraNacional,
                 VesperaNatal,
                 Natal,
                 AnoNovo,
             ]
         )
 
     @property
```

### Comparing `exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_cmes.py` & `exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_cmes.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_iepa.py` & `exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_iepa.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xams.py` & `exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xams.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xasx.py` & `exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xasx.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xbkk.py` & `exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xbkk.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xbog.py` & `exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xbog.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xbom.py` & `exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xbom.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xbru.py` & `exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xbru.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xbse.py` & `exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xbse.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xbud.py` & `exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xbud.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xbue.py` & `exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xbue.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xcbf.py` & `exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xcbf.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xcse.py` & `exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xcse.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xdub.py` & `exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xdub.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,21 +55,30 @@
 )
 
 LabourDayFrom2019 = european_labour_day(
     start_date="2019",
     observance=weekend_to_monday,
 )
 
-MayBankHoliday = Holiday(
+MayBankHolidayTo2018 = Holiday(
     "May Bank Holiday",
     month=5,
     day=1,
     end_date="2019",
     offset=DateOffset(weekday=MO(1)),
 )
+
+MayBankHolidayFrom2021 = Holiday(
+    "May Bank Holiday",
+    month=5,
+    day=1,
+    start_date="2021",
+    offset=DateOffset(weekday=MO(1)),
+)
+
 JuneBankHoliday = Holiday(
     "June Bank Holiday",
     month=6,
     day=1,
     end_date="2019",
     offset=DateOffset(weekday=MO(1)),
 )
@@ -139,15 +148,16 @@
             [
                 NewYearsDay,
                 StPatricksDay,
                 GoodFriday,
                 EasterMonday,
                 LabourDayTo2009,
                 LabourDayFrom2019,
-                MayBankHoliday,
+                MayBankHolidayTo2018,
+                MayBankHolidayFrom2021,
                 JuneBankHoliday,
                 ChristmasEve,
                 Christmas,
                 WeekendChristmas,
                 BoxingDay,
                 WeekendBoxingDay,
             ]
```

### Comparing `exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xetr.py` & `exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xetr.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xfra.py` & `exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xfra.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xhel.py` & `exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xhel.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xhkg.py` & `exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xhkg.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xice.py` & `exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xice.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xidx.py` & `exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xidx.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xist.py` & `exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xist.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xjse.py` & `exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xjse.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xkar.py` & `exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xkar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xkls.py` & `exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xkls.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xkrx.py` & `exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xkrx.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xlim.py` & `exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xlim.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xlis.py` & `exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xlis.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xlon.py` & `exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xlon.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xmad.py` & `exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xmad.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xmex.py` & `exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xmex.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xmil.py` & `exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xmil.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xmos.py` & `exchange_calendars-4.5.4/exchange_calendars/xbkk_holidays.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,321 +1,325 @@
-#
-# Copyright 2019 Quantopian, Inc.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
 from __future__ import annotations
 
 import datetime
-from itertools import chain
-from zoneinfo import ZoneInfo
 
-from pandas.tseries.holiday import Holiday, weekend_to_monday
+import pandas as pd
+from pandas.tseries.holiday import (
+    Holiday,
+    next_monday_or_tuesday,
+    sunday_to_monday,
+    weekend_to_monday,
+)
 
 from .common_holidays import european_labour_day, new_years_day, new_years_eve
-from .exchange_calendar import WEEKDAYS, HolidayCalendar, ExchangeCalendar
+from .exchange_calendar import MONDAY, SUNDAY
 
 
 def new_years_eve_observance(dt: datetime.datetime) -> datetime.datetime | None:
-    # For some reason New Year's Eve was not a holiday these years.
-    return None if dt.year in [2008, 2009] else weekend_to_monday(dt)
+    # New Year's Eve is a holiday every year except for 2003 for some reason.
+    return weekend_to_monday(dt) if dt.year != 2003 else None
 
 
 def new_years_day_observance(dt: datetime.datetime) -> datetime.datetime | None:
-    # New Year's Day did not follow the next-non-holiday rule these years.
-    return None if dt.year in [2022] else weekend_to_monday(dt)
-
-
-def new_years_holiday_observance(dt: datetime.datetime) -> datetime.datetime | None:
-    # New Year's Holiday did not follow the next-non-holiday rule these years.
-    return None if dt.year in [2016, 2021, 2022] else weekend_to_monday(dt)
-
+    # There was no extra observance of New Year's Day in 2006.
+    return next_monday_or_tuesday(dt) if dt.year != 2006 else None
 
-def orthodox_christmas_observance(dt: datetime.datetime) -> datetime.datetime | None:
-    # Orthodox Christmas did not follow the next-non-holiday rule these years.
-    return None if dt.year in [2012, 2017, 2023, 2024] else weekend_to_monday(dt)
 
-
-def defender_of_fatherland_observance(
-    dt: datetime.datetime,
-) -> datetime.datetime | None:
-    # Defender of the Fatherland Day did not follow the next-non-holiday rule
-    # these years.
-    return None if dt.year in [2013, 2014, 2019] else weekend_to_monday(dt)
-
-
-def victory_day_observance(dt: datetime.datetime) -> datetime.datetime | None:
-    # Victory Day did not follow the next-non-holiday rule these years.
-    return None if dt.year in [2021] else weekend_to_monday(dt)
+def songkran_festival_last_day_observance(dt: datetime.datetime) -> datetime.datetime:
+    """
+    This function is similar to the pandas function `next_monday_or_tuesday`
+    except it does not observe Saturday holidays on Monday.
+    """
+    if dt.weekday() == SUNDAY or dt.weekday() == MONDAY:
+        return dt + datetime.timedelta(days=1)
+    return dt
 
 
-def day_of_russia_observance(dt: datetime.datetime) -> datetime.datetime | None:
-    # Day of Russia did not follow the next-non-holiday rule these years.
-    return None if dt.year in [2021] else weekend_to_monday(dt)
+NewYearsDay = new_years_day(observance=new_years_day_observance)
 
+ChakriMemorialDay = Holiday(
+    "Chakri Memorial Day",
+    month=4,
+    day=6,
+    observance=weekend_to_monday,
+)
 
-def unity_day_observance(dt: datetime.datetime) -> datetime.datetime | None:
-    # Unity Day did not follow the next-non-holiday rule these years.
-    return None if dt.year in [2023] else weekend_to_monday(dt)
+# Thai New Year. This does not follow the usual observe-next-trading-day rule.
+SongkranFestival1 = Holiday("Songkran Festival", month=4, day=13)
+SongkranFestival2 = Holiday(
+    "Songkran Festival",
+    month=4,
+    day=14,
+    observance=sunday_to_monday,
+)
+SongkranFestival3 = Holiday(
+    "Songkran Festival",
+    month=4,
+    day=15,
+    observance=songkran_festival_last_day_observance,
+)
 
+LabourDay = european_labour_day(observance=weekend_to_monday)
 
-NewYearsDay = new_years_day(observance=new_years_day_observance)
-NewYearsHoliday = Holiday(
-    "New Year's Holiday",
-    month=1,
-    day=2,
-    observance=new_years_holiday_observance,
-)
-NewYearsHoliday2 = Holiday(
-    "New Year's Holiday",
-    month=1,
-    day=3,
-    start_date="2005",
-    end_date="2012",
-)
-NewYearsHoliday3 = Holiday(
-    "New Year's Holiday",
-    month=1,
-    day=4,
-    start_date="2005",
-    end_date="2012",
-)
-NewYearsHoliday4 = Holiday(
-    "New Year's Holiday",
-    month=1,
+CoronationDay2016AndBefore = Holiday(
+    "Coronation Day For King #9",
+    month=5,
     day=5,
-    start_date="2005",
-    end_date="2012",
+    observance=weekend_to_monday,
+    end_date="2017",
 )
-NewYearsHoliday5 = Holiday(
-    "New Year's Holiday",
-    month=1,
-    day=6,
-    start_date="2005",
-    end_date="2012",
+CoronationDay2019AndAfter = Holiday(
+    "Coronation Day For King #10",
+    month=5,
+    day=4,
+    observance=weekend_to_monday,
+    start_date="2019",
 )
 
-OrthodoxChristmas = Holiday(
-    "Orthodox Christmas",
-    month=1,
-    day=7,
-    observance=orthodox_christmas_observance,
+HMQueensBirthday = Holiday(
+    "Her Majesty The Queen's Birthday",
+    month=6,
+    day=3,
+    observance=weekend_to_monday,
+    start_date="2019",
 )
-
-DefenderOfTheFatherlandDay = Holiday(
-    "Defender of the Fatherland Day",
-    month=2,
-    day=23,
-    observance=defender_of_fatherland_observance,
+HMKingsBirthday = Holiday(
+    "His Majesty The King's Birthday",
+    month=7,
+    day=28,
+    observance=weekend_to_monday,
+    start_date="2017",
 )
-
-WomensDay = Holiday(
-    "Women's Day",
-    month=3,
-    day=8,
+HMQueenMothersBirthday = Holiday(
+    "Her Majesty The Queen Mother's Birthday",
+    month=8,
+    day=12,
     observance=weekend_to_monday,
 )
 
-LabourDay = european_labour_day(observance=weekend_to_monday)
+# This holiday was historically used as a "catch up" day for the exchange, so
+# it does not need to follow the usual observe-next-trading-day rule.
+HalfYearHoliday = Holiday(
+    "Half Year Holiday",
+    month=7,
+    day=1,
+    start_date="2002",
+    end_date="2017",
+)
 
-VictoryDay = Holiday(
-    "Victory Day",
-    month=5,
-    day=9,
-    observance=victory_day_observance,
+ThePassingOfKingBhumibol = Holiday(
+    "The Passing of King Bhumibol",
+    month=10,
+    day=13,
+    observance=weekend_to_monday,
+    start_date="2017",
 )
 
-DayOfRussia = Holiday(
-    "Day of Russia",
-    month=6,
-    day=12,
-    observance=day_of_russia_observance,
+ChulalongkornDay = Holiday(
+    "Chulalongkorn Day",
+    month=10,
+    day=23,
+    observance=weekend_to_monday,
 )
 
-UnityDay = Holiday(
-    "Unity Day",
-    month=11,
-    day=4,
-    observance=unity_day_observance,
-    start_date="2005",
+KingBhumibolsBirthday = Holiday(
+    "King Bhumibol's Birthday",
+    month=12,
+    day=5,
+    observance=weekend_to_monday,
 )
 
-NewYearsEve = new_years_eve(
-    observance=new_years_eve_observance,
-    days_of_week=WEEKDAYS,
+ThailandConstitutionDay = Holiday(
+    "Thailand Constitution Day",
+    month=12,
+    day=10,
+    observance=weekend_to_monday,
 )
 
+NewYearsEve = new_years_eve(observance=new_years_eve_observance)
 
 # Adhoc Holidays
 # --------------
 
-# All of the following "extensions" are bridge holidays, meaning they are
-# either a Monday or Friday that is made into a holiday to fill in the gap
-# between a Tuesday or Thursday holiday, respectively. Unfortunately having
-# these bridge days is not consistently the rule, so they are treated as adhoc.
-# This means that in the future there may be manual additions needed here.
-new_years_extensions = [
-    "2003-01-03",
-    "2013-01-03",
-    "2013-01-04",
-    "2014-01-03",
-]
-
-orthodox_christmas_extensions = [
-    "2003-01-06",
-    "2005-01-10",
-    "2008-01-08",
-    "2009-01-08",
-    "2009-01-09",
-    "2010-01-08",
-    "2011-01-10",
-    "2016-01-08",
+new_years_bridge_days = [
+    pd.Timestamp("2002-12-30"),
+    pd.Timestamp("2004-01-02"),
+    pd.Timestamp("2009-01-02"),
+    pd.Timestamp("2013-12-30"),
+    pd.Timestamp("2015-01-02"),
 ]
 
-defender_of_the_fatherland_extensions = [
-    "2006-02-24",
-    "2010-02-22",
+asanha_bucha_bridge_days = [
+    pd.Timestamp("2009-07-06"),
+    pd.Timestamp("2016-07-18"),
 ]
 
-womens_day_extensions = [
-    "2005-03-07",
-    "2011-03-07",
-    "2012-03-09",
-    "2022-03-07",
+queens_birthday_bridge_days = [
+    pd.Timestamp("2010-08-13"),
+    pd.Timestamp("2014-08-11"),
 ]
 
-labour_day_extensions = [
-    "2002-05-02",
-    "2002-05-03",
-    "2003-05-02",
-    "2004-05-04",
-    "2007-04-30",
-    "2008-05-02",
-    "2012-04-30",
-    "2015-05-04",
-    "2016-05-03",
-    # LabourDay Holiday extended to Tuesday.
-    "2022-05-03",
+coronation_bridge_days = [
+    pd.Timestamp("2015-05-04"),
+    pd.Timestamp("2016-05-06"),
 ]
 
-victory_day_extensions = [
-    "2002-05-10",
-    "2005-05-10",
-    "2006-05-08",
-    "2017-05-08",
-    # Victory Day Holiday extended to Tuesday.
-    "2022-05-10",
-]
-
-day_of_russia_extensions = [
-    "2003-06-13",
-    "2007-06-11",
-    "2008-06-13",
-    "2012-06-11",
-    "2014-06-13",
-]
-
-unity_day_extensions = [
-    "2008-11-03",
-    "2010-11-05",
+vesak_bridge_days = [
+    pd.Timestamp("2011-05-16"),
 ]
 
 misc_adhoc = [
-    # Exchange Holidays.
-    "2002-11-07",
-    "2002-11-08",
-    "2002-12-12",
-    "2002-12-13",
-    "2003-11-07",
-    "2003-12-12",
-    "2004-11-08",
-    "2004-12-13",
-    "2008-09-18",
-    # Trading Suspended.
-    "2008-10-10",
-    "2008-10-27",
-    # Non-Working Days.
-    "2020-06-24",
-    "2020-07-01",
+    pd.Timestamp("2006-04-19"),  # Special Holiday
+    pd.Timestamp("2006-06-12"),  # Special Holiday
+    pd.Timestamp("2006-06-13"),  # Special Holiday
+    pd.Timestamp("2006-09-20"),  # Exchange Holiday
+    pd.Timestamp("2007-12-24"),  # Exchange Holiday
+    pd.Timestamp("2010-05-20"),  # Closure Due to Security Concerns
+    pd.Timestamp("2010-05-21"),  # Closure Due to Security Concerns
+    pd.Timestamp("2012-04-09"),  # Bank Holiday
+    pd.Timestamp("2017-10-26"),  # Cremation of King Bhumibol
 ]
 
+# Lunar Holidays
+# --------------
 
-class XMOSExchangeCalendar(ExchangeCalendar):
-    """
-    Exchange calendar for the Moscow Stock Exchange.
-
-    Open Time: 10:00 AM, MSK (Moscow Standard Time)
-    Close Time: 6:45 PM, MSK (Moscow Standard Time)
-
-    Regularly-Observed Holidays:
-      - New Year's Day
-      - New Year's Holiday
-      - Orthodox Christmas Day
-      - Defender of the Fatherland Day
-      - Women's Day
-      - Spring and Labour Day
-      - Victory Day
-      - Day of Russia
-      - Unity Day
-      - New Year's Eve
-
-    Holidays No Longer Observed:
-      - New Year's Holiday Week
-
-    Early Closes:
-      - None
-    """
-
-    name = "XMOS"
-
-    tz = ZoneInfo("Europe/Moscow")
-
-    open_times = ((None, datetime.time(10)),)
-
-    close_times = ((None, datetime.time(18, 45)),)
-
-    @property
-    def regular_holidays(self):
-        return HolidayCalendar(
-            [
-                NewYearsDay,
-                NewYearsHoliday,
-                NewYearsHoliday2,
-                NewYearsHoliday3,
-                NewYearsHoliday4,
-                NewYearsHoliday5,
-                OrthodoxChristmas,
-                DefenderOfTheFatherlandDay,
-                WomensDay,
-                LabourDay,
-                VictoryDay,
-                DayOfRussia,
-                UnityDay,
-                NewYearsEve,
-            ]
-        )
-
-    @property
-    def adhoc_holidays(self):
-        return list(
-            chain(
-                new_years_extensions,
-                orthodox_christmas_extensions,
-                defender_of_the_fatherland_extensions,
-                womens_day_extensions,
-                labour_day_extensions,
-                victory_day_extensions,
-                day_of_russia_extensions,
-                unity_day_extensions,
-                misc_adhoc,
-            ),
-        )
+# Makha Bucha (also known as Magha Puja) is celebrated on the day of the Full
+# Moon of Magha in the Buddhist calendar. This falls sometime between February
+# and March.
+makha_bucha = pd.to_datetime(
+    [
+        "1981-02-18",
+        "1982-02-08",
+        "1983-02-27",
+        "1984-02-16",
+        "1985-03-06",
+        "1986-02-24",
+        "1987-02-13",
+        "1988-03-03",
+        "1989-02-20",
+        "1990-02-09",
+        "1991-02-28",
+        "1992-02-18",
+        "1993-03-08",
+        "1994-02-25",
+        "1995-02-15",
+        "1996-03-05",
+        "1997-02-22",
+        "1998-02-11",
+        "1999-03-02",
+        "2000-02-19",
+        "2001-02-08",
+        "2002-02-26",
+        "2003-02-17",
+        "2004-03-05",
+        "2005-02-23",
+        "2006-02-13",
+        "2007-03-05",
+        "2008-02-21",
+        "2009-02-09",
+        "2010-03-01",
+        "2011-02-18",
+        "2012-03-07",
+        "2013-02-25",
+        "2014-02-14",
+        "2015-03-04",
+        "2016-02-22",
+        "2017-02-13",
+        "2018-03-01",
+        "2019-02-19",
+        "2020-02-10",
+    ]
+)
+
+# Vesak (also known as Buddha Day) is celebrated on the day of the Full Moon of
+# Visakha in the Buddhist calendar. This typically falls in May.
+vesak = pd.to_datetime(
+    [
+        "1981-05-18",
+        "1982-05-07",
+        "1983-05-26",
+        "1984-05-15",
+        "1985-06-02",
+        "1986-05-23",
+        "1987-05-13",
+        "1988-05-31",
+        "1989-05-20",
+        "1990-05-09",
+        "1991-05-28",
+        "1992-05-16",
+        "1993-06-04",
+        "1994-05-24",
+        "1995-05-14",
+        "1996-06-01",
+        "1997-05-22",
+        "1998-05-11",
+        "1999-05-30",
+        "2000-05-18",
+        "2001-05-07",
+        "2002-05-27",
+        "2003-05-15",
+        "2004-06-02",
+        "2005-05-23",
+        "2006-05-12",
+        "2007-05-31",
+        "2008-05-19",
+        "2009-05-08",
+        "2010-05-28",
+        "2011-05-17",
+        "2012-06-04",
+        "2013-05-24",
+        "2014-05-13",
+        "2015-06-01",
+        "2016-05-20",
+        "2017-05-10",
+        "2018-05-29",
+        "2019-05-20",
+        "2020-05-06",
+    ]
+)
+
+# Asanha Bucha (also known as Asalha Puja) is celebrated on the day of the Full
+# Moon of Asadha in the Buddhist calendar. This typically falls in July.
+asanha_bucha = pd.to_datetime(
+    [
+        "1981-07-17",
+        "1982-07-06",
+        "1983-07-24",
+        "1984-07-12",
+        "1985-07-31",
+        "1986-07-21",
+        "1987-07-10",
+        "1988-07-28",
+        "1989-07-18",
+        "1990-07-07",
+        "1991-07-26",
+        "1992-07-14",
+        "1993-08-02",
+        "1994-07-22",
+        "1995-07-12",
+        "1996-07-30",
+        "1997-07-19",
+        "1998-07-09",
+        "1999-07-28",
+        "2000-07-16",
+        "2001-07-05",
+        "2002-07-25",
+        "2003-07-14",
+        "2004-08-02",
+        "2005-07-22",
+        "2006-07-11",
+        "2007-07-30",
+        "2008-07-17",
+        "2009-07-07",
+        "2010-07-26",
+        "2011-07-15",
+        "2012-08-02",
+        "2013-07-22",
+        "2014-07-11",
+        "2015-07-30",
+        "2016-07-19",
+        "2017-07-10",
+        "2018-07-27",
+        "2019-07-16",
+        "2020-07-06",
+    ]
+)
```

### Comparing `exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xnys.py` & `exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xnys.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xnze.py` & `exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xnze.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xosl.py` & `exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xosl.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xpar.py` & `exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xpar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xphs.py` & `exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xphs.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xpra.py` & `exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xpra.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xsau.py` & `exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xsau.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xses.py` & `exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xses.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xsgo.py` & `exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xsgo.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xshg.py` & `exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xshg.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xsto.py` & `exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xsto.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xswx.py` & `exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xswx.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xtae.py` & `exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xtae.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xtai.py` & `exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xtai.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xtks.py` & `exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xtks.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xtse.py` & `exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xtse.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xwar.py` & `exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xwar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/exchange_calendars/exchange_calendar_xwbo.py` & `exchange_calendars-4.5.4/exchange_calendars/exchange_calendar_xwbo.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/exchange_calendars/lunisolar_holidays.py` & `exchange_calendars-4.5.4/exchange_calendars/lunisolar_holidays.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/exchange_calendars/pandas_extensions/holiday.py` & `exchange_calendars-4.5.4/exchange_calendars/pandas_extensions/holiday.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/exchange_calendars/pandas_extensions/korean_holiday.py` & `exchange_calendars-4.5.4/exchange_calendars/pandas_extensions/korean_holiday.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/exchange_calendars/pandas_extensions/offsets.py` & `exchange_calendars-4.5.4/exchange_calendars/pandas_extensions/offsets.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,16 @@
                     pd.Timestamp.min, right.left - pd.Timedelta(1, unit="D")
                 )
                 business_days_all_intervals.append(interval)
             business_days_all_intervals.append(right)
             for left, right in toolz.sliding_window(
                 2, toolz.concatv(self._business_days_index)
             ):
-                if right.left - left.right > pd.Timestamp(1, unit="D"):
+                if pd.Timestamp((right.left - left.right).days,
+                                unit="D") > pd.Timestamp(1, unit="D"):
                     interval = pd.Interval(
                         left.right + pd.Timedelta(1, unit="D"),
                         right.left - pd.Timedelta(1, unit="D"),
                     )
                     business_days_all_intervals.append(interval)
                 business_days_all_intervals.append(right)
             left = self._business_days_index[-1]
@@ -161,15 +162,15 @@
                 moved += self._moved(previous_other, other, bday)
                 remaining = self.n - moved
                 if remaining == 0:
                     break
                 bday, interval = self._custom_business_day_for(
                     other, remaining, is_edge=True, with_interval=True
                 )
-                result = bday.apply(other)
+                result = bday._apply(other)
             return result
         else:
             return super().apply(other)
 
     # backwards compat
     apply = _apply
```

### Comparing `exchange_calendars-4.5.3/exchange_calendars/precomputed_exchange_calendar.py` & `exchange_calendars-4.5.4/exchange_calendars/precomputed_exchange_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/exchange_calendars/tase_holidays.py` & `exchange_calendars-4.5.4/exchange_calendars/tase_holidays.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/exchange_calendars/us_futures_calendar.py` & `exchange_calendars-4.5.4/exchange_calendars/us_futures_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/exchange_calendars/us_holidays.py` & `exchange_calendars-4.5.4/exchange_calendars/us_holidays.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/exchange_calendars/utils/pandas_utils.py` & `exchange_calendars-4.5.4/exchange_calendars/utils/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/exchange_calendars/xkls_holidays.py` & `exchange_calendars-4.5.4/exchange_calendars/xkls_holidays.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/exchange_calendars/xkrx_holidays.py` & `exchange_calendars-4.5.4/exchange_calendars/xkrx_holidays.py`

 * *Files 0% similar despite different names*

```diff
@@ -1106,14 +1106,15 @@
 
 # This index contains holidays that were manually copied from the exchange website
 #  (https://global.krx.co.kr/contents/GLB/05/0501/0501110000/GLB0501110000.jsp)
 manually_added_holidays = pd.DatetimeIndex(
     [
         "2023-05-29",  # Buddha's birthday holiday in lieu
         "2023-10-02",  # Extra day for Chuseok holiday
+        "2024-04-10",  # Parliamentary election day
     ]
 )
 
 
 # Merging two holidays to get full precomputed holidays list.
 precomputed_krx_holidays = original_precomputed_krx_holidays.union(
     dumped_precomputed_krx_holidays
```

### Comparing `exchange_calendars-4.5.3/exchange_calendars/xtks_holidays.py` & `exchange_calendars-4.5.4/exchange_calendars/xtks_holidays.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/exchange_calendars.egg-info/PKG-INFO` & `exchange_calendars-4.5.4/exchange_calendars.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exchange_calendars
-Version: 4.5.3
+Version: 4.5.4
 Summary: Calendars for securities exchanges
 Author: Gerry Manoim
 Author-email: gerrymanoim@gmail.com
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `exchange_calendars-4.5.3/exchange_calendars.egg-info/SOURCES.txt` & `exchange_calendars-4.5.4/exchange_calendars.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/pyproject.toml` & `exchange_calendars-4.5.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/setup.cfg` & `exchange_calendars-4.5.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/resources/24-5.csv` & `exchange_calendars-4.5.4/tests/resources/24-5.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/resources/24-7.csv` & `exchange_calendars-4.5.4/tests/resources/24-7.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/resources/aixk.csv` & `exchange_calendars-4.5.4/tests/resources/aixk.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/resources/asex.csv` & `exchange_calendars-4.5.4/tests/resources/asex.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/resources/bvmf.csv` & `exchange_calendars-4.5.4/tests/resources/bvmf.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/resources/cmes.csv` & `exchange_calendars-4.5.4/tests/resources/cmes.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/resources/iepa.csv` & `exchange_calendars-4.5.4/tests/resources/iepa.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/resources/test.csv` & `exchange_calendars-4.5.4/tests/resources/test.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/resources/xams.csv` & `exchange_calendars-4.5.4/tests/resources/xams.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/resources/xasx.csv` & `exchange_calendars-4.5.4/tests/resources/xasx.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/resources/xbkk.csv` & `exchange_calendars-4.5.4/tests/resources/xbkk.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/resources/xbog.csv` & `exchange_calendars-4.5.4/tests/resources/xbog.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/resources/xbom.csv` & `exchange_calendars-4.5.4/tests/resources/xbom.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/resources/xbru.csv` & `exchange_calendars-4.5.4/tests/resources/xbru.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/resources/xbse.csv` & `exchange_calendars-4.5.4/tests/resources/xbse.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/resources/xbud.csv` & `exchange_calendars-4.5.4/tests/resources/xbud.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/resources/xbue.csv` & `exchange_calendars-4.5.4/tests/resources/xbue.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/resources/xcbf.csv` & `exchange_calendars-4.5.4/tests/resources/xcbf.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/resources/xcse.csv` & `exchange_calendars-4.5.4/tests/resources/xcse.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/resources/xdub.csv` & `exchange_calendars-4.5.4/tests/resources/xdub.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/resources/xetr.csv` & `exchange_calendars-4.5.4/tests/resources/xetr.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/resources/xfra.csv` & `exchange_calendars-4.5.4/tests/resources/xfra.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/resources/xhel.csv` & `exchange_calendars-4.5.4/tests/resources/xhel.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/resources/xhkg.csv` & `exchange_calendars-4.5.4/tests/resources/xhkg.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/resources/xice.csv` & `exchange_calendars-4.5.4/tests/resources/xice.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/resources/xidx.csv` & `exchange_calendars-4.5.4/tests/resources/xidx.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/resources/xist.csv` & `exchange_calendars-4.5.4/tests/resources/xist.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/resources/xjse.csv` & `exchange_calendars-4.5.4/tests/resources/xjse.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/resources/xkar.csv` & `exchange_calendars-4.5.4/tests/resources/xkar.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/resources/xkls.csv` & `exchange_calendars-4.5.4/tests/resources/xkls.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/resources/xkrx.csv` & `exchange_calendars-4.5.4/tests/resources/xkrx.csv`

 * *Files 0% similar despite different names*

```diff
@@ -10044,15 +10044,14 @@
 2024-04-01T00:00:00Z,2024-04-01T00:00:00Z,2024-04-01T06:30:00Z,,
 2024-04-02T00:00:00Z,2024-04-02T00:00:00Z,2024-04-02T06:30:00Z,,
 2024-04-03T00:00:00Z,2024-04-03T00:00:00Z,2024-04-03T06:30:00Z,,
 2024-04-04T00:00:00Z,2024-04-04T00:00:00Z,2024-04-04T06:30:00Z,,
 2024-04-05T00:00:00Z,2024-04-05T00:00:00Z,2024-04-05T06:30:00Z,,
 2024-04-08T00:00:00Z,2024-04-08T00:00:00Z,2024-04-08T06:30:00Z,,
 2024-04-09T00:00:00Z,2024-04-09T00:00:00Z,2024-04-09T06:30:00Z,,
-2024-04-10T00:00:00Z,2024-04-10T00:00:00Z,2024-04-10T06:30:00Z,,
 2024-04-11T00:00:00Z,2024-04-11T00:00:00Z,2024-04-11T06:30:00Z,,
 2024-04-12T00:00:00Z,2024-04-12T00:00:00Z,2024-04-12T06:30:00Z,,
 2024-04-15T00:00:00Z,2024-04-15T00:00:00Z,2024-04-15T06:30:00Z,,
 2024-04-16T00:00:00Z,2024-04-16T00:00:00Z,2024-04-16T06:30:00Z,,
 2024-04-17T00:00:00Z,2024-04-17T00:00:00Z,2024-04-17T06:30:00Z,,
 2024-04-18T00:00:00Z,2024-04-18T00:00:00Z,2024-04-18T06:30:00Z,,
 2024-04-19T00:00:00Z,2024-04-19T00:00:00Z,2024-04-19T06:30:00Z,,
@@ -10156,8 +10155,100 @@
 2024-09-11T00:00:00Z,2024-09-11T00:00:00Z,2024-09-11T06:30:00Z,,
 2024-09-12T00:00:00Z,2024-09-12T00:00:00Z,2024-09-12T06:30:00Z,,
 2024-09-13T00:00:00Z,2024-09-13T00:00:00Z,2024-09-13T06:30:00Z,,
 2024-09-19T00:00:00Z,2024-09-19T00:00:00Z,2024-09-19T06:30:00Z,,
 2024-09-20T00:00:00Z,2024-09-20T00:00:00Z,2024-09-20T06:30:00Z,,
 2024-09-23T00:00:00Z,2024-09-23T00:00:00Z,2024-09-23T06:30:00Z,,
 2024-09-24T00:00:00Z,2024-09-24T00:00:00Z,2024-09-24T06:30:00Z,,
-2024-09-25T00:00:00Z,2024-09-25T01:00:00Z,2024-09-25T06:30:00Z,,
+2024-09-25T00:00:00Z,2024-09-25T00:00:00Z,2024-09-25T06:30:00Z,,
+2024-09-26T00:00:00Z,2024-09-26T00:00:00Z,2024-09-26T06:30:00Z,,
+2024-09-27T00:00:00Z,2024-09-27T00:00:00Z,2024-09-27T06:30:00Z,,
+2024-09-30T00:00:00Z,2024-09-30T00:00:00Z,2024-09-30T06:30:00Z,,
+2024-10-01T00:00:00Z,2024-10-01T00:00:00Z,2024-10-01T06:30:00Z,,
+2024-10-02T00:00:00Z,2024-10-02T00:00:00Z,2024-10-02T06:30:00Z,,
+2024-10-04T00:00:00Z,2024-10-04T00:00:00Z,2024-10-04T06:30:00Z,,
+2024-10-07T00:00:00Z,2024-10-07T00:00:00Z,2024-10-07T06:30:00Z,,
+2024-10-08T00:00:00Z,2024-10-08T00:00:00Z,2024-10-08T06:30:00Z,,
+2024-10-10T00:00:00Z,2024-10-10T00:00:00Z,2024-10-10T06:30:00Z,,
+2024-10-11T00:00:00Z,2024-10-11T00:00:00Z,2024-10-11T06:30:00Z,,
+2024-10-14T00:00:00Z,2024-10-14T00:00:00Z,2024-10-14T06:30:00Z,,
+2024-10-15T00:00:00Z,2024-10-15T00:00:00Z,2024-10-15T06:30:00Z,,
+2024-10-16T00:00:00Z,2024-10-16T00:00:00Z,2024-10-16T06:30:00Z,,
+2024-10-17T00:00:00Z,2024-10-17T00:00:00Z,2024-10-17T06:30:00Z,,
+2024-10-18T00:00:00Z,2024-10-18T00:00:00Z,2024-10-18T06:30:00Z,,
+2024-10-21T00:00:00Z,2024-10-21T00:00:00Z,2024-10-21T06:30:00Z,,
+2024-10-22T00:00:00Z,2024-10-22T00:00:00Z,2024-10-22T06:30:00Z,,
+2024-10-23T00:00:00Z,2024-10-23T00:00:00Z,2024-10-23T06:30:00Z,,
+2024-10-24T00:00:00Z,2024-10-24T00:00:00Z,2024-10-24T06:30:00Z,,
+2024-10-25T00:00:00Z,2024-10-25T00:00:00Z,2024-10-25T06:30:00Z,,
+2024-10-28T00:00:00Z,2024-10-28T00:00:00Z,2024-10-28T06:30:00Z,,
+2024-10-29T00:00:00Z,2024-10-29T00:00:00Z,2024-10-29T06:30:00Z,,
+2024-10-30T00:00:00Z,2024-10-30T00:00:00Z,2024-10-30T06:30:00Z,,
+2024-10-31T00:00:00Z,2024-10-31T00:00:00Z,2024-10-31T06:30:00Z,,
+2024-11-01T00:00:00Z,2024-11-01T00:00:00Z,2024-11-01T06:30:00Z,,
+2024-11-04T00:00:00Z,2024-11-04T00:00:00Z,2024-11-04T06:30:00Z,,
+2024-11-05T00:00:00Z,2024-11-05T00:00:00Z,2024-11-05T06:30:00Z,,
+2024-11-06T00:00:00Z,2024-11-06T00:00:00Z,2024-11-06T06:30:00Z,,
+2024-11-07T00:00:00Z,2024-11-07T00:00:00Z,2024-11-07T06:30:00Z,,
+2024-11-08T00:00:00Z,2024-11-08T00:00:00Z,2024-11-08T06:30:00Z,,
+2024-11-11T00:00:00Z,2024-11-11T00:00:00Z,2024-11-11T06:30:00Z,,
+2024-11-12T00:00:00Z,2024-11-12T00:00:00Z,2024-11-12T06:30:00Z,,
+2024-11-13T00:00:00Z,2024-11-13T00:00:00Z,2024-11-13T06:30:00Z,,
+2024-11-14T00:00:00Z,2024-11-14T00:00:00Z,2024-11-14T06:30:00Z,,
+2024-11-15T00:00:00Z,2024-11-15T00:00:00Z,2024-11-15T06:30:00Z,,
+2024-11-18T00:00:00Z,2024-11-18T00:00:00Z,2024-11-18T06:30:00Z,,
+2024-11-19T00:00:00Z,2024-11-19T00:00:00Z,2024-11-19T06:30:00Z,,
+2024-11-20T00:00:00Z,2024-11-20T00:00:00Z,2024-11-20T06:30:00Z,,
+2024-11-21T00:00:00Z,2024-11-21T00:00:00Z,2024-11-21T06:30:00Z,,
+2024-11-22T00:00:00Z,2024-11-22T00:00:00Z,2024-11-22T06:30:00Z,,
+2024-11-25T00:00:00Z,2024-11-25T00:00:00Z,2024-11-25T06:30:00Z,,
+2024-11-26T00:00:00Z,2024-11-26T00:00:00Z,2024-11-26T06:30:00Z,,
+2024-11-27T00:00:00Z,2024-11-27T00:00:00Z,2024-11-27T06:30:00Z,,
+2024-11-28T00:00:00Z,2024-11-28T00:00:00Z,2024-11-28T06:30:00Z,,
+2024-11-29T00:00:00Z,2024-11-29T00:00:00Z,2024-11-29T06:30:00Z,,
+2024-12-02T00:00:00Z,2024-12-02T00:00:00Z,2024-12-02T06:30:00Z,,
+2024-12-03T00:00:00Z,2024-12-03T00:00:00Z,2024-12-03T06:30:00Z,,
+2024-12-04T00:00:00Z,2024-12-04T00:00:00Z,2024-12-04T06:30:00Z,,
+2024-12-05T00:00:00Z,2024-12-05T00:00:00Z,2024-12-05T06:30:00Z,,
+2024-12-06T00:00:00Z,2024-12-06T00:00:00Z,2024-12-06T06:30:00Z,,
+2024-12-09T00:00:00Z,2024-12-09T00:00:00Z,2024-12-09T06:30:00Z,,
+2024-12-10T00:00:00Z,2024-12-10T00:00:00Z,2024-12-10T06:30:00Z,,
+2024-12-11T00:00:00Z,2024-12-11T00:00:00Z,2024-12-11T06:30:00Z,,
+2024-12-12T00:00:00Z,2024-12-12T00:00:00Z,2024-12-12T06:30:00Z,,
+2024-12-13T00:00:00Z,2024-12-13T00:00:00Z,2024-12-13T06:30:00Z,,
+2024-12-16T00:00:00Z,2024-12-16T00:00:00Z,2024-12-16T06:30:00Z,,
+2024-12-17T00:00:00Z,2024-12-17T00:00:00Z,2024-12-17T06:30:00Z,,
+2024-12-18T00:00:00Z,2024-12-18T00:00:00Z,2024-12-18T06:30:00Z,,
+2024-12-19T00:00:00Z,2024-12-19T00:00:00Z,2024-12-19T06:30:00Z,,
+2024-12-20T00:00:00Z,2024-12-20T00:00:00Z,2024-12-20T06:30:00Z,,
+2024-12-23T00:00:00Z,2024-12-23T00:00:00Z,2024-12-23T06:30:00Z,,
+2024-12-24T00:00:00Z,2024-12-24T00:00:00Z,2024-12-24T06:30:00Z,,
+2024-12-26T00:00:00Z,2024-12-26T00:00:00Z,2024-12-26T06:30:00Z,,
+2024-12-27T00:00:00Z,2024-12-27T00:00:00Z,2024-12-27T06:30:00Z,,
+2024-12-30T00:00:00Z,2024-12-30T00:00:00Z,2024-12-30T06:30:00Z,,
+2025-01-02T00:00:00Z,2025-01-02T01:00:00Z,2025-01-02T06:30:00Z,,
+2025-01-03T00:00:00Z,2025-01-03T00:00:00Z,2025-01-03T06:30:00Z,,
+2025-01-06T00:00:00Z,2025-01-06T00:00:00Z,2025-01-06T06:30:00Z,,
+2025-01-07T00:00:00Z,2025-01-07T00:00:00Z,2025-01-07T06:30:00Z,,
+2025-01-08T00:00:00Z,2025-01-08T00:00:00Z,2025-01-08T06:30:00Z,,
+2025-01-09T00:00:00Z,2025-01-09T00:00:00Z,2025-01-09T06:30:00Z,,
+2025-01-10T00:00:00Z,2025-01-10T00:00:00Z,2025-01-10T06:30:00Z,,
+2025-01-13T00:00:00Z,2025-01-13T00:00:00Z,2025-01-13T06:30:00Z,,
+2025-01-14T00:00:00Z,2025-01-14T00:00:00Z,2025-01-14T06:30:00Z,,
+2025-01-15T00:00:00Z,2025-01-15T00:00:00Z,2025-01-15T06:30:00Z,,
+2025-01-16T00:00:00Z,2025-01-16T00:00:00Z,2025-01-16T06:30:00Z,,
+2025-01-17T00:00:00Z,2025-01-17T00:00:00Z,2025-01-17T06:30:00Z,,
+2025-01-20T00:00:00Z,2025-01-20T00:00:00Z,2025-01-20T06:30:00Z,,
+2025-01-21T00:00:00Z,2025-01-21T00:00:00Z,2025-01-21T06:30:00Z,,
+2025-01-22T00:00:00Z,2025-01-22T00:00:00Z,2025-01-22T06:30:00Z,,
+2025-01-23T00:00:00Z,2025-01-23T00:00:00Z,2025-01-23T06:30:00Z,,
+2025-01-24T00:00:00Z,2025-01-24T00:00:00Z,2025-01-24T06:30:00Z,,
+2025-01-27T00:00:00Z,2025-01-27T00:00:00Z,2025-01-27T06:30:00Z,,
+2025-01-31T00:00:00Z,2025-01-31T00:00:00Z,2025-01-31T06:30:00Z,,
+2025-02-03T00:00:00Z,2025-02-03T00:00:00Z,2025-02-03T06:30:00Z,,
+2025-02-04T00:00:00Z,2025-02-04T00:00:00Z,2025-02-04T06:30:00Z,,
+2025-02-05T00:00:00Z,2025-02-05T00:00:00Z,2025-02-05T06:30:00Z,,
+2025-02-06T00:00:00Z,2025-02-06T00:00:00Z,2025-02-06T06:30:00Z,,
+2025-02-07T00:00:00Z,2025-02-07T00:00:00Z,2025-02-07T06:30:00Z,,
+2025-02-10T00:00:00Z,2025-02-10T00:00:00Z,2025-02-10T06:30:00Z,,
+2025-02-11T00:00:00Z,2025-02-11T00:00:00Z,2025-02-11T06:30:00Z,,
+2025-02-12T00:00:00Z,2025-02-12T01:00:00Z,2025-02-12T06:30:00Z,,
```

### Comparing `exchange_calendars-4.5.3/tests/resources/xlim.csv` & `exchange_calendars-4.5.4/tests/resources/xlim.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/resources/xlis.csv` & `exchange_calendars-4.5.4/tests/resources/xlis.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/resources/xlon.csv` & `exchange_calendars-4.5.4/tests/resources/xlon.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/resources/xmad.csv` & `exchange_calendars-4.5.4/tests/resources/xmad.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/resources/xmex.csv` & `exchange_calendars-4.5.4/tests/resources/xmex.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/resources/xmil.csv` & `exchange_calendars-4.5.4/tests/resources/xmil.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/resources/xmos.csv` & `exchange_calendars-4.5.4/tests/resources/xmos.csv`

 * *Files 0% similar despite different names*

```diff
@@ -2270,14 +2270,15 @@
 1998-12-25T00:00:00Z,1998-12-25T07:00:00Z,1998-12-25T15:45:00Z,,
 1998-12-28T00:00:00Z,1998-12-28T07:00:00Z,1998-12-28T15:45:00Z,,
 1998-12-29T00:00:00Z,1998-12-29T07:00:00Z,1998-12-29T15:45:00Z,,
 1998-12-30T00:00:00Z,1998-12-30T07:00:00Z,1998-12-30T15:45:00Z,,
 1999-01-05T00:00:00Z,1999-01-05T07:00:00Z,1999-01-05T15:45:00Z,,
 1999-01-06T00:00:00Z,1999-01-06T07:00:00Z,1999-01-06T15:45:00Z,,
 1999-01-08T00:00:00Z,1999-01-08T07:00:00Z,1999-01-08T15:45:00Z,,
+1999-01-10T00:00:00Z,1999-01-10T07:00:00Z,1999-01-10T15:45:00Z,,
 1999-01-11T00:00:00Z,1999-01-11T07:00:00Z,1999-01-11T15:45:00Z,,
 1999-01-12T00:00:00Z,1999-01-12T07:00:00Z,1999-01-12T15:45:00Z,,
 1999-01-13T00:00:00Z,1999-01-13T07:00:00Z,1999-01-13T15:45:00Z,,
 1999-01-14T00:00:00Z,1999-01-14T07:00:00Z,1999-01-14T15:45:00Z,,
 1999-01-15T00:00:00Z,1999-01-15T07:00:00Z,1999-01-15T15:45:00Z,,
 1999-01-18T00:00:00Z,1999-01-18T07:00:00Z,1999-01-18T15:45:00Z,,
 1999-01-19T00:00:00Z,1999-01-19T07:00:00Z,1999-01-19T15:45:00Z,,
@@ -2604,14 +2605,15 @@
 2000-04-26T00:00:00Z,2000-04-26T06:00:00Z,2000-04-26T14:45:00Z,,
 2000-04-27T00:00:00Z,2000-04-27T06:00:00Z,2000-04-27T14:45:00Z,,
 2000-04-28T00:00:00Z,2000-04-28T06:00:00Z,2000-04-28T14:45:00Z,,
 2000-05-02T00:00:00Z,2000-05-02T06:00:00Z,2000-05-02T14:45:00Z,,
 2000-05-03T00:00:00Z,2000-05-03T06:00:00Z,2000-05-03T14:45:00Z,,
 2000-05-04T00:00:00Z,2000-05-04T06:00:00Z,2000-05-04T14:45:00Z,,
 2000-05-05T00:00:00Z,2000-05-05T06:00:00Z,2000-05-05T14:45:00Z,,
+2000-05-06T00:00:00Z,2000-05-06T06:00:00Z,2000-05-06T14:45:00Z,,
 2000-05-08T00:00:00Z,2000-05-08T06:00:00Z,2000-05-08T14:45:00Z,,
 2000-05-10T00:00:00Z,2000-05-10T06:00:00Z,2000-05-10T14:45:00Z,,
 2000-05-11T00:00:00Z,2000-05-11T06:00:00Z,2000-05-11T14:45:00Z,,
 2000-05-12T00:00:00Z,2000-05-12T06:00:00Z,2000-05-12T14:45:00Z,,
 2000-05-15T00:00:00Z,2000-05-15T06:00:00Z,2000-05-15T14:45:00Z,,
 2000-05-16T00:00:00Z,2000-05-16T06:00:00Z,2000-05-16T14:45:00Z,,
 2000-05-17T00:00:00Z,2000-05-17T06:00:00Z,2000-05-17T14:45:00Z,,
@@ -2732,14 +2734,15 @@
 2000-10-26T00:00:00Z,2000-10-26T06:00:00Z,2000-10-26T14:45:00Z,,
 2000-10-27T00:00:00Z,2000-10-27T06:00:00Z,2000-10-27T14:45:00Z,,
 2000-10-30T00:00:00Z,2000-10-30T07:00:00Z,2000-10-30T15:45:00Z,,
 2000-10-31T00:00:00Z,2000-10-31T07:00:00Z,2000-10-31T15:45:00Z,,
 2000-11-01T00:00:00Z,2000-11-01T07:00:00Z,2000-11-01T15:45:00Z,,
 2000-11-02T00:00:00Z,2000-11-02T07:00:00Z,2000-11-02T15:45:00Z,,
 2000-11-03T00:00:00Z,2000-11-03T07:00:00Z,2000-11-03T15:45:00Z,,
+2000-11-04T00:00:00Z,2000-11-04T07:00:00Z,2000-11-04T15:45:00Z,,
 2000-11-06T00:00:00Z,2000-11-06T07:00:00Z,2000-11-06T15:45:00Z,,
 2000-11-07T00:00:00Z,2000-11-07T07:00:00Z,2000-11-07T15:45:00Z,,
 2000-11-08T00:00:00Z,2000-11-08T07:00:00Z,2000-11-08T15:45:00Z,,
 2000-11-09T00:00:00Z,2000-11-09T07:00:00Z,2000-11-09T15:45:00Z,,
 2000-11-10T00:00:00Z,2000-11-10T07:00:00Z,2000-11-10T15:45:00Z,,
 2000-11-13T00:00:00Z,2000-11-13T07:00:00Z,2000-11-13T15:45:00Z,,
 2000-11-14T00:00:00Z,2000-11-14T07:00:00Z,2000-11-14T15:45:00Z,,
@@ -2757,14 +2760,15 @@
 2000-11-30T00:00:00Z,2000-11-30T07:00:00Z,2000-11-30T15:45:00Z,,
 2000-12-01T00:00:00Z,2000-12-01T07:00:00Z,2000-12-01T15:45:00Z,,
 2000-12-04T00:00:00Z,2000-12-04T07:00:00Z,2000-12-04T15:45:00Z,,
 2000-12-05T00:00:00Z,2000-12-05T07:00:00Z,2000-12-05T15:45:00Z,,
 2000-12-06T00:00:00Z,2000-12-06T07:00:00Z,2000-12-06T15:45:00Z,,
 2000-12-07T00:00:00Z,2000-12-07T07:00:00Z,2000-12-07T15:45:00Z,,
 2000-12-08T00:00:00Z,2000-12-08T07:00:00Z,2000-12-08T15:45:00Z,,
+2000-12-09T00:00:00Z,2000-12-09T07:00:00Z,2000-12-09T15:45:00Z,,
 2000-12-11T00:00:00Z,2000-12-11T07:00:00Z,2000-12-11T15:45:00Z,,
 2000-12-12T00:00:00Z,2000-12-12T07:00:00Z,2000-12-12T15:45:00Z,,
 2000-12-13T00:00:00Z,2000-12-13T07:00:00Z,2000-12-13T15:45:00Z,,
 2000-12-14T00:00:00Z,2000-12-14T07:00:00Z,2000-12-14T15:45:00Z,,
 2000-12-15T00:00:00Z,2000-12-15T07:00:00Z,2000-12-15T15:45:00Z,,
 2000-12-18T00:00:00Z,2000-12-18T07:00:00Z,2000-12-18T15:45:00Z,,
 2000-12-19T00:00:00Z,2000-12-19T07:00:00Z,2000-12-19T15:45:00Z,,
@@ -2817,14 +2821,15 @@
 2001-02-28T00:00:00Z,2001-02-28T07:00:00Z,2001-02-28T15:45:00Z,,
 2001-03-01T00:00:00Z,2001-03-01T07:00:00Z,2001-03-01T15:45:00Z,,
 2001-03-02T00:00:00Z,2001-03-02T07:00:00Z,2001-03-02T15:45:00Z,,
 2001-03-05T00:00:00Z,2001-03-05T07:00:00Z,2001-03-05T15:45:00Z,,
 2001-03-06T00:00:00Z,2001-03-06T07:00:00Z,2001-03-06T15:45:00Z,,
 2001-03-07T00:00:00Z,2001-03-07T07:00:00Z,2001-03-07T15:45:00Z,,
 2001-03-09T00:00:00Z,2001-03-09T07:00:00Z,2001-03-09T15:45:00Z,,
+2001-03-11T00:00:00Z,2001-03-11T07:00:00Z,2001-03-11T15:45:00Z,,
 2001-03-12T00:00:00Z,2001-03-12T07:00:00Z,2001-03-12T15:45:00Z,,
 2001-03-13T00:00:00Z,2001-03-13T07:00:00Z,2001-03-13T15:45:00Z,,
 2001-03-14T00:00:00Z,2001-03-14T07:00:00Z,2001-03-14T15:45:00Z,,
 2001-03-15T00:00:00Z,2001-03-15T07:00:00Z,2001-03-15T15:45:00Z,,
 2001-03-16T00:00:00Z,2001-03-16T07:00:00Z,2001-03-16T15:45:00Z,,
 2001-03-19T00:00:00Z,2001-03-19T07:00:00Z,2001-03-19T15:45:00Z,,
 2001-03-20T00:00:00Z,2001-03-20T07:00:00Z,2001-03-20T15:45:00Z,,
@@ -2852,14 +2857,15 @@
 2001-04-19T00:00:00Z,2001-04-19T06:00:00Z,2001-04-19T14:45:00Z,,
 2001-04-20T00:00:00Z,2001-04-20T06:00:00Z,2001-04-20T14:45:00Z,,
 2001-04-23T00:00:00Z,2001-04-23T06:00:00Z,2001-04-23T14:45:00Z,,
 2001-04-24T00:00:00Z,2001-04-24T06:00:00Z,2001-04-24T14:45:00Z,,
 2001-04-25T00:00:00Z,2001-04-25T06:00:00Z,2001-04-25T14:45:00Z,,
 2001-04-26T00:00:00Z,2001-04-26T06:00:00Z,2001-04-26T14:45:00Z,,
 2001-04-27T00:00:00Z,2001-04-27T06:00:00Z,2001-04-27T14:45:00Z,,
+2001-04-28T00:00:00Z,2001-04-28T06:00:00Z,2001-04-28T14:45:00Z,,
 2001-04-30T00:00:00Z,2001-04-30T06:00:00Z,2001-04-30T14:45:00Z,,
 2001-05-02T00:00:00Z,2001-05-02T06:00:00Z,2001-05-02T14:45:00Z,,
 2001-05-03T00:00:00Z,2001-05-03T06:00:00Z,2001-05-03T14:45:00Z,,
 2001-05-04T00:00:00Z,2001-05-04T06:00:00Z,2001-05-04T14:45:00Z,,
 2001-05-07T00:00:00Z,2001-05-07T06:00:00Z,2001-05-07T14:45:00Z,,
 2001-05-08T00:00:00Z,2001-05-08T06:00:00Z,2001-05-08T14:45:00Z,,
 2001-05-10T00:00:00Z,2001-05-10T06:00:00Z,2001-05-10T14:45:00Z,,
@@ -2880,14 +2886,15 @@
 2001-05-31T00:00:00Z,2001-05-31T06:00:00Z,2001-05-31T14:45:00Z,,
 2001-06-01T00:00:00Z,2001-06-01T06:00:00Z,2001-06-01T14:45:00Z,,
 2001-06-04T00:00:00Z,2001-06-04T06:00:00Z,2001-06-04T14:45:00Z,,
 2001-06-05T00:00:00Z,2001-06-05T06:00:00Z,2001-06-05T14:45:00Z,,
 2001-06-06T00:00:00Z,2001-06-06T06:00:00Z,2001-06-06T14:45:00Z,,
 2001-06-07T00:00:00Z,2001-06-07T06:00:00Z,2001-06-07T14:45:00Z,,
 2001-06-08T00:00:00Z,2001-06-08T06:00:00Z,2001-06-08T14:45:00Z,,
+2001-06-09T00:00:00Z,2001-06-09T06:00:00Z,2001-06-09T14:45:00Z,,
 2001-06-11T00:00:00Z,2001-06-11T06:00:00Z,2001-06-11T14:45:00Z,,
 2001-06-13T00:00:00Z,2001-06-13T06:00:00Z,2001-06-13T14:45:00Z,,
 2001-06-14T00:00:00Z,2001-06-14T06:00:00Z,2001-06-14T14:45:00Z,,
 2001-06-15T00:00:00Z,2001-06-15T06:00:00Z,2001-06-15T14:45:00Z,,
 2001-06-18T00:00:00Z,2001-06-18T06:00:00Z,2001-06-18T14:45:00Z,,
 2001-06-19T00:00:00Z,2001-06-19T06:00:00Z,2001-06-19T14:45:00Z,,
 2001-06-20T00:00:00Z,2001-06-20T06:00:00Z,2001-06-20T14:45:00Z,,
@@ -3024,14 +3031,15 @@
 2001-12-20T00:00:00Z,2001-12-20T07:00:00Z,2001-12-20T15:45:00Z,,
 2001-12-21T00:00:00Z,2001-12-21T07:00:00Z,2001-12-21T15:45:00Z,,
 2001-12-24T00:00:00Z,2001-12-24T07:00:00Z,2001-12-24T15:45:00Z,,
 2001-12-25T00:00:00Z,2001-12-25T07:00:00Z,2001-12-25T15:45:00Z,,
 2001-12-26T00:00:00Z,2001-12-26T07:00:00Z,2001-12-26T15:45:00Z,,
 2001-12-27T00:00:00Z,2001-12-27T07:00:00Z,2001-12-27T15:45:00Z,,
 2001-12-28T00:00:00Z,2001-12-28T07:00:00Z,2001-12-28T15:45:00Z,,
+2001-12-29T00:00:00Z,2001-12-29T07:00:00Z,2001-12-29T15:45:00Z,,
 2002-01-03T00:00:00Z,2002-01-03T07:00:00Z,2002-01-03T15:45:00Z,,
 2002-01-04T00:00:00Z,2002-01-04T07:00:00Z,2002-01-04T15:45:00Z,,
 2002-01-08T00:00:00Z,2002-01-08T07:00:00Z,2002-01-08T15:45:00Z,,
 2002-01-09T00:00:00Z,2002-01-09T07:00:00Z,2002-01-09T15:45:00Z,,
 2002-01-10T00:00:00Z,2002-01-10T07:00:00Z,2002-01-10T15:45:00Z,,
 2002-01-11T00:00:00Z,2002-01-11T07:00:00Z,2002-01-11T15:45:00Z,,
 2002-01-14T00:00:00Z,2002-01-14T07:00:00Z,2002-01-14T15:45:00Z,,
@@ -3103,24 +3111,26 @@
 2002-04-18T00:00:00Z,2002-04-18T06:00:00Z,2002-04-18T14:45:00Z,,
 2002-04-19T00:00:00Z,2002-04-19T06:00:00Z,2002-04-19T14:45:00Z,,
 2002-04-22T00:00:00Z,2002-04-22T06:00:00Z,2002-04-22T14:45:00Z,,
 2002-04-23T00:00:00Z,2002-04-23T06:00:00Z,2002-04-23T14:45:00Z,,
 2002-04-24T00:00:00Z,2002-04-24T06:00:00Z,2002-04-24T14:45:00Z,,
 2002-04-25T00:00:00Z,2002-04-25T06:00:00Z,2002-04-25T14:45:00Z,,
 2002-04-26T00:00:00Z,2002-04-26T06:00:00Z,2002-04-26T14:45:00Z,,
+2002-04-27T00:00:00Z,2002-04-27T06:00:00Z,2002-04-27T14:45:00Z,,
 2002-04-29T00:00:00Z,2002-04-29T06:00:00Z,2002-04-29T14:45:00Z,,
 2002-04-30T00:00:00Z,2002-04-30T06:00:00Z,2002-04-30T14:45:00Z,,
 2002-05-06T00:00:00Z,2002-05-06T06:00:00Z,2002-05-06T14:45:00Z,,
 2002-05-07T00:00:00Z,2002-05-07T06:00:00Z,2002-05-07T14:45:00Z,,
 2002-05-08T00:00:00Z,2002-05-08T06:00:00Z,2002-05-08T14:45:00Z,,
 2002-05-13T00:00:00Z,2002-05-13T06:00:00Z,2002-05-13T14:45:00Z,,
 2002-05-14T00:00:00Z,2002-05-14T06:00:00Z,2002-05-14T14:45:00Z,,
 2002-05-15T00:00:00Z,2002-05-15T06:00:00Z,2002-05-15T14:45:00Z,,
 2002-05-16T00:00:00Z,2002-05-16T06:00:00Z,2002-05-16T14:45:00Z,,
 2002-05-17T00:00:00Z,2002-05-17T06:00:00Z,2002-05-17T14:45:00Z,,
+2002-05-18T00:00:00Z,2002-05-18T06:00:00Z,2002-05-18T14:45:00Z,,
 2002-05-20T00:00:00Z,2002-05-20T06:00:00Z,2002-05-20T14:45:00Z,,
 2002-05-21T00:00:00Z,2002-05-21T06:00:00Z,2002-05-21T14:45:00Z,,
 2002-05-22T00:00:00Z,2002-05-22T06:00:00Z,2002-05-22T14:45:00Z,,
 2002-05-23T00:00:00Z,2002-05-23T06:00:00Z,2002-05-23T14:45:00Z,,
 2002-05-24T00:00:00Z,2002-05-24T06:00:00Z,2002-05-24T14:45:00Z,,
 2002-05-27T00:00:00Z,2002-05-27T06:00:00Z,2002-05-27T14:45:00Z,,
 2002-05-28T00:00:00Z,2002-05-28T06:00:00Z,2002-05-28T14:45:00Z,,
@@ -3235,14 +3245,15 @@
 2002-10-29T00:00:00Z,2002-10-29T07:00:00Z,2002-10-29T15:45:00Z,,
 2002-10-30T00:00:00Z,2002-10-30T07:00:00Z,2002-10-30T15:45:00Z,,
 2002-10-31T00:00:00Z,2002-10-31T07:00:00Z,2002-10-31T15:45:00Z,,
 2002-11-01T00:00:00Z,2002-11-01T07:00:00Z,2002-11-01T15:45:00Z,,
 2002-11-04T00:00:00Z,2002-11-04T07:00:00Z,2002-11-04T15:45:00Z,,
 2002-11-05T00:00:00Z,2002-11-05T07:00:00Z,2002-11-05T15:45:00Z,,
 2002-11-06T00:00:00Z,2002-11-06T07:00:00Z,2002-11-06T15:45:00Z,,
+2002-11-10T00:00:00Z,2002-11-10T07:00:00Z,2002-11-10T15:45:00Z,,
 2002-11-11T00:00:00Z,2002-11-11T07:00:00Z,2002-11-11T15:45:00Z,,
 2002-11-12T00:00:00Z,2002-11-12T07:00:00Z,2002-11-12T15:45:00Z,,
 2002-11-13T00:00:00Z,2002-11-13T07:00:00Z,2002-11-13T15:45:00Z,,
 2002-11-14T00:00:00Z,2002-11-14T07:00:00Z,2002-11-14T15:45:00Z,,
 2002-11-15T00:00:00Z,2002-11-15T07:00:00Z,2002-11-15T15:45:00Z,,
 2002-11-18T00:00:00Z,2002-11-18T07:00:00Z,2002-11-18T15:45:00Z,,
 2002-11-19T00:00:00Z,2002-11-19T07:00:00Z,2002-11-19T15:45:00Z,,
@@ -3258,25 +3269,28 @@
 2002-12-03T00:00:00Z,2002-12-03T07:00:00Z,2002-12-03T15:45:00Z,,
 2002-12-04T00:00:00Z,2002-12-04T07:00:00Z,2002-12-04T15:45:00Z,,
 2002-12-05T00:00:00Z,2002-12-05T07:00:00Z,2002-12-05T15:45:00Z,,
 2002-12-06T00:00:00Z,2002-12-06T07:00:00Z,2002-12-06T15:45:00Z,,
 2002-12-09T00:00:00Z,2002-12-09T07:00:00Z,2002-12-09T15:45:00Z,,
 2002-12-10T00:00:00Z,2002-12-10T07:00:00Z,2002-12-10T15:45:00Z,,
 2002-12-11T00:00:00Z,2002-12-11T07:00:00Z,2002-12-11T15:45:00Z,,
+2002-12-15T00:00:00Z,2002-12-15T07:00:00Z,2002-12-15T15:45:00Z,,
 2002-12-16T00:00:00Z,2002-12-16T07:00:00Z,2002-12-16T15:45:00Z,,
 2002-12-17T00:00:00Z,2002-12-17T07:00:00Z,2002-12-17T15:45:00Z,,
 2002-12-18T00:00:00Z,2002-12-18T07:00:00Z,2002-12-18T15:45:00Z,,
 2002-12-19T00:00:00Z,2002-12-19T07:00:00Z,2002-12-19T15:45:00Z,,
 2002-12-20T00:00:00Z,2002-12-20T07:00:00Z,2002-12-20T15:45:00Z,,
 2002-12-23T00:00:00Z,2002-12-23T07:00:00Z,2002-12-23T15:45:00Z,,
 2002-12-24T00:00:00Z,2002-12-24T07:00:00Z,2002-12-24T15:45:00Z,,
 2002-12-25T00:00:00Z,2002-12-25T07:00:00Z,2002-12-25T15:45:00Z,,
 2002-12-26T00:00:00Z,2002-12-26T07:00:00Z,2002-12-26T15:45:00Z,,
 2002-12-27T00:00:00Z,2002-12-27T07:00:00Z,2002-12-27T15:45:00Z,,
 2002-12-30T00:00:00Z,2002-12-30T07:00:00Z,2002-12-30T15:45:00Z,,
+2003-01-04T00:00:00Z,2003-01-04T07:00:00Z,2003-01-04T15:45:00Z,,
+2003-01-05T00:00:00Z,2003-01-05T07:00:00Z,2003-01-05T15:45:00Z,,
 2003-01-08T00:00:00Z,2003-01-08T07:00:00Z,2003-01-08T15:45:00Z,,
 2003-01-09T00:00:00Z,2003-01-09T07:00:00Z,2003-01-09T15:45:00Z,,
 2003-01-10T00:00:00Z,2003-01-10T07:00:00Z,2003-01-10T15:45:00Z,,
 2003-01-13T00:00:00Z,2003-01-13T07:00:00Z,2003-01-13T15:45:00Z,,
 2003-01-14T00:00:00Z,2003-01-14T07:00:00Z,2003-01-14T15:45:00Z,,
 2003-01-15T00:00:00Z,2003-01-15T07:00:00Z,2003-01-15T15:45:00Z,,
 2003-01-16T00:00:00Z,2003-01-16T07:00:00Z,2003-01-16T15:45:00Z,,
@@ -3380,14 +3394,15 @@
 2003-06-10T00:00:00Z,2003-06-10T06:00:00Z,2003-06-10T14:45:00Z,,
 2003-06-11T00:00:00Z,2003-06-11T06:00:00Z,2003-06-11T14:45:00Z,,
 2003-06-16T00:00:00Z,2003-06-16T06:00:00Z,2003-06-16T14:45:00Z,,
 2003-06-17T00:00:00Z,2003-06-17T06:00:00Z,2003-06-17T14:45:00Z,,
 2003-06-18T00:00:00Z,2003-06-18T06:00:00Z,2003-06-18T14:45:00Z,,
 2003-06-19T00:00:00Z,2003-06-19T06:00:00Z,2003-06-19T14:45:00Z,,
 2003-06-20T00:00:00Z,2003-06-20T06:00:00Z,2003-06-20T14:45:00Z,,
+2003-06-21T00:00:00Z,2003-06-21T06:00:00Z,2003-06-21T14:45:00Z,,
 2003-06-23T00:00:00Z,2003-06-23T06:00:00Z,2003-06-23T14:45:00Z,,
 2003-06-24T00:00:00Z,2003-06-24T06:00:00Z,2003-06-24T14:45:00Z,,
 2003-06-25T00:00:00Z,2003-06-25T06:00:00Z,2003-06-25T14:45:00Z,,
 2003-06-26T00:00:00Z,2003-06-26T06:00:00Z,2003-06-26T14:45:00Z,,
 2003-06-27T00:00:00Z,2003-06-27T06:00:00Z,2003-06-27T14:45:00Z,,
 2003-06-30T00:00:00Z,2003-06-30T06:00:00Z,2003-06-30T14:45:00Z,,
 2003-07-01T00:00:00Z,2003-07-01T06:00:00Z,2003-07-01T14:45:00Z,,
@@ -3803,14 +3818,15 @@
 2005-02-24T00:00:00Z,2005-02-24T07:00:00Z,2005-02-24T15:45:00Z,,
 2005-02-25T00:00:00Z,2005-02-25T07:00:00Z,2005-02-25T15:45:00Z,,
 2005-02-28T00:00:00Z,2005-02-28T07:00:00Z,2005-02-28T15:45:00Z,,
 2005-03-01T00:00:00Z,2005-03-01T07:00:00Z,2005-03-01T15:45:00Z,,
 2005-03-02T00:00:00Z,2005-03-02T07:00:00Z,2005-03-02T15:45:00Z,,
 2005-03-03T00:00:00Z,2005-03-03T07:00:00Z,2005-03-03T15:45:00Z,,
 2005-03-04T00:00:00Z,2005-03-04T07:00:00Z,2005-03-04T15:45:00Z,,
+2005-03-05T00:00:00Z,2005-03-05T07:00:00Z,2005-03-05T15:45:00Z,,
 2005-03-09T00:00:00Z,2005-03-09T07:00:00Z,2005-03-09T15:45:00Z,,
 2005-03-10T00:00:00Z,2005-03-10T07:00:00Z,2005-03-10T15:45:00Z,,
 2005-03-11T00:00:00Z,2005-03-11T07:00:00Z,2005-03-11T15:45:00Z,,
 2005-03-14T00:00:00Z,2005-03-14T07:00:00Z,2005-03-14T15:45:00Z,,
 2005-03-15T00:00:00Z,2005-03-15T07:00:00Z,2005-03-15T15:45:00Z,,
 2005-03-16T00:00:00Z,2005-03-16T07:00:00Z,2005-03-16T15:45:00Z,,
 2005-03-17T00:00:00Z,2005-03-17T07:00:00Z,2005-03-17T15:45:00Z,,
@@ -3848,14 +3864,15 @@
 2005-05-03T00:00:00Z,2005-05-03T06:00:00Z,2005-05-03T14:45:00Z,,
 2005-05-04T00:00:00Z,2005-05-04T06:00:00Z,2005-05-04T14:45:00Z,,
 2005-05-05T00:00:00Z,2005-05-05T06:00:00Z,2005-05-05T14:45:00Z,,
 2005-05-06T00:00:00Z,2005-05-06T06:00:00Z,2005-05-06T14:45:00Z,,
 2005-05-11T00:00:00Z,2005-05-11T06:00:00Z,2005-05-11T14:45:00Z,,
 2005-05-12T00:00:00Z,2005-05-12T06:00:00Z,2005-05-12T14:45:00Z,,
 2005-05-13T00:00:00Z,2005-05-13T06:00:00Z,2005-05-13T14:45:00Z,,
+2005-05-14T00:00:00Z,2005-05-14T06:00:00Z,2005-05-14T14:45:00Z,,
 2005-05-16T00:00:00Z,2005-05-16T06:00:00Z,2005-05-16T14:45:00Z,,
 2005-05-17T00:00:00Z,2005-05-17T06:00:00Z,2005-05-17T14:45:00Z,,
 2005-05-18T00:00:00Z,2005-05-18T06:00:00Z,2005-05-18T14:45:00Z,,
 2005-05-19T00:00:00Z,2005-05-19T06:00:00Z,2005-05-19T14:45:00Z,,
 2005-05-20T00:00:00Z,2005-05-20T06:00:00Z,2005-05-20T14:45:00Z,,
 2005-05-23T00:00:00Z,2005-05-23T06:00:00Z,2005-05-23T14:45:00Z,,
 2005-05-24T00:00:00Z,2005-05-24T06:00:00Z,2005-05-24T14:45:00Z,,
@@ -4043,14 +4060,15 @@
 2006-02-14T00:00:00Z,2006-02-14T07:00:00Z,2006-02-14T15:45:00Z,,
 2006-02-15T00:00:00Z,2006-02-15T07:00:00Z,2006-02-15T15:45:00Z,,
 2006-02-16T00:00:00Z,2006-02-16T07:00:00Z,2006-02-16T15:45:00Z,,
 2006-02-17T00:00:00Z,2006-02-17T07:00:00Z,2006-02-17T15:45:00Z,,
 2006-02-20T00:00:00Z,2006-02-20T07:00:00Z,2006-02-20T15:45:00Z,,
 2006-02-21T00:00:00Z,2006-02-21T07:00:00Z,2006-02-21T15:45:00Z,,
 2006-02-22T00:00:00Z,2006-02-22T07:00:00Z,2006-02-22T15:45:00Z,,
+2006-02-26T00:00:00Z,2006-02-26T07:00:00Z,2006-02-26T15:45:00Z,,
 2006-02-27T00:00:00Z,2006-02-27T07:00:00Z,2006-02-27T15:45:00Z,,
 2006-02-28T00:00:00Z,2006-02-28T07:00:00Z,2006-02-28T15:45:00Z,,
 2006-03-01T00:00:00Z,2006-03-01T07:00:00Z,2006-03-01T15:45:00Z,,
 2006-03-02T00:00:00Z,2006-03-02T07:00:00Z,2006-03-02T15:45:00Z,,
 2006-03-03T00:00:00Z,2006-03-03T07:00:00Z,2006-03-03T15:45:00Z,,
 2006-03-06T00:00:00Z,2006-03-06T07:00:00Z,2006-03-06T15:45:00Z,,
 2006-03-07T00:00:00Z,2006-03-07T07:00:00Z,2006-03-07T15:45:00Z,,
@@ -4091,14 +4109,15 @@
 2006-04-26T00:00:00Z,2006-04-26T06:00:00Z,2006-04-26T14:45:00Z,,
 2006-04-27T00:00:00Z,2006-04-27T06:00:00Z,2006-04-27T14:45:00Z,,
 2006-04-28T00:00:00Z,2006-04-28T06:00:00Z,2006-04-28T14:45:00Z,,
 2006-05-02T00:00:00Z,2006-05-02T06:00:00Z,2006-05-02T14:45:00Z,,
 2006-05-03T00:00:00Z,2006-05-03T06:00:00Z,2006-05-03T14:45:00Z,,
 2006-05-04T00:00:00Z,2006-05-04T06:00:00Z,2006-05-04T14:45:00Z,,
 2006-05-05T00:00:00Z,2006-05-05T06:00:00Z,2006-05-05T14:45:00Z,,
+2006-05-06T00:00:00Z,2006-05-06T06:00:00Z,2006-05-06T14:45:00Z,,
 2006-05-10T00:00:00Z,2006-05-10T06:00:00Z,2006-05-10T14:45:00Z,,
 2006-05-11T00:00:00Z,2006-05-11T06:00:00Z,2006-05-11T14:45:00Z,,
 2006-05-12T00:00:00Z,2006-05-12T06:00:00Z,2006-05-12T14:45:00Z,,
 2006-05-15T00:00:00Z,2006-05-15T06:00:00Z,2006-05-15T14:45:00Z,,
 2006-05-16T00:00:00Z,2006-05-16T06:00:00Z,2006-05-16T14:45:00Z,,
 2006-05-17T00:00:00Z,2006-05-17T06:00:00Z,2006-05-17T14:45:00Z,,
 2006-05-18T00:00:00Z,2006-05-18T06:00:00Z,2006-05-18T14:45:00Z,,
@@ -4334,14 +4353,15 @@
 2007-04-19T00:00:00Z,2007-04-19T06:00:00Z,2007-04-19T14:45:00Z,,
 2007-04-20T00:00:00Z,2007-04-20T06:00:00Z,2007-04-20T14:45:00Z,,
 2007-04-23T00:00:00Z,2007-04-23T06:00:00Z,2007-04-23T14:45:00Z,,
 2007-04-24T00:00:00Z,2007-04-24T06:00:00Z,2007-04-24T14:45:00Z,,
 2007-04-25T00:00:00Z,2007-04-25T06:00:00Z,2007-04-25T14:45:00Z,,
 2007-04-26T00:00:00Z,2007-04-26T06:00:00Z,2007-04-26T14:45:00Z,,
 2007-04-27T00:00:00Z,2007-04-27T06:00:00Z,2007-04-27T14:45:00Z,,
+2007-04-28T00:00:00Z,2007-04-28T06:00:00Z,2007-04-28T14:45:00Z,,
 2007-05-02T00:00:00Z,2007-05-02T06:00:00Z,2007-05-02T14:45:00Z,,
 2007-05-03T00:00:00Z,2007-05-03T06:00:00Z,2007-05-03T14:45:00Z,,
 2007-05-04T00:00:00Z,2007-05-04T06:00:00Z,2007-05-04T14:45:00Z,,
 2007-05-07T00:00:00Z,2007-05-07T06:00:00Z,2007-05-07T14:45:00Z,,
 2007-05-08T00:00:00Z,2007-05-08T06:00:00Z,2007-05-08T14:45:00Z,,
 2007-05-10T00:00:00Z,2007-05-10T06:00:00Z,2007-05-10T14:45:00Z,,
 2007-05-11T00:00:00Z,2007-05-11T06:00:00Z,2007-05-11T14:45:00Z,,
@@ -4361,14 +4381,15 @@
 2007-05-31T00:00:00Z,2007-05-31T06:00:00Z,2007-05-31T14:45:00Z,,
 2007-06-01T00:00:00Z,2007-06-01T06:00:00Z,2007-06-01T14:45:00Z,,
 2007-06-04T00:00:00Z,2007-06-04T06:00:00Z,2007-06-04T14:45:00Z,,
 2007-06-05T00:00:00Z,2007-06-05T06:00:00Z,2007-06-05T14:45:00Z,,
 2007-06-06T00:00:00Z,2007-06-06T06:00:00Z,2007-06-06T14:45:00Z,,
 2007-06-07T00:00:00Z,2007-06-07T06:00:00Z,2007-06-07T14:45:00Z,,
 2007-06-08T00:00:00Z,2007-06-08T06:00:00Z,2007-06-08T14:45:00Z,,
+2007-06-09T00:00:00Z,2007-06-09T06:00:00Z,2007-06-09T14:45:00Z,,
 2007-06-13T00:00:00Z,2007-06-13T06:00:00Z,2007-06-13T14:45:00Z,,
 2007-06-14T00:00:00Z,2007-06-14T06:00:00Z,2007-06-14T14:45:00Z,,
 2007-06-15T00:00:00Z,2007-06-15T06:00:00Z,2007-06-15T14:45:00Z,,
 2007-06-18T00:00:00Z,2007-06-18T06:00:00Z,2007-06-18T14:45:00Z,,
 2007-06-19T00:00:00Z,2007-06-19T06:00:00Z,2007-06-19T14:45:00Z,,
 2007-06-20T00:00:00Z,2007-06-20T06:00:00Z,2007-06-20T14:45:00Z,,
 2007-06-21T00:00:00Z,2007-06-21T06:00:00Z,2007-06-21T14:45:00Z,,
@@ -4582,14 +4603,15 @@
 2008-04-22T00:00:00Z,2008-04-22T06:00:00Z,2008-04-22T14:45:00Z,,
 2008-04-23T00:00:00Z,2008-04-23T06:00:00Z,2008-04-23T14:45:00Z,,
 2008-04-24T00:00:00Z,2008-04-24T06:00:00Z,2008-04-24T14:45:00Z,,
 2008-04-25T00:00:00Z,2008-04-25T06:00:00Z,2008-04-25T14:45:00Z,,
 2008-04-28T00:00:00Z,2008-04-28T06:00:00Z,2008-04-28T14:45:00Z,,
 2008-04-29T00:00:00Z,2008-04-29T06:00:00Z,2008-04-29T14:45:00Z,,
 2008-04-30T00:00:00Z,2008-04-30T06:00:00Z,2008-04-30T14:45:00Z,,
+2008-05-04T00:00:00Z,2008-05-04T06:00:00Z,2008-05-04T14:45:00Z,,
 2008-05-05T00:00:00Z,2008-05-05T06:00:00Z,2008-05-05T14:45:00Z,,
 2008-05-06T00:00:00Z,2008-05-06T06:00:00Z,2008-05-06T14:45:00Z,,
 2008-05-07T00:00:00Z,2008-05-07T06:00:00Z,2008-05-07T14:45:00Z,,
 2008-05-08T00:00:00Z,2008-05-08T06:00:00Z,2008-05-08T14:45:00Z,,
 2008-05-12T00:00:00Z,2008-05-12T06:00:00Z,2008-05-12T14:45:00Z,,
 2008-05-13T00:00:00Z,2008-05-13T06:00:00Z,2008-05-13T14:45:00Z,,
 2008-05-14T00:00:00Z,2008-05-14T06:00:00Z,2008-05-14T14:45:00Z,,
@@ -4606,14 +4628,15 @@
 2008-05-29T00:00:00Z,2008-05-29T06:00:00Z,2008-05-29T14:45:00Z,,
 2008-05-30T00:00:00Z,2008-05-30T06:00:00Z,2008-05-30T14:45:00Z,,
 2008-06-02T00:00:00Z,2008-06-02T06:00:00Z,2008-06-02T14:45:00Z,,
 2008-06-03T00:00:00Z,2008-06-03T06:00:00Z,2008-06-03T14:45:00Z,,
 2008-06-04T00:00:00Z,2008-06-04T06:00:00Z,2008-06-04T14:45:00Z,,
 2008-06-05T00:00:00Z,2008-06-05T06:00:00Z,2008-06-05T14:45:00Z,,
 2008-06-06T00:00:00Z,2008-06-06T06:00:00Z,2008-06-06T14:45:00Z,,
+2008-06-07T00:00:00Z,2008-06-07T06:00:00Z,2008-06-07T14:45:00Z,,
 2008-06-09T00:00:00Z,2008-06-09T06:00:00Z,2008-06-09T14:45:00Z,,
 2008-06-10T00:00:00Z,2008-06-10T06:00:00Z,2008-06-10T14:45:00Z,,
 2008-06-11T00:00:00Z,2008-06-11T06:00:00Z,2008-06-11T14:45:00Z,,
 2008-06-16T00:00:00Z,2008-06-16T06:00:00Z,2008-06-16T14:45:00Z,,
 2008-06-17T00:00:00Z,2008-06-17T06:00:00Z,2008-06-17T14:45:00Z,,
 2008-06-18T00:00:00Z,2008-06-18T06:00:00Z,2008-06-18T14:45:00Z,,
 2008-06-19T00:00:00Z,2008-06-19T06:00:00Z,2008-06-19T14:45:00Z,,
@@ -4706,14 +4729,15 @@
 2008-10-22T00:00:00Z,2008-10-22T06:00:00Z,2008-10-22T14:45:00Z,,
 2008-10-23T00:00:00Z,2008-10-23T06:00:00Z,2008-10-23T14:45:00Z,,
 2008-10-24T00:00:00Z,2008-10-24T06:00:00Z,2008-10-24T14:45:00Z,,
 2008-10-28T00:00:00Z,2008-10-28T07:00:00Z,2008-10-28T15:45:00Z,,
 2008-10-29T00:00:00Z,2008-10-29T07:00:00Z,2008-10-29T15:45:00Z,,
 2008-10-30T00:00:00Z,2008-10-30T07:00:00Z,2008-10-30T15:45:00Z,,
 2008-10-31T00:00:00Z,2008-10-31T07:00:00Z,2008-10-31T15:45:00Z,,
+2008-11-01T00:00:00Z,2008-11-01T07:00:00Z,2008-11-01T15:45:00Z,,
 2008-11-05T00:00:00Z,2008-11-05T07:00:00Z,2008-11-05T15:45:00Z,,
 2008-11-06T00:00:00Z,2008-11-06T07:00:00Z,2008-11-06T15:45:00Z,,
 2008-11-07T00:00:00Z,2008-11-07T07:00:00Z,2008-11-07T15:45:00Z,,
 2008-11-10T00:00:00Z,2008-11-10T07:00:00Z,2008-11-10T15:45:00Z,,
 2008-11-11T00:00:00Z,2008-11-11T07:00:00Z,2008-11-11T15:45:00Z,,
 2008-11-12T00:00:00Z,2008-11-12T07:00:00Z,2008-11-12T15:45:00Z,,
 2008-11-13T00:00:00Z,2008-11-13T07:00:00Z,2008-11-13T15:45:00Z,,
@@ -5028,14 +5052,15 @@
 2010-02-16T00:00:00Z,2010-02-16T07:00:00Z,2010-02-16T15:45:00Z,,
 2010-02-17T00:00:00Z,2010-02-17T07:00:00Z,2010-02-17T15:45:00Z,,
 2010-02-18T00:00:00Z,2010-02-18T07:00:00Z,2010-02-18T15:45:00Z,,
 2010-02-19T00:00:00Z,2010-02-19T07:00:00Z,2010-02-19T15:45:00Z,,
 2010-02-24T00:00:00Z,2010-02-24T07:00:00Z,2010-02-24T15:45:00Z,,
 2010-02-25T00:00:00Z,2010-02-25T07:00:00Z,2010-02-25T15:45:00Z,,
 2010-02-26T00:00:00Z,2010-02-26T07:00:00Z,2010-02-26T15:45:00Z,,
+2010-02-27T00:00:00Z,2010-02-27T07:00:00Z,2010-02-27T15:45:00Z,,
 2010-03-01T00:00:00Z,2010-03-01T07:00:00Z,2010-03-01T15:45:00Z,,
 2010-03-02T00:00:00Z,2010-03-02T07:00:00Z,2010-03-02T15:45:00Z,,
 2010-03-03T00:00:00Z,2010-03-03T07:00:00Z,2010-03-03T15:45:00Z,,
 2010-03-04T00:00:00Z,2010-03-04T07:00:00Z,2010-03-04T15:45:00Z,,
 2010-03-05T00:00:00Z,2010-03-05T07:00:00Z,2010-03-05T15:45:00Z,,
 2010-03-09T00:00:00Z,2010-03-09T07:00:00Z,2010-03-09T15:45:00Z,,
 2010-03-10T00:00:00Z,2010-03-10T07:00:00Z,2010-03-10T15:45:00Z,,
@@ -5207,14 +5232,15 @@
 2010-11-02T00:00:00Z,2010-11-02T07:00:00Z,2010-11-02T15:45:00Z,,
 2010-11-03T00:00:00Z,2010-11-03T07:00:00Z,2010-11-03T15:45:00Z,,
 2010-11-08T00:00:00Z,2010-11-08T07:00:00Z,2010-11-08T15:45:00Z,,
 2010-11-09T00:00:00Z,2010-11-09T07:00:00Z,2010-11-09T15:45:00Z,,
 2010-11-10T00:00:00Z,2010-11-10T07:00:00Z,2010-11-10T15:45:00Z,,
 2010-11-11T00:00:00Z,2010-11-11T07:00:00Z,2010-11-11T15:45:00Z,,
 2010-11-12T00:00:00Z,2010-11-12T07:00:00Z,2010-11-12T15:45:00Z,,
+2010-11-13T00:00:00Z,2010-11-13T07:00:00Z,2010-11-13T15:45:00Z,,
 2010-11-15T00:00:00Z,2010-11-15T07:00:00Z,2010-11-15T15:45:00Z,,
 2010-11-16T00:00:00Z,2010-11-16T07:00:00Z,2010-11-16T15:45:00Z,,
 2010-11-17T00:00:00Z,2010-11-17T07:00:00Z,2010-11-17T15:45:00Z,,
 2010-11-18T00:00:00Z,2010-11-18T07:00:00Z,2010-11-18T15:45:00Z,,
 2010-11-19T00:00:00Z,2010-11-19T07:00:00Z,2010-11-19T15:45:00Z,,
 2010-11-22T00:00:00Z,2010-11-22T07:00:00Z,2010-11-22T15:45:00Z,,
 2010-11-23T00:00:00Z,2010-11-23T07:00:00Z,2010-11-23T15:45:00Z,,
@@ -5279,14 +5305,15 @@
 2011-02-24T00:00:00Z,2011-02-24T07:00:00Z,2011-02-24T15:45:00Z,,
 2011-02-25T00:00:00Z,2011-02-25T07:00:00Z,2011-02-25T15:45:00Z,,
 2011-02-28T00:00:00Z,2011-02-28T07:00:00Z,2011-02-28T15:45:00Z,,
 2011-03-01T00:00:00Z,2011-03-01T07:00:00Z,2011-03-01T15:45:00Z,,
 2011-03-02T00:00:00Z,2011-03-02T07:00:00Z,2011-03-02T15:45:00Z,,
 2011-03-03T00:00:00Z,2011-03-03T07:00:00Z,2011-03-03T15:45:00Z,,
 2011-03-04T00:00:00Z,2011-03-04T07:00:00Z,2011-03-04T15:45:00Z,,
+2011-03-05T00:00:00Z,2011-03-05T07:00:00Z,2011-03-05T15:45:00Z,,
 2011-03-09T00:00:00Z,2011-03-09T07:00:00Z,2011-03-09T15:45:00Z,,
 2011-03-10T00:00:00Z,2011-03-10T07:00:00Z,2011-03-10T15:45:00Z,,
 2011-03-11T00:00:00Z,2011-03-11T07:00:00Z,2011-03-11T15:45:00Z,,
 2011-03-14T00:00:00Z,2011-03-14T07:00:00Z,2011-03-14T15:45:00Z,,
 2011-03-15T00:00:00Z,2011-03-15T07:00:00Z,2011-03-15T15:45:00Z,,
 2011-03-16T00:00:00Z,2011-03-16T07:00:00Z,2011-03-16T15:45:00Z,,
 2011-03-17T00:00:00Z,2011-03-17T07:00:00Z,2011-03-17T15:45:00Z,,
@@ -5534,14 +5561,15 @@
 2012-02-28T00:00:00Z,2012-02-28T06:00:00Z,2012-02-28T14:45:00Z,,
 2012-02-29T00:00:00Z,2012-02-29T06:00:00Z,2012-02-29T14:45:00Z,,
 2012-03-01T00:00:00Z,2012-03-01T06:00:00Z,2012-03-01T14:45:00Z,,
 2012-03-02T00:00:00Z,2012-03-02T06:00:00Z,2012-03-02T14:45:00Z,,
 2012-03-05T00:00:00Z,2012-03-05T06:00:00Z,2012-03-05T14:45:00Z,,
 2012-03-06T00:00:00Z,2012-03-06T06:00:00Z,2012-03-06T14:45:00Z,,
 2012-03-07T00:00:00Z,2012-03-07T06:00:00Z,2012-03-07T14:45:00Z,,
+2012-03-11T00:00:00Z,2012-03-11T06:00:00Z,2012-03-11T14:45:00Z,,
 2012-03-12T00:00:00Z,2012-03-12T06:00:00Z,2012-03-12T14:45:00Z,,
 2012-03-13T00:00:00Z,2012-03-13T06:00:00Z,2012-03-13T14:45:00Z,,
 2012-03-14T00:00:00Z,2012-03-14T06:00:00Z,2012-03-14T14:45:00Z,,
 2012-03-15T00:00:00Z,2012-03-15T06:00:00Z,2012-03-15T14:45:00Z,,
 2012-03-16T00:00:00Z,2012-03-16T06:00:00Z,2012-03-16T14:45:00Z,,
 2012-03-19T00:00:00Z,2012-03-19T06:00:00Z,2012-03-19T14:45:00Z,,
 2012-03-20T00:00:00Z,2012-03-20T06:00:00Z,2012-03-20T14:45:00Z,,
@@ -5569,21 +5597,24 @@
 2012-04-19T00:00:00Z,2012-04-19T06:00:00Z,2012-04-19T14:45:00Z,,
 2012-04-20T00:00:00Z,2012-04-20T06:00:00Z,2012-04-20T14:45:00Z,,
 2012-04-23T00:00:00Z,2012-04-23T06:00:00Z,2012-04-23T14:45:00Z,,
 2012-04-24T00:00:00Z,2012-04-24T06:00:00Z,2012-04-24T14:45:00Z,,
 2012-04-25T00:00:00Z,2012-04-25T06:00:00Z,2012-04-25T14:45:00Z,,
 2012-04-26T00:00:00Z,2012-04-26T06:00:00Z,2012-04-26T14:45:00Z,,
 2012-04-27T00:00:00Z,2012-04-27T06:00:00Z,2012-04-27T14:45:00Z,,
+2012-04-28T00:00:00Z,2012-04-28T06:00:00Z,2012-04-28T14:45:00Z,,
 2012-05-02T00:00:00Z,2012-05-02T06:00:00Z,2012-05-02T14:45:00Z,,
 2012-05-03T00:00:00Z,2012-05-03T06:00:00Z,2012-05-03T14:45:00Z,,
 2012-05-04T00:00:00Z,2012-05-04T06:00:00Z,2012-05-04T14:45:00Z,,
+2012-05-05T00:00:00Z,2012-05-05T06:00:00Z,2012-05-05T14:45:00Z,,
 2012-05-07T00:00:00Z,2012-05-07T06:00:00Z,2012-05-07T14:45:00Z,,
 2012-05-08T00:00:00Z,2012-05-08T06:00:00Z,2012-05-08T14:45:00Z,,
 2012-05-10T00:00:00Z,2012-05-10T06:00:00Z,2012-05-10T14:45:00Z,,
 2012-05-11T00:00:00Z,2012-05-11T06:00:00Z,2012-05-11T14:45:00Z,,
+2012-05-12T00:00:00Z,2012-05-12T06:00:00Z,2012-05-12T14:45:00Z,,
 2012-05-14T00:00:00Z,2012-05-14T06:00:00Z,2012-05-14T14:45:00Z,,
 2012-05-15T00:00:00Z,2012-05-15T06:00:00Z,2012-05-15T14:45:00Z,,
 2012-05-16T00:00:00Z,2012-05-16T06:00:00Z,2012-05-16T14:45:00Z,,
 2012-05-17T00:00:00Z,2012-05-17T06:00:00Z,2012-05-17T14:45:00Z,,
 2012-05-18T00:00:00Z,2012-05-18T06:00:00Z,2012-05-18T14:45:00Z,,
 2012-05-21T00:00:00Z,2012-05-21T06:00:00Z,2012-05-21T14:45:00Z,,
 2012-05-22T00:00:00Z,2012-05-22T06:00:00Z,2012-05-22T14:45:00Z,,
@@ -5596,14 +5627,15 @@
 2012-05-31T00:00:00Z,2012-05-31T06:00:00Z,2012-05-31T14:45:00Z,,
 2012-06-01T00:00:00Z,2012-06-01T06:00:00Z,2012-06-01T14:45:00Z,,
 2012-06-04T00:00:00Z,2012-06-04T06:00:00Z,2012-06-04T14:45:00Z,,
 2012-06-05T00:00:00Z,2012-06-05T06:00:00Z,2012-06-05T14:45:00Z,,
 2012-06-06T00:00:00Z,2012-06-06T06:00:00Z,2012-06-06T14:45:00Z,,
 2012-06-07T00:00:00Z,2012-06-07T06:00:00Z,2012-06-07T14:45:00Z,,
 2012-06-08T00:00:00Z,2012-06-08T06:00:00Z,2012-06-08T14:45:00Z,,
+2012-06-09T00:00:00Z,2012-06-09T06:00:00Z,2012-06-09T14:45:00Z,,
 2012-06-13T00:00:00Z,2012-06-13T06:00:00Z,2012-06-13T14:45:00Z,,
 2012-06-14T00:00:00Z,2012-06-14T06:00:00Z,2012-06-14T14:45:00Z,,
 2012-06-15T00:00:00Z,2012-06-15T06:00:00Z,2012-06-15T14:45:00Z,,
 2012-06-18T00:00:00Z,2012-06-18T06:00:00Z,2012-06-18T14:45:00Z,,
 2012-06-19T00:00:00Z,2012-06-19T06:00:00Z,2012-06-19T14:45:00Z,,
 2012-06-20T00:00:00Z,2012-06-20T06:00:00Z,2012-06-20T14:45:00Z,,
 2012-06-21T00:00:00Z,2012-06-21T06:00:00Z,2012-06-21T14:45:00Z,,
@@ -6521,14 +6553,15 @@
 2016-02-11T00:00:00Z,2016-02-11T07:00:00Z,2016-02-11T15:45:00Z,,
 2016-02-12T00:00:00Z,2016-02-12T07:00:00Z,2016-02-12T15:45:00Z,,
 2016-02-15T00:00:00Z,2016-02-15T07:00:00Z,2016-02-15T15:45:00Z,,
 2016-02-16T00:00:00Z,2016-02-16T07:00:00Z,2016-02-16T15:45:00Z,,
 2016-02-17T00:00:00Z,2016-02-17T07:00:00Z,2016-02-17T15:45:00Z,,
 2016-02-18T00:00:00Z,2016-02-18T07:00:00Z,2016-02-18T15:45:00Z,,
 2016-02-19T00:00:00Z,2016-02-19T07:00:00Z,2016-02-19T15:45:00Z,,
+2016-02-20T00:00:00Z,2016-02-20T07:00:00Z,2016-02-20T15:45:00Z,,
 2016-02-22T00:00:00Z,2016-02-22T07:00:00Z,2016-02-22T15:45:00Z,,
 2016-02-24T00:00:00Z,2016-02-24T07:00:00Z,2016-02-24T15:45:00Z,,
 2016-02-25T00:00:00Z,2016-02-25T07:00:00Z,2016-02-25T15:45:00Z,,
 2016-02-26T00:00:00Z,2016-02-26T07:00:00Z,2016-02-26T15:45:00Z,,
 2016-02-29T00:00:00Z,2016-02-29T07:00:00Z,2016-02-29T15:45:00Z,,
 2016-03-01T00:00:00Z,2016-03-01T07:00:00Z,2016-03-01T15:45:00Z,,
 2016-03-02T00:00:00Z,2016-03-02T07:00:00Z,2016-03-02T15:45:00Z,,
@@ -7071,14 +7104,15 @@
 2018-04-19T00:00:00Z,2018-04-19T07:00:00Z,2018-04-19T15:45:00Z,,
 2018-04-20T00:00:00Z,2018-04-20T07:00:00Z,2018-04-20T15:45:00Z,,
 2018-04-23T00:00:00Z,2018-04-23T07:00:00Z,2018-04-23T15:45:00Z,,
 2018-04-24T00:00:00Z,2018-04-24T07:00:00Z,2018-04-24T15:45:00Z,,
 2018-04-25T00:00:00Z,2018-04-25T07:00:00Z,2018-04-25T15:45:00Z,,
 2018-04-26T00:00:00Z,2018-04-26T07:00:00Z,2018-04-26T15:45:00Z,,
 2018-04-27T00:00:00Z,2018-04-27T07:00:00Z,2018-04-27T15:45:00Z,,
+2018-04-28T00:00:00Z,2018-04-28T07:00:00Z,2018-04-28T15:45:00Z,,
 2018-04-30T00:00:00Z,2018-04-30T07:00:00Z,2018-04-30T15:45:00Z,,
 2018-05-02T00:00:00Z,2018-05-02T07:00:00Z,2018-05-02T15:45:00Z,,
 2018-05-03T00:00:00Z,2018-05-03T07:00:00Z,2018-05-03T15:45:00Z,,
 2018-05-04T00:00:00Z,2018-05-04T07:00:00Z,2018-05-04T15:45:00Z,,
 2018-05-07T00:00:00Z,2018-05-07T07:00:00Z,2018-05-07T15:45:00Z,,
 2018-05-08T00:00:00Z,2018-05-08T07:00:00Z,2018-05-08T15:45:00Z,,
 2018-05-10T00:00:00Z,2018-05-10T07:00:00Z,2018-05-10T15:45:00Z,,
@@ -7099,14 +7133,15 @@
 2018-05-31T00:00:00Z,2018-05-31T07:00:00Z,2018-05-31T15:45:00Z,,
 2018-06-01T00:00:00Z,2018-06-01T07:00:00Z,2018-06-01T15:45:00Z,,
 2018-06-04T00:00:00Z,2018-06-04T07:00:00Z,2018-06-04T15:45:00Z,,
 2018-06-05T00:00:00Z,2018-06-05T07:00:00Z,2018-06-05T15:45:00Z,,
 2018-06-06T00:00:00Z,2018-06-06T07:00:00Z,2018-06-06T15:45:00Z,,
 2018-06-07T00:00:00Z,2018-06-07T07:00:00Z,2018-06-07T15:45:00Z,,
 2018-06-08T00:00:00Z,2018-06-08T07:00:00Z,2018-06-08T15:45:00Z,,
+2018-06-09T00:00:00Z,2018-06-09T07:00:00Z,2018-06-09T15:45:00Z,,
 2018-06-11T00:00:00Z,2018-06-11T07:00:00Z,2018-06-11T15:45:00Z,,
 2018-06-13T00:00:00Z,2018-06-13T07:00:00Z,2018-06-13T15:45:00Z,,
 2018-06-14T00:00:00Z,2018-06-14T07:00:00Z,2018-06-14T15:45:00Z,,
 2018-06-15T00:00:00Z,2018-06-15T07:00:00Z,2018-06-15T15:45:00Z,,
 2018-06-18T00:00:00Z,2018-06-18T07:00:00Z,2018-06-18T15:45:00Z,,
 2018-06-19T00:00:00Z,2018-06-19T07:00:00Z,2018-06-19T15:45:00Z,,
 2018-06-20T00:00:00Z,2018-06-20T07:00:00Z,2018-06-20T15:45:00Z,,
@@ -7242,14 +7277,15 @@
 2018-12-20T00:00:00Z,2018-12-20T07:00:00Z,2018-12-20T15:45:00Z,,
 2018-12-21T00:00:00Z,2018-12-21T07:00:00Z,2018-12-21T15:45:00Z,,
 2018-12-24T00:00:00Z,2018-12-24T07:00:00Z,2018-12-24T15:45:00Z,,
 2018-12-25T00:00:00Z,2018-12-25T07:00:00Z,2018-12-25T15:45:00Z,,
 2018-12-26T00:00:00Z,2018-12-26T07:00:00Z,2018-12-26T15:45:00Z,,
 2018-12-27T00:00:00Z,2018-12-27T07:00:00Z,2018-12-27T15:45:00Z,,
 2018-12-28T00:00:00Z,2018-12-28T07:00:00Z,2018-12-28T15:45:00Z,,
+2018-12-29T00:00:00Z,2018-12-29T07:00:00Z,2018-12-29T15:45:00Z,,
 2019-01-03T00:00:00Z,2019-01-03T07:00:00Z,2019-01-03T15:45:00Z,,
 2019-01-04T00:00:00Z,2019-01-04T07:00:00Z,2019-01-04T15:45:00Z,,
 2019-01-08T00:00:00Z,2019-01-08T07:00:00Z,2019-01-08T15:45:00Z,,
 2019-01-09T00:00:00Z,2019-01-09T07:00:00Z,2019-01-09T15:45:00Z,,
 2019-01-10T00:00:00Z,2019-01-10T07:00:00Z,2019-01-10T15:45:00Z,,
 2019-01-11T00:00:00Z,2019-01-11T07:00:00Z,2019-01-11T15:45:00Z,,
 2019-01-14T00:00:00Z,2019-01-14T07:00:00Z,2019-01-14T15:45:00Z,,
@@ -7778,14 +7814,15 @@
 2021-02-11T00:00:00Z,2021-02-11T07:00:00Z,2021-02-11T15:45:00Z,,
 2021-02-12T00:00:00Z,2021-02-12T07:00:00Z,2021-02-12T15:45:00Z,,
 2021-02-15T00:00:00Z,2021-02-15T07:00:00Z,2021-02-15T15:45:00Z,,
 2021-02-16T00:00:00Z,2021-02-16T07:00:00Z,2021-02-16T15:45:00Z,,
 2021-02-17T00:00:00Z,2021-02-17T07:00:00Z,2021-02-17T15:45:00Z,,
 2021-02-18T00:00:00Z,2021-02-18T07:00:00Z,2021-02-18T15:45:00Z,,
 2021-02-19T00:00:00Z,2021-02-19T07:00:00Z,2021-02-19T15:45:00Z,,
+2021-02-20T00:00:00Z,2021-02-20T07:00:00Z,2021-02-20T15:45:00Z,,
 2021-02-22T00:00:00Z,2021-02-22T07:00:00Z,2021-02-22T15:45:00Z,,
 2021-02-24T00:00:00Z,2021-02-24T07:00:00Z,2021-02-24T15:45:00Z,,
 2021-02-25T00:00:00Z,2021-02-25T07:00:00Z,2021-02-25T15:45:00Z,,
 2021-02-26T00:00:00Z,2021-02-26T07:00:00Z,2021-02-26T15:45:00Z,,
 2021-03-01T00:00:00Z,2021-03-01T07:00:00Z,2021-03-01T15:45:00Z,,
 2021-03-02T00:00:00Z,2021-03-02T07:00:00Z,2021-03-02T15:45:00Z,,
 2021-03-03T00:00:00Z,2021-03-03T07:00:00Z,2021-03-03T15:45:00Z,,
@@ -8583,14 +8620,15 @@
 2024-04-18T00:00:00Z,2024-04-18T07:00:00Z,2024-04-18T15:45:00Z,,
 2024-04-19T00:00:00Z,2024-04-19T07:00:00Z,2024-04-19T15:45:00Z,,
 2024-04-22T00:00:00Z,2024-04-22T07:00:00Z,2024-04-22T15:45:00Z,,
 2024-04-23T00:00:00Z,2024-04-23T07:00:00Z,2024-04-23T15:45:00Z,,
 2024-04-24T00:00:00Z,2024-04-24T07:00:00Z,2024-04-24T15:45:00Z,,
 2024-04-25T00:00:00Z,2024-04-25T07:00:00Z,2024-04-25T15:45:00Z,,
 2024-04-26T00:00:00Z,2024-04-26T07:00:00Z,2024-04-26T15:45:00Z,,
+2024-04-27T00:00:00Z,2024-04-27T07:00:00Z,2024-04-27T15:45:00Z,,
 2024-04-29T00:00:00Z,2024-04-29T07:00:00Z,2024-04-29T15:45:00Z,,
 2024-04-30T00:00:00Z,2024-04-30T07:00:00Z,2024-04-30T15:45:00Z,,
 2024-05-02T00:00:00Z,2024-05-02T07:00:00Z,2024-05-02T15:45:00Z,,
 2024-05-03T00:00:00Z,2024-05-03T07:00:00Z,2024-05-03T15:45:00Z,,
 2024-05-06T00:00:00Z,2024-05-06T07:00:00Z,2024-05-06T15:45:00Z,,
 2024-05-07T00:00:00Z,2024-05-07T07:00:00Z,2024-05-07T15:45:00Z,,
 2024-05-08T00:00:00Z,2024-05-08T07:00:00Z,2024-05-08T15:45:00Z,,
@@ -8715,14 +8753,15 @@
 2024-10-24T00:00:00Z,2024-10-24T07:00:00Z,2024-10-24T15:45:00Z,,
 2024-10-25T00:00:00Z,2024-10-25T07:00:00Z,2024-10-25T15:45:00Z,,
 2024-10-28T00:00:00Z,2024-10-28T07:00:00Z,2024-10-28T15:45:00Z,,
 2024-10-29T00:00:00Z,2024-10-29T07:00:00Z,2024-10-29T15:45:00Z,,
 2024-10-30T00:00:00Z,2024-10-30T07:00:00Z,2024-10-30T15:45:00Z,,
 2024-10-31T00:00:00Z,2024-10-31T07:00:00Z,2024-10-31T15:45:00Z,,
 2024-11-01T00:00:00Z,2024-11-01T07:00:00Z,2024-11-01T15:45:00Z,,
+2024-11-02T00:00:00Z,2024-11-02T07:00:00Z,2024-11-02T15:45:00Z,,
 2024-11-05T00:00:00Z,2024-11-05T07:00:00Z,2024-11-05T15:45:00Z,,
 2024-11-06T00:00:00Z,2024-11-06T07:00:00Z,2024-11-06T15:45:00Z,,
 2024-11-07T00:00:00Z,2024-11-07T07:00:00Z,2024-11-07T15:45:00Z,,
 2024-11-08T00:00:00Z,2024-11-08T07:00:00Z,2024-11-08T15:45:00Z,,
 2024-11-11T00:00:00Z,2024-11-11T07:00:00Z,2024-11-11T15:45:00Z,,
 2024-11-12T00:00:00Z,2024-11-12T07:00:00Z,2024-11-12T15:45:00Z,,
 2024-11-13T00:00:00Z,2024-11-13T07:00:00Z,2024-11-13T15:45:00Z,,
@@ -8754,8 +8793,9 @@
 2024-12-19T00:00:00Z,2024-12-19T07:00:00Z,2024-12-19T15:45:00Z,,
 2024-12-20T00:00:00Z,2024-12-20T07:00:00Z,2024-12-20T15:45:00Z,,
 2024-12-23T00:00:00Z,2024-12-23T07:00:00Z,2024-12-23T15:45:00Z,,
 2024-12-24T00:00:00Z,2024-12-24T07:00:00Z,2024-12-24T15:45:00Z,,
 2024-12-25T00:00:00Z,2024-12-25T07:00:00Z,2024-12-25T15:45:00Z,,
 2024-12-26T00:00:00Z,2024-12-26T07:00:00Z,2024-12-26T15:45:00Z,,
 2024-12-27T00:00:00Z,2024-12-27T07:00:00Z,2024-12-27T15:45:00Z,,
+2024-12-28T00:00:00Z,2024-12-28T07:00:00Z,2024-12-28T15:45:00Z,,
 2024-12-30T00:00:00Z,2024-12-30T07:00:00Z,2024-12-30T15:45:00Z,,
```

### Comparing `exchange_calendars-4.5.3/tests/resources/xnys.csv` & `exchange_calendars-4.5.4/tests/resources/xnys.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/resources/xnze.csv` & `exchange_calendars-4.5.4/tests/resources/xnze.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/resources/xosl.csv` & `exchange_calendars-4.5.4/tests/resources/xosl.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/resources/xpar.csv` & `exchange_calendars-4.5.4/tests/resources/xpar.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/resources/xphs.csv` & `exchange_calendars-4.5.4/tests/resources/xphs.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/resources/xpra.csv` & `exchange_calendars-4.5.4/tests/resources/xpra.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/resources/xsau.csv` & `exchange_calendars-4.5.4/tests/resources/xsau.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/resources/xses.csv` & `exchange_calendars-4.5.4/tests/resources/xses.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/resources/xsgo.csv` & `exchange_calendars-4.5.4/tests/resources/xsgo.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/resources/xshg.csv` & `exchange_calendars-4.5.4/tests/resources/xshg.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/resources/xsto.csv` & `exchange_calendars-4.5.4/tests/resources/xsto.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/resources/xswx.csv` & `exchange_calendars-4.5.4/tests/resources/xswx.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/resources/xtae.csv` & `exchange_calendars-4.5.4/tests/resources/xtae.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/resources/xtai.csv` & `exchange_calendars-4.5.4/tests/resources/xtai.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/resources/xtks.csv` & `exchange_calendars-4.5.4/tests/resources/xtks.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/resources/xtse.csv` & `exchange_calendars-4.5.4/tests/resources/xtse.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/resources/xwar.csv` & `exchange_calendars-4.5.4/tests/resources/xwar.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/resources/xwbo.csv` & `exchange_calendars-4.5.4/tests/resources/xwbo.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/test_aixk_calendar.py` & `exchange_calendars-4.5.4/tests/test_aixk_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/test_always_open.py` & `exchange_calendars-4.5.4/tests/test_always_open.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/test_asex_calendar.py` & `exchange_calendars-4.5.4/tests/test_asex_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/test_bvmf_calendar.py` & `exchange_calendars-4.5.4/tests/test_bvmf_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/test_calendar_dispatcher.py` & `exchange_calendars-4.5.4/tests/test_calendar_dispatcher.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/test_calendar_helpers.py` & `exchange_calendars-4.5.4/tests/test_calendar_helpers.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/test_cmes_calendar.py` & `exchange_calendars-4.5.4/tests/test_cmes_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/test_exchange_calendar.py` & `exchange_calendars-4.5.4/tests/test_exchange_calendar.py`

 * *Files 0% similar despite different names*

```diff
@@ -2229,16 +2229,17 @@
         cls = calendar_cls
         for name in non_valid_overrides:
             on_cls, on_base = getattr(cls, name), getattr(ExchangeCalendar, name)
             # covers properties, instance methods and class mathods...
             try:
                 assert on_cls == on_base or on_cls.__qualname__ == on_base.__qualname__
             except AttributeError:
-                if not (cls.name == "XKRX" and name == "day"):
+                if not (cls.name in ["XKRX", "XMOS"] and name == "day"):
                     # allow exchange_calendar_xkrx to overwrite 'day'.
+                    # allow exchange_calendar_xmos to overwrite 'day'.
                     raise
 
     def test_calculated_against_csv(self, default_calendar_with_answers):
         calendar, ans = default_calendar_with_answers
         tm.assert_index_equal(calendar.schedule.index, ans.sessions)
 
     def test_start_end(self, default_answers, calendar_cls):
```

### Comparing `exchange_calendars-4.5.3/tests/test_iepa_calendar.py` & `exchange_calendars-4.5.4/tests/test_iepa_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/test_weekday_calendar.py` & `exchange_calendars-4.5.4/tests/test_weekday_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/test_xams_calendar.py` & `exchange_calendars-4.5.4/tests/test_xams_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/test_xasx_calendar.py` & `exchange_calendars-4.5.4/tests/test_xasx_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/test_xbkk_calendar.py` & `exchange_calendars-4.5.4/tests/test_xbkk_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/test_xbog_calendar.py` & `exchange_calendars-4.5.4/tests/test_xbog_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/test_xbom_calendar.py` & `exchange_calendars-4.5.4/tests/test_xbom_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/test_xbru_calendar.py` & `exchange_calendars-4.5.4/tests/test_xbru_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/test_xbse_calendar.py` & `exchange_calendars-4.5.4/tests/test_xbse_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/test_xbud_calendar.py` & `exchange_calendars-4.5.4/tests/test_xbud_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/test_xbue_calendar.py` & `exchange_calendars-4.5.4/tests/test_xbue_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/test_xcbf_calendar.py` & `exchange_calendars-4.5.4/tests/test_xcbf_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/test_xcse_calendar.py` & `exchange_calendars-4.5.4/tests/test_xcse_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/test_xdub_calendar.py` & `exchange_calendars-4.5.4/tests/test_xdub_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/test_xetr_calendar.py` & `exchange_calendars-4.5.4/tests/test_xetr_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/test_xfra_calendar.py` & `exchange_calendars-4.5.4/tests/test_xfra_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/test_xhel_calendar.py` & `exchange_calendars-4.5.4/tests/test_xhel_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/test_xhkg_calendar.py` & `exchange_calendars-4.5.4/tests/test_xhkg_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/test_xice_calendar.py` & `exchange_calendars-4.5.4/tests/test_xice_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/test_xidx_calendar.py` & `exchange_calendars-4.5.4/tests/test_xidx_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/test_xist_calendar.py` & `exchange_calendars-4.5.4/tests/test_xist_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/test_xjse_calendar.py` & `exchange_calendars-4.5.4/tests/test_xjse_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/test_xkar_calendar.py` & `exchange_calendars-4.5.4/tests/test_xkar_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/test_xkls_calendar.py` & `exchange_calendars-4.5.4/tests/test_xkls_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/test_xkrx_calendar.py` & `exchange_calendars-4.5.4/tests/test_xkrx_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/test_xlim_calendar.py` & `exchange_calendars-4.5.4/tests/test_xlim_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/test_xlis_calendar.py` & `exchange_calendars-4.5.4/tests/test_xlis_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/test_xlon_calendar.py` & `exchange_calendars-4.5.4/tests/test_xlon_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/test_xmad_calendar.py` & `exchange_calendars-4.5.4/tests/test_xmad_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/test_xmex_calendar.py` & `exchange_calendars-4.5.4/tests/test_xmex_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/test_xmil_calendar.py` & `exchange_calendars-4.5.4/tests/test_xmil_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/test_xmos_calendar.py` & `exchange_calendars-4.5.4/tests/test_xmos_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/test_xnys_calendar.py` & `exchange_calendars-4.5.4/tests/test_xnys_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/test_xnze_calendar.py` & `exchange_calendars-4.5.4/tests/test_xnze_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/test_xosl_calendar.py` & `exchange_calendars-4.5.4/tests/test_xosl_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/test_xpar_calendar.py` & `exchange_calendars-4.5.4/tests/test_xpar_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/test_xphs_calendar.py` & `exchange_calendars-4.5.4/tests/test_xphs_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/test_xpra_calendar.py` & `exchange_calendars-4.5.4/tests/test_xpra_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/test_xsau_calendar.py` & `exchange_calendars-4.5.4/tests/test_xsau_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/test_xses_calendar.py` & `exchange_calendars-4.5.4/tests/test_xses_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/test_xsgo_calendar.py` & `exchange_calendars-4.5.4/tests/test_xsgo_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/test_xshg_calendar.py` & `exchange_calendars-4.5.4/tests/test_xshg_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/test_xsto_calendar.py` & `exchange_calendars-4.5.4/tests/test_xsto_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/test_xswx_calendar.py` & `exchange_calendars-4.5.4/tests/test_xswx_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/test_xtae_calendar.py` & `exchange_calendars-4.5.4/tests/test_xtae_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/test_xtai_calendar.py` & `exchange_calendars-4.5.4/tests/test_xtai_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/test_xtks_calendar.py` & `exchange_calendars-4.5.4/tests/test_xtks_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/test_xtse_calendar.py` & `exchange_calendars-4.5.4/tests/test_xtse_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/test_xwar_calendar.py` & `exchange_calendars-4.5.4/tests/test_xwar_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.5.3/tests/test_xwbo_calendar.py` & `exchange_calendars-4.5.4/tests/test_xwbo_calendar.py`

 * *Files identical despite different names*

