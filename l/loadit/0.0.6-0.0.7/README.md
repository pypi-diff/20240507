# Comparing `tmp/loadit-0.0.6.tar.gz` & `tmp/loadit-0.0.7.tar.gz`

## Comparing `loadit-0.0.6.tar` & `loadit-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 loadit-0.0.6/config.toml
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 loadit-0.0.6/scc_setup.sh
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 loadit-0.0.6/src/loadit/__about__.py
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 loadit-0.0.6/src/loadit/__init__.py
--rw-r--r--   0        0        0     4136 2020-02-02 00:00:00.000000 loadit-0.0.6/src/loadit/cache_base.py
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 loadit-0.0.6/src/loadit/dict_cache.py
--rw-r--r--   0        0        0     7203 2020-02-02 00:00:00.000000 loadit-0.0.6/src/loadit/loadit.py
--rw-r--r--   0        0        0    12060 2020-02-02 00:00:00.000000 loadit-0.0.6/src/loadit/sharded_dataset.py
--rw-r--r--   0        0        0     6155 2020-02-02 00:00:00.000000 loadit-0.0.6/src/loadit/util.py
--rw-r--r--   0        0        0     7422 2020-02-02 00:00:00.000000 loadit-0.0.6/src/loadit/writer.py
--rw-r--r--   0        0        0    13524 2020-02-02 00:00:00.000000 loadit-0.0.6/tests/test_iteration.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 loadit-0.0.6/.gitignore
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 loadit-0.0.6/LICENSE.txt
--rw-r--r--   0        0        0     9449 2020-02-02 00:00:00.000000 loadit-0.0.6/README.md
--rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 loadit-0.0.6/pyproject.toml
--rw-r--r--   0        0        0    10613 2020-02-02 00:00:00.000000 loadit-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 loadit-0.0.7/config.toml
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 loadit-0.0.7/scc_setup.sh
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 loadit-0.0.7/src/loadit/__about__.py
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 loadit-0.0.7/src/loadit/__init__.py
+-rw-r--r--   0        0        0     4136 2020-02-02 00:00:00.000000 loadit-0.0.7/src/loadit/cache_base.py
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 loadit-0.0.7/src/loadit/dict_cache.py
+-rw-r--r--   0        0        0     7650 2020-02-02 00:00:00.000000 loadit-0.0.7/src/loadit/loadit.py
+-rw-r--r--   0        0        0    12210 2020-02-02 00:00:00.000000 loadit-0.0.7/src/loadit/sharded_dataset.py
+-rw-r--r--   0        0        0     6589 2020-02-02 00:00:00.000000 loadit-0.0.7/src/loadit/util.py
+-rw-r--r--   0        0        0     7371 2020-02-02 00:00:00.000000 loadit-0.0.7/src/loadit/writer.py
+-rw-r--r--   0        0        0    14605 2020-02-02 00:00:00.000000 loadit-0.0.7/tests/test_iteration.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 loadit-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 loadit-0.0.7/LICENSE.txt
+-rw-r--r--   0        0        0    10069 2020-02-02 00:00:00.000000 loadit-0.0.7/README.md
+-rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 loadit-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0    11233 2020-02-02 00:00:00.000000 loadit-0.0.7/PKG-INFO
```

### Comparing `loadit-0.0.6/src/loadit/cache_base.py` & `loadit-0.0.7/src/loadit/cache_base.py`

 * *Files identical despite different names*

### Comparing `loadit-0.0.6/src/loadit/dict_cache.py` & `loadit-0.0.7/src/loadit/dict_cache.py`

 * *Files identical despite different names*

### Comparing `loadit-0.0.6/src/loadit/loadit.py` & `loadit-0.0.7/src/loadit/loadit.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from .writer import WriterPool
 from .util import size_estimator, SequenceView, is_sequence
 from typing import Any, Union, Optional, Iterable, Callable, List
 from pathlib import Path
 from concurrent.futures import ThreadPoolExecutor
 import time
 import re
+from .util import _get_iter
 from collections.abc import Sequence
 
 import logging
 
 logger = logging.getLogger("loadit")
 
 PreloadType = Callable[[Any, int], List[int]]
