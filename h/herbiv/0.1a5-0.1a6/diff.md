# Comparing `tmp/herbiv-0.1a5.tar.gz` & `tmp/herbiv-0.1a6.tar.gz`

## Comparing `herbiv-0.1a5.tar` & `herbiv-0.1a6.tar`

### file list

```diff
@@ -1,16 +1,32 @@
--rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 herbiv-0.1a5/setup.py
--rw-r--r--   0        0        0     8202 2020-02-02 00:00:00.000000 herbiv-0.1a5/src/herbiv/analysis.py
--rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 herbiv-0.1a5/src/herbiv/compute.py
--rw-r--r--   0        0        0     5423 2020-02-02 00:00:00.000000 herbiv-0.1a5/src/herbiv/get.py
--rw-r--r--   0        0        0     3548 2020-02-02 00:00:00.000000 herbiv-0.1a5/src/herbiv/output.py
--rw-r--r--   0        0        0 13073523 2020-02-02 00:00:00.000000 herbiv-0.1a5/src/herbiv/data/HerbiV_chemical_protein_links.csv
--rw-r--r--   0        0        0  1377866 2020-02-02 00:00:00.000000 herbiv-0.1a5/src/herbiv/data/HerbiV_chemicals.csv
--rw-r--r--   0        0        0  1978068 2020-02-02 00:00:00.000000 herbiv-0.1a5/src/herbiv/data/HerbiV_proteins.csv
--rw-r--r--   0        0        0  1227198 2020-02-02 00:00:00.000000 herbiv-0.1a5/src/herbiv/data/HerbiV_tcm.csv
--rw-r--r--   0        0        0  1029771 2020-02-02 00:00:00.000000 herbiv-0.1a5/src/herbiv/data/HerbiV_tcm_chemical_links.csv
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 herbiv-0.1a5/src/herbiv/result/Network.csv
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 herbiv-0.1a5/src/herbiv/result/Type.csv
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 herbiv-0.1a5/LICENSE
--rw-r--r--   0        0        0    11814 2020-02-02 00:00:00.000000 herbiv-0.1a5/README.md
--rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 herbiv-0.1a5/pyproject.toml
--rw-r--r--   0        0        0    12767 2020-02-02 00:00:00.000000 herbiv-0.1a5/PKG-INFO
+-rw-r--r--   0        0        0    61580 2020-02-02 00:00:00.000000 herbiv-0.1a6/demo.ipynb
+-rw-r--r--   0        0        0    23588 2020-02-02 00:00:00.000000 herbiv-0.1a6/logo.png
+-rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 herbiv-0.1a6/setup.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 herbiv-0.1a6/.idea/.gitignore
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 herbiv-0.1a6/.idea/HerbiV.iml
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 herbiv-0.1a6/.idea/csv-editor.xml
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 herbiv-0.1a6/.idea/misc.xml
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 herbiv-0.1a6/.idea/modules.xml
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 herbiv-0.1a6/.idea/vcs.xml
+-rw-r--r--   0        0        0    17647 2020-02-02 00:00:00.000000 herbiv-0.1a6/.idea/workspace.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 herbiv-0.1a6/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 herbiv-0.1a6/.idea/shelf/_2023_5_27_20_12____.xml
+-rw-r--r--   0        0        0   181921 2020-02-02 00:00:00.000000 herbiv-0.1a6/.idea/shelf/在进行更新之前于_2023_5_27_20_12_取消提交了更改_[更改]/shelved.patch
+-rw-r--r--   0        0        0    85738 2020-02-02 00:00:00.000000 herbiv-0.1a6/.ipynb_checkpoints/demo-checkpoint.ipynb
+-rw-r--r--   0        0        0    10849 2020-02-02 00:00:00.000000 herbiv-0.1a6/herbiv/analysis.py
+-rw-r--r--   0        0        0     7820 2020-02-02 00:00:00.000000 herbiv-0.1a6/herbiv/compute.py
+-rw-r--r--   0        0        0     7310 2020-02-02 00:00:00.000000 herbiv-0.1a6/herbiv/get.py
+-rw-r--r--   0        0        0     5766 2020-02-02 00:00:00.000000 herbiv-0.1a6/herbiv/output.py
+-rw-r--r--   0        0        0 13073523 2020-02-02 00:00:00.000000 herbiv-0.1a6/herbiv/data/HerbiV_chemical_protein_links.csv
+-rw-r--r--   0        0        0  1377866 2020-02-02 00:00:00.000000 herbiv-0.1a6/herbiv/data/HerbiV_chemicals.csv
+-rw-r--r--   0        0        0  1803372 2020-02-02 00:00:00.000000 herbiv-0.1a6/herbiv/data/HerbiV_formula.csv
+-rw-r--r--   0        0        0   481317 2020-02-02 00:00:00.000000 herbiv-0.1a6/herbiv/data/HerbiV_formula_tcm_links.csv
+-rw-r--r--   0        0        0  1978064 2020-02-02 00:00:00.000000 herbiv-0.1a6/herbiv/data/HerbiV_proteins.csv
+-rw-r--r--   0        0        0  1227198 2020-02-02 00:00:00.000000 herbiv-0.1a6/herbiv/data/HerbiV_tcm.csv
+-rw-r--r--   0        0        0  1029771 2020-02-02 00:00:00.000000 herbiv-0.1a6/herbiv/data/HerbiV_tcm_chemical_links.csv
+-rw-r--r--   0        0        0    15258 2020-02-02 00:00:00.000000 herbiv-0.1a6/herbiv/result/Graph.html
+-rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 herbiv-0.1a6/herbiv/result/Network.csv
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 herbiv-0.1a6/herbiv/result/Type.csv
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 herbiv-0.1a6/LICENSE
+-rw-r--r--   0        0        0    12056 2020-02-02 00:00:00.000000 herbiv-0.1a6/README.md
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 herbiv-0.1a6/pyproject.toml
+-rw-r--r--   0        0        0    13005 2020-02-02 00:00:00.000000 herbiv-0.1a6/PKG-INFO
```

