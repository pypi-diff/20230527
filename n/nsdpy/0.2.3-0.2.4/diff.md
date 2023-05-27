# Comparing `tmp/nsdpy-0.2.3.tar.gz` & `tmp/nsdpy-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nsdpy-0.2.3.tar", max compression
+gzip compressed data, was "nsdpy-0.2.4.tar", max compression
```

## Comparing `nsdpy-0.2.3.tar` & `nsdpy-0.2.4.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     1071 2022-02-14 11:39:09.498105 nsdpy-0.2.3/LICENSE
--rw-r--r--   0        0        0     2720 2022-02-14 11:39:09.498220 nsdpy-0.2.3/README.md
--rw-r--r--   0        0        0    34824 2022-02-14 11:39:09.540135 nsdpy-0.2.3/functions.py
--rw-r--r--   0        0        0    12575 2022-02-14 11:51:04.753014 nsdpy-0.2.3/nsdpy.py
--rw-r--r--   0        0        0      836 2022-02-14 11:51:01.378939 nsdpy-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     3721 2022-02-14 11:53:07.180240 nsdpy-0.2.3/setup.py
--rw-r--r--   0        0        0     3677 2022-02-14 11:53:07.180718 nsdpy-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-27 13:47:59.346367 nsdpy-0.2.4/LICENSE
+-rw-r--r--   0        0        0     2720 2023-05-27 13:47:59.346590 nsdpy-0.2.4/README.md
+-rw-r--r--   0        0        0    35687 2023-05-27 13:47:59.386545 nsdpy-0.2.4/functions.py
+-rw-r--r--   0        0        0    12577 2023-05-27 15:10:50.380161 nsdpy-0.2.4/nsdpy.py
+-rw-r--r--   0        0        0      836 2023-05-27 15:10:50.297755 nsdpy-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     3728 1970-01-01 00:00:00.000000 nsdpy-0.2.4/PKG-INFO
```

### Comparing `nsdpy-0.2.3/LICENSE` & `nsdpy-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nsdpy-0.2.3/README.md` & `nsdpy-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `nsdpy-0.2.3/functions.py` & `nsdpy-0.2.4/functions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,61 @@
-import requests             #https://requests.readthedocs.io/en/master/
+#import from standard library
 import os
 import re
 import csv
 from collections import Counter
 
+#third party imports
+import requests             #https://requests.readthedocs.io/en/master/
+
+    
+
+def countDown(iteration, total, message=''):
+    """
+    Take the number of iteration, the range of a forloop and a message and output a message with the percent of job done
+
+    INPUTS: countDown(iteration, total, message='')
+    iteration:  positive INT
+    total: positive INT
+    message: STRING
+
+    OUTPUT: STRING
+        
+    """
+    
+    if message:
+        message = message + ": "
+
+    if iteration < 0:
+        raise ValueError('iteration must be a positive integer')
+    
+    if total < 0:
+        raise ValueError('total must be a positive integer')
+
+    if total < 1:
+        return f'{message}no job to be done'
+
+    iteration = iteration + 1
+    left = round( ( iteration / total ) * 100, 1 )
+    if left > 100:
+        left = 100
+    return f'{message}{left}%'
+
 
 def download(parameters, address):
-    ##send requests to the API until getting a result
+    """ 
+    Sends requests to the API until getting a result
+    
+    INPUTS: download(parameters, address)
+        parameters: DICT, parameters of the get request to the API
+        Address: STRING, API bas URL
+
+    OUTPUT: object, <class 'requests.models.Response'>
+        if an exceptions.HTTPError is triggered: returns 1
+    """ 
     connect = 0
     while True:
         try:
             result = requests.get(address, params = parameters, timeout = 60)
             break
         except requests.exceptions.HTTPError as errh:
             print("Http Error:", errh)
@@ -78,15 +123,15 @@
     if count < retmax:
         retmax = count
 
     if count % retmax == 0:
         nb = count//retmax
     else: 
         nb = (count//retmax) + 1
-   
+
     for x in range(nb):
         ##build the API address
         esummaryaddress = "https://eutils.ncbi.nlm.nih.gov/entrez/eutils/esummary.fcgi"
         #parameters 
         parameters = {}
         parameters['db'] = "taxonomy"
         parameters['query_key'] = querykey
@@ -95,24 +140,16 @@
         parameters['retmax'] = str(retmax)
         parameters['rettype'] = "uilist"
         parameters['retmode'] = "text"
         result = download(parameters, esummaryaddress)
 
         #comments
         if verb and verb > 1:
-            start = (x * retmax) + retmax
-            dl = round((start / count) * 100, 1)
-            if dl > 100:
-                dl = 100
-            print(f'{dl} %  of the TaxIDs downloaded')
-
-        # if verb and verb > 1:
-        #     ret = parameters['retstart']
-        #     print(f'{round(((int(ret) + 100)/count)*100, 1)} %  of the TaxIDs downloaded')
-
+            print(countDown(x, nb, "Downloading TaxIDs"))
+            
         ###extract the TaxIDs and accession numbers (record in text file and in dict_ids)
         f = result.text.splitlines()
         for line in f:
             if len(line.split('<DocSum>')) > 1:
                 taxid = ''
                 seqnb = ''
             else:
@@ -137,27 +174,35 @@
         with open(path, 'a') as summary:
             [summary.write(f'{key}  {value}\n') for key, value in dict_ids.items()]
 
     return dict_ids
 
 
 def dispatch(lineage, classif):
+    """
+        take the lineage of a sequence and the classification option and return the base name of the file to store 
+        the sequence.
+
+        INPUTS: dispatch(lineage, classif) 
+            lineage: LIST
+            classif: INT or LIST
+    """
     ###Phylums
     Plantae = ['Chlorophyta', 'Charophyta', 'Bryophyta', 'Marchantiophyta', 'Lycopodiophyta', 'Ophioglossophyta', 'Pteridophyta',\
     'Cycadophyta', 'Ginkgophyta', 'Gnetophyta', 'Pinophyta', 'Magnoliophyta', 'Equisetidae', 'Psilophyta', 'Bacillariophyta',\
     'Cyanidiophyta', 'Glaucophyta', 'Prasinophyceae','Rhodophyta']
     Fungi = ['Chytridiomycota', 'Zygomycota', 'Ascomycota', 'Basidiomycota', 'Glomeromycota']
     Metazoa = ['Acanthocephala', 'Acoelomorpha', 'Annelida', 'Arthropoda', 'Brachiopoda', 'Ectoprocta', 'Bryozoa', 'Chaetognatha',\
     'Chordata', 'Cnidaria', 'Ctenophora', 'Cycliophora', 'Echinodermata', 'Echiura', 'Entoprocta', 'Gastrotricha', 'Gnathostomulida',\
     'Hemichordata', 'Kinorhyncha', 'Loricifera', 'Micrognathozoa', 'Mollusca', 'Nematoda', 'Nematomorpha', 'Nemertea', 'Onychophora'\
     'Orthonectida', 'Phoronida', 'Placozoa', 'Plathelminthes', 'Porifera', 'Priapulida', 'Rhombozoa', 'Rotifera', 'Sipuncula',\
     'Tardigrada', 'Xenoturbella']
 
     ##no option selected
-    if classif == 3 or classif == 2:
+    if classif == 2:
         return "sequences"
     ##user gave list of taxonomic levels
     if isinstance(classif, list):
         try:
             other = [rank for rank in lineage if rank in classif][0]
         except IndexError:
             other = "OTHERS"
@@ -285,15 +330,15 @@
     ## Unpack parameters
     (_, api_key) = QUERY
     (verb, genelist, classif, _, tsv, information)= OPTIONS
 
     # Comment:
     if verb and verb > 0:
         print("Downloading the CDS fasta files...")
-   
+
     # List of accession number for wich a gene is found or the file has been retrieve if no gene filter:
     found = []
     count = len(list_of_ids)
 
     # Number of accession numbers to be sent at each API query
     retmax = 200 
     if count < retmax:
@@ -324,26 +369,22 @@
         raw_result = download(parameters, efetchaddress)
         raw_result = raw_result.text
 
         ## Extract available information
         if not information and not genelist and classif == 3:
             result_fasta = raw_result.split(">lcl|")[1:]
             sublist = [r.split("_cds")[0] for r in result_fasta]
-  
+
         ##analyse the results     
         sublist = extract(path, raw_result, dict_ids, dict_taxo, genelist, OPTIONS, verb)
         found = found + sublist
 
         #comments
         if verb > 1:
-            start = (x * retmax) + retmax
-            dl = round((start / count) * 100, 1)
-            if dl > 100:
-                dl = 100
-            print(f'{dl} %  of the CDS fasta files downloaded')
+            print(countDown(x, nb , "Downloading the cds_fasta files"))
 
     return found
 
 
 def subextract(seq, path, dict_ids, dict_taxo, genelist, OPTIONS=None):
 
     if OPTIONS is None:
@@ -588,19 +629,15 @@
 
             if tsv:
                 tsv_file_writer(tsv_file, data, OPTIONS)
 
             keys.append(key)
 
         if verb > 1:
-            start = (x * retmax) + retmax
-            dl = round((start / count) * 100, 1)
-            if dl > 100:
-                dl = 100
-            print(f'{dl} %  of the fasta files downloaded')
+            print(countDown(x, nb, "Downloading the fasta files"))  
 
     return keys
 
 
 def duplicates(listofaccess, path):
     filename = path + "/duplicates.txt"
     count = Counter(listofaccess)
@@ -710,15 +747,15 @@
                         if information:
                             try:
                                 name = dict_taxo[taxid]['Name']
                                 name = "_".join(name.split())
                             except:
                                 name = "not found"
                             info_line = ">" + name + "-" + dictCDS["version"] + "_cds_" + dictCDS["proteinid"].strip('"') + " | " + taxid + " | " +  "".join(taxo).rstrip(".")
-                     
+                    
                         else:
                             info_line = ">" + dictCDS["version"] + "_cds_" + dictCDS["proteinid"].strip('"') + " [gene=" + dictCDS["gene"] + "] " + "[protein=" + dictCDS["proteinid"] + "] " + \
                                 "[location=" + dictCDS["loc"].strip() + "] " + "[gbkey=CDS] " + "[definition=" + " ".join(dictCDS["definition"].split(" " * 12)).rstrip(".") + "]"
 
                         ## append to file
                         with open(fasta_file, 'a') as a:
                             a.write(f"{info_line}\n")
@@ -927,7 +964,12 @@
         writer = csv.writer(outtsv, delimiter='\t')
         if information:
             writer.writerow([name, seqid, taxid, lineage, len(dna), dna])
         else:
             writer.writerow([seqid, taxid, len(dna), dna])
 
     return
+
+if __name__=="_main_":
+    countDown()
+    download()
+    dispatch()
```

