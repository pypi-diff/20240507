# Comparing `tmp/torch.redstone-0.0.5-py3-none-any.whl.zip` & `tmp/torch.redstone-0.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,22 @@
-Zip file size: 18894 bytes, number of entries: 19
--rw-rw-rw-  2.0 fat       30 b- defN 22-Sep-28 06:59 torch/redstone/__init__.py
--rw-rw-rw-  2.0 fat      257 b- defN 23-Feb-12 11:07 torch_redstone/__init__.py
--rw-rw-rw-  2.0 fat     2231 b- defN 23-Feb-12 12:21 torch_redstone/hooking.py
--rw-rw-rw-  2.0 fat     8841 b- defN 23-Feb-23 10:14 torch_redstone/lib.py
--rw-rw-rw-  2.0 fat     4904 b- defN 23-Feb-27 07:50 torch_redstone/log.py
--rw-rw-rw-  2.0 fat     8590 b- defN 23-Feb-25 06:19 torch_redstone/loop.py
--rw-rw-rw-  2.0 fat      382 b- defN 22-Aug-03 07:29 torch_redstone/loss.py
--rw-rw-rw-  2.0 fat      354 b- defN 23-Mar-01 03:39 torch_redstone/metric.py
--rw-rw-rw-  2.0 fat     2065 b- defN 23-Feb-25 06:19 torch_redstone/polyfill.py
--rw-rw-rw-  2.0 fat      875 b- defN 23-Feb-23 10:07 torch_redstone/processor.py
--rw-rw-rw-  2.0 fat      428 b- defN 22-Aug-02 11:27 torch_redstone/task.py
--rw-rw-rw-  2.0 fat      312 b- defN 22-Aug-03 07:31 torch_redstone/types.py
--rw-rw-rw-  2.0 fat     5872 b- defN 23-Feb-25 06:17 torch_redstone/utils.py
--rw-rw-rw-  2.0 fat       23 b- defN 23-Mar-01 11:28 torch_redstone/version.py
--rw-rw-rw-  2.0 fat    11538 b- defN 23-Mar-01 11:28 torch.redstone-0.0.5.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1417 b- defN 23-Mar-01 11:28 torch.redstone-0.0.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Mar-01 11:28 torch.redstone-0.0.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       21 b- defN 23-Mar-01 11:28 torch.redstone-0.0.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1543 b- defN 23-Mar-01 11:28 torch.redstone-0.0.5.dist-info/RECORD
-19 files, 49775 bytes uncompressed, 16374 bytes compressed:  67.1%
+Zip file size: 21136 bytes, number of entries: 20
+-rw-r--r--  2.0 unx       29 b- defN 24-May-07 17:19 torch/redstone/__init__.py
+-rw-r--r--  2.0 unx      241 b- defN 24-May-07 17:19 torch_redstone/__init__.py
+-rw-r--r--  2.0 unx     6755 b- defN 24-May-07 17:19 torch_redstone/dtr.py
+-rw-r--r--  2.0 unx     2150 b- defN 24-May-07 17:19 torch_redstone/hooking.py
+-rw-r--r--  2.0 unx     9157 b- defN 24-May-07 17:19 torch_redstone/lib.py
+-rw-r--r--  2.0 unx     4776 b- defN 24-May-07 17:19 torch_redstone/log.py
+-rw-r--r--  2.0 unx     8854 b- defN 24-May-07 17:19 torch_redstone/loop.py
+-rw-r--r--  2.0 unx      367 b- defN 24-May-07 17:19 torch_redstone/loss.py
+-rw-r--r--  2.0 unx      338 b- defN 24-May-07 17:19 torch_redstone/metric.py
+-rw-r--r--  2.0 unx     2004 b- defN 24-May-07 17:19 torch_redstone/polyfill.py
+-rw-r--r--  2.0 unx      938 b- defN 24-May-07 17:19 torch_redstone/processor.py
+-rw-r--r--  2.0 unx      413 b- defN 24-May-07 17:19 torch_redstone/task.py
+-rw-r--r--  2.0 unx      295 b- defN 24-May-07 17:19 torch_redstone/types.py
+-rw-r--r--  2.0 unx     6082 b- defN 24-May-07 17:19 torch_redstone/utils.py
+-rw-r--r--  2.0 unx       22 b- defN 24-May-07 17:19 torch_redstone/version.py
+-rw-r--r--  2.0 unx    11337 b- defN 24-May-07 17:19 torch.redstone-0.0.6.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1395 b- defN 24-May-07 17:19 torch.redstone-0.0.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-07 17:19 torch.redstone-0.0.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       21 b- defN 24-May-07 17:19 torch.redstone-0.0.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1621 b- defN 24-May-07 17:19 torch.redstone-0.0.6.dist-info/RECORD
+20 files, 56887 bytes uncompressed, 18498 bytes compressed:  67.5%
```

## zipnote {}

```diff
@@ -1,13 +1,16 @@
 Filename: torch/redstone/__init__.py
 Comment: 
 
 Filename: torch_redstone/__init__.py
 Comment: 
 
+Filename: torch_redstone/dtr.py
+Comment: 
+
 Filename: torch_redstone/hooking.py
 Comment: 
 
 Filename: torch_redstone/lib.py
 Comment: 
 
 Filename: torch_redstone/log.py
@@ -36,23 +39,23 @@
 
 Filename: torch_redstone/utils.py
 Comment: 
 
 Filename: torch_redstone/version.py
 Comment: 
 
-Filename: torch.redstone-0.0.5.dist-info/LICENSE
+Filename: torch.redstone-0.0.6.dist-info/LICENSE
 Comment: 
 
-Filename: torch.redstone-0.0.5.dist-info/METADATA
+Filename: torch.redstone-0.0.6.dist-info/METADATA
 Comment: 
 
-Filename: torch.redstone-0.0.5.dist-info/WHEEL
+Filename: torch.redstone-0.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: torch.redstone-0.0.5.dist-info/top_level.txt
+Filename: torch.redstone-0.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: torch.redstone-0.0.5.dist-info/RECORD
+Filename: torch.redstone-0.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## torch/redstone/__init__.py

 * *Ordering differences only*

```diff
@@ -1 +1 @@
-from torch_redstone import *
+from torch_redstone import *
```

## torch_redstone/__init__.py

 * *Ordering differences only*

```diff
@@ -1,16 +1,16 @@
-from .utils import *
-from .hooking import *
-
-from .task import *
-from .metric import *
-from .loss import *
-
-from .processor import *
-
-from .log import *
-from .loop import *
-
-from .polyfill import *
-from .lib import *
-
-from .version import *
+from .utils import *
+from .hooking import *
+
+from .task import *
+from .metric import *
+from .loss import *
+
+from .processor import *
+
+from .log import *
+from .loop import *
+
+from .polyfill import *
+from .lib import *
+
+from .version import *
```

## torch_redstone/hooking.py

 * *Ordering differences only*

```diff
@@ -1,81 +1,81 @@
-import contextlib
-import torch.nn as nn
-from typing import Optional
-from torch.utils.hooks import RemovableHandle
-
-
-class StopExecution(Exception):
-    pass
-
-
-class RedstoneDisposeHandle(object):
-    def __init__(self) -> None:
-        self.handle: Optional[RemovableHandle] = None
-
-    def dispose(self):
-        if self.handle is not None:
-            self.handle.remove()
-            self.handle = None
-
-
-class RedstoneCatchHook(RedstoneDisposeHandle):
-    def __init__(self, count, raise_on_record) -> None:
-        super().__init__()
-        self.record = []
-        self.count = count
-        self.raise_on_record = raise_on_record
-
-    def get_all(self):
-        try:
-            return self.record
-        finally:
-            self.record.clear()
-
-    def get(self):
-        return self.record.pop(0)
-
-    def __del__(self):
-        self.dispose()
-
-    def add(self, x):
-        if self.count and len(self.record) >= self.count:
-            raise ValueError("`catch_input` got more catches than `check_catch_count`", self.count)
-        self.record.append(x)
-        if self.raise_on_record:
-            raise StopExecution(x)
-
-
-class RedstoneCatchInput(RedstoneCatchHook):
-
-    def __call__(self, module, inputs):
-        if len(inputs) == 1:
-            inputs = inputs[0]
-        self.add(inputs)
-
-
-class RedstoneCatchOutput(RedstoneCatchHook):
-
-    def __call__(self, module, inputs, output):
-        self.add(output)
-
-
-def catch_input_to(module: nn.Module, check_catch_count: Optional[int] = 1):
-    rci = RedstoneCatchInput(check_catch_count, False)
-    rci.handle = module.register_forward_pre_hook(rci)
-    return rci
-
-
-def catch_output_from(module: nn.Module, check_catch_count: Optional[int] = 1, raise_stop_execution: bool = False):
-    rco = RedstoneCatchOutput(check_catch_count, raise_stop_execution)
-    rco.handle = module.register_forward_hook(rco)
-    return rco
-
-
-def modify_input_to(module: nn.Module, apply_func):
-    rc = RedstoneDisposeHandle()
-    rc.handle = module.register_forward_pre_hook(lambda mod, inputs: apply_func(*inputs))
-    return rc
-
-
-def catching_scope():
-    return contextlib.suppress(StopExecution)
+import contextlib
+import torch.nn as nn
+from typing import Optional
+from torch.utils.hooks import RemovableHandle
+
+
+class StopExecution(Exception):
+    pass
+
+
+class RedstoneDisposeHandle(object):
+    def __init__(self) -> None:
+        self.handle: Optional[RemovableHandle] = None
+
+    def dispose(self):
+        if self.handle is not None:
+            self.handle.remove()
+            self.handle = None
+
+
+class RedstoneCatchHook(RedstoneDisposeHandle):
+    def __init__(self, count, raise_on_record) -> None:
+        super().__init__()
+        self.record = []
+        self.count = count
+        self.raise_on_record = raise_on_record
+
+    def get_all(self):
+        try:
+            return self.record
+        finally:
+            self.record.clear()
+
+    def get(self):
+        return self.record.pop(0)
+
+    def __del__(self):
+        self.dispose()
+
+    def add(self, x):
+        if self.count and len(self.record) >= self.count:
+            raise ValueError("`catch_input` got more catches than `check_catch_count`", self.count)
+        self.record.append(x)
+        if self.raise_on_record:
+            raise StopExecution(x)
+
+
+class RedstoneCatchInput(RedstoneCatchHook):
+
+    def __call__(self, module, inputs):
+        if len(inputs) == 1:
+            inputs = inputs[0]
+        self.add(inputs)
+
+
+class RedstoneCatchOutput(RedstoneCatchHook):
+
+    def __call__(self, module, inputs, output):
+        self.add(output)
+
+
+def catch_input_to(module: nn.Module, check_catch_count: Optional[int] = 1):
+    rci = RedstoneCatchInput(check_catch_count, False)
+    rci.handle = module.register_forward_pre_hook(rci)
+    return rci
+
+
+def catch_output_from(module: nn.Module, check_catch_count: Optional[int] = 1, raise_stop_execution: bool = False):
+    rco = RedstoneCatchOutput(check_catch_count, raise_stop_execution)
+    rco.handle = module.register_forward_hook(rco)
+    return rco
+
+
+def modify_input_to(module: nn.Module, apply_func):
+    rc = RedstoneDisposeHandle()
+    rc.handle = module.register_forward_pre_hook(lambda mod, inputs: apply_func(*inputs))
+    return rc
+
+
+def catching_scope():
+    return contextlib.suppress(StopExecution)
```