### Comparing `herbiv-0.1a5/setup.py` & `herbiv-0.1a6/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 here = pathlib.Path(__file__).parent.resolve()
 
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="herbiv",
-    version="0.1a5",
+    version="0.1a6",
     description="HerbiV是一个具有多种功能的中药网络药理学分析工具，可进行经典的网络药理学及反向网络药理学分析。HerbiV is a multi-functional traditional chinese medicine network pharmacology analysis tool for classical network pharmacology and reverse network pharmacology.",
     # Optional
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/MLi-lab-Bioinformatics-NJUCM/HerbiV",
     author="王皓阳",
     author_email="Wesady@qq.com",
@@ -30,13 +30,15 @@
     keywords="network pharmacology",
     package_dir={"": "src"},
     packages=find_packages(where="src"),
     python_requires=">=3.8",
     install_requires=[
                       "numpy",
                       "pandas",
+                      "tqdm",
+                      "pyecharts"
                       ],
     project_urls={
         "Bug Reports": "https://github.com/MLi-lab-Bioinformatics-NJUCM/pharmastar/issues",
         "Source": "https://github.com/MLi-lab-Bioinformatics-NJUCM/pharmastar",
     },
 )
```

### Comparing `herbiv-0.1a5/src/herbiv/analysis.py` & `herbiv-0.1a6/herbiv/analysis.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,108 +1,150 @@
 import get
 import compute
 import output
 
 
-def from_tcm(tcm,
-             score=900,
-             out_for_cytoscape=True,
-             re=True,
-             path='result/'):
+def from_tcm_or_formula(tcm_or_formula,
+                        score=900,
+                        out_for_cytoscape=True,
+                        out_graph=True,
+                        re=True,
+                        path='result/'):
     r"""
     进行经典的正向网络药理学分析
-    :param tcm: 任何可以使用in判断一个元素是否在其中的组合数据类型，拟分析的中药的中文名称
+    :param tcm_or_formula: 任何可以使用in判断一个元素是否在其中的组合数据类型，拟分析的中药或复方的ID
     :param score: int类型，仅combined_score大于等于score的记录会被筛选出，默认为900
     :param out_for_cytoscape: 布尔类型，是否输出用于Cytoscape绘图的文件
+    :param out_graph: 布尔类型，是否输出图
     :param re: 布尔类型，是否返回原始分析结果（中药、化合物（中药成分）、蛋白质（靶点）及其连接信息）
     :param path: 字符串类型，存放结果的目录
     :return: tcm: pd.DataFrame类型，中药信息
     :return: tcm_chem_links: pd.DataFrame类型，中药-化合物（中药成分）连接信息
     :return: chem: pd.DataFrame类型，化合物（中药成分）信息
     :return: chem_protein_links: pd.DataFrame类型，化合物（中药成分）-蛋白质（靶点）连接信息
     :return: proteins: pd.DataFrame类型，蛋白质（靶点）信息
     """
-    tcm = get.get_tcm('cn_name', tcm)
+    if tcm_or_formula[0][2] == 'P':
+        formula = get.get_formula('HVPID', tcm_or_formula)
+        formula_tcm_links = get.get_formula_tcm_links('HVPID', formula['HVPID'])
+        tcm = get.get_tcm('HVMID', formula_tcm_links['HVMID'])
+    else:
+        formula = None
+        formula_tcm_links = None
+        tcm = get.get_tcm('HVMID', tcm_or_formula)
+
     tcm_chem_links = get.get_tcm_chem_links('HVMID', tcm['HVMID'])
     chem = get.get_chemicals('HVCID', tcm_chem_links['HVCID'])
     chem_protein_links = get.get_chem_protein_links('HVCID', chem['HVCID'], score)
     proteins = get.get_proteins('Ensembl_ID', chem_protein_links['Ensembl_ID'])
 
     # 若化合物（中药成分）-蛋白质（靶点）连接使用了score过滤，则需要依照过滤结果修改chem、tcm_chem_links和tcm
     if score > 0:
         chem = chem.loc[chem.loc[:, 'HVCID'].isin(chem_protein_links['HVCID'])]
         tcm_chem_links = tcm_chem_links.loc[tcm_chem_links.loc[:, 'HVCID'].isin(chem['HVCID'])]
         tcm = tcm.loc[tcm.loc[:, 'HVMID'].isin(tcm_chem_links['HVMID'])]
         # 重新编号（chem和tcm在计算score时会重新编号，此处不再重新编号）
         tcm_chem_links.index = range(tcm_chem_links.shape[0])
 
