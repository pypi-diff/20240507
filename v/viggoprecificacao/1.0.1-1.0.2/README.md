# Comparing `tmp/viggoprecificacao-1.0.1.tar.gz` & `tmp/viggoprecificacao-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viggoprecificacao-1.0.1.tar", last modified: Mon May  6 20:12:00 2024, max compression
+gzip compressed data, was "viggoprecificacao-1.0.2.tar", last modified: Tue May  7 12:06:47 2024, max compression
```

## Comparing `viggoprecificacao-1.0.1.tar` & `viggoprecificacao-1.0.2.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:12:00.551429 viggoprecificacao-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 20:11:14.000000 viggoprecificacao-1.0.1/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-06 20:11:14.000000 viggoprecificacao-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-06 20:12:00.551429 viggoprecificacao-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-06 20:11:14.000000 viggoprecificacao-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-06 20:11:14.000000 viggoprecificacao-1.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-06 20:12:00.551429 viggoprecificacao-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-06 20:11:14.000000 viggoprecificacao-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:12:00.547429 viggoprecificacao-1.0.1/viggoprecificacao/
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-05-06 20:11:14.000000 viggoprecificacao-1.0.1/viggoprecificacao/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-06 20:11:14.000000 viggoprecificacao-1.0.1/viggoprecificacao/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-06 20:11:14.000000 viggoprecificacao-1.0.1/viggoprecificacao/packages.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-06 20:11:14.000000 viggoprecificacao-1.0.1/viggoprecificacao/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:12:00.547429 viggoprecificacao-1.0.1/viggoprecificacao/subsystem/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 20:11:14.000000 viggoprecificacao-1.0.1/viggoprecificacao/subsystem/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:12:00.551429 viggoprecificacao-1.0.1/viggoprecificacao/subsystem/parametrizacao/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 20:11:14.000000 viggoprecificacao-1.0.1/viggoprecificacao/subsystem/parametrizacao/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:12:00.551429 viggoprecificacao-1.0.1/viggoprecificacao/subsystem/parametrizacao/contrato_viggo/
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-06 20:11:14.000000 viggoprecificacao-1.0.1/viggoprecificacao/subsystem/parametrizacao/contrato_viggo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-06 20:11:14.000000 viggoprecificacao-1.0.1/viggoprecificacao/subsystem/parametrizacao/contrato_viggo/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-06 20:11:14.000000 viggoprecificacao-1.0.1/viggoprecificacao/subsystem/parametrizacao/contrato_viggo/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    10214 2024-05-06 20:11:14.000000 viggoprecificacao-1.0.1/viggoprecificacao/subsystem/parametrizacao/contrato_viggo/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-06 20:11:14.000000 viggoprecificacao-1.0.1/viggoprecificacao/subsystem/parametrizacao/contrato_viggo/router.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:12:00.551429 viggoprecificacao-1.0.1/viggoprecificacao/subsystem/parametrizacao/plano_viggo/
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-06 20:11:14.000000 viggoprecificacao-1.0.1/viggoprecificacao/subsystem/parametrizacao/plano_viggo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-06 20:11:14.000000 viggoprecificacao-1.0.1/viggoprecificacao/subsystem/parametrizacao/plano_viggo/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-06 20:11:14.000000 viggoprecificacao-1.0.1/viggoprecificacao/subsystem/parametrizacao/plano_viggo/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     8860 2024-05-06 20:11:14.000000 viggoprecificacao-1.0.1/viggoprecificacao/subsystem/parametrizacao/plano_viggo/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-06 20:11:14.000000 viggoprecificacao-1.0.1/viggoprecificacao/subsystem/parametrizacao/plano_viggo/router.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:12:00.551429 viggoprecificacao-1.0.1/viggoprecificacao/subsystem/parametrizacao/produto_viggo/
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-06 20:11:14.000000 viggoprecificacao-1.0.1/viggoprecificacao/subsystem/parametrizacao/produto_viggo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-05-06 20:11:14.000000 viggoprecificacao-1.0.1/viggoprecificacao/subsystem/parametrizacao/produto_viggo/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:12:00.551429 viggoprecificacao-1.0.1/viggoprecificacao/subsystem/parametrizacao/servico_viggo/
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-06 20:11:14.000000 viggoprecificacao-1.0.1/viggoprecificacao/subsystem/parametrizacao/servico_viggo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-05-06 20:11:14.000000 viggoprecificacao-1.0.1/viggoprecificacao/subsystem/parametrizacao/servico_viggo/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:12:00.551429 viggoprecificacao-1.0.1/viggoprecificacao/subsystem/parametrizacao/termo_aceite_viggo/
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-06 20:11:14.000000 viggoprecificacao-1.0.1/viggoprecificacao/subsystem/parametrizacao/termo_aceite_viggo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-05-06 20:11:14.000000 viggoprecificacao-1.0.1/viggoprecificacao/subsystem/parametrizacao/termo_aceite_viggo/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-05-06 20:11:14.000000 viggoprecificacao-1.0.1/viggoprecificacao/subsystem/parametrizacao/termo_aceite_viggo/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-05-06 20:11:14.000000 viggoprecificacao-1.0.1/viggoprecificacao/subsystem/parametrizacao/termo_aceite_viggo/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:12:00.547429 viggoprecificacao-1.0.1/viggoprecificacao.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-06 20:12:00.000000 viggoprecificacao-1.0.1/viggoprecificacao.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-05-06 20:12:00.000000 viggoprecificacao-1.0.1/viggoprecificacao.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 20:12:00.000000 viggoprecificacao-1.0.1/viggoprecificacao.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-06 20:12:00.000000 viggoprecificacao-1.0.1/viggoprecificacao.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-06 20:12:00.000000 viggoprecificacao-1.0.1/viggoprecificacao.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:06:47.701130 viggoprecificacao-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 12:06:02.000000 viggoprecificacao-1.0.2/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-07 12:06:02.000000 viggoprecificacao-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-07 12:06:47.701130 viggoprecificacao-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-07 12:06:02.000000 viggoprecificacao-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-07 12:06:02.000000 viggoprecificacao-1.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-07 12:06:47.701130 viggoprecificacao-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-07 12:06:02.000000 viggoprecificacao-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:06:47.697130 viggoprecificacao-1.0.2/viggoprecificacao/
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-05-07 12:06:02.000000 viggoprecificacao-1.0.2/viggoprecificacao/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-07 12:06:02.000000 viggoprecificacao-1.0.2/viggoprecificacao/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-07 12:06:02.000000 viggoprecificacao-1.0.2/viggoprecificacao/packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-07 12:06:02.000000 viggoprecificacao-1.0.2/viggoprecificacao/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:06:47.701130 viggoprecificacao-1.0.2/viggoprecificacao/subsystem/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 12:06:02.000000 viggoprecificacao-1.0.2/viggoprecificacao/subsystem/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:06:47.701130 viggoprecificacao-1.0.2/viggoprecificacao/subsystem/parametrizacao/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 12:06:02.000000 viggoprecificacao-1.0.2/viggoprecificacao/subsystem/parametrizacao/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:06:47.701130 viggoprecificacao-1.0.2/viggoprecificacao/subsystem/parametrizacao/contrato_viggo/
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-07 12:06:02.000000 viggoprecificacao-1.0.2/viggoprecificacao/subsystem/parametrizacao/contrato_viggo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-07 12:06:02.000000 viggoprecificacao-1.0.2/viggoprecificacao/subsystem/parametrizacao/contrato_viggo/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-07 12:06:02.000000 viggoprecificacao-1.0.2/viggoprecificacao/subsystem/parametrizacao/contrato_viggo/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10646 2024-05-07 12:06:02.000000 viggoprecificacao-1.0.2/viggoprecificacao/subsystem/parametrizacao/contrato_viggo/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-07 12:06:02.000000 viggoprecificacao-1.0.2/viggoprecificacao/subsystem/parametrizacao/contrato_viggo/router.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:06:47.701130 viggoprecificacao-1.0.2/viggoprecificacao/subsystem/parametrizacao/plano_viggo/
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-07 12:06:02.000000 viggoprecificacao-1.0.2/viggoprecificacao/subsystem/parametrizacao/plano_viggo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-07 12:06:02.000000 viggoprecificacao-1.0.2/viggoprecificacao/subsystem/parametrizacao/plano_viggo/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-07 12:06:02.000000 viggoprecificacao-1.0.2/viggoprecificacao/subsystem/parametrizacao/plano_viggo/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9268 2024-05-07 12:06:02.000000 viggoprecificacao-1.0.2/viggoprecificacao/subsystem/parametrizacao/plano_viggo/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-07 12:06:02.000000 viggoprecificacao-1.0.2/viggoprecificacao/subsystem/parametrizacao/plano_viggo/router.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:06:47.701130 viggoprecificacao-1.0.2/viggoprecificacao/subsystem/parametrizacao/produto_viggo/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-07 12:06:02.000000 viggoprecificacao-1.0.2/viggoprecificacao/subsystem/parametrizacao/produto_viggo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-05-07 12:06:02.000000 viggoprecificacao-1.0.2/viggoprecificacao/subsystem/parametrizacao/produto_viggo/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:06:47.701130 viggoprecificacao-1.0.2/viggoprecificacao/subsystem/parametrizacao/servico_viggo/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-07 12:06:02.000000 viggoprecificacao-1.0.2/viggoprecificacao/subsystem/parametrizacao/servico_viggo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-05-07 12:06:02.000000 viggoprecificacao-1.0.2/viggoprecificacao/subsystem/parametrizacao/servico_viggo/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:06:47.701130 viggoprecificacao-1.0.2/viggoprecificacao/subsystem/parametrizacao/termo_aceite_viggo/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-07 12:06:02.000000 viggoprecificacao-1.0.2/viggoprecificacao/subsystem/parametrizacao/termo_aceite_viggo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-05-07 12:06:02.000000 viggoprecificacao-1.0.2/viggoprecificacao/subsystem/parametrizacao/termo_aceite_viggo/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-05-07 12:06:02.000000 viggoprecificacao-1.0.2/viggoprecificacao/subsystem/parametrizacao/termo_aceite_viggo/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-05-07 12:06:02.000000 viggoprecificacao-1.0.2/viggoprecificacao/subsystem/parametrizacao/termo_aceite_viggo/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 12:06:47.697130 viggoprecificacao-1.0.2/viggoprecificacao.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-07 12:06:47.000000 viggoprecificacao-1.0.2/viggoprecificacao.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-05-07 12:06:47.000000 viggoprecificacao-1.0.2/viggoprecificacao.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 12:06:47.000000 viggoprecificacao-1.0.2/viggoprecificacao.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-07 12:06:47.000000 viggoprecificacao-1.0.2/viggoprecificacao.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-07 12:06:47.000000 viggoprecificacao-1.0.2/viggoprecificacao.egg-info/top_level.txt
```

### Comparing `viggoprecificacao-1.0.1/viggoprecificacao/__init__.py` & `viggoprecificacao-1.0.2/viggoprecificacao/__init__.py`

 * *Files identical despite different names*

### Comparing `viggoprecificacao-1.0.1/viggoprecificacao/subsystem/parametrizacao/contrato_viggo/controller.py` & `viggoprecificacao-1.0.2/viggoprecificacao/subsystem/parametrizacao/contrato_viggo/controller.py`

 * *Files identical despite different names*

### Comparing `viggoprecificacao-1.0.1/viggoprecificacao/subsystem/parametrizacao/contrato_viggo/manager.py` & `viggoprecificacao-1.0.2/viggoprecificacao/subsystem/parametrizacao/contrato_viggo/manager.py`

 * *Files identical despite different names*

### Comparing `viggoprecificacao-1.0.1/viggoprecificacao/subsystem/parametrizacao/contrato_viggo/resource.py` & `viggoprecificacao-1.0.2/viggoprecificacao/subsystem/parametrizacao/contrato_viggo/resource.py`

 * *Files 8% similar despite different names*

```diff
@@ -115,14 +115,16 @@
 
 class ContratoPapel(entity.Entity, db.Model):
 
     attributes = ['contrato_viggo_id', 'role_id', 'qtd', 'valor']
     attributes += entity.Entity.attributes
 
     # ligações diretas
