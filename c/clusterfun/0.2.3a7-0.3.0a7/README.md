# Comparing `tmp/clusterfun-0.2.3a7.tar.gz` & `tmp/clusterfun-0.3.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clusterfun-0.2.3a7.tar", max compression
+gzip compressed data, was "clusterfun-0.3.0a7.tar", max compression
```

## Comparing `clusterfun-0.2.3a7.tar` & `clusterfun-0.3.0a7.tar`

### file list

```diff
@@ -1,100 +1,105 @@
--rw-r--r--   0        0        0    11357 2024-04-28 22:32:09.819834 clusterfun-0.2.3a7/LICENSE
--rw-r--r--   0        0        0     9280 2024-04-28 22:32:09.820288 clusterfun-0.2.3a7/README.md
--rw-r--r--   0        0        0      660 2024-04-28 22:32:09.852017 clusterfun-0.2.3a7/clusterfun/__init__.py
--rw-r--r--   0        0        0      970 2024-05-02 18:48:38.705980 clusterfun-0.2.3a7/clusterfun/app.py
--rw-r--r--   0        0        0     2137 2024-04-28 22:32:09.852532 clusterfun-0.2.3a7/clusterfun/config.py
--rw-r--r--   0        0        0      715 2024-04-28 22:32:09.852760 clusterfun-0.2.3a7/clusterfun/constants.py
--rw-r--r--   0        0        0     6790 2024-05-02 18:20:15.918521 clusterfun-0.2.3a7/clusterfun/frontend/404.html
--rw-r--r--   0        0        0      224 2024-05-02 18:20:15.920034 clusterfun-0.2.3a7/clusterfun/frontend/_next/static/0L8U1RGbBQqzpAEgBP-4y/_buildManifest.js
--rw-r--r--   0        0        0       80 2024-05-02 18:20:15.920441 clusterfun-0.2.3a7/clusterfun/frontend/_next/static/0L8U1RGbBQqzpAEgBP-4y/_ssgManifest.js
--rw-r--r--   0        0        0      224 2024-05-01 14:48:56.190992 clusterfun-0.2.3a7/clusterfun/frontend/_next/static/7K0stYTjLuE1ieiHwaOY8/_buildManifest.js
--rw-r--r--   0        0        0       80 2024-05-01 14:48:56.191316 clusterfun-0.2.3a7/clusterfun/frontend/_next/static/7K0stYTjLuE1ieiHwaOY8/_ssgManifest.js
--rw-r--r--   0        0        0      224 2024-05-01 14:48:56.192076 clusterfun-0.2.3a7/clusterfun/frontend/_next/static/9m8W0thtsOjMrVxSpss7G/_buildManifest.js
--rw-r--r--   0        0        0       80 2024-05-01 14:48:56.192715 clusterfun-0.2.3a7/clusterfun/frontend/_next/static/9m8W0thtsOjMrVxSpss7G/_ssgManifest.js
--rw-r--r--   0        0        0      224 2024-05-02 18:20:15.921043 clusterfun-0.2.3a7/clusterfun/frontend/_next/static/FajzyA8s2dBSB6nVAodLv/_buildManifest.js
--rw-r--r--   0        0        0       80 2024-05-02 18:20:15.921298 clusterfun-0.2.3a7/clusterfun/frontend/_next/static/FajzyA8s2dBSB6nVAodLv/_ssgManifest.js
--rw-r--r--   0        0        0     8025 2024-05-01 14:48:56.193828 clusterfun-0.2.3a7/clusterfun/frontend/_next/static/chunks/22.94ebc66962dcd0f8.js
--rw-r--r--   0        0        0   121966 2024-05-01 17:49:28.318074 clusterfun-0.2.3a7/clusterfun/frontend/_next/static/chunks/23-8126128752749016.js
--rw-r--r--   0        0        0   110785 2024-05-01 14:48:56.198064 clusterfun-0.2.3a7/clusterfun/frontend/_next/static/chunks/472-07a7dd51a787971b.js
--rw-r--r--   0        0        0   143320 2024-05-01 14:48:56.199462 clusterfun-0.2.3a7/clusterfun/frontend/_next/static/chunks/483-2d99a375fdcaeaa9.js
--rw-r--r--   0        0        0   131700 2024-05-02 18:20:15.926209 clusterfun-0.2.3a7/clusterfun/frontend/_next/static/chunks/500-9855c0cda36bb0be.js
--rw-r--r--   0        0        0   131700 2024-05-01 17:49:28.305857 clusterfun-0.2.3a7/clusterfun/frontend/_next/static/chunks/500-9beb637c2f8db305.js
--rw-r--r--   0        0        0     7388 2024-05-01 17:49:28.304285 clusterfun-0.2.3a7/clusterfun/frontend/_next/static/chunks/8.d9282dffb5cd6834.js
--rw-r--r--   0        0        0     4290 2024-05-01 17:49:28.328879 clusterfun-0.2.3a7/clusterfun/frontend/_next/static/chunks/870fdd6f-4049d31c55f7218c.js
--rw-r--r--   0        0        0     4290 2024-05-01 14:48:56.203293 clusterfun-0.2.3a7/clusterfun/frontend/_next/static/chunks/870fdd6f-51765f2c6413dd54.js
--rw-r--r--   0        0        0     1744 2024-05-01 17:49:28.315083 clusterfun-0.2.3a7/clusterfun/frontend/_next/static/chunks/app/_not-found/page-6eda385f9819e210.js
--rw-r--r--   0        0        0     1840 2024-05-01 14:48:56.204570 clusterfun-0.2.3a7/clusterfun/frontend/_next/static/chunks/app/_not-found-bee08356a690a144.js
--rw-r--r--   0        0        0      480 2024-05-02 18:20:15.926928 clusterfun-0.2.3a7/clusterfun/frontend/_next/static/chunks/app/layout-0f23d4766ac3d9e3.js
--rw-r--r--   0        0        0      480 2024-05-01 17:49:28.317493 clusterfun-0.2.3a7/clusterfun/frontend/_next/static/chunks/app/layout-15dece07a8c94bf7.js
--rw-r--r--   0        0        0      477 2024-05-01 14:48:56.206202 clusterfun-0.2.3a7/clusterfun/frontend/_next/static/chunks/app/layout-f917f547d72d1629.js
--rw-r--r--   0        0        0    26631 2024-05-02 18:20:15.927503 clusterfun-0.2.3a7/clusterfun/frontend/_next/static/chunks/app/page-0dc09429eb1650c3.js
--rw-r--r--   0        0        0    26688 2024-05-01 15:15:14.526938 clusterfun-0.2.3a7/clusterfun/frontend/_next/static/chunks/app/page-0dcd9b5adc14930a.js
--rw-r--r--   0        0        0    26619 2024-05-01 14:48:56.207662 clusterfun-0.2.3a7/clusterfun/frontend/_next/static/chunks/app/page-4f1f75de895ef2e9.js
--rw-r--r--   0        0        0    26640 2024-05-01 14:48:56.208488 clusterfun-0.2.3a7/clusterfun/frontend/_next/static/chunks/app/page-cc11fa76e9925a25.js
--rw-r--r--   0        0        0    27859 2024-05-01 14:48:56.209652 clusterfun-0.2.3a7/clusterfun/frontend/_next/static/chunks/app/page-facced18ab368811.js
--rw-r--r--   0        0        0  3613214 2024-05-01 17:49:28.308142 clusterfun-0.2.3a7/clusterfun/frontend/_next/static/chunks/f2d0f643.3ca4096564deaa88.js
--rw-r--r--   0        0        0  3842147 2024-05-01 14:48:56.238679 clusterfun-0.2.3a7/clusterfun/frontend/_next/static/chunks/f2d0f643.db7d448233298422.js
--rw-r--r--   0        0        0   172831 2024-05-01 17:49:28.318810 clusterfun-0.2.3a7/clusterfun/frontend/_next/static/chunks/fd9d1056-3324b1349d932382.js
--rw-r--r--   0        0        0   163906 2024-05-01 14:48:56.242705 clusterfun-0.2.3a7/clusterfun/frontend/_next/static/chunks/fd9d1056-e13d3c2807942cb7.js
--rw-r--r--   0        0        0   140171 2024-05-01 14:48:56.244603 clusterfun-0.2.3a7/clusterfun/frontend/_next/static/chunks/framework-8883d1e9be70c3da.js
--rw-r--r--   0        0        0   140981 2024-05-01 17:49:28.322207 clusterfun-0.2.3a7/clusterfun/frontend/_next/static/chunks/framework-aec844d2ccbe7592.js
--rw-r--r--   0        0        0   115325 2024-05-01 14:48:56.246881 clusterfun-0.2.3a7/clusterfun/frontend/_next/static/chunks/main-01a7d75e7a6a7c98.js
--rw-r--r--   0        0        0   109895 2024-05-01 17:49:28.327144 clusterfun-0.2.3a7/clusterfun/frontend/_next/static/chunks/main-0ba5df58c56b45df.js
--rw-r--r--   0        0        0      508 2024-05-01 14:48:56.248662 clusterfun-0.2.3a7/clusterfun/frontend/_next/static/chunks/main-app-27650c6b197f0cd8.js
--rw-r--r--   0        0        0      462 2024-05-01 17:49:28.322878 clusterfun-0.2.3a7/clusterfun/frontend/_next/static/chunks/main-app-e01e327631e02231.js
--rw-r--r--   0        0        0      325 2024-05-01 14:48:56.250189 clusterfun-0.2.3a7/clusterfun/frontend/_next/static/chunks/pages/_app-1534f180665c857f.js
--rw-r--r--   0        0        0      280 2024-05-01 17:49:28.324373 clusterfun-0.2.3a7/clusterfun/frontend/_next/static/chunks/pages/_app-6a626577ffa902a4.js
--rw-r--r--   0        0        0      247 2024-05-01 17:49:28.325168 clusterfun-0.2.3a7/clusterfun/frontend/_next/static/chunks/pages/_error-1be831200e60c5c0.js
--rw-r--r--   0        0        0      247 2024-05-01 14:48:56.252577 clusterfun-0.2.3a7/clusterfun/frontend/_next/static/chunks/pages/_error-b646007f40c4f0a8.js
--rw-r--r--   0        0        0    91381 2024-05-01 17:49:28.328041 clusterfun-0.2.3a7/clusterfun/frontend/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js
--rw-r--r--   0        0        0    91460 2024-05-01 14:48:56.253498 clusterfun-0.2.3a7/clusterfun/frontend/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
--rw-r--r--   0        0        0     4659 2024-05-01 14:48:56.254092 clusterfun-0.2.3a7/clusterfun/frontend/_next/static/chunks/webpack-60a4426b837ea404.js
--rw-r--r--   0        0        0     3824 2024-05-01 17:49:28.321608 clusterfun-0.2.3a7/clusterfun/frontend/_next/static/chunks/webpack-9c62b174fdbd129f.js
--rw-r--r--   0        0        0    28962 2024-05-01 17:49:28.302614 clusterfun-0.2.3a7/clusterfun/frontend/_next/static/css/23cc4be46f2171d6.css
--rw-r--r--   0        0        0    28962 2024-05-01 14:48:56.256127 clusterfun-0.2.3a7/clusterfun/frontend/_next/static/css/64b8c25cc96a1f37.css
--rw-r--r--   0        0        0      224 2024-05-01 14:48:56.256638 clusterfun-0.2.3a7/clusterfun/frontend/_next/static/gTuZP6baQRuoAlSBQfJhW/_buildManifest.js
--rw-r--r--   0        0        0       80 2024-05-01 14:48:56.256845 clusterfun-0.2.3a7/clusterfun/frontend/_next/static/gTuZP6baQRuoAlSBQfJhW/_ssgManifest.js
--rw-r--r--   0        0        0      224 2024-05-02 18:20:15.928020 clusterfun-0.2.3a7/clusterfun/frontend/_next/static/lbjNsPpWYZod25BysgHf4/_buildManifest.js
--rw-r--r--   0        0        0       80 2024-05-02 18:20:15.928227 clusterfun-0.2.3a7/clusterfun/frontend/_next/static/lbjNsPpWYZod25BysgHf4/_ssgManifest.js
--rw-r--r--   0        0        0      224 2024-05-01 14:48:56.257630 clusterfun-0.2.3a7/clusterfun/frontend/_next/static/mBEYttyj_pgzUHdneL-73/_buildManifest.js
--rw-r--r--   0        0        0       80 2024-05-01 14:48:56.257857 clusterfun-0.2.3a7/clusterfun/frontend/_next/static/mBEYttyj_pgzUHdneL-73/_ssgManifest.js
--rw-r--r--   0        0        0    10496 2024-05-01 17:49:28.333095 clusterfun-0.2.3a7/clusterfun/frontend/_next/static/media/05a31a2ca4975f99-s.woff2
--rw-r--r--   0        0        0    17612 2024-05-01 17:49:28.338830 clusterfun-0.2.3a7/clusterfun/frontend/_next/static/media/513657b02c5c193f-s.woff2
--rw-r--r--   0        0        0    22524 2024-05-01 17:49:28.333816 clusterfun-0.2.3a7/clusterfun/frontend/_next/static/media/51ed15f9841b9f9d-s.woff2
--rw-r--r--   0        0        0     9628 2024-05-01 17:49:28.332479 clusterfun-0.2.3a7/clusterfun/frontend/_next/static/media/Oliver-Regular-400.365d360e.woff
--rw-r--r--   0        0        0    46552 2024-05-01 17:49:28.334721 clusterfun-0.2.3a7/clusterfun/frontend/_next/static/media/c9a5bc6a7c948fb0-s.p.woff2
--rw-r--r--   0        0        0    80044 2024-05-01 17:49:28.337484 clusterfun-0.2.3a7/clusterfun/frontend/_next/static/media/d6b16ce4a6175f26-s.woff2
--rw-r--r--   0        0        0    27316 2024-05-01 17:49:28.335265 clusterfun-0.2.3a7/clusterfun/frontend/_next/static/media/ec159349637c90ad-s.woff2
--rw-r--r--   0        0        0    12768 2024-05-01 17:49:28.338209 clusterfun-0.2.3a7/clusterfun/frontend/_next/static/media/fd4db3eb5472fc27-s.woff2
--rw-r--r--   0        0        0     7406 2024-05-01 17:49:28.340320 clusterfun-0.2.3a7/clusterfun/frontend/favicon.ico
--rw-r--r--   0        0        0     9628 2024-05-01 17:49:28.341591 clusterfun-0.2.3a7/clusterfun/frontend/fonts/Oliver-Regular-400.woff
--rw-r--r--   0        0        0     4959 2024-05-02 18:20:15.928889 clusterfun-0.2.3a7/clusterfun/frontend/index.html
--rw-r--r--   0        0        0     2499 2024-05-02 18:20:15.929514 clusterfun-0.2.3a7/clusterfun/frontend/index.txt
--rw-r--r--   0        0        0     3341 2024-05-02 18:09:00.068465 clusterfun-0.2.3a7/clusterfun/main.py
--rw-r--r--   0        0        0        0 2024-04-28 22:32:09.895406 clusterfun-0.2.3a7/clusterfun/models/__init__.py
--rw-r--r--   0        0        0     3111 2024-04-28 22:32:09.895643 clusterfun-0.2.3a7/clusterfun/models/filter.py
--rw-r--r--   0        0        0     1159 2024-04-28 22:32:09.895855 clusterfun-0.2.3a7/clusterfun/models/media_indices.py
--rw-r--r--   0        0        0     1207 2024-04-28 22:32:09.896105 clusterfun-0.2.3a7/clusterfun/models/media_item.py
--rw-r--r--   0        0        0     8100 2024-05-02 18:09:06.692436 clusterfun-0.2.3a7/clusterfun/plot.py
--rw-r--r--   0        0        0     1183 2024-04-28 22:32:09.896695 clusterfun-0.2.3a7/clusterfun/plot_types/__init__.py
--rw-r--r--   0        0        0     3586 2024-04-28 22:32:09.898400 clusterfun-0.2.3a7/clusterfun/plot_types/bar_chart.py
--rw-r--r--   0        0        0     3166 2024-04-28 22:32:09.898957 clusterfun-0.2.3a7/clusterfun/plot_types/confusion_matrix.py
--rw-r--r--   0        0        0     1217 2024-04-28 22:32:09.899339 clusterfun-0.2.3a7/clusterfun/plot_types/grid.py
--rw-r--r--   0        0        0     4248 2024-04-28 22:32:09.899527 clusterfun-0.2.3a7/clusterfun/plot_types/histogram.py
--rw-r--r--   0        0        0     6119 2024-04-28 22:32:09.899714 clusterfun-0.2.3a7/clusterfun/plot_types/pie_chart.py
--rw-r--r--   0        0        0     1356 2024-04-28 22:32:09.899978 clusterfun-0.2.3a7/clusterfun/plot_types/scatter.py
--rw-r--r--   0        0        0     4277 2024-04-28 22:32:09.900224 clusterfun-0.2.3a7/clusterfun/plot_types/violin.py
--rw-r--r--   0        0        0     1721 2024-04-28 22:32:09.900538 clusterfun-0.2.3a7/clusterfun/serve_cli.py
--rw-r--r--   0        0        0        0 2024-04-28 22:32:09.900856 clusterfun-0.2.3a7/clusterfun/storage/__init__.py
--rw-r--r--   0        0        0     2238 2024-04-28 22:32:09.901088 clusterfun-0.2.3a7/clusterfun/storage/loader.py
--rw-r--r--   0        0        0        0 2024-04-28 22:32:09.902140 clusterfun-0.2.3a7/clusterfun/storage/local/__init__.py
--rw-r--r--   0        0        0     5387 2024-04-28 22:32:09.902560 clusterfun-0.2.3a7/clusterfun/storage/local/data.py
--rw-r--r--   0        0        0     4767 2024-05-02 18:20:15.931749 clusterfun-0.2.3a7/clusterfun/storage/local/helpers.py
--rw-r--r--   0        0        0     5101 2024-04-28 22:32:09.903144 clusterfun-0.2.3a7/clusterfun/storage/local/loader.py
--rw-r--r--   0        0        0     2744 2024-04-28 22:32:09.903488 clusterfun-0.2.3a7/clusterfun/storage/local/storer.py
--rw-r--r--   0        0        0     2753 2024-05-01 14:25:08.851394 clusterfun-0.2.3a7/clusterfun/storage/storer.py
--rw-r--r--   0        0        0        0 2024-04-28 22:32:09.903988 clusterfun-0.2.3a7/clusterfun/utils/__init__.py
--rw-r--r--   0        0        0     1193 2024-04-28 22:32:09.904259 clusterfun-0.2.3a7/clusterfun/utils/s3.py
--rw-r--r--   0        0        0     2258 2024-04-28 22:32:09.904443 clusterfun-0.2.3a7/clusterfun/validation.py
--rw-r--r--   0        0        0     1130 2024-05-02 19:30:55.402311 clusterfun-0.2.3a7/pyproject.toml
--rw-r--r--   0        0        0    10021 1970-01-01 00:00:00.000000 clusterfun-0.2.3a7/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-28 22:32:09.819834 clusterfun-0.3.0a7/LICENSE
+-rw-r--r--   0        0        0     9280 2024-04-28 22:32:09.820288 clusterfun-0.3.0a7/README.md
+-rw-r--r--   0        0        0      660 2024-04-28 22:32:09.852017 clusterfun-0.3.0a7/clusterfun/__init__.py
+-rw-r--r--   0        0        0      970 2024-05-02 18:48:38.705980 clusterfun-0.3.0a7/clusterfun/app.py
+-rw-r--r--   0        0        0     2137 2024-04-28 22:32:09.852532 clusterfun-0.3.0a7/clusterfun/config.py
+-rw-r--r--   0        0        0      715 2024-04-28 22:32:09.852760 clusterfun-0.3.0a7/clusterfun/constants.py
+-rw-r--r--   0        0        0     6790 2024-05-07 09:53:06.282457 clusterfun-0.3.0a7/clusterfun/frontend/404.html
+-rw-r--r--   0        0        0      224 2024-05-02 18:20:15.920034 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/0L8U1RGbBQqzpAEgBP-4y/_buildManifest.js
+-rw-r--r--   0        0        0       80 2024-05-02 18:20:15.920441 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/0L8U1RGbBQqzpAEgBP-4y/_ssgManifest.js
+-rw-r--r--   0        0        0      224 2024-05-07 09:53:06.289880 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/0t2IpDcBx6FIaFpL5-DTX/_buildManifest.js
+-rw-r--r--   0        0        0       80 2024-05-07 09:53:06.288728 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/0t2IpDcBx6FIaFpL5-DTX/_ssgManifest.js
+-rw-r--r--   0        0        0      224 2024-05-01 14:48:56.190992 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/7K0stYTjLuE1ieiHwaOY8/_buildManifest.js
+-rw-r--r--   0        0        0       80 2024-05-01 14:48:56.191316 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/7K0stYTjLuE1ieiHwaOY8/_ssgManifest.js
+-rw-r--r--   0        0        0      224 2024-05-01 14:48:56.192076 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/9m8W0thtsOjMrVxSpss7G/_buildManifest.js
+-rw-r--r--   0        0        0       80 2024-05-01 14:48:56.192715 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/9m8W0thtsOjMrVxSpss7G/_ssgManifest.js
+-rw-r--r--   0        0        0      224 2024-05-02 18:20:15.921043 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/FajzyA8s2dBSB6nVAodLv/_buildManifest.js
+-rw-r--r--   0        0        0       80 2024-05-02 18:20:15.921298 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/FajzyA8s2dBSB6nVAodLv/_ssgManifest.js
+-rw-r--r--   0        0        0     8025 2024-05-01 14:48:56.193828 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/22.94ebc66962dcd0f8.js
+-rw-r--r--   0        0        0   121966 2024-05-07 09:53:06.305902 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/23-8126128752749016.js
+-rw-r--r--   0        0        0   110785 2024-05-01 14:48:56.198064 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/472-07a7dd51a787971b.js
+-rw-r--r--   0        0        0   143320 2024-05-01 14:48:56.199462 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/483-2d99a375fdcaeaa9.js
+-rw-r--r--   0        0        0   131700 2024-05-02 18:20:15.926209 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/500-9855c0cda36bb0be.js
+-rw-r--r--   0        0        0   131700 2024-05-07 09:53:06.297351 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/500-9beb637c2f8db305.js
+-rw-r--r--   0        0        0     7388 2024-05-07 09:53:06.296139 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/8.d9282dffb5cd6834.js
+-rw-r--r--   0        0        0     4290 2024-05-07 09:53:06.321491 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/870fdd6f-4049d31c55f7218c.js
+-rw-r--r--   0        0        0     4290 2024-05-01 14:48:56.203293 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/870fdd6f-51765f2c6413dd54.js
+-rw-r--r--   0        0        0     1744 2024-05-07 09:53:06.303313 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/app/_not-found/page-6eda385f9819e210.js
+-rw-r--r--   0        0        0     1840 2024-05-01 14:48:56.204570 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/app/_not-found-bee08356a690a144.js
+-rw-r--r--   0        0        0      480 2024-05-02 18:20:15.926928 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/app/layout-0f23d4766ac3d9e3.js
+-rw-r--r--   0        0        0      480 2024-05-07 09:53:06.304580 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/app/layout-15dece07a8c94bf7.js
+-rw-r--r--   0        0        0      477 2024-05-01 14:48:56.206202 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/app/layout-f917f547d72d1629.js
+-rw-r--r--   0        0        0    26631 2024-05-07 09:53:06.301663 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/app/page-0dc09429eb1650c3.js
+-rw-r--r--   0        0        0    26688 2024-05-01 15:15:14.526938 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/app/page-0dcd9b5adc14930a.js
+-rw-r--r--   0        0        0    26619 2024-05-01 14:48:56.207662 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/app/page-4f1f75de895ef2e9.js
+-rw-r--r--   0        0        0    26640 2024-05-01 14:48:56.208488 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/app/page-cc11fa76e9925a25.js
+-rw-r--r--   0        0        0    27859 2024-05-01 14:48:56.209652 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/app/page-facced18ab368811.js
+-rw-r--r--   0        0        0  3613214 2024-05-07 09:53:06.299257 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/f2d0f643.3ca4096564deaa88.js
+-rw-r--r--   0        0        0  3842147 2024-05-01 14:48:56.238679 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/f2d0f643.db7d448233298422.js
+-rw-r--r--   0        0        0   172831 2024-05-07 09:53:06.306982 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/fd9d1056-3324b1349d932382.js
+-rw-r--r--   0        0        0   163906 2024-05-01 14:48:56.242705 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/fd9d1056-e13d3c2807942cb7.js
+-rw-r--r--   0        0        0   140171 2024-05-01 14:48:56.244603 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/framework-8883d1e9be70c3da.js
+-rw-r--r--   0        0        0   140981 2024-05-07 09:53:06.312488 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/framework-aec844d2ccbe7592.js
+-rw-r--r--   0        0        0   115325 2024-05-01 14:48:56.246881 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/main-01a7d75e7a6a7c98.js
+-rw-r--r--   0        0        0   109895 2024-05-07 09:53:06.318305 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/main-0ba5df58c56b45df.js
+-rw-r--r--   0        0        0      508 2024-05-01 14:48:56.248662 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/main-app-27650c6b197f0cd8.js
+-rw-r--r--   0        0        0      462 2024-05-07 09:53:06.314953 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/main-app-e01e327631e02231.js
+-rw-r--r--   0        0        0      325 2024-05-01 14:48:56.250189 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/pages/_app-1534f180665c857f.js
+-rw-r--r--   0        0        0      280 2024-05-07 09:53:06.316951 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/pages/_app-6a626577ffa902a4.js
+-rw-r--r--   0        0        0      247 2024-05-07 09:53:06.317661 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/pages/_error-1be831200e60c5c0.js
+-rw-r--r--   0        0        0      247 2024-05-01 14:48:56.252577 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/pages/_error-b646007f40c4f0a8.js
+-rw-r--r--   0        0        0    91381 2024-05-07 09:53:06.320646 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js
+-rw-r--r--   0        0        0    91460 2024-05-01 14:48:56.253498 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
+-rw-r--r--   0        0        0     4659 2024-05-01 14:48:56.254092 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/webpack-60a4426b837ea404.js
+-rw-r--r--   0        0        0     3824 2024-05-07 09:53:06.309226 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/webpack-9c62b174fdbd129f.js
+-rw-r--r--   0        0        0    28962 2024-05-07 09:53:06.287289 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/css/23cc4be46f2171d6.css
+-rw-r--r--   0        0        0    28962 2024-05-01 14:48:56.256127 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/css/64b8c25cc96a1f37.css
+-rw-r--r--   0        0        0      224 2024-05-01 14:48:56.256638 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/gTuZP6baQRuoAlSBQfJhW/_buildManifest.js
+-rw-r--r--   0        0        0       80 2024-05-01 14:48:56.256845 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/gTuZP6baQRuoAlSBQfJhW/_ssgManifest.js
+-rw-r--r--   0        0        0      224 2024-05-02 18:20:15.928020 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/lbjNsPpWYZod25BysgHf4/_buildManifest.js
+-rw-r--r--   0        0        0       80 2024-05-02 18:20:15.928227 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/lbjNsPpWYZod25BysgHf4/_ssgManifest.js
+-rw-r--r--   0        0        0      224 2024-05-01 14:48:56.257630 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/mBEYttyj_pgzUHdneL-73/_buildManifest.js
+-rw-r--r--   0        0        0       80 2024-05-01 14:48:56.257857 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/mBEYttyj_pgzUHdneL-73/_ssgManifest.js
+-rw-r--r--   0        0        0    10496 2024-05-07 09:53:06.326401 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/media/05a31a2ca4975f99-s.woff2
+-rw-r--r--   0        0        0    17612 2024-05-07 09:53:06.331658 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/media/513657b02c5c193f-s.woff2
+-rw-r--r--   0        0        0    22524 2024-05-07 09:53:06.327827 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/media/51ed15f9841b9f9d-s.woff2
+-rw-r--r--   0        0        0     9628 2024-05-07 09:53:06.325530 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/media/Oliver-Regular-400.365d360e.woff
+-rw-r--r--   0        0        0    46552 2024-05-07 09:53:06.329101 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/media/c9a5bc6a7c948fb0-s.p.woff2
+-rw-r--r--   0        0        0    80044 2024-05-07 09:53:06.330311 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/media/d6b16ce4a6175f26-s.woff2
+-rw-r--r--   0        0        0    27316 2024-05-07 09:53:06.329676 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/media/ec159349637c90ad-s.woff2
+-rw-r--r--   0        0        0    12768 2024-05-07 09:53:06.331057 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/media/fd4db3eb5472fc27-s.woff2
+-rw-r--r--   0        0        0     7406 2024-05-07 09:53:06.332516 clusterfun-0.3.0a7/clusterfun/frontend/favicon.ico
+-rw-r--r--   0        0        0     9628 2024-05-07 09:53:06.335678 clusterfun-0.3.0a7/clusterfun/frontend/fonts/Oliver-Regular-400.woff
+-rw-r--r--   0        0        0     4959 2024-05-07 09:53:06.336748 clusterfun-0.3.0a7/clusterfun/frontend/index.html
+-rw-r--r--   0        0        0     2499 2024-05-07 09:53:06.337830 clusterfun-0.3.0a7/clusterfun/frontend/index.txt
+-rw-r--r--   0        0        0     3341 2024-05-03 13:14:22.092512 clusterfun-0.3.0a7/clusterfun/main.py
+-rw-r--r--   0        0        0        0 2024-04-28 22:32:09.895406 clusterfun-0.3.0a7/clusterfun/models/__init__.py
+-rw-r--r--   0        0        0     3111 2024-04-28 22:32:09.895643 clusterfun-0.3.0a7/clusterfun/models/filter.py
+-rw-r--r--   0        0        0     1159 2024-04-28 22:32:09.895855 clusterfun-0.3.0a7/clusterfun/models/media_indices.py
+-rw-r--r--   0        0        0      945 2024-05-06 22:44:34.090007 clusterfun-0.3.0a7/clusterfun/models/media_item.py
+-rw-r--r--   0        0        0     8100 2024-05-03 13:14:27.292482 clusterfun-0.3.0a7/clusterfun/plot.py
+-rw-r--r--   0        0        0     1183 2024-04-28 22:32:09.896695 clusterfun-0.3.0a7/clusterfun/plot_types/__init__.py
+-rw-r--r--   0        0        0     3586 2024-04-28 22:32:09.898400 clusterfun-0.3.0a7/clusterfun/plot_types/bar_chart.py
+-rw-r--r--   0        0        0     3166 2024-04-28 22:32:09.898957 clusterfun-0.3.0a7/clusterfun/plot_types/confusion_matrix.py
+-rw-r--r--   0        0        0     1217 2024-04-28 22:32:09.899339 clusterfun-0.3.0a7/clusterfun/plot_types/grid.py
+-rw-r--r--   0        0        0     4248 2024-04-28 22:32:09.899527 clusterfun-0.3.0a7/clusterfun/plot_types/histogram.py
+-rw-r--r--   0        0        0     6119 2024-04-28 22:32:09.899714 clusterfun-0.3.0a7/clusterfun/plot_types/pie_chart.py
+-rw-r--r--   0        0        0     1356 2024-04-28 22:32:09.899978 clusterfun-0.3.0a7/clusterfun/plot_types/scatter.py
+-rw-r--r--   0        0        0     4277 2024-04-28 22:32:09.900224 clusterfun-0.3.0a7/clusterfun/plot_types/violin.py
+-rw-r--r--   0        0        0     1721 2024-04-28 22:32:09.900538 clusterfun-0.3.0a7/clusterfun/serve_cli.py
+-rw-r--r--   0        0        0        0 2024-04-28 22:32:09.900856 clusterfun-0.3.0a7/clusterfun/storage/__init__.py
+-rw-r--r--   0        0        0      944 2024-05-07 09:54:30.442488 clusterfun-0.3.0a7/clusterfun/storage/client/__init__.py
+-rw-r--r--   0        0        0     1249 2024-05-07 09:18:46.136998 clusterfun-0.3.0a7/clusterfun/storage/client/base.py
+-rw-r--r--   0        0        0      800 2024-05-07 09:18:46.136720 clusterfun-0.3.0a7/clusterfun/storage/client/http.py
+-rw-r--r--   0        0        0     1071 2024-05-07 09:18:46.140218 clusterfun-0.3.0a7/clusterfun/storage/client/local.py
+-rw-r--r--   0        0        0     1680 2024-05-07 09:51:17.155237 clusterfun-0.3.0a7/clusterfun/storage/client/s3.py
+-rw-r--r--   0        0        0     2238 2024-04-28 22:32:09.901088 clusterfun-0.3.0a7/clusterfun/storage/loader.py
+-rw-r--r--   0        0        0        0 2024-04-28 22:32:09.902140 clusterfun-0.3.0a7/clusterfun/storage/local/__init__.py
+-rw-r--r--   0        0        0     5387 2024-04-28 22:32:09.902560 clusterfun-0.3.0a7/clusterfun/storage/local/data.py
+-rw-r--r--   0        0        0     4767 2024-05-02 18:20:15.931749 clusterfun-0.3.0a7/clusterfun/storage/local/helpers.py
+-rw-r--r--   0        0        0     5113 2024-05-03 13:14:04.608491 clusterfun-0.3.0a7/clusterfun/storage/local/loader.py
+-rw-r--r--   0        0        0     2744 2024-04-28 22:32:09.903488 clusterfun-0.3.0a7/clusterfun/storage/local/storer.py
+-rw-r--r--   0        0        0     2629 2024-05-06 22:44:34.096055 clusterfun-0.3.0a7/clusterfun/storage/storer.py
+-rw-r--r--   0        0        0     2258 2024-04-28 22:32:09.904443 clusterfun-0.3.0a7/clusterfun/validation.py
+-rw-r--r--   0        0        0     1130 2024-05-07 09:54:33.240814 clusterfun-0.3.0a7/pyproject.toml
+-rw-r--r--   0        0        0    10021 1970-01-01 00:00:00.000000 clusterfun-0.3.0a7/PKG-INFO
```

### Comparing `clusterfun-0.2.3a7/LICENSE` & `clusterfun-0.3.0a7/LICENSE`

 * *Files identical despite different names*

### Comparing `clusterfun-0.2.3a7/README.md` & `clusterfun-0.3.0a7/README.md`

 * *Files identical despite different names*

### Comparing `clusterfun-0.2.3a7/clusterfun/__init__.py` & `clusterfun-0.3.0a7/clusterfun/__init__.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.2.3a7/clusterfun/app.py` & `clusterfun-0.3.0a7/clusterfun/app.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.2.3a7/clusterfun/config.py` & `clusterfun-0.3.0a7/clusterfun/config.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.2.3a7/clusterfun/constants.py` & `clusterfun-0.3.0a7/clusterfun/constants.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.2.3a7/clusterfun/frontend/404.html` & `clusterfun-0.3.0a7/clusterfun/frontend/404.html`

 * *Files 2% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html lang="en"><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width, initial-scale=1"/><link rel="preload" href="/_next/static/media/c9a5bc6a7c948fb0-s.p.woff2" as="font" crossorigin="" type="font/woff2"/><link rel="stylesheet" href="/_next/static/css/23cc4be46f2171d6.css" data-precedence="next"/><link rel="preload" as="script" fetchPriority="low" href="/_next/static/chunks/webpack-9c62b174fdbd129f.js"/><script src="/_next/static/chunks/fd9d1056-3324b1349d932382.js" async=""></script><script src="/_next/static/chunks/23-8126128752749016.js" async=""></script><script src="/_next/static/chunks/main-app-e01e327631e02231.js" async=""></script><title>404: This page could not be found.</title><title>Clusterfun</title><meta name="description" content="Explore data with one line of code"/><meta name="next-size-adjust"/><script src="/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js" noModule=""></script></head><body class="__className_aaf875"><div style="font-family:system-ui,&quot;Segoe UI&quot;,Roboto,Helvetica,Arial,sans-serif,&quot;Apple Color Emoji&quot;,&quot;Segoe UI Emoji&quot;;height:100vh;text-align:center;display:flex;flex-direction:column;align-items:center;justify-content:center"><div><style>body{color:#000;background:#fff;margin:0}.next-error-h1{border-right:1px solid rgba(0,0,0,.3)}@media (prefers-color-scheme:dark){body{color:#fff;background:#000}.next-error-h1{border-right:1px solid rgba(255,255,255,.3)}}</style><h1 class="next-error-h1" style="display:inline-block;margin:0 20px 0 0;padding:0 23px 0 0;font-size:24px;font-weight:500;vertical-align:top;line-height:49px">404</h1><div style="display:inline-block"><h2 style="font-size:14px;font-weight:400;line-height:49px;margin:0">This page could not be found.</h2></div></div></div><script src="/_next/static/chunks/webpack-9c62b174fdbd129f.js" async=""></script><script>(self.__next_f=self.__next_f||[]).push([0]);self.__next_f.push([2,null])</script><script>self.__next_f.push([1,"1:HL[\"/_next/static/media/c9a5bc6a7c948fb0-s.p.woff2\",\"font\",{\"crossOrigin\":\"\",\"type\":\"font/woff2\"}]\n2:HL[\"/_next/static/css/23cc4be46f2171d6.css\",\"style\"]\n"])</script><script>self.__next_f.push([1,"3:I[5751,[],\"\"]\n5:I[9275,[],\"\"]\n6:I[1343,[],\"\"]\nc:I[6130,[],\"\"]\n7:{\"fontFamily\":\"system-ui,\\\"Segoe UI\\\",Roboto,Helvetica,Arial,sans-serif,\\\"Apple Color Emoji\\\",\\\"Segoe UI Emoji\\\"\",\"height\":\"100vh\",\"textAlign\":\"center\",\"display\":\"flex\",\"flexDirection\":\"column\",\"alignItems\":\"center\",\"justifyContent\":\"center\"}\n8:{\"display\":\"inline-block\",\"margin\":\"0 20px 0 0\",\"padding\":\"0 23px 0 0\",\"fontSize\":24,\"fontWeight\":500,\"verticalAlign\":\"top\",\"lineHeight\":\"49px\"}\n9:{\"display\":\"inline-block\"}\na:{\"fontSize\":14,\"fontWeight\":400,\"lineHeight\":\"49px\",\"margin\":0}\nd:[]\n"])</script><script>self.__next_f.push([1,"0:[[[\"$\",\"link\",\"0\",{\"rel\":\"stylesheet\",\"href\":\"/_next/static/css/23cc4be46f2171d6.css\",\"precedence\":\"next\",\"crossOrigin\":\"$undefined\"}]],[\"$\",\"$L3\",null,{\"buildId\":\"0L8U1RGbBQqzpAEgBP-4y\",\"assetPrefix\":\"\",\"initialCanonicalUrl\":\"/_not-found\",\"initialTree\":[\"\",{\"children\":[\"/_not-found\",{\"children\":[\"__PAGE__\",{}]}]},\"$undefined\",\"$undefined\",true],\"initialSeedData\":[\"\",{\"children\":[\"/_not-found\",{\"children\":[\"__PAGE__\",{},[[\"$L4\",[[\"$\",\"title\",null,{\"children\":\"404: This page could not be found.\"}],[\"$\",\"div\",null,{\"style\":{\"fontFamily\":\"system-ui,\\\"Segoe UI\\\",Roboto,Helvetica,Arial,sans-serif,\\\"Apple Color Emoji\\\",\\\"Segoe UI Emoji\\\"\",\"height\":\"100vh\",\"textAlign\":\"center\",\"display\":\"flex\",\"flexDirection\":\"column\",\"alignItems\":\"center\",\"justifyContent\":\"center\"},\"children\":[\"$\",\"div\",null,{\"children\":[[\"$\",\"style\",null,{\"dangerouslySetInnerHTML\":{\"__html\":\"body{color:#000;background:#fff;margin:0}.next-error-h1{border-right:1px solid rgba(0,0,0,.3)}@media (prefers-color-scheme:dark){body{color:#fff;background:#000}.next-error-h1{border-right:1px solid rgba(255,255,255,.3)}}\"}}],[\"$\",\"h1\",null,{\"className\":\"next-error-h1\",\"style\":{\"display\":\"inline-block\",\"margin\":\"0 20px 0 0\",\"padding\":\"0 23px 0 0\",\"fontSize\":24,\"fontWeight\":500,\"verticalAlign\":\"top\",\"lineHeight\":\"49px\"},\"children\":\"404\"}],[\"$\",\"div\",null,{\"style\":{\"display\":\"inline-block\"},\"children\":[\"$\",\"h2\",null,{\"style\":{\"fontSize\":14,\"fontWeight\":400,\"lineHeight\":\"49px\",\"margin\":0},\"children\":\"This page could not be found.\"}]}]]}]}]]],null],null]},[\"$\",\"$L5\",null,{\"parallelRouterKey\":\"children\",\"segmentPath\":[\"children\",\"/_not-found\",\"children\"],\"error\":\"$undefined\",\"errorStyles\":\"$undefined\",\"errorScripts\":\"$undefined\",\"template\":[\"$\",\"$L6\",null,{}],\"templateStyles\":\"$undefined\",\"templateScripts\":\"$undefined\",\"notFound\":\"$undefined\",\"notFoundStyles\":\"$undefined\",\"styles\":null}],null]},[[\"$\",\"html\",null,{\"lang\":\"en\",\"children\":[null,[\"$\",\"body\",null,{\"className\":\"__className_aaf875\",\"children\":[\"$\",\"$L5\",null,{\"parallelRouterKey\":\"children\",\"segmentPath\":[\"children\"],\"error\":\"$undefined\",\"errorStyles\":\"$undefined\",\"errorScripts\":\"$undefined\",\"template\":[\"$\",\"$L6\",null,{}],\"templateStyles\":\"$undefined\",\"templateScripts\":\"$undefined\",\"notFound\":[[\"$\",\"title\",null,{\"children\":\"404: This page could not be found.\"}],[\"$\",\"div\",null,{\"style\":\"$7\",\"children\":[\"$\",\"div\",null,{\"children\":[[\"$\",\"style\",null,{\"dangerouslySetInnerHTML\":{\"__html\":\"body{color:#000;background:#fff;margin:0}.next-error-h1{border-right:1px solid rgba(0,0,0,.3)}@media (prefers-color-scheme:dark){body{color:#fff;background:#000}.next-error-h1{border-right:1px solid rgba(255,255,255,.3)}}\"}}],[\"$\",\"h1\",null,{\"className\":\"next-error-h1\",\"style\":\"$8\",\"children\":\"404\"}],[\"$\",\"div\",null,{\"style\":\"$9\",\"children\":[\"$\",\"h2\",null,{\"style\":\"$a\",\"children\":\"This page could not be found.\"}]}]]}]}]],\"notFoundStyles\":[],\"styles\":null}]}]]}],null],null],\"couldBeIntercepted\":false,\"initialHead\":[false,\"$Lb\"],\"globalErrorComponent\":\"$c\",\"missingSlots\":\"$Wd\"}]]\n"])</script><script>self.__next_f.push([1,"b:[[\"$\",\"meta\",\"0\",{\"name\":\"viewport\",\"content\":\"width=device-width, initial-scale=1\"}],[\"$\",\"meta\",\"1\",{\"charSet\":\"utf-8\"}],[\"$\",\"title\",\"2\",{\"children\":\"Clusterfun\"}],[\"$\",\"meta\",\"3\",{\"name\":\"description\",\"content\":\"Explore data with one line of code\"}],[\"$\",\"meta\",\"4\",{\"name\":\"next-size-adjust\"}]]\n4:null\n"])</script></body></html>
+<!DOCTYPE html><html lang="en"><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width, initial-scale=1"/><link rel="preload" href="/_next/static/media/c9a5bc6a7c948fb0-s.p.woff2" as="font" crossorigin="" type="font/woff2"/><link rel="stylesheet" href="/_next/static/css/23cc4be46f2171d6.css" data-precedence="next"/><link rel="preload" as="script" fetchPriority="low" href="/_next/static/chunks/webpack-9c62b174fdbd129f.js"/><script src="/_next/static/chunks/fd9d1056-3324b1349d932382.js" async=""></script><script src="/_next/static/chunks/23-8126128752749016.js" async=""></script><script src="/_next/static/chunks/main-app-e01e327631e02231.js" async=""></script><title>404: This page could not be found.</title><title>Clusterfun</title><meta name="description" content="Explore data with one line of code"/><meta name="next-size-adjust"/><script src="/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js" noModule=""></script></head><body class="__className_aaf875"><div style="font-family:system-ui,&quot;Segoe UI&quot;,Roboto,Helvetica,Arial,sans-serif,&quot;Apple Color Emoji&quot;,&quot;Segoe UI Emoji&quot;;height:100vh;text-align:center;display:flex;flex-direction:column;align-items:center;justify-content:center"><div><style>body{color:#000;background:#fff;margin:0}.next-error-h1{border-right:1px solid rgba(0,0,0,.3)}@media (prefers-color-scheme:dark){body{color:#fff;background:#000}.next-error-h1{border-right:1px solid rgba(255,255,255,.3)}}</style><h1 class="next-error-h1" style="display:inline-block;margin:0 20px 0 0;padding:0 23px 0 0;font-size:24px;font-weight:500;vertical-align:top;line-height:49px">404</h1><div style="display:inline-block"><h2 style="font-size:14px;font-weight:400;line-height:49px;margin:0">This page could not be found.</h2></div></div></div><script src="/_next/static/chunks/webpack-9c62b174fdbd129f.js" async=""></script><script>(self.__next_f=self.__next_f||[]).push([0]);self.__next_f.push([2,null])</script><script>self.__next_f.push([1,"1:HL[\"/_next/static/media/c9a5bc6a7c948fb0-s.p.woff2\",\"font\",{\"crossOrigin\":\"\",\"type\":\"font/woff2\"}]\n2:HL[\"/_next/static/css/23cc4be46f2171d6.css\",\"style\"]\n"])</script><script>self.__next_f.push([1,"3:I[5751,[],\"\"]\n5:I[9275,[],\"\"]\n6:I[1343,[],\"\"]\nc:I[6130,[],\"\"]\n7:{\"fontFamily\":\"system-ui,\\\"Segoe UI\\\",Roboto,Helvetica,Arial,sans-serif,\\\"Apple Color Emoji\\\",\\\"Segoe UI Emoji\\\"\",\"height\":\"100vh\",\"textAlign\":\"center\",\"display\":\"flex\",\"flexDirection\":\"column\",\"alignItems\":\"center\",\"justifyContent\":\"center\"}\n8:{\"display\":\"inline-block\",\"margin\":\"0 20px 0 0\",\"padding\":\"0 23px 0 0\",\"fontSize\":24,\"fontWeight\":500,\"verticalAlign\":\"top\",\"lineHeight\":\"49px\"}\n9:{\"display\":\"inline-block\"}\na:{\"fontSize\":14,\"fontWeight\":400,\"lineHeight\":\"49px\",\"margin\":0}\nd:[]\n"])</script><script>self.__next_f.push([1,"0:[[[\"$\",\"link\",\"0\",{\"rel\":\"stylesheet\",\"href\":\"/_next/static/css/23cc4be46f2171d6.css\",\"precedence\":\"next\",\"crossOrigin\":\"$undefined\"}]],[\"$\",\"$L3\",null,{\"buildId\":\"0t2IpDcBx6FIaFpL5-DTX\",\"assetPrefix\":\"\",\"initialCanonicalUrl\":\"/_not-found\",\"initialTree\":[\"\",{\"children\":[\"/_not-found\",{\"children\":[\"__PAGE__\",{}]}]},\"$undefined\",\"$undefined\",true],\"initialSeedData\":[\"\",{\"children\":[\"/_not-found\",{\"children\":[\"__PAGE__\",{},[[\"$L4\",[[\"$\",\"title\",null,{\"children\":\"404: This page could not be found.\"}],[\"$\",\"div\",null,{\"style\":{\"fontFamily\":\"system-ui,\\\"Segoe UI\\\",Roboto,Helvetica,Arial,sans-serif,\\\"Apple Color Emoji\\\",\\\"Segoe UI Emoji\\\"\",\"height\":\"100vh\",\"textAlign\":\"center\",\"display\":\"flex\",\"flexDirection\":\"column\",\"alignItems\":\"center\",\"justifyContent\":\"center\"},\"children\":[\"$\",\"div\",null,{\"children\":[[\"$\",\"style\",null,{\"dangerouslySetInnerHTML\":{\"__html\":\"body{color:#000;background:#fff;margin:0}.next-error-h1{border-right:1px solid rgba(0,0,0,.3)}@media (prefers-color-scheme:dark){body{color:#fff;background:#000}.next-error-h1{border-right:1px solid rgba(255,255,255,.3)}}\"}}],[\"$\",\"h1\",null,{\"className\":\"next-error-h1\",\"style\":{\"display\":\"inline-block\",\"margin\":\"0 20px 0 0\",\"padding\":\"0 23px 0 0\",\"fontSize\":24,\"fontWeight\":500,\"verticalAlign\":\"top\",\"lineHeight\":\"49px\"},\"children\":\"404\"}],[\"$\",\"div\",null,{\"style\":{\"display\":\"inline-block\"},\"children\":[\"$\",\"h2\",null,{\"style\":{\"fontSize\":14,\"fontWeight\":400,\"lineHeight\":\"49px\",\"margin\":0},\"children\":\"This page could not be found.\"}]}]]}]}]]],null],null]},[\"$\",\"$L5\",null,{\"parallelRouterKey\":\"children\",\"segmentPath\":[\"children\",\"/_not-found\",\"children\"],\"error\":\"$undefined\",\"errorStyles\":\"$undefined\",\"errorScripts\":\"$undefined\",\"template\":[\"$\",\"$L6\",null,{}],\"templateStyles\":\"$undefined\",\"templateScripts\":\"$undefined\",\"notFound\":\"$undefined\",\"notFoundStyles\":\"$undefined\",\"styles\":null}],null]},[[\"$\",\"html\",null,{\"lang\":\"en\",\"children\":[null,[\"$\",\"body\",null,{\"className\":\"__className_aaf875\",\"children\":[\"$\",\"$L5\",null,{\"parallelRouterKey\":\"children\",\"segmentPath\":[\"children\"],\"error\":\"$undefined\",\"errorStyles\":\"$undefined\",\"errorScripts\":\"$undefined\",\"template\":[\"$\",\"$L6\",null,{}],\"templateStyles\":\"$undefined\",\"templateScripts\":\"$undefined\",\"notFound\":[[\"$\",\"title\",null,{\"children\":\"404: This page could not be found.\"}],[\"$\",\"div\",null,{\"style\":\"$7\",\"children\":[\"$\",\"div\",null,{\"children\":[[\"$\",\"style\",null,{\"dangerouslySetInnerHTML\":{\"__html\":\"body{color:#000;background:#fff;margin:0}.next-error-h1{border-right:1px solid rgba(0,0,0,.3)}@media (prefers-color-scheme:dark){body{color:#fff;background:#000}.next-error-h1{border-right:1px solid rgba(255,255,255,.3)}}\"}}],[\"$\",\"h1\",null,{\"className\":\"next-error-h1\",\"style\":\"$8\",\"children\":\"404\"}],[\"$\",\"div\",null,{\"style\":\"$9\",\"children\":[\"$\",\"h2\",null,{\"style\":\"$a\",\"children\":\"This page could not be found.\"}]}]]}]}]],\"notFoundStyles\":[],\"styles\":null}]}]]}],null],null],\"couldBeIntercepted\":false,\"initialHead\":[false,\"$Lb\"],\"globalErrorComponent\":\"$c\",\"missingSlots\":\"$Wd\"}]]\n"])</script><script>self.__next_f.push([1,"b:[[\"$\",\"meta\",\"0\",{\"name\":\"viewport\",\"content\":\"width=device-width, initial-scale=1\"}],[\"$\",\"meta\",\"1\",{\"charSet\":\"utf-8\"}],[\"$\",\"title\",\"2\",{\"children\":\"Clusterfun\"}],[\"$\",\"meta\",\"3\",{\"name\":\"description\",\"content\":\"Explore data with one line of code\"}],[\"$\",\"meta\",\"4\",{\"name\":\"next-size-adjust\"}]]\n4:null\n"])</script></body></html>
```