-    tcm, chem = compute.score(tcm, tcm_chem_links, chem, chem_protein_links)
+    tcm, chem, formula = compute.score(tcm, tcm_chem_links, chem, chem_protein_links, formula, formula_tcm_links)
 
     if out_for_cytoscape:
         output.out_for_cyto(tcm, tcm_chem_links, chem, chem_protein_links, proteins, path)
 
+    if out_graph:
+        output.vis(tcm, tcm_chem_links, chem, chem_protein_links, proteins, path)
+
     if re:
-        return tcm, tcm_chem_links, chem, chem_protein_links, proteins
+        if tcm_or_formula[0][2] == 'P':
+            return formula, formula_tcm_links, tcm, tcm_chem_links, chem, chem_protein_links, proteins
+        else:
+            return tcm, tcm_chem_links, chem, chem_protein_links, proteins
 
 
 def from_proteins(proteins,
                   score=0,
+                  random_state=None,
+                  num=1000,
+                  tcm_component=True,
+                  formula_component=True,
                   out_for_cytoscape=True,
                   re=True,
                   path='result/'):
     r"""
     进行逆向网络药理学分析
     :param proteins: 任何可以使用in判断一个元素是否在其中的组合数据类型，存储拟分析蛋白质（靶点）在STITCH中的Ensembl_ID
     :param score: int类型，仅combined_score大于等于score的记录会被筛选出，默认为0
+    :param random_state: int类型，指定随机数种子
+    :param num: int类型，指定优化时需生成的解的组数
+    :param tcm_component: 布尔类型，是否优化中药组合
+    :param formula_component: 布尔类型，是否优化复方组合
     :param out_for_cytoscape: 布尔类型，是否输出用于Cytoscape绘图的文件
     :param re: 布尔类型，是否返回原始分析结果
     :param path: 字符串类型，存放结果的目录
     :return: tcm: pd.DataFrame类型，中药信息
     :return: tcm_chem_links: pd.DataFrame类型，中药-化合物（中药成分）连接信息
     :return: chem: pd.DataFrame类型，化合物（中药成分）信息
     :return: chem_protein_links: pd.DataFrame类型，化合物（中药成分）-蛋白质（靶点）连接信息
     :return: protein: pd.DataFrame类型，蛋白质（靶点）信息
     """
     protein = get.get_proteins('Ensembl_ID', proteins)
     chem_protein_links = get.get_chem_protein_links('Ensembl_ID', protein['Ensembl_ID'], score)
     chem = get.get_chemicals('HVCID', chem_protein_links['HVCID'])
     tcm_chem_links = get.get_tcm_chem_links('HVCID', chem['HVCID'])
     tcm = get.get_tcm('HVMID', tcm_chem_links['HVMID'])
+    formula_tcm_links = get.get_formula_tcm_links('HVMID', tcm['HVMID'])
+    formula = get.get_formula('HVPID', formula_tcm_links['HVPID'])
+
+    # 计算Score
+    tcm, chem, formula = compute.score(tcm, tcm_chem_links, chem, chem_protein_links, formula, formula_tcm_links)
 
-    tcm, chem = compute.score(tcm, tcm_chem_links, chem, chem_protein_links)
+    # 优化模型
+    tcms = compute.component(tcm.loc[tcm['Importance Score'] != 1.0], random_state, num) if tcm_component else None
+    formulas = compute.component(formula.loc[formula['Importance Score'] != 1.0],
+                                 random_state, num) if formula_component else None
 
     if out_for_cytoscape:
         output.out_for_cyto(tcm, tcm_chem_links, chem, chem_protein_links, protein, path)
 
     if re:
-        return tcm, tcm_chem_links, chem, chem_protein_links, protein
+        return formula, tcm, tcm_chem_links, chem, chem_protein_links, protein, tcms, formulas
 
 
-def from_tcm_protein(tcm,
-                     proteins,
-                     score=0,
-                     out_for_cytoscape=True,
-                     re=True,
-                     path='result/'):
+def from_tcm_or_tcm_protein(tcm_or_formula,
+                            proteins,
+                            score=0,
+                            out_for_cytoscape=True,
+                            out_graph=True,
+                            re=True,
+                            path='result/'):
     r"""
     进行经典的正向网络药理学分析，并根据给定的靶点筛选结果
-    :param tcm: 任何可以使用in判断一个元素是否在其中的组合数据类型，拟分析的中药的中文名称
+    :param tcm_or_formula: 任何可以使用in判断一个元素是否在其中的组合数据类型，拟分析的中药或复方的ID
     :param proteins: 任何可以使用in判断一个元素是否在其中的组合数据类型，拟分析蛋白质（靶点）在STITCH中的Ensembl_ID
     :param score: int类型，仅combined_score大于等于score的记录会被筛选出
     :param out_for_cytoscape: 布尔类型，是否输出用于Cytoscape绘图的文件
+    :param out_graph: 布尔类型，是否输出图
     :param re: 布尔类型，是否返回原始分析结果
     :param path: 字符串类型，存放结果的目录
     :return: tcm: pd.DataFrame类型，中药信息
     :return: tcm_chem_links: pd.DataFrame类型，中药-化合物（中药成分）连接信息
     :return: chem: pd.DataFrame类型，化合物（中药成分）信息
     :return: chem_protein_links: pd.DataFrame类型，化合物（中药成分）-蛋白质（靶点）连接信息
     :return: protein: pd.DataFrame类型，蛋白质（靶点）信息
     """
-    # 检索中药和蛋白质（靶点）
-    tcm = get.get_tcm('cn_name', tcm)
+
+    if tcm_or_formula[0][2] == 'P':
+        formula = get.get_formula('HVPID', tcm_or_formula)
+        formula_tcm_links = get.get_formula_tcm_links('HVPID', formula['HVPID'])
+        tcm = get.get_tcm('HVMID', formula_tcm_links['HVMID'])
+    else:
+        formula = None
+        formula_tcm_links = None
+        tcm = get.get_tcm('HVMID', tcm_or_formula)
+
     proteins = get.get_proteins('Ensembl_ID', proteins)
 
     # 根据中药和蛋白质（靶点）获取中药-化合物（中药成分）连接和化合物（中药成分）-蛋白质（靶点）连接
     tcm_chem_links = get.get_tcm_chem_links('HVMID', tcm['HVMID'])
     chem_protein_links = get.get_chem_protein_links('Ensembl_ID', proteins['Ensembl_ID'], score)
 
     # 获取中药-化合物（中药成分）连接和化合物（中药成分）-蛋白质（靶点）连接中化合物（中药成分）的交集
@@ -117,23 +159,32 @@
     proteins = proteins.loc[proteins.loc[:, 'Ensembl_ID'].isin(chem_protein_links['Ensembl_ID'])]
 
     # 重新编号（chem和tcm在计算score时会重新编号，此处不再重新编号）
     tcm_chem_links.index = range(tcm_chem_links.shape[0])
     chem_protein_links.index = range(chem_protein_links.shape[0])
     proteins.index = range(proteins.shape[0])
 
-    tcm, chem = compute.score(tcm, tcm_chem_links, chem, chem_protein_links)
+    tcm, chem, formula = compute.score(tcm, tcm_chem_links, chem, chem_protein_links, formula, formula_tcm_links)
 
     if out_for_cytoscape:
         output.out_for_cyto(tcm, tcm_chem_links, chem, chem_protein_links, proteins, path)
 
+    if out_graph:
+        output.vis(tcm, tcm_chem_links, chem, chem_protein_links, proteins, path)
+
     if re:
-        return tcm, tcm_chem_links, chem, chem_protein_links, proteins
+        if tcm_or_formula[0][2] == 'P':
+            return formula, formula_tcm_links, tcm, tcm_chem_links, chem, chem_protein_links, proteins
+        else:
+            return tcm, tcm_chem_links, chem, chem_protein_links, proteins
 
 
 if __name__ == '__main__':
-    tcm_ft, tcm_chem_links_ft, chem_ft, chem_protein_links_ft, protein_ft = from_tcm(['柴胡', '黄芩'])
-    tcm_fg, tcm_chem_links_fg, chem_fg, chem_protein_links_fg, protein_fg = from_proteins(['ENSP00000381588',
-                                                                                           'ENSP00000252519'])
-    tcm_ftp, tcm_chem_links_ftp, chem_ftp, chem_protein_links_ftp, protein_ftp = from_tcm_protein(['柴胡', '黄芩'],
-                                                                                                  ['ENSP00000381588',
-                                                                                                   'ENSP00000252519'])
+    tcm_ft, tcm_chem_links_ft, chem_ft, chem_protein_links_ft, protein_ft = from_tcm_or_formula(['HVM0367', 'HVM1695'])
+    formula_ff, formula_tcm_links_ff, tcm_ff, tcm_chem_links_ff, chem_ff, chem_protein_links_ff, protein_ff = \
+        from_tcm_or_formula(['HVP1625'])
+    formula_fg, tcm_fg, tcm_chem_l_fg, chem_fg, chem_protein_l_fg, protein_fg, tcms_fg, formulas_fg = from_proteins(
+        ['ENSP00000381588', 'ENSP00000252519'], num=10)
+    tcm_ftp, tcm_chem_links_ftp, chem_ftp, chem_protein_links_ftp, protein_ftp = \
+        from_tcm_or_tcm_protein(['HVM0367', 'HVM1695'], ['ENSP00000381588', 'ENSP00000252519'])
+    formula_ffp, formula_tcm_links_ffp, tcm_ffp, tcm_chem_links_ffp, chem_ffp, chem_protein_links_ffp, protein_ffp = \
+        from_tcm_or_tcm_protein(['HVP1625'], ['ENSP00000381588', 'ENSP00000252519'])
```

### Comparing `herbiv-0.1a5/src/herbiv/get.py` & `herbiv-0.1a6/herbiv/get.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,52 @@
 import os
 import pandas as pd
 
 