+    contrato_viggo_id = db.Column(
+        db.CHAR(32), db.ForeignKey("contrato_viggo.id"), nullable=False)
     role_id = db.Column(
         db.CHAR(32), db.ForeignKey("role.id"), nullable=False)
     role = orm.relationship('Role', backref=orm.backref(
         'contrato_papel_role'))
 
     # atributos
     qtd = db.Column(db.Numeric(4), nullable=True)
@@ -151,14 +153,16 @@
 
     attributes = ['contrato_viggo_id', 'servico_id', 'v_aquisicao',
                   'v_recorrencia', 'v_adicional', 'dias_carencia',
                   'dias_vigencia']
     attributes += entity.Entity.attributes
 
     # ligações diretas
+    contrato_viggo_id = db.Column(
+        db.CHAR(32), db.ForeignKey("contrato_viggo.id"), nullable=False)
     servico_id = db.Column(
         db.CHAR(32), db.ForeignKey("servico_viggo.id"), nullable=False)
     servico = orm.relationship('ServicoViggo', backref=orm.backref(
         'contrato_servico_servico_viggo'))
 
     # atributos
     v_aquisicao = db.Column(db.Numeric(17, 4), nullable=True)
@@ -194,14 +198,16 @@
 class ContratoProduto(entity.Entity, db.Model):
 
     attributes = ['contrato_viggo_id', 'produto_id', 'valor', 'qtd',
                   'qtd_dias_p_entrega', 'tem_garantia']
     attributes += entity.Entity.attributes
 
     # ligações diretas
