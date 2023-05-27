# Comparing `tmp/ckanext-iso19115-0.1.0.tar.gz` & `tmp/ckanext-iso19115-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-iso19115-0.1.0.tar", last modified: Mon Apr 24 12:37:36 2023, max compression
+gzip compressed data, was "ckanext-iso19115-0.1.1.tar", last modified: Sat May 27 15:19:58 2023, max compression
```

## Comparing `ckanext-iso19115-0.1.0.tar` & `ckanext-iso19115-0.1.1.tar`

### file list

```diff
@@ -1,520 +1,520 @@
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.184146 ckanext-iso19115-0.1.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)    34500 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/LICENSE
--rw-r--r--   0 sergey    (1000) sergey    (1000)      220 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/MANIFEST.in
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3983 2023-04-24 12:37:36.184146 ckanext-iso19115-0.1.0/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3336 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/README.md
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.094145 ckanext-iso19115-0.1.0/ckanext/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      221 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/__init__.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.094145 ckanext-iso19115-0.1.0/ckanext/iso19115/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/__init__.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.094145 ckanext-iso19115-0.1.0/ckanext/iso19115/assets/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1982 2023-04-20 14:35:28.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/assets/iso19115-script.js
--rw-r--r--   0 sergey    (1000) sergey    (1000)      755 2022-10-20 16:05:53.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/assets/iso19115-style.css
--rw-r--r--   0 sergey    (1000) sergey    (1000)      313 2022-10-20 16:02:32.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/assets/webassets.yml
--rw-r--r--   0 sergey    (1000) sergey    (1000)    17689 2023-04-20 15:10:15.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/builder.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2712 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/cli.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      324 2023-04-24 12:36:18.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/config_declaration.yaml
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.094145 ckanext-iso19115-0.1.0/ckanext/iso19115/converter/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     9306 2022-10-20 20:12:54.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/converter/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3158 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/converter/helpers.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      684 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/formatter.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3844 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/helpers.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      240 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/interfaces.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.094145 ckanext-iso19115-0.1.0/ckanext/iso19115/logic/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/logic/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1387 2022-10-20 19:05:20.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/logic/action.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.084145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.064145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19110/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.064145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19110/fcc/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.094145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19110/fcc/1.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2125 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19110/fcc/1.0/abstract.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)      386 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19110/fcc/1.0/fcc.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.064145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19110/gfc/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.094145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19110/gfc/1.1/
--rw-r--r--   0 sergey    (1000) sergey    (1000)    22662 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19110/gfc/1.1/exampleInstance.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)    36680 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19110/gfc/1.1/featureCatalogue.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1105 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19110/gfc/1.1/gfc.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.074145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.064145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-2/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.064145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-2/gmi/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.104145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-2/gmi/1.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)    23194 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-2/gmi/1.0/acquisitionInformation.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     8343 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-2/gmi/1.0/contentInformation.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)    11876 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-2/gmi/1.0/dataQualityInformation.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1673 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-2/gmi/1.0/gmi.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2425 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-2/gmi/1.0/metadataEntitySet.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     7268 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-2/gmi/1.0/spatialRepresentationInformation.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.074145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.064145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/cat/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.104145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/cat/1.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1094 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/cat/1.0/cat.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3176 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/cat/1.0/catalogues.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2504 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/cat/1.0/codelistItem.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     7990 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/cat/1.0/crsItem.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1908 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/cat/1.0/uomItem.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.064145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/cit/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.104145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/cit/1.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      568 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/cit/1.0/cit.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2628 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/cit/1.0/cit_invalid.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3120 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/cit/1.0/cit_valid.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)    24147 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/cit/1.0/citation.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)    69580 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/cit/1.0/codelists.xml
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.104145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/cit/2.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      536 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/cit/2.0/cit.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)      985 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/cit/2.0/cit_revised.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)    24458 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/cit/2.0/citation.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)    69580 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/cit/2.0/codelists.xml
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.064145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/gco/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.104145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/gco/1.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)    28570 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/gco/1.0/baseTypes2014.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1488 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/gco/1.0/gco.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.064145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/gcx/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.104145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/gcx/1.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5292 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/gcx/1.0/extendedTypes.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2676 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/gcx/1.0/extendedTypes_autoFromShapeChange.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3291 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/gcx/1.0/gcx.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)      665 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/gcx/1.0/gcx.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.064145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/gex/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.104145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/gex/1.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)    11689 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/gex/1.0/extent.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)      770 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/gex/1.0/gex.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1515 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/gex/1.0/gex_invalid.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     6015 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/gex/1.0/gex_valid.xml
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.064145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/gml/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.104145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/gml/3.2.1/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1076 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/gml/3.2.1/gml.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.064145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/gmw/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.104145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/gmw/1.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     7647 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/gmw/1.0/gmlWrapperTypes2014.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1647 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/gmw/1.0/gmw.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.064145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/lan/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.104145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/lan/1.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      830 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/lan/1.0/lan.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     6397 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/lan/1.0/language.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.064145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mac/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.104145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mac/1.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)    27705 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mac/1.0/acquisitionInformationImagery.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)      529 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mac/1.0/mac.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.114145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mac/2.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)    31317 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mac/2.0/acquisitionInformationImagery.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     6197 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mac/2.0/event.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     8729 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mac/2.0/mac.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)      565 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mac/2.0/mac.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.064145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mas/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.114145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mas/1.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3484 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mas/1.0/applicationSchema.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)      963 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mas/1.0/mas.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.064145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mcc/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.114145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mcc/1.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)    15388 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mcc/1.0/AbstractCommonClasses.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)    47074 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mcc/1.0/codelists.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)    10279 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mcc/1.0/commonClasses.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)      773 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mcc/1.0/mcc.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.064145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mco/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.114145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mco/1.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)    27250 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mco/1.0/codelists.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     9857 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mco/1.0/constraints.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)      772 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mco/1.0/mco.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3303 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mco/1.0/mco_invalid.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5163 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mco/1.0/mco_valid.xml
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.074145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/md1/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.114145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/md1/1.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3291 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/md1/1.0/md1.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1208 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/md1/1.0/md1.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)      385 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/md1/1.0/metadataWExtendedType.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.114145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/md1/2.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3697 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/md1/2.0/md1.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1225 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/md1/2.0/md1.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)      391 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/md1/2.0/metadataWExtendedType.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.074145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/md2/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.114145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/md2/1.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     7315 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/md2/1.0/md2.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2089 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/md2/1.0/md2.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)      385 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/md2/1.0/metadataWithExtensions.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.114145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/md2/2.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     7719 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/md2/2.0/md2.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2115 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/md2/2.0/md2.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)      391 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/md2/2.0/metadataWithExtensions.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.074145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mda/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.114145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mda/1.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)    16887 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mda/1.0/mda.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)      808 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mda/1.0/mda.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     8053 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mda/1.0/metadataApplication.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.114145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mda/2.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)    18555 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mda/2.0/mda.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)      818 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mda/2.0/mda.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     8063 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mda/2.0/metadataApplication.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.074145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mdb/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.114145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mdb/1.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     6129 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mdb/1.0/AppendixD.1MinimalExample.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2130 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mdb/1.0/mdb.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1657 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mdb/1.0/mdb.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3984 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mdb/1.0/mdb_invalid.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3130 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mdb/1.0/mdb_valid.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     6840 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mdb/1.0/metadataBase.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.114145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mdb/2.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2588 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mdb/2.0/mdb.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1932 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mdb/2.0/mdb.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     6851 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mdb/2.0/metadataBase.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.074145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mds/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.124145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mds/1.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)    35846 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mds/1.0/AppendixD.2VectorSmartMapExample.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5968 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mds/1.0/mds.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3486 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mds/1.0/mds.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)      385 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mds/1.0/metadataDataServices.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.124145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mds/2.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     7331 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mds/2.0/mds.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3486 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mds/2.0/mds.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)      385 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mds/2.0/metadataDataServices.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.074145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mdt/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.124145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mdt/1.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     7351 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mdt/1.0/codelists.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4362 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mdt/1.0/mdt.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1215 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mdt/1.0/mdt.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5481 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mdt/1.0/metadataTransfer.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.124145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mdt/2.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     7351 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mdt/2.0/codelists.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4662 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mdt/2.0/mdt.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1219 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mdt/2.0/mdt.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5495 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mdt/2.0/metadataTransfer.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.074145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mex/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.124145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mex/1.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)    19498 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mex/1.0/codelists.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     7911 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mex/1.0/metadataExtension.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)      770 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mex/1.0/mex.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5078 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mex/1.0/mex_invalid.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5550 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mex/1.0/mex_valid.xml
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.074145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mmi/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.124145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mmi/1.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)    15443 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mmi/1.0/codelists.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4323 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mmi/1.0/maintenance.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)      785 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mmi/1.0/mmi.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1382 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mmi/1.0/mmi_invalid.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2053 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mmi/1.0/mmi_valid.xml
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.074145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mpc/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.124145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mpc/1.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      840 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mpc/1.0/mpc.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1888 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mpc/1.0/portrayalCatalogue.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.074145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrc/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.124145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrc/1.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)    21615 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrc/1.0/codelists.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)    21458 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrc/1.0/content.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     8503 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrc/1.0/contentInformationImagery.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1199 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrc/1.0/mrc.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2672 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrc/1.0/mrc_invalid.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3543 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrc/1.0/mrc_valid.xml
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.124145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrc/2.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)    21615 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrc/2.0/codelists.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)    21654 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrc/2.0/content.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     8883 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrc/2.0/contentInformationImagery.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)    13672 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrc/2.0/mrc.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1199 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrc/2.0/mrc.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.074145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrd/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.134145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrd/1.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     8415 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrd/1.0/codelists.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)    13524 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrd/1.0/distribution.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)      804 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrd/1.0/mrd.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1144 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrd/1.0/mrd_invalid.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3690 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrd/1.0/mrd_valid.xml
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.074145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mri/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.134145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mri/1.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)    63662 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mri/1.0/codelists.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)    28519 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mri/1.0/identification.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)      966 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mri/1.0/mri.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3542 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mri/1.0/mri_invalid.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     8115 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mri/1.0/mri_valid.xml
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.074145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrl/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.134145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrl/1.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     7751 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrl/1.0/lineage.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)    10412 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrl/1.0/lineageImagery.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)      816 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrl/1.0/mrl.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.134145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrl/2.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     7751 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrl/2.0/lineage.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)    15790 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrl/2.0/lineageImagery.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)    11514 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrl/2.0/mrl.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)      822 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrl/2.0/mrl.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.074145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrs/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.134145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrs/1.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)    34660 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrs/1.0/codelists.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)      815 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrs/1.0/mrs.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2530 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrs/1.0/referenceSystem.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.074145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/msr/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.134145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/msr/1.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1067 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/msr/1.0/msr.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)    18947 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/msr/1.0/spatialRepresentation.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5793 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/msr/1.0/spatialRepresentationImagery.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.134145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/msr/2.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3816 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/msr/2.0/msr.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1085 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/msr/2.0/msr.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)    19216 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/msr/2.0/spatialRepresentation.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5797 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/msr/2.0/spatialRepresentationImagery.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.074145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/srv/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.134145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/srv/2.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)    17869 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/srv/2.0/codelists.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)    14304 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/srv/2.0/serviceInformation.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)      766 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/srv/2.0/srv.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3106 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/srv/2.0/srv_invalid.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3080 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/srv/2.0/srv_valid.xml
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.074145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.074145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.134145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/cat/
--rw-r--r--   0 sergey    (1000) sergey    (1000)   343012 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/cat/codelists.xml
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.144146 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1298 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/CD_PixelinCell.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5491 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/CI_DateTypeCode.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3666 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/CI_OnLineFunctionCode.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     7611 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/CI_PresentationFormCode.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     6397 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/CI_RoleCode.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1356 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/CI_TelephoneTypeCode.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     9309 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/CS_AxisDirection.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1275 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/CS_RangeMeaning.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3158 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/DCPList.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3303 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/DS_AssociationTypeCode.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4780 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/DS_InitiativeTypeCode.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1382 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/FC_RoleType.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1759 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_CellGeometryTypeCode.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3116 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_ClassificationCode.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3482 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_CoverageContentTypeCode.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5198 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_DatatypeCode.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2609 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_DimensionNameTypeCode.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2613 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_GeometricObjectTypeCode.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3892 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_ImagingConditionCode.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5085 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_KeywordTypeCode.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4764 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_MaintenanceFrequencyCode.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2458 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_MediumFormatCode.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1380 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_ObligationCode.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2110 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_PixelOrientationCode.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5518 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_ProgressCode.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)    13239 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_ReferenceSystemTypeCode.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     6065 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_RestrictionCode.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     8025 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_ScopeCode.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2341 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_SpatialRepresentationTypeCode.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     9218 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_TopicCategoryCode.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3764 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_TopologyLevelCode.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2425 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_BandDefinition.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1457 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_ContextCode.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1734 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_GeometryTypeCode.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1490 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_ObjectiveTypeCode.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1234 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_OperationTypeCode.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2235 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_PolarisationOrientationCode.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1770 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_PriorityCode.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)      821 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_SensorTypeCode.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1443 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_SequenceCode.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1454 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_TransferFunctionTypeCode.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1448 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_TriggerCode.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1258 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/RE_AmendmentType.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1497 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/RE_DecisionStatus.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1506 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/RE_Disposition.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1750 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/RE_ItemStatus.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2277 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/SC_DerivedCRSType.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1752 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/SV_CouplingType.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1489 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/SV_ParameterDirection.xml
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.144146 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/namespaceInformationAndTools/
--rw-r--r--   0 sergey    (1000) sergey    (1000)    53123 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/namespaceInformationAndTools/ISONamespaceInformation.xml
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.074145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19135/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.074145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19135/-2/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.074145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19135/-2/pre/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.144146 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19135/-2/pre/1.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1786 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19135/-2/pre/1.0/abstract.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)      390 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19135/-2/pre/1.0/pre.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.074145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19135/-2/reg/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.144146 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19135/-2/reg/1.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1126 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19135/-2/reg/1.0/reg.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)    26600 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19135/-2/reg/1.0/registration.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.074145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19139/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.154146 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19139/resources/
--rw-r--r--   0 sergey    (1000) sergey    (1000)    44106 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19139/resources/ML_gmxCodelists.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)    16835 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19139/resources/gmiCodelists.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)    97327 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19139/resources/gmxCodelists.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3766 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19139/resources/tcCodelists.xml
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.074145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19155/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.074145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19155/gpi/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.154146 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19155/gpi/1.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      746 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19155/gpi/1.0/gpi.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3870 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19155/gpi/1.0/placeIdentifier.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)      477 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19155/gpi/1.0/point.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)      788 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19155/gpi/1.0/referenceSystem.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2131 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19155/gpi/1.0/sampleGMLApplicationSchema.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4186 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19155/gpi/1.0/sampleGMLApplicationSchema.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.084145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.084145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/-2/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.084145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/-2/dqc/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.154146 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/-2/dqc/1.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1947 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/-2/dqc/1.0/abstract.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)      963 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/-2/dqc/1.0/dqc.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.084145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/-2/dqm/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.154146 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/-2/dqm/1.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     6136 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/-2/dqm/1.0/codelists.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     8465 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/-2/dqm/1.0/dqm.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)      946 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/-2/dqm/1.0/dqm.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3569 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/-2/dqm/1.0/dqm_invalid.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3543 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/-2/dqm/1.0/dqm_valid.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)    14230 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/-2/dqm/1.0/qualityMeasures.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.084145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/-2/mdq/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.154146 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/-2/mdq/1.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4638 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/-2/mdq/1.0/codelists.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)    24482 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/-2/mdq/1.0/dataQualityElement.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     8411 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/-2/mdq/1.0/dataQualityEvaluation.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3723 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/-2/mdq/1.0/dataQualityImagery.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     6522 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/-2/mdq/1.0/dataQualityResult.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     6231 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/-2/mdq/1.0/mdq.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1218 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/-2/mdq/1.0/mdq.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1911 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/-2/mdq/1.0/mdq_invalid.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2961 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/-2/mdq/1.0/mdq_valid.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3718 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/-2/mdq/1.0/metaquality.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.084145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/resources/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.084145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/resources/Codelists/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.154146 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/resources/Codelists/cat/
--rw-r--r--   0 sergey    (1000) sergey    (1000)    12203 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/resources/Codelists/cat/codelists.xml
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.154146 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/resources/Codelists/gml/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2618 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/resources/Codelists/gml/DQM_ValueStructure.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1669 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/resources/Codelists/gml/DQ_EvaluationMethodTypeCode.xml
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.084145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19165/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.084145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19165/gpm/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.154146 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19165/gpm/1.0/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.154146 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19165/gpm/1.0/examples/
--rw-r--r--   0 sergey    (1000) sergey    (1000)    78922 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19165/gpm/1.0/examples/localSchema.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)    78916 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19165/gpm/1.0/examples/of5mv60sd0f279110s1r100ca5-gpm.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)    17207 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19165/gpm/1.0/geospatialPreservationMetadata.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)      520 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19165/gpm/1.0/gpm.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.084145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.084145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.164146 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/
--rw-r--r--   0 sergey    (1000) sergey    (1000)    14905 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/basicTypes.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)    33323 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/coordinateOperations.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)    18420 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/coordinateReferenceSystems.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)    18701 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/coordinateSystems.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)    20827 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/coverage.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)    15923 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/datums.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)    34674 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/deprecatedTypes.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     7137 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/dictionary.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4161 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/direction.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     6807 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/dynamicFeature.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5584 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/feature.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)    11523 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/geometryAggregates.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)    18929 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/geometryBasic0d1d.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     6625 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/geometryBasic2d.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5824 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/geometryComplexes.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)    42649 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/geometryPrimitives.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1076 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/gml.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)    12756 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/gmlBase.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4132 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/grids.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3104 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/measures.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5530 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/observation.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4680 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/referenceSystems.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)    15598 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/temporal.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)    12679 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/temporalReferenceSystems.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     7795 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/temporalTopology.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)    22790 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/topology.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)    12283 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/units.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)    11438 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/valueObjects.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.084145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.084145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.084145 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.164146 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gco/
--rw-r--r--   0 sergey    (1000) sergey    (1000)    22050 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gco/basicTypes.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1159 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gco/gco.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4087 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gco/gcoBase.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.164146 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3188 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/applicationSchema.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)    15521 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/citation.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     6555 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/constraints.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)    11423 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/content.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)    30936 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/dataQuality.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)    11736 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/distribution.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)    11329 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/extent.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     7160 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/freeText.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1170 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/gmd.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)    19751 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/identification.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5983 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/maintenance.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     9289 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/metadataApplication.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5877 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/metadataEntity.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     6429 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/metadataExtension.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2664 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/portrayalCatalogue.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5723 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/referenceSystem.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)    13883 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/spatialRepresentation.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.164146 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gsr/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1180 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gsr/gsr.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2166 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gsr/spatialReferencing.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.164146 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gss/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2700 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gss/geometry.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1166 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gss/gss.xsd
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.164146 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gts/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1173 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gts/gts.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2787 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gts/temporalObjects.xsd
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1773 2023-03-01 20:48:28.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/plugin.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5963 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/presets.yaml
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.174146 ckanext-iso19115-0.1.0/ckanext/iso19115/schematron/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2192 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/schematron/cit.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3229 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/schematron/dqm.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3369 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/schematron/gex.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3915 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/schematron/mco.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5156 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/schematron/mdb.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1464 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/schematron/mdq.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5063 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/schematron/mex.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1465 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/schematron/mmi.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2269 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/schematron/mrc.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1000 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/schematron/mrd.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     9064 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/schematron/mri.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5740 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/schematron/srv.xml
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.084145 ckanext-iso19115-0.1.0/ckanext/iso19115/templates/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.174146 ckanext-iso19115-0.1.0/ckanext/iso19115/templates/iso19115/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      784 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/templates/iso19115/validate.html
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.174146 ckanext-iso19115-0.1.0/ckanext/iso19115/tests/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/tests/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1012 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/tests/conftest.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.174146 ckanext-iso19115-0.1.0/ckanext/iso19115/tests/converter/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/tests/converter/__init__.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.084145 ckanext-iso19115-0.1.0/ckanext/iso19115/tests/examples/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.174146 ckanext-iso19115-0.1.0/ckanext/iso19115/tests/examples/v3.2/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     7062 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/tests/examples/v3.2/basic.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     7740 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/tests/examples/v3.2/complex.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3099 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/tests/examples/v3.2/identification.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4689 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/tests/examples/v3.2/identification_no_category.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3445 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/tests/examples/v3.2/identification_no_geo.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2059 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/tests/examples/v3.2/minimal.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2117 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/tests/examples/v3.2/sch_no_creation_date.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2445 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/tests/examples/v3.2/sch_no_default_locale.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)       55 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/tests/examples/v3.2/sch_no_root.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2421 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/tests/examples/v3.2/sch_non_dataset_scope.xml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1751 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/tests/test_converter.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1188 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/tests/test_plugin.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.174146 ckanext-iso19115-0.1.0/ckanext/iso19115/types/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      473 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/types/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2023 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/types/base.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3833 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/types/cit.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1219 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/types/gco.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      245 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/types/gcx.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1367 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/types/gex.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)    10400 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/types/gml.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      546 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/types/lan.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     7528 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/types/mac.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      566 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/types/mas.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3721 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/types/mcc.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      930 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/types/mco.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3016 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/types/mdb.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4763 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/types/mdq.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      129 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/types/mex.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      854 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/types/mmi.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      298 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/types/mpc.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1763 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/types/mrc.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2696 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/types/mrd.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2236 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/types/mri.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1528 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/types/mrl.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      452 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/types/mrs.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1532 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/types/msr.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1304 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/types/srv.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     8286 2023-04-20 15:09:16.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/utils.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1134 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/ckanext/iso19115/views.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-04-24 12:37:36.184146 ckanext-iso19115-0.1.0/ckanext_iso19115.egg-info/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3983 2023-04-24 12:37:35.000000 ckanext-iso19115-0.1.0/ckanext_iso19115.egg-info/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)    23163 2023-04-24 12:37:36.000000 ckanext-iso19115-0.1.0/ckanext_iso19115.egg-info/SOURCES.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2023-04-24 12:37:35.000000 ckanext-iso19115-0.1.0/ckanext_iso19115.egg-info/dependency_links.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)       65 2023-04-24 12:37:35.000000 ckanext-iso19115-0.1.0/ckanext_iso19115.egg-info/entry_points.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-04-24 12:37:35.000000 ckanext-iso19115-0.1.0/ckanext_iso19115.egg-info/namespace_packages.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)       58 2023-04-24 12:37:35.000000 ckanext-iso19115-0.1.0/ckanext_iso19115.egg-info/requires.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-04-24 12:37:35.000000 ckanext-iso19115-0.1.0/ckanext_iso19115.egg-info/top_level.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)      106 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/pyproject.toml
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-10-20 21:32:30.000000 ckanext-iso19115-0.1.0/requirements.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1654 2023-04-24 12:37:36.184146 ckanext-iso19115-0.1.0/setup.cfg
--rw-r--r--   0 sergey    (1000) sergey    (1000)       38 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.0/setup.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.285524 ckanext-iso19115-0.1.1/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    34500 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/LICENSE
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      220 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/MANIFEST.in
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2334 2023-05-27 15:19:58.285524 ckanext-iso19115-0.1.1/PKG-INFO
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1687 2023-05-27 15:15:33.000000 ckanext-iso19115-0.1.1/README.md
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.225524 ckanext-iso19115-0.1.1/ckanext/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      221 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/__init__.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.225524 ckanext-iso19115-0.1.1/ckanext/iso19115/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/__init__.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.225524 ckanext-iso19115-0.1.1/ckanext/iso19115/assets/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1982 2023-04-20 14:35:28.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/assets/iso19115-script.js
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      755 2022-10-20 16:05:53.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/assets/iso19115-style.css
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      313 2022-10-20 16:02:32.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/assets/webassets.yml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    17643 2023-05-27 15:16:33.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/builder.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2692 2023-05-27 15:16:32.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/cli.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      324 2023-04-24 12:36:18.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/config_declaration.yaml
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.225524 ckanext-iso19115-0.1.1/ckanext/iso19115/converter/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     9205 2023-05-27 15:16:32.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/converter/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3152 2023-05-27 15:16:32.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/converter/helpers.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      685 2023-05-27 15:16:32.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/formatter.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3871 2023-05-27 15:16:32.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/helpers.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      240 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/interfaces.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.225524 ckanext-iso19115-0.1.1/ckanext/iso19115/logic/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/logic/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1651 2023-05-27 15:16:32.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/logic/action.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.225524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.205524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19110/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.205524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19110/fcc/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.225524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19110/fcc/1.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2125 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19110/fcc/1.0/abstract.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      386 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19110/fcc/1.0/fcc.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.205524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19110/gfc/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.225524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19110/gfc/1.1/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    22662 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19110/gfc/1.1/exampleInstance.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    36680 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19110/gfc/1.1/featureCatalogue.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1105 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19110/gfc/1.1/gfc.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.215524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.205524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-2/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.205524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-2/gmi/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.235524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-2/gmi/1.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    23194 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-2/gmi/1.0/acquisitionInformation.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     8343 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-2/gmi/1.0/contentInformation.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    11876 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-2/gmi/1.0/dataQualityInformation.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1673 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-2/gmi/1.0/gmi.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2425 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-2/gmi/1.0/metadataEntitySet.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     7268 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-2/gmi/1.0/spatialRepresentationInformation.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.215524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.205524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/cat/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.235524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/cat/1.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1094 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/cat/1.0/cat.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3176 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/cat/1.0/catalogues.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2504 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/cat/1.0/codelistItem.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     7990 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/cat/1.0/crsItem.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1908 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/cat/1.0/uomItem.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.205524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/cit/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.235524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/cit/1.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      568 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/cit/1.0/cit.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2628 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/cit/1.0/cit_invalid.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3120 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/cit/1.0/cit_valid.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    24147 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/cit/1.0/citation.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    69580 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/cit/1.0/codelists.xml
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.235524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/cit/2.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      536 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/cit/2.0/cit.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      985 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/cit/2.0/cit_revised.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    24458 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/cit/2.0/citation.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    69580 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/cit/2.0/codelists.xml
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.205524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/gco/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.235524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/gco/1.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    28570 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/gco/1.0/baseTypes2014.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1488 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/gco/1.0/gco.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.205524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/gcx/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.235524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/gcx/1.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5292 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/gcx/1.0/extendedTypes.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2676 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/gcx/1.0/extendedTypes_autoFromShapeChange.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3291 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/gcx/1.0/gcx.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      665 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/gcx/1.0/gcx.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.205524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/gex/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.235524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/gex/1.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    11689 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/gex/1.0/extent.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      770 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/gex/1.0/gex.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1515 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/gex/1.0/gex_invalid.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     6015 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/gex/1.0/gex_valid.xml
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.205524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/gml/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.235524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/gml/3.2.1/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1076 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/gml/3.2.1/gml.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.205524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/gmw/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.235524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/gmw/1.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     7647 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/gmw/1.0/gmlWrapperTypes2014.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1647 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/gmw/1.0/gmw.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.205524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/lan/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.235524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/lan/1.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      830 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/lan/1.0/lan.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     6397 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/lan/1.0/language.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.205524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mac/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.235524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mac/1.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    27705 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mac/1.0/acquisitionInformationImagery.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      529 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mac/1.0/mac.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.235524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mac/2.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    31317 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mac/2.0/acquisitionInformationImagery.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     6197 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mac/2.0/event.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     8729 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mac/2.0/mac.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      565 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mac/2.0/mac.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.205524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mas/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.235524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mas/1.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3484 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mas/1.0/applicationSchema.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      963 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mas/1.0/mas.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.205524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mcc/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.235524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mcc/1.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    15388 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mcc/1.0/AbstractCommonClasses.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    47074 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mcc/1.0/codelists.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    10279 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mcc/1.0/commonClasses.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      773 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mcc/1.0/mcc.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.205524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mco/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.235524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mco/1.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    27250 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mco/1.0/codelists.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     9857 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mco/1.0/constraints.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      772 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mco/1.0/mco.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3303 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mco/1.0/mco_invalid.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5163 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mco/1.0/mco_valid.xml
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.205524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/md1/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.235524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/md1/1.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3291 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/md1/1.0/md1.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1208 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/md1/1.0/md1.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      385 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/md1/1.0/metadataWExtendedType.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.235524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/md1/2.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3697 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/md1/2.0/md1.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1225 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/md1/2.0/md1.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      391 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/md1/2.0/metadataWExtendedType.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.215524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/md2/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.235524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/md2/1.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     7315 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/md2/1.0/md2.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2089 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/md2/1.0/md2.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      385 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/md2/1.0/metadataWithExtensions.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.235524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/md2/2.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     7719 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/md2/2.0/md2.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2115 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/md2/2.0/md2.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      391 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/md2/2.0/metadataWithExtensions.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.215524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mda/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.245524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mda/1.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    16887 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mda/1.0/mda.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      808 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mda/1.0/mda.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     8053 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mda/1.0/metadataApplication.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.245524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mda/2.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    18555 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mda/2.0/mda.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      818 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mda/2.0/mda.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     8063 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mda/2.0/metadataApplication.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.215524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mdb/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.245524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mdb/1.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     6129 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mdb/1.0/AppendixD.1MinimalExample.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2130 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mdb/1.0/mdb.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1657 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mdb/1.0/mdb.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3984 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mdb/1.0/mdb_invalid.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3130 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mdb/1.0/mdb_valid.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     6840 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mdb/1.0/metadataBase.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.245524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mdb/2.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2588 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mdb/2.0/mdb.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1932 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mdb/2.0/mdb.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     6851 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mdb/2.0/metadataBase.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.215524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mds/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.245524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mds/1.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    35846 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mds/1.0/AppendixD.2VectorSmartMapExample.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5968 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mds/1.0/mds.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3486 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mds/1.0/mds.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      385 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mds/1.0/metadataDataServices.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.245524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mds/2.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     7331 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mds/2.0/mds.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3486 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mds/2.0/mds.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      385 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mds/2.0/metadataDataServices.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.215524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mdt/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.245524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mdt/1.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     7351 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mdt/1.0/codelists.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4362 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mdt/1.0/mdt.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1215 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mdt/1.0/mdt.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5481 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mdt/1.0/metadataTransfer.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.245524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mdt/2.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     7351 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mdt/2.0/codelists.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4662 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mdt/2.0/mdt.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1219 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mdt/2.0/mdt.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5495 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mdt/2.0/metadataTransfer.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.215524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mex/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.245524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mex/1.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    19498 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mex/1.0/codelists.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     7911 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mex/1.0/metadataExtension.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      770 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mex/1.0/mex.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5078 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mex/1.0/mex_invalid.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5550 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mex/1.0/mex_valid.xml
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.215524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mmi/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.245524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mmi/1.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    15443 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mmi/1.0/codelists.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4323 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mmi/1.0/maintenance.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      785 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mmi/1.0/mmi.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1382 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mmi/1.0/mmi_invalid.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2053 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mmi/1.0/mmi_valid.xml
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.215524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mpc/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.245524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mpc/1.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      840 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mpc/1.0/mpc.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1888 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mpc/1.0/portrayalCatalogue.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.215524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mrc/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.245524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mrc/1.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    21615 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mrc/1.0/codelists.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    21458 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mrc/1.0/content.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     8503 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mrc/1.0/contentInformationImagery.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1199 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mrc/1.0/mrc.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2672 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mrc/1.0/mrc_invalid.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3543 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mrc/1.0/mrc_valid.xml
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.245524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mrc/2.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    21615 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mrc/2.0/codelists.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    21654 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mrc/2.0/content.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     8883 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mrc/2.0/contentInformationImagery.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    13672 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mrc/2.0/mrc.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1199 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mrc/2.0/mrc.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.215524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mrd/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.245524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mrd/1.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     8415 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mrd/1.0/codelists.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    13524 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mrd/1.0/distribution.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      804 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mrd/1.0/mrd.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1144 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mrd/1.0/mrd_invalid.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3690 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mrd/1.0/mrd_valid.xml
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.215524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mri/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.245524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mri/1.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    63662 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mri/1.0/codelists.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    28519 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mri/1.0/identification.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      966 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mri/1.0/mri.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3542 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mri/1.0/mri_invalid.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     8115 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mri/1.0/mri_valid.xml
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.215524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mrl/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.255524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mrl/1.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     7751 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mrl/1.0/lineage.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    10412 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mrl/1.0/lineageImagery.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      816 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mrl/1.0/mrl.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.255524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mrl/2.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     7751 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mrl/2.0/lineage.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    15790 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mrl/2.0/lineageImagery.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    11514 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mrl/2.0/mrl.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      822 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mrl/2.0/mrl.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.215524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mrs/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.255524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mrs/1.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    34660 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mrs/1.0/codelists.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      815 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mrs/1.0/mrs.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2530 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mrs/1.0/referenceSystem.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.215524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/msr/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.255524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/msr/1.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1067 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/msr/1.0/msr.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    18947 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/msr/1.0/spatialRepresentation.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5793 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/msr/1.0/spatialRepresentationImagery.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.255524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/msr/2.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3816 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/msr/2.0/msr.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1085 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/msr/2.0/msr.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    19216 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/msr/2.0/spatialRepresentation.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5797 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/msr/2.0/spatialRepresentationImagery.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.215524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/srv/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.255524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/srv/2.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    17869 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/srv/2.0/codelists.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    14304 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/srv/2.0/serviceInformation.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      766 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/srv/2.0/srv.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3106 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/srv/2.0/srv_invalid.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3080 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/srv/2.0/srv_valid.xml
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.215524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.215524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.255524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/cat/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)   343012 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/cat/codelists.xml
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.265524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1298 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/CD_PixelinCell.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5491 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/CI_DateTypeCode.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3666 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/CI_OnLineFunctionCode.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     7611 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/CI_PresentationFormCode.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     6397 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/CI_RoleCode.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1356 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/CI_TelephoneTypeCode.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     9309 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/CS_AxisDirection.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1275 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/CS_RangeMeaning.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3158 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/DCPList.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3303 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/DS_AssociationTypeCode.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4780 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/DS_InitiativeTypeCode.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1382 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/FC_RoleType.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1759 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_CellGeometryTypeCode.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3116 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_ClassificationCode.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3482 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_CoverageContentTypeCode.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5198 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_DatatypeCode.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2609 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_DimensionNameTypeCode.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2613 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_GeometricObjectTypeCode.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3892 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_ImagingConditionCode.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5085 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_KeywordTypeCode.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4764 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_MaintenanceFrequencyCode.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2458 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_MediumFormatCode.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1380 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_ObligationCode.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2110 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_PixelOrientationCode.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5518 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_ProgressCode.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    13239 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_ReferenceSystemTypeCode.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     6065 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_RestrictionCode.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     8025 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_ScopeCode.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2341 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_SpatialRepresentationTypeCode.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     9218 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_TopicCategoryCode.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3764 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_TopologyLevelCode.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2425 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_BandDefinition.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1457 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_ContextCode.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1734 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_GeometryTypeCode.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1490 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_ObjectiveTypeCode.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1234 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_OperationTypeCode.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2235 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_PolarisationOrientationCode.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1770 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_PriorityCode.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      821 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_SensorTypeCode.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1443 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_SequenceCode.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1454 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_TransferFunctionTypeCode.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1448 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_TriggerCode.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1258 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/RE_AmendmentType.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1497 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/RE_DecisionStatus.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1506 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/RE_Disposition.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1750 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/RE_ItemStatus.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2277 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/SC_DerivedCRSType.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1752 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/SV_CouplingType.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1489 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/SV_ParameterDirection.xml
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.265524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/namespaceInformationAndTools/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    53123 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/namespaceInformationAndTools/ISONamespaceInformation.xml
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.215524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19135/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.215524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19135/-2/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.215524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19135/-2/pre/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.265524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19135/-2/pre/1.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1786 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19135/-2/pre/1.0/abstract.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      390 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19135/-2/pre/1.0/pre.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.215524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19135/-2/reg/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.265524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19135/-2/reg/1.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1126 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19135/-2/reg/1.0/reg.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    26600 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19135/-2/reg/1.0/registration.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.215524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19139/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.265524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19139/resources/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    44106 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19139/resources/ML_gmxCodelists.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    16835 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19139/resources/gmiCodelists.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    97327 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19139/resources/gmxCodelists.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3766 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19139/resources/tcCodelists.xml
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.215524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19155/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.215524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19155/gpi/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.265524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19155/gpi/1.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      746 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19155/gpi/1.0/gpi.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3870 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19155/gpi/1.0/placeIdentifier.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      477 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19155/gpi/1.0/point.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      788 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19155/gpi/1.0/referenceSystem.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2131 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19155/gpi/1.0/sampleGMLApplicationSchema.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4186 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19155/gpi/1.0/sampleGMLApplicationSchema.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.225524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19157/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.215524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19157/-2/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.215524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19157/-2/dqc/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.265524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19157/-2/dqc/1.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1947 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19157/-2/dqc/1.0/abstract.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      963 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19157/-2/dqc/1.0/dqc.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.215524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19157/-2/dqm/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.265524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19157/-2/dqm/1.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     6136 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19157/-2/dqm/1.0/codelists.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     8465 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19157/-2/dqm/1.0/dqm.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      946 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19157/-2/dqm/1.0/dqm.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3569 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19157/-2/dqm/1.0/dqm_invalid.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3543 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19157/-2/dqm/1.0/dqm_valid.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    14230 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19157/-2/dqm/1.0/qualityMeasures.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.215524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19157/-2/mdq/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.265524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19157/-2/mdq/1.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4638 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19157/-2/mdq/1.0/codelists.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    24482 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19157/-2/mdq/1.0/dataQualityElement.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     8411 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19157/-2/mdq/1.0/dataQualityEvaluation.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3723 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19157/-2/mdq/1.0/dataQualityImagery.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     6522 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19157/-2/mdq/1.0/dataQualityResult.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     6231 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19157/-2/mdq/1.0/mdq.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1218 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19157/-2/mdq/1.0/mdq.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1911 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19157/-2/mdq/1.0/mdq_invalid.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2961 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19157/-2/mdq/1.0/mdq_valid.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3718 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19157/-2/mdq/1.0/metaquality.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.225524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19157/resources/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.225524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19157/resources/Codelists/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.265524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19157/resources/Codelists/cat/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    12203 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19157/resources/Codelists/cat/codelists.xml
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.265524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19157/resources/Codelists/gml/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2618 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19157/resources/Codelists/gml/DQM_ValueStructure.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1669 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19157/resources/Codelists/gml/DQ_EvaluationMethodTypeCode.xml
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.225524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19165/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.225524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19165/gpm/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.265524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19165/gpm/1.0/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.265524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19165/gpm/1.0/examples/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    78922 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19165/gpm/1.0/examples/localSchema.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    78916 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19165/gpm/1.0/examples/of5mv60sd0f279110s1r100ca5-gpm.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    17207 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19165/gpm/1.0/geospatialPreservationMetadata.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      520 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19165/gpm/1.0/gpm.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.225524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.225524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/gml/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.275524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    14905 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/basicTypes.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    33323 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/coordinateOperations.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    18420 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/coordinateReferenceSystems.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    18701 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/coordinateSystems.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    20827 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/coverage.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    15923 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/datums.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    34674 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/deprecatedTypes.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     7137 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/dictionary.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4161 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/direction.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     6807 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/dynamicFeature.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5584 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/feature.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    11523 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/geometryAggregates.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    18929 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/geometryBasic0d1d.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     6625 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/geometryBasic2d.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5824 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/geometryComplexes.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    42649 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/geometryPrimitives.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1076 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/gml.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    12756 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/gmlBase.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4132 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/grids.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3104 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/measures.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5530 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/observation.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4680 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/referenceSystems.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    15598 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/temporal.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    12679 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/temporalReferenceSystems.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     7795 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/temporalTopology.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    22790 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/topology.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    12283 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/units.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    11438 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/valueObjects.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.225524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/iso/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.225524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.225524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.275524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gco/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    22050 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gco/basicTypes.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1159 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gco/gco.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4087 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gco/gcoBase.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.275524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3188 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/applicationSchema.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    15521 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/citation.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     6555 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/constraints.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    11423 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/content.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    30936 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/dataQuality.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    11736 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/distribution.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    11329 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/extent.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     7160 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/freeText.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1170 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/gmd.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    19751 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/identification.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5983 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/maintenance.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     9289 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/metadataApplication.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5877 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/metadataEntity.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     6429 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/metadataExtension.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2664 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/portrayalCatalogue.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5723 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/referenceSystem.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    13883 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/spatialRepresentation.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.275524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gsr/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1180 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gsr/gsr.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2166 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gsr/spatialReferencing.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.275524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gss/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2700 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gss/geometry.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1166 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gss/gss.xsd
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.275524 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gts/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1173 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gts/gts.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2787 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gts/temporalObjects.xsd
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1773 2023-05-27 15:16:32.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/plugin.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5963 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/presets.yaml
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.275524 ckanext-iso19115-0.1.1/ckanext/iso19115/schematron/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2192 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/schematron/cit.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3229 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/schematron/dqm.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3369 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/schematron/gex.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3915 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/schematron/mco.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5156 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/schematron/mdb.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1464 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/schematron/mdq.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5063 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/schematron/mex.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1465 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/schematron/mmi.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2269 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/schematron/mrc.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1000 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/schematron/mrd.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     9064 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/schematron/mri.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5740 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/schematron/srv.xml
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.225524 ckanext-iso19115-0.1.1/ckanext/iso19115/templates/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.275524 ckanext-iso19115-0.1.1/ckanext/iso19115/templates/iso19115/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      784 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/templates/iso19115/validate.html
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.285524 ckanext-iso19115-0.1.1/ckanext/iso19115/tests/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/tests/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      996 2023-05-27 15:16:32.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/tests/conftest.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.285524 ckanext-iso19115-0.1.1/ckanext/iso19115/tests/converter/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/tests/converter/__init__.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.225524 ckanext-iso19115-0.1.1/ckanext/iso19115/tests/examples/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.285524 ckanext-iso19115-0.1.1/ckanext/iso19115/tests/examples/v3.2/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     7062 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/tests/examples/v3.2/basic.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     7740 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/tests/examples/v3.2/complex.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3099 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/tests/examples/v3.2/identification.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4689 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/tests/examples/v3.2/identification_no_category.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3445 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/tests/examples/v3.2/identification_no_geo.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2059 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/tests/examples/v3.2/minimal.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2117 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/tests/examples/v3.2/sch_no_creation_date.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2445 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/tests/examples/v3.2/sch_no_default_locale.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       55 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/tests/examples/v3.2/sch_no_root.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2421 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/tests/examples/v3.2/sch_non_dataset_scope.xml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1707 2023-05-27 15:16:32.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/tests/test_converter.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1188 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/tests/test_plugin.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.285524 ckanext-iso19115-0.1.1/ckanext/iso19115/types/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      473 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/types/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2022 2023-05-27 15:16:32.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/types/base.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3777 2023-05-27 15:16:32.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/types/cit.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1220 2023-05-27 15:16:32.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/types/gco.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      245 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/types/gcx.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1353 2023-05-27 15:16:32.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/types/gex.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    10350 2023-05-27 15:16:32.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/types/gml.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      546 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/types/lan.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     7430 2023-05-27 15:16:32.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/types/mac.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      566 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/types/mas.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3595 2023-05-27 15:16:32.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/types/mcc.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      930 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/types/mco.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2918 2023-05-27 15:16:32.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/types/mdb.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4637 2023-05-27 15:16:32.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/types/mdq.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      129 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/types/mex.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      812 2023-05-27 15:16:32.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/types/mmi.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      284 2023-05-27 15:16:32.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/types/mpc.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1721 2023-05-27 15:16:32.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/types/mrc.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2626 2023-05-27 15:16:32.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/types/mrd.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2222 2023-05-27 15:16:32.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/types/mri.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1472 2023-05-27 15:16:32.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/types/mrl.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      437 2023-05-27 15:16:32.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/types/mrs.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1518 2023-05-27 15:16:32.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/types/msr.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1276 2023-05-27 15:16:32.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/types/srv.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     8135 2023-05-27 15:16:32.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/utils.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1128 2023-05-27 15:16:32.000000 ckanext-iso19115-0.1.1/ckanext/iso19115/views.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-05-27 15:19:58.285524 ckanext-iso19115-0.1.1/ckanext_iso19115.egg-info/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2334 2023-05-27 15:19:58.000000 ckanext-iso19115-0.1.1/ckanext_iso19115.egg-info/PKG-INFO
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    23163 2023-05-27 15:19:58.000000 ckanext-iso19115-0.1.1/ckanext_iso19115.egg-info/SOURCES.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2023-05-27 15:19:58.000000 ckanext-iso19115-0.1.1/ckanext_iso19115.egg-info/dependency_links.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       65 2023-05-27 15:19:58.000000 ckanext-iso19115-0.1.1/ckanext_iso19115.egg-info/entry_points.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-05-27 15:19:58.000000 ckanext-iso19115-0.1.1/ckanext_iso19115.egg-info/namespace_packages.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       58 2023-05-27 15:19:58.000000 ckanext-iso19115-0.1.1/ckanext_iso19115.egg-info/requires.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-05-27 15:19:58.000000 ckanext-iso19115-0.1.1/ckanext_iso19115.egg-info/top_level.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4164 2023-05-27 15:16:29.000000 ckanext-iso19115-0.1.1/pyproject.toml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-10-20 21:32:30.000000 ckanext-iso19115-0.1.1/requirements.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1654 2023-05-27 15:19:58.285524 ckanext-iso19115-0.1.1/setup.cfg
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       38 2022-10-20 12:15:36.000000 ckanext-iso19115-0.1.1/setup.py
```

### Comparing `ckanext-iso19115-0.1.0/LICENSE` & `ckanext-iso19115-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/assets/iso19115-script.js` & `ckanext-iso19115-0.1.1/ckanext/iso19115/assets/iso19115-script.js`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/assets/iso19115-style.css` & `ckanext-iso19115-0.1.1/ckanext/iso19115/assets/iso19115-style.css`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/builder.py` & `ckanext-iso19115-0.1.1/ckanext/iso19115/builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,17 +119,15 @@
         self,
         fmt,
         skip_optional,
         qualified: bool = True,
         max_depth: int = 0,
         annotated: bool = False,
     ):
