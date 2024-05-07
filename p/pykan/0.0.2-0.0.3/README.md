# Comparing `tmp/pykan-0.0.2.tar.gz` & `tmp/pykan-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pykan-0.0.2.tar", last modified: Mon Apr 29 17:00:37 2024, max compression
+gzip compressed data, was "pykan-0.0.3.tar", last modified: Tue May  7 01:20:49 2024, max compression
```

## Comparing `pykan-0.0.2.tar` & `pykan-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:00:37.450201 pykan-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-29 17:00:29.000000 pykan-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-04-29 17:00:37.450201 pykan-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-04-29 17:00:29.000000 pykan-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:00:37.450201 pykan-0.0.2/kan/
--rw-r--r--   0 runner    (1001) docker     (127)    51663 2024-04-29 17:00:29.000000 pykan-0.0.2/kan/KAN.py
--rw-r--r--   0 runner    (1001) docker     (127)    15013 2024-04-29 17:00:29.000000 pykan-0.0.2/kan/KANLayer.py
--rw-r--r--   0 runner    (1001) docker     (127)    17384 2024-04-29 17:00:29.000000 pykan-0.0.2/kan/LBFGS.py
--rw-r--r--   0 runner    (1001) docker     (127)     7938 2024-04-29 17:00:29.000000 pykan-0.0.2/kan/Symbolic_KANLayer.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-29 17:00:29.000000 pykan-0.0.2/kan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4888 2024-04-29 17:00:29.000000 pykan-0.0.2/kan/spline.py
--rw-r--r--   0 runner    (1001) docker     (127)     9405 2024-04-29 17:00:29.000000 pykan-0.0.2/kan/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:00:37.450201 pykan-0.0.2/pykan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-04-29 17:00:37.000000 pykan-0.0.2/pykan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-29 17:00:37.000000 pykan-0.0.2/pykan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 17:00:37.000000 pykan-0.0.2/pykan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-29 17:00:37.000000 pykan-0.0.2/pykan.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 17:00:37.450201 pykan-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-29 17:00:29.000000 pykan-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:20:49.091100 pykan-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-07 01:20:39.000000 pykan-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13170 2024-05-07 01:20:49.091100 pykan-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12963 2024-05-07 01:20:39.000000 pykan-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:20:49.091100 pykan-0.0.3/kan/
+-rw-r--r--   0 runner    (1001) docker     (127)    51213 2024-05-07 01:20:39.000000 pykan-0.0.3/kan/KAN.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15235 2024-05-07 01:20:39.000000 pykan-0.0.3/kan/KANLayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17384 2024-05-07 01:20:39.000000 pykan-0.0.3/kan/LBFGS.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7991 2024-05-07 01:20:39.000000 pykan-0.0.3/kan/Symbolic_KANLayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-07 01:20:39.000000 pykan-0.0.3/kan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4955 2024-05-07 01:20:39.000000 pykan-0.0.3/kan/spline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9523 2024-05-07 01:20:39.000000 pykan-0.0.3/kan/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:20:49.091100 pykan-0.0.3/pykan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13170 2024-05-07 01:20:49.000000 pykan-0.0.3/pykan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-07 01:20:49.000000 pykan-0.0.3/pykan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 01:20:49.000000 pykan-0.0.3/pykan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-07 01:20:49.000000 pykan-0.0.3/pykan.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 01:20:49.091100 pykan-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-07 01:20:39.000000 pykan-0.0.3/setup.py
```

### Comparing `pykan-0.0.2/LICENSE` & `pykan-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pykan-0.0.2/kan/KAN.py` & `pykan-0.0.3/kan/KAN.py`

 * *Files 9% similar despite different names*

```diff
@@ -72,22 +72,24 @@
         remove_node():
             remove some node of KAN
         auto_symbolic():
             automatically fit all splines to be symbolic functions
         symbolic_formula():
             obtain the symbolic formula of the KAN network
     '''
-    def __init__(self, width=None, grid=3, k=3, noise_scale=0.1, noise_scale_base=0.1, base_fun=torch.nn.SiLU(), symbolic_enabled=True, bias_trainable=True, grid_eps=1.0, grid_range=[-1,1], sp_trainable=True, sb_trainable=True, device='cpu', seed=0):
+
+    def __init__(self, width=None, grid=3, k=3, noise_scale=0.1, noise_scale_base=0.1, base_fun=torch.nn.SiLU(), symbolic_enabled=True, bias_trainable=True, grid_eps=1.0, grid_range=[-1, 1], sp_trainable=True, sb_trainable=True,
+                 device='cpu', seed=0):
         '''
         initalize a KAN model
         
         Args:
         -----
             width : list of int
-                [n0, n1, .., n_{L-1}] specify the number of neurons in each layer (including inputs/outputs)
+                :math:`[n_0, n_1, .., n_{L-1}]` specify the number of neurons in each layer (including inputs/outputs)
             grid : int
                 number of grid intervals. Default: 3.
             k : int
                 order of piecewise polynomial. Default: 3.
             noise_scale : float
                 initial injected noise to spline. Default: 0.1.
             base_fun : fun
@@ -116,55 +118,56 @@
         Example
         -------
         >>> model = KAN(width=[2,5,1], grid=5, k=3)
         >>> (model.act_fun[0].in_dim, model.act_fun[0].out_dim), (model.act_fun[1].in_dim, model.act_fun[1].out_dim)
         ((2, 5), (5, 1))
         '''
         super(KAN, self).__init__()
-        
+
         torch.manual_seed(seed)
         np.random.seed(seed)
         random.seed(seed)
-        
+
         ### initializeing the numerical front ###
-        
+
         self.biases = []
         self.act_fun = []
         self.depth = len(width) - 1
         self.width = width
-        
+
         for l in range(self.depth):
             # splines
-            scale_base = 1/np.sqrt(width[l]) + (torch.randn(width[l]*width[l+1],)*2-1) * noise_scale_base
-            sp_batch = KANLayer(in_dim=width[l],out_dim=width[l+1],num=grid,k=k,noise_scale=noise_scale,scale_base=scale_base, scale_sp=1., base_fun=base_fun, grid_eps=grid_eps, grid_range=grid_range, sp_trainable=sp_trainable, sb_trainable=sb_trainable)
+            scale_base = 1 / np.sqrt(width[l]) + (torch.randn(width[l] * width[l + 1], ) * 2 - 1) * noise_scale_base
+            sp_batch = KANLayer(in_dim=width[l], out_dim=width[l + 1], num=grid, k=k, noise_scale=noise_scale, scale_base=scale_base, scale_sp=1., base_fun=base_fun, grid_eps=grid_eps, grid_range=grid_range, sp_trainable=sp_trainable,
+                                sb_trainable=sb_trainable, device=device)
             self.act_fun.append(sp_batch)
-        
+
             # bias
-            bias = nn.Linear(width[l+1],1,bias=False).requires_grad_(bias_trainable)
-            bias.weight.data *= 0.  
+            bias = nn.Linear(width[l + 1], 1, bias=False, device=device).requires_grad_(bias_trainable)
+            bias.weight.data *= 0.
             self.biases.append(bias)
-        
-        
+
         self.biases = nn.ModuleList(self.biases)
         self.act_fun = nn.ModuleList(self.act_fun)
-        
+
         self.grid = grid
         self.k = k
         self.base_fun = base_fun
-        
+
         ### initializing the symbolic front ###
         self.symbolic_fun = []
         for l in range(self.depth):
-            sb_batch = Symbolic_KANLayer(in_dim=width[l], out_dim=width[l+1])
+            sb_batch = Symbolic_KANLayer(in_dim=width[l], out_dim=width[l + 1], device=device)
             self.symbolic_fun.append(sb_batch)
-            
+
         self.symbolic_fun = nn.ModuleList(self.symbolic_fun)
         self.symbolic_enabled = symbolic_enabled
-    
-    
+        
+        self.device = device
+
     def initialize_from_another_model(self, another_model, x):
         '''
         initialize from a parent model. The parent has the same width as the current model but may have different grids.
         
         Args:
         -----
             another_model : KAN
@@ -183,42 +186,40 @@
         >>> print(model_fine.act_fun[0].coef[0][0].data)
         >>> x = torch.normal(0,1,size=(100,2))
         >>> model_fine.initialize_from_another_model(model_coarse, x);
         >>> print(model_fine.act_fun[0].coef[0][0].data)
         tensor(-0.0030)
         tensor(0.0506)
         '''
-        another_model(x) # get activations
+        another_model(x)  # get activations
         batch = x.shape[0]
-        
+
         self.initialize_grid_from_another_model(another_model, x)
-        
+
         for l in range(self.depth):
             spb = self.act_fun[l]
             spb_parent = another_model.act_fun[l]
-            
-            #spb = spb_parent
+
+            # spb = spb_parent
             preacts = another_model.spline_preacts[l]
             postsplines = another_model.spline_postsplines[l]
-            self.act_fun[l].coef.data = curve2coef(preacts.reshape(batch,spb.size).permute(1,0), postsplines.reshape(batch,spb.size).permute(1,0), spb.grid, k=spb.k)
+            self.act_fun[l].coef.data = curve2coef(preacts.reshape(batch, spb.size).permute(1, 0), postsplines.reshape(batch, spb.size).permute(1, 0), spb.grid, k=spb.k)
             spb.scale_base.data = spb_parent.scale_base.data
             spb.scale_sp.data = spb_parent.scale_sp.data
             spb.mask.data = spb_parent.mask.data
-            #print(spb.mask.data, self.act_fun[l].mask.data)
-            
+            # print(spb.mask.data, self.act_fun[l].mask.data)
+
         for l in range(self.depth):
             self.biases[l].weight.data = another_model.biases[l].weight.data
-            
-            
+
         for l in range(self.depth):
             self.symbolic_fun[l] = another_model.symbolic_fun[l]
 
         return self
-    
-    
+
     def update_grid_from_samples(self, x):
         '''
         update grid from samples
         
         Args:
         -----
             x : 2D torch.float
@@ -237,16 +238,15 @@
         >>> print(model.act_fun[0].grid[0].data)
         tensor([-1.0000, -0.6000, -0.2000,  0.2000,  0.6000,  1.0000])
         tensor([0.0128, 1.0064, 2.0000, 2.9937, 3.9873, 4.9809])
         '''
         for l in range(self.depth):
             self.forward(x)
             self.act_fun[l].update_grid_from_samples(self.acts[l])
-        
-        
+
     def initialize_grid_from_another_model(self, model, x):
         '''
         initialize grid from a parent model
         
         Args:
         -----
             model : KAN