+def get_formula(by, items):
+    """
+    读取HerbiV_formula数据集，返回items中复方的信息
+    :param by: str类型，数据集中与items相匹配的列的列名
+    :param items: 任何可以使用in判断一个元素是否在其中的组合数据类型，存放要查询的复方
+    :return: pd.DataFrame类型，items中复方的信息
+    """
+
+    # 读取数据集
+    current_directory = os.path.dirname(os.path.abspath(__file__))
+    formula_all = pd.read_csv(current_directory + r'/data/HerbiV_formula.csv')
+
+    # 在HerbiV_tcm中获取items中复方的信息
+    formula = formula_all.loc[formula_all[by].isin(items)].copy()
+
+    # 重新设置索引
+    formula.index = range(formula.shape[0])
+
+    return formula
+
+
+def get_formula_tcm_links(by, items):
+    """
+    读取HerbiV_formula_tcm_links数据集，返回items中复方/中药的复方-中药连接信息
+    :param by: str类型，数据集中与items相匹配的列的列名
+    :param items: pd.DataFrame或其他任何可以使用in判断一个元素是否在其中的组合数据类型，存放要查询的复方/中药
+    :return: pd.DataFrame类型，items中复方/中药的复方-中药连接信息
+    """
+    # 读取数据集
+    current_directory = os.path.dirname(os.path.abspath(__file__))
+    formula_tcm_links_all = pd.read_csv(current_directory + r'/data/HerbiV_formula_tcm_links.csv')
+
+    # 在HerbiV_formula_tcm_links中获取items中复方/中药的复方-中药连接信息
+    formula_tcm_links = formula_tcm_links_all.loc[formula_tcm_links_all[by].isin(items)].copy()
+
+    # 重新设置索引
+    formula_tcm_links.index = range(formula_tcm_links.shape[0])
+
+    return formula_tcm_links
+
+
 def get_tcm(by, items):
     """
     读取HerbiV_tcm数据集，返回items中中药的信息
     :param by: str类型，数据集中与items相匹配的列的列名
     :param items: 任何可以使用in判断一个元素是否在其中的组合数据类型，存放要查询的中药
     :return: pd.DataFrame类型，items中中药的信息
     """
@@ -109,12 +150,14 @@
     # 重置索引
     proteins.index = range(proteins.shape[0])
 
     return proteins
 
 
 if __name__ == '__main__':
-    tcm_info = get_tcm('cn_name', ['柴胡', '黄芩'])
+    formula_info = get_formula('HVPID', ['HVP1625'])
+    formula_tcm_links_info = get_formula_tcm_links('HVPID', formula_info['HVPID'])
+    tcm_info = get_tcm('HVMID', formula_tcm_links_info['HVMID'])
     tcm_chem_links_info = get_tcm_chem_links('HVMID', tcm_info['HVMID'])
     chem_info = get_chemicals('HVCID', tcm_chem_links_info['HVCID'])
     chem_protein_links_info = get_chem_protein_links('HVCID', chem_info['HVCID'])
     protein_info = get_proteins('Ensembl_ID', chem_protein_links_info['Ensembl_ID'])
```

### Comparing `herbiv-0.1a5/src/herbiv/data/HerbiV_chemical_protein_links.csv` & `herbiv-0.1a6/herbiv/data/HerbiV_chemical_protein_links.csv`

 * *Files identical despite different names*

### Comparing `herbiv-0.1a5/src/herbiv/data/HerbiV_chemicals.csv` & `herbiv-0.1a6/herbiv/data/HerbiV_chemicals.csv`

 * *Files identical despite different names*

### Comparing `herbiv-0.1a5/src/herbiv/data/HerbiV_proteins.csv` & `herbiv-0.1a6/herbiv/data/HerbiV_proteins.csv`

 * *Files 0% similar despite different names*

```diff
@@ -7220,14 +7220,15 @@
 ENSP00000332766,Neuropeptide B (Preproprotein L7) (hPPL7) [Cleaved into: Neuropeptide B-23 (NPB23) (hL7); Neuropeptide B-29 (NPB29) (hL7C)],NPB PPL7 PPNPB
 ENSP00000332771,Chloride channel protein ClC-Ka (Chloride channel Ka) (ClC-K1),CLCNKA
 ENSP00000332772,Protein YIPF7 (Five-pass transmembrane protein localizing in the Golgi apparatus and the endoplasmic reticulum 9) (YIP1 family member 7),YIPF7 FINGER9 YIP1B
 ENSP00000332773,Immunoglobulin superfamily DCC subclass member 3 (Putative neuronal cell adhesion molecule),IGDCC3 PUNC
 ENSP00000332788,Anoctamin-9 (Transmembrane protein 16J) (Tumor protein p53-inducible protein 5) (p53-induced gene 5 protein),ANO9 PIG5 TMEM16J TP53I5
 ENSP00000332790,Histone H2A type 2-B (H2A-clustered histone 21),H2AC21 HIST2H2AB
 ENSP00000332791,Kelch-like protein 15,KLHL15 KIAA1677
