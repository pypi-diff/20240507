# Comparing `tmp/pathier-1.5.1.tar.gz` & `tmp/pathier-1.5.2.tar.gz`

## Comparing `pathier-1.5.1.tar` & `pathier-1.5.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     4943 2020-02-02 00:00:00.000000 pathier-1.5.1/CHANGELOG.md
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 pathier-1.5.1/docs/index.html
--rw-r--r--   0        0        0   354638 2020-02-02 00:00:00.000000 pathier-1.5.1/docs/pathier.html
--rw-r--r--   0        0        0    64648 2020-02-02 00:00:00.000000 pathier-1.5.1/docs/search.js
--rw-r--r--   0        0        0    21254 2020-02-02 00:00:00.000000 pathier-1.5.1/htmlcov/coverage_html.js
--rw-r--r--   0        0        0    85191 2020-02-02 00:00:00.000000 pathier-1.5.1/htmlcov/d_a44f0ac069e85531_test_pathier_py.html
--rw-r--r--   0        0        0    13838 2020-02-02 00:00:00.000000 pathier-1.5.1/htmlcov/d_d98317d23aadd1b8___init___py.html
--rw-r--r--   0        0        0   172139 2020-02-02 00:00:00.000000 pathier-1.5.1/htmlcov/d_d98317d23aadd1b8_pathier_py.html
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 pathier-1.5.1/htmlcov/favicon_32.png
--rw-r--r--   0        0        0     4535 2020-02-02 00:00:00.000000 pathier-1.5.1/htmlcov/index.html
--rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 pathier-1.5.1/htmlcov/keybd_closed.png
--rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 pathier-1.5.1/htmlcov/keybd_open.png
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 pathier-1.5.1/htmlcov/status.json
--rw-r--r--   0        0        0    12740 2020-02-02 00:00:00.000000 pathier-1.5.1/htmlcov/style.css
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 pathier-1.5.1/src/pathier/__init__.py
--rw-r--r--   0        0        0    23146 2020-02-02 00:00:00.000000 pathier-1.5.1/src/pathier/pathier.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathier-1.5.1/src/pathier/py.typed
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 pathier-1.5.1/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pathier-1.5.1/LICENSE.txt
--rw-r--r--   0        0        0     5355 2020-02-02 00:00:00.000000 pathier-1.5.1/README.md
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 pathier-1.5.1/pyproject.toml
--rw-r--r--   0        0        0     6021 2020-02-02 00:00:00.000000 pathier-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0     5030 2020-02-02 00:00:00.000000 pathier-1.5.2/CHANGELOG.md
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 pathier-1.5.2/docs/index.html
+-rw-r--r--   0        0        0   357931 2020-02-02 00:00:00.000000 pathier-1.5.2/docs/pathier.html
+-rw-r--r--   0        0        0    64654 2020-02-02 00:00:00.000000 pathier-1.5.2/docs/search.js
+-rw-r--r--   0        0        0    21254 2020-02-02 00:00:00.000000 pathier-1.5.2/htmlcov/coverage_html.js
+-rw-r--r--   0        0        0    85191 2020-02-02 00:00:00.000000 pathier-1.5.2/htmlcov/d_a44f0ac069e85531_test_pathier_py.html
+-rw-r--r--   0        0        0    18026 2020-02-02 00:00:00.000000 pathier-1.5.2/htmlcov/d_d98317d23aadd1b8___init___py.html
+-rw-r--r--   0        0        0   172092 2020-02-02 00:00:00.000000 pathier-1.5.2/htmlcov/d_d98317d23aadd1b8_pathier_py.html
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 pathier-1.5.2/htmlcov/favicon_32.png
+-rw-r--r--   0        0        0     4536 2020-02-02 00:00:00.000000 pathier-1.5.2/htmlcov/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 pathier-1.5.2/htmlcov/keybd_closed.png
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 pathier-1.5.2/htmlcov/keybd_open.png
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 pathier-1.5.2/htmlcov/status.json
+-rw-r--r--   0        0        0    12740 2020-02-02 00:00:00.000000 pathier-1.5.2/htmlcov/style.css
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 pathier-1.5.2/src/pathier/__init__.py
+-rw-r--r--   0        0        0    23148 2020-02-02 00:00:00.000000 pathier-1.5.2/src/pathier/pathier.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pathier-1.5.2/src/pathier/py.typed
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 pathier-1.5.2/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pathier-1.5.2/LICENSE.txt
+-rw-r--r--   0        0        0     5333 2020-02-02 00:00:00.000000 pathier-1.5.2/README.md
+-rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 pathier-1.5.2/pyproject.toml
+-rw-r--r--   0        0        0     6019 2020-02-02 00:00:00.000000 pathier-1.5.2/PKG-INFO
```

### Comparing `pathier-1.5.1/CHANGELOG.md` & `pathier-1.5.2/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # Changelog
 
+## v1.5.1 (2024-02-16)
+
+#### Refactorings
+
+* improve type annotation coverage
+
+
 ## v1.5.0 (2024-01-23)
 
 #### New Features
 
 * add default value for `default` param when calling `json.dumps()` and add default custom tomlkit encoder
```

### Comparing `pathier-1.5.1/docs/pathier.html` & `pathier-1.5.2/docs/pathier.html`

 * *Files 0% similar despite different names*

```diff
@@ -181,43 +181,61 @@
 pathier    </h1>
 
                 
                         <input id="mod-pathier-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 
                         <label class="view-source-button" for="mod-pathier-view-source"><span>View Source</span></label>
 
-                        <div class="pdoc-code codehilite"><pre><span></span><span id="L-1"><a href="#L-1"><span class="linenos"> 1</span></a><span class="kn">import</span> <span class="nn">griddle</span>
-</span><span id="L-2"><a href="#L-2"><span class="linenos"> 2</span></a><span class="kn">import</span> <span class="nn">noiftimer</span>
-</span><span id="L-3"><a href="#L-3"><span class="linenos"> 3</span></a><span class="kn">import</span> <span class="nn">printbuddies</span>
-</span><span id="L-4"><a href="#L-4"><span class="linenos"> 4</span></a>
-</span><span id="L-5"><a href="#L-5"><span class="linenos"> 5</span></a><span class="kn">from</span> <span class="nn">.pathier</span> <span class="kn">import</span> <span class="n">Pathier</span><span class="p">,</span> <span class="n">Pathish</span><span class="p">,</span> <span class="n">Pathy</span>
-</span><span id="L-6"><a href="#L-6"><span class="linenos"> 6</span></a>
-</span><span id="L-7"><a href="#L-7"><span class="linenos"> 7</span></a><span class="n">__all__</span> <span class="o">=</span> <span class="p">[</span><span class="s2">&quot;Pathier&quot;</span><span class="p">,</span> <span class="s2">&quot;Pathy&quot;</span><span class="p">,</span> <span class="s2">&quot;Pathish&quot;</span><span class="p">]</span>
-</span><span id="L-8"><a href="#L-8"><span class="linenos"> 8</span></a>
+                        <div class="pdoc-code codehilite"><pre><span></span><span id="L-1"><a href="#L-1"><span class="linenos"> 1</span></a><span class="kn">import</span> <span class="nn">argparse</span>
+</span><span id="L-2"><a href="#L-2"><span class="linenos"> 2</span></a>
+</span><span id="L-3"><a href="#L-3"><span class="linenos"> 3</span></a><span class="kn">import</span> <span class="nn">griddle</span>
+</span><span id="L-4"><a href="#L-4"><span class="linenos"> 4</span></a><span class="kn">import</span> <span class="nn">noiftimer</span>
+</span><span id="L-5"><a href="#L-5"><span class="linenos"> 5</span></a><span class="kn">import</span> <span class="nn">printbuddies</span>
+</span><span id="L-6"><a href="#L-6"><span class="linenos"> 6</span></a><span class="kn">import</span> <span class="nn">younotyou</span>
+</span><span id="L-7"><a href="#L-7"><span class="linenos"> 7</span></a>
+</span><span id="L-8"><a href="#L-8"><span class="linenos"> 8</span></a><span class="kn">from</span> <span class="nn">.pathier</span> <span class="kn">import</span> <span class="n">Pathier</span><span class="p">,</span> <span class="n">Pathish</span><span class="p">,</span> <span class="n">Pathy</span>
 </span><span id="L-9"><a href="#L-9"><span class="linenos"> 9</span></a>