@@ -269,16 +269,15 @@
         >>> print(model.act_fun[0].grid.data)
         tensor([[-1.0000, -0.6000, -0.2000,  0.2000,  0.6000,  1.0000]])
         tensor([[-2.0000, -1.2000, -0.4000,  0.4000,  1.2000,  2.0000]])
         '''
         model(x)
         for l in range(self.depth):
             self.act_fun[l].initialize_grid_from_parent(model.act_fun[l], model.acts[l])
-           
-        
+
     def forward(self, x):
         '''
         KAN forward
         
         Args:
         -----
             x : 2D torch.float
@@ -292,54 +291,53 @@
         Example
         -------
         >>> model = KAN(width=[2,5,3], grid=5, k=3)
         >>> x = torch.normal(0,1,size=(100,2))
         >>> model(x).shape
         torch.Size([100, 3])
         '''
-        
-        self.acts = [] # shape ([batch, n0], [batch, n1], ..., [batch, n_L])
+
+        self.acts = []  # shape ([batch, n0], [batch, n1], ..., [batch, n_L])
         self.spline_preacts = []
         self.spline_postsplines = []
         self.spline_postacts = []
         self.acts_scale = []
         self.acts_scale_std = []
-        #self.neurons_scale = []
-        
-        self.acts.append(x) # acts shape: (batch, width[l])
+        # self.neurons_scale = []
+
+        self.acts.append(x)  # acts shape: (batch, width[l])
 
-        
         for l in range(self.depth):
 
             x_numerical, preacts, postacts_numerical, postspline = self.act_fun[l](x)
 
             if self.symbolic_enabled == True:
                 x_symbolic, postacts_symbolic = self.symbolic_fun[l](x)
             else:
                 x_symbolic = 0.
                 postacts_symbolic = 0.
-            
+
             x = x_numerical + x_symbolic
             postacts = postacts_numerical + postacts_symbolic
-            
-            #self.neurons_scale.append(torch.mean(torch.abs(x), dim=0))
-            grid_reshape = self.act_fun[l].grid.reshape(self.width[l+1],self.width[l],-1)
-            input_range = grid_reshape[:,:,-1] - grid_reshape[:,:,0] + 1e-4
+
+            # self.neurons_scale.append(torch.mean(torch.abs(x), dim=0))
+            grid_reshape = self.act_fun[l].grid.reshape(self.width[l + 1], self.width[l], -1)
+            input_range = grid_reshape[:, :, -1] - grid_reshape[:, :, 0] + 1e-4
             output_range = torch.mean(torch.abs(postacts), dim=0)
-            self.acts_scale.append(output_range/input_range)
+            self.acts_scale.append(output_range / input_range)
             self.acts_scale_std.append(torch.std(postacts, dim=0))
             self.spline_preacts.append(preacts.detach())
-            self.spline_postacts.append(postacts.detach()) 
+            self.spline_postacts.append(postacts.detach())
             self.spline_postsplines.append(postspline.detach())
-            
+
             x = x + self.biases[l].weight
             self.acts.append(x)
-                
-        return x 
-    
+
+        return x
+
     def set_mode(self, l, i, j, mode, mask_n=None):
         '''
         set (l,i,j) activation to have mode 
         
         Args:
         -----
             l : int
@@ -354,31 +352,33 @@
                 magnitude of the numeric front
         
         Returns:
         --------
             None
         '''
         if mode == "s":
-            mask_n = 0.; mask_s = 1.
+            mask_n = 0.;
+            mask_s = 1.
         elif mode == "n":
-            mask_n = 1.; mask_s = 0.
+            mask_n = 1.;
+            mask_s = 0.
         elif mode == "sn" or mode == "ns":
             if mask_n == None:
                 mask_n = 1.
             else:
                 mask_n = mask_n
             mask_s = 1.
         else:
-            mask_n = 0.; mask_s = 0.
-            
-        self.act_fun[l].mask.data[j*self.act_fun[l].in_dim+i] = mask_n
-        self.symbolic_fun[l].mask.data[j,i] = mask_s
-            
-    
-    def fix_symbolic(self, l, i, j, fun_name, fit_params_bool=True, a_range=(-10,10), b_range=(-10,10), verbose=True, random=False):
+            mask_n = 0.;
+            mask_s = 0.
+
+        self.act_fun[l].mask.data[j * self.act_fun[l].in_dim + i] = mask_n
+        self.symbolic_fun[l].mask.data[j, i] = mask_s
+
+    def fix_symbolic(self, l, i, j, fun_name, fit_params_bool=True, a_range=(-10, 10), b_range=(-10, 10), verbose=True, random=False):
         '''
         set (l,i,j) activation to be symbolic (specified by fun_name)
         
         Args:
         -----
             l : int
                 layer index
@@ -427,50 +427,49 @@
         r2 is 0.8131332993507385
         r2 is not very high, please double check if you are choosing the correct symbolic function.
         tensor([[1., 1., 1., 1., 1.],
                 [1., 1., 0., 1., 1.]])
         tensor([[0., 0., 0., 0., 0.],
                 [0., 0., 1., 0., 0.]])
         '''
-        self.set_mode(l,i,j,mode="s")
+        self.set_mode(l, i, j, mode="s")
         if not fit_params_bool:
-            self.symbolic_fun[l].fix_symbolic(i,j,fun_name, verbose=verbose, random=random)
+            self.symbolic_fun[l].fix_symbolic(i, j, fun_name, verbose=verbose, random=random)
             return None
         else:
-            x = self.acts[l][:,i]
-            y = self.spline_postacts[l][:,j,i]
-            r2 = self.symbolic_fun[l].fix_symbolic(i,j,fun_name,x,y,a_range=a_range,b_range=b_range, verbose=verbose)
+            x = self.acts[l][:, i]
+            y = self.spline_postacts[l][:, j, i]
+            r2 = self.symbolic_fun[l].fix_symbolic(i, j, fun_name, x, y, a_range=a_range, b_range=b_range, verbose=verbose)
             return r2
-        
-        
+
     def unfix_symbolic(self, l, i, j):
         '''
         unfix the (l,i,j) activation function.
         '''
-        self.set_mode(l,i,j,mode="n")
-        
+        self.set_mode(l, i, j, mode="n")
+
     def unfix_symbolic_all(self):
         '''
         unfix all activation functions.
         '''
-        for l in range(len(self.width)-1):
+        for l in range(len(self.width) - 1):
             for i in range(self.width[l]):
-                for j in range(self.width[l+1]):
-                    self.unfix_symbolic(l,i,j)
-        
+                for j in range(self.width[l + 1]):
+                    self.unfix_symbolic(l, i, j)
+
     def lock(self, l, ids):
         '''
         lock ids in the l-th layer to be the same function
         
         Args:
         -----
             l : int
                 layer index
             ids : 2D list
-                [[i1,j1],[i2,j2],...] set (l,ii,j1), (l,i2,j2), ... to be the same function
+                :math:`[[i_1,j_1],[i_2,j_2],...]` set :math:`(l,i_i,j_1), (l,i_2,j_2), ...` to be the same function
         
         Returns:
         --------
             None
          
         Example
         -------
@@ -482,15 +481,15 @@
                 [2, 3],
                 [4, 5]])
         tensor([[0, 1],
                 [2, 1],
                 [4, 5]])
         '''
         self.act_fun[l].lock(ids)
-        
+
     def unlock(self, l, ids):
         '''
         unlock ids in the l-th layer to be the same function
         
         Args:
         -----
             l : int
@@ -509,16 +508,15 @@
                 [2, 1],
                 [4, 5]])
         tensor([[0, 1],
                 [2, 3],
                 [4, 5]])
         '''
         self.act_fun[l].unlock(ids)
-        
-        
+
     def get_range(self, l, i, j, verbose=True):
         '''
         Get the input range and output range of the (l,i,j) activation
         
         Args:
         -----
             l : int
@@ -545,26 +543,25 @@
         >>> x = torch.normal(0,1,size=(100,2))
         >>> model(x) # do a forward pass to obtain model.acts
         >>> model.get_range(0,0,0)
         x range: [-2.13 , 2.75 ]
         y range: [-0.50 , 1.83 ]
         (tensor(-2.1288), tensor(2.7498), tensor(-0.5042), tensor(1.8275))
         '''
-        x = self.spline_preacts[l][:,j,i]
-        y = self.spline_postacts[l][:,j,i]
+        x = self.spline_preacts[l][:, j, i]
+        y = self.spline_postacts[l][:, j, i]
         x_min = torch.min(x)
         x_max = torch.max(x)
         y_min = torch.min(y)
         y_max = torch.max(y)
         if verbose:
-            print('x range: ['+'%.2f'%x_min,',','%.2f'%x_max,']')
-            print('y range: ['+'%.2f'%y_min,',','%.2f'%y_max,']')
+            print('x range: [' + '%.2f' % x_min, ',', '%.2f' % x_max, ']')
+            print('y range: [' + '%.2f' % y_min, ',', '%.2f' % y_max, ']')
         return x_min, x_max, y_min, y_max
-    
-    
+
     def plot(self, folder="./figures", beta=3, mask=False, mode="supervised", scale=0.5, tick=False, sample=False, in_vars=None, out_vars=None, title=None):
         '''
         plot KAN
         
         Args:
         -----
             folder : str
