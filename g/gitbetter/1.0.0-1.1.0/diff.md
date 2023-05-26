# Comparing `tmp/gitbetter-1.0.0.tar.gz` & `tmp/gitbetter-1.1.0.tar.gz`

## Comparing `gitbetter-1.0.0.tar` & `gitbetter-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 gitbetter-1.0.0/CHANGELOG.md
--rw-r--r--   0        0        0    34128 2020-02-02 00:00:00.000000 gitbetter-1.0.0/docs/gitbetter.html
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 gitbetter-1.0.0/docs/index.html
--rw-r--r--   0        0        0    63165 2020-02-02 00:00:00.000000 gitbetter-1.0.0/docs/search.js
--rw-r--r--   0        0        0   224647 2020-02-02 00:00:00.000000 gitbetter-1.0.0/docs/gitbetter/git.html
--rw-r--r--   0        0        0   249963 2020-02-02 00:00:00.000000 gitbetter-1.0.0/docs/gitbetter/gitbetter.html
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 gitbetter-1.0.0/src/gitbetter/__init__.py
--rw-r--r--   0        0        0     8480 2020-02-02 00:00:00.000000 gitbetter-1.0.0/src/gitbetter/git.py
--rw-r--r--   0        0        0    10217 2020-02-02 00:00:00.000000 gitbetter-1.0.0/src/gitbetter/gitbetter.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 gitbetter-1.0.0/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 gitbetter-1.0.0/LICENSE.txt
--rw-r--r--   0        0        0     5091 2020-02-02 00:00:00.000000 gitbetter-1.0.0/README.md
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 gitbetter-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     5670 2020-02-02 00:00:00.000000 gitbetter-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 gitbetter-1.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0    34128 2020-02-02 00:00:00.000000 gitbetter-1.1.0/docs/gitbetter.html
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 gitbetter-1.1.0/docs/index.html
+-rw-r--r--   0        0        0    63347 2020-02-02 00:00:00.000000 gitbetter-1.1.0/docs/search.js
+-rw-r--r--   0        0        0   226499 2020-02-02 00:00:00.000000 gitbetter-1.1.0/docs/gitbetter/git.html
+-rw-r--r--   0        0        0   249963 2020-02-02 00:00:00.000000 gitbetter-1.1.0/docs/gitbetter/gitbetter.html
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 gitbetter-1.1.0/src/gitbetter/__init__.py
+-rw-r--r--   0        0        0     8593 2020-02-02 00:00:00.000000 gitbetter-1.1.0/src/gitbetter/git.py
+-rw-r--r--   0        0        0    10217 2020-02-02 00:00:00.000000 gitbetter-1.1.0/src/gitbetter/gitbetter.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 gitbetter-1.1.0/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 gitbetter-1.1.0/LICENSE.txt
+-rw-r--r--   0        0        0     5091 2020-02-02 00:00:00.000000 gitbetter-1.1.0/README.md
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 gitbetter-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     5670 2020-02-02 00:00:00.000000 gitbetter-1.1.0/PKG-INFO
```

### Comparing `gitbetter-1.0.0/CHANGELOG.md` & `gitbetter-1.1.0/CHANGELOG.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,41 @@
 # Changelog
 
+## v1.0.0 (2023-05-21)
+
+#### New Features
+
+* all git functions can return stdout as a string
+#### Fixes
+
+* fix issue where git.add() would remove path separators
+#### Refactorings
+
+* git bindings are now contained in the `Git` class
+* do_commit() doesn't assume arg string is a message
+* make capture_stdout a class property
+* update shell to use Git class
+* move git functions into a class so dev can specify whether to capture stdout or not
+#### Docs
+
+* update readme
+
+
 ## v0.5.2 (2023-05-15)
 
 #### Fixes
 
 * fix create_remote_from_cwd function to properly add remote and push
 
 
 ## v0.5.1 (2023-05-13)
 
 #### Fixes
 
 * fix  create_remote_from_cwd() not setting remote to upstream
-#### Others
-
-* build v0.5.1
-* update changelog
 
 
 ## v0.5.0 (2023-05-11)
 
 #### New Features
 
 * add create_remote_from_cwd()
@@ -27,40 +43,28 @@
 
 * rename do_list_branches() to do_branches()
 * do_new_gh_remote invokes create_remote_from_cwd so url no longer needs to be added manually after creating remote
 #### Docs
 
 * update readme
 * update doc string
-#### Others
-
-* build v0.5.0
-* update changelog
 
 
 ## v0.4.0 (2023-05-04)
 
 #### New Features
 
 * add status command
-#### Others
-
-* build v0.4.0
-* update changelog
 
 
 ## v0.3.0 (2023-05-02)
 
 #### Refactorings
 
 * remove do_cmd as it's now covered by parent class's do_sys
-#### Others
-
-* build v0.3.0
-* update changelog
 
 
 ## v0.2.0 (2023-05-02)
 
 #### New Features
 
 * override do_help to display unrecognized_command_behavior_status after standard help message
@@ -72,29 +76,21 @@
 * set requires-python to >=3.10
 #### Refactorings
 
 * remove cwd command
 #### Docs
 
 * update readme
-#### Others
-
-* build v0.2.0
-* update changelog
 
 
 ## v0.1.1 (2023-04-30)
 
 #### Fixes
 
 * cast Pathier objects to strings in recurse_files()
-#### Others
-
-* build v0.1.1
-* update changelog
 
 
 ## v0.1.0 (2023-04-30)
 
 #### New Features
 
 * add do_cmd() to excute shell commands without quitting gitbetter
@@ -102,14 +98,10 @@
 #### Refactorings
 
 * rename some functions
 #### Docs
 
 * update readme
 * add future feature to list in readme
-#### Others
-
-* build v0.1.0
-* update changelog
 
 
 ## v0.0.0 (2023-04-29)
