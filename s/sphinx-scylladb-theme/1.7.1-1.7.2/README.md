# Comparing `tmp/sphinx_scylladb_theme-1.7.1.tar.gz` & `tmp/sphinx_scylladb_theme-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx_scylladb_theme-1.7.1.tar", max compression
+gzip compressed data, was "sphinx_scylladb_theme-1.7.2.tar", max compression
```

## Comparing `sphinx_scylladb_theme-1.7.1.tar` & `sphinx_scylladb_theme-1.7.2.tar`

### file list

```diff
@@ -1,162 +1,162 @@
--rw-r--r--   0        0        0    11338 2021-09-29 09:25:27.778592 sphinx_scylladb_theme-1.7.1/LICENSE
--rw-r--r--   0        0        0      184 2022-12-09 15:36:29.292783 sphinx_scylladb_theme-1.7.1/PYPI.rst
--rw-r--r--   0        0        0      950 2024-04-12 09:32:29.960247 sphinx_scylladb_theme-1.7.1/pyproject.toml
--rw-r--r--   0        0        0     1220 2024-04-02 09:38:37.390140 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/404.html
--rw-r--r--   0        0        0     3566 2024-04-12 09:32:29.960247 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/__init__.py
--rw-r--r--   0        0        0       89 2024-04-02 09:38:37.390140 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/_version.py
--rw-r--r--   0        0        0      734 2024-04-02 09:38:37.390140 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/breadcrumbs.html
--rw-r--r--   0        0        0     1075 2022-02-09 11:51:08.094565 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/content-navigation.html
--rw-r--r--   0        0        0     1122 2024-04-02 09:38:37.390140 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/contribute.html
--rw-r--r--   0        0        0        0 2021-09-29 09:25:27.800533 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/extensions/__init__.py
--rw-r--r--   0        0        0     4383 2024-04-05 11:00:24.590582 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/extensions/hero_box.py
--rw-r--r--   0        0        0      999 2022-11-15 12:53:40.356983 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/extensions/labels.py
--rw-r--r--   0        0        0     2952 2024-04-02 09:38:37.390140 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/extensions/multiversion.py
--rw-r--r--   0        0        0     2797 2022-02-09 11:51:08.097564 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/extensions/navigation.py
--rw-r--r--   0        0        0     1379 2022-10-07 12:02:26.581739 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/extensions/panel_box.py
--rw-r--r--   0        0        0     4250 2024-04-05 11:00:24.591580 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/extensions/topic_box.py
--rw-r--r--   0        0        0     1719 2024-04-02 09:38:37.390140 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/extensions/utils.py
--rw-r--r--   0        0        0      783 2024-04-02 09:38:37.390140 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/extensions/validations.py
--rw-r--r--   0        0        0     3067 2024-04-02 09:38:37.390140 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/feedback.html
--rw-r--r--   0        0        0     3232 2024-02-28 20:33:57.551090 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/footer.html
--rw-r--r--   0        0        0     4057 2024-04-02 09:38:37.390140 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/header.html
--rw-r--r--   0        0        0      219 2022-02-09 11:51:08.101577 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/last-updated.html
--rw-r--r--   0        0        0     5851 2024-04-12 09:32:29.960247 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/layout.html
--rw-r--r--   0        0        0        0 2022-02-09 11:52:03.175492 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/lexers/__init__.py
--rw-r--r--   0        0        0     6754 2021-09-29 09:25:27.805520 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/lexers/cql.py
--rw-r--r--   0        0        0       84 2021-09-29 09:25:27.805520 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/lexers/ditaa.py
--rw-r--r--   0        0        0       25 2024-04-02 09:38:37.390140 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/local-scripts.html
--rw-r--r--   0        0        0       27 2024-04-02 09:38:37.390140 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/notice.html
--rw-r--r--   0        0        0      802 2024-04-02 09:38:37.390140 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/promo-banner.html
--rw-r--r--   0        0        0     1588 2024-04-02 09:38:37.390140 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/scylladb-scripts.html
--rw-r--r--   0        0        0      275 2022-03-29 08:31:29.866817 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/secondary-side-nav.html
--rw-r--r--   0        0        0      186 2022-02-09 11:51:08.103844 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/side-nav-toggle.html
--rw-r--r--   0        0        0      962 2024-04-02 09:38:37.390140 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/side-nav.html
--rw-r--r--   0        0        0   226508 2024-04-05 12:23:37.426260 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/css/main.css
--rw-r--r--   0        0        0        0 2024-04-05 12:23:37.423258 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/.gitkeep
--rw-r--r--   0        0        0      635 2024-04-05 12:23:37.426260 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/banner-background.svg
--rw-r--r--   0        0        0     4428 2024-04-05 12:23:37.426260 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/favicon-228x228.png
--rw-r--r--   0        0        0      837 2024-04-05 12:23:37.426260 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/favicon-32x32.png
--rw-r--r--   0        0        0     1150 2024-04-05 12:23:37.426260 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/favicon.ico
--rw-r--r--   0        0        0     1854 2024-04-05 12:23:37.427259 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-about-team.svg
--rw-r--r--   0        0        0     2187 2024-04-05 12:23:37.426260 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-about-us-m.svg
--rw-r--r--   0        0        0     1924 2024-04-05 12:23:37.427259 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-about-us.svg
--rw-r--r--   0        0        0      695 2024-04-05 12:23:37.427259 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-alternator.svg
--rw-r--r--   0        0        0      588 2024-04-05 12:23:37.431260 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-apps.svg
--rw-r--r--   0        0        0     1264 2024-04-05 12:23:37.431260 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-architecture.svg
--rw-r--r--   0        0        0      616 2024-04-05 12:23:37.431260 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-benchmarks.svg
--rw-r--r--   0        0        0      579 2024-04-05 12:23:37.431260 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-blog.svg
--rw-r--r--   0        0        0      622 2024-04-05 12:23:37.432259 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-careers.svg
--rw-r--r--   0        0        0      219 2024-04-05 12:23:37.432259 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-chevron-left.svg
--rw-r--r--   0        0        0      196 2024-04-05 12:23:37.432259 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-chevron-right.svg
--rw-r--r--   0        0        0     1007 2024-04-05 12:23:37.432259 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-circe.svg
--rw-r--r--   0        0        0      324 2024-04-05 12:23:37.433258 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-clock.svg
--rw-r--r--   0        0        0     1263 2024-04-05 12:23:37.433258 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-close.svg
--rw-r--r--   0        0        0      642 2024-04-05 12:23:37.433258 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-cloud-docs.svg
--rw-r--r--   0        0        0      994 2024-04-05 12:23:37.433258 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-cloud.svg
--rw-r--r--   0        0        0     1344 2024-04-05 12:23:37.433258 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-comparison.svg
--rw-r--r--   0        0        0      702 2024-04-05 12:23:37.434258 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-contact-us.svg
--rw-r--r--   0        0        0      563 2024-04-05 12:23:37.434258 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-developers-blog.svg
--rw-r--r--   0        0        0      496 2024-04-05 12:23:37.435258 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-docs.svg
--rw-r--r--   0        0        0     1930 2024-04-05 12:23:37.435258 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-enterprise-m.svg
--rw-r--r--   0        0        0      847 2024-04-05 12:23:37.435258 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-enterprise.svg
--rw-r--r--   0        0        0     1142 2024-04-05 12:23:37.436259 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-events.svg
--rw-r--r--   0        0        0      935 2024-04-05 12:23:37.436259 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-exclamation.svg
--rw-r--r--   0        0        0     1590 2024-04-05 12:23:37.437265 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-expand.svg
--rw-r--r--   0        0        0      403 2024-04-05 12:23:37.437265 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-forum.svg
--rw-r--r--   0        0        0      345 2024-04-05 12:23:37.437265 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-getting-started.svg
--rw-r--r--   0        0        0      744 2024-04-05 12:23:37.437265 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-glossary.svg
--rw-r--r--   0        0        0      465 2024-04-05 12:23:37.437265 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-home.svg
--rw-r--r--   0        0        0      623 2024-04-05 12:23:37.438261 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-infoworld.svg
--rw-r--r--   0        0        0     1319 2024-04-05 12:23:37.438261 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-integrations.svg
--rw-r--r--   0        0        0      702 2024-04-05 12:23:37.438261 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-knowledge-base.svg
--rw-r--r--   0        0        0      971 2024-04-05 12:23:37.439258 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-less.svg
--rw-r--r--   0        0        0     1303 2024-04-05 12:23:37.439258 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-live-test.svg
--rw-r--r--   0        0        0      357 2024-04-05 12:23:37.440266 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-mail-list.svg
--rw-r--r--   0        0        0      710 2024-04-05 12:23:37.440266 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-manager.svg
--rw-r--r--   0        0        0     1372 2024-04-05 12:23:37.440266 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-memory-management.svg
--rw-r--r--   0        0        0      720 2024-04-05 12:23:37.441273 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-modeling.svg
--rw-r--r--   0        0        0      719 2024-04-05 12:23:37.441273 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-monitoring.svg
--rw-r--r--   0        0        0      809 2024-04-05 12:23:37.442264 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-networking.svg
--rw-r--r--   0        0        0      611 2024-04-05 12:23:37.442264 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-news.svg
--rw-r--r--   0        0        0      661 2024-04-05 12:23:37.442264 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-newsletter.svg
--rw-r--r--   0        0        0      635 2024-04-05 12:23:37.443267 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-nsql-guides.svg
--rw-r--r--   0        0        0     1258 2024-04-05 12:23:37.443267 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-open-source.svg
--rw-r--r--   0        0        0     3545 2024-04-05 12:23:37.443267 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-operator.svg
--rw-r--r--   0        0        0      712 2024-04-05 12:23:37.443267 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-overview.svg
--rw-r--r--   0        0        0      916 2024-04-05 12:23:37.444266 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-partners.svg
--rw-r--r--   0        0        0     1811 2024-04-05 12:23:37.444266 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-plus.svg
--rw-r--r--   0        0        0      631 2024-04-05 12:23:37.444266 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-pricing.svg
--rw-r--r--   0        0        0      749 2024-04-05 12:23:37.445267 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-release-notes.svg
--rw-r--r--   0        0        0     1054 2024-04-05 12:23:37.446265 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-resource-center.svg
--rw-r--r--   0        0        0      938 2024-04-05 12:23:37.446265 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-roadmap.svg
--rw-r--r--   0        0        0      434 2024-04-05 12:23:37.447265 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-search.svg
--rw-r--r--   0        0        0     1238 2024-04-05 12:23:37.447265 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-slack.svg
--rw-r--r--   0        0        0      763 2024-04-05 12:23:37.448265 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-stack-overflow.svg
--rw-r--r--   0        0        0      772 2024-04-05 12:23:37.448265 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-summit.svg
--rw-r--r--   0        0        0     1442 2024-04-05 12:23:37.448265 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-support.svg
--rw-r--r--   0        0        0      596 2024-04-05 12:23:37.449269 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-tech-talks.svg
--rw-r--r--   0        0        0      419 2024-04-05 12:23:37.449269 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-testing.svg
--rw-r--r--   0        0        0      374 2024-04-05 12:23:37.449269 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-thumbs-down.svg
--rw-r--r--   0        0        0      354 2024-04-05 12:23:37.449269 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-thumbs-up.svg
--rw-r--r--   0        0        0      672 2024-04-05 12:23:37.450268 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-tip.svg
--rw-r--r--   0        0        0      760 2024-04-05 12:23:37.451266 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-training.svg
--rw-r--r--   0        0        0      185 2024-04-05 12:23:37.451266 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-triangle-down.svg
--rw-r--r--   0        0        0      543 2024-04-05 12:23:37.452266 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-university.svg
--rw-r--r--   0        0        0     1493 2024-04-05 12:23:37.452266 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-users-blog.svg
--rw-r--r--   0        0        0     1769 2024-04-05 12:23:37.453267 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-warning.svg
--rw-r--r--   0        0        0      600 2024-04-05 12:23:37.453267 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-webinars.svg
--rw-r--r--   0        0        0      880 2024-04-05 12:23:37.453267 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-whitepapers.svg
--rw-r--r--   0        0        0      646 2024-04-05 12:23:37.453267 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-workshop.svg
--rw-r--r--   0        0        0    12897 2024-04-05 12:23:37.427259 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/logo-docs.svg
--rw-r--r--   0        0        0     6483 2024-04-05 12:23:37.427259 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/logo-scylla-horizontal-RGB.svg
--rw-r--r--   0        0        0    29400 2024-04-05 12:23:37.453267 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/mascots/404.jpg
--rw-r--r--   0        0        0    35624 2024-04-05 12:23:37.453267 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/mascots/scylla-3monsters.png
--rw-r--r--   0        0        0    67593 2024-04-05 12:23:37.453267 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/mascots/scylla-advisor-crystal.png
--rw-r--r--   0        0        0     5546 2024-04-05 12:23:37.453267 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/mascots/scylla-alternator.svg
--rw-r--r--   0        0        0     6383 2024-04-05 12:23:37.454777 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/mascots/scylla-cloud.svg
--rw-r--r--   0        0        0    44539 2024-04-05 12:23:37.454777 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/mascots/scylla-computer-3-monsters.png
--rw-r--r--   0        0        0    22297 2024-04-05 12:23:37.454777 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/mascots/scylla-computer-headset.png
--rw-r--r--   0        0        0    22675 2024-04-05 12:23:37.455789 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/mascots/scylla-cup-number-one.png
--rw-r--r--   0        0        0     5043 2024-04-05 12:23:37.455789 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/mascots/scylla-docs.svg
--rw-r--r--   0        0        0    17850 2024-04-05 12:23:37.456787 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/mascots/scylla-drivers.svg
--rw-r--r--   0        0        0    17439 2024-04-05 12:23:37.456787 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/mascots/scylla-enterprise.svg
--rw-r--r--   0        0        0    29196 2024-04-05 12:23:37.456787 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/mascots/scylla-forklift-boxes.png
--rw-r--r--   0        0        0    24191 2024-04-05 12:23:37.456787 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/mascots/scylla-forklift-migration.png
--rw-r--r--   0        0        0    64841 2024-04-05 12:23:37.457788 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/mascots/scylla-gear.png
--rw-r--r--   0        0        0    20163 2024-04-05 12:23:37.457788 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/mascots/scylla-hardhat.png
--rw-r--r--   0        0        0    40533 2024-04-05 12:23:37.457788 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/mascots/scylla-headband.png
--rw-r--r--   0        0        0    19094 2024-04-05 12:23:37.457788 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/mascots/scylla-headset.png
--rw-r--r--   0        0        0    22252 2024-04-05 12:23:37.458788 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/mascots/scylla-hearts.png
--rw-r--r--   0        0        0    70044 2024-04-05 12:23:37.458788 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/mascots/scylla-looking-down.png
--rw-r--r--   0        0        0    69083 2024-04-05 12:23:37.458788 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/mascots/scylla-looking-up.png
--rw-r--r--   0        0        0    17463 2024-04-05 12:23:37.459787 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/mascots/scylla-magnifying-glass-fronting.png
--rw-r--r--   0        0        0    16651 2024-04-05 12:23:37.459787 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/mascots/scylla-magnifying-glass.png
--rw-r--r--   0        0        0     8013 2024-04-05 12:23:37.460789 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/mascots/scylla-manager.svg
--rw-r--r--   0        0        0    15621 2024-04-05 12:23:37.460789 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/mascots/scylla-monitor.svg
--rw-r--r--   0        0        0    18439 2024-04-05 12:23:37.461789 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/mascots/scylla-movement-fast.png
--rw-r--r--   0        0        0    14720 2024-04-05 12:23:37.461789 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/mascots/scylla-movement.png
--rw-r--r--   0        0        0    33081 2024-04-05 12:23:37.461789 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/mascots/scylla-onpremise.png
--rw-r--r--   0        0        0     3712 2024-04-05 12:23:37.461789 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/mascots/scylla-opensource.svg
--rw-r--r--   0        0        0    10033 2024-04-05 12:23:37.462790 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/mascots/scylla-operator.svg
--rw-r--r--   0        0        0    52683 2024-04-05 12:23:37.461789 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/mascots/scylla-plugin.png
--rw-r--r--   0        0        0    31893 2024-04-05 12:23:37.462790 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/mascots/scylla-release-mascot.png
--rw-r--r--   0        0        0    21261 2024-04-05 12:23:37.462790 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/mascots/scylla-repair.png
--rw-r--r--   0        0        0    48529 2024-04-05 12:23:37.462790 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/mascots/scylla-server.png
--rw-r--r--   0        0        0    12942 2024-04-05 12:23:37.463788 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/mascots/scylla-sleeping.png
--rw-r--r--   0        0        0    18996 2024-04-05 12:23:37.464788 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/mascots/scylla-tall-measure.png
--rw-r--r--   0        0        0    26146 2024-04-05 12:23:37.464788 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/mascots/scylla-university.png
--rw-r--r--   0        0        0    40973 2024-04-05 12:23:37.465788 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/mascots/scylla-weights.png
--rw-r--r--   0        0        0    34761 2024-04-05 12:23:37.465788 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/mascots/scylla-window-cleaning.png
--rw-r--r--   0        0        0    18803 2024-04-05 12:23:37.465788 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/mascots/scylla-with-computer-2.png
--rw-r--r--   0        0        0    19926 2024-04-05 12:23:37.465788 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/mascots/scylla-with-computer.png
--rw-r--r--   0        0        0    45076 2024-04-05 12:23:37.465788 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/mascots/scylla-with-linux.png
--rw-r--r--   0        0        0    34449 2024-04-05 12:23:37.465788 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/mascots/scylla-writting.png
--rw-r--r--   0        0        0      284 2024-04-05 12:23:37.427259 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/menu.svg
--rw-r--r--   0        0        0   296001 2024-04-12 09:32:29.968247 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/js/main.bundle.js
--rw-r--r--   0        0        0     8876 2024-04-05 12:23:37.465788 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/js/main.bundle.js.LICENSE.txt
--rw-r--r--   0        0        0     1282 2024-04-05 12:23:37.426260 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/js/runtime.bundle.js
--rw-r--r--   0        0        0      865 2024-04-02 09:38:37.405825 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/theme.conf
--rw-r--r--   0        0        0      738 2024-04-02 09:38:37.406825 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/utils.py
--rw-r--r--   0        0        0      776 2022-03-15 17:17:19.871003 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/version-warning.html
--rw-r--r--   0        0        0     1365 2022-10-04 08:24:19.934941 sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/versions.html
--rw-r--r--   0        0        0     1081 1970-01-01 00:00:00.000000 sphinx_scylladb_theme-1.7.1/PKG-INFO
+-rw-r--r--   0        0        0    11338 2021-09-29 09:25:27.778592 sphinx_scylladb_theme-1.7.2/LICENSE
+-rw-r--r--   0        0        0      184 2022-12-09 15:36:29.292783 sphinx_scylladb_theme-1.7.2/PYPI.rst
+-rw-r--r--   0        0        0      950 2024-05-07 10:21:20.146732 sphinx_scylladb_theme-1.7.2/pyproject.toml
+-rw-r--r--   0        0        0     1220 2024-05-07 10:21:13.452437 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/404.html
+-rw-r--r--   0        0        0     3566 2024-05-07 10:21:13.453439 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/__init__.py
+-rw-r--r--   0        0        0       89 2024-05-07 10:21:13.454440 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/_version.py
+-rw-r--r--   0        0        0      734 2024-05-07 10:21:13.454440 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/breadcrumbs.html
+-rw-r--r--   0        0        0     1075 2022-02-09 11:51:08.094565 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/content-navigation.html
+-rw-r--r--   0        0        0     1131 2024-05-07 10:21:20.147729 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/contribute.html
+-rw-r--r--   0        0        0        0 2021-09-29 09:25:27.800533 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/extensions/__init__.py
+-rw-r--r--   0        0        0     4383 2024-05-07 10:21:13.456438 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/extensions/hero_box.py
+-rw-r--r--   0        0        0      999 2022-11-15 12:53:40.356983 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/extensions/labels.py
+-rw-r--r--   0        0        0     2952 2024-05-07 10:21:13.457438 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/extensions/multiversion.py
+-rw-r--r--   0        0        0     2797 2022-02-09 11:51:08.097564 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/extensions/navigation.py
+-rw-r--r--   0        0        0     1379 2022-10-07 12:02:26.581739 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/extensions/panel_box.py
+-rw-r--r--   0        0        0     4250 2024-05-07 10:21:13.458437 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/extensions/topic_box.py
+-rw-r--r--   0        0        0     1719 2024-05-07 10:21:13.459438 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/extensions/utils.py
+-rw-r--r--   0        0        0      783 2024-05-07 10:21:13.459438 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/extensions/validations.py
+-rw-r--r--   0        0        0     3076 2024-05-07 10:21:20.149729 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/feedback.html
+-rw-r--r--   0        0        0     3232 2024-05-07 10:21:13.461438 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/footer.html
+-rw-r--r--   0        0        0     4057 2024-05-07 10:21:13.462439 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/header.html
+-rw-r--r--   0        0        0      219 2022-02-09 11:51:08.101577 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/last-updated.html
+-rw-r--r--   0        0        0     5851 2024-05-07 10:21:13.463444 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/layout.html
+-rw-r--r--   0        0        0        0 2022-02-09 11:52:03.175492 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/lexers/__init__.py
+-rw-r--r--   0        0        0     6754 2021-09-29 09:25:27.805520 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/lexers/cql.py
+-rw-r--r--   0        0        0       84 2021-09-29 09:25:27.805520 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/lexers/ditaa.py
+-rw-r--r--   0        0        0       25 2024-05-07 10:21:13.464439 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/local-scripts.html
+-rw-r--r--   0        0        0       27 2024-05-07 10:21:13.464439 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/notice.html
+-rw-r--r--   0        0        0      802 2024-05-07 10:21:13.465438 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/promo-banner.html
+-rw-r--r--   0        0        0     1588 2024-05-07 10:21:13.465438 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/scylladb-scripts.html
+-rw-r--r--   0        0        0      275 2022-03-29 08:31:29.866817 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/secondary-side-nav.html
+-rw-r--r--   0        0        0      186 2022-02-09 11:51:08.103844 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/side-nav-toggle.html
+-rw-r--r--   0        0        0      962 2024-05-07 10:21:13.466439 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/side-nav.html
+-rw-r--r--   0        0        0   226508 2024-05-07 10:21:13.469439 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/css/main.css
+-rw-r--r--   0        0        0        0 2024-04-30 14:12:22.044104 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/.gitkeep
+-rw-r--r--   0        0        0      635 2024-04-30 14:12:22.048102 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/banner-background.svg
+-rw-r--r--   0        0        0     4428 2024-04-30 14:12:22.048102 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/favicon-228x228.png
+-rw-r--r--   0        0        0      837 2024-04-30 14:12:22.048102 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/favicon-32x32.png
+-rw-r--r--   0        0        0     1150 2024-04-30 14:12:22.048102 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/favicon.ico
+-rw-r--r--   0        0        0     1854 2024-04-30 14:12:22.048102 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-about-team.svg
+-rw-r--r--   0        0        0     2187 2024-05-07 10:21:13.470437 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-about-us-m.svg
+-rw-r--r--   0        0        0     1924 2024-05-07 10:21:13.470437 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-about-us.svg
+-rw-r--r--   0        0        0      695 2024-05-07 10:21:13.471439 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-alternator.svg
+-rw-r--r--   0        0        0      588 2024-04-30 14:12:22.051103 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-apps.svg
+-rw-r--r--   0        0        0     1264 2024-04-30 14:12:22.052104 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-architecture.svg
+-rw-r--r--   0        0        0      616 2024-04-30 14:12:22.052104 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-benchmarks.svg
+-rw-r--r--   0        0        0      579 2024-04-30 14:12:22.052104 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-blog.svg
+-rw-r--r--   0        0        0      622 2024-04-30 14:12:22.052104 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-careers.svg
+-rw-r--r--   0        0        0      219 2024-04-30 14:12:22.053105 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-chevron-left.svg
+-rw-r--r--   0        0        0      196 2024-04-30 14:12:22.053105 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-chevron-right.svg
+-rw-r--r--   0        0        0     1007 2024-04-30 14:12:22.053105 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-circe.svg
+-rw-r--r--   0        0        0      324 2024-04-30 14:12:22.053105 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-clock.svg
+-rw-r--r--   0        0        0     1263 2024-04-30 14:12:22.053105 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-close.svg
+-rw-r--r--   0        0        0      642 2024-04-30 14:12:22.054104 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-cloud-docs.svg
+-rw-r--r--   0        0        0      994 2024-05-07 10:21:13.471439 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-cloud.svg
+-rw-r--r--   0        0        0     1344 2024-04-30 14:12:22.054104 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-comparison.svg
+-rw-r--r--   0        0        0      702 2024-04-30 14:12:22.055104 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-contact-us.svg
+-rw-r--r--   0        0        0      563 2024-04-30 14:12:22.055104 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-developers-blog.svg
+-rw-r--r--   0        0        0      496 2024-04-30 14:12:22.057104 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-docs.svg
+-rw-r--r--   0        0        0     1930 2024-05-07 10:21:13.472439 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-enterprise-m.svg
+-rw-r--r--   0        0        0      847 2024-05-07 10:21:13.472439 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-enterprise.svg
+-rw-r--r--   0        0        0     1142 2024-04-30 14:12:22.057104 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-events.svg
+-rw-r--r--   0        0        0      935 2024-04-30 14:12:22.057104 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-exclamation.svg
+-rw-r--r--   0        0        0     1590 2024-04-30 14:12:22.057104 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-expand.svg
+-rw-r--r--   0        0        0      403 2024-04-30 14:12:22.058104 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-forum.svg
+-rw-r--r--   0        0        0      345 2024-04-30 14:12:22.058104 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-getting-started.svg
+-rw-r--r--   0        0        0      744 2024-04-30 14:12:22.058104 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-glossary.svg
+-rw-r--r--   0        0        0      465 2024-04-30 14:12:22.058104 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-home.svg
+-rw-r--r--   0        0        0      623 2024-04-30 14:12:22.059104 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-infoworld.svg
+-rw-r--r--   0        0        0     1319 2024-04-30 14:12:22.059104 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-integrations.svg
+-rw-r--r--   0        0        0      702 2024-04-30 14:12:22.059104 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-knowledge-base.svg
+-rw-r--r--   0        0        0      971 2024-04-30 14:12:22.060103 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-less.svg
+-rw-r--r--   0        0        0     1303 2024-04-30 14:12:22.060103 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-live-test.svg
+-rw-r--r--   0        0        0      357 2024-04-30 14:12:22.061106 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-mail-list.svg
+-rw-r--r--   0        0        0      710 2024-04-30 14:12:22.061106 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-manager.svg
+-rw-r--r--   0        0        0     1372 2024-04-30 14:12:22.061106 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-memory-management.svg
+-rw-r--r--   0        0        0      720 2024-04-30 14:12:22.061106 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-modeling.svg
+-rw-r--r--   0        0        0      719 2024-04-30 14:12:22.062105 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-monitoring.svg
+-rw-r--r--   0        0        0      809 2024-04-30 14:12:22.062105 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-networking.svg
+-rw-r--r--   0        0        0      611 2024-04-30 14:12:22.063104 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-news.svg
+-rw-r--r--   0        0        0      661 2024-04-30 14:12:22.063104 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-newsletter.svg
+-rw-r--r--   0        0        0      635 2024-04-30 14:12:22.064104 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-nsql-guides.svg
+-rw-r--r--   0        0        0     1258 2024-04-30 14:12:22.063104 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-open-source.svg
+-rw-r--r--   0        0        0     3545 2024-05-07 10:21:13.473439 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-operator.svg
+-rw-r--r--   0        0        0      712 2024-04-30 14:12:22.064104 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-overview.svg
+-rw-r--r--   0        0        0      916 2024-04-30 14:12:22.065104 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-partners.svg
+-rw-r--r--   0        0        0     1811 2024-04-30 14:12:22.065104 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-plus.svg
+-rw-r--r--   0        0        0      631 2024-04-30 14:12:22.066105 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-pricing.svg
+-rw-r--r--   0        0        0      749 2024-04-30 14:12:22.066105 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-release-notes.svg
+-rw-r--r--   0        0        0     1054 2024-04-30 14:12:22.066105 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-resource-center.svg
+-rw-r--r--   0        0        0      938 2024-04-30 14:12:22.066105 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-roadmap.svg
+-rw-r--r--   0        0        0      434 2024-04-30 14:12:22.067105 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-search.svg
+-rw-r--r--   0        0        0     1238 2024-04-30 14:12:22.067105 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-slack.svg
+-rw-r--r--   0        0        0      763 2024-04-30 14:12:22.068104 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-stack-overflow.svg
+-rw-r--r--   0        0        0      772 2024-04-30 14:12:22.068104 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-summit.svg
+-rw-r--r--   0        0        0     1442 2024-04-30 14:12:22.068104 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-support.svg
+-rw-r--r--   0        0        0      596 2024-04-30 14:12:22.068104 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-tech-talks.svg
+-rw-r--r--   0        0        0      419 2024-04-30 14:12:22.069104 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-testing.svg
+-rw-r--r--   0        0        0      374 2024-05-07 10:21:13.473439 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-thumbs-down.svg
+-rw-r--r--   0        0        0      354 2024-05-07 10:21:13.474439 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-thumbs-up.svg
+-rw-r--r--   0        0        0      672 2024-04-30 14:12:22.070104 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-tip.svg
+-rw-r--r--   0        0        0      760 2024-04-30 14:12:22.070104 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-training.svg
+-rw-r--r--   0        0        0      185 2024-04-30 14:12:22.071105 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-triangle-down.svg
+-rw-r--r--   0        0        0      543 2024-04-30 14:12:22.071105 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-university.svg
+-rw-r--r--   0        0        0     1493 2024-04-30 14:12:22.071105 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-users-blog.svg
+-rw-r--r--   0        0        0     1769 2024-04-30 14:12:22.071105 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-warning.svg
+-rw-r--r--   0        0        0      600 2024-04-30 14:12:22.072105 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-webinars.svg
+-rw-r--r--   0        0        0      880 2024-04-30 14:12:22.072105 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-whitepapers.svg
+-rw-r--r--   0        0        0      646 2024-04-30 14:12:22.072105 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-workshop.svg
+-rw-r--r--   0        0        0    12897 2024-04-30 14:12:22.048102 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/logo-docs.svg
+-rw-r--r--   0        0        0     6483 2024-04-30 14:12:22.048102 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/logo-scylla-horizontal-RGB.svg
+-rw-r--r--   0        0        0    29400 2024-04-30 14:12:22.072105 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/mascots/404.jpg
+-rw-r--r--   0        0        0    35624 2024-04-30 14:12:22.072105 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/mascots/scylla-3monsters.png
+-rw-r--r--   0        0        0    67593 2024-04-30 14:12:22.073105 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/mascots/scylla-advisor-crystal.png
+-rw-r--r--   0        0        0     5546 2024-04-30 14:12:22.073105 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/mascots/scylla-alternator.svg
+-rw-r--r--   0        0        0     6383 2024-04-30 14:12:22.073105 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/mascots/scylla-cloud.svg
+-rw-r--r--   0        0        0    44539 2024-04-30 14:12:22.074107 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/mascots/scylla-computer-3-monsters.png
+-rw-r--r--   0        0        0    22297 2024-04-30 14:12:22.075106 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/mascots/scylla-computer-headset.png
+-rw-r--r--   0        0        0    22675 2024-04-30 14:12:22.075106 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/mascots/scylla-cup-number-one.png
+-rw-r--r--   0        0        0     5043 2024-04-30 14:12:22.075106 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/mascots/scylla-docs.svg
+-rw-r--r--   0        0        0    17850 2024-04-30 14:12:22.075106 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/mascots/scylla-drivers.svg
+-rw-r--r--   0        0        0    17439 2024-04-30 14:12:22.076104 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/mascots/scylla-enterprise.svg
+-rw-r--r--   0        0        0    29196 2024-04-30 14:12:22.076104 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/mascots/scylla-forklift-boxes.png
+-rw-r--r--   0        0        0    24191 2024-04-30 14:12:22.076104 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/mascots/scylla-forklift-migration.png
+-rw-r--r--   0        0        0    64841 2024-04-30 14:12:22.077106 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/mascots/scylla-gear.png
+-rw-r--r--   0        0        0    20163 2024-04-30 14:12:22.077106 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/mascots/scylla-hardhat.png
+-rw-r--r--   0        0        0    40533 2024-04-30 14:12:22.077106 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/mascots/scylla-headband.png
+-rw-r--r--   0        0        0    19094 2024-04-30 14:12:22.078107 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/mascots/scylla-headset.png
+-rw-r--r--   0        0        0    22252 2024-04-30 14:12:22.078107 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/mascots/scylla-hearts.png
+-rw-r--r--   0        0        0    70044 2024-04-30 14:12:22.078107 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/mascots/scylla-looking-down.png
+-rw-r--r--   0        0        0    69083 2024-04-30 14:12:22.080107 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/mascots/scylla-looking-up.png
+-rw-r--r--   0        0        0    17463 2024-04-30 14:12:22.080107 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/mascots/scylla-magnifying-glass-fronting.png
+-rw-r--r--   0        0        0    16651 2024-04-30 14:12:22.080107 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/mascots/scylla-magnifying-glass.png
+-rw-r--r--   0        0        0     8013 2024-04-30 14:12:22.080107 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/mascots/scylla-manager.svg
+-rw-r--r--   0        0        0    15621 2024-04-30 14:12:22.080107 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/mascots/scylla-monitor.svg
+-rw-r--r--   0        0        0    18439 2024-04-30 14:12:22.080107 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/mascots/scylla-movement-fast.png
+-rw-r--r--   0        0        0    14720 2024-04-30 14:12:22.080107 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/mascots/scylla-movement.png
+-rw-r--r--   0        0        0    33081 2024-04-30 14:12:22.081105 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/mascots/scylla-onpremise.png
+-rw-r--r--   0        0        0     3712 2024-04-30 14:12:22.081105 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/mascots/scylla-opensource.svg
+-rw-r--r--   0        0        0    10033 2024-04-30 14:12:22.082104 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/mascots/scylla-operator.svg
+-rw-r--r--   0        0        0    52683 2024-04-30 14:12:22.083104 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/mascots/scylla-plugin.png
+-rw-r--r--   0        0        0    31893 2024-04-30 14:12:22.083104 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/mascots/scylla-release-mascot.png
+-rw-r--r--   0        0        0    21261 2024-04-30 14:12:22.083104 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/mascots/scylla-repair.png
+-rw-r--r--   0        0        0    48529 2024-04-30 14:12:22.083104 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/mascots/scylla-server.png
+-rw-r--r--   0        0        0    12942 2024-04-30 14:12:22.085106 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/mascots/scylla-sleeping.png
+-rw-r--r--   0        0        0    18996 2024-04-30 14:12:22.086106 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/mascots/scylla-tall-measure.png
+-rw-r--r--   0        0        0    26146 2024-04-30 14:12:22.086106 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/mascots/scylla-university.png
+-rw-r--r--   0        0        0    40973 2024-04-30 14:12:22.086106 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/mascots/scylla-weights.png
+-rw-r--r--   0        0        0    34761 2024-04-30 14:12:22.086106 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/mascots/scylla-window-cleaning.png
+-rw-r--r--   0        0        0    18803 2024-04-30 14:12:22.086106 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/mascots/scylla-with-computer-2.png
+-rw-r--r--   0        0        0    19926 2024-04-30 14:12:22.086106 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/mascots/scylla-with-computer.png
+-rw-r--r--   0        0        0    45076 2024-04-30 14:12:22.086106 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/mascots/scylla-with-linux.png
+-rw-r--r--   0        0        0    34449 2024-04-30 14:12:22.087106 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/mascots/scylla-writting.png
+-rw-r--r--   0        0        0      284 2024-04-30 14:12:22.049105 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/menu.svg
+-rw-r--r--   0        0        0   296049 2024-05-07 10:21:20.153727 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/js/main.bundle.js
+-rw-r--r--   0        0        0     8876 2024-04-30 14:12:22.086106 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/js/main.bundle.js.LICENSE.txt
+-rw-r--r--   0        0        0     1282 2024-04-30 14:12:22.047103 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/js/runtime.bundle.js
+-rw-r--r--   0        0        0      892 2024-05-07 10:21:20.154729 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/theme.conf
+-rw-r--r--   0        0        0      738 2024-05-07 10:21:13.478440 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/utils.py
+-rw-r--r--   0        0        0      776 2022-03-15 17:17:19.871003 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/version-warning.html
+-rw-r--r--   0        0        0     1365 2022-10-04 08:24:19.934941 sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/versions.html
+-rw-r--r--   0        0        0     1081 1970-01-01 00:00:00.000000 sphinx_scylladb_theme-1.7.2/PKG-INFO
```

### Comparing `sphinx_scylladb_theme-1.7.1/LICENSE` & `sphinx_scylladb_theme-1.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/pyproject.toml` & `sphinx_scylladb_theme-1.7.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sphinx-scylladb-theme"
-version = "1.7.1"
+version = "1.7.2"
 description = "A Sphinx Theme for ScyllaDB documentation projects"
 authors = ["David García <hi@davidgarcia.dev>"]
 exclude = [".github", "config", "docs", "extensions", ".postcss.config.js", ".prettierrc.json", "deploy.sh", "src", "package.json", "package-lock.json"]
 readme = "PYPI.rst"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/404.html` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/404.html`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/__init__.py` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/breadcrumbs.html` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/breadcrumbs.html`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/content-navigation.html` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/content-navigation.html`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/contribute.html` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/contribute.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 {% if theme_github_repository %}
     <ul class="contribute">
         <li class="contribute__item">