-</span><span id="L-10"><a href="#L-10"><span class="linenos">10</span></a><span class="nd">@noiftimer</span><span class="o">.</span><span class="n">time_it</span><span class="p">()</span>
-</span><span id="L-11"><a href="#L-11"><span class="linenos">11</span></a><span class="k">def</span> <span class="nf">sizeup</span><span class="p">():</span>
-</span><span id="L-12"><a href="#L-12"><span class="linenos">12</span></a>    <span class="sd">&quot;&quot;&quot;Print the sub-directories and their sizes of the current working directory.&quot;&quot;&quot;</span>
-</span><span id="L-13"><a href="#L-13"><span class="linenos">13</span></a>    <span class="n">sizes</span><span class="p">:</span> <span class="nb">dict</span><span class="p">[</span><span class="nb">str</span><span class="p">,</span> <span class="nb">int</span><span class="p">]</span> <span class="o">=</span> <span class="p">{}</span>
-</span><span id="L-14"><a href="#L-14"><span class="linenos">14</span></a>    <span class="n">folders</span> <span class="o">=</span> <span class="p">[</span><span class="n">folder</span> <span class="k">for</span> <span class="n">folder</span> <span class="ow">in</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">iterdir</span><span class="p">()</span> <span class="k">if</span> <span class="n">folder</span><span class="o">.</span><span class="n">is_dir</span><span class="p">()]</span>
-</span><span id="L-15"><a href="#L-15"><span class="linenos">15</span></a>    <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Sizing up </span><span class="si">{</span><span class="nb">len</span><span class="p">(</span><span class="n">folders</span><span class="p">)</span><span class="si">}</span><span class="s2"> directories...&quot;</span><span class="p">)</span>
-</span><span id="L-16"><a href="#L-16"><span class="linenos">16</span></a>    <span class="k">with</span> <span class="n">printbuddies</span><span class="o">.</span><span class="n">ProgBar</span><span class="p">(</span><span class="nb">len</span><span class="p">(</span><span class="n">folders</span><span class="p">))</span> <span class="k">as</span> <span class="n">prog</span><span class="p">:</span>
-</span><span id="L-17"><a href="#L-17"><span class="linenos">17</span></a>        <span class="k">for</span> <span class="n">folder</span> <span class="ow">in</span> <span class="n">folders</span><span class="p">:</span>
-</span><span id="L-18"><a href="#L-18"><span class="linenos">18</span></a>            <span class="n">prog</span><span class="o">.</span><span class="n">display</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Scanning &#39;</span><span class="si">{</span><span class="n">folder</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2">&#39;&quot;</span><span class="p">)</span>
-</span><span id="L-19"><a href="#L-19"><span class="linenos">19</span></a>            <span class="n">sizes</span><span class="p">[</span><span class="n">folder</span><span class="o">.</span><span class="n">name</span><span class="p">]</span> <span class="o">=</span> <span class="n">folder</span><span class="o">.</span><span class="n">size</span>
-</span><span id="L-20"><a href="#L-20"><span class="linenos">20</span></a>    <span class="n">total_size</span> <span class="o">=</span> <span class="nb">sum</span><span class="p">(</span><span class="n">sizes</span><span class="p">[</span><span class="n">folder</span><span class="p">]</span> <span class="k">for</span> <span class="n">folder</span> <span class="ow">in</span> <span class="n">sizes</span><span class="p">)</span>
-</span><span id="L-21"><a href="#L-21"><span class="linenos">21</span></a>    <span class="n">size_list</span> <span class="o">=</span> <span class="p">[</span>
-</span><span id="L-22"><a href="#L-22"><span class="linenos">22</span></a>        <span class="p">(</span><span class="n">folder</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">format_bytes</span><span class="p">(</span><span class="n">sizes</span><span class="p">[</span><span class="n">folder</span><span class="p">]))</span>
-</span><span id="L-23"><a href="#L-23"><span class="linenos">23</span></a>        <span class="k">for</span> <span class="n">folder</span> <span class="ow">in</span> <span class="nb">sorted</span><span class="p">(</span><span class="nb">list</span><span class="p">(</span><span class="n">sizes</span><span class="o">.</span><span class="n">keys</span><span class="p">()),</span> <span class="n">key</span><span class="o">=</span><span class="k">lambda</span> <span class="n">f</span><span class="p">:</span> <span class="n">sizes</span><span class="p">[</span><span class="n">f</span><span class="p">],</span> <span class="n">reverse</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
-</span><span id="L-24"><a href="#L-24"><span class="linenos">24</span></a>    <span class="p">]</span>
-</span><span id="L-25"><a href="#L-25"><span class="linenos">25</span></a>    <span class="nb">print</span><span class="p">(</span><span class="n">griddle</span><span class="o">.</span><span class="n">griddy</span><span class="p">(</span><span class="n">size_list</span><span class="p">,</span> <span class="p">[</span><span class="s2">&quot;Dir&quot;</span><span class="p">,</span> <span class="s2">&quot;Size&quot;</span><span class="p">]))</span>
-</span><span id="L-26"><a href="#L-26"><span class="linenos">26</span></a>    <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Total size of &#39;</span><span class="si">{</span><span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="si">}</span><span class="s2">&#39;: </span><span class="si">{</span><span class="n">Pathier</span><span class="o">.</span><span class="n">format_bytes</span><span class="p">(</span><span class="n">total_size</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-27"><a href="#L-27"><span class="linenos">27</span></a>
-</span><span id="L-28"><a href="#L-28"><span class="linenos">28</span></a>
-</span><span id="L-29"><a href="#L-29"><span class="linenos">29</span></a><span class="n">__version__</span> <span class="o">=</span> <span class="s2">&quot;1.5.1&quot;</span>
+</span><span id="L-10"><a href="#L-10"><span class="linenos">10</span></a><span class="n">__all__</span> <span class="o">=</span> <span class="p">[</span><span class="s2">&quot;Pathier&quot;</span><span class="p">,</span> <span class="s2">&quot;Pathy&quot;</span><span class="p">,</span> <span class="s2">&quot;Pathish&quot;</span><span class="p">]</span>
+</span><span id="L-11"><a href="#L-11"><span class="linenos">11</span></a>
+</span><span id="L-12"><a href="#L-12"><span class="linenos">12</span></a>
+</span><span id="L-13"><a href="#L-13"><span class="linenos">13</span></a><span class="nd">@noiftimer</span><span class="o">.</span><span class="n">time_it</span><span class="p">()</span>
+</span><span id="L-14"><a href="#L-14"><span class="linenos">14</span></a><span class="k">def</span> <span class="nf">sizeup</span><span class="p">():</span>
+</span><span id="L-15"><a href="#L-15"><span class="linenos">15</span></a>    <span class="sd">&quot;&quot;&quot;Print the sub-directories and their sizes of the current working directory.&quot;&quot;&quot;</span>
+</span><span id="L-16"><a href="#L-16"><span class="linenos">16</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">argparse</span><span class="o">.</span><span class="n">ArgumentParser</span><span class="p">(</span><span class="s2">&quot;sizeup&quot;</span><span class="p">)</span>
+</span><span id="L-17"><a href="#L-17"><span class="linenos">17</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-18"><a href="#L-18"><span class="linenos">18</span></a>        <span class="s2">&quot;-i&quot;</span><span class="p">,</span>
+</span><span id="L-19"><a href="#L-19"><span class="linenos">19</span></a>        <span class="s2">&quot;--ignore&quot;</span><span class="p">,</span>
+</span><span id="L-20"><a href="#L-20"><span class="linenos">20</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;*&quot;</span><span class="p">,</span>
+</span><span id="L-21"><a href="#L-21"><span class="linenos">21</span></a>        <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
+</span><span id="L-22"><a href="#L-22"><span class="linenos">22</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
+</span><span id="L-23"><a href="#L-23"><span class="linenos">23</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;Directory patterns to ignore.&quot;</span><span class="p">,</span>
+</span><span id="L-24"><a href="#L-24"><span class="linenos">24</span></a>    <span class="p">)</span>
+</span><span id="L-25"><a href="#L-25"><span class="linenos">25</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="o">.</span><span class="n">parse_args</span><span class="p">()</span>
+</span><span id="L-26"><a href="#L-26"><span class="linenos">26</span></a>    <span class="n">matcher</span> <span class="o">=</span> <span class="n">younotyou</span><span class="o">.</span><span class="n">Matcher</span><span class="p">(</span><span class="n">exclude_patterns</span><span class="o">=</span><span class="n">args</span><span class="o">.</span><span class="n">ignore</span><span class="p">)</span>
+</span><span id="L-27"><a href="#L-27"><span class="linenos">27</span></a>    <span class="n">sizes</span><span class="p">:</span> <span class="nb">dict</span><span class="p">[</span><span class="nb">str</span><span class="p">,</span> <span class="nb">int</span><span class="p">]</span> <span class="o">=</span> <span class="p">{}</span>
+</span><span id="L-28"><a href="#L-28"><span class="linenos">28</span></a>    <span class="n">folders</span> <span class="o">=</span> <span class="p">[</span>
+</span><span id="L-29"><a href="#L-29"><span class="linenos">29</span></a>        <span class="n">folder</span>
+</span><span id="L-30"><a href="#L-30"><span class="linenos">30</span></a>        <span class="k">for</span> <span class="n">folder</span> <span class="ow">in</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">iterdir</span><span class="p">()</span>
+</span><span id="L-31"><a href="#L-31"><span class="linenos">31</span></a>        <span class="k">if</span> <span class="n">folder</span><span class="o">.</span><span class="n">is_dir</span><span class="p">()</span> <span class="ow">and</span> <span class="nb">str</span><span class="p">(</span><span class="n">folder</span><span class="p">)</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">matcher</span>
+</span><span id="L-32"><a href="#L-32"><span class="linenos">32</span></a>    <span class="p">]</span>
+</span><span id="L-33"><a href="#L-33"><span class="linenos">33</span></a>    <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Sizing up </span><span class="si">{</span><span class="nb">len</span><span class="p">(</span><span class="n">folders</span><span class="p">)</span><span class="si">}</span><span class="s2"> directories...&quot;</span><span class="p">)</span>
+</span><span id="L-34"><a href="#L-34"><span class="linenos">34</span></a>    <span class="k">with</span> <span class="n">printbuddies</span><span class="o">.</span><span class="n">ProgBar</span><span class="p">(</span><span class="nb">len</span><span class="p">(</span><span class="n">folders</span><span class="p">))</span> <span class="k">as</span> <span class="n">prog</span><span class="p">:</span>
+</span><span id="L-35"><a href="#L-35"><span class="linenos">35</span></a>        <span class="k">for</span> <span class="n">folder</span> <span class="ow">in</span> <span class="n">folders</span><span class="p">:</span>
+</span><span id="L-36"><a href="#L-36"><span class="linenos">36</span></a>            <span class="n">prog</span><span class="o">.</span><span class="n">display</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Scanning &#39;</span><span class="si">{</span><span class="n">folder</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2">&#39;&quot;</span><span class="p">)</span>
+</span><span id="L-37"><a href="#L-37"><span class="linenos">37</span></a>            <span class="n">sizes</span><span class="p">[</span><span class="n">folder</span><span class="o">.</span><span class="n">name</span><span class="p">]</span> <span class="o">=</span> <span class="n">folder</span><span class="o">.</span><span class="n">size</span>
+</span><span id="L-38"><a href="#L-38"><span class="linenos">38</span></a>    <span class="n">total_size</span> <span class="o">=</span> <span class="nb">sum</span><span class="p">(</span><span class="n">sizes</span><span class="p">[</span><span class="n">folder</span><span class="p">]</span> <span class="k">for</span> <span class="n">folder</span> <span class="ow">in</span> <span class="n">sizes</span><span class="p">)</span>
+</span><span id="L-39"><a href="#L-39"><span class="linenos">39</span></a>    <span class="n">size_list</span> <span class="o">=</span> <span class="p">[</span>
+</span><span id="L-40"><a href="#L-40"><span class="linenos">40</span></a>        <span class="p">(</span><span class="n">folder</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">format_bytes</span><span class="p">(</span><span class="n">sizes</span><span class="p">[</span><span class="n">folder</span><span class="p">]))</span>
+</span><span id="L-41"><a href="#L-41"><span class="linenos">41</span></a>        <span class="k">for</span> <span class="n">folder</span> <span class="ow">in</span> <span class="nb">sorted</span><span class="p">(</span><span class="nb">list</span><span class="p">(</span><span class="n">sizes</span><span class="o">.</span><span class="n">keys</span><span class="p">()),</span> <span class="n">key</span><span class="o">=</span><span class="k">lambda</span> <span class="n">f</span><span class="p">:</span> <span class="n">sizes</span><span class="p">[</span><span class="n">f</span><span class="p">],</span> <span class="n">reverse</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
+</span><span id="L-42"><a href="#L-42"><span class="linenos">42</span></a>    <span class="p">]</span>
+</span><span id="L-43"><a href="#L-43"><span class="linenos">43</span></a>    <span class="nb">print</span><span class="p">(</span><span class="n">griddle</span><span class="o">.</span><span class="n">griddy</span><span class="p">(</span><span class="n">size_list</span><span class="p">,</span> <span class="p">[</span><span class="s2">&quot;Dir&quot;</span><span class="p">,</span> <span class="s2">&quot;Size&quot;</span><span class="p">]))</span>
+</span><span id="L-44"><a href="#L-44"><span class="linenos">44</span></a>    <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Total size of &#39;</span><span class="si">{</span><span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="si">}</span><span class="s2">&#39;: </span><span class="si">{</span><span class="n">Pathier</span><span class="o">.</span><span class="n">format_bytes</span><span class="p">(</span><span class="n">total_size</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-45"><a href="#L-45"><span class="linenos">45</span></a>
+</span><span id="L-46"><a href="#L-46"><span class="linenos">46</span></a>
+</span><span id="L-47"><a href="#L-47"><span class="linenos">47</span></a><span class="n">__version__</span> <span class="o">=</span> <span class="s2">&quot;1.5.2&quot;</span>
 </span></pre></div>
 
 
             </section>
                 <section id="Pathier">
                             <input id="Pathier-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr class">
@@ -565,15 +583,15 @@
 </span><span id="Pathier-350"><a href="#Pathier-350"><span class="linenos">350</span></a>        <span class="k">if</span> <span class="n">new_line</span><span class="p">:</span>
 </span><span id="Pathier-351"><a href="#Pathier-351"><span class="linenos">351</span></a>            <span class="n">data</span> <span class="o">+=</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span>
 </span><span id="Pathier-352"><a href="#Pathier-352"><span class="linenos">352</span></a>        <span class="k">with</span> <span class="bp">self</span><span class="o">.</span><span class="n">open</span><span class="p">(</span><span class="s2">&quot;a&quot;</span><span class="p">,</span> <span class="n">encoding</span><span class="o">=</span><span class="n">encoding</span><span class="p">)</span> <span class="k">as</span> <span class="n">file</span><span class="p">:</span>
 </span><span id="Pathier-353"><a href="#Pathier-353"><span class="linenos">353</span></a>            <span class="n">file</span><span class="o">.</span><span class="n">write</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
 </span><span id="Pathier-354"><a href="#Pathier-354"><span class="linenos">354</span></a>
 </span><span id="Pathier-355"><a href="#Pathier-355"><span class="linenos">355</span></a>    <span class="k">def</span> <span class="nf">replace_strings</span><span class="p">(</span>
 </span><span id="Pathier-356"><a href="#Pathier-356"><span class="linenos">356</span></a>        <span class="bp">self</span><span class="p">,</span>
-</span><span id="Pathier-357"><a href="#Pathier-357"><span class="linenos">357</span></a>        <span class="n">substitutions</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">[</span><span class="nb">str</span><span class="p">,</span> <span class="nb">str</span><span class="p">]],</span>
+</span><span id="Pathier-357"><a href="#Pathier-357"><span class="linenos">357</span></a>        <span class="n">substitutions</span><span class="p">:</span> <span class="n">Sequence</span><span class="p">[</span><span class="nb">tuple</span><span class="p">[</span><span class="nb">str</span><span class="p">,</span> <span class="nb">str</span><span class="p">]],</span>
 </span><span id="Pathier-358"><a href="#Pathier-358"><span class="linenos">358</span></a>        <span class="n">count</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="o">-</span><span class="mi">1</span><span class="p">,</span>
 </span><span id="Pathier-359"><a href="#Pathier-359"><span class="linenos">359</span></a>        <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
 </span><span id="Pathier-360"><a href="#Pathier-360"><span class="linenos">360</span></a>    <span class="p">):</span>
 </span><span id="Pathier-361"><a href="#Pathier-361"><span class="linenos">361</span></a>        <span class="sd">&quot;&quot;&quot;For each pair in `substitutions`, replace the first string with the second string.</span>
 </span><span id="Pathier-362"><a href="#Pathier-362"><span class="linenos">362</span></a>
 </span><span id="Pathier-363"><a href="#Pathier-363"><span class="linenos">363</span></a><span class="sd">        #### :params:</span>
 </span><span id="Pathier-364"><a href="#Pathier-364"><span class="linenos">364</span></a>
@@ -590,15 +608,15 @@
 </span><span id="Pathier-375"><a href="#Pathier-375"><span class="linenos">375</span></a><span class="sd">        &gt;&gt;&gt; path.write_text(path.read_text().replace(&quot;hello&quot;, &quot;yeet&quot;).replace(&quot;goodbye&quot;, &quot;yeehaw&quot;))</span>
 </span><span id="Pathier-376"><a href="#Pathier-376"><span class="linenos">376</span></a><span class="sd">        &quot;&quot;&quot;</span>
 </span><span id="Pathier-377"><a href="#Pathier-377"><span class="linenos">377</span></a>        <span class="n">text</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">read_text</span><span class="p">(</span><span class="n">encoding</span><span class="p">)</span>
 </span><span id="Pathier-378"><a href="#Pathier-378"><span class="linenos">378</span></a>        <span class="k">for</span> <span class="n">sub</span> <span class="ow">in</span> <span class="n">substitutions</span><span class="p">:</span>
 </span><span id="Pathier-379"><a href="#Pathier-379"><span class="linenos">379</span></a>            <span class="n">text</span> <span class="o">=</span> <span class="n">text</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="n">sub</span><span class="p">[</span><span class="mi">0</span><span class="p">],</span> <span class="n">sub</span><span class="p">[</span><span class="mi">1</span><span class="p">],</span> <span class="n">count</span><span class="p">)</span>
 </span><span id="Pathier-380"><a href="#Pathier-380"><span class="linenos">380</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">text</span><span class="p">,</span> <span class="n">encoding</span><span class="o">=</span><span class="n">encoding</span><span class="p">)</span>
 </span><span id="Pathier-381"><a href="#Pathier-381"><span class="linenos">381</span></a>
-</span><span id="Pathier-382"><a href="#Pathier-382"><span class="linenos">382</span></a>    <span class="k">def</span> <span class="nf">join</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">data</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">],</span> <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">sep</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">):</span>
+</span><span id="Pathier-382"><a href="#Pathier-382"><span class="linenos">382</span></a>    <span class="k">def</span> <span class="nf">join</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">data</span><span class="p">:</span> <span class="n">Sequence</span><span class="p">[</span><span class="nb">str</span><span class="p">],</span> <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">sep</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">):</span>
 </span><span id="Pathier-383"><a href="#Pathier-383"><span class="linenos">383</span></a>        <span class="sd">&quot;&quot;&quot;Write a list of strings, joined by `sep`, to the file pointed at by this instance.</span>
 </span><span id="Pathier-384"><a href="#Pathier-384"><span class="linenos">384</span></a>
 </span><span id="Pathier-385"><a href="#Pathier-385"><span class="linenos">385</span></a><span class="sd">        Equivalent to `Pathier(&quot;somefile.txt&quot;).write_text(sep.join(data), encoding=encoding)`</span>
 </span><span id="Pathier-386"><a href="#Pathier-386"><span class="linenos">386</span></a>
 </span><span id="Pathier-387"><a href="#Pathier-387"><span class="linenos">387</span></a><span class="sd">        #### :params:</span>
 </span><span id="Pathier-388"><a href="#Pathier-388"><span class="linenos">388</span></a>
 </span><span id="Pathier-389"><a href="#Pathier-389"><span class="linenos">389</span></a><span class="sd">        `encoding`: The file encoding to use.</span>
