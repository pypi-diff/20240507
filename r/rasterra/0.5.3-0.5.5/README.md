# Comparing `tmp/rasterra-0.5.3.tar.gz` & `tmp/rasterra-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rasterra-0.5.3.tar", max compression
+gzip compressed data, was "rasterra-0.5.5.tar", max compression
```

## Comparing `rasterra-0.5.3.tar` & `rasterra-0.5.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1521 2024-03-18 13:07:59.942917 rasterra-0.5.3/LICENSE
--rw-r--r--   0        0        0     2688 2024-03-18 13:07:59.942917 rasterra-0.5.3/README.md
--rw-r--r--   0        0        0     2626 2024-03-18 13:07:59.942917 rasterra-0.5.3/pyproject.toml
--rw-r--r--   0        0        0       77 2024-03-18 13:07:59.942917 rasterra-0.5.3/src/rasterra/__init__.py
--rw-r--r--   0        0        0    18168 2024-03-18 13:07:59.942917 rasterra-0.5.3/src/rasterra/_array.py
--rw-r--r--   0        0        0     3223 2024-03-18 13:07:59.942917 rasterra-0.5.3/src/rasterra/_features.py
--rw-r--r--   0        0        0     1644 2024-03-18 13:07:59.942917 rasterra-0.5.3/src/rasterra/_io.py
--rw-r--r--   0        0        0     3640 2024-03-18 13:07:59.942917 rasterra-0.5.3/src/rasterra/_plotting.py
--rw-r--r--   0        0        0      495 2024-03-18 13:07:59.942917 rasterra-0.5.3/src/rasterra/_typing.py
--rw-r--r--   0        0        0        0 2024-03-18 13:07:59.942917 rasterra-0.5.3/src/rasterra/py.typed
--rw-r--r--   0        0        0     3998 1970-01-01 00:00:00.000000 rasterra-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1521 2024-05-07 20:43:35.010338 rasterra-0.5.5/LICENSE
+-rw-r--r--   0        0        0     2687 2024-05-07 20:43:35.010338 rasterra-0.5.5/README.md
+-rw-r--r--   0        0        0     3548 2024-05-07 20:43:35.014338 rasterra-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0      152 2024-05-07 20:43:35.014338 rasterra-0.5.5/src/rasterra/__init__.py
+-rw-r--r--   0        0        0    19220 2024-05-07 20:43:35.014338 rasterra-0.5.5/src/rasterra/_array.py
+-rw-r--r--   0        0        0     3267 2024-05-07 20:43:35.014338 rasterra-0.5.5/src/rasterra/_features.py
+-rw-r--r--   0        0        0     1657 2024-05-07 20:43:35.014338 rasterra-0.5.5/src/rasterra/_io.py
+-rw-r--r--   0        0        0     3795 2024-05-07 20:43:35.014338 rasterra-0.5.5/src/rasterra/_plotting.py
+-rw-r--r--   0        0        0      565 2024-05-07 20:43:35.014338 rasterra-0.5.5/src/rasterra/_typing.py
+-rw-r--r--   0        0        0        0 2024-05-07 20:43:35.014338 rasterra-0.5.5/src/rasterra/py.typed
+-rw-r--r--   0        0        0     3997 1970-01-01 00:00:00.000000 rasterra-0.5.5/PKG-INFO
```

### Comparing `rasterra-0.5.3/LICENSE` & `rasterra-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `rasterra-0.5.3/README.md` & `rasterra-0.5.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 
 ```sh
 pip install rasterra
 ```
 
 ## Usage
 
-
 ### File I/O
 
 Reading and writing raster data is done using the `load_raster` and `to_file` functions.
 
 ```python
 import rasterra as rt
```

### Comparing `rasterra-0.5.3/src/rasterra/_array.py` & `rasterra-0.5.5/src/rasterra/_array.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,44 @@
 import numbers
 import typing
 
 import geopandas as gpd
 import numpy as np
+import numpy.typing as npt
 from affine import Affine
 from numpy.core.multiarray import flagsobj
 from rasterio.crs import CRS
 from rasterio.warp import Resampling, reproject
 from shapely.geometry import MultiPolygon, Polygon
 
 from rasterra._features import raster_geometry_mask, to_gdf
 from rasterra._plotting import Plotter
