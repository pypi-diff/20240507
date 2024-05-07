# Comparing `tmp/django_herobiz_ds-2.2.4.tar.gz` & `tmp/django_herobiz_ds-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_herobiz_ds-2.2.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "django_herobiz_ds-2.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `django_herobiz_ds-2.2.4.tar` & `django_herobiz_ds-2.3.0.tar`

### file list

```diff
@@ -1,179 +1,179 @@
--rw-r--r--   0        0        0     6148 2024-04-09 05:23:37.809838 django_herobiz_ds-2.2.4/.DS_Store
--rw-r--r--   0        0        0       66 2024-03-20 23:56:06.731106 django_herobiz_ds-2.2.4/.gitattributes
--rw-r--r--   0        0        0       29 2024-03-23 01:35:28.619023 django_herobiz_ds-2.2.4/.gitignore
--rw-r--r--   0        0        0       52 2024-03-20 23:57:31.872658 django_herobiz_ds-2.2.4/.idea/.gitignore
--rw-r--r--   0        0        0      407 2024-03-20 23:57:31.821245 django_herobiz_ds-2.2.4/.idea/django-herobiz-ds.iml
--rw-r--r--   0        0        0      174 2024-03-20 23:57:31.832580 django_herobiz_ds-2.2.4/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      425 2024-03-21 00:02:45.749953 django_herobiz_ds-2.2.4/.idea/misc.xml
--rw-r--r--   0        0        0      286 2024-03-20 23:57:31.826587 django_herobiz_ds-2.2.4/.idea/modules.xml
--rw-r--r--   0        0        0      167 2024-03-20 23:57:31.834402 django_herobiz_ds-2.2.4/.idea/vcs.xml
--rw-r--r--   0        0        0     1079 2024-03-19 03:45:10.033383 django_herobiz_ds-2.2.4/LICENSE
--rw-r--r--   0        0        0     5020 2024-04-21 10:52:50.701216 django_herobiz_ds-2.2.4/README.md
--rw-r--r--   0        0        0     8196 2024-03-28 02:01:43.009711 django_herobiz_ds-2.2.4/django_herobiz_ds/.DS_Store
--rw-r--r--   0        0        0        0 2024-03-28 01:56:00.401301 django_herobiz_ds-2.2.4/django_herobiz_ds/__init__.py
--rw-r--r--   0        0        0      612 2024-04-20 01:31:00.212458 django_herobiz_ds-2.2.4/django_herobiz_ds/admin.py
--rw-r--r--   0        0        0      164 2024-03-28 01:56:00.402678 django_herobiz_ds-2.2.4/django_herobiz_ds/apps.py
--rw-r--r--   0        0        0     1201 2024-04-20 02:08:26.881448 django_herobiz_ds-2.2.4/django_herobiz_ds/forms.py
--rw-r--r--   0        0        0     1988 2024-04-05 02:30:48.031309 django_herobiz_ds-2.2.4/django_herobiz_ds/migrations/0001_initial.py
--rw-r--r--   0        0        0      421 2024-04-05 03:09:43.264596 django_herobiz_ds-2.2.4/django_herobiz_ds/migrations/0002_portfolio_client.py
--rw-r--r--   0        0        0     2353 2024-04-19 06:58:00.234598 django_herobiz_ds-2.2.4/django_herobiz_ds/migrations/0003_post_profile.py
--rw-r--r--   0        0        0        0 2024-03-28 01:56:00.403238 django_herobiz_ds-2.2.4/django_herobiz_ds/migrations/__init__.py
--rw-r--r--   0        0        0     3116 2024-05-03 07:26:53.545281 django_herobiz_ds-2.2.4/django_herobiz_ds/models.py
--rw-r--r--   0        0        0      555 2024-04-19 06:57:49.960018 django_herobiz_ds-2.2.4/django_herobiz_ds/sitemaps.py
--rwxr-xr-x   0        0        0    60252 2024-03-29 01:14:08.439726 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/css/main.css
--rwxr-xr-x   0        0        0     7992 2024-04-03 08:26:33.002126 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/css/variables-blue.css
--rwxr-xr-x   0        0        0     7989 2024-04-03 08:32:44.614276 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/css/variables-green.css
--rwxr-xr-x   0        0        0     7992 2024-04-03 08:32:44.619981 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/css/variables-orange.css
--rwxr-xr-x   0        0        0     7994 2024-04-03 08:32:44.616432 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/css/variables-pink.css
--rwxr-xr-x   0        0        0     7992 2024-04-03 08:32:44.612088 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/css/variables-purple.css
--rwxr-xr-x   0        0        0     7986 2024-04-03 08:32:44.607824 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/css/variables-red.css
--rwxr-xr-x   0        0        0     7985 2024-04-03 08:32:44.618152 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/css/variables.css
--rwxr-xr-x   0        0        0      766 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/img/about-bg.png
--rwxr-xr-x   0        0        0    95604 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/img/faq.jpg
--rwxr-xr-x   0        0        0    13287 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/img/hero-bg.png
--rwxr-xr-x   0        0        0    13081 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/img/onfocus-content-bg.jpg
--rwxr-xr-x   0        0        0    61855 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/img/pricing-bg.jpg
--rwxr-xr-x   0        0        0     8186 2024-03-17 05:37:08.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/js/main.js
--rwxr-xr-x   0        0        0      281 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/scss/_blog.scss
--rwxr-xr-x   0        0        0     3649 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/scss/_footer.scss
--rwxr-xr-x   0        0        0     3770 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/scss/_general.scss
--rwxr-xr-x   0        0        0     1118 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/scss/_header.scss
--rwxr-xr-x   0        0        0      643 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/scss/_index.scss
--rwxr-xr-x   0        0        0     5712 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/scss/_nav.scss
--rwxr-xr-x   0        0        0     1320 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/scss/_portfolio-details.scss
--rwxr-xr-x   0        0        0     2172 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/scss/blog/_comments.scss
--rwxr-xr-x   0        0        0     3738 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/scss/blog/_details.scss
--rwxr-xr-x   0        0        0      758 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/scss/blog/_pagination.scss
--rwxr-xr-x   0        0        0     1813 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/scss/blog/_posts-list.scss
--rwxr-xr-x   0        0        0     3480 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/scss/blog/_sidebar.scss
--rwxr-xr-x   0        0        0     1676 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/scss/index/_about.scss
--rwxr-xr-x   0        0        0      377 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/scss/index/_clients.scss
--rwxr-xr-x   0        0        0     3086 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/scss/index/_contact.scss
--rwxr-xr-x   0        0        0     1882 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/scss/index/_cta.scss
--rwxr-xr-x   0        0        0     1674 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/scss/index/_faq.scss
--rwxr-xr-x   0        0        0      981 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/scss/index/_featured-services.scss
--rwxr-xr-x   0        0        0     1762 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/scss/index/_features.scss
--rwxr-xr-x   0        0        0     2205 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/scss/index/_hero-animated.scss
--rwxr-xr-x   0        0        0     1990 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/scss/index/_hero-fullscreen.scss
--rwxr-xr-x   0        0        0     1764 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/scss/index/_hero-static.scss
--rwxr-xr-x   0        0        0     3481 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/scss/index/_hero.scss
--rwxr-xr-x   0        0        0     3798 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/scss/index/_onfocus.scss
--rwxr-xr-x   0        0        0     2264 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/scss/index/_portfolio.scss
--rwxr-xr-x   0        0        0     2551 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/scss/index/_pricing.scss
--rwxr-xr-x   0        0        0     1512 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/scss/index/_recent-blog-posts.scss
--rwxr-xr-x   0        0        0     1718 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/scss/index/_services.scss
--rwxr-xr-x   0        0        0     1922 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/scss/index/_team.scss
--rwxr-xr-x   0        0        0     2203 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/scss/index/_testimonials.scss
--rwxr-xr-x   0        0        0      253 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/scss/main.scss
--rwxr-xr-x   0        0        0     7960 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/scss/variables-blue.css
--rwxr-xr-x   0        0        0     7957 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/scss/variables-green.css
--rwxr-xr-x   0        0        0     7960 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/scss/variables-orange.css
--rwxr-xr-x   0        0        0     7962 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/scss/variables-pink.css
--rwxr-xr-x   0        0        0     7960 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/scss/variables-purple.css
--rwxr-xr-x   0        0        0     7954 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/scss/variables-red.css
--rwxr-xr-x   0        0        0     7953 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/scss/variables.css
--rw-r--r--   0        0        0    19941 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/aos/aos.cjs.js
--rw-r--r--   0        0        0    28765 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/aos/aos.css
--rw-r--r--   0        0        0    19768 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/aos/aos.esm.js
--rw-r--r--   0        0        0    13800 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/aos/aos.js
--rw-r--r--   0        0        0    56459 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/aos/aos.js.map
--rw-r--r--   0        0        0    98255 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap-icons/bootstrap-icons.css
--rw-r--r--   0        0        0    52358 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap-icons/bootstrap-icons.json
--rw-r--r--   0        0        0    85875 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap-icons/bootstrap-icons.min.css
--rw-r--r--   0        0        0    57755 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap-icons/bootstrap-icons.scss
--rw-r--r--   0        0        0   176032 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap-icons/fonts/bootstrap-icons.woff
--rw-r--r--   0        0        0   130396 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap-icons/fonts/bootstrap-icons.woff2
--rw-r--r--   0        0        0    70329 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-grid.css
--rw-r--r--   0        0        0   203221 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-grid.css.map
--rw-r--r--   0        0        0    51795 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-grid.min.css
--rw-r--r--   0        0        0   115986 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-grid.min.css.map
--rw-r--r--   0        0        0    70403 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-grid.rtl.css
--rw-r--r--   0        0        0   203225 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-grid.rtl.css.map
--rw-r--r--   0        0        0    51870 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-grid.rtl.min.css
--rw-r--r--   0        0        0   116063 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-grid.rtl.min.css.map
--rw-r--r--   0        0        0    12065 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-reboot.css
--rw-r--r--   0        0        0   129371 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-reboot.css.map
--rw-r--r--   0        0        0    10126 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-reboot.min.css
--rw-r--r--   0        0        0    51369 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-reboot.min.css.map
--rw-r--r--   0        0        0    12058 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-reboot.rtl.css
--rw-r--r--   0        0        0   129386 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-reboot.rtl.css.map
--rw-r--r--   0        0        0    10198 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css
--rw-r--r--   0        0        0    63943 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css.map
--rw-r--r--   0        0        0   107823 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-utilities.css
--rw-r--r--   0        0        0   267535 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-utilities.css.map
--rw-r--r--   0        0        0    85352 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-utilities.min.css
--rw-r--r--   0        0        0   180381 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-utilities.min.css.map
--rw-r--r--   0        0        0   107691 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-utilities.rtl.css
--rw-r--r--   0        0        0   267476 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-utilities.rtl.css.map
--rw-r--r--   0        0        0    85281 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css
--rw-r--r--   0        0        0   180217 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css.map
--rw-r--r--   0        0        0   281046 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap.css
--rw-r--r--   0        0        0   679755 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap.css.map
--rw-r--r--   0        0        0   232803 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap.min.css
--rw-r--r--   0        0        0   589892 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap.min.css.map
--rw-r--r--   0        0        0   280259 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap.rtl.css
--rw-r--r--   0        0        0   679615 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap.rtl.css.map
--rw-r--r--   0        0        0   232911 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap.rtl.min.css
--rw-r--r--   0        0        0   589087 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap.rtl.min.css.map
--rw-r--r--   0        0        0   207819 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.bundle.js
--rw-r--r--   0        0        0   444579 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.bundle.js.map
--rw-r--r--   0        0        0    80721 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.bundle.min.js
--rw-r--r--   0        0        0   332090 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.bundle.min.js.map
--rw-r--r--   0        0        0   135829 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.esm.js
--rw-r--r--   0        0        0   305438 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.esm.js.map
--rw-r--r--   0        0        0    73935 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.esm.min.js
--rw-r--r--   0        0        0   222455 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.esm.min.js.map
--rw-r--r--   0        0        0   145401 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.js
--rw-r--r--   0        0        0   306606 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.js.map
--rw-r--r--   0        0        0    60635 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.min.js
--rw-r--r--   0        0        0   220561 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.min.js.map
--rw-r--r--   0        0        0    17372 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/glightbox/css/glightbox.css
--rw-r--r--   0        0        0    13749 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/glightbox/css/glightbox.min.css
--rw-r--r--   0        0        0    52561 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/glightbox/css/plyr.css
--rw-r--r--   0        0        0    45081 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/glightbox/css/plyr.min.css
--rw-r--r--   0        0        0   109391 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/glightbox/js/glightbox.js
--rw-r--r--   0        0        0    55880 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/glightbox/js/glightbox.min.js
--rw-r--r--   0        0        0    91398 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/isotope-layout/isotope.pkgd.js
--rw-r--r--   0        0        0    35445 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/isotope-layout/isotope.pkgd.min.js
--rwxr-xr-x   0        0        0   238381 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/php-email-form/php-email-form.php
--rwxr-xr-x   0        0        0     2734 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/php-email-form/validate.js
--rw-r--r--   0        0        0    18436 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/swiper/swiper-bundle.min.css
--rw-r--r--   0        0        0   149147 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/swiper/swiper-bundle.min.js
--rw-r--r--   0        0        0   201656 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/swiper/swiper-bundle.min.js.map
--rw-r--r--   0        0        0     2088 2024-04-09 00:06:50.834370 django_herobiz_ds-2.2.4/django_herobiz_ds/templates/herobizds/_about.html
--rw-r--r--   0        0        0      430 2024-03-29 06:35:13.298882 django_herobiz_ds-2.2.4/django_herobiz_ds/templates/herobizds/_clients.html
--rw-r--r--   0        0        0     2983 2024-04-03 07:06:14.783362 django_herobiz_ds-2.2.4/django_herobiz_ds/templates/herobizds/_contact.html
--rw-r--r--   0        0        0     1103 2024-04-09 05:54:45.913368 django_herobiz_ds-2.2.4/django_herobiz_ds/templates/herobizds/_cta.html
--rw-r--r--   0        0        0     1595 2024-04-02 01:30:23.624024 django_herobiz_ds-2.2.4/django_herobiz_ds/templates/herobizds/_faq.html
--rw-r--r--   0        0        0      794 2024-03-29 06:50:25.784512 django_herobiz_ds-2.2.4/django_herobiz_ds/templates/herobizds/_featured-services.html
--rw-r--r--   0        0        0     2035 2024-03-30 02:24:00.706893 django_herobiz_ds-2.2.4/django_herobiz_ds/templates/herobizds/_features.html
--rw-r--r--   0        0        0      963 2024-04-05 08:07:21.261387 django_herobiz_ds-2.2.4/django_herobiz_ds/templates/herobizds/_hero-animated.html
--rw-r--r--   0        0        0     1819 2024-03-29 05:34:15.457629 django_herobiz_ds-2.2.4/django_herobiz_ds/templates/herobizds/_hero-carousel.html
--rw-r--r--   0        0        0      857 2024-03-29 05:40:32.332271 django_herobiz_ds-2.2.4/django_herobiz_ds/templates/herobizds/_hero-fullscreen.html
--rw-r--r--   0        0        0      867 2024-03-29 05:42:02.021045 django_herobiz_ds-2.2.4/django_herobiz_ds/templates/herobizds/_hero-static.html
--rw-r--r--   0        0        0     1836 2024-04-09 06:01:02.688991 django_herobiz_ds-2.2.4/django_herobiz_ds/templates/herobizds/_onfocus.html
--rw-r--r--   0        0        0     1482 2024-04-02 05:48:18.679857 django_herobiz_ds-2.2.4/django_herobiz_ds/templates/herobizds/_portfolio.html
--rw-r--r--   0        0        0     1530 2024-04-02 01:24:08.992741 django_herobiz_ds-2.2.4/django_herobiz_ds/templates/herobizds/_pricing.html
--rw-r--r--   0        0        0     1085 2024-04-21 01:06:13.810908 django_herobiz_ds-2.2.4/django_herobiz_ds/templates/herobizds/_recent-blog-posts.html
--rw-r--r--   0        0        0      956 2024-03-30 02:24:56.706034 django_herobiz_ds-2.2.4/django_herobiz_ds/templates/herobizds/_services.html
--rw-r--r--   0        0        0     1660 2024-04-20 23:25:08.777077 django_herobiz_ds-2.2.4/django_herobiz_ds/templates/herobizds/_sidebar.html
--rw-r--r--   0        0        0     1485 2024-04-02 07:02:37.695381 django_herobiz_ds-2.2.4/django_herobiz_ds/templates/herobizds/_team.html
--rw-r--r--   0        0        0     1325 2024-04-02 00:03:23.122974 django_herobiz_ds-2.2.4/django_herobiz_ds/templates/herobizds/_testimonials.html
--rwxr-xr-x   0        0        0    10257 2024-04-21 02:26:19.039647 django_herobiz_ds-2.2.4/django_herobiz_ds/templates/herobizds/blog-details.html
--rwxr-xr-x   0        0        0     2859 2024-04-21 01:06:13.803930 django_herobiz_ds-2.2.4/django_herobiz_ds/templates/herobizds/blog.html
--rw-r--r--   0        0        0      342 2024-04-05 03:18:33.503234 django_herobiz_ds-2.2.4/django_herobiz_ds/templates/herobizds/breadcrumb.html
--rw-r--r--   0        0        0     3934 2024-04-04 04:44:18.713512 django_herobiz_ds-2.2.4/django_herobiz_ds/templates/herobizds/footer.html
--rwxr-xr-x   0        0        0     1341 2024-03-12 00:49:58.000000 django_herobiz_ds-2.2.4/django_herobiz_ds/templates/herobizds/forms/contact.php
--rw-r--r--   0        0        0     1366 2024-04-21 07:21:08.296478 django_herobiz_ds-2.2.4/django_herobiz_ds/templates/herobizds/header.html
--rwxr-xr-x   0        0        0     5086 2024-05-02 04:57:47.243792 django_herobiz_ds-2.2.4/django_herobiz_ds/templates/herobizds/index.html
--rwxr-xr-x   0        0        0     2532 2024-04-20 00:39:34.120518 django_herobiz_ds-2.2.4/django_herobiz_ds/templates/herobizds/portfolio-details.html
--rwxr-xr-x   0        0        0    16269 2024-04-21 00:18:44.160532 django_herobiz_ds-2.2.4/django_herobiz_ds/templates/herobizds/privacy.html
--rw-r--r--   0        0        0     2012 2024-04-03 07:59:23.373918 django_herobiz_ds-2.2.4/django_herobiz_ds/templates/herobizds/seo.html
--rwxr-xr-x   0        0        0    16309 2024-04-21 00:18:44.168769 django_herobiz_ds-2.2.4/django_herobiz_ds/templates/herobizds/terms.html
--rw-r--r--   0        0        0        0 2023-03-21 07:32:09.033136 django_herobiz_ds-2.2.4/django_herobiz_ds/templatetags/__init__.py
--rw-r--r--   0        0        0     4745 2024-05-03 01:09:29.808810 django_herobiz_ds-2.2.4/django_herobiz_ds/templatetags/herobizds_tags.py
--rw-r--r--   0        0        0       60 2024-03-28 01:56:00.403087 django_herobiz_ds-2.2.4/django_herobiz_ds/tests.py
--rw-r--r--   0        0        0     1111 2024-04-21 00:26:33.998664 django_herobiz_ds-2.2.4/django_herobiz_ds/urls.py
--rw-r--r--   0        0        0     7373 2024-05-02 07:53:42.673922 django_herobiz_ds-2.2.4/django_herobiz_ds/views.py
--rw-r--r--   0        0        0      969 2024-05-03 07:26:53.543222 django_herobiz_ds-2.2.4/pyproject.toml
--rw-r--r--   0        0        0     5756 1970-01-01 00:00:00.000000 django_herobiz_ds-2.2.4/PKG-INFO
+-rw-r--r--   0        0        0    10244 2024-05-07 00:45:14.907601 django_herobiz_ds-2.3.0/.DS_Store
+-rw-r--r--   0        0        0       66 2024-03-20 23:56:06.731106 django_herobiz_ds-2.3.0/.gitattributes
+-rw-r--r--   0        0        0       40 2024-05-07 00:28:25.952876 django_herobiz_ds-2.3.0/.gitignore
+-rw-r--r--   0        0        0       52 2024-03-20 23:57:31.872658 django_herobiz_ds-2.3.0/.idea/.gitignore
+-rw-r--r--   0        0        0      407 2024-03-20 23:57:31.821245 django_herobiz_ds-2.3.0/.idea/django-herobiz-ds.iml
+-rw-r--r--   0        0        0      174 2024-03-20 23:57:31.832580 django_herobiz_ds-2.3.0/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      425 2024-03-21 00:02:45.749953 django_herobiz_ds-2.3.0/.idea/misc.xml
+-rw-r--r--   0        0        0      286 2024-03-20 23:57:31.826587 django_herobiz_ds-2.3.0/.idea/modules.xml
+-rw-r--r--   0        0        0      167 2024-03-20 23:57:31.834402 django_herobiz_ds-2.3.0/.idea/vcs.xml
+-rw-r--r--   0        0        0     1079 2024-03-19 03:45:10.033383 django_herobiz_ds-2.3.0/LICENSE
+-rw-r--r--   0        0        0     5021 2024-05-07 00:57:37.575559 django_herobiz_ds-2.3.0/README.md
+-rw-r--r--   0        0        0     8196 2024-03-28 02:01:43.009711 django_herobiz_ds-2.3.0/django_herobiz_ds/.DS_Store
+-rw-r--r--   0        0        0        0 2024-03-28 01:56:00.401301 django_herobiz_ds-2.3.0/django_herobiz_ds/__init__.py
+-rw-r--r--   0        0        0      612 2024-04-20 01:31:00.212458 django_herobiz_ds-2.3.0/django_herobiz_ds/admin.py
+-rw-r--r--   0        0        0      164 2024-03-28 01:56:00.402678 django_herobiz_ds-2.3.0/django_herobiz_ds/apps.py
+-rw-r--r--   0        0        0     1201 2024-04-20 02:08:26.881448 django_herobiz_ds-2.3.0/django_herobiz_ds/forms.py
+-rw-r--r--   0        0        0     1988 2024-04-05 02:30:48.031309 django_herobiz_ds-2.3.0/django_herobiz_ds/migrations/0001_initial.py
+-rw-r--r--   0        0        0      421 2024-04-05 03:09:43.264596 django_herobiz_ds-2.3.0/django_herobiz_ds/migrations/0002_portfolio_client.py
+-rw-r--r--   0        0        0     2353 2024-04-19 06:58:00.234598 django_herobiz_ds-2.3.0/django_herobiz_ds/migrations/0003_post_profile.py
+-rw-r--r--   0        0        0        0 2024-03-28 01:56:00.403238 django_herobiz_ds-2.3.0/django_herobiz_ds/migrations/__init__.py
+-rw-r--r--   0        0        0     3116 2024-05-03 07:26:53.545281 django_herobiz_ds-2.3.0/django_herobiz_ds/models.py
+-rw-r--r--   0        0        0      555 2024-04-19 06:57:49.960018 django_herobiz_ds-2.3.0/django_herobiz_ds/sitemaps.py
+-rwxr-xr-x   0        0        0    60252 2024-03-29 01:14:08.439726 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/css/main.css
+-rwxr-xr-x   0        0        0     7992 2024-04-03 08:26:33.002126 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/css/variables-blue.css
+-rwxr-xr-x   0        0        0     7989 2024-04-03 08:32:44.614276 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/css/variables-green.css
+-rwxr-xr-x   0        0        0     7992 2024-04-03 08:32:44.619981 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/css/variables-orange.css
+-rwxr-xr-x   0        0        0     7994 2024-04-03 08:32:44.616432 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/css/variables-pink.css
+-rwxr-xr-x   0        0        0     7992 2024-04-03 08:32:44.612088 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/css/variables-purple.css
+-rwxr-xr-x   0        0        0     7986 2024-04-03 08:32:44.607824 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/css/variables-red.css
+-rwxr-xr-x   0        0        0     7985 2024-04-03 08:32:44.618152 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/css/variables.css
+-rwxr-xr-x   0        0        0      766 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/img/about-bg.png
+-rwxr-xr-x   0        0        0    95604 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/img/faq.jpg
+-rwxr-xr-x   0        0        0    13287 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/img/hero-bg.png
+-rwxr-xr-x   0        0        0    13081 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/img/onfocus-content-bg.jpg
+-rwxr-xr-x   0        0        0    61855 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/img/pricing-bg.jpg
+-rwxr-xr-x   0        0        0     8186 2024-03-17 05:37:08.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/js/main.js
+-rwxr-xr-x   0        0        0      281 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/_blog.scss
+-rwxr-xr-x   0        0        0     3649 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/_footer.scss
+-rwxr-xr-x   0        0        0     3770 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/_general.scss
+-rwxr-xr-x   0        0        0     1118 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/_header.scss
+-rwxr-xr-x   0        0        0      643 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/_index.scss
+-rwxr-xr-x   0        0        0     5712 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/_nav.scss
+-rwxr-xr-x   0        0        0     1320 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/_portfolio-details.scss
+-rwxr-xr-x   0        0        0     2172 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/blog/_comments.scss
+-rwxr-xr-x   0        0        0     3738 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/blog/_details.scss
+-rwxr-xr-x   0        0        0      758 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/blog/_pagination.scss
+-rwxr-xr-x   0        0        0     1813 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/blog/_posts-list.scss
+-rwxr-xr-x   0        0        0     3480 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/blog/_sidebar.scss
+-rwxr-xr-x   0        0        0     1676 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/index/_about.scss
+-rwxr-xr-x   0        0        0      377 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/index/_clients.scss
+-rwxr-xr-x   0        0        0     3086 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/index/_contact.scss
+-rwxr-xr-x   0        0        0     1882 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/index/_cta.scss
+-rwxr-xr-x   0        0        0     1674 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/index/_faq.scss
+-rwxr-xr-x   0        0        0      981 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/index/_featured-services.scss
+-rwxr-xr-x   0        0        0     1762 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/index/_features.scss
+-rwxr-xr-x   0        0        0     2205 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/index/_hero-animated.scss
+-rwxr-xr-x   0        0        0     1990 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/index/_hero-fullscreen.scss
+-rwxr-xr-x   0        0        0     1764 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/index/_hero-static.scss
+-rwxr-xr-x   0        0        0     3481 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/index/_hero.scss
+-rwxr-xr-x   0        0        0     3798 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/index/_onfocus.scss
+-rwxr-xr-x   0        0        0     2264 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/index/_portfolio.scss
+-rwxr-xr-x   0        0        0     2551 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/index/_pricing.scss
+-rwxr-xr-x   0        0        0     1512 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/index/_recent-blog-posts.scss
+-rwxr-xr-x   0        0        0     1718 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/index/_services.scss
+-rwxr-xr-x   0        0        0     1922 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/index/_team.scss
+-rwxr-xr-x   0        0        0     2203 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/index/_testimonials.scss
+-rwxr-xr-x   0        0        0      253 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/main.scss
+-rwxr-xr-x   0        0        0     7960 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/variables-blue.css
+-rwxr-xr-x   0        0        0     7957 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/variables-green.css
+-rwxr-xr-x   0        0        0     7960 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/variables-orange.css
+-rwxr-xr-x   0        0        0     7962 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/variables-pink.css
+-rwxr-xr-x   0        0        0     7960 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/variables-purple.css
+-rwxr-xr-x   0        0        0     7954 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/variables-red.css
+-rwxr-xr-x   0        0        0     7953 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/variables.css
+-rw-r--r--   0        0        0    19941 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/aos/aos.cjs.js
+-rw-r--r--   0        0        0    28765 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/aos/aos.css
+-rw-r--r--   0        0        0    19768 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/aos/aos.esm.js
+-rw-r--r--   0        0        0    13800 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/aos/aos.js
+-rw-r--r--   0        0        0    56459 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/aos/aos.js.map
+-rw-r--r--   0        0        0    98255 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap-icons/bootstrap-icons.css
+-rw-r--r--   0        0        0    52358 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap-icons/bootstrap-icons.json
+-rw-r--r--   0        0        0    85875 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap-icons/bootstrap-icons.min.css
+-rw-r--r--   0        0        0    57755 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap-icons/bootstrap-icons.scss
+-rw-r--r--   0        0        0   176032 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap-icons/fonts/bootstrap-icons.woff
+-rw-r--r--   0        0        0   130396 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap-icons/fonts/bootstrap-icons.woff2
+-rw-r--r--   0        0        0    70329 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-grid.css
+-rw-r--r--   0        0        0   203221 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-grid.css.map
+-rw-r--r--   0        0        0    51795 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-grid.min.css
+-rw-r--r--   0        0        0   115986 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-grid.min.css.map
+-rw-r--r--   0        0        0    70403 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-grid.rtl.css
+-rw-r--r--   0        0        0   203225 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-grid.rtl.css.map
+-rw-r--r--   0        0        0    51870 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-grid.rtl.min.css
+-rw-r--r--   0        0        0   116063 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-grid.rtl.min.css.map
+-rw-r--r--   0        0        0    12065 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-reboot.css
+-rw-r--r--   0        0        0   129371 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-reboot.css.map
+-rw-r--r--   0        0        0    10126 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-reboot.min.css
+-rw-r--r--   0        0        0    51369 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-reboot.min.css.map
+-rw-r--r--   0        0        0    12058 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-reboot.rtl.css
+-rw-r--r--   0        0        0   129386 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-reboot.rtl.css.map
+-rw-r--r--   0        0        0    10198 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css
+-rw-r--r--   0        0        0    63943 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css.map
+-rw-r--r--   0        0        0   107823 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-utilities.css
+-rw-r--r--   0        0        0   267535 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-utilities.css.map
+-rw-r--r--   0        0        0    85352 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-utilities.min.css
+-rw-r--r--   0        0        0   180381 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-utilities.min.css.map
+-rw-r--r--   0        0        0   107691 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-utilities.rtl.css
+-rw-r--r--   0        0        0   267476 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-utilities.rtl.css.map
+-rw-r--r--   0        0        0    85281 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css
+-rw-r--r--   0        0        0   180217 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css.map
+-rw-r--r--   0        0        0   281046 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap.css
+-rw-r--r--   0        0        0   679755 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap.css.map
+-rw-r--r--   0        0        0   232803 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap.min.css
+-rw-r--r--   0        0        0   589892 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap.min.css.map
+-rw-r--r--   0        0        0   280259 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap.rtl.css
+-rw-r--r--   0        0        0   679615 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap.rtl.css.map
+-rw-r--r--   0        0        0   232911 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap.rtl.min.css
+-rw-r--r--   0        0        0   589087 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap.rtl.min.css.map
+-rw-r--r--   0        0        0   207819 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.bundle.js
+-rw-r--r--   0        0        0   444579 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.bundle.js.map
+-rw-r--r--   0        0        0    80721 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.bundle.min.js
+-rw-r--r--   0        0        0   332090 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.bundle.min.js.map
+-rw-r--r--   0        0        0   135829 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.esm.js
+-rw-r--r--   0        0        0   305438 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.esm.js.map
+-rw-r--r--   0        0        0    73935 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.esm.min.js
+-rw-r--r--   0        0        0   222455 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.esm.min.js.map
+-rw-r--r--   0        0        0   145401 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.js
+-rw-r--r--   0        0        0   306606 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.js.map
+-rw-r--r--   0        0        0    60635 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.min.js
+-rw-r--r--   0        0        0   220561 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.min.js.map
+-rw-r--r--   0        0        0    17372 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/glightbox/css/glightbox.css
+-rw-r--r--   0        0        0    13749 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/glightbox/css/glightbox.min.css
+-rw-r--r--   0        0        0    52561 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/glightbox/css/plyr.css
+-rw-r--r--   0        0        0    45081 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/glightbox/css/plyr.min.css
+-rw-r--r--   0        0        0   109391 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/glightbox/js/glightbox.js
+-rw-r--r--   0        0        0    55880 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/glightbox/js/glightbox.min.js
+-rw-r--r--   0        0        0    91398 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/isotope-layout/isotope.pkgd.js
+-rw-r--r--   0        0        0    35445 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/isotope-layout/isotope.pkgd.min.js
+-rwxr-xr-x   0        0        0   238381 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/php-email-form/php-email-form.php
+-rwxr-xr-x   0        0        0     2734 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/php-email-form/validate.js
+-rw-r--r--   0        0        0    18436 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/swiper/swiper-bundle.min.css
+-rw-r--r--   0        0        0   149147 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/swiper/swiper-bundle.min.js
+-rw-r--r--   0        0        0   201656 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/swiper/swiper-bundle.min.js.map
+-rw-r--r--   0        0        0     2088 2024-04-09 00:06:50.834370 django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/_about.html
+-rw-r--r--   0        0        0      430 2024-03-29 06:35:13.298882 django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/_clients.html
+-rw-r--r--   0        0        0     2983 2024-04-03 07:06:14.783362 django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/_contact.html
+-rw-r--r--   0        0        0     1149 2024-05-07 00:54:12.174157 django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/_cta.html
+-rw-r--r--   0        0        0     1595 2024-04-02 01:30:23.624024 django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/_faq.html
+-rw-r--r--   0        0        0      794 2024-03-29 06:50:25.784512 django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/_featured-services.html
+-rw-r--r--   0        0        0     2035 2024-03-30 02:24:00.706893 django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/_features.html
+-rw-r--r--   0        0        0      963 2024-04-05 08:07:21.261387 django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/_hero-animated.html
+-rw-r--r--   0        0        0     1819 2024-03-29 05:34:15.457629 django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/_hero-carousel.html
+-rw-r--r--   0        0        0      857 2024-03-29 05:40:32.332271 django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/_hero-fullscreen.html
+-rw-r--r--   0        0        0      867 2024-03-29 05:42:02.021045 django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/_hero-static.html
+-rw-r--r--   0        0        0     1873 2024-05-07 00:56:09.871135 django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/_onfocus.html
+-rw-r--r--   0        0        0     1482 2024-04-02 05:48:18.679857 django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/_portfolio.html
+-rw-r--r--   0        0        0     1530 2024-04-02 01:24:08.992741 django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/_pricing.html
+-rw-r--r--   0        0        0     1085 2024-04-21 01:06:13.810908 django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/_recent-blog-posts.html
+-rw-r--r--   0        0        0      956 2024-03-30 02:24:56.706034 django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/_services.html
+-rw-r--r--   0        0        0     1660 2024-04-20 23:25:08.777077 django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/_sidebar.html
+-rw-r--r--   0        0        0     1485 2024-04-02 07:02:37.695381 django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/_team.html
+-rw-r--r--   0        0        0     1325 2024-04-02 00:03:23.122974 django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/_testimonials.html
+-rwxr-xr-x   0        0        0    10257 2024-04-21 02:26:19.039647 django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/blog-details.html
+-rwxr-xr-x   0        0        0     2859 2024-04-21 01:06:13.803930 django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/blog.html
+-rw-r--r--   0        0        0      342 2024-04-05 03:18:33.503234 django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/breadcrumb.html
+-rw-r--r--   0        0        0     3934 2024-04-04 04:44:18.713512 django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/footer.html
+-rwxr-xr-x   0        0        0     1341 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/forms/contact.php
+-rw-r--r--   0        0        0     1366 2024-04-21 07:21:08.296478 django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/header.html
+-rwxr-xr-x   0        0        0     5086 2024-05-02 04:57:47.243792 django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/index.html
+-rwxr-xr-x   0        0        0     2532 2024-04-20 00:39:34.120518 django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/portfolio-details.html
+-rwxr-xr-x   0        0        0    16269 2024-04-21 00:18:44.160532 django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/privacy.html
+-rw-r--r--   0        0        0     2012 2024-04-03 07:59:23.373918 django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/seo.html
+-rwxr-xr-x   0        0        0    16309 2024-04-21 00:18:44.168769 django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/terms.html
+-rw-r--r--   0        0        0        0 2023-03-21 07:32:09.033136 django_herobiz_ds-2.3.0/django_herobiz_ds/templatetags/__init__.py
+-rw-r--r--   0        0        0     4745 2024-05-03 01:09:29.808810 django_herobiz_ds-2.3.0/django_herobiz_ds/templatetags/herobizds_tags.py
+-rw-r--r--   0        0        0       60 2024-03-28 01:56:00.403087 django_herobiz_ds-2.3.0/django_herobiz_ds/tests.py
+-rw-r--r--   0        0        0     1111 2024-04-21 00:26:33.998664 django_herobiz_ds-2.3.0/django_herobiz_ds/urls.py
+-rw-r--r--   0        0        0     7373 2024-05-02 07:53:42.673922 django_herobiz_ds-2.3.0/django_herobiz_ds/views.py
+-rw-r--r--   0        0        0      969 2024-05-07 00:57:37.579961 django_herobiz_ds-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0     5757 1970-01-01 00:00:00.000000 django_herobiz_ds-2.3.0/PKG-INFO
```