## torch_redstone/lib.py

```diff
@@ -1,254 +1,271 @@
-from typing import List, Sequence, Union, Callable, Any, Optional
-from typing_extensions import Literal
-import torch
-import torch.autograd.functional as ad
-import torch.nn as nn
-import torch.nn.functional as F
-from torch import Tensor
-
-from .processor import Processor, Adapter
-from .loss import Loss
-from .metric import Metric
-from .utils import container_catamorphism, AttrPath, visit_attr, ObjectProxy
-
-
-AttrPathType = Union[AttrPath, str, Callable[[Any], Tensor], None]
-
-
-class Index:
-    def __init__(self, idx: int) -> None:
-        self.idx = idx
-
-    def __index__(self):
-        return self.idx
-
-
-class AdvTrainingPGD(Processor):
-    def __init__(
-        self, loss_metric: Metric,
-        no_perturb_attrs: List[AttrPathType]=[],
-        eps=0.03, step_scale=0.5, n_steps=8, attack_at_test=False
-    ) -> None:
-        """
-        Processor for L_inf PGD adversarial (robust) training.
-        """
-        super().__init__()
-        self.loss = loss_metric
-        self.n_steps = n_steps
-        self.eps = eps
-        self.step = eps * step_scale
-        self.skipped = no_perturb_attrs
-        self.attack_at_test = attack_at_test
-
-    def pre_forward(self, inputs, model: nn.Module):
-        if not self.attack_at_test and not model.training:
-            return
-        skip = []
-        collect = []
-        perturb = []
-        for skip_attr in self.skipped:
-            skip.append(visit_attr(inputs, skip_attr))
-
-        def _cata_indexing(tnsr):
-            if isinstance(tnsr, Tensor) and torch.is_floating_point(tnsr):
-                if any(x is tnsr for x in skip):
-                    return tnsr
-                collect.append(tnsr)
-                perturb.append(torch.zeros_like(tnsr))
-                return Index(len(collect) - 1)
-            return tnsr
-
-        def _cata_fill(vals):
-            return lambda x: collect[x] + vals[x] if isinstance(x, Index) else x
-
-        def _cata_detach(tnsr):
-            if isinstance(tnsr, Tensor):
-                return tnsr.detach().clone()
-            return tnsr
-
-        def _wrap_fun(*vals):
-            fill = container_catamorphism(indexed, _cata_fill(vals))
-            loss_inputs = container_catamorphism(inputs, _cata_detach)
-            loss = self.loss(loss_inputs, self.feed(model, fill))
-            return self.gscaler.scale(loss).reshape_as(loss)
-
-        indexed = container_catamorphism(inputs, _cata_indexing)
-
-        for _ in range(self.n_steps):
-            grad = ad.jacobian(_wrap_fun, tuple(perturb))
-            with torch.no_grad():
-                for i in range(len(collect)):
-                    perturb[i] += torch.sign(grad[i]) * self.step
-                    perturb[i] = torch.clamp(perturb[i], -self.eps, self.eps)
-        # print(inputs, container_catamorphism(indexed, _cata_fill(perturb)))
-        return container_catamorphism(indexed, _cata_fill(perturb))
-
-
-class Lambda(nn.Module):
-    def __init__(self, lam) -> None:
-        super().__init__()
-        self.lam = lam
-
-    def forward(self, inputs):
-        return self.lam(inputs)
-
-
-class GetItem(nn.Module):
-    def __init__(self, index) -> None:
-        super().__init__()
-        self.index = index
-
-    def forward(self, inputs):
-        return inputs[self.index]
-
-
-def supercat(tensors: Sequence[Tensor], dim: int = 0):
-    """
-    Similar to `torch.cat`, but supports broadcasting. For example:
-
-    [M, 32], [N, 1, 64] -- supercat 2 --> [N, M, 96]
-    """
-    ndim = max(x.ndim for x in tensors)
-    tensors = [x.reshape(*[1] * (ndim - x.ndim), *x.shape) for x in tensors]
-    shape = [max(x.size(i) for x in tensors) for i in range(ndim)]
-    shape[dim] = -1
-    tensors = [torch.broadcast_to(x, shape) for x in tensors]
-    return torch.cat(tensors, dim)
-
-
-xcat = supercat
-
-
-def xreshape(
-    tensor: torch.Tensor, shape: Sequence[int],
-    s: Optional[int] = None, e: Optional[int] = None, dim: Optional[int] = None
-):
-    """
-    Similar to torch.reshape, but supports reshaping a section (`s`-th dim to `e`-th dim, included) of the shape.
-
-    If dim is set, s and e will be set to dim. An error will be raised if both dim and s or e is set.
-    If either s or e is None, the reshape will start from the beginning or go through the end of the shape.
-
-    [K, A * B, C] -- xreshape [A, B] dim 1 --> [K, A, B, C]
-
-    [K, A * B, C * D] -- xreshape [A, -1, D] s -2 --> [K, A, B * C, D]
-    """
-    if dim is not None:
-        if s is not None or e is not None:
-            raise ValueError("`dim` and `s` or `e` cannot be set at the same time for `xreshape`")
-        s = e = dim
-    ndim = tensor.ndim
-    if s is None:
-        s = 0
-    if e is None:
-        e = -1
-    if s < 0:
-        s += ndim
-    if e < 0:
-        e += ndim
-    if s > e:
-        raise ValueError("Starting dim `s` cannot be greater than `e`")
-    flat = tensor
-    if s != e:
-        flat = tensor.flatten(s, e)
-    return flat.reshape(*tensor.shape[:s], *shape, *tensor.shape[e + 1:])
-
-
-class MLP(nn.Module):
-    def __init__(
-        self,
-        sizes: List[int],
-        n_group_dims: Literal[0, 1, 2, 3] = 0,
-        activation: Callable[[Tensor], Tensor] = F.relu,
-        norm: Literal['batch', 'instance', None] = 'batch'
-    ) -> None:
-        """
-        Multi-layer perceptron (Fully connected). The output layer is also normalized and activated.
-
-        sizes: sizes of layers, including the input. [n_in, h_1, h_2, ..., n_out].
-        n_group_dims: 0 if input is of shape [B, C], 1 if [B, C, N], 2 if [B, C, H, W], 3 if [B, C, D, H, W].
-        activation: a `Tensor -> Tensor` function like `torch.relu`. Defaults to `relu`.
-        norm: 'batch', 'instance', or `None`. Normalization layers type.
-        """
-        super().__init__()
-        lin = [lambda a, b, _: nn.Linear(a, b), nn.Conv1d, nn.Conv2d, nn.Conv3d][n_group_dims]
-        norm_dict = {
-            'batch': [nn.BatchNorm1d, nn.BatchNorm1d, nn.BatchNorm2d, nn.BatchNorm3d],
-            'instance': [nn.InstanceNorm1d, nn.InstanceNorm1d, nn.InstanceNorm2d, nn.InstanceNorm3d]
-        }
-        self.layers = nn.ModuleList()
-        self.norms = nn.ModuleList()
-        units = sizes[0]
-        for units_latter in sizes[1:]:
-            self.layers.append(lin(units, units_latter, 1))
-            if norm is not None:
-                self.norms.append(norm_dict[norm][n_group_dims](units_latter))
-            else:
-                self.norms.append(Lambda(lambda x: x))
-            units = units_latter
-        self.activation = activation
-
-    def forward(self, x):
-        for layer, norm in zip(self.layers, self.norms):
-            x = self.activation(norm(layer(x)))
-        return x
-
-
-class DirectPredictionAdapter(Adapter):
-    def transform(self, inputs):
-        x, y = inputs
-        return ObjectProxy(x=x, y=y)
-
-    def feed(self, net: nn.Module, inputs):
-        return ObjectProxy(logits=net(inputs.x))
-
-
-class TorchMetric(Loss, Metric):
-    def __init__(
-        self, torch_module: nn.Module, name = 'Loss',
-        pred_path: AttrPathType = 'logits', label_path: AttrPathType = 'y'
-    ) -> None:
-        super().__init__()
-        self.name = name
-        self.torch_module = torch_module
-        self.pred_path = pred_path
-        self.label_path = label_path
-
-    def __call__(self, inputs, model_return, metrics: ObjectProxy = None) -> torch.Tensor:
-        return self.torch_module(
-            visit_attr(model_return, self.pred_path),
-            visit_attr(inputs, self.label_path)
-        )
-
-
-class BinaryAcc(nn.Module):
-
-    def __init__(self, th_logits = 0.0, th_label = 0.5) -> None:
-        super().__init__()
-        self.th_logits = th_logits
-        self.th_label = th_label
-
-    def forward(self, inputs, targets):
-        return ((inputs > self.th_logits) == (targets > self.th_label)).float().mean()
-
-    def redstone(self, name: str = 'Acc', pred_path: AttrPathType = 'logits', label_path: AttrPathType = 'y'):
-        return TorchMetric(self, name, pred_path, label_path)
-
-
-class CategoricalAcc(nn.Module):
-
-    def __init__(self, dim: int = 1) -> None:
-        super().__init__()
-        self.dim = dim
-
-    def forward(self, inputs, targets):
-        return (inputs.argmax(self.dim) == targets).float().mean()
-
-    def redstone(self, name: str = 'Acc', pred_path: AttrPathType = 'logits', label_path: AttrPathType = 'y'):
-        return TorchMetric(self, name, pred_path, label_path)
-
-
-def _loss_redstone(self, name: str = 'Loss', pred_path: AttrPathType = 'logits', label_path: AttrPathType = 'y'):
-    return TorchMetric(self, name, pred_path, label_path)
-
-torch.nn.modules.loss._Loss.redstone = _loss_redstone
+from typing import List, Sequence, Union, Callable, Any, Optional
+from typing_extensions import Literal
+import torch
+import torch.autograd.functional as ad
+import torch.nn as nn
+import torch.nn.functional as F
+from torch import Tensor
+from torch.optim.optimizer import Optimizer
+
+from .processor import Processor, Adapter
+from .loss import Loss
+from .metric import Metric
+from .utils import container_catamorphism, AttrPath, visit_attr, ObjectProxy
+
+
+AttrPathType = Union[AttrPath, str, Callable[[Any], Tensor], None]
+
+
+class Index:
+    def __init__(self, idx: int) -> None:
+        self.idx = idx
+
+    def __index__(self):
+        return self.idx
+
+
+class AdvTrainingPGD(Processor):
+    def __init__(
+        self, loss_metric: Metric,
+        no_perturb_attrs: List[AttrPathType]=[],
+        eps=0.03, step_scale=0.5, n_steps=8, attack_at_test=False
+    ) -> None:
+        """
+        Processor for L_inf PGD adversarial (robust) training.
+        """
+        super().__init__()
+        self.loss = loss_metric
+        self.n_steps = n_steps
+        self.eps = eps
+        self.step = eps * step_scale
+        self.skipped = no_perturb_attrs
+        self.attack_at_test = attack_at_test
+
+    def pre_forward(self, inputs, model: nn.Module):
+        if not self.attack_at_test and not model.training:
+            return
+        skip = []
+        collect = []
+        perturb = []
+        for skip_attr in self.skipped:
+            skip.append(visit_attr(inputs, skip_attr))
+
+        def _cata_indexing(tnsr):
+            if isinstance(tnsr, Tensor) and torch.is_floating_point(tnsr):
+                if any(x is tnsr for x in skip):
+                    return tnsr
+                collect.append(tnsr)
+                perturb.append(torch.zeros_like(tnsr))
+                return Index(len(collect) - 1)
+            return tnsr
+
+        def _cata_fill(vals):
+            return lambda x: collect[x] + vals[x] if isinstance(x, Index) else x
+
+        def _cata_detach(tnsr):
+            if isinstance(tnsr, Tensor):
+                return tnsr.detach().clone()
+            return tnsr
+
+        def _wrap_fun(*vals):
+            fill = container_catamorphism(indexed, _cata_fill(vals))
+            loss_inputs = container_catamorphism(inputs, _cata_detach)
+            loss = self.loss(loss_inputs, self.feed(model, fill))
+            return self.gscaler.scale(loss).reshape_as(loss)
+
+        indexed = container_catamorphism(inputs, _cata_indexing)
+
+        for _ in range(self.n_steps):
+            grad = ad.jacobian(_wrap_fun, tuple(perturb))
+            with torch.no_grad():
+                for i in range(len(collect)):
+                    perturb[i] += torch.sign(grad[i]) * self.step
+                    perturb[i] = torch.clamp(perturb[i], -self.eps, self.eps)
+        # print(inputs, container_catamorphism(indexed, _cata_fill(perturb)))
+        return container_catamorphism(indexed, _cata_fill(perturb))
+
+
+class Lambda(nn.Module):
+    def __init__(self, lam) -> None:
+        super().__init__()
+        self.lam = lam
+
+    def forward(self, inputs):
+        return self.lam(inputs)
+
+
+class GetItem(nn.Module):
+    def __init__(self, index) -> None:
+        super().__init__()
+        self.index = index
+
+    def forward(self, inputs):
+        return inputs[self.index]
+
+
+def supercat(tensors: Sequence[Tensor], dim: int = 0):
+    """
+    Similar to `torch.cat`, but supports broadcasting. For example:
+
+    [M, 32], [N, 1, 64] -- supercat 2 --> [N, M, 96]
+    """
+    ndim = max(x.ndim for x in tensors)
+    tensors = [x.reshape(*[1] * (ndim - x.ndim), *x.shape) for x in tensors]
+    shape = [max(x.size(i) for x in tensors) for i in range(ndim)]
+    shape[dim] = -1
+    tensors = [torch.broadcast_to(x, shape) for x in tensors]
+    return torch.cat(tensors, dim)
+
+
+xcat = supercat
+
+
+def xreshape(
+    tensor: torch.Tensor, shape: Sequence[int],
+    s: Optional[int] = None, e: Optional[int] = None, dim: Optional[int] = None
+):
+    """
+    Similar to torch.reshape, but supports reshaping a section (`s`-th dim to `e`-th dim, included) of the shape.
+
+    If dim is set, s and e will be set to dim. An error will be raised if both dim and s or e is set.
+    If either s or e is None, the reshape will start from the beginning or go through the end of the shape.
+
+    [K, A * B, C] -- xreshape [A, B] dim 1 --> [K, A, B, C]
+
+    [K, A * B, C * D] -- xreshape [A, -1, D] s -2 --> [K, A, B * C, D]
+    """
+    if dim is not None:
+        if s is not None or e is not None:
+            raise ValueError("`dim` and `s` or `e` cannot be set at the same time for `xreshape`")
+        s = e = dim
+    ndim = tensor.ndim
+    if s is None:
+        s = 0
+    if e is None:
+        e = -1
+    if s < 0:
+        s += ndim
+    if e < 0:
+        e += ndim
+    if s > e:
+        raise ValueError("Starting dim `s` cannot be greater than `e`")
+    flat = tensor
+    if s != e:
+        flat = tensor.flatten(s, e)
+    return flat.reshape(*tensor.shape[:s], *shape, *tensor.shape[e + 1:])
+
+
+class MLP(nn.Module):
+    def __init__(
+        self,
+        sizes: List[int],
+        n_group_dims: Literal[0, 1, 2, 3] = 0,
+        activation: Callable[[Tensor], Tensor] = F.relu,
+        norm: Literal['batch', 'instance', None] = 'batch'
+    ) -> None:
+        """
+        Multi-layer perceptron (Fully connected). The output layer is also normalized and activated.
+
+        sizes: sizes of layers, including the input. [n_in, h_1, h_2, ..., n_out].
+        n_group_dims: 0 if input is of shape [B, C], 1 if [B, C, N], 2 if [B, C, H, W], 3 if [B, C, D, H, W].
+        activation: a `Tensor -> Tensor` function like `torch.relu`. Defaults to `relu`.
+        norm: 'batch', 'instance', or `None`. Normalization layers type.
+        """
+        super().__init__()
+        lin = [lambda a, b, _: nn.Linear(a, b), nn.Conv1d, nn.Conv2d, nn.Conv3d][n_group_dims]
+        norm_dict = {
+            'batch': [nn.BatchNorm1d, nn.BatchNorm1d, nn.BatchNorm2d, nn.BatchNorm3d],
+            'instance': [nn.InstanceNorm1d, nn.InstanceNorm1d, nn.InstanceNorm2d, nn.InstanceNorm3d]
+        }
+        self.layers = nn.ModuleList()
+        self.norms = nn.ModuleList()
+        units = sizes[0]
+        for units_latter in sizes[1:]:
+            self.layers.append(lin(units, units_latter, 1))
+            if norm is not None:
+                self.norms.append(norm_dict[norm][n_group_dims](units_latter))
+            else:
+                self.norms.append(Lambda(lambda x: x))
+            units = units_latter
+        self.activation = activation
+
+    def forward(self, x):
+        for layer, norm in zip(self.layers, self.norms):
+            x = self.activation(norm(layer(x)))
+        return x
+
+
+class GradientNormOperator(Processor):
+
+    def __init__(self, clip_norm: float, reject_norm: float) -> None:
+        super().__init__()
+        self.clip_norm = clip_norm
+        self.reject_norm = reject_norm
+
+    def pre_step(self, model: nn.Module, optimizer: Optimizer, metrics):
+        total_grad_norm = torch.nn.utils.clip_grad_norm_(
+            model.parameters(), max_norm=self.clip_norm
+        )
+        metrics.grad_norm = total_grad_norm
+        if total_grad_norm > self.reject_norm:
+            return True
+
+
+class DirectPredictionAdapter(Adapter):
+    def transform(self, inputs):
+        x, y = inputs
+        return ObjectProxy(x=x, y=y)
+
+    def feed(self, net: nn.Module, inputs):
+        return ObjectProxy(logits=net(inputs.x))
+
+
+class TorchMetric(Loss, Metric):
+    def __init__(
+        self, torch_module: nn.Module, name = 'Loss',
+        pred_path: AttrPathType = 'logits', label_path: AttrPathType = 'y'
+    ) -> None:
+        super().__init__()
+        self.name = name
+        self.torch_module = torch_module
+        self.pred_path = pred_path
+        self.label_path = label_path
+
+    def __call__(self, inputs, model_return, metrics: ObjectProxy = None) -> torch.Tensor:
+        return self.torch_module(
+            visit_attr(model_return, self.pred_path),
+            visit_attr(inputs, self.label_path)
+        )
+
+
+class BinaryAcc(nn.Module):
+
+    def __init__(self, th_logits = 0.0, th_label = 0.5) -> None:
+        super().__init__()
+        self.th_logits = th_logits
+        self.th_label = th_label
+
+    def forward(self, inputs, targets):
+        return ((inputs > self.th_logits) == (targets > self.th_label)).float().mean()
+
+    def redstone(self, name: str = 'Acc', pred_path: AttrPathType = 'logits', label_path: AttrPathType = 'y'):
+        return TorchMetric(self, name, pred_path, label_path)
+
+
+class CategoricalAcc(nn.Module):
+
+    def __init__(self, dim: int = 1) -> None:
+        super().__init__()
+        self.dim = dim
+
+    def forward(self, inputs, targets):
+        return (inputs.argmax(self.dim) == targets).float().mean()
+
+    def redstone(self, name: str = 'Acc', pred_path: AttrPathType = 'logits', label_path: AttrPathType = 'y'):
+        return TorchMetric(self, name, pred_path, label_path)
+
+
+def _loss_redstone(self, name: str = 'Loss', pred_path: AttrPathType = 'logits', label_path: AttrPathType = 'y'):
+    return TorchMetric(self, name, pred_path, label_path)
+
+torch.nn.modules.loss._Loss.redstone = _loss_redstone
```