+ENSP00000258743,,IL6
 ENSP00000332805,Keratin-associated protein 8-1 (High glycine-tyrosine keratin-associated protein 8.1),KRTAP8-1 KAP8.1 KRTAP8.1
 ENSP00000332806,EMILIN-3 (EMILIN-5) (Elastin microfibril interface-located protein 3) (Elastin microfibril interfacer 3) (Elastin microfibril interface-located protein 5) (Elastin microfibril interfacer 5),EMILIN3 C20orf130 EMILIN5
 ENSP00000332809,Photoreceptor cilium actin regulator,PCARE C2orf71
 ENSP00000332812,Prostaglandin D2 receptor 2 (Chemoattractant receptor-homologous molecule expressed on Th2 cells) (G-protein coupled receptor 44) (CD antigen CD294),PTGDR2 CRTH2 DL1R GPR44
 ENSP00000332861,Zinc finger protein 530,ZNF530 KIAA1508
 ENSP00000332879,Leucine-rich repeat transmembrane protein FLRT2 (Fibronectin-like domain-containing leucine-rich transmembrane protein 2),FLRT2 KIAA0405 UNQ232/PRO265
 ENSP00000332886,FRAS1-related extracellular matrix protein 3,FREM3
@@ -14140,15 +14141,15 @@
 ENSP00000468354,Ankyrin repeat domain-containing protein 29,ANKRD29
 ENSP00000468367,PCAF N-terminal domain-containing protein,
 ENSP00000468633,Signal peptidase complex catalytic subunit SEC11C (EC 3.4.21.89) (Microsomal signal peptidase 21 kDa subunit) (SPase 21 kDa subunit) (SEC11 homolog C) (SEC11-like protein 3) (SPC21),SEC11C SEC11L3 SPC21 SPCS4C
 ENSP00000468678,Pleckstrin homology domain-containing family H member 3 (PH domain-containing family H member 3),PLEKHH3
 ENSP00000468690,Glucose-6-phosphate isomerase,
 ENSP00000468720,Zinc finger protein 253 (Bone marrow zinc finger 1) (BMZF-1) (Zinc finger protein 411),ZNF253 BMZF1 ZNF411
 ENSP00000468969,PAT complex subunit Asterix (Protein associated with the ER translocon of 10kDa) (PAT-10) (PAT10) (WD repeat domain 83 opposite strand) (WDR83 opposite strand),WDR83OS C19orf56 CGI-140 My006 PTD008
-ENSP00000469049,"Tumor necrosis factor ligand superfamily member 14 (Herpes virus entry mediator ligand) (HVEM-L) (Herpesvirus entry mediator ligand) (CD antigen CD258) [Cleaved into: Tumor necrosis factor ligand superfamily member 14, membrane form; Tumor necrosis factor ligand superfamily member 14, soluble form]",TNFSF14 HVEML LIGHT UNQ391/PRO726
+ENSP00000469049,"Tumor necrosis factor ligand superfamily member 14 (Herpes virus entry mediator ligand) (HVEM-L) (Herpesvirus entry mediator ligand) (CD antigen CD258) [Cleaved into: Tumor necrosis factor ligand superfamily member 14, membrane form; Tumor necrosis factor ligand superfamily member 14, soluble form]",TNFSF14
 ENSP00000469315,Kallikrein-15 (EC 3.4.21.-) (ACO protease),KLK15
 ENSP00000469337,Leucine-rich repeat-containing protein 63,LRRC63
 ENSP00000469468,U6 snRNA-associated Sm-like protein LSm4 (Glycine-rich protein) (GRP),LSM4
 ENSP00000469582,Zinc finger protein 729,ZNF729
 ENSP00000469958,Zinc finger protein 626,ZNF626
 ENSP00000470059,RRM domain-containing protein,
 ENSP00000470082,DNA-binding death effector domain-containing protein 2 (DED-containing protein FLAME-3) (FADD-like anti-apoptotic molecule 3),DEDD2 FLAME3 PSEC0004