@@ -594,189 +591,179 @@
         >>> model = KAN(width=[2,3,1], grid=3, k=3, noise_scale=1.0)
         >>> x = torch.normal(0,1,size=(100,2))
         >>> model(x) # do a forward pass to obtain model.acts
         >>> model.plot()
         '''
         if not os.path.exists(folder):
             os.makedirs(folder)
-        #matplotlib.use('Agg')
+        # matplotlib.use('Agg')
         depth = len(self.width) - 1
         for l in range(depth):
             w_large = 2.0
             for i in range(self.width[l]):
-                for j in range(self.width[l+1]):
-                    rank = torch.argsort(self.acts[l][:,i])
-                    fig, ax = plt.subplots(figsize=(w_large,w_large))
-                    
+                for j in range(self.width[l + 1]):
+                    rank = torch.argsort(self.acts[l][:, i])
+                    fig, ax = plt.subplots(figsize=(w_large, w_large))
+
                     num = rank.shape[0]
-                    
+
                     symbol_mask = self.symbolic_fun[l].mask[j][i]
-                    numerical_mask = self.act_fun[l].mask.reshape(self.width[l+1], self.width[l])[j][i]
+                    numerical_mask = self.act_fun[l].mask.reshape(self.width[l + 1], self.width[l])[j][i]
                     if symbol_mask > 0. and numerical_mask > 0.:
                         color = 'purple'
                         alpha_mask = 1
                     if symbol_mask > 0. and numerical_mask == 0.:
                         color = "red"
                         alpha_mask = 1
                     if symbol_mask == 0. and numerical_mask > 0.:
                         color = "black"
                         alpha_mask = 1
                     if symbol_mask == 0. and numerical_mask == 0.:
                         color = "white"
                         alpha_mask = 0
-                    
+
                     if tick == True:
-                        ax.tick_params(axis="y",direction="in", pad=-22, labelsize=50)
-                        ax.tick_params(axis="x",direction="in", pad=-15, labelsize=50)
-                        x_min, x_max, y_min, y_max = self.get_range(l,i,j,verbose=False)
-                        plt.xticks([x_min, x_max],['%2.f'%x_min, '%2.f'%x_max])
-                        plt.yticks([y_min, y_max],['%2.f'%y_min, '%2.f'%y_max])
+                        ax.tick_params(axis="y", direction="in", pad=-22, labelsize=50)
+                        ax.tick_params(axis="x", direction="in", pad=-15, labelsize=50)
+                        x_min, x_max, y_min, y_max = self.get_range(l, i, j, verbose=False)
+                        plt.xticks([x_min, x_max], ['%2.f' % x_min, '%2.f' % x_max])
+                        plt.yticks([y_min, y_max], ['%2.f' % y_min, '%2.f' % y_max])
                     else:
                         plt.xticks([])
                         plt.yticks([])
                     if alpha_mask == 1:
                         plt.gca().patch.set_edgecolor('black')
                     else:
                         plt.gca().patch.set_edgecolor('white')
-                    plt.gca().patch.set_linewidth(1.5)  
-                    #plt.axis('off')
-                
-                    
-                    plt.plot(self.acts[l][:,i][rank].cpu().detach().numpy(), self.spline_postacts[l][:,j,i][rank].cpu().detach().numpy(), color=color, lw=5)
+                    plt.gca().patch.set_linewidth(1.5)
+                    # plt.axis('off')
+
+                    plt.plot(self.acts[l][:, i][rank].cpu().detach().numpy(), self.spline_postacts[l][:, j, i][rank].cpu().detach().numpy(), color=color, lw=5)
                     if sample == True:
-                        plt.scatter(self.acts[l][:,i][rank].cpu().detach().numpy(), self.spline_postacts[l][:,j,i][rank].cpu().detach().numpy(), color=color, s=400*scale**2)
+                        plt.scatter(self.acts[l][:, i][rank].cpu().detach().numpy(), self.spline_postacts[l][:, j, i][rank].cpu().detach().numpy(), color=color, s=400 * scale ** 2)
                     plt.gca().spines[:].set_color(color)
-                    
-                    lock_id = self.act_fun[l].lock_id[j*self.width[l]+i].long().item()
-                    if  lock_id > 0:
+
+                    lock_id = self.act_fun[l].lock_id[j * self.width[l] + i].long().item()
+                    if lock_id > 0:
                         im = plt.imread(f'{folder}/lock.png')
-                        newax = fig.add_axes([0.15,0.7,0.15,0.15])
-                        plt.text(500,400, lock_id, fontsize=15)
+                        newax = fig.add_axes([0.15, 0.7, 0.15, 0.15])
+                        plt.text(500, 400, lock_id, fontsize=15)
                         newax.imshow(im)
                         newax.axis('off')
 
-                    
                     plt.savefig(f'{folder}/sp_{l}_{i}_{j}.png', bbox_inches="tight", dpi=400)
                     plt.close()
-                    
+
         def score2alpha(score):
-            return np.tanh(beta*score)
+            return np.tanh(beta * score)
 
         if mode == "supervised":
             alpha = [score2alpha(score.cpu().detach().numpy()) for score in self.acts_scale]
         elif mode == "unsupervised":
             alpha = [score2alpha(score.cpu().detach().numpy()) for score in self.acts_scale_std]
-        
+
         # draw skeleton
         width = np.array(self.width)
         A = 1
-        y0 = 0.4 # 0.4
-
+        y0 = 0.4  # 0.4
 
-        #plt.figure(figsize=(5,5*(neuron_depth-1)*y0))
+        # plt.figure(figsize=(5,5*(neuron_depth-1)*y0))
         neuron_depth = len(width)
-        min_spacing = A/np.maximum(np.max(width),5)
+        min_spacing = A / np.maximum(np.max(width), 5)
 
         max_neuron = np.max(width)
         max_num_weights = np.max(width[:-1] * width[1:])
-        y1 = 0.4/np.maximum(max_num_weights,3)
-
-        fig, ax = plt.subplots(figsize=(10*scale,10*scale*(neuron_depth-1)*y0))
-        #fig, ax = plt.subplots(figsize=(5,5*(neuron_depth-1)*y0))
+        y1 = 0.4 / np.maximum(max_num_weights, 3)
 
+        fig, ax = plt.subplots(figsize=(10 * scale, 10 * scale * (neuron_depth - 1) * y0))
+        # fig, ax = plt.subplots(figsize=(5,5*(neuron_depth-1)*y0))
 
         # plot scatters and lines
         for l in range(neuron_depth):
             n = width[l]
-            spacing = A/n
+            spacing = A / n
             for i in range(n):
-                plt.scatter(1/(2*n)+i/n, l*y0, s=min_spacing**2*10000*scale**2, color='black')
+                plt.scatter(1 / (2 * n) + i / n, l * y0, s=min_spacing ** 2 * 10000 * scale ** 2, color='black')
 
                 if l < neuron_depth - 1:
                     # plot connections
-                    n_next = width[l+1]
+                    n_next = width[l + 1]
                     N = n * n_next
                     for j in range(n_next):
-                        id_ = i*n_next + j
+                        id_ = i * n_next + j
 
                         symbol_mask = self.symbolic_fun[l].mask[j][i]
-                        numerical_mask = self.act_fun[l].mask.reshape(self.width[l+1], self.width[l])[j][i]
+                        numerical_mask = self.act_fun[l].mask.reshape(self.width[l + 1], self.width[l])[j][i]
                         if symbol_mask == 1. and numerical_mask == 1.:
                             color = 'purple'
                             alpha_mask = 1.
                         if symbol_mask == 1. and numerical_mask == 0.:
                             color = "red"
                             alpha_mask = 1.
                         if symbol_mask == 0. and numerical_mask == 1.:
                             color = "black"
                             alpha_mask = 1.
                         if symbol_mask == 0. and numerical_mask == 0.:
                             color = "white"
                             alpha_mask = 0.
                         if mask == True:
-                            plt.plot([1/(2*n)+i/n, 1/(2*N)+id_/N], [l*y0, (l+1/2)*y0-y1], color=color, lw=2*scale, alpha=alpha[l][j][i]*self.mask[l][i].item()*self.mask[l+1][j].item())
-                            plt.plot([1/(2*N)+id_/N, 1/(2*n_next)+j/n_next], [(l+1/2)*y0+y1, (l+1)*y0], color=color, lw=2*scale, alpha=alpha[l][j][i]*self.mask[l][i].item()*self.mask[l+1][j].item())
+                            plt.plot([1 / (2 * n) + i / n, 1 / (2 * N) + id_ / N], [l * y0, (l + 1 / 2) * y0 - y1], color=color, lw=2 * scale, alpha=alpha[l][j][i] * self.mask[l][i].item() * self.mask[l + 1][j].item())
+                            plt.plot([1 / (2 * N) + id_ / N, 1 / (2 * n_next) + j / n_next], [(l + 1 / 2) * y0 + y1, (l + 1) * y0], color=color, lw=2 * scale, alpha=alpha[l][j][i] * self.mask[l][i].item() * self.mask[l + 1][j].item())
                         else:
-                            plt.plot([1/(2*n)+i/n, 1/(2*N)+id_/N], [l*y0, (l+1/2)*y0-y1], color=color, lw=2*scale, alpha=alpha[l][j][i]*alpha_mask)
-                            plt.plot([1/(2*N)+id_/N, 1/(2*n_next)+j/n_next], [(l+1/2)*y0+y1, (l+1)*y0], color=color, lw=2*scale, alpha=alpha[l][j][i]*alpha_mask)
-
-            plt.xlim(0,1)
-            plt.ylim(-0.1*y0, (neuron_depth-1+0.1)*y0)
+                            plt.plot([1 / (2 * n) + i / n, 1 / (2 * N) + id_ / N], [l * y0, (l + 1 / 2) * y0 - y1], color=color, lw=2 * scale, alpha=alpha[l][j][i] * alpha_mask)
+                            plt.plot([1 / (2 * N) + id_ / N, 1 / (2 * n_next) + j / n_next], [(l + 1 / 2) * y0 + y1, (l + 1) * y0], color=color, lw=2 * scale, alpha=alpha[l][j][i] * alpha_mask)
 
+            plt.xlim(0, 1)
+            plt.ylim(-0.1 * y0, (neuron_depth - 1 + 0.1) * y0)
 
         # -- Transformation functions
         DC_to_FC = ax.transData.transform
         FC_to_NFC = fig.transFigure.inverted().transform
         # -- Take data coordinates and transform them to normalized figure coordinates
         DC_to_NFC = lambda x: FC_to_NFC(DC_to_FC(x))
 
         plt.axis('off')
 
         # plot splines
-        for l in range(neuron_depth-1):
+        for l in range(neuron_depth - 1):
             n = width[l]
             for i in range(n):
-                n_next = width[l+1]
+                n_next = width[l + 1]
                 N = n * n_next
                 for j in range(n_next):
-                    id_ = i*n_next + j
+                    id_ = i * n_next + j
                     im = plt.imread(f'{folder}/sp_{l}_{i}_{j}.png')
-                    left = DC_to_NFC([1/(2*N)+id_/N-y1,0])[0]
-                    right = DC_to_NFC([1/(2*N)+id_/N+y1,0])[0]
-                    bottom = DC_to_NFC([0,(l+1/2)*y0-y1])[1]
-                    up = DC_to_NFC([0,(l+1/2)*y0+y1])[1]
-                    newax = fig.add_axes([left,bottom,right-left,up-bottom])
-                    #newax = fig.add_axes([1/(2*N)+id_/N-y1, (l+1/2)*y0-y1, y1, y1], anchor='NE')
+                    left = DC_to_NFC([1 / (2 * N) + id_ / N - y1, 0])[0]
+                    right = DC_to_NFC([1 / (2 * N) + id_ / N + y1, 0])[0]
+                    bottom = DC_to_NFC([0, (l + 1 / 2) * y0 - y1])[1]
+                    up = DC_to_NFC([0, (l + 1 / 2) * y0 + y1])[1]
+                    newax = fig.add_axes([left, bottom, right - left, up - bottom])
+                    # newax = fig.add_axes([1/(2*N)+id_/N-y1, (l+1/2)*y0-y1, y1, y1], anchor='NE')
                     if mask == False:
                         newax.imshow(im, alpha=alpha[l][j][i])
                     else:
                         ### make sure to run model.prune() first to compute mask ###
-                        newax.imshow(im, alpha=alpha[l][j][i]*self.mask[l][i].item()*self.mask[l+1][j].item())
+                        newax.imshow(im, alpha=alpha[l][j][i] * self.mask[l][i].item() * self.mask[l + 1][j].item())
                     newax.axis('off')
-                    
-                    
+
         if in_vars != None:
             n = self.width[0]
             for i in range(n):
-                plt.gcf().get_axes()[0].text(1/(2*(n))+i/(n),-0.1,in_vars[i], fontsize=40*scale,horizontalalignment='center', verticalalignment='center')
-                
-                
+                plt.gcf().get_axes()[0].text(1 / (2 * (n)) + i / (n), -0.1, in_vars[i], fontsize=40 * scale, horizontalalignment='center', verticalalignment='center')
+
         if out_vars != None:
             n = self.width[-1]
             for i in range(n):
-                plt.gcf().get_axes()[0].text(1/(2*(n))+i/(n),y0*(len(self.width)-1)+0.1,out_vars[i], fontsize=40*scale,horizontalalignment='center',verticalalignment='center')
-                
+                plt.gcf().get_axes()[0].text(1 / (2 * (n)) + i / (n), y0 * (len(self.width) - 1) + 0.1, out_vars[i], fontsize=40 * scale, horizontalalignment='center', verticalalignment='center')
 
         if title != None:
-            plt.gcf().get_axes()[0].text(0.5,y0*(len(self.width)-1)+0.2,title, fontsize=40*scale,horizontalalignment='center',verticalalignment='center')
-        
-                    
-                    
-                    
-    def train(self, dataset, opt="LBFGS", steps=100, log=1, lamb=0., lamb_l1 = 1., lamb_entropy = 2., lamb_coef = 0., lamb_coefdiff=0., update_grid=True, grid_update_num=10, loss_fn = None, lr=1., stop_grid_update_step=50, batch=-1, small_mag_threshold=1e-16, small_reg_factor=1., metrics=None, sglr_avoid=False, save_fig=False, in_vars=None, out_vars=None, beta=3, save_fig_freq=1, img_folder='./video', device='cpu'):
+            plt.gcf().get_axes()[0].text(0.5, y0 * (len(self.width) - 1) + 0.2, title, fontsize=40 * scale, horizontalalignment='center', verticalalignment='center')
+
+    def train(self, dataset, opt="LBFGS", steps=100, log=1, lamb=0., lamb_l1=1., lamb_entropy=2., lamb_coef=0., lamb_coefdiff=0., update_grid=True, grid_update_num=10, loss_fn=None, lr=1., stop_grid_update_step=50, batch=-1,
+              small_mag_threshold=1e-16, small_reg_factor=1., metrics=None, sglr_avoid=False, save_fig=False, in_vars=None, out_vars=None, beta=3, save_fig_freq=1, img_folder='./video', device='cpu'):
         '''
         training
 
         Args:
         -----
             dataset : dic
                 contains dataset['train_input'], dataset['train_label'], dataset['test_input'], dataset['test_label']