## torch_redstone/log.py

 * *Ordering differences only*

```diff
@@ -1,128 +1,128 @@
-import os
-import time
-from typing import List, Type, Union
-import torch
-
-from .metric import Metric
-from .utils import AttrPath, visit_attr
-from .types import EpochResultInterface
-from .processor import Processor
-
-
-module_load_time = int(time.time())
-
-
-class Logger(Processor):
-    def __init__(self, exp_name: str = "training", directory: str = "./logs/"):
-        super().__init__()
-        self.exp_name = exp_name
-        self.path = directory
-        self.wrote_headers = False
-        os.makedirs(self.path, exist_ok=True)
-
-    def get_file_path(self):
-        filename = "%s_%d.csv" % (self.exp_name, module_load_time)
-        return os.path.join(self.path, filename)
-
-    def write_log(self, *data):
-        with open(self.get_file_path(), "a") as fo:
-            for d in data:
-                fo.write(str(d))
-                fo.write(",")
-            fo.write("\n")
-
-    def post_epoch(self, model, epoch, epoch_result: EpochResultInterface):
-        train = epoch_result.train.metrics.__dict__ if epoch_result.train else {}
-        val = epoch_result.val.metrics.__dict__ if epoch_result.val else {}
-        ti = list(train.items())
-        vi = list(val.items())
-        keys = ["epoch"] + ["train_" + k for k, v in ti] + ["val_" + k for k, v in vi]
-        vals = [epoch] + [v for k, v in ti] + [v for k, v in vi]
-        if not self.wrote_headers:
-            self.write_log(*keys)
-            self.wrote_headers = True
-        self.write_log(*vals)
-
-
-class BestSaver(Processor):
-    def __init__(
-        self, metric: Union[AttrPath, str, Type[Metric]] = "acc",
-        model_name: str = "model", directory: str = "./logs/",
-        lower_better: bool = False, verbose=1
-    ) -> None:
-        super().__init__()
-        self.model_name = model_name
-        self.path = directory
-        if isinstance(metric, type):
-            metric = metric.__name__.lower()
-        self.metric_attr = metric
-        self.best = float('inf') if lower_better else -float('inf')
-        self.lower_better = lower_better
-        self.verbose = verbose
-        os.makedirs(self.path, exist_ok=True)
-
-    def get_file_path(self):
-        filename = "%s_%d.dat" % (self.model_name, module_load_time)
-        return os.path.join(self.path, filename)
-
-    def get_lastest_save(self):
-        fs: List[str] = os.listdir(self.path)
-        prefix = self.model_name + '_'
-        paths = [os.path.join(self.path, x) for x in fs
-                 if x.startswith(prefix) and x.endswith('.dat')]
-        return max(paths, key=lambda x: os.stat(x).st_mtime)
-
-    def post_epoch(self, model, epoch, epoch_result: EpochResultInterface):
-        if isinstance(self.metric_attr, str):
-            if epoch_result.val:
-                met = getattr(epoch_result.val.metrics, self.metric_attr)
-            elif epoch_result.train:
-                met = getattr(epoch_result.train.metrics, self.metric_attr)
-        else:
-            met = visit_attr(epoch_result, self.metric_attr)
-        if self.lower_better:
-            if met < self.best:
-                self.best = met
-                if self.verbose >= 1:
-                    print("New best!")
-                torch.save(model.state_dict(), self.get_file_path())
-        else:
-            if met > self.best:
-                self.best = met
-                if self.verbose >= 1:
-                    print("New best!")
-                torch.save(model.state_dict(), self.get_file_path())
-
-
-class BestLossSaver(BestSaver):
-    def __init__(self, model_name: str = "model", directory: str = "./logs/") -> None:
-        super().__init__("loss", model_name, directory, lower_better=True)
-
-
-class LatestSaver(BestSaver):
-    def __init__(self, fmt: str = "model_{start_time}", cond = lambda epoch: True, directory: str = "./logs/") -> None:
-        """
-        Save latest checkpoints, with optional `cond` of checking according to epoch number (starting `0`).
-
-        Return `False` in `cond(epoch)` to skip a save.
-
-        `fmt` can have parameters `{start_time}` and `{epoch}`.
-        Supports python formatting: `{epoch:04}`
-        """
-        super().__init__(lambda _: time.time(), "", directory, verbose=0)
-        self.epoch = 0
-        self.fmt = fmt
-        self.get_file_path()  # check fmt validity
-        cond(0)  # check cond validity
-        self.cond = cond
-
-    def post_epoch(self, model, epoch, epoch_result: EpochResultInterface):
-        self.epoch = epoch
-        if self.cond(epoch):
-            return super().post_epoch(model, epoch, epoch_result)
-
-    def get_file_path(self):
-        file = self.fmt.format(epoch=self.epoch, start_time=module_load_time)
-        dirpath = os.path.dirname(os.path.join(self.path, file))
-        os.makedirs(dirpath, exist_ok=True)
-        return os.path.join(self.path, file)
+import os
+import time
+from typing import List, Type, Union
+import torch
+
+from .metric import Metric
+from .utils import AttrPath, visit_attr
+from .types import EpochResultInterface
+from .processor import Processor
+
+
+module_load_time = int(time.time())
+
+
+class Logger(Processor):
+    def __init__(self, exp_name: str = "training", directory: str = "./logs/"):
+        super().__init__()
+        self.exp_name = exp_name
+        self.path = directory
+        self.wrote_headers = False
+        os.makedirs(self.path, exist_ok=True)
+
+    def get_file_path(self):
+        filename = "%s_%d.csv" % (self.exp_name, module_load_time)
+        return os.path.join(self.path, filename)
+
+    def write_log(self, *data):
+        with open(self.get_file_path(), "a") as fo:
+            for d in data:
+                fo.write(str(d))
+                fo.write(",")
+            fo.write("\n")
+
+    def post_epoch(self, model, epoch, epoch_result: EpochResultInterface):
+        train = epoch_result.train.metrics.__dict__ if epoch_result.train else {}
+        val = epoch_result.val.metrics.__dict__ if epoch_result.val else {}
+        ti = list(train.items())
+        vi = list(val.items())
+        keys = ["epoch"] + ["train_" + k for k, v in ti] + ["val_" + k for k, v in vi]
+        vals = [epoch] + [v for k, v in ti] + [v for k, v in vi]
+        if not self.wrote_headers:
+            self.write_log(*keys)
+            self.wrote_headers = True
+        self.write_log(*vals)
+
+
+class BestSaver(Processor):
+    def __init__(
+        self, metric: Union[AttrPath, str, Type[Metric]] = "acc",
+        model_name: str = "model", directory: str = "./logs/",
+        lower_better: bool = False, verbose=1
+    ) -> None:
+        super().__init__()
+        self.model_name = model_name
+        self.path = directory
+        if isinstance(metric, type):
+            metric = metric.__name__.lower()
+        self.metric_attr = metric
+        self.best = float('inf') if lower_better else -float('inf')
+        self.lower_better = lower_better
+        self.verbose = verbose
+        os.makedirs(self.path, exist_ok=True)
+
+    def get_file_path(self):
+        filename = "%s_%d.dat" % (self.model_name, module_load_time)
+        return os.path.join(self.path, filename)
+
+    def get_lastest_save(self):
+        fs: List[str] = os.listdir(self.path)
+        prefix = self.model_name + '_'
+        paths = [os.path.join(self.path, x) for x in fs
+                 if x.startswith(prefix) and x.endswith('.dat')]
+        return max(paths, key=lambda x: os.stat(x).st_mtime)
+
+    def post_epoch(self, model, epoch, epoch_result: EpochResultInterface):
+        if isinstance(self.metric_attr, str):
+            if epoch_result.val:
+                met = getattr(epoch_result.val.metrics, self.metric_attr)
+            elif epoch_result.train:
+                met = getattr(epoch_result.train.metrics, self.metric_attr)
+        else:
+            met = visit_attr(epoch_result, self.metric_attr)
+        if self.lower_better:
+            if met < self.best:
+                self.best = met
+                if self.verbose >= 1:
+                    print("New best!")
+                torch.save(model.state_dict(), self.get_file_path())
+        else:
+            if met > self.best:
+                self.best = met
+                if self.verbose >= 1:
+                    print("New best!")
+                torch.save(model.state_dict(), self.get_file_path())
+
+
+class BestLossSaver(BestSaver):
+    def __init__(self, model_name: str = "model", directory: str = "./logs/") -> None:
+        super().__init__("loss", model_name, directory, lower_better=True)
+
+
+class LatestSaver(BestSaver):
+    def __init__(self, fmt: str = "model_{start_time}", cond = lambda epoch: True, directory: str = "./logs/") -> None:
+        """
+        Save latest checkpoints, with optional `cond` of checking according to epoch number (starting `0`).
+
+        Return `False` in `cond(epoch)` to skip a save.
+
+        `fmt` can have parameters `{start_time}` and `{epoch}`.
+        Supports python formatting: `{epoch:04}`
+        """
+        super().__init__(lambda _: time.time(), "", directory, verbose=0)
+        self.epoch = 0
+        self.fmt = fmt
+        self.get_file_path()  # check fmt validity
+        cond(0)  # check cond validity
+        self.cond = cond
+
+    def post_epoch(self, model, epoch, epoch_result: EpochResultInterface):
+        self.epoch = epoch
+        if self.cond(epoch):
+            return super().post_epoch(model, epoch, epoch_result)
+
+    def get_file_path(self):
+        file = self.fmt.format(epoch=self.epoch, start_time=module_load_time)
+        dirpath = os.path.dirname(os.path.join(self.path, file))
+        os.makedirs(dirpath, exist_ok=True)
+        return os.path.join(self.path, file)
```

