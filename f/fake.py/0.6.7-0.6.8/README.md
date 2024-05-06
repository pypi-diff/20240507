# Comparing `tmp/fake.py-0.6.7.tar.gz` & `tmp/fake_py-0.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fake.py-0.6.7.tar", last modified: Tue Jan 16 23:35:13 2024, max compression
+gzip compressed data, was "fake_py-0.6.8.tar", last modified: Mon May  6 22:26:42 2024, max compression
```

## Comparing `fake.py-0.6.7.tar` & `fake_py-0.6.8.tar`

### file list

```diff
@@ -1,189 +1,189 @@
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-01-16 23:35:13.263383 fake.py-0.6.7/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       29 2022-12-17 15:38:13.000000 fake.py-0.6.7/.coveralls.yml
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       34 2022-12-17 15:38:13.000000 fake.py-0.6.7/.env
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-01-16 23:35:13.203382 fake.py-0.6.7/.github/
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-01-16 23:35:13.215382 fake.py-0.6.7/.github/workflows/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)    11430 2023-12-11 23:32:41.000000 fake.py-0.6.7/.github/workflows/test.yml
--rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      611 2023-12-16 00:28:30.000000 fake.py-0.6.7/.gitignore
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1422 2023-11-24 22:03:33.000000 fake.py-0.6.7/.pre-commit-config.yaml
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      361 2022-12-27 21:29:13.000000 fake.py-0.6.7/.pre-commit-hooks.yaml
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1020 2023-11-24 23:49:27.000000 fake.py-0.6.7/.readthedocs.yaml
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2588 2023-12-17 23:22:17.000000 fake.py-0.6.7/.secrets.baseline
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2540 2024-01-16 23:35:00.000000 fake.py-0.6.7/CHANGELOG.rst
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     5397 2023-12-01 00:01:18.000000 fake.py-0.6.7/CODE_OF_CONDUCT.md
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     5397 2023-12-01 00:01:18.000000 fake.py-0.6.7/CODE_OF_CONDUCT.rst
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     4070 2023-12-11 23:32:41.000000 fake.py-0.6.7/CONTRIBUTING.rst
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1073 2023-11-01 19:30:30.000000 fake.py-0.6.7/LICENSE
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     4230 2024-01-16 23:35:00.000000 fake.py-0.6.7/Makefile
--rw-r--r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)    12567 2024-01-16 23:35:13.263383 fake.py-0.6.7/PKG-INFO
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)    10529 2023-12-29 00:35:45.000000 fake.py-0.6.7/README.rst
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1378 2023-12-09 00:44:20.000000 fake.py-0.6.7/SECURITY.md
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1378 2023-12-09 00:44:20.000000 fake.py-0.6.7/SECURITY.rst
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)   146229 2024-01-16 23:35:00.000000 fake.py-0.6.7/__copy_fake.py
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-01-16 23:35:13.219382 fake.py-0.6.7/docs/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      634 2023-11-25 21:31:30.000000 fake.py-0.6.7/docs/Makefile
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-01-16 23:35:13.203382 fake.py-0.6.7/docs/_static/
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-01-16 23:35:13.207382 fake.py-0.6.7/docs/_static/examples/
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-01-16 23:35:13.223382 fake.py-0.6.7/docs/_static/examples/creating_docx/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       50 2023-12-03 00:58:59.000000 fake.py-0.6.7/docs/_static/examples/creating_docx/docx_bytes_1.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       87 2023-12-03 00:58:59.000000 fake.py-0.6.7/docs/_static/examples/creating_docx/docx_bytes_2.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       62 2023-12-03 00:58:59.000000 fake.py-0.6.7/docs/_static/examples/creating_docx/docx_bytes_3.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       54 2023-12-03 00:58:59.000000 fake.py-0.6.7/docs/_static/examples/creating_docx/docx_file_1.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       91 2023-12-03 00:58:59.000000 fake.py-0.6.7/docs/_static/examples/creating_docx/docx_file_2.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       66 2023-12-03 00:58:59.000000 fake.py-0.6.7/docs/_static/examples/creating_docx/docx_file_3.py
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-01-16 23:35:13.223382 fake.py-0.6.7/docs/_static/examples/creating_images/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       48 2023-12-03 00:58:59.000000 fake.py-0.6.7/docs/_static/examples/creating_images/png_bytes_1.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       86 2023-12-03 00:58:59.000000 fake.py-0.6.7/docs/_static/examples/creating_images/png_bytes_2.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       52 2023-12-03 00:58:59.000000 fake.py-0.6.7/docs/_static/examples/creating_images/png_file_1.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       90 2023-12-03 00:58:59.000000 fake.py-0.6.7/docs/_static/examples/creating_images/png_file_2.py
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-01-16 23:35:13.227383 fake.py-0.6.7/docs/_static/examples/creating_pdf/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       98 2023-12-01 00:01:18.000000 fake.py-0.6.7/docs/_static/examples/creating_pdf/graphic_pdf_bytes_1.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      112 2023-12-01 00:01:18.000000 fake.py-0.6.7/docs/_static/examples/creating_pdf/graphic_pdf_bytes_2.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      102 2023-12-01 00:01:18.000000 fake.py-0.6.7/docs/_static/examples/creating_pdf/graphic_pdf_file_1.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      116 2023-12-01 00:01:18.000000 fake.py-0.6.7/docs/_static/examples/creating_pdf/graphic_pdf_file_2.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       92 2023-12-01 00:01:18.000000 fake.py-0.6.7/docs/_static/examples/creating_pdf/text_pdf_bytes_1.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      131 2023-12-01 00:01:18.000000 fake.py-0.6.7/docs/_static/examples/creating_pdf/text_pdf_bytes_2.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      106 2023-12-01 00:01:18.000000 fake.py-0.6.7/docs/_static/examples/creating_pdf/text_pdf_bytes_3.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       96 2023-12-01 00:01:18.000000 fake.py-0.6.7/docs/_static/examples/creating_pdf/text_pdf_file_1.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      135 2023-12-01 00:01:18.000000 fake.py-0.6.7/docs/_static/examples/creating_pdf/text_pdf_file_2.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      110 2023-12-01 00:01:18.000000 fake.py-0.6.7/docs/_static/examples/creating_pdf/text_pdf_file_3.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      241 2023-12-03 00:58:59.000000 fake.py-0.6.7/docs/_static/examples/creating_pdf/text_pdf_file_django_1.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      308 2023-12-03 00:58:59.000000 fake.py-0.6.7/docs/_static/examples/creating_pdf/text_pdf_file_pydantic_1.py
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-01-16 23:35:13.207382 fake.py-0.6.7/docs/_static/examples/factories/
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-01-16 23:35:13.207382 fake.py-0.6.7/docs/_static/examples/factories/dataclasses/
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-01-16 23:35:13.231382 fake.py-0.6.7/docs/_static/examples/factories/dataclasses/article/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2907 2023-12-17 23:22:17.000000 fake.py-0.6.7/docs/_static/examples/factories/dataclasses/article/factories.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1273 2023-12-17 23:21:49.000000 fake.py-0.6.7/docs/_static/examples/factories/dataclasses/article/models.py
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-01-16 23:35:13.207382 fake.py-0.6.7/docs/_static/examples/factories/django/
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-01-16 23:35:13.231382 fake.py-0.6.7/docs/_static/examples/factories/django/article/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     4517 2023-12-17 23:22:17.000000 fake.py-0.6.7/docs/_static/examples/factories/django/article/factories.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      835 2024-01-10 21:32:55.000000 fake.py-0.6.7/docs/_static/examples/factories/django/article/models.py
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-01-16 23:35:13.207382 fake.py-0.6.7/docs/_static/examples/factories/pydantic/
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-01-16 23:35:13.231382 fake.py-0.6.7/docs/_static/examples/factories/pydantic/article/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2651 2023-12-17 23:22:17.000000 fake.py-0.6.7/docs/_static/examples/factories/pydantic/article/factories.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1926 2023-12-17 23:21:49.000000 fake.py-0.6.7/docs/_static/examples/factories/pydantic/article/models.py
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-01-16 23:35:13.231382 fake.py-0.6.7/docs/_static/examples/factories/sqlalchemy/
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-01-16 23:35:13.231382 fake.py-0.6.7/docs/_static/examples/factories/sqlalchemy/article/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     3652 2023-12-21 20:14:56.000000 fake.py-0.6.7/docs/_static/examples/factories/sqlalchemy/article/factories.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2636 2023-12-17 23:21:49.000000 fake.py-0.6.7/docs/_static/examples/factories/sqlalchemy/article/models.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      425 2023-12-11 23:32:41.000000 fake.py-0.6.7/docs/_static/examples/factories/sqlalchemy/config.py
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-01-16 23:35:13.207382 fake.py-0.6.7/docs/_static/examples/factories/tortoise/
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-01-16 23:35:13.235383 fake.py-0.6.7/docs/_static/examples/factories/tortoise/article/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2792 2023-12-17 23:22:17.000000 fake.py-0.6.7/docs/_static/examples/factories/tortoise/article/factories.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1895 2023-12-17 23:21:49.000000 fake.py-0.6.7/docs/_static/examples/factories/tortoise/article/models.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       30 2022-12-17 15:38:13.000000 fake.py-0.6.7/docs/changelog.rst
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       36 2023-12-01 00:01:18.000000 fake.py-0.6.7/docs/code_of_conduct.rst
--rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2389 2023-12-21 20:14:56.000000 fake.py-0.6.7/docs/conf.py
--rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     9004 2023-11-25 21:22:55.000000 fake.py-0.6.7/docs/conf.py.distrib
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       33 2023-12-01 00:01:18.000000 fake.py-0.6.7/docs/contributor_guidelines.rst
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2377 2023-12-03 00:58:59.000000 fake.py-0.6.7/docs/creating_docx.rst
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2151 2023-12-04 20:42:03.000000 fake.py-0.6.7/docs/creating_images.rst
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     4102 2023-12-03 00:58:59.000000 fake.py-0.6.7/docs/creating_pdf.rst
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     6056 2023-12-09 20:33:04.000000 fake.py-0.6.7/docs/customization.rst
--rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      302 2023-12-07 00:03:15.000000 fake.py-0.6.7/docs/documentation.rst
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     5816 2023-12-17 23:22:17.000000 fake.py-0.6.7/docs/factories.rst
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      100 2023-11-25 00:03:04.000000 fake.py-0.6.7/docs/fake.rst
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       58 2023-11-25 21:31:30.000000 fake.py-0.6.7/docs/index.rst
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       58 2022-12-17 15:38:13.000000 fake.py-0.6.7/docs/index.rst.distrib
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      800 2023-11-25 21:31:30.000000 fake.py-0.6.7/docs/make.bat
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      149 2023-11-25 21:27:34.000000 fake.py-0.6.7/docs/package.rst
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)    14518 2024-01-15 21:54:25.000000 fake.py-0.6.7/docs/recipes.rst
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     5142 2024-01-15 21:54:25.000000 fake.py-0.6.7/docs/requirements.txt
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       29 2023-12-01 00:01:18.000000 fake.py-0.6.7/docs/security.rst
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-01-16 23:35:13.235383 fake.py-0.6.7/examples/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      357 2023-12-21 20:14:56.000000 fake.py-0.6.7/examples/README.rst
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-01-16 23:35:13.235383 fake.py-0.6.7/examples/customization/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      219 2023-12-21 20:14:56.000000 fake.py-0.6.7/examples/customization/README.rst
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-01-16 23:35:13.239383 fake.py-0.6.7/examples/customization/address/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-12-08 00:35:23.000000 fake.py-0.6.7/examples/customization/address/__init__.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1469 2023-12-09 22:54:37.000000 fake.py-0.6.7/examples/customization/address/factories.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      590 2023-12-08 00:35:23.000000 fake.py-0.6.7/examples/customization/address/models.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1592 2023-12-09 00:44:20.000000 fake.py-0.6.7/examples/customization/address/tests.py
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-01-16 23:35:13.239383 fake.py-0.6.7/examples/customization/band/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-12-09 00:44:20.000000 fake.py-0.6.7/examples/customization/band/__init__.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      402 2023-12-09 00:44:20.000000 fake.py-0.6.7/examples/customization/band/factories.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      291 2023-12-09 00:44:20.000000 fake.py-0.6.7/examples/customization/band/models.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      725 2023-12-09 00:44:20.000000 fake.py-0.6.7/examples/customization/band/tests.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     4291 2023-12-08 00:35:23.000000 fake.py-0.6.7/examples/customization/data.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1529 2023-12-09 22:54:37.000000 fake.py-0.6.7/examples/customization/fake_address.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1145 2023-12-09 00:44:20.000000 fake.py-0.6.7/examples/customization/fake_band.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      955 2023-12-09 00:44:20.000000 fake.py-0.6.7/examples/customization/manage.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      719 2023-12-09 22:54:37.000000 fake.py-0.6.7/examples/customization/override_default_data.py
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-01-16 23:35:13.239383 fake.py-0.6.7/examples/dataclasses/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      131 2023-12-21 20:14:56.000000 fake.py-0.6.7/examples/dataclasses/README.rst
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-01-16 23:35:13.239383 fake.py-0.6.7/examples/dataclasses/article/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-12-03 00:58:59.000000 fake.py-0.6.7/examples/dataclasses/article/__init__.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2907 2023-12-17 23:22:17.000000 fake.py-0.6.7/examples/dataclasses/article/factories.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1273 2023-12-17 23:21:49.000000 fake.py-0.6.7/examples/dataclasses/article/models.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1925 2023-12-17 23:21:49.000000 fake.py-0.6.7/examples/dataclasses/article/tests.py
--rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      956 2023-12-06 00:04:22.000000 fake.py-0.6.7/examples/dataclasses/manage.py
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-01-16 23:35:13.243383 fake.py-0.6.7/examples/django/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       87 2023-12-21 20:14:56.000000 fake.py-0.6.7/examples/django/README.rst
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-01-16 23:35:13.243383 fake.py-0.6.7/examples/django/article/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-12-01 00:01:18.000000 fake.py-0.6.7/examples/django/article/__init__.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      303 2023-12-01 00:01:18.000000 fake.py-0.6.7/examples/django/article/admin.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      146 2023-12-01 00:01:18.000000 fake.py-0.6.7/examples/django/article/apps.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     4517 2023-12-17 23:22:17.000000 fake.py-0.6.7/examples/django/article/factories.py
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-01-16 23:35:13.247383 fake.py-0.6.7/examples/django/article/migrations/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1725 2023-12-17 23:22:17.000000 fake.py-0.6.7/examples/django/article/migrations/0001_initial.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-12-01 00:01:18.000000 fake.py-0.6.7/examples/django/article/migrations/__init__.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      835 2024-01-10 21:32:55.000000 fake.py-0.6.7/examples/django/article/models.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     3312 2023-12-16 00:28:30.000000 fake.py-0.6.7/examples/django/article/tests.py
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-01-16 23:35:13.247383 fake.py-0.6.7/examples/django/blog/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-12-01 00:01:18.000000 fake.py-0.6.7/examples/django/blog/__init__.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      385 2023-12-01 00:01:18.000000 fake.py-0.6.7/examples/django/blog/asgi.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     3389 2023-12-01 00:01:18.000000 fake.py-0.6.7/examples/django/blog/settings.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      914 2023-12-01 00:01:18.000000 fake.py-0.6.7/examples/django/blog/urls.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      385 2023-12-01 00:01:18.000000 fake.py-0.6.7/examples/django/blog/wsgi.py
--rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      726 2023-12-06 00:04:22.000000 fake.py-0.6.7/examples/django/manage.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       14 2023-12-11 23:32:41.000000 fake.py-0.6.7/examples/django/requirements.in
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-01-16 23:35:13.247383 fake.py-0.6.7/examples/hypothesis/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       96 2023-12-21 20:14:56.000000 fake.py-0.6.7/examples/hypothesis/README.rst
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      948 2023-12-08 00:35:23.000000 fake.py-0.6.7/examples/hypothesis/manage.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       11 2023-12-08 00:35:23.000000 fake.py-0.6.7/examples/hypothesis/requirements.in
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     8548 2023-12-08 00:35:23.000000 fake.py-0.6.7/examples/hypothesis/tests.py
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-01-16 23:35:13.247383 fake.py-0.6.7/examples/lazyfuzzy/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      199 2023-12-21 20:14:56.000000 fake.py-0.6.7/examples/lazyfuzzy/README.rst
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-01-16 23:35:13.251383 fake.py-0.6.7/examples/lazyfuzzy/article/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-12-13 00:06:45.000000 fake.py-0.6.7/examples/lazyfuzzy/article/__init__.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2507 2023-12-13 00:47:49.000000 fake.py-0.6.7/examples/lazyfuzzy/article/factories.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      976 2023-12-13 00:47:49.000000 fake.py-0.6.7/examples/lazyfuzzy/article/models.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1674 2023-12-13 00:47:49.000000 fake.py-0.6.7/examples/lazyfuzzy/article/tests.py
--rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      956 2023-12-13 00:06:45.000000 fake.py-0.6.7/examples/lazyfuzzy/manage.py
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-01-16 23:35:13.251383 fake.py-0.6.7/examples/pydantic/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       97 2023-12-21 20:14:56.000000 fake.py-0.6.7/examples/pydantic/README.rst
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-01-16 23:35:13.251383 fake.py-0.6.7/examples/pydantic/article/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-12-01 00:01:18.000000 fake.py-0.6.7/examples/pydantic/article/__init__.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2651 2023-12-17 23:22:17.000000 fake.py-0.6.7/examples/pydantic/article/factories.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1926 2023-12-17 23:21:49.000000 fake.py-0.6.7/examples/pydantic/article/models.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1925 2023-12-17 23:21:49.000000 fake.py-0.6.7/examples/pydantic/article/tests.py
--rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      956 2023-12-06 00:04:22.000000 fake.py-0.6.7/examples/pydantic/manage.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        9 2023-12-07 00:03:15.000000 fake.py-0.6.7/examples/pydantic/requirements.in
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-01-16 23:35:13.255383 fake.py-0.6.7/examples/sqlalchemy/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      100 2023-12-21 20:14:56.000000 fake.py-0.6.7/examples/sqlalchemy/README.rst
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-01-16 23:35:13.255383 fake.py-0.6.7/examples/sqlalchemy/article/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-12-11 23:32:41.000000 fake.py-0.6.7/examples/sqlalchemy/article/__init__.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     3652 2023-12-21 20:14:56.000000 fake.py-0.6.7/examples/sqlalchemy/article/factories.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2636 2023-12-17 23:21:49.000000 fake.py-0.6.7/examples/sqlalchemy/article/models.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1299 2023-12-17 23:21:49.000000 fake.py-0.6.7/examples/sqlalchemy/article/tests.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      425 2023-12-11 23:32:41.000000 fake.py-0.6.7/examples/sqlalchemy/config.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1070 2023-12-11 23:32:41.000000 fake.py-0.6.7/examples/sqlalchemy/manage.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       11 2023-12-11 23:32:41.000000 fake.py-0.6.7/examples/sqlalchemy/requirements.in
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-01-16 23:35:13.259383 fake.py-0.6.7/examples/tortoise/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      107 2023-12-21 20:14:56.000000 fake.py-0.6.7/examples/tortoise/README.rst
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-01-16 23:35:13.259383 fake.py-0.6.7/examples/tortoise/article/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-12-01 00:01:18.000000 fake.py-0.6.7/examples/tortoise/article/__init__.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2792 2023-12-17 23:22:17.000000 fake.py-0.6.7/examples/tortoise/article/factories.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1895 2023-12-17 23:21:49.000000 fake.py-0.6.7/examples/tortoise/article/models.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     4082 2023-12-17 23:21:49.000000 fake.py-0.6.7/examples/tortoise/article/tests.py
--rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1350 2023-12-06 00:04:22.000000 fake.py-0.6.7/examples/tortoise/manage.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       13 2023-12-07 00:03:15.000000 fake.py-0.6.7/examples/tortoise/requirements.in
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)   146229 2024-01-16 23:35:00.000000 fake.py-0.6.7/fake.py
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-01-16 23:35:13.259383 fake.py-0.6.7/fake.py.egg-info/
--rw-r--r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)    12567 2024-01-16 23:35:13.000000 fake.py-0.6.7/fake.py.egg-info/PKG-INFO
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     5145 2024-01-16 23:35:13.000000 fake.py-0.6.7/fake.py.egg-info/SOURCES.txt
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        1 2024-01-16 23:35:13.000000 fake.py-0.6.7/fake.py.egg-info/dependency_links.txt
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      189 2024-01-16 23:35:13.000000 fake.py-0.6.7/fake.py.egg-info/requires.txt
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        5 2024-01-16 23:35:13.000000 fake.py-0.6.7/fake.py.egg-info/top_level.txt
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     3910 2024-01-16 23:35:00.000000 fake.py-0.6.7/pyproject.toml
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       38 2024-01-16 23:35:13.263383 fake.py-0.6.7/setup.cfg
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-06 22:26:42.474301 fake_py-0.6.8/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       29 2022-12-17 15:38:13.000000 fake_py-0.6.8/.coveralls.yml
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       34 2022-12-17 15:38:13.000000 fake_py-0.6.8/.env
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-06 22:26:42.442301 fake_py-0.6.8/.github/
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-06 22:26:42.450301 fake_py-0.6.8/.github/workflows/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)    11430 2023-12-11 23:32:41.000000 fake_py-0.6.8/.github/workflows/test.yml
+-rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      625 2024-05-06 22:26:08.000000 fake_py-0.6.8/.gitignore
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1422 2023-11-24 22:03:33.000000 fake_py-0.6.8/.pre-commit-config.yaml
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      361 2022-12-27 21:29:13.000000 fake_py-0.6.8/.pre-commit-hooks.yaml
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1020 2023-11-24 23:49:27.000000 fake_py-0.6.8/.readthedocs.yaml
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2588 2024-05-06 22:26:08.000000 fake_py-0.6.8/.secrets.baseline
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2588 2024-05-06 22:26:08.000000 fake_py-0.6.8/CHANGELOG.rst
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     5397 2023-12-01 00:01:18.000000 fake_py-0.6.8/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     5397 2023-12-01 00:01:18.000000 fake_py-0.6.8/CODE_OF_CONDUCT.rst
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     4070 2023-12-11 23:32:41.000000 fake_py-0.6.8/CONTRIBUTING.rst
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1073 2023-11-01 19:30:30.000000 fake_py-0.6.8/LICENSE
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     4495 2024-05-06 22:26:08.000000 fake_py-0.6.8/Makefile
+-rw-r--r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)    13524 2024-05-06 22:26:42.474301 fake_py-0.6.8/PKG-INFO
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)    11443 2024-05-06 22:26:08.000000 fake_py-0.6.8/README.rst
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1378 2023-12-09 00:44:20.000000 fake_py-0.6.8/SECURITY.md
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1378 2023-12-09 00:44:20.000000 fake_py-0.6.8/SECURITY.rst
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)   146229 2024-05-06 22:26:08.000000 fake_py-0.6.8/__copy_fake.py
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-06 22:26:42.454301 fake_py-0.6.8/docs/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      634 2023-11-25 21:31:30.000000 fake_py-0.6.8/docs/Makefile
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-06 22:26:42.442301 fake_py-0.6.8/docs/_static/
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-06 22:26:42.442301 fake_py-0.6.8/docs/_static/examples/
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-06 22:26:42.454301 fake_py-0.6.8/docs/_static/examples/creating_docx/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       50 2023-12-03 00:58:59.000000 fake_py-0.6.8/docs/_static/examples/creating_docx/docx_bytes_1.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       87 2023-12-03 00:58:59.000000 fake_py-0.6.8/docs/_static/examples/creating_docx/docx_bytes_2.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       62 2023-12-03 00:58:59.000000 fake_py-0.6.8/docs/_static/examples/creating_docx/docx_bytes_3.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       54 2023-12-03 00:58:59.000000 fake_py-0.6.8/docs/_static/examples/creating_docx/docx_file_1.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       91 2023-12-03 00:58:59.000000 fake_py-0.6.8/docs/_static/examples/creating_docx/docx_file_2.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       66 2023-12-03 00:58:59.000000 fake_py-0.6.8/docs/_static/examples/creating_docx/docx_file_3.py
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-06 22:26:42.454301 fake_py-0.6.8/docs/_static/examples/creating_images/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       48 2023-12-03 00:58:59.000000 fake_py-0.6.8/docs/_static/examples/creating_images/png_bytes_1.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       86 2023-12-03 00:58:59.000000 fake_py-0.6.8/docs/_static/examples/creating_images/png_bytes_2.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       52 2023-12-03 00:58:59.000000 fake_py-0.6.8/docs/_static/examples/creating_images/png_file_1.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       90 2023-12-03 00:58:59.000000 fake_py-0.6.8/docs/_static/examples/creating_images/png_file_2.py
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-06 22:26:42.458301 fake_py-0.6.8/docs/_static/examples/creating_pdf/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       98 2023-12-01 00:01:18.000000 fake_py-0.6.8/docs/_static/examples/creating_pdf/graphic_pdf_bytes_1.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      112 2023-12-01 00:01:18.000000 fake_py-0.6.8/docs/_static/examples/creating_pdf/graphic_pdf_bytes_2.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      102 2023-12-01 00:01:18.000000 fake_py-0.6.8/docs/_static/examples/creating_pdf/graphic_pdf_file_1.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      116 2023-12-01 00:01:18.000000 fake_py-0.6.8/docs/_static/examples/creating_pdf/graphic_pdf_file_2.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       92 2023-12-01 00:01:18.000000 fake_py-0.6.8/docs/_static/examples/creating_pdf/text_pdf_bytes_1.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      131 2023-12-01 00:01:18.000000 fake_py-0.6.8/docs/_static/examples/creating_pdf/text_pdf_bytes_2.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      106 2023-12-01 00:01:18.000000 fake_py-0.6.8/docs/_static/examples/creating_pdf/text_pdf_bytes_3.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       96 2023-12-01 00:01:18.000000 fake_py-0.6.8/docs/_static/examples/creating_pdf/text_pdf_file_1.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      135 2023-12-01 00:01:18.000000 fake_py-0.6.8/docs/_static/examples/creating_pdf/text_pdf_file_2.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      110 2023-12-01 00:01:18.000000 fake_py-0.6.8/docs/_static/examples/creating_pdf/text_pdf_file_3.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      241 2023-12-03 00:58:59.000000 fake_py-0.6.8/docs/_static/examples/creating_pdf/text_pdf_file_django_1.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      308 2023-12-03 00:58:59.000000 fake_py-0.6.8/docs/_static/examples/creating_pdf/text_pdf_file_pydantic_1.py
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-06 22:26:42.442301 fake_py-0.6.8/docs/_static/examples/factories/
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-06 22:26:42.442301 fake_py-0.6.8/docs/_static/examples/factories/dataclasses/
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-06 22:26:42.458301 fake_py-0.6.8/docs/_static/examples/factories/dataclasses/article/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2907 2023-12-17 23:22:17.000000 fake_py-0.6.8/docs/_static/examples/factories/dataclasses/article/factories.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1273 2023-12-17 23:21:49.000000 fake_py-0.6.8/docs/_static/examples/factories/dataclasses/article/models.py
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-06 22:26:42.442301 fake_py-0.6.8/docs/_static/examples/factories/django/
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-06 22:26:42.458301 fake_py-0.6.8/docs/_static/examples/factories/django/article/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     4517 2023-12-17 23:22:17.000000 fake_py-0.6.8/docs/_static/examples/factories/django/article/factories.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      835 2024-01-10 21:32:55.000000 fake_py-0.6.8/docs/_static/examples/factories/django/article/models.py
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-06 22:26:42.442301 fake_py-0.6.8/docs/_static/examples/factories/pydantic/
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-06 22:26:42.458301 fake_py-0.6.8/docs/_static/examples/factories/pydantic/article/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2651 2023-12-17 23:22:17.000000 fake_py-0.6.8/docs/_static/examples/factories/pydantic/article/factories.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1926 2023-12-17 23:21:49.000000 fake_py-0.6.8/docs/_static/examples/factories/pydantic/article/models.py
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-06 22:26:42.458301 fake_py-0.6.8/docs/_static/examples/factories/sqlalchemy/
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-06 22:26:42.458301 fake_py-0.6.8/docs/_static/examples/factories/sqlalchemy/article/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     3652 2023-12-21 20:14:56.000000 fake_py-0.6.8/docs/_static/examples/factories/sqlalchemy/article/factories.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2636 2023-12-17 23:21:49.000000 fake_py-0.6.8/docs/_static/examples/factories/sqlalchemy/article/models.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      425 2023-12-11 23:32:41.000000 fake_py-0.6.8/docs/_static/examples/factories/sqlalchemy/config.py
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-06 22:26:42.442301 fake_py-0.6.8/docs/_static/examples/factories/tortoise/
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-06 22:26:42.458301 fake_py-0.6.8/docs/_static/examples/factories/tortoise/article/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2792 2023-12-17 23:22:17.000000 fake_py-0.6.8/docs/_static/examples/factories/tortoise/article/factories.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1895 2023-12-17 23:21:49.000000 fake_py-0.6.8/docs/_static/examples/factories/tortoise/article/models.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       30 2022-12-17 15:38:13.000000 fake_py-0.6.8/docs/changelog.rst
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       36 2023-12-01 00:01:18.000000 fake_py-0.6.8/docs/code_of_conduct.rst
+-rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2728 2024-05-06 22:26:08.000000 fake_py-0.6.8/docs/conf.py
+-rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     9004 2023-11-25 21:22:55.000000 fake_py-0.6.8/docs/conf.py.distrib
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       33 2023-12-01 00:01:18.000000 fake_py-0.6.8/docs/contributor_guidelines.rst
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2377 2023-12-03 00:58:59.000000 fake_py-0.6.8/docs/creating_docx.rst
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2151 2023-12-04 20:42:03.000000 fake_py-0.6.8/docs/creating_images.rst
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     4102 2023-12-03 00:58:59.000000 fake_py-0.6.8/docs/creating_pdf.rst
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     6175 2024-05-06 22:26:08.000000 fake_py-0.6.8/docs/customization.rst
+-rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      302 2023-12-07 00:03:15.000000 fake_py-0.6.8/docs/documentation.rst
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     5816 2023-12-17 23:22:17.000000 fake_py-0.6.8/docs/factories.rst
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      100 2023-11-25 00:03:04.000000 fake_py-0.6.8/docs/fake.rst
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       58 2023-11-25 21:31:30.000000 fake_py-0.6.8/docs/index.rst
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       58 2022-12-17 15:38:13.000000 fake_py-0.6.8/docs/index.rst.distrib
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      800 2023-11-25 21:31:30.000000 fake_py-0.6.8/docs/make.bat
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      149 2023-11-25 21:27:34.000000 fake_py-0.6.8/docs/package.rst
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)    14518 2024-01-15 21:54:25.000000 fake_py-0.6.8/docs/recipes.rst
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     5380 2024-05-06 22:26:08.000000 fake_py-0.6.8/docs/requirements.txt
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       29 2023-12-01 00:01:18.000000 fake_py-0.6.8/docs/security.rst
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-06 22:26:42.458301 fake_py-0.6.8/examples/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      357 2023-12-21 20:14:56.000000 fake_py-0.6.8/examples/README.rst
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-06 22:26:42.458301 fake_py-0.6.8/examples/customization/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      219 2023-12-21 20:14:56.000000 fake_py-0.6.8/examples/customization/README.rst
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-06 22:26:42.462301 fake_py-0.6.8/examples/customization/address/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-12-08 00:35:23.000000 fake_py-0.6.8/examples/customization/address/__init__.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1469 2023-12-09 22:54:37.000000 fake_py-0.6.8/examples/customization/address/factories.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      590 2023-12-08 00:35:23.000000 fake_py-0.6.8/examples/customization/address/models.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1592 2023-12-09 00:44:20.000000 fake_py-0.6.8/examples/customization/address/tests.py
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-06 22:26:42.462301 fake_py-0.6.8/examples/customization/band/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-12-09 00:44:20.000000 fake_py-0.6.8/examples/customization/band/__init__.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      402 2023-12-09 00:44:20.000000 fake_py-0.6.8/examples/customization/band/factories.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      291 2023-12-09 00:44:20.000000 fake_py-0.6.8/examples/customization/band/models.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      725 2023-12-09 00:44:20.000000 fake_py-0.6.8/examples/customization/band/tests.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     4291 2023-12-08 00:35:23.000000 fake_py-0.6.8/examples/customization/data.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1529 2023-12-09 22:54:37.000000 fake_py-0.6.8/examples/customization/fake_address.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1145 2023-12-09 00:44:20.000000 fake_py-0.6.8/examples/customization/fake_band.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      955 2023-12-09 00:44:20.000000 fake_py-0.6.8/examples/customization/manage.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      719 2023-12-09 22:54:37.000000 fake_py-0.6.8/examples/customization/override_default_data.py
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-06 22:26:42.462301 fake_py-0.6.8/examples/dataclasses/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      131 2023-12-21 20:14:56.000000 fake_py-0.6.8/examples/dataclasses/README.rst
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-06 22:26:42.462301 fake_py-0.6.8/examples/dataclasses/article/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-12-03 00:58:59.000000 fake_py-0.6.8/examples/dataclasses/article/__init__.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2907 2023-12-17 23:22:17.000000 fake_py-0.6.8/examples/dataclasses/article/factories.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1273 2023-12-17 23:21:49.000000 fake_py-0.6.8/examples/dataclasses/article/models.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1925 2023-12-17 23:21:49.000000 fake_py-0.6.8/examples/dataclasses/article/tests.py
+-rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      956 2023-12-06 00:04:22.000000 fake_py-0.6.8/examples/dataclasses/manage.py
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-06 22:26:42.462301 fake_py-0.6.8/examples/django/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       87 2023-12-21 20:14:56.000000 fake_py-0.6.8/examples/django/README.rst
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-06 22:26:42.462301 fake_py-0.6.8/examples/django/article/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-12-01 00:01:18.000000 fake_py-0.6.8/examples/django/article/__init__.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      303 2023-12-01 00:01:18.000000 fake_py-0.6.8/examples/django/article/admin.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      146 2023-12-01 00:01:18.000000 fake_py-0.6.8/examples/django/article/apps.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     4517 2023-12-17 23:22:17.000000 fake_py-0.6.8/examples/django/article/factories.py
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-06 22:26:42.462301 fake_py-0.6.8/examples/django/article/migrations/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1725 2023-12-17 23:22:17.000000 fake_py-0.6.8/examples/django/article/migrations/0001_initial.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-12-01 00:01:18.000000 fake_py-0.6.8/examples/django/article/migrations/__init__.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      835 2024-01-10 21:32:55.000000 fake_py-0.6.8/examples/django/article/models.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     3312 2023-12-16 00:28:30.000000 fake_py-0.6.8/examples/django/article/tests.py
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-06 22:26:42.466301 fake_py-0.6.8/examples/django/blog/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-12-01 00:01:18.000000 fake_py-0.6.8/examples/django/blog/__init__.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      385 2023-12-01 00:01:18.000000 fake_py-0.6.8/examples/django/blog/asgi.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     3389 2023-12-01 00:01:18.000000 fake_py-0.6.8/examples/django/blog/settings.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      914 2023-12-01 00:01:18.000000 fake_py-0.6.8/examples/django/blog/urls.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      385 2023-12-01 00:01:18.000000 fake_py-0.6.8/examples/django/blog/wsgi.py
+-rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      726 2023-12-06 00:04:22.000000 fake_py-0.6.8/examples/django/manage.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       14 2023-12-11 23:32:41.000000 fake_py-0.6.8/examples/django/requirements.in
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-06 22:26:42.466301 fake_py-0.6.8/examples/hypothesis/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       96 2023-12-21 20:14:56.000000 fake_py-0.6.8/examples/hypothesis/README.rst
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      948 2023-12-08 00:35:23.000000 fake_py-0.6.8/examples/hypothesis/manage.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       11 2023-12-08 00:35:23.000000 fake_py-0.6.8/examples/hypothesis/requirements.in
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     8548 2023-12-08 00:35:23.000000 fake_py-0.6.8/examples/hypothesis/tests.py
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-06 22:26:42.466301 fake_py-0.6.8/examples/lazyfuzzy/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      199 2023-12-21 20:14:56.000000 fake_py-0.6.8/examples/lazyfuzzy/README.rst
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-06 22:26:42.466301 fake_py-0.6.8/examples/lazyfuzzy/article/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-12-13 00:06:45.000000 fake_py-0.6.8/examples/lazyfuzzy/article/__init__.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2507 2023-12-13 00:47:49.000000 fake_py-0.6.8/examples/lazyfuzzy/article/factories.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      976 2023-12-13 00:47:49.000000 fake_py-0.6.8/examples/lazyfuzzy/article/models.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1674 2023-12-13 00:47:49.000000 fake_py-0.6.8/examples/lazyfuzzy/article/tests.py
+-rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      956 2023-12-13 00:06:45.000000 fake_py-0.6.8/examples/lazyfuzzy/manage.py
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-06 22:26:42.466301 fake_py-0.6.8/examples/pydantic/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       97 2023-12-21 20:14:56.000000 fake_py-0.6.8/examples/pydantic/README.rst
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-06 22:26:42.466301 fake_py-0.6.8/examples/pydantic/article/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-12-01 00:01:18.000000 fake_py-0.6.8/examples/pydantic/article/__init__.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2651 2023-12-17 23:22:17.000000 fake_py-0.6.8/examples/pydantic/article/factories.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1926 2023-12-17 23:21:49.000000 fake_py-0.6.8/examples/pydantic/article/models.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1925 2023-12-17 23:21:49.000000 fake_py-0.6.8/examples/pydantic/article/tests.py
+-rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      956 2023-12-06 00:04:22.000000 fake_py-0.6.8/examples/pydantic/manage.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        9 2023-12-07 00:03:15.000000 fake_py-0.6.8/examples/pydantic/requirements.in
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-06 22:26:42.466301 fake_py-0.6.8/examples/sqlalchemy/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      100 2023-12-21 20:14:56.000000 fake_py-0.6.8/examples/sqlalchemy/README.rst
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-06 22:26:42.470301 fake_py-0.6.8/examples/sqlalchemy/article/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-12-11 23:32:41.000000 fake_py-0.6.8/examples/sqlalchemy/article/__init__.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     3652 2023-12-21 20:14:56.000000 fake_py-0.6.8/examples/sqlalchemy/article/factories.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2636 2023-12-17 23:21:49.000000 fake_py-0.6.8/examples/sqlalchemy/article/models.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1299 2023-12-17 23:21:49.000000 fake_py-0.6.8/examples/sqlalchemy/article/tests.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      425 2023-12-11 23:32:41.000000 fake_py-0.6.8/examples/sqlalchemy/config.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1070 2023-12-11 23:32:41.000000 fake_py-0.6.8/examples/sqlalchemy/manage.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       11 2023-12-11 23:32:41.000000 fake_py-0.6.8/examples/sqlalchemy/requirements.in
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-06 22:26:42.470301 fake_py-0.6.8/examples/tortoise/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      107 2023-12-21 20:14:56.000000 fake_py-0.6.8/examples/tortoise/README.rst
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-06 22:26:42.470301 fake_py-0.6.8/examples/tortoise/article/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-12-01 00:01:18.000000 fake_py-0.6.8/examples/tortoise/article/__init__.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2792 2023-12-17 23:22:17.000000 fake_py-0.6.8/examples/tortoise/article/factories.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1895 2023-12-17 23:21:49.000000 fake_py-0.6.8/examples/tortoise/article/models.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     4082 2023-12-17 23:21:49.000000 fake_py-0.6.8/examples/tortoise/article/tests.py
+-rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1350 2023-12-06 00:04:22.000000 fake_py-0.6.8/examples/tortoise/manage.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       13 2023-12-07 00:03:15.000000 fake_py-0.6.8/examples/tortoise/requirements.in
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)   146229 2024-05-06 22:26:08.000000 fake_py-0.6.8/fake.py
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-06 22:26:42.470301 fake_py-0.6.8/fake.py.egg-info/
+-rw-r--r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)    13524 2024-05-06 22:26:42.000000 fake_py-0.6.8/fake.py.egg-info/PKG-INFO
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     5145 2024-05-06 22:26:42.000000 fake_py-0.6.8/fake.py.egg-info/SOURCES.txt
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        1 2024-05-06 22:26:42.000000 fake_py-0.6.8/fake.py.egg-info/dependency_links.txt
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      200 2024-05-06 22:26:42.000000 fake_py-0.6.8/fake.py.egg-info/requires.txt
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        5 2024-05-06 22:26:42.000000 fake_py-0.6.8/fake.py.egg-info/top_level.txt
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     3957 2024-05-06 22:26:08.000000 fake_py-0.6.8/pyproject.toml
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       38 2024-05-06 22:26:42.474301 fake_py-0.6.8/setup.cfg
```

### Comparing `fake.py-0.6.7/.github/workflows/test.yml` & `fake_py-0.6.8/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `fake.py-0.6.7/.gitignore` & `fake_py-0.6.8/.gitignore`

 * *Files 16% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 /tmp/
 .zip
 /examples/db/
 /var/
 /examples/tmp/
 /examples/logs/
 /builddocs/