@@ -58,67 +59,78 @@
 
         return self.loader.get(self.indices[idx], preload_fn=self.preload_fn)
 
 
 class LoadIt(SequenceView):
     def __init__(
         self,
-        create_it: Optional[Callable[None, Iterable]],
-        root_dir: Union[str, Path] = "cache/",
+        root_dir: Union[str, Path],
+        create_iter: Optional[Callable[None, Iterable]] = None,
         max_shard_length: Optional[Union[str, int]] = "64mb",
         max_cache_size: int = 128,
-        max_workers: int = 3,
+        max_workers: int = 1,
         memory_limit: Optional[int] = None,
         compression: Optional[str] = None,
         preload_fn: Optional[PreloadType] = preload_next_shard,
-        preload_all_async=False,
-        info=None,
+        preload_all_async: bool=False,
+        info: Any=None,
+        iterator_thread_safe: bool=False,
+        length: Optional[int]=None,
     ):
-        if create_it is None:
+        if create_iter is None:
             max_shard_length = None
 
+        if not iterator_thread_safe and max_workers != 1:
+            raise ValueError(f'If you want to use max_workers>1, you must set iterator_thread_safe=True (requested max_workers={max_workers})')
+
+        self.manual_length = length
+
+
         if isinstance(max_shard_length, str):
             match = re.fullmatch("([0-9]+)mb", max_shard_length.lower())
             if not match:
                 raise ValueError(
                     "Invalid max_shard_length! Must be an integer or match ([0-9]+)mb."
                 )
             length_mb = float(match.group(1))
 
             metadata = dataset_metadata(root_dir)
             if metadata is None:
                 max_shard_length = int(
                     length_mb
                     * (2**20)
-                    / size_estimator(create_it(), compression=compression)
+                    / size_estimator(_get_iter(create_iter), compression=compression)
                 )
             else:
                 max_shard_length = metadata.max_shard_length
                 logger.warn(
                     "User-specified max_shard_length in mb for an already-existing ShardedDataset! Ignoring user specification"
                 )
 
-        if create_it is not None:
+        if create_iter is not None:
             self.writer_pool = WriterPool(
-                create_it=create_it,
-                num_workers=max_workers,
+                create_iter=create_iter,
+                num_workers=max_workers
             )
             shard_load_fn = self.writer_pool.load_fn
         else:
             self.writer_pool = None
             shard_load_fn = None
 
         self.shards = ShardedDataset(
             max_size_bytes=memory_limit,
             root_dir=root_dir,
             max_shard_length=max_shard_length,
             load_fn=shard_load_fn,
             compression=compression,
             info=info,
         )
+        if create_iter is None:
+            self.shards.stop_observer()
+
         self.max_workers = max_workers
         if self.max_workers > 1:
             self.executor = ThreadPoolExecutor(max_workers=self.max_workers - 1)
         else:
             self.executor = None
 
         def load_from_disk(d, k):
```

### Comparing `loadit-0.0.6/src/loadit/sharded_dataset.py` & `loadit-0.0.7/src/loadit/sharded_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,14 +143,22 @@
         self.handler = TimestampHandler(self, [self.pattern])
         self.observer.schedule(self.handler, path=self.shard_dir, recursive=False)
         self.observer.start()
 
         self.initialize_timestamps()
         super().__init__(max_size_bytes, load_fn)
 
+    def stop_observer(self):
+        self.observer.stop()
+        self.observer.join()
+        
+
+    def __del__(self):
+        self.stop_observer()
+
     def initialize_timestamps(self):
         with self.writer_file_lock:
             all_shard_info = self.get_all_shards()
             for info in all_shard_info:
                 if info not in self.timestamps:
                     self.timestamps[info.start] = time.time()
```

### Comparing `loadit-0.0.6/src/loadit/util.py` & `loadit-0.0.7/src/loadit/util.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,28 +7,38 @@
 from itertools import chain
 from collections import deque
 from collections.abc import Sequence
 import numpy as np
 import json
 
 
+def _get_iter(create_it):
+    if hasattr(create_it, "__iter__"):
+        return create_it.__iter__()
+    else:
+        return create_it()
+
+
 def is_sequence(s):
     seq_attrs = ["__getitem__", "__len__", "__iter__"]
     for at in seq_attrs:
         if not hasattr(s, at):
             return False
     return True
 
 
 def size_estimator(it: Iterable, num_samples: int = 16, compression=None) -> int:
     buffer = []
     for count, x in enumerate(it):
         buffer.append(x)
         if count == num_samples - 1:
             break
+    if count == 0:
+        raise ValueError("iterable provided to LoadIt is empty!")
+
     fd, name = tempfile.mkstemp()
     with fsspec.open(name, mode="wb", compression=compression) as f:
         pickle.dump(buffer, f)
     os.close(fd)
     size = os.path.getsize(name)
     os.unlink(name)
     return size / count
