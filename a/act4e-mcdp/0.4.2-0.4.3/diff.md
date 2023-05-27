# Comparing `tmp/act4e_mcdp-0.4.2-py3-none-any.whl.zip` & `tmp/act4e_mcdp-0.4.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 22388 bytes, number of entries: 14
+Zip file size: 35412 bytes, number of entries: 14
 -rw-r--r--  2.0 unx      347 b- defN 80-Jan-01 00:00 act4e_mcdp/__init__.py
--rw-r--r--  2.0 unx    30570 b- defN 80-Jan-01 00:00 act4e_mcdp/autogen_packed_test_data.py
+-rw-r--r--  2.0 unx    67896 b- defN 80-Jan-01 00:00 act4e_mcdp/autogen_packed_test_data.py
 -rw-r--r--  2.0 unx      571 b- defN 80-Jan-01 00:00 act4e_mcdp/download.py
--rw-r--r--  2.0 unx     9138 b- defN 80-Jan-01 00:00 act4e_mcdp/loading.py
+-rw-r--r--  2.0 unx    10217 b- defN 80-Jan-01 00:00 act4e_mcdp/loading.py
 -rw-r--r--  2.0 unx     3363 b- defN 80-Jan-01 00:00 act4e_mcdp/main.py
 -rw-r--r--  2.0 unx     4381 b- defN 80-Jan-01 00:00 act4e_mcdp/nameddps.py
 -rw-r--r--  2.0 unx     1790 b- defN 80-Jan-01 00:00 act4e_mcdp/posets.py
--rw-r--r--  2.0 unx    10766 b- defN 80-Jan-01 00:00 act4e_mcdp/primitivedps.py
+-rw-r--r--  2.0 unx    11777 b- defN 80-Jan-01 00:00 act4e_mcdp/primitivedps.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 act4e_mcdp/py.typed
 -rw-r--r--  2.0 unx     3944 b- defN 80-Jan-01 00:00 act4e_mcdp/solution_interface.py
--rw-r--r--  2.0 unx      361 b- defN 80-Jan-01 00:00 act4e_mcdp-0.4.2.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 act4e_mcdp-0.4.2.dist-info/WHEEL
--rw-r--r--  2.0 unx      109 b- defN 80-Jan-01 00:00 act4e_mcdp-0.4.2.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     1120 b- defN 16-Jan-01 00:00 act4e_mcdp-0.4.2.dist-info/RECORD
-14 files, 66548 bytes uncompressed, 20536 bytes compressed:  69.1%
+-rw-r--r--  2.0 unx      361 b- defN 80-Jan-01 00:00 act4e_mcdp-0.4.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 act4e_mcdp-0.4.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx      109 b- defN 80-Jan-01 00:00 act4e_mcdp-0.4.3.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     1121 b- defN 16-Jan-01 00:00 act4e_mcdp-0.4.3.dist-info/RECORD
+14 files, 105965 bytes uncompressed, 33560 bytes compressed:  68.3%
```

## zipnote {}

```diff
@@ -24,20 +24,20 @@
 
 Filename: act4e_mcdp/py.typed
 Comment: 
 
 Filename: act4e_mcdp/solution_interface.py
 Comment: 
 
-Filename: act4e_mcdp-0.4.2.dist-info/METADATA
+Filename: act4e_mcdp-0.4.3.dist-info/METADATA
 Comment: 
 
-Filename: act4e_mcdp-0.4.2.dist-info/WHEEL
+Filename: act4e_mcdp-0.4.3.dist-info/WHEEL
 Comment: 
 
-Filename: act4e_mcdp-0.4.2.dist-info/entry_points.txt
+Filename: act4e_mcdp-0.4.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: act4e_mcdp-0.4.2.dist-info/RECORD
+Filename: act4e_mcdp-0.4.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## act4e_mcdp/autogen_packed_test_data.py