+/docs/_build/
 /builddocs.zip
 /build/
 /dist/
 fake.py.egg-info
 matyan.log*
 db.sqlite3
 sample_db.sqlite
```

### Comparing `fake.py-0.6.7/.pre-commit-config.yaml` & `fake_py-0.6.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fake.py-0.6.7/.readthedocs.yaml` & `fake_py-0.6.8/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `fake.py-0.6.7/.secrets.baseline` & `fake_py-0.6.8/.secrets.baseline`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8%*

 * *Differences: {"'generated_at'": "'2024-05-06T22:16:59Z'", "'version'": "'1.5.0'"}*

```diff
@@ -35,15 +35,15 @@
         {
             "path": "detect_secrets.filters.heuristic.is_swagger_file"
         },
         {
             "path": "detect_secrets.filters.heuristic.is_templated_secret"
         }
     ],
-    "generated_at": "2023-12-17T23:16:36Z",
+    "generated_at": "2024-05-06T22:16:59Z",
     "plugins_used": [
         {
             "name": "ArtifactoryDetector"
         },
         {
             "name": "AWSKeyDetector"
         },
@@ -118,9 +118,9 @@
                 "hashed_secret": "9bc34549d565d9505b287de0cd20ac77be1d3f2c",
                 "is_verified": true,
                 "line_number": 96,
                 "type": "Secret Keyword"
             }
         ]
     },
-    "version": "1.4.0"
+    "version": "1.5.0"
 }
```