### Comparing `clusterfun-0.2.3a7/clusterfun/frontend/_next/static/chunks/22.94ebc66962dcd0f8.js` & `clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/22.94ebc66962dcd0f8.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.2.3a7/clusterfun/frontend/_next/static/chunks/23-8126128752749016.js` & `clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/23-8126128752749016.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.2.3a7/clusterfun/frontend/_next/static/chunks/472-07a7dd51a787971b.js` & `clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/472-07a7dd51a787971b.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.2.3a7/clusterfun/frontend/_next/static/chunks/483-2d99a375fdcaeaa9.js` & `clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/483-2d99a375fdcaeaa9.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.2.3a7/clusterfun/frontend/_next/static/chunks/500-9855c0cda36bb0be.js` & `clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/500-9855c0cda36bb0be.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.2.3a7/clusterfun/frontend/_next/static/chunks/500-9beb637c2f8db305.js` & `clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/500-9beb637c2f8db305.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.2.3a7/clusterfun/frontend/_next/static/chunks/8.d9282dffb5cd6834.js` & `clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/8.d9282dffb5cd6834.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.2.3a7/clusterfun/frontend/_next/static/chunks/870fdd6f-4049d31c55f7218c.js` & `clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/870fdd6f-4049d31c55f7218c.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.2.3a7/clusterfun/frontend/_next/static/chunks/870fdd6f-51765f2c6413dd54.js` & `clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/870fdd6f-51765f2c6413dd54.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.2.3a7/clusterfun/frontend/_next/static/chunks/app/_not-found/page-6eda385f9819e210.js` & `clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/app/_not-found/page-6eda385f9819e210.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.2.3a7/clusterfun/frontend/_next/static/chunks/app/_not-found-bee08356a690a144.js` & `clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/app/_not-found-bee08356a690a144.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.2.3a7/clusterfun/frontend/_next/static/chunks/app/page-0dc09429eb1650c3.js` & `clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/app/page-0dc09429eb1650c3.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.2.3a7/clusterfun/frontend/_next/static/chunks/app/page-0dcd9b5adc14930a.js` & `clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/app/page-0dcd9b5adc14930a.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.2.3a7/clusterfun/frontend/_next/static/chunks/app/page-4f1f75de895ef2e9.js` & `clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/app/page-4f1f75de895ef2e9.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.2.3a7/clusterfun/frontend/_next/static/chunks/app/page-cc11fa76e9925a25.js` & `clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/app/page-cc11fa76e9925a25.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.2.3a7/clusterfun/frontend/_next/static/chunks/app/page-facced18ab368811.js` & `clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/app/page-facced18ab368811.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.2.3a7/clusterfun/frontend/_next/static/chunks/f2d0f643.3ca4096564deaa88.js` & `clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/f2d0f643.3ca4096564deaa88.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.2.3a7/clusterfun/frontend/_next/static/chunks/f2d0f643.db7d448233298422.js` & `clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/f2d0f643.db7d448233298422.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.2.3a7/clusterfun/frontend/_next/static/chunks/fd9d1056-3324b1349d932382.js` & `clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/fd9d1056-3324b1349d932382.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.2.3a7/clusterfun/frontend/_next/static/chunks/fd9d1056-e13d3c2807942cb7.js` & `clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/fd9d1056-e13d3c2807942cb7.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.2.3a7/clusterfun/frontend/_next/static/chunks/framework-8883d1e9be70c3da.js` & `clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/framework-8883d1e9be70c3da.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.2.3a7/clusterfun/frontend/_next/static/chunks/framework-aec844d2ccbe7592.js` & `clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/framework-aec844d2ccbe7592.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.2.3a7/clusterfun/frontend/_next/static/chunks/main-01a7d75e7a6a7c98.js` & `clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/main-01a7d75e7a6a7c98.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.2.3a7/clusterfun/frontend/_next/static/chunks/main-0ba5df58c56b45df.js` & `clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/main-0ba5df58c56b45df.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.2.3a7/clusterfun/frontend/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js` & `clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.2.3a7/clusterfun/frontend/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js` & `clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.2.3a7/clusterfun/frontend/_next/static/chunks/webpack-60a4426b837ea404.js` & `clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/webpack-60a4426b837ea404.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.2.3a7/clusterfun/frontend/_next/static/chunks/webpack-9c62b174fdbd129f.js` & `clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/webpack-9c62b174fdbd129f.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.2.3a7/clusterfun/frontend/_next/static/css/23cc4be46f2171d6.css` & `clusterfun-0.3.0a7/clusterfun/frontend/_next/static/css/23cc4be46f2171d6.css`

 * *Files identical despite different names*

