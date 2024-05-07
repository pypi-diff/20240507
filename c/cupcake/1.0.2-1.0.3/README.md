# Comparing `tmp/cupcake-1.0.2.tar.gz` & `tmp/cupcake-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cupcake-1.0.2.tar", max compression
+gzip compressed data, was "cupcake-1.0.3.tar", max compression
```

## Comparing `cupcake-1.0.2.tar` & `cupcake-1.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      761 2023-03-01 17:58:55.790012 cupcake-1.0.2/LICENSE
--rw-r--r--   0        0        0      594 2024-05-04 21:06:45.174223 cupcake-1.0.2/pyproject.toml
--rw-r--r--   0        0        0       73 2023-03-13 22:19:09.065654 cupcake-1.0.2/src/cupcake/__init__.py
--rw-r--r--   0        0        0     3965 2024-02-28 04:41:46.514999 cupcake-1.0.2/src/cupcake/cascade.py
--rw-r--r--   0        0        0    10078 2024-02-22 06:16:05.800878 cupcake-1.0.2/src/cupcake/confee.py
--rw-r--r--   0        0        0     1027 2024-01-11 04:42:54.793235 cupcake-1.0.2/src/cupcake/data/cmake_names.py
--rw-r--r--   0        0        0       58 2024-03-30 22:14:37.710534 cupcake-1.0.2/src/cupcake/data/new/.gitignore
--rw-r--r--   0        0        0     1031 2024-04-30 21:17:59.470632 cupcake-1.0.2/src/cupcake/data/new/CMakeLists.txt
--rw-r--r--   0        0        0     2477 2024-04-29 20:21:28.383431 cupcake-1.0.2/src/cupcake/data/new/conanfile.py
--rw-r--r--   0        0        0      438 2024-03-19 14:45:33.698677 cupcake-1.0.2/src/cupcake/data/new/include/{{name}}/{{name}}.hpp
--rw-r--r--   0        0        0      103 2024-03-19 14:16:34.798335 cupcake-1.0.2/src/cupcake/data/new/src/lib{{name}}.cpp
--rw-r--r--   0        0        0      227 2024-03-19 14:16:51.427197 cupcake-1.0.2/src/cupcake/data/new/src/{{name}}.cpp
--rw-r--r--   0        0        0      470 2024-02-01 17:18:45.120789 cupcake-1.0.2/src/cupcake/data/new/tests/CMakeLists.txt
--rw-r--r--   0        0        0      203 2024-03-19 13:09:50.402090 cupcake-1.0.2/src/cupcake/data/new/tests/{{name}}.cpp
--rw-r--r--   0        0        0      177 2023-03-01 15:12:58.048397 cupcake-1.0.2/src/cupcake/data/query/CMakeLists.txt
--rw-r--r--   0        0        0     1758 2024-02-06 16:16:50.206575 cupcake-1.0.2/src/cupcake/expression.py
--rw-r--r--   0        0        0      227 2024-02-04 01:50:29.311228 cupcake-1.0.2/src/cupcake/functional.py
--rw-r--r--   0        0        0    55263 2024-05-04 21:06:05.660247 cupcake-1.0.2/src/cupcake/main.py
--rw-r--r--   0        0        0     1053 2024-04-26 23:12:40.126982 cupcake-1.0.2/src/cupcake/transformations.py
--rw-r--r--   0        0        0      579 1970-01-01 00:00:00.000000 cupcake-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0      761 2023-03-01 17:58:55.790012 cupcake-1.0.3/LICENSE
+-rw-r--r--   0        0        0      594 2024-05-07 13:12:26.668058 cupcake-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0       73 2023-03-13 22:19:09.065654 cupcake-1.0.3/src/cupcake/__init__.py
+-rw-r--r--   0        0        0     3965 2024-02-28 04:41:46.514999 cupcake-1.0.3/src/cupcake/cascade.py
+-rw-r--r--   0        0        0    10186 2024-05-07 04:36:31.961880 cupcake-1.0.3/src/cupcake/confee.py
+-rw-r--r--   0        0        0     1027 2024-01-11 04:42:54.793235 cupcake-1.0.3/src/cupcake/data/cmake_names.py
+-rw-r--r--   0        0        0       58 2024-03-30 22:14:37.710534 cupcake-1.0.3/src/cupcake/data/new/.gitignore
+-rw-r--r--   0        0        0     1031 2024-04-30 21:17:59.470632 cupcake-1.0.3/src/cupcake/data/new/CMakeLists.txt
+-rw-r--r--   0        0        0     2477 2024-04-29 20:21:28.383431 cupcake-1.0.3/src/cupcake/data/new/conanfile.py
+-rw-r--r--   0        0        0      438 2024-03-19 14:45:33.698677 cupcake-1.0.3/src/cupcake/data/new/include/{{name}}/{{name}}.hpp
+-rw-r--r--   0        0        0      103 2024-03-19 14:16:34.798335 cupcake-1.0.3/src/cupcake/data/new/src/lib{{name}}.cpp
+-rw-r--r--   0        0        0      227 2024-03-19 14:16:51.427197 cupcake-1.0.3/src/cupcake/data/new/src/{{name}}.cpp
+-rw-r--r--   0        0        0      470 2024-02-01 17:18:45.120789 cupcake-1.0.3/src/cupcake/data/new/tests/CMakeLists.txt
+-rw-r--r--   0        0        0      203 2024-03-19 13:09:50.402090 cupcake-1.0.3/src/cupcake/data/new/tests/{{name}}.cpp
+-rw-r--r--   0        0        0      177 2023-03-01 15:12:58.048397 cupcake-1.0.3/src/cupcake/data/query/CMakeLists.txt
+-rw-r--r--   0        0        0     1758 2024-02-06 16:16:50.206575 cupcake-1.0.3/src/cupcake/expression.py
+-rw-r--r--   0        0        0      227 2024-02-04 01:50:29.311228 cupcake-1.0.3/src/cupcake/functional.py
+-rw-r--r--   0        0        0    56076 2024-05-07 13:09:21.595122 cupcake-1.0.3/src/cupcake/main.py
+-rw-r--r--   0        0        0     1053 2024-04-26 23:12:40.126982 cupcake-1.0.3/src/cupcake/transformations.py
+-rw-r--r--   0        0        0      579 1970-01-01 00:00:00.000000 cupcake-1.0.3/PKG-INFO
```

### Comparing `cupcake-1.0.2/LICENSE` & `cupcake-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cupcake-1.0.2/pyproject.toml` & `cupcake-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cupcake"
-version = "1.0.2"
+version = "1.0.3"
 description = "Make C++ a piece of cake."
 authors = ["John Freeman <jfreeman08@gmail.com>"]
 packages = [{include = "cupcake", from = "src"}]
 
 [tool.poetry.scripts]
 cupcake = 'cupcake.main:main'