## torch_redstone/loop.py

```diff
@@ -1,209 +1,219 @@
-from typing import List, Sequence, Optional, Union
-from typing_extensions import Literal
-import torch
-import torch.optim
-import torch.nn
-from torch.utils.data import DataLoader, Dataset
-import tqdm
-
-from .loss import Loss, DefaultLoss
-from .metric import Metric
-from .task import Task
-from .processor import Processor, Adapter
-from .utils import Meter, ObjectProxy, torch_to, torch_to_numpy
-from .utils import cat_proxies, collate_support_object_proxy, sanitize_name
-from .types import EllipsisType, ResultInterface
-from .log import Logger
-
-
-def take_first(iterable, n):
-    iterator = iter(iterable)
-    for _ in range(n):
-        yield next(iterator)
-
-
-class AMPLoss(Loss):
-    def __init__(self, gscaler: torch.cuda.amp.GradScaler, original_loss: Loss) -> None:
-        super().__init__()
-        self.original_loss = original_loss
-        self.gscaler = gscaler
-
-    def __call__(self, inputs, model_return, metrics: ObjectProxy) -> torch.Tensor:
-        loss = self.original_loss(inputs, model_return, metrics)
-        return self.gscaler.scale(loss).reshape_as(loss)
-
-
-class DefaultLoop:
-    def __init__(
-        self,
-        model: torch.nn.Module,
-        task: Task,
-        loss: Optional[Loss] = None,
-        metrics: Optional[Sequence[Union[Metric, EllipsisType]]] = None,
-        processors: Sequence[Processor] = None,
-        optimizer: Union[str, torch.optim.Optimizer] = 'adam',
-        adapter: Adapter = Adapter(),
-        scheduler: Optional[torch.optim.lr_scheduler._LRScheduler] = None,
-        scheduler_base: Literal['epoch', 'step'] = 'step',
-        *,
-        batch_size=32, num_workers=0, amp=False
-    ) -> None:
-        """
-        Construct the default training loop.
-
-        Notes on `metrics`:
-            `None` for task defaults.
-            A list for custom ones.
-            Ellipsis in list means appending task defaults.
-            Default displayed name for a metric is its class name.
-            This can be overridden by setting `metric.name`.
-            In returned `ObjectProxy` for metrics, attribute names are lower-case displayed names.
-
-        Notes on `loss`:
-            `None` for taking `metrics.loss` as loss.
-
-        Notes on `optimizer`:
-            It may be `torch.optim.Optimizer` instance or name of optimizer.
-            Supported names are adaptive optimizers: `adam`, `adadelta`, `sgd` and `rmsprop`.
-
-        Notes on data loaders:
-            `batch_size` and `num_workers` are ignored if the task generates DataLoaders already.
-            You may override the creation behavior in `create_data_loader`.
-        """
-        self.task = task
-        self.model = model
-        train, val = task.data()
-        self.batch_size, self.num_workers = batch_size, num_workers
-        self.train = self.create_data_loader(train, True)
-        self.val = self.create_data_loader(val, False)
-
-        self.metrics: List[Metric] = []
-        if metrics is None:
-            metrics = [...]
-        for met in metrics:
-            if met is ...:
-                for task_metric in task.metrics():
-                    self.add_metric(task_metric)
-            else:
-                self.add_metric(met)
-
-        if loss is None:
-            loss = DefaultLoss()
-        self.loss = loss
-
-        if isinstance(optimizer, str):
-            if optimizer == 'adam':
-                optimizer = torch.optim.Adam(model.parameters())
-            elif optimizer == 'rmsprop':
-                optimizer = torch.optim.RMSprop(model.parameters())
-            elif optimizer == 'adadelta':
-                optimizer = torch.optim.Adadelta(model.parameters())
-            elif optimizer == 'sgd':
-                optimizer = torch.optim.SGD(model.parameters(), 0.01, 0.9, nesterov=True)
-            else:
-                raise ValueError("Unsupported optimizer", optimizer)
-        self.optimizer = optimizer
-        if processors is None:
-            processors = [Logger()]
-        self.processors = processors
-        self.adapter = adapter
-        self.scheduler = scheduler
-        self.scheduler_base = scheduler_base
-        self.amp = amp
-        self.gscaler = torch.cuda.amp.GradScaler(enabled=amp)
-        if amp:
-            self.loss = AMPLoss(self.gscaler, self.loss)
-
-    def create_data_loader(self, data: Union[Dataset, list], is_train: bool):
-        return DataLoader(
-            data, self.batch_size, is_train, num_workers=self.num_workers,
-            collate_fn=collate_support_object_proxy
-        )
-
-    def add_metric(self, metric: Metric):
-        self.metrics.append(metric)
-
-    def run(self, num_epochs, train=True, val=True, max_steps=None, quiet=False):
-        for epoch in range(num_epochs):
-            for prx in self.processors:
-                prx.gscaler = self.gscaler
-                prx._adapter = self.adapter
-                prx.pre_epoch(self.model, epoch)
-            train_rs = self.epoch(True, epoch, max_steps=max_steps, quiet=quiet) if train else None
-            val_rs = self.epoch(False, epoch, max_steps=max_steps, quiet=quiet) if val else None
-            epoch_rs = ObjectProxy(train=train_rs, val=val_rs)
-            if self.scheduler is not None and self.scheduler_base == "epoch":
-                self.scheduler.step()
-            for prx in self.processors:
-                prx.post_epoch(self.model, epoch, epoch_rs)
-        return epoch_rs
-
-    def epoch(
-        self,
-        training: bool = False,
-        epoch: Optional[int] = None,
-        loader: Optional[DataLoader] = None,
-        max_steps: Optional[int] = None,
-        return_input: bool = False,
-        return_pred: bool = False,
-        quiet: bool = False
-    ) -> ResultInterface:
-        self.model.train(training)
-        if loader is None:
-            loader = self.train if training else self.val
-        meter = Meter()
-        ref_pt = next(self.model.parameters())
-        torch.set_grad_enabled(training)
-        if max_steps is not None:
-            if quiet:
-                prog = take_first(loader, max_steps)
-            else:
-                prog = tqdm.tqdm(take_first(loader, max_steps), total=max_steps)
-        else:
-            if quiet:
-                prog = loader
-            else:
-                prog = tqdm.tqdm(loader)
-        result: ResultInterface = ObjectProxy(metrics=None, inputs=[], preds=[])
-        for d in prog:
-            if return_input:
-                result.inputs.append(torch_to_numpy(d))
-            d = torch_to(d, ref_pt.device)
-            d = self.adapter.transform(d)
-            with torch.autocast(ref_pt.device.type, enabled=self.amp):
-                for prx in self.processors:
-                    ret = prx.pre_forward(d, self.model)
-                    if ret is not None:
-                        d = ret
-                output = self.adapter.feed(self.model, d)
-                for prx in self.processors:
-                    ret = prx.post_forward(d, self.model, output)
-                    if ret is not None:
-                        output = ret
-                metvals = ObjectProxy()
-                for met in self.metrics:
-                    mval = met(d, output)
-                    setattr(metvals, sanitize_name(met.name.lower()), mval)
-                    meter.u(met.name, mval.item())
-                if training:
-                    loss = self.loss(d, output, metvals)
-            if training:
-                loss.backward()
-                self.gscaler.step(self.optimizer)
-                self.gscaler.update()
-                if self.scheduler is not None and self.scheduler_base == "step":
-                    self.scheduler.step()
-                for prx in self.processors:
-                    prx.post_step(self.model, self.optimizer, metvals)
-                self.optimizer.zero_grad()
-            if return_pred:
-                result.preds.append(torch_to_numpy(output))
-            desc = "VT"[training] + (" %02d" % epoch if epoch is not None else "")
-            for k in sorted(meter.k):
-                desc += " %s: %.4f" % (k, meter[k])
-            if hasattr(prog, 'set_description'):
-                prog.set_description(desc)
-        result.metrics = ObjectProxy(**{sanitize_name(k.lower()): meter[k] for k in sorted(meter.k)})
-        result.inputs = cat_proxies(result.inputs) if return_input else None
-        result.preds = cat_proxies(result.preds) if return_pred else None
-        return result
+from typing import List, Sequence, Optional, Union
+from typing_extensions import Literal
+import torch
+import torch.optim
+import torch.nn
+from torch.utils.data import DataLoader, Dataset
+import tqdm
+
+from .loss import Loss, DefaultLoss
+from .metric import Metric
+from .task import Task
+from .processor import Processor, Adapter
+from .utils import Meter, ObjectProxy, torch_to, torch_to_numpy
+from .utils import cat_proxies, collate_support_object_proxy, sanitize_name
+from .types import EllipsisType, ResultInterface
+from .log import Logger
+
+
+def take_first(iterable, n):
+    iterator = iter(iterable)
+    for _ in range(n):
+        yield next(iterator)
+
+
+class AMPLoss(Loss):
+    def __init__(self, gscaler: torch.cuda.amp.GradScaler, original_loss: Loss) -> None:
+        super().__init__()
+        self.original_loss = original_loss
+        self.gscaler = gscaler
+
+    def __call__(self, inputs, model_return, metrics: ObjectProxy) -> torch.Tensor:
+        loss = self.original_loss(inputs, model_return, metrics)
+        return self.gscaler.scale(loss).reshape_as(loss)
+
+
+class DefaultLoop:
+    def __init__(
+        self,
+        model: torch.nn.Module,
+        task: Task,
+        loss: Optional[Loss] = None,
+        metrics: Optional[Sequence[Union[Metric, EllipsisType]]] = None,
+        processors: Sequence[Processor] = None,
+        optimizer: Union[str, torch.optim.Optimizer] = 'adam',
+        adapter: Adapter = Adapter(),
+        scheduler: Optional[torch.optim.lr_scheduler._LRScheduler] = None,
+        scheduler_base: Literal['epoch', 'step'] = 'step',
+        *,
+        batch_size=32, num_workers=0, amp=False
+    ) -> None:
+        """
+        Construct the default training loop.
+
+        Notes on `metrics`:
+            `None` for task defaults.
+            A list for custom ones.
+            Ellipsis in list means appending task defaults.
+            Default displayed name for a metric is its class name.
+            This can be overridden by setting `metric.name`.
+            In returned `ObjectProxy` for metrics, attribute names are lower-case displayed names.
+
+        Notes on `loss`:
+            `None` for taking `metrics.loss` as loss.
+
+        Notes on `optimizer`:
+            It may be `torch.optim.Optimizer` instance or name of optimizer.
+            Supported names are adaptive optimizers: `adam`, `adadelta`, `sgd` and `rmsprop`.
+
+        Notes on data loaders:
+            `batch_size` and `num_workers` are ignored if the task generates DataLoaders already.
+            You may override the creation behavior in `create_data_loader`.
+        """
+        self.task = task
+        self.model = model
+        train, val = task.data()
+        self.batch_size, self.num_workers = batch_size, num_workers
+        self.train = self.create_data_loader(train, True)
+        self.val = self.create_data_loader(val, False)
+
+        self.metrics: List[Metric] = []
+        if metrics is None:
+            metrics = [...]
+        for met in metrics:
+            if met is ...:
+                for task_metric in task.metrics():
+                    self.add_metric(task_metric)
+            else:
+                self.add_metric(met)
+
+        if loss is None:
+            loss = DefaultLoss()
+        self.loss = loss
+
+        if isinstance(optimizer, str):
+            if optimizer == 'adam':
+                optimizer = torch.optim.Adam(model.parameters())
+            elif optimizer == 'rmsprop':
+                optimizer = torch.optim.RMSprop(model.parameters())
+            elif optimizer == 'adadelta':
+                optimizer = torch.optim.Adadelta(model.parameters())
+            elif optimizer == 'sgd':
+                optimizer = torch.optim.SGD(model.parameters(), 0.01, 0.9, nesterov=True)
+            else:
+                raise ValueError("Unsupported optimizer", optimizer)
+        self.optimizer = optimizer
+        if processors is None:
+            processors = [Logger()]
+        self.processors = processors
+        self.adapter = adapter
+        self.scheduler = scheduler
+        self.scheduler_base = scheduler_base
+        if amp is True:
+            amp = torch.float16
+        self.amp = amp
+        self.gscaler = torch.cuda.amp.GradScaler(enabled=amp == torch.float16)
+        if amp == torch.float16:
+            self.loss = AMPLoss(self.gscaler, self.loss)
+
+    def create_data_loader(self, data: Union[Dataset, list], is_train: bool, **kwargs):
+        return DataLoader(
+            data, self.batch_size, is_train, num_workers=self.num_workers,
+            collate_fn=collate_support_object_proxy, **kwargs
+        )
+
+    def add_metric(self, metric: Metric):
+        self.metrics.append(metric)
+
+    def run(self, num_epochs, train=True, val=True, max_steps=None, quiet=False):
+        for epoch in range(num_epochs):
+            for prx in self.processors:
+                prx.gscaler = self.gscaler
+                prx._adapter = self.adapter
+                prx.pre_epoch(self.model, epoch)
+            train_rs = self.epoch(True, epoch, max_steps=max_steps, quiet=quiet) if train else None
+            val_rs = self.epoch(False, epoch, max_steps=max_steps, quiet=quiet) if val else None
+            epoch_rs = ObjectProxy(train=train_rs, val=val_rs)
+            if self.scheduler is not None and self.scheduler_base == "epoch":
+                self.scheduler.step()
+            for prx in self.processors:
+                prx.post_epoch(self.model, epoch, epoch_rs)
+        return epoch_rs
+
+    def epoch(
+        self,
+        training: bool = False,
+        epoch: Optional[int] = None,
+        loader: Optional[DataLoader] = None,
+        max_steps: Optional[int] = None,
+        return_input: bool = False,
+        return_pred: bool = False,
+        quiet: bool = False
+    ) -> ResultInterface:
+        self.model.train(training)
+        if loader is None:
+            loader = self.train if training else self.val
+        meter = Meter()
+        ref_pt = next(self.model.parameters())
+        torch.set_grad_enabled(training)
+        if max_steps is not None:
+            if quiet:
+                prog = take_first(loader, max_steps)
+            else:
+                prog = tqdm.tqdm(take_first(loader, max_steps), total=max_steps)
+        else:
+            if quiet:
+                prog = loader
+            else:
+                prog = tqdm.tqdm(loader)
+        result: ResultInterface = ObjectProxy(metrics=None, inputs=[], preds=[])
+        for d in prog:
+            if return_input:
+                result.inputs.append(torch_to_numpy(d))
+            d = torch_to(d, ref_pt.device)
+            d = self.adapter.transform(d)
+            if self.amp:
+                ac = torch.autocast(ref_pt.device.type, enabled=bool(self.amp), dtype=self.amp)
+            else:
+                ac = torch.autocast(ref_pt.device.type, enabled=False)
+            with ac:
+                for prx in self.processors:
+                    ret = prx.pre_forward(d, self.model)
+                    if ret is not None:
+                        d = ret
+                output = self.adapter.feed(self.model, d)
+                for prx in self.processors:
+                    ret = prx.post_forward(d, self.model, output)
+                    if ret is not None:
+                        output = ret
+                metvals = ObjectProxy()
+                for met in self.metrics:
+                    mval = met(d, output)
+                    setattr(metvals, sanitize_name(met.name.lower()), mval)
+                    meter.u(met.name, mval.item())
+                if training:
+                    loss = self.loss(d, output, metvals)
+            if training:
+                loss.backward()
+                skip = False
+                for prx in self.processors:
+                    skip = skip or prx.pre_step(self.model, self.optimizer, metvals)
+                if not skip:
+                    self.gscaler.step(self.optimizer)
+                    self.gscaler.update()
+                    if self.scheduler is not None and self.scheduler_base == "step":
+                        self.scheduler.step()
+                for prx in self.processors:
+                    prx.post_step(self.model, self.optimizer, metvals)
+                self.optimizer.zero_grad()
+            if return_pred:
+                result.preds.append(torch_to_numpy(output))
+            desc = "VT"[training] + (" %02d" % epoch if epoch is not None else "")
+            for k in sorted(meter.k):
+                desc += " %s: %.4f" % (k, meter[k])
+            if hasattr(prog, 'set_description'):
+                prog.set_description(desc)
+        result.metrics = ObjectProxy(**{sanitize_name(k.lower()): meter[k] for k in sorted(meter.k)})
+        result.inputs = cat_proxies(result.inputs) if return_input else None
+        result.preds = cat_proxies(result.preds) if return_pred else None
+        return result
```