-from rasterra._typing import FilePath, Number, NumpyDtype, NumpyUFuncMethod, RawCRS
+from rasterra._typing import (
+    FilePath,
+    NumpyUFuncMethod,
+    RasterData,
+    RasterMask,
+    RawCRS,
+    SupportedDtypes,
+)
 
 _RESAMPLING_MAP = {data.name: data for data in Resampling}
 
 NO_DATA_UNSET = None
 
+_IDENTITY_TRANSFORM: Affine = Affine.identity()
+
 
 class RasterArray(np.lib.mixins.NDArrayOperatorsMixin):
     def __init__(
         self,
-        data: np.ndarray,
-        transform: Affine = Affine.identity(),
+        data: RasterData,
+        transform: Affine = _IDENTITY_TRANSFORM,
         crs: RawCRS | None = None,
-        no_data_value: Number | None = NO_DATA_UNSET,
+        no_data_value: SupportedDtypes | None = NO_DATA_UNSET,
     ):
         """
         Initialize a RasterArray.
 
         Parameters
         ----------
         data
@@ -88,70 +98,73 @@
 
     @property
     def nbytes(self) -> int:
         """Number of bytes in the raster."""
         return self._ndarray.nbytes
 
     @property
-    def base(self) -> np.ndarray | None:
+    def base(self) -> RasterData | None:
         """Base object of the raster."""
         return self._ndarray.base
 
     @property
-    def dtype(self) -> np.dtype:
+    def dtype(self) -> np.dtype[SupportedDtypes]:
         """Data type of the raster."""
         return self._ndarray.dtype
 
     @property
     def T(self) -> typing.NoReturn:  # noqa: N802
         """Transpose of the raster."""
-        raise TypeError("Transpose of a raster is not defined.")
+        msg = "Transpose of a raster is not defined."
+        raise TypeError(msg)
 
     @property
-    def real(self) -> "RasterArray":
+    def real(self) -> typing.NoReturn:
         """Real part of the raster."""
-        return RasterArray(
-            self._ndarray.real, self._transform, self._crs, self._no_data_value
-        )
+        msg = "Complex raster data is not supported."
+        raise NotImplementedError(msg)
 
     @property
-    def imag(self) -> "RasterArray":
+    def imag(self) -> typing.NoReturn:
         """Imaginary part of the raster."""
-        return RasterArray(
-            self._ndarray.imag, self._transform, self._crs, self._no_data_value
-        )
+        msg = "Complex raster data is not supported."
+        raise NotImplementedError(msg)
 
     @property
-    def flat(self) -> np.flatiter:
+    def flat(self) -> np.flatiter[RasterData]:
         """Flat iterator of the raster."""
         return self._ndarray.flat
 
     @property
     def ctypes(self) -> typing.NoReturn:
         """ctypes object of the raster."""
-        raise TypeError("ctypes object of a raster is not defined.")
+        msg = "ctypes object of a raster is not defined."
+        raise TypeError(msg)
 
     def __getitem__(self, item: int | slice | tuple[int, int] | tuple[slice, slice]):  # type: ignore[no-untyped-def]
         def _process_item(_item: int | slice) -> int | slice:
             if isinstance(_item, int):
                 return _item
             elif isinstance(_item, slice):
                 if _item.step is not None:
-                    raise ValueError("Slicing with a step is not supported")
+                    msg = "Slicing with a step is not supported."
+                    raise ValueError(msg)
                 return _item.start or 0
             else:
-                raise TypeError("Invalid index type")
+                msg = "Invalid index type"
+                raise TypeError(msg)
 
         new_data = self._ndarray[item]
         if not isinstance(new_data, np.ndarray):
             return new_data
 
         if isinstance(item, tuple):
-            if not len(item) == 2:
-                raise ValueError("Invalid number of indices")
+            if len(item) != 2:  # noqa: PLR2004
+                msg = "Invalid number of indices"
+                raise ValueError(msg)
             y_item, x_item = item
 
             yi = _process_item(y_item)
             xi = _process_item(x_item)
         else:
             yi = _process_item(item)
             xi = 0
@@ -166,56 +179,60 @@
         )
 
         return RasterArray(new_data, new_transform, self._crs, self._no_data_value)
 
     # ----------------------------------------------------------------
     # NumPy array interface
 
-    def astype(self, dtype: NumpyDtype) -> "RasterArray":
+    def astype(self, dtype: np.dtype[SupportedDtypes]) -> "RasterArray":
         """Cast the raster to a new data type."""
         return RasterArray(
             self._ndarray.astype(dtype), self._transform, self._crs, self._no_data_value
         )
 
-    def to_numpy(self) -> np.ndarray:
+    def to_numpy(self) -> RasterData:
         """Convert the raster to a NumPy array."""
         return self._ndarray.copy()
 
-    def __array__(self, dtype: NumpyDtype | None = None) -> np.ndarray:
+    def __array__(self, dtype: np.dtype[SupportedDtypes] | None = None) -> RasterData:
         return np.asarray(self._ndarray, dtype=dtype)
 
     def __array_ufunc__(
         self,
         ufunc: np.ufunc,
         method: NumpyUFuncMethod,
-        *inputs: np.ndarray | Number | "RasterArray",
+        *inputs: typing.Union[RasterData, SupportedDtypes, "RasterArray"],
         **kwargs: typing.Any,
     ) -> typing.Union[tuple["RasterArray", ...], "RasterArray"]:
         out = kwargs.get("out", ())
         for x in inputs + out:
             # Only support operations with instances of _HANDLED_TYPES.
             # Use RasterArray instead of type(self) for isinstance to
             # allow subclasses that don't override __array_ufunc__ to
             # handle RasterArray objects.
             handled_types = (np.ndarray, numbers.Number, RasterArray)
             if not isinstance(x, handled_types):
                 return NotImplemented
             if isinstance(x, RasterArray):
-                if x._crs != self._crs:
-                    raise ValueError("Coordinate reference systems do not match.")
-                if not self._no_data_equal(x._no_data_value):
-                    raise ValueError("No data values do not match.")
-                if x._transform != self._transform:
-                    raise ValueError("Affine transforms do not match.")
+                if x._crs != self._crs:  # noqa: SLF001
+                    msg = "Coordinate reference systems do not match."
+                    raise ValueError(msg)
+                if not self._no_data_equal(x._no_data_value):  # noqa: SLF001
+                    msg = "No data values do not match."
+                    raise ValueError(msg)
+                if x._transform != self._transform:  # noqa: SLF001
+                    msg = "Affine transforms do not match."
+                    raise ValueError(msg)
 
         # Defer to the implementation of the ufunc on unwrapped values.
-        inputs = tuple(x._ndarray if isinstance(x, RasterArray) else x for x in inputs)
+        inputs = tuple(x._ndarray if isinstance(x, RasterArray) else x for x in inputs)  # noqa: SLF001
         if out:
             kwargs["out"] = tuple(
-                x._ndarray if isinstance(x, RasterArray) else x for x in out
+                x._ndarray if isinstance(x, RasterArray) else x  # noqa: SLF001
+                for x in out
             )
         result = getattr(ufunc, method)(*inputs, **kwargs)
 
         if type(result) is tuple:
             # multiple return values
             return tuple(
                 type(self)(x, self._transform, self._crs, self._no_data_value)
@@ -243,67 +260,67 @@
     def transform(self) -> Affine:
         """Affine transform to georeference the raster."""
         return self._transform
 
     @property
     def x_min(self) -> float:
         """Minimum x coordinate."""
-        return self.transform.c
+        return self.transform.c  # type: ignore[no-any-return]
 
     @property
     def x_max(self) -> float:
         """Maximum x coordinate."""
         return self.x_min + self.x_resolution * self.width
 
     @property
     def y_min(self) -> float:
         """Minimum y coordinate."""
         return self.y_max + self.y_resolution * self.height
 
     @property
     def y_max(self) -> float:
         """Maximum y coordinate."""
-        return self.transform.f
+        return self.transform.f  # type: ignore[no-any-return]
 
     @property
     def width(self) -> int:
         """Width of the raster."""
         return self._ndarray.shape[1]
 
     @property
     def height(self) -> int:
         """Height of the raster."""
         return self._ndarray.shape[0]
 
     @property
     def x_resolution(self) -> float:
         """Resolution in x direction."""
-        return self.transform.a
+        return self.transform.a  # type: ignore[no-any-return]
 
     @property
     def y_resolution(self) -> float:
         """Resolution in y direction."""
-        return self.transform.e
+        return self.transform.e  # type: ignore[no-any-return]
 
-    def x_coordinates(self, center: bool = False) -> np.ndarray:
+    def x_coordinates(self, *, center: bool = False) -> npt.NDArray[np.float64]:
         """x coordinates of the raster."""
         if center:
             return np.linspace(
                 self.x_min + self.x_resolution / 2,
                 self.x_max - self.x_resolution / 2,
                 self.width,
             )
         else:
             return np.linspace(
                 self.x_min,
                 self.x_max - self.x_resolution,
                 self.width,
             )
 
-    def y_coordinates(self, center: bool = False) -> np.ndarray:
+    def y_coordinates(self, *, center: bool = False) -> npt.NDArray[np.float64]:
         """y coordinates of the raster."""
         if center:
             return np.linspace(
                 self.y_min - self.y_resolution / 2,
                 self.y_max + self.y_resolution / 2,
                 self.height,
             )
@@ -319,32 +336,34 @@
         """Bounding box of the raster."""
         return self.x_min, self.x_max, self.y_min, self.y_max
 
     @property
     def crs(self) -> str | None:
         """Coordinate reference system."""
         if isinstance(self._crs, CRS):
-            return self._crs.to_string()
+            return self._crs.to_string()  # type: ignore[no-any-return]
         else:
             return self._crs
 
     def set_crs(self, new_crs: RawCRS) -> "RasterArray":
         if self._crs is not None:
-            raise ValueError(
+            msg = (
                 "Coordinate reference system is already set. Use to_crs() to reproject "
                 "to a new coordinate reference system."
             )
+            raise ValueError(msg)
         return RasterArray(
             self._ndarray.copy(), self._transform, new_crs, self._no_data_value
         )
 
     def to_crs(self, new_crs: str, resampling: str = "nearest") -> "RasterArray":
         """Reproject the raster to a new coordinate reference system."""
         if self._crs is None:
-            raise ValueError("Coordinate reference system is not set.")
+            msg = "Coordinate reference system is not set."
+            raise ValueError(msg)
         resampling = _RESAMPLING_MAP[resampling]
         new_crs = CRS.from_user_input(new_crs)
 
         new_data, transform = reproject(
             source=self._ndarray,
             src_transform=self._transform,
             src_crs=self._crs,
@@ -353,48 +372,49 @@
             resampling=resampling,
         )
         return RasterArray(
             new_data[0], transform, new_crs, no_data_value=self._no_data_value
         )
 
     @property
-    def no_data_value(self) -> Number:
+    def no_data_value(self) -> SupportedDtypes:
         """Value representing no data."""
         if self._no_data_value is NO_DATA_UNSET:
-            raise ValueError("No data value is not set.")
+            msg = "No data value is not set."
+            raise ValueError(msg)
         return self._no_data_value
 
-    def set_no_data_value(self, new_no_data_value: Number) -> "RasterArray":
+    def set_no_data_value(self, new_no_data_value: SupportedDtypes) -> "RasterArray":
         new_data = self._ndarray.copy()
         if self._no_data_value is not NO_DATA_UNSET:
             new_data[self.no_data_mask] = new_no_data_value
         return RasterArray(new_data, self._transform, self._crs, new_no_data_value)
 
-    def _no_data_equal(self, other_no_data_value: Number | None) -> bool:
+    def _no_data_equal(self, other_no_data_value: SupportedDtypes | None) -> bool:
         if self._no_data_value is NO_DATA_UNSET:
             return other_no_data_value is NO_DATA_UNSET
         elif other_no_data_value is NO_DATA_UNSET:
             return False
         elif np.isnan(self._no_data_value):
-            return np.isnan(other_no_data_value)
+            return np.isnan(other_no_data_value)  # type: ignore[no-any-return]
         elif np.isinf(self._no_data_value):
-            return np.isinf(other_no_data_value) and np.sign(
-                self._no_data_value
-            ) == np.sign(other_no_data_value)
+            other_inf = np.isinf(other_no_data_value)
+            sign_match = np.sign(self._no_data_value) == np.sign(other_no_data_value)
+            return other_inf and sign_match  # type: ignore[no-any-return]
         else:
-            return self._no_data_value == other_no_data_value
+            return self._no_data_value == other_no_data_value  # type: ignore[no-any-return]
 
     def unset_no_data_value(self) -> "RasterArray":
         """Unset value representing no data."""
         return RasterArray(
             self._ndarray.copy(), self._transform, self._crs, NO_DATA_UNSET
         )
 
     @property
-    def no_data_mask(self) -> np.ndarray:
+    def no_data_mask(self) -> RasterMask:
         """Mask representing no data."""
         if self._no_data_value is NO_DATA_UNSET:
             return np.zeros_like(self._ndarray, dtype=bool)
         elif np.isnan(self._no_data_value):
             return np.isnan(self._ndarray)
         elif np.isinf(self._no_data_value):
             return np.isinf(self._ndarray)
@@ -425,35 +445,39 @@
 
     def resample_to(
         self, target: "RasterArray", resampling: str = "nearest"
     ) -> "RasterArray":
         """Resample the raster to match the resolution of another raster."""
         resampling = _RESAMPLING_MAP[resampling]
 
-        destination = np.empty_like(target._ndarray, dtype=self._ndarray.dtype)
+        destination = np.empty_like(target._ndarray, dtype=self._ndarray.dtype)  # noqa: SLF001
         new_data, transform = reproject(
             source=self._ndarray,
             src_transform=self._transform,
             src_crs=self._crs,
             src_nodata=self._no_data_value,
             destination=destination,
             dst_transform=target.transform,
-            dst_crs=target._crs,
+            dst_crs=target._crs,  # noqa: SLF001
             resampling=resampling,
         )
         return RasterArray(
-            new_data, transform, target._crs, no_data_value=self.no_data_value
+            new_data,
+            transform,
+            target._crs,  # noqa: SLF001
+            no_data_value=self.no_data_value,
         )
 
     def _coerce_to_shapely(
         self, shape: Polygon | MultiPolygon | gpd.GeoDataFrame | gpd.GeoSeries
     ) -> Polygon | MultiPolygon:
         if isinstance(shape, (gpd.GeoDataFrame, gpd.GeoSeries)):
-            if not shape.crs == self._crs:
-                raise ValueError("Coordinate reference systems do not match.")
+            if shape.crs != self._crs:
+                msg = "Coordinate reference systems do not match."
+                raise ValueError(msg)
             return shape.geometry.unary_union
         return shape
 
     def clip(
         self, shape: Polygon | MultiPolygon | gpd.GeoDataFrame | gpd.GeoSeries
     ) -> "RasterArray":
         """Clip the raster to a shape."""
@@ -472,23 +496,26 @@
         return RasterArray(
             new_data, transform, self._crs, no_data_value=self.no_data_value
         )
 
     def mask(
         self,
         shape: Polygon | MultiPolygon | gpd.GeoDataFrame | gpd.GeoSeries,
-        fill_value: Number | None = None,
+        *,
+        fill_value: SupportedDtypes | None = None,
         all_touched: bool = False,
         invert: bool = False,
     ) -> "RasterArray":
         """Mask the raster with a shape."""
         shape = self._coerce_to_shapely(shape)
         if fill_value is None and self._no_data_value is NO_DATA_UNSET:
-            raise ValueError("No fill value is set.")
-        elif fill_value is None:
+            msg = "No fill value is set."
+            raise ValueError(msg)
+
+        if fill_value is None:
             fill_value = self.no_data_value
 
         shape_mask, *_ = raster_geometry_mask(
             data_transform=self.transform,
             data_width=self._ndarray.shape[1],
             data_height=self._ndarray.shape[0],
             shapes=[shape],
```

### Comparing `rasterra-0.5.3/src/rasterra/_features.py` & `rasterra-0.5.5/src/rasterra/_features.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 import numpy as np
 from affine import Affine
 from rasterio.features import bounds, rasterize
 from rasterio.windows import Window
 from shapely import box
 from shapely.geometry import MultiPolygon, Polygon
 
+from rasterra._typing import RasterData
+
 if typing.TYPE_CHECKING:
     from rasterra import RasterArray
 
 
 def _geometry_window(
     data_transform: Affine,
     data_width: int,
@@ -42,17 +44,15 @@
         row_off=row_start,
         width=max(col_stop - col_start, 0),
         height=max(row_stop - row_start, 0),
     )
 
     # Make sure that window overlaps raster
     raster_window = Window(0, 0, data_width, data_height)
-    window = window.intersection(raster_window)
-
-    return window
+    return window.intersection(raster_window)
 
 
 def _window_transform(
     window: Window,
     transform: Affine,
 ) -> Affine:
     x, y = transform * (window.col_off or 0.0, window.row_off or 0.0)
@@ -60,22 +60,24 @@
 
 
 def raster_geometry_mask(
     data_transform: Affine,
     data_width: int,
     data_height: int,
     shapes: list[Polygon | MultiPolygon],
+    *,
     all_touched: bool = False,
     invert: bool = False,
     crop: bool = False,
     pad_x: float = 0.0,
     pad_y: float = 0.0,
-) -> tuple[np.ndarray, Affine, Window]:
+) -> tuple[RasterData, Affine, Window]:
     if crop and invert:
-        raise ValueError("crop and invert cannot both be True.")
+        msg = "Crop and invert cannot both be True"
+        raise ValueError(msg)
 
     window = _geometry_window(
         data_transform,
         data_width,
         data_height,
         shapes,
         pad_x=pad_x,
```

### Comparing `rasterra-0.5.3/src/rasterra/_io.py` & `rasterra-0.5.5/src/rasterra/_io.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,29 +1,31 @@
-from typing import Sequence
+from collections.abc import Sequence
 
 import rasterio
 from rasterio.merge import merge
 
 from rasterra._array import RasterArray
 from rasterra._typing import FilePath
 
 
 def load_raster(path: FilePath) -> RasterArray:
     """Load a raster from a file."""
+
     with rasterio.open(path) as f:
         data = f.read()
         if data.shape[0] == 1:
             return RasterArray(
                 data[0],
                 transform=f.transform,
                 crs=f.crs,
                 no_data_value=f.nodata,
             )
         else:
-            raise NotImplementedError("Only single-band rasters are supported.")
+            msg = "Only single-band rasters are supported"
+            raise NotImplementedError(msg)
 
 
 def write_raster(
     raster: RasterArray,
     path: FilePath,
 ) -> None:
     """Write a raster to a file."""
@@ -44,16 +46,16 @@
 
 def load_mf_raster(paths: Sequence[FilePath]) -> RasterArray:
     """Load multiple files into a single raster."""
     with rasterio.open(paths[0]) as f:
         data = f.read()
         if data.shape[0] == 1:
             merged, transform = merge(paths)
-            assert merged.shape[0] == 1
             return RasterArray(
                 merged[0],
                 transform=transform,
                 crs=f.crs,
                 no_data_value=f.nodata,
             )
         else:
-            raise NotImplementedError("Only single-band rasters are supported.")
+            msg = "Only single-band rasters are supported."
+            raise NotImplementedError(msg)
```

### Comparing `rasterra-0.5.3/src/rasterra/_plotting.py` & `rasterra-0.5.5/src/rasterra/_plotting.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,38 +1,44 @@
-from typing import Any, Union
+from typing import Any
 
 import affine
 import matplotlib.pyplot as plt
 import numpy as np
 from matplotlib.axes import Axes
 from matplotlib.colors import Colormap, Normalize
 from mpl_toolkits.axes_grid1 import make_axes_locatable
 from rasterio.plot import plotting_extent
 
+from rasterra._typing import RasterData, RasterMask
+
 
 class Plotter:
     def __init__(
-        self, data: np.ndarray, data_mask: np.ndarray, transform: affine.Affine
+        self,
+        data: RasterData,
+        data_mask: RasterMask,
+        transform: affine.Affine,
     ) -> None:
         self._data = data
         self._mask = data_mask
         self._transform = transform
 
     def __call__(
         self,
-        ax: Union[Axes, None] = None,
-        cmap: Union[str, Colormap] = "viridis",
-        vmin: Union[float, None] = None,
-        vmax: Union[float, None] = None,
-        under_color: Union[str, None] = None,
-        norm: Union[Normalize, None] = None,
+        ax: Axes | None = None,
+        cmap: str | Colormap = "viridis",
+        vmin: float | None = None,
+        vmax: float | None = None,
+        under_color: str | None = None,
+        norm: Normalize | None = None,
         **kwargs: Any,
     ) -> Axes:
         if (vmin is not None or vmax is not None) and norm is not None:
-            raise ValueError("Cannot pass both vmin/vmax and norm.")
+            msg = "Cannot pass both vmin/vmax and norm."
+            raise ValueError(msg)
         if norm is None:
             norm = Normalize(vmin=vmin, vmax=vmax)
 
         kwargs["extent"] = plotting_extent(self._data, self._transform)
 
         show_plt = False
         if not ax:
@@ -46,20 +52,20 @@
 
         return ax
 
     def test_normalization(
         self,
         norm: Normalize,
         nbins: int = 50,
-        cmap: Union[str, Colormap] = "viridis",
-        under_color: Union[str, None] = None,
+        cmap: str | Colormap = "viridis",
+        under_color: str | None = None,
     ) -> None:
         """Test a normalization of the data for plotting."""
-        vmin = norm.vmin
-        vmax = norm.vmax
+        vmin = norm.vmin if norm.vmin is not None else self._data.min()
+        vmax = norm.vmax if norm.vmax is not None else self._data.max()
         mask = (vmin <= self._data) & (self._data <= vmax) & ~self._mask
         data = self._data[mask].flatten()
 
         result = norm(data)
 
         fig, axes = plt.subplots(figsize=(15, 15), ncols=2, nrows=2)
 
@@ -76,15 +82,15 @@
         _make_hist_plot(result, nbins, "Normalized data", axes[0, 1])
         _make_image_plot(result, self._mask, norm, cmap, under_color, axes[1, 1])
 
         plt.show()
 
 
 def _make_hist_plot(
-    data: np.ndarray,
+    data: RasterData,
     nbins: int,
     title: str,
     ax: Axes,
 ) -> Axes:
     """Plot a histogram of the data."""
     hist, bins = np.histogram(data, nbins)
     cdf = hist.cumsum()
@@ -95,24 +101,24 @@
     ax2 = ax.twinx()
     ax2.plot(bins[:-1], cdf, color="tab:orange")  # type: ignore[attr-defined]
     ax2.set_ylabel("Cumulative frequency", color="tab:orange", fontsize=14)
     return ax
 
 
 def _make_image_plot(
-    data: np.ndarray,
-    mask: np.ndarray,
+    data: RasterData,
+    mask: RasterMask,
     norm: Normalize,
-    cmap: Union[str, Colormap],
-    under_color: Union[str, None],
+    cmap: str | Colormap,
+    under_color: str | None,
     ax: Axes,
     **kwargs: Any,
 ) -> Axes:
     """Plot a histogram of the data."""
-    masked: np.ma.MaskedArray = np.ma.masked_array(data, mask=mask)
+    masked = np.ma.masked_array(data, mask=mask)  # type: ignore[no-untyped-call,var-annotated]
     im = ax.imshow(
         masked,
         cmap=cmap,
         norm=norm,
         **kwargs,
     )
     if under_color is not None:
```

### Comparing `rasterra-0.5.3/PKG-INFO` & `rasterra-0.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rasterra
-Version: 0.5.3
+Version: 0.5.5
 Summary: A sleek, object-oriented interface designed for intuitive raster data manipulation in Python.
 Home-page: https://collijk.github.io/rasterra
 License: BSD-3-Clause
 Author: James Collins
 Author-email: collijk1@gmail.com
 Requires-Python: >=3.10,<3.13
 Classifier: Development Status :: 4 - Beta
@@ -61,15 +61,14 @@
 
 ```sh
 pip install rasterra
 ```
 
 ## Usage
 
-
 ### File I/O
 
 Reading and writing raster data is done using the `load_raster` and `to_file` functions.
 
 ```python
 import rasterra as rt
```