### Comparing `django_herobiz_ds-2.2.4/LICENSE` & `django_herobiz_ds-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/README.md` & `django_herobiz_ds-2.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 블로그 포스트를 위해 admin에서 markdown 형식으로 글작성이 가능하다. 단, 이미지 삽입시 responsive 를 위해 class=img-fluid 클래스명 설정이
 필요하며 마크다운 에디터에서 이미지 마크 다운에 {: .img-fluid}를 넣어줘야 적용이 된다.
 
 ---
 #### Requirements
 
-Django >= 5.0.3
+Django >= 4.2.11
 libsass>=0.23.0
 django-analyticsds >= 0.3.1
 django-calendards >= 0.4.0
 django-modalds >= 0.1.0
 django-utilsds >= 0.4.0
 django-mdeditor >= 0.1.20
 django-hitcount >= 1.3.5
```

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/.DS_Store` & `django_herobiz_ds-2.3.0/django_herobiz_ds/.DS_Store`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/admin.py` & `django_herobiz_ds-2.3.0/django_herobiz_ds/admin.py`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/forms.py` & `django_herobiz_ds-2.3.0/django_herobiz_ds/forms.py`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/migrations/0001_initial.py` & `django_herobiz_ds-2.3.0/django_herobiz_ds/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/migrations/0003_post_profile.py` & `django_herobiz_ds-2.3.0/django_herobiz_ds/migrations/0003_post_profile.py`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/models.py` & `django_herobiz_ds-2.3.0/django_herobiz_ds/models.py`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/sitemaps.py` & `django_herobiz_ds-2.3.0/django_herobiz_ds/sitemaps.py`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/css/main.css` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/css/main.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/css/variables-blue.css` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/css/variables-blue.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/css/variables-green.css` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/css/variables-green.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/css/variables-orange.css` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/css/variables-orange.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/css/variables-pink.css` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/css/variables-pink.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/css/variables-purple.css` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/css/variables-purple.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/css/variables-red.css` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/css/variables-red.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/css/variables.css` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/css/variables.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/img/about-bg.png` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/img/about-bg.png`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/img/faq.jpg` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/img/faq.jpg`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/img/hero-bg.png` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/img/hero-bg.png`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/img/onfocus-content-bg.jpg` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/img/onfocus-content-bg.jpg`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/img/pricing-bg.jpg` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/img/pricing-bg.jpg`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/js/main.js` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/js/main.js`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/scss/_footer.scss` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/_footer.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/scss/_general.scss` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/_general.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/scss/_header.scss` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/_header.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/scss/_index.scss` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/_index.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/scss/_nav.scss` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/_nav.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/scss/_portfolio-details.scss` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/_portfolio-details.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/scss/blog/_comments.scss` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/blog/_comments.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/scss/blog/_details.scss` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/blog/_details.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/scss/blog/_pagination.scss` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/blog/_pagination.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/scss/blog/_posts-list.scss` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/blog/_posts-list.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/scss/blog/_sidebar.scss` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/blog/_sidebar.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/scss/index/_about.scss` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/index/_about.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/scss/index/_contact.scss` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/index/_contact.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/scss/index/_cta.scss` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/index/_cta.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/scss/index/_faq.scss` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/index/_faq.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/scss/index/_featured-services.scss` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/index/_featured-services.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/scss/index/_features.scss` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/index/_features.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/scss/index/_hero-animated.scss` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/index/_hero-animated.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/scss/index/_hero-fullscreen.scss` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/index/_hero-fullscreen.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/scss/index/_hero-static.scss` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/index/_hero-static.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/scss/index/_hero.scss` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/index/_hero.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/scss/index/_onfocus.scss` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/index/_onfocus.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/scss/index/_portfolio.scss` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/index/_portfolio.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/scss/index/_pricing.scss` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/index/_pricing.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/scss/index/_recent-blog-posts.scss` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/index/_recent-blog-posts.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/scss/index/_services.scss` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/index/_services.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/scss/index/_team.scss` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/index/_team.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/scss/index/_testimonials.scss` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/index/_testimonials.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/scss/variables-blue.css` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/variables-blue.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/scss/variables-green.css` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/variables-green.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/scss/variables-orange.css` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/variables-orange.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/scss/variables-pink.css` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/variables-pink.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/scss/variables-purple.css` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/variables-purple.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/scss/variables-red.css` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/variables-red.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/scss/variables.css` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/variables.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/aos/aos.cjs.js` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/aos/aos.cjs.js`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/aos/aos.css` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/aos/aos.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/aos/aos.esm.js` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/aos/aos.esm.js`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/aos/aos.js` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/aos/aos.js`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/aos/aos.js.map` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/aos/aos.js.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap-icons/bootstrap-icons.css` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap-icons/bootstrap-icons.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap-icons/bootstrap-icons.json` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap-icons/bootstrap-icons.json`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap-icons/bootstrap-icons.min.css` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap-icons/bootstrap-icons.min.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap-icons/bootstrap-icons.scss` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap-icons/bootstrap-icons.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap-icons/fonts/bootstrap-icons.woff` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap-icons/fonts/bootstrap-icons.woff`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap-icons/fonts/bootstrap-icons.woff2` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap-icons/fonts/bootstrap-icons.woff2`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-grid.css` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-grid.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-grid.css.map` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-grid.css.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-grid.min.css` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-grid.min.css.map` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-grid.min.css.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-grid.rtl.css` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-grid.rtl.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-grid.rtl.css.map` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-grid.rtl.css.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-grid.rtl.min.css` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-grid.rtl.min.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-grid.rtl.min.css.map` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-grid.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-reboot.css` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-reboot.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-reboot.css.map` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-reboot.css.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-reboot.min.css` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-reboot.min.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-reboot.min.css.map` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-reboot.min.css.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-reboot.rtl.css` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-reboot.rtl.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-reboot.rtl.css.map` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-reboot.rtl.css.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css.map` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-utilities.css` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-utilities.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-utilities.css.map` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-utilities.css.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-utilities.min.css` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-utilities.min.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-utilities.min.css.map` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-utilities.min.css.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-utilities.rtl.css` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-utilities.rtl.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-utilities.rtl.css.map` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-utilities.rtl.css.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css.map` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap.css` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap.css.map` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap.min.css` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap.min.css.map` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap.rtl.css` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap.rtl.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap.rtl.css.map` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap.rtl.css.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap.rtl.min.css` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap.rtl.min.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap.rtl.min.css.map` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.bundle.js` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.bundle.js`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.bundle.js.map` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.bundle.js.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.bundle.min.js` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.bundle.min.js.map` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.esm.js` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.esm.js`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.esm.js.map` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.esm.js.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.esm.min.js` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.esm.min.js`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.esm.min.js.map` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.esm.min.js.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.js` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.js.map` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.min.js` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.min.js.map` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/glightbox/css/glightbox.css` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/glightbox/css/glightbox.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/glightbox/css/glightbox.min.css` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/glightbox/css/glightbox.min.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/glightbox/css/plyr.css` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/glightbox/css/plyr.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/glightbox/css/plyr.min.css` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/glightbox/css/plyr.min.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/glightbox/js/glightbox.js` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/glightbox/js/glightbox.js`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/glightbox/js/glightbox.min.js` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/glightbox/js/glightbox.min.js`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/isotope-layout/isotope.pkgd.js` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/isotope-layout/isotope.pkgd.js`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/isotope-layout/isotope.pkgd.min.js` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/isotope-layout/isotope.pkgd.min.js`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/php-email-form/php-email-form.php` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/php-email-form/php-email-form.php`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/php-email-form/validate.js` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/php-email-form/validate.js`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/swiper/swiper-bundle.min.css` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/swiper/swiper-bundle.min.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/swiper/swiper-bundle.min.js` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/swiper/swiper-bundle.min.js`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/static/herobizds/vendor/swiper/swiper-bundle.min.js.map` & `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/swiper/swiper-bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/templates/herobizds/_about.html` & `django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/_about.html`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/templates/herobizds/_contact.html` & `django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/_contact.html`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/templates/herobizds/_cta.html` & `django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/_cta.html`

 * *Files 25% similar despite different names*