### Comparing `fake.py-0.6.7/CHANGELOG.rst` & `fake_py-0.6.8/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,20 @@
 - It's always safe to upgrade within the same minor version (for example, from
   0.3 to 0.3.4).
 - Minor version changes might be backwards incompatible. Read the
   release notes carefully before upgrading (for example, when upgrading from
   0.3.4 to 0.4).
 - All backwards incompatible changes are mentioned in this document.
 
+0.6.8
+-----
+2024-05-06
+
+- Minor fixes in docs.
+
 0.6.7
 -----
 2024-01-17
 
 - Add ``uuids``, ``first_names``, ``last_names``, ``names``, ``usernames`` and
   ``slugs`` plural providers (return ``List``).
```

### Comparing `fake.py-0.6.7/CODE_OF_CONDUCT.md` & `fake_py-0.6.8/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `fake.py-0.6.7/CODE_OF_CONDUCT.rst` & `fake_py-0.6.8/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `fake.py-0.6.7/CONTRIBUTING.rst` & `fake_py-0.6.8/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `fake.py-0.6.7/LICENSE` & `fake_py-0.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `fake.py-0.6.7/Makefile` & `fake_py-0.6.8/Makefile`

 * *Files 9% similar despite different names*

```diff
@@ -10,14 +10,23 @@
 	cd builddocs && zip -r ../builddocs.zip . -x ".*" && cd ..
 
 rebuild_docs:
 	source $(VENV) && sphinx-apidoc . --full -o docs -H 'fake.py' -A 'Artur Barseghyan <artur.barseghyan@gmail.com>' -f -d 20
 	cp docs/conf.py.distrib docs/conf.py
 	cp docs/index.rst.distrib docs/index.rst
 