@@ -828,45 +815,43 @@
         >>> f = lambda x: torch.exp(torch.sin(torch.pi*x[:,[0]]) + x[:,[1]]**2)
         >>> dataset = create_dataset(f, n_var=2)
         >>> model.train(dataset, opt='LBFGS', steps=50, lamb=0.01);
         >>> model.plot()
         '''
 
         def reg(acts_scale):
-            
+
             def nonlinear(x, th=small_mag_threshold, factor=small_reg_factor):
-                return (x < th) * x * factor + (x > th) * (x + (factor-1)*th)
-                
+                return (x < th) * x * factor + (x > th) * (x + (factor - 1) * th)
 
             reg_ = 0.
             for i in range(len(acts_scale)):
-                vec = acts_scale[i].reshape(-1,)
-               
-                p = vec/torch.sum(vec)               
-                l1 = torch.sum(nonlinear(vec))                
-                entropy = - torch.sum(p*torch.log2(p+1e-4))                
-                reg_ += lamb_l1 * l1 + lamb_entropy * entropy # both l1 and entropy
+                vec = acts_scale[i].reshape(-1, )
+
+                p = vec / torch.sum(vec)
+                l1 = torch.sum(nonlinear(vec))
+                entropy = - torch.sum(p * torch.log2(p + 1e-4))
+                reg_ += lamb_l1 * l1 + lamb_entropy * entropy  # both l1 and entropy
 
             # regularize coefficient to encourage spline to be zero
             for i in range(len(self.act_fun)):
                 coeff_l1 = torch.sum(torch.mean(torch.abs(self.act_fun[i].coef), dim=1))
-                coeff_diff_l1 = torch.sum(torch.mean(torch.abs(torch.diff(self.act_fun[i].coef)),dim=1))
+                coeff_diff_l1 = torch.sum(torch.mean(torch.abs(torch.diff(self.act_fun[i].coef)), dim=1))
                 reg_ += lamb_coef * coeff_l1 + lamb_coefdiff * coeff_diff_l1
 
             return reg_
 
-
         pbar = tqdm(range(steps), desc='description', ncols=100)
 
         if loss_fn == None:
-            loss_fn = loss_fn_eval = lambda x,y: torch.mean((x-y)**2)
+            loss_fn = loss_fn_eval = lambda x, y: torch.mean((x - y) ** 2)
         else:
             loss_fn = loss_fn_eval = loss_fn
 
-        grid_update_freq = int(stop_grid_update_step/grid_update_num)
+        grid_update_freq = int(stop_grid_update_step / grid_update_num)
 
         if opt == "Adam":
             optimizer = torch.optim.Adam(self.parameters(), lr=lr)
         elif opt == "LBFGS":
             optimizer = LBFGS(self.parameters(), lr=lr, history_size=10, line_search_fn="strong_wolfe", tolerance_grad=1e-32, tolerance_change=1e-32, tolerance_ys=1e-32)
 
         results = {}
@@ -879,86 +864,79 @@
 
         if batch == -1 or batch > dataset['train_input'].shape[0]:
             batch_size = dataset['train_input'].shape[0]
             batch_size_test = dataset['test_input'].shape[0]
         else:
             batch_size = batch
             batch_size_test = batch
-            
+
         global train_loss, reg_
-        
+
         def closure():
             global train_loss, reg_
             optimizer.zero_grad()
             pred = self.forward(dataset['train_input'][train_id].to(device))
-            if sglr_avoid == True:          
+            if sglr_avoid == True:
                 id_ = torch.where(torch.isnan(torch.sum(pred, dim=1)) == False)[0]
                 train_loss = loss_fn(pred[id_], dataset['train_label'][train_id][id_].to(device))
             else:
                 train_loss = loss_fn(pred, dataset['train_label'][train_id].to(device))
             reg_ = reg(self.acts_scale)
-            objective = train_loss + lamb*reg_
+            objective = train_loss + lamb * reg_
             objective.backward()
             return objective
-        
+
         if save_fig:
             if not os.path.exists(img_folder):
                 os.makedirs(img_folder)
 
         for _ in pbar:
 
             train_id = np.random.choice(dataset['train_input'].shape[0], batch_size, replace=False)
             test_id = np.random.choice(dataset['test_input'].shape[0], batch_size_test, replace=False)
 
             if _ % grid_update_freq == 0 and _ < stop_grid_update_step and update_grid:
                 self.update_grid_from_samples(dataset['train_input'][train_id].to(device))
 
-
             if opt == "LBFGS":
                 optimizer.step(closure)
-            
+
             if opt == "Adam":
                 pred = self.forward(dataset['train_input'][train_id].to(device))
-                if sglr_avoid == True:          
+                if sglr_avoid == True:
                     id_ = torch.where(torch.isnan(torch.sum(pred, dim=1)) == False)[0]
                     train_loss = loss_fn(pred[id_], dataset['train_label'][train_id][id_].to(device))
                 else:
                     train_loss = loss_fn(pred, dataset['train_label'][train_id].to(device))
                 reg_ = reg(self.acts_scale)
-                loss = train_loss + lamb*reg_
+                loss = train_loss + lamb * reg_
                 optimizer.zero_grad()
                 loss.backward()
                 optimizer.step()
-                
+
             test_loss = loss_fn_eval(self.forward(dataset['test_input'][test_id].to(device)), dataset['test_label'][test_id].to(device))
-            
+
             if _ % log == 0:
                 pbar.set_description("train loss: %.2e | test loss: %.2e | reg: %.2e " % (torch.sqrt(train_loss).cpu().detach().numpy(), torch.sqrt(test_loss).cpu().detach().numpy(), reg_.cpu().detach().numpy()))
-                    
-                    
+
             if metrics != None:
                 for i in range(len(metrics)):
                     results[metrics[i].__name__].append(metrics[i]().item())
 
-
-
             results['train_loss'].append(torch.sqrt(train_loss).cpu().detach().numpy())
             results['test_loss'].append(torch.sqrt(test_loss).cpu().detach().numpy())
             results['reg'].append(reg_.cpu().detach().numpy())
-            
+
             if save_fig and _ % save_fig_freq == 0:
-                
                 self.plot(folder=img_folder, in_vars=in_vars, out_vars=out_vars, title="Step {}".format(_), beta=beta)
-                plt.savefig(img_folder+'/'+str(_)+'.jpg', bbox_inches='tight', dpi=200)
+                plt.savefig(img_folder + '/' + str(_) + '.jpg', bbox_inches='tight', dpi=200)
                 plt.close()
-            
-            
+
         return results
-    
-    
+
     def prune(self, threshold=1e-2, mode="auto", active_neurons_id=None):
         '''
         pruning KAN on the node level. If a node has small incoming or outgoing connection, it will be pruned away.
         
         Args:
         -----
             threshold : float