```diff
@@ -6,18 +6,20 @@
     <div class="row g-5">
       {% autoescape off %}
       <div class="col-lg-8 col-md-6 content d-flex flex-column justify-content-center order-last order-md-first">
         <h3>{{ cta.h3 }}</h3>
         <p> {{ cta.p }}</p>
         <div class="row row-cols-auto">
         <div class="col">
-          {% if cta.cta1.set_conversion %}
-          <a class="cta-btn align-self-start" href="{{ cta.cta1.link }}" onclick="cta1_gtag_report_conversion('{{ cta.cta1.link }}');" target="_blank">{{ cta.cta1.title }}</a>
+          {% if cta.btn.conversion_name %}
+          <a class="cta-btn align-self-start" href="{{ cta.btn.link }}"
+             onclick="{{ cta.btn.conversion_name }}_gtag_report_conversion('{{ cta.btn.link }}');"
+             target="_blank">{{ cta.btn.title }}</a>
           {% else %}
-          <a class="cta-btn align-self-start" href="{{ cta.cta1.link }}" target="_blank">{{ cta.cta1.title }}</a>
+          <a class="cta-btn align-self-start" href="{{ cta.btn.link }}" target="_blank">{{ cta.btn.title }}</a>
           {% endif %}
         </div>
         </div>
         {% endautoescape %}
       </div>
 
       <div class="col-lg-4 col-md-6 order-first order-md-last d-flex align-items-center">
```

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/templates/herobizds/_faq.html` & `django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/_faq.html`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/templates/herobizds/_featured-services.html` & `django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/_featured-services.html`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/templates/herobizds/_features.html` & `django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/_features.html`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/templates/herobizds/_hero-animated.html` & `django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/_hero-animated.html`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/templates/herobizds/_hero-carousel.html` & `django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/_hero-carousel.html`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/templates/herobizds/_hero-fullscreen.html` & `django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/_hero-fullscreen.html`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/templates/herobizds/_hero-static.html` & `django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/_hero-static.html`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/templates/herobizds/_onfocus.html` & `django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/_onfocus.html`

 * *Files 8% similar despite different names*