```diff
@@ -106,76 +106,132 @@
 
 
 __all__ = [
     "lib1_parts_discrete_posets_mcdpr1_yaml",
     "lib1_parts_discrete_posets_mcdpr1_yaml_fresh",
     "lib1_parts_e01_empty_models_mcdpr1_yaml",
     "lib1_parts_e01_empty_models_mcdpr1_yaml_fresh",
+    "lib1_parts_e01_empty_primitivedps_mcdpr1_yaml",
+    "lib1_parts_e01_empty_primitivedps_mcdpr1_yaml_fresh",
     "lib1_parts_e02_direct_connection_models_mcdpr1_yaml",
     "lib1_parts_e02_direct_connection_models_mcdpr1_yaml_fresh",
+    "lib1_parts_e02_direct_connection_primitivedps_mcdpr1_yaml",
+    "lib1_parts_e02_direct_connection_primitivedps_mcdpr1_yaml_fresh",
     "lib1_parts_e03_splitter1_models_mcdpr1_yaml",
     "lib1_parts_e03_splitter1_models_mcdpr1_yaml_fresh",
+    "lib1_parts_e03_splitter1_primitivedps_mcdpr1_yaml",
+    "lib1_parts_e03_splitter1_primitivedps_mcdpr1_yaml_fresh",
     "lib1_parts_e04_splitter2_models_mcdpr1_yaml",
     "lib1_parts_e04_splitter2_models_mcdpr1_yaml_fresh",
+    "lib1_parts_e04_splitter2_primitivedps_mcdpr1_yaml",
+    "lib1_parts_e04_splitter2_primitivedps_mcdpr1_yaml_fresh",
     "lib1_parts_e05_multf_models_mcdpr1_yaml",
     "lib1_parts_e05_multf_models_mcdpr1_yaml_fresh",
+    "lib1_parts_e05_multf_primitivedps_mcdpr1_yaml",
+    "lib1_parts_e05_multf_primitivedps_mcdpr1_yaml_fresh",
     "lib1_parts_e05_multr_models_mcdpr1_yaml",
     "lib1_parts_e05_multr_models_mcdpr1_yaml_fresh",
+    "lib1_parts_e05_multr_primitivedps_mcdpr1_yaml",
+    "lib1_parts_e05_multr_primitivedps_mcdpr1_yaml_fresh",
     "lib1_parts_e05_scalef_models_mcdpr1_yaml",
     "lib1_parts_e05_scalef_models_mcdpr1_yaml_fresh",
+    "lib1_parts_e05_scalef_primitivedps_mcdpr1_yaml",
+    "lib1_parts_e05_scalef_primitivedps_mcdpr1_yaml_fresh",
     "lib1_parts_e05_scaler_models_mcdpr1_yaml",
     "lib1_parts_e05_scaler_models_mcdpr1_yaml_fresh",
+    "lib1_parts_e05_scaler_primitivedps_mcdpr1_yaml",
+    "lib1_parts_e05_scaler_primitivedps_mcdpr1_yaml_fresh",
     "lib1_parts_e05_sumf_models_mcdpr1_yaml",
     "lib1_parts_e05_sumf_models_mcdpr1_yaml_fresh",
+    "lib1_parts_e05_sumf_primitivedps_mcdpr1_yaml",
+    "lib1_parts_e05_sumf_primitivedps_mcdpr1_yaml_fresh",
     "lib1_parts_e06_addf_models_mcdpr1_yaml",
     "lib1_parts_e06_addf_models_mcdpr1_yaml_fresh",
+    "lib1_parts_e06_addf_primitivedps_mcdpr1_yaml",
+    "lib1_parts_e06_addf_primitivedps_mcdpr1_yaml_fresh",
     "lib1_parts_e06_addr_models_mcdpr1_yaml",
     "lib1_parts_e06_addr_models_mcdpr1_yaml_fresh",
+    "lib1_parts_e06_addr_primitivedps_mcdpr1_yaml",
+    "lib1_parts_e06_addr_primitivedps_mcdpr1_yaml_fresh",
     "lib1_parts_e06_sumr_models_mcdpr1_yaml",
     "lib1_parts_e06_sumr_models_mcdpr1_yaml_fresh",
+    "lib1_parts_e06_sumr_primitivedps_mcdpr1_yaml",
+    "lib1_parts_e06_sumr_primitivedps_mcdpr1_yaml_fresh",
     "lib1_parts_e07_ceil_models_mcdpr1_yaml",
     "lib1_parts_e07_ceil_models_mcdpr1_yaml_fresh",
+    "lib1_parts_e07_ceil_primitivedps_mcdpr1_yaml",
+    "lib1_parts_e07_ceil_primitivedps_mcdpr1_yaml_fresh",
     "lib1_parts_e07_floor_models_mcdpr1_yaml",
     "lib1_parts_e07_floor_models_mcdpr1_yaml_fresh",
+    "lib1_parts_e07_floor_primitivedps_mcdpr1_yaml",
+    "lib1_parts_e07_floor_primitivedps_mcdpr1_yaml_fresh",
     "lib1_parts_e10_conversions1_models_mcdpr1_yaml",
     "lib1_parts_e10_conversions1_models_mcdpr1_yaml_fresh",
+    "lib1_parts_e10_conversions1_primitivedps_mcdpr1_yaml",
+    "lib1_parts_e10_conversions1_primitivedps_mcdpr1_yaml_fresh",
     "lib1_parts_e10_conversions2_models_mcdpr1_yaml",
     "lib1_parts_e10_conversions2_models_mcdpr1_yaml_fresh",
+    "lib1_parts_e10_conversions2_primitivedps_mcdpr1_yaml",
+    "lib1_parts_e10_conversions2_primitivedps_mcdpr1_yaml_fresh",
     "lib1_parts_e11_constant_fun_models_mcdpr1_yaml",
     "lib1_parts_e11_constant_fun_models_mcdpr1_yaml_fresh",
+    "lib1_parts_e11_constant_fun_primitivedps_mcdpr1_yaml",
+    "lib1_parts_e11_constant_fun_primitivedps_mcdpr1_yaml_fresh",
     "lib1_parts_e11_constant_res_models_mcdpr1_yaml",
     "lib1_parts_e11_constant_res_models_mcdpr1_yaml_fresh",
+    "lib1_parts_e11_constant_res_primitivedps_mcdpr1_yaml",
+    "lib1_parts_e11_constant_res_primitivedps_mcdpr1_yaml_fresh",
+    "lib1_parts_e12_catalogue_empty_models_mcdpr1_yaml",
+    "lib1_parts_e12_catalogue_empty_models_mcdpr1_yaml_fresh",
+    "lib1_parts_e12_catalogue_empty_primitivedps_mcdpr1_yaml",
+    "lib1_parts_e12_catalogue_empty_primitivedps_mcdpr1_yaml_fresh",
+    "lib1_parts_e12_catalogue_models_mcdpr1_yaml",
+    "lib1_parts_e12_catalogue_models_mcdpr1_yaml_fresh",
+    "lib1_parts_e12_catalogue_primitivedps_mcdpr1_yaml",
+    "lib1_parts_e12_catalogue_primitivedps_mcdpr1_yaml_fresh",
+    "lib1_parts_e12_catalogue_true_models_mcdpr1_yaml",
+    "lib1_parts_e12_catalogue_true_models_mcdpr1_yaml_fresh",
+    "lib1_parts_e12_catalogue_true_primitivedps_mcdpr1_yaml",
+    "lib1_parts_e12_catalogue_true_primitivedps_mcdpr1_yaml_fresh",
     "lib1_parts_nats_posets_mcdpr1_yaml",
     "lib1_parts_nats_posets_mcdpr1_yaml_fresh",
     "lib1_parts_reals_posets_mcdpr1_yaml",
     "lib1_parts_reals_posets_mcdpr1_yaml_fresh",
     "lib1_parts_reals_with_units_posets_mcdpr1_yaml",
     "lib1_parts_reals_with_units_posets_mcdpr1_yaml_fresh",
+    "lib1_simple_all_together_models_mcdpr1_yaml",
+    "lib1_simple_all_together_models_mcdpr1_yaml_fresh",
+    "lib1_simple_all_together_primitivedps_mcdpr1_yaml",
+    "lib1_simple_all_together_primitivedps_mcdpr1_yaml_fresh",
+    "lib1_simple_drone1_models_mcdpr1_yaml",
+    "lib1_simple_drone1_models_mcdpr1_yaml_fresh",
+    "lib1_simple_drone1_primitivedps_mcdpr1_yaml",
+    "lib1_simple_drone1_primitivedps_mcdpr1_yaml_fresh",
     "resources",
 ]
 
 
 lib1_parts_discrete_posets_mcdpr1_yaml: str = decode_to_str(
-    b"eJxNirsNwCAMBXumcJE2CzBA6qzA50lYASMF768YaFKcdH6+Y6SCFrwjUtYKTxcLK+4+oDY+LNnTvlDR"
-    b"IDq8OykYxUhGNqIB96IG5S4rmRHRfs1wel4el+Pn+dcn9wFHAiR4",
+    b"eJxNirsJwDAMBXtPoSJtFtAAqbOCPw8s4g/E2p/IdpPi4PR0x4gZ1bMjUtECpkuaKO4+oDY+0hLTvlBQ"
+    b"0XSwOyka2UiGN2AE96J4ld5WMiOinczndPx87355+Hl0H0euJHg=",
 )
 
 
 def lib1_parts_discrete_posets_mcdpr1_yaml_fresh() -> str:
     return get_updated_str(
         lib1_parts_discrete_posets_mcdpr1_yaml,
         "../../assets/test-data/downloaded/lib1-parts.discrete.posets.mcdpr1.yaml",
     )
 
 
 _check_md5(
     "lib1_parts_discrete_posets_mcdpr1_yaml",
     lib1_parts_discrete_posets_mcdpr1_yaml,
     149,
-    "c9661b0bd5daf948643f6b0043954d36",
+    "563123836404de299f7bdaa92f0d0dd7",
     "../../assets/test-data/downloaded/lib1-parts.discrete.posets.mcdpr1.yaml",
 )
 lib1_parts_e01_empty_models_mcdpr1_yaml: str = decode_to_str(
     b"eJw1yjEOgCAMheGdU3TwFKw6G3fjQKDGRmgNlMl4d4nB7X15/1D8gclZA6CkES2Mki4ppDi7hGFa2nMS"
     b"Bwu/98peSdhFUsJi4X5MxiI1+y6W0JcXZvzq5nUzL1bHJqc=",
 )
 
@@ -190,14 +246,35 @@
 _check_md5(
     "lib1_parts_e01_empty_models_mcdpr1_yaml",
     lib1_parts_e01_empty_models_mcdpr1_yaml,
     111,
     "5eded1fa7fca3ac02260dc9224ff0e72",
     "../../assets/test-data/downloaded/lib1-parts.e01_empty.models.mcdpr1.yaml",
 )
+lib1_parts_e01_empty_primitivedps_mcdpr1_yaml: str = decode_to_str(
+    b"eJxTKU7OSM1NtOJSUCjJLMlJtVLwLa0AcrIz81KsFAKKMnMzSzLLUl0CgGIpqcXJRZkFJZn5eVYKuaUV"
+    b"GmmaCo86lygUcbmB9KsgjILrzy9OLQHzoYaDBQKK8lNKk0HixaVJxVYK0bFcyfn5RSnFGKZAdTmDZT1T"
+    b"UvOAApVQxUa4VecWAK3xySwGWZEM4uUBdUIsCqLUpYl5eVZcALe2YXI=",
+)
+
+
+def lib1_parts_e01_empty_primitivedps_mcdpr1_yaml_fresh() -> str:
+    return get_updated_str(
+        lib1_parts_e01_empty_primitivedps_mcdpr1_yaml,
+        "../../assets/test-data/downloaded/lib1-parts.e01_empty.primitivedps.mcdpr1.yaml",
+    )
+
+
+_check_md5(
+    "lib1_parts_e01_empty_primitivedps_mcdpr1_yaml",
+    lib1_parts_e01_empty_primitivedps_mcdpr1_yaml,
+    308,
+    "6ca825ed2c62bbc0252e71e62cf4e890",
+    "../../assets/test-data/downloaded/lib1-parts.e01_empty.primitivedps.mcdpr1.yaml",
+)
 lib1_parts_e02_direct_connection_models_mcdpr1_yaml: str = decode_to_str(
     b"eJy9kDsOwjAMhvecwkOlTkjMWWFhqXqFPhxh0dhV4gwIcXeStBWcgAxW/Pvx2W7idEc/WAOgpAtauIhf"
     b"JZJiN3icr32OPIhnC4fvEk9KwsNCShhLqSsGoPk2K28r6yWi7sqO6JIfMcQqjqIq3kJ7bquvslq4sSMm"
     b"fVYl5V/MCa0JGCWFaWOG/zBZ5syD19tMwox188w/gQu5RU3+PcjTgiu3lC10TGwhmA+kLGsW",
 )
 
 
@@ -211,14 +288,35 @@
 _check_md5(
     "lib1_parts_e02_direct_connection_models_mcdpr1_yaml",
     lib1_parts_e02_direct_connection_models_mcdpr1_yaml,
     363,
     "b6057c5b1d569ea09dfeb12e782cfacd",
     "../../assets/test-data/downloaded/lib1-parts.e02_direct_connection.models.mcdpr1.yaml",
 )
+lib1_parts_e02_direct_connection_primitivedps_mcdpr1_yaml: str = decode_to_str(
+    b"eJy1jUEKwkAMRfdziiwKs3WdtQhupHiDtpNi0EnKTCr0CN7Dk3kS0yJ6AlfJfyHvN3W4UO4wABjbjRCO"
+    b"icTXZd86u7IkhLZwZuM7bSxRHQpPxioII7weTyjhsBqan+z7qpVsyx/9ac49leqoVzPNCHEX13advFtG"
+    b"Fu/2PPusfozh/D91J4LhDfC/Tn8=",
+)
+
+
+def lib1_parts_e02_direct_connection_primitivedps_mcdpr1_yaml_fresh() -> str:
+    return get_updated_str(
+        lib1_parts_e02_direct_connection_primitivedps_mcdpr1_yaml,
+        "../../assets/test-data/downloaded/lib1-parts.e02_direct_connection.primitivedps.mcdpr1.yaml",
+    )
+
+
+_check_md5(
+    "lib1_parts_e02_direct_connection_primitivedps_mcdpr1_yaml",
+    lib1_parts_e02_direct_connection_primitivedps_mcdpr1_yaml,
+    257,
+    "d83b088af959eb075da77089b6496018",
+    "../../assets/test-data/downloaded/lib1-parts.e02_direct_connection.primitivedps.mcdpr1.yaml",
+)
 lib1_parts_e03_splitter1_models_mcdpr1_yaml: str = decode_to_str(
     b"eJzNVT1uwyAU3nOKN0TyFCnJyJqoUodGUTt0RMQGldaAxU+ljM3U3qNDz5WTFIgd27HdIUNcBgse8P3w"
     b"8GNq0hcqCJoAWG5zimClRKEMt3RDBM3WWz/zxmWGoBozJ1PLlSQ5t5yasJWFD8C0BgvttG2rDLVlpKTY"
     b"OLGj2sTgTlmrBIJknsSxVQWCe8m45HYfI873jF+QTDQ1yun0xKnx4jasgWp5GyqpspM5/Kq4xEz6I+93"
     b"WRI9cVHk9FmToiWpTp3PTTddoeEzVAe739qAvT6L/TYvT9WfazOfURTD8/FlRR2L8XVkRUXZUVAyPVBq"
     b"N2tH8jLXDWmaC5/vd9qY8Xcr1bwIlwEBg+PXt0/B8fABx8+f0DmUK+/Gtw6w+g8iiJQV6+P1emJ4q1Xm"
     b"0nrWuJ2pEWZ9oEOwg0b7rQ6Z7dodX0eqpKSxXPnDmQHTHiQuDJURtcriOYyrMoJi/QgvmUKt+oLCY3Ed"
@@ -236,14 +334,36 @@
 _check_md5(
     "lib1_parts_e03_splitter1_models_mcdpr1_yaml",
     lib1_parts_e03_splitter1_models_mcdpr1_yaml,
     1927,
     "ac5e9a2f4da020e29c7ff2a8c893dc6e",
     "../../assets/test-data/downloaded/lib1-parts.e03_splitter1.models.mcdpr1.yaml",
 )
+lib1_parts_e03_splitter1_primitivedps_mcdpr1_yaml: str = decode_to_str(
+    b"eJy9jjsOwjAMhveewkOlTkjMWamQGKgqbtCHKyyaBCUOEiOd4B4MnKsnIakQrzKwwOT4i/35j221RlmI"
+    b"CICJWxSwROQsdUWb5h5uSNUCckOSmHY4sBptZWjLpJWABvrTGcD03QH64yU8umgefPFDffdoizz0t2OZ"
+    b"kyUa61GpmbUUkEyTkEVvBSxUQ4p473vnq/WfSTT7nbpQSkSrb/0DyI2uXRW4daUN85PX5fH6h4DvEcch"
+    b"n2P+48YVYqGeHw==",
+)
+
+
+def lib1_parts_e03_splitter1_primitivedps_mcdpr1_yaml_fresh() -> str:
+    return get_updated_str(
+        lib1_parts_e03_splitter1_primitivedps_mcdpr1_yaml,
+        "../../assets/test-data/downloaded/lib1-parts.e03_splitter1.primitivedps.mcdpr1.yaml",
+    )
+
+
+_check_md5(
+    "lib1_parts_e03_splitter1_primitivedps_mcdpr1_yaml",
+    lib1_parts_e03_splitter1_primitivedps_mcdpr1_yaml,
+    527,
+    "c37493fb59793a7824e39769ee9e72df",
+    "../../assets/test-data/downloaded/lib1-parts.e03_splitter1.primitivedps.mcdpr1.yaml",
+)
 lib1_parts_e04_splitter2_models_mcdpr1_yaml: str = decode_to_str(
     b"eJzNVb1uwyAQ3vMUN0TKFCnJyJqqUjtEUTt0tIiNVdrAWYArZWym9j069Ln8JAWMazu2M2SIw2K4M98P"
     b"h46pjl+ZoGQCYLjZMwJrFBlqbtiGCpbcbW3mncuEQLVOcxkbjpLuueFMu61ptHQfgGkN50a5cYuamRAJ"
     b"JJtc7JjSPrhDY1AQmC1mfm0wI/AgUy65OfhIbmfa/jDzVKvrUCmmMVdxaVBdh1NiUvJFb8hllEp75P0n"
     b"G4ieucj27EXRrCWpLp09sG653IhUtKjmHfR+cwMG+0z2Gz2tZdCxHF9Hq9heFh1fVJJVlB0FgenR3pJN"
     b"qHNDluLC1vqDNTL2XsWKZ+4iEEiL4ycUX79ucoTi+wdU+HE9vmuAp1sQQaWsWO8v1+PDW4VJHtdZne90"
     b"jTDvAx2CHTTab3XIbNfu+DpilJL5TmUPZw6psiCdBnYg7q1xjxWWSdcxSatd/oejk42u450HXl0MvGwB"
@@ -261,14 +381,36 @@
 _check_md5(
     "lib1_parts_e04_splitter2_models_mcdpr1_yaml",
     lib1_parts_e04_splitter2_models_mcdpr1_yaml,
     1932,
     "8bb893879ecd7ec400103d18ca2c516f",
     "../../assets/test-data/downloaded/lib1-parts.e04_splitter2.models.mcdpr1.yaml",
 )
+lib1_parts_e04_splitter2_primitivedps_mcdpr1_yaml: str = decode_to_str(
+    b"eJy9jjsOwjAMhvecwkOlTkjMXkFIMFQVN+gjFRYkQYmDxEgnuAcD5+pJSCrEqwwsMDn+Yn/+E1etpCpQ"
+    b"ADDxRiIsDOlsmgewJl0j5JYUMe1kz2rpKktbJqMRmq49QHe8xEcL3ekMVkyiKnlY7xrjJPf97U7mVSmt"
+    b"C6g0zEYhpOM0xjBbhLluSBPvQ+9DdeEzFcvfqQutUcy+9fcgt6b2VeTOly7Oj16Xh+sfAr5HHIZ8jvmP"
+    b"G1foupxy",
+)
+
+
+def lib1_parts_e04_splitter2_primitivedps_mcdpr1_yaml_fresh() -> str:
+    return get_updated_str(
+        lib1_parts_e04_splitter2_primitivedps_mcdpr1_yaml,
+        "../../assets/test-data/downloaded/lib1-parts.e04_splitter2.primitivedps.mcdpr1.yaml",
+    )
+
+
+_check_md5(
+    "lib1_parts_e04_splitter2_primitivedps_mcdpr1_yaml",
+    lib1_parts_e04_splitter2_primitivedps_mcdpr1_yaml,
+    522,
+    "ccaf3abae85cdb986424751303ff2306",
+    "../../assets/test-data/downloaded/lib1-parts.e04_splitter2.primitivedps.mcdpr1.yaml",
+)
 lib1_parts_e05_multf_models_mcdpr1_yaml: str = decode_to_str(
     b"eJzFVb1uwyAQ3vMUDJE8RUoysraq1CFRlA4dEcFYRbUB8VPJYyN1qPoafbI8SQHj2olxh6iKWYA7833f"
     b"3eFjrskLrTCcAWCYKSkEd6KSQjNDt7ii+f3OeV4ZzyFo94XlxDDBcckMo9ofLdDKTwDMOzg/moM7oamJ"
     b"lkiytdWBKh2MB2GMqCDIllnYGyEheOQF48zUwWLdSrsPskC1vg2VolpYRZoA1W04ucgbPiSVyNM5jRRP"
     b"rJIlfVZYnonpiuZSNSyUH0jIZbseoKfDGgktFV46xMsqRh2r6XWclTnIUt16Olm5bCkHCiLTBu2pRhtb"
     b"GibLeoN5jWLdeyIVq1zt32jP424YUUz6iwFBcTq+n74+3HQEp89voOJn++kzAICQWmJC/1/KYkCdEoQ5"
     b"b5kertcQzDv3N1vSebU99O7YIgU6BjsaXDrTY7keZnt6HURwTkPHcslZgEI5kEEjq6F/bfxzJRqn75kw"
@@ -286,14 +428,36 @@
 _check_md5(
     "lib1_parts_e05_multf_models_mcdpr1_yaml",
     lib1_parts_e05_multf_models_mcdpr1_yaml,
     1918,
     "cf9998520ab5d047b14a6f529f66a15e",
     "../../assets/test-data/downloaded/lib1-parts.e05_multf.models.mcdpr1.yaml",
 )
+lib1_parts_e05_multf_primitivedps_mcdpr1_yaml: str = decode_to_str(
+    b"eJy9kL8KwkAMxvc+RQahk+B8swgOleILlP65YrC9Oy45oaMFB/E1fLI+idciaq2DODiFfEm+X5IZ5TtZ"
+    b"pyIAYORKCoiSraQkchWjqZooVU2yjH15j6oQEFuskfEgB62QlFs0jFoJKLv22F1OPrTQna9gg21vO3sS"
+    b"HiaaJA/5nblxdSYteSnTzLoWEC7CfiVtBKxViQq58bnzkXwxDLQhk+byd8D8xXaMSZUSwepb50GIrS5c"
+    b"3uvkMur75+Ph6fiH1d6vn97/+oF/MG7Sp6Q5",
+)
+
+
+def lib1_parts_e05_multf_primitivedps_mcdpr1_yaml_fresh() -> str:
+    return get_updated_str(
+        lib1_parts_e05_multf_primitivedps_mcdpr1_yaml,
+        "../../assets/test-data/downloaded/lib1-parts.e05_multf.primitivedps.mcdpr1.yaml",
+    )
+
+
+_check_md5(
+    "lib1_parts_e05_multf_primitivedps_mcdpr1_yaml",
+    lib1_parts_e05_multf_primitivedps_mcdpr1_yaml,
+    534,
+    "5328f1843337ca06d23a7c57bb94d9f5",
+    "../../assets/test-data/downloaded/lib1-parts.e05_multf.primitivedps.mcdpr1.yaml",
+)
 lib1_parts_e05_multr_models_mcdpr1_yaml: str = decode_to_str(
     b"eJzFVb1qwzAQ3vMUGgKeAklGrS2BDgmhHToaR5apqPWDfgIeG+hQ+hp9sjxJT7JdO7G8hBJrsK2T7vu+"
     b"u5NPc0PeKM/wDCHLbEkxepBcScMs3WWc5o97WHlnIseonRdOEMukyEpmGTXetfAPhOYdmB+1214aahtL"
     b"Q7Fz/EC1CcaDtFZyjJJlEuZWKoyeRMEEs1WwOPgysCGZaWqk06Tm1OnqPqyean0fKiHzOriUiSN3pY2H"
     b"2LC8MK5K+qozdaGnqxsUZlgrP1LIJKC30wFBPLiRAGNBxgO9zitktl/RoEwqs5xeVy1kNb2QXLWUAwUN"
     b"0zbdOJFuoZxMldU2E1XaFL8nUjMOB+BIeytw0ohmyp8OjAp0/vpB+nz6OH9/wuvUbNtMnwGEoBIqI/T/"
     b"pSwG1DFBmRAt0/PtGoJ5r2XuSLdq3MF0CIsY6BjsaHDxTI/lepjt6XUQKQQNbQuSs0CFBpCw0bdH3PXG"
@@ -311,14 +475,36 @@
 _check_md5(
     "lib1_parts_e05_multr_models_mcdpr1_yaml",
     lib1_parts_e05_multr_models_mcdpr1_yaml,
     1930,
     "15ea7bc6c0929b1c749e6a4ac925223f",
     "../../assets/test-data/downloaded/lib1-parts.e05_multr.models.mcdpr1.yaml",
 )
+lib1_parts_e05_multr_primitivedps_mcdpr1_yaml: str = decode_to_str(
+    b"eJy9kL8KwkAMxvc+RYZCp4LzzVJwqBRfoPTPFYPt3XGXEzpacBBfwyfrk3gtoq11EAenkC/J90vim2LP"
+    b"m4x5AIRUcwZxGlmRxrYmVHUbZ6JN14krH1CUDBKNDRIe+aiV3BQaFaEUDCroLzfQfXfqr2cXOi8abP0X"
+    b"4WkiDacxfzC3tsm5Nk7KJZFsGASrYFhJKgYbUaFAal1uXTSuGHhSGZUV/HdAOLGdYzIhmLf71nkUEi1L"
+    b"Wwy6sbkZ+sP58HL8w2rv1y/vn37gH4w709OkRA==",
+)
+
+
+def lib1_parts_e05_multr_primitivedps_mcdpr1_yaml_fresh() -> str:
+    return get_updated_str(
+        lib1_parts_e05_multr_primitivedps_mcdpr1_yaml,
+        "../../assets/test-data/downloaded/lib1-parts.e05_multr.primitivedps.mcdpr1.yaml",
+    )
+
+
+_check_md5(
+    "lib1_parts_e05_multr_primitivedps_mcdpr1_yaml",
+    lib1_parts_e05_multr_primitivedps_mcdpr1_yaml,
+    534,
+    "3e8afb2d48f9fc8b8f816a9c04daa3b1",
+    "../../assets/test-data/downloaded/lib1-parts.e05_multr.primitivedps.mcdpr1.yaml",
+)
 lib1_parts_e05_scalef_models_mcdpr1_yaml: str = decode_to_str(
     b"eJzNVEtqwzAQ3fsUswhkFUi22qYEukgoKbRLo9gyFbU0Qp9ADtBF6TV6spykki3Xdqx0VZp6YaSRZt68"
     b"N/abmeKFCUoyAMttzQisUSg03LIdFay8e/Anr1yWBLp95WRhOUpac8uZCalVeAHM+mLhadMe0DAbIxFi"
     b"58SBadMED2gtCgLz5bzZW1QE7mXFJbenJuL8yvgL80wzg04XLab+G0yJZYuXC1fbVRI0QjxyoWr2rKka"
     b"NdPr6IWaaheeHNWyW0+qp2ldoZail6Y4phl2I3mbtnS/vl1bpeogJx1EpG2+Zybf+vlwVZ/WKI2l0uZR"
     b"80Gjmguv+5ENTvx0C81VGAqBCs4fb7Bawvn9E3S8s7m9BABH92MXEe+J1o5tNIpxP8cQ9sVWA1gVbgxL"
     b"JKpeY3eV34DhECuSvIhdUkRlFC3Y76u9mKib0nz/H8ZMpSRZgVKyxib837eAys+TTNzj5L/WYNrYHgWb"
@@ -336,14 +522,36 @@
 _check_md5(
     "lib1_parts_e05_scalef_models_mcdpr1_yaml",
     lib1_parts_e05_scalef_models_mcdpr1_yaml,
     1589,
     "3974b96a2701df7c01207fda12ee89fd",
     "../../assets/test-data/downloaded/lib1-parts.e05_scalef.models.mcdpr1.yaml",
 )
+lib1_parts_e05_scalef_primitivedps_mcdpr1_yaml: str = decode_to_str(
+    b"eJy1ULsKwjAU3fsVdxA6CbpmVQQHRTq4lrRe8WLzILkp+AEO4m/4ZX6Jaa2PopPgFM5JziNn4MsdKikS"
+    b"ACauUMAiz9Dni1Ax2eowMdqz1JxPV/HJnvRGwMqRIqYaW26DvnRkmYwWsIXr+QjjEVxPF3DJrPEdvCKe"
+    b"DsYjt7gLXQZVoPORKgyzUQLSUdp0MlbAXG9JEx8iDvH08TJN6vDh3XmtZRVw5ox6pNQNEUXj1tI27F3Q"
+    b"U392+9Lurd/drav4RK+CxnorS/x9geHbv/s7ZP+bVWotkhty7J+C",
+)
+
+
+def lib1_parts_e05_scalef_primitivedps_mcdpr1_yaml_fresh() -> str:
+    return get_updated_str(
+        lib1_parts_e05_scalef_primitivedps_mcdpr1_yaml,
+        "../../assets/test-data/downloaded/lib1-parts.e05_scalef.primitivedps.mcdpr1.yaml",
+    )
+
+
+_check_md5(
+    "lib1_parts_e05_scalef_primitivedps_mcdpr1_yaml",
+    lib1_parts_e05_scalef_primitivedps_mcdpr1_yaml,
+    529,
+    "628d0a553ce019bf5a45011ff74c5414",
+    "../../assets/test-data/downloaded/lib1-parts.e05_scalef.primitivedps.mcdpr1.yaml",
+)
 lib1_parts_e05_scaler_models_mcdpr1_yaml: str = decode_to_str(
     b"eJzNVMlOwzAQvecr5lCpp4r26mtRJQ5FFUhwjNzEERbxIi+R+gn8B1/GlzBOHOos7QlRfIjiZebNe7Ms"
     b"bPHGBCUZgOOuZgS2SmhluWOPVLDy/oA371yWBPp95WXhuJK05o4zG0yr8AFYnJ2F1ZkdlGUunkSIRy+O"
     b"zNj28KicU4LAcr1s905pAg+y4pK7U3vi8c/ig2VmmFXeFB2m+RtMqcoOL+eyEb52Da0928yCR6hnLnTN"
     b"Xg3Vg6DOeqJgUw3DypEhQvTbCcA8wwss55jOsx0yDruB0m1kStv17eMqdQ85iSAi7fOdl/keVeS6Pm2V"
     b"tI5Kl0fdk0ANF6h9w5IbzHRhuA6JIVDBHWzW8PXxCSa+2N1eAIDGX40i4r2EKt0ZJYbxtMWLzjYJrA4v"
     b"UhczXi+xu8gvYZhiRZKjszFFrDVNC/b7aq8m6s5p/vQf0kylJFmhpGTtoMBGXEGF+exCCVOJjEbSz0Xe"
@@ -361,14 +569,36 @@
 _check_md5(
     "lib1_parts_e05_scaler_models_mcdpr1_yaml",
     lib1_parts_e05_scaler_models_mcdpr1_yaml,
     1621,
     "bdf1242b955e22310d960c2e274e1001",
     "../../assets/test-data/downloaded/lib1-parts.e05_scaler.models.mcdpr1.yaml",
 )
+lib1_parts_e05_scaler_primitivedps_mcdpr1_yaml: str = decode_to_str(
+    b"eJy1ULsKwjAU3fsVdxA6ibpmVQoOSnFwLbGmeLG5CclNwU/wP/wyv8S0VqvoJDiFc5LzyBn58qC0FAkA"
+    b"I9dKwKrIAhWrUDPa+jQ35FkSF4s8Pjki7QXkDjUyNqrj9sqXDi2jIQEVTGA2hev5Ai7JWtfREPDUG6+4"
+    b"w33kOuidcj5SO8NstIB0mraNjBWwpAoJ+RRxiKePl2nShA/v3msr66AyZ/QjpWmJKJp1lrZl74I39We3"
+    b"L+1e+t3d+opPNBQ01ltZqt8XGL/8+32Hzf9mlUQiuQEeC52+",
+)
+
+
+def lib1_parts_e05_scaler_primitivedps_mcdpr1_yaml_fresh() -> str:
+    return get_updated_str(
+        lib1_parts_e05_scaler_primitivedps_mcdpr1_yaml,
+        "../../assets/test-data/downloaded/lib1-parts.e05_scaler.primitivedps.mcdpr1.yaml",
+    )
+
+
+_check_md5(
+    "lib1_parts_e05_scaler_primitivedps_mcdpr1_yaml",
+    lib1_parts_e05_scaler_primitivedps_mcdpr1_yaml,
+    529,
+    "bb1e2bc499d96d496104a99d8c422773",
+    "../../assets/test-data/downloaded/lib1-parts.e05_scaler.primitivedps.mcdpr1.yaml",
+)
 lib1_parts_e05_sumf_models_mcdpr1_yaml: str = decode_to_str(
     b"eJzFVbtqwzAU3fMVdwhkKIEko7bSUuiQENKho1AkmYpaD/QoZGy2/ke/LF9SyY84ie1SQom9yLpXOg9d"
     b"cTV29I1LgkYAXvicI3jQ0mgnPF8RydnjOmbehWII6nkWFPVCK5ILL7hLWzM8TwPAuIFLX7lxrR33VaQi"
     b"WQW55dYVwa32XksEk9mkmHttEDyrTCjhd0UkxD8XF0wKqsVtqCx3OlhaGrS34VSalXzYBdl9pBXDi5Am"
     b"56+WmDMtTc3iSbXrlD7suZWzetbC7/bV463LX7fHyzIelcyHV3JW6UJYjITcD6+MmZqypaBiWuINd/ie"
     b"sSVRO1xV/kSfFTJW/4OfZOIVo1aYdDUQZIf9J9ylYQ+Hr2+w1TJtnCGU//8RTFuW/3ZZNsNXA4AoVbM+"
     b"Xa+nCK+tZoE2WRe2rkGYdoH2wfYa7bbaZ7Ztd3gdVCvFiy4WD2cKmY0grea2Q+kBSi+YLpOpjaKyhx7n"
@@ -386,14 +616,36 @@
 _check_md5(
     "lib1_parts_e05_sumf_models_mcdpr1_yaml",
     lib1_parts_e05_sumf_models_mcdpr1_yaml,
     1943,
     "4873dc1a1e537bcfb68623fb97dcafa4",
     "../../assets/test-data/downloaded/lib1-parts.e05_sumf.models.mcdpr1.yaml",
 )
+lib1_parts_e05_sumf_primitivedps_mcdpr1_yaml: str = decode_to_str(
+    b"eJy9jjEKwkAQRfs9xRRCCglYbyeIYBEJuUBIshscdHfDzkZIaTrv4clyErNBNBoRsbD6zJ+Z/9+Mip1U"
+    b"GWcADt1BcojSRFK6FCLKdJOu4n6zRy04xBYVOjzKwROSCouVQ6M5lF17grmXFrrzBSwzFVVZIX3u7FFx"
+    b"jzIk3TDfSre1yqWl3sqNc0ZxCDe6RI2u8WSm4jCa616JQxCw5PeCYBF8jM605mz9bf5gxNaIuvA+1Tn5"
+    b"+/D5efr+BvAVcQo5xvxHxxVZs6OA",
+)
+
+
+def lib1_parts_e05_sumf_primitivedps_mcdpr1_yaml_fresh() -> str:
+    return get_updated_str(
+        lib1_parts_e05_sumf_primitivedps_mcdpr1_yaml,
+        "../../assets/test-data/downloaded/lib1-parts.e05_sumf.primitivedps.mcdpr1.yaml",
+    )
+
+
+_check_md5(
+    "lib1_parts_e05_sumf_primitivedps_mcdpr1_yaml",
+    lib1_parts_e05_sumf_primitivedps_mcdpr1_yaml,
+    543,
+    "f417dc92123952f346308679254fd955",
+    "../../assets/test-data/downloaded/lib1-parts.e05_sumf.primitivedps.mcdpr1.yaml",
+)
 lib1_parts_e06_addf_models_mcdpr1_yaml: str = decode_to_str(
     b"eJzdVkFOwzAQvPcVe0DqASE1PVpwQEWVOFAhkOAYpYkjLGKvZTuV+gT+wct4CXbi0KRxC0Utrcghstf2"
     b"zs6sd+Uznb5QnpABgGGmoAQmyCVqZugs4TS7ubcrr0xkBJp5XorUMBRJwQyj2h3N3Q/gbOXMffWxe9TU"
     b"eIuHmJV8TpWujHM0BjmB4WhYzQ1KArciZ4KZZWUp7UjbDcOBohpLldaY6m8wBWY1XiyLUkdBUA/xyLgs"
     b"6LNKZCeYlY5WqL527otRjppxz3uY1gZqIXphil2abtaRtwpLrcZ7DCvaMa5MNpi9EDzUXfxAdXydZRMU"
     b"2iTCxF7vVpCKcav5grZWbGZTxaRLCIEcziEaweUVKL9hevyUACzKrVF4vKekKOlUIe/Gs3DmNcWl29F2"
     b"EfC6id1Gfhuy60mu2dYpotQySen+1b7oqfszzR9O4NIDJEJUfSdFsbAu7SU9YPeJToBysP+Mj1+E3/ef"
@@ -412,14 +664,38 @@
 _check_md5(
     "lib1_parts_e06_addf_models_mcdpr1_yaml",
     lib1_parts_e06_addf_models_mcdpr1_yaml,
     2635,
     "1152ad2764168d59ece4e256afdc33ff",
     "../../assets/test-data/downloaded/lib1-parts.e06_addf.models.mcdpr1.yaml",
 )
+lib1_parts_e06_addf_primitivedps_mcdpr1_yaml: str = decode_to_str(
+    b"eJzVVMtqwzAQvPsr9hDIoRjsq2gPoSXQQ0NwoFcj2xsqYj2QZEM+of/RL+uXVFac+BG3GJoeejH2rHZm"
+    b"tDt4YfI35JQEAJbZEgnsUDM0GwccmCgIbDXjzLIan7ZBoQwJQlh0TZe2lzRBk66K4lEKY6mwqTvf1K9Z"
+    b"GrRAk2umLJOCwB7uII7g/gG0K65PvAORC400aFukFd5UPENtPJhJayUnsIyWJ29SEXgWeyaYPXqkcm/G"
+    b"HWjqdTWp1PK+0rLCtZa806wbyDXHLb1qKue2EcuU40nPPddn3tZ477tvWyqjaI6/n1I4mMzPs0pusJR4"
+    b"1laoEN9lbMUzhsK6hNWO3EVnfsA+3z9uFq5598gl5077321p/pJKmmHpfwghRP4ZB77ghzwwMbZwZWAo"
+    b"PxbvpJO/o/4Ct6JpDA==",
+)
+
+
+def lib1_parts_e06_addf_primitivedps_mcdpr1_yaml_fresh() -> str:
+    return get_updated_str(
+        lib1_parts_e06_addf_primitivedps_mcdpr1_yaml,
+        "../../assets/test-data/downloaded/lib1-parts.e06_addf.primitivedps.mcdpr1.yaml",
+    )
+
+
+_check_md5(
+    "lib1_parts_e06_addf_primitivedps_mcdpr1_yaml",
+    lib1_parts_e06_addf_primitivedps_mcdpr1_yaml,
+    1289,
+    "0d92bc8580680592c29ea0892d96ac2c",
+    "../../assets/test-data/downloaded/lib1-parts.e06_addf.primitivedps.mcdpr1.yaml",
+)
 lib1_parts_e06_addr_models_mcdpr1_yaml: str = decode_to_str(
     b"eJzdVktqwzAQ3ecUswhkUQLJVruQEuiiIbTQLo1jy1TU0ghJNuQIvUdP1pNUUpRE/qRtStOGemGksWfe"
     b"e6OZQUOdPVGekgGAYaakBObIJWpm6DLlNL9e2S/PTOQEdvuiEplhKNKSGUa1cy3cC2B4COaerdsKNTXB"
     b"EiCWFV9Tpb1xjcYgJzCajPzeoCRwIwommNl4S2VX2v4wGiiqsVLZFlP9DqbAfIuXMFHLstIop73IAeee"
     b"cVnSR5XKBqNDMm22ugl0T6IO6070fm1H9DU0ToPIfqFNsW7XSLLnhXJyBl4n0srlDrLDICDdJotKJLM8"
     b"n6PQJhUmCfmOOCrGbc5rGn2xx5spJt2BECjg7eUVFFzBdBL+WFzAmQDU1Yc0AuBDWlZ0oZA3CdXO3IKV"
     b"7o84RE/UY/KOCjwiMYhs2doSUWqZZvTn0z3uZPdrOb/7+6oHSIXw0ydDUduItkrPNX4uos270+cypuLn"
@@ -438,14 +714,38 @@
 _check_md5(
     "lib1_parts_e06_addr_models_mcdpr1_yaml",
     lib1_parts_e06_addr_models_mcdpr1_yaml,
     2645,
     "d610426b8f462b4f8dca16c3365bb9d4",
     "../../assets/test-data/downloaded/lib1-parts.e06_addr.models.mcdpr1.yaml",
 )
+lib1_parts_e06_addr_primitivedps_mcdpr1_yaml: str = decode_to_str(
+    b"eJzVlE1qwzAQhfc+xSwCWRRDvNUutBi6aAgpdGtke0KHWj9IsqFH6D16sp6ksuLGP3GLoemiG2O/kd73"
+    b"hhm8ssUzCs4iAEeuQgaPaAjtzgsvJEsGe0OCHDV4t49KbVkUw6q/dL62FTmhdLdKNmgsKRmKlxatWqIt"
+    b"DGnnTzE4wsfbOxhfSE+GI/ezhbLoOqUj7mqRe1QQc+WcEgzWm/UplNIM7uWRJLnXoNT+zfoDbb1QQnj0"
+    b"r2nxiPAz83CF5pJF3XEpvxvSQ5bWMtuWpR+TdVy6rJvI8jnBDSSbKw1rWT9NPYvqjJ94VWNqlOihTSsN"
+    b"7HVb+bo2cZmLPBt6JnYXfPA9jK201bzA/7dly5es4jlW4Y8QwyY8kygUwnKMQkwjXAQY46fwHn34O+tP"
+    b"V9hqoQ==",
+)
+
+
+def lib1_parts_e06_addr_primitivedps_mcdpr1_yaml_fresh() -> str:
+    return get_updated_str(
+        lib1_parts_e06_addr_primitivedps_mcdpr1_yaml,
+        "../../assets/test-data/downloaded/lib1-parts.e06_addr.primitivedps.mcdpr1.yaml",
+    )
+
+
+_check_md5(
+    "lib1_parts_e06_addr_primitivedps_mcdpr1_yaml",
+    lib1_parts_e06_addr_primitivedps_mcdpr1_yaml,
+    1288,
+    "227c7738aa42860df1aa2a8e748f7916",
+    "../../assets/test-data/downloaded/lib1-parts.e06_addr.primitivedps.mcdpr1.yaml",
+)
 lib1_parts_e06_sumr_models_mcdpr1_yaml: str = decode_to_str(
     b"eJzFVb1uwjAQ3nmKG5AYKiRg9Fa1QuoAQu3QMQqOo1pNbMs/SIxl63v0yXiSnoPTBOJIpaqIhyQ+++77"
     b"vjvnPDb0jZUpGQFYbgtG4EGWShpu2TotWfa4wZV3LjIC9Tx3glouRVpwy5nxrrl/AIybYH6c3DbSMBss"
     b"AWLtyi3TpjJupbWyJDCZTaq5lYrAk8i54HZfWRx+GdwwGWlmpNP0hKnntwFFpMVtkITMTtISLnaqcCau"
     b"MKC88FIV7FWn6oxPUzUsS7dSfiSYR1fYetoBiIvrERgTGRd6mVZMbLueFbPZ8KSQxXx4FpmqITsMAtIq"
     b"WTqR3GfZKhX7JFS8xU/zEqu+Y60VPF5Uc+WPBIEcjp9foI+HD7jzr0PYthxePIBURqWU/T+VaQf6d4RS"
     b"IWrs57+zqswbLTNHm1XjtqaJMI0F7QvbKzee+z6xXbnD86BSCFZ1L0zOFHKNQaqNvkuSpkX+2JK6m+Di"
@@ -463,14 +763,36 @@
 _check_md5(
     "lib1_parts_e06_sumr_models_mcdpr1_yaml",
     lib1_parts_e06_sumr_models_mcdpr1_yaml,
     1929,
     "5425908ff226be82e1a967dfe67eb7cb",
     "../../assets/test-data/downloaded/lib1-parts.e06_sumr.models.mcdpr1.yaml",
 )
+lib1_parts_e06_sumr_primitivedps_mcdpr1_yaml: str = decode_to_str(
+    b"eJy9kD0KwkAQhfucYgohhQSstxMkYBEJXiAk2Q0Ouj/sj5DSdN7Dk+Uk7gbRaBTEwmqYNzPve8zM1DvG"
+    b"SxIBWLQHRiArUieKJaVZKdpilfvJHgUlkGvkaPHIBo0yU2tUFqUg0EB/voDuuxPMQ+miNDjOHuZ3E2mY"
+    b"HfobbuN4xbTxUiWtlZxAvIhDGqkIrEWDAm3re+er8cM4ksqosma/A5KR7WdMKQSJtt9SBiHXkro66MZV"
+    b"Juwnz8fT8zcxXz8xDTmO+Q/GFaQxo4s=",
+)
+
+
+def lib1_parts_e06_sumr_primitivedps_mcdpr1_yaml_fresh() -> str:
+    return get_updated_str(
+        lib1_parts_e06_sumr_primitivedps_mcdpr1_yaml,
+        "../../assets/test-data/downloaded/lib1-parts.e06_sumr.primitivedps.mcdpr1.yaml",
+    )
+
+
+_check_md5(
+    "lib1_parts_e06_sumr_primitivedps_mcdpr1_yaml",
+    lib1_parts_e06_sumr_primitivedps_mcdpr1_yaml,
+    543,
+    "8916ed32afe8b6ea66fef3f65ecec1ea",
+    "../../assets/test-data/downloaded/lib1-parts.e06_sumr.primitivedps.mcdpr1.yaml",
+)
 lib1_parts_e07_ceil_models_mcdpr1_yaml: str = decode_to_str(
     b"eJzNVMFOwzAMvfcrfJhUOCBt11yHkDgwTUVox6pLXRHRxFGSIu0T+A++jC8hSVvarkWcgOVQJXbs92zn"
     b"dWX5M8qCJQBOuBoZbElqssLhrpBY3u6950WokkF/rhrFnSBV1MIJtCG0Ch+A1ZAsrDZsTxZdZ+kgdo08"
     b"orHReCTnSDJI12k8O9IM7lUllHCnaGn8zvoLaWLQUmN4i2l+E9M69KZ0k54xUFS26HnW1Jih3aKo893h"
     b"abPIpsN+FFLXeDCFnrAcGuw7OG9qWDnpdb+fZV+u95ual+pern1acThN+h5pmWH/l7SmY5kTLXVPYsap"
     b"w37I48S6ro+oGiF9519x5PGj5kboMBYG3IddVdfw8fYOprty9/+jASBtdcHxEqhkl/gmAAqlWMJJKYwS"
     b"8y/3Birjs8+Ud2JQhT8hta6gdjaX+pcvP4sNap3k/jFBrywWJTWCHhwm+QSbpICx",
@@ -487,14 +809,35 @@
 _check_md5(
     "lib1_parts_e07_ceil_models_mcdpr1_yaml",
     lib1_parts_e07_ceil_models_mcdpr1_yaml,
     1442,
     "33792070ecc13388d7f7bfcc0eac761c",
     "../../assets/test-data/downloaded/lib1-parts.e07_ceil.models.mcdpr1.yaml",
 )
+lib1_parts_e07_ceil_primitivedps_mcdpr1_yaml: str = decode_to_str(
+    b"eJy1jk0KwkAMRvdziiwKozvdzlYRXCilFyjtNMVg54eZVPAI3sOTeRLTIop7XYXvJbwvRbYndI1RAEw8"
+    b"oIFDvUEa6m0p6Ey+M1AmcsR0wZl1mG2iyBS8ASuni34Jj9sdktpNmuJjfAtCRp7zq+M4uhZTFtQG5uAM"
+    b"6JWeXgjRwN735ImvkkeZWZZahZhjY/F/BdWv1ZlRgF7rr5rGe6OecB9vZg==",
+)
+
+
+def lib1_parts_e07_ceil_primitivedps_mcdpr1_yaml_fresh() -> str:
+    return get_updated_str(
+        lib1_parts_e07_ceil_primitivedps_mcdpr1_yaml,
+        "../../assets/test-data/downloaded/lib1-parts.e07_ceil.primitivedps.mcdpr1.yaml",
+    )
+
+
+_check_md5(
+    "lib1_parts_e07_ceil_primitivedps_mcdpr1_yaml",
+    lib1_parts_e07_ceil_primitivedps_mcdpr1_yaml,
+    371,
+    "50ef8cce8a2fd099f65be31e75545cc2",
+    "../../assets/test-data/downloaded/lib1-parts.e07_ceil.primitivedps.mcdpr1.yaml",
+)
 lib1_parts_e07_floor_models_mcdpr1_yaml: str = decode_to_str(
     b"eJzNVMFugzAMvfMVPlRiO0xqr7luqrTDUNVq6hFRMFo0EkdJmNRP2H/sy/YlS0IYMJh2mtocELax3/Nz"
     b"zMqULygKlgBYbhtkcE9CkeEWs0Jg9bBzkVcuKwa9XbeytJxk0XDL0fjU2j8AVkMxf7q0HRm00RMhslac"
     b"UJvgPJG1JBik6zTYlhSDR1lzye05eIxF50o3Xbx1fuPMNNFoqNVlx0D/J4MBU1LV4eX7tsFtK7cNkc6z"
     b"4/NmkUCEO3ChGjzqQk2IDQo7Ceeq+pPr4X1WfbnFX9pcanW53bnoUxG8NRE/ECW1vgTRKa1K9ZAzBhHp"
     b"KQ8jc6PLo/IjcpoLp/4bjiJu3qXmyo+GQQ2f7x9Q+wI3+jZ+s73G+QCQMqoo8fIzAdhfA4lCSpaUJCWG"
     b"PXMX9w5q7WqFuF9strDV38G8v/EsXHX/vyQ2WQUGelJyvNFnd3dGKX+j/Uj26MkXagaEcA==",
@@ -511,14 +854,35 @@
 _check_md5(
     "lib1_parts_e07_floor_models_mcdpr1_yaml",
     lib1_parts_e07_floor_models_mcdpr1_yaml,
     1450,
     "97d1f3d49214444c3916f83a84c0ee42",
     "../../assets/test-data/downloaded/lib1-parts.e07_floor.models.mcdpr1.yaml",
 )
+lib1_parts_e07_floor_primitivedps_mcdpr1_yaml: str = decode_to_str(
+    b"eJy1jk0KwjAQhfc5xSwK0Z1us5aCC6X0AqU/UxxsMiGZCh7Be3gyT2JSxF5Al+8b3vemiP0FbWsUgJBM"
+    b"aODUlBNzKGfXHKqEr+QGA1UgS0I3XNiAsQ/khdgZGOH1eMKYS5uwVWV2Fav2a+CIsuTP0Hm2HYaYUMci"
+    b"bA3onc5/sDdwdCM5knvKUTABvc+3ObGYglbso297/PXYOlD/T906Z9QbIBRxmQ==",
+)
+
+
+def lib1_parts_e07_floor_primitivedps_mcdpr1_yaml_fresh() -> str:
+    return get_updated_str(
+        lib1_parts_e07_floor_primitivedps_mcdpr1_yaml,
+        "../../assets/test-data/downloaded/lib1-parts.e07_floor.primitivedps.mcdpr1.yaml",
+    )
+
+
+_check_md5(
+    "lib1_parts_e07_floor_primitivedps_mcdpr1_yaml",
+    lib1_parts_e07_floor_primitivedps_mcdpr1_yaml,
+    376,
+    "eacc9fd8a15d0752c1a435366bd6e54e",
+    "../../assets/test-data/downloaded/lib1-parts.e07_floor.primitivedps.mcdpr1.yaml",
+)
 lib1_parts_e10_conversions1_models_mcdpr1_yaml: str = decode_to_str(
     b"eJzFVMFqwzAMvecrdCgUBmXp1deOwi6lbIwdi+sozLS2jO0U+gn7j33ZvmS24zTLko0dxupDsCVLT3rK"
     b"88yJF1ScFQBe+iMyWJEy5KTHDVdY3W2D5yB1xaA7140WXpLmR+kluhhaxw/ArE8WVxu2JYc+WzLEplF7"
     b"tC4Z9+Q9KQbzcp7OngyDe11LLf05WZqwcwxUYdFRY0ULaf8B8qAKTVWLtxOkTyFDaHw5CZ2BHqUyR3y2"
     b"3AxK6skMbI0JjGtHpuz2o+zTzX3T4FST040O+I2HAcepKtvvr1DVoS2rMh3kqIKM9BTury4junhzdVaq"
     b"wPUJ8wRSSnTCShMHwaCGG1jD8nZZliW8v76BzffWV58IwMP1+Qcg4wwX+PelLEbQvyKl5sKTZXlm2ci1"
     b"ZkUQqsYksPDjLqC2AWWku3OYeXzzqHVFmbOBxi/m3ZewKNNB2p9iOzmxpKNPgL3DFh/QgH7i",
@@ -535,47 +899,93 @@
 _check_md5(
     "lib1_parts_e10_conversions1_models_mcdpr1_yaml",
     lib1_parts_e10_conversions1_models_mcdpr1_yaml,
     1410,
     "8ef6750a72b874683fd332aa802f5a26",
     "../../assets/test-data/downloaded/lib1-parts.e10_conversions1.models.mcdpr1.yaml",
 )
+lib1_parts_e10_conversions1_primitivedps_mcdpr1_yaml: str = decode_to_str(
+    b"eJy1kE0KwjAQhfc5xSyEgiCm29kqBTdSBA+QpikONT8k04JH8B6ezJOYSlE3bgRXw3sM33szi6RPxioU"
+    b"AEx8NghHR7zxbjQxkXfZ78m1CHUkS0yj2dbZa03SkQLnDYQOllBBuS6llHC/3iCKagIu3uwXxSfDTz2n"
+    b"7Qfb5KRsNZ7ZW4RCFlMZHxB2rqPc5pL1kGdCsOLwJ3JvhQ8pKG1+D1h9YL8e0CnNPuL8L6GcQ/EAiXt2"
+    b"+Q==",
+)
+
+
+def lib1_parts_e10_conversions1_primitivedps_mcdpr1_yaml_fresh() -> str:
+    return get_updated_str(
+        lib1_parts_e10_conversions1_primitivedps_mcdpr1_yaml,
+        "../../assets/test-data/downloaded/lib1-parts.e10_conversions1.primitivedps.mcdpr1.yaml",
+    )
+
+
+_check_md5(
+    "lib1_parts_e10_conversions1_primitivedps_mcdpr1_yaml",
+    lib1_parts_e10_conversions1_primitivedps_mcdpr1_yaml,
+    388,
+    "7b31d54893ce8b12e3e44280bb7f2139",
+    "../../assets/test-data/downloaded/lib1-parts.e10_conversions1.primitivedps.mcdpr1.yaml",
+)
 lib1_parts_e10_conversions2_models_mcdpr1_yaml: str = decode_to_str(
-    b"eJztWd1q2zAUvs9T6KJQ6MiSNIx1ZrsoHYHBUkrLtkuj2MoqZv0gyRm5XGEXY6+xJ8uTTLKtWI6lZk2T"
-    b"JoXpJrZknfOdo0+ffnIkk1tEYNQBQGGVoQhcMMKZxApdQoLS91e65RumaQTs+zSnicKMwgwrjKTpmmKp"
-    b"IE2QeQbgqLZpStn7ikmkqprK02VOJkjIonLClGIkAsf94+JdMR6BD3SKKVbzoibXTzICpCOQZLlISs+S"
-    b"I5Q+gdtpLjJGv8qeLDJFniLUWx2m7FCWlqHGmM5InqmB13Xl6AYTnqEvAvIGpHosAfCMnymxzqu2bl9b"
-    b"DvzxBWL0xemPtZnjk9teaaAxyAU8xmV/v+BqAlhAgz0CKtlhKlJuvbZAVM7G8Sin8VgPL+bZfAzpPK7I"
-    b"4OAUmGhCzJDTopmXCMwNW3QGwOLXHyAWdz8Wv3/qn7vqs9GBUAYAPSIcWhXaJp5uy78PFaTUerreHENR"
-    b"fSVYmid1q8wnsrbQ9RkNmQ0G5093KOHhibBnPHYexATTXM5glqNnp5Dd/sv+YHjWPzsdbkkr9yyVS2z/"
-    b"ok3XSMbnaXrBqNlFqI2k6QWoU2gBgLfvgNihSD1u1ACY5feCqtx/NoweCUaa8Aqim0HxYODmS9fUtqen"
-    b"x2cVeaDtEOU6gOoR0r3l5axaT+KE0Zk2q5m+K2Hbr16QgIoJJA9u1q7XsxskdGov10pYypfRedfP5XHM"
-    b"Dn47co8stoTxBIzA8M3wde/07NXgtG9KuY9bdoEE8rViYcV6DHk8jm8SmKH4E+dIuJ51fhudvJbCwnOP"
-    b"9IT2BuHdwQq7yjKFiWIiWk2I80VLk3YVR1ujHhxNwtIDzHdTw0xx9sUl2+I0h9lGlPvIvj8DyrVTYIlX"
-    b"c65nOPifeDua6E3KuS+jtbx7mmNLjfb6QBA1WXvfmnROJhhR9dilqbkMHcrArE7ehBHC6O7A+ebjAyHu"
-    b"kkHe7dKDETpTMIMTlDlbny7oO8+DTqvDPu+X7CzdxaFg842oPhBQVGzkdR67YCrsKmjuiqP6onhZF9vN"
-    b"dVTeo3aMo7JL3VJcpW9ibuA1Zy7Jfdaca5qAQRdeEIJ7lJlH9m6m4XDlE/snRdu6c8AKOzC4POF4+zrh"
-    b"6Me2Q28OAhH9BZwYioE=",
+    b"eJzVWMuK2zAU3ecrtBgYmJLGTihNTbsYUgJdJIQMbZfGsZVG1JKMHoEsO9BF6W/0y/Illfx2LM80r7Hr"
+    b"jfWw7j33oXNl3XB/A7Hn9AAQSITQAROKI8qRgHMPw+DjQs18RyRwQNZfS+ILRIkXIoEg10sDxIVHfKjb"
+    b"ANwUMvWTrF5QDkU6kmqaS7yCjMeDKyoExQ64tW7jvqCRAz6RNSJI7OIRqVrcAbjHIKeS+YlmHkEYvIDa"
+    b"tWQhJd/4gMeewi9h6kaZyXuEBompLiJbLENhG1Wnih4QjkL4lXlRBVIRSwAM8dOPq/yqpGfdmgKzfQ02"
+    b"muw021r18d1mkAioBDmGRyNutQuuSIAMkN0ioCQ79EAQZVprIFJlM3cqiTtT4UVRuJt5ZOemyVDCyRBW"
+    b"CbGFpRmVeT5Dkc4W5QGw//UHsP3jj/3vn+r1mH427UjKAKAiEnkZC10ST7+m34TKIyTTtDwdQzy8YDSQ"
+    b"fjHL5YoXEvomoU1iG40zu7vJ4c0boWU82T5wMSKSb71Qwv+OIfvWa8seja3xcHQhrmyZKnNs/8JNS8jd"
+    b"+yCYUKJPEeIkanoFChdmAMD7D4BdkaTOixoAW/kkqFT9F53RU0ZxFV6c6DooBgyR/rIs6tLb06Aztbxh"
+    b"rot03YDqDOq+cDlL64nrU7JVYlWmX4vY2uUL3MBiDPLO7drn+ewBMuXa+bMUFkS5dcb6mYr7rDBM8gSo"
+    b"W2+gxho53oEpGL0bvR0Mx2/soaWf5CyXL5leky2OKOY4H1p2BFF1SxpI69Lo6uR1hNfWni8ocw6jnc+X"
+    b"jqhPJd09XiFIzs67bubYYUR9ijElnQroIcRrbgYjHx6NsJRYobeCYYnb+sAqte1ebUGbP5DZ1rlG1T+9"
+    b"0qiKT2BcqZUf+2CtTn8JHH0Z5BQ3QfmYm1VPJ7ko6WlFTqWuOsld2SnibKM4fQtmklb6D2sQWIbXCKF8"
+    b"Vtk52c9XReHBJ9ktZF166QTVrEDjMphjXFsyRzXrCo0+aLDoL8QCmtY=",
 )
 
 
 def lib1_parts_e10_conversions2_models_mcdpr1_yaml_fresh() -> str:
     return get_updated_str(
         lib1_parts_e10_conversions2_models_mcdpr1_yaml,
         "../../assets/test-data/downloaded/lib1-parts.e10_conversions2.models.mcdpr1.yaml",
     )
 
 
 _check_md5(
     "lib1_parts_e10_conversions2_models_mcdpr1_yaml",
     lib1_parts_e10_conversions2_models_mcdpr1_yaml,
-    6550,
-    "c82585c7a83af500a45a04c8042d5736",
+    5495,
+    "e5812d2c48dfba7dd5b29df7b522ee02",
     "../../assets/test-data/downloaded/lib1-parts.e10_conversions2.models.mcdpr1.yaml",
 )
+lib1_parts_e10_conversions2_primitivedps_mcdpr1_yaml: str = decode_to_str(
+    b"eJzFVstKw0AU3fcr7kIQlNi0QayDLkQpuKiUim5LHlM7mJkJ8yh0qeBC/A2/rF/iZJI2Jq2laoxZTJo7"
+    b"c+ece8/JNHsynGLqoxaAIirGCG6xIFjemMAjYRGCoSCUKDLDV8NWlEjUcmCvSFql3TGiLjmbYSEJZ3Zm"
+    b"PT+NRliGgiTKrEIwgQPog3fqnbS7veNO100vWLy+gzCL+xlCCW61LZdY5ZGcwo2mgYG3wYArxSmCfXc/"
+    b"Y8kTBNdsQgzNuY1o80sioOZh1ADORIuDaTtN4olM/BD/HtMp4WytcOKHigtU7bSZ8Rn7StILGhDMfqRq"
+    b"kwoWnQ05pQa/qcYWwHUYyHGP3I7Xc3tdb+eCt4g3GI+wHF9EkZFPKp+pca7UTvodQsFmiQdn57Vp+pNi"
+    b"Z3ojcA5z78ca9wWnBYVZGkoNVMFK0hXL9MpumwrZWMpng1b2z6vZEP/3s6Bey+7+Zm41al+z8UDHiiTx"
+    b"fOCz+becak+axfPT4u3F3J4bP3MaUtA28Nuq2dBQ8EiH2YzUgcyynFqcXzJ8qYDPrYo5e5Bt2SzulGuT"
+    b"GPsBju1HiwOuHTt27NrRa9m+WseUaFUprdEpU6nSWP3zjnbduaLUUqe1btVu40KbP8bK9PgAyZLzHg==",
+)
+
+
+def lib1_parts_e10_conversions2_primitivedps_mcdpr1_yaml_fresh() -> str:
+    return get_updated_str(
+        lib1_parts_e10_conversions2_primitivedps_mcdpr1_yaml,
+        "../../assets/test-data/downloaded/lib1-parts.e10_conversions2.primitivedps.mcdpr1.yaml",
+    )
+
+
+_check_md5(
+    "lib1_parts_e10_conversions2_primitivedps_mcdpr1_yaml",
+    lib1_parts_e10_conversions2_primitivedps_mcdpr1_yaml,
+    2660,
+    "3ac1d5bc206138e8473bfa71a71ad9d6",
+    "../../assets/test-data/downloaded/lib1-parts.e10_conversions2.primitivedps.mcdpr1.yaml",
+)
 lib1_parts_e11_constant_fun_models_mcdpr1_yaml: str = decode_to_str(
     b"eJzFVd1KwzAYve9TfBeDXQ2229zJZCCIDAW9EBn9STHY/JCkgyE+gO/hk/kkJlnamqWdOjfWi5KcNN85"
     b"p8lJRip/xjRFCYAmusII5pwKrojGNynFxeXSjLwQViBo+mXNck04SyuiCVZ2amlfAKOumH2205ZcYe0R"
     b"T3FT0wxL5cCMa80pgvF07PqaCwRXrCSM6I1DatNSCGgiseK1zA0lvL4ljBdb8lVF6KxXgKe7I1RU+EGm"
     b"IhDW+TMGYk/2WVVNK6rdb3DAZGB05p22bgOkdWs7oWOLFKIREOnxvNeEkk6OlygtSNbY23WVsMolEdY1"
     b"ghI+3z9gNvW8AIvzGgfI9wrwVPdpVeOF5DSUsrbwTnlhv/heoqfqkLFBawPm+uxFBlPGGu7bw3+2g5eS"
     b"F3Xejao6M0SPTzYcOWdrI9ms8qkywsX0BJtld68ER0L0O7ugNKpk1z7PFv45qRc0I5jpebtCh6VWnjCy"
@@ -594,14 +1004,36 @@
 _check_md5(
     "lib1_parts_e11_constant_fun_models_mcdpr1_yaml",
     lib1_parts_e11_constant_fun_models_mcdpr1_yaml,
     2092,
     "563104572fd6b5530dd4813ca08b645a",
     "../../assets/test-data/downloaded/lib1-parts.e11_constant_fun.models.mcdpr1.yaml",
 )
+lib1_parts_e11_constant_fun_primitivedps_mcdpr1_yaml: str = decode_to_str(
+    b"eJyNj70KwjAUhfc8xR2Eru16ZykIIsXBRRzaNMWLTVLyU/ARfA+fzCcxaWtV6uAUzgfnuycry89ClsgA"
+    b"HLlWIGxJkgvxQqpGKEyM1It1EVgtLDfUOdIKoYHH7Q5ZCpLlsb96q+a2tsINeZLvvKyEsQFV2jktEZI0"
+    b"ibd1h7BRDSly15B9eC0GM1+YJ9OhbL3IjZavG30EwZcNwi7SsfDVXi77se1j3WibBs5pnlcqhWz/7+8H"
+    b"UBhdex659VWQHE/sCbpOcao=",
+)
+
+
+def lib1_parts_e11_constant_fun_primitivedps_mcdpr1_yaml_fresh() -> str:
+    return get_updated_str(
+        lib1_parts_e11_constant_fun_primitivedps_mcdpr1_yaml,
+        "../../assets/test-data/downloaded/lib1-parts.e11_constant_fun.primitivedps.mcdpr1.yaml",
+    )
+
+
+_check_md5(
+    "lib1_parts_e11_constant_fun_primitivedps_mcdpr1_yaml",
+    lib1_parts_e11_constant_fun_primitivedps_mcdpr1_yaml,
+    387,
+    "d2be1e96e81cd4343d58dcfbdb5d33ee",
+    "../../assets/test-data/downloaded/lib1-parts.e11_constant_fun.primitivedps.mcdpr1.yaml",
+)
 lib1_parts_e11_constant_res_models_mcdpr1_yaml: str = decode_to_str(
     b"eJzFVctKAzEU3c9X3IXQVaHdZieVgptSFHQhUuaRweDkQZIpFPED/A+/zC8xSTOPtBm1OtJZlNybzD3n"
     b"3NwzvVD5E6YpSgA00RVGsOBUcEU0XqUUF1drs/NMWIGgicua5ZpwllZEE6wQvLwmEitey9xE5ri0PwAX"
     b"XWn77IusucLaZzzgqqYZlsolM641pwgms4mLNRcIrllJGNE7l6nNymDShPFiD7fJo3i++i2hosL3MhUB"
     b"j04cQEyQzQei7NMgRdDiCgdUBkrnXmorN8i0cm1QiAbuCL29PKZ0yjp8z0kSarRtsVfsimGVSyKscATz"
     b"GVD4eHsH6fe/VurR7tKqxkvJaah5a9MHOoQ90S8RqTrUwcEeDnQx1seDTgLcnPcqAVLGGsTl77m49Fry"
     b"os67XVVnBujh0ZmDs60ha255PrJNGlNwMTtvL499Krv1iJQOGQXfpSNW35v1kmYEM71ob+hU15aBZf8w"
@@ -620,14 +1052,168 @@
 _check_md5(
     "lib1_parts_e11_constant_res_models_mcdpr1_yaml",
     lib1_parts_e11_constant_res_models_mcdpr1_yaml,
     2079,
     "1befc235bc8bd89ea9f9221a291625be",
     "../../assets/test-data/downloaded/lib1-parts.e11_constant_res.models.mcdpr1.yaml",
 )
+lib1_parts_e11_constant_res_primitivedps_mcdpr1_yaml: str = decode_to_str(
+    b"eJyNzr0OwiAQwPGdp7ihSdd2ZdU0cTHEwcU49APjxQINHE18BN/DJ/NJhGqw2sXx/uF+R+bas1Q1ZwCE"
+    b"1EsOK6Md1ZpCuaDuOAiLCglHuRahddK1FgdCozmUBSh43O5gWRuJ7KMlb1/3XlbWKGGcjOoYA4e8LPIw"
+    b"DbG+Fr620/X31kzcetVI66bYGCKjkhbemGE2eY3kOCi2W3zvl1/giZ6syd3oEwbxymZyrTVn1b/8FIQ1"
+    b"nW9jd74JyOHInqDYcwE=",
+)
+
+
+def lib1_parts_e11_constant_res_primitivedps_mcdpr1_yaml_fresh() -> str:
+    return get_updated_str(
+        lib1_parts_e11_constant_res_primitivedps_mcdpr1_yaml,
+        "../../assets/test-data/downloaded/lib1-parts.e11_constant_res.primitivedps.mcdpr1.yaml",
+    )
+
+
+_check_md5(
+    "lib1_parts_e11_constant_res_primitivedps_mcdpr1_yaml",
+    lib1_parts_e11_constant_res_primitivedps_mcdpr1_yaml,
+    390,
+    "98006c8f6ba701ec3d3eec9134d42763",
+    "../../assets/test-data/downloaded/lib1-parts.e11_constant_res.primitivedps.mcdpr1.yaml",
+)
+lib1_parts_e12_catalogue_models_mcdpr1_yaml: str = decode_to_str(
+    b"eJzVlE9rgzAYxu9+ivdQ8FSYtqdcVwbbocjK8ChR4xbqm0j+jO3bLyaW2VXBXoR5Me+j7+/Jk4RsdPXB"
+    b"kJIIwHDTMgInjl3LckU7p525qAkcKbL6kEWNFZXhUtCWG85039QUSf8C2PyC+ic0ZlIzMygD/mixZEp7"
+    b"sZTGSCQQP8S+NrIj8CwaLrj59op1I03gxTulKzhhpJiWVlUhnlol3tvp4L3WCJhHddeTr0wG4CM1tJXv"
+    b"lrm9Hjkrjm6/P4P6dN8cvZQpWdsqfNG21KFr+xcyhZkMext3KvDV6VnRDl35+v9WKRzCFQ1zVzJh1HCT"
+    b"AKCsWZtcbJsC6del2I6Q47EqkIvRT0l8M/bUdAk1maPuZ6i7OWp671x3I+p+CTVduAI/Vol7hQ==",
+)
+
+
+def lib1_parts_e12_catalogue_models_mcdpr1_yaml_fresh() -> str:
+    return get_updated_str(
+        lib1_parts_e12_catalogue_models_mcdpr1_yaml,
+        "../../assets/test-data/downloaded/lib1-parts.e12_catalogue.models.mcdpr1.yaml",
+    )
+
+
+_check_md5(
+    "lib1_parts_e12_catalogue_models_mcdpr1_yaml",
+    lib1_parts_e12_catalogue_models_mcdpr1_yaml,
+    1504,
+    "86887ab52aa23e7993afd0a92c653739",
+    "../../assets/test-data/downloaded/lib1-parts.e12_catalogue.models.mcdpr1.yaml",
+)
+lib1_parts_e12_catalogue_primitivedps_mcdpr1_yaml: str = decode_to_str(
+    b"eJzNkDELwjAQhff+igxCJ8G2Tlktgg5SFHGU1EY9bBJJLqL/XpNKiliqi+D28vLue7kMzO7IBaMRIQhY"
+    b"c0omDFmtDpbnxcM8gawoKTQIQLg4b+qyg3YsZJTh6M9PkDcKrSq7c76xpXH54evw+3gALKwouTbeLBWi"
+    b"EpTEo7jpUGdKZnIPEvDmHftQhpL57ytEtPzvP1iv8t+XbCIuUQP3CwlV8TppivZbwa6NHAZMq/RWgAzX"
+    b"SfyiPCft5yRdnHEHJ+vipN++JwuccT8n/bjXHblb3Uw=",
+)
+
+
+def lib1_parts_e12_catalogue_primitivedps_mcdpr1_yaml_fresh() -> str:
+    return get_updated_str(
+        lib1_parts_e12_catalogue_primitivedps_mcdpr1_yaml,
+        "../../assets/test-data/downloaded/lib1-parts.e12_catalogue.primitivedps.mcdpr1.yaml",
+    )
+
+
+_check_md5(
+    "lib1_parts_e12_catalogue_primitivedps_mcdpr1_yaml",
+    lib1_parts_e12_catalogue_primitivedps_mcdpr1_yaml,
+    869,
+    "953a808cfeea94e797dde3567f8161a3",
+    "../../assets/test-data/downloaded/lib1-parts.e12_catalogue.primitivedps.mcdpr1.yaml",
+)
+lib1_parts_e12_catalogue_empty_models_mcdpr1_yaml: str = decode_to_str(
+    b"eJzVVD1LBDEQ7fMrpji4SlDLtB6CFsdyh2wp2d1ZHdwkSzI5OMT/bj4W9HQbm4Bpknlh3puXGbLx/Stq"
+    b"JQUAE08o4Uh6nrB1ao7YG5lBwl5pHHaNGIPpmaxREzGhT0nj803aADZfRGmVxMZ65AVZ6PdBd+h8BjvL"
+    b"bLWE7fU2x2xnCQ9mJEN8zkiIJy/hMSvdVlDSwqG3wfXFnqti7+m4y1o1DLZimBPzhchCeKdYTfYlYOz1"
+    b"N2VHOvb7VND7v9WYocbZIfTlxofOl6yrnyRrNKtmf9tdM3wxPRXldAwP/++VyhBWFGxjiIZd+kng/UN8"
+    b"ArpjPns=",
+)
+
+
+def lib1_parts_e12_catalogue_empty_models_mcdpr1_yaml_fresh() -> str:
+    return get_updated_str(
+        lib1_parts_e12_catalogue_empty_models_mcdpr1_yaml,
+        "../../assets/test-data/downloaded/lib1-parts.e12_catalogue_empty.models.mcdpr1.yaml",
+    )
+
+
+_check_md5(
+    "lib1_parts_e12_catalogue_empty_models_mcdpr1_yaml",
+    lib1_parts_e12_catalogue_empty_models_mcdpr1_yaml,
+    1163,
+    "fedd3bae33683c29f43549e43a67ecda",
+    "../../assets/test-data/downloaded/lib1-parts.e12_catalogue_empty.models.mcdpr1.yaml",
+)
+lib1_parts_e12_catalogue_empty_primitivedps_mcdpr1_yaml: str = decode_to_str(
+    b"eJzNkD0LwjAQhvf8ihsKnQTnrBZBBwmKOKftqYdNUpKLIOJ/t4lSEeeC23sP7wdcEZozGi0FABN3KGGh"
+    b"WXfuFLFSA7yQbSUoT4aYroktk7f4xEaPC8j5fhdloLxrY5N4iHVI/tl3+Dc+FmyiqdGHDGvH7IyEcl6+"
+    b"NlwvYWWPZIlvmcRBBQnr6SeM2P73D/a7avqRg0DLnnCQ94d4Arhup0I=",
+)
+
+
+def lib1_parts_e12_catalogue_empty_primitivedps_mcdpr1_yaml_fresh() -> str:
+    return get_updated_str(
+        lib1_parts_e12_catalogue_empty_primitivedps_mcdpr1_yaml,
+        "../../assets/test-data/downloaded/lib1-parts.e12_catalogue_empty.primitivedps.mcdpr1.yaml",
+    )
+
+
+_check_md5(
+    "lib1_parts_e12_catalogue_empty_primitivedps_mcdpr1_yaml",
+    lib1_parts_e12_catalogue_empty_primitivedps_mcdpr1_yaml,
+    584,
+    "633bf530fecabe6bea26773d49ce61ef",
+    "../../assets/test-data/downloaded/lib1-parts.e12_catalogue_empty.primitivedps.mcdpr1.yaml",
+)
+lib1_parts_e12_catalogue_true_models_mcdpr1_yaml: str = decode_to_str(
+    b"eJy9kbsOwjAMRfd+hQekrrBmBSGxVBUMjFXaumARJ1XiIPh70gfi8QHNYCVXvvdE9io0V2StMgAhMajg"
+    b"RNwbPHvdJ+1GtlVQaMZ2V2ZdtI2Qs9qQEIbB1A0FYPWJGc5kK11AmZU5vIhcow+jWDsRxwrydT6+xfUK"
+    b"DrYjS/IclZhuITXkmcfgom8mpl+G2fZD9A9lTtxq0cZdIqaZfKE9cZrLfVL3y3wS4LgUCK34eesA7Fo0"
+    b"mzetq1g//qxpTxWTndJfynWsOg==",
+)
+
+
+def lib1_parts_e12_catalogue_true_models_mcdpr1_yaml_fresh() -> str:
+    return get_updated_str(
+        lib1_parts_e12_catalogue_true_models_mcdpr1_yaml,
+        "../../assets/test-data/downloaded/lib1-parts.e12_catalogue_true.models.mcdpr1.yaml",
+    )
+
+
+_check_md5(
+    "lib1_parts_e12_catalogue_true_models_mcdpr1_yaml",
+    lib1_parts_e12_catalogue_true_models_mcdpr1_yaml,
+    615,
+    "f03468b23c7fceecfacbdc04da73bda4",
+    "../../assets/test-data/downloaded/lib1-parts.e12_catalogue_true.models.mcdpr1.yaml",
+)
+lib1_parts_e12_catalogue_true_primitivedps_mcdpr1_yaml: str = decode_to_str(
+    b"eJy1jbEOwjAMRPd+hYdKWWHNCkJiQRU/UKXUBYs4RolTwd+TUATiA5isO9+9a9PpguxsA6CkHi1snDov"
+    b"54zbrphXCqOFLhKT0ly9Xc2239onIwn1pd+gQ+YBYyrWIKrCFszK1B25WdiHiQLpo+hcbipP0xz/h8ag"
+    b"kTBVKsuIfr3wp57d/acCEHumsBCfLG1Ujg==",
+)
+
+
+def lib1_parts_e12_catalogue_true_primitivedps_mcdpr1_yaml_fresh() -> str:
+    return get_updated_str(
+        lib1_parts_e12_catalogue_true_primitivedps_mcdpr1_yaml,
+        "../../assets/test-data/downloaded/lib1-parts.e12_catalogue_true.primitivedps.mcdpr1.yaml",
+    )
+
+
+_check_md5(
+    "lib1_parts_e12_catalogue_true_primitivedps_mcdpr1_yaml",
+    lib1_parts_e12_catalogue_true_primitivedps_mcdpr1_yaml,
+    286,
+    "b058b8e3886d66fd7999e84a6d0e9bb7",
+    "../../assets/test-data/downloaded/lib1-parts.e12_catalogue_true.primitivedps.mcdpr1.yaml",
+)
 lib1_parts_nats_posets_mcdpr1_yaml: str = decode_to_str(
     b"eJwNx7ENgEAIAMCeKShMaLVlAxvjCr5iJPqPESzcXrq7ztdD6sKAeGrbGGdziVxoXMI4vbXI41Aswioj"
     b"9QRhN+PYdm0aH3hIlgaCN+9Jgh+sjBrN",
 )
 
 
 def lib1_parts_nats_posets_mcdpr1_yaml_fresh() -> str:
@@ -680,32 +1266,212 @@
 _check_md5(
     "lib1_parts_reals_with_units_posets_mcdpr1_yaml",
     lib1_parts_reals_with_units_posets_mcdpr1_yaml,
     77,
     "76c89aa9190ae359a5e49e3e5a9778b9",
     "../../assets/test-data/downloaded/lib1-parts.reals_with_units.posets.mcdpr1.yaml",
 )
+lib1_simple_all_together_models_mcdpr1_yaml: str = decode_to_str(
+    b"eJztWd1umzAUvu9T+KJSWk3dIL2puKsyRdpFoyrT1ktEwKjW8I9sEykPsItpr7En65Ps2CENBJM0WQhk"
+    b"W24CNj7f+fH36RguVfyMaRRcIKSJznCARpwKrojGk4ji5OMjzHwjLAnQ6j7NWawJZ1FGNMHKLE1D3/wh"
+    b"dLk2Z37LhY9cYV2MFCCTnM6wVHZwxrXmNEADb2DvNRcB+sRSwohe2JEcrhQ8MLiQWPFcxktUeSpUxpMl"
+    b"YjjNMzzFaoRJFk6evrjxC7TPhIoMP8lIVPxapxXyVk+l+YVceKvrmnV3hA1RuiJ1R1uN2NxVcm3dkuvr"
+    b"U7qlNIbhgT9ocDQRKydqPhXYD6GtWJH1kquSUMj8HJdmoNSxJMKUJUAxLLtKr9HLj19IFo+Muy8NQlwo"
+    b"EcW4D65M+7gnEIoYs5SleaZb5Knfx+id1B12v1newlSQ1/ABakZEthhxpnTE9AHMTdHLz+/ornvm7t6p"
+    b"83yrX4UHX6Msx2PJadXDuRkGY3dr+8I8ULbgMNoUbmPApZBLUEXQ1aGTadVNLdmuEnSiT01qZBqIcc7G"
+    b"GeeyzQ4C+H7bx91eVybQ0DNRJls0KN5hagQ6lBoDV/K633L0r7cWTdQlbG56CSu4LdIWILqP2kVT1cmZ"
+    b"5BjNv+HsUVqKD8h/P+y+pWilgYDITtdCVMBWTcTG4P82Yp9jDqiTyHLFxZl1FP4RlOlsGgjQofsk+bNT"
+    b"jREf9A75XosKtG9RjiVB3gkVyHMIkNdj/el5dxRzNgeLsEtbfNnSA547X630QRh3C9A9nRHM9Oi1Ugeq"
+    b"T59an5hTytnfzcn91diSEhjJsGUS7NUblILsBjWCLQLz8ebCGF5Omm8dQf1Dx+tcuLHa0LJifaeBFYMC"
+    b"S506tH1huxXPbwKsvFlxIhoRKUGuZ2TotFo59DVYVJ47fw3ebAZk9KMBuujo3hLJdn8dmPCUC3Uj+9Vi"
+    b"OQBLur+1ZkMXmHNxFfLWGWMtMc6k/gavyHrO",
+)
+
+
+def lib1_simple_all_together_models_mcdpr1_yaml_fresh() -> str:
+    return get_updated_str(
+        lib1_simple_all_together_models_mcdpr1_yaml,
+        "../../assets/test-data/downloaded/lib1-simple.all_together.models.mcdpr1.yaml",
+    )
+
+
+_check_md5(
+    "lib1_simple_all_together_models_mcdpr1_yaml",
+    lib1_simple_all_together_models_mcdpr1_yaml,
+    7375,
+    "26de67a46b7162f02e2007e477f744da",
+    "../../assets/test-data/downloaded/lib1-simple.all_together.models.mcdpr1.yaml",
+)
+lib1_simple_all_together_primitivedps_mcdpr1_yaml: str = decode_to_str(
+    b"eJzdV91qwjAUvvcpciFUGTrrNpDeiaOwC0Uc7Lb0J2VhbVKStOAD7GLsNfZkPsmS2Nq1VbDVduDNwX7J"
+    b"+c45PV9Oap+57zC0jR4AHPEAGuAVUgTZSgAfCHsGWFMUIo4S+LzueREzeiPQz50ObktrAVFgiU0SrLpK"
+    b"1IPMpSjiiGADuGL7wB+C3dcPoGLZ3NMVuA9EhEGeImm8VRw6kDIFOoRzEhpAm2j7lEhkgBfsI4z4ViGx"
+    b"+MXEBrlOIhbZLuwq3KbNQIxDAWm6VglrY3y6VRvIrGUccBQF2wXBjNuY12idD3bfn2DWTetOl5jER+Om"
+    b"Ud7sIIYmJWGeQSIh4Tzbc0VyIfMqkRxL/2gBf0pIadMi8sdWxDcqvKTya2tVdGfKbB46CGIu9JUIbiGc"
+    b"GvLqeia4JAxF6Ja7cv3BoF/apKVlxtiae16zMSD7BO6APrlSs86rp/HBz+ivffIz3uzo58//cPY7vH5q"
+    b"ieyiC+ce6ONp93OhudLG05aklhEftJYDt3bRNPy6MQNCqFRc3VHmS8cBHbatsNN13dK3aaVfge3AQP2B"
+    b"GIGJsrqyU2UflH1U9qmnHFQTCsmVU6skVkyrnFSe0qY96l+p/bJm",
+)
+
+
+def lib1_simple_all_together_primitivedps_mcdpr1_yaml_fresh() -> str:
+    return get_updated_str(
+        lib1_simple_all_together_primitivedps_mcdpr1_yaml,
+        "../../assets/test-data/downloaded/lib1-simple.all_together.primitivedps.mcdpr1.yaml",
+    )
+
+
+_check_md5(
+    "lib1_simple_all_together_primitivedps_mcdpr1_yaml",
+    lib1_simple_all_together_primitivedps_mcdpr1_yaml,
+    3397,
+    "fe37e37237f85efe4616ed1b0e41a2f3",
+    "../../assets/test-data/downloaded/lib1-simple.all_together.primitivedps.mcdpr1.yaml",
+)
+lib1_simple_drone1_models_mcdpr1_yaml: str = decode_to_str(
+    b"eJztW81u3DYQvu9T8BAgQApnf4oWqW6FDQMx4IXhoN2jQEvcteqVKEjUpnuMgQAt8ho99JxHyKP4SULq"
+    b"lxRJ7Ub7Qy7svdgiRc7HIeebGZJ6lXr3KITOAAASkCVywDkOY5wGBE1hiPyLG1rzEES+A6rneRZ5JMAR"
+    b"XAYkQClriiI/S2DkIfYAwKumU/Yrmt/gFJGypBQ1zcI7lKR54R0mBIcOeD16nT8THDvgfTQPooCs85KM"
+    b"/pc6gL2O/iYJdGO4XmLoH0Hmw6IRij+i5AgiZ4MEpThLvELDIUzT4ww0wn4h8g4SgpK1Uqp+rTSY+DLF"
+    b"mmE/D8bQoxCqZ0mOeoSaUapGqh4tN+KrvEDQNfs1+jaCKl9wANRzwX5umC3JuBNUKf5DEMZLNEtgLAEW"
+    b"J0o7Mbk8HI/4Z6VEvSo61KFTiV4tnGqu6kJp0nLUifhsC+o3D4vh7L6u8mMejxJiCePavUWpexGsAh+d"
+    b"4yglMCIuN4PcWJIgpLO4Qq1auoa8JIjZNDtgDobgl9EIzO6HDwvw9O9/IOFevrRRdVzhKtsKYAnjT7jM"
+    b"0GWCQxnqilVRMFQVIpyYvdruTyOmSxOduuC0IQEoNaKqqFwDmzquCscppVFk+dTd2oivZZUAwCiq+dbD"
+    b"0YqKomZzZNYdn4CqtOQ7sRA8Zy7bE+8ftO15vQT68+0bcAnGw59/paR7EnQr2YSNlmuGAM+UkHqodA49"
+    b"ghOnXBcq/qHkE6GcJEoLOwNz6sma4fAcsnbqULoK0HHzJosinTJ8FArdVh+Me5Sy9D1UNODktq8XznHp"
+    b"RgjjLgzajkQkEwWU5g0W3dNiOgkZzM00f+cwOc4ymJNO93HYTGI64Ideo+LSWCOwZoNq4pr8Jk6wf0xP"
+    b"WxihjTnOdLObpaZoI/BvX3t42mv3hi3HXbKab19PwrlOuUIb3So/f9Q8M9rHhCvwEdX1mCvgw+WX7Ym2"
+    b"Bk9pg2LWy27Z1sQ1nfcgXq73sjnx9OUzGL0djSZgNpyeilELRrP3LYpcHWY3KRQQqm0KZVW1poaiaiyN"
+    b"020k4hlX2DsnYKGnIg4uI+k83BJj6HYwXkZISln6XsRInLKDHoOZnKR5IQ+DabmbZuG4KwuQfNbW8b9L"
+    b"UBKOOv3iMULtEki3gz4GEMkpStGsIWCN35MACP7ud9+/htGad3N6Fye6t6fHT+An9udRcGwSL+5LAzIP"
+    b"brVSbo3PhRBZXvaHkxffUIrKvKY2ze64COxMTfg6uteSvZrqdUQv0bxxGPqD7Z0p0I7NBkv3QDbTznua"
+    b"dtF/1z0IR6CZHexob2ZtEbXw+017d/pCcmrO5ePYpMNP9Q7fIKqrH/L2VXa7g8unOa3k8k3aQXUqazjs"
+    b"ePHwR4SR35qLULLovM/Vn/D4vhX96wd64HtcluB6Hk6+IhYbyK1y8jSxnxwysTfpX+tD8CK1twCKLrmf"
+    b"mIf2kt7Xy8WkfdYgnof75+6pmMfBH9EdIuOxlYBMss/0h8in6yxt+3Dgy2fw29t3YxAO09YRmsnooDYF"
+    b"/oRMf0qsORmrTsXYABvB0oHYnk1NlFadfbVLy4HmareD+00yfXXXoST6jyhY3JPDkA/ft8GxSuRjCa7n"
+    b"kX1U682iNe/+hYPInUd0BR/K7ULzjC77XHa/0jW5AdpkRjkUCwKTLSIAhMj0IoPLvkYIEpaAPP3zP/vn"
+    b"0QKLrGfh3AYQXMKxA0W8JBxb4xCuq/DXN4qrG/Xt67rMlS9mVNc2ytse7JpG83r7qki+ISNIar3BfcLb"
+    b"p++xYhStZqq7L6KcSrpaTlEri2m12qio5lqO9lJNl56q77l7dKxUUquVdENHFFJs2mqFlNWymHa7Rkxd"
+    b"IwoqP3HWSqo/qti8popv0ZWrarJhVemW1aRjWU1kSc1NKP2HFQpBrWbyZxSimCKk1Yopq2U57XaNnLpG"
+    b"FKSgB9X1NsWIuKBLOa4iOukzVWoNbiVvzMlrfYgidymtS+nTlRZ0JYT2CODgO66Y2XU=",
+)
+
+
+def lib1_simple_drone1_models_mcdpr1_yaml_fresh() -> str:
+    return get_updated_str(
+        lib1_simple_drone1_models_mcdpr1_yaml,
+        "../../assets/test-data/downloaded/lib1-simple.drone1.models.mcdpr1.yaml",
+    )
+
+
+_check_md5(
+    "lib1_simple_drone1_models_mcdpr1_yaml",
+    lib1_simple_drone1_models_mcdpr1_yaml,
+    16821,
+    "bc7362db884c202af2ecf16be1e1d949",
+    "../../assets/test-data/downloaded/lib1-simple.drone1.models.mcdpr1.yaml",
+)
+lib1_simple_drone1_primitivedps_mcdpr1_yaml: str = decode_to_str(
+    b"eJztXc1u20YQvvsp9hAgbQpHst0UrW6FDQMpYsNQ0epoyBJtE5ZIgaRc+9gAAVLkNXroOY+QR/GTlEtR"
+    b"5P7MzlISKS7J3UtiSpr5dmZ2ZndnuPsqnNw78/HggJDIjWbOgPzuBK4TXsYPHlxvOiBXgTt3I/fRObs6"
+    b"mC7CwcEheZX/KPvZ2dUH318cJ4/kHxIyXRytvs/9GOCqIkBJhKtfHYpEMjIXy6fsEUwkIeSEk8BdRK7v"
+    b"Dch8+fTd7ffk5Z9/SZB+4zynKzHK6PqhEzFPUwDJ46vAny4n+afh8ibMKQDo1WRxwiJpJXE1+YzB5XJ+"
+    b"4wQh9+GNH0X+fEBe91/zmPzFgLz3bl3PjZ65T5bxk3BAQvMgPdyZh2m0o1HIYGAoKiApjPWwm/h+MA1R"
+    b"408Zn/rzRQzqgxvmuCb0med4kd7WESowHURjKC0VNYQeQ5FKg9IVvhHrxHkakCPhsRf50YAcC08DJ4xk"
+    b"FkreAvf30xi5aDy7Q+/vATrAPeMvclojOJGewxhQFFqTWDWVYawaImOgr4Ca9PYKCglUEKQeSDDVmIWo"
+    b"lO3NQq0OTBkaVeCK0DkgQCCAMGQFyELYRd1HgLpPSlC3SuBqcaPCxkS9ih3HTQ0e5g3GfYQXzEeLzmCN"
+    b"QMS1q4+uxH9CA6ou/ykKrPQZQROtu+4ZiGzFMIIyrBvEgYwz9UhTo9HgaUeYbK+pCgoZdnEDQsFAZoHO"
+    b"UtRs0CW8ehGPLeOlFXQZ8JRygCShmbFh7DTywCSCywTY3uiqXeTEDB101WyxjT1Pt1N7NQ7Gs5kzy0eO"
+    b"ar822/ZV9BPcQcYIciR1sU/GiZMWiOtnZzJuHQOJRZEtIbgfelYAs2KrRLhfRRiCLIvuA1xcX/l/OcE1"
+    b"QLUY74Q/myC4/faVyw6w7RzGopmL4V6Z6YzKM9OGeeeEBOqhaQNj16oN29Cvb1+hqfVyDs3yqc49eMqd"
+    b"OTO2FTXGoRNeXyxnkbuYPZ/6XhiNvahM2yQvXz6R/tt+/5iMepdtt1RQo4/LXRZEf45nS+c88OfqTj7S"
+    b"r1D4VMxwF+hOlGJdpgVSRMqF5MxKWg01lTf+lfUErgeL3F+Ei/HEqd+kDlGz0RlWG7zcCPgQ9Fiz8Y0z"
+    b"A8PqIbAHQZ/KzhAkDHoWVIY6CWrlh0tPJztl3APtoQE9EW2gyPRsveMARpkikUiMQ2Dcqcw2kEUybdBC"
+    b"mTZtWs/0wV2ZiXZVoIBLgz0l5CchLwkQBEbBrns2qLpgZWlUZYYrk51yObC7ad6At7CGJzSlZ7CGt63h"
+    b"6Xej2DpNoUfYtpCmbnPdrL+1Zl+LvxULKNfNjOIoPA8NbX2pcuJl5aEViNDcOJYdx3AV2IfRl17SVp7I"
+    b"1an/6kSu6JZUvlWAdqdNt4XmgVXL6uplC7juYgK0U9baY/eeYUsL5gLTxySv8ut0ejH2nqF0yoZzyduX"
+    b"j3+TH+g/H8EJpXK/u+rSC/X+9sYFGLRVMLj2UjxCm91X6byvgDbm5G05eVOOPuFDpmRMkinZCi5oO253"
+    b"qN0YYJKjNawurVBlni5TpC0c0mWI7KDjG/DybMmm1FYhCf5cDhRimBCDhEBAsEzjS1fbo1cbcbaLONZ+"
+    b"ZL8wbNgorjjQWyMpXJavSFNpqrILpKeaFlisSfIM9+K3oDRSF0+/MPj15KacwgFAB1M9XTSvhqq1hlM0"
+    b"7FRKWnEaB48Nq9xqVjPF4V5RgfIpG0x6aB7l5csnMI9SkgWV+sLib8xDMMdTBUo4p6PC2vCNiS6PwyID"
+    b"78x9dKeO6s2wTYYe6ZF3/T4Z3fce7qpadlQ2+MR3uPDpCPLO1vpdrVgUPBzwDa0KTUcCkEoE+mBtOVR1"
+    b"dXiknVRnpF9/83DXG91vFxH/iGnEA/IxRhOPrO3H4xtyTo56Jz/Fg7IRw1GSmYmarWeAbBayEZHejieR"
+    b"HwxSu9hyxuY40eXZcjzbJVhQiyQBLXt5+fwf/c9Hw82TU/yp6QCFWZtdPfHiMRufmD3kc4d85pAvLaF/"
+    b"nXB//cj99S77izMQbrwZeUxMky3Pns3ENXs2k7SOHBo//lp/EnqGCTviCaxEQo9iwiqQzPe6VWm9u/bO"
+    b"hF0+yrMxno3wzA86eStEkx28Dfxcs4G/24cydvJQ2e5MnDqlAnsDVNbMVpSpmDqlgv3f62TGefFV3QKx"
+    b"x2tV9KLe1y0o9koNPWwQdIvvKWjxpT/1mHtNZY/tMfeKPcP2cY8F1tR7UvYY9+xiNW12srtxd83DVMd9"
+    b"GDZZYpMlpSVLarh4BT3jZ8OadNXZPqYXkHFOzfhyPFuqnrXmFT1t8pZIKeXq9OKSX97+fETmvRC4t8T4"
+    b"GsTSS9apMOqtWZcRpEIBP0mFkqjPfJ9qovdkYybnPDepQGxYJWF3Jv0lTB1lYDAsFSjBzmzJC0LersLL"
+    b"7a55mOyeUmmi3La7pTo01p3lzix3ZXltfl6Xnzm3zLVJ3YC6oNYWqylQJvXYVUmC3rVUqiQYptjdaGtF"
+    b"iwAg9jBzzuSH1mrVkipYTF69nlInk7oYAYLMXiXVXKJAPxB9832QewDh58b73tipq7mq4UfH77B5WonF"
+    b"JPASit3gjResyK2BtpkYC1vKJPCFU6NcSpTNEbMpUFVSRkpNcgUPKv58mlRMjqpTQBK3DU2Vla0oWVmu"
+    b"rFQTh7WeTq2mUqtpVPJBYiscCBECbCVrG5F6XG4PwupZJEKqmMfoYFhUzjl9nrpIO0f/Pwu6rvo=",
+)
+
+
+def lib1_simple_drone1_primitivedps_mcdpr1_yaml_fresh() -> str:
+    return get_updated_str(
+        lib1_simple_drone1_primitivedps_mcdpr1_yaml,
+        "../../assets/test-data/downloaded/lib1-simple.drone1.primitivedps.mcdpr1.yaml",
+    )
+
+
+_check_md5(
+    "lib1_simple_drone1_primitivedps_mcdpr1_yaml",
+    lib1_simple_drone1_primitivedps_mcdpr1_yaml,
+    38308,
+    "9d162a77d77b6a581ae1f6d38d9be0c3",
+    "../../assets/test-data/downloaded/lib1-simple.drone1.primitivedps.mcdpr1.yaml",
+)
 
 resources = {
     "lib1-parts.discrete.posets.mcdpr1.yaml": lib1_parts_discrete_posets_mcdpr1_yaml,
     "lib1-parts.e01_empty.models.mcdpr1.yaml": lib1_parts_e01_empty_models_mcdpr1_yaml,
+    "lib1-parts.e01_empty.primitivedps.mcdpr1.yaml": lib1_parts_e01_empty_primitivedps_mcdpr1_yaml,
     "lib1-parts.e02_direct_connection.models.mcdpr1.yaml": lib1_parts_e02_direct_connection_models_mcdpr1_yaml,
+    "lib1-parts.e02_direct_connection.primitivedps.mcdpr1.yaml": lib1_parts_e02_direct_connection_primitivedps_mcdpr1_yaml,
     "lib1-parts.e03_splitter1.models.mcdpr1.yaml": lib1_parts_e03_splitter1_models_mcdpr1_yaml,
+    "lib1-parts.e03_splitter1.primitivedps.mcdpr1.yaml": lib1_parts_e03_splitter1_primitivedps_mcdpr1_yaml,
     "lib1-parts.e04_splitter2.models.mcdpr1.yaml": lib1_parts_e04_splitter2_models_mcdpr1_yaml,
+    "lib1-parts.e04_splitter2.primitivedps.mcdpr1.yaml": lib1_parts_e04_splitter2_primitivedps_mcdpr1_yaml,
     "lib1-parts.e05_multf.models.mcdpr1.yaml": lib1_parts_e05_multf_models_mcdpr1_yaml,
+    "lib1-parts.e05_multf.primitivedps.mcdpr1.yaml": lib1_parts_e05_multf_primitivedps_mcdpr1_yaml,
     "lib1-parts.e05_multr.models.mcdpr1.yaml": lib1_parts_e05_multr_models_mcdpr1_yaml,
+    "lib1-parts.e05_multr.primitivedps.mcdpr1.yaml": lib1_parts_e05_multr_primitivedps_mcdpr1_yaml,
     "lib1-parts.e05_scalef.models.mcdpr1.yaml": lib1_parts_e05_scalef_models_mcdpr1_yaml,
+    "lib1-parts.e05_scalef.primitivedps.mcdpr1.yaml": lib1_parts_e05_scalef_primitivedps_mcdpr1_yaml,
     "lib1-parts.e05_scaler.models.mcdpr1.yaml": lib1_parts_e05_scaler_models_mcdpr1_yaml,
+    "lib1-parts.e05_scaler.primitivedps.mcdpr1.yaml": lib1_parts_e05_scaler_primitivedps_mcdpr1_yaml,
     "lib1-parts.e05_sumf.models.mcdpr1.yaml": lib1_parts_e05_sumf_models_mcdpr1_yaml,
+    "lib1-parts.e05_sumf.primitivedps.mcdpr1.yaml": lib1_parts_e05_sumf_primitivedps_mcdpr1_yaml,
     "lib1-parts.e06_addf.models.mcdpr1.yaml": lib1_parts_e06_addf_models_mcdpr1_yaml,
+    "lib1-parts.e06_addf.primitivedps.mcdpr1.yaml": lib1_parts_e06_addf_primitivedps_mcdpr1_yaml,
     "lib1-parts.e06_addr.models.mcdpr1.yaml": lib1_parts_e06_addr_models_mcdpr1_yaml,
+    "lib1-parts.e06_addr.primitivedps.mcdpr1.yaml": lib1_parts_e06_addr_primitivedps_mcdpr1_yaml,
     "lib1-parts.e06_sumr.models.mcdpr1.yaml": lib1_parts_e06_sumr_models_mcdpr1_yaml,
+    "lib1-parts.e06_sumr.primitivedps.mcdpr1.yaml": lib1_parts_e06_sumr_primitivedps_mcdpr1_yaml,
     "lib1-parts.e07_ceil.models.mcdpr1.yaml": lib1_parts_e07_ceil_models_mcdpr1_yaml,
+    "lib1-parts.e07_ceil.primitivedps.mcdpr1.yaml": lib1_parts_e07_ceil_primitivedps_mcdpr1_yaml,
     "lib1-parts.e07_floor.models.mcdpr1.yaml": lib1_parts_e07_floor_models_mcdpr1_yaml,
+    "lib1-parts.e07_floor.primitivedps.mcdpr1.yaml": lib1_parts_e07_floor_primitivedps_mcdpr1_yaml,
     "lib1-parts.e10_conversions1.models.mcdpr1.yaml": lib1_parts_e10_conversions1_models_mcdpr1_yaml,
+    "lib1-parts.e10_conversions1.primitivedps.mcdpr1.yaml": lib1_parts_e10_conversions1_primitivedps_mcdpr1_yaml,
     "lib1-parts.e10_conversions2.models.mcdpr1.yaml": lib1_parts_e10_conversions2_models_mcdpr1_yaml,
+    "lib1-parts.e10_conversions2.primitivedps.mcdpr1.yaml": lib1_parts_e10_conversions2_primitivedps_mcdpr1_yaml,
     "lib1-parts.e11_constant_fun.models.mcdpr1.yaml": lib1_parts_e11_constant_fun_models_mcdpr1_yaml,
+    "lib1-parts.e11_constant_fun.primitivedps.mcdpr1.yaml": lib1_parts_e11_constant_fun_primitivedps_mcdpr1_yaml,
     "lib1-parts.e11_constant_res.models.mcdpr1.yaml": lib1_parts_e11_constant_res_models_mcdpr1_yaml,
+    "lib1-parts.e11_constant_res.primitivedps.mcdpr1.yaml": lib1_parts_e11_constant_res_primitivedps_mcdpr1_yaml,
+    "lib1-parts.e12_catalogue.models.mcdpr1.yaml": lib1_parts_e12_catalogue_models_mcdpr1_yaml,
+    "lib1-parts.e12_catalogue.primitivedps.mcdpr1.yaml": lib1_parts_e12_catalogue_primitivedps_mcdpr1_yaml,
+    "lib1-parts.e12_catalogue_empty.models.mcdpr1.yaml": lib1_parts_e12_catalogue_empty_models_mcdpr1_yaml,
+    "lib1-parts.e12_catalogue_empty.primitivedps.mcdpr1.yaml": lib1_parts_e12_catalogue_empty_primitivedps_mcdpr1_yaml,
+    "lib1-parts.e12_catalogue_true.models.mcdpr1.yaml": lib1_parts_e12_catalogue_true_models_mcdpr1_yaml,
+    "lib1-parts.e12_catalogue_true.primitivedps.mcdpr1.yaml": lib1_parts_e12_catalogue_true_primitivedps_mcdpr1_yaml,
     "lib1-parts.nats.posets.mcdpr1.yaml": lib1_parts_nats_posets_mcdpr1_yaml,
     "lib1-parts.reals.posets.mcdpr1.yaml": lib1_parts_reals_posets_mcdpr1_yaml,
     "lib1-parts.reals_with_units.posets.mcdpr1.yaml": lib1_parts_reals_with_units_posets_mcdpr1_yaml,
+    "lib1-simple.all_together.models.mcdpr1.yaml": lib1_simple_all_together_models_mcdpr1_yaml,
+    "lib1-simple.all_together.primitivedps.mcdpr1.yaml": lib1_simple_all_together_primitivedps_mcdpr1_yaml,
+    "lib1-simple.drone1.models.mcdpr1.yaml": lib1_simple_drone1_models_mcdpr1_yaml,
+    "lib1-simple.drone1.primitivedps.mcdpr1.yaml": lib1_simple_drone1_primitivedps_mcdpr1_yaml,
 }
```