@@ -980,50 +958,49 @@
         >>> model = KAN(width=[2,5,1], grid=5, k=3, noise_scale=0.1, seed=0)
         >>> f = lambda x: torch.exp(torch.sin(torch.pi*x[:,[0]]) + x[:,[1]]**2)
         >>> dataset = create_dataset(f, n_var=2)
         >>> model.train(dataset, opt='LBFGS', steps=50, lamb=0.01);
         >>> model.prune()
         >>> model.plot(mask=True)
         '''
-        mask = [torch.ones(self.width[0],)]
+        mask = [torch.ones(self.width[0], )]
         active_neurons = [list(range(self.width[0]))]
-        for i in range(len(self.acts_scale)-1):
+        for i in range(len(self.acts_scale) - 1):
             if mode == "auto":
                 in_important = torch.max(self.acts_scale[i], dim=1)[0] > threshold
-                out_important = torch.max(self.acts_scale[i+1], dim=0)[0] > threshold
+                out_important = torch.max(self.acts_scale[i + 1], dim=0)[0] > threshold
                 overall_important = in_important * out_important
             elif mode == "manual":
-                overall_important = torch.zeros(self.width[i+1], dtype=torch.bool)
-                overall_important[active_neurons_id[i+1]] = True
+                overall_important = torch.zeros(self.width[i + 1], dtype=torch.bool)
+                overall_important[active_neurons_id[i + 1]] = True
             mask.append(overall_important.float())
-            active_neurons.append(torch.where(overall_important==True)[0])
+            active_neurons.append(torch.where(overall_important == True)[0])
         active_neurons.append(list(range(self.width[-1])))
-        mask.append(torch.ones(self.width[-1],))
-        
-        self.mask = mask # this is neuron mask for the whole model
-        
+        mask.append(torch.ones(self.width[-1], ))
+
+        self.mask = mask  # this is neuron mask for the whole model
+
         # update act_fun[l].mask
-        for l in range(len(self.acts_scale)-1):
-            for i in range(self.width[l+1]):
-                if i not in active_neurons[l+1]:
-                    self.remove_node(l+1, i)
-        
-        
-        model2 = KAN(copy.deepcopy(self.width), self.grid, self.k, base_fun=self.base_fun)
+        for l in range(len(self.acts_scale) - 1):
+            for i in range(self.width[l + 1]):
+                if i not in active_neurons[l + 1]:
+                    self.remove_node(l + 1, i)
+
+        model2 = KAN(copy.deepcopy(self.width), self.grid, self.k, base_fun=self.base_fun, device=self.device)
         model2.load_state_dict(self.state_dict())
         for i in range(len(self.acts_scale)):
             if i < len(self.acts_scale) - 1:
-                model2.biases[i].weight.data = model2.biases[i].weight.data[:,active_neurons[i+1]]
-            
-            model2.act_fun[i] = model2.act_fun[i].get_subset(active_neurons[i], active_neurons[i+1])
+                model2.biases[i].weight.data = model2.biases[i].weight.data[:, active_neurons[i + 1]]
+
+            model2.act_fun[i] = model2.act_fun[i].get_subset(active_neurons[i], active_neurons[i + 1])
             model2.width[i] = len(active_neurons[i])
-            model2.symbolic_fun[i] = self.symbolic_fun[i].get_subset(active_neurons[i], active_neurons[i+1])
-            
+            model2.symbolic_fun[i] = self.symbolic_fun[i].get_subset(active_neurons[i], active_neurons[i + 1])
+
         return model2
-    
+
     def remove_edge(self, l, i, j):
         '''
         remove activtion phi(l,i,j) (set its mask to zero)
         
         Args:
         -----
             l : int
@@ -1033,16 +1010,16 @@
             j : int
                 output neuron index
         
         Returns:
         --------
             None
         '''
-        self.act_fun[l].mask[j*self.width[l]+i] = 0.
-        
+        self.act_fun[l].mask[j * self.width[l] + i] = 0.
+
     def remove_node(self, l, i):
         '''
         remove neuron (l,i) (set the masks of all incoming and outgoing activation functions to zero)
         
         Args:
         -----
             l : int
@@ -1050,21 +1027,20 @@
             i : int
                 neuron index
         
         Returns:
         --------
             None
         '''
-        self.act_fun[l-1].mask[i*self.width[l-1]+torch.arange(self.width[l-1])] = 0.
-        self.act_fun[l].mask[torch.arange(self.width[l+1])*self.width[l]+i] = 0.
-        self.symbolic_fun[l-1].mask[i,:] *= 0.
-        self.symbolic_fun[l].mask[:,i] *= 0.
-        
-        
-    def suggest_symbolic(self, l, i, j, a_range=(-10,10), b_range=(-10,10), lib = None, topk=5, verbose=True):
+        self.act_fun[l - 1].mask[i * self.width[l - 1] + torch.arange(self.width[l - 1])] = 0.
+        self.act_fun[l].mask[torch.arange(self.width[l + 1]) * self.width[l] + i] = 0.
+        self.symbolic_fun[l - 1].mask[i, :] *= 0.
+        self.symbolic_fun[l].mask[:, i] *= 0.
+
+    def suggest_symbolic(self, l, i, j, a_range=(-10, 10), b_range=(-10, 10), lib=None, topk=5, verbose=True):
         '''suggest the symbolic candidates of phi(l,i,j)
         
         Args:
         -----
             l : int
                 layer index
             i : int 
@@ -1095,43 +1071,42 @@
         sin , 0.9994412064552307
         gaussian , 0.9196369051933289
         tanh , 0.8608126044273376
         sigmoid , 0.8578218817710876
         arctan , 0.842217743396759
         '''
         r2s = []
-        
+
         if lib == None:
             symbolic_lib = SYMBOLIC_LIB
         else:
             symbolic_lib = {}
             for item in lib:
                 symbolic_lib[item] = SYMBOLIC_LIB[item]
-        
+
         for (name, fun) in symbolic_lib.items():
-            r2 = self.fix_symbolic(l,i,j,name,a_range=a_range,b_range=b_range,verbose=False)
+            r2 = self.fix_symbolic(l, i, j, name, a_range=a_range, b_range=b_range, verbose=False)
             r2s.append(r2.item())
-            
-        self.unfix_symbolic(l,i,j)
+
+        self.unfix_symbolic(l, i, j)
 
         sorted_ids = np.argsort(r2s)[::-1][:topk]
         r2s = np.array(r2s)[sorted_ids][:topk]
         topk = np.minimum(topk, len(symbolic_lib))
         if verbose == True:
-            print('function',',','r2')
+            print('function', ',', 'r2')
             for i in range(topk):
-                print(list(symbolic_lib.items())[sorted_ids[i]][0],',',r2s[i])
-        
+                print(list(symbolic_lib.items())[sorted_ids[i]][0], ',', r2s[i])
+
         best_name = list(symbolic_lib.items())[sorted_ids[0]][0]
         best_fun = list(symbolic_lib.items())[sorted_ids[0]][1]
         best_r2 = r2s[0]
         return best_name, best_fun, best_r2
-    
-    
-    def auto_symbolic(self, a_range=(-10,10), b_range=(-10,10), lib=None, verbose=1):
+
+    def auto_symbolic(self, a_range=(-10, 10), b_range=(-10, 10), lib=None, verbose=1):
         '''
         automatic symbolic regression: using top 1 suggestion from suggest_symbolic to replace splines with symbolic activations
         
         Args:
         -----
             lib : None or a list of function names
                 the symbolic library 
@@ -1168,28 +1143,25 @@
         >>> >>> model = model.prune()
         >>> model(dataset['train_input'])
         >>> model.auto_symbolic(lib=['exp','sin','x^2'])
         fixing (0,0,0) with sin, r2=0.999411404132843
         fixing (0,1,0) with x^2, r2=0.9962921738624573
         fixing (1,0,0) with exp, r2=0.9980258941650391
         '''
-        for l in range(len(self.width)-1):
+        for l in range(len(self.width) - 1):
             for i in range(self.width[l]):
-                for j in range(self.width[l+1]):
-                    if self.symbolic_fun[l].mask[j,i] > 0.:
+                for j in range(self.width[l + 1]):
+                    if self.symbolic_fun[l].mask[j, i] > 0.:
                         print(f'skipping ({l},{i},{j}) since already symbolic')
                     else:
                         name, fun, r2 = self.suggest_symbolic(l, i, j, a_range=a_range, b_range=b_range, lib=lib, verbose=False)
-                        self.fix_symbolic(l,i,j,name,verbose=verbose>1)
+                        self.fix_symbolic(l, i, j, name, verbose=verbose > 1)
                         if verbose >= 1:
                             print(f'fixing ({l},{i},{j}) with {name}, r2={r2}')
-                    
-                        
-                        
-          
+
     def symbolic_formula(self, floating_digit=2, var=None, normalizer=None, simplify=False):
         '''
         obtain the symbolic formula
         
         Args:
         -----
             floating_digit : int
@@ -1225,71 +1197,69 @@
             for a in sympy.preorder_traversal(ex1):
                 if isinstance(a, sympy.Float):
                     ex2 = ex2.subs(a, round(a, floating_digit))
             return ex2
 
         # define variables
         if var == None:
-            for ii in range(1,self.width[0]+1):
+            for ii in range(1, self.width[0] + 1):
                 exec(f"x{ii} = sympy.Symbol('x_{ii}')")
                 exec(f"x.append(x{ii})")
         else:
             x = [sympy.symbols(var_) for var_ in var]
-            
+
         x0 = x
-            
+
         if normalizer != None:
             mean = normalizer[0]
             std = normalizer[1]
-            x = [(x[i] - mean[i])/std[i] for i in range(len(x))]
-
+            x = [(x[i] - mean[i]) / std[i] for i in range(len(x))]
 
         symbolic_acts.append(x)
 
-        for l in range(len(self.width)-1):
+        for l in range(len(self.width) - 1):
             y = []
-            for j in range(self.width[l+1]):
+            for j in range(self.width[l + 1]):
                 yj = 0.
                 for i in range(self.width[l]):