### Comparing `clusterfun-0.2.3a7/clusterfun/frontend/_next/static/css/64b8c25cc96a1f37.css` & `clusterfun-0.3.0a7/clusterfun/frontend/_next/static/css/64b8c25cc96a1f37.css`

 * *Files identical despite different names*

### Comparing `clusterfun-0.2.3a7/clusterfun/frontend/_next/static/media/05a31a2ca4975f99-s.woff2` & `clusterfun-0.3.0a7/clusterfun/frontend/_next/static/media/05a31a2ca4975f99-s.woff2`

 * *Files identical despite different names*

### Comparing `clusterfun-0.2.3a7/clusterfun/frontend/_next/static/media/513657b02c5c193f-s.woff2` & `clusterfun-0.3.0a7/clusterfun/frontend/_next/static/media/513657b02c5c193f-s.woff2`

 * *Files identical despite different names*

### Comparing `clusterfun-0.2.3a7/clusterfun/frontend/_next/static/media/51ed15f9841b9f9d-s.woff2` & `clusterfun-0.3.0a7/clusterfun/frontend/_next/static/media/51ed15f9841b9f9d-s.woff2`

 * *Files identical despite different names*

### Comparing `clusterfun-0.2.3a7/clusterfun/frontend/_next/static/media/Oliver-Regular-400.365d360e.woff` & `clusterfun-0.3.0a7/clusterfun/frontend/_next/static/media/Oliver-Regular-400.365d360e.woff`

 * *Files identical despite different names*