## act4e_mcdp/loading.py

```diff
@@ -13,30 +13,36 @@
     NodeResource,
     SimpleWrap,
 )
 from .posets import FinitePoset, Numbers, Poset, PosetProduct
 from .primitivedps import (
     AmbientConversion,
     CatalogueDP,
+    M_Res_DivideConstant_DP,
     Constant,
+    DPLoop2,
     DPSeries,
     EntryInfo,
+    IdentityDP,
     JoinNDP,
     Limit,
     M_Ceil_DP,
     M_FloorFun_DP,
     M_Fun_AddConstant_DP,
     M_Fun_AddMany_DP,
     M_Fun_MultiplyConstant_DP,
     M_Fun_MultiplyMany_DP,
+    M_Power_DP,
     M_Res_AddConstant_DP,
     M_Res_AddMany_DP,
     M_Res_MultiplyConstant_DP,
     M_Res_MultiplyMany_DP,
     MeetNDualDP,
+    Mux,
+    ParallelDP,
     PrimitiveDP,
     UnitConversion,
     ValueFromPoset,
 )
 
 loaders = {}
 
@@ -110,14 +116,40 @@
 
 @loader_for("M_Res_MultiplyConstant_DP")
 def load_M_Res_MultiplyConstant_DP(ob: dict):
     fields = _load_DP_fields(ob)
     return M_Res_MultiplyConstant_DP(**fields)
 
 
+@loader_for("M_Res_DivideConstant_DP")
+def load_M_Res_DivideConstant_DP(ob: dict):
+    fields = _load_DP_fields(ob)
+    return M_Res_DivideConstant_DP(**fields)
+
+
+@loader_for("IdentityDP")
+def load_Identity_DP(ob: dict):
+    fields = _load_DP_fields(ob)
+    return IdentityDP(**fields)
+
+
+@loader_for("Mux")
+def load_Mux(ob: dict):
+    fields = _load_DP_fields(ob)
+    fields["coords"] = ob["coords"]
+    return Mux(**fields)
+
+
+@loader_for("DPLoop2")
+def load_DPLoop2(ob: dict):
+    fields = _load_DP_fields(ob)
+    fields["dp"] = load_repr1(ob["dp1"], PrimitiveDP)
+    return DPLoop2(**fields)
+
+
 @loader_for("M_Fun_MultiplyConstant_DP")
 def load_M_Fun_MultiplyConstant_DP(ob: dict):
     fields = _load_DP_fields(ob)
     return M_Fun_MultiplyConstant_DP(**fields)
 
 
 @loader_for("M_Res_AddConstant_DP")
@@ -147,14 +179,21 @@
 @loader_for("M_Fun_MultiplyMany_DP")
 def load_M_Fun_MultiplyMany_DP(ob: dict):
     fields = _load_DP_fields(ob)
 
     return M_Fun_MultiplyMany_DP(**fields)
 
 
+@loader_for("M_Power_DP")
+def load_M_Power_DP(ob: dict):
+    fields = _load_DP_fields(ob)
+
+    return M_Power_DP(**fields, num=ob["num"], den=ob["den"])
+
+
 @loader_for("M_Ceil_DP")
 def load_M_Ceil_DP(ob: dict):
     fields = _load_DP_fields(ob)
 
     return M_Ceil_DP(**fields)
 
 
@@ -181,14 +220,26 @@
     for dp in ob["dps"]:
         dp = load_repr1(dp, PrimitiveDP)
         subs.append(dp)
 
     return DPSeries(**fields, subs=subs)
 
 
+@loader_for("ParallelN")
+def load_ParallelN(ob: dict):
+    fields = _load_DP_fields(ob)
+
+    subs = []
+    for dp in ob["dps"]:
+        dp = load_repr1(dp, PrimitiveDP)
+        subs.append(dp)
+
+    return ParallelDP(**fields, subs=subs)
+
+
 #
 # @loader_for('M_Ceil_DP')
 # def load_M_Ceil_DP(ob: dict):
 #     F = load_repr1(ob['F'], Poset)
 #     R = load_repr1(ob['R'], Poset)
 #
 #     return PrimitiveDP(F=F, R=R)
@@ -327,15 +378,15 @@
         raise ValueError(msg)
     loader = loaders[title]
     try:
         return loader(data)
     except Exception as e:
         datas = yaml.dump(data, allow_unicode=True)
         logger.exception("Error while loading %r\n%s", title, datas, exc_info=e)
-        msg = f"Error while loading {title!r}: \n{datas}"
+        msg = f"Error while loading {title!r}:"
         raise ValueError(msg) from e
 
 
 def parse_yaml_value(poset: Poset, ob: object) -> object:
     match poset:
         case Numbers():
             if not isinstance(ob, (int, str, float, bool)):
```