+build_docs_epub:
+	$(MAKE) -C docs/ epub
+
+build_docs_pdf:
+	$(MAKE) -C docs/ latexpdf
+
+pre-commit:
+	pre-commit run --all-files
+
 # Format code using Black
 black:
 	source $(VENV) && black .
 
 # Sort imports using isort
 isort:
 	source $(VENV) && isort . --overwrite-in-place
@@ -25,17 +34,17 @@
 doc8:
 	source $(VENV) && doc8
 
 # Run ruff on the codebase
 ruff:
 	source $(VENV) && ruff .
 
-# Serve the built docs on port 5000
+# Serve the built docs on port 5001
 serve_docs:
-	source $(VENV) && cd builddocs && python -m http.server 5000
+	source $(VENV) && cd builddocs && python -m http.server 5001
 
 # Install the project
 install:
 	source $(VENV) && pip install -e .[all]
 
 test: clean
 	source $(VENV) && pytest -vrx -s
@@ -131,14 +140,17 @@
 	rm -rf .mypy_cache/
 	rm -rf .ruff_cache/
 	rm -rf dist/
 
 compile-requirements:
 	source $(VENV) && python -m piptools compile --extra all -o docs/requirements.txt pyproject.toml
 
+compile-requirements-upgrade:
+	source $(VENV) && python -m piptools compile --extra all -o docs/requirements.txt pyproject.toml --upgrade
+
 update-version:
 	#sed -i 's/"version": "[0-9.]\+"/"version": "$(VERSION)"/' package.json
 	sed -i 's/version = "[0-9.]\+"/version = "$(VERSION)"/' pyproject.toml
 	sed -i 's/__version__ = "[0-9.]\+"/__version__ = "$(VERSION)"/' fake.py
 #	find src/ -type f -name '*.css' -exec sed -i 's/@version [0-9.]\+/@version $(VERSION)/' {} \;
 #	find src/ -type f -name '*.js' -exec sed -i 's/@version [0-9.]\+/@version $(VERSION)/' {} \;