@@ -173,28 +183,34 @@
             return self.seq[idx]
 
     def __len__(self):
         return len(self.seq)
 
 
 def chunk_shuffle_idx(chunk_size: int, length: int, seed: Optional = None):
-    num_chunks = (chunk_size + length - 1) // chunk_size
+    num_chunks = length // chunk_size
 
     rng = np.random.default_rng(seed)
+    last_chunk_size = length - num_chunks * chunk_size
+    if last_chunk_size > 0:
+        last_chunk = [num_chunks * chunk_size + rng.permutation(last_chunk_size)]
+    else:
+        last_chunk = []
 
     permutations = np.concatenate(
         [i * chunk_size + rng.permutation(chunk_size) for i in range(num_chunks)]
+        + last_chunk
     )
     return permutations
 
 
 def chunk_shuffle(
     seq: Sequence,
     chunk_size: Optional[int],
-    length: Optional[int],
+    length: Optional[int] = None,
     seed: Optional = None,
 ):
     if length is None:
         length = len(seq)
 
     if chunk_size is None:
         chunk_size = len(seq)
```

### Comparing `loadit-0.0.6/src/loadit/writer.py` & `loadit-0.0.7/src/loadit/writer.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,26 +5,26 @@
 
 logger = logging.getLogger("loadit")
 
 
 class Writer:
     def __init__(
         self,
-        create_it: Optional[Union[Iterable, Callable[None, Iterable]]] = None,
+        create_iter: Optional[Union[Iterable, Callable[None, Iterable]]] = None,
     ):
         assert is_iterator_creator(
-            create_it
+            create_iter
         ), "you must supply a function that creates iterables!"
-        self.it = enumerate(create_it())
+        self.it = enumerate(create_iter())
         self.current_idx = -1
         self.finished = False
-        self.create_it = create_it
+        self.create_iter = create_iter
 
     def reset_iterator(self):
-        self.it = enumerate(self.create_it())
+        self.it = enumerate(self.create_iter())
 
         self.finished = False
         self.current_idx = -1
 
     def iterate_and_write_shard(
         self, start_idx: int, shards: ShardedDataset
     ) -> List[Any]:
@@ -86,17 +86,17 @@
     try:
         it = enumerate(it)
         return True
     except TypeError:
         return False
 
 
-def is_iterator_creator(create_it: Any) -> bool:
+def is_iterator_creator(create_iter: Any) -> bool:
     try:
-        return is_iterator(create_it())
+        return is_iterator(create_iter())
     except TypeError:
         return False
 
 
 class QueueItem:
     def __init__(self, start_idx: int, writer: Writer):
         self.start_idx = start_idx
@@ -106,28 +106,27 @@
         self.finished = False
 
 
 class WriterPool:
     def __init__(
         self,
         writers: Optional[List[Writer]] = None,
-        create_it: Optional[Callable[None, Iterable]] = None,
+        create_iter: Optional[Callable[None, Iterable]] = None,
         num_workers: int = 1,
     ):
-        assert exactly_one_not_none(writers, create_it)
+        assert exactly_one_not_none(writers, create_iter)
         if writers is not None:
             self.writers = writers
-        if create_it is not None:
-            self.writers = [Writer(create_it=create_it) for _ in range(num_workers)]
+        if create_iter is not None:
+            self.writers = [Writer(create_iter=create_iter) for _ in range(num_workers)]
         self.queue_lock = Lock()
         # self.queue_cv = Condition()
         self.queues = {writer: [] for writer in self.writers}
 
     def add_to_queue(self, start_idx: int, shards: ShardedDataset) -> Optional[Writer]:
-        # returns None if the selected writer does not need to be scheduled.
         writer_to_append = None
         smallest_gap = float("inf")
         with self.queue_lock:
             for writer in self.writers:
                 queue = self.queues[writer]
                 if len(queue) == 0:
                     # this writer's current_idx is correct
```

### Comparing `loadit-0.0.6/tests/test_iteration.py` & `loadit-0.0.7/tests/test_iteration.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from concurrent.futures import ThreadPoolExecutor
 
 
 def get_array(n):
     return (np.reshape(np.arange(0, (n + 1) * 10000, n + 1), (100, 100)),)
 
 