## act4e_mcdp/primitivedps.py

```diff
@@ -2,31 +2,39 @@
 from fractions import Fraction
 from typing import Optional
 
 from .posets import Poset
 
 __all__ = [
     "AmbientConversion",
+    "CatalogueDP",
     "Constant",
+    "DPLoop2",
     "DPSeries",
+    "EntryInfo",
+    "IdentityDP",
     "JoinNDP",
     "Limit",
     "M_Ceil_DP",
     "M_FloorFun_DP",
     "M_Fun_AddConstant_DP",
     "M_Fun_AddMany_DP",
     "M_Fun_MultiplyConstant_DP",
     "M_Fun_MultiplyMany_DP",
     "M_Fun_MultiplyMany_DP",
+    "M_Power_DP",
     "M_Res_AddConstant_DP",
     "M_Res_AddMany_DP",
+    "M_Res_DivideConstant_DP",
     "M_Res_MultiplyConstant_DP",
     "M_Res_MultiplyMany_DP",
     "MeetNDualDP",
     "MeetNDualDP",
+    "Mux",
+    "ParallelDP",
     "PrimitiveDP",
     "UnitConversion",
     "ValueFromPoset",
 ]
 
 
 @dataclass
@@ -58,14 +66,21 @@
         subs: The list of DPs
     """
 
     subs: list[PrimitiveDP]
 
 
 @dataclass
+class ParallelDP(PrimitiveDP):
+    r""" """
+
+    subs: list[PrimitiveDP]
+
+
+@dataclass
 class ValueFromPoset:
     r"""
     A value in a particular poset (a "typed" value).
 
     Depending on the poset, we have different types:
 
     - For [FinitePoset][act4e_mcdp.posets.FinitePoset] the values are strings.
@@ -103,14 +118,22 @@
     """
 
     vu: ValueFromPoset
     opspace: Poset
 
 
 @dataclass
+class M_Res_DivideConstant_DP(PrimitiveDP):
+    r""" """
+
+    vu: ValueFromPoset
+    opspace: Poset
+
+
+@dataclass
 class M_Fun_MultiplyConstant_DP(PrimitiveDP):
     r"""
     Multiplication by a constant on the right side.
 
     Relation:
 
         $$
@@ -248,14 +271,28 @@
 
     """
 
     opspace: Poset
 
 
 @dataclass
+class Mux(PrimitiveDP):
+    r""" """
+
+    coords: object
+
+
+@dataclass
+class M_Power_DP(PrimitiveDP):
+    r""" """
+    num: int
+    den: int
+
+
+@dataclass
 class M_Fun_MultiplyMany_DP(PrimitiveDP):
     r"""
     Multiplication on the right side.
 
 
     Relation:
 
@@ -400,14 +437,46 @@
 
     """
 
     common: Poset
 
 
 @dataclass
+class IdentityDP(PrimitiveDP):
+    r"""
+    This is the identity DP ($\F = \R$)
+
+    Relation:
+
+        $$
+          \fun \leq \res
+        $$
+
+
+    Attributes:
+
+        F (Poset): The functionality poset $\F$
+        R (Poset): The resources poset $\R$
+
+
+    Note:
+
+        It can be seen as a special case
+        of [AmbientConversion][act4e_mcdp.primitivedps.AmbientConversion]
+        where $\common = \F = \R$.
+    """
+
+
+@dataclass
+class DPLoop2(PrimitiveDP):
+    r""" """
+    dp: PrimitiveDP
+
+
+@dataclass
 class Limit(PrimitiveDP):
     r"""
     Implements a bound on the functionality.
 
     This is the dual of [Constant][act4e_mcdp.primitivedps.Constant].
 
     Relation:
```