### Comparing `clusterfun-0.2.3a7/clusterfun/frontend/_next/static/media/c9a5bc6a7c948fb0-s.p.woff2` & `clusterfun-0.3.0a7/clusterfun/frontend/_next/static/media/c9a5bc6a7c948fb0-s.p.woff2`

 * *Files identical despite different names*

### Comparing `clusterfun-0.2.3a7/clusterfun/frontend/_next/static/media/d6b16ce4a6175f26-s.woff2` & `clusterfun-0.3.0a7/clusterfun/frontend/_next/static/media/d6b16ce4a6175f26-s.woff2`

 * *Files identical despite different names*

### Comparing `clusterfun-0.2.3a7/clusterfun/frontend/_next/static/media/ec159349637c90ad-s.woff2` & `clusterfun-0.3.0a7/clusterfun/frontend/_next/static/media/ec159349637c90ad-s.woff2`

 * *Files identical despite different names*

### Comparing `clusterfun-0.2.3a7/clusterfun/frontend/_next/static/media/fd4db3eb5472fc27-s.woff2` & `clusterfun-0.3.0a7/clusterfun/frontend/_next/static/media/fd4db3eb5472fc27-s.woff2`

 * *Files identical despite different names*

### Comparing `clusterfun-0.2.3a7/clusterfun/frontend/favicon.ico` & `clusterfun-0.3.0a7/clusterfun/frontend/favicon.ico`

 * *Files identical despite different names*