-def create_it(N: int = 100000, delay=0):
+def create_iter(N: int = 100000, delay=0):
     for n in range(N):
         result = {
             "array": get_array(n),
             "label": f"item_{n}",
             "index": n,
         }
         if delay > 0:
@@ -65,53 +65,69 @@
 def memory_limit(request, max_shard_length):
     if request.param is None:
         return None
     return request.param * max_shard_length * one_item_memory_size()
 
 
 def one_item_memory_size():
-    it = create_it(N=10)
+    it = create_iter(N=10)
     minishard = list(it)
     s = pickle.dumps(minishard)
     return len(s) / 10
 
 
 @pytest.fixture
+def small_cache_loader_multiwrite(tmp_path):
+    loader = loadit.LoadIt(
+        create_iter=lambda: create_iter(),
+        root_dir=tmp_path,
+        max_shard_length=16,
+        max_cache_size=10,
+        max_workers=5,
+        iterator_thread_safe=True,
+        memory_limit=20 * 16 * one_item_memory_size(),
+    )
+    return loader
+
+@pytest.fixture
 def small_cache_loader(tmp_path):
     loader = loadit.LoadIt(
-        create_it=lambda: create_it(),
+        create_iter=lambda: create_iter(),
         root_dir=tmp_path,
         max_shard_length=16,
         max_cache_size=10,
         max_workers=5,
+        iterator_thread_safe=True,
         memory_limit=20 * 16 * one_item_memory_size(),
     )
     return loader
 
 
 def nowriter_loader(tmp_path):
     loader = loadit.LoadIt(
-        create_it=None,
+        create_iter=None,
         root_dir=tmp_path,
         max_shard_length=16,
         max_cache_size=5,
         max_workers=10,
+        iterator_thread_safe=True,
         memory_limit=None,
     )
     return loader
 
 
 @pytest.fixture
 def full_save_loader(tmp_path):
     loader = loadit.LoadIt(
-        create_it=lambda: create_it(N=16 * 100),
+        create_iter=lambda: create_iter(N=16 * 100),
         root_dir=tmp_path,
         max_shard_length=16,
         max_cache_size=5,
         max_workers=10,
+        iterator_thread_safe=True,
         memory_limit=None,
     )
     return loader
 
 
 @pytest.fixture
 def loader(
@@ -119,79 +135,83 @@
     it_size,
     delay,
     max_shard_length,
     max_cache_size,
     memory_limit,
     max_workers,
 ):
-    create_it_fn = lambda: create_it(it_size, delay)
+    create_iter_fn = lambda: create_iter(it_size, delay)
     loader = loadit.LoadIt(
-        create_it=create_it_fn,
+        create_iter=create_iter_fn,
         root_dir=tmp_path,
         max_shard_length=max_shard_length,
         max_cache_size=max_cache_size,
         memory_limit=memory_limit,
         max_workers=max_workers,
+        iterator_thread_safe=max_workers > 1,
     )
 
     yield loader
 
     loader.shards.observer.unschedule_all()
     loader.shards.observer.stop()
     loader.shards.observer.join()
 
 
 def test_shard_size_mb(tmp_path):
-    create_it = lambda: [np.arange(i, i + 128) for i in range(2024)]
+    create_iter = lambda: [np.arange(i, i + 128) for i in range(2024)]
     loader = loadit.LoadIt(
-        create_it=create_it,
+        create_iter=create_iter,
         root_dir=tmp_path,
         max_shard_length="1mb",
         max_cache_size=5,
         max_workers=10,
+        iterator_thread_safe=True,
         memory_limit=None,
     )
 
     for x in loader:
         pass
 
     cached_loader = loadit.LoadIt(
-        create_it=None,
+        create_iter=None,
         root_dir=tmp_path,
         max_shard_length=None,
         max_cache_size=5,
         max_workers=10,
+        iterator_thread_safe=True,
         memory_limit=None,
     )
     for i, x in enumerate(loader):
         assert np.array_equal(np.arange(i, i + 128), x)
 
     assert len(loader.shards.get_all_shards()) == 3
 
     for p in sorted(loader.shards.get_all_shards(), key=lambda p: p.start)[:-1]:
         assert p.size <= 2**20
         assert p.size >= 0.9 * 2**20
 
 
 def test_parallel_loaders(tmp_path, delay):
-    create_it_fn = lambda: create_it(2000, delay)
+    create_iter_fn = lambda: create_iter(2000, delay)
 