-                    a, b, c, d = self.symbolic_fun[l].affine[j,i]
+                    a, b, c, d = self.symbolic_fun[l].affine[j, i]
                     sympy_fun = self.symbolic_fun[l].funs_sympy[j][i]
                     try:
-                        yj += c*sympy_fun(a*x[i]+b)+d
+                        yj += c * sympy_fun(a * x[i] + b) + d
                     except:
                         print('make sure all activations need to be converted to symbolic formulas first!')
                         return
                 if simplify == True:
-                    y.append(sympy.simplify(yj + self.biases[l].weight.data[0,j]))
+                    y.append(sympy.simplify(yj + self.biases[l].weight.data[0, j]))
                 else:
-                    y.append(yj + self.biases[l].weight.data[0,j])
+                    y.append(yj + self.biases[l].weight.data[0, j])
 
             x = y
             symbolic_acts.append(x)
 
         self.symbolic_acts = [[ex_round(symbolic_acts[l][i]) for i in range(len(symbolic_acts[l]))] for l in range(len(symbolic_acts))]
 
         out_dim = len(symbolic_acts[-1])
         return [ex_round(symbolic_acts[-1][i]) for i in range(len(symbolic_acts[-1]))], x0
-    
-    
+
     def clear_ckpts(self, folder='./model_ckpt'):
         '''
         clear all checkpoints
         
         Args:
         -----
             folder : str
                 the folder that stores checkpoints
         
         Returns:
         --------
             None
         '''
         if os.path.exists(folder):
-            files = glob.glob(folder+'/*')
+            files = glob.glob(folder + '/*')
             for f in files:
                 os.remove(f)
         else:
             os.makedirs(folder)
 
     def save_ckpt(self, name, folder='./model_ckpt'):
         '''
@@ -1306,16 +1276,16 @@
         --------
             None
         '''
 
         if not os.path.exists(folder):
             os.makedirs(folder)
 
-        torch.save(self.state_dict(), folder+'/'+name)
-        print('save this model to', folder+'/'+name)
+        torch.save(self.state_dict(), folder + '/' + name)
+        print('save this model to', folder + '/' + name)
 
     def load_ckpt(self, name, folder='./model_ckpt'):
         '''
         load a checkpoint to the current model
         
         Args:
         -----
@@ -1324,8 +1294,8 @@
             folder : str
                 the folder that stores checkpoints
                
         Returns:
         --------
             None
         '''
-        self.load_state_dict(torch.load(folder+'/'+name))
+        self.load_state_dict(torch.load(folder + '/' + name))
```

### Comparing `pykan-0.0.2/kan/KANLayer.py` & `pykan-0.0.3/kan/KANLayer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import torch
 import torch.nn as nn
 import numpy as np
 from .spline import *
-import inspect
 
 
 class KANLayer(nn.Module):
     """
     KANLayer class
     
 
@@ -59,15 +58,15 @@
             get subset of the KANLayer (used for pruning)
         lock():
             lock several activation functions to share parameters
         unlock():
             unlock already locked activation functions
     """
 
-    def __init__(self, in_dim=3, out_dim=2, num=5, k=3, noise_scale=0.1, scale_base=1.0, scale_sp=1.0, base_fun=torch.nn.SiLU(), grid_eps=0.02, grid_range=[-1,1], sp_trainable=True, sb_trainable=True, device='cpu'):
+    def __init__(self, in_dim=3, out_dim=2, num=5, k=3, noise_scale=0.1, scale_base=1.0, scale_sp=1.0, base_fun=torch.nn.SiLU(), grid_eps=0.02, grid_range=[-1, 1], sp_trainable=True, sb_trainable=True, device='cpu'):
         ''''
         initialize a KANLayer
         
         Args:
         -----
             in_dim : int
                 input dimension. Default: 2.
@@ -104,42 +103,41 @@
         -------
         >>> model = KANLayer(in_dim=3, out_dim=5)
         >>> (model.in_dim, model.out_dim)
         (3, 5)
         '''
         super(KANLayer, self).__init__()
         # size 
-        self.size = size = out_dim*in_dim
+        self.size = size = out_dim * in_dim
         self.out_dim = out_dim
         self.in_dim = in_dim
         self.num = num
         self.k = k
-        
+
         # shape: (size, num)
-        self.grid = torch.einsum('i,j->ij', torch.ones(size,), torch.linspace(grid_range[0],grid_range[1],steps=num+1))
+        self.grid = torch.einsum('i,j->ij', torch.ones(size, device=device), torch.linspace(grid_range[0], grid_range[1], steps=num + 1, device=device))
         self.grid = torch.nn.Parameter(self.grid).requires_grad_(False)
-        noises = (torch.rand(size,self.grid.shape[1])-1/2)*noise_scale/num
+        noises = (torch.rand(size, self.grid.shape[1]) - 1 / 2) * noise_scale / num
         noises = noises.to(device)
         # shape: (size, coef)
-        self.coef = torch.nn.Parameter(curve2coef(self.grid, noises, self.grid, k))
+        self.coef = torch.nn.Parameter(curve2coef(self.grid, noises, self.grid, k, device))
         if isinstance(scale_base, float):
-            self.scale_base = torch.nn.Parameter(torch.ones(size,) * scale_base).requires_grad_(sb_trainable)  # make scale trainable
+            self.scale_base = torch.nn.Parameter(torch.ones(size, device=device) * scale_base).requires_grad_(sb_trainable)  # make scale trainable
         else:
-            self.scale_base = torch.nn.Parameter(scale_base).requires_grad_(sb_trainable)
-        self.scale_sp = torch.nn.Parameter(torch.ones(size,) * scale_sp).requires_grad_(sp_trainable) # make scale trainable
+            self.scale_base = torch.nn.Parameter(torch.FloatTensor(scale_base).cuda()).requires_grad_(sb_trainable)
+        self.scale_sp = torch.nn.Parameter(torch.ones(size, device=device) * scale_sp).requires_grad_(sp_trainable)  # make scale trainable
         self.base_fun = base_fun
-        
-        self.mask = torch.nn.Parameter(torch.ones(size,)).requires_grad_(False)
+
+        self.mask = torch.nn.Parameter(torch.ones(size, device=device)).requires_grad_(False)
         self.grid_eps = grid_eps
         self.weight_sharing = torch.arange(size)
         self.lock_counter = 0
         self.lock_id = torch.zeros(size)
         self.device = device
-        
-    
+
     def forward(self, x):
         '''
         KANLayer forward given input x
         
         Args:
         -----
             x : 2D torch.float
@@ -165,29 +163,29 @@
         (torch.Size([100, 5]),
          torch.Size([100, 5, 3]),
          torch.Size([100, 5, 3]),
          torch.Size([100, 5, 3]))
         '''
         batch = x.shape[0]
         # x: shape (batch, in_dim) => shape (size, batch) (size = out_dim * in_dim)
-        x = torch.einsum('ij,k->ikj', x, torch.ones(self.out_dim,).to(self.device)).reshape(batch, self.size).permute(1,0)
-        preacts = x.permute(1,0).clone().reshape(batch, self.out_dim, self.in_dim)
-        base = self.base_fun(x).permute(1,0) # shape (batch, size)
-        y = coef2curve(x_eval=x, grid=self.grid[self.weight_sharing], coef=self.coef[self.weight_sharing], k=self.k) # shape (size, batch)
-        y = y.permute(1,0) # shape (batch, size)
+        x = torch.einsum('ij,k->ikj', x, torch.ones(self.out_dim, device=self.device)).reshape(batch, self.size).permute(1, 0)
+        preacts = x.permute(1, 0).clone().reshape(batch, self.out_dim, self.in_dim)
+        base = self.base_fun(x).permute(1, 0)  # shape (batch, size)
+        y = coef2curve(x_eval=x, grid=self.grid[self.weight_sharing], coef=self.coef[self.weight_sharing], k=self.k, device=self.device)  # shape (size, batch)
+        y = y.permute(1, 0)  # shape (batch, size)
         postspline = y.clone().reshape(batch, self.out_dim, self.in_dim)
         y = self.scale_base.unsqueeze(dim=0) * base + self.scale_sp.unsqueeze(dim=0) * y
-        y = self.mask[None,:] * y
+        y = self.mask[None, :] * y
         postacts = y.clone().reshape(batch, self.out_dim, self.in_dim)
-        y = torch.sum(y.reshape(batch, self.out_dim, self.in_dim), dim=2) # shape (batch, out_dim)
+        y = torch.sum(y.reshape(batch, self.out_dim, self.in_dim), dim=2)  # shape (batch, out_dim)
         # y shape: (batch, out_dim); preacts shape: (batch, in_dim, out_dim)
         # postspline shape: (batch, in_dim, out_dim); postacts: (batch, in_dim, out_dim)
         # postspline is for extension; postacts is for visualization
         return y, preacts, postacts, postspline
-    
+
     def update_grid_from_samples(self, x):
         '''
         update grid from samples
         
         Args:
         -----
             x : 2D torch.float
@@ -204,26 +202,25 @@
         >>> x = torch.linspace(-3,3,steps=100)[:,None]
         >>> model.update_grid_from_samples(x)
         >>> print(model.grid.data)
         tensor([[-1.0000, -0.6000, -0.2000,  0.2000,  0.6000,  1.0000]])
         tensor([[-3.0002, -1.7882, -0.5763,  0.6357,  1.8476,  3.0002]])
         '''
         batch = x.shape[0]
-        x = torch.einsum('ij,k->ikj', x, torch.ones(self.out_dim,).to(self.device)).reshape(batch, self.size).permute(1,0)
+        x = torch.einsum('ij,k->ikj', x, torch.ones(self.out_dim, ).to(self.device)).reshape(batch, self.size).permute(1, 0)
         x_pos = torch.sort(x, dim=1)[0]
-        y_eval = coef2curve(x_pos, self.grid, self.coef, self.k)
+        y_eval = coef2curve(x_pos, self.grid, self.coef, self.k, device=self.device)
         num_interval = self.grid.shape[1] - 1
-        ids = [int(batch/num_interval*i) for i in range(num_interval)] + [-1]
+        ids = [int(batch / num_interval * i) for i in range(num_interval)] + [-1]
         grid_adaptive = x_pos[:, ids]
         margin = 0.01