### Comparing `clusterfun-0.2.3a7/clusterfun/frontend/fonts/Oliver-Regular-400.woff` & `clusterfun-0.3.0a7/clusterfun/frontend/fonts/Oliver-Regular-400.woff`

 * *Files identical despite different names*

### Comparing `clusterfun-0.2.3a7/clusterfun/frontend/index.html` & `clusterfun-0.3.0a7/clusterfun/frontend/index.html`

 * *Files 4% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html lang="en"><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width, initial-scale=1"/><link rel="preload" href="/_next/static/media/c9a5bc6a7c948fb0-s.p.woff2" as="font" crossorigin="" type="font/woff2"/><link rel="stylesheet" href="/_next/static/css/23cc4be46f2171d6.css" data-precedence="next"/><link rel="preload" as="script" fetchPriority="low" href="/_next/static/chunks/webpack-9c62b174fdbd129f.js"/><script src="/_next/static/chunks/fd9d1056-3324b1349d932382.js" async=""></script><script src="/_next/static/chunks/23-8126128752749016.js" async=""></script><script src="/_next/static/chunks/main-app-e01e327631e02231.js" async=""></script><script src="/_next/static/chunks/870fdd6f-4049d31c55f7218c.js" async=""></script><script src="/_next/static/chunks/500-9beb637c2f8db305.js" async=""></script><script src="/_next/static/chunks/app/page-0dc09429eb1650c3.js" async=""></script><title>Clusterfun</title><meta name="description" content="Explore data with one line of code"/><link rel="icon" href="/favicon.ico" type="image/x-icon" sizes="48x48"/><meta name="next-size-adjust"/><script src="/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js" noModule=""></script></head><body class="__className_aaf875"><div class="m-2"><div></div></div><script src="/_next/static/chunks/webpack-9c62b174fdbd129f.js" async=""></script><script>(self.__next_f=self.__next_f||[]).push([0]);self.__next_f.push([2,null])</script><script>self.__next_f.push([1,"1:HL[\"/_next/static/media/c9a5bc6a7c948fb0-s.p.woff2\",\"font\",{\"crossOrigin\":\"\",\"type\":\"font/woff2\"}]\n2:HL[\"/_next/static/css/23cc4be46f2171d6.css\",\"style\"]\n"])</script><script>self.__next_f.push([1,"3:I[5751,[],\"\"]\n5:I[6513,[],\"ClientPageRoot\"]\n6:I[9835,[\"676\",\"static/chunks/870fdd6f-4049d31c55f7218c.js\",\"500\",\"static/chunks/500-9beb637c2f8db305.js\",\"931\",\"static/chunks/app/page-0dc09429eb1650c3.js\"],\"default\"]\n7:I[9275,[],\"\"]\n8:I[1343,[],\"\"]\na:I[6130,[],\"\"]\nb:[]\n"])</script><script>self.__next_f.push([1,"0:[[[\"$\",\"link\",\"0\",{\"rel\":\"stylesheet\",\"href\":\"/_next/static/css/23cc4be46f2171d6.css\",\"precedence\":\"next\",\"crossOrigin\":\"$undefined\"}]],[\"$\",\"$L3\",null,{\"buildId\":\"0L8U1RGbBQqzpAEgBP-4y\",\"assetPrefix\":\"\",\"initialCanonicalUrl\":\"/\",\"initialTree\":[\"\",{\"children\":[\"__PAGE__\",{}]},\"$undefined\",\"$undefined\",true],\"initialSeedData\":[\"\",{\"children\":[\"__PAGE__\",{},[[\"$L4\",[\"$\",\"$L5\",null,{\"props\":{\"params\":{},\"searchParams\":{}},\"Component\":\"$6\"}]],null],null]},[[\"$\",\"html\",null,{\"lang\":\"en\",\"children\":[null,[\"$\",\"body\",null,{\"className\":\"__className_aaf875\",\"children\":[\"$\",\"$L7\",null,{\"parallelRouterKey\":\"children\",\"segmentPath\":[\"children\"],\"error\":\"$undefined\",\"errorStyles\":\"$undefined\",\"errorScripts\":\"$undefined\",\"template\":[\"$\",\"$L8\",null,{}],\"templateStyles\":\"$undefined\",\"templateScripts\":\"$undefined\",\"notFound\":[[\"$\",\"title\",null,{\"children\":\"404: This page could not be found.\"}],[\"$\",\"div\",null,{\"style\":{\"fontFamily\":\"system-ui,\\\"Segoe UI\\\",Roboto,Helvetica,Arial,sans-serif,\\\"Apple Color Emoji\\\",\\\"Segoe UI Emoji\\\"\",\"height\":\"100vh\",\"textAlign\":\"center\",\"display\":\"flex\",\"flexDirection\":\"column\",\"alignItems\":\"center\",\"justifyContent\":\"center\"},\"children\":[\"$\",\"div\",null,{\"children\":[[\"$\",\"style\",null,{\"dangerouslySetInnerHTML\":{\"__html\":\"body{color:#000;background:#fff;margin:0}.next-error-h1{border-right:1px solid rgba(0,0,0,.3)}@media (prefers-color-scheme:dark){body{color:#fff;background:#000}.next-error-h1{border-right:1px solid rgba(255,255,255,.3)}}\"}}],[\"$\",\"h1\",null,{\"className\":\"next-error-h1\",\"style\":{\"display\":\"inline-block\",\"margin\":\"0 20px 0 0\",\"padding\":\"0 23px 0 0\",\"fontSize\":24,\"fontWeight\":500,\"verticalAlign\":\"top\",\"lineHeight\":\"49px\"},\"children\":\"404\"}],[\"$\",\"div\",null,{\"style\":{\"display\":\"inline-block\"},\"children\":[\"$\",\"h2\",null,{\"style\":{\"fontSize\":14,\"fontWeight\":400,\"lineHeight\":\"49px\",\"margin\":0},\"children\":\"This page could not be found.\"}]}]]}]}]],\"notFoundStyles\":[],\"styles\":null}]}]]}],null],null],\"couldBeIntercepted\":false,\"initialHead\":[false,\"$L9\"],\"globalErrorComponent\":\"$a\",\"missingSlots\":\"$Wb\"}]]\n"])</script><script>self.__next_f.push([1,"9:[[\"$\",\"meta\",\"0\",{\"name\":\"viewport\",\"content\":\"width=device-width, initial-scale=1\"}],[\"$\",\"meta\",\"1\",{\"charSet\":\"utf-8\"}],[\"$\",\"title\",\"2\",{\"children\":\"Clusterfun\"}],[\"$\",\"meta\",\"3\",{\"name\":\"description\",\"content\":\"Explore data with one line of code\"}],[\"$\",\"link\",\"4\",{\"rel\":\"icon\",\"href\":\"/favicon.ico\",\"type\":\"image/x-icon\",\"sizes\":\"48x48\"}],[\"$\",\"meta\",\"5\",{\"name\":\"next-size-adjust\"}]]\n4:null\n"])</script></body></html>
