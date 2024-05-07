# Comparing `tmp/pauli_tracker-0.1.0.tar.gz` & `tmp/pauli_tracker-0.1.1.tar.gz`

## Comparing `pauli_tracker-0.1.0.tar` & `pauli_tracker-0.1.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0     1001      127      739 2024-02-11 22:56:59.000000 pauli_tracker-0.1.0/rust/Cargo.toml
--rw-r--r--   0     1001      127     2502 2024-02-11 22:56:59.000000 pauli_tracker-0.1.0/rust/src/frames/map.rs
--rw-r--r--   0     1001      127     2304 2024-02-11 22:56:59.000000 pauli_tracker-0.1.0/rust/src/frames/vec.rs
--rw-r--r--   0     1001      127     9147 2024-02-11 22:56:59.000000 pauli_tracker-0.1.0/rust/src/frames.rs
--rw-r--r--   0     1001      127      591 2024-02-11 22:56:59.000000 pauli_tracker-0.1.0/rust/src/impl_helper/doc.rs
--rw-r--r--   0     1001      127     1116 2024-02-11 22:56:59.000000 pauli_tracker-0.1.0/rust/src/impl_helper/links.rs
--rw-r--r--   0     1001      127     5964 2024-02-11 22:56:59.000000 pauli_tracker-0.1.0/rust/src/impl_helper/serialization.rs
--rw-r--r--   0     1001      127     1653 2024-02-11 22:56:59.000000 pauli_tracker-0.1.0/rust/src/impl_helper/tracker.rs
--rw-r--r--   0     1001      127       68 2024-02-11 22:56:59.000000 pauli_tracker-0.1.0/rust/src/impl_helper.rs
--rw-r--r--   0     1001      127     1266 2024-02-11 22:56:59.000000 pauli_tracker-0.1.0/rust/src/lib.rs
--rw-r--r--   0     1001      127     2191 2024-02-11 22:56:59.000000 pauli_tracker-0.1.0/rust/src/live/map.rs
--rw-r--r--   0     1001      127     1965 2024-02-11 22:56:59.000000 pauli_tracker-0.1.0/rust/src/live/vec.rs
--rw-r--r--   0     1001      127     2429 2024-02-11 22:56:59.000000 pauli_tracker-0.1.0/rust/src/live.rs
--rw-r--r--   0     1001      127     4192 2024-02-11 22:56:59.000000 pauli_tracker-0.1.0/rust/src/pauli.rs
--rw-r--r--   0        0        0      634 1970-01-01 00:00:00.000000 pauli_tracker-0.1.0/rust/_lib/Cargo.toml
--rw-r--r--   0     1001      127      175 2024-02-11 22:56:59.000000 pauli_tracker-0.1.0/rust/_lib/src/lib.rs
--rw-r--r--   0     1001      127     2818 2024-02-11 22:56:59.000000 pauli_tracker-0.1.0/README.md
--rw-r--r--   0     1001      127    14312 2024-02-11 22:57:09.000000 pauli_tracker-0.1.0/rust/_lib/Cargo.lock
--rw-r--r--   0     1001      127      703 2024-02-11 22:56:59.000000 pauli_tracker-0.1.0/pyproject.toml
--rw-r--r--   0     1001      127      234 2024-02-11 22:56:59.000000 pauli_tracker-0.1.0/python/pauli_tracker/live/map.py
--rw-r--r--   0     1001      127      252 2024-02-11 22:56:59.000000 pauli_tracker-0.1.0/python/pauli_tracker/live/vec.py
--rw-r--r--   0     1001      127      234 2024-02-11 22:56:59.000000 pauli_tracker-0.1.0/python/pauli_tracker/live/__init__.py
--rw-r--r--   0     1001      127      244 2024-02-11 22:56:59.000000 pauli_tracker-0.1.0/python/pauli_tracker/frames/map.py
--rw-r--r--   0     1001      127      262 2024-02-11 22:56:59.000000 pauli_tracker-0.1.0/python/pauli_tracker/frames/vec.py
--rw-r--r--   0     1001      127      287 2024-02-11 22:56:59.000000 pauli_tracker-0.1.0/python/pauli_tracker/frames/__init__.py
--rw-r--r--   0     1001      127      453 2024-02-11 22:56:59.000000 pauli_tracker-0.1.0/python/pauli_tracker/pauli.py
--rw-r--r--   0     1001      127     1615 2024-02-11 22:56:59.000000 pauli_tracker-0.1.0/python/pauli_tracker/__init__.py
--rw-r--r--   0     1001      127    11357 2024-02-11 22:56:59.000000 pauli_tracker-0.1.0/LICENSE-APACHE
--rw-r--r--   0     1001      127     1067 2024-02-11 22:56:59.000000 pauli_tracker-0.1.0/LICENSE-MIT
--rw-r--r--   0        0        0     3419 1970-01-01 00:00:00.000000 pauli_tracker-0.1.0/PKG-INFO
+-rw-r--r--   0     1001      127      739 2024-05-07 00:56:10.000000 pauli_tracker-0.1.1/rust/Cargo.toml
+-rw-r--r--   0     1001      127     2502 2024-05-07 00:56:10.000000 pauli_tracker-0.1.1/rust/src/frames/map.rs
+-rw-r--r--   0     1001      127     2304 2024-05-07 00:56:10.000000 pauli_tracker-0.1.1/rust/src/frames/vec.rs
+-rw-r--r--   0     1001      127     9147 2024-05-07 00:56:10.000000 pauli_tracker-0.1.1/rust/src/frames.rs
+-rw-r--r--   0     1001      127      591 2024-05-07 00:56:10.000000 pauli_tracker-0.1.1/rust/src/impl_helper/doc.rs
+-rw-r--r--   0     1001      127     1116 2024-05-07 00:56:10.000000 pauli_tracker-0.1.1/rust/src/impl_helper/links.rs
+-rw-r--r--   0     1001      127     6778 2024-05-07 00:56:10.000000 pauli_tracker-0.1.1/rust/src/impl_helper/serialization.rs
+-rw-r--r--   0     1001      127     1750 2024-05-07 00:56:10.000000 pauli_tracker-0.1.1/rust/src/impl_helper/tracker.rs
+-rw-r--r--   0     1001      127       68 2024-05-07 00:56:10.000000 pauli_tracker-0.1.1/rust/src/impl_helper.rs
+-rw-r--r--   0     1001      127     1266 2024-05-07 00:56:10.000000 pauli_tracker-0.1.1/rust/src/lib.rs
+-rw-r--r--   0     1001      127     2191 2024-05-07 00:56:10.000000 pauli_tracker-0.1.1/rust/src/live/map.rs
+-rw-r--r--   0     1001      127     1965 2024-05-07 00:56:10.000000 pauli_tracker-0.1.1/rust/src/live/vec.rs
+-rw-r--r--   0     1001      127     2429 2024-05-07 00:56:10.000000 pauli_tracker-0.1.1/rust/src/live.rs
+-rw-r--r--   0     1001      127     5641 2024-05-07 00:56:10.000000 pauli_tracker-0.1.1/rust/src/pauli.rs
+-rw-r--r--   0        0        0      634 1970-01-01 00:00:00.000000 pauli_tracker-0.1.1/rust/_lib/Cargo.toml
+-rw-r--r--   0     1001      127      175 2024-05-07 00:56:10.000000 pauli_tracker-0.1.1/rust/_lib/src/lib.rs
+-rw-r--r--   0     1001      127     2818 2024-05-07 00:56:10.000000 pauli_tracker-0.1.1/README.md
+-rw-r--r--   0     1001      127    14785 2024-05-07 00:56:27.000000 pauli_tracker-0.1.1/rust/_lib/Cargo.lock
+-rw-r--r--   0     1001      127      760 2024-05-07 00:56:10.000000 pauli_tracker-0.1.1/pyproject.toml
+-rw-r--r--   0     1001      127     1615 2024-05-07 00:56:10.000000 pauli_tracker-0.1.1/python/pauli_tracker/__init__.py
+-rw-r--r--   0     1001      127      453 2024-05-07 00:56:10.000000 pauli_tracker-0.1.1/python/pauli_tracker/pauli.py
+-rw-r--r--   0     1001      127      244 2024-05-07 00:56:10.000000 pauli_tracker-0.1.1/python/pauli_tracker/frames/map.py
+-rw-r--r--   0     1001      127      262 2024-05-07 00:56:10.000000 pauli_tracker-0.1.1/python/pauli_tracker/frames/vec.py
+-rw-r--r--   0     1001      127      287 2024-05-07 00:56:10.000000 pauli_tracker-0.1.1/python/pauli_tracker/frames/__init__.py
+-rw-r--r--   0     1001      127      234 2024-05-07 00:56:10.000000 pauli_tracker-0.1.1/python/pauli_tracker/live/map.py
+-rw-r--r--   0     1001      127      252 2024-05-07 00:56:10.000000 pauli_tracker-0.1.1/python/pauli_tracker/live/vec.py
+-rw-r--r--   0     1001      127      234 2024-05-07 00:56:10.000000 pauli_tracker-0.1.1/python/pauli_tracker/live/__init__.py
+-rw-r--r--   0     1001      127    11357 2024-05-07 00:56:10.000000 pauli_tracker-0.1.1/LICENSE-APACHE
+-rw-r--r--   0     1001      127     1067 2024-05-07 00:56:10.000000 pauli_tracker-0.1.1/LICENSE-MIT
+-rw-r--r--   0        0        0     3486 1970-01-01 00:00:00.000000 pauli_tracker-0.1.1/PKG-INFO
```

### Comparing `pauli_tracker-0.1.0/rust/Cargo.toml` & `pauli_tracker-0.1.1/rust/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 license = "MIT OR Apache-2.0"
 
 [lib]
 name = "pauli_tracker_pyo3"
 crate-type = ["lib"]
 
 [dependencies]