-        tree = DfsTree(
-            self.root, skip_optional, qualified, max_depth, annotated
-        )
+        tree = DfsTree(self.root, skip_optional, qualified, max_depth, annotated)
         if fmt == "overview":
             print(tree)
         elif fmt == "dataclass":
             tree.max_depth = 2
             print_dataclass(tree)
 
     def implementations(self) -> list[BaseNode]:
@@ -228,21 +226,18 @@
             if n is node:
                 yield n
             else:
                 yield from self._yield_from_node(n)
 
         with node.visit() as children:
             for child in children:
-
                 yield from self._yield_from_node(child)
 
     def __str__(self):
-        return "\n".join(
-            n.into_indent(self.qualified, self.annotated) for n in self
-        )
+        return "\n".join(n.into_indent(self.qualified, self.annotated) for n in self)
 
 
 def make_node(node: XsdType) -> BaseNode:
     if isinstance(node, XsdElement):
         return ElementNode(node)
     if isinstance(node, XsdAtomic):
         return AtomicNode(node)
@@ -548,15 +543,14 @@
 
     def is_composed(self):
         return False
 
 
 class ElementNode(BaseNode):
     def __init__(self, node: XsdElement):
-
         if node.abstract:
             children = self._resolve_substitutions(node)
         else:
             type_ = node.type
             if isinstance(type_, XsdComplexType):
                 type_ = type_.content
             if isinstance(type_, (XsdGroup, XsdList, XsdAtomic, XsdUnion)):
