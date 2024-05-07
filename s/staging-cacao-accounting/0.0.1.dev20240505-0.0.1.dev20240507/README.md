# Comparing `tmp/staging_cacao_accounting-0.0.1.dev20240505.tar.gz` & `tmp/staging_cacao_accounting-0.0.1.dev20240507.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "staging_cacao_accounting-0.0.1.dev20240505.tar", last modified: Sun May  5 15:13:21 2024, max compression
+gzip compressed data, was "staging_cacao_accounting-0.0.1.dev20240507.tar", last modified: Tue May  7 15:17:49 2024, max compression
```

## Comparing `staging_cacao_accounting-0.0.1.dev20240505.tar` & `staging_cacao_accounting-0.0.1.dev20240507.tar`

### file list

```diff
@@ -1,205 +1,205 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 15:13:21.569090 staging_cacao_accounting-0.0.1.dev20240505/
--rw-rw-rw-   0        0        0     1204 2024-04-17 03:35:19.000000 staging_cacao_accounting-0.0.1.dev20240505/Dockerfile
--rw-rw-rw-   0        0        0    11557 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/LICENSE
--rw-rw-rw-   0        0        0    29397 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/Licencias_de_Terceros.md
--rw-rw-rw-   0        0        0      522 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/MANIFEST.in
--rw-rw-rw-   0        0        0    19269 2024-05-05 15:13:21.564900 staging_cacao_accounting-0.0.1.dev20240505/PKG-INFO
--rw-rw-rw-   0        0        0     4391 2024-04-17 03:24:18.000000 staging_cacao_accounting-0.0.1.dev20240505/README.md
-drwxrwxrwx   0        0        0        0 2024-05-05 15:13:21.129905 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/
--rw-rw-rw-   0        0        0      702 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/I18N.py
--rw-rw-rw-   0        0        0     8063 2024-03-22 16:05:19.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/__init__.py
--rw-rw-rw-   0        0        0      814 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/__main__.py
-drwxrwxrwx   0        0        0        0 2024-05-05 15:13:21.134345 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/admin/
--rw-rw-rw-   0        0        0     1403 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/admin/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-05 15:13:21.138299 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/admin/registros/
--rw-rw-rw-   0        0        0      693 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/admin/registros/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-05 15:13:21.140764 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/admin/templates/
-drwxrwxrwx   0        0        0        0 2024-05-05 15:13:21.140764 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/admin/templates/admin/
--rw-rw-rw-   0        0        0      311 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/admin/templates/admin/modulos.html
--rw-rw-rw-   0        0        0      458 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/admin/templates/admin.html
-drwxrwxrwx   0        0        0        0 2024-05-05 15:13:21.145596 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/ajax/
--rw-rw-rw-   0        0        0      786 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/ajax/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-05 15:13:21.145596 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/app/
--rw-rw-rw-   0        0        0     2430 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/app/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-05 15:13:21.152430 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/app/templates/
--rw-rw-rw-   0        0        0      213 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/app/templates/app.html
--rw-rw-rw-   0        0        0      643 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/app/templates/development.html
-drwxrwxrwx   0        0        0        0 2024-05-05 15:13:21.167826 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/auth/
--rw-rw-rw-   0        0        0     3712 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/auth/__init__.py
--rw-rw-rw-   0        0        0     1085 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/auth/forms.py
--rw-rw-rw-   0        0        0    27146 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/auth/permisos.py
-drwxrwxrwx   0        0        0        0 2024-05-05 15:13:21.170354 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/auth/registros/
--rw-rw-rw-   0        0        0      974 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/auth/registros/__init__.py
--rw-rw-rw-   0        0        0     5566 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/auth/roles.py
-drwxrwxrwx   0        0        0        0 2024-05-05 15:13:21.176896 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/auth/templates/
--rw-rw-rw-   0        0        0     1738 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/auth/templates/login.html
--rw-rw-rw-   0        0        0     6923 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/auth/templates/test_roles.html
-drwxrwxrwx   0        0        0        0 2024-05-05 15:13:21.180091 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/bancos/
--rw-rw-rw-   0        0        0     1161 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/bancos/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-05 15:13:21.180091 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/bancos/templates/
--rw-rw-rw-   0        0        0      350 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/bancos/templates/bancos.html
--rw-rw-rw-   0        0        0     1154 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/cli.py
-drwxrwxrwx   0        0        0        0 2024-05-05 15:13:21.184564 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/compras/
--rw-rw-rw-   0        0        0     1114 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/compras/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-05 15:13:21.185776 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/compras/templates/
--rw-rw-rw-   0        0        0      344 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/compras/templates/compras.html
--rw-rw-rw-   0        0        0     6840 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/config.py
-drwxrwxrwx   0        0        0        0 2024-05-05 15:13:21.194683 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/contabilidad/
--rw-rw-rw-   0        0        0    18754 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/contabilidad/__init__.py
--rw-rw-rw-   0        0        0     3989 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/contabilidad/auxiliares.py
-drwxrwxrwx   0        0        0        0 2024-05-05 15:13:21.199880 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/contabilidad/ctas/
--rw-rw-rw-   0        0        0     2394 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/contabilidad/ctas/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-05 15:13:21.202439 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/contabilidad/ctas/catalogos/
--rw-rw-rw-   0        0        0    11237 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/contabilidad/ctas/catalogos/base.csv
--rw-rw-rw-   0        0        0     2635 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/contabilidad/forms.py
-drwxrwxrwx   0        0        0        0 2024-05-05 15:13:21.229171 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/contabilidad/registros/
--rw-rw-rw-   0        0        0      698 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/contabilidad/registros/__init__.py
--rw-rw-rw-   0        0        0     1028 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/contabilidad/registros/ccosto.py
--rw-rw-rw-   0        0        0     1014 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/contabilidad/registros/cuenta.py
--rw-rw-rw-   0        0        0     1136 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/contabilidad/registros/entidad.py
--rw-rw-rw-   0        0        0      999 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/contabilidad/registros/moneda.py
--rw-rw-rw-   0        0        0     1062 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/contabilidad/registros/periodo.py
--rw-rw-rw-   0        0        0     1019 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/contabilidad/registros/proyecto.py
--rw-rw-rw-   0        0        0     1009 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/contabilidad/registros/tasa_cambio.py
--rw-rw-rw-   0        0        0      998 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/contabilidad/registros/unidad.py
-drwxrwxrwx   0        0        0        0 2024-05-05 15:13:21.229171 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/contabilidad/templates/
-drwxrwxrwx   0        0        0        0 2024-05-05 15:13:21.288756 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/contabilidad/templates/contabilidad/
--rw-rw-rw-   0        0        0      837 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/contabilidad/templates/contabilidad/centro-costo.html
--rw-rw-rw-   0        0        0     3650 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/contabilidad/templates/contabilidad/centro-costo_lista.html
--rw-rw-rw-   0        0        0      829 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/contabilidad/templates/contabilidad/cuenta.html
--rw-rw-rw-   0        0        0     8935 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/contabilidad/templates/contabilidad/cuenta_lista.html
--rw-rw-rw-   0        0        0     2852 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/contabilidad/templates/contabilidad/entidad.html
--rw-rw-rw-   0        0        0     2960 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/contabilidad/templates/contabilidad/entidad_crear.html
--rw-rw-rw-   0        0        0     2459 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/contabilidad/templates/contabilidad/entidad_editar.html
--rw-rw-rw-   0        0        0     2240 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/contabilidad/templates/contabilidad/entidad_lista.html
--rw-rw-rw-   0        0        0     1363 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/contabilidad/templates/contabilidad/moneda_lista.html
--rw-rw-rw-   0        0        0     1702 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/contabilidad/templates/contabilidad/periodo_lista.html
--rw-rw-rw-   0        0        0     2097 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/contabilidad/templates/contabilidad/proyecto_lista.html
--rw-rw-rw-   0        0        0     1593 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/contabilidad/templates/contabilidad/tc_lista.html
--rw-rw-rw-   0        0        0     1001 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/contabilidad/templates/contabilidad/unidad.html
--rw-rw-rw-   0        0        0     2326 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/contabilidad/templates/contabilidad/unidad_crear.html
--rw-rw-rw-   0        0        0     1917 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/contabilidad/templates/contabilidad/unidad_lista.html
--rw-rw-rw-   0        0        0     1364 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/contabilidad/templates/contabilidad.html
-drwxrwxrwx   0        0        0        0 2024-05-05 15:13:21.296970 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/database/
--rw-rw-rw-   0        0        0    22671 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/database/__init__.py
--rw-rw-rw-   0        0        0     5736 2024-03-29 16:38:35.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/database/helpers.py
-drwxrwxrwx   0        0        0        0 2024-05-05 15:13:21.296970 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/datos/
--rw-rw-rw-   0        0        0      887 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/datos/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-05 15:13:21.302426 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/datos/base/
--rw-rw-rw-   0        0        0     5021 2024-03-29 16:38:58.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/datos/base/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-05 15:13:21.308385 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/datos/dev/
--rw-rw-rw-   0        0        0    34358 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/datos/dev/__init__.py
--rw-rw-rw-   0        0        0     2120 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/decorators.py
--rw-rw-rw-   0        0        0      354 2024-03-22 19:39:54.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/desktop.py
-drwxrwxrwx   0        0        0        0 2024-05-05 15:13:21.312412 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/exceptions/
--rw-rw-rw-   0        0        0     1325 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/exceptions/__init__.py
--rw-rw-rw-   0        0        0     1011 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/exceptions/mensajes.py
-drwxrwxrwx   0        0        0        0 2024-05-05 15:13:21.317783 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/inventario/
--rw-rw-rw-   0        0        0     1150 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/inventario/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-05 15:13:21.320005 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/inventario/templates/
--rw-rw-rw-   0        0        0      358 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/inventario/templates/inventario.html
--rw-rw-rw-   0        0        0      807 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/loggin.py
--rw-rw-rw-   0        0        0      837 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/metadata.py
-drwxrwxrwx   0        0        0        0 2024-05-05 15:13:21.063023 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/misc/
-drwxrwxrwx   0        0        0        0 2024-05-05 15:13:21.320005 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/misc/ejemplos/
--rw-rw-rw-   0        0        0      596 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/misc/ejemplos/cacao-accounting.unit
--rw-rw-rw-   0        0        0     4066 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/modulos.py
-drwxrwxrwx   0        0        0        0 2024-05-05 15:13:21.325544 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/registro/
--rw-rw-rw-   0        0        0     6179 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/registro/__init__.py
--rw-rw-rw-   0        0        0     2043 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/server.py
-drwxrwxrwx   0        0        0        0 2024-05-05 15:13:21.332952 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/
-drwxrwxrwx   0        0        0        0 2024-05-05 15:13:21.348026 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/css/
--rw-rw-rw-   0        0        0       35 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/css/cacaoaccounting.css
--rw-rw-rw-   0        0        0     1521 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/css/dashboard.css
--rw-rw-rw-   0        0        0     2658 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/css/purecss-treeview.css
--rw-rw-rw-   0        0        0      769 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/css/signin.css
--rw-rw-rw-   0        0        0      760 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/manifest.json
-drwxrwxrwx   0        0        0        0 2024-05-05 15:13:21.394077 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/
--rw-rw-rw-   0        0        0   480402 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/Cacao Accounting SVG.svg
--rw-rw-rw-   0        0        0    27950 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/Cacao Accounting-01.png
-drwxrwxrwx   0        0        0        0 2024-05-05 15:13:21.410735 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/Linux/
--rw-rw-rw-   0        0        0      740 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/Linux/Cacao Accounting 16px.png
--rw-rw-rw-   0        0        0    28208 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/Linux/Cacao Accounting 256px.png
--rw-rw-rw-   0        0        0     2212 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/Linux/Cacao Accounting 32px.png
--rw-rw-rw-   0        0        0     3851 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/Linux/Cacao Accounting 48px.png
--rw-rw-rw-   0        0        0     5536 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/Linux/Cacao Accounting 64px.png
--rw-rw-rw-   0        0        0   457104 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/Linux/Cacao Accounting Ícono SVG.svg
-drwxrwxrwx   0        0        0        0 2024-05-05 15:13:21.424777 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/Web/
--rw-rw-rw-   0        0        0   480402 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/Web/Cacao Accounting SVG.svg
--rw-rw-rw-   0        0        0   457104 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/Web/Cacao Accounting Ícono SVG.svg
--rw-rw-rw-   0        0        0    27950 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/Web/Cacao Accounting-01.png
--rw-rw-rw-   0        0        0    28208 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/Web/Cacao Accounting.png
-drwxrwxrwx   0        0        0        0 2024-05-05 15:13:21.446991 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/Windows/
--rw-rw-rw-   0        0        0     1150 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/Windows/Cacao Accounting 16px.ico
--rw-rw-rw-   0        0        0   270398 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/Windows/Cacao Accounting 256px.ico
--rw-rw-rw-   0        0        0     4286 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/Windows/Cacao Accounting 32px.ico
--rw-rw-rw-   0        0        0     9662 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/Windows/Cacao Accounting 48px.ico
--rw-rw-rw-   0        0        0    16958 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/Windows/Cacao Accounting 64px.ico
--rw-rw-rw-   0        0        0    61298 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/Windows/Cacao Accounting múltilple tamaño.ico
--rw-rw-rw-   0        0        0    20365 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/brand.svg
--rw-rw-rw-   0        0        0    27950 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/cacao_accounting _logo.png
--rw-rw-rw-   0        0        0    20365 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/cacao_accounting _logo.svg
--rw-rw-rw-   0        0        0    28208 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/cacao_accounting.png
--rw-rw-rw-   0        0        0   457104 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/cacao_accounting.svg
--rw-rw-rw-   0        0        0   480402 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/cacao_logo.svg
--rw-rw-rw-   0        0        0      301 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/circle-solid.svg
-drwxrwxrwx   0        0        0        0 2024-05-05 15:13:21.514899 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/favicon/
--rw-rw-rw-   0        0        0    23238 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/favicon/android-icon-144x144.png
--rw-rw-rw-   0        0        0    30582 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/favicon/android-icon-192x192.png
--rw-rw-rw-   0        0        0     3820 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/favicon/android-icon-36x36.png
--rw-rw-rw-   0        0        0     5627 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/favicon/android-icon-48x48.png
--rw-rw-rw-   0        0        0     9202 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/favicon/android-icon-72x72.png
--rw-rw-rw-   0        0        0    13210 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/favicon/android-icon-96x96.png
--rw-rw-rw-   0        0        0    16894 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/favicon/apple-icon-114x114.png
--rw-rw-rw-   0        0        0    18160 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/favicon/apple-icon-120x120.png
--rw-rw-rw-   0        0        0    23238 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/favicon/apple-icon-144x144.png
--rw-rw-rw-   0        0        0    24785 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/favicon/apple-icon-152x152.png
--rw-rw-rw-   0        0        0    31048 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/favicon/apple-icon-180x180.png
--rw-rw-rw-   0        0        0     6938 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/favicon/apple-icon-57x57.png
--rw-rw-rw-   0        0        0     7341 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/favicon/apple-icon-60x60.png
--rw-rw-rw-   0        0        0     9202 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/favicon/apple-icon-72x72.png
--rw-rw-rw-   0        0        0     9743 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/favicon/apple-icon-76x76.png
--rw-rw-rw-   0        0        0    31156 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/favicon/apple-icon-precomposed.png
--rw-rw-rw-   0        0        0    31156 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/favicon/apple-icon.png
--rw-rw-rw-   0        0        0     1607 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/favicon/favicon-16x16.png
--rw-rw-rw-   0        0        0     3317 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/favicon/favicon-32x32.png
--rw-rw-rw-   0        0        0    13210 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/favicon/favicon-96x96.png
--rw-rw-rw-   0        0        0     1150 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/favicon/favicon.ico
--rw-rw-rw-   0        0        0    23238 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/favicon/ms-icon-144x144.png
--rw-rw-rw-   0        0        0    24371 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/favicon/ms-icon-150x150.png
--rw-rw-rw-   0        0        0    67679 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/favicon/ms-icon-310x310.png
--rw-rw-rw-   0        0        0     8745 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/favicon/ms-icon-70x70.png
--rw-rw-rw-   0        0        0      740 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/favicon-16x16.png
--rw-rw-rw-   0        0        0     2212 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/favicon-32x32.png
--rw-rw-rw-   0        0        0     1883 2024-04-17 03:24:18.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/package-lock.json
--rw-rw-rw-   0        0        0      581 2024-04-17 03:24:18.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/package.json
-drwxrwxrwx   0        0        0        0 2024-05-05 15:13:21.536246 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/templates/
--rw-rw-rw-   0        0        0     1161 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/templates/400.html
--rw-rw-rw-   0        0        0     1170 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/templates/403.html
--rw-rw-rw-   0        0        0     1144 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/templates/404.html
--rw-rw-rw-   0        0        0     1458 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/templates/base.html
--rw-rw-rw-   0        0        0     8312 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/templates/macros.html
-drwxrwxrwx   0        0        0        0 2024-05-05 15:13:21.539750 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/templates/setup/
--rw-rw-rw-   0        0        0     2922 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/templates/setup/setup.html
-drwxrwxrwx   0        0        0        0 2024-05-05 15:13:21.540640 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/transaccion/
--rw-rw-rw-   0        0        0     2784 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/transaccion/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-05 15:13:21.546117 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/validaciones/
--rw-rw-rw-   0        0        0     1277 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/validaciones/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-05 15:13:21.548124 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/ventas/
--rw-rw-rw-   0        0        0     1082 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/ventas/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-05 15:13:21.548124 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/ventas/templates/
--rw-rw-rw-   0        0        0      343 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/ventas/templates/ventas.html
--rw-rw-rw-   0        0        0      978 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/version.py
--rw-rw-rw-   0        0        0     1608 2024-05-05 15:12:19.000000 staging_cacao_accounting-0.0.1.dev20240505/pyproject.toml
--rw-rw-rw-   0        0        0      285 2024-04-17 03:24:18.000000 staging_cacao_accounting-0.0.1.dev20240505/requirements.txt
--rw-rw-rw-   0        0        0      201 2024-05-05 15:13:21.569090 staging_cacao_accounting-0.0.1.dev20240505/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-05 15:13:21.564900 staging_cacao_accounting-0.0.1.dev20240505/staging_cacao_accounting.egg-info/
--rw-rw-rw-   0        0        0    19269 2024-05-05 15:13:19.000000 staging_cacao_accounting-0.0.1.dev20240505/staging_cacao_accounting.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7512 2024-05-05 15:13:21.000000 staging_cacao_accounting-0.0.1.dev20240505/staging_cacao_accounting.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 15:13:19.000000 staging_cacao_accounting-0.0.1.dev20240505/staging_cacao_accounting.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-05-05 15:13:19.000000 staging_cacao_accounting-0.0.1.dev20240505/staging_cacao_accounting.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      230 2024-05-05 15:13:19.000000 staging_cacao_accounting-0.0.1.dev20240505/staging_cacao_accounting.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-05 15:13:19.000000 staging_cacao_accounting-0.0.1.dev20240505/staging_cacao_accounting.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-05 15:13:21.562895 staging_cacao_accounting-0.0.1.dev20240505/tests/
--rw-rw-rw-   0        0        0       48 2024-04-17 03:28:01.000000 staging_cacao_accounting-0.0.1.dev20240505/tests/test_basicos.py
--rw-rw-rw-   0        0        0     1104 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240505/wsgi.py
+drwxrwxrwx   0        0        0        0 2024-05-07 15:17:49.515684 staging_cacao_accounting-0.0.1.dev20240507/
+-rw-rw-rw-   0        0        0     1204 2024-04-17 03:35:19.000000 staging_cacao_accounting-0.0.1.dev20240507/Dockerfile
+-rw-rw-rw-   0        0        0    11557 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/LICENSE
+-rw-rw-rw-   0        0        0    29397 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/Licencias_de_Terceros.md
+-rw-rw-rw-   0        0        0      522 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/MANIFEST.in
+-rw-rw-rw-   0        0        0    19143 2024-05-07 15:17:49.515684 staging_cacao_accounting-0.0.1.dev20240507/PKG-INFO
+-rw-rw-rw-   0        0        0     4391 2024-04-17 03:24:18.000000 staging_cacao_accounting-0.0.1.dev20240507/README.md
+drwxrwxrwx   0        0        0        0 2024-05-07 15:17:49.015836 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/
+-rw-rw-rw-   0        0        0      702 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/I18N.py
+-rw-rw-rw-   0        0        0     8063 2024-03-22 16:05:19.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/__init__.py
+-rw-rw-rw-   0        0        0      814 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/__main__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 15:17:49.015836 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/admin/
+-rw-rw-rw-   0        0        0     1403 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/admin/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 15:17:49.025090 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/admin/registros/
+-rw-rw-rw-   0        0        0      693 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/admin/registros/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 15:17:49.025090 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/admin/templates/
+drwxrwxrwx   0        0        0        0 2024-05-07 15:17:49.032103 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/admin/templates/admin/
+-rw-rw-rw-   0        0        0      311 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/admin/templates/admin/modulos.html
+-rw-rw-rw-   0        0        0      458 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/admin/templates/admin.html
+drwxrwxrwx   0        0        0        0 2024-05-07 15:17:49.040296 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/ajax/
+-rw-rw-rw-   0        0        0      786 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/ajax/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 15:17:49.040924 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/app/
+-rw-rw-rw-   0        0        0     2430 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/app/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 15:17:49.048431 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/app/templates/
+-rw-rw-rw-   0        0        0      213 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/app/templates/app.html
+-rw-rw-rw-   0        0        0      643 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/app/templates/development.html
+drwxrwxrwx   0        0        0        0 2024-05-07 15:17:49.074279 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/auth/
+-rw-rw-rw-   0        0        0     3712 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/auth/__init__.py
+-rw-rw-rw-   0        0        0     1085 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/auth/forms.py
+-rw-rw-rw-   0        0        0    27146 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/auth/permisos.py
+drwxrwxrwx   0        0        0        0 2024-05-07 15:17:49.080919 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/auth/registros/
+-rw-rw-rw-   0        0        0      974 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/auth/registros/__init__.py
+-rw-rw-rw-   0        0        0     5566 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/auth/roles.py
+drwxrwxrwx   0        0        0        0 2024-05-07 15:17:49.090892 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/auth/templates/
+-rw-rw-rw-   0        0        0     1738 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/auth/templates/login.html
+-rw-rw-rw-   0        0        0     6923 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/auth/templates/test_roles.html
+drwxrwxrwx   0        0        0        0 2024-05-07 15:17:49.097399 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/bancos/
+-rw-rw-rw-   0        0        0     1161 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/bancos/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 15:17:49.097399 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/bancos/templates/
+-rw-rw-rw-   0        0        0      350 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/bancos/templates/bancos.html
+-rw-rw-rw-   0        0        0     1154 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/cli.py
+drwxrwxrwx   0        0        0        0 2024-05-07 15:17:49.108113 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/compras/
+-rw-rw-rw-   0        0        0     1114 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/compras/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 15:17:49.113625 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/compras/templates/
+-rw-rw-rw-   0        0        0      344 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/compras/templates/compras.html
+-rw-rw-rw-   0        0        0     6840 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/config.py
+drwxrwxrwx   0        0        0        0 2024-05-07 15:17:49.129760 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/contabilidad/
+-rw-rw-rw-   0        0        0    18754 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/contabilidad/__init__.py
+-rw-rw-rw-   0        0        0     3989 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/contabilidad/auxiliares.py
+drwxrwxrwx   0        0        0        0 2024-05-07 15:17:49.129760 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/contabilidad/ctas/
+-rw-rw-rw-   0        0        0     2394 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/contabilidad/ctas/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 15:17:49.137772 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/contabilidad/ctas/catalogos/
+-rw-rw-rw-   0        0        0    11237 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/contabilidad/ctas/catalogos/base.csv
+-rw-rw-rw-   0        0        0     2635 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/contabilidad/forms.py
+drwxrwxrwx   0        0        0        0 2024-05-07 15:17:49.176025 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/contabilidad/registros/
+-rw-rw-rw-   0        0        0      698 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/contabilidad/registros/__init__.py
+-rw-rw-rw-   0        0        0     1028 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/contabilidad/registros/ccosto.py
+-rw-rw-rw-   0        0        0     1014 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/contabilidad/registros/cuenta.py
+-rw-rw-rw-   0        0        0     1136 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/contabilidad/registros/entidad.py
+-rw-rw-rw-   0        0        0      999 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/contabilidad/registros/moneda.py
+-rw-rw-rw-   0        0        0     1062 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/contabilidad/registros/periodo.py
+-rw-rw-rw-   0        0        0     1019 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/contabilidad/registros/proyecto.py
+-rw-rw-rw-   0        0        0     1009 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/contabilidad/registros/tasa_cambio.py
+-rw-rw-rw-   0        0        0      998 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/contabilidad/registros/unidad.py
+drwxrwxrwx   0        0        0        0 2024-05-07 15:17:49.177946 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/contabilidad/templates/
+drwxrwxrwx   0        0        0        0 2024-05-07 15:17:49.229179 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/contabilidad/templates/contabilidad/
+-rw-rw-rw-   0        0        0      837 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/contabilidad/templates/contabilidad/centro-costo.html
+-rw-rw-rw-   0        0        0     3650 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/contabilidad/templates/contabilidad/centro-costo_lista.html
+-rw-rw-rw-   0        0        0      829 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/contabilidad/templates/contabilidad/cuenta.html
+-rw-rw-rw-   0        0        0     8935 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/contabilidad/templates/contabilidad/cuenta_lista.html
+-rw-rw-rw-   0        0        0     2852 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/contabilidad/templates/contabilidad/entidad.html
+-rw-rw-rw-   0        0        0     2960 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/contabilidad/templates/contabilidad/entidad_crear.html
+-rw-rw-rw-   0        0        0     2459 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/contabilidad/templates/contabilidad/entidad_editar.html
+-rw-rw-rw-   0        0        0     2240 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/contabilidad/templates/contabilidad/entidad_lista.html
+-rw-rw-rw-   0        0        0     1363 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/contabilidad/templates/contabilidad/moneda_lista.html
+-rw-rw-rw-   0        0        0     1702 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/contabilidad/templates/contabilidad/periodo_lista.html
+-rw-rw-rw-   0        0        0     2097 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/contabilidad/templates/contabilidad/proyecto_lista.html
+-rw-rw-rw-   0        0        0     1593 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/contabilidad/templates/contabilidad/tc_lista.html
+-rw-rw-rw-   0        0        0     1001 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/contabilidad/templates/contabilidad/unidad.html
+-rw-rw-rw-   0        0        0     2326 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/contabilidad/templates/contabilidad/unidad_crear.html
+-rw-rw-rw-   0        0        0     1917 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/contabilidad/templates/contabilidad/unidad_lista.html
+-rw-rw-rw-   0        0        0     1364 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/contabilidad/templates/contabilidad.html
+drwxrwxrwx   0        0        0        0 2024-05-07 15:17:49.237664 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/database/
+-rw-rw-rw-   0        0        0    22671 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/database/__init__.py
+-rw-rw-rw-   0        0        0     5736 2024-03-29 16:38:35.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/database/helpers.py
+drwxrwxrwx   0        0        0        0 2024-05-07 15:17:49.245919 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/datos/
+-rw-rw-rw-   0        0        0      887 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/datos/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 15:17:49.246771 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/datos/base/
+-rw-rw-rw-   0        0        0     5021 2024-03-29 16:38:58.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/datos/base/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 15:17:49.254274 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/datos/dev/
+-rw-rw-rw-   0        0        0    34358 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/datos/dev/__init__.py
+-rw-rw-rw-   0        0        0     2120 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/decorators.py
+-rw-rw-rw-   0        0        0      354 2024-03-22 19:39:54.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/desktop.py
+drwxrwxrwx   0        0        0        0 2024-05-07 15:17:49.261146 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/exceptions/
+-rw-rw-rw-   0        0        0     1325 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/exceptions/__init__.py
+-rw-rw-rw-   0        0        0     1011 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/exceptions/mensajes.py
+drwxrwxrwx   0        0        0        0 2024-05-07 15:17:49.262092 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/inventario/
+-rw-rw-rw-   0        0        0     1150 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/inventario/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 15:17:49.262092 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/inventario/templates/
+-rw-rw-rw-   0        0        0      358 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/inventario/templates/inventario.html
+-rw-rw-rw-   0        0        0      807 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/loggin.py
+-rw-rw-rw-   0        0        0      837 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/metadata.py
+drwxrwxrwx   0        0        0        0 2024-05-07 15:17:48.900444 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/misc/
+drwxrwxrwx   0        0        0        0 2024-05-07 15:17:49.270094 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/misc/ejemplos/
+-rw-rw-rw-   0        0        0      596 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/misc/ejemplos/cacao-accounting.unit
+-rw-rw-rw-   0        0        0     4066 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/modulos.py
+drwxrwxrwx   0        0        0        0 2024-05-07 15:17:49.270660 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/registro/
+-rw-rw-rw-   0        0        0     6179 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/registro/__init__.py
+-rw-rw-rw-   0        0        0     2043 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/server.py
+drwxrwxrwx   0        0        0        0 2024-05-07 15:17:49.278165 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/
+drwxrwxrwx   0        0        0        0 2024-05-07 15:17:49.286192 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/css/
+-rw-rw-rw-   0        0        0       35 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/css/cacaoaccounting.css
+-rw-rw-rw-   0        0        0     1521 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/css/dashboard.css
+-rw-rw-rw-   0        0        0     2658 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/css/purecss-treeview.css
+-rw-rw-rw-   0        0        0      769 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/css/signin.css
+-rw-rw-rw-   0        0        0      760 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/manifest.json
+drwxrwxrwx   0        0        0        0 2024-05-07 15:17:49.335606 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/
+-rw-rw-rw-   0        0        0   480402 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/Cacao Accounting SVG.svg
+-rw-rw-rw-   0        0        0    27950 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/Cacao Accounting-01.png
+drwxrwxrwx   0        0        0        0 2024-05-07 15:17:49.352881 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/Linux/
+-rw-rw-rw-   0        0        0      740 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/Linux/Cacao Accounting 16px.png
+-rw-rw-rw-   0        0        0    28208 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/Linux/Cacao Accounting 256px.png
+-rw-rw-rw-   0        0        0     2212 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/Linux/Cacao Accounting 32px.png
+-rw-rw-rw-   0        0        0     3851 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/Linux/Cacao Accounting 48px.png
+-rw-rw-rw-   0        0        0     5536 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/Linux/Cacao Accounting 64px.png
+-rw-rw-rw-   0        0        0   457104 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/Linux/Cacao Accounting Ícono SVG.svg
+drwxrwxrwx   0        0        0        0 2024-05-07 15:17:49.368587 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/Web/
+-rw-rw-rw-   0        0        0   480402 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/Web/Cacao Accounting SVG.svg
+-rw-rw-rw-   0        0        0   457104 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/Web/Cacao Accounting Ícono SVG.svg
+-rw-rw-rw-   0        0        0    27950 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/Web/Cacao Accounting-01.png
+-rw-rw-rw-   0        0        0    28208 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/Web/Cacao Accounting.png
+drwxrwxrwx   0        0        0        0 2024-05-07 15:17:49.391393 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/Windows/
+-rw-rw-rw-   0        0        0     1150 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/Windows/Cacao Accounting 16px.ico
+-rw-rw-rw-   0        0        0   270398 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/Windows/Cacao Accounting 256px.ico
+-rw-rw-rw-   0        0        0     4286 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/Windows/Cacao Accounting 32px.ico
+-rw-rw-rw-   0        0        0     9662 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/Windows/Cacao Accounting 48px.ico
+-rw-rw-rw-   0        0        0    16958 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/Windows/Cacao Accounting 64px.ico
+-rw-rw-rw-   0        0        0    61298 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/Windows/Cacao Accounting múltilple tamaño.ico
+-rw-rw-rw-   0        0        0    20365 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/brand.svg
+-rw-rw-rw-   0        0        0    27950 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/cacao_accounting _logo.png
+-rw-rw-rw-   0        0        0    20365 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/cacao_accounting _logo.svg
+-rw-rw-rw-   0        0        0    28208 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/cacao_accounting.png
+-rw-rw-rw-   0        0        0   457104 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/cacao_accounting.svg
+-rw-rw-rw-   0        0        0   480402 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/cacao_logo.svg
+-rw-rw-rw-   0        0        0      301 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/circle-solid.svg
+drwxrwxrwx   0        0        0        0 2024-05-07 15:17:49.466921 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/favicon/
+-rw-rw-rw-   0        0        0    23238 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/favicon/android-icon-144x144.png
+-rw-rw-rw-   0        0        0    30582 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/favicon/android-icon-192x192.png
+-rw-rw-rw-   0        0        0     3820 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/favicon/android-icon-36x36.png
+-rw-rw-rw-   0        0        0     5627 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/favicon/android-icon-48x48.png
+-rw-rw-rw-   0        0        0     9202 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/favicon/android-icon-72x72.png
+-rw-rw-rw-   0        0        0    13210 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/favicon/android-icon-96x96.png
+-rw-rw-rw-   0        0        0    16894 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/favicon/apple-icon-114x114.png
+-rw-rw-rw-   0        0        0    18160 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/favicon/apple-icon-120x120.png
+-rw-rw-rw-   0        0        0    23238 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/favicon/apple-icon-144x144.png
+-rw-rw-rw-   0        0        0    24785 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/favicon/apple-icon-152x152.png
+-rw-rw-rw-   0        0        0    31048 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/favicon/apple-icon-180x180.png
+-rw-rw-rw-   0        0        0     6938 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/favicon/apple-icon-57x57.png
+-rw-rw-rw-   0        0        0     7341 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/favicon/apple-icon-60x60.png
+-rw-rw-rw-   0        0        0     9202 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/favicon/apple-icon-72x72.png
+-rw-rw-rw-   0        0        0     9743 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/favicon/apple-icon-76x76.png
+-rw-rw-rw-   0        0        0    31156 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/favicon/apple-icon-precomposed.png
+-rw-rw-rw-   0        0        0    31156 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/favicon/apple-icon.png
+-rw-rw-rw-   0        0        0     1607 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/favicon/favicon-16x16.png
+-rw-rw-rw-   0        0        0     3317 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/favicon/favicon-32x32.png
+-rw-rw-rw-   0        0        0    13210 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/favicon/favicon-96x96.png
+-rw-rw-rw-   0        0        0     1150 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/favicon/favicon.ico
+-rw-rw-rw-   0        0        0    23238 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/favicon/ms-icon-144x144.png
+-rw-rw-rw-   0        0        0    24371 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/favicon/ms-icon-150x150.png
+-rw-rw-rw-   0        0        0    67679 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/favicon/ms-icon-310x310.png
+-rw-rw-rw-   0        0        0     8745 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/favicon/ms-icon-70x70.png
+-rw-rw-rw-   0        0        0      740 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/favicon-16x16.png
+-rw-rw-rw-   0        0        0     2212 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/favicon-32x32.png
+-rw-rw-rw-   0        0        0     1883 2024-04-17 03:24:18.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/package-lock.json
+-rw-rw-rw-   0        0        0      581 2024-04-17 03:24:18.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/package.json
+drwxrwxrwx   0        0        0        0 2024-05-07 15:17:49.483113 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/templates/
+-rw-rw-rw-   0        0        0     1161 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/templates/400.html
+-rw-rw-rw-   0        0        0     1170 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/templates/403.html
+-rw-rw-rw-   0        0        0     1144 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/templates/404.html
+-rw-rw-rw-   0        0        0     1458 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/templates/base.html
+-rw-rw-rw-   0        0        0     8312 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/templates/macros.html
+drwxrwxrwx   0        0        0        0 2024-05-07 15:17:49.483113 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/templates/setup/
+-rw-rw-rw-   0        0        0     2922 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/templates/setup/setup.html
+drwxrwxrwx   0        0        0        0 2024-05-07 15:17:49.483113 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/transaccion/
+-rw-rw-rw-   0        0        0     2784 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/transaccion/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 15:17:49.491138 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/validaciones/
+-rw-rw-rw-   0        0        0     1277 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/validaciones/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 15:17:49.491138 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/ventas/
+-rw-rw-rw-   0        0        0     1082 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/ventas/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 15:17:49.499633 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/ventas/templates/
+-rw-rw-rw-   0        0        0      343 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/ventas/templates/ventas.html
+-rw-rw-rw-   0        0        0      978 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/version.py
+-rw-rw-rw-   0        0        0     1608 2024-05-05 15:12:19.000000 staging_cacao_accounting-0.0.1.dev20240507/pyproject.toml
+-rw-rw-rw-   0        0        0      234 2024-05-07 15:16:56.000000 staging_cacao_accounting-0.0.1.dev20240507/requirements.txt
+-rw-rw-rw-   0        0        0      201 2024-05-07 15:17:49.515684 staging_cacao_accounting-0.0.1.dev20240507/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-07 15:17:49.515684 staging_cacao_accounting-0.0.1.dev20240507/staging_cacao_accounting.egg-info/
+-rw-rw-rw-   0        0        0    19143 2024-05-07 15:17:47.000000 staging_cacao_accounting-0.0.1.dev20240507/staging_cacao_accounting.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7512 2024-05-07 15:17:48.000000 staging_cacao_accounting-0.0.1.dev20240507/staging_cacao_accounting.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 15:17:47.000000 staging_cacao_accounting-0.0.1.dev20240507/staging_cacao_accounting.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-05-07 15:17:47.000000 staging_cacao_accounting-0.0.1.dev20240507/staging_cacao_accounting.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      184 2024-05-07 15:17:47.000000 staging_cacao_accounting-0.0.1.dev20240507/staging_cacao_accounting.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-07 15:17:47.000000 staging_cacao_accounting-0.0.1.dev20240507/staging_cacao_accounting.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-07 15:17:49.507661 staging_cacao_accounting-0.0.1.dev20240507/tests/
+-rw-rw-rw-   0        0        0       48 2024-04-17 03:28:01.000000 staging_cacao_accounting-0.0.1.dev20240507/tests/test_basicos.py
+-rw-rw-rw-   0        0        0     1104 2024-03-22 15:37:45.000000 staging_cacao_accounting-0.0.1.dev20240507/wsgi.py
```

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/Dockerfile` & `staging_cacao_accounting-0.0.1.dev20240507/Dockerfile`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/LICENSE` & `staging_cacao_accounting-0.0.1.dev20240507/LICENSE`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/Licencias_de_Terceros.md` & `staging_cacao_accounting-0.0.1.dev20240507/Licencias_de_Terceros.md`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/MANIFEST.in` & `staging_cacao_accounting-0.0.1.dev20240507/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/PKG-INFO` & `staging_cacao_accounting-0.0.1.dev20240507/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: staging_cacao_accounting
-Version: 0.0.1.dev20240505
+Version: 0.0.1.dev20240507
 Summary: Accounting solution for the management of Accounts Payable, Accounts Receivable, Inventory, Treasury and General Accounting.
 Author-email: William Moreno Reyes <williamjmorenor@gmail.com>, BMO Soluciones <development@bmogroup.solutions>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -221,34 +221,29 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: Licencias_de_Terceros.md
 Requires-Dist: alembic
 Requires-Dist: bcrypt
 Requires-Dist: babel