## torch_redstone/loss.py

 * *Ordering differences only*

```diff
@@ -1,15 +1,15 @@
-from abc import abstractmethod
-import torch
-
-from .utils import ObjectProxy
-
-
-class Loss:
-    @abstractmethod
-    def __call__(self, inputs, model_return, metrics: ObjectProxy) -> torch.Tensor:
-        raise NotImplementedError
-
-
-class DefaultLoss(Loss):
-    def __call__(self, inputs, model_return, metrics: ObjectProxy) -> torch.Tensor:
-        return metrics.loss
+from abc import abstractmethod
+import torch
+
+from .utils import ObjectProxy
+
+
+class Loss:
+    @abstractmethod
+    def __call__(self, inputs, model_return, metrics: ObjectProxy) -> torch.Tensor:
+        raise NotImplementedError
+
+
+class DefaultLoss(Loss):
+    def __call__(self, inputs, model_return, metrics: ObjectProxy) -> torch.Tensor:
+        return metrics.loss
```

## torch_redstone/metric.py

 * *Ordering differences only*

```diff
@@ -1,16 +1,16 @@
-from abc import abstractmethod
-import torch
-
-
-class Metric:
-    @property
-    def name(self):
-        return getattr(self, '_name', self.__class__.__name__)
-
-    @name.setter
-    def name(self, n):
-        self._name = n
-
-    @abstractmethod
-    def __call__(self, inputs, model_return) -> torch.Tensor:
-        raise NotImplementedError
+from abc import abstractmethod
+import torch
+
+
+class Metric:
+    @property
+    def name(self):
+        return getattr(self, '_name', self.__class__.__name__)
+
+    @name.setter
+    def name(self, n):
+        self._name = n
+
+    @abstractmethod
+    def __call__(self, inputs, model_return) -> torch.Tensor:
+        raise NotImplementedError
```