-    def make_loader(create_it_fn):
+    def make_loader(create_iter_fn):
         loader = loadit.LoadIt(
-            create_it=create_it_fn,
+            create_iter=create_iter_fn,
             root_dir=tmp_path,
             max_shard_length=16,
             max_cache_size=32,
             memory_limit=None,
             max_workers=10,
+            iterator_thread_safe=True,
         )
         return loader
 
     def iterate():
-        l = make_loader(create_it_fn)
+        l = make_loader(create_iter_fn)
         for i, x in enumerate(l):
             validate_data(x, i)
         l.shards.observer.unschedule_all()
         l.shards.observer.stop()
         l.shards.observer.join()
         return 0
 
@@ -210,19 +230,20 @@
         if i == 100:
             break
     assert i == min(100, it_size - 1)
 
 
 def test_loader_can_compress(tmp_path):
     loader = loadit.LoadIt(
-        create_it=lambda: create_it(N=1000),
+        create_iter=lambda: create_iter(N=1000),
         root_dir=tmp_path,
         max_shard_length=100,
         max_cache_size=5,
         max_workers=10,
+        iterator_thread_safe=True,
         memory_limit=None,
         preload_all_async=True,
         compression="zstd",
     )
     for i, x in enumerate(loader):
         validate_data(x, i)
         if i == 100:
@@ -234,19 +255,20 @@
         assert False, "should not be able to load a compressed file..."
     except pickle.PickleError:
         pass
 
 
 def test_preload_when_infinite_memory(tmp_path):
     loader = loadit.LoadIt(
-        create_it=lambda: create_it(N=1000),
+        create_iter=lambda: create_iter(N=1000),
         root_dir=tmp_path,
         max_shard_length=100,
         max_cache_size=5,
         max_workers=10,
+        iterator_thread_safe=True,
         memory_limit=None,
         preload_all_async=True,
     )
 
     assert not loader.all_cached_to_disk()
 
     loader.wait_until_all_cached()
@@ -323,26 +345,26 @@
         x = full_save_loader[i]
     full_save_loader.finalize()
 
     new_loader = nowriter_loader(tmp_path)
     assert len(new_loader) == 16
 
 
-def test_uses_multiple_writers(small_cache_loader):
-    loader = small_cache_loader
+def test_uses_multiple_writers(small_cache_loader_multiwrite):
+    loader = small_cache_loader_multiwrite
     loader.preload_fn = None
-    x = small_cache_loader[11 * loader.shards.max_shard_length]
+    x = loader[11 * loader.shards.max_shard_length]
 
     assert (
         loader.writer_pool.writers[0].current_idx
         == 12 * loader.shards.max_shard_length - 1
     )
     assert loader.writer_pool.writers[1].current_idx == -1
 