## Comparing `act4e_mcdp-0.4.2.dist-info/RECORD` & `act4e_mcdp-0.4.3.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 act4e_mcdp/__init__.py,sha256=E_ujpgzc-ou4a5DKP7fNLO7NZVky0K3bl5mp2ob3ahU,347
-act4e_mcdp/autogen_packed_test_data.py,sha256=C2PZegLbjS0c2lWXVBSP0EIivpLM3lyVrfSY_mzx6gs,30570
+act4e_mcdp/autogen_packed_test_data.py,sha256=Iadf_CeH5_iFkDPJWFATFzLRM_FImr7fg2yN7lDYsVg,67896
 act4e_mcdp/download.py,sha256=fXm46ISIYvpFjouSMB0l0XLuJWw5CxZSpgi-fvmxMGA,571
-act4e_mcdp/loading.py,sha256=xrozob-NEjeAUT7LYslgnn7obwTKad23Atd-BCGdCuI,9138
+act4e_mcdp/loading.py,sha256=ooKDUB74HRcWabiMkuApRCvO1YWYlgqeZIU4IOSpe-s,10217
 act4e_mcdp/main.py,sha256=c_Fy0nmJrrikwDQpdv_y0shFrH3AHg1auOdk1Dsc_Hs,3363
 act4e_mcdp/nameddps.py,sha256=OaYt-P9pGt6TQa9oXWWHZI4PFRt9kPyfQatPEx9rH60,4381
 act4e_mcdp/posets.py,sha256=7iijB7waZd3nTyK-_eNBR6YZOWhcTUYtKqCm7irpFKE,1790