## torch_redstone/polyfill.py

 * *Ordering differences only*

```diff
@@ -1,61 +1,61 @@
-import torch
-
-
-class Polyfill:
-    @staticmethod
-    def cdist2(src: torch.Tensor, dst: torch.Tensor):
-        """
-        Computes batched the squared 2-norm distance between each pair of the two collections of row vectors.
-        src (Tensor): input tensor of shape [B, N, C].
-        dst (Tensor): input tensor of shape [B, M, C].
-        Output: per-point square distance of shape [B, N, M].
-        """
-        B, M, _ = dst.shape
-        dist = torch.baddbmm(torch.sum(src ** 2, -1, keepdim=True), src, dst.permute(0, 2, 1), alpha=-2)
-        dist += torch.sum(dst ** 2, -1).view(B, 1, M)
-        return dist
-
-    @staticmethod
-    def cdist(src: torch.Tensor, dst: torch.Tensor):
-        """
-        Computes batched the 2-norm distance between each pair of the two collections of row vectors.
-        src (Tensor): input tensor of shape [B, N, C].
-        dst (Tensor): input tensor of shape [B, M, C].
-        Output: per-point distance of shape [B, N, M].
-        """
-        return Polyfill.cdist2(src, dst).sqrt_()
-
-    @staticmethod
-    def square(x: torch.Tensor):
-        return x * x
-
-    @staticmethod
-    def broadcast_to(tensor: torch.Tensor, shape):
-        return tensor.expand(shape)
-
-    @staticmethod
-    def autocast_cuda_only(device_type: str, enabled: bool = True):
-        return torch.cuda.amp.autocast(enabled=enabled)
-
-
-# Polyfill impls
-if not hasattr(torch, 'square'):
-    torch.square = Polyfill.square
-if not hasattr(torch, 'broadcast_to'):
-    torch.broadcast_to = Polyfill.broadcast_to
-if not hasattr(torch, 'cdist'):
-    torch.cdist = Polyfill.cdist
-if not hasattr(torch, 'autocast'):
-    torch.autocast = Polyfill.autocast_cuda_only
-
-# Aliases
-if not hasattr(torch, 'absolute'):
-    torch.absolute = torch.abs
-if not hasattr(torch, 'arccos'):
-    torch.arccos = torch.acos
-if not hasattr(torch, 'arcsin'):
-    torch.arcsin = torch.asin
-if not hasattr(torch, 'arctan'):
-    torch.arctan = torch.atan
-if not hasattr(torch, 'arctan2'):
-    torch.arctan2 = torch.atan2
+import torch
+
+
+class Polyfill:
+    @staticmethod
+    def cdist2(src: torch.Tensor, dst: torch.Tensor):
+        """
+        Computes batched the squared 2-norm distance between each pair of the two collections of row vectors.
+        src (Tensor): input tensor of shape [B, N, C].
+        dst (Tensor): input tensor of shape [B, M, C].
+        Output: per-point square distance of shape [B, N, M].
+        """
+        B, M, _ = dst.shape
+        dist = torch.baddbmm(torch.sum(src ** 2, -1, keepdim=True), src, dst.permute(0, 2, 1), alpha=-2)
+        dist += torch.sum(dst ** 2, -1).view(B, 1, M)
+        return dist
+
+    @staticmethod
+    def cdist(src: torch.Tensor, dst: torch.Tensor):
+        """
+        Computes batched the 2-norm distance between each pair of the two collections of row vectors.
+        src (Tensor): input tensor of shape [B, N, C].
+        dst (Tensor): input tensor of shape [B, M, C].
+        Output: per-point distance of shape [B, N, M].
+        """
+        return Polyfill.cdist2(src, dst).sqrt_()
+
+    @staticmethod
+    def square(x: torch.Tensor):
+        return x * x
+
+    @staticmethod
+    def broadcast_to(tensor: torch.Tensor, shape):
+        return tensor.expand(shape)
+
+    @staticmethod
+    def autocast_cuda_only(device_type: str, enabled: bool = True):
+        return torch.cuda.amp.autocast(enabled=enabled)
+
+
+# Polyfill impls
+if not hasattr(torch, 'square'):
+    torch.square = Polyfill.square
+if not hasattr(torch, 'broadcast_to'):
+    torch.broadcast_to = Polyfill.broadcast_to
+if not hasattr(torch, 'cdist'):
+    torch.cdist = Polyfill.cdist
+if not hasattr(torch, 'autocast'):
+    torch.autocast = Polyfill.autocast_cuda_only
+
+# Aliases
+if not hasattr(torch, 'absolute'):
+    torch.absolute = torch.abs
+if not hasattr(torch, 'arccos'):
+    torch.arccos = torch.acos
+if not hasattr(torch, 'arcsin'):
+    torch.arcsin = torch.asin
+if not hasattr(torch, 'arctan'):
+    torch.arctan = torch.atan
+if not hasattr(torch, 'arctan2'):
+    torch.arctan2 = torch.atan2
```