+<!DOCTYPE html><html lang="en"><head><meta charSet="utf-8"/><meta name="viewport" content="width=device-width, initial-scale=1"/><link rel="preload" href="/_next/static/media/c9a5bc6a7c948fb0-s.p.woff2" as="font" crossorigin="" type="font/woff2"/><link rel="stylesheet" href="/_next/static/css/23cc4be46f2171d6.css" data-precedence="next"/><link rel="preload" as="script" fetchPriority="low" href="/_next/static/chunks/webpack-9c62b174fdbd129f.js"/><script src="/_next/static/chunks/fd9d1056-3324b1349d932382.js" async=""></script><script src="/_next/static/chunks/23-8126128752749016.js" async=""></script><script src="/_next/static/chunks/main-app-e01e327631e02231.js" async=""></script><script src="/_next/static/chunks/870fdd6f-4049d31c55f7218c.js" async=""></script><script src="/_next/static/chunks/500-9beb637c2f8db305.js" async=""></script><script src="/_next/static/chunks/app/page-0dc09429eb1650c3.js" async=""></script><title>Clusterfun</title><meta name="description" content="Explore data with one line of code"/><link rel="icon" href="/favicon.ico" type="image/x-icon" sizes="48x48"/><meta name="next-size-adjust"/><script src="/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js" noModule=""></script></head><body class="__className_aaf875"><div class="m-2"><div></div></div><script src="/_next/static/chunks/webpack-9c62b174fdbd129f.js" async=""></script><script>(self.__next_f=self.__next_f||[]).push([0]);self.__next_f.push([2,null])</script><script>self.__next_f.push([1,"1:HL[\"/_next/static/media/c9a5bc6a7c948fb0-s.p.woff2\",\"font\",{\"crossOrigin\":\"\",\"type\":\"font/woff2\"}]\n2:HL[\"/_next/static/css/23cc4be46f2171d6.css\",\"style\"]\n"])</script><script>self.__next_f.push([1,"3:I[5751,[],\"\"]\n5:I[6513,[],\"ClientPageRoot\"]\n6:I[9835,[\"676\",\"static/chunks/870fdd6f-4049d31c55f7218c.js\",\"500\",\"static/chunks/500-9beb637c2f8db305.js\",\"931\",\"static/chunks/app/page-0dc09429eb1650c3.js\"],\"default\"]\n7:I[9275,[],\"\"]\n8:I[1343,[],\"\"]\na:I[6130,[],\"\"]\nb:[]\n"])</script><script>self.__next_f.push([1,"0:[[[\"$\",\"link\",\"0\",{\"rel\":\"stylesheet\",\"href\":\"/_next/static/css/23cc4be46f2171d6.css\",\"precedence\":\"next\",\"crossOrigin\":\"$undefined\"}]],[\"$\",\"$L3\",null,{\"buildId\":\"0t2IpDcBx6FIaFpL5-DTX\",\"assetPrefix\":\"\",\"initialCanonicalUrl\":\"/\",\"initialTree\":[\"\",{\"children\":[\"__PAGE__\",{}]},\"$undefined\",\"$undefined\",true],\"initialSeedData\":[\"\",{\"children\":[\"__PAGE__\",{},[[\"$L4\",[\"$\",\"$L5\",null,{\"props\":{\"params\":{},\"searchParams\":{}},\"Component\":\"$6\"}]],null],null]},[[\"$\",\"html\",null,{\"lang\":\"en\",\"children\":[null,[\"$\",\"body\",null,{\"className\":\"__className_aaf875\",\"children\":[\"$\",\"$L7\",null,{\"parallelRouterKey\":\"children\",\"segmentPath\":[\"children\"],\"error\":\"$undefined\",\"errorStyles\":\"$undefined\",\"errorScripts\":\"$undefined\",\"template\":[\"$\",\"$L8\",null,{}],\"templateStyles\":\"$undefined\",\"templateScripts\":\"$undefined\",\"notFound\":[[\"$\",\"title\",null,{\"children\":\"404: This page could not be found.\"}],[\"$\",\"div\",null,{\"style\":{\"fontFamily\":\"system-ui,\\\"Segoe UI\\\",Roboto,Helvetica,Arial,sans-serif,\\\"Apple Color Emoji\\\",\\\"Segoe UI Emoji\\\"\",\"height\":\"100vh\",\"textAlign\":\"center\",\"display\":\"flex\",\"flexDirection\":\"column\",\"alignItems\":\"center\",\"justifyContent\":\"center\"},\"children\":[\"$\",\"div\",null,{\"children\":[[\"$\",\"style\",null,{\"dangerouslySetInnerHTML\":{\"__html\":\"body{color:#000;background:#fff;margin:0}.next-error-h1{border-right:1px solid rgba(0,0,0,.3)}@media (prefers-color-scheme:dark){body{color:#fff;background:#000}.next-error-h1{border-right:1px solid rgba(255,255,255,.3)}}\"}}],[\"$\",\"h1\",null,{\"className\":\"next-error-h1\",\"style\":{\"display\":\"inline-block\",\"margin\":\"0 20px 0 0\",\"padding\":\"0 23px 0 0\",\"fontSize\":24,\"fontWeight\":500,\"verticalAlign\":\"top\",\"lineHeight\":\"49px\"},\"children\":\"404\"}],[\"$\",\"div\",null,{\"style\":{\"display\":\"inline-block\"},\"children\":[\"$\",\"h2\",null,{\"style\":{\"fontSize\":14,\"fontWeight\":400,\"lineHeight\":\"49px\",\"margin\":0},\"children\":\"This page could not be found.\"}]}]]}]}]],\"notFoundStyles\":[],\"styles\":null}]}]]}],null],null],\"couldBeIntercepted\":false,\"initialHead\":[false,\"$L9\"],\"globalErrorComponent\":\"$a\",\"missingSlots\":\"$Wb\"}]]\n"])</script><script>self.__next_f.push([1,"9:[[\"$\",\"meta\",\"0\",{\"name\":\"viewport\",\"content\":\"width=device-width, initial-scale=1\"}],[\"$\",\"meta\",\"1\",{\"charSet\":\"utf-8\"}],[\"$\",\"title\",\"2\",{\"children\":\"Clusterfun\"}],[\"$\",\"meta\",\"3\",{\"name\":\"description\",\"content\":\"Explore data with one line of code\"}],[\"$\",\"link\",\"4\",{\"rel\":\"icon\",\"href\":\"/favicon.ico\",\"type\":\"image/x-icon\",\"sizes\":\"48x48\"}],[\"$\",\"meta\",\"5\",{\"name\":\"next-size-adjust\"}]]\n4:null\n"])</script></body></html>
```

### Comparing `clusterfun-0.2.3a7/clusterfun/frontend/index.txt` & `clusterfun-0.3.0a7/clusterfun/frontend/index.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 2:I[6513,[],"ClientPageRoot"]
 3:I[9835,["676","static/chunks/870fdd6f-4049d31c55f7218c.js","500","static/chunks/500-9beb637c2f8db305.js","931","static/chunks/app/page-0dc09429eb1650c3.js"],"default"]
 4:I[9275,[],""]
 5:I[1343,[],""]