```diff
@@ -32,19 +32,20 @@
           </p>
           <ul>
             {% for item in onfocus.li %}
             <li><i class="bi bi-check-circle"></i>{{ item }}</li>
             {% endfor %}
           </ul>
           {% endautoescape %}
-          {% if onfocus.cta2.set_conversion %}
-          <a class="read-more align-self-start" href="{{ onfocus.cta2.link }}" onclick="cta2_gtag_report_conversion('{{ onfocus.cta2.link }}');"
-             target="_blank"><span>{{ onfocus.cta2.title }}</span><i class="bi bi-arrow-right"></i></a>
+          {% if onfocus.btn.conversion_name %}
+          <a class="read-more align-self-start" href="{{ onfocus.btn.link }}"
+             onclick="{{ onfocus.btn.conversion_name }}_gtag_report_conversion('{{ onfocus.btn.link }}');"
+             target="_blank"><span>{{ onfocus.btn.title }}</span><i class="bi bi-arrow-right"></i></a>
           {% else %}
-          <a class="read-more align-self-start" href="{{ onfocus.cta2.link }}"><span>{{ onfocus.cta2.title }}</span>
+          <a class="read-more align-self-start" href="{{ onfocus.btn.link }}"><span>{{ onfocus.btn.title }}</span>
             <i class="bi bi-arrow-right"></i></a>
           {% endif %}
         </div>
       </div>
     </div>
 
   </div>
```