-            <a href="https://github.com/{{ theme_github_issues_repository}}/issues/new?title=docs:%20Issue on page {{ title|striptags|e }}&&body=I%20would%20like%20to%20report%20an%20issue%20on%20page%20{{html_baseurl}}/{% if versions and current_version %}{{ current_version.name }}/{% endif %}{{ pagename }}%0A%0A%23%23%23%20Problem%0A%0A%23%23%23%20%20Suggest%20a%20fix&labels=documentation"
+            <a href="https://github.com/{{ theme_github_issues_repository}}/issues/new?title=docs:%20Issue on page {{ title|striptags|e }}&&body=I%20would%20like%20to%20report%20an%20issue%20on%20page%20{{html_baseurl}}/{% if versions and current_version %}{{ current_version.name }}/{% endif %}{{ pagename }}%0A%0A%23%23%23%20Problem%0A%0A%23%23%23%20%20Suggest%20a%20fix&labels={{theme_github_label}}"
                target="_blank">
                 <i class="icon fab fa-github" aria-hidden="true"></i>Create an issue
             </a>
         </li>
         {% if theme_hide_edit_this_page_button|lower == 'false'%}
             <li class="contribute__item">
                 <a href="https://github.com/{{ theme_github_repository }}/edit/{{ theme_default_branch }}/{{ theme_conf_py_path }}{{ pagename }}{{ page_source_suffix }}"