-        grid_uniform = torch.cat([grid_adaptive[:,[0]] - margin  + (grid_adaptive[:,[-1]] - grid_adaptive[:,[0]] + 2*margin)*a for a in np.linspace(0,1,num=self.grid.shape[1])], dim=1)
-        self.grid.data = self.grid_eps * grid_uniform + (1-self.grid_eps) * grid_adaptive
-        self.coef.data = curve2coef(x_pos, y_eval, self.grid, self.k)
-        
-        
+        grid_uniform = torch.cat([grid_adaptive[:, [0]] - margin + (grid_adaptive[:, [-1]] - grid_adaptive[:, [0]] + 2 * margin) * a for a in np.linspace(0, 1, num=self.grid.shape[1])], dim=1)
+        self.grid.data = self.grid_eps * grid_uniform + (1 - self.grid_eps) * grid_adaptive
+        self.coef.data = curve2coef(x_pos, y_eval, self.grid, self.k, device=self.device)
+
     def initialize_grid_from_parent(self, parent, x):
         '''
         update grid from a parent KANLayer & samples
         
         Args:
         -----
             parent : KANLayer
@@ -246,24 +243,23 @@
         >>> print(model.grid.data)
         tensor([[-1.0000, -0.6000, -0.2000,  0.2000,  0.6000,  1.0000]])
         tensor([[-1.0000, -0.8000, -0.6000, -0.4000, -0.2000,  0.0000,  0.2000,  0.4000,
           0.6000,  0.8000,  1.0000]])
         '''
         batch = x.shape[0]
         # preacts: shape (batch, in_dim) => shape (size, batch) (size = out_dim * in_dim)
-        x_eval = torch.einsum('ij,k->ikj', x, torch.ones(self.out_dim,).to(self.device)).reshape(batch, self.size).permute(1,0)
+        x_eval = torch.einsum('ij,k->ikj', x, torch.ones(self.out_dim, ).to(self.device)).reshape(batch, self.size).permute(1, 0)
         x_pos = parent.grid
-        sp2 = KANLayer(in_dim=1,out_dim=self.size,k=1,num=x_pos.shape[1]-1,scale_base=0.).to(self.device)
+        sp2 = KANLayer(in_dim=1, out_dim=self.size, k=1, num=x_pos.shape[1] - 1, scale_base=0.).to(self.device)
         sp2.coef.data = curve2coef(sp2.grid, x_pos, sp2.grid, k=1)
-        y_eval = coef2curve(x_eval, parent.grid, parent.coef, parent.k)
-        percentile = torch.linspace(-1,1,self.num+1).to(self.device)
-        self.grid.data = sp2(percentile.unsqueeze(dim=1))[0].permute(1,0)
-        self.coef.data = curve2coef(x_eval, y_eval, self.grid, self.k)
-        
-        
+        y_eval = coef2curve(x_eval, parent.grid, parent.coef, parent.k, device=self.device)
+        percentile = torch.linspace(-1, 1, self.num + 1).to(self.device)
+        self.grid.data = sp2(percentile.unsqueeze(dim=1))[0].permute(1, 0)
+        self.coef.data = curve2coef(x_eval, y_eval, self.grid, self.k, self.device)
+
     def get_subset(self, in_id, out_id):
         '''
         get a smaller KANLayer from a larger KANLayer (used for pruning)
         
         Args:
         -----
             in_id : list
@@ -278,26 +274,26 @@
         Example
         -------
         >>> kanlayer_large = KANLayer(in_dim=10, out_dim=10, num=5, k=3)
         >>> kanlayer_small = kanlayer_large.get_subset([0,9],[1,2,3])
         >>> kanlayer_small.in_dim, kanlayer_small.out_dim
         (2, 3)
         '''
-        spb = KANLayer(len(in_id), len(out_id), self.num, self.k, base_fun=self.base_fun)
-        spb.grid.data = self.grid.reshape(self.out_dim,self.in_dim,spb.num+1)[out_id][:,in_id].reshape(-1,spb.num+1)
-        spb.coef.data = self.coef.reshape(self.out_dim,self.in_dim,spb.coef.shape[1])[out_id][:,in_id].reshape(-1,spb.coef.shape[1])
-        spb.scale_base.data = self.scale_base.reshape(self.out_dim,self.in_dim)[out_id][:,in_id].reshape(-1,)
-        spb.scale_sp.data = self.scale_sp.reshape(self.out_dim,self.in_dim)[out_id][:,in_id].reshape(-1,)
-        spb.mask.data = self.mask.reshape(self.out_dim,self.in_dim)[out_id][:,in_id].reshape(-1,)
-        
+        spb = KANLayer(len(in_id), len(out_id), self.num, self.k, base_fun=self.base_fun, device=self.device)
+        spb.grid.data = self.grid.reshape(self.out_dim, self.in_dim, spb.num + 1)[out_id][:, in_id].reshape(-1, spb.num + 1)
+        spb.coef.data = self.coef.reshape(self.out_dim, self.in_dim, spb.coef.shape[1])[out_id][:, in_id].reshape(-1, spb.coef.shape[1])
+        spb.scale_base.data = self.scale_base.reshape(self.out_dim, self.in_dim)[out_id][:, in_id].reshape(-1, )
+        spb.scale_sp.data = self.scale_sp.reshape(self.out_dim, self.in_dim)[out_id][:, in_id].reshape(-1, )
+        spb.mask.data = self.mask.reshape(self.out_dim, self.in_dim)[out_id][:, in_id].reshape(-1, )
+
         spb.in_dim = len(in_id)
         spb.out_dim = len(out_id)
         spb.size = spb.in_dim * spb.out_dim
         return spb
-    
+
     def lock(self, ids):
         '''
         lock activation functions to share parameters based on ids
         
         Args:
         -----
             ids : list
@@ -320,17 +316,17 @@
                 [3, 4, 0],
                 [6, 0, 8]])
         '''
         self.lock_counter += 1
         # ids: [[i1,j1],[i2,j2],[i3,j3],...]
         for i in range(len(ids)):
             if i != 0:
-                self.weight_sharing[ids[i][1]*self.in_dim+ids[i][0]] = ids[0][1]*self.in_dim+ids[0][0]
-            self.lock_id[ids[i][1]*self.in_dim+ids[i][0]] = self.lock_counter
-        
+                self.weight_sharing[ids[i][1] * self.in_dim + ids[i][0]] = ids[0][1] * self.in_dim + ids[0][0]
+            self.lock_id[ids[i][1] * self.in_dim + ids[i][0]] = self.lock_counter
+
     def unlock(self, ids):
         '''
         unlock activation functions
         
         Args:
         -----
             ids : list
@@ -354,17 +350,15 @@
                 [3, 4, 5],
                 [6, 7, 8]])
         '''
         # check ids are locked
         num = len(ids)
         locked = True
         for i in range(num):
-            locked *= (self.weight_sharing[ids[i][1]*self.in_dim+ids[i][0]] == self.weight_sharing[ids[0][1]*self.in_dim+ids[0][0]])
+            locked *= (self.weight_sharing[ids[i][1] * self.in_dim + ids[i][0]] == self.weight_sharing[ids[0][1] * self.in_dim + ids[0][0]])
         if locked == False:
             print("they are not locked. unlock failed.")
             return 0
         for i in range(len(ids)):
-            self.weight_sharing[ids[i][1]*self.in_dim+ids[i][0]] = ids[i][1]*self.in_dim+ids[i][0]
-            self.lock_id[ids[i][1]*self.in_dim+ids[i][0]] = 0
+            self.weight_sharing[ids[i][1] * self.in_dim + ids[i][0]] = ids[i][1] * self.in_dim + ids[i][0]
+            self.lock_id[ids[i][1] * self.in_dim + ids[i][0]] = 0
         self.lock_counter -= 1
-
-
```

### Comparing `pykan-0.0.2/kan/LBFGS.py` & `pykan-0.0.3/kan/LBFGS.py`

 * *Files identical despite different names*

### Comparing `pykan-0.0.2/kan/Symbolic_KANLayer.py` & `pykan-0.0.3/kan/Symbolic_KANLayer.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,48 +32,52 @@
         forward():
             forward
         get_subset():
             get subset of the KANLayer (used for pruning)
         fix_symbolic():
             fix an activation function to be symbolic
     '''
-    def __init__(self, in_dim=3, out_dim=2):
+    def __init__(self, in_dim=3, out_dim=2, device='cpu'):
         '''
         initialize a Symbolic_KANLayer (activation functions are initialized to be identity functions)
         
         Args:
         -----
             in_dim : int
                 input dimension
             out_dim : int
                 output dimension
+            device : str
+                device
             
         Returns:
         --------
             self
             
         Example
         -------
         >>> sb = Symbolic_KANLayer(in_dim=3, out_dim=3)
         >>> len(sb.funs), len(sb.funs[0])
         (3, 3)
         '''
         super(Symbolic_KANLayer, self).__init__()
         self.out_dim = out_dim
         self.in_dim = in_dim
-        self.mask = torch.nn.Parameter(torch.zeros(out_dim, in_dim)).requires_grad_(False)
+        self.mask = torch.nn.Parameter(torch.zeros(out_dim, in_dim, device=device)).requires_grad_(False)
         # torch
         self.funs = [[lambda x: x for i in range(self.in_dim)] for j in range(self.out_dim)]
         # name
         self.funs_name = [['' for i in range(self.in_dim)] for j in range(self.out_dim)]
         # sympy
         self.funs_sympy = [['' for i in range(self.in_dim)] for j in range(self.out_dim)]
         
-        self.affine = torch.nn.Parameter(torch.zeros(out_dim, in_dim, 4))
+        self.affine = torch.nn.Parameter(torch.zeros(out_dim, in_dim, 4, device=device))
         # c*f(a*x+b)+d
+        
+        self.device = device
     
     def forward(self, x):
         '''
         forward
         
         Args:
         -----