### Comparing `nsdpy-0.2.3/nsdpy.py` & `nsdpy-0.2.4/nsdpy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.2.3'
+__version__ = '0.2.4'
 __author__ = "Raphael Hebert, Emese Meglecz"
 __email__ = "raphaelhebert18@gmail.com, emese.meglecz@imbe.fr"
 __license__ = "MIT"
 
 from functions import esearchquery, completetaxo, taxids, cds_fasta, taxo, fasta, duplicates
 import sys
 import os
@@ -39,16 +39,16 @@
     parser.add_argument("-t", "--tsv", default=None, help="create a tsv file based on fasta file output", action="store_true")
     #Taxonomy
     group3 = parser.add_mutually_exclusive_group()
     group3.add_argument("-k", "--kingdom", help="output four different text files file: Plantae and Fungi, Metazoa and  Others", action="store_true" )
     group3.add_argument("-p", "--phylum", help="output one file text per phylum", action="store_true" )
     group3.add_argument("-l", "--levels", help="find only the taxon given by user", nargs="+")
     group3.add_argument("-s", "--species",\
-        help="classify the results in different text file one for each specie+n level found, exp: -s correspond to lowest levels, -ss 2nd lowest, -sssss 5th lowest and so on",\
-        action="count", default=3)
+        help="classify the results in different text file one for each (specie + n) level found, exp: -s correspond to lowest levels, -ss 2nd lowest, -sssss 5th lowest and so on",\
+        action="count", default=2)
 
     #information line
     parser.add_argument("-i", "--information", help="just add the taxonomic information in the information line of the output file(s)", action="store_true" )
 
     args = parser.parse_args()
 
     #################################################