## torch_redstone/processor.py

```diff
@@ -1,36 +1,39 @@
-import torch
-import torch.nn as nn
-import torch.optim
-
-from .types import EpochResultInterface
-
-
-class Adapter:
-    def transform(self, inputs):
-        return inputs
-
-    def feed(self, net: nn.Module, inputs):
-        return net(inputs)
-
-
-class Processor:
-    gscaler: torch.cuda.amp.GradScaler
-    _adapter: Adapter
-
-    def feed(self, model: nn.Module, inputs):
-        return self._adapter.feed(model, inputs)
-
-    def pre_forward(self, inputs, model: nn.Module):
-        pass
-
-    def post_forward(self, inputs, model: nn.Module, model_return):
-        pass
-
-    def post_step(self, model: nn.Module, optimizer: torch.optim.Optimizer, metrics):
-        pass
-
-    def pre_epoch(self, model: nn.Module, epoch: int):
-        pass
-
-    def post_epoch(self, model: nn.Module, epoch: int, epoch_result: EpochResultInterface):
-        pass
+import torch
+import torch.nn as nn
+import torch.optim
+
+from .types import EpochResultInterface
+
+
+class Adapter:
+    def transform(self, inputs):
+        return inputs
+
+    def feed(self, net: nn.Module, inputs):
+        return net(inputs)
+
+
+class Processor:
+    gscaler: torch.cuda.amp.GradScaler
+    _adapter: Adapter
+
+    def feed(self, model: nn.Module, inputs):
+        return self._adapter.feed(model, inputs)
+
+    def pre_forward(self, inputs, model: nn.Module):
+        pass
+
+    def post_forward(self, inputs, model: nn.Module, model_return):
+        pass
+
+    def pre_step(self, model: nn.Module, optimizer: torch.optim.Optimizer, metrics):
+        pass
+
+    def post_step(self, model: nn.Module, optimizer: torch.optim.Optimizer, metrics):
+        pass
+
+    def pre_epoch(self, model: nn.Module, epoch: int):
+        pass
+
+    def post_epoch(self, model: nn.Module, epoch: int, epoch_result: EpochResultInterface):
+        pass
```

## torch_redstone/task.py

 * *Ordering differences only*

```diff
@@ -1,15 +1,15 @@
-from abc import abstractmethod
-from typing import Sequence, Tuple, Union
-from torch.utils.data import Dataset, DataLoader
-
-from .metric import Metric
-
-
-class Task:
-    @abstractmethod
-    def data(self) -> Tuple[Union[Dataset, DataLoader, list], Union[Dataset, DataLoader, list]]:
-        raise NotImplementedError
-
-    @abstractmethod
-    def metrics(self) -> Sequence[Metric]:
-        raise NotImplementedError
+from abc import abstractmethod
+from typing import Sequence, Tuple, Union
+from torch.utils.data import Dataset, DataLoader
+
+from .metric import Metric
+
+
+class Task:
+    @abstractmethod
+    def data(self) -> Tuple[Union[Dataset, DataLoader, list], Union[Dataset, DataLoader, list]]:
+        raise NotImplementedError
+
+    @abstractmethod
+    def metrics(self) -> Sequence[Metric]:
+        raise NotImplementedError
```

## torch_redstone/types.py

 * *Ordering differences only*

```diff
@@ -1,17 +1,17 @@
-from typing import Any, Optional
-
-from .utils import ObjectProxy
-
-
-EllipsisType = type(...)
-
-
-class ResultInterface:
-    metrics: ObjectProxy
-    inputs: Optional[Any]
-    preds: Optional[Any]
-
-
-class EpochResultInterface:
-    train: Optional[ResultInterface]
-    val: Optional[ResultInterface]
+from typing import Any, Optional
+
+from .utils import ObjectProxy
+
+
+EllipsisType = type(...)
+
+
+class ResultInterface:
+    metrics: ObjectProxy
+    inputs: Optional[Any]
+    preds: Optional[Any]
+
+
+class EpochResultInterface:
+    train: Optional[ResultInterface]
+    val: Optional[ResultInterface]
```

## torch_redstone/utils.py