```

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/cli.py` & `ckanext-iso19115-0.1.1/ckanext/iso19115/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,17 +28,15 @@
 
 
 @build.command("xml")
 @click.argument("source", type=click.File("r"), default=sys.stdin)
 def build_xml(source):
     content = bytes(source.read(), "utf8")
     b = utils.get_builder("mdb:MD_Metadata")
-    xml = xmlschema.etree_tostring(
-        b.build(json.loads(content)), namespaces=utils.ns
-    )
+    xml = xmlschema.etree_tostring(b.build(json.loads(content)), namespaces=utils.ns)
 
     click.echo(xml)
 
 
 @build.command("describe")
 @click.option("-r", "--root", default="mdb:MD_Metadata")
 @click.option("-s", "--skip-optional", is_flag=True)
@@ -61,17 +59,15 @@
 ):
     b = utils.get_builder(root)
     b.print_tree(format, skip_optional, qualified, max_depth, annotated)
 
 
 @build.command("example")
 @click.option("-r", "--root", default="mdb:MD_Metadata")
-@click.option(
-    "-f", "--format", type=click.Choice(["json", "xml"]), default="json"
-)
+@click.option("-f", "--format", type=click.Choice(["json", "xml"]), default="json")
 @click.option(
     "--seed",
 )
 @click.option("-s", "--skip-optional", is_flag=True)
 @click.option("-d", "--max-depth", type=int, default=0)
 def build_example(
     root: str,
```

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/converter/__init__.py` & `ckanext-iso19115-0.1.1/ckanext/iso19115/converter/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,17 +60,15 @@
 
     def build(self):
         result = jml(self.data)
         return result
 
     def _add_identifier(self):
         mcc.MD_Identifier