@@ -131,15 +135,15 @@
         Example
         -------
         >>> sb_large = Symbolic_KANLayer(in_dim=10, out_dim=10)
         >>> sb_small = sb_large.get_subset([0,9],[1,2,3])
         >>> sb_small.in_dim, sb_small.out_dim
         (2, 3)
         '''
-        sbb = Symbolic_KANLayer(self.in_dim, self.out_dim)
+        sbb = Symbolic_KANLayer(self.in_dim, self.out_dim, device=self.device)
         sbb.in_dim = len(in_id)
         sbb.out_dim = len(out_id)
         sbb.mask.data = self.mask.data[out_id][:,in_id]
         sbb.funs = [[self.funs[j][i] for i in in_id] for j in out_id]
         sbb.funs_sympy = [[self.funs_sympy[j][i] for i in in_id] for j in out_id]
         sbb.funs_name = [[self.funs_name[j][i] for i in in_id] for j in out_id]
         sbb.affine.data = self.affine.data[out_id][:,in_id]
@@ -178,22 +182,17 @@
         >>> # when x & y are not provided. Affine parameters are set to a = 1, b = 0, c = 1, d = 0
         >>> sb = Symbolic_KANLayer(in_dim=3, out_dim=2)
         >>> sb.fix_symbolic(2,1,'sin')
         >>> print(sb.funs_name)
         >>> print(sb.affine)
         [['', '', ''], ['', '', 'sin']]
         Parameter containing:
-        tensor([[[0., 0., 0., 0.],
-                 [0., 0., 0., 0.],
-                 [0., 0., 0., 0.]],
-
-                [[0., 0., 0., 0.],
+        tensor([[0., 0., 0., 0.],
                  [0., 0., 0., 0.],
-                 [1., 0., 1., 0.]]], requires_grad=True)
-        
+                 [1., 0., 1., 0.]], requires_grad=True)
         Example 2
         ---------
         >>> # when x & y are provided, fit_params() is called to find the best fit coefficients
         >>> sb = Symbolic_KANLayer(in_dim=3, out_dim=2)
         >>> batch = 100
         >>> x = torch.linspace(-1,1,steps=batch)
         >>> noises = torch.normal(0,1,(batch,)) * 0.02
@@ -216,15 +215,15 @@
                 if random == False:
                     self.affine.data[j][i] = torch.tensor([1.,0.,1.,0.])
                 else:
                     self.affine.data[j][i] = torch.rand(4,) * 2 - 1
                 return None
             else:
                 #initialize from x & y and fun
-                params, r2 = fit_params(x,y,fun, a_range=a_range, b_range=b_range, verbose=verbose)
+                params, r2 = fit_params(x,y,fun, a_range=a_range, b_range=b_range, verbose=verbose, device=self.device)
                 self.funs[j][i] = fun
                 self.affine.data[j][i] = params
                 return r2
         else:
             # if fun_name itself is a function
             fun = fun_name
             fun_sympy = fun_name
@@ -232,8 +231,8 @@
             self.funs_name[j][i] = "anonymous"
 
             self.funs[j][i] = fun
             if random == False:
                 self.affine.data[j][i] = torch.tensor([1.,0.,1.,0.])
             else:
                 self.affine.data[j][i] = torch.rand(4,) * 2 - 1
-            return None
+            return None
```

### Comparing `pykan-0.0.2/kan/spline.py` & `pykan-0.0.3/kan/spline.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,37 +30,38 @@
     >>> num_grid_interval = 10
     >>> k = 3
     >>> x = torch.normal(0,1,size=(num_spline, num_sample))
     >>> grids = torch.einsum('i,j->ij', torch.ones(num_spline,), torch.linspace(-1,1,steps=num_grid_interval+1))
     >>> B_batch(x, grids, k=k).shape
     torch.Size([5, 13, 100])
     '''
+
     # x shape: (size, x); grid shape: (size, grid)
     def extend_grid(grid, k_extend=0):
         # pad k to left and right
         # grid shape: (batch, grid)
-        h = (grid[:,[-1]] - grid[:,[0]])/(grid.shape[1]-1)
+        h = (grid[:, [-1]] - grid[:, [0]]) / (grid.shape[1] - 1)
 
         for i in range(k_extend):
-            grid = torch.cat([grid[:,[0]]-h, grid], dim=1)
-            grid = torch.cat([grid, grid[:,[-1]]+h], dim=1)
+            grid = torch.cat([grid[:, [0]] - h, grid], dim=1)
+            grid = torch.cat([grid, grid[:, [-1]] + h], dim=1)
         grid = grid.to(device)
         return grid
-    
+
     if extend == True:
         grid = extend_grid(grid, k_extend=k)
-        
+
     grid = grid.unsqueeze(dim=2).to(device)
     x = x.unsqueeze(dim=1).to(device)
-    
-    if k==0:
-        value = (x>=grid[:,:-1])*(x<grid[:,1:])
+
+    if k == 0:
+        value = (x >= grid[:, :-1]) * (x < grid[:, 1:])
     else:
-        B_km1 = B_batch(x[:,0],grid=grid[:,:,0],k=k-1,extend=False)
-        value = (x-grid[:,:-(k+1)])/(grid[:,k:-1]-grid[:,:-(k+1)])*B_km1[:,:-1]+ (grid[:,k+1:]-x)/(grid[:,k+1:]-grid[:,1:(-k)])*B_km1[:,1:]
+        B_km1 = B_batch(x[:, 0], grid=grid[:, :, 0], k=k - 1, extend=False, device=device)
+        value = (x - grid[:, :-(k + 1)]) / (grid[:, k:-1] - grid[:, :-(k + 1)]) * B_km1[:, :-1] + (grid[:, k + 1:] - x) / (grid[:, k + 1:] - grid[:, 1:(-k)]) * B_km1[:, 1:]
     return value
 
 
 def coef2curve(x_eval, grid, coef, k, device="cpu"):
     '''
     converting B-spline coefficients to B-spline curves. Evaluate x on B-spline curves (summing up B_batch results over B-spline basis).
     
@@ -96,16 +97,14 @@
     '''
     # x_eval: (size, batch), grid: (size, grid), coef: (size, coef)
     # coef: (size, coef), B_batch: (size, coef, batch), summer over coef
     y_eval = torch.einsum('ij,ijk->ik', coef, B_batch(x_eval, grid, k, device=device))
     return y_eval
 
 
-
-
 def curve2coef(x_eval, y_eval, grid, k, device="cpu"):
     '''
     converting B-spline curves to B-spline coefficients using least squares.
     
     Args:
     -----
         x_eval : 2D torch.tensor
@@ -128,10 +127,10 @@
     >>> x_eval = torch.normal(0,1,size=(num_spline, num_sample))
     >>> y_eval = torch.normal(0,1,size=(num_spline, num_sample))
     >>> grids = torch.einsum('i,j->ij', torch.ones(num_spline,), torch.linspace(-1,1,steps=num_grid_interval+1))
     >>> curve2coef(x_eval, y_eval, grids, k=k).shape
     torch.Size([5, 13])
     '''
     # x_eval: (size, batch); y_eval: (size, batch); grid: (size, grid); k: scalar
-    mat = B_batch(x_eval, grid, k, device=device).permute(0,2,1)
-    coef = torch.linalg.lstsq(mat.to('cpu'), y_eval.unsqueeze(dim=2).to('cpu')).solution[:,:,0] # sometimes 'cuda' version may diverge
-    return coef.to(device)
+    mat = B_batch(x_eval, grid, k, device=device).permute(0, 2, 1)
+    coef = torch.linalg.lstsq(mat.to('cpu'), y_eval.unsqueeze(dim=2).to('cpu')).solution[:, :, 0]  # sometimes 'cuda' version may diverge
+    return coef.to(device)
```

### Comparing `pykan-0.0.2/kan/utils.py` & `pykan-0.0.3/kan/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -120,15 +120,15 @@
     dataset['train_label'] = train_label.to(device)
     dataset['test_label'] = test_label.to(device)
 
     return dataset
 
 
 
-def fit_params(x, y, fun, a_range=(-10,10), b_range=(-10,10), grid_number=101, iteration=3, verbose=True):
+def fit_params(x, y, fun, a_range=(-10,10), b_range=(-10,10), grid_number=101, iteration=3, verbose=True, device='cpu'):
     '''
     fit a, b, c, d such that
     
     .. math::
         |y-(cf(ax+b)+d)|^2
         
     is minimized. Both x and y are 1D array. Sweep a and b, find the best fitted model.
@@ -147,14 +147,16 @@
             sweeping range of b
         grid_num : int
             number of steps along a and b
         iteration : int
             number of zooming in
         verbose : bool
             print extra information if True
+        device : str
+            device
         
     Returns:
     --------
         a_best : float
             best fitted a
         b_best : float
             best fitted b
@@ -174,16 +176,16 @@
     >>> fit_params(x, y, torch.sin)
     r2 is 0.9999727010726929
     (tensor([2.9982, 1.9996, 5.0053, 0.7011]), tensor(1.0000))
     '''
     # fit a, b, c, d such that y=c*fun(a*x+b)+d; both x and y are 1D array.
     # sweep a and b, choose the best fitted model   
     for _ in range(iteration):
-        a_ = torch.linspace(a_range[0], a_range[1], steps=grid_number)
-        b_ = torch.linspace(b_range[0], b_range[1], steps=grid_number)
+        a_ = torch.linspace(a_range[0], a_range[1], steps=grid_number, device=device)
+        b_ = torch.linspace(b_range[0], b_range[1], steps=grid_number, device=device)
         a_grid, b_grid = torch.meshgrid(a_, b_, indexing='ij')
         post_fun = fun(a_grid[None,:,:] * x[:,None,None] + b_grid[None,:,:])
         x_mean = torch.mean(post_fun, dim=[0], keepdim=True)
         y_mean = torch.mean(y, dim=[0], keepdim=True)
         numerator = torch.sum((post_fun - x_mean)*(y-y_mean)[:,None,None], dim=0)**2
         denominator = torch.sum((post_fun - x_mean)**2, dim=0)*torch.sum((y - y_mean)[:,None,None]**2, dim=0)
         r2 = numerator/(denominator+1e-4)
@@ -217,17 +219,17 @@
     
     if verbose == True:
         print(f"r2 is {r2_best}")
         if r2_best < 0.9:
             print(f'r2 is not very high, please double check if you are choosing the correct symbolic function.')
 
     post_fun = torch.nan_to_num(post_fun)
-    reg = LinearRegression().fit(post_fun[:,None].detach().numpy(), y.detach().numpy())
-    c_best = torch.from_numpy(reg.coef_)[0]
-    d_best = torch.from_numpy(np.array(reg.intercept_))
+    reg = LinearRegression().fit(post_fun[:,None].detach().cpu().numpy(), y.detach().cpu().numpy())
+    c_best = torch.from_numpy(reg.coef_)[0].to(device)
+    d_best = torch.from_numpy(np.array(reg.intercept_)).to(device)
     return torch.stack([a_best, b_best, c_best, d_best]), r2_best
 
 
 
 def add_symbolic(name, fun):
     '''
     add a symbolic function to library
```