```

### Comparing `gitbetter-1.0.0/docs/gitbetter.html` & `gitbetter-1.1.0/docs/gitbetter.html`

 * *Files identical despite different names*

### Comparing `gitbetter-1.0.0/docs/search.js` & `gitbetter-1.1.0/docs/search.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -785,16 +785,16 @@
         "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span>, </span><span class=\"param\"><span class=\"n\">files</span><span class=\"p\">:</span> <span class=\"nb\">list</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">]</span> <span class=\"o\">|</span> <span class=\"kc\">None</span> <span class=\"o\">=</span> <span class=\"kc\">None</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">str</span> <span class=\"o\">|</span> <span class=\"nb\">int</span>:</span></span>",
         "funcdef": "def"
     }, {
         "fullname": "gitbetter.git.Git.tag",
         "modulename": "gitbetter.git",
         "qualname": "Git.tag",
         "kind": "function",
-        "doc": "<p>Tag the current commit with <code>id_</code>.</p>\n\n<p>Equivalent to <code>git tag {id_}</code>.</p>\n",
-        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span>, </span><span class=\"param\"><span class=\"n\">id_</span><span class=\"p\">:</span> <span class=\"nb\">str</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">str</span> <span class=\"o\">|</span> <span class=\"nb\">int</span>:</span></span>",
+        "doc": "<p>Execute the <code>tag</code> command with <code>args</code>.</p>\n\n<p>e.g.</p>\n\n<p><code>self.tag(\"--sort=-committerdate\")</code></p>\n\n<p>will list all the tags for this repository in descending commit date.</p>\n",
+        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span>, </span><span class=\"param\"><span class=\"n\">args</span><span class=\"p\">:</span> <span class=\"nb\">str</span> <span class=\"o\">=</span> <span class=\"s1\">&#39;&#39;</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">str</span> <span class=\"o\">|</span> <span class=\"nb\">int</span>:</span></span>",
         "funcdef": "def"
     }, {
         "fullname": "gitbetter.git.Git.add_remote_url",
         "modulename": "gitbetter.git",
         "qualname": "Git.add_remote_url",
         "kind": "function",
         "doc": "<p>Add remote url to repo.</p>\n",
```

### Comparing `gitbetter-1.0.0/docs/gitbetter/git.html` & `gitbetter-1.1.0/docs/gitbetter/git.html`

 * *Files 1% similar despite different names*

```diff
@@ -224,148 +224,152 @@
 </span><span id="L-75"><a href="#L-75"><span class="linenos"> 75</span></a>
 </span><span id="L-76"><a href="#L-76"><span class="linenos"> 76</span></a><span class="sd">        Equivalent to:</span>
 </span><span id="L-77"><a href="#L-77"><span class="linenos"> 77</span></a><span class="sd">        &gt;&gt;&gt; git add {files}</span>
 </span><span id="L-78"><a href="#L-78"><span class="linenos"> 78</span></a><span class="sd">        &gt;&gt;&gt; git commit --amend --no-edit</span>
 </span><span id="L-79"><a href="#L-79"><span class="linenos"> 79</span></a><span class="sd">        &quot;&quot;&quot;</span>
 </span><span id="L-80"><a href="#L-80"><span class="linenos"> 80</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">add</span><span class="p">(</span><span class="n">files</span><span class="p">)</span> <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">commit</span><span class="p">(</span><span class="s2">&quot;--amend --no-edit&quot;</span><span class="p">)</span>  <span class="c1"># type: ignore</span>
 </span><span id="L-81"><a href="#L-81"><span class="linenos"> 81</span></a>
-</span><span id="L-82"><a href="#L-82"><span class="linenos"> 82</span></a>    <span class="k">def</span> <span class="nf">tag</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">id_</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="L-83"><a href="#L-83"><span class="linenos"> 83</span></a>        <span class="sd">&quot;&quot;&quot;Tag the current commit with `id_`.</span>
+</span><span id="L-82"><a href="#L-82"><span class="linenos"> 82</span></a>    <span class="k">def</span> <span class="nf">tag</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="L-83"><a href="#L-83"><span class="linenos"> 83</span></a>        <span class="sd">&quot;&quot;&quot;Execute the `tag` command with `args`.</span>
 </span><span id="L-84"><a href="#L-84"><span class="linenos"> 84</span></a>
-</span><span id="L-85"><a href="#L-85"><span class="linenos"> 85</span></a><span class="sd">        Equivalent to `git tag {id_}`.&quot;&quot;&quot;</span>
-</span><span id="L-86"><a href="#L-86"><span class="linenos"> 86</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;tag </span><span class="si">{</span><span class="n">id_</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-87"><a href="#L-87"><span class="linenos"> 87</span></a>
-</span><span id="L-88"><a href="#L-88"><span class="linenos"> 88</span></a>    <span class="c1"># ==========================================Push/Pull==========================================</span>
-</span><span id="L-89"><a href="#L-89"><span class="linenos"> 89</span></a>    <span class="k">def</span> <span class="nf">add_remote_url</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">url</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;origin&quot;</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="L-90"><a href="#L-90"><span class="linenos"> 90</span></a>        <span class="sd">&quot;&quot;&quot;Add remote url to repo.&quot;&quot;&quot;</span>
-</span><span id="L-91"><a href="#L-91"><span class="linenos"> 91</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;remote add </span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">url</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-92"><a href="#L-92"><span class="linenos"> 92</span></a>
-</span><span id="L-93"><a href="#L-93"><span class="linenos"> 93</span></a>    <span class="k">def</span> <span class="nf">push</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="L-94"><a href="#L-94"><span class="linenos"> 94</span></a>        <span class="sd">&quot;&quot;&quot;Equivalent to `git push {args}`.&quot;&quot;&quot;</span>
-</span><span id="L-95"><a href="#L-95"><span class="linenos"> 95</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;push </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-85"><a href="#L-85"><span class="linenos"> 85</span></a><span class="sd">        e.g.</span>
+</span><span id="L-86"><a href="#L-86"><span class="linenos"> 86</span></a>
+</span><span id="L-87"><a href="#L-87"><span class="linenos"> 87</span></a><span class="sd">        `self.tag(&quot;--sort=-committerdate&quot;)`</span>
+</span><span id="L-88"><a href="#L-88"><span class="linenos"> 88</span></a>
+</span><span id="L-89"><a href="#L-89"><span class="linenos"> 89</span></a><span class="sd">        will list all the tags for this repository in descending commit date.&quot;&quot;&quot;</span>
+</span><span id="L-90"><a href="#L-90"><span class="linenos"> 90</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;tag </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-91"><a href="#L-91"><span class="linenos"> 91</span></a>
+</span><span id="L-92"><a href="#L-92"><span class="linenos"> 92</span></a>    <span class="c1"># ==========================================Push/Pull==========================================</span>
+</span><span id="L-93"><a href="#L-93"><span class="linenos"> 93</span></a>    <span class="k">def</span> <span class="nf">add_remote_url</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">url</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;origin&quot;</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="L-94"><a href="#L-94"><span class="linenos"> 94</span></a>        <span class="sd">&quot;&quot;&quot;Add remote url to repo.&quot;&quot;&quot;</span>
+</span><span id="L-95"><a href="#L-95"><span class="linenos"> 95</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;remote add </span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">url</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span><span id="L-96"><a href="#L-96"><span class="linenos"> 96</span></a>
-</span><span id="L-97"><a href="#L-97"><span class="linenos"> 97</span></a>    <span class="k">def</span> <span class="nf">pull</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="L-98"><a href="#L-98"><span class="linenos"> 98</span></a>        <span class="sd">&quot;&quot;&quot;Equivalent to `git pull {args}`.&quot;&quot;&quot;</span>
-</span><span id="L-99"><a href="#L-99"><span class="linenos"> 99</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;pull </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-97"><a href="#L-97"><span class="linenos"> 97</span></a>    <span class="k">def</span> <span class="nf">push</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="L-98"><a href="#L-98"><span class="linenos"> 98</span></a>        <span class="sd">&quot;&quot;&quot;Equivalent to `git push {args}`.&quot;&quot;&quot;</span>
+</span><span id="L-99"><a href="#L-99"><span class="linenos"> 99</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;push </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span><span id="L-100"><a href="#L-100"><span class="linenos">100</span></a>
-</span><span id="L-101"><a href="#L-101"><span class="linenos">101</span></a>    <span class="k">def</span> <span class="nf">push_new_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="L-102"><a href="#L-102"><span class="linenos">102</span></a>        <span class="sd">&quot;&quot;&quot;Push a new branch to origin with tracking.</span>
-</span><span id="L-103"><a href="#L-103"><span class="linenos">103</span></a>
-</span><span id="L-104"><a href="#L-104"><span class="linenos">104</span></a><span class="sd">        Equivalent to `git push -u origin {branch}`.&quot;&quot;&quot;</span>
-</span><span id="L-105"><a href="#L-105"><span class="linenos">105</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;-u origin </span><span class="si">{</span><span class="n">branch</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-106"><a href="#L-106"><span class="linenos">106</span></a>
-</span><span id="L-107"><a href="#L-107"><span class="linenos">107</span></a>    <span class="k">def</span> <span class="nf">pull_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="L-108"><a href="#L-108"><span class="linenos">108</span></a>        <span class="sd">&quot;&quot;&quot;Pull `branch` from origin.&quot;&quot;&quot;</span>
-</span><span id="L-109"><a href="#L-109"><span class="linenos">109</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">pull</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;origin </span><span class="si">{</span><span class="n">branch</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-101"><a href="#L-101"><span class="linenos">101</span></a>    <span class="k">def</span> <span class="nf">pull</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="L-102"><a href="#L-102"><span class="linenos">102</span></a>        <span class="sd">&quot;&quot;&quot;Equivalent to `git pull {args}`.&quot;&quot;&quot;</span>
+</span><span id="L-103"><a href="#L-103"><span class="linenos">103</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;pull </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-104"><a href="#L-104"><span class="linenos">104</span></a>
+</span><span id="L-105"><a href="#L-105"><span class="linenos">105</span></a>    <span class="k">def</span> <span class="nf">push_new_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="L-106"><a href="#L-106"><span class="linenos">106</span></a>        <span class="sd">&quot;&quot;&quot;Push a new branch to origin with tracking.</span>
+</span><span id="L-107"><a href="#L-107"><span class="linenos">107</span></a>
+</span><span id="L-108"><a href="#L-108"><span class="linenos">108</span></a><span class="sd">        Equivalent to `git push -u origin {branch}`.&quot;&quot;&quot;</span>
+</span><span id="L-109"><a href="#L-109"><span class="linenos">109</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;-u origin </span><span class="si">{</span><span class="n">branch</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span><span id="L-110"><a href="#L-110"><span class="linenos">110</span></a>
-</span><span id="L-111"><a href="#L-111"><span class="linenos">111</span></a>    <span class="c1"># ============================================Checkout/Branches============================================</span>
-</span><span id="L-112"><a href="#L-112"><span class="linenos">112</span></a>    <span class="k">def</span> <span class="nf">branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="L-113"><a href="#L-113"><span class="linenos">113</span></a>        <span class="sd">&quot;&quot;&quot;Equivalent to `git branch {args}`.&quot;&quot;&quot;</span>
-</span><span id="L-114"><a href="#L-114"><span class="linenos">114</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;branch </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-115"><a href="#L-115"><span class="linenos">115</span></a>
-</span><span id="L-116"><a href="#L-116"><span class="linenos">116</span></a>    <span class="k">def</span> <span class="nf">list_branches</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="L-117"><a href="#L-117"><span class="linenos">117</span></a>        <span class="sd">&quot;&quot;&quot;Print a list of branches.&quot;&quot;&quot;</span>
-</span><span id="L-118"><a href="#L-118"><span class="linenos">118</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">branch</span><span class="p">(</span><span class="s2">&quot;-vva&quot;</span><span class="p">)</span>
+</span><span id="L-111"><a href="#L-111"><span class="linenos">111</span></a>    <span class="k">def</span> <span class="nf">pull_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="L-112"><a href="#L-112"><span class="linenos">112</span></a>        <span class="sd">&quot;&quot;&quot;Pull `branch` from origin.&quot;&quot;&quot;</span>
+</span><span id="L-113"><a href="#L-113"><span class="linenos">113</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">pull</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;origin </span><span class="si">{</span><span class="n">branch</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-114"><a href="#L-114"><span class="linenos">114</span></a>
+</span><span id="L-115"><a href="#L-115"><span class="linenos">115</span></a>    <span class="c1"># ============================================Checkout/Branches============================================</span>
+</span><span id="L-116"><a href="#L-116"><span class="linenos">116</span></a>    <span class="k">def</span> <span class="nf">branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="L-117"><a href="#L-117"><span class="linenos">117</span></a>        <span class="sd">&quot;&quot;&quot;Equivalent to `git branch {args}`.&quot;&quot;&quot;</span>
+</span><span id="L-118"><a href="#L-118"><span class="linenos">118</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;branch </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span><span id="L-119"><a href="#L-119"><span class="linenos">119</span></a>
-</span><span id="L-120"><a href="#L-120"><span class="linenos">120</span></a>    <span class="k">def</span> <span class="nf">checkout</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="L-121"><a href="#L-121"><span class="linenos">121</span></a>        <span class="sd">&quot;&quot;&quot;Equivalent to `git checkout {args}`.&quot;&quot;&quot;</span>
-</span><span id="L-122"><a href="#L-122"><span class="linenos">122</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;checkout </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-120"><a href="#L-120"><span class="linenos">120</span></a>    <span class="k">def</span> <span class="nf">list_branches</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="L-121"><a href="#L-121"><span class="linenos">121</span></a>        <span class="sd">&quot;&quot;&quot;Print a list of branches.&quot;&quot;&quot;</span>
+</span><span id="L-122"><a href="#L-122"><span class="linenos">122</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">branch</span><span class="p">(</span><span class="s2">&quot;-vva&quot;</span><span class="p">)</span>
 </span><span id="L-123"><a href="#L-123"><span class="linenos">123</span></a>
-</span><span id="L-124"><a href="#L-124"><span class="linenos">124</span></a>    <span class="k">def</span> <span class="nf">switch_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="L-125"><a href="#L-125"><span class="linenos">125</span></a>        <span class="sd">&quot;&quot;&quot;Switch to the branch specified by `branch_name`.</span>
-</span><span id="L-126"><a href="#L-126"><span class="linenos">126</span></a>
-</span><span id="L-127"><a href="#L-127"><span class="linenos">127</span></a><span class="sd">        Equivalent to `git checkout {branch_name}`.&quot;&quot;&quot;</span>
-</span><span id="L-128"><a href="#L-128"><span class="linenos">128</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">checkout</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
-</span><span id="L-129"><a href="#L-129"><span class="linenos">129</span></a>
-</span><span id="L-130"><a href="#L-130"><span class="linenos">130</span></a>    <span class="k">def</span> <span class="nf">create_new_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="L-131"><a href="#L-131"><span class="linenos">131</span></a>        <span class="sd">&quot;&quot;&quot;Create and switch to a new branch named with `branch_name`.</span>
-</span><span id="L-132"><a href="#L-132"><span class="linenos">132</span></a>
-</span><span id="L-133"><a href="#L-133"><span class="linenos">133</span></a><span class="sd">        Equivalent to `git checkout -b {branch_name} --track`.&quot;&quot;&quot;</span>
-</span><span id="L-134"><a href="#L-134"><span class="linenos">134</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">checkout</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;-b </span><span class="si">{</span><span class="n">branch_name</span><span class="si">}</span><span class="s2"> --track&quot;</span><span class="p">)</span>
-</span><span id="L-135"><a href="#L-135"><span class="linenos">135</span></a>
-</span><span id="L-136"><a href="#L-136"><span class="linenos">136</span></a>    <span class="k">def</span> <span class="nf">delete_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">local_only</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="L-137"><a href="#L-137"><span class="linenos">137</span></a>        <span class="sd">&quot;&quot;&quot;Delete `branch_name` from repo.</span>
-</span><span id="L-138"><a href="#L-138"><span class="linenos">138</span></a>
-</span><span id="L-139"><a href="#L-139"><span class="linenos">139</span></a><span class="sd">        #### :params:</span>
-</span><span id="L-140"><a href="#L-140"><span class="linenos">140</span></a>
-</span><span id="L-141"><a href="#L-141"><span class="linenos">141</span></a><span class="sd">        `local_only`: Only delete the local copy of `branch`, otherwise also delete the remote branch on origin and remote-tracking branch.&quot;&quot;&quot;</span>
-</span><span id="L-142"><a href="#L-142"><span class="linenos">142</span></a>        <span class="n">output</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">branch</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;--delete </span><span class="si">{</span><span class="n">branch_name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-143"><a href="#L-143"><span class="linenos">143</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">local_only</span><span class="p">:</span>
-</span><span id="L-144"><a href="#L-144"><span class="linenos">144</span></a>            <span class="k">return</span> <span class="n">output</span> <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;origin --delete </span><span class="si">{</span><span class="n">branch_name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>  <span class="c1"># type:ignore</span>
-</span><span id="L-145"><a href="#L-145"><span class="linenos">145</span></a>        <span class="k">return</span> <span class="n">output</span>
-</span><span id="L-146"><a href="#L-146"><span class="linenos">146</span></a>
-</span><span id="L-147"><a href="#L-147"><span class="linenos">147</span></a>    <span class="k">def</span> <span class="nf">undo</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="L-148"><a href="#L-148"><span class="linenos">148</span></a>        <span class="sd">&quot;&quot;&quot;Undo uncommitted changes.</span>
-</span><span id="L-149"><a href="#L-149"><span class="linenos">149</span></a>
-</span><span id="L-150"><a href="#L-150"><span class="linenos">150</span></a><span class="sd">        Equivalent to `git checkout .`.&quot;&quot;&quot;</span>
-</span><span id="L-151"><a href="#L-151"><span class="linenos">151</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">checkout</span><span class="p">(</span><span class="s2">&quot;.&quot;</span><span class="p">)</span>
-</span><span id="L-152"><a href="#L-152"><span class="linenos">152</span></a>
-</span><span id="L-153"><a href="#L-153"><span class="linenos">153</span></a>    <span class="k">def</span> <span class="nf">merge</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="L-154"><a href="#L-154"><span class="linenos">154</span></a>        <span class="sd">&quot;&quot;&quot;Merge branch `branch_name` with currently active branch.&quot;&quot;&quot;</span>
-</span><span id="L-155"><a href="#L-155"><span class="linenos">155</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;merge </span><span class="si">{</span><span class="n">branch_name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-124"><a href="#L-124"><span class="linenos">124</span></a>    <span class="k">def</span> <span class="nf">checkout</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="L-125"><a href="#L-125"><span class="linenos">125</span></a>        <span class="sd">&quot;&quot;&quot;Equivalent to `git checkout {args}`.&quot;&quot;&quot;</span>
+</span><span id="L-126"><a href="#L-126"><span class="linenos">126</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;checkout </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-127"><a href="#L-127"><span class="linenos">127</span></a>
+</span><span id="L-128"><a href="#L-128"><span class="linenos">128</span></a>    <span class="k">def</span> <span class="nf">switch_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="L-129"><a href="#L-129"><span class="linenos">129</span></a>        <span class="sd">&quot;&quot;&quot;Switch to the branch specified by `branch_name`.</span>
+</span><span id="L-130"><a href="#L-130"><span class="linenos">130</span></a>
+</span><span id="L-131"><a href="#L-131"><span class="linenos">131</span></a><span class="sd">        Equivalent to `git checkout {branch_name}`.&quot;&quot;&quot;</span>
+</span><span id="L-132"><a href="#L-132"><span class="linenos">132</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">checkout</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
+</span><span id="L-133"><a href="#L-133"><span class="linenos">133</span></a>
+</span><span id="L-134"><a href="#L-134"><span class="linenos">134</span></a>    <span class="k">def</span> <span class="nf">create_new_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="L-135"><a href="#L-135"><span class="linenos">135</span></a>        <span class="sd">&quot;&quot;&quot;Create and switch to a new branch named with `branch_name`.</span>
+</span><span id="L-136"><a href="#L-136"><span class="linenos">136</span></a>
+</span><span id="L-137"><a href="#L-137"><span class="linenos">137</span></a><span class="sd">        Equivalent to `git checkout -b {branch_name} --track`.&quot;&quot;&quot;</span>
+</span><span id="L-138"><a href="#L-138"><span class="linenos">138</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">checkout</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;-b </span><span class="si">{</span><span class="n">branch_name</span><span class="si">}</span><span class="s2"> --track&quot;</span><span class="p">)</span>
+</span><span id="L-139"><a href="#L-139"><span class="linenos">139</span></a>
+</span><span id="L-140"><a href="#L-140"><span class="linenos">140</span></a>    <span class="k">def</span> <span class="nf">delete_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">local_only</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="L-141"><a href="#L-141"><span class="linenos">141</span></a>        <span class="sd">&quot;&quot;&quot;Delete `branch_name` from repo.</span>
+</span><span id="L-142"><a href="#L-142"><span class="linenos">142</span></a>
+</span><span id="L-143"><a href="#L-143"><span class="linenos">143</span></a><span class="sd">        #### :params:</span>
+</span><span id="L-144"><a href="#L-144"><span class="linenos">144</span></a>
+</span><span id="L-145"><a href="#L-145"><span class="linenos">145</span></a><span class="sd">        `local_only`: Only delete the local copy of `branch`, otherwise also delete the remote branch on origin and remote-tracking branch.&quot;&quot;&quot;</span>
+</span><span id="L-146"><a href="#L-146"><span class="linenos">146</span></a>        <span class="n">output</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">branch</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;--delete </span><span class="si">{</span><span class="n">branch_name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-147"><a href="#L-147"><span class="linenos">147</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">local_only</span><span class="p">:</span>
+</span><span id="L-148"><a href="#L-148"><span class="linenos">148</span></a>            <span class="k">return</span> <span class="n">output</span> <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;origin --delete </span><span class="si">{</span><span class="n">branch_name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>  <span class="c1"># type:ignore</span>
+</span><span id="L-149"><a href="#L-149"><span class="linenos">149</span></a>        <span class="k">return</span> <span class="n">output</span>
+</span><span id="L-150"><a href="#L-150"><span class="linenos">150</span></a>
+</span><span id="L-151"><a href="#L-151"><span class="linenos">151</span></a>    <span class="k">def</span> <span class="nf">undo</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="L-152"><a href="#L-152"><span class="linenos">152</span></a>        <span class="sd">&quot;&quot;&quot;Undo uncommitted changes.</span>
+</span><span id="L-153"><a href="#L-153"><span class="linenos">153</span></a>
+</span><span id="L-154"><a href="#L-154"><span class="linenos">154</span></a><span class="sd">        Equivalent to `git checkout .`.&quot;&quot;&quot;</span>
+</span><span id="L-155"><a href="#L-155"><span class="linenos">155</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">checkout</span><span class="p">(</span><span class="s2">&quot;.&quot;</span><span class="p">)</span>
 </span><span id="L-156"><a href="#L-156"><span class="linenos">156</span></a>
-</span><span id="L-157"><a href="#L-157"><span class="linenos">157</span></a>    <span class="c1"># ===============================Requires GitHub CLI to be installed and configured===============================</span>
-</span><span id="L-158"><a href="#L-158"><span class="linenos">158</span></a>
-</span><span id="L-159"><a href="#L-159"><span class="linenos">159</span></a>    <span class="k">def</span> <span class="nf">create_remote</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">public</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="L-160"><a href="#L-160"><span class="linenos">160</span></a>        <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be installed and configured) to create a remote GitHub repo.</span>
-</span><span id="L-161"><a href="#L-161"><span class="linenos">161</span></a>
-</span><span id="L-162"><a href="#L-162"><span class="linenos">162</span></a><span class="sd">        #### :params:</span>
-</span><span id="L-163"><a href="#L-163"><span class="linenos">163</span></a>
-</span><span id="L-164"><a href="#L-164"><span class="linenos">164</span></a><span class="sd">        `name`: The name for the repo.</span>
+</span><span id="L-157"><a href="#L-157"><span class="linenos">157</span></a>    <span class="k">def</span> <span class="nf">merge</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="L-158"><a href="#L-158"><span class="linenos">158</span></a>        <span class="sd">&quot;&quot;&quot;Merge branch `branch_name` with currently active branch.&quot;&quot;&quot;</span>
+</span><span id="L-159"><a href="#L-159"><span class="linenos">159</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;merge </span><span class="si">{</span><span class="n">branch_name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-160"><a href="#L-160"><span class="linenos">160</span></a>
+</span><span id="L-161"><a href="#L-161"><span class="linenos">161</span></a>    <span class="c1"># ===============================Requires GitHub CLI to be installed and configured===============================</span>
+</span><span id="L-162"><a href="#L-162"><span class="linenos">162</span></a>
+</span><span id="L-163"><a href="#L-163"><span class="linenos">163</span></a>    <span class="k">def</span> <span class="nf">create_remote</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">public</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="L-164"><a href="#L-164"><span class="linenos">164</span></a>        <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be installed and configured) to create a remote GitHub repo.</span>
 </span><span id="L-165"><a href="#L-165"><span class="linenos">165</span></a>
-</span><span id="L-166"><a href="#L-166"><span class="linenos">166</span></a><span class="sd">        `public`: Set to `True` to create the repo as public, otherwise it&#39;ll be created as private.&quot;&quot;&quot;</span>
-</span><span id="L-167"><a href="#L-167"><span class="linenos">167</span></a>        <span class="n">visibility</span> <span class="o">=</span> <span class="s2">&quot;--public&quot;</span> <span class="k">if</span> <span class="n">public</span> <span class="k">else</span> <span class="s2">&quot;--private&quot;</span>
-</span><span id="L-168"><a href="#L-168"><span class="linenos">168</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_run</span><span class="p">([</span><span class="s2">&quot;gh&quot;</span><span class="p">,</span> <span class="s2">&quot;repo&quot;</span><span class="p">,</span> <span class="s2">&quot;create&quot;</span><span class="p">,</span> <span class="n">name</span><span class="p">,</span> <span class="n">visibility</span><span class="p">])</span>
+</span><span id="L-166"><a href="#L-166"><span class="linenos">166</span></a><span class="sd">        #### :params:</span>
+</span><span id="L-167"><a href="#L-167"><span class="linenos">167</span></a>
+</span><span id="L-168"><a href="#L-168"><span class="linenos">168</span></a><span class="sd">        `name`: The name for the repo.</span>
 </span><span id="L-169"><a href="#L-169"><span class="linenos">169</span></a>
-</span><span id="L-170"><a href="#L-170"><span class="linenos">170</span></a>    <span class="k">def</span> <span class="nf">create_remote_from_cwd</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">public</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="L-171"><a href="#L-171"><span class="linenos">171</span></a>        <span class="sd">&quot;&quot;&quot;Use GitHub CLI (must be installed and configured) to create a remote GitHub repo from</span>
-</span><span id="L-172"><a href="#L-172"><span class="linenos">172</span></a><span class="sd">        the current working directory repo and add its url as this repo&#39;s remote origin.</span>
+</span><span id="L-170"><a href="#L-170"><span class="linenos">170</span></a><span class="sd">        `public`: Set to `True` to create the repo as public, otherwise it&#39;ll be created as private.&quot;&quot;&quot;</span>
+</span><span id="L-171"><a href="#L-171"><span class="linenos">171</span></a>        <span class="n">visibility</span> <span class="o">=</span> <span class="s2">&quot;--public&quot;</span> <span class="k">if</span> <span class="n">public</span> <span class="k">else</span> <span class="s2">&quot;--private&quot;</span>
+</span><span id="L-172"><a href="#L-172"><span class="linenos">172</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_run</span><span class="p">([</span><span class="s2">&quot;gh&quot;</span><span class="p">,</span> <span class="s2">&quot;repo&quot;</span><span class="p">,</span> <span class="s2">&quot;create&quot;</span><span class="p">,</span> <span class="n">name</span><span class="p">,</span> <span class="n">visibility</span><span class="p">])</span>
 </span><span id="L-173"><a href="#L-173"><span class="linenos">173</span></a>
-</span><span id="L-174"><a href="#L-174"><span class="linenos">174</span></a><span class="sd">        #### :params:</span>
-</span><span id="L-175"><a href="#L-175"><span class="linenos">175</span></a>
-</span><span id="L-176"><a href="#L-176"><span class="linenos">176</span></a><span class="sd">        `public`: Create the GitHub repo as a public repo, default is to create it as private.&quot;&quot;&quot;</span>
-</span><span id="L-177"><a href="#L-177"><span class="linenos">177</span></a>        <span class="n">visibility</span> <span class="o">=</span> <span class="s2">&quot;public&quot;</span> <span class="k">if</span> <span class="n">public</span> <span class="k">else</span> <span class="s2">&quot;private&quot;</span>
-</span><span id="L-178"><a href="#L-178"><span class="linenos">178</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_run</span><span class="p">(</span>
-</span><span id="L-179"><a href="#L-179"><span class="linenos">179</span></a>            <span class="p">[</span><span class="s2">&quot;gh&quot;</span><span class="p">,</span> <span class="s2">&quot;repo&quot;</span><span class="p">,</span> <span class="s2">&quot;create&quot;</span><span class="p">,</span> <span class="s2">&quot;--source&quot;</span><span class="p">,</span> <span class="s2">&quot;.&quot;</span><span class="p">,</span> <span class="sa">f</span><span class="s2">&quot;--</span><span class="si">{</span><span class="n">visibility</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">,</span> <span class="s2">&quot;--push&quot;</span><span class="p">]</span>
-</span><span id="L-180"><a href="#L-180"><span class="linenos">180</span></a>        <span class="p">)</span>
-</span><span id="L-181"><a href="#L-181"><span class="linenos">181</span></a>
-</span><span id="L-182"><a href="#L-182"><span class="linenos">182</span></a>    <span class="k">def</span> <span class="nf">_change_visibility</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">visibility</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="L-183"><a href="#L-183"><span class="linenos">183</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_run</span><span class="p">(</span>
-</span><span id="L-184"><a href="#L-184"><span class="linenos">184</span></a>            <span class="p">[</span><span class="s2">&quot;gh&quot;</span><span class="p">,</span> <span class="s2">&quot;repo&quot;</span><span class="p">,</span> <span class="s2">&quot;edit&quot;</span><span class="p">,</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">owner</span><span class="si">}</span><span class="s2">/</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">,</span> <span class="s2">&quot;--visibility&quot;</span><span class="p">,</span> <span class="n">visibility</span><span class="p">]</span>
-</span><span id="L-185"><a href="#L-185"><span class="linenos">185</span></a>        <span class="p">)</span>
-</span><span id="L-186"><a href="#L-186"><span class="linenos">186</span></a>
-</span><span id="L-187"><a href="#L-187"><span class="linenos">187</span></a>    <span class="k">def</span> <span class="nf">make_private</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="L-188"><a href="#L-188"><span class="linenos">188</span></a>        <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be installed and configured) to set the repo&#39;s visibility to private.</span>
-</span><span id="L-189"><a href="#L-189"><span class="linenos">189</span></a>
-</span><span id="L-190"><a href="#L-190"><span class="linenos">190</span></a><span class="sd">        #### :params:</span>
-</span><span id="L-191"><a href="#L-191"><span class="linenos">191</span></a>
-</span><span id="L-192"><a href="#L-192"><span class="linenos">192</span></a><span class="sd">        `owner`: The repo owner.</span>
+</span><span id="L-174"><a href="#L-174"><span class="linenos">174</span></a>    <span class="k">def</span> <span class="nf">create_remote_from_cwd</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">public</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="L-175"><a href="#L-175"><span class="linenos">175</span></a>        <span class="sd">&quot;&quot;&quot;Use GitHub CLI (must be installed and configured) to create a remote GitHub repo from</span>
+</span><span id="L-176"><a href="#L-176"><span class="linenos">176</span></a><span class="sd">        the current working directory repo and add its url as this repo&#39;s remote origin.</span>
+</span><span id="L-177"><a href="#L-177"><span class="linenos">177</span></a>
+</span><span id="L-178"><a href="#L-178"><span class="linenos">178</span></a><span class="sd">        #### :params:</span>
+</span><span id="L-179"><a href="#L-179"><span class="linenos">179</span></a>
+</span><span id="L-180"><a href="#L-180"><span class="linenos">180</span></a><span class="sd">        `public`: Create the GitHub repo as a public repo, default is to create it as private.&quot;&quot;&quot;</span>
+</span><span id="L-181"><a href="#L-181"><span class="linenos">181</span></a>        <span class="n">visibility</span> <span class="o">=</span> <span class="s2">&quot;public&quot;</span> <span class="k">if</span> <span class="n">public</span> <span class="k">else</span> <span class="s2">&quot;private&quot;</span>
+</span><span id="L-182"><a href="#L-182"><span class="linenos">182</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_run</span><span class="p">(</span>
+</span><span id="L-183"><a href="#L-183"><span class="linenos">183</span></a>            <span class="p">[</span><span class="s2">&quot;gh&quot;</span><span class="p">,</span> <span class="s2">&quot;repo&quot;</span><span class="p">,</span> <span class="s2">&quot;create&quot;</span><span class="p">,</span> <span class="s2">&quot;--source&quot;</span><span class="p">,</span> <span class="s2">&quot;.&quot;</span><span class="p">,</span> <span class="sa">f</span><span class="s2">&quot;--</span><span class="si">{</span><span class="n">visibility</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">,</span> <span class="s2">&quot;--push&quot;</span><span class="p">]</span>
+</span><span id="L-184"><a href="#L-184"><span class="linenos">184</span></a>        <span class="p">)</span>
+</span><span id="L-185"><a href="#L-185"><span class="linenos">185</span></a>
+</span><span id="L-186"><a href="#L-186"><span class="linenos">186</span></a>    <span class="k">def</span> <span class="nf">_change_visibility</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">visibility</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="L-187"><a href="#L-187"><span class="linenos">187</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_run</span><span class="p">(</span>
+</span><span id="L-188"><a href="#L-188"><span class="linenos">188</span></a>            <span class="p">[</span><span class="s2">&quot;gh&quot;</span><span class="p">,</span> <span class="s2">&quot;repo&quot;</span><span class="p">,</span> <span class="s2">&quot;edit&quot;</span><span class="p">,</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">owner</span><span class="si">}</span><span class="s2">/</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">,</span> <span class="s2">&quot;--visibility&quot;</span><span class="p">,</span> <span class="n">visibility</span><span class="p">]</span>
+</span><span id="L-189"><a href="#L-189"><span class="linenos">189</span></a>        <span class="p">)</span>
+</span><span id="L-190"><a href="#L-190"><span class="linenos">190</span></a>
+</span><span id="L-191"><a href="#L-191"><span class="linenos">191</span></a>    <span class="k">def</span> <span class="nf">make_private</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="L-192"><a href="#L-192"><span class="linenos">192</span></a>        <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be installed and configured) to set the repo&#39;s visibility to private.</span>
 </span><span id="L-193"><a href="#L-193"><span class="linenos">193</span></a>
-</span><span id="L-194"><a href="#L-194"><span class="linenos">194</span></a><span class="sd">        `name`: The name of the repo to edit.&quot;&quot;&quot;</span>
-</span><span id="L-195"><a href="#L-195"><span class="linenos">195</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_change_visibility</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">name</span><span class="p">,</span> <span class="s2">&quot;private&quot;</span><span class="p">)</span>
-</span><span id="L-196"><a href="#L-196"><span class="linenos">196</span></a>
-</span><span id="L-197"><a href="#L-197"><span class="linenos">197</span></a>    <span class="k">def</span> <span class="nf">make_public</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="L-198"><a href="#L-198"><span class="linenos">198</span></a>        <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be installed and configured) to set the repo&#39;s visibility to public.</span>
-</span><span id="L-199"><a href="#L-199"><span class="linenos">199</span></a>
-</span><span id="L-200"><a href="#L-200"><span class="linenos">200</span></a><span class="sd">        #### :params:</span>
-</span><span id="L-201"><a href="#L-201"><span class="linenos">201</span></a>
-</span><span id="L-202"><a href="#L-202"><span class="linenos">202</span></a><span class="sd">        `owner`: The repo owner.</span>
+</span><span id="L-194"><a href="#L-194"><span class="linenos">194</span></a><span class="sd">        #### :params:</span>
+</span><span id="L-195"><a href="#L-195"><span class="linenos">195</span></a>
+</span><span id="L-196"><a href="#L-196"><span class="linenos">196</span></a><span class="sd">        `owner`: The repo owner.</span>
+</span><span id="L-197"><a href="#L-197"><span class="linenos">197</span></a>
+</span><span id="L-198"><a href="#L-198"><span class="linenos">198</span></a><span class="sd">        `name`: The name of the repo to edit.&quot;&quot;&quot;</span>
+</span><span id="L-199"><a href="#L-199"><span class="linenos">199</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_change_visibility</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">name</span><span class="p">,</span> <span class="s2">&quot;private&quot;</span><span class="p">)</span>
+</span><span id="L-200"><a href="#L-200"><span class="linenos">200</span></a>
+</span><span id="L-201"><a href="#L-201"><span class="linenos">201</span></a>    <span class="k">def</span> <span class="nf">make_public</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="L-202"><a href="#L-202"><span class="linenos">202</span></a>        <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be installed and configured) to set the repo&#39;s visibility to public.</span>
 </span><span id="L-203"><a href="#L-203"><span class="linenos">203</span></a>
-</span><span id="L-204"><a href="#L-204"><span class="linenos">204</span></a><span class="sd">        `name`: The name of the repo to edit.&quot;&quot;&quot;</span>
-</span><span id="L-205"><a href="#L-205"><span class="linenos">205</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_change_visibility</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">name</span><span class="p">,</span> <span class="s2">&quot;public&quot;</span><span class="p">)</span>
-</span><span id="L-206"><a href="#L-206"><span class="linenos">206</span></a>
-</span><span id="L-207"><a href="#L-207"><span class="linenos">207</span></a>    <span class="k">def</span> <span class="nf">delete_remote</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="L-208"><a href="#L-208"><span class="linenos">208</span></a>        <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be isntalled and configured) to delete the remote for this repo.</span>
-</span><span id="L-209"><a href="#L-209"><span class="linenos">209</span></a>
-</span><span id="L-210"><a href="#L-210"><span class="linenos">210</span></a><span class="sd">        #### :params:</span>
-</span><span id="L-211"><a href="#L-211"><span class="linenos">211</span></a>
-</span><span id="L-212"><a href="#L-212"><span class="linenos">212</span></a><span class="sd">        `owner`: The repo owner.</span>
+</span><span id="L-204"><a href="#L-204"><span class="linenos">204</span></a><span class="sd">        #### :params:</span>
+</span><span id="L-205"><a href="#L-205"><span class="linenos">205</span></a>
+</span><span id="L-206"><a href="#L-206"><span class="linenos">206</span></a><span class="sd">        `owner`: The repo owner.</span>
+</span><span id="L-207"><a href="#L-207"><span class="linenos">207</span></a>
+</span><span id="L-208"><a href="#L-208"><span class="linenos">208</span></a><span class="sd">        `name`: The name of the repo to edit.&quot;&quot;&quot;</span>
+</span><span id="L-209"><a href="#L-209"><span class="linenos">209</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_change_visibility</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">name</span><span class="p">,</span> <span class="s2">&quot;public&quot;</span><span class="p">)</span>
+</span><span id="L-210"><a href="#L-210"><span class="linenos">210</span></a>
+</span><span id="L-211"><a href="#L-211"><span class="linenos">211</span></a>    <span class="k">def</span> <span class="nf">delete_remote</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="L-212"><a href="#L-212"><span class="linenos">212</span></a>        <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be isntalled and configured) to delete the remote for this repo.</span>
 </span><span id="L-213"><a href="#L-213"><span class="linenos">213</span></a>
-</span><span id="L-214"><a href="#L-214"><span class="linenos">214</span></a><span class="sd">        `name`: The name of the remote repo to delete.&quot;&quot;&quot;</span>
-</span><span id="L-215"><a href="#L-215"><span class="linenos">215</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_run</span><span class="p">([</span><span class="s2">&quot;gh&quot;</span><span class="p">,</span> <span class="s2">&quot;repo&quot;</span><span class="p">,</span> <span class="s2">&quot;delete&quot;</span><span class="p">,</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">owner</span><span class="si">}</span><span class="s2">/</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">,</span> <span class="s2">&quot;--yes&quot;</span><span class="p">])</span>
+</span><span id="L-214"><a href="#L-214"><span class="linenos">214</span></a><span class="sd">        #### :params:</span>
+</span><span id="L-215"><a href="#L-215"><span class="linenos">215</span></a>
+</span><span id="L-216"><a href="#L-216"><span class="linenos">216</span></a><span class="sd">        `owner`: The repo owner.</span>
+</span><span id="L-217"><a href="#L-217"><span class="linenos">217</span></a>
+</span><span id="L-218"><a href="#L-218"><span class="linenos">218</span></a><span class="sd">        `name`: The name of the remote repo to delete.&quot;&quot;&quot;</span>
+</span><span id="L-219"><a href="#L-219"><span class="linenos">219</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_run</span><span class="p">([</span><span class="s2">&quot;gh&quot;</span><span class="p">,</span> <span class="s2">&quot;repo&quot;</span><span class="p">,</span> <span class="s2">&quot;delete&quot;</span><span class="p">,</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">owner</span><span class="si">}</span><span class="s2">/</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">,</span> <span class="s2">&quot;--yes&quot;</span><span class="p">])</span>
 </span></pre></div>
 
 
             </section>
                 <section id="Git">
                             <input id="Git-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr class">
@@ -450,148 +454,152 @@
 </span><span id="Git-76"><a href="#Git-76"><span class="linenos"> 76</span></a>
 </span><span id="Git-77"><a href="#Git-77"><span class="linenos"> 77</span></a><span class="sd">        Equivalent to:</span>
 </span><span id="Git-78"><a href="#Git-78"><span class="linenos"> 78</span></a><span class="sd">        &gt;&gt;&gt; git add {files}</span>
 </span><span id="Git-79"><a href="#Git-79"><span class="linenos"> 79</span></a><span class="sd">        &gt;&gt;&gt; git commit --amend --no-edit</span>
 </span><span id="Git-80"><a href="#Git-80"><span class="linenos"> 80</span></a><span class="sd">        &quot;&quot;&quot;</span>
 </span><span id="Git-81"><a href="#Git-81"><span class="linenos"> 81</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">add</span><span class="p">(</span><span class="n">files</span><span class="p">)</span> <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">commit</span><span class="p">(</span><span class="s2">&quot;--amend --no-edit&quot;</span><span class="p">)</span>  <span class="c1"># type: ignore</span>
 </span><span id="Git-82"><a href="#Git-82"><span class="linenos"> 82</span></a>
-</span><span id="Git-83"><a href="#Git-83"><span class="linenos"> 83</span></a>    <span class="k">def</span> <span class="nf">tag</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">id_</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git-84"><a href="#Git-84"><span class="linenos"> 84</span></a>        <span class="sd">&quot;&quot;&quot;Tag the current commit with `id_`.</span>
+</span><span id="Git-83"><a href="#Git-83"><span class="linenos"> 83</span></a>    <span class="k">def</span> <span class="nf">tag</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git-84"><a href="#Git-84"><span class="linenos"> 84</span></a>        <span class="sd">&quot;&quot;&quot;Execute the `tag` command with `args`.</span>
 </span><span id="Git-85"><a href="#Git-85"><span class="linenos"> 85</span></a>
-</span><span id="Git-86"><a href="#Git-86"><span class="linenos"> 86</span></a><span class="sd">        Equivalent to `git tag {id_}`.&quot;&quot;&quot;</span>
-</span><span id="Git-87"><a href="#Git-87"><span class="linenos"> 87</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;tag </span><span class="si">{</span><span class="n">id_</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="Git-88"><a href="#Git-88"><span class="linenos"> 88</span></a>
-</span><span id="Git-89"><a href="#Git-89"><span class="linenos"> 89</span></a>    <span class="c1"># ==========================================Push/Pull==========================================</span>
-</span><span id="Git-90"><a href="#Git-90"><span class="linenos"> 90</span></a>    <span class="k">def</span> <span class="nf">add_remote_url</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">url</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;origin&quot;</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git-91"><a href="#Git-91"><span class="linenos"> 91</span></a>        <span class="sd">&quot;&quot;&quot;Add remote url to repo.&quot;&quot;&quot;</span>
-</span><span id="Git-92"><a href="#Git-92"><span class="linenos"> 92</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;remote add </span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">url</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="Git-93"><a href="#Git-93"><span class="linenos"> 93</span></a>
-</span><span id="Git-94"><a href="#Git-94"><span class="linenos"> 94</span></a>    <span class="k">def</span> <span class="nf">push</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git-95"><a href="#Git-95"><span class="linenos"> 95</span></a>        <span class="sd">&quot;&quot;&quot;Equivalent to `git push {args}`.&quot;&quot;&quot;</span>
-</span><span id="Git-96"><a href="#Git-96"><span class="linenos"> 96</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;push </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="Git-86"><a href="#Git-86"><span class="linenos"> 86</span></a><span class="sd">        e.g.</span>
+</span><span id="Git-87"><a href="#Git-87"><span class="linenos"> 87</span></a>
+</span><span id="Git-88"><a href="#Git-88"><span class="linenos"> 88</span></a><span class="sd">        `self.tag(&quot;--sort=-committerdate&quot;)`</span>
+</span><span id="Git-89"><a href="#Git-89"><span class="linenos"> 89</span></a>
+</span><span id="Git-90"><a href="#Git-90"><span class="linenos"> 90</span></a><span class="sd">        will list all the tags for this repository in descending commit date.&quot;&quot;&quot;</span>
+</span><span id="Git-91"><a href="#Git-91"><span class="linenos"> 91</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;tag </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="Git-92"><a href="#Git-92"><span class="linenos"> 92</span></a>
+</span><span id="Git-93"><a href="#Git-93"><span class="linenos"> 93</span></a>    <span class="c1"># ==========================================Push/Pull==========================================</span>
+</span><span id="Git-94"><a href="#Git-94"><span class="linenos"> 94</span></a>    <span class="k">def</span> <span class="nf">add_remote_url</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">url</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;origin&quot;</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git-95"><a href="#Git-95"><span class="linenos"> 95</span></a>        <span class="sd">&quot;&quot;&quot;Add remote url to repo.&quot;&quot;&quot;</span>
+</span><span id="Git-96"><a href="#Git-96"><span class="linenos"> 96</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;remote add </span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">url</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span><span id="Git-97"><a href="#Git-97"><span class="linenos"> 97</span></a>
-</span><span id="Git-98"><a href="#Git-98"><span class="linenos"> 98</span></a>    <span class="k">def</span> <span class="nf">pull</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git-99"><a href="#Git-99"><span class="linenos"> 99</span></a>        <span class="sd">&quot;&quot;&quot;Equivalent to `git pull {args}`.&quot;&quot;&quot;</span>
-</span><span id="Git-100"><a href="#Git-100"><span class="linenos">100</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;pull </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="Git-98"><a href="#Git-98"><span class="linenos"> 98</span></a>    <span class="k">def</span> <span class="nf">push</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git-99"><a href="#Git-99"><span class="linenos"> 99</span></a>        <span class="sd">&quot;&quot;&quot;Equivalent to `git push {args}`.&quot;&quot;&quot;</span>
+</span><span id="Git-100"><a href="#Git-100"><span class="linenos">100</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;push </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span><span id="Git-101"><a href="#Git-101"><span class="linenos">101</span></a>
-</span><span id="Git-102"><a href="#Git-102"><span class="linenos">102</span></a>    <span class="k">def</span> <span class="nf">push_new_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git-103"><a href="#Git-103"><span class="linenos">103</span></a>        <span class="sd">&quot;&quot;&quot;Push a new branch to origin with tracking.</span>
-</span><span id="Git-104"><a href="#Git-104"><span class="linenos">104</span></a>
-</span><span id="Git-105"><a href="#Git-105"><span class="linenos">105</span></a><span class="sd">        Equivalent to `git push -u origin {branch}`.&quot;&quot;&quot;</span>
-</span><span id="Git-106"><a href="#Git-106"><span class="linenos">106</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;-u origin </span><span class="si">{</span><span class="n">branch</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="Git-107"><a href="#Git-107"><span class="linenos">107</span></a>
-</span><span id="Git-108"><a href="#Git-108"><span class="linenos">108</span></a>    <span class="k">def</span> <span class="nf">pull_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git-109"><a href="#Git-109"><span class="linenos">109</span></a>        <span class="sd">&quot;&quot;&quot;Pull `branch` from origin.&quot;&quot;&quot;</span>
-</span><span id="Git-110"><a href="#Git-110"><span class="linenos">110</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">pull</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;origin </span><span class="si">{</span><span class="n">branch</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="Git-102"><a href="#Git-102"><span class="linenos">102</span></a>    <span class="k">def</span> <span class="nf">pull</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git-103"><a href="#Git-103"><span class="linenos">103</span></a>        <span class="sd">&quot;&quot;&quot;Equivalent to `git pull {args}`.&quot;&quot;&quot;</span>
+</span><span id="Git-104"><a href="#Git-104"><span class="linenos">104</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;pull </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="Git-105"><a href="#Git-105"><span class="linenos">105</span></a>
+</span><span id="Git-106"><a href="#Git-106"><span class="linenos">106</span></a>    <span class="k">def</span> <span class="nf">push_new_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git-107"><a href="#Git-107"><span class="linenos">107</span></a>        <span class="sd">&quot;&quot;&quot;Push a new branch to origin with tracking.</span>
+</span><span id="Git-108"><a href="#Git-108"><span class="linenos">108</span></a>
+</span><span id="Git-109"><a href="#Git-109"><span class="linenos">109</span></a><span class="sd">        Equivalent to `git push -u origin {branch}`.&quot;&quot;&quot;</span>
+</span><span id="Git-110"><a href="#Git-110"><span class="linenos">110</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;-u origin </span><span class="si">{</span><span class="n">branch</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span><span id="Git-111"><a href="#Git-111"><span class="linenos">111</span></a>
-</span><span id="Git-112"><a href="#Git-112"><span class="linenos">112</span></a>    <span class="c1"># ============================================Checkout/Branches============================================</span>
-</span><span id="Git-113"><a href="#Git-113"><span class="linenos">113</span></a>    <span class="k">def</span> <span class="nf">branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git-114"><a href="#Git-114"><span class="linenos">114</span></a>        <span class="sd">&quot;&quot;&quot;Equivalent to `git branch {args}`.&quot;&quot;&quot;</span>
-</span><span id="Git-115"><a href="#Git-115"><span class="linenos">115</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;branch </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="Git-116"><a href="#Git-116"><span class="linenos">116</span></a>
-</span><span id="Git-117"><a href="#Git-117"><span class="linenos">117</span></a>    <span class="k">def</span> <span class="nf">list_branches</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git-118"><a href="#Git-118"><span class="linenos">118</span></a>        <span class="sd">&quot;&quot;&quot;Print a list of branches.&quot;&quot;&quot;</span>
-</span><span id="Git-119"><a href="#Git-119"><span class="linenos">119</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">branch</span><span class="p">(</span><span class="s2">&quot;-vva&quot;</span><span class="p">)</span>
+</span><span id="Git-112"><a href="#Git-112"><span class="linenos">112</span></a>    <span class="k">def</span> <span class="nf">pull_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git-113"><a href="#Git-113"><span class="linenos">113</span></a>        <span class="sd">&quot;&quot;&quot;Pull `branch` from origin.&quot;&quot;&quot;</span>
+</span><span id="Git-114"><a href="#Git-114"><span class="linenos">114</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">pull</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;origin </span><span class="si">{</span><span class="n">branch</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="Git-115"><a href="#Git-115"><span class="linenos">115</span></a>
+</span><span id="Git-116"><a href="#Git-116"><span class="linenos">116</span></a>    <span class="c1"># ============================================Checkout/Branches============================================</span>
+</span><span id="Git-117"><a href="#Git-117"><span class="linenos">117</span></a>    <span class="k">def</span> <span class="nf">branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git-118"><a href="#Git-118"><span class="linenos">118</span></a>        <span class="sd">&quot;&quot;&quot;Equivalent to `git branch {args}`.&quot;&quot;&quot;</span>
+</span><span id="Git-119"><a href="#Git-119"><span class="linenos">119</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;branch </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span><span id="Git-120"><a href="#Git-120"><span class="linenos">120</span></a>
-</span><span id="Git-121"><a href="#Git-121"><span class="linenos">121</span></a>    <span class="k">def</span> <span class="nf">checkout</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git-122"><a href="#Git-122"><span class="linenos">122</span></a>        <span class="sd">&quot;&quot;&quot;Equivalent to `git checkout {args}`.&quot;&quot;&quot;</span>
-</span><span id="Git-123"><a href="#Git-123"><span class="linenos">123</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;checkout </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="Git-121"><a href="#Git-121"><span class="linenos">121</span></a>    <span class="k">def</span> <span class="nf">list_branches</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git-122"><a href="#Git-122"><span class="linenos">122</span></a>        <span class="sd">&quot;&quot;&quot;Print a list of branches.&quot;&quot;&quot;</span>
+</span><span id="Git-123"><a href="#Git-123"><span class="linenos">123</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">branch</span><span class="p">(</span><span class="s2">&quot;-vva&quot;</span><span class="p">)</span>
 </span><span id="Git-124"><a href="#Git-124"><span class="linenos">124</span></a>
-</span><span id="Git-125"><a href="#Git-125"><span class="linenos">125</span></a>    <span class="k">def</span> <span class="nf">switch_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git-126"><a href="#Git-126"><span class="linenos">126</span></a>        <span class="sd">&quot;&quot;&quot;Switch to the branch specified by `branch_name`.</span>
-</span><span id="Git-127"><a href="#Git-127"><span class="linenos">127</span></a>
-</span><span id="Git-128"><a href="#Git-128"><span class="linenos">128</span></a><span class="sd">        Equivalent to `git checkout {branch_name}`.&quot;&quot;&quot;</span>
-</span><span id="Git-129"><a href="#Git-129"><span class="linenos">129</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">checkout</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
-</span><span id="Git-130"><a href="#Git-130"><span class="linenos">130</span></a>
-</span><span id="Git-131"><a href="#Git-131"><span class="linenos">131</span></a>    <span class="k">def</span> <span class="nf">create_new_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git-132"><a href="#Git-132"><span class="linenos">132</span></a>        <span class="sd">&quot;&quot;&quot;Create and switch to a new branch named with `branch_name`.</span>
-</span><span id="Git-133"><a href="#Git-133"><span class="linenos">133</span></a>
-</span><span id="Git-134"><a href="#Git-134"><span class="linenos">134</span></a><span class="sd">        Equivalent to `git checkout -b {branch_name} --track`.&quot;&quot;&quot;</span>
-</span><span id="Git-135"><a href="#Git-135"><span class="linenos">135</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">checkout</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;-b </span><span class="si">{</span><span class="n">branch_name</span><span class="si">}</span><span class="s2"> --track&quot;</span><span class="p">)</span>
-</span><span id="Git-136"><a href="#Git-136"><span class="linenos">136</span></a>
-</span><span id="Git-137"><a href="#Git-137"><span class="linenos">137</span></a>    <span class="k">def</span> <span class="nf">delete_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">local_only</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git-138"><a href="#Git-138"><span class="linenos">138</span></a>        <span class="sd">&quot;&quot;&quot;Delete `branch_name` from repo.</span>
-</span><span id="Git-139"><a href="#Git-139"><span class="linenos">139</span></a>
-</span><span id="Git-140"><a href="#Git-140"><span class="linenos">140</span></a><span class="sd">        #### :params:</span>
-</span><span id="Git-141"><a href="#Git-141"><span class="linenos">141</span></a>
-</span><span id="Git-142"><a href="#Git-142"><span class="linenos">142</span></a><span class="sd">        `local_only`: Only delete the local copy of `branch`, otherwise also delete the remote branch on origin and remote-tracking branch.&quot;&quot;&quot;</span>
-</span><span id="Git-143"><a href="#Git-143"><span class="linenos">143</span></a>        <span class="n">output</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">branch</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;--delete </span><span class="si">{</span><span class="n">branch_name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="Git-144"><a href="#Git-144"><span class="linenos">144</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">local_only</span><span class="p">:</span>
-</span><span id="Git-145"><a href="#Git-145"><span class="linenos">145</span></a>            <span class="k">return</span> <span class="n">output</span> <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;origin --delete </span><span class="si">{</span><span class="n">branch_name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>  <span class="c1"># type:ignore</span>
-</span><span id="Git-146"><a href="#Git-146"><span class="linenos">146</span></a>        <span class="k">return</span> <span class="n">output</span>
-</span><span id="Git-147"><a href="#Git-147"><span class="linenos">147</span></a>
-</span><span id="Git-148"><a href="#Git-148"><span class="linenos">148</span></a>    <span class="k">def</span> <span class="nf">undo</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git-149"><a href="#Git-149"><span class="linenos">149</span></a>        <span class="sd">&quot;&quot;&quot;Undo uncommitted changes.</span>
-</span><span id="Git-150"><a href="#Git-150"><span class="linenos">150</span></a>
-</span><span id="Git-151"><a href="#Git-151"><span class="linenos">151</span></a><span class="sd">        Equivalent to `git checkout .`.&quot;&quot;&quot;</span>
-</span><span id="Git-152"><a href="#Git-152"><span class="linenos">152</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">checkout</span><span class="p">(</span><span class="s2">&quot;.&quot;</span><span class="p">)</span>
-</span><span id="Git-153"><a href="#Git-153"><span class="linenos">153</span></a>
-</span><span id="Git-154"><a href="#Git-154"><span class="linenos">154</span></a>    <span class="k">def</span> <span class="nf">merge</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git-155"><a href="#Git-155"><span class="linenos">155</span></a>        <span class="sd">&quot;&quot;&quot;Merge branch `branch_name` with currently active branch.&quot;&quot;&quot;</span>
-</span><span id="Git-156"><a href="#Git-156"><span class="linenos">156</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;merge </span><span class="si">{</span><span class="n">branch_name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="Git-125"><a href="#Git-125"><span class="linenos">125</span></a>    <span class="k">def</span> <span class="nf">checkout</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git-126"><a href="#Git-126"><span class="linenos">126</span></a>        <span class="sd">&quot;&quot;&quot;Equivalent to `git checkout {args}`.&quot;&quot;&quot;</span>
+</span><span id="Git-127"><a href="#Git-127"><span class="linenos">127</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;checkout </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="Git-128"><a href="#Git-128"><span class="linenos">128</span></a>
+</span><span id="Git-129"><a href="#Git-129"><span class="linenos">129</span></a>    <span class="k">def</span> <span class="nf">switch_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git-130"><a href="#Git-130"><span class="linenos">130</span></a>        <span class="sd">&quot;&quot;&quot;Switch to the branch specified by `branch_name`.</span>
+</span><span id="Git-131"><a href="#Git-131"><span class="linenos">131</span></a>
+</span><span id="Git-132"><a href="#Git-132"><span class="linenos">132</span></a><span class="sd">        Equivalent to `git checkout {branch_name}`.&quot;&quot;&quot;</span>
+</span><span id="Git-133"><a href="#Git-133"><span class="linenos">133</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">checkout</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
+</span><span id="Git-134"><a href="#Git-134"><span class="linenos">134</span></a>
+</span><span id="Git-135"><a href="#Git-135"><span class="linenos">135</span></a>    <span class="k">def</span> <span class="nf">create_new_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git-136"><a href="#Git-136"><span class="linenos">136</span></a>        <span class="sd">&quot;&quot;&quot;Create and switch to a new branch named with `branch_name`.</span>
+</span><span id="Git-137"><a href="#Git-137"><span class="linenos">137</span></a>
+</span><span id="Git-138"><a href="#Git-138"><span class="linenos">138</span></a><span class="sd">        Equivalent to `git checkout -b {branch_name} --track`.&quot;&quot;&quot;</span>
+</span><span id="Git-139"><a href="#Git-139"><span class="linenos">139</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">checkout</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;-b </span><span class="si">{</span><span class="n">branch_name</span><span class="si">}</span><span class="s2"> --track&quot;</span><span class="p">)</span>
+</span><span id="Git-140"><a href="#Git-140"><span class="linenos">140</span></a>
+</span><span id="Git-141"><a href="#Git-141"><span class="linenos">141</span></a>    <span class="k">def</span> <span class="nf">delete_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">local_only</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git-142"><a href="#Git-142"><span class="linenos">142</span></a>        <span class="sd">&quot;&quot;&quot;Delete `branch_name` from repo.</span>
+</span><span id="Git-143"><a href="#Git-143"><span class="linenos">143</span></a>
+</span><span id="Git-144"><a href="#Git-144"><span class="linenos">144</span></a><span class="sd">        #### :params:</span>
+</span><span id="Git-145"><a href="#Git-145"><span class="linenos">145</span></a>
+</span><span id="Git-146"><a href="#Git-146"><span class="linenos">146</span></a><span class="sd">        `local_only`: Only delete the local copy of `branch`, otherwise also delete the remote branch on origin and remote-tracking branch.&quot;&quot;&quot;</span>
+</span><span id="Git-147"><a href="#Git-147"><span class="linenos">147</span></a>        <span class="n">output</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">branch</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;--delete </span><span class="si">{</span><span class="n">branch_name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="Git-148"><a href="#Git-148"><span class="linenos">148</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">local_only</span><span class="p">:</span>
+</span><span id="Git-149"><a href="#Git-149"><span class="linenos">149</span></a>            <span class="k">return</span> <span class="n">output</span> <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;origin --delete </span><span class="si">{</span><span class="n">branch_name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>  <span class="c1"># type:ignore</span>
+</span><span id="Git-150"><a href="#Git-150"><span class="linenos">150</span></a>        <span class="k">return</span> <span class="n">output</span>
+</span><span id="Git-151"><a href="#Git-151"><span class="linenos">151</span></a>
+</span><span id="Git-152"><a href="#Git-152"><span class="linenos">152</span></a>    <span class="k">def</span> <span class="nf">undo</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git-153"><a href="#Git-153"><span class="linenos">153</span></a>        <span class="sd">&quot;&quot;&quot;Undo uncommitted changes.</span>
+</span><span id="Git-154"><a href="#Git-154"><span class="linenos">154</span></a>
+</span><span id="Git-155"><a href="#Git-155"><span class="linenos">155</span></a><span class="sd">        Equivalent to `git checkout .`.&quot;&quot;&quot;</span>
+</span><span id="Git-156"><a href="#Git-156"><span class="linenos">156</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">checkout</span><span class="p">(</span><span class="s2">&quot;.&quot;</span><span class="p">)</span>
 </span><span id="Git-157"><a href="#Git-157"><span class="linenos">157</span></a>
-</span><span id="Git-158"><a href="#Git-158"><span class="linenos">158</span></a>    <span class="c1"># ===============================Requires GitHub CLI to be installed and configured===============================</span>
-</span><span id="Git-159"><a href="#Git-159"><span class="linenos">159</span></a>
-</span><span id="Git-160"><a href="#Git-160"><span class="linenos">160</span></a>    <span class="k">def</span> <span class="nf">create_remote</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">public</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git-161"><a href="#Git-161"><span class="linenos">161</span></a>        <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be installed and configured) to create a remote GitHub repo.</span>
-</span><span id="Git-162"><a href="#Git-162"><span class="linenos">162</span></a>
-</span><span id="Git-163"><a href="#Git-163"><span class="linenos">163</span></a><span class="sd">        #### :params:</span>
-</span><span id="Git-164"><a href="#Git-164"><span class="linenos">164</span></a>
-</span><span id="Git-165"><a href="#Git-165"><span class="linenos">165</span></a><span class="sd">        `name`: The name for the repo.</span>
+</span><span id="Git-158"><a href="#Git-158"><span class="linenos">158</span></a>    <span class="k">def</span> <span class="nf">merge</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git-159"><a href="#Git-159"><span class="linenos">159</span></a>        <span class="sd">&quot;&quot;&quot;Merge branch `branch_name` with currently active branch.&quot;&quot;&quot;</span>
+</span><span id="Git-160"><a href="#Git-160"><span class="linenos">160</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;merge </span><span class="si">{</span><span class="n">branch_name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="Git-161"><a href="#Git-161"><span class="linenos">161</span></a>
+</span><span id="Git-162"><a href="#Git-162"><span class="linenos">162</span></a>    <span class="c1"># ===============================Requires GitHub CLI to be installed and configured===============================</span>
+</span><span id="Git-163"><a href="#Git-163"><span class="linenos">163</span></a>
+</span><span id="Git-164"><a href="#Git-164"><span class="linenos">164</span></a>    <span class="k">def</span> <span class="nf">create_remote</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">public</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git-165"><a href="#Git-165"><span class="linenos">165</span></a>        <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be installed and configured) to create a remote GitHub repo.</span>
 </span><span id="Git-166"><a href="#Git-166"><span class="linenos">166</span></a>
-</span><span id="Git-167"><a href="#Git-167"><span class="linenos">167</span></a><span class="sd">        `public`: Set to `True` to create the repo as public, otherwise it&#39;ll be created as private.&quot;&quot;&quot;</span>
-</span><span id="Git-168"><a href="#Git-168"><span class="linenos">168</span></a>        <span class="n">visibility</span> <span class="o">=</span> <span class="s2">&quot;--public&quot;</span> <span class="k">if</span> <span class="n">public</span> <span class="k">else</span> <span class="s2">&quot;--private&quot;</span>
-</span><span id="Git-169"><a href="#Git-169"><span class="linenos">169</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_run</span><span class="p">([</span><span class="s2">&quot;gh&quot;</span><span class="p">,</span> <span class="s2">&quot;repo&quot;</span><span class="p">,</span> <span class="s2">&quot;create&quot;</span><span class="p">,</span> <span class="n">name</span><span class="p">,</span> <span class="n">visibility</span><span class="p">])</span>
+</span><span id="Git-167"><a href="#Git-167"><span class="linenos">167</span></a><span class="sd">        #### :params:</span>
+</span><span id="Git-168"><a href="#Git-168"><span class="linenos">168</span></a>
+</span><span id="Git-169"><a href="#Git-169"><span class="linenos">169</span></a><span class="sd">        `name`: The name for the repo.</span>
 </span><span id="Git-170"><a href="#Git-170"><span class="linenos">170</span></a>
-</span><span id="Git-171"><a href="#Git-171"><span class="linenos">171</span></a>    <span class="k">def</span> <span class="nf">create_remote_from_cwd</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">public</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git-172"><a href="#Git-172"><span class="linenos">172</span></a>        <span class="sd">&quot;&quot;&quot;Use GitHub CLI (must be installed and configured) to create a remote GitHub repo from</span>
-</span><span id="Git-173"><a href="#Git-173"><span class="linenos">173</span></a><span class="sd">        the current working directory repo and add its url as this repo&#39;s remote origin.</span>
+</span><span id="Git-171"><a href="#Git-171"><span class="linenos">171</span></a><span class="sd">        `public`: Set to `True` to create the repo as public, otherwise it&#39;ll be created as private.&quot;&quot;&quot;</span>
+</span><span id="Git-172"><a href="#Git-172"><span class="linenos">172</span></a>        <span class="n">visibility</span> <span class="o">=</span> <span class="s2">&quot;--public&quot;</span> <span class="k">if</span> <span class="n">public</span> <span class="k">else</span> <span class="s2">&quot;--private&quot;</span>
+</span><span id="Git-173"><a href="#Git-173"><span class="linenos">173</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_run</span><span class="p">([</span><span class="s2">&quot;gh&quot;</span><span class="p">,</span> <span class="s2">&quot;repo&quot;</span><span class="p">,</span> <span class="s2">&quot;create&quot;</span><span class="p">,</span> <span class="n">name</span><span class="p">,</span> <span class="n">visibility</span><span class="p">])</span>
 </span><span id="Git-174"><a href="#Git-174"><span class="linenos">174</span></a>
-</span><span id="Git-175"><a href="#Git-175"><span class="linenos">175</span></a><span class="sd">        #### :params:</span>
-</span><span id="Git-176"><a href="#Git-176"><span class="linenos">176</span></a>
-</span><span id="Git-177"><a href="#Git-177"><span class="linenos">177</span></a><span class="sd">        `public`: Create the GitHub repo as a public repo, default is to create it as private.&quot;&quot;&quot;</span>
-</span><span id="Git-178"><a href="#Git-178"><span class="linenos">178</span></a>        <span class="n">visibility</span> <span class="o">=</span> <span class="s2">&quot;public&quot;</span> <span class="k">if</span> <span class="n">public</span> <span class="k">else</span> <span class="s2">&quot;private&quot;</span>
-</span><span id="Git-179"><a href="#Git-179"><span class="linenos">179</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_run</span><span class="p">(</span>
-</span><span id="Git-180"><a href="#Git-180"><span class="linenos">180</span></a>            <span class="p">[</span><span class="s2">&quot;gh&quot;</span><span class="p">,</span> <span class="s2">&quot;repo&quot;</span><span class="p">,</span> <span class="s2">&quot;create&quot;</span><span class="p">,</span> <span class="s2">&quot;--source&quot;</span><span class="p">,</span> <span class="s2">&quot;.&quot;</span><span class="p">,</span> <span class="sa">f</span><span class="s2">&quot;--</span><span class="si">{</span><span class="n">visibility</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">,</span> <span class="s2">&quot;--push&quot;</span><span class="p">]</span>
-</span><span id="Git-181"><a href="#Git-181"><span class="linenos">181</span></a>        <span class="p">)</span>
-</span><span id="Git-182"><a href="#Git-182"><span class="linenos">182</span></a>
-</span><span id="Git-183"><a href="#Git-183"><span class="linenos">183</span></a>    <span class="k">def</span> <span class="nf">_change_visibility</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">visibility</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git-184"><a href="#Git-184"><span class="linenos">184</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_run</span><span class="p">(</span>
-</span><span id="Git-185"><a href="#Git-185"><span class="linenos">185</span></a>            <span class="p">[</span><span class="s2">&quot;gh&quot;</span><span class="p">,</span> <span class="s2">&quot;repo&quot;</span><span class="p">,</span> <span class="s2">&quot;edit&quot;</span><span class="p">,</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">owner</span><span class="si">}</span><span class="s2">/</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">,</span> <span class="s2">&quot;--visibility&quot;</span><span class="p">,</span> <span class="n">visibility</span><span class="p">]</span>
-</span><span id="Git-186"><a href="#Git-186"><span class="linenos">186</span></a>        <span class="p">)</span>
-</span><span id="Git-187"><a href="#Git-187"><span class="linenos">187</span></a>
-</span><span id="Git-188"><a href="#Git-188"><span class="linenos">188</span></a>    <span class="k">def</span> <span class="nf">make_private</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git-189"><a href="#Git-189"><span class="linenos">189</span></a>        <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be installed and configured) to set the repo&#39;s visibility to private.</span>
-</span><span id="Git-190"><a href="#Git-190"><span class="linenos">190</span></a>
-</span><span id="Git-191"><a href="#Git-191"><span class="linenos">191</span></a><span class="sd">        #### :params:</span>
-</span><span id="Git-192"><a href="#Git-192"><span class="linenos">192</span></a>
-</span><span id="Git-193"><a href="#Git-193"><span class="linenos">193</span></a><span class="sd">        `owner`: The repo owner.</span>
+</span><span id="Git-175"><a href="#Git-175"><span class="linenos">175</span></a>    <span class="k">def</span> <span class="nf">create_remote_from_cwd</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">public</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git-176"><a href="#Git-176"><span class="linenos">176</span></a>        <span class="sd">&quot;&quot;&quot;Use GitHub CLI (must be installed and configured) to create a remote GitHub repo from</span>
+</span><span id="Git-177"><a href="#Git-177"><span class="linenos">177</span></a><span class="sd">        the current working directory repo and add its url as this repo&#39;s remote origin.</span>
+</span><span id="Git-178"><a href="#Git-178"><span class="linenos">178</span></a>
+</span><span id="Git-179"><a href="#Git-179"><span class="linenos">179</span></a><span class="sd">        #### :params:</span>
+</span><span id="Git-180"><a href="#Git-180"><span class="linenos">180</span></a>
+</span><span id="Git-181"><a href="#Git-181"><span class="linenos">181</span></a><span class="sd">        `public`: Create the GitHub repo as a public repo, default is to create it as private.&quot;&quot;&quot;</span>
+</span><span id="Git-182"><a href="#Git-182"><span class="linenos">182</span></a>        <span class="n">visibility</span> <span class="o">=</span> <span class="s2">&quot;public&quot;</span> <span class="k">if</span> <span class="n">public</span> <span class="k">else</span> <span class="s2">&quot;private&quot;</span>
+</span><span id="Git-183"><a href="#Git-183"><span class="linenos">183</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_run</span><span class="p">(</span>
+</span><span id="Git-184"><a href="#Git-184"><span class="linenos">184</span></a>            <span class="p">[</span><span class="s2">&quot;gh&quot;</span><span class="p">,</span> <span class="s2">&quot;repo&quot;</span><span class="p">,</span> <span class="s2">&quot;create&quot;</span><span class="p">,</span> <span class="s2">&quot;--source&quot;</span><span class="p">,</span> <span class="s2">&quot;.&quot;</span><span class="p">,</span> <span class="sa">f</span><span class="s2">&quot;--</span><span class="si">{</span><span class="n">visibility</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">,</span> <span class="s2">&quot;--push&quot;</span><span class="p">]</span>
+</span><span id="Git-185"><a href="#Git-185"><span class="linenos">185</span></a>        <span class="p">)</span>
+</span><span id="Git-186"><a href="#Git-186"><span class="linenos">186</span></a>
+</span><span id="Git-187"><a href="#Git-187"><span class="linenos">187</span></a>    <span class="k">def</span> <span class="nf">_change_visibility</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">visibility</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git-188"><a href="#Git-188"><span class="linenos">188</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_run</span><span class="p">(</span>
+</span><span id="Git-189"><a href="#Git-189"><span class="linenos">189</span></a>            <span class="p">[</span><span class="s2">&quot;gh&quot;</span><span class="p">,</span> <span class="s2">&quot;repo&quot;</span><span class="p">,</span> <span class="s2">&quot;edit&quot;</span><span class="p">,</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">owner</span><span class="si">}</span><span class="s2">/</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">,</span> <span class="s2">&quot;--visibility&quot;</span><span class="p">,</span> <span class="n">visibility</span><span class="p">]</span>
+</span><span id="Git-190"><a href="#Git-190"><span class="linenos">190</span></a>        <span class="p">)</span>
+</span><span id="Git-191"><a href="#Git-191"><span class="linenos">191</span></a>
+</span><span id="Git-192"><a href="#Git-192"><span class="linenos">192</span></a>    <span class="k">def</span> <span class="nf">make_private</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git-193"><a href="#Git-193"><span class="linenos">193</span></a>        <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be installed and configured) to set the repo&#39;s visibility to private.</span>
 </span><span id="Git-194"><a href="#Git-194"><span class="linenos">194</span></a>
-</span><span id="Git-195"><a href="#Git-195"><span class="linenos">195</span></a><span class="sd">        `name`: The name of the repo to edit.&quot;&quot;&quot;</span>
-</span><span id="Git-196"><a href="#Git-196"><span class="linenos">196</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_change_visibility</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">name</span><span class="p">,</span> <span class="s2">&quot;private&quot;</span><span class="p">)</span>
-</span><span id="Git-197"><a href="#Git-197"><span class="linenos">197</span></a>
-</span><span id="Git-198"><a href="#Git-198"><span class="linenos">198</span></a>    <span class="k">def</span> <span class="nf">make_public</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git-199"><a href="#Git-199"><span class="linenos">199</span></a>        <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be installed and configured) to set the repo&#39;s visibility to public.</span>
-</span><span id="Git-200"><a href="#Git-200"><span class="linenos">200</span></a>
-</span><span id="Git-201"><a href="#Git-201"><span class="linenos">201</span></a><span class="sd">        #### :params:</span>
-</span><span id="Git-202"><a href="#Git-202"><span class="linenos">202</span></a>
-</span><span id="Git-203"><a href="#Git-203"><span class="linenos">203</span></a><span class="sd">        `owner`: The repo owner.</span>
+</span><span id="Git-195"><a href="#Git-195"><span class="linenos">195</span></a><span class="sd">        #### :params:</span>
+</span><span id="Git-196"><a href="#Git-196"><span class="linenos">196</span></a>
+</span><span id="Git-197"><a href="#Git-197"><span class="linenos">197</span></a><span class="sd">        `owner`: The repo owner.</span>
+</span><span id="Git-198"><a href="#Git-198"><span class="linenos">198</span></a>
+</span><span id="Git-199"><a href="#Git-199"><span class="linenos">199</span></a><span class="sd">        `name`: The name of the repo to edit.&quot;&quot;&quot;</span>
+</span><span id="Git-200"><a href="#Git-200"><span class="linenos">200</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_change_visibility</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">name</span><span class="p">,</span> <span class="s2">&quot;private&quot;</span><span class="p">)</span>
+</span><span id="Git-201"><a href="#Git-201"><span class="linenos">201</span></a>
+</span><span id="Git-202"><a href="#Git-202"><span class="linenos">202</span></a>    <span class="k">def</span> <span class="nf">make_public</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git-203"><a href="#Git-203"><span class="linenos">203</span></a>        <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be installed and configured) to set the repo&#39;s visibility to public.</span>
 </span><span id="Git-204"><a href="#Git-204"><span class="linenos">204</span></a>
-</span><span id="Git-205"><a href="#Git-205"><span class="linenos">205</span></a><span class="sd">        `name`: The name of the repo to edit.&quot;&quot;&quot;</span>
-</span><span id="Git-206"><a href="#Git-206"><span class="linenos">206</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_change_visibility</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">name</span><span class="p">,</span> <span class="s2">&quot;public&quot;</span><span class="p">)</span>
-</span><span id="Git-207"><a href="#Git-207"><span class="linenos">207</span></a>
-</span><span id="Git-208"><a href="#Git-208"><span class="linenos">208</span></a>    <span class="k">def</span> <span class="nf">delete_remote</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git-209"><a href="#Git-209"><span class="linenos">209</span></a>        <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be isntalled and configured) to delete the remote for this repo.</span>
-</span><span id="Git-210"><a href="#Git-210"><span class="linenos">210</span></a>
-</span><span id="Git-211"><a href="#Git-211"><span class="linenos">211</span></a><span class="sd">        #### :params:</span>
-</span><span id="Git-212"><a href="#Git-212"><span class="linenos">212</span></a>
-</span><span id="Git-213"><a href="#Git-213"><span class="linenos">213</span></a><span class="sd">        `owner`: The repo owner.</span>
+</span><span id="Git-205"><a href="#Git-205"><span class="linenos">205</span></a><span class="sd">        #### :params:</span>
+</span><span id="Git-206"><a href="#Git-206"><span class="linenos">206</span></a>
+</span><span id="Git-207"><a href="#Git-207"><span class="linenos">207</span></a><span class="sd">        `owner`: The repo owner.</span>
+</span><span id="Git-208"><a href="#Git-208"><span class="linenos">208</span></a>
+</span><span id="Git-209"><a href="#Git-209"><span class="linenos">209</span></a><span class="sd">        `name`: The name of the repo to edit.&quot;&quot;&quot;</span>
+</span><span id="Git-210"><a href="#Git-210"><span class="linenos">210</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_change_visibility</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">name</span><span class="p">,</span> <span class="s2">&quot;public&quot;</span><span class="p">)</span>
+</span><span id="Git-211"><a href="#Git-211"><span class="linenos">211</span></a>
+</span><span id="Git-212"><a href="#Git-212"><span class="linenos">212</span></a>    <span class="k">def</span> <span class="nf">delete_remote</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git-213"><a href="#Git-213"><span class="linenos">213</span></a>        <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be isntalled and configured) to delete the remote for this repo.</span>
 </span><span id="Git-214"><a href="#Git-214"><span class="linenos">214</span></a>
-</span><span id="Git-215"><a href="#Git-215"><span class="linenos">215</span></a><span class="sd">        `name`: The name of the remote repo to delete.&quot;&quot;&quot;</span>
-</span><span id="Git-216"><a href="#Git-216"><span class="linenos">216</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_run</span><span class="p">([</span><span class="s2">&quot;gh&quot;</span><span class="p">,</span> <span class="s2">&quot;repo&quot;</span><span class="p">,</span> <span class="s2">&quot;delete&quot;</span><span class="p">,</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">owner</span><span class="si">}</span><span class="s2">/</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">,</span> <span class="s2">&quot;--yes&quot;</span><span class="p">])</span>
+</span><span id="Git-215"><a href="#Git-215"><span class="linenos">215</span></a><span class="sd">        #### :params:</span>
+</span><span id="Git-216"><a href="#Git-216"><span class="linenos">216</span></a>
+</span><span id="Git-217"><a href="#Git-217"><span class="linenos">217</span></a><span class="sd">        `owner`: The repo owner.</span>
+</span><span id="Git-218"><a href="#Git-218"><span class="linenos">218</span></a>
+</span><span id="Git-219"><a href="#Git-219"><span class="linenos">219</span></a><span class="sd">        `name`: The name of the remote repo to delete.&quot;&quot;&quot;</span>
+</span><span id="Git-220"><a href="#Git-220"><span class="linenos">220</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_run</span><span class="p">([</span><span class="s2">&quot;gh&quot;</span><span class="p">,</span> <span class="s2">&quot;repo&quot;</span><span class="p">,</span> <span class="s2">&quot;delete&quot;</span><span class="p">,</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">owner</span><span class="si">}</span><span class="s2">/</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">,</span> <span class="s2">&quot;--yes&quot;</span><span class="p">])</span>
 </span></pre></div>
 
 
     
 
                             <div id="Git.__init__" class="classattr">
                                         <input id="Git.__init__-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
@@ -870,31 +878,39 @@
 
                             </div>
                             <div id="Git.tag" class="classattr">
                                         <input id="Git.tag-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
-        <span class="name">tag</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">id_</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">) -> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span>:</span></span>
+        <span class="name">tag</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">args</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s1">&#39;&#39;</span></span><span class="return-annotation">) -> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span>:</span></span>
 
                 <label class="view-source-button" for="Git.tag-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Git.tag"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.tag-83"><a href="#Git.tag-83"><span class="linenos">83</span></a>    <span class="k">def</span> <span class="nf">tag</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">id_</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git.tag-84"><a href="#Git.tag-84"><span class="linenos">84</span></a>        <span class="sd">&quot;&quot;&quot;Tag the current commit with `id_`.</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.tag-83"><a href="#Git.tag-83"><span class="linenos">83</span></a>    <span class="k">def</span> <span class="nf">tag</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git.tag-84"><a href="#Git.tag-84"><span class="linenos">84</span></a>        <span class="sd">&quot;&quot;&quot;Execute the `tag` command with `args`.</span>
 </span><span id="Git.tag-85"><a href="#Git.tag-85"><span class="linenos">85</span></a>
-</span><span id="Git.tag-86"><a href="#Git.tag-86"><span class="linenos">86</span></a><span class="sd">        Equivalent to `git tag {id_}`.&quot;&quot;&quot;</span>
-</span><span id="Git.tag-87"><a href="#Git.tag-87"><span class="linenos">87</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;tag </span><span class="si">{</span><span class="n">id_</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="Git.tag-86"><a href="#Git.tag-86"><span class="linenos">86</span></a><span class="sd">        e.g.</span>
+</span><span id="Git.tag-87"><a href="#Git.tag-87"><span class="linenos">87</span></a>
+</span><span id="Git.tag-88"><a href="#Git.tag-88"><span class="linenos">88</span></a><span class="sd">        `self.tag(&quot;--sort=-committerdate&quot;)`</span>
+</span><span id="Git.tag-89"><a href="#Git.tag-89"><span class="linenos">89</span></a>
+</span><span id="Git.tag-90"><a href="#Git.tag-90"><span class="linenos">90</span></a><span class="sd">        will list all the tags for this repository in descending commit date.&quot;&quot;&quot;</span>
+</span><span id="Git.tag-91"><a href="#Git.tag-91"><span class="linenos">91</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;tag </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
-            <div class="docstring"><p>Tag the current commit with <code>id_</code>.</p>
+            <div class="docstring"><p>Execute the <code><a href="#Git.tag">tag</a></code> command with <code>args</code>.</p>
 
-<p>Equivalent to <code>git tag {id_}</code>.</p>
+<p>e.g.</p>
+
+<p><code>self.tag("--sort=-committerdate")</code></p>
+
+<p>will list all the tags for this repository in descending commit date.</p>
 </div>
 
 
                             </div>
                             <div id="Git.add_remote_url" class="classattr">
                                         <input id="Git.add_remote_url-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
@@ -902,17 +918,17 @@
         <span class="def">def</span>
         <span class="name">add_remote_url</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">url</span><span class="p">:</span> <span class="nb">str</span>, </span><span class="param"><span class="n">name</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s1">&#39;origin&#39;</span></span><span class="return-annotation">) -> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span>:</span></span>
 
                 <label class="view-source-button" for="Git.add_remote_url-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Git.add_remote_url"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.add_remote_url-90"><a href="#Git.add_remote_url-90"><span class="linenos">90</span></a>    <span class="k">def</span> <span class="nf">add_remote_url</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">url</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;origin&quot;</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git.add_remote_url-91"><a href="#Git.add_remote_url-91"><span class="linenos">91</span></a>        <span class="sd">&quot;&quot;&quot;Add remote url to repo.&quot;&quot;&quot;</span>
-</span><span id="Git.add_remote_url-92"><a href="#Git.add_remote_url-92"><span class="linenos">92</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;remote add </span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">url</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.add_remote_url-94"><a href="#Git.add_remote_url-94"><span class="linenos">94</span></a>    <span class="k">def</span> <span class="nf">add_remote_url</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">url</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;origin&quot;</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git.add_remote_url-95"><a href="#Git.add_remote_url-95"><span class="linenos">95</span></a>        <span class="sd">&quot;&quot;&quot;Add remote url to repo.&quot;&quot;&quot;</span>
+</span><span id="Git.add_remote_url-96"><a href="#Git.add_remote_url-96"><span class="linenos">96</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;remote add </span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">url</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Add remote url to repo.</p>
 </div>
 
 
@@ -924,17 +940,17 @@
         <span class="def">def</span>
         <span class="name">push</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">args</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s1">&#39;&#39;</span></span><span class="return-annotation">) -> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span>:</span></span>
 
                 <label class="view-source-button" for="Git.push-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Git.push"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.push-94"><a href="#Git.push-94"><span class="linenos">94</span></a>    <span class="k">def</span> <span class="nf">push</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git.push-95"><a href="#Git.push-95"><span class="linenos">95</span></a>        <span class="sd">&quot;&quot;&quot;Equivalent to `git push {args}`.&quot;&quot;&quot;</span>
-</span><span id="Git.push-96"><a href="#Git.push-96"><span class="linenos">96</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;push </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.push-98"><a href="#Git.push-98"><span class="linenos"> 98</span></a>    <span class="k">def</span> <span class="nf">push</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git.push-99"><a href="#Git.push-99"><span class="linenos"> 99</span></a>        <span class="sd">&quot;&quot;&quot;Equivalent to `git push {args}`.&quot;&quot;&quot;</span>
+</span><span id="Git.push-100"><a href="#Git.push-100"><span class="linenos">100</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;push </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Equivalent to <code>git push {args}</code>.</p>
 </div>
 
 
@@ -946,17 +962,17 @@
         <span class="def">def</span>
         <span class="name">pull</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">args</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s1">&#39;&#39;</span></span><span class="return-annotation">) -> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span>:</span></span>
 
                 <label class="view-source-button" for="Git.pull-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Git.pull"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.pull-98"><a href="#Git.pull-98"><span class="linenos"> 98</span></a>    <span class="k">def</span> <span class="nf">pull</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git.pull-99"><a href="#Git.pull-99"><span class="linenos"> 99</span></a>        <span class="sd">&quot;&quot;&quot;Equivalent to `git pull {args}`.&quot;&quot;&quot;</span>
-</span><span id="Git.pull-100"><a href="#Git.pull-100"><span class="linenos">100</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;pull </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.pull-102"><a href="#Git.pull-102"><span class="linenos">102</span></a>    <span class="k">def</span> <span class="nf">pull</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git.pull-103"><a href="#Git.pull-103"><span class="linenos">103</span></a>        <span class="sd">&quot;&quot;&quot;Equivalent to `git pull {args}`.&quot;&quot;&quot;</span>
+</span><span id="Git.pull-104"><a href="#Git.pull-104"><span class="linenos">104</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;pull </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Equivalent to <code>git pull {args}</code>.</p>
 </div>
 
 
@@ -968,19 +984,19 @@
         <span class="def">def</span>
         <span class="name">push_new_branch</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">branch</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">) -> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span>:</span></span>
 
                 <label class="view-source-button" for="Git.push_new_branch-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Git.push_new_branch"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.push_new_branch-102"><a href="#Git.push_new_branch-102"><span class="linenos">102</span></a>    <span class="k">def</span> <span class="nf">push_new_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git.push_new_branch-103"><a href="#Git.push_new_branch-103"><span class="linenos">103</span></a>        <span class="sd">&quot;&quot;&quot;Push a new branch to origin with tracking.</span>
-</span><span id="Git.push_new_branch-104"><a href="#Git.push_new_branch-104"><span class="linenos">104</span></a>
-</span><span id="Git.push_new_branch-105"><a href="#Git.push_new_branch-105"><span class="linenos">105</span></a><span class="sd">        Equivalent to `git push -u origin {branch}`.&quot;&quot;&quot;</span>
-</span><span id="Git.push_new_branch-106"><a href="#Git.push_new_branch-106"><span class="linenos">106</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;-u origin </span><span class="si">{</span><span class="n">branch</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.push_new_branch-106"><a href="#Git.push_new_branch-106"><span class="linenos">106</span></a>    <span class="k">def</span> <span class="nf">push_new_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git.push_new_branch-107"><a href="#Git.push_new_branch-107"><span class="linenos">107</span></a>        <span class="sd">&quot;&quot;&quot;Push a new branch to origin with tracking.</span>
+</span><span id="Git.push_new_branch-108"><a href="#Git.push_new_branch-108"><span class="linenos">108</span></a>
+</span><span id="Git.push_new_branch-109"><a href="#Git.push_new_branch-109"><span class="linenos">109</span></a><span class="sd">        Equivalent to `git push -u origin {branch}`.&quot;&quot;&quot;</span>
+</span><span id="Git.push_new_branch-110"><a href="#Git.push_new_branch-110"><span class="linenos">110</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;-u origin </span><span class="si">{</span><span class="n">branch</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Push a new branch to origin with tracking.</p>
 
 <p>Equivalent to <code>git push -u origin {branch}</code>.</p>
 </div>
@@ -994,17 +1010,17 @@
         <span class="def">def</span>
         <span class="name">pull_branch</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">branch</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">) -> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span>:</span></span>
 
                 <label class="view-source-button" for="Git.pull_branch-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Git.pull_branch"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.pull_branch-108"><a href="#Git.pull_branch-108"><span class="linenos">108</span></a>    <span class="k">def</span> <span class="nf">pull_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git.pull_branch-109"><a href="#Git.pull_branch-109"><span class="linenos">109</span></a>        <span class="sd">&quot;&quot;&quot;Pull `branch` from origin.&quot;&quot;&quot;</span>
-</span><span id="Git.pull_branch-110"><a href="#Git.pull_branch-110"><span class="linenos">110</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">pull</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;origin </span><span class="si">{</span><span class="n">branch</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.pull_branch-112"><a href="#Git.pull_branch-112"><span class="linenos">112</span></a>    <span class="k">def</span> <span class="nf">pull_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git.pull_branch-113"><a href="#Git.pull_branch-113"><span class="linenos">113</span></a>        <span class="sd">&quot;&quot;&quot;Pull `branch` from origin.&quot;&quot;&quot;</span>
+</span><span id="Git.pull_branch-114"><a href="#Git.pull_branch-114"><span class="linenos">114</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">pull</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;origin </span><span class="si">{</span><span class="n">branch</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Pull <code><a href="#Git.branch">branch</a></code> from origin.</p>
 </div>
 
 
@@ -1016,17 +1032,17 @@
         <span class="def">def</span>
         <span class="name">branch</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">args</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">) -> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span>:</span></span>
 
                 <label class="view-source-button" for="Git.branch-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Git.branch"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.branch-113"><a href="#Git.branch-113"><span class="linenos">113</span></a>    <span class="k">def</span> <span class="nf">branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git.branch-114"><a href="#Git.branch-114"><span class="linenos">114</span></a>        <span class="sd">&quot;&quot;&quot;Equivalent to `git branch {args}`.&quot;&quot;&quot;</span>
-</span><span id="Git.branch-115"><a href="#Git.branch-115"><span class="linenos">115</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;branch </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.branch-117"><a href="#Git.branch-117"><span class="linenos">117</span></a>    <span class="k">def</span> <span class="nf">branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git.branch-118"><a href="#Git.branch-118"><span class="linenos">118</span></a>        <span class="sd">&quot;&quot;&quot;Equivalent to `git branch {args}`.&quot;&quot;&quot;</span>
+</span><span id="Git.branch-119"><a href="#Git.branch-119"><span class="linenos">119</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;branch </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Equivalent to <code>git branch {args}</code>.</p>
 </div>
 
 
@@ -1038,17 +1054,17 @@
         <span class="def">def</span>
         <span class="name">list_branches</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span></span><span class="return-annotation">) -> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span>:</span></span>
 
                 <label class="view-source-button" for="Git.list_branches-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Git.list_branches"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.list_branches-117"><a href="#Git.list_branches-117"><span class="linenos">117</span></a>    <span class="k">def</span> <span class="nf">list_branches</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git.list_branches-118"><a href="#Git.list_branches-118"><span class="linenos">118</span></a>        <span class="sd">&quot;&quot;&quot;Print a list of branches.&quot;&quot;&quot;</span>
-</span><span id="Git.list_branches-119"><a href="#Git.list_branches-119"><span class="linenos">119</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">branch</span><span class="p">(</span><span class="s2">&quot;-vva&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.list_branches-121"><a href="#Git.list_branches-121"><span class="linenos">121</span></a>    <span class="k">def</span> <span class="nf">list_branches</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git.list_branches-122"><a href="#Git.list_branches-122"><span class="linenos">122</span></a>        <span class="sd">&quot;&quot;&quot;Print a list of branches.&quot;&quot;&quot;</span>
+</span><span id="Git.list_branches-123"><a href="#Git.list_branches-123"><span class="linenos">123</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">branch</span><span class="p">(</span><span class="s2">&quot;-vva&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Print a list of branches.</p>
 </div>
 
 
@@ -1060,17 +1076,17 @@
         <span class="def">def</span>
         <span class="name">checkout</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">args</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">) -> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span>:</span></span>
 
                 <label class="view-source-button" for="Git.checkout-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Git.checkout"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.checkout-121"><a href="#Git.checkout-121"><span class="linenos">121</span></a>    <span class="k">def</span> <span class="nf">checkout</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git.checkout-122"><a href="#Git.checkout-122"><span class="linenos">122</span></a>        <span class="sd">&quot;&quot;&quot;Equivalent to `git checkout {args}`.&quot;&quot;&quot;</span>
-</span><span id="Git.checkout-123"><a href="#Git.checkout-123"><span class="linenos">123</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;checkout </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.checkout-125"><a href="#Git.checkout-125"><span class="linenos">125</span></a>    <span class="k">def</span> <span class="nf">checkout</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git.checkout-126"><a href="#Git.checkout-126"><span class="linenos">126</span></a>        <span class="sd">&quot;&quot;&quot;Equivalent to `git checkout {args}`.&quot;&quot;&quot;</span>
+</span><span id="Git.checkout-127"><a href="#Git.checkout-127"><span class="linenos">127</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;checkout </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Equivalent to <code>git checkout {args}</code>.</p>
 </div>
 
 
@@ -1082,19 +1098,19 @@
         <span class="def">def</span>
         <span class="name">switch_branch</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">) -> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span>:</span></span>
 
                 <label class="view-source-button" for="Git.switch_branch-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Git.switch_branch"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.switch_branch-125"><a href="#Git.switch_branch-125"><span class="linenos">125</span></a>    <span class="k">def</span> <span class="nf">switch_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git.switch_branch-126"><a href="#Git.switch_branch-126"><span class="linenos">126</span></a>        <span class="sd">&quot;&quot;&quot;Switch to the branch specified by `branch_name`.</span>
-</span><span id="Git.switch_branch-127"><a href="#Git.switch_branch-127"><span class="linenos">127</span></a>
-</span><span id="Git.switch_branch-128"><a href="#Git.switch_branch-128"><span class="linenos">128</span></a><span class="sd">        Equivalent to `git checkout {branch_name}`.&quot;&quot;&quot;</span>
-</span><span id="Git.switch_branch-129"><a href="#Git.switch_branch-129"><span class="linenos">129</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">checkout</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.switch_branch-129"><a href="#Git.switch_branch-129"><span class="linenos">129</span></a>    <span class="k">def</span> <span class="nf">switch_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git.switch_branch-130"><a href="#Git.switch_branch-130"><span class="linenos">130</span></a>        <span class="sd">&quot;&quot;&quot;Switch to the branch specified by `branch_name`.</span>
+</span><span id="Git.switch_branch-131"><a href="#Git.switch_branch-131"><span class="linenos">131</span></a>
+</span><span id="Git.switch_branch-132"><a href="#Git.switch_branch-132"><span class="linenos">132</span></a><span class="sd">        Equivalent to `git checkout {branch_name}`.&quot;&quot;&quot;</span>
+</span><span id="Git.switch_branch-133"><a href="#Git.switch_branch-133"><span class="linenos">133</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">checkout</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Switch to the branch specified by <code>branch_name</code>.</p>
 
 <p>Equivalent to <code>git checkout {branch_name}</code>.</p>
 </div>
@@ -1108,19 +1124,19 @@
         <span class="def">def</span>
         <span class="name">create_new_branch</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">) -> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span>:</span></span>
 
                 <label class="view-source-button" for="Git.create_new_branch-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Git.create_new_branch"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.create_new_branch-131"><a href="#Git.create_new_branch-131"><span class="linenos">131</span></a>    <span class="k">def</span> <span class="nf">create_new_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git.create_new_branch-132"><a href="#Git.create_new_branch-132"><span class="linenos">132</span></a>        <span class="sd">&quot;&quot;&quot;Create and switch to a new branch named with `branch_name`.</span>
-</span><span id="Git.create_new_branch-133"><a href="#Git.create_new_branch-133"><span class="linenos">133</span></a>
-</span><span id="Git.create_new_branch-134"><a href="#Git.create_new_branch-134"><span class="linenos">134</span></a><span class="sd">        Equivalent to `git checkout -b {branch_name} --track`.&quot;&quot;&quot;</span>
-</span><span id="Git.create_new_branch-135"><a href="#Git.create_new_branch-135"><span class="linenos">135</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">checkout</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;-b </span><span class="si">{</span><span class="n">branch_name</span><span class="si">}</span><span class="s2"> --track&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.create_new_branch-135"><a href="#Git.create_new_branch-135"><span class="linenos">135</span></a>    <span class="k">def</span> <span class="nf">create_new_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git.create_new_branch-136"><a href="#Git.create_new_branch-136"><span class="linenos">136</span></a>        <span class="sd">&quot;&quot;&quot;Create and switch to a new branch named with `branch_name`.</span>
+</span><span id="Git.create_new_branch-137"><a href="#Git.create_new_branch-137"><span class="linenos">137</span></a>
+</span><span id="Git.create_new_branch-138"><a href="#Git.create_new_branch-138"><span class="linenos">138</span></a><span class="sd">        Equivalent to `git checkout -b {branch_name} --track`.&quot;&quot;&quot;</span>
+</span><span id="Git.create_new_branch-139"><a href="#Git.create_new_branch-139"><span class="linenos">139</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">checkout</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;-b </span><span class="si">{</span><span class="n">branch_name</span><span class="si">}</span><span class="s2"> --track&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Create and switch to a new branch named with <code>branch_name</code>.</p>
 
 <p>Equivalent to <code>git checkout -b {branch_name} --track</code>.</p>
 </div>
@@ -1134,24 +1150,24 @@
         <span class="def">def</span>
         <span class="name">delete_branch</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span>, </span><span class="param"><span class="n">local_only</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span></span><span class="return-annotation">) -> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span>:</span></span>
 
                 <label class="view-source-button" for="Git.delete_branch-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Git.delete_branch"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.delete_branch-137"><a href="#Git.delete_branch-137"><span class="linenos">137</span></a>    <span class="k">def</span> <span class="nf">delete_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">local_only</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git.delete_branch-138"><a href="#Git.delete_branch-138"><span class="linenos">138</span></a>        <span class="sd">&quot;&quot;&quot;Delete `branch_name` from repo.</span>
-</span><span id="Git.delete_branch-139"><a href="#Git.delete_branch-139"><span class="linenos">139</span></a>
-</span><span id="Git.delete_branch-140"><a href="#Git.delete_branch-140"><span class="linenos">140</span></a><span class="sd">        #### :params:</span>
-</span><span id="Git.delete_branch-141"><a href="#Git.delete_branch-141"><span class="linenos">141</span></a>
-</span><span id="Git.delete_branch-142"><a href="#Git.delete_branch-142"><span class="linenos">142</span></a><span class="sd">        `local_only`: Only delete the local copy of `branch`, otherwise also delete the remote branch on origin and remote-tracking branch.&quot;&quot;&quot;</span>
-</span><span id="Git.delete_branch-143"><a href="#Git.delete_branch-143"><span class="linenos">143</span></a>        <span class="n">output</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">branch</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;--delete </span><span class="si">{</span><span class="n">branch_name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="Git.delete_branch-144"><a href="#Git.delete_branch-144"><span class="linenos">144</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">local_only</span><span class="p">:</span>
-</span><span id="Git.delete_branch-145"><a href="#Git.delete_branch-145"><span class="linenos">145</span></a>            <span class="k">return</span> <span class="n">output</span> <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;origin --delete </span><span class="si">{</span><span class="n">branch_name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>  <span class="c1"># type:ignore</span>
-</span><span id="Git.delete_branch-146"><a href="#Git.delete_branch-146"><span class="linenos">146</span></a>        <span class="k">return</span> <span class="n">output</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.delete_branch-141"><a href="#Git.delete_branch-141"><span class="linenos">141</span></a>    <span class="k">def</span> <span class="nf">delete_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">local_only</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git.delete_branch-142"><a href="#Git.delete_branch-142"><span class="linenos">142</span></a>        <span class="sd">&quot;&quot;&quot;Delete `branch_name` from repo.</span>
+</span><span id="Git.delete_branch-143"><a href="#Git.delete_branch-143"><span class="linenos">143</span></a>
+</span><span id="Git.delete_branch-144"><a href="#Git.delete_branch-144"><span class="linenos">144</span></a><span class="sd">        #### :params:</span>
+</span><span id="Git.delete_branch-145"><a href="#Git.delete_branch-145"><span class="linenos">145</span></a>
+</span><span id="Git.delete_branch-146"><a href="#Git.delete_branch-146"><span class="linenos">146</span></a><span class="sd">        `local_only`: Only delete the local copy of `branch`, otherwise also delete the remote branch on origin and remote-tracking branch.&quot;&quot;&quot;</span>
+</span><span id="Git.delete_branch-147"><a href="#Git.delete_branch-147"><span class="linenos">147</span></a>        <span class="n">output</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">branch</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;--delete </span><span class="si">{</span><span class="n">branch_name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="Git.delete_branch-148"><a href="#Git.delete_branch-148"><span class="linenos">148</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">local_only</span><span class="p">:</span>
+</span><span id="Git.delete_branch-149"><a href="#Git.delete_branch-149"><span class="linenos">149</span></a>            <span class="k">return</span> <span class="n">output</span> <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;origin --delete </span><span class="si">{</span><span class="n">branch_name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>  <span class="c1"># type:ignore</span>
+</span><span id="Git.delete_branch-150"><a href="#Git.delete_branch-150"><span class="linenos">150</span></a>        <span class="k">return</span> <span class="n">output</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Delete <code>branch_name</code> from repo.</p>
 
 <h4 id="params">:params:</h4>
 
@@ -1167,19 +1183,19 @@
         <span class="def">def</span>
         <span class="name">undo</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span></span><span class="return-annotation">) -> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span>:</span></span>
 
                 <label class="view-source-button" for="Git.undo-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Git.undo"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.undo-148"><a href="#Git.undo-148"><span class="linenos">148</span></a>    <span class="k">def</span> <span class="nf">undo</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git.undo-149"><a href="#Git.undo-149"><span class="linenos">149</span></a>        <span class="sd">&quot;&quot;&quot;Undo uncommitted changes.</span>
-</span><span id="Git.undo-150"><a href="#Git.undo-150"><span class="linenos">150</span></a>
-</span><span id="Git.undo-151"><a href="#Git.undo-151"><span class="linenos">151</span></a><span class="sd">        Equivalent to `git checkout .`.&quot;&quot;&quot;</span>
-</span><span id="Git.undo-152"><a href="#Git.undo-152"><span class="linenos">152</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">checkout</span><span class="p">(</span><span class="s2">&quot;.&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.undo-152"><a href="#Git.undo-152"><span class="linenos">152</span></a>    <span class="k">def</span> <span class="nf">undo</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git.undo-153"><a href="#Git.undo-153"><span class="linenos">153</span></a>        <span class="sd">&quot;&quot;&quot;Undo uncommitted changes.</span>
+</span><span id="Git.undo-154"><a href="#Git.undo-154"><span class="linenos">154</span></a>
+</span><span id="Git.undo-155"><a href="#Git.undo-155"><span class="linenos">155</span></a><span class="sd">        Equivalent to `git checkout .`.&quot;&quot;&quot;</span>
+</span><span id="Git.undo-156"><a href="#Git.undo-156"><span class="linenos">156</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">checkout</span><span class="p">(</span><span class="s2">&quot;.&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Undo uncommitted changes.</p>
 
 <p>Equivalent to <code>git checkout .</code>.</p>
 </div>
@@ -1193,17 +1209,17 @@
         <span class="def">def</span>
         <span class="name">merge</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">) -> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span>:</span></span>
 
                 <label class="view-source-button" for="Git.merge-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Git.merge"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.merge-154"><a href="#Git.merge-154"><span class="linenos">154</span></a>    <span class="k">def</span> <span class="nf">merge</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git.merge-155"><a href="#Git.merge-155"><span class="linenos">155</span></a>        <span class="sd">&quot;&quot;&quot;Merge branch `branch_name` with currently active branch.&quot;&quot;&quot;</span>
-</span><span id="Git.merge-156"><a href="#Git.merge-156"><span class="linenos">156</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;merge </span><span class="si">{</span><span class="n">branch_name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.merge-158"><a href="#Git.merge-158"><span class="linenos">158</span></a>    <span class="k">def</span> <span class="nf">merge</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git.merge-159"><a href="#Git.merge-159"><span class="linenos">159</span></a>        <span class="sd">&quot;&quot;&quot;Merge branch `branch_name` with currently active branch.&quot;&quot;&quot;</span>
+</span><span id="Git.merge-160"><a href="#Git.merge-160"><span class="linenos">160</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;merge </span><span class="si">{</span><span class="n">branch_name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Merge branch <code>branch_name</code> with currently active branch.</p>
 </div>
 
 
@@ -1215,24 +1231,24 @@
         <span class="def">def</span>
         <span class="name">create_remote</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">name</span><span class="p">:</span> <span class="nb">str</span>, </span><span class="param"><span class="n">public</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span></span><span class="return-annotation">) -> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span>:</span></span>
 
                 <label class="view-source-button" for="Git.create_remote-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Git.create_remote"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.create_remote-160"><a href="#Git.create_remote-160"><span class="linenos">160</span></a>    <span class="k">def</span> <span class="nf">create_remote</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">public</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git.create_remote-161"><a href="#Git.create_remote-161"><span class="linenos">161</span></a>        <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be installed and configured) to create a remote GitHub repo.</span>
-</span><span id="Git.create_remote-162"><a href="#Git.create_remote-162"><span class="linenos">162</span></a>
-</span><span id="Git.create_remote-163"><a href="#Git.create_remote-163"><span class="linenos">163</span></a><span class="sd">        #### :params:</span>
-</span><span id="Git.create_remote-164"><a href="#Git.create_remote-164"><span class="linenos">164</span></a>
-</span><span id="Git.create_remote-165"><a href="#Git.create_remote-165"><span class="linenos">165</span></a><span class="sd">        `name`: The name for the repo.</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.create_remote-164"><a href="#Git.create_remote-164"><span class="linenos">164</span></a>    <span class="k">def</span> <span class="nf">create_remote</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">public</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git.create_remote-165"><a href="#Git.create_remote-165"><span class="linenos">165</span></a>        <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be installed and configured) to create a remote GitHub repo.</span>
 </span><span id="Git.create_remote-166"><a href="#Git.create_remote-166"><span class="linenos">166</span></a>
-</span><span id="Git.create_remote-167"><a href="#Git.create_remote-167"><span class="linenos">167</span></a><span class="sd">        `public`: Set to `True` to create the repo as public, otherwise it&#39;ll be created as private.&quot;&quot;&quot;</span>
-</span><span id="Git.create_remote-168"><a href="#Git.create_remote-168"><span class="linenos">168</span></a>        <span class="n">visibility</span> <span class="o">=</span> <span class="s2">&quot;--public&quot;</span> <span class="k">if</span> <span class="n">public</span> <span class="k">else</span> <span class="s2">&quot;--private&quot;</span>
-</span><span id="Git.create_remote-169"><a href="#Git.create_remote-169"><span class="linenos">169</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_run</span><span class="p">([</span><span class="s2">&quot;gh&quot;</span><span class="p">,</span> <span class="s2">&quot;repo&quot;</span><span class="p">,</span> <span class="s2">&quot;create&quot;</span><span class="p">,</span> <span class="n">name</span><span class="p">,</span> <span class="n">visibility</span><span class="p">])</span>
+</span><span id="Git.create_remote-167"><a href="#Git.create_remote-167"><span class="linenos">167</span></a><span class="sd">        #### :params:</span>
+</span><span id="Git.create_remote-168"><a href="#Git.create_remote-168"><span class="linenos">168</span></a>
+</span><span id="Git.create_remote-169"><a href="#Git.create_remote-169"><span class="linenos">169</span></a><span class="sd">        `name`: The name for the repo.</span>
+</span><span id="Git.create_remote-170"><a href="#Git.create_remote-170"><span class="linenos">170</span></a>
+</span><span id="Git.create_remote-171"><a href="#Git.create_remote-171"><span class="linenos">171</span></a><span class="sd">        `public`: Set to `True` to create the repo as public, otherwise it&#39;ll be created as private.&quot;&quot;&quot;</span>
+</span><span id="Git.create_remote-172"><a href="#Git.create_remote-172"><span class="linenos">172</span></a>        <span class="n">visibility</span> <span class="o">=</span> <span class="s2">&quot;--public&quot;</span> <span class="k">if</span> <span class="n">public</span> <span class="k">else</span> <span class="s2">&quot;--private&quot;</span>
+</span><span id="Git.create_remote-173"><a href="#Git.create_remote-173"><span class="linenos">173</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_run</span><span class="p">([</span><span class="s2">&quot;gh&quot;</span><span class="p">,</span> <span class="s2">&quot;repo&quot;</span><span class="p">,</span> <span class="s2">&quot;create&quot;</span><span class="p">,</span> <span class="n">name</span><span class="p">,</span> <span class="n">visibility</span><span class="p">])</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Uses GitHub CLI (must be installed and configured) to create a remote GitHub repo.</p>
 
 <h4 id="params">:params:</h4>
 
@@ -1250,25 +1266,25 @@
         <span class="def">def</span>
         <span class="name">create_remote_from_cwd</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">public</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span></span><span class="return-annotation">) -> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span>:</span></span>
 
                 <label class="view-source-button" for="Git.create_remote_from_cwd-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Git.create_remote_from_cwd"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.create_remote_from_cwd-171"><a href="#Git.create_remote_from_cwd-171"><span class="linenos">171</span></a>    <span class="k">def</span> <span class="nf">create_remote_from_cwd</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">public</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git.create_remote_from_cwd-172"><a href="#Git.create_remote_from_cwd-172"><span class="linenos">172</span></a>        <span class="sd">&quot;&quot;&quot;Use GitHub CLI (must be installed and configured) to create a remote GitHub repo from</span>
-</span><span id="Git.create_remote_from_cwd-173"><a href="#Git.create_remote_from_cwd-173"><span class="linenos">173</span></a><span class="sd">        the current working directory repo and add its url as this repo&#39;s remote origin.</span>
-</span><span id="Git.create_remote_from_cwd-174"><a href="#Git.create_remote_from_cwd-174"><span class="linenos">174</span></a>
-</span><span id="Git.create_remote_from_cwd-175"><a href="#Git.create_remote_from_cwd-175"><span class="linenos">175</span></a><span class="sd">        #### :params:</span>
-</span><span id="Git.create_remote_from_cwd-176"><a href="#Git.create_remote_from_cwd-176"><span class="linenos">176</span></a>
-</span><span id="Git.create_remote_from_cwd-177"><a href="#Git.create_remote_from_cwd-177"><span class="linenos">177</span></a><span class="sd">        `public`: Create the GitHub repo as a public repo, default is to create it as private.&quot;&quot;&quot;</span>
-</span><span id="Git.create_remote_from_cwd-178"><a href="#Git.create_remote_from_cwd-178"><span class="linenos">178</span></a>        <span class="n">visibility</span> <span class="o">=</span> <span class="s2">&quot;public&quot;</span> <span class="k">if</span> <span class="n">public</span> <span class="k">else</span> <span class="s2">&quot;private&quot;</span>
-</span><span id="Git.create_remote_from_cwd-179"><a href="#Git.create_remote_from_cwd-179"><span class="linenos">179</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_run</span><span class="p">(</span>
-</span><span id="Git.create_remote_from_cwd-180"><a href="#Git.create_remote_from_cwd-180"><span class="linenos">180</span></a>            <span class="p">[</span><span class="s2">&quot;gh&quot;</span><span class="p">,</span> <span class="s2">&quot;repo&quot;</span><span class="p">,</span> <span class="s2">&quot;create&quot;</span><span class="p">,</span> <span class="s2">&quot;--source&quot;</span><span class="p">,</span> <span class="s2">&quot;.&quot;</span><span class="p">,</span> <span class="sa">f</span><span class="s2">&quot;--</span><span class="si">{</span><span class="n">visibility</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">,</span> <span class="s2">&quot;--push&quot;</span><span class="p">]</span>
-</span><span id="Git.create_remote_from_cwd-181"><a href="#Git.create_remote_from_cwd-181"><span class="linenos">181</span></a>        <span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.create_remote_from_cwd-175"><a href="#Git.create_remote_from_cwd-175"><span class="linenos">175</span></a>    <span class="k">def</span> <span class="nf">create_remote_from_cwd</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">public</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git.create_remote_from_cwd-176"><a href="#Git.create_remote_from_cwd-176"><span class="linenos">176</span></a>        <span class="sd">&quot;&quot;&quot;Use GitHub CLI (must be installed and configured) to create a remote GitHub repo from</span>
+</span><span id="Git.create_remote_from_cwd-177"><a href="#Git.create_remote_from_cwd-177"><span class="linenos">177</span></a><span class="sd">        the current working directory repo and add its url as this repo&#39;s remote origin.</span>
+</span><span id="Git.create_remote_from_cwd-178"><a href="#Git.create_remote_from_cwd-178"><span class="linenos">178</span></a>
+</span><span id="Git.create_remote_from_cwd-179"><a href="#Git.create_remote_from_cwd-179"><span class="linenos">179</span></a><span class="sd">        #### :params:</span>
+</span><span id="Git.create_remote_from_cwd-180"><a href="#Git.create_remote_from_cwd-180"><span class="linenos">180</span></a>
+</span><span id="Git.create_remote_from_cwd-181"><a href="#Git.create_remote_from_cwd-181"><span class="linenos">181</span></a><span class="sd">        `public`: Create the GitHub repo as a public repo, default is to create it as private.&quot;&quot;&quot;</span>
+</span><span id="Git.create_remote_from_cwd-182"><a href="#Git.create_remote_from_cwd-182"><span class="linenos">182</span></a>        <span class="n">visibility</span> <span class="o">=</span> <span class="s2">&quot;public&quot;</span> <span class="k">if</span> <span class="n">public</span> <span class="k">else</span> <span class="s2">&quot;private&quot;</span>
+</span><span id="Git.create_remote_from_cwd-183"><a href="#Git.create_remote_from_cwd-183"><span class="linenos">183</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_run</span><span class="p">(</span>
+</span><span id="Git.create_remote_from_cwd-184"><a href="#Git.create_remote_from_cwd-184"><span class="linenos">184</span></a>            <span class="p">[</span><span class="s2">&quot;gh&quot;</span><span class="p">,</span> <span class="s2">&quot;repo&quot;</span><span class="p">,</span> <span class="s2">&quot;create&quot;</span><span class="p">,</span> <span class="s2">&quot;--source&quot;</span><span class="p">,</span> <span class="s2">&quot;.&quot;</span><span class="p">,</span> <span class="sa">f</span><span class="s2">&quot;--</span><span class="si">{</span><span class="n">visibility</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">,</span> <span class="s2">&quot;--push&quot;</span><span class="p">]</span>
+</span><span id="Git.create_remote_from_cwd-185"><a href="#Git.create_remote_from_cwd-185"><span class="linenos">185</span></a>        <span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Use GitHub CLI (must be installed and configured) to create a remote GitHub repo from
 the current working directory repo and add its url as this repo's remote origin.</p>
 
 <h4 id="params">:params:</h4>
@@ -1285,23 +1301,23 @@
         <span class="def">def</span>
         <span class="name">make_private</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">owner</span><span class="p">:</span> <span class="nb">str</span>, </span><span class="param"><span class="n">name</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">) -> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span>:</span></span>
 
                 <label class="view-source-button" for="Git.make_private-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Git.make_private"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.make_private-188"><a href="#Git.make_private-188"><span class="linenos">188</span></a>    <span class="k">def</span> <span class="nf">make_private</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git.make_private-189"><a href="#Git.make_private-189"><span class="linenos">189</span></a>        <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be installed and configured) to set the repo&#39;s visibility to private.</span>
-</span><span id="Git.make_private-190"><a href="#Git.make_private-190"><span class="linenos">190</span></a>
-</span><span id="Git.make_private-191"><a href="#Git.make_private-191"><span class="linenos">191</span></a><span class="sd">        #### :params:</span>
-</span><span id="Git.make_private-192"><a href="#Git.make_private-192"><span class="linenos">192</span></a>
-</span><span id="Git.make_private-193"><a href="#Git.make_private-193"><span class="linenos">193</span></a><span class="sd">        `owner`: The repo owner.</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.make_private-192"><a href="#Git.make_private-192"><span class="linenos">192</span></a>    <span class="k">def</span> <span class="nf">make_private</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git.make_private-193"><a href="#Git.make_private-193"><span class="linenos">193</span></a>        <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be installed and configured) to set the repo&#39;s visibility to private.</span>
 </span><span id="Git.make_private-194"><a href="#Git.make_private-194"><span class="linenos">194</span></a>
-</span><span id="Git.make_private-195"><a href="#Git.make_private-195"><span class="linenos">195</span></a><span class="sd">        `name`: The name of the repo to edit.&quot;&quot;&quot;</span>
-</span><span id="Git.make_private-196"><a href="#Git.make_private-196"><span class="linenos">196</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_change_visibility</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">name</span><span class="p">,</span> <span class="s2">&quot;private&quot;</span><span class="p">)</span>
+</span><span id="Git.make_private-195"><a href="#Git.make_private-195"><span class="linenos">195</span></a><span class="sd">        #### :params:</span>
+</span><span id="Git.make_private-196"><a href="#Git.make_private-196"><span class="linenos">196</span></a>
+</span><span id="Git.make_private-197"><a href="#Git.make_private-197"><span class="linenos">197</span></a><span class="sd">        `owner`: The repo owner.</span>
+</span><span id="Git.make_private-198"><a href="#Git.make_private-198"><span class="linenos">198</span></a>
+</span><span id="Git.make_private-199"><a href="#Git.make_private-199"><span class="linenos">199</span></a><span class="sd">        `name`: The name of the repo to edit.&quot;&quot;&quot;</span>
+</span><span id="Git.make_private-200"><a href="#Git.make_private-200"><span class="linenos">200</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_change_visibility</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">name</span><span class="p">,</span> <span class="s2">&quot;private&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Uses GitHub CLI (must be installed and configured) to set the repo's visibility to private.</p>
 
 <h4 id="params">:params:</h4>
 
@@ -1319,23 +1335,23 @@
         <span class="def">def</span>
         <span class="name">make_public</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">owner</span><span class="p">:</span> <span class="nb">str</span>, </span><span class="param"><span class="n">name</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">) -> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span>:</span></span>
 
                 <label class="view-source-button" for="Git.make_public-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Git.make_public"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.make_public-198"><a href="#Git.make_public-198"><span class="linenos">198</span></a>    <span class="k">def</span> <span class="nf">make_public</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git.make_public-199"><a href="#Git.make_public-199"><span class="linenos">199</span></a>        <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be installed and configured) to set the repo&#39;s visibility to public.</span>
-</span><span id="Git.make_public-200"><a href="#Git.make_public-200"><span class="linenos">200</span></a>
-</span><span id="Git.make_public-201"><a href="#Git.make_public-201"><span class="linenos">201</span></a><span class="sd">        #### :params:</span>
-</span><span id="Git.make_public-202"><a href="#Git.make_public-202"><span class="linenos">202</span></a>
-</span><span id="Git.make_public-203"><a href="#Git.make_public-203"><span class="linenos">203</span></a><span class="sd">        `owner`: The repo owner.</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.make_public-202"><a href="#Git.make_public-202"><span class="linenos">202</span></a>    <span class="k">def</span> <span class="nf">make_public</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git.make_public-203"><a href="#Git.make_public-203"><span class="linenos">203</span></a>        <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be installed and configured) to set the repo&#39;s visibility to public.</span>
 </span><span id="Git.make_public-204"><a href="#Git.make_public-204"><span class="linenos">204</span></a>
-</span><span id="Git.make_public-205"><a href="#Git.make_public-205"><span class="linenos">205</span></a><span class="sd">        `name`: The name of the repo to edit.&quot;&quot;&quot;</span>
-</span><span id="Git.make_public-206"><a href="#Git.make_public-206"><span class="linenos">206</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_change_visibility</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">name</span><span class="p">,</span> <span class="s2">&quot;public&quot;</span><span class="p">)</span>
+</span><span id="Git.make_public-205"><a href="#Git.make_public-205"><span class="linenos">205</span></a><span class="sd">        #### :params:</span>
+</span><span id="Git.make_public-206"><a href="#Git.make_public-206"><span class="linenos">206</span></a>
+</span><span id="Git.make_public-207"><a href="#Git.make_public-207"><span class="linenos">207</span></a><span class="sd">        `owner`: The repo owner.</span>
+</span><span id="Git.make_public-208"><a href="#Git.make_public-208"><span class="linenos">208</span></a>
+</span><span id="Git.make_public-209"><a href="#Git.make_public-209"><span class="linenos">209</span></a><span class="sd">        `name`: The name of the repo to edit.&quot;&quot;&quot;</span>
+</span><span id="Git.make_public-210"><a href="#Git.make_public-210"><span class="linenos">210</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_change_visibility</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">name</span><span class="p">,</span> <span class="s2">&quot;public&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Uses GitHub CLI (must be installed and configured) to set the repo's visibility to public.</p>
 
 <h4 id="params">:params:</h4>
 
@@ -1353,23 +1369,23 @@
         <span class="def">def</span>
         <span class="name">delete_remote</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">owner</span><span class="p">:</span> <span class="nb">str</span>, </span><span class="param"><span class="n">name</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">) -> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span>:</span></span>
 
                 <label class="view-source-button" for="Git.delete_remote-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Git.delete_remote"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.delete_remote-208"><a href="#Git.delete_remote-208"><span class="linenos">208</span></a>    <span class="k">def</span> <span class="nf">delete_remote</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
-</span><span id="Git.delete_remote-209"><a href="#Git.delete_remote-209"><span class="linenos">209</span></a>        <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be isntalled and configured) to delete the remote for this repo.</span>
-</span><span id="Git.delete_remote-210"><a href="#Git.delete_remote-210"><span class="linenos">210</span></a>
-</span><span id="Git.delete_remote-211"><a href="#Git.delete_remote-211"><span class="linenos">211</span></a><span class="sd">        #### :params:</span>
-</span><span id="Git.delete_remote-212"><a href="#Git.delete_remote-212"><span class="linenos">212</span></a>
-</span><span id="Git.delete_remote-213"><a href="#Git.delete_remote-213"><span class="linenos">213</span></a><span class="sd">        `owner`: The repo owner.</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Git.delete_remote-212"><a href="#Git.delete_remote-212"><span class="linenos">212</span></a>    <span class="k">def</span> <span class="nf">delete_remote</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
+</span><span id="Git.delete_remote-213"><a href="#Git.delete_remote-213"><span class="linenos">213</span></a>        <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be isntalled and configured) to delete the remote for this repo.</span>
 </span><span id="Git.delete_remote-214"><a href="#Git.delete_remote-214"><span class="linenos">214</span></a>
-</span><span id="Git.delete_remote-215"><a href="#Git.delete_remote-215"><span class="linenos">215</span></a><span class="sd">        `name`: The name of the remote repo to delete.&quot;&quot;&quot;</span>
-</span><span id="Git.delete_remote-216"><a href="#Git.delete_remote-216"><span class="linenos">216</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_run</span><span class="p">([</span><span class="s2">&quot;gh&quot;</span><span class="p">,</span> <span class="s2">&quot;repo&quot;</span><span class="p">,</span> <span class="s2">&quot;delete&quot;</span><span class="p">,</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">owner</span><span class="si">}</span><span class="s2">/</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">,</span> <span class="s2">&quot;--yes&quot;</span><span class="p">])</span>
+</span><span id="Git.delete_remote-215"><a href="#Git.delete_remote-215"><span class="linenos">215</span></a><span class="sd">        #### :params:</span>
+</span><span id="Git.delete_remote-216"><a href="#Git.delete_remote-216"><span class="linenos">216</span></a>
+</span><span id="Git.delete_remote-217"><a href="#Git.delete_remote-217"><span class="linenos">217</span></a><span class="sd">        `owner`: The repo owner.</span>
+</span><span id="Git.delete_remote-218"><a href="#Git.delete_remote-218"><span class="linenos">218</span></a>
+</span><span id="Git.delete_remote-219"><a href="#Git.delete_remote-219"><span class="linenos">219</span></a><span class="sd">        `name`: The name of the remote repo to delete.&quot;&quot;&quot;</span>
+</span><span id="Git.delete_remote-220"><a href="#Git.delete_remote-220"><span class="linenos">220</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_run</span><span class="p">([</span><span class="s2">&quot;gh&quot;</span><span class="p">,</span> <span class="s2">&quot;repo&quot;</span><span class="p">,</span> <span class="s2">&quot;delete&quot;</span><span class="p">,</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">owner</span><span class="si">}</span><span class="s2">/</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">,</span> <span class="s2">&quot;--yes&quot;</span><span class="p">])</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Uses GitHub CLI (must be isntalled and configured) to delete the remote for this repo.</p>
 
 <h4 id="params">:params:</h4>
```

#### html2text {}

```diff
@@ -125,165 +125,170 @@
 _76        Equivalent to:
 _77        >>> git add {files}
 _78        >>> git commit --amend --no-edit
 _79        """
 _80        return self.add(files) + self.commit("--amend --no-edit")  # type:
 ignore
 _81
-_82    def tag(self, id_: str) -> str | int:
-_83        """Tag the current commit with `id_`.
+_82    def tag(self, args: str = "") -> str | int:
+_83        """Execute the `tag` command with `args`.
 _84
-_85        Equivalent to `git tag {id_}`."""
-_86        return self.execute(f"tag {id_}")
-_87
-_88    # ==========================================Push/
+_85        e.g.
+_86
+_87        `self.tag("--sort=-committerdate")`
+_88
+_89        will list all the tags for this repository in descending commit
+date."""
+_90        return self.execute(f"tag {args}")
+_91
+_92    # ==========================================Push/
 Pull==========================================
-_89    def add_remote_url(self, url: str, name: str = "origin") -> str | int:
-_90        """Add remote url to repo."""
-_91        return self.execute(f"remote add {name} {url}")
-_92
-_93    def push(self, args: str = "") -> str | int:
-_94        """Equivalent to `git push {args}`."""
-_95        return self.execute(f"push {args}")
+_93    def add_remote_url(self, url: str, name: str = "origin") -> str | int:
+_94        """Add remote url to repo."""
+_95        return self.execute(f"remote add {name} {url}")
 _96
-_97    def pull(self, args: str = "") -> str | int:
-_98        """Equivalent to `git pull {args}`."""
-_99        return self.execute(f"pull {args}")
+_97    def push(self, args: str = "") -> str | int:
+_98        """Equivalent to `git push {args}`."""
+_99        return self.execute(f"push {args}")
 100
-101    def push_new_branch(self, branch: str) -> str | int:
-102        """Push a new branch to origin with tracking.
-103
-104        Equivalent to `git push -u origin {branch}`."""
-105        return self.push(f"-u origin {branch}")
-106
-107    def pull_branch(self, branch: str) -> str | int:
-108        """Pull `branch` from origin."""
-109        return self.pull(f"origin {branch}")
+101    def pull(self, args: str = "") -> str | int:
+102        """Equivalent to `git pull {args}`."""
+103        return self.execute(f"pull {args}")
+104
+105    def push_new_branch(self, branch: str) -> str | int:
+106        """Push a new branch to origin with tracking.
+107
+108        Equivalent to `git push -u origin {branch}`."""
+109        return self.push(f"-u origin {branch}")
 110
-111    # ============================================Checkout/
+111    def pull_branch(self, branch: str) -> str | int:
+112        """Pull `branch` from origin."""
+113        return self.pull(f"origin {branch}")
+114
+115    # ============================================Checkout/
 Branches============================================
-112    def branch(self, args: str) -> str | int:
-113        """Equivalent to `git branch {args}`."""
-114        return self.execute(f"branch {args}")
-115
-116    def list_branches(self) -> str | int:
-117        """Print a list of branches."""
-118        return self.branch("-vva")
+116    def branch(self, args: str) -> str | int:
+117        """Equivalent to `git branch {args}`."""
+118        return self.execute(f"branch {args}")
 119
-120    def checkout(self, args: str) -> str | int:
-121        """Equivalent to `git checkout {args}`."""
-122        return self.execute(f"checkout {args}")
+120    def list_branches(self) -> str | int:
+121        """Print a list of branches."""
+122        return self.branch("-vva")
 123
-124    def switch_branch(self, branch_name: str) -> str | int:
-125        """Switch to the branch specified by `branch_name`.
-126
-127        Equivalent to `git checkout {branch_name}`."""
-128        return self.checkout(branch_name)
-129
-130    def create_new_branch(self, branch_name: str) -> str | int:
-131        """Create and switch to a new branch named with `branch_name`.
-132
-133        Equivalent to `git checkout -b {branch_name} --track`."""
-134        return self.checkout(f"-b {branch_name} --track")
-135
-136    def delete_branch(self, branch_name: str, local_only: bool = True) -
+124    def checkout(self, args: str) -> str | int:
+125        """Equivalent to `git checkout {args}`."""
+126        return self.execute(f"checkout {args}")
+127
+128    def switch_branch(self, branch_name: str) -> str | int:
+129        """Switch to the branch specified by `branch_name`.
+130
+131        Equivalent to `git checkout {branch_name}`."""
+132        return self.checkout(branch_name)
+133
+134    def create_new_branch(self, branch_name: str) -> str | int:
+135        """Create and switch to a new branch named with `branch_name`.
+136
+137        Equivalent to `git checkout -b {branch_name} --track`."""
+138        return self.checkout(f"-b {branch_name} --track")
+139
+140    def delete_branch(self, branch_name: str, local_only: bool = True) -
 > str | int:
-137        """Delete `branch_name` from repo.
-138
-139        #### :params:
-140
-141        `local_only`: Only delete the local copy of `branch`, otherwise also
+141        """Delete `branch_name` from repo.
+142
+143        #### :params:
+144
+145        `local_only`: Only delete the local copy of `branch`, otherwise also
 delete the remote branch on origin and remote-tracking branch."""
-142        output = self.branch(f"--delete {branch_name}")
-143        if not local_only:
-144            return output + self.push(f"origin --delete {branch_name}")  #
+146        output = self.branch(f"--delete {branch_name}")
+147        if not local_only:
+148            return output + self.push(f"origin --delete {branch_name}")  #
 type:ignore
-145        return output
-146
-147    def undo(self) -> str | int:
-148        """Undo uncommitted changes.
-149
-150        Equivalent to `git checkout .`."""
-151        return self.checkout(".")
-152
-153    def merge(self, branch_name: str) -> str | int:
-154        """Merge branch `branch_name` with currently active branch."""
-155        return self.execute(f"merge {branch_name}")
+149        return output
+150
+151    def undo(self) -> str | int:
+152        """Undo uncommitted changes.
+153
+154        Equivalent to `git checkout .`."""
+155        return self.checkout(".")
 156
-157    # ===============================Requires GitHub CLI to be installed and
+157    def merge(self, branch_name: str) -> str | int:
+158        """Merge branch `branch_name` with currently active branch."""
+159        return self.execute(f"merge {branch_name}")
+160
+161    # ===============================Requires GitHub CLI to be installed and
 configured===============================
-158
-159    def create_remote(self, name: str, public: bool = False) -> str | int:
-160        """Uses GitHub CLI (must be installed and configured) to create a
+162
+163    def create_remote(self, name: str, public: bool = False) -> str | int:
+164        """Uses GitHub CLI (must be installed and configured) to create a
 remote GitHub repo.
-161
-162        #### :params:
-163
-164        `name`: The name for the repo.
 165
-166        `public`: Set to `True` to create the repo as public, otherwise
-it'll be created as private."""
-167        visibility = "--public" if public else "--private"
-168        return self._run(["gh", "repo", "create", name, visibility])
+166        #### :params:
+167
+168        `name`: The name for the repo.
 169
-170    def create_remote_from_cwd(self, public: bool = False) -> str | int:
-171        """Use GitHub CLI (must be installed and configured) to create a
+170        `public`: Set to `True` to create the repo as public, otherwise
+it'll be created as private."""
+171        visibility = "--public" if public else "--private"
+172        return self._run(["gh", "repo", "create", name, visibility])
+173
+174    def create_remote_from_cwd(self, public: bool = False) -> str | int:
+175        """Use GitHub CLI (must be installed and configured) to create a
 remote GitHub repo from
-172        the current working directory repo and add its url as this repo's
+176        the current working directory repo and add its url as this repo's
 remote origin.
-173
-174        #### :params:
-175
-176        `public`: Create the GitHub repo as a public repo, default is to
+177
+178        #### :params:
+179
+180        `public`: Create the GitHub repo as a public repo, default is to
 create it as private."""
-177        visibility = "public" if public else "private"
-178        return self._run(
-179            ["gh", "repo", "create", "--source", ".", f"--{visibility}", "--
+181        visibility = "public" if public else "private"
+182        return self._run(
+183            ["gh", "repo", "create", "--source", ".", f"--{visibility}", "--
 push"]
-180        )
-181
-182    def _change_visibility(self, owner: str, name: str, visibility: str) -
+184        )
+185
+186    def _change_visibility(self, owner: str, name: str, visibility: str) -
 > str | int:
-183        return self._run(
-184            ["gh", "repo", "edit", f"{owner}/{name}", "--visibility",
+187        return self._run(
+188            ["gh", "repo", "edit", f"{owner}/{name}", "--visibility",
 visibility]
-185        )
-186
-187    def make_private(self, owner: str, name: str) -> str | int:
-188        """Uses GitHub CLI (must be installed and configured) to set the
+189        )
+190
+191    def make_private(self, owner: str, name: str) -> str | int:
+192        """Uses GitHub CLI (must be installed and configured) to set the
 repo's visibility to private.
-189
-190        #### :params:
-191
-192        `owner`: The repo owner.
 193
-194        `name`: The name of the repo to edit."""
-195        return self._change_visibility(owner, name, "private")
-196
-197    def make_public(self, owner: str, name: str) -> str | int:
-198        """Uses GitHub CLI (must be installed and configured) to set the
+194        #### :params:
+195
+196        `owner`: The repo owner.
+197
+198        `name`: The name of the repo to edit."""
+199        return self._change_visibility(owner, name, "private")
+200
+201    def make_public(self, owner: str, name: str) -> str | int:
+202        """Uses GitHub CLI (must be installed and configured) to set the
 repo's visibility to public.
-199
-200        #### :params:
-201
-202        `owner`: The repo owner.
 203
-204        `name`: The name of the repo to edit."""
-205        return self._change_visibility(owner, name, "public")
-206
-207    def delete_remote(self, owner: str, name: str) -> str | int:
-208        """Uses GitHub CLI (must be isntalled and configured) to delete the
+204        #### :params:
+205
+206        `owner`: The repo owner.
+207
+208        `name`: The name of the repo to edit."""
+209        return self._change_visibility(owner, name, "public")
+210
+211    def delete_remote(self, owner: str, name: str) -> str | int:
+212        """Uses GitHub CLI (must be isntalled and configured) to delete the
 remote for this repo.
-209
-210        #### :params:
-211
-212        `owner`: The repo owner.
 213
-214        `name`: The name of the remote repo to delete."""
-215        return self._run(["gh", "repo", "delete", f"{owner}/{name}", "--
+214        #### :params:
+215
+216        `owner`: The repo owner.
+217
+218        `name`: The name of the remote repo to delete."""
+219        return self._run(["gh", "repo", "delete", f"{owner}/{name}", "--
 yes"])
   ⁰
 class Git: View Source
 __6class Git:
 __7    def __init__(self, capture_stdout: bool = False):
 __8        """If `capture_stdout` is `True`, all functions will return their
 generated `stdout` as a string.
@@ -366,165 +371,170 @@
 _77        Equivalent to:
 _78        >>> git add {files}
 _79        >>> git commit --amend --no-edit
 _80        """
 _81        return self.add(files) + self.commit("--amend --no-edit")  # type:
 ignore
 _82
-_83    def tag(self, id_: str) -> str | int:
-_84        """Tag the current commit with `id_`.
+_83    def tag(self, args: str = "") -> str | int:
+_84        """Execute the `tag` command with `args`.
 _85
-_86        Equivalent to `git tag {id_}`."""
-_87        return self.execute(f"tag {id_}")
-_88
-_89    # ==========================================Push/
+_86        e.g.
+_87
+_88        `self.tag("--sort=-committerdate")`
+_89
+_90        will list all the tags for this repository in descending commit
+date."""
+_91        return self.execute(f"tag {args}")
+_92
+_93    # ==========================================Push/
 Pull==========================================
-_90    def add_remote_url(self, url: str, name: str = "origin") -> str | int:
-_91        """Add remote url to repo."""
-_92        return self.execute(f"remote add {name} {url}")
-_93
-_94    def push(self, args: str = "") -> str | int:
-_95        """Equivalent to `git push {args}`."""
-_96        return self.execute(f"push {args}")
+_94    def add_remote_url(self, url: str, name: str = "origin") -> str | int:
+_95        """Add remote url to repo."""
+_96        return self.execute(f"remote add {name} {url}")
 _97
-_98    def pull(self, args: str = "") -> str | int:
-_99        """Equivalent to `git pull {args}`."""
-100        return self.execute(f"pull {args}")
+_98    def push(self, args: str = "") -> str | int:
+_99        """Equivalent to `git push {args}`."""
+100        return self.execute(f"push {args}")
 101
-102    def push_new_branch(self, branch: str) -> str | int:
-103        """Push a new branch to origin with tracking.
-104
-105        Equivalent to `git push -u origin {branch}`."""
-106        return self.push(f"-u origin {branch}")
-107
-108    def pull_branch(self, branch: str) -> str | int:
-109        """Pull `branch` from origin."""
-110        return self.pull(f"origin {branch}")
+102    def pull(self, args: str = "") -> str | int:
+103        """Equivalent to `git pull {args}`."""
+104        return self.execute(f"pull {args}")
+105
+106    def push_new_branch(self, branch: str) -> str | int:
+107        """Push a new branch to origin with tracking.
+108
+109        Equivalent to `git push -u origin {branch}`."""
+110        return self.push(f"-u origin {branch}")
 111
-112    # ============================================Checkout/
+112    def pull_branch(self, branch: str) -> str | int:
+113        """Pull `branch` from origin."""
+114        return self.pull(f"origin {branch}")
+115
+116    # ============================================Checkout/
 Branches============================================
-113    def branch(self, args: str) -> str | int:
-114        """Equivalent to `git branch {args}`."""
-115        return self.execute(f"branch {args}")
-116
-117    def list_branches(self) -> str | int:
-118        """Print a list of branches."""
-119        return self.branch("-vva")
+117    def branch(self, args: str) -> str | int:
+118        """Equivalent to `git branch {args}`."""
+119        return self.execute(f"branch {args}")
 120
-121    def checkout(self, args: str) -> str | int:
-122        """Equivalent to `git checkout {args}`."""
-123        return self.execute(f"checkout {args}")
+121    def list_branches(self) -> str | int:
+122        """Print a list of branches."""
+123        return self.branch("-vva")
 124
-125    def switch_branch(self, branch_name: str) -> str | int:
-126        """Switch to the branch specified by `branch_name`.
-127
-128        Equivalent to `git checkout {branch_name}`."""
-129        return self.checkout(branch_name)
-130
-131    def create_new_branch(self, branch_name: str) -> str | int:
-132        """Create and switch to a new branch named with `branch_name`.
-133
-134        Equivalent to `git checkout -b {branch_name} --track`."""
-135        return self.checkout(f"-b {branch_name} --track")
-136
-137    def delete_branch(self, branch_name: str, local_only: bool = True) -
+125    def checkout(self, args: str) -> str | int:
+126        """Equivalent to `git checkout {args}`."""
+127        return self.execute(f"checkout {args}")
+128
+129    def switch_branch(self, branch_name: str) -> str | int:
+130        """Switch to the branch specified by `branch_name`.
+131
+132        Equivalent to `git checkout {branch_name}`."""
+133        return self.checkout(branch_name)
+134
+135    def create_new_branch(self, branch_name: str) -> str | int:
+136        """Create and switch to a new branch named with `branch_name`.
+137
+138        Equivalent to `git checkout -b {branch_name} --track`."""
+139        return self.checkout(f"-b {branch_name} --track")
+140
+141    def delete_branch(self, branch_name: str, local_only: bool = True) -
 > str | int:
-138        """Delete `branch_name` from repo.
-139
-140        #### :params:
-141
-142        `local_only`: Only delete the local copy of `branch`, otherwise also
+142        """Delete `branch_name` from repo.
+143
+144        #### :params:
+145
+146        `local_only`: Only delete the local copy of `branch`, otherwise also
 delete the remote branch on origin and remote-tracking branch."""
-143        output = self.branch(f"--delete {branch_name}")
-144        if not local_only:
-145            return output + self.push(f"origin --delete {branch_name}")  #
+147        output = self.branch(f"--delete {branch_name}")
+148        if not local_only:
+149            return output + self.push(f"origin --delete {branch_name}")  #
 type:ignore
-146        return output
-147
-148    def undo(self) -> str | int:
-149        """Undo uncommitted changes.
-150
-151        Equivalent to `git checkout .`."""
-152        return self.checkout(".")
-153
-154    def merge(self, branch_name: str) -> str | int:
-155        """Merge branch `branch_name` with currently active branch."""
-156        return self.execute(f"merge {branch_name}")
+150        return output
+151
+152    def undo(self) -> str | int:
+153        """Undo uncommitted changes.
+154
+155        Equivalent to `git checkout .`."""
+156        return self.checkout(".")
 157
-158    # ===============================Requires GitHub CLI to be installed and
+158    def merge(self, branch_name: str) -> str | int:
+159        """Merge branch `branch_name` with currently active branch."""
+160        return self.execute(f"merge {branch_name}")
+161
+162    # ===============================Requires GitHub CLI to be installed and
 configured===============================
-159
-160    def create_remote(self, name: str, public: bool = False) -> str | int:
-161        """Uses GitHub CLI (must be installed and configured) to create a
+163
+164    def create_remote(self, name: str, public: bool = False) -> str | int:
+165        """Uses GitHub CLI (must be installed and configured) to create a
 remote GitHub repo.
-162
-163        #### :params:
-164
-165        `name`: The name for the repo.
 166
-167        `public`: Set to `True` to create the repo as public, otherwise
-it'll be created as private."""
-168        visibility = "--public" if public else "--private"
-169        return self._run(["gh", "repo", "create", name, visibility])
+167        #### :params:
+168
+169        `name`: The name for the repo.
 170
-171    def create_remote_from_cwd(self, public: bool = False) -> str | int:
-172        """Use GitHub CLI (must be installed and configured) to create a
+171        `public`: Set to `True` to create the repo as public, otherwise
+it'll be created as private."""
+172        visibility = "--public" if public else "--private"
+173        return self._run(["gh", "repo", "create", name, visibility])
+174
+175    def create_remote_from_cwd(self, public: bool = False) -> str | int:
+176        """Use GitHub CLI (must be installed and configured) to create a
 remote GitHub repo from
-173        the current working directory repo and add its url as this repo's
+177        the current working directory repo and add its url as this repo's
 remote origin.
-174
-175        #### :params:
-176
-177        `public`: Create the GitHub repo as a public repo, default is to
+178
+179        #### :params:
+180
+181        `public`: Create the GitHub repo as a public repo, default is to
 create it as private."""
-178        visibility = "public" if public else "private"
-179        return self._run(
-180            ["gh", "repo", "create", "--source", ".", f"--{visibility}", "--
+182        visibility = "public" if public else "private"
+183        return self._run(
+184            ["gh", "repo", "create", "--source", ".", f"--{visibility}", "--
 push"]
-181        )
-182
-183    def _change_visibility(self, owner: str, name: str, visibility: str) -
+185        )
+186
+187    def _change_visibility(self, owner: str, name: str, visibility: str) -
 > str | int:
-184        return self._run(
-185            ["gh", "repo", "edit", f"{owner}/{name}", "--visibility",
+188        return self._run(
+189            ["gh", "repo", "edit", f"{owner}/{name}", "--visibility",
 visibility]
-186        )
-187
-188    def make_private(self, owner: str, name: str) -> str | int:
-189        """Uses GitHub CLI (must be installed and configured) to set the
+190        )
+191
+192    def make_private(self, owner: str, name: str) -> str | int:
+193        """Uses GitHub CLI (must be installed and configured) to set the
 repo's visibility to private.
-190
-191        #### :params:
-192
-193        `owner`: The repo owner.
 194
-195        `name`: The name of the repo to edit."""
-196        return self._change_visibility(owner, name, "private")
-197
-198    def make_public(self, owner: str, name: str) -> str | int:
-199        """Uses GitHub CLI (must be installed and configured) to set the
+195        #### :params:
+196
+197        `owner`: The repo owner.
+198
+199        `name`: The name of the repo to edit."""
+200        return self._change_visibility(owner, name, "private")
+201
+202    def make_public(self, owner: str, name: str) -> str | int:
+203        """Uses GitHub CLI (must be installed and configured) to set the
 repo's visibility to public.
-200
-201        #### :params:
-202
-203        `owner`: The repo owner.
 204
-205        `name`: The name of the repo to edit."""
-206        return self._change_visibility(owner, name, "public")
-207
-208    def delete_remote(self, owner: str, name: str) -> str | int:
-209        """Uses GitHub CLI (must be isntalled and configured) to delete the
+205        #### :params:
+206
+207        `owner`: The repo owner.
+208
+209        `name`: The name of the repo to edit."""
+210        return self._change_visibility(owner, name, "public")
+211
+212    def delete_remote(self, owner: str, name: str) -> str | int:
+213        """Uses GitHub CLI (must be isntalled and configured) to delete the
 remote for this repo.
-210
-211        #### :params:
-212
-213        `owner`: The repo owner.
 214
-215        `name`: The name of the remote repo to delete."""
-216        return self._run(["gh", "repo", "delete", f"{owner}/{name}", "--
+215        #### :params:
+216
+217        `owner`: The repo owner.
+218
+219        `name`: The name of the remote repo to delete."""
+220        return self._run(["gh", "repo", "delete", f"{owner}/{name}", "--
 yes"])
 ⁰
 Git(capture_stdout: bool = False) View Source
 _7    def __init__(self, capture_stdout: bool = False):
 _8        """If `capture_stdout` is `True`, all functions will return their
 generated `stdout` as a string.
 _9        Otherwise, the functions return the call's exit code."""
@@ -617,218 +627,225 @@
 ignore
 Stage and commit changes to the previous commit.
 If files is None, all files will be staged.
 Equivalent to:
 >>> git add {files}
 >>> git commit --amend --no-edit
 ⁰
-def tag(self, id_: str) -> str | int: View Source
-83    def tag(self, id_: str) -> str | int:
-84        """Tag the current commit with `id_`.
+def tag(self, args: str = '') -> str | int: View Source
+83    def tag(self, args: str = "") -> str | int:
+84        """Execute the `tag` command with `args`.
 85
-86        Equivalent to `git tag {id_}`."""
-87        return self.execute(f"tag {id_}")
-Tag the current commit with id_.
-Equivalent to git tag {id_}.
+86        e.g.
+87
+88        `self.tag("--sort=-committerdate")`
+89
+90        will list all the tags for this repository in descending commit
+date."""
+91        return self.execute(f"tag {args}")
+Execute the tag command with args.
+e.g.
+self.tag("--sort=-committerdate")
+will list all the tags for this repository in descending commit date.
 ⁰
 def add_remote_url(self, url: str, name: str = 'origin') -> str | int: View
 Source
-90    def add_remote_url(self, url: str, name: str = "origin") -> str | int:
-91        """Add remote url to repo."""
-92        return self.execute(f"remote add {name} {url}")
+94    def add_remote_url(self, url: str, name: str = "origin") -> str | int:
+95        """Add remote url to repo."""
+96        return self.execute(f"remote add {name} {url}")
 Add remote url to repo.
 ⁰
 def push(self, args: str = '') -> str | int: View Source
-94    def push(self, args: str = "") -> str | int:
-95        """Equivalent to `git push {args}`."""
-96        return self.execute(f"push {args}")
+_98    def push(self, args: str = "") -> str | int:
+_99        """Equivalent to `git push {args}`."""
+100        return self.execute(f"push {args}")
 Equivalent to git push {args}.
 ⁰
 def pull(self, args: str = '') -> str | int: View Source
-_98    def pull(self, args: str = "") -> str | int:
-_99        """Equivalent to `git pull {args}`."""
-100        return self.execute(f"pull {args}")
+102    def pull(self, args: str = "") -> str | int:
+103        """Equivalent to `git pull {args}`."""
+104        return self.execute(f"pull {args}")
 Equivalent to git pull {args}.
 ⁰
 def push_new_branch(self, branch: str) -> str | int: View Source
-102    def push_new_branch(self, branch: str) -> str | int:
-103        """Push a new branch to origin with tracking.
-104
-105        Equivalent to `git push -u origin {branch}`."""
-106        return self.push(f"-u origin {branch}")
+106    def push_new_branch(self, branch: str) -> str | int:
+107        """Push a new branch to origin with tracking.
+108
+109        Equivalent to `git push -u origin {branch}`."""
+110        return self.push(f"-u origin {branch}")
 Push a new branch to origin with tracking.
 Equivalent to git push -u origin {branch}.
 ⁰
 def pull_branch(self, branch: str) -> str | int: View Source
-108    def pull_branch(self, branch: str) -> str | int:
-109        """Pull `branch` from origin."""
-110        return self.pull(f"origin {branch}")
+112    def pull_branch(self, branch: str) -> str | int:
+113        """Pull `branch` from origin."""
+114        return self.pull(f"origin {branch}")
 Pull branch from origin.
 ⁰
 def branch(self, args: str) -> str | int: View Source
-113    def branch(self, args: str) -> str | int:
-114        """Equivalent to `git branch {args}`."""
-115        return self.execute(f"branch {args}")
+117    def branch(self, args: str) -> str | int:
+118        """Equivalent to `git branch {args}`."""
+119        return self.execute(f"branch {args}")
 Equivalent to git branch {args}.
 ⁰
 def list_branches(self) -> str | int: View Source
-117    def list_branches(self) -> str | int:
-118        """Print a list of branches."""
-119        return self.branch("-vva")
+121    def list_branches(self) -> str | int:
+122        """Print a list of branches."""
+123        return self.branch("-vva")
 Print a list of branches.
 ⁰
 def checkout(self, args: str) -> str | int: View Source
-121    def checkout(self, args: str) -> str | int:
-122        """Equivalent to `git checkout {args}`."""
-123        return self.execute(f"checkout {args}")
+125    def checkout(self, args: str) -> str | int:
+126        """Equivalent to `git checkout {args}`."""
+127        return self.execute(f"checkout {args}")
 Equivalent to git checkout {args}.
 ⁰
 def switch_branch(self, branch_name: str) -> str | int: View Source
-125    def switch_branch(self, branch_name: str) -> str | int:
-126        """Switch to the branch specified by `branch_name`.
-127
-128        Equivalent to `git checkout {branch_name}`."""
-129        return self.checkout(branch_name)
+129    def switch_branch(self, branch_name: str) -> str | int:
+130        """Switch to the branch specified by `branch_name`.
+131
+132        Equivalent to `git checkout {branch_name}`."""
+133        return self.checkout(branch_name)
 Switch to the branch specified by branch_name.
 Equivalent to git checkout {branch_name}.
 ⁰
 def create_new_branch(self, branch_name: str) -> str | int: View Source
-131    def create_new_branch(self, branch_name: str) -> str | int:
-132        """Create and switch to a new branch named with `branch_name`.
-133
-134        Equivalent to `git checkout -b {branch_name} --track`."""
-135        return self.checkout(f"-b {branch_name} --track")
+135    def create_new_branch(self, branch_name: str) -> str | int:
+136        """Create and switch to a new branch named with `branch_name`.
+137
+138        Equivalent to `git checkout -b {branch_name} --track`."""
+139        return self.checkout(f"-b {branch_name} --track")
 Create and switch to a new branch named with branch_name.
 Equivalent to git checkout -b {branch_name} --track.
 ⁰
 def delete_branch(self, branch_name: str, local_only: bool = True) -> str |
 int: View Source
-137    def delete_branch(self, branch_name: str, local_only: bool = True) -
+141    def delete_branch(self, branch_name: str, local_only: bool = True) -
 > str | int:
-138        """Delete `branch_name` from repo.
-139
-140        #### :params:
-141
-142        `local_only`: Only delete the local copy of `branch`, otherwise also
+142        """Delete `branch_name` from repo.
+143
+144        #### :params:
+145
+146        `local_only`: Only delete the local copy of `branch`, otherwise also
 delete the remote branch on origin and remote-tracking branch."""
-143        output = self.branch(f"--delete {branch_name}")
-144        if not local_only:
-145            return output + self.push(f"origin --delete {branch_name}")  #
+147        output = self.branch(f"--delete {branch_name}")
+148        if not local_only:
+149            return output + self.push(f"origin --delete {branch_name}")  #
 type:ignore
-146        return output
+150        return output
 Delete branch_name from repo.
 *** :params: ***
 local_only: Only delete the local copy of branch, otherwise also delete the
 remote branch on origin and remote-tracking branch.
 ⁰
 def undo(self) -> str | int: View Source
-148    def undo(self) -> str | int:
-149        """Undo uncommitted changes.
-150
-151        Equivalent to `git checkout .`."""
-152        return self.checkout(".")
+152    def undo(self) -> str | int:
+153        """Undo uncommitted changes.
+154
+155        Equivalent to `git checkout .`."""
+156        return self.checkout(".")
 Undo uncommitted changes.
 Equivalent to git checkout ..
 ⁰
 def merge(self, branch_name: str) -> str | int: View Source
-154    def merge(self, branch_name: str) -> str | int:
-155        """Merge branch `branch_name` with currently active branch."""
-156        return self.execute(f"merge {branch_name}")
+158    def merge(self, branch_name: str) -> str | int:
+159        """Merge branch `branch_name` with currently active branch."""
+160        return self.execute(f"merge {branch_name}")
 Merge branch branch_name with currently active branch.
 ⁰
 def create_remote(self, name: str, public: bool = False) -> str | int: View
 Source
-160    def create_remote(self, name: str, public: bool = False) -> str | int:
-161        """Uses GitHub CLI (must be installed and configured) to create a
+164    def create_remote(self, name: str, public: bool = False) -> str | int:
+165        """Uses GitHub CLI (must be installed and configured) to create a
 remote GitHub repo.
-162
-163        #### :params:
-164
-165        `name`: The name for the repo.
 166
-167        `public`: Set to `True` to create the repo as public, otherwise
+167        #### :params:
+168
+169        `name`: The name for the repo.
+170
+171        `public`: Set to `True` to create the repo as public, otherwise
 it'll be created as private."""
-168        visibility = "--public" if public else "--private"
-169        return self._run(["gh", "repo", "create", name, visibility])
+172        visibility = "--public" if public else "--private"
+173        return self._run(["gh", "repo", "create", name, visibility])
 Uses GitHub CLI (must be installed and configured) to create a remote GitHub
 repo.
 *** :params: ***
 name: The name for the repo.
 public: Set to True to create the repo as public, otherwise it'll be created as
 private.
 ⁰
 def create_remote_from_cwd(self, public: bool = False) -> str | int: View
 Source
-171    def create_remote_from_cwd(self, public: bool = False) -> str | int:
-172        """Use GitHub CLI (must be installed and configured) to create a
+175    def create_remote_from_cwd(self, public: bool = False) -> str | int:
+176        """Use GitHub CLI (must be installed and configured) to create a
 remote GitHub repo from
-173        the current working directory repo and add its url as this repo's
+177        the current working directory repo and add its url as this repo's
 remote origin.
-174
-175        #### :params:
-176
-177        `public`: Create the GitHub repo as a public repo, default is to
+178
+179        #### :params:
+180
+181        `public`: Create the GitHub repo as a public repo, default is to
 create it as private."""
-178        visibility = "public" if public else "private"
-179        return self._run(
-180            ["gh", "repo", "create", "--source", ".", f"--{visibility}", "--
+182        visibility = "public" if public else "private"
+183        return self._run(
+184            ["gh", "repo", "create", "--source", ".", f"--{visibility}", "--
 push"]
-181        )
+185        )
 Use GitHub CLI (must be installed and configured) to create a remote GitHub
 repo from the current working directory repo and add its url as this repo's
 remote origin.
 *** :params: ***
 public: Create the GitHub repo as a public repo, default is to create it as
 private.
 ⁰
 def make_private(self, owner: str, name: str) -> str | int: View Source
-188    def make_private(self, owner: str, name: str) -> str | int:
-189        """Uses GitHub CLI (must be installed and configured) to set the
+192    def make_private(self, owner: str, name: str) -> str | int:
+193        """Uses GitHub CLI (must be installed and configured) to set the
 repo's visibility to private.
-190
-191        #### :params:
-192
-193        `owner`: The repo owner.
 194
-195        `name`: The name of the repo to edit."""
-196        return self._change_visibility(owner, name, "private")
+195        #### :params:
+196
+197        `owner`: The repo owner.
+198
+199        `name`: The name of the repo to edit."""
+200        return self._change_visibility(owner, name, "private")
 Uses GitHub CLI (must be installed and configured) to set the repo's visibility
 to private.
 *** :params: ***
 owner: The repo owner.
 name: The name of the repo to edit.
 ⁰
 def make_public(self, owner: str, name: str) -> str | int: View Source
-198    def make_public(self, owner: str, name: str) -> str | int:
-199        """Uses GitHub CLI (must be installed and configured) to set the
+202    def make_public(self, owner: str, name: str) -> str | int:
+203        """Uses GitHub CLI (must be installed and configured) to set the
 repo's visibility to public.
-200
-201        #### :params:
-202
-203        `owner`: The repo owner.
 204
-205        `name`: The name of the repo to edit."""
-206        return self._change_visibility(owner, name, "public")
+205        #### :params:
+206
+207        `owner`: The repo owner.
+208
+209        `name`: The name of the repo to edit."""
+210        return self._change_visibility(owner, name, "public")
 Uses GitHub CLI (must be installed and configured) to set the repo's visibility
 to public.
 *** :params: ***
 owner: The repo owner.
 name: The name of the repo to edit.
 ⁰
 def delete_remote(self, owner: str, name: str) -> str | int: View Source
-208    def delete_remote(self, owner: str, name: str) -> str | int:
-209        """Uses GitHub CLI (must be isntalled and configured) to delete the
+212    def delete_remote(self, owner: str, name: str) -> str | int:
+213        """Uses GitHub CLI (must be isntalled and configured) to delete the
 remote for this repo.
-210
-211        #### :params:
-212
-213        `owner`: The repo owner.
 214
-215        `name`: The name of the remote repo to delete."""
-216        return self._run(["gh", "repo", "delete", f"{owner}/{name}", "--
+215        #### :params:
+216
+217        `owner`: The repo owner.
+218
+219        `name`: The name of the remote repo to delete."""
+220        return self._run(["gh", "repo", "delete", f"{owner}/{name}", "--
 yes"])
 Uses GitHub CLI (must be isntalled and configured) to delete the remote for
 this repo.
 *** :params: ***
 owner: The repo owner.
 name: The name of the remote repo to delete.
```

### Comparing `gitbetter-1.0.0/docs/gitbetter/gitbetter.html` & `gitbetter-1.1.0/docs/gitbetter/gitbetter.html`

 * *Files identical despite different names*

### Comparing `gitbetter-1.0.0/src/gitbetter/git.py` & `gitbetter-1.1.0/src/gitbetter/git.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,19 +75,23 @@
 
         Equivalent to:
         >>> git add {files}
         >>> git commit --amend --no-edit
         """
         return self.add(files) + self.commit("--amend --no-edit")  # type: ignore
 
-    def tag(self, id_: str) -> str | int:
-        """Tag the current commit with `id_`.
+    def tag(self, args: str = "") -> str | int:
+        """Execute the `tag` command with `args`.
 
-        Equivalent to `git tag {id_}`."""
-        return self.execute(f"tag {id_}")
+        e.g.
+
+        `self.tag("--sort=-committerdate")`
+
+        will list all the tags for this repository in descending commit date."""
+        return self.execute(f"tag {args}")
 
     # ==========================================Push/Pull==========================================
     def add_remote_url(self, url: str, name: str = "origin") -> str | int:
         """Add remote url to repo."""
         return self.execute(f"remote add {name} {url}")
 
     def push(self, args: str = "") -> str | int:
```

### Comparing `gitbetter-1.0.0/src/gitbetter/gitbetter.py` & `gitbetter-1.1.0/src/gitbetter/gitbetter.py`

 * *Files identical despite different names*

### Comparing `gitbetter-1.0.0/LICENSE.txt` & `gitbetter-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gitbetter-1.0.0/README.md` & `gitbetter-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `gitbetter-1.0.0/pyproject.toml` & `gitbetter-1.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 00000040: 6c69 6e67 2e62 7569 6c64 220d 0a0d 0a5b  ling.build"....[
 00000050: 7072 6f6a 6563 745d 0d0a 6e61 6d65 203d  project]..name =
 00000060: 2022 6769 7462 6574 7465 7222 0d0a 6465   "gitbetter"..de
 00000070: 7363 7269 7074 696f 6e20 3d20 2243 7573  scription = "Cus
 00000080: 746f 6d20 6769 7420 7368 656c 6c20 746f  tom git shell to
 00000090: 2074 7970 6520 6c65 7373 2061 6e64 2063   type less and c
 000000a0: 6f6d 6d69 7420 6d6f 7265 2e22 0d0a 7665  ommit more."..ve
-000000b0: 7273 696f 6e20 3d20 2231 2e30 2e30 220d  rsion = "1.0.0".
+000000b0: 7273 696f 6e20 3d20 2231 2e31 2e30 220d  rsion = "1.1.0".
 000000c0: 0a72 6571 7569 7265 732d 7079 7468 6f6e  .requires-python
 000000d0: 203d 2022 3e3d 332e 3130 220d 0a64 6570   = ">=3.10"..dep
 000000e0: 656e 6465 6e63 6965 7320 3d20 5b22 6172  endencies = ["ar
 000000f0: 6773 6865 6c6c 222c 2022 7061 7468 6965  gshell", "pathie
 00000100: 7222 2c20 2270 7974 6573 7422 5d0d 0a72  r", "pytest"]..r
 00000110: 6561 646d 6520 3d20 2252 4541 444d 452e  eadme = "README.
 00000120: 6d64 220d 0a6b 6579 776f 7264 7320 3d20  md"..keywords =
```

### Comparing `gitbetter-1.0.0/PKG-INFO` & `gitbetter-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitbetter
-Version: 1.0.0
+Version: 1.1.0
 Summary: Custom git shell to type less and commit more.
 Project-URL: Homepage, https://github.com/matt-manes/gitbetter
 Project-URL: Documentation, https://github.com/matt-manes/gitbetter/tree/main/docs
 Project-URL: Source code, https://github.com/matt-manes/gitbetter/tree/main/src/gitbetter
 Author-email: Matt Manes <mattmanes@pm.me>
 License-File: LICENSE.txt
 Keywords: cli,commit,git,shell,terminal
```