```

### Comparing `cupcake-1.0.2/src/cupcake/cascade.py` & `cupcake-1.0.3/src/cupcake/cascade.py`

 * *Files identical despite different names*

### Comparing `cupcake-1.0.2/src/cupcake/confee.py` & `cupcake-1.0.3/src/cupcake/confee.py`

 * *Files 8% similar despite different names*

```diff
@@ -124,15 +124,15 @@
     def object(self):
         return tomlkit.table()
 
 class JsonType:
     def read(self, file):
         return json.load(file)
     def write(self, file, value):
-        json.dump(value, file)
+        json.dump(value, file, indent=2)
     def root(self):
         return {}
     def object(self):
         return {}
 
 def read(pathlike, typ=None):
     path = pathlib.Path(pathlike)
@@ -300,18 +300,19 @@
     elif stop > length:
         stop = length
 
     while sign(stop - start) == sign(step):
         yield start
         start += step
 
-def _path(self, suffix=''):
+def _path(self):
     if self.parent is None:
         return ''
-    return _path(self.parent, '.') + self.name + suffix
+    step = f'[{self.name}]' if (type(self.name) is int) else f'.{self.name}'
+    return _path(self.parent) + step
 
 def path(proxy):
     return _path(_SELVES[proxy])
 
 def set(proxy, value):
     self = _SELVES[proxy]
     if self.parent is None:
@@ -329,11 +330,11 @@
 
 def filter(proxies, pred):
     for proxy in proxies:
         if evaluate(pred, proxy()):
             yield proxy
 
 def remove_if(proxies, pred):
-    for proxy in proxies:
-        # Is no default correct here?
-        if evaluate(pred, proxy()):
-            delete(proxy)
+    # Collect everything to remove before removing anything.
+    chosen = [proxy for proxy in proxies if evaluate(pred, proxy())]
+    for proxy in chosen:
+        delete(proxy)
```

### Comparing `cupcake-1.0.2/src/cupcake/data/cmake_names.py` & `cupcake-1.0.3/src/cupcake/data/cmake_names.py`

 * *Files identical despite different names*

### Comparing `cupcake-1.0.2/src/cupcake/data/new/CMakeLists.txt` & `cupcake-1.0.3/src/cupcake/data/new/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cupcake-1.0.2/src/cupcake/data/new/conanfile.py` & `cupcake-1.0.3/src/cupcake/data/new/conanfile.py`

 * *Files identical despite different names*

### Comparing `cupcake-1.0.2/src/cupcake/expression.py` & `cupcake-1.0.3/src/cupcake/expression.py`

 * *Files identical despite different names*

### Comparing `cupcake-1.0.2/src/cupcake/main.py` & `cupcake-1.0.3/src/cupcake/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -916,15 +916,15 @@
         return cmake
 
     @cascade.command()
     @cascade.argument('executable', required=False)
     # TODO: No way to pass arguments to default executable.
     @cascade.argument('arguments', nargs=-1)
     def exe(self, CMAKE, cmake_dir_, flavor_, cmake, executable, arguments):
-        """Execute an executable target."""
+        """Execute an executable."""
         target = 'execute'
         if executable is not None:
             target += '.' + executable
         command = [CMAKE, '--build', cmake_dir_, '--target', target]
         if cmake.multiConfig():
             command.extend(['--config', FLAVORS[flavor_]])
         env = os.environ.copy()
@@ -955,15 +955,15 @@
         cmake_dir_,
         flavor_,
         jobs_,
         verbosity_,
         cmake,
         regex,
     ):
-        """Test the selected flavor."""
+        """Execute tests."""
         confee.write(config_)
         template = confee.resolve(None, config_.scripts.test, TEST_TEMPLATE_)
         template = jinja2.Template(template)
         context = {
             'ctest': CTEST,
             'cmakeDir': cmake_dir_,
             'multiConfig': cmake.multiConfig(),
@@ -1240,15 +1240,15 @@
                     line += ' -> ' + ', '.join(links)
                 print(line)
 
     @cascade.command()
     @cascade.argument('downstream', required=True)
     @cascade.argument('upstreams', required=True, nargs=-1)
     def link(self, source_dir_, downstream, upstreams):
-        """Link downstream artifact to upstream libraries."""
+        """Link a downstream target to upstream libraries."""
         metadata = confee.read(source_dir_ / 'cupcake.json')
         pname = metadata.project.name()
 
         def unprefix(reference):
             for prefix in (pname + '.', '${PROJECT_NAME}.'):
                 if reference.startswith(prefix):
                     return reference[len(prefix):]
@@ -1290,15 +1290,15 @@
 
         confee.write(metadata)
 
     @cascade.command()
     @cascade.argument('downstream', required=True)
     @cascade.argument('upstreams', required=True, nargs=-1)
     def unlink(self, source_dir_, downstream, upstreams):
-        """Unlink downstream artifact from upstream libraries."""
+        """Unlink a downstream target from upstream libraries."""
         metadata = confee.read(source_dir_ / 'cupcake.json')
         pname = metadata.project.name()
 
         def unprefix(reference):
             for prefix in (pname + '.', '${PROJECT_NAME}.'):
                 if reference.startswith(prefix):
                     return reference[len(prefix):]
@@ -1331,209 +1331,220 @@
             ))
 
         confee.write(metadata)
 
     @cascade.command('add:lib')
     @cascade.option('--public/--private', is_flag=True, default=True, help='Whether to export the library.')
     @cascade.option('--header-only', is_flag=True, help='Whether to create a source file.')