-lib = { package = "pauli_tracker", version = "0.4.0", features = ["serde", "bitvec"] }
+lib = { package = "pauli_tracker", version = "0.4.1", features = ["serde", "bitvec"] }
 # lib = { package = "pauli_tracker", version = "0.4.1-alpha.1", features = [
 #   "serde",
 #   "bitvec",
 # ], git = "https://github.com/taeruh/pauli_tracker" }
 pyo3 = { version = "0.20.2", default-features = false, features = [
   "macros",
   "multiple-pymethods",
```

### Comparing `pauli_tracker-0.1.0/rust/src/frames/map.rs` & `pauli_tracker-0.1.1/rust/src/frames/map.rs`

 * *Files identical despite different names*

### Comparing `pauli_tracker-0.1.0/rust/src/frames/vec.rs` & `pauli_tracker-0.1.1/rust/src/frames/vec.rs`

 * *Files identical despite different names*

### Comparing `pauli_tracker-0.1.0/rust/src/frames.rs` & `pauli_tracker-0.1.1/rust/src/frames.rs`

 * *Files identical despite different names*

### Comparing `pauli_tracker-0.1.0/rust/src/impl_helper/doc.rs` & `pauli_tracker-0.1.1/rust/src/impl_helper/doc.rs`

 * *Files identical despite different names*

### Comparing `pauli_tracker-0.1.0/rust/src/impl_helper/links.rs` & `pauli_tracker-0.1.1/rust/src/impl_helper/links.rs`

 * *Files identical despite different names*

### Comparing `pauli_tracker-0.1.0/rust/src/impl_helper/serialization.rs` & `pauli_tracker-0.1.1/rust/src/impl_helper/serialization.rs`

 * *Files 25% similar despite different names*

```diff
@@ -33,16 +33,42 @@
 }
 
 pub fn deserialize_error<T: fmt::Display>(error: T) -> pyo3::PyErr {
     pyo3::exceptions::PyValueError::new_err(format!("failed to deserialize: {error}"))
 }
 
 #[macro_export]
+macro_rules! inner_type {
+    (newtype, $self:expr) => {
+        $self.0
+    };
+    (plain, $self:expr) => {
+        $self
+    };
+}
+#[macro_export]
+macro_rules! map_type {
+    (newtype, $to_wrap:expr) => {
+        Result::map($to_wrap, Self)
+    };
+    (plain, $to_wrap:expr) => {
+        $to_wrap
+    };
+}
+
+// most of the times, we are dealing with a newtype, but sometimes it is a plain type
+// (don't remove this functionality here (if it is not needed here), because
+// mbqc_scheduling relies on it (at the moment))
+
+#[macro_export]
 macro_rules! serde {
     ($type:ty) => {
+        $crate::serde!($type, newtype);
+    };
+    ($type:ty, $opaque:tt) => {
         #[pyo3::pymethods]
         impl $type {
             /// Serialize the internal data structure into a file.
             ///
             /// Args:
             ///     file_path (str): The path to the file to write to.
             #[doc = $crate::serialization_format!()]
@@ -50,15 +76,15 @@
             fn serialize(
                 &self,
                 file_path: &str,
                 serialization_format: &str,
             ) -> pyo3::PyResult<()> {
                 $crate::impl_helper::serialization::serialize_to_file(
                     file_path,
-                    &self.0,
+                    &$crate::inner_type!($opaque, self),
                     serialization_format,
                 )
                 .map_err($crate::impl_helper::serialization::serialize_error)
             }
 
             /// Deserialize the internal data structure from a file.
             ///
@@ -67,33 +93,35 @@
             #[doc = $crate::serialization_format!()]
             #[staticmethod]
             #[pyo3(signature = (file_path, serialization_format="serde_json"))]
             fn deserialize(
                 file_path: &str,
                 serialization_format: &str,
             ) -> pyo3::PyResult<Self> {
-                $crate::impl_helper::serialization::deserialize_from_file(
-                    file_path,
-                    serialization_format,
+                $crate::map_type!(
+                    $opaque,
+                    $crate::impl_helper::serialization::deserialize_from_file(
+                        file_path,
+                        serialization_format,
+                    )
                 )
-                .map(Self)
                 .map_err($crate::impl_helper::serialization::deserialize_error)
             }
 
             /// Serialize the internal data structure into a string.
             ///
             /// Args:
             #[doc = $crate::serialization_format_string_compatible!()]
             #[pyo3(signature = (serialization_format="serde_json"))]
             fn serialize_to_string(
                 &self,
                 serialization_format: &str,
             ) -> pyo3::PyResult<String> {
                 $crate::impl_helper::serialization::serialize_to_string(
-                    &self.0,
+                    &$crate::inner_type!($opaque, self),
                     serialization_format,
                 )
                 .map_err($crate::impl_helper::serialization::serialize_error)
             }
 
             /// Deserialize the internal data structure from a string.
             ///
@@ -102,19 +130,21 @@
             #[doc = $crate::serialization_format_string_compatible!()]
             #[staticmethod]
             #[pyo3(signature = (string, serialization_format="serde_json"))]
             fn deserialize_from_string(
                 string: &str,
                 serialization_format: &str,
             ) -> pyo3::PyResult<Self> {
-                $crate::impl_helper::serialization::deserialize_from_string(
-                    string,
-                    serialization_format,
+                $crate::map_type!(
+                    $opaque,
+                    $crate::impl_helper::serialization::deserialize_from_string(
+                        string,
+                        serialization_format,
+                    )
                 )
-                .map(Self)
                 .map_err($crate::impl_helper::serialization::deserialize_error)
             }
         }
     };
 }
 use std::{
     error,
```

### Comparing `pauli_tracker-0.1.0/rust/src/impl_helper/tracker.rs` & `pauli_tracker-0.1.1/rust/src/impl_helper/tracker.rs`

 * *Files 6% similar despite different names*

```diff
@@ -31,21 +31,23 @@
     };
 }
 
 macro_rules! tracker_impl {
     ($type:ty) => {
         crate::impl_helper::tracker::single_pass!(
             $type, track_x, track_y, track_z, id, x, y, z, s, sdg, sz, szdg, hxy, h, sh,
-            hs, shs, sx, sxdg, hyz,
+            hs, shs, sx, sxdg, hyz, remove_z, remove_x,
         );
-        crate::impl_helper::tracker::double_pass!($type, cz, swap, iswap, iswapdg,);
+        crate::impl_helper::tracker::double_pass!($type, cz, swap, zcx, iswap, iswapdg,);
         crate::impl_helper::tracker::double_pass_named_bits!(
             $type,
             (cx, control, target),
             (cy, control, target),
+            (zcz, control, target),
+            (zcy, control, target),
             (move_z_to_z, source, destination),
             (move_z_to_x, source, destination),
             (move_x_to_z, source, destination),
             (move_x_to_x, source, destination),
         );
     };
 }
```

### Comparing `pauli_tracker-0.1.0/rust/src/lib.rs` & `pauli_tracker-0.1.1/rust/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pauli_tracker-0.1.0/rust/src/live/map.rs` & `pauli_tracker-0.1.1/rust/src/live/map.rs`

 * *Files identical despite different names*

### Comparing `pauli_tracker-0.1.0/rust/src/live/vec.rs` & `pauli_tracker-0.1.1/rust/src/live/vec.rs`

 * *Files identical despite different names*

### Comparing `pauli_tracker-0.1.0/rust/src/live.rs` & `pauli_tracker-0.1.1/rust/src/live.rs`

 * *Files identical despite different names*

### Comparing `pauli_tracker-0.1.0/rust/src/pauli.rs` & `pauli_tracker-0.1.1/rust/src/pauli.rs`

 * *Files 19% similar despite different names*

```diff
@@ -76,44 +76,69 @@
 
 #[pyo3::pyclass(subclass)]
 /// `PauliStack
 /// <https://docs.rs/pauli_tracker/latest/pauli_tracker/pauli/struct.PauliStack.html>`_\<`BitVec
 /// <https://docs.rs/bitvec/latest/bitvec/vec/struct.BitVec.html>`_\>.
 ///
 /// The Pauli Z and X stacks are bitvectors where each chunk consists of 64 bits. In the
-/// chunk the bits are ordered from least to most significant. You can use
-/// :func:`~pauli_tracker.bitvector_to_boolvector` to convert the bitvector to a list of
-/// booleans.
+/// chunk the bits are ordered from least to most significant.
 #[derive(Clone)]
 pub struct PauliStack(pub pauli::PauliStack<BitVec>);
 
 #[pyo3::pymethods]
 impl PauliStack {
     /// **Not defined**
     fn __init__(&self) {}
 
     #[doc = crate::transform!()]
+    /// You can use :func:`~pauli_tracker.bitvector_to_boolvector` to convert the
+    /// bitvector to a list of booleans, or directly use :func:`into_py_bool_tuple`.
     ///
     /// Returns:
     ///     tuple[list[int], list[int]]: The Z (left tuple element) and X (right tuple
     ///     element) components
     #[allow(clippy::wrong_self_convention)]
     pub fn into_py_tuple(&self) -> (Vec<u64>, Vec<u64>) {
         stack_into_py_tuple(self.0.clone())
     }
 
     #[doc = crate::take_transform!()]
+    /// You can use :func:`~pauli_tracker.bitvector_to_boolvector` to convert the
+    /// bitvector to a list of booleans, or directly use :func:`take_into_py_bool_tuple`.
     ///
     /// Returns:
     ///     tuple[list[int], list[int]]: The Z (left tuple element) and X (right tuple
     ///     element) components
     fn take_into_py_tuple(&mut self) -> (Vec<u64>, Vec<u64>) {
         stack_into_py_tuple(mem::take(&mut self.0))
     }
 
+    /// Transform the internal Rust data structure into the according Python tuple of
+    /// lists of booleans.  If you do this mutiple times consider using the according
+    /// `take_` method to avoid an additional clone, however, be aware that the internal
+    /// data is replaced with its default value.
+    ///
+    /// Returns:
+    ///     tuple[list[bool], list[bool]]: The Z (left tuple element) and X (right tuple
+    ///     element) components
+    #[allow(clippy::wrong_self_convention)]
+    pub fn into_py_bool_tuple(&self) -> (Vec<bool>, Vec<bool>) {
+        stack_into_py_bool_tuple(self.0.clone())
+    }
+
+    /// Transform the internal Rust data structure into the according Python tuple of
+    /// list of booleans, replacing the internal data with its default value.
+    ///
+    /// Returns:
+    ///     tuple[list[bool], list[bool]]: The Z (left tuple element) and X (right tuple
+    ///     element) components
+    fn take_into_py_bool_tuple(&mut self) -> (Vec<bool>, Vec<bool>) {
+        stack_into_py_bool_tuple(mem::take(&mut self.0))
+    }
+
     #[staticmethod]
     fn zeros(len: usize) -> Self {
         PauliStack(pauli::PauliStack::zeros(len))
     }
 
     pub fn xor_inplace(&mut self, other: &PauliStack) {
         self.0.xor_inplace(&other.0);
@@ -128,14 +153,18 @@
     }
 }
 
 fn stack_into_py_tuple(stack: pauli::PauliStack<BitVec>) -> (Vec<u64>, Vec<u64>) {
     (stack.z.into_vec(), stack.x.into_vec())
 }
 
+fn stack_into_py_bool_tuple(stack: pauli::PauliStack<BitVec>) -> (Vec<bool>, Vec<bool>) {
+    (stack.z.into_iter().collect(), stack.x.into_iter().collect())
+}
+
 serialization::serde!(PauliStack);
 
 pub fn add_module(py: Python<'_>, parent_module: &Module) -> PyResult<()> {
     let module = Module::new(py, "pauli", parent_module.path.clone())?;
     module.pymodule.add_class::<PauliDense>()?;
     module.pymodule.add_class::<PauliTuple>()?;
     module.pymodule.add_class::<PauliStack>()?;
```

### Comparing `pauli_tracker-0.1.0/rust/_lib/Cargo.toml` & `pauli_tracker-0.1.1/rust/_lib/Cargo.toml`

 * *Files identical despite different names*

### Comparing `pauli_tracker-0.1.0/README.md` & `pauli_tracker-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pauli_tracker-0.1.0/rust/_lib/Cargo.lock` & `pauli_tracker-0.1.1/rust/_lib/Cargo.lock`

 * *Files 9% similar despite different names*

```diff
@@ -8,35 +8,35 @@
 dependencies = [
  "pauli_tracker_pyo3",
  "pyo3",
 ]
 
 [[package]]
 name = "ahash"
-version = "0.8.8"
+version = "0.8.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "42cd52102d3df161c77a887b608d7a4897d7cc112886a9537b738a887a03aaff"
+checksum = "e89da841a80418a9b391ebaea17f5c112ffaaa96f621d2c285b5174da76b9011"
 dependencies = [
  "cfg-if",
  "once_cell",
  "version_check",
  "zerocopy",
 ]
 
 [[package]]
 name = "allocator-api2"
-version = "0.2.16"
+version = "0.2.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0942ffc6dcaadf03badf6e6a2d0228460359d5e34b57ccdc720b7382dfbd5ec5"
+checksum = "5c6cb57a04249c6480766f7f7cef5467412af1490f8d1e243141daddada3264f"
 
 [[package]]
 name = "autocfg"
-version = "1.1.0"
+version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
+checksum = "0c4b4d0bd25bd0b74681c0ad21497610ce1b7c91b1022cd21c80c6fbdd9476b0"
 
 [[package]]
 name = "bincode"
 version = "1.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b1f45e9417d87227c7a56d22e471c6206462cba514c7590c09aff4cf6d1ddcad"
 dependencies = [
@@ -50,17 +50,17 @@
 checksum = "349f9b6a179ed607305526ca489b34ad0a41aed5f7980fa90eb03160b69598fb"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "bitflags"
-version = "1.3.2"
+version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
+checksum = "cf4b9d6a944f767f8e5e0db018570623c85f3d925ac718db4e06d0187adb21c1"
 
 [[package]]
 name = "bitvec"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1bc2832c24239b0141d5674bb9174f9d68a8b5b3f2753311927c172ca46f7e9c"
 dependencies = [
@@ -80,58 +80,58 @@
  "serde",
  "smallvec",
  "wide",
 ]
 
 [[package]]
 name = "bytemuck"
-version = "1.14.3"
+version = "1.15.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a2ef034f05691a48569bd920a96c81b9d91bbad1ab5ac7c4616c1f6ef36cb79f"
+checksum = "5d6d68c57235a3a081186990eca2867354726650f42f7516ca50c28d6281fd15"
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "either"
-version = "1.10.0"
+version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "11157ac094ffbdde99aa67b23417ebdd801842852b500e395a45a9c0aac03e4a"
+checksum = "a47c1c47d2f5964e29c61246e81db715514cd532db6b5116a25ea3c03d6780a2"
 
 [[package]]
 name = "funty"
 version = "2.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e6d5a32815ae3f33302d95fdcb2ce17862f8c65363dcfd29360480ba1001fc9c"
 
 [[package]]
 name = "hashbrown"
-version = "0.14.3"
+version = "0.14.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "290f1a1d9242c78d09ce40a5e87e7554ee637af1351968159f4952f028f75604"
+checksum = "e5274423e17b7c9fc20b6e7e208532f9b19825d82dfd615708b70edd83df41f1"
 dependencies = [
  "ahash",
  "allocator-api2",
  "serde",
 ]
 
 [[package]]
 name = "heck"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
 
 [[package]]
 name = "indoc"
-version = "2.0.4"
+version = "2.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1e186cfbae8084e513daff4240b4797e342f988cecda4fb6c939150f96315fd8"
+checksum = "b248f5224d1d606005e02c97f5aa4e88eeb230488bcc03bc9ca4d7991399f2b5"
 
 [[package]]
 name = "inventory"
 version = "0.3.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f958d3d68f4167080a18141e10381e7634563984a537f2a49a30fd8e53ac5767"
 
@@ -142,77 +142,77 @@
 checksum = "ba291022dbbd398a455acf126c1e341954079855bc60dfdda641363bd6922569"
 dependencies = [
  "either",
 ]
 
 [[package]]
 name = "itoa"
-version = "1.0.10"
+version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b1a46d1a171d865aa5f83f92695765caa047a9b4cbae2cbf37dbd613a793fd4c"
+checksum = "49f1f14873335454500d59611f1cf4a4b0f786f9ac11f4312a78e4cf2566695b"
 
 [[package]]
 name = "libc"
-version = "0.2.153"
+version = "0.2.154"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
+checksum = "ae743338b92ff9146ce83992f766a31066a91a8c84a45e0e9f21e7cf6de6d346"
 
 [[package]]
 name = "lock_api"
-version = "0.4.11"
+version = "0.4.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3c168f8615b12bc01f9c17e2eb0cc07dcae1940121185446edc3744920e8ef45"
+checksum = "07af8b9cdd281b7915f413fa73f29ebd5d55d0d3f0155584dade1ff18cea1b17"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "memoffset"
-version = "0.9.0"
+version = "0.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
+checksum = "488016bfae457b036d996092f6cb448677611ce4449e970ceaf42695203f218a"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "once_cell"
 version = "1.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3fdb12b2476b595f9358c5161aa467c2438859caa136dec86c26fdd2efe17b92"
 
 [[package]]
 name = "parking_lot"
-version = "0.12.1"
+version = "0.12.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
+checksum = "7e4af0ca4f6caed20e900d564c242b8e5d4903fdacf31d3daf527b66fe6f42fb"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.9"
+version = "0.9.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c42a9226546d68acdd9c0a280d17ce19bfe27a46bf68784e4066115788d008e"
+checksum = "1e401f977ab385c9e4e3ab30627d6f26d00e2c73eef317493c4ec6d468726cf8"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
  "windows-targets",
 ]
 
 [[package]]
 name = "pauli_tracker"
-version = "0.4.0"
+version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da0f59848a5d13c655a14bc4521071dbd3585f8bf918f6a6c066059817897ceb"
+checksum = "2cb29073861435437f4145faa0e1bdfb4719216f0126d2a581f76ec6bc5b2a28"
 dependencies = [
  "bit-vec",
  "bitvec",
  "bitvec_simd",
  "hashbrown",
  "itertools",
  "serde",
@@ -229,119 +229,127 @@
  "pyo3",
  "rustc-hash",
  "serde",
  "serde_json",
 ]
 
 [[package]]
+name = "portable-atomic"
+version = "1.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7170ef9988bc169ba16dd36a7fa041e5c4cbeb6a35b76d4c03daded371eae7c0"
+
+[[package]]
 name = "proc-macro2"
-version = "1.0.78"
+version = "1.0.81"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e2422ad645d89c99f8f3e6b88a9fdeca7fabeac836b1002371c4367c8f984aae"
+checksum = "3d1597b0c024618f09a9c3b8655b7e430397a36d23fdafec26d6965e9eec3eba"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.20.2"
+version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9a89dc7a5850d0e983be1ec2a463a171d20990487c3cfcd68b5363f1ee3d6fe0"
+checksum = "53bdbb96d49157e65d45cc287af5f32ffadd5f4761438b527b055fb0d4bb8233"
 dependencies = [
  "cfg-if",
  "indoc",
  "inventory",
  "libc",
  "memoffset",
  "parking_lot",
+ "portable-atomic",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.20.2"
+version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "07426f0d8fe5a601f26293f300afd1a7b1ed5e78b2a705870c5f30893c5163be"
+checksum = "deaa5745de3f5231ce10517a1f5dd97d53e5a2fd77aa6b5842292085831d48d7"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.20.2"
+version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dbb7dec17e17766b46bca4f1a4215a85006b4c2ecde122076c562dd058da6cf1"
+checksum = "62b42531d03e08d4ef1f6e85a2ed422eb678b8cd62b762e53891c05faf0d4afa"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.20.2"
+version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "05f738b4e40d50b5711957f142878cfa0f28e054aa0ebdfc3fd137a843f74ed3"
+checksum = "7305c720fa01b8055ec95e484a6eca7a83c841267f0dd5280f0c8b8551d2c158"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.20.2"
+version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0fc910d4851847827daf9d6cdd4a823fbdaab5b8818325c5e97a86da79e8881f"
+checksum = "7c7e9b68bb9c3149c5b0cade5d07f953d6d125eb4337723c4ccdb665f1f96185"
 dependencies = [
  "heck",
  "proc-macro2",
+ "pyo3-build-config",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.35"
+version = "1.0.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "291ec9ab5efd934aaf503a6466c5d5251535d108ee747472c3977cc5acc868ef"
+checksum = "0fa76aaf39101c457836aec0ce2316dbdc3ab723cdda1c6bd4e6ad4208acaca7"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "radium"
 version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc33ff2d4973d518d823d61aa239014831e521c75da58e3df4840d3f47749d09"
 
 [[package]]
 name = "redox_syscall"
-version = "0.4.1"
+version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
+checksum = "469052894dcb553421e483e4209ee581a45100d31b4018de03e5a7ad86374a7e"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "rustc-hash"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "08d43f7aa6b08d49f382cde6a7982047c3426db949b1424bc4b7ec9ae12c6ce2"
 
 [[package]]
 name = "ryu"
-version = "1.0.16"
+version = "1.0.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f98d2aa92eebf49b69786be48e4477826b256916e84a57ff2a4f21923b48eb4c"
+checksum = "e86697c916019a8588c99b5fac3cead74ec0b4b819707a682fd4d23fa0ce1ba1"
 
 [[package]]
 name = "safe_arch"
 version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f398075ce1e6a179b46f51bd88d0598b92b00d3551f1a2d4ac49e771b56ac354"
 dependencies = [
@@ -352,89 +360,89 @@
 name = "scopeguard"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
 name = "serde"
-version = "1.0.196"
+version = "1.0.200"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "870026e60fa08c69f064aa766c10f10b1d62db9ccd4d0abb206472bee0ce3b32"
+checksum = "ddc6f9cc94d67c0e21aaf7eda3a010fd3af78ebf6e096aa6e2e13c79749cce4f"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.196"
+version = "1.0.200"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "33c85360c95e7d137454dc81d9a4ed2b8efd8fbe19cee57357b32b9771fccb67"
+checksum = "856f046b9400cee3c8c94ed572ecdb752444c24528c035cd35882aad6f492bcb"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.113"
+version = "1.0.116"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "69801b70b1c3dac963ecb03a364ba0ceda9cf60c71cfe475e99864759c8b8a79"
+checksum = "3e17db7126d17feb94eb3fad46bf1a96b034e8aacbc2e775fe81505f8b0b2813"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
 name = "smallvec"
-version = "1.13.1"
+version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e6ecd384b10a64542d77071bd64bd7b231f4ed5940fba55e98c3de13824cf3d7"
+checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.48"
+version = "2.0.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0f3531638e407dfc0814761abb7c00a5b54992b849452a0646b7f65c9f770f3f"
+checksum = "909518bc7b1c9b779f1bbf07f2929d35af9f0f37e47c6e9ef7f9dddc1e1821f3"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "tap"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "55937e1799185b12863d447f42597ed69d9928686b8d88a1df17376a097d8369"
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.13"
+version = "0.12.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "69758bda2e78f098e4ccb393021a0963bb3442eac05f135c30f61b7370bbafae"
+checksum = "e1fc403891a21bcfb7c37834ba66a547a8f402146eba7265b5a6d88059c9ff2f"
 
 [[package]]
 name = "thiserror"
-version = "1.0.57"
+version = "1.0.59"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1e45bcbe8ed29775f228095caf2cd67af7a4ccf756ebff23a306bf3e8b47b24b"
+checksum = "f0126ad08bff79f29fc3ae6a55cc72352056dfff61e3ff8bb7129476d44b23aa"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.57"
+version = "1.0.59"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a953cb265bef375dae3de6663da4d3804eee9682ea80d8e2542529b73c531c81"
+checksum = "d1cd413b5d558b4c5bf3680e324a6fa5014e7b7c067a51e69dbdf47eb7148b66"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
@@ -453,100 +461,107 @@
 name = "version_check"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
 
 [[package]]
 name = "wide"
-version = "0.7.15"
+version = "0.7.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "89beec544f246e679fc25490e3f8e08003bc4bf612068f325120dad4cea02c1c"
+checksum = "0f0e39d2c603fdc0504b12b458cf1f34e0b937ed2f4f2dc20796e3e86f34e11f"
 dependencies = [
  "bytemuck",
  "safe_arch",
 ]
 
 [[package]]
 name = "windows-targets"
-version = "0.48.5"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9a2fa6e2155d7247be68c096456083145c183cbbbc2764150dda45a87197940c"
+checksum = "6f0713a46559409d202e70e28227288446bf7841d3211583a4b53e3f6d96e7eb"
 dependencies = [
  "windows_aarch64_gnullvm",
  "windows_aarch64_msvc",
  "windows_i686_gnu",
+ "windows_i686_gnullvm",
  "windows_i686_msvc",
  "windows_x86_64_gnu",
  "windows_x86_64_gnullvm",
  "windows_x86_64_msvc",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.48.5"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2b38e32f0abccf9987a4e3079dfb67dcd799fb61361e53e2882c3cbaf0d905d8"
+checksum = "7088eed71e8b8dda258ecc8bac5fb1153c5cffaf2578fc8ff5d61e23578d3263"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.48.5"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dc35310971f3b2dbbf3f0690a219f40e2d9afcf64f9ab7cc1be722937c26b4bc"
+checksum = "9985fd1504e250c615ca5f281c3f7a6da76213ebd5ccc9561496568a2752afb6"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.48.5"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "88ba073cf16d5372720ec942a8ccbf61626074c6d4dd2e745299726ce8b89670"
+
+[[package]]
+name = "windows_i686_gnullvm"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a75915e7def60c94dcef72200b9a8e58e5091744960da64ec734a6c6e9b3743e"
+checksum = "87f4261229030a858f36b459e748ae97545d6f1ec60e5e0d6a3d32e0dc232ee9"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.48.5"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8f55c233f70c4b27f66c523580f78f1004e8b5a8b659e05a4eb49d4166cca406"
+checksum = "db3c2bf3d13d5b658be73463284eaf12830ac9a26a90c717b7f771dfe97487bf"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.48.5"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "53d40abd2583d23e4718fddf1ebec84dbff8381c07cae67ff7768bbf19c6718e"
+checksum = "4e4246f76bdeff09eb48875a0fd3e2af6aada79d409d33011886d3e1581517d9"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.48.5"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0b7b52767868a23d5bab768e390dc5f5c55825b6d30b86c844ff2dc7414044cc"
+checksum = "852298e482cd67c356ddd9570386e2862b5673c85bd5f88df9ab6802b334c596"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.48.5"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ed94fce61571a4006852b7389a063ab983c02eb1bb37b47f8272ce92d06d9538"
+checksum = "bec47e5bfd1bff0eeaf6d8b485cc1074891a197ab4225d504cb7a1ab88b02bf0"
 
 [[package]]
 name = "wyz"
 version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "05f360fc0b24296329c78fda852a1e9ae82de9cf7b27dae4b7f62f118f77b9ed"
 dependencies = [
  "tap",
 ]
 
 [[package]]
 name = "zerocopy"
-version = "0.7.32"
+version = "0.7.33"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "74d4d3961e53fa4c9a25a8637fc2bfaf2595b3d3ae34875568a5cf64787716be"
+checksum = "087eca3c1eaf8c47b94d02790dd086cd594b912d2043d4de4bfdd466b3befb7c"
 dependencies = [
  "zerocopy-derive",
 ]
 
 [[package]]
 name = "zerocopy-derive"
-version = "0.7.32"
+version = "0.7.33"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9ce1b18ccd8e73a9321186f97e46f9f04b778851177567b1975109d26a08d2a6"
+checksum = "6f4b6c273f496d8fd4eaf18853e6b448760225dc030ff2c485a786859aea6393"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
```

### Comparing `pauli_tracker-0.1.0/pyproject.toml` & `pauli_tracker-0.1.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 [build-system]
 requires = ["maturin>=1.4,<2.0"]
 build-backend = "maturin"
 
 [project]
 name = "pauli_tracker"
-version = "0.1.0"
+version = "0.1.1"
 authors = [{name="Jannis Ruh", email="ruh.j81@gmail.com"}]
 
-description = "A library to track Pauli gates through a Clifford circuit."
+description = "A library to track Pauli gates through Clifford circuits."
 
 readme = "README.md"
 
 requires-python = ">=3.8"
 classifiers = [
   "License :: OSI Approved :: MIT License",
   "License :: OSI Approved :: Apache Software License",
 ]
 
 [project.urls]
 Repository = "https://github.com/taeruh/pauli_tracker"
+Documentation = "https://taeruh.github.io/pauli_tracker/"
 
 [tool.maturin]
 features = ["pyo3/extension-module"]
 module-name = "pauli_tracker._lib"
 manifest-path = "rust/_lib/Cargo.toml"
 python-source = "python"
 include = [{ path = "LICENSE*", format = "sdist" }]
```

### Comparing `pauli_tracker-0.1.0/python/pauli_tracker/__init__.py` & `pauli_tracker-0.1.1/python/pauli_tracker/__init__.py`

 * *Files identical despite different names*

### Comparing `pauli_tracker-0.1.0/LICENSE-APACHE` & `pauli_tracker-0.1.1/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `pauli_tracker-0.1.0/LICENSE-MIT` & `pauli_tracker-0.1.1/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `pauli_tracker-0.1.0/PKG-INFO` & `pauli_tracker-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: pauli_tracker
-Version: 0.1.0
+Version: 0.1.1
 Classifier: License :: OSI Approved :: MIT License
 Classifier: License :: OSI Approved :: Apache Software License
 License-File: LICENSE-APACHE
 License-File: LICENSE-MIT
-Summary: A library to track Pauli gates through a Clifford circuit.
+Summary: A library to track Pauli gates through Clifford circuits.
 Keywords: quantum,clifford,pauli,mbqc
 Author: Jannis Ruh <ruh.j81@gmail.com>
 Author-email: Jannis Ruh <ruh.j81@gmail.com>
 License: MIT OR Apache-2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Repository, https://github.com/taeruh/pauli_tracker
+Project-URL: Documentation, https://taeruh.github.io/pauli_tracker/
 
 # Python wrapper around pauli_tracker
 
 This Python package is a wrapper around the [pauli_tracker crate] exporting its basic
 functionality.
 
 If some essential functionality is missing, because we just forgot to implement it, please
```