@@ -1554,23 +1572,23 @@
 
                             </div>
                             <div id="Pathier.replace_strings" class="classattr">
                                         <input id="Pathier.replace_strings-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
-        <span class="name">replace_strings</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">substitutions</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">[</span><span class="nb">str</span><span class="p">,</span> <span class="nb">str</span><span class="p">]]</span>,</span><span class="param">	<span class="n">count</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="o">-</span><span class="mi">1</span>,</span><span class="param">	<span class="n">encoding</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span></span><span class="return-annotation">):</span></span>
+        <span class="name">replace_strings</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">substitutions</span><span class="p">:</span> <span class="n">Sequence</span><span class="p">[</span><span class="nb">tuple</span><span class="p">[</span><span class="nb">str</span><span class="p">,</span> <span class="nb">str</span><span class="p">]]</span>,</span><span class="param">	<span class="n">count</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="o">-</span><span class="mi">1</span>,</span><span class="param">	<span class="n">encoding</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="Pathier.replace_strings-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Pathier.replace_strings"></a>
             <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.replace_strings-355"><a href="#Pathier.replace_strings-355"><span class="linenos">355</span></a>    <span class="k">def</span> <span class="nf">replace_strings</span><span class="p">(</span>
 </span><span id="Pathier.replace_strings-356"><a href="#Pathier.replace_strings-356"><span class="linenos">356</span></a>        <span class="bp">self</span><span class="p">,</span>
-</span><span id="Pathier.replace_strings-357"><a href="#Pathier.replace_strings-357"><span class="linenos">357</span></a>        <span class="n">substitutions</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">[</span><span class="nb">str</span><span class="p">,</span> <span class="nb">str</span><span class="p">]],</span>
+</span><span id="Pathier.replace_strings-357"><a href="#Pathier.replace_strings-357"><span class="linenos">357</span></a>        <span class="n">substitutions</span><span class="p">:</span> <span class="n">Sequence</span><span class="p">[</span><span class="nb">tuple</span><span class="p">[</span><span class="nb">str</span><span class="p">,</span> <span class="nb">str</span><span class="p">]],</span>
 </span><span id="Pathier.replace_strings-358"><a href="#Pathier.replace_strings-358"><span class="linenos">358</span></a>        <span class="n">count</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="o">-</span><span class="mi">1</span><span class="p">,</span>
 </span><span id="Pathier.replace_strings-359"><a href="#Pathier.replace_strings-359"><span class="linenos">359</span></a>        <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
 </span><span id="Pathier.replace_strings-360"><a href="#Pathier.replace_strings-360"><span class="linenos">360</span></a>    <span class="p">):</span>
 </span><span id="Pathier.replace_strings-361"><a href="#Pathier.replace_strings-361"><span class="linenos">361</span></a>        <span class="sd">&quot;&quot;&quot;For each pair in `substitutions`, replace the first string with the second string.</span>
 </span><span id="Pathier.replace_strings-362"><a href="#Pathier.replace_strings-362"><span class="linenos">362</span></a>
 </span><span id="Pathier.replace_strings-363"><a href="#Pathier.replace_strings-363"><span class="linenos">363</span></a><span class="sd">        #### :params:</span>
 </span><span id="Pathier.replace_strings-364"><a href="#Pathier.replace_strings-364"><span class="linenos">364</span></a>