-        identifier: mcc.MD_Identifier = h.id(
-            self.pkg["id"], codeSpace="urn:uuid"
-        )
+        identifier: mcc.MD_Identifier = h.id(self.pkg["id"], codeSpace="urn:uuid")
         self.data.metadataIdentifier = identifier
 
     def _add_default_locale(self):
         lan.PT_Locale
         locale = h.locale(
             self.pkg.get("language") or tk.config.get("ckan.locale_default")
         )
@@ -87,15 +85,14 @@
         )
 
         self.data.metadataScope.append(scope)
 
     def _add_contacts(self):
         cit.CI_Responsibility
         for contact in self.pkg.get("contact", []):
-
             ind = cit.CI_Individual(
                 name=h.cs(contact.get("inidvidual")),
                 positionName=h.cs(contact.get("position")),
             )
             org = h.org(
                 contact.get("name"),
                 contactInfo=[
@@ -117,17 +114,15 @@
 
     def _add_dates(self):
         cit.CI_Date
         has_creation = False
 
         for date in self.pkg.get("date_info", []):
             self.data.add_dateInfo(
-                cit.CI_Date(
-                    h.date(date["date"]), cit.CI_DateTypeCode(date["type"])
-                )
+                cit.CI_Date(h.date(date["date"]), cit.CI_DateTypeCode(date["type"]))
             )
             if date["type"] == "creation":
                 has_creation = True
 
         if not has_creation:
             creation = self.pkg["metadata_created"]
 
@@ -182,15 +177,17 @@
         mcc.Abstract_ResourceDescription
         mri.MD_DataIdentification
         srv.SV_ServiceIdentification
 
         citation: cit.CI_Citation = h.citation(
             self.pkg["title"], identifier=h.id(self.pkg["id"])
         )
-        kw = [h.keyword(t if isinstance(t, str) else t['name']) for t in self.pkg["tags"]]
+        kw = [
+            h.keyword(t if isinstance(t, str) else t["name"]) for t in self.pkg["tags"]
+        ]
 
         ident: mri.MD_DataIdentification = mri.MD_DataIdentification(
             citation,
             self.pkg["notes"],
             descriptiveKeywords=kw,
         )
         self.data.add_identificationInfo(ident)
@@ -227,17 +224,15 @@
         for dq in self.pkg.get("data_quality", []):
             result = mdq.DQ_DescriptiveResult(
                 statement=h.cs(dq.get("details") or "...")
             )
             if "date" in dq:
                 result.dateTime = h.date(dq["date"], True)
 
-            report: mdq.AbstractDQ_Element = h.make(
-                dq["type"], result=[result]
-            )
+            report: mdq.AbstractDQ_Element = h.make(dq["type"], result=[result])
 
             self.data.dataQualityInfo.append(
                 mdq.DQ_DataQuality(
                     scope=mcc.MD_Scope(mcc.MD_ScopeCode("dataset")),
                     report=[report],
                 )
             )
@@ -295,17 +290,15 @@
 
             if not dataclasses.is_dataclass(element):
                 if is_cs(field):
                     element = h.cs(element)
                 elif is_codelist(field):
                     element = h.codelist(field, element)
 
-            content = (
-                jml(element) if dataclasses.is_dataclass(element) else element
-            )
+            content = jml(element) if dataclasses.is_dataclass(element) else element
             if content != []:
                 child.append(content)
             child.refine_attributes()
 
     data.refine_attributes()
     return data
```

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/converter/helpers.py` & `ckanext-iso19115-0.1.1/ckanext/iso19115/converter/helpers.py`

 * *Files 5% similar despite different names*

```diff
@@ -86,17 +86,15 @@
     return cit.CI_Individual(cs(name), **kwargs)
 
 
 def org(name: str, **kwargs) -> cit.CI_Organisation:
     return cit.CI_Organisation(cs(name), **kwargs)
 
 
-def responsibility(
-    role: str, party: cit.AbstractCI_Party
-) -> cit.CI_Responsibility:
+def responsibility(role: str, party: cit.AbstractCI_Party) -> cit.CI_Responsibility:
     return cit.CI_Responsibility(cit.CI_RoleCode(role), party=[party])
 
 
 def citation(title: str, **kwargs):
     return cit.CI_Citation(cs(title), **kwargs)
```

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/formatter.py` & `ckanext-iso19115-0.1.1/ckanext/iso19115/formatter.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,9 +18,10 @@
         xml = xmlschema.etree_tostring(el, namespaces=ns)
         return xml
 
 
 class Iso19115Html(HTMLFormat):
     pass
 
+
 class Iso19115Pdf(PDFFormat):
     pass
```

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/helpers.py` & `ckanext-iso19115-0.1.1/ckanext/iso19115/helpers.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 CONFIG_ALLOWED = "ckanext.iso19115.options.allowed"
 
 DEFAULT_ALLOWED = []
 DEFAULT_LANGUAGES = "eng"
 
 log = logging.getLogger(__name__)
 
+
 def get_helpers():
     return {
         "iso19115_implementation_as_options": implementations,
         "iso19115_codelist_as_options": codelist,
         "iso19115_languages": languages,
         "iso19115_option_label": option_label,
     }
@@ -38,17 +39,15 @@
     return _get_languages()
 
 
 @functools.lru_cache(1)
 def _get_languages() -> list[AnnotatedOption]:
     supported = tk.aslist(tk.config.get(CONFIG_LANGUAGES, DEFAULT_LANGUAGES))
     languages = (
-        map(pycountry.languages.lookup, supported)
-        if supported
-        else pycountry.languages
+        map(pycountry.languages.lookup, supported) if supported else pycountry.languages
     )
 
     return [
         AnnotatedOption(value=l.alpha_3, label=l.name, annotation=None)
         for l in languages
     ]
 
@@ -61,79 +60,87 @@
     options = []
     for impl in base.implementations():
         name = impl.name(False)
         if not name:
             continue
         label = _uncamelize(name.split(":")[-1].replace("_", " "))
         options.append(
-            AnnotatedOption(
-                value=name, label=label, annotation=impl.annotation()
-            )
+            AnnotatedOption(value=name, label=label, annotation=impl.annotation())
         )
 
     return options
 
 
 def implementations(field: dict[str, Any]):
     source = field["iso19115_source"]
-    allowed = set(tk.aslist(tk.config.get(CONFIG_ALLOWED + "." + source.replace(":", "."), DEFAULT_ALLOWED)))
+    allowed = set(
+        tk.aslist(
+            tk.config.get(
+                CONFIG_ALLOWED + "." + source.replace(":", "."), DEFAULT_ALLOWED
+            )
+        )
+    )
     options = _get_implementations(source)
 
     if allowed:
-        options = [
-            o for o in options
-            if o["value"] in allowed
-        ]
+        options = [o for o in options if o["value"] in allowed]
     return options
 
+
 @functools.lru_cache()
 def _get_codelist(name: str) -> list[AnnotatedOption]:
     return [
         AnnotatedOption(
             value=code.name,
             label=_uncamelize(code.name).capitalize(),
             annotation=code.definition,
         )
         for code in utils.codelist_options(name)
     ]
 
 
 def codelist(field: dict[str, Any]):
     source = field["iso19115_source"]
-    allowed = set(tk.aslist(tk.config.get(CONFIG_ALLOWED + "." + source.replace(":", "."), DEFAULT_ALLOWED)))
+    allowed = set(
+        tk.aslist(
+            tk.config.get(
+                CONFIG_ALLOWED + "." + source.replace(":", "."), DEFAULT_ALLOWED
+            )
+        )
+    )
     options = _get_codelist(source)
     if allowed:
-        options = [
-            o for o in options
-            if o["value"] in allowed
-        ]
+        options = [o for o in options if o["value"] in allowed]
     return options
 
+
 def _uncamelize(v):
     return _swap_case.sub(" ", v)
 
 
-def option_label(type_: str, field: Union[str, list[str]], value: str, entity: str = "dataset"):
+def option_label(
+    type_: str, field: Union[str, list[str]], value: str, entity: str = "dataset"
+):
     schema = tk.h.scheming_get_schema(entity, type_)
     if not schema:
         log.warning("Schema for %s type %s is not defined", entity, type_)
         return value
 
     if isinstance(field, str):
         field = [field]
-    fields = schema['dataset_fields']
+    fields = schema["dataset_fields"]
     field_data = {}
 
     for step in field:
         field_data = tk.h.scheming_field_by_name(fields, step)
         if not field_data:
             log.warning("Field %s is not defined inside %s schema", field, type_)
             return value
         if "repeating_subfields" in field_data:
-            fields = field_data['repeating_subfields']
+            fields = field_data["repeating_subfields"]
 
     choices = tk.h.scheming_field_choices(field_data)
     if not choices:
         log.warning("Field %s from the %s schema does not have choices", field, type_)
         return value
 
     return tk.h.scheming_choices_label(choices, value)
```

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/logic/action.py` & `ckanext-iso19115-0.1.1/ckanext/iso19115/logic/action.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 from datetime import datetime
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Any
 
 import ckan.plugins as p
 import ckan.plugins.toolkit as tk
 
 from xmlschema import etree_tostring
 import ckanext.iso19115.utils as u
 import ckanext.iso19115.converter as c
@@ -21,35 +21,43 @@
         "iso19115_package_check": package_check,
     }
 
 
 @tk.side_effect_free
 def package_check(context, data_dict):
     pkg = tk.get_action("iso19115_package_show")(context, data_dict)
-    builder = u.get_builder("mdb:MD_Metadata")
-
-    xml = builder.build(pkg)
-    content = bytes(etree_tostring(xml, namespaces=u.ns), "utf8")
+    content = _pkg_into_xml(pkg)
     u.validate_schema(content, validate_codelists=True)
     u.validate_schematron(content)
 
     return True
 
 
 @tk.side_effect_free
 def package_show(context, data_dict):
-    implementations = iter(p.PluginImplementations(IIso19115))
-    conv: c.Converter = next(implementations).iso19115_metadata_converter(
-        data_dict
-    )
+    if data_dict.get("format") == "xml":
+        pkg = tk.get_action("iso19115_package_show")(
+            context, {"id": tk.get_or_bust(data_dict, "id")}
+        )
+        return _pkg_into_xml(pkg)
 
     pkg = tk.get_action("package_show")(context, data_dict)
+
+    implementations = iter(p.PluginImplementations(IIso19115))
+    conv: c.Converter = next(implementations).iso19115_metadata_converter(data_dict)
     conv.initialize(pkg)
     conv.process()
     conv.finalize()
 
     try:
         result = conv.build()
     except ValueError as e:
         raise tk.ValidationError({"schema": [str(e)]})
 
     return result
+
+
+def _pkg_into_xml(pkg: dict[str, Any]):
+    builder = u.get_builder("mdb:MD_Metadata")
+
+    xml = builder.build(pkg)
+    return bytes(etree_tostring(xml, namespaces=u.ns), "utf8")
```

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19110/fcc/1.0/abstract.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19110/fcc/1.0/abstract.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19110/gfc/1.1/exampleInstance.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19110/gfc/1.1/exampleInstance.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19110/gfc/1.1/featureCatalogue.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19110/gfc/1.1/featureCatalogue.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19110/gfc/1.1/gfc.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19110/gfc/1.1/gfc.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-2/gmi/1.0/acquisitionInformation.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-2/gmi/1.0/acquisitionInformation.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-2/gmi/1.0/contentInformation.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-2/gmi/1.0/contentInformation.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-2/gmi/1.0/dataQualityInformation.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-2/gmi/1.0/dataQualityInformation.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-2/gmi/1.0/gmi.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-2/gmi/1.0/gmi.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-2/gmi/1.0/metadataEntitySet.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-2/gmi/1.0/metadataEntitySet.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-2/gmi/1.0/spatialRepresentationInformation.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-2/gmi/1.0/spatialRepresentationInformation.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/cat/1.0/cat.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/cat/1.0/cat.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/cat/1.0/catalogues.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/cat/1.0/catalogues.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/cat/1.0/codelistItem.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/cat/1.0/codelistItem.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/cat/1.0/crsItem.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/cat/1.0/crsItem.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/cat/1.0/uomItem.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/cat/1.0/uomItem.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/cit/1.0/cit.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/cit/1.0/cit.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/cit/1.0/cit_invalid.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/cit/1.0/cit_invalid.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/cit/1.0/cit_valid.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/cit/1.0/cit_valid.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/cit/1.0/citation.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/cit/1.0/citation.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/cit/1.0/codelists.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/cit/1.0/codelists.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/cit/2.0/cit.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/cit/2.0/cit.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/cit/2.0/cit_revised.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/cit/2.0/cit_revised.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/cit/2.0/citation.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/cit/2.0/citation.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/cit/2.0/codelists.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/cit/2.0/codelists.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/gco/1.0/baseTypes2014.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/gco/1.0/baseTypes2014.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/gco/1.0/gco.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/gco/1.0/gco.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/gcx/1.0/extendedTypes.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/gcx/1.0/extendedTypes.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/gcx/1.0/extendedTypes_autoFromShapeChange.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/gcx/1.0/extendedTypes_autoFromShapeChange.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/gcx/1.0/gcx.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/gcx/1.0/gcx.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/gcx/1.0/gcx.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/gcx/1.0/gcx.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/gex/1.0/extent.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/gex/1.0/extent.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/gex/1.0/gex.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/gex/1.0/gex.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/gex/1.0/gex_invalid.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/gex/1.0/gex_invalid.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/gex/1.0/gex_valid.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/gex/1.0/gex_valid.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/gml/3.2.1/gml.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/gml/3.2.1/gml.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/gmw/1.0/gmlWrapperTypes2014.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/gmw/1.0/gmlWrapperTypes2014.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/gmw/1.0/gmw.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/gmw/1.0/gmw.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/lan/1.0/lan.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/lan/1.0/lan.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/lan/1.0/language.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/lan/1.0/language.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mac/1.0/acquisitionInformationImagery.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mac/1.0/acquisitionInformationImagery.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mac/1.0/mac.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mac/1.0/mac.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mac/2.0/acquisitionInformationImagery.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mac/2.0/acquisitionInformationImagery.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mac/2.0/event.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mac/2.0/event.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mac/2.0/mac.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mac/2.0/mac.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mac/2.0/mac.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mac/2.0/mac.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mas/1.0/applicationSchema.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mas/1.0/applicationSchema.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mas/1.0/mas.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mas/1.0/mas.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mcc/1.0/AbstractCommonClasses.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mcc/1.0/AbstractCommonClasses.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mcc/1.0/codelists.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mcc/1.0/codelists.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mcc/1.0/commonClasses.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mcc/1.0/commonClasses.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mcc/1.0/mcc.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mcc/1.0/mcc.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mco/1.0/codelists.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mco/1.0/codelists.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mco/1.0/constraints.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mco/1.0/constraints.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mco/1.0/mco.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mco/1.0/mco.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mco/1.0/mco_invalid.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mco/1.0/mco_invalid.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mco/1.0/mco_valid.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mco/1.0/mco_valid.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/md1/1.0/md1.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/md1/1.0/md1.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/md1/1.0/md1.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/md1/1.0/md1.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/md1/2.0/md1.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/md1/2.0/md1.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/md1/2.0/md1.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/md1/2.0/md1.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/md2/1.0/md2.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/md2/1.0/md2.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/md2/1.0/md2.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/md2/1.0/md2.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/md2/2.0/md2.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/md2/2.0/md2.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/md2/2.0/md2.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/md2/2.0/md2.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mda/1.0/mda.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mda/1.0/mda.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mda/1.0/mda.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mda/1.0/mda.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mda/1.0/metadataApplication.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mda/1.0/metadataApplication.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mda/2.0/mda.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mda/2.0/mda.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mda/2.0/mda.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mda/2.0/mda.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mda/2.0/metadataApplication.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mda/2.0/metadataApplication.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mdb/1.0/AppendixD.1MinimalExample.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mdb/1.0/AppendixD.1MinimalExample.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mdb/1.0/mdb.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mdb/1.0/mdb.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mdb/1.0/mdb.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mdb/1.0/mdb.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mdb/1.0/mdb_invalid.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mdb/1.0/mdb_invalid.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mdb/1.0/mdb_valid.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mdb/1.0/mdb_valid.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mdb/1.0/metadataBase.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mdb/1.0/metadataBase.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mdb/2.0/mdb.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mdb/2.0/mdb.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mdb/2.0/mdb.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mdb/2.0/mdb.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mdb/2.0/metadataBase.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mdb/2.0/metadataBase.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mds/1.0/AppendixD.2VectorSmartMapExample.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mds/1.0/AppendixD.2VectorSmartMapExample.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mds/1.0/mds.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mds/1.0/mds.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mds/1.0/mds.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mds/1.0/mds.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mds/2.0/mds.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mds/2.0/mds.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mds/2.0/mds.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mds/2.0/mds.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mdt/1.0/codelists.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mdt/1.0/codelists.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mdt/1.0/mdt.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mdt/1.0/mdt.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mdt/1.0/mdt.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mdt/1.0/mdt.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mdt/1.0/metadataTransfer.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mdt/1.0/metadataTransfer.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mdt/2.0/codelists.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mdt/2.0/codelists.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mdt/2.0/mdt.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mdt/2.0/mdt.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mdt/2.0/mdt.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mdt/2.0/mdt.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mdt/2.0/metadataTransfer.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mdt/2.0/metadataTransfer.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mex/1.0/codelists.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mex/1.0/codelists.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mex/1.0/metadataExtension.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mex/1.0/metadataExtension.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mex/1.0/mex.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mex/1.0/mex.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mex/1.0/mex_invalid.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mex/1.0/mex_invalid.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mex/1.0/mex_valid.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mex/1.0/mex_valid.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mmi/1.0/codelists.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mmi/1.0/codelists.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mmi/1.0/maintenance.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mmi/1.0/maintenance.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mmi/1.0/mmi.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mmi/1.0/mmi.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mmi/1.0/mmi_invalid.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mmi/1.0/mmi_invalid.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mmi/1.0/mmi_valid.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mmi/1.0/mmi_valid.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mpc/1.0/mpc.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mpc/1.0/mpc.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mpc/1.0/portrayalCatalogue.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mpc/1.0/portrayalCatalogue.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrc/1.0/codelists.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mrc/1.0/codelists.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrc/1.0/content.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mrc/1.0/content.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrc/1.0/contentInformationImagery.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mrc/1.0/contentInformationImagery.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrc/1.0/mrc.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mrc/1.0/mrc.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrc/1.0/mrc_invalid.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mrc/1.0/mrc_invalid.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrc/1.0/mrc_valid.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mrc/1.0/mrc_valid.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrc/2.0/codelists.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mrc/2.0/codelists.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrc/2.0/content.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mrc/2.0/content.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrc/2.0/contentInformationImagery.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mrc/2.0/contentInformationImagery.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrc/2.0/mrc.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mrc/2.0/mrc.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrc/2.0/mrc.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mrc/2.0/mrc.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrd/1.0/codelists.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mrd/1.0/codelists.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrd/1.0/distribution.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mrd/1.0/distribution.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrd/1.0/mrd.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mrd/1.0/mrd.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrd/1.0/mrd_invalid.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mrd/1.0/mrd_invalid.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrd/1.0/mrd_valid.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mrd/1.0/mrd_valid.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mri/1.0/codelists.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mri/1.0/codelists.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mri/1.0/identification.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mri/1.0/identification.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mri/1.0/mri.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mri/1.0/mri.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mri/1.0/mri_invalid.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mri/1.0/mri_invalid.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mri/1.0/mri_valid.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mri/1.0/mri_valid.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrl/1.0/lineage.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mrl/1.0/lineage.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrl/1.0/lineageImagery.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mrl/1.0/lineageImagery.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrl/1.0/mrl.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mrl/1.0/mrl.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrl/2.0/lineage.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mrl/2.0/lineage.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrl/2.0/lineageImagery.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mrl/2.0/lineageImagery.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrl/2.0/mrl.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mrl/2.0/mrl.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrl/2.0/mrl.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mrl/2.0/mrl.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrs/1.0/codelists.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mrs/1.0/codelists.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrs/1.0/mrs.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mrs/1.0/mrs.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/mrs/1.0/referenceSystem.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/mrs/1.0/referenceSystem.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/msr/1.0/msr.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/msr/1.0/msr.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/msr/1.0/spatialRepresentation.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/msr/1.0/spatialRepresentation.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/msr/1.0/spatialRepresentationImagery.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/msr/1.0/spatialRepresentationImagery.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/msr/2.0/msr.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/msr/2.0/msr.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/msr/2.0/msr.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/msr/2.0/msr.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/msr/2.0/spatialRepresentation.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/msr/2.0/spatialRepresentation.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/msr/2.0/spatialRepresentationImagery.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/msr/2.0/spatialRepresentationImagery.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/srv/2.0/codelists.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/srv/2.0/codelists.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/srv/2.0/serviceInformation.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/srv/2.0/serviceInformation.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/srv/2.0/srv.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/srv/2.0/srv.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/srv/2.0/srv_invalid.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/srv/2.0/srv_invalid.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/-3/srv/2.0/srv_valid.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/-3/srv/2.0/srv_valid.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/cat/codelists.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/cat/codelists.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/CD_PixelinCell.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/CD_PixelinCell.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/CI_DateTypeCode.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/CI_DateTypeCode.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/CI_OnLineFunctionCode.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/CI_OnLineFunctionCode.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/CI_PresentationFormCode.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/CI_PresentationFormCode.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/CI_RoleCode.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/CI_RoleCode.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/CI_TelephoneTypeCode.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/CI_TelephoneTypeCode.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/CS_AxisDirection.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/CS_AxisDirection.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/CS_RangeMeaning.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/CS_RangeMeaning.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/DCPList.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/DCPList.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/DS_AssociationTypeCode.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/DS_AssociationTypeCode.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/DS_InitiativeTypeCode.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/DS_InitiativeTypeCode.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/FC_RoleType.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/FC_RoleType.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_CellGeometryTypeCode.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_CellGeometryTypeCode.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_ClassificationCode.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_ClassificationCode.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_CoverageContentTypeCode.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_CoverageContentTypeCode.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_DatatypeCode.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_DatatypeCode.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_DimensionNameTypeCode.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_DimensionNameTypeCode.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_GeometricObjectTypeCode.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_GeometricObjectTypeCode.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_ImagingConditionCode.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_ImagingConditionCode.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_KeywordTypeCode.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_KeywordTypeCode.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_MaintenanceFrequencyCode.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_MaintenanceFrequencyCode.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_MediumFormatCode.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_MediumFormatCode.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_ObligationCode.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_ObligationCode.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_PixelOrientationCode.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_PixelOrientationCode.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_ProgressCode.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_ProgressCode.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_ReferenceSystemTypeCode.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_ReferenceSystemTypeCode.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_RestrictionCode.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_RestrictionCode.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_ScopeCode.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_ScopeCode.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_SpatialRepresentationTypeCode.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_SpatialRepresentationTypeCode.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_TopicCategoryCode.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_TopicCategoryCode.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_TopologyLevelCode.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MD_TopologyLevelCode.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_BandDefinition.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_BandDefinition.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_ContextCode.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_ContextCode.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_GeometryTypeCode.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_GeometryTypeCode.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_ObjectiveTypeCode.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_ObjectiveTypeCode.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_OperationTypeCode.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_OperationTypeCode.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_PolarisationOrientationCode.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_PolarisationOrientationCode.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_PriorityCode.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_PriorityCode.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_SensorTypeCode.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_SensorTypeCode.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_SequenceCode.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_SequenceCode.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_TransferFunctionTypeCode.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_TransferFunctionTypeCode.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_TriggerCode.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/MI_TriggerCode.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/RE_AmendmentType.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/RE_AmendmentType.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/RE_DecisionStatus.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/RE_DecisionStatus.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/RE_Disposition.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/RE_Disposition.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/RE_ItemStatus.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/RE_ItemStatus.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/SC_DerivedCRSType.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/SC_DerivedCRSType.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/SV_CouplingType.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/SV_CouplingType.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/SV_ParameterDirection.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/Codelists/gml/SV_ParameterDirection.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19115/resources/namespaceInformationAndTools/ISONamespaceInformation.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19115/resources/namespaceInformationAndTools/ISONamespaceInformation.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19135/-2/pre/1.0/abstract.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19135/-2/pre/1.0/abstract.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19135/-2/reg/1.0/reg.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19135/-2/reg/1.0/reg.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19135/-2/reg/1.0/registration.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19135/-2/reg/1.0/registration.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19139/resources/ML_gmxCodelists.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19139/resources/ML_gmxCodelists.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19139/resources/gmiCodelists.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19139/resources/gmiCodelists.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19139/resources/gmxCodelists.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19139/resources/gmxCodelists.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19139/resources/tcCodelists.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19139/resources/tcCodelists.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19155/gpi/1.0/gpi.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19155/gpi/1.0/gpi.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19155/gpi/1.0/placeIdentifier.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19155/gpi/1.0/placeIdentifier.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19155/gpi/1.0/referenceSystem.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19155/gpi/1.0/referenceSystem.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19155/gpi/1.0/sampleGMLApplicationSchema.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19155/gpi/1.0/sampleGMLApplicationSchema.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19155/gpi/1.0/sampleGMLApplicationSchema.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19155/gpi/1.0/sampleGMLApplicationSchema.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/-2/dqc/1.0/abstract.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19157/-2/dqc/1.0/abstract.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/-2/dqc/1.0/dqc.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19157/-2/dqc/1.0/dqc.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/-2/dqm/1.0/codelists.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19157/-2/dqm/1.0/codelists.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/-2/dqm/1.0/dqm.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19157/-2/dqm/1.0/dqm.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/-2/dqm/1.0/dqm.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19157/-2/dqm/1.0/dqm.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/-2/dqm/1.0/dqm_invalid.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19157/-2/dqm/1.0/dqm_invalid.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/-2/dqm/1.0/dqm_valid.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19157/-2/dqm/1.0/dqm_valid.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/-2/dqm/1.0/qualityMeasures.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19157/-2/dqm/1.0/qualityMeasures.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/-2/mdq/1.0/codelists.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19157/-2/mdq/1.0/codelists.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/-2/mdq/1.0/dataQualityElement.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19157/-2/mdq/1.0/dataQualityElement.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/-2/mdq/1.0/dataQualityEvaluation.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19157/-2/mdq/1.0/dataQualityEvaluation.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/-2/mdq/1.0/dataQualityImagery.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19157/-2/mdq/1.0/dataQualityImagery.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/-2/mdq/1.0/dataQualityResult.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19157/-2/mdq/1.0/dataQualityResult.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/-2/mdq/1.0/mdq.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19157/-2/mdq/1.0/mdq.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/-2/mdq/1.0/mdq.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19157/-2/mdq/1.0/mdq.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/-2/mdq/1.0/mdq_invalid.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19157/-2/mdq/1.0/mdq_invalid.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/-2/mdq/1.0/mdq_valid.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19157/-2/mdq/1.0/mdq_valid.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/-2/mdq/1.0/metaquality.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19157/-2/mdq/1.0/metaquality.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/resources/Codelists/cat/codelists.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19157/resources/Codelists/cat/codelists.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/resources/Codelists/gml/DQM_ValueStructure.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19157/resources/Codelists/gml/DQM_ValueStructure.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19157/resources/Codelists/gml/DQ_EvaluationMethodTypeCode.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19157/resources/Codelists/gml/DQ_EvaluationMethodTypeCode.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19165/gpm/1.0/examples/localSchema.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19165/gpm/1.0/examples/localSchema.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19165/gpm/1.0/examples/of5mv60sd0f279110s1r100ca5-gpm.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19165/gpm/1.0/examples/of5mv60sd0f279110s1r100ca5-gpm.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19165/gpm/1.0/geospatialPreservationMetadata.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19165/gpm/1.0/geospatialPreservationMetadata.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/19165/gpm/1.0/gpm.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/19165/gpm/1.0/gpm.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/basicTypes.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/basicTypes.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/coordinateOperations.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/coordinateOperations.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/coordinateReferenceSystems.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/coordinateReferenceSystems.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/coordinateSystems.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/coordinateSystems.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/coverage.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/coverage.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/datums.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/datums.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/deprecatedTypes.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/deprecatedTypes.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/dictionary.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/dictionary.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/direction.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/direction.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/dynamicFeature.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/dynamicFeature.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/feature.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/feature.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/geometryAggregates.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/geometryAggregates.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/geometryBasic0d1d.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/geometryBasic0d1d.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/geometryBasic2d.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/geometryBasic2d.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/geometryComplexes.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/geometryComplexes.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/geometryPrimitives.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/geometryPrimitives.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/gml.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/gml.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/gmlBase.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/gmlBase.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/grids.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/grids.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/measures.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/measures.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/observation.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/observation.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/referenceSystems.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/referenceSystems.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/temporal.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/temporal.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/temporalReferenceSystems.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/temporalReferenceSystems.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/temporalTopology.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/temporalTopology.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/topology.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/topology.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/units.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/units.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/valueObjects.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/gml/3.2.1/valueObjects.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gco/basicTypes.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gco/basicTypes.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gco/gco.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gco/gco.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gco/gcoBase.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gco/gcoBase.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/applicationSchema.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/applicationSchema.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/citation.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/citation.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/constraints.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/constraints.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/content.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/content.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/dataQuality.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/dataQuality.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/distribution.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/distribution.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/extent.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/extent.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/freeText.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/freeText.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/gmd.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/gmd.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/identification.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/identification.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/maintenance.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/maintenance.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/metadataApplication.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/metadataApplication.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/metadataEntity.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/metadataEntity.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/metadataExtension.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/metadataExtension.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/portrayalCatalogue.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/portrayalCatalogue.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/referenceSystem.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/referenceSystem.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/spatialRepresentation.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gmd/spatialRepresentation.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gsr/gsr.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gsr/gsr.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gsr/spatialReferencing.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gsr/spatialReferencing.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gss/geometry.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gss/geometry.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gss/gss.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gss/gss.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gts/gts.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gts/gts.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gts/temporalObjects.xsd` & `ckanext-iso19115-0.1.1/ckanext/iso19115/namespaces/schemas.opengis.net/iso/19139/20070417/gts/temporalObjects.xsd`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/plugin.py` & `ckanext-iso19115-0.1.1/ckanext/iso19115/plugin.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from .logic import action
 
 try:
     config_declarations = tk.blanket.config_declarations
 except AttributeError:
     config_declarations = lambda cls: cls
 
+
 @config_declarations
 class Iso19115Plugin(plugins.SingletonPlugin):
     plugins.implements(plugins.IActions)
     plugins.implements(plugins.IClick)
     plugins.implements(plugins.IBlueprint)
     plugins.implements(plugins.IConfigurer)
     plugins.implements(plugins.ITemplateHelpers)
@@ -47,15 +48,14 @@
     def register_metaexport_format(self):
         from . import formatter
 
         return dict(
             iso19115=formatter.Iso19115(),
             iso19115_html=formatter.Iso19115Html(),
             iso19115_pdf=formatter.Iso19115Pdf(),
-
         )
 
     def register_data_extractors(self, formatters):
         formatters.get("iso19115").set_data_extractor(_data_extractor)
 
     # ITemplateHelpers
     def get_helpers(self):
```

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/presets.yaml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/presets.yaml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/schematron/cit.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/schematron/cit.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/schematron/dqm.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/schematron/dqm.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/schematron/gex.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/schematron/gex.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/schematron/mco.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/schematron/mco.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/schematron/mdb.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/schematron/mdb.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/schematron/mdq.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/schematron/mdq.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/schematron/mex.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/schematron/mex.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/schematron/mmi.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/schematron/mmi.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/schematron/mrc.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/schematron/mrc.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/schematron/mrd.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/schematron/mrd.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/schematron/mri.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/schematron/mri.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/schematron/srv.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/schematron/srv.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/templates/iso19115/validate.html` & `ckanext-iso19115-0.1.1/ckanext/iso19115/templates/iso19115/validate.html`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/tests/conftest.py` & `ckanext-iso19115-0.1.1/ckanext/iso19115/tests/conftest.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,17 +10,15 @@
 def examples():
     return Path(__file__).parent / "examples"
 
 
 @pytest.fixture()
 def example(examples, request):
     name = next(
-        m.args[0]
-        for m in request.node.iter_markers()
-        if m.name == "xml_example"
+        m.args[0] for m in request.node.iter_markers() if m.name == "xml_example"
     )
     path = examples / name
     return path.open("rb").read()
 
 
 @pytest.fixture()
 def schema_errors(example):
```

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/tests/examples/v3.2/basic.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/tests/examples/v3.2/basic.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/tests/examples/v3.2/complex.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/tests/examples/v3.2/complex.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/tests/examples/v3.2/identification.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/tests/examples/v3.2/identification.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/tests/examples/v3.2/identification_no_category.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/tests/examples/v3.2/identification_no_category.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/tests/examples/v3.2/identification_no_geo.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/tests/examples/v3.2/identification_no_geo.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/tests/examples/v3.2/minimal.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/tests/examples/v3.2/minimal.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/tests/examples/v3.2/sch_no_creation_date.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/tests/examples/v3.2/sch_no_creation_date.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/tests/examples/v3.2/sch_no_default_locale.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/tests/examples/v3.2/sch_no_default_locale.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/tests/examples/v3.2/sch_non_dataset_scope.xml` & `ckanext-iso19115-0.1.1/ckanext/iso19115/tests/examples/v3.2/sch_non_dataset_scope.xml`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/tests/test_converter.py` & `ckanext-iso19115-0.1.1/ckanext/iso19115/tests/test_converter.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,32 +12,28 @@
     print(etree_tostring(el, namespaces=u.ns))
 
 
 class TestConverter:
     def test_minimal_xml(self, faker):
         el: t.mdb.MD_Metadata = h.make("mdb:MD_Metadata")
         dt1 = faker.date_time()
-        el.add_dateInfo(
-            t.cit.CI_Date(h.date(dt1), t.cit.CI_DateTypeCode("creation"))
-        )
+        el.add_dateInfo(t.cit.CI_Date(h.date(dt1), t.cit.CI_DateTypeCode("creation")))
         data = c.jml(el)
         builder = u.get_builder("mdb:MD_Metadata")
         assert builder.build(data)
 
     def test_with_party(self, faker):
         el: t.mdb.MD_Metadata = h.make("mdb:MD_Metadata")
         el.add_dateInfo(
             t.cit.CI_Date(
                 h.date(faker.date_time().date()),
                 t.cit.CI_DateTypeCode("creation"),
             )
         )
-        el.add_contact(
-            h.responsibility("author", t.cit.CI_Individual(h.cs("author")))
-        )
+        el.add_contact(h.responsibility("author", t.cit.CI_Individual(h.cs("author"))))
 
         builder = u.get_builder("mdb:MD_Metadata")
         data = c.jml(el)
         builder.build(data)
 
     def test_with_identification(self, faker):
         el: t.mdb.MD_Metadata = h.make("mdb:MD_Metadata")
```

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/tests/test_plugin.py` & `ckanext-iso19115-0.1.1/ckanext/iso19115/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/types/base.py` & `ckanext-iso19115-0.1.1/ckanext/iso19115/types/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,15 +52,14 @@
                 return option
         raise ValueError(
             f"Codelist {ns}:{name} does not contain value {value}:"
             f" {[o.name for o in options]}"
         )
 
     def as_jml(self):
-
         ns, name = self._qualify()
         data = JmlRecord(f"{ns}:{name}")
 
         option = self._into_clv(self.value)
 
         data.attrs.update(
             {
```

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/types/cit.py` & `ckanext-iso19115-0.1.1/ckanext/iso19115/types/cit.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,17 +39,15 @@
 @dataclass
 class CI_Address:
     deliveryPoint: list[gco.CharacterString] = field(default_factory=list)
     city: Optional[gco.CharacterString] = None
     administrativeArea: Optional[gco.CharacterString] = None
     postalCode: Optional[gco.CharacterString] = None
     country: Optional[gco.CharacterString] = None
-    electronicMailAddress: list[gco.CharacterString] = field(
-        default_factory=list
-    )
+    electronicMailAddress: list[gco.CharacterString] = field(default_factory=list)
 
 
 @dataclass
 class CI_OnlineResource:
     linkage: gco.CharacterString
     protocol: Optional[gco.CharacterString] = None
     applicationProfile: Optional[gco.CharacterString] = None
@@ -93,17 +91,15 @@
     page: Optional[str] = None
 
 
 @dataclass
 class AbstractCI_Party:
     name: gco.CharacterString = None
     contactInfo: Optional[list[CI_Contact]] = field(default_factory=list)
-    partyIdentifier: Optional[list[mcc.MD_Identifier]] = field(
-        default_factory=list
-    )
+    partyIdentifier: Optional[list[mcc.MD_Identifier]] = field(default_factory=list)
 
 
 @dataclass
 class CI_Individual(AbstractCI_Party):
     positionName: Optional[gco.CharacterString] = None
 
 
@@ -112,30 +108,26 @@
     logo: Optional[list[mcc.MD_BrowseGraphic]] = field(default_factory=list)
     individual: Optional[list[CI_Individual]] = field(default_factory=list)
 
 
 @dataclass
 class CI_Citation:
     title: gco.CharacterString
-    alternateTitle: Optional[list[gco.CharacterString]] = field(
-        default_factory=list
-    )
+    alternateTitle: Optional[list[gco.CharacterString]] = field(default_factory=list)
     date: Optional[list[CI_Date]] = field(default_factory=list)
     edition: Optional[gco.CharacterString] = None
     editionDate: Optional[gco.DateTime] = None
     identifier: Optional[list[mcc.MD_Identifier]] = field(default_factory=list)
     citedResponsibleParty: Optional[list[CI_Responsibility]] = field(
         default_factory=list
     )
-    presentationForm: Optional[
-        list[Codelist[cit.CI_PresentationFormCode]]
-    ] = field(default_factory=list)
+    presentationForm: Optional[list[Codelist[cit.CI_PresentationFormCode]]] = field(
+        default_factory=list
+    )
     series: Optional[CI_Series] = None
     otherCitationDetails: Optional[list[gco.CharacterString]] = field(
         default_factory=list
     )
     ISBN: Optional[gco.CharacterString] = None
     ISSN: Optional[gco.CharacterString] = None
-    onlineResource: Optional[list[CI_OnlineResource]] = field(
-        default_factory=list
-    )
+    onlineResource: Optional[list[CI_OnlineResource]] = field(default_factory=list)
     graphic: Optional[list[mcc.MD_BrowseGraphic]] = field(default_factory=list)
```

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/types/gco.py` & `ckanext-iso19115-0.1.1/ckanext/iso19115/types/gco.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,14 +40,15 @@
     value: str
 
 
 @dataclass
 class Real(Atomic):
     value: float
 
+
 @dataclass
 class Decimal(Atomic):
     value: str
 
 
 @dataclass
 class Measure(Atomic):
```

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/types/gex.py` & `ckanext-iso19115-0.1.1/ckanext/iso19115/types/gex.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,17 +6,15 @@
 if TYPE_CHECKING:
     from . import *
 
 
 @dataclass
 class EX_Extent:
     description: Optional[gco.CharacterString] = None
-    geographicElement: list[AbstractEX_GeographicExtent] = field(
-        default_factory=list
-    )
+    geographicElement: list[AbstractEX_GeographicExtent] = field(default_factory=list)
     temporalElement: list[EX_TemporalExtent] = field(default_factory=list)
     verticalElement: list[EX_VerticalExtent] = field(default_factory=list)
 
 
 @dataclass
 class EX_VerticalExtent:
     minimumValue: str
```

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/types/gml.py` & `ckanext-iso19115-0.1.1/ckanext/iso19115/types/gml.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,24 +177,20 @@
 @dataclass
 class MultiPoint(AbstractGeometry):
     pointMember: list[Point] = field(default_factory=list)
     pointMembers: list[Point] = field(default_factory=list)
 
 
 @dataclass
-class CompositeSolid(
-    AbstractGeometry, AbstractGeometricPrimitive, AbstractSolid
-):
+class CompositeSolid(AbstractGeometry, AbstractGeometricPrimitive, AbstractSolid):
     solidMember: list[AbstractSolid] = field(default_factory=list)
 
 
 @dataclass
-class Ring(
-    AbstractGeometry, AbstractRing, AbstractGeometricPrimitive, AbstractCurve
-):
+class Ring(AbstractGeometry, AbstractRing, AbstractGeometricPrimitive, AbstractCurve):
     curveMember: list[AbstractCurve] = field(default_factory=list)
 
 
 @dataclass
 class MultiSolid(AbstractGeometry):
     solidMember: list[AbstractSolid] = field(default_factory=list)
     solidMembers: list[AbstractSolid] = field(default_factory=list)
@@ -208,37 +204,31 @@
 @dataclass
 class MultiGeometry(AbstractGeometry):
     geometryMember: list[AbstractGeometry] = field(default_factory=list)
     geometryMembers: list[AbstractGeometry] = field(default_factory=list)
 
 
 @dataclass
-class CompositeSurface(
-    AbstractGeometry, AbstractGeometricPrimitive, AbstractSurface
-):
+class CompositeSurface(AbstractGeometry, AbstractGeometricPrimitive, AbstractSurface):
     surfaceMember: list[AbstractSurface] = field(default_factory=list)
 
 
 @dataclass
 class Point(AbstractGeometry, AbstractGeometricPrimitive):
     pos: list[str] = field(default_factory=list)
     coordinates: Optional[str] = None
 
 
 @dataclass
-class CompositeCurve(
-    AbstractGeometry, AbstractGeometricPrimitive, AbstractCurve
-):
+class CompositeCurve(AbstractGeometry, AbstractGeometricPrimitive, AbstractCurve):
     curveMember: list[AbstractCurve] = field(default_factory=list)
 
 
 @dataclass
-class OrientableCurve(
-    AbstractGeometry, AbstractGeometricPrimitive, AbstractCurve
-):
+class OrientableCurve(AbstractGeometry, AbstractGeometricPrimitive, AbstractCurve):
     baseCurve: list[AbstractCurve] = field(default_factory=list)
 
 
 @dataclass
 class Solid(AbstractGeometry, AbstractGeometricPrimitive, AbstractSolid):
     exterior: Optional[Shell] = None
     interior: list[Shell] = field(default_factory=list)
@@ -257,17 +247,15 @@
 
 @dataclass
 class GeometricComplex(AbstractGeometry):
     element: list[AbstractGeometricPrimitive] = field(default_factory=list)
 
 
 @dataclass
-class OrientableSurface(
-    AbstractGeometry, AbstractGeometricPrimitive, AbstractSurface
-):
+class OrientableSurface(AbstractGeometry, AbstractGeometricPrimitive, AbstractSurface):
     baseSurface: Optional[AbstractSurface] = None
 
 
 @dataclass
 class Surface(AbstractGeometry, AbstractGeometricPrimitive, AbstractSurface):
     patches: list[AbstractSurfacePatch] = field(default_factory=list)
 
@@ -377,17 +365,15 @@
     name: Optional[str] = None
     remarks: Optional[str] = None
     scope: list[str] = field(default_factory=list)
 
 
 @dataclass
 class UnitDefinition:
-    metaDataProperty: Optional[list[GenericMetaData]] = field(
-        default_factory=list
-    )
+    metaDataProperty: Optional[list[GenericMetaData]] = field(default_factory=list)
     description: Optional[str] = None
     descriptionReference: Optional[Any] = None
     identifier: Any = None
     name: Optional[list[str]] = field(default_factory=list)
     remarks: Optional[str] = None
     quantityType: Optional[str] = None
     quantityTypeReference: Optional[str] = None
```

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/types/lan.py` & `ckanext-iso19115-0.1.1/ckanext/iso19115/types/lan.py`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/types/mac.py` & `ckanext-iso19115-0.1.1/ckanext/iso19115/types/mac.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,17 +61,15 @@
     identifier: list[mcc.MD_Identifier] = field(default_factory=list)
     priority: Optional[gco.CharacterString] = None
     type: Optional[list[Codelist[mac.MI_ObjectiveTypeCode]]] = field(
         default_factory=list
     )
     function: Optional[list[gco.CharacterString]] = field(default_factory=list)
     extent: Optional[list[gex.EX_Extent]] = field(default_factory=list)
-    sensingInstrument: Optional[list[mac.MI_Instrument]] = field(
-        default_factory=list
-    )
+    sensingInstrument: Optional[list[mac.MI_Instrument]] = field(default_factory=list)
     # pass: Optional[list[mac.MI_PlatformPass]] = field(default_factory=list)
     objectiveOccurence: list[mac.MI_Event] = field(default_factory=list)
 
 
 @dataclass
 class MI_Plan:
     type: Optional[Codelist[mac.MI_GeometryTypeCode]] = None
@@ -94,30 +92,24 @@
 class MI_Event:
     identifier: mcc.MD_Identifier
     trigger: Codelist[mac.MI_TriggerCode]
     context: Codelist[mac.MI_ContextCode]
     sequence: Codelist[mac.MI_SequenceCode]
     time: gco.DateTime
     relatedPass: Optional[mac.MI_PlatformPass] = None
-    relatedSensor: Optional[list[mac.MI_Instrument]] = field(
-        default_factory=list
-    )
-    expectedObjective: Optional[list[mac.MI_Objective]] = field(
-        default_factory=list
-    )
+    relatedSensor: Optional[list[mac.MI_Instrument]] = field(default_factory=list)
+    expectedObjective: Optional[list[mac.MI_Objective]] = field(default_factory=list)
 
 
 @dataclass
 class MI_Platform:
     citation: Optional[list[cit.CI_Citation]] = field(default_factory=list)
     identifier: mcc.MD_Identifier = None
     description: gco.CharacterString = None
-    sponsor: Optional[list[cit.CI_Responsibility]] = field(
-        default_factory=list
-    )
+    sponsor: Optional[list[cit.CI_Responsibility]] = field(default_factory=list)
     instrument: list[mac.MI_Instrument] = field(default_factory=list)
     otherPropertyType: Optional[gco.RecordType] = None
     otherProperty: Optional[gco.Record] = None
     history: Optional[list[mac.MI_InstrumentationEventList]] = field(
         default_factory=list
     )
 
@@ -143,17 +135,15 @@
 class MI_InstrumentationEvent:
     citation: Optional[list[cit.CI_Citation]] = field(default_factory=list)
     description: gco.CharacterString = None
     extent: Optional[list[gex.EX_Extent]] = field(default_factory=list)
     type: list[Codelist[mac.MI_InstrumentationEventTypeCode]] = field(
         default_factory=list
     )
-    revisionHistory: Optional[list[mac.MI_Revision]] = field(
-        default_factory=list
-    )
+    revisionHistory: Optional[list[mac.MI_Revision]] = field(default_factory=list)
 
 
 @dataclass
 class MI_InstrumentationEventList:
     citation: cit.CI_Citation
     description: gco.CharacterString
     locale: Optional[lan.PT_Locale] = None
@@ -185,23 +175,19 @@
 class MI_Operation:
     description: Optional[gco.CharacterString] = None
     citation: Optional[cit.CI_Citation] = None
     identifier: Optional[mcc.MD_Identifier] = None
     status: Codelist[mcc.MD_ProgressCode] = None
     type: Optional[Codelist[mac.MI_OperationTypeCode]] = None
     parentOperation: Optional[mac.MI_Operation] = None
-    childOperation: Optional[list[mac.MI_Operation]] = field(
-        default_factory=list
-    )
+    childOperation: Optional[list[mac.MI_Operation]] = field(default_factory=list)
     platform: Optional[list[mac.MI_Platform]] = field(default_factory=list)
     objective: Optional[list[mac.MI_Objective]] = field(default_factory=list)
     plan: Optional[mac.MI_Plan] = None
-    significantEvent: Optional[list[mac.MI_Event]] = field(
-        default_factory=list
-    )
+    significantEvent: Optional[list[mac.MI_Event]] = field(default_factory=list)
     otherPropertyType: Optional[gco.RecordType] = None
     otherProperty: Optional[gco.Record] = None
 
 
 @dataclass
 class MI_AcquisitionInformation:
     scope: mcc.MD_Scope
```

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/types/mas.py` & `ckanext-iso19115-0.1.1/ckanext/iso19115/types/mas.py`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/types/mcc.py` & `ckanext-iso19115-0.1.1/ckanext/iso19115/types/mcc.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,20 +29,16 @@
 
 
 @dataclass
 class MD_BrowseGraphic:
     fileName: gco.CharacterString
     fileDescription: Optional[gco.CharacterString] = None
     fileType: Optional[gco.CharacterString] = None
-    imageConstraints: Optional[list[mco.MD_Constraints]] = field(
-        default_factory=list
-    )
-    linkage: Optional[list[cit.CI_OnlineResource]] = field(
-        default_factory=list
-    )
+    imageConstraints: Optional[list[mco.MD_Constraints]] = field(default_factory=list)
+    linkage: Optional[list[cit.CI_OnlineResource]] = field(default_factory=list)
 
 
 @dataclass
 class MD_ScopeCode(Codelist):
     pass
 
 
@@ -70,50 +66,36 @@
 
 @dataclass
 class Abstract_ResourceDescription:
     citation: cit.CI_Citation
     abstract: gco.CharacterString
     purpose: Optional[gco.CharacterString] = None
     credit: Optional[list[gco.CharacterString]] = field(default_factory=list)
-    status: Optional[list[Codelist[mcc.MD_ProgressCode]]] = field(
-        default_factory=list
-    )
-    pointOfContact: Optional[list[cit.CI_Responsibility]] = field(
-        default_factory=list
-    )
+    status: Optional[list[Codelist[mcc.MD_ProgressCode]]] = field(default_factory=list)
+    pointOfContact: Optional[list[cit.CI_Responsibility]] = field(default_factory=list)
     spatialRepresentationType: Optional[
         list[Codelist[mcc.MD_SpatialRepresentationTypeCode]]
     ] = field(default_factory=list)
-    spatialResolution: Optional[list[mri.MD_Resolution]] = field(
-        default_factory=list
-    )
+    spatialResolution: Optional[list[mri.MD_Resolution]] = field(default_factory=list)
     temporalResolution: Optional[list[gco.TM_PeriodDuration]] = field(
         default_factory=list
     )
     topicCategory: Optional[list[Codelist[mri.MD_TopicCategoryCode]]] = field(
         default_factory=list
     )
     extent: Optional[list[gex.EX_Extent]] = field(default_factory=list)
-    additionalDocumentation: list[cit.CI_Citation] = field(
-        default_factory=list
-    )
+    additionalDocumentation: list[cit.CI_Citation] = field(default_factory=list)
     processingLevel: Optional[mcc.MD_Identifier] = None
     resourceMaintenance: Optional[list[mmi.MD_MaintenanceInformation]] = field(
         default_factory=list
     )
-    graphicOverview: Optional[list[mcc.MD_BrowseGraphic]] = field(
-        default_factory=list
-    )
+    graphicOverview: Optional[list[mcc.MD_BrowseGraphic]] = field(default_factory=list)
     resourceFormat: Optional[list[mrd.MD_Format]] = field(default_factory=list)
-    descriptiveKeywords: Optional[list[mri.MD_Keywords]] = field(
-        default_factory=list
-    )
-    resourceSpecificUsage: Optional[list[mri.MD_Usage]] = field(
-        default_factory=list
-    )
+    descriptiveKeywords: Optional[list[mri.MD_Keywords]] = field(default_factory=list)
+    resourceSpecificUsage: Optional[list[mri.MD_Usage]] = field(default_factory=list)
     resourceConstraints: Optional[list[mco.MD_Constraints]] = field(
         default_factory=list
     )
     associatedResource: Optional[list[mri.MD_AssociatedResource]] = field(
         default_factory=list
     )
```

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/types/mco.py` & `ckanext-iso19115-0.1.1/ckanext/iso19115/types/mco.py`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/types/mdb.py` & `ckanext-iso19115-0.1.1/ckanext/iso19115/types/mdb.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,74 +16,60 @@
 
 
 @dataclass
 class MD_Metadata:
     metadataIdentifier: Optional[mcc.MD_Identifier] = None
     defaultLocale: Optional[lan.PT_Locale] = None
     parentMetadata: Optional[cit.CI_Citation] = None
-    metadataScope: Optional[list[mdb.MD_MetadataScope]] = field(
-        default_factory=list
-    )
+    metadataScope: Optional[list[mdb.MD_MetadataScope]] = field(default_factory=list)
 
     contact: list[cit.CI_Responsibility] = field(default_factory=list)
     dateInfo: list[cit.CI_Date] = field(default_factory=list)
 
-    metadataStandard: Optional[list[cit.CI_Citation]] = field(
-        default_factory=list
-    )
-    metadataProfile: Optional[list[cit.CI_Citation]] = field(
-        default_factory=list
-    )
+    metadataStandard: Optional[list[cit.CI_Citation]] = field(default_factory=list)
+    metadataProfile: Optional[list[cit.CI_Citation]] = field(default_factory=list)
     alternativeMetadataReference: Optional[list[cit.CI_Citation]] = field(
         default_factory=list
     )
 
     otherLocale: Optional[list[lan.PT_Locale]] = field(default_factory=list)
-    metadataLinkage: Optional[list[cit.CI_OnlineResource]] = field(
-        default_factory=list
-    )
+    metadataLinkage: Optional[list[cit.CI_OnlineResource]] = field(default_factory=list)
     spatialRepresentationInfo: Optional[
         list[mcc.Abstract_SpatialRepresentation]
     ] = field(default_factory=list)
     referenceSystemInfo: Optional[list[mrs.MD_ReferenceSystem]] = field(
         default_factory=list
     )
-    metadataExtensionInfo: Optional[
-        list[mex.MD_MetadataExtensionInformation]
-    ] = field(default_factory=list)
+    metadataExtensionInfo: Optional[list[mex.MD_MetadataExtensionInformation]] = field(
+        default_factory=list
+    )
 
     identificationInfo: list[mcc.Abstract_ResourceDescription] = field(
         default_factory=list
     )
 
     contentInfo: Optional[list[mcc.Abstract_ContentInformation]] = field(
         default_factory=list
     )
-    distributionInfo: Optional[list[mrd.MD_Distribution]] = field(
+    distributionInfo: Optional[list[mrd.MD_Distribution]] = field(default_factory=list)
+    dataQualityInfo: Optional[list[mdq.DQ_DataQuality]] = field(default_factory=list)
+    resourceLineage: Optional[list[mrl.LI_Lineage]] = field(default_factory=list)
+    portrayalCatalogueInfo: Optional[list[mpc.MD_PortrayalCatalogueReference]] = field(
         default_factory=list
     )
-    dataQualityInfo: Optional[list[mdq.DQ_DataQuality]] = field(
+    metadataConstraints: Optional[list[mco.MD_Constraints]] = field(
         default_factory=list
     )
-    resourceLineage: Optional[list[mrl.LI_Lineage]] = field(
+    applicationSchemaInfo: Optional[list[mas.MD_ApplicationSchemaInformation]] = field(
         default_factory=list
     )
-    portrayalCatalogueInfo: Optional[
-        list[mpc.MD_PortrayalCatalogueReference]
-    ] = field(default_factory=list)
-    metadataConstraints: Optional[list[mco.MD_Constraints]] = field(
+    metadataMaintenance: Optional[mmi.MD_MaintenanceInformation] = None
+    acquisitionInformation: Optional[list[mac.MI_AcquisitionInformation]] = field(
         default_factory=list
     )
-    applicationSchemaInfo: Optional[
-        list[mas.MD_ApplicationSchemaInformation]
-    ] = field(default_factory=list)
-    metadataMaintenance: Optional[mmi.MD_MaintenanceInformation] = None
-    acquisitionInformation: Optional[
-        list[mac.MI_AcquisitionInformation]
-    ] = field(default_factory=list)
 
     def add_dateInfo(self, date: cit.CI_Date):
         self.dateInfo.append(date)
 
     def add_contact(self, contact: cit.CI_Responsibility):
         self.contact.append(contact)
```

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/types/mdq.py` & `ckanext-iso19115-0.1.1/ckanext/iso19115/types/mdq.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,58 +21,48 @@
     fileFormat: mrd.MD_Format
 
 
 @dataclass
 class DQ_StandaloneQualityReportInformation:
     reportReference: cit.CI_Citation
     abstract: gco.CharacterString
-    elementReport: Optional[list[mdq.AbstractDQ_Element]] = field(
-        default_factory=list
-    )
+    elementReport: Optional[list[mdq.AbstractDQ_Element]] = field(default_factory=list)
 
 
 @dataclass
 class DQ_DataQuality:
     scope: mcc.MD_Scope
-    standaloneQualityReport: Optional[
-        mdq.DQ_StandaloneQualityReportInformation
-    ] = None
+    standaloneQualityReport: Optional[mdq.DQ_StandaloneQualityReportInformation] = None
     report: list[mdq.AbstractDQ_Element] = field(default_factory=list)
 
 
 @dataclass
 class DQ_EvaluationMethod:
     dateTime: Optional[list[gco.DateTime]] = field(default_factory=list)
     evaluationMethodDescription: Optional[gco.CharacterString] = None
     evaluationProcedure: Optional[cit.CI_Citation] = None
     referenceDoc: Optional[list[cit.CI_Citation]] = field(default_factory=list)
-    evaluationMethodType: Optional[
-        Codelist[mdq.DQ_EvaluationMethodTypeCode]
-    ] = None
+    evaluationMethodType: Optional[Codelist[mdq.DQ_EvaluationMethodTypeCode]] = None
 
 
 @dataclass
 class DQ_MeasureReference:
     measureIdentification: Optional[mcc.MD_Identifier] = None
-    nameOfMeasure: Optional[list[gco.CharacterString]] = field(
-        default_factory=list
-    )
+    nameOfMeasure: Optional[list[gco.CharacterString]] = field(default_factory=list)
     measureDescription: Optional[gco.CharacterString] = None
 
 
 @dataclass
 class AbstractDQ_Element:
     dateTime: Optional[list[gco.DateTime]] = field(default_factory=list)
     standaloneQualityReportDetails: Optional[gco.CharacterString] = None
     measure: Optional[mdq.DQ_MeasureReference] = None
     evaluationMethod: Optional[mdq.DQ_EvaluationMethod] = None
     result: list[mdq.AbstractDQ_Result] = field(default_factory=list)
-    derivedElement: Optional[list[mdq.AbstractDQ_Element]] = field(
-        default_factory=list
-    )
+    derivedElement: Optional[list[mdq.AbstractDQ_Element]] = field(default_factory=list)
 
 
 @dataclass
 class DQ_DomainConsistency(AbstractDQ_Element):
     pass
 
 
@@ -89,17 +79,15 @@
 @dataclass
 class DQ_TopologicalConsistency(AbstractDQ_Element):
     pass
 
 
 @dataclass
 class DQ_Confidence(AbstractDQ_Element):
-    relatedElement: Optional[list[mdq.AbstractDQ_Element]] = field(
-        default_factory=list
-    )
+    relatedElement: Optional[list[mdq.AbstractDQ_Element]] = field(default_factory=list)
 
 
 @dataclass
 class DQ_NonQuantitativeAttributeCorrectness(AbstractDQ_Element):
     pass
 
 
@@ -122,17 +110,15 @@
 class DQ_AbsoluteExternalPositionalAccuracy(AbstractDQ_Element):
     pass
 
 
 @dataclass
 class DQ_Representativity(AbstractDQ_Element):
     pass
-    relatedElement: Optional[list[mdq.AbstractDQ_Element]] = field(
-        default_factory=list
-    )
+    relatedElement: Optional[list[mdq.AbstractDQ_Element]] = field(default_factory=list)
 
 
 @dataclass
 class DQ_QuantitativeAttributeAccuracy(AbstractDQ_Element):
     pass
 
 
@@ -160,17 +146,15 @@
 class DQ_CompletenessOmission(AbstractDQ_Element):
     pass
 
 
 @dataclass
 class DQ_Homogeneity(AbstractDQ_Element):
     pass
-    relatedElement: Optional[list[mdq.AbstractDQ_Element]] = field(
-        default_factory=list
-    )
+    relatedElement: Optional[list[mdq.AbstractDQ_Element]] = field(default_factory=list)
 
 
 @dataclass
 class DQ_ThematicClassificationCorrectness(AbstractDQ_Element):
     pass
 
 
@@ -178,17 +162,15 @@
 class AbstractDQ_Result:
     dateTime: Optional[gco.DateTime] = None
     resultScope: Optional[mcc.MD_Scope] = None
 
 
 @dataclass
 class QE_CoverageResult(AbstractDQ_Result):
-    spatialRepresentationType: Codelist[
-        mcc.MD_SpatialRepresentationTypeCode
-    ] = None
+    spatialRepresentationType: Codelist[mcc.MD_SpatialRepresentationTypeCode] = None
     resultFile: mdq.QualityResultFile = None
     resultSpatialRepresentation: mcc.Abstract_SpatialRepresentation = None
     resultContentDescription: mcc.Abstract_ContentInformation = None
     resultFormat: mrd.MD_Format = None
 
 
 @dataclass
```

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/types/mmi.py` & `ckanext-iso19115-0.1.1/ckanext/iso19115/types/mmi.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,16 +17,10 @@
 @dataclass
 class MD_MaintenanceInformation:
     maintenanceAndUpdateFrequency: Optional[
         Codelist[mmi.MD_MaintenanceFrequencyCode]
     ] = None
     maintenanceDate: Optional[list[cit.CI_Date]] = field(default_factory=list)
     userDefinedMaintenanceFrequency: Optional[gco.TM_PeriodDuration] = None
-    maintenanceScope: Optional[list[mcc.MD_Scope]] = field(
-        default_factory=list
-    )
-    maintenanceNote: Optional[list[gco.CharacterString]] = field(
-        default_factory=list
-    )
-    contact: Optional[list[cit.CI_Responsibility]] = field(
-        default_factory=list
-    )
+    maintenanceScope: Optional[list[mcc.MD_Scope]] = field(default_factory=list)
+    maintenanceNote: Optional[list[gco.CharacterString]] = field(default_factory=list)
+    contact: Optional[list[cit.CI_Responsibility]] = field(default_factory=list)
```

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/types/mrc.py` & `ckanext-iso19115-0.1.1/ckanext/iso19115/types/mrc.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,37 +29,31 @@
 
 
 @dataclass
 class MD_AttributeGroup:
     contentType: list[Codelist[mrc.MD_CoverageContentTypeCode]] = field(
         default_factory=list
     )
-    attribute: Optional[list[mrc.MD_RangeDimension]] = field(
-        default_factory=list
-    )
+    attribute: Optional[list[mrc.MD_RangeDimension]] = field(default_factory=list)
 
 
 @dataclass
 class MD_FeatureCatalogueDescription(mcc.Abstract_ContentInformation):
     complianceCode: Optional[gco.Boolean] = None
     locale: Optional[list[lan.PT_Locale]] = field(default_factory=list)
     includedWithDataset: Optional[gco.Boolean] = None
-    featureTypes: Optional[list[mrc.MD_FeatureTypeInfo]] = field(
-        default_factory=list
-    )
+    featureTypes: Optional[list[mrc.MD_FeatureTypeInfo]] = field(default_factory=list)
     featureCatalogueCitation: Optional[list[cit.CI_Citation]] = field(
         default_factory=list
     )
 
 
 @dataclass
 class MD_CoverageDescription(mcc.Abstract_ContentInformation):
     attributeDescription: gco.RecordType = None
     processingLevelCode: Optional[mcc.MD_Identifier] = None
-    attributeGroup: Optional[list[mrc.MD_AttributeGroup]] = field(
-        default_factory=list
-    )
+    attributeGroup: Optional[list[mrc.MD_AttributeGroup]] = field(default_factory=list)
 
 
 @dataclass
 class MD_FeatureCatalogue(mcc.Abstract_ContentInformation):
     featureCatalogue: list[Any] = field(default_factory=list)
```

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/types/mrd.py` & `ckanext-iso19115-0.1.1/ckanext/iso19115/types/mrd.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,35 +13,31 @@
 class MD_MediumFormatCode(Codelist):
     pass
 
 
 @dataclass
 class MD_Distributor:
     distributorContact: cit.CI_Responsibility
-    distributionOrderProcess: Optional[
-        list[mrd.MD_StandardOrderProcess]
-    ] = field(default_factory=list)
-    distributorFormat: Optional[list[mrd.MD_Format]] = field(
+    distributionOrderProcess: Optional[list[mrd.MD_StandardOrderProcess]] = field(
+        default_factory=list
+    )
+    distributorFormat: Optional[list[mrd.MD_Format]] = field(default_factory=list)
+    distributorTransferOptions: Optional[list[mrd.MD_DigitalTransferOptions]] = field(
         default_factory=list
     )
-    distributorTransferOptions: Optional[
-        list[mrd.MD_DigitalTransferOptions]
-    ] = field(default_factory=list)
 
 
 @dataclass
 class MD_DigitalTransferOptions:
     unitsOfDistribution: Optional[gco.CharacterString] = None
     transferSize: Optional[gco.Real] = None
     onLine: Optional[list[cit.CI_OnlineResource]] = field(default_factory=list)
     offLine: Optional[list[mrd.MD_Medium]] = field(default_factory=list)
     transferFrequency: Optional[gco.TM_PeriodDuration] = None
-    distributionFormat: Optional[list[mrd.MD_Format]] = field(
-        default_factory=list
-    )
+    distributionFormat: Optional[list[mrd.MD_Format]] = field(default_factory=list)
 
 
 @dataclass
 class MD_Medium:
     name: Optional[cit.CI_Citation] = None
     density: Optional[gco.Real] = None
     densityUnits: Optional[gco.CharacterString] = None
@@ -55,17 +51,15 @@
 
 @dataclass
 class MD_Format:
     formatSpecificationCitation: cit.CI_Citation
     amendmentNumber: Optional[gco.CharacterString] = None
     fileDecompressionTechnique: Optional[gco.CharacterString] = None
     medium: Optional[list[mrd.MD_Medium]] = field(default_factory=list)
-    formatDistributor: Optional[list[mrd.MD_Distributor]] = field(
-        default_factory=list
-    )
+    formatDistributor: Optional[list[mrd.MD_Distributor]] = field(default_factory=list)
 
 
 @dataclass
 class MD_StandardOrderProcess:
     fees: Optional[gco.CharacterString] = None
     plannedAvailableDateTime: Optional[gco.DateTime] = None
     orderingInstructions: Optional[gco.CharacterString] = None
@@ -73,16 +67,12 @@
     orderOptionsType: Optional[gco.RecordType] = None
     orderOptions: Optional[gco.Record] = None
 
 
 @dataclass
 class MD_Distribution:
     description: Optional[gco.CharacterString] = None
-    distributionFormat: Optional[list[mrd.MD_Format]] = field(
-        default_factory=list
-    )
-    distributor: Optional[list[mrd.MD_Distributor]] = field(
-        default_factory=list
-    )
+    distributionFormat: Optional[list[mrd.MD_Format]] = field(default_factory=list)
+    distributor: Optional[list[mrd.MD_Distributor]] = field(default_factory=list)
     transferOptions: Optional[list[mrd.MD_DigitalTransferOptions]] = field(
         default_factory=list
     )
```

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/types/mri.py` & `ckanext-iso19115-0.1.1/ckanext/iso19115/types/mri.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,17 +57,15 @@
 @dataclass
 class MD_Usage:
     specificUsage: gco.CharacterString
     usageDateTime: Optional[list[gml.AbstractTimePrimitive]] = field(
         default_factory=list
     )
     userDeterminedLimitations: Optional[gco.CharacterString] = None
-    userContactInfo: Optional[list[cit.CI_Responsibility]] = field(
-        default_factory=list
-    )
+    userContactInfo: Optional[list[cit.CI_Responsibility]] = field(default_factory=list)
     response: Optional[list[gco.CharacterString]] = field(default_factory=list)
     additionalDocumentation: Optional[list[cit.CI_Citation]] = field(
         default_factory=list
     )
     identifiedIssues: Optional[cit.CI_Citation] = None
```

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/types/mrl.py` & `ckanext-iso19115-0.1.1/ckanext/iso19115/types/mrl.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,41 +8,33 @@
 
 
 @dataclass
 class LI_ProcessStep:
     description: gco.CharacterString
     rationale: Optional[gco.CharacterString] = None
     stepDateTime: Optional[gml.AbstractTimePrimitive] = None
-    processor: Optional[list[cit.CI_Responsibility]] = field(
-        default_factory=list
-    )
+    processor: Optional[list[cit.CI_Responsibility]] = field(default_factory=list)
     reference: Optional[list[cit.CI_Citation]] = field(default_factory=list)
     scope: Optional[mcc.MD_Scope] = None
     source: Optional[list[mrl.LI_Source]] = field(default_factory=list)
 
 
 @dataclass
 class LI_Source:
     description: Optional[gco.CharacterString] = None
     sourceSpatialResolution: Optional[mri.MD_Resolution] = None
     sourceReferenceSystem: Optional[mrs.MD_ReferenceSystem] = None
     sourceCitation: Optional[cit.CI_Citation] = None
-    sourceMetadata: Optional[list[cit.CI_Citation]] = field(
-        default_factory=list
-    )
+    sourceMetadata: Optional[list[cit.CI_Citation]] = field(default_factory=list)
     scope: Optional[mcc.MD_Scope] = None
-    sourceStep: Optional[list[mrl.LI_ProcessStep]] = field(
-        default_factory=list
-    )
+    sourceStep: Optional[list[mrl.LI_ProcessStep]] = field(default_factory=list)
 
 
 @dataclass
 class LI_Lineage:
     statement: Optional[gco.CharacterString] = None
     scope: Optional[mcc.MD_Scope] = None
     additionalDocumentation: Optional[list[cit.CI_Citation]] = field(
         default_factory=list
     )
     source: Optional[list[mrl.LI_Source]] = field(default_factory=list)
-    processStep: Optional[list[mrl.LI_ProcessStep]] = field(
-        default_factory=list
-    )
+    processStep: Optional[list[mrl.LI_ProcessStep]] = field(default_factory=list)
```

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/types/msr.py` & `ckanext-iso19115-0.1.1/ckanext/iso19115/types/msr.py`

 * *Files 8% similar despite different names*

```diff
@@ -54,10 +54,8 @@
     cellGeometry: Codelist[msr.MD_CellGeometryCode] = None
     transformationParameterAvailability: gco.Boolean = gco.Boolean(False)
 
 
 @dataclass
 class MD_VectorSpatialRepresentation(mcc.Abstract_SpatialRepresentation):
     topologyLevel: Optional[Codelist[MD_TopologyLevelCode]] = None
-    geometricObjects: Optional[list[MD_GeometricObjects]] = field(
-        default_factory=list
-    )
+    geometricObjects: Optional[list[MD_GeometricObjects]] = field(default_factory=list)
```

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/types/srv.py` & `ckanext-iso19115-0.1.1/ckanext/iso19115/types/srv.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,10 @@
     serviceTypeVersion: list[str] = field(default_factory=list)
     accessProperties: Optional[mrd.MD_StandardOrderProcess] = None
     couplingType: Optional[Codelist[srv.SV_CouplingType]] = None
     coupledResource: list[SV_CoupledResource] = field(default_factory=list)
     operatedDataset: list[cit.CI_Citation] = field(default_factory=list)
     profile: list[cit.CI_Citation] = field(default_factory=list)
     serviceStandard: list[cit.CI_Citation] = field(default_factory=list)
-    containsOperations: list[SV_OperationMetadata] = field(
-        default_factory=list
-    )
+    containsOperations: list[SV_OperationMetadata] = field(default_factory=list)
     operatesOn: list[mri.MD_DataIdentification] = field(default_factory=list)
-    containsChain: list[SV_OperationChainMetadata] = field(
-        default_factory=list
-    )
+    containsChain: list[SV_OperationChainMetadata] = field(default_factory=list)
```

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/utils.py` & `ckanext-iso19115-0.1.1/ckanext/iso19115/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,15 +87,14 @@
 
 def _get_cache_path(name):
     cache_dir = Path(tk.config.get(CONFIG_CACHE_DIR) or _tempdir)
     cache_dir.mkdir(parents=True, exist_ok=True)
     return cache_dir / f"{name}.pickle"
 
 
-
 def lookup(root: str, schema: xmlschema.XMLSchema):
     qualified_root = root
 
     try:
         _ns, tag = root.split(":")
         qualified_root = "{%s}%s" % (ns[_ns], tag)
     except (ValueError, KeyError):
@@ -117,17 +116,15 @@
     return el
 
 
 def _get_schema(name: str, rebuild: bool = False) -> xmlschema.XMLSchema:
     cache = _get_cache_path(name)
     if not cache.is_file() or rebuild:
         log.info("Building the cache at %s...", cache)
-        schema = xmlschema.XMLSchema(
-            str(_schema_mapping[name]), validation="lax"
-        )
+        schema = xmlschema.XMLSchema(str(_schema_mapping[name]), validation="lax")
         with cache.open("wb") as dest:
             pickle.dump(schema, dest)
     with cache.open("rb") as src:
         return pickle.load(src)
 
 
 def get_builder(root, name: str = DEFAULT_XSD) -> builder.Builder:
@@ -161,42 +158,36 @@
 def validate_schematron(content: bytes, schemas: Iterable[str] = frozenset()):
     errors = []
     if not schemas:
         schemas = _schematron_mapping.keys()
     for name in schemas:
         path = str(_schematron_mapping[name])
         with open(path, "rb") as src:
-            sch = isoschematron.Schematron(
-                ltree.XML(src.read()), store_report=True
-            )
+            sch = isoschematron.Schematron(ltree.XML(src.read()), store_report=True)
         if sch.validate(ltree.XML(content)):
             continue
 
         failed = sch.validation_report.xpath(
             "//*[local-name() = 'failed-assert']/*[text()]"
         )
-        errors.extend(
-            " ".join(l.strip() for l in f.itertext()) for f in failed
-        )
+        errors.extend(" ".join(l.strip() for l in f.itertext()) for f in failed)
     if errors:
         raise tk.ValidationError({"schematron": list(set(errors))})
 
 
 def validate_codelist(el: xtree.Element, xsd: xmlschema.XMLSchemaBase):
     if xsd.type.local_name != "CodeListValue_Type":
         return
     if xsd.local_name not in codelist_names():
         return
 
     validOptions = {c.name for c in codelist_options(xsd.local_name)}
     value = el.attrib["codeListValue"]
     if value not in validOptions:
-        reason = (
-            f"{value} is not a valid code. Valid options are: {validOptions}"
-        )
+        reason = f"{value} is not a valid code. Valid options are: {validOptions}"
         raise xmlschema.XMLSchemaValidationError(xsd, el, reason)
 
 
 def get_extra_validator(codelists: bool):
     def validator(el: xtree.Element, xsd: xmlschema.XMLSchemaBase):
         if codelists:
             validate_codelist(el, xsd)
@@ -220,17 +211,15 @@
     codes = xml.xpath(xpath, namespaces=namespaces)
 
     return [
         CodeListValue(
             code.find(
                 "cat:identifier/gco:ScopedName", namespaces=namespaces
             ).text.strip(),
-            code.find(
-                "cat:definition/gco:CharacterString", namespaces=namespaces
-            ).text,
+            code.find("cat:definition/gco:CharacterString", namespaces=namespaces).text,
         )
         for code in codes
     ]
 
 
 @functools.lru_cache(1)
 def enum_elements(name: str = DEFAULT_XSD) -> dict[str, xmlschema.XsdElement]:
@@ -244,11 +233,9 @@
     }
 
 
 @functools.lru_cache()
 def enum_values(name: str, schema: str = DEFAULT_XSD) -> Optional[list[Any]]:
     el = enum_elements(schema)[name]
     if el.local_name == name:
-        type_ = cast(
-            xmlschema.validators.simple_types.XsdAtomicRestriction, el.type
-        )
+        type_ = cast(xmlschema.validators.simple_types.XsdAtomicRestriction, el.type)
         return type_.enumeration
```

### Comparing `ckanext-iso19115-0.1.0/ckanext/iso19115/views.py` & `ckanext-iso19115-0.1.1/ckanext/iso19115/views.py`

 * *Files 11% similar despite different names*

```diff
@@ -37,10 +37,8 @@
 
     def _render(self, data=None, errors=None):
         extra_vars = {"data": data, "errors": errors}
 
         return tk.render("iso19115/validate.html", extra_vars)
 
 
-iso19115.add_url_rule(
-    "/-iso19115/validate", view_func=ValidateView.as_view("validate")
-)
+iso19115.add_url_rule("/-iso19115/validate", view_func=ValidateView.as_view("validate"))
```

### Comparing `ckanext-iso19115-0.1.0/ckanext_iso19115.egg-info/SOURCES.txt` & `ckanext-iso19115-0.1.1/ckanext_iso19115.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ckanext-iso19115-0.1.0/setup.cfg` & `ckanext-iso19115-0.1.1/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ckanext-iso19115
-version = 0.1.0
+version = 0.1.1
 description = 
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/DataShades/ckanext-iso19115
 author = Sergey Motornyuk
 author_email = sergey.motornyuk@linkdigital.com.au
 license = AGPL
```