-    @cascade.argument('name', required=True)
-    def add_lib(self, source_dir_, public, header_only, name):
-        """Add a library."""
+    @cascade.argument('names', required=True, nargs=-1)
+    def add_lib(self, source_dir_, public, header_only, names):
+        """Add one or more libraries."""
         jenv = self.jenv_('data/new')
 
         tnames = ['include/{{name}}/{{name}}.hpp']
         if not header_only:
             tnames.append('src/lib{{name}}.cpp')
-        self.generate_(jenv, source_dir_, tnames, name, context={})
-
         metadata = confee.read(source_dir_ / 'cupcake.json')
-        library = {'name': name, 'links': ['${PROJECT_NAME}.imports.main'] }
-        if not public:
-            library['private'] = True
-        confee.add(metadata.libraries, library)
+
+        for name in names:
+            self.generate_(jenv, source_dir_, tnames, name, context={})
+            library = {'name': name, 'links': ['${PROJECT_NAME}.imports.main'] }
+            if not public:
+                library['private'] = True
+            confee.add(metadata.libraries, library)
+
         confee.write(metadata)
 
     @cascade.command('remove:lib')
-    @cascade.argument('name', required=True)
-    def remove_lib(self, source_dir_, name):
-        """Remove a library."""
-        # Find the library in the metadata.
+    @cascade.argument('names', required=True, nargs=-1)
+    def remove_lib(self, source_dir_, names):
+        """Remove one or more libraries."""
         metadata = confee.read(source_dir_ / 'cupcake.json')