```

### Comparing `herbiv-0.1a5/src/herbiv/data/HerbiV_tcm.csv` & `herbiv-0.1a6/herbiv/data/HerbiV_tcm.csv`

 * *Files identical despite different names*

### Comparing `herbiv-0.1a5/src/herbiv/data/HerbiV_tcm_chemical_links.csv` & `herbiv-0.1a6/herbiv/data/HerbiV_tcm_chemical_links.csv`

 * *Files identical despite different names*

### Comparing `herbiv-0.1a5/LICENSE` & `herbiv-0.1a6/LICENSE`

 * *Files identical despite different names*

### Comparing `herbiv-0.1a5/README.md` & `herbiv-0.1a6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <h1 align="center">
 <img src="https://github.com/MLi-lab-Bioinformatics-NJUCM/HerbiV/blob/main/logo.png" width="200">
 </h1>
 
-[![Downloads](https://static.pepy.tech/personalized-badge/herbiv?period=month&units=international_system&left_color=brightgreen&right_color=blue&left_text=Downloads)](https://pepy.tech/project/herbiv)
+[![Downloads](https://static.pepy.tech/personalized-badge/herbiv?period=total&units=international_system&left_color=brightgreen&right_color=blue&left_text=Downloads)](https://pepy.tech/project/herbiv)
 
-HerbiV一个开发中的具有多种功能的中药网络药理学分析工具，可进行经典的网络药理学及反向网络药理学分析。
+HerbiV是一个开发中的具有多种功能的中药网络药理学分析工具，可进行经典的网络药理学及反向网络药理学分析。
 
 HerbiV is a multifunctional traditional chinese medicine network pharmacology analysis tool 
 under development for classical network pharmacology and reverse network pharmacology.
 
 <!-- toc -->
 
 - [中文](#中文)
@@ -167,14 +167,16 @@
 - `score`: int, which will not be picked out unless the combined_score is no less than it, `900` by default;
 - `out_for_cytoscape`: boolean, decides whether to output the file which will be used for Cytoscape mapping, `True` by default;
 - `re`: boolean, decides whether to return to the original analysis results, `True` by default. If `re` is `True`, the function will turn to the result of `tcm`, `tcm_chem links`, `chem`, `chem_protein_links` and `proteins`, all of which are in pd.DataFrame form, storing the information of tcm, the information of tcm-componds or ingredients connection, the information of the compounds or the ingredients, the information of the compounds or ingredients-proteins or the targets connection and the information of the proteins or targets, respectively;
 - `path`: str, which is the path to store the results, defaulted to `result/`. A corrsponding catalogue will be established automatically if the path can not be found.
 
 ### `from_proteins`
 
+The pipeline function that is utilized for reverse network pharmacology. Only a few commands are needed to use it
+
 ```python
 from herbiv import analysis
 analysis.from_proteins(proteins, score, out_for_cytoscape, re, path)
 ```
 
 It needs a required parameter `proteins`,  which is a combined data type that can judge whether an element lies in it using in, storing the Ensembl_ID in STITCH of the proteins or targets which are supposed to be analyzed, e.g. `['ENSP00000381588', 'ENSP00000252519']`.
 
@@ -182,14 +184,16 @@
 - `score`: int, which will not be picked out unless the combined_score is no less than it, `0` by default;
 - `out_for_cytoscape`: boolean, decides whether to output the file which will be used for Cytoscape mapping later, `True` by default;
 - `re`: boolean, decides whether to return to the original analysis results, `True` by default. If `re` is `true`, the function will turn to the result of `tcm`, `tcm_chem links`, `chem`, `chem_protein_links` and `proteins`, all of which are in pd.DataFrame form, storing the information of tcm, the information of tcm-componds or ingredients connection, the information of the compounds or the ingredients, the information of the compounds or ingredients-proteins or the targets connection and the information of the proteins or targets, respectively;
 - `path`: str, which is the path to store the results, defaulted to `result/`. A corrsponding catalogue will be established automatically if the path can not be found.
 
 ### `from_tcm_protein`
 
+The pipeline function that searches for tcm and the targets at the same time. Only a few commands are needed to use it
+
 ```python
 from herbiv import analysis
 analysis.from_proteins(tcm, proteins, score, out_for_cytoscape, re, path)
 ```
 
 It needs two required parameters `tcm` and `proteins`, either of which is a combined data type that can judge whether an element lies in it using in, storing the chinese name of tcm that is supposed to be inquired, e.g. `['柴胡', '黄芩']` and the Ensembl_ID in STITCH of the proteins or targets which are supposed to be analyzed, e.g. `['ENSP00000381588', 'ENSP00000252519']`.
```

### Comparing `herbiv-0.1a5/pyproject.toml` & `herbiv-0.1a6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 [build-system]
 requires = [
     "hatchling",
     "numpy",
     "pandas",
+    "tqdm",
+    "pyecharts",
     "typing-extensions",
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "herbiv"
-version = "0.1a5"
+version = "0.1a6"
 authors = [
   { name="王皓阳", email="Wesady@qq.com" },
 ]
 description = "HerbiV是一个具有多种功能的中药网络药理学分析工具，可进行经典的网络药理学及反向网络药理学分析。HerbiV is a multi-functional traditional chinese medicine network pharmacology analysis tool for classical network pharmacology and reverse network pharmacology."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `herbiv-0.1a5/PKG-INFO` & `herbiv-0.1a6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: herbiv
-Version: 0.1a5
+Version: 0.1a6
 Summary: HerbiV是一个具有多种功能的中药网络药理学分析工具，可进行经典的网络药理学及反向网络药理学分析。HerbiV is a multi-functional traditional chinese medicine network pharmacology analysis tool for classical network pharmacology and reverse network pharmacology.
 Project-URL: Homepage, https://github.com/MLi-lab-Bioinformatics-NJUCM/pharmastar
 Project-URL: Bug Tracker, https://github.com/MLi-lab-Bioinformatics-NJUCM/pharmastar/issues
 Author-email: 王皓阳 <Wesady@qq.com>
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Healthcare Industry
@@ -19,17 +19,17 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 <h1 align="center">
 <img src="https://github.com/MLi-lab-Bioinformatics-NJUCM/HerbiV/blob/main/logo.png" width="200">
 </h1>
 
-[![Downloads](https://static.pepy.tech/personalized-badge/herbiv?period=month&units=international_system&left_color=brightgreen&right_color=blue&left_text=Downloads)](https://pepy.tech/project/herbiv)
+[![Downloads](https://static.pepy.tech/personalized-badge/herbiv?period=total&units=international_system&left_color=brightgreen&right_color=blue&left_text=Downloads)](https://pepy.tech/project/herbiv)
 
-HerbiV一个开发中的具有多种功能的中药网络药理学分析工具，可进行经典的网络药理学及反向网络药理学分析。
+HerbiV是一个开发中的具有多种功能的中药网络药理学分析工具，可进行经典的网络药理学及反向网络药理学分析。
 
 HerbiV is a multifunctional traditional chinese medicine network pharmacology analysis tool 
 under development for classical network pharmacology and reverse network pharmacology.
 
 <!-- toc -->
 
 - [中文](#中文)
@@ -188,14 +188,16 @@
 - `score`: int, which will not be picked out unless the combined_score is no less than it, `900` by default;
 - `out_for_cytoscape`: boolean, decides whether to output the file which will be used for Cytoscape mapping, `True` by default;
 - `re`: boolean, decides whether to return to the original analysis results, `True` by default. If `re` is `True`, the function will turn to the result of `tcm`, `tcm_chem links`, `chem`, `chem_protein_links` and `proteins`, all of which are in pd.DataFrame form, storing the information of tcm, the information of tcm-componds or ingredients connection, the information of the compounds or the ingredients, the information of the compounds or ingredients-proteins or the targets connection and the information of the proteins or targets, respectively;
 - `path`: str, which is the path to store the results, defaulted to `result/`. A corrsponding catalogue will be established automatically if the path can not be found.
 
 ### `from_proteins`
 
+The pipeline function that is utilized for reverse network pharmacology. Only a few commands are needed to use it
+
 ```python
 from herbiv import analysis
 analysis.from_proteins(proteins, score, out_for_cytoscape, re, path)
 ```
 
 It needs a required parameter `proteins`,  which is a combined data type that can judge whether an element lies in it using in, storing the Ensembl_ID in STITCH of the proteins or targets which are supposed to be analyzed, e.g. `['ENSP00000381588', 'ENSP00000252519']`.
 
@@ -203,14 +205,16 @@
 - `score`: int, which will not be picked out unless the combined_score is no less than it, `0` by default;
 - `out_for_cytoscape`: boolean, decides whether to output the file which will be used for Cytoscape mapping later, `True` by default;
 - `re`: boolean, decides whether to return to the original analysis results, `True` by default. If `re` is `true`, the function will turn to the result of `tcm`, `tcm_chem links`, `chem`, `chem_protein_links` and `proteins`, all of which are in pd.DataFrame form, storing the information of tcm, the information of tcm-componds or ingredients connection, the information of the compounds or the ingredients, the information of the compounds or ingredients-proteins or the targets connection and the information of the proteins or targets, respectively;
 - `path`: str, which is the path to store the results, defaulted to `result/`. A corrsponding catalogue will be established automatically if the path can not be found.
 
 ### `from_tcm_protein`
 
+The pipeline function that searches for tcm and the targets at the same time. Only a few commands are needed to use it
+
 ```python
 from herbiv import analysis
 analysis.from_proteins(tcm, proteins, score, out_for_cytoscape, re, path)
 ```
 
 It needs two required parameters `tcm` and `proteins`, either of which is a combined data type that can judge whether an element lies in it using in, storing the chinese name of tcm that is supposed to be inquired, e.g. `['柴胡', '黄芩']` and the Ensembl_ID in STITCH of the proteins or targets which are supposed to be analyzed, e.g. `['ENSP00000381588', 'ENSP00000252519']`.
```