-act4e_mcdp/primitivedps.py,sha256=yyXovQ4cfb4SzSpGRFf46Xg1cnTeiOxgBREHnDVdSAg,10766
+act4e_mcdp/primitivedps.py,sha256=-Ppy6XjZUGN3sS8lRvRezIpEb7JODNnP-hWD62360_8,11777
 act4e_mcdp/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 act4e_mcdp/solution_interface.py,sha256=7TjPbeJKbZ_29c1l5eW-TlWQEP0TxEl9I9JclJY9pi4,3944
-act4e_mcdp-0.4.2.dist-info/METADATA,sha256=o1CpGI6Z181wCKnrcdlDPQ0HWcQuUHv9XyX8XItAa0w,361
-act4e_mcdp-0.4.2.dist-info/WHEEL,sha256=WGfLGfLX43Ei_YORXSnT54hxFygu34kMpcQdmgmEwCQ,88
-act4e_mcdp-0.4.2.dist-info/entry_points.txt,sha256=ab4CbY_rBOTC8YJBuIQeKxZExEYTrXx6fDsX1GivxXo,109
-act4e_mcdp-0.4.2.dist-info/RECORD,,
+act4e_mcdp-0.4.3.dist-info/METADATA,sha256=1grx67BgZhdm1I-jyL8BThu8gCrMifq1kVI2ygTZD_c,361
+act4e_mcdp-0.4.3.dist-info/WHEEL,sha256=WGfLGfLX43Ei_YORXSnT54hxFygu34kMpcQdmgmEwCQ,88
+act4e_mcdp-0.4.3.dist-info/entry_points.txt,sha256=ab4CbY_rBOTC8YJBuIQeKxZExEYTrXx6fDsX1GivxXo,109
+act4e_mcdp-0.4.3.dist-info/RECORD,,
```