+Requires-Dist: cryptography
 Requires-Dist: Flask
-Requires-Dist: Flask[async]
 Requires-Dist: Flask-Alembic
 Requires-Dist: flask-babel
 Requires-Dist: flask-login
 Requires-Dist: flask-sqlalchemy
 Requires-Dist: flask-wtf
 Requires-Dist: loguru
-Requires-Dist: lxml
-Requires-Dist: pdf_reports
-Requires-Dist: openpyxl
+Requires-Dist: pg8000
+Requires-Dist: PyMySQL
 Requires-Dist: sqlalchemy
 Requires-Dist: teritorio
 Requires-Dist: waitress
 Requires-Dist: wtforms
 Requires-Dist: WTForms-SQLAlchemy
-Requires-Dist: pillow
-Requires-Dist: pg8000
-Requires-Dist: PyMySQL
-Requires-Dist: cryptography
 
 ![Logo](https://raw.githubusercontent.com/cacao-accounting/cacao-accounting/development/cacao_accounting/static/media/cacao_accounting%20_logo.png)
 
 # Cacao Accounting
 
 ![PyPI - License](https://img.shields.io/pypi/l/cacao-accounting?color=green&logo=apache)
 [![Pruebas de Integración Continua](https://github.com/cacao-accounting/cacao-accounting/actions/workflows/python-package.yml/badge.svg)](https://github.com/cacao-accounting/cacao-accounting/actions/workflows/python-package.yml)
```

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/README.md` & `staging_cacao_accounting-0.0.1.dev20240507/README.md`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/I18N.py` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/I18N.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/__init__.py` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/__init__.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/__main__.py` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/__main__.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/admin/__init__.py` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/admin/registros/__init__.py` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/admin/registros/__init__.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/ajax/__init__.py` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/ajax/__init__.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/app/__init__.py` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/app/__init__.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/app/templates/development.html` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/app/templates/development.html`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/auth/__init__.py` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/auth/forms.py` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/auth/forms.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/auth/permisos.py` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/auth/permisos.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/auth/registros/__init__.py` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/auth/registros/__init__.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/auth/roles.py` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/auth/roles.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/auth/templates/login.html` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/auth/templates/login.html`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/auth/templates/test_roles.html` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/auth/templates/test_roles.html`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/bancos/__init__.py` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/bancos/__init__.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/cli.py` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/cli.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/compras/__init__.py` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/compras/__init__.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/config.py` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/config.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/contabilidad/__init__.py` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/contabilidad/__init__.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/contabilidad/auxiliares.py` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/contabilidad/auxiliares.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/contabilidad/ctas/__init__.py` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/contabilidad/ctas/__init__.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/contabilidad/ctas/catalogos/base.csv` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/contabilidad/ctas/catalogos/base.csv`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/contabilidad/forms.py` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/contabilidad/forms.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/contabilidad/registros/__init__.py` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/contabilidad/registros/__init__.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/contabilidad/registros/ccosto.py` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/contabilidad/registros/ccosto.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/contabilidad/registros/cuenta.py` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/contabilidad/registros/cuenta.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/contabilidad/registros/entidad.py` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/contabilidad/registros/entidad.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/contabilidad/registros/moneda.py` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/contabilidad/registros/moneda.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/contabilidad/registros/periodo.py` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/contabilidad/registros/periodo.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/contabilidad/registros/proyecto.py` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/contabilidad/registros/proyecto.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/contabilidad/registros/tasa_cambio.py` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/contabilidad/registros/tasa_cambio.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/contabilidad/registros/unidad.py` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/contabilidad/registros/unidad.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/contabilidad/templates/contabilidad/centro-costo.html` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/contabilidad/templates/contabilidad/centro-costo.html`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/contabilidad/templates/contabilidad/centro-costo_lista.html` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/contabilidad/templates/contabilidad/centro-costo_lista.html`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/contabilidad/templates/contabilidad/cuenta.html` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/contabilidad/templates/contabilidad/cuenta.html`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/contabilidad/templates/contabilidad/cuenta_lista.html` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/contabilidad/templates/contabilidad/cuenta_lista.html`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/contabilidad/templates/contabilidad/entidad.html` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/contabilidad/templates/contabilidad/entidad.html`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/contabilidad/templates/contabilidad/entidad_crear.html` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/contabilidad/templates/contabilidad/entidad_crear.html`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/contabilidad/templates/contabilidad/entidad_editar.html` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/contabilidad/templates/contabilidad/entidad_editar.html`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/contabilidad/templates/contabilidad/entidad_lista.html` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/contabilidad/templates/contabilidad/entidad_lista.html`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/contabilidad/templates/contabilidad/moneda_lista.html` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/contabilidad/templates/contabilidad/moneda_lista.html`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/contabilidad/templates/contabilidad/periodo_lista.html` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/contabilidad/templates/contabilidad/periodo_lista.html`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/contabilidad/templates/contabilidad/proyecto_lista.html` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/contabilidad/templates/contabilidad/proyecto_lista.html`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/contabilidad/templates/contabilidad/tc_lista.html` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/contabilidad/templates/contabilidad/tc_lista.html`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/contabilidad/templates/contabilidad/unidad.html` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/contabilidad/templates/contabilidad/unidad.html`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/contabilidad/templates/contabilidad/unidad_crear.html` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/contabilidad/templates/contabilidad/unidad_crear.html`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/contabilidad/templates/contabilidad/unidad_lista.html` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/contabilidad/templates/contabilidad/unidad_lista.html`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/contabilidad/templates/contabilidad.html` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/contabilidad/templates/contabilidad.html`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/database/__init__.py` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/database/__init__.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/database/helpers.py` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/database/helpers.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/datos/__init__.py` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/datos/__init__.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/datos/base/__init__.py` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/datos/base/__init__.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/datos/dev/__init__.py` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/datos/dev/__init__.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/decorators.py` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/decorators.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/exceptions/__init__.py` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/exceptions/mensajes.py` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/exceptions/mensajes.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/inventario/__init__.py` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/inventario/__init__.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/loggin.py` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/loggin.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/metadata.py` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/metadata.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/misc/ejemplos/cacao-accounting.unit` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/misc/ejemplos/cacao-accounting.unit`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/modulos.py` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/modulos.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/registro/__init__.py` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/registro/__init__.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/server.py` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/server.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/css/dashboard.css` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/css/dashboard.css`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/css/purecss-treeview.css` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/css/purecss-treeview.css`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/css/signin.css` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/css/signin.css`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/manifest.json` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/manifest.json`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/Cacao Accounting SVG.svg` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/Cacao Accounting SVG.svg`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/Cacao Accounting-01.png` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/Cacao Accounting-01.png`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/Linux/Cacao Accounting 16px.png` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/Linux/Cacao Accounting 16px.png`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/Linux/Cacao Accounting 256px.png` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/Linux/Cacao Accounting 256px.png`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/Linux/Cacao Accounting 32px.png` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/Linux/Cacao Accounting 32px.png`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/Linux/Cacao Accounting 48px.png` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/Linux/Cacao Accounting 48px.png`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/Linux/Cacao Accounting 64px.png` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/Linux/Cacao Accounting 64px.png`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/Linux/Cacao Accounting Ícono SVG.svg` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/Linux/Cacao Accounting Ícono SVG.svg`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/Web/Cacao Accounting SVG.svg` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/Web/Cacao Accounting SVG.svg`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/Web/Cacao Accounting Ícono SVG.svg` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/Web/Cacao Accounting Ícono SVG.svg`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/Web/Cacao Accounting-01.png` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/Web/Cacao Accounting-01.png`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/Web/Cacao Accounting.png` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/Web/Cacao Accounting.png`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/Windows/Cacao Accounting 16px.ico` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/Windows/Cacao Accounting 16px.ico`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/Windows/Cacao Accounting 256px.ico` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/Windows/Cacao Accounting 256px.ico`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/Windows/Cacao Accounting 32px.ico` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/Windows/Cacao Accounting 32px.ico`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/Windows/Cacao Accounting 48px.ico` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/Windows/Cacao Accounting 48px.ico`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/Windows/Cacao Accounting 64px.ico` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/Windows/Cacao Accounting 64px.ico`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/Windows/Cacao Accounting múltilple tamaño.ico` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/Windows/Cacao Accounting múltilple tamaño.ico`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/brand.svg` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/brand.svg`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/cacao_accounting _logo.png` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/cacao_accounting _logo.png`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/cacao_accounting _logo.svg` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/cacao_accounting _logo.svg`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/cacao_accounting.png` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/cacao_accounting.png`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/cacao_accounting.svg` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/cacao_accounting.svg`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/cacao_logo.svg` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/cacao_logo.svg`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/favicon/android-icon-144x144.png` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/favicon/android-icon-144x144.png`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/favicon/android-icon-192x192.png` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/favicon/android-icon-192x192.png`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/favicon/android-icon-36x36.png` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/favicon/android-icon-36x36.png`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/favicon/android-icon-48x48.png` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/favicon/android-icon-48x48.png`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/favicon/android-icon-72x72.png` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/favicon/android-icon-72x72.png`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/favicon/android-icon-96x96.png` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/favicon/android-icon-96x96.png`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/favicon/apple-icon-114x114.png` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/favicon/apple-icon-114x114.png`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/favicon/apple-icon-120x120.png` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/favicon/apple-icon-120x120.png`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/favicon/apple-icon-144x144.png` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/favicon/apple-icon-144x144.png`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/favicon/apple-icon-152x152.png` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/favicon/apple-icon-152x152.png`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/favicon/apple-icon-180x180.png` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/favicon/apple-icon-180x180.png`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/favicon/apple-icon-57x57.png` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/favicon/apple-icon-57x57.png`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/favicon/apple-icon-60x60.png` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/favicon/apple-icon-60x60.png`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/favicon/apple-icon-72x72.png` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/favicon/apple-icon-72x72.png`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/favicon/apple-icon-76x76.png` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/favicon/apple-icon-76x76.png`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/favicon/apple-icon-precomposed.png` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/favicon/apple-icon-precomposed.png`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/favicon/apple-icon.png` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/favicon/apple-icon.png`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/favicon/favicon-16x16.png` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/favicon/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/favicon/favicon-32x32.png` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/favicon/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/favicon/favicon-96x96.png` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/favicon/favicon-96x96.png`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/favicon/favicon.ico` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/favicon/favicon.ico`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/favicon/ms-icon-144x144.png` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/favicon/ms-icon-144x144.png`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/favicon/ms-icon-150x150.png` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/favicon/ms-icon-150x150.png`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/favicon/ms-icon-310x310.png` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/favicon/ms-icon-310x310.png`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/favicon/ms-icon-70x70.png` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/favicon/ms-icon-70x70.png`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/favicon-16x16.png` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/media/favicon-32x32.png` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/media/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/package-lock.json` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/package-lock.json`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/static/package.json` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/static/package.json`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/templates/400.html` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/templates/400.html`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/templates/403.html` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/templates/403.html`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/templates/404.html` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/templates/404.html`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/templates/base.html` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/templates/base.html`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/templates/macros.html` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/templates/macros.html`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/templates/setup/setup.html` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/templates/setup/setup.html`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/transaccion/__init__.py` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/transaccion/__init__.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/validaciones/__init__.py` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/validaciones/__init__.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/ventas/__init__.py` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/ventas/__init__.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/cacao_accounting/version.py` & `staging_cacao_accounting-0.0.1.dev20240507/cacao_accounting/version.py`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/pyproject.toml` & `staging_cacao_accounting-0.0.1.dev20240507/pyproject.toml`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/staging_cacao_accounting.egg-info/PKG-INFO` & `staging_cacao_accounting-0.0.1.dev20240507/staging_cacao_accounting.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: staging_cacao_accounting
-Version: 0.0.1.dev20240505
+Version: 0.0.1.dev20240507
 Summary: Accounting solution for the management of Accounts Payable, Accounts Receivable, Inventory, Treasury and General Accounting.
 Author-email: William Moreno Reyes <williamjmorenor@gmail.com>, BMO Soluciones <development@bmogroup.solutions>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -221,34 +221,29 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: Licencias_de_Terceros.md
 Requires-Dist: alembic
 Requires-Dist: bcrypt
 Requires-Dist: babel
+Requires-Dist: cryptography
 Requires-Dist: Flask
-Requires-Dist: Flask[async]
 Requires-Dist: Flask-Alembic
 Requires-Dist: flask-babel
 Requires-Dist: flask-login
 Requires-Dist: flask-sqlalchemy
 Requires-Dist: flask-wtf
 Requires-Dist: loguru
-Requires-Dist: lxml
-Requires-Dist: pdf_reports
-Requires-Dist: openpyxl
+Requires-Dist: pg8000
+Requires-Dist: PyMySQL
 Requires-Dist: sqlalchemy
 Requires-Dist: teritorio
 Requires-Dist: waitress
 Requires-Dist: wtforms
 Requires-Dist: WTForms-SQLAlchemy
-Requires-Dist: pillow
-Requires-Dist: pg8000
-Requires-Dist: PyMySQL
-Requires-Dist: cryptography
 
 ![Logo](https://raw.githubusercontent.com/cacao-accounting/cacao-accounting/development/cacao_accounting/static/media/cacao_accounting%20_logo.png)
 
 # Cacao Accounting
 
 ![PyPI - License](https://img.shields.io/pypi/l/cacao-accounting?color=green&logo=apache)
 [![Pruebas de Integración Continua](https://github.com/cacao-accounting/cacao-accounting/actions/workflows/python-package.yml/badge.svg)](https://github.com/cacao-accounting/cacao-accounting/actions/workflows/python-package.yml)
```

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/staging_cacao_accounting.egg-info/SOURCES.txt` & `staging_cacao_accounting-0.0.1.dev20240507/staging_cacao_accounting.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `staging_cacao_accounting-0.0.1.dev20240505/wsgi.py` & `staging_cacao_accounting-0.0.1.dev20240507/wsgi.py`

 * *Files identical despite different names*