+    contrato_viggo_id = db.Column(
+        db.CHAR(32), db.ForeignKey("contrato_viggo.id"), nullable=False)
     produto_id = db.Column(
         db.CHAR(32), db.ForeignKey("produto_viggo.id"), nullable=False)
     produto = orm.relationship('ProdutoViggo', backref=orm.backref(
         'contrato_produto_produto_viggo'))
 
     # atributos
     valor = db.Column(db.Numeric(17, 4), nullable=True)
@@ -236,14 +242,16 @@
 
 class ContratoTermoAceite(entity.Entity, db.Model):
 
     attributes = ['contrato_viggo_id', 'termo_aceite_id']
     attributes += entity.Entity.attributes
 
     # ligações diretas
+    contrato_viggo_id = db.Column(
+        db.CHAR(32), db.ForeignKey("contrato_viggo.id"), nullable=False)
     termo_aceite_id = db.Column(
         db.CHAR(32), db.ForeignKey("termo_aceite_viggo.id"), nullable=False)
     termo_aceite = orm.relationship('TermoAceiteViggo', backref=orm.backref(
         'contrato_termo_aceite_termo_aceite'))
 
     def __init__(self, id, contrato_viggo_id, termo_aceite_id,
                  active=True, created_at=None, created_by=None,
```

### Comparing `viggoprecificacao-1.0.1/viggoprecificacao/subsystem/parametrizacao/plano_viggo/controller.py` & `viggoprecificacao-1.0.2/viggoprecificacao/subsystem/parametrizacao/plano_viggo/controller.py`

 * *Files identical despite different names*

### Comparing `viggoprecificacao-1.0.1/viggoprecificacao/subsystem/parametrizacao/plano_viggo/manager.py` & `viggoprecificacao-1.0.2/viggoprecificacao/subsystem/parametrizacao/plano_viggo/manager.py`

 * *Files identical despite different names*

### Comparing `viggoprecificacao-1.0.1/viggoprecificacao/subsystem/parametrizacao/plano_viggo/resource.py` & `viggoprecificacao-1.0.2/viggoprecificacao/subsystem/parametrizacao/plano_viggo/resource.py`

 * *Files 7% similar despite different names*

```diff
@@ -98,14 +98,16 @@
 
 class PlanoPapel(entity.Entity, db.Model):
 
     attributes = ['plano_viggo_id', 'role_id', 'qtd', 'valor']
     attributes += entity.Entity.attributes
 
     # ligações diretas
+    plano_viggo_id = db.Column(
+        db.CHAR(32), db.ForeignKey("plano_viggo.id"), nullable=False)
     role_id = db.Column(
         db.CHAR(32), db.ForeignKey("role.id"), nullable=False)
     role = orm.relationship('Role', backref=orm.backref(
         'plano_papel_role'))
 
     # atributos
     qtd = db.Column(db.Numeric(4), nullable=True)
@@ -134,14 +136,16 @@
 
     attributes = ['plano_viggo_id', 'servico_id', 'v_aquisicao',
                   'v_recorrencia', 'v_adicional', 'dias_carencia',
                   'dias_vigencia']
     attributes += entity.Entity.attributes
 
     # ligações diretas
+    plano_viggo_id = db.Column(
+        db.CHAR(32), db.ForeignKey("plano_viggo.id"), nullable=False)
     servico_id = db.Column(
         db.CHAR(32), db.ForeignKey("servico_viggo.id"), nullable=False)
     servico = orm.relationship('ServicoViggo', backref=orm.backref(
         'plano_servico_servico_viggo'))
 
     # atributos
     v_aquisicao = db.Column(db.Numeric(17, 4), nullable=True)
@@ -177,14 +181,16 @@
 class PlanoProduto(entity.Entity, db.Model):
 
     attributes = ['plano_viggo_id', 'produto_id', 'valor', 'qtd',
                   'qtd_dias_p_entrega', 'tem_garantia']
     attributes += entity.Entity.attributes
 
     # ligações diretas
+    plano_viggo_id = db.Column(
+        db.CHAR(32), db.ForeignKey("plano_viggo.id"), nullable=False)
     produto_id = db.Column(
         db.CHAR(32), db.ForeignKey("produto_viggo.id"), nullable=False)
     produto = orm.relationship('ProdutoViggo', backref=orm.backref(
         'plano_produto_produto_viggo'))
 
     # atributos
     valor = db.Column(db.Numeric(17, 4), nullable=True)
@@ -216,14 +222,16 @@
 
 class PlanoTermoAceite(entity.Entity, db.Model):
 
     attributes = ['plano_viggo_id', 'termo_aceite_id']
     attributes += entity.Entity.attributes
 
     # ligações diretas
+    plano_viggo_id = db.Column(
+        db.CHAR(32), db.ForeignKey("plano_viggo.id"), nullable=False)
     termo_aceite_id = db.Column(
         db.CHAR(32), db.ForeignKey("termo_aceite_viggo.id"), nullable=False)
     termo_aceite = orm.relationship('TermoAceiteViggo', backref=orm.backref(
         'plano_termo_aceite_termo_aceite'))
 
     def __init__(self, id, plano_viggo_id, termo_aceite_id,
                  active=True, created_at=None, created_by=None,
```

### Comparing `viggoprecificacao-1.0.1/viggoprecificacao/subsystem/parametrizacao/produto_viggo/resource.py` & `viggoprecificacao-1.0.2/viggoprecificacao/subsystem/parametrizacao/produto_viggo/resource.py`

 * *Files identical despite different names*

### Comparing `viggoprecificacao-1.0.1/viggoprecificacao/subsystem/parametrizacao/servico_viggo/resource.py` & `viggoprecificacao-1.0.2/viggoprecificacao/subsystem/parametrizacao/servico_viggo/resource.py`

 * *Files identical despite different names*

### Comparing `viggoprecificacao-1.0.1/viggoprecificacao/subsystem/parametrizacao/termo_aceite_viggo/controller.py` & `viggoprecificacao-1.0.2/viggoprecificacao/subsystem/parametrizacao/termo_aceite_viggo/controller.py`

 * *Files identical despite different names*

### Comparing `viggoprecificacao-1.0.1/viggoprecificacao/subsystem/parametrizacao/termo_aceite_viggo/manager.py` & `viggoprecificacao-1.0.2/viggoprecificacao/subsystem/parametrizacao/termo_aceite_viggo/manager.py`

 * *Files identical despite different names*

### Comparing `viggoprecificacao-1.0.1/viggoprecificacao/subsystem/parametrizacao/termo_aceite_viggo/resource.py` & `viggoprecificacao-1.0.2/viggoprecificacao/subsystem/parametrizacao/termo_aceite_viggo/resource.py`

 * *Files identical despite different names*

### Comparing `viggoprecificacao-1.0.1/viggoprecificacao.egg-info/SOURCES.txt` & `viggoprecificacao-1.0.2/viggoprecificacao.egg-info/SOURCES.txt`

 * *Files identical despite different names*