-        libraries = confee.filter(metadata.libraries[:], subject['name'] == name)
-        libraries = list(libraries)
-        # Exit if it is missing or ambiguous.
-        if len(libraries) < 1:
-            raise SystemExit(f'unknown library name: {name}')
-        if len(libraries) > 1:
-            raise SystemExit(f'ambiguous library name: {name}')
-        [proxy] = libraries
-        library = proxy()
-        confee.delete(proxy)
-
-        # TODO: Remove its sources according to its section.
-        (source_dir_ / 'include' / f'{name}.hpp').unlink(missing_ok=True)
-        (source_dir_ / 'include' / f'{name}.h').unlink(missing_ok=True)
-        try:
-            shutil.rmtree(source_dir_ / 'include' / f'{name}')
-        except FileNotFoundError:
-            pass
-
-        (source_dir_ / 'src' / f'lib{name}.cpp').unlink(missing_ok=True)
-        (source_dir_ / 'src' / f'lib{name}.c').unlink(missing_ok=True)
-        try:
-            shutil.rmtree(source_dir_ / 'src' / f'lib{name}')
-        except FileNotFoundError:
-            pass
-
-        # Find links to the library in the metadata.
-        # It must be an internal library.
-        targets = [f'${{PROJECT_NAME}}.lib{name}']
-        if metadata.project.name:
-            targets.append(f'{metadata.project.name()}.lib{name}')
-
-        for kind in {'libraries', 'executables', 'tests'}:
-            for target in metadata[kind][:]:
-                for link in target.links[:]:
-                    # Take target from shorthand or longhand.
-                    ltarget = link()
-                    if 'target' in ltarget:
-                        ltarget = ltarget['target']
-                    # Proceed only if target matches removed library.
-                    if ltarget not in targets:
-                        continue
-                    # Remove link from metadata.
-                    confee.delete(link)
-                    # Remove includes from source files.
-                    section = 'tests' if kind == 'tests' else 'exports'
-                    section = target.section(section)
-                    root = 'tests' if section == 'tests' else 'src'
-                    root = pathlib.Path(root)
-                    for suffix in ('h', 'hpp', 'c', 'cpp'):
-                        if (file := root / f'{name}.{suffix}').is_file():
-                            print(file)
-                            transformations.remove_includes(file, name)
-                    for parent, _, files in os.walk(root / name):
-                        parent = pathlib.Path(parent)
-                        for file in files:
-                            print(parent / file)
-                            transformations.remove_includes(parent / file, name)
+
+        for name in names:
+            # Find the library in the metadata.
+            libraries = confee.filter(metadata.libraries[:], subject['name'] == name)
+            libraries = list(libraries)
+            # Exit if it is missing or ambiguous.
+            if len(libraries) < 1:
+                raise SystemExit(f'unknown library name: {name}')
+            if len(libraries) > 1:
+                raise SystemExit(f'ambiguous library name: {name}')
+            [proxy] = libraries
+            library = proxy()
+            confee.delete(proxy)
+
+            # TODO: Remove its sources according to its section.
+            (source_dir_ / 'include' / f'{name}.hpp').unlink(missing_ok=True)
+            (source_dir_ / 'include' / f'{name}.h').unlink(missing_ok=True)
+            try:
+                shutil.rmtree(source_dir_ / 'include' / f'{name}')
+            except FileNotFoundError:
+                pass
+
+            (source_dir_ / 'src' / f'lib{name}.cpp').unlink(missing_ok=True)
+            (source_dir_ / 'src' / f'lib{name}.c').unlink(missing_ok=True)
+            try:
+                shutil.rmtree(source_dir_ / 'src' / f'lib{name}')
+            except FileNotFoundError:
+                pass
+
+            # Find links to the library in the metadata.
+            # It must be an internal library.
+            targets = [f'${{PROJECT_NAME}}.lib{name}']
+            if metadata.project.name:
+                targets.append(f'{metadata.project.name()}.lib{name}')
+
+            for kind in {'libraries', 'executables', 'tests'}:
+                for target in metadata[kind][:]:
+                    for link in target.links[:]:
+                        # Take target from shorthand or longhand.
+                        ltarget = link()
+                        if 'target' in ltarget:
+                            ltarget = ltarget['target']
+                        # Proceed only if target matches removed library.
+                        if ltarget not in targets:
+                            continue
+                        # Remove link from metadata.
+                        confee.delete(link)
+                        # Remove includes from source files.
+                        section = 'tests' if kind == 'tests' else 'exports'
+                        section = target.section(section)
+                        root = 'tests' if section == 'tests' else 'src'
+                        root = pathlib.Path(root)
+                        for suffix in ('h', 'hpp', 'c', 'cpp'):
+                            if (file := root / f'{name}.{suffix}').is_file():
+                                print(file)
+                                transformations.remove_includes(file, name)
+                        for parent, _, files in os.walk(root / name):
+                            parent = pathlib.Path(parent)
+                            for file in files:
+                                print(parent / file)
+                                transformations.remove_includes(parent / file, name)
 
         confee.write(metadata)
 
     @cascade.command('add:exe')
     @cascade.option('--public/--private', is_flag=True, default=True, help='Whether to export the executable.')
-    @cascade.argument('name', required=True)
-    def add_exe(self, source_dir_, public, name):
-        """Add an executable."""
+    @cascade.argument('names', required=True, nargs=-1)
+    def add_exe(self, source_dir_, public, names):
+        """Add one or more executables."""
         jenv = self.jenv_('data/new')
-
         tnames = ['src/{{name}}.cpp']
-        self.generate_(jenv, source_dir_, tnames, name, context={})
-
         metadata = confee.read(source_dir_ / 'cupcake.json')