```

### Comparing `fake.py-0.6.7/PKG-INFO` & `fake_py-0.6.8/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fake.py
-Version: 0.6.7
+Version: 0.6.8
 Summary: Minimalistic, standalone alternative fake data generator with no dependencies.
 Author-email: Artur Barseghyan <artur.barseghyan@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/barseghyanartur/fake.py/
 Project-URL: Bug Tracker, https://github.com/barseghyanartur/fake.py/issues
 Project-URL: Documentation, https://fakepy.readthedocs.io/
 Project-URL: Source Code, https://github.com/barseghyanartur/fake.py/
@@ -37,14 +37,15 @@
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
+Requires-Dist: pytest-rst; extra == "test"
 Provides-Extra: docs
 Requires-Dist: sphinx<6.0; extra == "docs"
 Requires-Dist: sphinx-rtd-theme>=1.3.0; extra == "docs"
 Requires-Dist: sphinx-no-pragma; extra == "docs"
 
 =======
 fake.py
@@ -160,100 +161,119 @@
 Usage
 =====
 Generate data
 -------------
 Person names
 ~~~~~~~~~~~~
 .. code-block:: python
+    :name: test_person_names
 
     from fake import FAKER
 
-    FAKER.first_name()
-    FAKER.last_name()
-    FAKER.name()
-    FAKER.username()
+    FAKER.first_name()  # str
+    FAKER.first_names()  # list[str]
+    FAKER.last_name()  # str
+    FAKER.last_names()  # list[str]
+    FAKER.name()  # str
+    FAKER.names()  # list[str]
+    FAKER.username()  # str
+    FAKER.usernames()  # list[str]
 
 Random texts
 ~~~~~~~~~~~~
 .. code-block:: python
+    :name: test_random_texts
 
     from fake import FAKER
 
-    FAKER.slug()
-    FAKER.word()
-    FAKER.sentence()
-    FAKER.paragraph()
-    FAKER.text()
+    FAKER.slug()  # str
+    FAKER.slugs()  # list[str]
+    FAKER.word()  # str
+    FAKER.words()  # list[str]
+    FAKER.sentence()  # str
+    FAKER.sentences()  # list[str]
+    FAKER.paragraph()  # str
+    FAKER.paragraphs()  # list[str]
+    FAKER.text()  # str
+    FAKER.texts()  # list[str]
 
 Internet
 ~~~~~~~~
 .. code-block:: python
+    :name: test_internet
 
     from fake import FAKER
 
-    FAKER.email()
-    FAKER.url()
-    FAKER.ipv4()
+    FAKER.email()  # str
+    FAKER.url()  # str
+    FAKER.image_url()  # str
+    FAKER.ipv4()  # str
 
 Filenames
 ~~~~~~~~~
 .. code-block:: python
+    :name: test_filenames
 
     from fake import FAKER
 
-    FAKER.filename()
+    FAKER.file_name()  # str
 
 Primitive data types
 ~~~~~~~~~~~~~~~~~~~~
 .. code-block:: python
+    :name: test_primitive_data_types
 
     from fake import FAKER
 
-    FAKER.pyint()
-    FAKER.pybool()
-    FAKER.pystr()
-    FAKER.pyfloat()
+    FAKER.pyint()  # int
+    FAKER.pybool()  # bool
+    FAKER.pystr()  # str
+    FAKER.pyfloat()  # flot
+    FAKER.uuid()  # uuid.UUID
 
 Dates
 ~~~~~
 .. code-block:: python
+    :name: test_dates
 
     from fake import FAKER
 
-    FAKER.date()
-    FAKER.date_time()
+    FAKER.date()  # datetime.date
+    FAKER.date_time()  # datetime.datetime
 
 Generate files
 --------------
 As bytes
 ~~~~~~~~
 .. code-block:: python
+    :name: test_generate_files_as_bytes
 
     from fake import FAKER
 
-    FAKER.pdf()
-    FAKER.docx()
-    FAKER.png()
-    FAKER.svg()
-    FAKER.bmp()
-    FAKER.gif()
+    FAKER.pdf()  # bytes
+    FAKER.docx()  # bytes
+    FAKER.png()  # bytes
+    FAKER.svg()  # bytes
+    FAKER.bmp()  # bytes
+    FAKER.gif()  # bytes
 
 As files on the file system
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~
 .. code-block:: python
+    :name: test_generate_files_as_files_on_file_system
 
     from fake import FAKER
 
-    FAKER.pdf_file()
-    FAKER.docx_file()
-    FAKER.png_file()
-    FAKER.svg_file()
-    FAKER.bmp_file()
-    FAKER.gif_file()
-    FAKER.txt_file()
+    FAKER.pdf_file()  # str
+    FAKER.docx_file()  # str
+    FAKER.png_file()  # str
+    FAKER.svg_file()  # str
+    FAKER.bmp_file()  # str
+    FAKER.gif_file()  # str
+    FAKER.txt_file()  # str
 
 Factories
 ---------
 This is how you could define factories for `Django`_'s built-in ``Group``
 and ``User`` models.
 
 .. code-block:: python
@@ -345,14 +365,15 @@
     )
 
 Customize
 ---------
 Make your own custom providers and utilize factories with them.
 
 .. code-block:: python
+    :name: test_customize
 
     import random
     import string
 
     from fake import Faker, Factory, provider
```

### Comparing `fake.py-0.6.7/README.rst` & `fake_py-0.6.8/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -112,100 +112,119 @@
 Usage
 =====
 Generate data
 -------------
 Person names
 ~~~~~~~~~~~~
 .. code-block:: python
+    :name: test_person_names
 
     from fake import FAKER
 
-    FAKER.first_name()
-    FAKER.last_name()
-    FAKER.name()
-    FAKER.username()
+    FAKER.first_name()  # str
+    FAKER.first_names()  # list[str]
+    FAKER.last_name()  # str
+    FAKER.last_names()  # list[str]
+    FAKER.name()  # str
+    FAKER.names()  # list[str]
+    FAKER.username()  # str
+    FAKER.usernames()  # list[str]
 
 Random texts
 ~~~~~~~~~~~~
 .. code-block:: python
+    :name: test_random_texts
 
     from fake import FAKER
 
-    FAKER.slug()
-    FAKER.word()
-    FAKER.sentence()
-    FAKER.paragraph()
-    FAKER.text()
+    FAKER.slug()  # str
+    FAKER.slugs()  # list[str]
+    FAKER.word()  # str
+    FAKER.words()  # list[str]
+    FAKER.sentence()  # str
+    FAKER.sentences()  # list[str]
+    FAKER.paragraph()  # str
+    FAKER.paragraphs()  # list[str]
+    FAKER.text()  # str
+    FAKER.texts()  # list[str]
 
 Internet
 ~~~~~~~~
 .. code-block:: python