```diff
@@ -1,196 +1,207 @@
-import re
-import types
-import typing
-import random
-import inspect
-import collections
-import numpy
-import torch
-from typing import Any, Callable, Sequence, Type, Union
-from torch.utils.data.dataloader import default_collate
-
-
-class Meter:
-    def __init__(self) -> None:
-        self.k = collections.defaultdict(int)
-        self.v = collections.defaultdict(int)
-
-    def __getitem__(self, k):
-        if self.k[k] == 0:
-            return 0
-        return self.v[k] / self.k[k]
-
-    def u(self, k, v):
-        self.k[k] += 1
-        self.v[k] += v
-
-
-class AttrPath:
-    def __init__(self, get=lambda x: x, set=lambda x, v: None) -> None:
-        self.get = get
-        self.set = set
-
-    def __getattr__(self, attr):
-        return AttrPath(
-            lambda x: getattr(self.get(x), attr),
-            lambda x, v: setattr(self.get(x), attr, v)
-        )
-
-
-def visit_attr(Q, attr: Union[AttrPath, str, Callable[[Any], torch.Tensor], None]):
-    if attr is None:
-        return Q
-    if isinstance(attr, str):
-        for sec in attr.split('.'):
-            Q = getattr(Q, sec)
-        return Q
-    if isinstance(attr, AttrPath):
-        return attr.get(Q)
-    return attr(Q)
-
-
-def sanitize_name(name):
-    return re.sub(r'\W|^(?=\d)', '_', name)
-
-
-class ObjectProxy(types.SimpleNamespace):
-
-    def __getattr__(self, name):
-        proxy = ObjectProxy()
-        setattr(self, name, proxy)
-        return proxy
-
-    def __len__(self):
-        return len(self.__dict__)
-
-    def __contains__(self, k):
-        return k in self.__dict__
-
-    def __getitem__(self, k):
-        return self.__dict__[k]
-
-    def __setitem__(self, k, v):
-        self.__dict__[k] = v
-
-    @classmethod
-    def zip(cls, **kwargs):
-        """
-        zip(k1=v1, k2=v2, ...) -> Iter[ObjectProxy], where `v1`, ... are iterable.
-
-        Each `ObjectProxy` has attributes `k1`, `k2`, ... whose values are
-        the corresponding items in `v1`, `v2`, ...
-        """
-        keys = []
-        vals = []
-        for k, v in kwargs.items():
-            keys.append(k)
-            vals.append(v)
-        for vs in zip(*vals):
-            yield cls(**dict(zip(keys, vs)))
-
-
-TElem = typing.TypeVar('TElem')
-TRes = typing.TypeVar('TRes')
-
-
-class TC(typing.Generic[TElem]):
-    pass
-
-
-def container_catamorphism(
-    data: TC[TElem], func: Callable[[TElem], TRes]
-) -> TC[TRes]:
-    """
-    Transforms `TElem` in `list`, `dict`, `ObjectProxy`, `tuple`, `set` with `func`.
-    Nested containers are also supported.
-    """
-    if isinstance(data, ObjectProxy):
-        return ObjectProxy(**container_catamorphism(data.__dict__, func))
-    if isinstance(data, dict):
-        return {
-            k: container_catamorphism(v, func) for k, v in data.items()
-        }
-    if isinstance(data, list):
-        return [container_catamorphism(x, func) for x in data]
-    if isinstance(data, tuple):
-        return tuple(container_catamorphism(x, func) for x in data)
-    if isinstance(data, set):
-        return {container_catamorphism(x, func) for x in data}
-    return func(data)
-
-
-def torch_to(data: TC[torch.Tensor], reference: Union[str, torch.device, torch.Tensor], strict=False) -> TC[torch.Tensor]:
-    """
-    Recursively send `torch.Tensor` in `list`, `dict`, `ObjectProxy`, `tuple`, `set` to `reference`.
-
-    strict: if `True`, unrecognized objects without `.to` function will cause an error.
-    """
-    if strict:
-        return container_catamorphism(data, lambda x: x.to(reference))
-    else:
-        return container_catamorphism(data, lambda x: x.to(reference) if hasattr(x, 'to') else x)
-
-
-def torch_to_numpy(data: TC[torch.Tensor], strict=False) -> TC[numpy.ndarray]:
-    """
-    Recursively fetch `torch.Tensor` in `list`, `dict`, `ObjectProxy`, `tuple`, `set` as numpy array.
-
-    strict: if `True`, unrecognized objects will cause an error.
-    """
-    if strict:
-        return container_catamorphism(data, lambda x: x.detach().cpu().numpy())
-    else:
-        return container_catamorphism(data, lambda x: x.detach().cpu().numpy() if hasattr(x, 'detach') else x)
-
-
-def container_pushdown(seq: Sequence[TC], target_cls: Type[TElem] = list) -> TC[TElem]:
-    """
-    Push sequence of containers (`list`, `dict`, `ObjectProxy`, `tuple`) inwards.
-    Nested containers supported.
-
-    Example: [{a: 0, b: 1}, {a: 1, b: 2}] -> {a: [0, 1], b: [1, 2]}
-    """
-    data = seq[0]
-    c = target_cls
-    if isinstance(data, ObjectProxy):
-        return ObjectProxy(**container_pushdown([x.__dict__ for x in seq], c))
-    if isinstance(data, dict):
-        return {
-            k: container_pushdown([x[k] for x in seq], c) for k in data.keys()
-        }
-    if isinstance(data, list):
-        return [container_pushdown([x[i] for x in seq], c) for i in range(len(data))]
-    if isinstance(data, tuple):
-        return tuple(container_pushdown([x[i] for x in seq], c) for i in range(len(data)))
-    return target_cls(seq)
-
-
-class CollateList:
-    def __init__(self, *args, **kwargs) -> None:
-        self.wrap = list(*args, **kwargs)
-
-
-def cat_proxies(proxies: Sequence[ObjectProxy], axis=0):
-    """
-    Merge (concatenate) sequence of `ObjectProxy` whose elements are numpy arrays.
-    """
-    return container_catamorphism(
-        container_pushdown(proxies, CollateList),
-        lambda x: numpy.concatenate(x.wrap, axis=axis)
-    )
-
-
-def collate_support_object_proxy(batch):
-    return container_catamorphism(
-        container_pushdown(batch, CollateList),
-        lambda x: default_collate(x.wrap)
-    )
-
-
-def seed(seed: int):
-    """
-    Set random seeds to `seed` for `torch`, `numpy` and python `random`.
-    """
-    torch.manual_seed(seed)
-    numpy.random.seed(seed)
-    random.seed(seed)
+import re
+import math
+import types
+import typing
+import random
+import inspect
+import collections
+import numpy
+import torch
+from typing import Any, Callable, Sequence, Type, Union
+from torch.utils.data.dataloader import default_collate
+
+
+class Meter:
+    def __init__(self) -> None:
+        self.k = collections.defaultdict(int)
+        self.v = collections.defaultdict(int)
+
+    def __getitem__(self, k):
+        if self.k[k] == 0:
+            return 0
+        return self.v[k] / self.k[k]
+
+    def u(self, k, v):
+        self.k[k] += 1
+        self.v[k] += v
+
+
+class AttrPath:
+    def __init__(self, get=lambda x: x, set=lambda x, v: None) -> None:
+        self.get = get
+        self.set = set
+
+    def __getattr__(self, attr):
+        return AttrPath(
+            lambda x: getattr(self.get(x), attr),
+            lambda x, v: setattr(self.get(x), attr, v)
+        )
+
+
+def visit_attr(Q, attr: Union[AttrPath, str, Callable[[Any], torch.Tensor], None]):
+    if attr is None:
+        return Q
+    if isinstance(attr, str):
+        for sec in attr.split('.'):
+            Q = getattr(Q, sec)
+        return Q
+    if isinstance(attr, AttrPath):
+        return attr.get(Q)
+    return attr(Q)
+
+
+def sanitize_name(name):
+    return re.sub(r'\W|^(?=\d)', '_', name)
+
+
+class ObjectProxy(types.SimpleNamespace):
+
+    def __getattr__(self, name):
+        if name.startswith('__') and name.endswith('__'):
+            raise AttributeError
+        proxy = ObjectProxy()
+        setattr(self, name, proxy)
+        return proxy
+
+    def __len__(self):
+        return len(self.__dict__)
+
+    def __contains__(self, k):
+        return k in self.__dict__
+
+    def __getitem__(self, k):
+        return self.__dict__[k]
+
+    def __setitem__(self, k, v):
+        self.__dict__[k] = v
+
+    @classmethod
+    def zip(cls, **kwargs):
+        """
+        zip(k1=v1, k2=v2, ...) -> Iter[ObjectProxy], where `v1`, ... are iterable.
+
+        Each `ObjectProxy` has attributes `k1`, `k2`, ... whose values are
+        the corresponding items in `v1`, `v2`, ...
+        """
+        keys = []
+        vals = []
+        for k, v in kwargs.items():
+            keys.append(k)
+            vals.append(v)
+        for vs in zip(*vals):
+            yield cls(**dict(zip(keys, vs)))
+
+
+TElem = typing.TypeVar('TElem')
+TRes = typing.TypeVar('TRes')
+
+
+class TC(typing.Generic[TElem]):
+    pass
+
+
+def container_catamorphism(
+    data: TC[TElem], func: Callable[[TElem], TRes]
+) -> TC[TRes]:
+    """
+    Transforms `TElem` in `list`, `dict`, `ObjectProxy`, `tuple`, `set` with `func`.
+    Nested containers are also supported.
+    """
+    if isinstance(data, ObjectProxy):
+        return ObjectProxy(**container_catamorphism(data.__dict__, func))
+    if isinstance(data, dict):
+        return {
+            k: container_catamorphism(v, func) for k, v in data.items()
+        }
+    if isinstance(data, list):
+        return [container_catamorphism(x, func) for x in data]
+    if isinstance(data, tuple):
+        return tuple(container_catamorphism(x, func) for x in data)
+    if isinstance(data, set):
+        return {container_catamorphism(x, func) for x in data}
+    return func(data)
+
+
+def torch_to(data: TC[torch.Tensor], reference: Union[str, torch.device, torch.Tensor], strict=False) -> TC[torch.Tensor]:
+    """
+    Recursively send `torch.Tensor` in `list`, `dict`, `ObjectProxy`, `tuple`, `set` to `reference`.
+
+    strict: if `True`, unrecognized objects without `.to` function will cause an error.
+    """
+    if strict:
+        return container_catamorphism(data, lambda x: x.to(reference))
+    else:
+        return container_catamorphism(data, lambda x: x.to(reference) if hasattr(x, 'to') else x)
+
+
+def torch_to_numpy(data: TC[torch.Tensor], strict=False) -> TC[numpy.ndarray]:
+    """
+    Recursively fetch `torch.Tensor` in `list`, `dict`, `ObjectProxy`, `tuple`, `set` as numpy array.
+
+    strict: if `True`, unrecognized objects will cause an error.
+    """
+    if strict:
+        return container_catamorphism(data, lambda x: x.detach().cpu().numpy())
+    else:
+        return container_catamorphism(data, lambda x: x.detach().cpu().numpy() if hasattr(x, 'detach') else x)
+
+
+def container_pushdown(seq: Sequence[TC], target_cls: Type[TElem] = list) -> TC[TElem]:
+    """
+    Push sequence of containers (`list`, `dict`, `ObjectProxy`, `tuple`) inwards.
+    Nested containers supported.
+
+    Example: [{a: 0, b: 1}, {a: 1, b: 2}] -> {a: [0, 1], b: [1, 2]}
+    """
+    data = seq[0]
+    c = target_cls
+    if isinstance(data, ObjectProxy):
+        return ObjectProxy(**container_pushdown([x.__dict__ for x in seq], c))
+    if isinstance(data, dict):
+        return {
+            k: container_pushdown([x[k] for x in seq], c) for k in data.keys()
+        }
+    if isinstance(data, list):
+        return [container_pushdown([x[i] for x in seq], c) for i in range(len(data))]
+    if isinstance(data, tuple):
+        return tuple(container_pushdown([x[i] for x in seq], c) for i in range(len(data)))
+    return target_cls(seq)
+
+
+class CollateList:
+    def __init__(self, *args, **kwargs) -> None:
+        self.wrap = list(*args, **kwargs)
+
+
+def cat_proxies(proxies: Sequence[ObjectProxy], axis=0):
+    """
+    Merge (concatenate) sequence of `ObjectProxy` whose elements are numpy arrays.
+    """
+    return container_catamorphism(
+        container_pushdown(proxies, CollateList),
+        lambda x: numpy.concatenate(x.wrap, axis=axis)
+    )
+
+
+def collate_support_object_proxy(batch):
+    return container_catamorphism(
+        container_pushdown(batch, CollateList),
+        lambda x: default_collate(x.wrap)
+    )
+
+
+def seed(seed: int):
+    """
+    Set random seeds to `seed` for `torch`, `numpy` and python `random`.
+    """
+    torch.manual_seed(seed)
+    numpy.random.seed(seed)
+    random.seed(seed)
+
+
+def log1m_exp(arr_x):
+    oob = arr_x < math.log(torch.finfo(arr_x.dtype).smallest_normal)
+    mask = arr_x > -0.6931472  # appox -log(2)
+    more_val = torch.log(-torch.expm1(arr_x))
+    less_val = torch.log1p(-torch.exp(arr_x))
+    return torch.where(oob, 0., torch.where(mask, more_val, less_val))
```

## torch_redstone/version.py

```diff
@@ -1 +1 @@
-__version__ = '0.0.5'
+__version__ = '0.0.6'
```

## Comparing `torch.redstone-0.0.5.dist-info/LICENSE` & `torch.redstone-0.0.6.dist-info/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright 2022 eliphat
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright 2022 eliphat
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

## Comparing `torch.redstone-0.0.5.dist-info/METADATA` & `torch.redstone-0.0.6.dist-info/METADATA`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: torch.redstone
-Version: 0.0.5
+Version: 0.0.6
 Summary: Redstone torch, common boilerplates for PyTorch.
 Home-page: https://github.com/eliphatfs/torch.redstone
 Author: flandre.info
 Author-email: flandre@scarletx.cn
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: ~=3.6
 Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: tqdm
 Requires-Dist: numpy
+Requires-Dist: tqdm
 Requires-Dist: typing-extensions
 
 # `torch.redstone`
 
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/eliphatfs/torch.redstone/build_and_run.yaml)](https://github.com/eliphatfs/torch.redstone/actions) [![PyPI](https://img.shields.io/pypi/v/torch.redstone)](https://pypi.org/project/torch.redstone/)
 
 Polyfills, common boilerplates and utilities -- A super light-weight library to boost development with PyTorch.
```