@@ -104,18 +104,18 @@
         classif = 0
         options_report.append("--phylum (-p)")
     elif args.levels:
         classif = args.levels
         options_report.append(f"--levels (-l) {args.levels[0]}")
     elif args.species:
         classif = args.species
-        if args.species != 3:
-            options_report.append("--species (-", + "s" * ( args.species - 3 ) + ")")
+        if args.species > 2:
+            options_report.append("--species (-" + "s" * ( args.species - 2 ) + ")")
     else:
-        classif = 3
+        classif = 2
 
     OPTIONS = (verb, args.cds, classif, args.taxids, args.tsv, args.information)
 
     ##foldername and path
     starting_time = str(datetime.now())
     starting_time = '_'.join(starting_time.split())[:19]
     starting_time = starting_time.replace(":", "-")
```

### Comparing `nsdpy-0.2.3/pyproject.toml` & `nsdpy-0.2.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nsdpy"
-version = "0.2.3"
+version = "0.2.4"
 description = "Automatize the download of DNA sequences from NCBI, sort them according to their taxonomy and filter them with a gene name (provided as a regular expression)"
 authors = ["RaphaelHebert <raphaelhebert18@gmail.com>", "Emese Meglecz <emese.meglecz@imbe.fr>"]
 include = ["functions.py"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/RaphaelHebert/nsdpy"
 homepage = "https://github.com/RaphaelHebert/nsdpy"
```

### Comparing `nsdpy-0.2.3/setup.py` & `nsdpy-0.2.4/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,108 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: nsdpy
+Version: 0.2.4
+Summary: Automatize the download of DNA sequences from NCBI, sort them according to their taxonomy and filter them with a gene name (provided as a regular expression)
+Home-page: https://github.com/RaphaelHebert/nsdpy
+License: MIT
+Keywords: NCBI,Taxonomy,DNA
+Author: RaphaelHebert
+Author-email: raphaelhebert18@gmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: certifi (>=2020.12.5,<2021.0.0)
+Requires-Dist: chardet (>=4.0.0,<5.0.0)
+Requires-Dist: idna (>=2.10,<3.0)
+Requires-Dist: requests (>=2.25.1,<3.0.0)
+Requires-Dist: urllib3 (>=1.26.2,<2.0.0)
+Project-URL: Repository, https://github.com/RaphaelHebert/nsdpy
+Description-Content-Type: text/markdown
+
+# nsdpy
+
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![pypi](https://img.shields.io/pypi/v/nsdpy)](https://pypi.org/project/nsdpy/)
+[![Python 3.8](https://upload.wikimedia.org/wikipedia/commons/a/a5/Blue_Python_3.8_Shield_Badge.svg)](https://www.python.org/)
+[![Documentation Status](https://readthedocs.org/projects/nsdpy/badge/?version=latest)](https://nsdpy.readthedocs.io/en/latest/?badge=latest)
+
+
+
+- [Introduction](#introduction)
+- [Workfolw](#workflow)
+- [Quick start](#quick-start)
+- [Usage](#usage)
+  - [Google Colab](#google-colab)
+  - [Command line](#command-line)
+- [Authors and acknowledgment](#authors-and-acknowledgment)
+- [Support](#support)
+- [Licence](#license)
+- [More Documentation](#more-documentation)
+
+## Introduction
+
+nsdpy (nucleotide or NCBI sequence downloader) aims to ease the download and sort of big bacth of DNA sequences from the NCBI database. 
+It can also be usefull to filter the sequences based on their annotations.
+Using nsdpy the user can:
+
+- **Search** NCBI nucleotide database
+- **Download** the fasta files or the cds_fasta files corresponding to the result of the search
+- **Sort** the sequences based on their taxonomy
+- **Select** coding sequences from cds files based on the gene names using one or more regular expressions. 
+This can help the user retrieve some sequences for which the gene name is annotated in another field.
+- **Retrieve** the taxonomic information and add it to the output sequences.  
+
+## Quick start
+
+- Clone the repo from Github: 
+```bash 
+git clone https://github.com/RaphaelHebert/nsdpy.git
+  ```
+- pip:  
+_depending on the user environment pip may be replaced by pip3 if pip3 is used_
+```bash 
+pip install nsdpy
+```  
+*minimum python version for nsdpy: 3.8.2* 
+
+- Google Colab: save a copy of [this notebook](https://colab.research.google.com/drive/1UmxzRc_k5sNeQ2RPGe29nWR_1_0FRPkq?usp=sharing) in your drive.
+
+## Workflow
+
+<img src="https://docs.google.com/drawings/d/e/2PACX-1vRD4h7l0S57op_4j-5xsz8iv1j1XBliw-jEdtnWOIq-JAU2l8kSV6d1NmkHd5Q4zhUmZCA3SHUSuHJw/pub?w=801&amp;h=744" width="600" />
+
+## Usage
+### Google colab
+
+[nsdpy colab notebook](https://colab.research.google.com/drive/1UmxzRc_k5sNeQ2RPGe29nWR_1_0FRPkq?usp=sharing)
+
+### Command line
+
+```bash
+nsdpy -r "USER'S REQUEST" [OPTIONS] 
+```
+
+## Authors and acknowledgment  
+
+[Raphael Hebert](https://github.com/RaphaelHebert)  
+[Emese Meglecz](https://github.com/meglecz)
+
+
+## Support
+
+## License
+
+Code and documentation copyright 2021 the nsdpy authors. Code released under the MIT License.
+
+## More Documentation
+
+Official documentation:  
+[Readthedocs](https://nsdpy.readthedocs.io/en/latest/main.html#overview)
+  
+
 
-modules = \
-['nsdpy']
-install_requires = \
-['certifi>=2020.12.5,<2021.0.0',
- 'chardet>=4.0.0,<5.0.0',
- 'idna>=2.10,<3.0',
- 'requests>=2.25.1,<3.0.0',
- 'urllib3>=1.26.2,<2.0.0']
-
-entry_points = \
-{'console_scripts': ['nsdpy = nsdpy:main']}
-
-setup_kwargs = {
-    'name': 'nsdpy',
-    'version': '0.2.3',
-    'description': 'Automatize the download of DNA sequences from NCBI, sort them according to their taxonomy and filter them with a gene name (provided as a regular expression)',
-    'long_description': '# nsdpy\n\n[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)\n[![pypi](https://img.shields.io/pypi/v/nsdpy)](https://pypi.org/project/nsdpy/)\n[![Python 3.8](https://upload.wikimedia.org/wikipedia/commons/a/a5/Blue_Python_3.8_Shield_Badge.svg)](https://www.python.org/)\n[![Documentation Status](https://readthedocs.org/projects/nsdpy/badge/?version=latest)](https://nsdpy.readthedocs.io/en/latest/?badge=latest)\n\n\n\n- [Introduction](#introduction)\n- [Workfolw](#workflow)\n- [Quick start](#quick-start)\n- [Usage](#usage)\n  - [Google Colab](#google-colab)\n  - [Command line](#command-line)\n- [Authors and acknowledgment](#authors-and-acknowledgment)\n- [Support](#support)\n- [Licence](#license)\n- [More Documentation](#more-documentation)\n\n## Introduction\n\nnsdpy (nucleotide or NCBI sequence downloader) aims to ease the download and sort of big bacth of DNA sequences from the NCBI database. \nIt can also be usefull to filter the sequences based on their annotations.\nUsing nsdpy the user can:\n\n- **Search** NCBI nucleotide database\n- **Download** the fasta files or the cds_fasta files corresponding to the result of the search\n- **Sort** the sequences based on their taxonomy\n- **Select** coding sequences from cds files based on the gene names using one or more regular expressions. \nThis can help the user retrieve some sequences for which the gene name is annotated in another field.\n- **Retrieve** the taxonomic information and add it to the output sequences.  \n\n## Quick start\n\n- Clone the repo from Github: \n```bash \ngit clone https://github.com/RaphaelHebert/nsdpy.git\n  ```\n- pip:  \n_depending on the user environment pip may be replaced by pip3 if pip3 is used_\n```bash \npip install nsdpy\n```  \n*minimum python version for nsdpy: 3.8.2* \n\n- Google Colab: save a copy of [this notebook](https://colab.research.google.com/drive/1UmxzRc_k5sNeQ2RPGe29nWR_1_0FRPkq?usp=sharing) in your drive.\n\n## Workflow\n\n<img src="https://docs.google.com/drawings/d/e/2PACX-1vRD4h7l0S57op_4j-5xsz8iv1j1XBliw-jEdtnWOIq-JAU2l8kSV6d1NmkHd5Q4zhUmZCA3SHUSuHJw/pub?w=801&amp;h=744" width="600" />\n\n## Usage\n### Google colab\n\n[nsdpy colab notebook](https://colab.research.google.com/drive/1UmxzRc_k5sNeQ2RPGe29nWR_1_0FRPkq?usp=sharing)\n\n### Command line\n\n```bash\nnsdpy -r "USER\'S REQUEST" [OPTIONS] \n```\n\n## Authors and acknowledgment  \n\n[Raphael Hebert](https://github.com/RaphaelHebert)  \n[Emese Meglecz](https://github.com/meglecz)\n\n\n## Support\n\n## License\n\nCode and documentation copyright 2021 the nsdpy authors. Code released under the MIT License.\n\n## More Documentation\n\nOfficial documentation:  \n[Readthedocs](https://nsdpy.readthedocs.io/en/latest/main.html#overview)\n  \n\n\n\n',
-    'author': 'RaphaelHebert',
-    'author_email': 'raphaelhebert18@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/RaphaelHebert/nsdpy',
-    'py_modules': modules,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<4.0',
-}
 
 
-setup(**setup_kwargs)
```