+    :name: test_internet
 
     from fake import FAKER
 
-    FAKER.email()
-    FAKER.url()
-    FAKER.ipv4()
+    FAKER.email()  # str
+    FAKER.url()  # str
+    FAKER.image_url()  # str
+    FAKER.ipv4()  # str
 
 Filenames
 ~~~~~~~~~
 .. code-block:: python
+    :name: test_filenames
 
     from fake import FAKER
 
-    FAKER.filename()
+    FAKER.file_name()  # str
 
 Primitive data types
 ~~~~~~~~~~~~~~~~~~~~
 .. code-block:: python
+    :name: test_primitive_data_types
 
     from fake import FAKER
 
-    FAKER.pyint()
-    FAKER.pybool()
-    FAKER.pystr()
-    FAKER.pyfloat()
+    FAKER.pyint()  # int
+    FAKER.pybool()  # bool
+    FAKER.pystr()  # str
+    FAKER.pyfloat()  # flot
+    FAKER.uuid()  # uuid.UUID
 
 Dates
 ~~~~~
 .. code-block:: python
+    :name: test_dates
 
     from fake import FAKER
 
-    FAKER.date()
-    FAKER.date_time()
+    FAKER.date()  # datetime.date
+    FAKER.date_time()  # datetime.datetime
 
 Generate files
 --------------
 As bytes
 ~~~~~~~~
 .. code-block:: python
+    :name: test_generate_files_as_bytes
 
     from fake import FAKER
 
-    FAKER.pdf()
-    FAKER.docx()
-    FAKER.png()
-    FAKER.svg()
-    FAKER.bmp()
-    FAKER.gif()
+    FAKER.pdf()  # bytes
+    FAKER.docx()  # bytes
+    FAKER.png()  # bytes
+    FAKER.svg()  # bytes
+    FAKER.bmp()  # bytes
+    FAKER.gif()  # bytes
 
 As files on the file system
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~
 .. code-block:: python
+    :name: test_generate_files_as_files_on_file_system
 
     from fake import FAKER
 
-    FAKER.pdf_file()
-    FAKER.docx_file()
-    FAKER.png_file()
-    FAKER.svg_file()
-    FAKER.bmp_file()
-    FAKER.gif_file()
-    FAKER.txt_file()
+    FAKER.pdf_file()  # str
+    FAKER.docx_file()  # str
+    FAKER.png_file()  # str
+    FAKER.svg_file()  # str
+    FAKER.bmp_file()  # str
+    FAKER.gif_file()  # str
+    FAKER.txt_file()  # str
 
 Factories
 ---------
 This is how you could define factories for `Django`_'s built-in ``Group``
 and ``User`` models.
 
 .. code-block:: python
@@ -297,14 +316,15 @@
     )
 
 Customize
 ---------
 Make your own custom providers and utilize factories with them.
 
 .. code-block:: python
+    :name: test_customize
 
     import random
     import string
 
     from fake import Faker, Factory, provider
```

### Comparing `fake.py-0.6.7/SECURITY.md` & `fake_py-0.6.8/SECURITY.md`

 * *Files identical despite different names*

### Comparing `fake.py-0.6.7/SECURITY.rst` & `fake_py-0.6.8/SECURITY.rst`

 * *Files identical despite different names*

### Comparing `fake.py-0.6.7/__copy_fake.py` & `fake_py-0.6.8/__copy_fake.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     get_args,
     get_origin,
     get_type_hints,
 )
 from uuid import UUID
 
 __title__ = "fake.py"