-    x = small_cache_loader[loader.shards.max_shard_length]
+    x = loader[loader.shards.max_shard_length]
 
     assert (
         loader.writer_pool.writers[0].current_idx
         == 12 * loader.shards.max_shard_length - 1
     )
     assert (
         loader.writer_pool.writers[1].current_idx
@@ -385,29 +407,31 @@
     validate_data(concat[it_size + 1], 4)
     validate_data(concat[it_size  + 2 + 2], 2)
 
 
 def test_shuffle(loader, it_size):
     chunk_size = 70
     shuffled = loadit.chunk_shuffle(loader, chunk_size=chunk_size, length=it_size)
+    assert len(shuffled) == len(loader)
     seen_indices = set()
     for i, x in enumerate(shuffled):
         idx = x["index"]
         assert idx not in seen_indices
         assert idx // chunk_size == i // chunk_size
         seen_indices.add(idx)
 
 
 def test_repeat(tmp_path):
     loader1 = loadit.LoadIt(
-        create_it=lambda: create_it(N=100),
+        create_iter=lambda: create_iter(N=100),
         root_dir=os.path.join(tmp_path, "l1"),
         max_shard_length=100,
         max_cache_size=5,
         max_workers=10,
+        iterator_thread_safe=True,
         memory_limit=None,
     )
 
     repeat3 = loadit.RepeatSequence(loader1, 3)
     assert repeat3[130]["index"] == 30
     assert repeat3[299]["index"] == 99
 
@@ -415,51 +439,56 @@
         _ = repeat3[300]
     except IndexError:
         pass
 
 
 def test_interleave(tmp_path):
     loader1 = loadit.LoadIt(
-        create_it=lambda: create_it(N=100),
+        create_iter=lambda: create_iter(N=100),
         root_dir=os.path.join(tmp_path, "l1"),
         max_shard_length=100,
         max_cache_size=5,
         max_workers=10,
+        iterator_thread_safe=True,
         memory_limit=None,
     )
     loader2 = loadit.LoadIt(
-        create_it=lambda: create_it(N=10),
+        create_iter=lambda: create_iter(N=10),
         root_dir=os.path.join(tmp_path, "l2"),
         max_shard_length=100,
         max_cache_size=5,
         max_workers=10,
+        iterator_thread_safe=True,
         memory_limit=None,
     )
     loader3 = loadit.LoadIt(
-        create_it=lambda: create_it(N=100),
+        create_iter=lambda: create_iter(N=100),
         root_dir=os.path.join(tmp_path, "l3"),
         max_shard_length=100,
         max_cache_size=5,
         max_workers=10,
+        iterator_thread_safe=True,
         memory_limit=None,
     )
     loader4 = loadit.LoadIt(
-        create_it=lambda: create_it(N=10),
+        create_iter=lambda: create_iter(N=10),
         root_dir=os.path.join(tmp_path, "l4"),
         max_shard_length=100,
         max_cache_size=5,
         max_workers=10,
+        iterator_thread_safe=True,
         memory_limit=None,
     )
     loader5 = loadit.LoadIt(
-        create_it=lambda: create_it(N=22),
+        create_iter=lambda: create_iter(N=22),
         root_dir=os.path.join(tmp_path, "l5"),
         max_shard_length=100,
         max_cache_size=5,
         max_workers=10,
+        iterator_thread_safe=True,
         memory_limit=None,
     )
 
     interleave = loadit.InterleaveSequences(
         *[
             loader1,
             loader2,
@@ -488,27 +517,29 @@
         idx = idx % len(test_lists)
 
         assert x["index"] == check_value
 
 
 def test_info(tmp_path):
     loader1 = loadit.LoadIt(
-        create_it=lambda: create_it(N=300),
+        create_iter=lambda: create_iter(N=300),
         root_dir=tmp_path,
         max_shard_length=100,
         max_cache_size=5,
         max_workers=3,
+        iterator_thread_safe=True,
         memory_limit=None,
         info={"hello": "there"},
     )
     loader2 = loadit.LoadIt(
-        create_it=None,
+        create_iter=None,
         root_dir=tmp_path,
         max_shard_length=None,
         max_workers=3,
+        iterator_thread_safe=True,
         memory_limit=None,
     )
 
     info2 = loader2.info()
 
     assert len(info2) == 1
     assert info2["hello"] == "there"
```

### Comparing `loadit-0.0.6/LICENSE.txt` & `loadit-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `loadit-0.0.6/README.md` & `loadit-0.0.7/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -124,15 +124,15 @@
 
 repeat = loadit.RepeatSequence(a, repeats=3)
 # like itertools.repeat. repeats=None will repeat infinitely
 
 shuffled = chunk_shuffle(seq, chunk_size=128, length=1024)
 # bins indices into groups of 128 and returns a view of the
 # first 1024 elements of seq that is shuffled within each bin.
-# if chunk_size of length is unspecified, they default to len(seq).
+# if chunk_size or length is unspecified, they default to len(seq).
 ```
 
 ### Features
 * Aims to provide the same user-interface as `loader = list(my_iterator)`.
 * Allows for iterators that do not fit in memory by caching iterations in the file system.
 * Previously cached data can be re-used: if the entire iterator can be cached, then you only need the cache.
 * If we don't have the disk space to cache all iterations, we'll automatically regenerate iterations on-demand.
@@ -150,41 +150,47 @@
 ### Detailed Options
 
 The `LoadIt` initialization signature is:
 ```python
 class LoadIt
     def __init__(
         self,
-        create_it: Optional[Callable[None, Iterable]],
         root_dir: Union[str, Path],
-        max_shard_length: Union[str,int] = "64mb",
+        create_iter: Optional[Callable[None, Iterable]] = None,
+        max_shard_length: Optional[Union[str, int]] = "64mb",
         max_cache_size: int = 128,
-        max_workers: int = 3,
+        max_workers: int = 1,
         memory_limit: Optional[int] = None,
         compression: Optional[str] = None,
-        preload_fn: Optional[Callable[[Self, int], Iterable[List[int]]]] = preload_next_shard,
-        preload_all_async: False,
+        preload_fn: Optional[PreloadType] = preload_next_shard,
+        preload_all_async: bool=False,
+        info: Any=None,
+        iterator_thread_safe: bool=False,
+        length: Optional[int]=None,
     ):
 ```
 The arguments are:
-* `create_it`: this is a function that takes no arguments and returns a new iterable (that is, it is possible to do `for x in create_it():`). If `create_it` is `None`, then we cannot load new iterates from scratch. However, if all of the data has already been cached on disk at `root_dir`, then things will still work fine - we don't need the iterator anymore.
 * `root_dir`: this is where we will stash iterations on the file system. If you instantiate a new `LoadIt` instance
-with the same `root_dir`, then either `create_it` should return the same iterator, or you can set `create_it` to `None`
+with the same `root_dir`, then either `create_iter` should return the same iterator, or you can set `create_iter` to `None`
 and simply use the cached data directly.
+* `create_iter`: this is a function that takes no arguments and returns a new iterable (that is, it is possible to do `for x in create_iter():`). If `create_iter` is `None`, then we cannot load new iterates from scratch. However, if all of the data has already been cached on disk at `root_dir`, then things will still work fine - we don't need the iterator anymore.
 * `max_shard_length`: Each file (a "shard") stored in the `root_dir` directory will contain at most this many iterations.
 You can also specify a string ending in `mb`, such as `32mb`. This will automatically set the length so that the size of the shards will be approximately the given number of megabytes.
 Note that this approximation is based on the size of the first 128 iterations, and so may be poor if there is high variation in iteration size.
 * `max_cache_size`: We will keep at most this shards in main memory (i.e. loaded in from disk) at once.
-* `max_workers`: This is the number of worker threads that will be spawned to write shards. CAUTION: if `max_workers` is >1, then the function `create_it` must be safe to run in multiple threads.
+* `max_workers`: This is the number of worker threads that will be spawned to write shards. CAUTION: if `max_workers` is >1, then the function `create_iter` must be safe to run in multiple threads. This must be explicitly acknowledged by setting `iterator_thread_safe` to `True`.
 * `memory_limit`: The total size of all shard files stored on disk in `root_dir` will be at most this many bytes.
 * `compression`: You can provide an optional string representing a compression format to use when caching data on disk. Compression uses `fsspec`, so anything in `fsspec.available_compressions()` is valid.
 * `preload_fn`: This function will be called every time you request an iterate to schedule pre-fetching of further iterates. By default it 
 fetches the next `max_workers/2` shards. Iterating over `preload_fn(loader, idx)` should yield lists of indices. For each list, a seperate thread
 will go in order over the list and make sure that each index is in memory.
 * `preload_all_async`: if True, then we will iterate through the iterator in the background and cache all iterations to disk. If False, then we will only iterate to cache iterations that are actually requested (plus a few speculative extra iterations specified by `preload_fn`).
+* `info`: optional metadata that will be stored with the cached data. Can be accessed with the `.info`  attribute.
+* `iterator_thread_safe`: a flag that indicates that it is safe to spawn multiple copies of the iterator with `create_iter` in different threads. If this is `False`, then setting `max_workers` greater than 1 will raise an error.
+* `length`: a optional manual specification  of the length of the iterator, if known.
 
 
 
 ## Storage format
 
 The goal of the storage format is to store the data to disk in a way that:
 * is very simple.
```

### Comparing `loadit-0.0.6/pyproject.toml` & `loadit-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `loadit-0.0.6/PKG-INFO` & `loadit-0.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: loadit
-Version: 0.0.6
+Version: 0.0.7
 Summary: Easily convert iterables over large datasets into random access.
 Project-URL: Documentation, https://github.com/acutkosky/loadit#readme
 Project-URL: Issues, https://github.com/acutkosky/loadit/issues
 Project-URL: Source, https://github.com/acutkosky/loadit
 Author-email: Ashok Cutkosky <ashok@cutkosky.com>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -152,15 +152,15 @@
 
 repeat = loadit.RepeatSequence(a, repeats=3)
 # like itertools.repeat. repeats=None will repeat infinitely
 
 shuffled = chunk_shuffle(seq, chunk_size=128, length=1024)
 # bins indices into groups of 128 and returns a view of the
 # first 1024 elements of seq that is shuffled within each bin.
-# if chunk_size of length is unspecified, they default to len(seq).
+# if chunk_size or length is unspecified, they default to len(seq).
 ```
 
 ### Features
 * Aims to provide the same user-interface as `loader = list(my_iterator)`.
 * Allows for iterators that do not fit in memory by caching iterations in the file system.
 * Previously cached data can be re-used: if the entire iterator can be cached, then you only need the cache.
 * If we don't have the disk space to cache all iterations, we'll automatically regenerate iterations on-demand.
@@ -178,41 +178,47 @@
 ### Detailed Options
 
 The `LoadIt` initialization signature is:
 ```python
 class LoadIt
     def __init__(
         self,
-        create_it: Optional[Callable[None, Iterable]],
         root_dir: Union[str, Path],
-        max_shard_length: Union[str,int] = "64mb",
+        create_iter: Optional[Callable[None, Iterable]] = None,
+        max_shard_length: Optional[Union[str, int]] = "64mb",
         max_cache_size: int = 128,
-        max_workers: int = 3,
+        max_workers: int = 1,
         memory_limit: Optional[int] = None,
         compression: Optional[str] = None,
-        preload_fn: Optional[Callable[[Self, int], Iterable[List[int]]]] = preload_next_shard,
-        preload_all_async: False,
+        preload_fn: Optional[PreloadType] = preload_next_shard,
+        preload_all_async: bool=False,
+        info: Any=None,
+        iterator_thread_safe: bool=False,
+        length: Optional[int]=None,
     ):
 ```
 The arguments are:
-* `create_it`: this is a function that takes no arguments and returns a new iterable (that is, it is possible to do `for x in create_it():`). If `create_it` is `None`, then we cannot load new iterates from scratch. However, if all of the data has already been cached on disk at `root_dir`, then things will still work fine - we don't need the iterator anymore.
 * `root_dir`: this is where we will stash iterations on the file system. If you instantiate a new `LoadIt` instance
-with the same `root_dir`, then either `create_it` should return the same iterator, or you can set `create_it` to `None`
+with the same `root_dir`, then either `create_iter` should return the same iterator, or you can set `create_iter` to `None`
 and simply use the cached data directly.
+* `create_iter`: this is a function that takes no arguments and returns a new iterable (that is, it is possible to do `for x in create_iter():`). If `create_iter` is `None`, then we cannot load new iterates from scratch. However, if all of the data has already been cached on disk at `root_dir`, then things will still work fine - we don't need the iterator anymore.
 * `max_shard_length`: Each file (a "shard") stored in the `root_dir` directory will contain at most this many iterations.
 You can also specify a string ending in `mb`, such as `32mb`. This will automatically set the length so that the size of the shards will be approximately the given number of megabytes.
 Note that this approximation is based on the size of the first 128 iterations, and so may be poor if there is high variation in iteration size.
 * `max_cache_size`: We will keep at most this shards in main memory (i.e. loaded in from disk) at once.
-* `max_workers`: This is the number of worker threads that will be spawned to write shards. CAUTION: if `max_workers` is >1, then the function `create_it` must be safe to run in multiple threads.
+* `max_workers`: This is the number of worker threads that will be spawned to write shards. CAUTION: if `max_workers` is >1, then the function `create_iter` must be safe to run in multiple threads. This must be explicitly acknowledged by setting `iterator_thread_safe` to `True`.
 * `memory_limit`: The total size of all shard files stored on disk in `root_dir` will be at most this many bytes.
 * `compression`: You can provide an optional string representing a compression format to use when caching data on disk. Compression uses `fsspec`, so anything in `fsspec.available_compressions()` is valid.
 * `preload_fn`: This function will be called every time you request an iterate to schedule pre-fetching of further iterates. By default it 
 fetches the next `max_workers/2` shards. Iterating over `preload_fn(loader, idx)` should yield lists of indices. For each list, a seperate thread
 will go in order over the list and make sure that each index is in memory.
 * `preload_all_async`: if True, then we will iterate through the iterator in the background and cache all iterations to disk. If False, then we will only iterate to cache iterations that are actually requested (plus a few speculative extra iterations specified by `preload_fn`).
+* `info`: optional metadata that will be stored with the cached data. Can be accessed with the `.info`  attribute.
+* `iterator_thread_safe`: a flag that indicates that it is safe to spawn multiple copies of the iterator with `create_iter` in different threads. If this is `False`, then setting `max_workers` greater than 1 will raise an error.
+* `length`: a optional manual specification  of the length of the iterator, if known.
 
 
 
 ## Storage format
 
 The goal of the storage format is to store the data to disk in a way that:
 * is very simple.
```