-        executable = { 'name': name, 'links': ['${PROJECT_NAME}.imports.main'] }
-        if not public:
-            executable['private'] = True
-        confee.add(metadata.executables, executable)
+
+        for name in names:
+            self.generate_(jenv, source_dir_, tnames, name, context={})
+            executable = { 'name': name, 'links': ['${PROJECT_NAME}.imports.main'] }
+            if not public:
+                executable['private'] = True
+            confee.add(metadata.executables, executable)
+
         confee.write(metadata)
 
     @cascade.command('remove:exe')
-    @cascade.argument('name', required=True)
-    def remove_exe(self, source_dir_, name):
-        """Remove an executable."""
-        # Find the executable in the metadata.
+    @cascade.argument('names', required=True, nargs=-1)
+    def remove_exe(self, source_dir_, names):
+        """Remove one or more executables."""
         metadata = confee.read(source_dir_ / 'cupcake.json')
-        executables = confee.filter(metadata.executables[:], subject['name'] == name)
-        executables = list(executables)
-        # Exit if it is missing or ambiguous.
-        if len(executables) < 1:
-            raise SystemExit(f'unknown executable name: {name}')
-        if len(executables) > 1:
-            raise SystemExit(f'ambiguous executable name: {name}')
-        [proxy] = executables
-        confee.delete(proxy)
-
-        (source_dir_ / 'src' / f'{name}.cpp').unlink(missing_ok=True)
-        (source_dir_ / 'src' / f'{name}.c').unlink(missing_ok=True)
-        try:
-            shutil.rmtree(source_dir_ / 'src' / f'{name}')
-        except FileNotFoundError:
-            pass
+
+        for name in names:
+            # Find the executable in the metadata.
+            executables = confee.filter(metadata.executables[:], subject['name'] == name)
+            executables = list(executables)
+            # Exit if it is missing or ambiguous.
+            if len(executables) < 1:
+                raise SystemExit(f'unknown executable name: {name}')
+            if len(executables) > 1:
+                raise SystemExit(f'ambiguous executable name: {name}')
+            [proxy] = executables
+            confee.delete(proxy)
+
+            (source_dir_ / 'src' / f'{name}.cpp').unlink(missing_ok=True)
+            (source_dir_ / 'src' / f'{name}.c').unlink(missing_ok=True)
+            try:
+                shutil.rmtree(source_dir_ / 'src' / f'{name}')
+            except FileNotFoundError:
+                pass
 
         confee.write(metadata)
 
     @cascade.command('add:test')
-    @cascade.argument('name', required=True)
-    def add_test(self, source_dir_, name):
-        """Add a test."""
+    @cascade.argument('names', required=True, nargs=-1)
+    def add_test(self, source_dir_, names):
+        """Add one or more tests."""
         jenv = self.jenv_('data/new')
-
         tnames = ['tests/{{name}}.cpp']
-        self.generate_(jenv, source_dir_, tnames, name, context={})
-
         metadata = confee.read(source_dir_ / 'cupcake.json')
-        confee.add(
-            metadata.tests,
-            {'name': name, 'links': ['${PROJECT_NAME}.imports.test'] },
-        )
+
+        for name in names:
+            self.generate_(jenv, source_dir_, tnames, name, context={})
+            confee.add(
+                metadata.tests,
+                {'name': name, 'links': ['${PROJECT_NAME}.imports.test'] },
+            )
+
         confee.write(metadata)
 
     @cascade.command('remove:test')
-    @cascade.argument('name', required=True)
-    def remove_test(self, source_dir_, name):
-        """Remove a test."""
-        # Find the test in the metadata.
+    @cascade.argument('names', required=True, nargs=-1)
+    def remove_test(self, source_dir_, names):
+        """Remove one or more tests."""
         metadata = confee.read(source_dir_ / 'cupcake.json')