-__version__ = "0.6.7"
+__version__ = "0.6.8"
 __author__ = "Artur Barseghyan <artur.barseghyan@gmail.com>"
 __copyright__ = "2023-2024 Artur Barseghyan"
 __license__ = "MIT"
 __all__ = (
     "AuthorshipData",
     "BaseStorage",
     "DjangoModelFactory",
```

### Comparing `fake.py-0.6.7/docs/Makefile` & `fake_py-0.6.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `fake.py-0.6.7/docs/_static/examples/factories/dataclasses/article/factories.py` & `fake_py-0.6.8/docs/_static/examples/factories/dataclasses/article/factories.py`

 * *Files identical despite different names*

### Comparing `fake.py-0.6.7/docs/_static/examples/factories/dataclasses/article/models.py` & `fake_py-0.6.8/docs/_static/examples/factories/dataclasses/article/models.py`

 * *Files identical despite different names*

### Comparing `fake.py-0.6.7/docs/_static/examples/factories/django/article/factories.py` & `fake_py-0.6.8/docs/_static/examples/factories/django/article/factories.py`

 * *Files identical despite different names*

### Comparing `fake.py-0.6.7/docs/_static/examples/factories/django/article/models.py` & `fake_py-0.6.8/docs/_static/examples/factories/django/article/models.py`

 * *Files identical despite different names*

### Comparing `fake.py-0.6.7/docs/_static/examples/factories/pydantic/article/factories.py` & `fake_py-0.6.8/docs/_static/examples/factories/pydantic/article/factories.py`

 * *Files identical despite different names*

### Comparing `fake.py-0.6.7/docs/_static/examples/factories/pydantic/article/models.py` & `fake_py-0.6.8/docs/_static/examples/factories/pydantic/article/models.py`

 * *Files identical despite different names*

### Comparing `fake.py-0.6.7/docs/_static/examples/factories/sqlalchemy/article/factories.py` & `fake_py-0.6.8/docs/_static/examples/factories/sqlalchemy/article/factories.py`

 * *Files identical despite different names*

### Comparing `fake.py-0.6.7/docs/_static/examples/factories/sqlalchemy/article/models.py` & `fake_py-0.6.8/docs/_static/examples/factories/sqlalchemy/article/models.py`

 * *Files identical despite different names*

### Comparing `fake.py-0.6.7/docs/_static/examples/factories/tortoise/article/factories.py` & `fake_py-0.6.8/docs/_static/examples/factories/tortoise/article/factories.py`

 * *Files identical despite different names*

### Comparing `fake.py-0.6.7/docs/_static/examples/factories/tortoise/article/models.py` & `fake_py-0.6.8/docs/_static/examples/factories/tortoise/article/models.py`

 * *Files identical despite different names*

### Comparing `fake.py-0.6.7/docs/conf.py` & `fake_py-0.6.8/docs/conf.py`

 * *Files 27% similar despite different names*

```diff
@@ -67,12 +67,20 @@
     f"{prismjs_base}/prism.min.js",
     f"{prismjs_base}/plugins/autoloader/prism-autoloader.min.js",
     f"{prismjs_base}/plugins/toolbar/prism-toolbar.min.js",
     f"{prismjs_base}/plugins/copy-to-clipboard/prism-copy-to-clipboard.min.js",
     "https://cdn.jsdelivr.net/gh/barseghyanartur/jsphinx@1.3.4/src/js/download_adapter.js",
 ]
 
-
 # -- Options for todo extension ----------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/extensions/todo.html#configuration
 
 todo_include_todos = True
+
+# -- Options for Epub output  ----------------------------------------------
+epub_title = project
+epub_author = author
+epub_publisher = "GitHub"
+epub_copyright = copyright
+epub_identifier = "https://github.com/barseghyanartur/fake.py"  # URL or ISBN
+epub_scheme = "URL"  # or "ISBN"
+epub_uid = "https://github.com/barseghyanartur/fake.py"
```

### Comparing `fake.py-0.6.7/docs/conf.py.distrib` & `fake_py-0.6.8/docs/conf.py.distrib`

 * *Files identical despite different names*

### Comparing `fake.py-0.6.7/docs/creating_docx.rst` & `fake_py-0.6.8/docs/creating_docx.rst`

 * *Files identical despite different names*

### Comparing `fake.py-0.6.7/docs/creating_images.rst` & `fake_py-0.6.8/docs/creating_images.rst`

 * *Files identical despite different names*

### Comparing `fake.py-0.6.7/docs/creating_pdf.rst` & `fake_py-0.6.8/docs/creating_pdf.rst`

 * *Files identical despite different names*

### Comparing `fake.py-0.6.7/docs/customization.rst` & `fake_py-0.6.8/docs/customization.rst`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
   initialized with ``fake.FAKER`` instance.
 
 The ``Faker`` class is easy to customize. See the following example:
 
 **custom_fake.py**
 
 .. code-block:: python
+    :name: test_customization_custom_fake
 
     import random
     import string
 
     from fake import Faker, Factory, provider
 
 
@@ -173,14 +174,15 @@
 ``@provider`` decorator.
 
 You can now use both ``FAKER`` and ``FACTORY`` as you would normally do.
 
 **models.py**
 
 .. code-block:: python
+    :name: test_customization_models
 
     from dataclasses import dataclass
     from datetime import date
 
 
     @dataclass
     class Address:
@@ -205,14 +207,15 @@
 
         def __str__(self) -> str:
             return self.username
 
 **factories.py**
 
 .. code-block:: python
+    :name: test_customization_factories
 
     from fake import ModelFactory, SubFactory, post_save, pre_save
 
     from models import Address, Person
     from custom_fake import FACTORY
```

### Comparing `fake.py-0.6.7/docs/factories.rst` & `fake_py-0.6.8/docs/factories.rst`

 * *Files identical despite different names*

### Comparing `fake.py-0.6.7/docs/make.bat` & `fake_py-0.6.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `fake.py-0.6.7/docs/recipes.rst` & `fake_py-0.6.8/docs/recipes.rst`

 * *Files identical despite different names*

### Comparing `fake.py-0.6.7/docs/requirements.txt` & `fake_py-0.6.8/docs/requirements.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,184 +1,200 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
 #    pip-compile --extra=all --output-file=docs/requirements.txt pyproject.toml
 #
-alabaster==0.7.13
+alabaster==0.7.16
     # via sphinx
 asttokens==2.4.1
     # via stack-data
-babel==2.13.1
+babel==2.15.0
     # via sphinx
-black==23.11.0
+backports-tarfile==1.1.1
+    # via jaraco-context
+black==24.4.2
     # via
     #   fake-py
     #   file:///home/delusionalinsanity/repos/fake-py
-build==1.0.3
+build==1.2.1
     # via pip-tools
-certifi==2023.11.17
+certifi==2024.2.2
     # via requests
 cffi==1.16.0
     # via cryptography
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via
     #   black
     #   pip-tools
-coverage[toml]==7.3.2
+coverage[toml]==7.5.1
     # via
     #   coverage
     #   pytest-cov
-cryptography==41.0.5
+cryptography==42.0.7
     # via secretstorage
 decorator==5.1.1
     # via ipython
-detect-secrets==1.4.0
+detect-secrets==1.5.0
     # via
     #   fake-py
     #   file:///home/delusionalinsanity/repos/fake-py
-doc8==0.11.2
+doc8==1.1.1
     # via
     #   fake-py
     #   file:///home/delusionalinsanity/repos/fake-py
-docutils==0.18.1
+docutils==0.19
     # via
     #   doc8
     #   readme-renderer
     #   restructuredtext-lint
     #   sphinx
     #   sphinx-no-pragma
     #   sphinx-rtd-theme
-exceptiongroup==1.2.0
+exceptiongroup==1.2.1
     # via
     #   ipython
     #   pytest
 executing==2.0.1
     # via stack-data
-idna==3.6
+fake-py[dev,docs,test] @ file:///home/delusionalinsanity/repos/fake.py
+    # via fake.py (pyproject.toml)
+idna==3.7
     # via requests
 imagesize==1.4.1
     # via sphinx
-importlib-metadata==6.8.0
+importlib-metadata==7.1.0
     # via
     #   keyring
     #   twine
 iniconfig==2.0.0
     # via pytest
-ipython==8.18.0
+ipython==8.24.0
     # via
     #   fake-py
     #   file:///home/delusionalinsanity/repos/fake-py
-isort==5.12.0
+isort==5.13.2
     # via
     #   fake-py
     #   file:///home/delusionalinsanity/repos/fake-py
-jaraco-classes==3.3.0
+jaraco-classes==3.4.0
+    # via keyring
+jaraco-context==5.3.0
+    # via keyring
+jaraco-functools==4.0.1
     # via keyring
 jedi==0.19.1
     # via ipython
 jeepney==0.8.0
     # via
     #   keyring
     #   secretstorage
-jinja2==3.1.3
+jinja2==3.1.4
     # via sphinx
-keyring==24.3.0
+keyring==25.2.0
     # via twine
 markdown-it-py==3.0.0
     # via rich
-markupsafe==2.1.3
+markupsafe==2.1.5
     # via jinja2
-matplotlib-inline==0.1.6
+matplotlib-inline==0.1.7
     # via ipython
 mdurl==0.1.2
     # via markdown-it-py
-more-itertools==10.1.0
-    # via jaraco-classes
-mypy==1.7.1
+more-itertools==10.2.0
+    # via
+    #   jaraco-classes
+    #   jaraco-functools
+mypy==1.10.0
     # via
     #   fake-py
     #   file:///home/delusionalinsanity/repos/fake-py
 mypy-extensions==1.0.0
     # via
     #   black
     #   mypy
-nh3==0.2.14
+nh3==0.2.17
     # via readme-renderer
-packaging==23.2
+packaging==24.0
     # via
     #   black
     #   build
     #   pytest
     #   sphinx
-parso==0.8.3
+parso==0.8.4
     # via jedi
-pathspec==0.11.2
+pathspec==0.12.1
     # via black
 pbr==6.0.0
     # via stevedore
 pexpect==4.9.0
     # via ipython
-pip-tools==7.3.0
+pip-tools==7.4.1
     # via
     #   fake-py
     #   file:///home/delusionalinsanity/repos/fake-py
-pkginfo==1.9.6
+pkginfo==1.10.0
     # via twine
-platformdirs==4.0.0
+platformdirs==4.2.1
     # via black
-pluggy==1.3.0
+pluggy==1.5.0
     # via pytest
-prompt-toolkit==3.0.41
+prompt-toolkit==3.0.43
     # via ipython
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
-pycparser==2.21
+pycparser==2.22
     # via cffi
-pygments==2.17.2
+pygments==2.18.0
     # via
     #   doc8
     #   ipython
     #   readme-renderer
     #   rich
     #   sphinx
-pyproject-hooks==1.0.0
-    # via build
-pytest==7.4.3
+pyproject-hooks==1.1.0
+    # via
+    #   build
+    #   pip-tools
+pytest==8.2.0
     # via
     #   fake-py
     #   file:///home/delusionalinsanity/repos/fake-py
     #   pytest-cov
-pytest-cov==4.1.0
+pytest-cov==5.0.0
+    # via
+    #   fake-py
+    #   file:///home/delusionalinsanity/repos/fake-py
+pytest-rst==0.1.5
     # via
     #   fake-py
     #   file:///home/delusionalinsanity/repos/fake-py
 pyyaml==6.0.1
     # via detect-secrets
-readme-renderer==42.0
+readme-renderer==43.0
     # via twine
 requests==2.31.0
     # via
     #   detect-secrets
     #   requests-toolbelt
     #   sphinx
     #   twine
 requests-toolbelt==1.0.0
     # via twine
 restructuredtext-lint==1.4.0
     # via doc8
 rfc3986==2.0.0
     # via twine
-rich==13.7.0
+rich==13.7.1
     # via twine
-ruff==0.1.6
+ruff==0.4.3
     # via
     #   fake-py
     #   file:///home/delusionalinsanity/repos/fake-py
 secretstorage==3.3.3
     # via keyring
 six==1.16.0
     # via asttokens
@@ -186,74 +202,70 @@
     # via sphinx
 sphinx==5.3.0
     # via
     #   fake-py
     #   file:///home/delusionalinsanity/repos/fake-py
     #   sphinx-no-pragma
     #   sphinx-rtd-theme
-    #   sphinxcontrib-applehelp
-    #   sphinxcontrib-devhelp
-    #   sphinxcontrib-htmlhelp
     #   sphinxcontrib-jquery
-    #   sphinxcontrib-qthelp
-    #   sphinxcontrib-serializinghtml
 sphinx-no-pragma==0.1
     # via
     #   fake-py
     #   file:///home/delusionalinsanity/repos/fake-py
-sphinx-rtd-theme==1.3.0
+sphinx-rtd-theme==2.0.0
     # via
     #   fake-py
     #   file:///home/delusionalinsanity/repos/fake-py
-sphinxcontrib-applehelp==1.0.7
+sphinxcontrib-applehelp==1.0.8
     # via sphinx
-sphinxcontrib-devhelp==1.0.5
+sphinxcontrib-devhelp==1.0.6
     # via sphinx
-sphinxcontrib-htmlhelp==2.0.4
+sphinxcontrib-htmlhelp==2.0.5
     # via sphinx
 sphinxcontrib-jquery==4.1
     # via sphinx-rtd-theme
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
-sphinxcontrib-qthelp==1.0.6
+sphinxcontrib-qthelp==1.0.7
     # via sphinx
-sphinxcontrib-serializinghtml==1.1.9
+sphinxcontrib-serializinghtml==1.1.10
     # via sphinx
 stack-data==0.6.3
     # via ipython
-stevedore==5.1.0
+stevedore==5.2.0
     # via doc8
 tomli==2.0.1
     # via
     #   black
     #   build
     #   coverage
+    #   doc8
     #   mypy
     #   pip-tools
-    #   pyproject-hooks
     #   pytest
-traitlets==5.13.0
+traitlets==5.14.3
     # via
     #   ipython
     #   matplotlib-inline
-twine==4.0.2
+twine==5.0.0
     # via
     #   fake-py
     #   file:///home/delusionalinsanity/repos/fake-py
-typing-extensions==4.8.0
+typing-extensions==4.11.0
     # via
     #   black
+    #   ipython
     #   mypy
-urllib3==2.1.0
+urllib3==2.2.1
     # via
     #   requests
     #   twine
-wcwidth==0.2.12
+wcwidth==0.2.13
     # via prompt-toolkit
-wheel==0.41.3
+wheel==0.43.0
     # via pip-tools
-zipp==3.17.0
+zipp==3.18.1
     # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # pip
 # setuptools
```

### Comparing `fake.py-0.6.7/examples/customization/address/factories.py` & `fake_py-0.6.8/examples/customization/address/factories.py`

 * *Files identical despite different names*

### Comparing `fake.py-0.6.7/examples/customization/address/models.py` & `fake_py-0.6.8/examples/customization/address/models.py`

 * *Files identical despite different names*

### Comparing `fake.py-0.6.7/examples/customization/address/tests.py` & `fake_py-0.6.8/examples/customization/address/tests.py`

 * *Files identical despite different names*

### Comparing `fake.py-0.6.7/examples/customization/band/tests.py` & `fake_py-0.6.8/examples/customization/band/tests.py`

 * *Files identical despite different names*

### Comparing `fake.py-0.6.7/examples/customization/data.py` & `fake_py-0.6.8/examples/customization/data.py`

 * *Files identical despite different names*

### Comparing `fake.py-0.6.7/examples/customization/fake_address.py` & `fake_py-0.6.8/examples/customization/fake_address.py`

 * *Files identical despite different names*

### Comparing `fake.py-0.6.7/examples/customization/fake_band.py` & `fake_py-0.6.8/examples/customization/fake_band.py`

 * *Files identical despite different names*

### Comparing `fake.py-0.6.7/examples/customization/manage.py` & `fake_py-0.6.8/examples/customization/manage.py`

 * *Files identical despite different names*

### Comparing `fake.py-0.6.7/examples/customization/override_default_data.py` & `fake_py-0.6.8/examples/customization/override_default_data.py`

 * *Files identical despite different names*

### Comparing `fake.py-0.6.7/examples/dataclasses/article/factories.py` & `fake_py-0.6.8/examples/dataclasses/article/factories.py`

 * *Files identical despite different names*

### Comparing `fake.py-0.6.7/examples/dataclasses/article/models.py` & `fake_py-0.6.8/examples/dataclasses/article/models.py`

 * *Files identical despite different names*

### Comparing `fake.py-0.6.7/examples/dataclasses/article/tests.py` & `fake_py-0.6.8/examples/dataclasses/article/tests.py`

 * *Files identical despite different names*

### Comparing `fake.py-0.6.7/examples/dataclasses/manage.py` & `fake_py-0.6.8/examples/dataclasses/manage.py`

 * *Files identical despite different names*

### Comparing `fake.py-0.6.7/examples/django/article/factories.py` & `fake_py-0.6.8/examples/django/article/factories.py`

 * *Files identical despite different names*

### Comparing `fake.py-0.6.7/examples/django/article/migrations/0001_initial.py` & `fake_py-0.6.8/examples/django/article/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `fake.py-0.6.7/examples/django/article/models.py` & `fake_py-0.6.8/examples/django/article/models.py`

 * *Files identical despite different names*

### Comparing `fake.py-0.6.7/examples/django/article/tests.py` & `fake_py-0.6.8/examples/django/article/tests.py`

 * *Files identical despite different names*

### Comparing `fake.py-0.6.7/examples/django/blog/settings.py` & `fake_py-0.6.8/examples/django/blog/settings.py`

 * *Files identical despite different names*

### Comparing `fake.py-0.6.7/examples/django/blog/urls.py` & `fake_py-0.6.8/examples/django/blog/urls.py`

 * *Files identical despite different names*

### Comparing `fake.py-0.6.7/examples/django/manage.py` & `fake_py-0.6.8/examples/django/manage.py`

 * *Files identical despite different names*

### Comparing `fake.py-0.6.7/examples/hypothesis/manage.py` & `fake_py-0.6.8/examples/hypothesis/manage.py`

 * *Files identical despite different names*

### Comparing `fake.py-0.6.7/examples/hypothesis/tests.py` & `fake_py-0.6.8/examples/hypothesis/tests.py`

 * *Files identical despite different names*

### Comparing `fake.py-0.6.7/examples/lazyfuzzy/article/factories.py` & `fake_py-0.6.8/examples/lazyfuzzy/article/factories.py`

 * *Files identical despite different names*

### Comparing `fake.py-0.6.7/examples/lazyfuzzy/article/models.py` & `fake_py-0.6.8/examples/lazyfuzzy/article/models.py`

 * *Files identical despite different names*

### Comparing `fake.py-0.6.7/examples/lazyfuzzy/article/tests.py` & `fake_py-0.6.8/examples/lazyfuzzy/article/tests.py`

 * *Files identical despite different names*

### Comparing `fake.py-0.6.7/examples/lazyfuzzy/manage.py` & `fake_py-0.6.8/examples/lazyfuzzy/manage.py`

 * *Files identical despite different names*

### Comparing `fake.py-0.6.7/examples/pydantic/article/factories.py` & `fake_py-0.6.8/examples/pydantic/article/factories.py`

 * *Files identical despite different names*

### Comparing `fake.py-0.6.7/examples/pydantic/article/models.py` & `fake_py-0.6.8/examples/pydantic/article/models.py`

 * *Files identical despite different names*

### Comparing `fake.py-0.6.7/examples/pydantic/article/tests.py` & `fake_py-0.6.8/examples/pydantic/article/tests.py`

 * *Files identical despite different names*

### Comparing `fake.py-0.6.7/examples/pydantic/manage.py` & `fake_py-0.6.8/examples/pydantic/manage.py`

 * *Files identical despite different names*

### Comparing `fake.py-0.6.7/examples/sqlalchemy/article/factories.py` & `fake_py-0.6.8/examples/sqlalchemy/article/factories.py`

 * *Files identical despite different names*

### Comparing `fake.py-0.6.7/examples/sqlalchemy/article/models.py` & `fake_py-0.6.8/examples/sqlalchemy/article/models.py`

 * *Files identical despite different names*

### Comparing `fake.py-0.6.7/examples/sqlalchemy/article/tests.py` & `fake_py-0.6.8/examples/sqlalchemy/article/tests.py`

 * *Files identical despite different names*

### Comparing `fake.py-0.6.7/examples/sqlalchemy/manage.py` & `fake_py-0.6.8/examples/sqlalchemy/manage.py`

 * *Files identical despite different names*

### Comparing `fake.py-0.6.7/examples/tortoise/article/factories.py` & `fake_py-0.6.8/examples/tortoise/article/factories.py`

 * *Files identical despite different names*

### Comparing `fake.py-0.6.7/examples/tortoise/article/models.py` & `fake_py-0.6.8/examples/tortoise/article/models.py`

 * *Files identical despite different names*

### Comparing `fake.py-0.6.7/examples/tortoise/article/tests.py` & `fake_py-0.6.8/examples/tortoise/article/tests.py`

 * *Files identical despite different names*

### Comparing `fake.py-0.6.7/examples/tortoise/manage.py` & `fake_py-0.6.8/examples/tortoise/manage.py`

 * *Files identical despite different names*

### Comparing `fake.py-0.6.7/fake.py` & `fake_py-0.6.8/fake.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     get_args,
     get_origin,
     get_type_hints,
 )
 from uuid import UUID
 
 __title__ = "fake.py"