```

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/extensions/hero_box.py` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/extensions/hero_box.py`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/extensions/labels.py` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/extensions/labels.py`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/extensions/multiversion.py` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/extensions/multiversion.py`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/extensions/navigation.py` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/extensions/navigation.py`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/extensions/panel_box.py` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/extensions/panel_box.py`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/extensions/topic_box.py` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/extensions/topic_box.py`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/extensions/utils.py` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/extensions/utils.py`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/extensions/validations.py` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/extensions/validations.py`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/feedback.html` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/feedback.html`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         }
 
         function showMessage(liked) {
             const feedbackMessage = document.getElementById('feedback-message');
             const themeGithubRepository = {% if theme_github_repository %}true{% else %}false{% endif %};
             let message = 'Great! Thanks for your feedback.';
             if (themeGithubRepository && !liked) {
-                message = "Thanks for your feedback! Please don't hesitate to <a href='https://github.com/{{ theme_github_issues_repository}}/issues/new?title=docs:%20Issue on page {{ title|striptags|e }}&&body=I%20would%20like%20to%20report%20an%20issue%20on%20page%20{{html_baseurl}}/{% if versions and current_version %}{{ current_version.name }}/{% endif %}{{ pagename }}%0A%0A%23%23%23%20Problem%0A%0A%23%23%23%20%20Suggest%20a%20fix&labels=documentation'>create an issue</a> if you have any suggestions on how we can improve.";
+                message = "Thanks for your feedback! Please don't hesitate to <a href='https://github.com/{{ theme_github_issues_repository}}/issues/new?title=docs:%20Issue on page {{ title|striptags|e }}&&body=I%20would%20like%20to%20report%20an%20issue%20on%20page%20{{html_baseurl}}/{% if versions and current_version %}{{ current_version.name }}/{% endif %}{{ pagename }}%0A%0A%23%23%23%20Problem%0A%0A%23%23%23%20%20Suggest%20a%20fix&labels={{theme_github_label}}'>create an issue</a> if you have any suggestions on how we can improve.";
             }
             feedbackMessage.innerHTML = message;
         }
 
         function sendGaEvent(liked) {
             const event_label = liked ? "positive" : "negative";
             const event = "feedback_" + event_label;
```

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/footer.html` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/footer.html`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/header.html` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/header.html`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/layout.html` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/layout.html`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/lexers/cql.py` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/lexers/cql.py`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/promo-banner.html` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/promo-banner.html`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/scylladb-scripts.html` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/scylladb-scripts.html`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/side-nav.html` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/side-nav.html`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/css/main.css` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/css/main.css`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/banner-background.svg` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/banner-background.svg`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/favicon-228x228.png` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/favicon-228x228.png`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/favicon-32x32.png` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/favicon.ico` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-about-team.svg` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-about-team.svg`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-about-us-m.svg` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-about-us-m.svg`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-about-us.svg` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-about-us.svg`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-alternator.svg` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-alternator.svg`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-apps.svg` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-apps.svg`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-architecture.svg` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-architecture.svg`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-benchmarks.svg` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-benchmarks.svg`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-blog.svg` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-blog.svg`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-careers.svg` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-careers.svg`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-circe.svg` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-circe.svg`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-close.svg` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-close.svg`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-cloud-docs.svg` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-cloud-docs.svg`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-cloud.svg` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-cloud.svg`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-comparison.svg` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-comparison.svg`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-contact-us.svg` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-contact-us.svg`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-developers-blog.svg` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-developers-blog.svg`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-enterprise-m.svg` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-enterprise-m.svg`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-enterprise.svg` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-enterprise.svg`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-events.svg` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-events.svg`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-exclamation.svg` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-exclamation.svg`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-expand.svg` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-expand.svg`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-glossary.svg` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-glossary.svg`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-infoworld.svg` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-infoworld.svg`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-integrations.svg` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-integrations.svg`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-knowledge-base.svg` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-knowledge-base.svg`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-less.svg` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-less.svg`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-live-test.svg` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-live-test.svg`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-manager.svg` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-manager.svg`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-memory-management.svg` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-memory-management.svg`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-modeling.svg` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-modeling.svg`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-monitoring.svg` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-monitoring.svg`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-networking.svg` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-networking.svg`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-news.svg` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-news.svg`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-newsletter.svg` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-newsletter.svg`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-nsql-guides.svg` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-nsql-guides.svg`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-open-source.svg` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-open-source.svg`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-operator.svg` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-operator.svg`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-overview.svg` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-overview.svg`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-partners.svg` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-partners.svg`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-plus.svg` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-plus.svg`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-pricing.svg` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-pricing.svg`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-release-notes.svg` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-release-notes.svg`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-resource-center.svg` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-resource-center.svg`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-roadmap.svg` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-roadmap.svg`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-slack.svg` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-slack.svg`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-stack-overflow.svg` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-stack-overflow.svg`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-summit.svg` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-summit.svg`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-support.svg` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-support.svg`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-tech-talks.svg` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-tech-talks.svg`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-tip.svg` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-tip.svg`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-training.svg` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-training.svg`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-university.svg` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-university.svg`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-users-blog.svg` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-users-blog.svg`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-warning.svg` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-warning.svg`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-webinars.svg` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-webinars.svg`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-whitepapers.svg` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-whitepapers.svg`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/icons/icon-workshop.svg` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/icons/icon-workshop.svg`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/logo-docs.svg` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/logo-docs.svg`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/logo-scylla-horizontal-RGB.svg` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/logo-scylla-horizontal-RGB.svg`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/mascots/404.jpg` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/mascots/404.jpg`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/mascots/scylla-3monsters.png` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/mascots/scylla-3monsters.png`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/mascots/scylla-advisor-crystal.png` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/mascots/scylla-advisor-crystal.png`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/mascots/scylla-alternator.svg` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/mascots/scylla-alternator.svg`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/mascots/scylla-cloud.svg` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/mascots/scylla-cloud.svg`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/mascots/scylla-computer-3-monsters.png` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/mascots/scylla-computer-3-monsters.png`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/mascots/scylla-computer-headset.png` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/mascots/scylla-computer-headset.png`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/mascots/scylla-cup-number-one.png` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/mascots/scylla-cup-number-one.png`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/mascots/scylla-docs.svg` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/mascots/scylla-docs.svg`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/mascots/scylla-drivers.svg` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/mascots/scylla-drivers.svg`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/mascots/scylla-enterprise.svg` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/mascots/scylla-enterprise.svg`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/mascots/scylla-forklift-boxes.png` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/mascots/scylla-forklift-boxes.png`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/mascots/scylla-forklift-migration.png` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/mascots/scylla-forklift-migration.png`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/mascots/scylla-gear.png` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/mascots/scylla-gear.png`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/mascots/scylla-hardhat.png` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/mascots/scylla-hardhat.png`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/mascots/scylla-headband.png` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/mascots/scylla-headband.png`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/mascots/scylla-headset.png` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/mascots/scylla-headset.png`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/mascots/scylla-hearts.png` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/mascots/scylla-hearts.png`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/mascots/scylla-looking-down.png` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/mascots/scylla-looking-down.png`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/mascots/scylla-looking-up.png` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/mascots/scylla-looking-up.png`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/mascots/scylla-magnifying-glass-fronting.png` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/mascots/scylla-magnifying-glass-fronting.png`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/mascots/scylla-magnifying-glass.png` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/mascots/scylla-magnifying-glass.png`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/mascots/scylla-manager.svg` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/mascots/scylla-manager.svg`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/mascots/scylla-monitor.svg` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/mascots/scylla-monitor.svg`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/mascots/scylla-movement-fast.png` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/mascots/scylla-movement-fast.png`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/mascots/scylla-movement.png` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/mascots/scylla-movement.png`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/mascots/scylla-onpremise.png` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/mascots/scylla-onpremise.png`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/mascots/scylla-opensource.svg` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/mascots/scylla-opensource.svg`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/mascots/scylla-operator.svg` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/mascots/scylla-operator.svg`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/mascots/scylla-plugin.png` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/mascots/scylla-plugin.png`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/mascots/scylla-release-mascot.png` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/mascots/scylla-release-mascot.png`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/mascots/scylla-repair.png` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/mascots/scylla-repair.png`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/mascots/scylla-server.png` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/mascots/scylla-server.png`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/mascots/scylla-sleeping.png` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/mascots/scylla-sleeping.png`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/mascots/scylla-tall-measure.png` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/mascots/scylla-tall-measure.png`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/mascots/scylla-university.png` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/mascots/scylla-university.png`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/mascots/scylla-weights.png` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/mascots/scylla-weights.png`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/mascots/scylla-window-cleaning.png` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/mascots/scylla-window-cleaning.png`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/mascots/scylla-with-computer-2.png` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/mascots/scylla-with-computer-2.png`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/mascots/scylla-with-computer.png` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/mascots/scylla-with-computer.png`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/mascots/scylla-with-linux.png` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/mascots/scylla-with-linux.png`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/img/mascots/scylla-writting.png` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/img/mascots/scylla-writting.png`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/js/main.bundle.js` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/js/main.bundle.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -9853,16 +9853,19 @@
                             if (!e) return null;
                             var n = JSON.parse(e);
                             return (new Date).getTime() > n.expiry ? (localStorage.removeItem(t), null) : n.value
                         }
                     }, {
                         key: "adjustScrollPaddingTop",
                         value: function() {
-                            var t = (p(".header").outerHeight() || 0) + (p(".promo-banner").outerHeight() || 0) + 10;
-                            p("html").css("scroll-padding-top", t + "px")
+                            var t = p(".header").outerHeight() || 0,
+                                e = 0;
+                            p(".promo-banner").is(":visible") && (e = p(".promo-banner").outerHeight());
+                            var n = t + e + 10;
+                            p("html").css("scroll-padding-top", n + "px")
                         }
                     }, {
                         key: "initBanner",
                         value: function() {
                             var t = p(".promo-banner"),
                                 e = t.outerHeight(),
                                 n = !1,
@@ -10000,15 +10003,15 @@
                         key: "onScrollHighlightSecondarySidebar",
                         value: function() {
                             var t = y(".content").find("h2").parent();
                             y(window).scroll((function() {
                                 var e = parseInt(y("html").css("scroll-padding-top")),
                                     n = y(this).scrollTop() + e;
                                 t.each((function() {
-                                    if (y(this).offset().top <= n) {
+                                    if (y(this).offset().top - 1 <= n) {
                                         var t = y(this).attr("id");
                                         y(".secondary-side-nav a").removeClass("current"), y('.secondary-side-nav a[href="#' + t + '"]').addClass("current")
                                     }
                                 }))
                             }))
                         }
                     }, {
```

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/js/main.bundle.js.LICENSE.txt` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/js/main.bundle.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/static/js/runtime.bundle.js` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/static/js/runtime.bundle.js`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/theme.conf` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/theme.conf`

 * *Files 13% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 banner_icon_path =
 branch_substring_removed = branch-
 collapse_navigation = false
 conf_py_path= docs/source/
 default_branch=master
 github_issues_repository = scylladb/scylla-doc-issues
 github_repository=
+github_label=documentation
 hide_banner = true
 hide_feedback_buttons = true
 hide_edit_this_page_button = true
 hide_version_dropdown =
 hide_versions_dropdown =
 navigation_depth= -1
 site_description = ScyllaDB is an Apache Cassandra-compatible NoSQL data store that can handle 1 million transactions per second on a single server.
```

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/utils.py` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/utils.py`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/version-warning.html` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/version-warning.html`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/sphinx_scylladb_theme/versions.html` & `sphinx_scylladb_theme-1.7.2/sphinx_scylladb_theme/versions.html`

 * *Files identical despite different names*

### Comparing `sphinx_scylladb_theme-1.7.1/PKG-INFO` & `sphinx_scylladb_theme-1.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-scylladb-theme
-Version: 1.7.1
+Version: 1.7.2
 Summary: A Sphinx Theme for ScyllaDB documentation projects
 Author: David García
 Author-email: hi@davidgarcia.dev
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