-0:["0L8U1RGbBQqzpAEgBP-4y",[[["",{"children":["__PAGE__",{}]},"$undefined","$undefined",true],["",{"children":["__PAGE__",{},[["$L1",["$","$L2",null,{"props":{"params":{},"searchParams":{}},"Component":"$3"}]],null],null]},[["$","html",null,{"lang":"en","children":[null,["$","body",null,{"className":"__className_aaf875","children":["$","$L4",null,{"parallelRouterKey":"children","segmentPath":["children"],"error":"$undefined","errorStyles":"$undefined","errorScripts":"$undefined","template":["$","$L5",null,{}],"templateStyles":"$undefined","templateScripts":"$undefined","notFound":[["$","title",null,{"children":"404: This page could not be found."}],["$","div",null,{"style":{"fontFamily":"system-ui,\"Segoe UI\",Roboto,Helvetica,Arial,sans-serif,\"Apple Color Emoji\",\"Segoe UI Emoji\"","height":"100vh","textAlign":"center","display":"flex","flexDirection":"column","alignItems":"center","justifyContent":"center"},"children":["$","div",null,{"children":[["$","style",null,{"dangerouslySetInnerHTML":{"__html":"body{color:#000;background:#fff;margin:0}.next-error-h1{border-right:1px solid rgba(0,0,0,.3)}@media (prefers-color-scheme:dark){body{color:#fff;background:#000}.next-error-h1{border-right:1px solid rgba(255,255,255,.3)}}"}}],["$","h1",null,{"className":"next-error-h1","style":{"display":"inline-block","margin":"0 20px 0 0","padding":"0 23px 0 0","fontSize":24,"fontWeight":500,"verticalAlign":"top","lineHeight":"49px"},"children":"404"}],["$","div",null,{"style":{"display":"inline-block"},"children":["$","h2",null,{"style":{"fontSize":14,"fontWeight":400,"lineHeight":"49px","margin":0},"children":"This page could not be found."}]}]]}]}]],"notFoundStyles":[],"styles":null}]}]]}],null],null],[[["$","link","0",{"rel":"stylesheet","href":"/_next/static/css/23cc4be46f2171d6.css","precedence":"next","crossOrigin":"$undefined"}]],"$L6"]]]]
+0:["0t2IpDcBx6FIaFpL5-DTX",[[["",{"children":["__PAGE__",{}]},"$undefined","$undefined",true],["",{"children":["__PAGE__",{},[["$L1",["$","$L2",null,{"props":{"params":{},"searchParams":{}},"Component":"$3"}]],null],null]},[["$","html",null,{"lang":"en","children":[null,["$","body",null,{"className":"__className_aaf875","children":["$","$L4",null,{"parallelRouterKey":"children","segmentPath":["children"],"error":"$undefined","errorStyles":"$undefined","errorScripts":"$undefined","template":["$","$L5",null,{}],"templateStyles":"$undefined","templateScripts":"$undefined","notFound":[["$","title",null,{"children":"404: This page could not be found."}],["$","div",null,{"style":{"fontFamily":"system-ui,\"Segoe UI\",Roboto,Helvetica,Arial,sans-serif,\"Apple Color Emoji\",\"Segoe UI Emoji\"","height":"100vh","textAlign":"center","display":"flex","flexDirection":"column","alignItems":"center","justifyContent":"center"},"children":["$","div",null,{"children":[["$","style",null,{"dangerouslySetInnerHTML":{"__html":"body{color:#000;background:#fff;margin:0}.next-error-h1{border-right:1px solid rgba(0,0,0,.3)}@media (prefers-color-scheme:dark){body{color:#fff;background:#000}.next-error-h1{border-right:1px solid rgba(255,255,255,.3)}}"}}],["$","h1",null,{"className":"next-error-h1","style":{"display":"inline-block","margin":"0 20px 0 0","padding":"0 23px 0 0","fontSize":24,"fontWeight":500,"verticalAlign":"top","lineHeight":"49px"},"children":"404"}],["$","div",null,{"style":{"display":"inline-block"},"children":["$","h2",null,{"style":{"fontSize":14,"fontWeight":400,"lineHeight":"49px","margin":0},"children":"This page could not be found."}]}]]}]}]],"notFoundStyles":[],"styles":null}]}]]}],null],null],[[["$","link","0",{"rel":"stylesheet","href":"/_next/static/css/23cc4be46f2171d6.css","precedence":"next","crossOrigin":"$undefined"}]],"$L6"]]]]
 6:[["$","meta","0",{"name":"viewport","content":"width=device-width, initial-scale=1"}],["$","meta","1",{"charSet":"utf-8"}],["$","title","2",{"children":"Clusterfun"}],["$","meta","3",{"name":"description","content":"Explore data with one line of code"}],["$","link","4",{"rel":"icon","href":"/favicon.ico","type":"image/x-icon","sizes":"48x48"}],["$","meta","5",{"name":"next-size-adjust"}]]
 1:null