#### html2text {}

```diff
@@ -2,12 +2,12 @@
 {% if onfocus.video_link %} {% endif %}
 {% autoescape off %}
 ******** {{{{ oonnffooccuuss..hh33 }}}} ********
 {{ onfocus.p }}
     * {% for item in onfocus.li %}
     * {{ item }}
     * {% endfor %}
-{% endautoescape %} {% if onfocus.cta2.set_conversion %}
-_{_{_ _o_n_f_o_c_u_s_._c_t_a_2_._t_i_t_l_e_ _}_}
+{% endautoescape %} {% if onfocus.btn.conversion_name %}
+_{_{_ _o_n_f_o_c_u_s_._b_t_n_._t_i_t_l_e_ _}_}
  {% else %}
-_{_{_ _o_n_f_o_c_u_s_._c_t_a_2_._t_i_t_l_e_ _}_}
+_{_{_ _o_n_f_o_c_u_s_._b_t_n_._t_i_t_l_e_ _}_}
 {% endif %}
```

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/templates/herobizds/_portfolio.html` & `django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/_portfolio.html`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/templates/herobizds/_pricing.html` & `django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/_pricing.html`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/templates/herobizds/_recent-blog-posts.html` & `django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/_recent-blog-posts.html`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/templates/herobizds/_services.html` & `django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/_services.html`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/templates/herobizds/_sidebar.html` & `django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/_sidebar.html`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/templates/herobizds/_team.html` & `django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/_team.html`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/templates/herobizds/_testimonials.html` & `django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/_testimonials.html`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/templates/herobizds/blog-details.html` & `django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/blog-details.html`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/templates/herobizds/blog.html` & `django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/blog.html`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/templates/herobizds/footer.html` & `django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/footer.html`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/templates/herobizds/forms/contact.php` & `django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/forms/contact.php`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/templates/herobizds/header.html` & `django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/header.html`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/templates/herobizds/index.html` & `django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/index.html`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/templates/herobizds/portfolio-details.html` & `django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/portfolio-details.html`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/templates/herobizds/privacy.html` & `django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/privacy.html`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/templates/herobizds/seo.html` & `django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/seo.html`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/templates/herobizds/terms.html` & `django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/terms.html`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/templatetags/herobizds_tags.py` & `django_herobiz_ds-2.3.0/django_herobiz_ds/templatetags/herobizds_tags.py`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/urls.py` & `django_herobiz_ds-2.3.0/django_herobiz_ds/urls.py`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/django_herobiz_ds/views.py` & `django_herobiz_ds-2.3.0/django_herobiz_ds/views.py`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.2.4/pyproject.toml` & `django_herobiz_ds-2.3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "django_herobiz_ds"
-version = "2.2.4"
+version = "2.3.0"
 description = "my demiansoft templates"
 authors = [{name = "Hyungjin Kim", email = "hj3415@gmail.com"}]
 readme = "README.md"
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: MIT License"]
 dependencies = [
     "Django >= 4.2.11",
```

### Comparing `django_herobiz_ds-2.2.4/PKG-INFO` & `django_herobiz_ds-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_herobiz_ds
-Version: 2.2.4
+Version: 2.3.0
 Summary: my demiansoft templates
 Author-email: Hyungjin Kim <hj3415@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: Django >= 4.2.11
 Requires-Dist: libsass>=0.23.0
 Requires-Dist: django-analyticsds >= 0.3.1
@@ -26,15 +26,15 @@
 
 블로그 포스트를 위해 admin에서 markdown 형식으로 글작성이 가능하다. 단, 이미지 삽입시 responsive 를 위해 class=img-fluid 클래스명 설정이
 필요하며 마크다운 에디터에서 이미지 마크 다운에 {: .img-fluid}를 넣어줘야 적용이 된다.
 
 ---
 #### Requirements
 
-Django >= 5.0.3
+Django >= 4.2.11
 libsass>=0.23.0
 django-analyticsds >= 0.3.1
 django-calendards >= 0.4.0
 django-modalds >= 0.1.0
 django-utilsds >= 0.4.0
 django-mdeditor >= 0.1.20
 django-hitcount >= 1.3.5
```