-        tests = confee.filter(metadata.tests[:], subject['name'] == name)
-        tests = list(tests)
-        # Exit if it is missing or ambiguous.
-        if len(tests) < 1:
-            raise SystemExit(f'unknown test name: {name}')
-        if len(tests) > 1:
-            raise SystemExit(f'ambiguous test name: {name}')
-        [proxy] = tests
-        confee.delete(proxy)
-
-        (source_dir_ / 'tests' / f'{name}.cpp').unlink(missing_ok=True)
-        (source_dir_ / 'tests' / f'{name}.c').unlink(missing_ok=True)
-        try:
-            shutil.rmtree(source_dir_ / 'tests' / f'{name}')
-        except FileNotFoundError:
-            pass
+
+        for name in names:
+            # Find the test in the metadata.
+            tests = confee.filter(metadata.tests[:], subject['name'] == name)
+            tests = list(tests)
+            # Exit if it is missing or ambiguous.
+            if len(tests) < 1:
+                raise SystemExit(f'unknown test name: {name}')
+            if len(tests) > 1:
+                raise SystemExit(f'ambiguous test name: {name}')
+            [proxy] = tests
+            confee.delete(proxy)
+
+            (source_dir_ / 'tests' / f'{name}.cpp').unlink(missing_ok=True)
+            (source_dir_ / 'tests' / f'{name}.c').unlink(missing_ok=True)
+            try:
+                shutil.rmtree(source_dir_ / 'tests' / f'{name}')
+            except FileNotFoundError:
+                pass
 
         confee.write(metadata)
 
     @cascade.command('add:header')
-    @cascade.argument('qname', required=True)
-    def add_header(self, source_dir_, qname):
+    @cascade.argument('qnames', required=True, nargs=-1)
+    def add_header(self, source_dir_, qnames):
         """
-        Add a new header to an existing library.
+        Add one or more public headers to an existing library.
 
-        The argument should be a qualified name,
+        The arguments should be qualified names,
         e.g. "foo.bar.baz" for include/foo/bar/baz.hpp.
         """
-        namespaces = qname.split('.')
-        for name in namespaces:
-            assert_legal_name(name)
-        path = source_dir_.joinpath('include', *namespaces).with_suffix('.hpp')
-        if path.exists():
-            raise SystemExit(f'file already exists: {path}')
-        name = namespaces.pop()
-
         metadata = confee.read(source_dir_ / 'cupcake.json')
-        if not any(l.name() == namespaces[0] for l in metadata.libraries[:]):
-            raise SystemExit(f'missing library: {namespaces[0]}')
+        for qname in qnames:
+            namespaces = qname.split('.')
+            for name in namespaces:
+                assert_legal_name(name)
+            path = source_dir_.joinpath('include', *namespaces).with_suffix('.hpp')
+            if path.exists():
+                raise SystemExit(f'file already exists: {path}')
+            name = namespaces.pop()
 
-        path.parent.mkdir(parents=True, exist_ok=True)
-        jenv = self.jenv_('data/new')
-        template = jenv.get_template('include/{{name}}/{{name}}.hpp')
-        path.write_text(template.render({
-            'namespaces': namespaces,
-            'name': name,
-        }))
+            if not any(l.name() == namespaces[0] for l in metadata.libraries[:]):
+                raise SystemExit(f'missing library: {namespaces[0]}')
+
+            path.parent.mkdir(parents=True, exist_ok=True)
+            jenv = self.jenv_('data/new')
+            template = jenv.get_template('include/{{name}}/{{name}}.hpp')
+            path.write_text(template.render({
+                'namespaces': namespaces,
+                'name': name,
+            }))
 
     @cascade.command()
     @cascade.argument('url', default='.')
     def export(self, CONAN, url):
         """
         Copy a Conan package to your local cache.
```

### Comparing `cupcake-1.0.2/src/cupcake/transformations.py` & `cupcake-1.0.3/src/cupcake/transformations.py`

 * *Files identical despite different names*

### Comparing `cupcake-1.0.2/PKG-INFO` & `cupcake-1.0.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cupcake
-Version: 1.0.2
+Version: 1.0.3
 Summary: Make C++ a piece of cake.
 Author: John Freeman
 Author-email: jfreeman08@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