```

### Comparing `clusterfun-0.2.3a7/clusterfun/main.py` & `clusterfun-0.3.0a7/clusterfun/main.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.2.3a7/clusterfun/models/filter.py` & `clusterfun-0.3.0a7/clusterfun/models/filter.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.2.3a7/clusterfun/models/media_indices.py` & `clusterfun-0.3.0a7/clusterfun/models/media_indices.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.2.3a7/clusterfun/plot.py` & `clusterfun-0.3.0a7/clusterfun/plot.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.2.3a7/clusterfun/plot_types/__init__.py` & `clusterfun-0.3.0a7/clusterfun/plot_types/__init__.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.2.3a7/clusterfun/plot_types/bar_chart.py` & `clusterfun-0.3.0a7/clusterfun/plot_types/bar_chart.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.2.3a7/clusterfun/plot_types/confusion_matrix.py` & `clusterfun-0.3.0a7/clusterfun/plot_types/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.2.3a7/clusterfun/plot_types/grid.py` & `clusterfun-0.3.0a7/clusterfun/plot_types/grid.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.2.3a7/clusterfun/plot_types/histogram.py` & `clusterfun-0.3.0a7/clusterfun/plot_types/histogram.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.2.3a7/clusterfun/plot_types/pie_chart.py` & `clusterfun-0.3.0a7/clusterfun/plot_types/pie_chart.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.2.3a7/clusterfun/plot_types/scatter.py` & `clusterfun-0.3.0a7/clusterfun/plot_types/scatter.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.2.3a7/clusterfun/plot_types/violin.py` & `clusterfun-0.3.0a7/clusterfun/plot_types/violin.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.2.3a7/clusterfun/serve_cli.py` & `clusterfun-0.3.0a7/clusterfun/serve_cli.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.2.3a7/clusterfun/storage/loader.py` & `clusterfun-0.3.0a7/clusterfun/storage/loader.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.2.3a7/clusterfun/storage/local/data.py` & `clusterfun-0.3.0a7/clusterfun/storage/local/data.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.2.3a7/clusterfun/storage/local/helpers.py` & `clusterfun-0.3.0a7/clusterfun/storage/local/helpers.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.2.3a7/clusterfun/storage/local/loader.py` & `clusterfun-0.3.0a7/clusterfun/storage/local/loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     def get_row(self, media_id: int, as_base64: bool = False) -> MediaItem:
         """Get a single row of data for a given uuid and media id."""
         result = run_query(self.db_path, f"SELECT * FROM database WHERE id = {media_id}", fetch_one=True)
         # index zero should be the id, index 1 the media src, everything else the remaining data
         src, height, width = load_media(
             result[1], as_base64=as_base64, common_media_path=self.load_config().common_media_path
         )
-        return MediaItem(index=media_id, src=src, height=height, width=width, information=result[2:])
+        return MediaItem(index=media_id, src=src, height=height, width=width, information=list(result[2:]))
 
     def get_rows(self, media_indices: MediaIndices) -> List[MediaItem]:
         """
         Gets a list of 50 rows, paginated
 
         Parameters
         ----------
@@ -95,15 +95,15 @@
             con = sqlite3.connect(self.db_path, check_same_thread=False)
             config = self.load_config()
         query = get_media_query(media_indices, config=config, con=con)
         result = run_query(self.db_path, query)
         items = []
         for item in result:
             src, height, width = load_media(item[1])
-            items.append(MediaItem(index=item[0], src=src, height=height, width=width, information=item[2:]))
+            items.append(MediaItem(index=item[0], src=src, height=height, width=width, information=list(item[2:])))
         return items
 
     def get_rows_metadata(self, media_indices: MediaIndices) -> List[Dict[str, Any]]:
         """
         Get the metadata for a list of media items.
 
         Parameters
```

### Comparing `clusterfun-0.2.3a7/clusterfun/storage/local/storer.py` & `clusterfun-0.3.0a7/clusterfun/storage/local/storer.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.2.3a7/clusterfun/storage/storer.py` & `clusterfun-0.3.0a7/clusterfun/storage/storer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """
 Base class for storing plots.
 """
+
 import abc
 import base64
 from io import BytesIO
 from typing import Any, Dict, List, Optional, Tuple
 
 import pandas as pd
-import requests
 from PIL import Image
 
 from clusterfun.config import Config
-from clusterfun.utils.s3 import get_presigned_url
+from clusterfun.storage.client import get_storage_client
 
 
 class Storer(abc.ABC):
     """Base class for storing plots."""
 
     @abc.abstractmethod
     def save(self, uuid: str, df: pd.DataFrame, cfg: Config):
@@ -63,19 +63,17 @@
 
     Returns
     -------
     Tuple[str, Optional[int], Optional[int]]
         The media, the height of the image, and the width of the image.
         Height and width are only returned if as_base64 is True.
     """
-    if url.startswith("s3://"):
-        url = get_presigned_url(url)
+
+    storage_client = get_storage_client(url, common_media_path)
+    url = storage_client.get_media(url)
+
     if as_base64:
-        if url.startswith("http"):
-            response = requests.get(url, timeout=60)
-            url = BytesIO(response.content)
-        else:
-            # assume local file
-            url = url.replace("/media", common_media_path)
-        image = Image.open(url)
+        image_bytes_or_str = storage_client.get_media_to_local(url)
+        image = Image.open(image_bytes_or_str)
         return f"data:image/png;base64, {image_to_base64(image)}", image.height, image.width
+
     return url, None, None
```

### Comparing `clusterfun-0.2.3a7/clusterfun/utils/s3.py` & `clusterfun-0.3.0a7/clusterfun/storage/client/s3.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,58 @@
 """Utilities for working with S3."""
+
 import os
 from functools import lru_cache
-from typing import Tuple
+from typing import Optional, Tuple
 
 import boto3
 from botocore.client import Config as BotoConfig
 
+from clusterfun.storage.client.http import HttpStorageClient
+
 
 @lru_cache()
 def get_client() -> boto3.client:
     """Get an S3 client."""
     client = boto3.client(
         "s3",
         region_name=os.environ.get("AWS_REGION"),
         config=BotoConfig(region_name=os.environ.get("AWS_REGION"), signature_version="s3v4"),
     )
     return client
 
 
-def get_presigned_url(s3_url: str) -> str:
-    """Generate a pre-signed URL for an S3 object. Defaults to 1 hour expiry."""
-    # Extract the bucket name and key from the full S3 URL
-    bucket_name, key = get_bucket_and_key(s3_url)
-    # Generate and return the pre-signed URL
-    return get_client().generate_presigned_url(
-        ClientMethod="get_object",
-        Params={
-            "Bucket": bucket_name,
-            "Key": key,
-        },
-        ExpiresIn=3600,
-    )
-
+class S3StorageClient(HttpStorageClient):
+    """S3 storage client."""
 
-def get_bucket_and_key(s3_path: str) -> Tuple[str, str]:
-    """Extract the bucket name and key from an S3 URL."""
-    path_parts = s3_path.replace("s3://", "").split("/")
-    bucket = path_parts.pop(0)
-    key = "/".join(path_parts)
-    return bucket, key
+    def __init__(self, common_media_path: Optional[str]):
+        super().__init__(common_media_path)
+        self.client = get_client()
+
+    def get_media(self, uri: str) -> str:
+        """Get media url.
+        Generate a pre-signed URL for an S3 object. Defaults to 1 hour expiry.
+
+        Args:
+            uri (str): media uri.
+
+        Returns:
+            str: media URL.
+        """
+        # Extract the bucket name and key from the full S3 URL
+        bucket_name, key = self.get_bucket_and_key(uri)
+        # Generate and return the pre-signed URL
+        return self.client.generate_presigned_url(
+            ClientMethod="get_object",
+            Params={
+                "Bucket": bucket_name,
+                "Key": key,
+            },
+            ExpiresIn=3600,
+        )
+
+    def get_bucket_and_key(self, s3_path: str) -> Tuple[str, str]:
+        """Extract the bucket name and key from an S3 URL."""
+        path_parts = s3_path.replace("s3://", "").split("/")
+        bucket = path_parts.pop(0)
+        key = "/".join(path_parts)
+        return bucket, key
```

### Comparing `clusterfun-0.2.3a7/clusterfun/validation.py` & `clusterfun-0.3.0a7/clusterfun/validation.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.2.3a7/pyproject.toml` & `clusterfun-0.3.0a7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "clusterfun"
-version = "0.2.3a7"
+version = "0.3.0a7"
 description = "Clusterfun - a plotting library to inspect data"
 authors = ["Jochem Gietema <jochem@giete.ma>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 pandas = "^2.0.0"
```

### Comparing `clusterfun-0.2.3a7/PKG-INFO` & `clusterfun-0.3.0a7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clusterfun
-Version: 0.2.3a7
+Version: 0.3.0a7
 Summary: Clusterfun - a plotting library to inspect data
 Author: Jochem Gietema
 Author-email: jochem@giete.ma
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