-__version__ = "0.6.7"
+__version__ = "0.6.8"
 __author__ = "Artur Barseghyan <artur.barseghyan@gmail.com>"
 __copyright__ = "2023-2024 Artur Barseghyan"
 __license__ = "MIT"
 __all__ = (
     "AuthorshipData",
     "BaseStorage",
     "DjangoModelFactory",
```

### Comparing `fake.py-0.6.7/fake.py.egg-info/PKG-INFO` & `fake_py-0.6.8/fake.py.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fake.py
-Version: 0.6.7
+Version: 0.6.8
 Summary: Minimalistic, standalone alternative fake data generator with no dependencies.
 Author-email: Artur Barseghyan <artur.barseghyan@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/barseghyanartur/fake.py/
 Project-URL: Bug Tracker, https://github.com/barseghyanartur/fake.py/issues
 Project-URL: Documentation, https://fakepy.readthedocs.io/
 Project-URL: Source Code, https://github.com/barseghyanartur/fake.py/
@@ -37,14 +37,15 @@
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
+Requires-Dist: pytest-rst; extra == "test"
 Provides-Extra: docs
 Requires-Dist: sphinx<6.0; extra == "docs"
 Requires-Dist: sphinx-rtd-theme>=1.3.0; extra == "docs"
 Requires-Dist: sphinx-no-pragma; extra == "docs"
 
 =======
 fake.py
@@ -160,100 +161,119 @@
 Usage
 =====
 Generate data
 -------------
 Person names
 ~~~~~~~~~~~~
 .. code-block:: python
+    :name: test_person_names
 
     from fake import FAKER
 
-    FAKER.first_name()
-    FAKER.last_name()
-    FAKER.name()
-    FAKER.username()
+    FAKER.first_name()  # str
+    FAKER.first_names()  # list[str]
+    FAKER.last_name()  # str
+    FAKER.last_names()  # list[str]
+    FAKER.name()  # str
+    FAKER.names()  # list[str]
+    FAKER.username()  # str
+    FAKER.usernames()  # list[str]
 
 Random texts
 ~~~~~~~~~~~~
 .. code-block:: python
+    :name: test_random_texts
 
     from fake import FAKER
 
-    FAKER.slug()
-    FAKER.word()
-    FAKER.sentence()
-    FAKER.paragraph()
-    FAKER.text()
+    FAKER.slug()  # str
+    FAKER.slugs()  # list[str]
+    FAKER.word()  # str
+    FAKER.words()  # list[str]
+    FAKER.sentence()  # str
+    FAKER.sentences()  # list[str]
+    FAKER.paragraph()  # str
+    FAKER.paragraphs()  # list[str]
+    FAKER.text()  # str
+    FAKER.texts()  # list[str]
 
 Internet
 ~~~~~~~~
 .. code-block:: python
+    :name: test_internet
 
     from fake import FAKER
 
-    FAKER.email()
-    FAKER.url()
-    FAKER.ipv4()
+    FAKER.email()  # str
+    FAKER.url()  # str
+    FAKER.image_url()  # str
+    FAKER.ipv4()  # str
 
 Filenames
 ~~~~~~~~~
 .. code-block:: python
+    :name: test_filenames
 
     from fake import FAKER
 
-    FAKER.filename()
+    FAKER.file_name()  # str
 
 Primitive data types
 ~~~~~~~~~~~~~~~~~~~~
 .. code-block:: python
+    :name: test_primitive_data_types
 
     from fake import FAKER
 
-    FAKER.pyint()
-    FAKER.pybool()
-    FAKER.pystr()
-    FAKER.pyfloat()
+    FAKER.pyint()  # int
+    FAKER.pybool()  # bool
+    FAKER.pystr()  # str
+    FAKER.pyfloat()  # flot
+    FAKER.uuid()  # uuid.UUID
 
 Dates
 ~~~~~
 .. code-block:: python
+    :name: test_dates
 
     from fake import FAKER
 
-    FAKER.date()
-    FAKER.date_time()
+    FAKER.date()  # datetime.date
+    FAKER.date_time()  # datetime.datetime
 
 Generate files
 --------------
 As bytes
 ~~~~~~~~
 .. code-block:: python
+    :name: test_generate_files_as_bytes
 
     from fake import FAKER
 
-    FAKER.pdf()
-    FAKER.docx()
-    FAKER.png()
-    FAKER.svg()
-    FAKER.bmp()
-    FAKER.gif()
+    FAKER.pdf()  # bytes
+    FAKER.docx()  # bytes
+    FAKER.png()  # bytes
+    FAKER.svg()  # bytes
+    FAKER.bmp()  # bytes
+    FAKER.gif()  # bytes
 
 As files on the file system
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~
 .. code-block:: python
+    :name: test_generate_files_as_files_on_file_system
 
     from fake import FAKER
 
-    FAKER.pdf_file()
-    FAKER.docx_file()
-    FAKER.png_file()
-    FAKER.svg_file()
-    FAKER.bmp_file()
-    FAKER.gif_file()
-    FAKER.txt_file()
+    FAKER.pdf_file()  # str
+    FAKER.docx_file()  # str
+    FAKER.png_file()  # str
+    FAKER.svg_file()  # str
+    FAKER.bmp_file()  # str
+    FAKER.gif_file()  # str
+    FAKER.txt_file()  # str
 
 Factories
 ---------
 This is how you could define factories for `Django`_'s built-in ``Group``
 and ``User`` models.
 
 .. code-block:: python
@@ -345,14 +365,15 @@
     )
 
 Customize
 ---------
 Make your own custom providers and utilize factories with them.
 
 .. code-block:: python
+    :name: test_customize
 
     import random
     import string
 
     from fake import Faker, Factory, provider
```

### Comparing `fake.py-0.6.7/fake.py.egg-info/SOURCES.txt` & `fake_py-0.6.8/fake.py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fake.py-0.6.7/pyproject.toml` & `fake_py-0.6.8/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name = "fake.py"
 description = "Minimalistic, standalone alternative fake data generator with no dependencies."
 readme = "README.rst"
-version = "0.6.7"
+version = "0.6.8"
 dependencies = []
 authors = [
     {name = "Artur Barseghyan", email = "artur.barseghyan@gmail.com"},
 ]
 license = {text = "MIT"}
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -46,14 +46,15 @@
     "pip-tools",
     "ruff",
     "twine",
 ]
 test = [
     "pytest",
     "pytest-cov",
+    "pytest-rst",
 ]
 docs = [
     "sphinx<6.0",
     "sphinx-rtd-theme>=1.3.0",
     "sphinx-no-pragma",
 ]
 
@@ -158,14 +159,16 @@
    "--cov-report=annotate",
    "--cov-append",
    "--capture=no",
 ]
 testpaths = [
     "fake.py",
     "__copy_fake.py",
+    "*.rst",
+    "**/*.rst",
 ]
 
 [tool.coverage.run]
 relative_files = true
 omit = [
     ".tox/*",
 ]
```