@@ -1617,21 +1635,21 @@
 
                             </div>
                             <div id="Pathier.join" class="classattr">
                                         <input id="Pathier.join-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
-        <span class="name">join</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">data</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span>,</span><span class="param">	<span class="n">encoding</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">sep</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s1">&#39;</span><span class="se">\n</span><span class="s1">&#39;</span></span><span class="return-annotation">):</span></span>
+        <span class="name">join</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">data</span><span class="p">:</span> <span class="n">Sequence</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span>,</span><span class="param">	<span class="n">encoding</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">sep</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s1">&#39;</span><span class="se">\n</span><span class="s1">&#39;</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="Pathier.join-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Pathier.join"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.join-382"><a href="#Pathier.join-382"><span class="linenos">382</span></a>    <span class="k">def</span> <span class="nf">join</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">data</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">],</span> <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">sep</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">):</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Pathier.join-382"><a href="#Pathier.join-382"><span class="linenos">382</span></a>    <span class="k">def</span> <span class="nf">join</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">data</span><span class="p">:</span> <span class="n">Sequence</span><span class="p">[</span><span class="nb">str</span><span class="p">],</span> <span class="n">encoding</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">sep</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">):</span>
 </span><span id="Pathier.join-383"><a href="#Pathier.join-383"><span class="linenos">383</span></a>        <span class="sd">&quot;&quot;&quot;Write a list of strings, joined by `sep`, to the file pointed at by this instance.</span>
 </span><span id="Pathier.join-384"><a href="#Pathier.join-384"><span class="linenos">384</span></a>
 </span><span id="Pathier.join-385"><a href="#Pathier.join-385"><span class="linenos">385</span></a><span class="sd">        Equivalent to `Pathier(&quot;somefile.txt&quot;).write_text(sep.join(data), encoding=encoding)`</span>
 </span><span id="Pathier.join-386"><a href="#Pathier.join-386"><span class="linenos">386</span></a>
 </span><span id="Pathier.join-387"><a href="#Pathier.join-387"><span class="linenos">387</span></a><span class="sd">        #### :params:</span>
 </span><span id="Pathier.join-388"><a href="#Pathier.join-388"><span class="linenos">388</span></a>
 </span><span id="Pathier.join-389"><a href="#Pathier.join-389"><span class="linenos">389</span></a><span class="sd">        `encoding`: The file encoding to use.</span>
```

#### html2text {}

```diff
@@ -45,47 +45,64 @@
           o _b_a_c_k_u_p
           o _e_x_e_c_u_t_e
     * _P_a_t_h_y
     * _P_a_t_h_i_s_h
 _b_u_i_l_t_ _w_i_t_h_ _p_d_o_c_[_p_d_o_c_ _l_o_g_o_]
 ************ ppaatthhiieerr ************
 ??View Source
-_ _1import griddle
-_ _2import noiftimer
-_ _3import printbuddies
-_ _4
-_ _5from .pathier import Pathier, Pathish, Pathy
-_ _6
-_ _7__all__ = ["Pathier", "Pathy", "Pathish"]
-_ _8
+_ _1import argparse
+_ _2
+_ _3import griddle
+_ _4import noiftimer
+_ _5import printbuddies
+_ _6import younotyou
+_ _7
+_ _8from .pathier import Pathier, Pathish, Pathy
 _ _9
-_1_0@noiftimer.time_it()
-_1_1def sizeup():
-_1_2    """Print the sub-directories and their sizes of the current working
+_1_0__all__ = ["Pathier", "Pathy", "Pathish"]
+_1_1
+_1_2
+_1_3@noiftimer.time_it()
+_1_4def sizeup():
+_1_5    """Print the sub-directories and their sizes of the current working
 directory."""
-_1_3    sizes: dict[str, int] = {}
-_1_4    folders = [folder for folder in Pathier.cwd().iterdir() if folder.is_dir
-()]
-_1_5    print(f"Sizing up {len(folders)} directories...")
-_1_6    with printbuddies.ProgBar(len(folders)) as prog:
-_1_7        for folder in folders:
-_1_8            prog.display(f"Scanning '{folder.name}'")
-_1_9            sizes[folder.name] = folder.size
-_2_0    total_size = sum(sizes[folder] for folder in sizes)
-_2_1    size_list = [
-_2_2        (folder, Pathier.format_bytes(sizes[folder]))
-_2_3        for folder in sorted(list(sizes.keys()), key=lambda f: sizes[f],
+_1_6    parser = argparse.ArgumentParser("sizeup")
+_1_7    parser.add_argument(
+_1_8        "-i",
+_1_9        "--ignore",
+_2_0        nargs="*",
+_2_1        default=None,
+_2_2        type=str,
+_2_3        help="Directory patterns to ignore.",
+_2_4    )
+_2_5    args = parser.parse_args()
+_2_6    matcher = younotyou.Matcher(exclude_patterns=args.ignore)
+_2_7    sizes: dict[str, int] = {}
+_2_8    folders = [
+_2_9        folder
+_3_0        for folder in Pathier.cwd().iterdir()
+_3_1        if folder.is_dir() and str(folder) not in matcher
+_3_2    ]
+_3_3    print(f"Sizing up {len(folders)} directories...")
+_3_4    with printbuddies.ProgBar(len(folders)) as prog:
+_3_5        for folder in folders:
+_3_6            prog.display(f"Scanning '{folder.name}'")
+_3_7            sizes[folder.name] = folder.size
+_3_8    total_size = sum(sizes[folder] for folder in sizes)
+_3_9    size_list = [
+_4_0        (folder, Pathier.format_bytes(sizes[folder]))
+_4_1        for folder in sorted(list(sizes.keys()), key=lambda f: sizes[f],
 reverse=True)
-_2_4    ]
-_2_5    print(griddle.griddy(size_list, ["Dir", "Size"]))
-_2_6    print(f"Total size of '{Pathier.cwd()}': {Pathier.format_bytes
+_4_2    ]
+_4_3    print(griddle.griddy(size_list, ["Dir", "Size"]))
+_4_4    print(f"Total size of '{Pathier.cwd()}': {Pathier.format_bytes
 (total_size)}")
-_2_7
-_2_8
-_2_9__version__ = "1.5.1"
+_4_5
+_4_6
+_4_7__version__ = "1.5.2"
 ??
 class Pathier(pathlib.Path): View Source
 _ _1_7class Pathier(pathlib.Path):
 _ _1_8    """Subclasses the standard library pathlib.Path class."""
 _ _1_9
 _ _2_0    def __new__(
 _ _2_1        cls,
@@ -457,15 +474,15 @@
 _3_5_0        if new_line:
 _3_5_1            data += "\n"
 _3_5_2        with self.open("a", encoding=encoding) as file:
 _3_5_3            file.write(data)
 _3_5_4
 _3_5_5    def replace_strings(
 _3_5_6        self,
-_3_5_7        substitutions: list[tuple[str, str]],
+_3_5_7        substitutions: Sequence[tuple[str, str]],
 _3_5_8        count: int = -1,
 _3_5_9        encoding: Any | None = None,
 _3_6_0    ):
 _3_6_1        """For each pair in `substitutions`, replace the first string with
 the second string.
 _3_6_2
 _3_6_3        #### :params:
@@ -484,16 +501,16 @@
 "yeet").replace("goodbye", "yeehaw"))
 _3_7_6        """
 _3_7_7        text = self.read_text(encoding)
 _3_7_8        for sub in substitutions:
 _3_7_9            text = text.replace(sub[0], sub[1], count)
 _3_8_0        self.write_text(text, encoding=encoding)
 _3_8_1
-_3_8_2    def join(self, data: list[str], encoding: Any | None = None, sep: str =
-"\n"):
+_3_8_2    def join(self, data: Sequence[str], encoding: Any | None = None, sep:
+str = "\n"):
 _3_8_3        """Write a list of strings, joined by `sep`, to the file pointed at
 by this instance.
 _3_8_4
 _3_8_5        Equivalent to `Pathier("somefile.txt").write_text(sep.join(data),
 encoding=encoding)`
 _3_8_6
 _3_8_7        #### :params:
@@ -1090,20 +1107,20 @@
 Append data to the file pointed to by this _P_a_t_h_i_e_r object.
 ****** ::ppaarraammss:: ******
 new_line: If True, add \n to data.
 encoding: The file encoding to use.
 ??
 def replace_strings(
 self,
-substitutions: list[tuple[str, str]],
+substitutions: Sequence[tuple[str, str]],
 count: int = -1,
 encoding: typing.Any | None = None): View Source
 _3_5_5    def replace_strings(
 _3_5_6        self,
-_3_5_7        substitutions: list[tuple[str, str]],
+_3_5_7        substitutions: Sequence[tuple[str, str]],
 _3_5_8        count: int = -1,
 _3_5_9        encoding: Any | None = None,
 _3_6_0    ):
 _3_6_1        """For each pair in `substitutions`, replace the first string with
 the second string.
 _3_6_2
 _3_6_3        #### :params:
@@ -1137,19 +1154,19 @@
 >>> path.replace([("hello", "yeet"), ("goodbye", "yeehaw")])
 equivalent to
 >>> path.write_text(path.read_text().replace("hello", "yeet").replace
 ("goodbye", "yeehaw"))
 ??
 def join(
 self,
-data: list[str],
+data: Sequence[str],
 encoding: typing.Any | None = None,
 sep: str = '\n'): View Source
-_3_8_2    def join(self, data: list[str], encoding: Any | None = None, sep: str =
-"\n"):
+_3_8_2    def join(self, data: Sequence[str], encoding: Any | None = None, sep:
+str = "\n"):
 _3_8_3        """Write a list of strings, joined by `sep`, to the file pointed at
 by this instance.
 _3_8_4
 _3_8_5        Equivalent to `Pathier("somefile.txt").write_text(sep.join(data),
 encoding=encoding)`
 _3_8_6
 _3_8_7        #### :params:
```

### Comparing `pathier-1.5.1/docs/search.js` & `pathier-1.5.2/docs/search.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -909,23 +909,23 @@
         "funcdef": "def"
     }, {
         "fullname": "pathier.Pathier.replace_strings",
         "modulename": "pathier",
         "qualname": "Pathier.replace_strings",
         "kind": "function",
         "doc": "<p>For each pair in <code>substitutions</code>, replace the first string with the second string.</p>\n\n<h4 id=\"params\">:params:</h4>\n\n<p><code>count</code>: Only replace this many occurences of each pair.\nBy default (<code>-1</code>), all occurences are replaced.</p>\n\n<p><code>encoding</code>: The file encoding to use.</p>\n\n<p>e.g.</p>\n\n<div class=\"pdoc-code codehilite\">\n<pre><span></span><code><span class=\"gp\">&gt;&gt;&gt; </span><span class=\"n\">path</span> <span class=\"o\">=</span> <span class=\"n\">Pathier</span><span class=\"p\">(</span><span class=\"s2\">&quot;somefile.txt&quot;</span><span class=\"p\">)</span>\n<span class=\"go\">&gt;&gt;&gt;</span>\n<span class=\"gp\">&gt;&gt;&gt; </span><span class=\"n\">path</span><span class=\"o\">.</span><span class=\"n\">replace</span><span class=\"p\">([(</span><span class=\"s2\">&quot;hello&quot;</span><span class=\"p\">,</span> <span class=\"s2\">&quot;yeet&quot;</span><span class=\"p\">),</span> <span class=\"p\">(</span><span class=\"s2\">&quot;goodbye&quot;</span><span class=\"p\">,</span> <span class=\"s2\">&quot;yeehaw&quot;</span><span class=\"p\">)])</span>\n<span class=\"go\">equivalent to</span>\n<span class=\"gp\">&gt;&gt;&gt; </span><span class=\"n\">path</span><span class=\"o\">.</span><span class=\"n\">write_text</span><span class=\"p\">(</span><span class=\"n\">path</span><span class=\"o\">.</span><span class=\"n\">read_text</span><span class=\"p\">()</span><span class=\"o\">.</span><span class=\"n\">replace</span><span class=\"p\">(</span><span class=\"s2\">&quot;hello&quot;</span><span class=\"p\">,</span> <span class=\"s2\">&quot;yeet&quot;</span><span class=\"p\">)</span><span class=\"o\">.</span><span class=\"n\">replace</span><span class=\"p\">(</span><span class=\"s2\">&quot;goodbye&quot;</span><span class=\"p\">,</span> <span class=\"s2\">&quot;yeehaw&quot;</span><span class=\"p\">))</span>\n</code></pre>\n</div>\n",
-        "signature": "<span class=\"signature pdoc-code multiline\">(<span class=\"param\">\t<span class=\"bp\">self</span>,</span><span class=\"param\">\t<span class=\"n\">substitutions</span><span class=\"p\">:</span> <span class=\"nb\">list</span><span class=\"p\">[</span><span class=\"nb\">tuple</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">,</span> <span class=\"nb\">str</span><span class=\"p\">]]</span>,</span><span class=\"param\">\t<span class=\"n\">count</span><span class=\"p\">:</span> <span class=\"nb\">int</span> <span class=\"o\">=</span> <span class=\"o\">-</span><span class=\"mi\">1</span>,</span><span class=\"param\">\t<span class=\"n\">encoding</span><span class=\"p\">:</span> <span class=\"n\">typing</span><span class=\"o\">.</span><span class=\"n\">Any</span> <span class=\"o\">|</span> <span class=\"kc\">None</span> <span class=\"o\">=</span> <span class=\"kc\">None</span></span><span class=\"return-annotation\">):</span></span>",
+        "signature": "<span class=\"signature pdoc-code multiline\">(<span class=\"param\">\t<span class=\"bp\">self</span>,</span><span class=\"param\">\t<span class=\"n\">substitutions</span><span class=\"p\">:</span> <span class=\"n\">Sequence</span><span class=\"p\">[</span><span class=\"nb\">tuple</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">,</span> <span class=\"nb\">str</span><span class=\"p\">]]</span>,</span><span class=\"param\">\t<span class=\"n\">count</span><span class=\"p\">:</span> <span class=\"nb\">int</span> <span class=\"o\">=</span> <span class=\"o\">-</span><span class=\"mi\">1</span>,</span><span class=\"param\">\t<span class=\"n\">encoding</span><span class=\"p\">:</span> <span class=\"n\">typing</span><span class=\"o\">.</span><span class=\"n\">Any</span> <span class=\"o\">|</span> <span class=\"kc\">None</span> <span class=\"o\">=</span> <span class=\"kc\">None</span></span><span class=\"return-annotation\">):</span></span>",
         "funcdef": "def"
     }, {
         "fullname": "pathier.Pathier.join",
         "modulename": "pathier",
         "qualname": "Pathier.join",
         "kind": "function",
         "doc": "<p>Write a list of strings, joined by <code>sep</code>, to the file pointed at by this instance.</p>\n\n<p>Equivalent to <code>Pathier(\"somefile.txt\").write_text(sep.join(data), encoding=encoding)</code></p>\n\n<h4 id=\"params\">:params:</h4>\n\n<p><code>encoding</code>: The file encoding to use.</p>\n\n<p><code>sep</code>: The separator to use when joining <code>data</code>.</p>\n",
-        "signature": "<span class=\"signature pdoc-code multiline\">(<span class=\"param\">\t<span class=\"bp\">self</span>,</span><span class=\"param\">\t<span class=\"n\">data</span><span class=\"p\">:</span> <span class=\"nb\">list</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">]</span>,</span><span class=\"param\">\t<span class=\"n\">encoding</span><span class=\"p\">:</span> <span class=\"n\">typing</span><span class=\"o\">.</span><span class=\"n\">Any</span> <span class=\"o\">|</span> <span class=\"kc\">None</span> <span class=\"o\">=</span> <span class=\"kc\">None</span>,</span><span class=\"param\">\t<span class=\"n\">sep</span><span class=\"p\">:</span> <span class=\"nb\">str</span> <span class=\"o\">=</span> <span class=\"s1\">&#39;</span><span class=\"se\">\\n</span><span class=\"s1\">&#39;</span></span><span class=\"return-annotation\">):</span></span>",
+        "signature": "<span class=\"signature pdoc-code multiline\">(<span class=\"param\">\t<span class=\"bp\">self</span>,</span><span class=\"param\">\t<span class=\"n\">data</span><span class=\"p\">:</span> <span class=\"n\">Sequence</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">]</span>,</span><span class=\"param\">\t<span class=\"n\">encoding</span><span class=\"p\">:</span> <span class=\"n\">typing</span><span class=\"o\">.</span><span class=\"n\">Any</span> <span class=\"o\">|</span> <span class=\"kc\">None</span> <span class=\"o\">=</span> <span class=\"kc\">None</span>,</span><span class=\"param\">\t<span class=\"n\">sep</span><span class=\"p\">:</span> <span class=\"nb\">str</span> <span class=\"o\">=</span> <span class=\"s1\">&#39;</span><span class=\"se\">\\n</span><span class=\"s1\">&#39;</span></span><span class=\"return-annotation\">):</span></span>",
         "funcdef": "def"
     }, {
         "fullname": "pathier.Pathier.split",
         "modulename": "pathier",
         "qualname": "Pathier.split",
         "kind": "function",
         "doc": "<p>Returns the content of the pointed at file as a list of strings, splitting at new line characters.</p>\n\n<p>Equivalent to <code>Pathier(\"somefile.txt\").read_text(encoding=encoding).splitlines()</code></p>\n\n<h4 id=\"params\">:params:</h4>\n\n<p><code>encoding</code>: The file encoding to use.</p>\n\n<p><code>keepend</code>: If <code>True</code>, line breaks will be included in returned strings.</p>\n",
```

### Comparing `pathier-1.5.1/htmlcov/coverage_html.js` & `pathier-1.5.2/htmlcov/coverage_html.js`

 * *Files identical despite different names*

### Comparing `pathier-1.5.1/htmlcov/d_a44f0ac069e85531_test_pathier_py.html` & `pathier-1.5.2/htmlcov/d_a44f0ac069e85531_test_pathier_py.html`

 * *Files identical despite different names*

### Comparing `pathier-1.5.1/htmlcov/d_d98317d23aadd1b8_pathier_py.html` & `pathier-1.5.2/htmlcov/d_d98317d23aadd1b8_pathier_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_d98317d23aadd1b8___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_a44f0ac069e85531_test_pathier_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.2">coverage.py v7.2.2</a>,
-            created at 2024-02-16 15:27 -0600
+            created at 2024-05-07 16:38 -0500
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -88,15 +88,15 @@
     <p class="run"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="key">import</span> <span class="nam">pickle</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="key">import</span> <span class="nam">shutil</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="key">import</span> <span class="nam">sys</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t"><span class="key">import</span> <span class="nam">time</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t"><span class="key">from</span> <span class="nam">typing</span> <span class="key">import</span> <span class="nam">Any</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t"><span class="key">import</span> <span class="nam">tomlkit</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t"><span class="key">from</span> <span class="nam">typing_extensions</span> <span class="key">import</span> <span class="nam">Callable</span><span class="op">,</span> <span class="nam">Self</span><span class="op">,</span> <span class="nam">Sequence</span><span class="op">,</span> <span class="nam">Buffer</span><span class="op">,</span> <span class="nam">IO</span><span class="op">,</span> <span class="nam">Type</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t"><span class="key">from</span> <span class="nam">typing_extensions</span> <span class="key">import</span> <span class="nam">IO</span><span class="op">,</span> <span class="nam">Buffer</span><span class="op">,</span> <span class="nam">Callable</span><span class="op">,</span> <span class="nam">Self</span><span class="op">,</span> <span class="nam">Sequence</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t"><span class="key">class</span> <span class="nam">Pathier</span><span class="op">(</span><span class="nam">pathlib</span><span class="op">.</span><span class="nam">Path</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t">    <span class="str">"""Subclasses the standard library pathlib.Path class."""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t">    <span class="key">def</span> <span class="nam">__new__</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t">        <span class="nam">cls</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
@@ -431,15 +431,15 @@
     <p class="run"><span class="n"><a id="t349" href="#t349">349</a></span><span class="t">        <span class="key">if</span> <span class="nam">new_line</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t350" href="#t350">350</a></span><span class="t">            <span class="nam">data</span> <span class="op">+=</span> <span class="str">"\n"</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t351" href="#t351">351</a></span><span class="t">        <span class="key">with</span> <span class="nam">self</span><span class="op">.</span><span class="nam">open</span><span class="op">(</span><span class="str">"a"</span><span class="op">,</span> <span class="nam">encoding</span><span class="op">=</span><span class="nam">encoding</span><span class="op">)</span> <span class="key">as</span> <span class="nam">file</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t352" href="#t352">352</a></span><span class="t">            <span class="nam">file</span><span class="op">.</span><span class="nam">write</span><span class="op">(</span><span class="nam">data</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t353" href="#t353">353</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t354" href="#t354">354</a></span><span class="t">    <span class="key">def</span> <span class="nam">replace_strings</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t355" href="#t355">355</a></span><span class="t">        <span class="nam">self</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t356" href="#t356">356</a></span><span class="t">        <span class="nam">substitutions</span><span class="op">:</span> <span class="nam">list</span><span class="op">[</span><span class="nam">tuple</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">str</span><span class="op">]</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t356" href="#t356">356</a></span><span class="t">        <span class="nam">substitutions</span><span class="op">:</span> <span class="nam">Sequence</span><span class="op">[</span><span class="nam">tuple</span><span class="op">[</span><span class="nam">str</span><span class="op">,</span> <span class="nam">str</span><span class="op">]</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t357" href="#t357">357</a></span><span class="t">        <span class="nam">count</span><span class="op">:</span> <span class="nam">int</span> <span class="op">=</span> <span class="op">-</span><span class="num">1</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t358" href="#t358">358</a></span><span class="t">        <span class="nam">encoding</span><span class="op">:</span> <span class="nam">Any</span> <span class="op">|</span> <span class="key">None</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t359" href="#t359">359</a></span><span class="t">    <span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t360" href="#t360">360</a></span><span class="t">        <span class="str">"""For each pair in `substitutions`, replace the first string with the second string.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t361" href="#t361">361</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t362" href="#t362">362</a></span><span class="t"><span class="str">        #### :params:</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t363" href="#t363">363</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
@@ -456,15 +456,15 @@
     <p class="pln"><span class="n"><a id="t374" href="#t374">374</a></span><span class="t"><span class="str">        >>> path.write_text(path.read_text().replace("hello", "yeet").replace("goodbye", "yeehaw"))</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t375" href="#t375">375</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t376" href="#t376">376</a></span><span class="t">        <span class="nam">text</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">read_text</span><span class="op">(</span><span class="nam">encoding</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t377" href="#t377">377</a></span><span class="t">        <span class="key">for</span> <span class="nam">sub</span> <span class="key">in</span> <span class="nam">substitutions</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t378" href="#t378">378</a></span><span class="t">            <span class="nam">text</span> <span class="op">=</span> <span class="nam">text</span><span class="op">.</span><span class="nam">replace</span><span class="op">(</span><span class="nam">sub</span><span class="op">[</span><span class="num">0</span><span class="op">]</span><span class="op">,</span> <span class="nam">sub</span><span class="op">[</span><span class="num">1</span><span class="op">]</span><span class="op">,</span> <span class="nam">count</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t379" href="#t379">379</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">write_text</span><span class="op">(</span><span class="nam">text</span><span class="op">,</span> <span class="nam">encoding</span><span class="op">=</span><span class="nam">encoding</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t380" href="#t380">380</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t381" href="#t381">381</a></span><span class="t">    <span class="key">def</span> <span class="nam">join</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">data</span><span class="op">:</span> <span class="nam">list</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span><span class="op">,</span> <span class="nam">encoding</span><span class="op">:</span> <span class="nam">Any</span> <span class="op">|</span> <span class="key">None</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span> <span class="nam">sep</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="str">"\n"</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t381" href="#t381">381</a></span><span class="t">    <span class="key">def</span> <span class="nam">join</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">data</span><span class="op">:</span> <span class="nam">Sequence</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span><span class="op">,</span> <span class="nam">encoding</span><span class="op">:</span> <span class="nam">Any</span> <span class="op">|</span> <span class="key">None</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span> <span class="nam">sep</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="str">"\n"</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t382" href="#t382">382</a></span><span class="t">        <span class="str">"""Write a list of strings, joined by `sep`, to the file pointed at by this instance.</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t383" href="#t383">383</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t384" href="#t384">384</a></span><span class="t"><span class="str">        Equivalent to `Pathier("somefile.txt").write_text(sep.join(data), encoding=encoding)`</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t385" href="#t385">385</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t386" href="#t386">386</a></span><span class="t"><span class="str">        #### :params:</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t387" href="#t387">387</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t388" href="#t388">388</a></span><span class="t"><span class="str">        `encoding`: The file encoding to use.</span>&nbsp;</span><span class="r"></span></p>
@@ -707,13 +707,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_d98317d23aadd1b8___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_a44f0ac069e85531_test_pathier_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.2">coverage.py v7.2.2</a>,
-            created at 2024-02-16 15:27 -0600
+            created at 2024-05-07 16:38 -0500
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -5,29 +5,29 @@
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 224466 ssttaatteemmeennttss ?  221199 rruunn 2277 mmiissssiinngg 00 eexxcclluuddeedd **********
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._2_._2, created at 2024-02-
-16 15:27 -0600
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._2_._2, created at 2024-05-
+07 16:38 -0500
 _1import datetime 
 _2import functools 
 _3import json 
 _4import os 
 _5import pathlib 
 _6import pickle 
 _7import shutil 
 _8import sys 
 _9import time 
 _1_0from typing import Any 
 _1_1 
 _1_2import tomlkit 
-_1_3from typing_extensions import Callable, Self, Sequence, Buffer, IO, Type 
+_1_3from typing_extensions import IO, Buffer, Callable, Self, Sequence 
 _1_4 
 _1_5 
 _1_6class Pathier(pathlib.Path): 
 _1_7 """Subclasses the standard library pathlib.Path class.""" 
 _1_8 
 _1_9 def __new__( 
 _2_0 cls, 
@@ -395,15 +395,15 @@
 _3_4_9 if new_line: 
 _3_5_0 data += "\n" 
 _3_5_1 with self.open("a", encoding=encoding) as file: 
 _3_5_2 file.write(data) 
 _3_5_3 
 _3_5_4 def replace_strings( 
 _3_5_5 self, 
-_3_5_6 substitutions: list[tuple[str, str]], 
+_3_5_6 substitutions: Sequence[tuple[str, str]], 
 _3_5_7 count: int = -1, 
 _3_5_8 encoding: Any | None = None, 
 _3_5_9 ): 
 _3_6_0 """For each pair in `substitutions`, replace the first string with the
 second string. 
 _3_6_1 
 _3_6_2 #### :params: 
@@ -422,15 +422,15 @@
 ("goodbye", "yeehaw")) 
 _3_7_5 """ 
 _3_7_6 text = self.read_text(encoding) 
 _3_7_7 for sub in substitutions: 
 _3_7_8 text = text.replace(sub[0], sub[1], count) 
 _3_7_9 self.write_text(text, encoding=encoding) 
 _3_8_0 
-_3_8_1 def join(self, data: list[str], encoding: Any | None = None, sep: str =
+_3_8_1 def join(self, data: Sequence[str], encoding: Any | None = None, sep: str =
 "\n"): 
 _3_8_2 """Write a list of strings, joined by `sep`, to the file pointed at by this
 instance. 
 _3_8_3 
 _3_8_4 Equivalent to `Pathier("somefile.txt").write_text(sep.join(data),
 encoding=encoding)` 
 _3_8_5 
@@ -686,9 +686,9 @@
 _6_1_6 __slots__ = () 
 _6_1_7 _last_read_time = None 
 _6_1_8 
 _6_1_9 
 _6_2_0class WindowsPath(Pathier, pathlib.PureWindowsPath): 
 _6_2_1 __slots__ = () 
 _6_2_2 _last_read_time = None 
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._2_._2, created at 2024-02-
-16 15:27 -0600
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._2_._2, created at 2024-05-
+07 16:38 -0500
```

### Comparing `pathier-1.5.1/htmlcov/favicon_32.png` & `pathier-1.5.2/htmlcov/favicon_32.png`

 * *Files identical despite different names*

### Comparing `pathier-1.5.1/htmlcov/index.html` & `pathier-1.5.2/htmlcov/index.html`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     <link rel="stylesheet" href="style.css" type="text/css">
     <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="indexfile">
 <header>
     <div class="content">
         <h1>Coverage report:
-            <span class="pc_cov">92%</span>
+            <span class="pc_cov">91%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
                 <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
             <div id="help_panel">
@@ -41,15 +41,15 @@
             </div>
         </aside>
         <form id="filter_container">
             <input id="filter" type="text" value="" placeholder="filter..." />
         </form>
         <p class="text">
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.2">coverage.py v7.2.2</a>,
-            created at 2024-02-16 15:27 -0600
+            created at 2024-05-07 16:42 -0500
         </p>
     </div>
 </header>
 <main id="index">
     <table class="index" data-sortable>
         <thead>
             <tr class="tablehead" title="Click to sort">
@@ -59,18 +59,18 @@
                 <th aria-sort="none" data-default-sort-order="descending" data-shortcut="x">excluded</th>
                 <th class="right" aria-sort="none" data-shortcut="c">coverage</th>
             </tr>
         </thead>
         <tbody>
             <tr class="file">
                 <td class="name left"><a href="d_d98317d23aadd1b8___init___py.html">src\pathier\__init__.py</a></td>
-                <td>19</td>
-                <td>11</td>
+                <td>25</td>
+                <td>15</td>
                 <td>0</td>
-                <td class="right" data-ratio="8 19">42%</td>
+                <td class="right" data-ratio="10 25">40%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_d98317d23aadd1b8_pathier_py.html">src\pathier\pathier.py</a></td>
                 <td>246</td>
                 <td>27</td>
                 <td>0</td>
                 <td class="right" data-ratio="219 246">89%</td>
@@ -82,30 +82,30 @@
                 <td>0</td>
                 <td class="right" data-ratio="210 210">100%</td>
             </tr>
         </tbody>
         <tfoot>
             <tr class="total">
                 <td class="name left">Total</td>
-                <td>475</td>
-                <td>38</td>
+                <td>481</td>
+                <td>42</td>
                 <td>0</td>
-                <td class="right" data-ratio="437 475">92%</td>
+                <td class="right" data-ratio="439 481">91%</td>
             </tr>
         </tfoot>
     </table>
     <p id="no_rows">
         No items found using the specified filter.
     </p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a class="nav" href="https://coverage.readthedocs.io/en/7.2.2">coverage.py v7.2.2</a>,
-            created at 2024-02-16 15:27 -0600
+            created at 2024-05-07 16:42 -0500
         </p>
     </div>
     <aside class="hidden">
         <a id="prevFileLink" class="nav" href="d_a44f0ac069e85531_test_pathier_py.html"/>
         <a id="nextFileLink" class="nav" href="d_d98317d23aadd1b8___init___py.html"/>
         <button type="button" class="button_prev_file" data-shortcut="["/>
         <button type="button" class="button_next_file" data-shortcut="]"/>
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-************ CCoovveerraaggee rreeppoorrtt:: 9922%% ************
+************ CCoovveerraaggee rreeppoorrtt:: 9911%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 n s m x c   change column sorting
 [ ]   prev/next file
 ?   show/hide this help
 [                    ]
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._2_._2, created at 2024-02-16 15:27 -0600
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._2_._2, created at 2024-05-07 16:42 -0500
 MMoodduullee                  ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd ccoovveerraaggee
-_s_r_c_\_p_a_t_h_i_e_r_\_____i_n_i_t_____._p_y 19         11      0        42%
+_s_r_c_\_p_a_t_h_i_e_r_\_____i_n_i_t_____._p_y 25         15      0        40%
 _s_r_c_\_p_a_t_h_i_e_r_\_p_a_t_h_i_e_r_._p_y  246        27      0        89%
 _t_e_s_t_s_\_t_e_s_t___p_a_t_h_i_e_r_._p_y   210        0       0        100%
-Total                   475        38      0        92%
+Total                   481        42      0        91%
 No items found using the specified filter.
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._2_._2, created at 2024-02-16 15:27 -0600
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._2_._2, created at 2024-05-07 16:42 -0500
```

### Comparing `pathier-1.5.1/htmlcov/keybd_closed.png` & `pathier-1.5.2/htmlcov/keybd_closed.png`

 * *Files identical despite different names*

### Comparing `pathier-1.5.1/htmlcov/keybd_open.png` & `pathier-1.5.2/htmlcov/keybd_open.png`

 * *Files identical despite different names*

### Comparing `pathier-1.5.1/htmlcov/style.css` & `pathier-1.5.2/htmlcov/style.css`

 * *Files identical despite different names*

### Comparing `pathier-1.5.1/src/pathier/__init__.py` & `pathier-1.5.2/src/pathier/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,47 @@
+import argparse
+
 import griddle
 import noiftimer
 import printbuddies
+import younotyou
 
 from .pathier import Pathier, Pathish, Pathy
 
 __all__ = ["Pathier", "Pathy", "Pathish"]
 
 
 @noiftimer.time_it()
 def sizeup():
     """Print the sub-directories and their sizes of the current working directory."""
+    parser = argparse.ArgumentParser("sizeup")
+    parser.add_argument(
+        "-i",
+        "--ignore",
+        nargs="*",
+        default=None,
+        type=str,
+        help="Directory patterns to ignore.",
+    )
+    args = parser.parse_args()
+    matcher = younotyou.Matcher(exclude_patterns=args.ignore)
     sizes: dict[str, int] = {}
-    folders = [folder for folder in Pathier.cwd().iterdir() if folder.is_dir()]
+    folders = [
+        folder
+        for folder in Pathier.cwd().iterdir()
+        if folder.is_dir() and str(folder) not in matcher
+    ]
     print(f"Sizing up {len(folders)} directories...")
     with printbuddies.ProgBar(len(folders)) as prog:
         for folder in folders:
             prog.display(f"Scanning '{folder.name}'")
             sizes[folder.name] = folder.size
     total_size = sum(sizes[folder] for folder in sizes)
     size_list = [
         (folder, Pathier.format_bytes(sizes[folder]))
         for folder in sorted(list(sizes.keys()), key=lambda f: sizes[f], reverse=True)
     ]
     print(griddle.griddy(size_list, ["Dir", "Size"]))
     print(f"Total size of '{Pathier.cwd()}': {Pathier.format_bytes(total_size)}")
 
 
-__version__ = "1.5.1"
+__version__ = "1.5.2"
```

### Comparing `pathier-1.5.1/src/pathier/pathier.py` & `pathier-1.5.2/src/pathier/pathier.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import pickle
 import shutil
 import sys
 import time
 from typing import Any
 
 import tomlkit
-from typing_extensions import IO, Buffer, Callable, Self, Sequence, Type
+from typing_extensions import IO, Buffer, Callable, Self, Sequence
 
 
 class Pathier(pathlib.Path):
     """Subclasses the standard library pathlib.Path class."""
 
     def __new__(
         cls,
@@ -349,15 +349,15 @@
         if new_line:
             data += "\n"
         with self.open("a", encoding=encoding) as file:
             file.write(data)
 
     def replace_strings(
         self,
-        substitutions: list[tuple[str, str]],
+        substitutions: Sequence[tuple[str, str]],
         count: int = -1,
         encoding: Any | None = None,
     ):
         """For each pair in `substitutions`, replace the first string with the second string.
 
         #### :params:
 
@@ -374,15 +374,15 @@
         >>> path.write_text(path.read_text().replace("hello", "yeet").replace("goodbye", "yeehaw"))
         """
         text = self.read_text(encoding)
         for sub in substitutions:
             text = text.replace(sub[0], sub[1], count)
         self.write_text(text, encoding=encoding)
 
-    def join(self, data: list[str], encoding: Any | None = None, sep: str = "\n"):
+    def join(self, data: Sequence[str], encoding: Any | None = None, sep: str = "\n"):
         """Write a list of strings, joined by `sep`, to the file pointed at by this instance.
 
         Equivalent to `Pathier("somefile.txt").write_text(sep.join(data), encoding=encoding)`
 
         #### :params:
 
         `encoding`: The file encoding to use.
```

### Comparing `pathier-1.5.1/LICENSE.txt` & `pathier-1.5.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pathier-1.5.1/README.md` & `pathier-1.5.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -2,33 +2,33 @@
 
 Extends the standard library pathlib.Path class.
 
 ## Installation
 
 Install with:
 
-<pre>
+```console
 pip install pathier
-</pre>
-
-
+```
 
 ## Usage
 
-Functions the same as pathlib.Path, but with added functions and some altered default arguments.<br>
+Functions the same as pathlib.Path, but with added functions and some altered default arguments.  
 
 #### Navigation
 
-New paths can be obtained by:<br>
+New paths can be obtained by:  
+
 * naming the parent with moveup()
 * subtracting a number of levels from the current path
 * naming the parent of the path you actually want with move_under()
 * separating a relative path at a named parent with separate()
 * set current working directory to path
-<pre>
+
+```python
 >>> from pathier import Pathier
 >>> path = Pathier("C:/some/directory/to/some/file/on/the/system")
 >>> path.moveup("directory")
 WindowsPath('C:/some/directory')
 >>> path - 3
 WindowsPath('C:/some/directory/to/some/file')
 >>> path.move_under("directory")
@@ -36,77 +36,80 @@
 >>> path.separate("file")
 WindowsPath('on/the/system')
 >>> path.separate("file", True)
 WindowsPath('file/on/the/system')
 >>> path.mkcwd()
 >>> Pathier.cwd()
 WindowsPath('C:/some/directory/to/some/file/on/the/system')
-</pre>
+```
 
 #### Environment PATH Variable
 
-Pathier objects can be added and removed from sys.path:<br>
+Pathier objects can be added and removed from sys.path:  
 (The path will only be added if it isn't already in sys.path)
-<pre>
+
+```python
 >>> from pathier import Pathier
 >>> path = Pathier.cwd()
 >>> path.in_PATH
 False
 >>> path.add_to_PATH(0)
 >>> path.in_PATH
 True
 >>> path.remove_from_PATH()
 >>> path.in_PATH
 False
 >>> path.append_to_PATH()
 >>> path.in_PATH
 True
-</pre>
-
+```
 
 #### Read and Write
 
 Can dump and load toml, json, and pickle files without needed to explicityly import and call functions from the respective libraries:
-<pre>
+
+```python
 from pathier import Pathier
 path = Pathier("some_file.toml")
 content = path.loads()
 path.with_suffix(".json").dumps(content, indent=2)
-</pre>
+```
 
-`Pathier().mkdir()` creates parent directories and doesn't throw an error if the path already exists by default.<br>
+`Pathier().mkdir()` creates parent directories and doesn't throw an error if the path already exists by default.  
 
-`Pathier().write_text()` and `Pathier().write_bytes()` will create parent directories by default if they won't exist.<br>
+`Pathier().write_text()` and `Pathier().write_bytes()` will create parent directories by default if they won't exist.  
 
-`Pathier().write_text()` will also try to cast the data to be written to a string if a TypeError is thrown.<br>
+`Pathier().write_text()` will also try to cast the data to be written to a string if a TypeError is thrown.  
 
-`Pathier().delete()` will delete a file or directory, event if that directory isn't empty.<br>
+`Pathier().delete()` will delete a file or directory, event if that directory isn't empty.  
 
-`Pathier().copy()` will copy a file or a directory tree to a new destination and return a Pathier object for the new path<br>
-By default, files in the destination will not be overwritten.<br>
+`Pathier().copy()` will copy a file or a directory tree to a new destination and return a Pathier object for the new path  
+By default, files in the destination will not be overwritten.  
 
 `Pathier().backup()` will create a copy of the path with `_backup` appended to the stem.
-If the optional parameter, `timestamp`, is `True`, a datetime string will be added after `_backup` to prevent overwriting previous backup files.<br>
+If the optional parameter, `timestamp`, is `True`, a datetime string will be added after `_backup` to prevent overwriting previous backup files.  
+
+`Pathier().replace_strings()` takes a list of string pairs and will read the file the instance points to, replace the first of each pair with the second of each pair, and then write it back to the file.  
+Essentially just condenses reading the file, using str.replace(), and then writing the new content into one function call.  
 
-`Pathier().replace_strings()` takes a list of string pairs and will read the file the instance points to, replace the first of each pair with the second of each pair, and then write it back to the file.<br>
-Essentially just condenses reading the file, using str.replace(), and then writing the new content into one function call.<br>
+`Pathier().execute()` wraps calling `os.system()` on the path pointed to be the `Pathier` instance.  
+Optional strings that should come before and after the path string can be specified with the `command` and `args` params, respectively.  
+`Pathier("file.py").execute("py", "--iterations 10")` is equivalent to `os.system("py file.py --iterations 10")`  
 
-`Pathier().execute()` wraps calling `os.system()` on the path pointed to be the `Pathier` instance.<br>
-Optional strings that should come before and after the path string can be specified with the `command` and `args` params, respectively.<br>
-`Pathier("file.py").execute("py", "--iterations 10")` is equivalent to `os.system("py file.py --iterations 10")`<br>
+`Pathier().append()` will append the given string to the file pointed at by the instance.  
 
-`Pathier().append()` will append the given string to the file pointed at by the instance.<br>
+`Pathier().join(data)` is equivalent to calling `Pathier().write_text("\n".join(data))`.  
+The joining string can be specified with the `sep` parameter.  
 
-`Pathier().join(data)` is equivalent to calling `Pathier().write_text("\n".join(data))`.<br>
-The joining string can be specified with the `sep` parameter.<br>
+`Pathier().split()` is equivalent to calling `Pathier().read_text().splitlines()`.  
+Optionally, line endings can be kept with `Pathier().split(keepends=True)`.  
 
-`Pathier().split()` is equivalent to calling `Pathier().read_text().splitlines()`.<br>
-Optionally, line endings can be kept with `Pathier().split(keepends=True)`.<br>
 #### Stats and Comparisons
-<pre>
+
+```python
 >>> from pathier import Pathier
 >>> p = Pathier.cwd() / "pathier.py"
 >>> i = p.parent / "__init__.py"
 >>> p.dob
 datetime.datetime(2023, 3, 31, 18, 43, 12, 360000)
 >>> p.age
 8846.024934
@@ -122,19 +125,21 @@
 '10.74 kb'
 >>> p.is_larger(i)
 True
 >>> p.is_older(i)
 False
 >>> p.modified_more_recently(i)
 True
-</pre>
+```
 
 #### CLI Scripts
+
 Execute `sizeup` from a terminal to get a grid of sub-directories and their sizes.
-<pre>
+
+```console
 P:\python\projects\pathier>sizeup
 Sizing up 7 directories...
 Scanning 'dist' [____________________________________________________________________________________________________________________________________________]-100.00%
 +---------------+-----------+
 | Dir           | Size      |
 +===============+===========+
 | docs          | 362.74 kb |
@@ -149,8 +154,8 @@
 +---------------+-----------+
 | .pytest_cache | 540 bytes |
 +---------------+-----------+
 | .vscode       | 197 bytes |
 +---------------+-----------+
 Total size of 'P:\python\projects\pathier': 564.11 kb
 sizeup average execution time: 37ms 895us
-</pre>
+```
```

### Comparing `pathier-1.5.1/pyproject.toml` & `pathier-1.5.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name = "pathier"
 description = "Extends the standard library pathlib.Path class."
-version = "1.5.1"
-dependencies = ["tomlkit>=0.11.8", "typing_extensions", "griddle", "noiftimer", "printbuddies"]
+version = "1.5.2"
+dependencies = ["tomlkit>=0.11.8", "typing_extensions", "griddle", "noiftimer", "printbuddies", "younotyou"]
 readme = "README.md"
 keywords = ["pathlib", "path", "json", "toml", "shutil", "extender", "extension"]
 classifiers = ["Programming Language :: Python :: 3", "License :: OSI Approved :: MIT License", "Operating System :: OS Independent"]
 requires-python = ">=3.10, <3.12"
 
 [[project.authors]]
 name = "Matt Manes"
```

### Comparing `pathier-1.5.1/PKG-INFO` & `pathier-1.5.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: pathier
-Version: 1.5.1
+Version: 1.5.2
 Summary: Extends the standard library pathlib.Path class.
 Project-URL: Homepage, https://github.com/matt-manes/pathier
 Project-URL: Documentation, https://github.com/matt-manes/pathier/tree/main/docs
 Project-URL: Source code, https://github.com/matt-manes/pathier/tree/main/src/pathier
 Author-email: Matt Manes <mattmanes@pm.me>
 License-File: LICENSE.txt
 Keywords: extender,extension,json,path,pathlib,shutil,toml
@@ -13,43 +13,44 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Python: <3.12,>=3.10
 Requires-Dist: griddle
 Requires-Dist: noiftimer
 Requires-Dist: printbuddies
 Requires-Dist: tomlkit>=0.11.8
 Requires-Dist: typing-extensions
+Requires-Dist: younotyou
 Description-Content-Type: text/markdown
 
 # pathier
 
 Extends the standard library pathlib.Path class.
 
 ## Installation
 
 Install with:
 
-<pre>
+```console
 pip install pathier
-</pre>
-
-
+```
 
 ## Usage
 
-Functions the same as pathlib.Path, but with added functions and some altered default arguments.<br>
+Functions the same as pathlib.Path, but with added functions and some altered default arguments.  
 
 #### Navigation
 
-New paths can be obtained by:<br>
+New paths can be obtained by:  
+
 * naming the parent with moveup()
 * subtracting a number of levels from the current path
 * naming the parent of the path you actually want with move_under()
 * separating a relative path at a named parent with separate()
 * set current working directory to path
-<pre>
+
+```python
 >>> from pathier import Pathier
 >>> path = Pathier("C:/some/directory/to/some/file/on/the/system")
 >>> path.moveup("directory")
 WindowsPath('C:/some/directory')
 >>> path - 3
 WindowsPath('C:/some/directory/to/some/file')
 >>> path.move_under("directory")
@@ -57,77 +58,80 @@
 >>> path.separate("file")
 WindowsPath('on/the/system')
 >>> path.separate("file", True)
 WindowsPath('file/on/the/system')
 >>> path.mkcwd()
 >>> Pathier.cwd()
 WindowsPath('C:/some/directory/to/some/file/on/the/system')
-</pre>
+```
 
 #### Environment PATH Variable
 
-Pathier objects can be added and removed from sys.path:<br>
+Pathier objects can be added and removed from sys.path:  
 (The path will only be added if it isn't already in sys.path)
-<pre>
+
+```python
 >>> from pathier import Pathier
 >>> path = Pathier.cwd()
 >>> path.in_PATH
 False
 >>> path.add_to_PATH(0)
 >>> path.in_PATH
 True
 >>> path.remove_from_PATH()
 >>> path.in_PATH
 False
 >>> path.append_to_PATH()
 >>> path.in_PATH
 True
-</pre>
-
+```
 
 #### Read and Write
 
 Can dump and load toml, json, and pickle files without needed to explicityly import and call functions from the respective libraries:
-<pre>
+
+```python
 from pathier import Pathier
 path = Pathier("some_file.toml")
 content = path.loads()
 path.with_suffix(".json").dumps(content, indent=2)
-</pre>
+```
 
-`Pathier().mkdir()` creates parent directories and doesn't throw an error if the path already exists by default.<br>
+`Pathier().mkdir()` creates parent directories and doesn't throw an error if the path already exists by default.  
 
-`Pathier().write_text()` and `Pathier().write_bytes()` will create parent directories by default if they won't exist.<br>
+`Pathier().write_text()` and `Pathier().write_bytes()` will create parent directories by default if they won't exist.  
 
-`Pathier().write_text()` will also try to cast the data to be written to a string if a TypeError is thrown.<br>
+`Pathier().write_text()` will also try to cast the data to be written to a string if a TypeError is thrown.  
 
-`Pathier().delete()` will delete a file or directory, event if that directory isn't empty.<br>
+`Pathier().delete()` will delete a file or directory, event if that directory isn't empty.  
 
-`Pathier().copy()` will copy a file or a directory tree to a new destination and return a Pathier object for the new path<br>
-By default, files in the destination will not be overwritten.<br>
+`Pathier().copy()` will copy a file or a directory tree to a new destination and return a Pathier object for the new path  
+By default, files in the destination will not be overwritten.  
 
 `Pathier().backup()` will create a copy of the path with `_backup` appended to the stem.
-If the optional parameter, `timestamp`, is `True`, a datetime string will be added after `_backup` to prevent overwriting previous backup files.<br>
+If the optional parameter, `timestamp`, is `True`, a datetime string will be added after `_backup` to prevent overwriting previous backup files.  
+
+`Pathier().replace_strings()` takes a list of string pairs and will read the file the instance points to, replace the first of each pair with the second of each pair, and then write it back to the file.  
+Essentially just condenses reading the file, using str.replace(), and then writing the new content into one function call.  
 
-`Pathier().replace_strings()` takes a list of string pairs and will read the file the instance points to, replace the first of each pair with the second of each pair, and then write it back to the file.<br>
-Essentially just condenses reading the file, using str.replace(), and then writing the new content into one function call.<br>
+`Pathier().execute()` wraps calling `os.system()` on the path pointed to be the `Pathier` instance.  
+Optional strings that should come before and after the path string can be specified with the `command` and `args` params, respectively.  
+`Pathier("file.py").execute("py", "--iterations 10")` is equivalent to `os.system("py file.py --iterations 10")`  
 
-`Pathier().execute()` wraps calling `os.system()` on the path pointed to be the `Pathier` instance.<br>
-Optional strings that should come before and after the path string can be specified with the `command` and `args` params, respectively.<br>
-`Pathier("file.py").execute("py", "--iterations 10")` is equivalent to `os.system("py file.py --iterations 10")`<br>
+`Pathier().append()` will append the given string to the file pointed at by the instance.  
 
-`Pathier().append()` will append the given string to the file pointed at by the instance.<br>
+`Pathier().join(data)` is equivalent to calling `Pathier().write_text("\n".join(data))`.  
+The joining string can be specified with the `sep` parameter.  
 
-`Pathier().join(data)` is equivalent to calling `Pathier().write_text("\n".join(data))`.<br>
-The joining string can be specified with the `sep` parameter.<br>
+`Pathier().split()` is equivalent to calling `Pathier().read_text().splitlines()`.  
+Optionally, line endings can be kept with `Pathier().split(keepends=True)`.  
 
-`Pathier().split()` is equivalent to calling `Pathier().read_text().splitlines()`.<br>
-Optionally, line endings can be kept with `Pathier().split(keepends=True)`.<br>
 #### Stats and Comparisons
-<pre>
+
+```python
 >>> from pathier import Pathier
 >>> p = Pathier.cwd() / "pathier.py"
 >>> i = p.parent / "__init__.py"
 >>> p.dob
 datetime.datetime(2023, 3, 31, 18, 43, 12, 360000)
 >>> p.age
 8846.024934
@@ -143,19 +147,21 @@
 '10.74 kb'
 >>> p.is_larger(i)
 True
 >>> p.is_older(i)
 False
 >>> p.modified_more_recently(i)
 True
-</pre>
+```
 
 #### CLI Scripts
+
 Execute `sizeup` from a terminal to get a grid of sub-directories and their sizes.
-<pre>
+
+```console
 P:\python\projects\pathier>sizeup
 Sizing up 7 directories...
 Scanning 'dist' [____________________________________________________________________________________________________________________________________________]-100.00%
 +---------------+-----------+
 | Dir           | Size      |
 +===============+===========+
 | docs          | 362.74 kb |
@@ -170,8 +176,8 @@
 +---------------+-----------+
 | .pytest_cache | 540 bytes |
 +---------------+-----------+
 | .vscode       | 197 bytes |
 +---------------+-----------+
 Total size of 'P:\python\projects\pathier': 564.11 kb
 sizeup average execution time: 37ms 895us
-</pre>
+```
```

