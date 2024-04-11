# Comparing `tmp/bipl-0.5.5.tar.gz` & `tmp/bipl-0.5.6.tar.gz`

## Comparing `bipl-0.5.5.tar` & `bipl-0.5.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 bipl-0.5.5/src/bipl/__init__.py
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 bipl-0.5.5/src/bipl/_env.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bipl-0.5.5/src/bipl/py.typed
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 bipl-0.5.5/src/bipl/io/__init__.py
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 bipl-0.5.5/src/bipl/io/_dzi.py
--rw-r--r--   0        0        0     3905 2020-02-02 00:00:00.000000 bipl-0.5.5/src/bipl/io/_gdal.py
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 bipl-0.5.5/src/bipl/io/_libs.py
--rw-r--r--   0        0        0     9567 2020-02-02 00:00:00.000000 bipl-0.5.5/src/bipl/io/_openslide.py
--rw-r--r--   0        0        0     9927 2020-02-02 00:00:00.000000 bipl-0.5.5/src/bipl/io/_slide.py
--rw-r--r--   0        0        0     6882 2020-02-02 00:00:00.000000 bipl-0.5.5/src/bipl/io/_slide_bases.py
--rw-r--r--   0        0        0    17549 2020-02-02 00:00:00.000000 bipl-0.5.5/src/bipl/io/_tiff.py
--rw-r--r--   0        0        0     5341 2020-02-02 00:00:00.000000 bipl-0.5.5/src/bipl/io/_util.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 bipl-0.5.5/src/bipl/ops/__init__.py
--rw-r--r--   0        0        0    13818 2020-02-02 00:00:00.000000 bipl-0.5.5/src/bipl/ops/_mosaic.py
--rw-r--r--   0        0        0     5455 2020-02-02 00:00:00.000000 bipl-0.5.5/src/bipl/ops/_tile.py
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 bipl-0.5.5/src/bipl/ops/_types.py
--rw-r--r--   0        0        0     5165 2020-02-02 00:00:00.000000 bipl-0.5.5/src/bipl/ops/_util.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 bipl-0.5.5/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 bipl-0.5.5/LICENSE
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 bipl-0.5.5/README.md
--rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 bipl-0.5.5/hatch_build.py
--rw-r--r--   0        0        0     5166 2020-02-02 00:00:00.000000 bipl-0.5.5/pyproject.toml
--rw-r--r--   0        0        0     5504 2020-02-02 00:00:00.000000 bipl-0.5.5/PKG-INFO
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 bipl-0.5.6/src/bipl/__init__.py
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 bipl-0.5.6/src/bipl/_env.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bipl-0.5.6/src/bipl/py.typed
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 bipl-0.5.6/src/bipl/io/__init__.py
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 bipl-0.5.6/src/bipl/io/_dzi.py
+-rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 bipl-0.5.6/src/bipl/io/_gdal.py
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 bipl-0.5.6/src/bipl/io/_libs.py
+-rw-r--r--   0        0        0     9570 2020-02-02 00:00:00.000000 bipl-0.5.6/src/bipl/io/_openslide.py
+-rw-r--r--   0        0        0     9637 2020-02-02 00:00:00.000000 bipl-0.5.6/src/bipl/io/_slide.py
+-rw-r--r--   0        0        0     7027 2020-02-02 00:00:00.000000 bipl-0.5.6/src/bipl/io/_slide_bases.py
+-rw-r--r--   0        0        0    18547 2020-02-02 00:00:00.000000 bipl-0.5.6/src/bipl/io/_tiff.py
+-rw-r--r--   0        0        0     5457 2020-02-02 00:00:00.000000 bipl-0.5.6/src/bipl/io/_util.py
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 bipl-0.5.6/src/bipl/ops/__init__.py
+-rw-r--r--   0        0        0    15085 2020-02-02 00:00:00.000000 bipl-0.5.6/src/bipl/ops/_mosaic.py
+-rw-r--r--   0        0        0     8556 2020-02-02 00:00:00.000000 bipl-0.5.6/src/bipl/ops/_tile.py
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 bipl-0.5.6/src/bipl/ops/_types.py
+-rw-r--r--   0        0        0     7259 2020-02-02 00:00:00.000000 bipl-0.5.6/src/bipl/ops/_util.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 bipl-0.5.6/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 bipl-0.5.6/LICENSE
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 bipl-0.5.6/README.md
+-rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 bipl-0.5.6/hatch_build.py
+-rw-r--r--   0        0        0     5166 2020-02-02 00:00:00.000000 bipl-0.5.6/pyproject.toml
+-rw-r--r--   0        0        0     5504 2020-02-02 00:00:00.000000 bipl-0.5.6/PKG-INFO
```

### Comparing `bipl-0.5.5/src/bipl/_env.py` & `bipl-0.5.6/src/bipl/_env.py`

 * *Files identical despite different names*

### Comparing `bipl-0.5.5/src/bipl/io/__init__.py` & `bipl-0.5.6/src/bipl/io/__init__.py`

 * *Files identical despite different names*

### Comparing `bipl-0.5.5/src/bipl/io/_dzi.py` & `bipl-0.5.6/src/bipl/io/_dzi.py`

 * *Files identical despite different names*

### Comparing `bipl-0.5.5/src/bipl/io/_gdal.py` & `bipl-0.5.6/src/bipl/io/_gdal.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 @dataclass(frozen=True)
 class _Level(ImageLevel):
     index: int
     g: 'Gdal'
     bands: tuple[gdal.Band, ...]
 
     def crop(self, *loc: slice) -> np.ndarray:
-        box, valid_box, shape = self._unpack_loc(*loc)
+        box, valid_box, shape = self._unpack_2d_loc(*loc)
 
         (y0, y1), (x0, x1) = valid_box.tolist()
         if y0 == y1 or x0 == x1:  # Patch is outside slide
             return np.broadcast_to(self.g.bg_color, (*shape, 3))
 
         h, w = y1 - y0, x1 - x0
         c = self.g.num_channels
```

### Comparing `bipl-0.5.5/src/bipl/io/_libs.py` & `bipl-0.5.6/src/bipl/io/_libs.py`

 * *Files identical despite different names*

### Comparing `bipl-0.5.5/src/bipl/io/_openslide.py` & `bipl-0.5.6/src/bipl/io/_openslide.py`

 * *Files 0% similar despite different names*

```diff
@@ -172,15 +172,15 @@
 @dataclass(frozen=True)
 class _Level(ImageLevel):
     downsample: int
     index: int
     osd: 'Openslide'
 
     def crop(self, *loc: slice) -> np.ndarray:
-        box, valid_box, shape = self._unpack_loc(*loc)
+        box, valid_box, shape = self._unpack_2d_loc(*loc)
 
         (y0, y1), (x0, x1) = valid_box
         if y0 == y1 or x0 == x1:  # Patch is outside slide
             return np.broadcast_to(self.osd.bg_color, (*shape, 3))
 
         bgra = np.empty((y1 - y0, x1 - x0, 4), dtype='u1')
         OSD.openslide_read_region(
```

### Comparing `bipl-0.5.5/src/bipl/io/_slide.py` & `bipl-0.5.6/src/bipl/io/_slide.py`

 * *Files 4% similar despite different names*

```diff
@@ -215,31 +215,24 @@
         """Use like `slide.pool(4)[y0:y1, x0:x1]` call"""
         d, lvl = self.best_level_for(downsample, tol=tol)
         if d == downsample:
             return lvl
         return lvl.rescale(d / downsample)
 
     def __getitem__(self, key: slice | tuple[slice, ...]) -> np.ndarray:
-        """Retrieves tile"""
-        # TODO: Ignore step, always redirect to self.levels[0].__getitem__
+        """Retrieve image patch from maximum resolution"""
         y_loc, x_loc, c_loc = normalize_loc(key, self.shape)
-
-        try:
-            step, = {y_loc.step, x_loc.step}
-        except ValueError:
-            raise ValueError('all slices should have the same step') from None
-        if step <= 0:
+        if y_loc.step <= 0 or x_loc.step <= 0:
             raise ValueError('slice steps should be positive')
 
-        ds, level = self.best_level_for(step)
-        yx_loc = *(slice(s.start // ds, s.stop // ds) for s in (y_loc, x_loc)),
-        image = level.crop(*yx_loc)
-
-        dsize = *(ceil((s.stop - s.start) / step) for s in (y_loc, x_loc)),
-        return resize(image, dsize)[:, :, c_loc]
+        r = self.levels[0].crop(
+            slice(y_loc.start, y_loc.stop),
+            slice(x_loc.start, x_loc.stop),
+        )
+        return r[::y_loc.step, ::x_loc.step, c_loc]
 
     @overload
     def at(self,
            z0_yx_offset: tuple[int, ...],
            dsize: int | tuple[int, ...],
            *,
            scale: float,
```

### Comparing `bipl-0.5.5/src/bipl/io/_slide_bases.py` & `bipl-0.5.6/src/bipl/io/_slide_bases.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,30 +56,30 @@
 
     def crop(self, *loc: slice) -> np.ndarray:
         """Reads crop of LOD. Overridable"""
         raise NotImplementedError
 
     @final
     def __getitem__(self, key: slice | tuple[slice, ...]) -> np.ndarray:
-        """Reads crop of LOD"""
+        """Retrieve sub-image as array from set location"""
         y_loc, x_loc, c_loc = normalize_loc(key, self.shape)
         if not y_loc.step == x_loc.step == 1:
             raise ValueError('Y/X slice steps should be 1 for now, '
                              f'got {y_loc.step} and {x_loc.step}')
         return self.crop(y_loc, x_loc)[:, :, c_loc]
 
     @final
     def numpy(self) -> np.ndarray:
-        """Reads whole image in single op"""
+        """Retrieve whole image as array"""
         return self[:, :]
 
     def rescale(self, scale: float) -> 'ImageLevel':
         """
-        Resize image to `src.size * scale`.
-        I.e. downscale if `scale < 1`, upscale otherwise.
+        Rescale image to set `scale`. Downscale if `scale` is less then 1,
+        upscale otherwise.
         """
         if scale == 1:
             return self
 
         base = self
         if isinstance(base, ProxyLevel):
             scale = base.scale * scale
@@ -91,37 +91,44 @@
         if scale > 0.5:  # Downscale to less then 2x, or upsample
             return ProxyLevel((h, w, c), mpp, scale, base)
 
         downsample = 2 ** (int(1 / scale).bit_length() - 1)
         r_tile = max(_MIN_TILE // downsample, 1)
         return TiledProxyLevel((h, w, c), mpp, scale, base, downsample, r_tile)
 
-    def _unpack_loc(
+    def _unpack_2d_loc(
         self,
         *slices: slice,
     ) -> tuple[np.ndarray, np.ndarray, list[int]]:
+        # box[axis, {start, stop}]
         box = np.array([(s.start, s.stop) for s in slices])
-        valid_box = box.T.clip([0, 0], self.shape[:2]).T  # (2, lo-hi)
-        shape = (box[:, 1] - box[:, 0]).tolist()
-        return box, valid_box, shape
+
+        # Slices guarantied to be within image shape
+        h, w = self.shape[:2]
+        valid_box = box.clip(0, [[h], [w]])
+
+        # Full output shape
+        out_shape = (box @ [-1, 1]).tolist()
+        return box, valid_box, out_shape
 
     def _expand(self, rgb: np.ndarray, valid_box: np.ndarray, box: np.ndarray,
                 bg_color: np.ndarray) -> np.ndarray:
         offsets = np.abs(valid_box - box)
         if offsets.any():
             tp, bm, lt, rt = offsets.ravel().tolist()
             rgb = cv2.copyMakeBorder(rgb, tp, bm, lt, rt, cv2.BORDER_CONSTANT,
                                      None, bg_color.tolist())
         return np.ascontiguousarray(rgb)
 
     @final
     def apply(  # type: ignore[override]
-            self,
-            fn: Callable[[np.ndarray], np.ndarray],
-            pad: int = 0) -> '_LambdaLevel':
+        self,
+        fn: Callable[[np.ndarray], np.ndarray],
+        pad: int = 0,
+    ) -> '_LambdaLevel':
         # _LambdaLevel is not subclass of _LambdaImage
         return _LambdaLevel(self.shape, self.mpp, self, fn, pad)
 
 
 @dataclass(frozen=True)
 class _LambdaImage(Image):
     base: Image
```

### Comparing `bipl-0.5.5/src/bipl/io/_tiff.py` & `bipl-0.5.6/src/bipl/io/_tiff.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,21 +15,23 @@
 from contextlib import contextmanager
 from ctypes import (POINTER, addressof, byref, c_char_p, c_float, c_int,
                     c_ubyte, c_uint16, c_uint32, c_uint64, c_void_p,
                     create_string_buffer, string_at)
 from dataclasses import dataclass, field
 from enum import Enum
 from functools import cached_property
+from itertools import product
 from threading import Lock
 from typing import NamedTuple, Protocol, TypeVar
 
 import cv2
 import imagecodecs
 import numpy as np
 from glow import sizeof
+from numpy.lib.stride_tricks import as_strided
 
 from bipl._env import env
 
 from ._libs import load_library
 from ._slide_bases import Driver, Image, ImageLevel
 from ._util import (Icc, is_aperio, parse_aperio_description, parse_xml,
                     unflatten)
@@ -289,71 +291,73 @@
     color: _ColorInfo
     bg_color: np.ndarray
     compression: _Compression
     jpt: bytes = field(repr=False)
     tile: tuple[int, ...]
     tile_sizes: np.ndarray = field(repr=False)
 
-    def _read_tile(self, y, x, ptr) -> SupportsArray:
-        offset = TIFF.TIFFComputeTile(ptr, x, y, 0, 0)
-        nbytes = int(self.tile_sizes[offset])
+    def _read_tile(self, iy, ix, ptr) -> SupportsArray:
+        nbytes = int(self.tile_sizes[iy, ix])
 
         if not nbytes:  # If nothing to read, don't read
             raise ValueError('File has corrupted tiles with zero size')
             # TODO: read from previous level
             # * If tile is empty on level N,
             # * then all tiles on levels >N are invalid, whether empty or not
             return np.broadcast_to(self.bg_color, self.tile)
 
+        offset = iy * self.tile_sizes.shape[1] + ix
+
         # if not self.compression.name.startswith('JPEG2000'):
         if self.compression not in {
                 _Compression.JPEG2000_RGB, _Compression.JPEG2000_YUV
         }:
             image = np.empty(self.tile, dtype='u1')
-            isok = TIFF.TIFFReadTile(ptr, c_void_p(image.ctypes.data), x, y, 0,
-                                     0)
+            isok = TIFF.TIFFReadEncodedTile(ptr, offset,
+                                            c_void_p(image.ctypes.data),
+                                            image.size)
             if isok == -1:
                 raise ValueError('TIFF tile read failed')
             return self.color.to_rgb(image)
 
         data = create_string_buffer(nbytes)
         TIFF.TIFFReadRawTile(ptr, offset, data, len(data))
 
         if self.jpt:
             return JpegArray(data, self.jpt, self.color.space.value)
         return CompressedArray(data)
 
-    def _get_tile(self, y: int, x: int, ptr, cache_ok: bool) -> SupportsArray:
+    def _get_tile(self, iy: int, ix: int, ptr, skip: bool) -> SupportsArray:
         # NOTE: like any op using TIFF pointer, this must be called under lock.
         # NOTE:
         # Like OpenSlide does we use private cache for each slide
         # with (level, y, x) key.
         # But:
         # - we store compressed data instead of pixel data to cache more tiles.
         # - we cache opened slides to not waste time on re-opening
         #   (that can lead to multiple caches existing at the same moment).
         # NOTE:
         # If tile becomes uncompressed we don't evict old compressed data.
         #   (but we should, that CAN LEAD TO HIGH MEMORY USAGE).
         # TODO: adjust cache size when tile is decoded.
         # TODO: cache pixel data
         tiff = self.tiff
-        key = (self.index, y, x)
+        key = (self.index, iy, ix)
         cache = tiff.cache
 
         # Cache hit, move to the end
         if (entry := cache.pop(key, None)) is not None:
             _, obj = cache[key] = entry
             return obj
 
         # Cache miss
-        obj = self._read_tile(y, x, ptr)
+        obj = self._read_tile(iy, ix, ptr)
 
         # Non-cacheable object or no cache at all
-        if not cache_ok or not (cache_cap := env.BIPL_TILE_CACHE):
+        if skip or not (cache_cap := env.BIPL_TILE_CACHE):
             return obj
         if (size := sizeof(obj)) > cache_cap:
             warnings.warn(
                 f'Rejecting overlarge cache entry of size {size} bytes',
                 stacklevel=3)
             return obj
 
@@ -361,102 +365,124 @@
         tiff.cache_size += size
         while tiff.cache_size > cache_cap:
             tiff.cache_size -= cache.pop(next(iter(cache)))[0]
         cache[key] = (size, obj)
         return obj
 
     def crop(self, *loc: slice) -> np.ndarray:
+        *tile, spp = self.tile
+
+        # (y/x lo/hi)
         box = np.array([(s.start, s.stop) for s in loc])
+        out_shape = np.r_[box[:, 1] - box[:, 0], spp]
 
-        *tile, spp = self.tile
-        dyx = box[:, 0]  # (2 lo-hi) -> (2)
-        out = np.ascontiguousarray(
-            np.broadcast_to(
-                self.bg_color,
-                np.r_[box[:, 1] - box[:, 0], spp],
-            ))
-
-        bmin, bmax = box.T.clip(0, self.shape[:2])
-
-        axes = *map(slice, bmin // tile, -(-bmax // tile)),
-        grid = np.mgrid[axes]  # (2 ih iw)
-        if not grid.size:
-            return out
+        if not out_shape.all():
+            return np.empty(out_shape, self.dtype)
+
+        bmin, bmax = box.T.clip(0, self.shape[:2])  # (y/x)
+        if (bmin == bmax).any():  # Crop is outside of image
+            return np.broadcast_to(self.bg_color, out_shape)
 
-        t_lo = grid.reshape(2, -1).T * tile  # (N 2)
+        iloc, masks, t_crops, o_crops, ((y0, y1), (x0, x1)) = zip(
+            *map(self._make_index, box[:, 0], bmin, bmax, tile))
+
+        with self.tiff.ifd(self.index) as ptr:
+            parts = self._get_n_tiles(iloc, masks, ptr)
+
+        out = np.empty(out_shape, self.dtype)
+        out[:y0] = self.bg_color
+        out[y0:y1, :x0] = self.bg_color
+        out[y0:y1, x1:] = self.bg_color
+        out[y1:] = self.bg_color
+
+        self._fill_result(out, parts, o_crops, t_crops)
+
+        return out
+
+    def _make_index(
+        self, min_: int, vmin: int, vmax: int, tile: int
+    ) -> tuple[np.ndarray, np.ndarray, np.ndarray, np.ndarray, np.ndarray]:
+        # (n + 1)
+        ids1 = np.arange(vmin // tile, 1 - (-vmax // tile))
+        n = ids1.size - 1
+        ts = ids1 * tile
+        vsep = ts.clip(vmin, vmax)
+
+        # (n lo/hi), source & target slices
+        u = vsep.itemsize
+        o_crops = as_strided(vsep - min_, (n, 2), (u, u))
+        t_crops = as_strided(vsep, (n, 2), (u, u)) - ts[:-1, None]
+
+        # (lo/hi), region of `out` to fill
+        o_span = o_crops[[0, -1], [0, 1]].tolist()
 
         # Cache only edges
         # Increases cache usage for linear reads (such as in `ops.Mosaic`)
-        _, ih, iw = grid.shape
-        is_edge = np.zeros(t_lo.shape[0], np.bool_)
-        is_edge[:iw] = True  # first row
-        is_edge[-iw:] = True  # last row
-        is_edge[0::iw] = True  # first col
-        is_edge[iw - 1::iw] = True  # last col
+        mask = np.zeros(n, np.bool_)
+        mask[1:-1] = True
 
-        with self.tiff.ifd(self.index) as ptr:
-            parts = [
-                self._get_tile(y, x, ptr, cache_ok)
-                for (y, x), cache_ok in zip(t_lo.tolist(), is_edge.tolist())
-            ]
-
-        # [N, lo-hi, yx]
-        crops = np.stack([t_lo, t_lo + tile], 1).clip(bmin, bmax)
-
-        # [N, yx, lo-hi]
-        o_crops = (crops - dyx).transpose(0, 2, 1)
-        t_crops = (crops - t_lo[:, None, :]).transpose(0, 2, 1)
-        for part, (oy, ox), (ty, tx) in zip(parts, o_crops, t_crops):
+        return ids1[:-1], mask, t_crops, o_crops, o_span
+
+    def _get_n_tiles(self, iloc, masks, ptr):
+        parts = [
+            self._get_tile(y, x, ptr, skip_cache)
+            for (y, x), skip_cache in zip(
+                product(*(ids.tolist() for ids in iloc)),
+                np.bitwise_and.outer(*masks).ravel().tolist(),
+            )
+        ]
+        return parts
+
+    def _fill_result(self, out, parts, o_crops, t_crops):
+        for part, (oy, ox), (ty, tx) in zip(parts, product(*o_crops),
+                                            product(*t_crops)):
             # NOTE: This call does decoding and caching of pixel data
             #       sequentially, but can be done in parallel.
             out[slice(*oy), slice(*ox)] = part[slice(*ty), slice(*tx)]
 
-        return out
-
 
 # FIXME: Get around slides from choked SVS encoder
 class Tiff(Driver):
     def __init__(self, path: str):
         # TODO: use memmap instead of libtiff
         self._ptr = (
             TIFF.TIFFOpenW(path, b'rm') if sys.platform == 'win32' else
             TIFF.TIFFOpen(path.encode(), b'rm'))
         if not self._ptr:
             raise ValueError(f'File {path} cannot be opened')
 
         weakref.finalize(self, TIFF.TIFFClose, self._ptr)
-
+        self._dir = 0
         self._lock = Lock()
         self.cache: dict[tuple, tuple[int, SupportsArray]] = {}
         self.cache_size = 0
 
     def __repr__(self) -> str:
         return f'{type(self).__name__}({addressof(self._ptr.contents):0x})'
 
     @contextmanager
     def ifd(self, index: int) -> Iterator:
         with self._lock:
-            TIFF.TIFFSetDirectory(self._ptr, index)
-            try:
-                yield self._ptr
-            finally:
-                TIFF.TIFFFreeDirectory(self._ptr, index)
+            if self._dir != index:
+                self._dir = index
+                TIFF.TIFFSetDirectory(self._ptr, index)
+            yield self._ptr
 
     def __len__(self) -> int:
         return TIFF.TIFFNumberOfDirectories(self._ptr)
 
     def _bg_color(self) -> np.ndarray:
         bg_hex = b'FFFFFF'
         bg_color_ptr = c_char_p()
         # TODO: find sample file to test this path. Never reached
         if TIFF.TIFFGetField(self._ptr, _Tag.BACKGROUND_COLOR,
                              byref(bg_color_ptr)):
             bg_hex = string_at(bg_color_ptr, 3)
             # TIFF._TIFFfree(bg_color_ptr)  # TODO: ensure no segfault
-        return np.frombuffer(bytes.fromhex(bg_hex.decode()), 'u1')
+        return np.frombuffer(bytes.fromhex(bg_hex.decode()), 'u1').copy()
 
     def _parse_description(self, desc: str,
                            make: str) -> tuple[str, list[str], dict[str, str]]:
         vendor = ''
         if is_aperio(desc):
             vendor = 'aperio'
             head, meta = parse_aperio_description(desc)
@@ -520,16 +546,16 @@
         tile = (*tags.tile_size, tags.spp)
         if len(tile) != 3:
             raise ValueError(f'Bad tile shape in TIFF: {tile}')
 
         tbc = np.empty([], 'u8')
         tbc_ptr = POINTER(c_uint64)()
         if TIFF.TIFFGetField(self._ptr, _Tag.TILE_BYTE_COUNTS, byref(tbc_ptr)):
-            num_tiles = TIFF.TIFFNumberOfTiles(self._ptr)
-            tbc = np.ctypeslib.as_array(tbc_ptr, [num_tiles]).copy()
+            num_tiles = *(len(range(0, s, t)) for s, t in zip(shape, tile)),
+            tbc = np.ctypeslib.as_array(tbc_ptr, num_tiles).copy()
             # TIFF._TIFFfree(tbc_ptr)  # TODO: ensure no segfault
             if (tbc == 0).any():
                 raise ValueError('Found 0s in tile size table')
 
         return _Level(shape, index, tags.icc, self, mpp, tags.color, bg_color,
                       tags.compression, jpt, tile, tbc)
```

### Comparing `bipl-0.5.5/src/bipl/io/_util.py` & `bipl-0.5.6/src/bipl/io/_util.py`

 * *Files 5% similar despite different names*

```diff
@@ -167,11 +167,17 @@
         return np.array(pil, copy=False)
 
 
 # -------------------------------- etc---------------------------------------
 
 
 def round2(x: float) -> int:
-    """Round to power to 2"""
+    """Round to power of 2"""
     assert x > 0
     power = round(log2(x))
     return 1 << power
+
+
+def floor2(x: float) -> int:
+    """Floor to power of 2"""
+    power = max(0, int(log2(x)))
+    return 1 << power
```

### Comparing `bipl-0.5.5/src/bipl/ops/_mosaic.py` & `bipl-0.5.6/src/bipl/ops/_mosaic.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-__all__ = ['Mosaic']
+__all__ = ['Mosaic', 'Patches', 'Tiles']
 
 import dataclasses
 from collections.abc import Callable, Iterable, Iterator, Sequence
 from contextlib import AbstractContextManager
 from dataclasses import dataclass
 from functools import partial
 from itertools import chain, starmap
 from math import ceil
-from typing import Literal, TypeVar, cast
+from typing import Literal
 
 import cv2
 import numpy as np
 import numpy.typing as npt
 from glow import chunked, map_n, starmap_n
 
-from ._tile import BlendCropper, Cropper, Decimator, Reconstructor, Zipper
-from ._types import NumpyLike, Tile, Vec
+from ._tile import BlendCropper, Decimator, Reconstructor, Stripper, Zipper
+from ._types import NDIndex, NumpyLike, Tile, Vec
 from ._util import get_trapz, padslice
 
 # TODO: allow result of .map/.map_batched to have different tile and step
 # NOTE: all classes here are stateless & their iterators are reentrant.
 
 # ---------------------------- utility functions -----------------------------
 
@@ -78,17 +78,15 @@
     @property
     def tile(self) -> int:
         return self.step + self.overlap
 
     def get_kernel(self) -> np.ndarray:
         return get_trapz(self.step, self.overlap)
 
-    def iterate(self,
-                image: NumpyLike,
-                max_workers: int = 1) -> '_TiledArrayView':
+    def iterate(self, image: NumpyLike, max_workers: int = 1) -> '_ArrayTiles':
         """Read tiles from input image"""
         # Source shape
         shape = image.shape[:2]
 
         # Index
         ih, iw = ishape = *((s + self.tile - 1) // self.step for s in shape),
         cells = np.ones(ishape, dtype=np.bool_)
@@ -100,82 +98,70 @@
         # All of (ih iw YX)
         # First tile is [origin: origin + tile]
         iyx = np.mgrid[:ih, :iw].transpose(1, 2, 0)
         yx0 = self.step * iyx + origin
         yx1 = self.tile + yx0
         locs = np.stack([yx0, yx1], -1)  # (ih iw YX lo-hi)
 
-        # TODO: read row by row - process rectangular tiles
-        # TODO: merge consecutive tiles from single row
-        return _TiledArrayView(self, shape, cells, locs, image, max_workers)
+        return _ArrayTiles(shape, self, cells, locs, image, max_workers)
 
 
-# --------------------------------- actions ----------------------------------
-
-_Self = TypeVar('_Self', bound='_BaseView')
+# ---------------------------------- pathes ----------------------------------
 
 
 @dataclass(frozen=True)
-class _BaseView:
-    m: Mosaic
+class Patches:
+    """Iterable of rectangular patches from non-uniform grid"""
     shape: Sequence[int]
-    cells: np.ndarray
-
-    @property
-    def ishape(self) -> Sequence[int]:
-        return self.cells.shape
 
     def __len__(self) -> int:
-        return int(self.cells.sum())
-
-    def report(self) -> dict[str, str]:
-        """Cells and area usage"""
-        used = int(self.cells.sum())
-        total = self.cells.size
-        coverage = (used / total) * (1 + self.m.overlap / self.m.step) ** 2
-        return {'cells': f'{used}/{total}', 'coverage': f'{coverage:.0%}'}
+        raise NotImplementedError
 
     def __iter__(self) -> Iterator[Tile]:
         raise NotImplementedError
 
-    def map(self: _Self,
+    def map(self,
             fn: Callable[[np.ndarray], np.ndarray],
             /,
-            max_workers: int = 0) -> _Self:
+            max_workers: int = 0) -> 'Patches':
         """
-        Applies function to each tile.
-        Note: change of tile shape besides channel count is forbidden.
-        Each tile is HWC-ordered ndarray.
+        Apply function to each patch.
+        Note: change of patch shape besides channel count is forbidden.
+        Each patch is HWC-ordered ndarray.
         Supports threading.
         """
-        tile_fn = partial(_apply, fn)
-        tiles = map_n(tile_fn, self, max_workers=max_workers)
-        return cast(
-            _Self,  # don't narrow type
-            _IterView(self.m, self.shape, self.cells, tiles),
-        )
+        patch_fn = partial(_apply, fn)
+        patches = map_n(patch_fn, self, max_workers=max_workers)
+        return _IterPatches(self.shape, patches, len(self))
 
-    def pool(self: _Self, stride: int = 1) -> _Self:
-        """Resizes each tile to desired stride"""
+    def pool(self, stride: int = 1) -> 'Patches':
+        """Resize each patch to desired stride"""
         if stride == 1:
             return self
-        if self.m.step % stride != 0 or self.m.overlap % stride != 0:
-            raise ValueError('stride should be a divisor of '
-                             f'{self.m.step}, {self.m.overlap}. Got: {stride}')
-
-        m = Mosaic(self.m.step // stride, self.m.overlap // stride)
         shape = *((s + stride - 1) // stride for s in self.shape),
-        return cast(  # don't narrow type
-            _Self,
-            _DecimatedView(m, shape, self.cells, stride, self),
-        )
+        return _IterPatches(shape, _Decimated(self, stride), len(self))
 
-    def crop(self) -> '_BaseView':
-        it = map(Cropper(self.shape), self)
-        return _IterView(self.m, self.shape, self.cells, it)
+    def transform(
+        self,
+        fn: Callable[[Iterable[Tile]], Iterable[Tile]],
+    ) -> 'Patches':
+        """
+        TODO: fill docs
+        """
+        patches = fn(self)
+        return _IterPatches(self.shape, patches, len(self))
+
+    def strip(self) -> 'Patches':
+        """Strip out-of-bounds regions. Produces non-square patches"""
+        it = map(Stripper(self.shape), self)
+        return _IterPatches(self.shape, it, len(self))
+
+    def crop(self) -> 'Patches':
+        # TODO: deprecate
+        return self.strip()
 
     def zip_with(
         self,
         view: NumpyLike,
         v_scale: float,
         interpolation: Literal[0, 1, 2, 3, 4] = 0,
     ) -> '_ZipView':
@@ -184,138 +170,203 @@
         Similar to RoIAlign used in some detectors.
 
         Interpolation is Nearest (0) by default, but Linear (1), Bicubic (2),
         Area (3) & Lanczos-4 (4) are also supported (OpenCV codes).
         """
         if v_scale <= 0:
             raise ValueError(f'v_scale should be positive, got: {v_scale}')
-        return _ZipView(self, view, v_scale, interpolation)
+        return _ZipView(self, len(self), view, v_scale, interpolation)
 
-    def with_cm(self: _Self, ctx: AbstractContextManager) -> _Self:
-        return cast(
-            _Self,
-            _ScopedView(self.m, self.shape, self.cells, self, ctx),
-        )
+    def with_(self, ctx: AbstractContextManager) -> 'Patches':
+        """Iterate with context. Reentrant if nested context is reentrant"""
+        return _IterPatches(self.shape, _Scoped(self, ctx), len(self))
 
 
 @dataclass(frozen=True)
 class _ZipView:
-    source: _BaseView
+    source: Iterable[Tile]
+    total: int
     view: NumpyLike
     v_scale: float
     interpolation: int
 
     def __len__(self) -> int:
-        return len(self.source)
+        return self.total
 
-    def __iter__(self) -> Iterator[tuple[Vec, Vec, np.ndarray, np.ndarray]]:
+    def __iter__(
+        self,
+    ) -> Iterator[tuple[NDIndex, Vec, np.ndarray, np.ndarray]]:
         return map(
             Zipper(self.view, self.v_scale, self.interpolation),
             self.source,
         )
 
 
 @dataclass(frozen=True)
-class _View(_BaseView):
+class _IterPatches(Patches):
+    source: Iterable[Tile]
+    total: int
+
+    def __len__(self) -> int:
+        return self.total
+
+    def __iter__(self) -> Iterator[Tile]:
+        return iter(self.source)
+
+
+# ---------------------------------- tiles -----------------------------------
+
+
+@dataclass(frozen=True)
+class Tiles(Patches):
+    """Iterable of (overlapping) square tiles from uniform grid"""
+    m: Mosaic
+    cells: npt.NDArray[np.bool_]
+
+    @property
+    def ishape(self) -> Sequence[int]:
+        return self.cells.shape
+
+    def __len__(self) -> int:
+        return int(self.cells.sum())
+
+    def report(self) -> dict[str, str]:
+        """Cells and area usage"""
+        used = int(self.cells.sum())
+        total = self.cells.size
+        coverage = (used / total) * (1 + self.m.overlap / self.m.step) ** 2
+        return {'cells': f'{used}/{total}', 'coverage': f'{coverage:.0%}'}
+
+    def map(self,
+            fn: Callable[[np.ndarray], np.ndarray],
+            /,
+            max_workers: int = 0) -> 'Tiles':
+        """
+        Apply function to each tile.
+        Note: change of tile shape besides channel count is forbidden.
+        Each tile is HWC-ordered ndarray.
+        Supports threading.
+        """
+        tile_fn = partial(_apply, fn)
+        tiles = map_n(tile_fn, self, max_workers=max_workers)
+        return _IterTiles(self.shape, self.m, self.cells, tiles)
+
     def map_batched(self,
                     fn: Callable[[list[np.ndarray]], Iterable[np.ndarray]],
                     /,
                     batch_size: int = 1,
-                    max_workers: int = 0) -> '_View':
+                    max_workers: int = 0) -> 'Tiles':
         """
-        Applies function to batches of tiles.
+        Apply function to batches of tiles.
         Note: change of tile shape besides channel count is forbidden.
         Each tile is HWC-ordered ndarray.
         Supports threading.
         """
         tile_fn = partial(_apply_batched, fn)
 
         chunks = chunked(self, batch_size)
         batches = map_n(tile_fn, chunks, max_workers=max_workers)
         tiles = chain.from_iterable(batches)
 
-        return _IterView(self.m, self.shape, self.cells, tiles)
+        return _IterTiles(self.shape, self.m, self.cells, tiles)
 
-    def transform(self, fn: Callable[[Iterable[Tile]],
-                                     Iterable[Tile]]) -> '_View':
-        """
-        TODO: fill docs
-        """
-        tiles = fn(self)
-        return _IterView(self.m, self.shape, self.cells, tiles)
+    def pool(self, stride: int = 1) -> 'Tiles':
+        """Resize each tile to desired stride"""
+        if stride == 1:
+            return self
+        if self.m.step % stride != 0 or self.m.overlap % stride != 0:
+            raise ValueError('stride should be a divisor of '
+                             f'{self.m.step}, {self.m.overlap}. Got: {stride}')
+
+        m = Mosaic(self.m.step // stride, self.m.overlap // stride)
+        shape = *((s + stride - 1) // stride for s in self.shape),
+        return _IterTiles(shape, m, self.cells, _Decimated(self, stride))
 
-    def reweight(self) -> '_View':
+    def with_(self, ctx: AbstractContextManager) -> 'Tiles':
+        """Iterate with context. Reentrant if nested context is reentrant"""
+        return _IterTiles(self.shape, self.m, self.cells, _Scoped(self, ctx))
+
+    def reweight(self) -> 'Tiles':
         """
-        Applies weight to tile edges to prepare them for summation
+        Apply weight to tile edges to prepare them for summation
         if overlap exists.
         Note: no need to call this method if you have already applied it.
         """
-        if not self.m.overlap:  # No need
+        if not self.m.overlap:  # No-op
             return self
-
         weight = self.m.get_kernel()
         tile_fn = partial(_reweight, weight)
         return self.map(tile_fn)
 
-    def merge(self) -> _BaseView:
+    def merge(self) -> Patches:
         """
-        Removes overlapping regions from all the tiles if any.
+        Remove overlapping regions from all the tiles if any.
         Tiles should be reweighted if overlap exists.
         """
-        if self.m.overlap:
-            return _BlendCropsView(self.m, self.shape, self.cells, self)
-        return self
+        if not self.m.overlap:  # No-op
+            return self
+        bcr = BlendCropper(self.cells, self.m.overlap, self.m.step)
+        return _IterPatches(self.shape, _Merged(self, bcr), bcr.size)
 
 
 @dataclass(frozen=True)
-class _IterView(_View):
+class _IterTiles(Tiles):
     source: Iterable[Tile]
 
     def __iter__(self) -> Iterator[Tile]:
         return iter(self.source)
 
 
-@dataclass(frozen=True)
-class _ScopedView(_BaseView):
+@dataclass(frozen=True, slots=True)
+class _Scoped:
     source: Iterable[Tile]
     _ctx: AbstractContextManager
 
     def __iter__(self) -> Iterator[Tile]:
-        """Iterator over tiles. Reentrant if nested context is reentrant"""
         with self._ctx:
             yield from self.source
 
 
-@dataclass(frozen=True)
-class _DecimatedView(_View):
+@dataclass(frozen=True, slots=True)
+class _Decimated:
     """
     Decimates tiles.
     Doesn't change size uniformity.
     Yields decimated views of original tiles.
     """
-    stride: int
     source: Iterable[Tile]
+    stride: int
 
     def __iter__(self) -> Iterator[Tile]:
         return map(Decimator(self.stride), self.source)
 
 
-@dataclass(frozen=True)
-class _TiledArrayView(_View):
+@dataclass(frozen=True, slots=True)
+class _Merged:
     """
-    Extracts tiles from array.
-    Yields same-sized tiles with overlaps.
+    Sums overlapping regions.
+    Returns non-uniform patches without overlaps.
     """
+    source: Iterable[Tile]
+    bcr: BlendCropper
+
+    def __iter__(self) -> Iterator[Tile]:
+        return self.bcr(self.source)
+
+
+@dataclass(frozen=True)
+class _ArrayTiles(Tiles):
+    """Extracts square tiles from array with overlaps."""
     locs: npt.NDArray[np.int64]  # (ih iw YX lo-hi)
     data: NumpyLike
     max_workers: int
 
     def select(self,
                mask: np.ndarray,
-               scale: float | None = None) -> '_TiledArrayView':
+               scale: float | None = None) -> '_ArrayTiles':
         """
         Subset non-masked (i.e. non-zeros in mask) tiles for iteration.
         Mask size is "scale"-multiple of source image.
 
         NOTE: `select(mask1).select(mask2)` is equal to `select(mask1 & mask2)`
         """
         if mask.ndim == 3:  # Strip extra dim
@@ -338,31 +389,33 @@
                 for s0, s1 in zip(mask.shape, view)),
         mask = padslice(mask, *loc)
 
         cells = cv2.resize(mask, (iw, ih), interpolation=cv2.INTER_AREA)
 
         return dataclasses.replace(self, cells=self.cells & cells.astype(bool))
 
-    def _get_tile(self, idx: Vec, *loc: slice) -> Tile:
+    def _get_tile(self, idx: NDIndex, *loc: slice) -> Tile:
         """Do `data[loc]`. Result could be cropped."""
         vec = *(s.start for s in loc),
         return Tile(idx=idx, vec=vec, data=self.data[loc])
 
-    def _get_tile_padded(self, idx: Vec, *loc: slice) -> Tile:
+    def _get_tile_padded(self, idx: NDIndex, *loc: slice) -> Tile:
         """Do `data[loc]` padding data in necessary."""
         vec = *(s.start for s in loc),
         return Tile(idx=idx, vec=vec, data=padslice(self.data, *loc))
 
-    def _ilocs(self,
-               locs: npt.NDArray[np.int64]) -> list[tuple[Vec, slice, slice]]:
-        """Precompute tile coordinates: index & Y/X-slices"""
-        idx = np.argwhere(self.cells).tolist()
-        boxes = locs[self.cells].tolist()
-        return [(tuple(i), slice(*ys), slice(*xs))
-                for i, (ys, xs) in zip(idx, boxes)]
+    def _ilocs(
+        self,
+        locs: npt.NDArray[np.int64],
+    ) -> list[tuple[NDIndex, slice, slice]]:
+        """Precompute tile coordinates: 2D index & Y/X-slices"""
+        iys, ixs = self.cells.nonzero()
+        boxes = locs[iys, ixs].tolist()
+        return [(i, slice(*ys), slice(*xs))
+                for i, (ys, xs) in zip(zip(iys.tolist(), ixs.tolist()), boxes)]
 
     def _drop_overlaps(self,
                        grid: npt.NDArray[np.int64]) -> npt.NDArray[np.int64]:
         grid = grid.copy()  # (ih iw YX lo-hi)
 
         # Cut top edge (y0) from tiles having neighbor from above (iy)
         grid[1:, :, 0, 0][self.cells[:-1, :]] += self.m.overlap
@@ -389,26 +442,11 @@
             return iter(parts)
 
         rcr = Reconstructor(self.m.overlap, self.cells)
         return map(rcr, parts)
 
     def get_tile(self, idx: int) -> Tile:
         """Get full tile by its flattened index"""
-        i = *np.argwhere(self.cells)[idx].tolist(),
+        iys, ixs = self.cells.nonzero()
+        i = int(iys[idx]), int(ixs[idx])
         ys, xs = self.locs[i].tolist()
         return self._get_tile_padded(i, slice(*ys), slice(*xs))
-
-
-@dataclass(frozen=True)
-class _BlendCropsView(_BaseView):
-    """
-    Applies weighted average over overlapping regions.
-    Yields tiles without overlaps, so their size can differ.
-
-    NOTE: can output 0-sized tiles.
-    """
-    source: Iterable[Tile]
-
-    def __iter__(self) -> Iterator[Tile]:
-        assert self.m.overlap
-        bcr = BlendCropper(self.m.step, self.m.overlap, self.cells)
-        return map(bcr, self.source)
```

### Comparing `bipl-0.5.5/src/bipl/ops/_util.py` & `bipl-0.5.6/src/bipl/ops/_util.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 __all__ = [
     'crop_to', 'get_fusion', 'get_trapz', 'normalize_loc',
     'probs_to_rgb_heatmap', 'resize'
 ]
 
 from collections.abc import Iterable, Sequence
 from itertools import zip_longest
+from math import ceil, floor
 
 import cv2
 import numpy as np
 
 from bipl import env
 
 from ._types import NumpyLike, Tile, Vec
@@ -44,15 +45,15 @@
         raise ValueError('not applicable for overlap 0')
     pad = np.linspace(0, 1, overlap + 2)[1:-1]  # strip initial 0 and final 1
     return np.r_[pad, np.ones(step - overlap), pad[::-1]].astype('f4')
 
 
 def normalize_loc(loc: Sequence[slice] | slice,
                   shape: Sequence[int]) -> tuple[slice, ...]:
-    """Ensures slices match ndim and have not none endpoints"""
+    """Ensures slices match ndim and have noo `None` endpoints"""
     if isinstance(loc, slice):
         loc = loc,
     ndim = len(shape)
     if len(loc) > ndim:
         raise ValueError(f'loc is too deep for {ndim}D, got: {loc}')
     it = (slice(
         s.start or 0,
@@ -64,20 +65,31 @@
 
 def padslice(a: NumpyLike, *loc: slice) -> np.ndarray:
     """
     Do `a[loc]`, but extend `a` (with 0s) if `loc` indices beyond `a.shape`.
     """
     loc = normalize_loc(loc, a.shape)
 
-    pos_loc = *(slice(max(0, s.start), max(0, s.stop)) for s in loc),
-    a = a[pos_loc]
-
-    pad = [(pos.start - raw.start, pos.stop - pos.start - size)
-           for raw, pos, size in zip(loc, pos_loc, a.shape)]
-    return np.pad(a, pad) if np.any(pad) else a
+    # No need to pad
+    if all(0 <= s.start <= s.stop <= size for s, size in zip(loc, a.shape)):
+        return a[loc]
+
+    iloc = *(slice(np.clip(s.start, 0, size), np.clip(s.stop, 0, size))
+             for s, size in zip(loc, a.shape)),
+    rloc = *(slice(i.start - s.start, i.stop - s.start)
+             for s, i in zip(loc, iloc)),
+
+    r = np.empty([s.stop - s.start for s in loc], a.dtype)
+    pad = ()
+    for o in rloc:
+        r[*pad, :o.start] = 0
+        r[*pad, o.stop:] = 0
+        pad += o,
+    r[rloc] = a[iloc]
+    return r
 
 
 def crop_to(vec: Vec, a: NumpyLike,
             shape: Sequence[int]) -> tuple[Vec, np.ndarray]:
     """
     Crop `a` to be completely within shape, i.e.
     `0 <= vec[i] <= vec[i] + a.shape[i] <= shape[i]`.
@@ -154,7 +166,60 @@
         if r is None:  # First iteration, initialize
             r = np.zeros((*shape, c), a.dtype)
         if c != r.shape[2]:
             raise RuntimeError('tile channel counts changed during iteration')
         r[y:y + h, x:x + w] = a
 
     return r
+
+
+def rescale_crop(a: NumpyLike,
+                 *loc: slice,
+                 scale: float = 1,
+                 interpolation: int = 0):
+    """
+    Rescale image, then crop with respect to subpixels.
+
+    Interpolation is Nearest (0) by default, but Linear (1), Bicubic (2),
+    Area (3) & Lanczos-4 (4) are also supported (OpenCV codes).
+
+    Effectively is same as:
+    ```
+    (y0, y1), (x0, x1) = ys * scale, xs * scale
+    h, w = ys[1] - ys[0], xs[1] - xs[0]
+    return cv2.resize(a[y0: y1, x0: x1], (w, h), interpolation=interpolation)
+    ```
+    """
+    assert 0 <= interpolation <= 4
+    if scale == 1:
+        return padslice(a, *loc)
+
+    box = np.array([[s.start, s.stop] for s in loc], 'i4')  # (y/x, start/stop)
+    h, w = (box[:, 1] - box[:, 0]).tolist()
+    if not h or not w:  # 0-size output
+        return np.empty((h, w, *a.shape[2:]), a.dtype)
+
+    lo_f, hi_f = np.multiply(box, scale, dtype='f4').T
+
+    # Extra margin to accomodate interpolation kernel
+    # 2x2 (0 extra) - nearest (0), bilinear (1), area (3)
+    # 4x4 (1 extra) - bicubic (2)
+    # 8x8 (3 extra) - lanczos4 (4)
+    eps = (0, 0, 1, 0, 3)[interpolation]
+
+    # Tight slice to have all necessary pixels
+    loc = tuple(
+        slice(*np.clip([floor(lo_) - eps, ceil(hi_) + eps], 0, size))
+        for lo_, hi_, size in zip(lo_f, hi_f, a.shape))
+    r = a[loc]
+    if not r.size:  # 0-size tight slice
+        return np.zeros((h, w, *a.shape[2:]), a.dtype)
+
+    # Resample image crop to destination grid
+    dy, dx = (lo_ - s.start + (scale - 1) / 2 for lo_, s in zip(lo_f, loc))
+    return cv2.warpAffine(
+        r,
+        np.array([[scale, 0, dx], [0, scale, dy]], 'f4'),
+        (w, h),
+        flags=interpolation | cv2.WARP_INVERSE_MAP,
+        borderMode=cv2.BORDER_CONSTANT,
+    )
```

### Comparing `bipl-0.5.5/LICENSE` & `bipl-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `bipl-0.5.5/README.md` & `bipl-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `bipl-0.5.5/hatch_build.py` & `bipl-0.5.6/hatch_build.py`

 * *Files identical despite different names*

### Comparing `bipl-0.5.5/pyproject.toml` & `bipl-0.5.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 [tool.hatch.build.targets.wheel]
 artifacts = ["*.dll"]  # only wheel keeps DLLs
 
 [tool.hatch.build.hooks.custom]  # enable "custom" hook
 
 [project]
 name = "bipl"
-version = "0.5.5"
+version = "0.5.6"
 description = "Openslide/libtiff/GDAL ndarray-like interface and lazy parallel tile-based processing"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {file = "LICENSE"}
 keywords = [
     "medical", "images", "pathology", "whole-slide", "wsi", "pyramid", "slide",
     "libtiff", "openslide", "osgeo", "gdal",  # backends
```

### Comparing `bipl-0.5.5/PKG-INFO` & `bipl-0.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: bipl
-Version: 0.5.5
+Version: 0.5.6
 Summary: Openslide/libtiff/GDAL ndarray-like interface and lazy parallel tile-based processing
 Project-URL: homepage, https://github.com/arquolo/bipl
 Project-URL: repository, https://github.com
 Author-email: Paul Maevskikh <arquolo@gmail.com>
 Maintainer-email: Paul Maevskikh <arquolo@gmail.com>
 License: MIT License
```

