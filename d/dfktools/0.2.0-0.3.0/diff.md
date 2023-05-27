# Comparing `tmp/dfktools-0.2.0.tar.gz` & `tmp/dfktools-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfktools-0.2.0.tar", last modified: Sun Dec 11 05:43:12 2022, max compression
+gzip compressed data, was "dfktools-0.3.0.tar", last modified: Sat May 27 14:19:42 2023, max compression
```

## Comparing `dfktools-0.2.0.tar` & `dfktools-0.3.0.tar`

### file list

```diff
@@ -1,159 +1,163 @@
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2022-12-11 05:43:12.551573 dfktools-0.2.0/
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     1098 2022-07-17 06:13:39.000000 dfktools-0.2.0/LICENSE
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     9965 2022-12-11 05:43:12.551573 dfktools-0.2.0/PKG-INFO
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     8418 2022-09-25 13:57:34.000000 dfktools-0.2.0/README.md
--rw-rw-r--   0 ortis     (1000) ortis     (1000)      563 2022-12-08 12:29:53.000000 dfktools-0.2.0/pyproject.toml
--rw-rw-r--   0 ortis     (1000) ortis     (1000)      579 2022-12-11 05:43:12.551573 dfktools-0.2.0/setup.cfg
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2022-12-11 05:43:12.539572 dfktools-0.2.0/src/
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2022-12-11 05:43:12.543573 dfktools-0.2.0/src/dfktools/
--rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 05:33:06.000000 dfktools-0.2.0/src/dfktools/__init__.py
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2022-12-11 05:43:12.543573 dfktools-0.2.0/src/dfktools/airdrop/
--rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-09-02 13:16:15.000000 dfktools-0.2.0/src/dfktools/airdrop/__init__.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     8905 2022-12-08 06:48:02.000000 dfktools-0.2.0/src/dfktools/airdrop/airdrop.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     1329 2022-12-08 08:58:25.000000 dfktools-0.2.0/src/dfktools/airdrop_example.py
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2022-12-11 05:43:12.543573 dfktools-0.2.0/src/dfktools/alchemist/
--rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 05:33:06.000000 dfktools-0.2.0/src/dfktools/alchemist/__init__.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)    10485 2022-12-08 06:49:04.000000 dfktools-0.2.0/src/dfktools/alchemist/alchemist.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     1800 2022-12-08 08:58:36.000000 dfktools-0.2.0/src/dfktools/alchemist_example.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)      681 2022-08-15 13:56:20.000000 dfktools-0.2.0/src/dfktools/assisting_example.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     3713 2022-12-08 09:01:05.000000 dfktools-0.2.0/src/dfktools/auction_example.py
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2022-12-11 05:43:12.543573 dfktools-0.2.0/src/dfktools/auctions/
--rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 05:33:06.000000 dfktools-0.2.0/src/dfktools/auctions/__init__.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     1918 2022-07-17 05:33:06.000000 dfktools-0.2.0/src/dfktools/auctions/auction.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)    17501 2022-07-18 13:44:08.000000 dfktools-0.2.0/src/dfktools/auctions/auction_core.py
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2022-12-11 05:43:12.543573 dfktools-0.2.0/src/dfktools/auctions/hero/
--rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 05:33:06.000000 dfktools-0.2.0/src/dfktools/auctions/hero/__init__.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     1874 2022-07-17 05:33:06.000000 dfktools-0.2.0/src/dfktools/auctions/hero/rent_auctions.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)    33259 2022-12-08 06:54:26.000000 dfktools-0.2.0/src/dfktools/auctions/hero/sale_auctions.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)      164 2022-12-08 06:49:54.000000 dfktools-0.2.0/src/dfktools/auctions/land.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)      248 2022-12-08 06:51:07.000000 dfktools-0.2.0/src/dfktools/auctions/pet.py
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2022-12-11 05:43:12.543573 dfktools-0.2.0/src/dfktools/auctions/utils/
--rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 05:33:06.000000 dfktools-0.2.0/src/dfktools/auctions/utils/__init__.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)      439 2022-07-17 14:24:54.000000 dfktools-0.2.0/src/dfktools/auctions/utils/utils.py
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2022-12-11 05:43:12.543573 dfktools-0.2.0/src/dfktools/bridge/
--rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-18 04:09:41.000000 dfktools-0.2.0/src/dfktools/bridge/__init__.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     6049 2022-07-18 13:44:08.000000 dfktools-0.2.0/src/dfktools/bridge/dfktears_bridge.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     8688 2022-12-08 06:54:26.000000 dfktools-0.2.0/src/dfktools/bridge/hero_bridge.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     1826 2022-07-18 13:44:08.000000 dfktools-0.2.0/src/dfktools/bridge_example.py
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2022-12-11 05:43:12.543573 dfktools-0.2.0/src/dfktools/consumable/
--rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 05:33:06.000000 dfktools-0.2.0/src/dfktools/consumable/__init__.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)    12945 2022-12-08 06:20:30.000000 dfktools-0.2.0/src/dfktools/consumable/consumable.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     1077 2022-12-08 09:06:06.000000 dfktools-0.2.0/src/dfktools/consumable_example.py
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2022-12-11 05:43:12.543573 dfktools-0.2.0/src/dfktools/dex/
--rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 05:33:06.000000 dfktools-0.2.0/src/dfktools/dex/__init__.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     3084 2022-08-13 02:17:33.000000 dfktools-0.2.0/src/dfktools/dex/crystal.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     5483 2022-12-08 08:57:45.000000 dfktools-0.2.0/src/dfktools/dex/erc1155.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)    34438 2022-12-08 12:28:36.000000 dfktools-0.2.0/src/dfktools/dex/erc20.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)    12437 2022-12-08 08:56:40.000000 dfktools-0.2.0/src/dfktools/dex/item_erc1155.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     3066 2022-12-08 06:46:42.000000 dfktools-0.2.0/src/dfktools/dex/jade.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     3070 2022-07-18 13:44:08.000000 dfktools-0.2.0/src/dfktools/dex/jewel.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)    21902 2022-12-08 06:47:24.000000 dfktools-0.2.0/src/dfktools/dex/master_gardener.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     3566 2022-12-08 09:09:10.000000 dfktools-0.2.0/src/dfktools/dex/uniswap_v2_factory.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)    14173 2022-07-18 13:44:08.000000 dfktools-0.2.0/src/dfktools/dex/uniswap_v2_pair.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)    18809 2022-12-08 06:55:52.000000 dfktools-0.2.0/src/dfktools/dex/uniswap_v2_router.py
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2022-12-11 05:43:12.543573 dfktools-0.2.0/src/dfktools/dex/utils/
--rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 05:33:06.000000 dfktools-0.2.0/src/dfktools/dex/utils/__init__.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     1078 2022-07-17 05:33:06.000000 dfktools-0.2.0/src/dfktools/dex/utils/utils.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     4408 2022-12-08 09:11:29.000000 dfktools-0.2.0/src/dfktools/dex_example.py
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2022-12-11 05:43:12.543573 dfktools-0.2.0/src/dfktools/duel/
--rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 06:15:15.000000 dfktools-0.2.0/src/dfktools/duel/__init__.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)    44446 2022-12-08 06:58:24.000000 dfktools-0.2.0/src/dfktools/duel/duel.py
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2022-12-11 05:43:12.547572 dfktools-0.2.0/src/dfktools/duel/utils/
--rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 06:15:15.000000 dfktools-0.2.0/src/dfktools/duel/utils/__init__.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)      934 2022-09-19 15:24:02.000000 dfktools-0.2.0/src/dfktools/duel/utils/utils.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     1803 2022-12-08 09:31:23.000000 dfktools-0.2.0/src/dfktools/duel_example.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     1066 2022-12-08 09:31:30.000000 dfktools-0.2.0/src/dfktools/erc20_example.py
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2022-12-11 05:43:12.547572 dfktools-0.2.0/src/dfktools/genes/
--rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 05:33:06.000000 dfktools-0.2.0/src/dfktools/genes/__init__.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     1824 2022-07-17 05:33:06.000000 dfktools-0.2.0/src/dfktools/genes/gene_science_v1.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     2162 2022-07-17 05:33:06.000000 dfktools-0.2.0/src/dfktools/genes/gene_science_v2.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     1423 2022-07-17 11:30:49.000000 dfktools-0.2.0/src/dfktools/genes_example.py
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2022-12-11 05:43:12.547572 dfktools-0.2.0/src/dfktools/hero/
--rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 05:33:06.000000 dfktools-0.2.0/src/dfktools/hero/__init__.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     1457 2022-07-17 06:13:39.000000 dfktools-0.2.0/src/dfktools/hero/hero.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)    33253 2022-12-08 06:20:30.000000 dfktools-0.2.0/src/dfktools/hero/hero_core.py
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2022-12-11 05:43:12.547572 dfktools-0.2.0/src/dfktools/hero/utils/
--rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 05:33:06.000000 dfktools-0.2.0/src/dfktools/hero/utils/__init__.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     7122 2022-12-08 10:14:17.000000 dfktools-0.2.0/src/dfktools/hero/utils/utils.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     2218 2022-12-08 09:36:19.000000 dfktools-0.2.0/src/dfktools/hero_example.py
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2022-12-11 05:43:12.547572 dfktools-0.2.0/src/dfktools/land/
--rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 05:33:06.000000 dfktools-0.2.0/src/dfktools/land/__init__.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)    16747 2022-12-08 07:01:16.000000 dfktools-0.2.0/src/dfktools/land/land.py
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2022-12-11 05:43:12.547572 dfktools-0.2.0/src/dfktools/land/utils/
--rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 05:33:06.000000 dfktools-0.2.0/src/dfktools/land/utils/__init__.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)      347 2022-07-17 05:33:06.000000 dfktools-0.2.0/src/dfktools/land/utils/utils.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     1218 2022-12-08 07:01:50.000000 dfktools-0.2.0/src/dfktools/land_example.py
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2022-12-11 05:43:12.547572 dfktools-0.2.0/src/dfktools/meditation/
--rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 05:33:06.000000 dfktools-0.2.0/src/dfktools/meditation/__init__.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)    32032 2022-12-08 07:03:58.000000 dfktools-0.2.0/src/dfktools/meditation/meditation.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     3687 2022-12-08 09:38:50.000000 dfktools-0.2.0/src/dfktools/meditation_example.py
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2022-12-11 05:43:12.547572 dfktools-0.2.0/src/dfktools/perilous_journey/
--rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 05:33:06.000000 dfktools-0.2.0/src/dfktools/perilous_journey/__init__.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)    10077 2022-07-17 05:33:06.000000 dfktools-0.2.0/src/dfktools/perilous_journey/perilous_journey.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     2567 2022-10-01 11:20:15.000000 dfktools-0.2.0/src/dfktools/pet_example.py
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2022-12-11 05:43:12.547572 dfktools-0.2.0/src/dfktools/pets/
--rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 13:32:00.000000 dfktools-0.2.0/src/dfktools/pets/__init__.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)    13130 2022-12-08 07:04:59.000000 dfktools-0.2.0/src/dfktools/pets/exchange.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)    15146 2022-12-08 07:04:59.000000 dfktools-0.2.0/src/dfktools/pets/hatchery.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)    22647 2022-12-08 07:05:23.000000 dfktools-0.2.0/src/dfktools/pets/pet_core.py
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2022-12-11 05:43:12.547572 dfktools-0.2.0/src/dfktools/pets/utils/
--rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 14:45:38.000000 dfktools-0.2.0/src/dfktools/pets/utils/__init__.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     1913 2022-07-17 15:02:12.000000 dfktools-0.2.0/src/dfktools/pets/utils/utils.py
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2022-12-11 05:43:12.547572 dfktools-0.2.0/src/dfktools/profile/
--rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 05:33:06.000000 dfktools-0.2.0/src/dfktools/profile/__init__.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     7561 2022-07-17 05:33:06.000000 dfktools-0.2.0/src/dfktools/profile/profile.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)    11708 2022-12-08 09:42:02.000000 dfktools-0.2.0/src/dfktools/profile/profile_v2.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)      692 2022-12-08 09:42:02.000000 dfktools-0.2.0/src/dfktools/profile_example.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     5623 2022-12-08 09:48:49.000000 dfktools-0.2.0/src/dfktools/quest_example.py
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2022-12-11 05:43:12.547572 dfktools-0.2.0/src/dfktools/quests/
--rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 05:33:06.000000 dfktools-0.2.0/src/dfktools/quests/__init__.py
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2022-12-11 05:43:12.547572 dfktools-0.2.0/src/dfktools/quests/professions/
--rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 05:33:06.000000 dfktools-0.2.0/src/dfktools/quests/professions/__init__.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)      329 2022-12-08 06:24:10.000000 dfktools-0.2.0/src/dfktools/quests/professions/fishing.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)      329 2022-12-08 06:24:41.000000 dfktools-0.2.0/src/dfktools/quests/professions/foraging.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     3345 2022-12-08 07:25:12.000000 dfktools-0.2.0/src/dfktools/quests/professions/gardening.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)      521 2022-12-08 06:25:47.000000 dfktools-0.2.0/src/dfktools/quests/professions/mining.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)    40738 2022-08-13 02:17:33.000000 dfktools-0.2.0/src/dfktools/quests/quest_core_v1.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)    32249 2022-12-08 06:22:38.000000 dfktools-0.2.0/src/dfktools/quests/quest_core_v2.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     2479 2022-07-18 04:06:28.000000 dfktools-0.2.0/src/dfktools/quests/quest_v1.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     2308 2022-09-19 15:00:40.000000 dfktools-0.2.0/src/dfktools/quests/quest_v2.py
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2022-12-11 05:43:12.551573 dfktools-0.2.0/src/dfktools/quests/training/
--rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 05:33:06.000000 dfktools-0.2.0/src/dfktools/quests/training/__init__.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)      259 2022-12-08 06:33:57.000000 dfktools-0.2.0/src/dfktools/quests/training/agility_training.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)      260 2022-12-08 06:44:01.000000 dfktools-0.2.0/src/dfktools/quests/training/dexterity_training.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)      260 2022-12-08 06:44:14.000000 dfktools-0.2.0/src/dfktools/quests/training/endurance_training.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)      263 2022-12-08 06:44:28.000000 dfktools-0.2.0/src/dfktools/quests/training/intelligence_training.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)      255 2022-12-08 06:44:45.000000 dfktools-0.2.0/src/dfktools/quests/training/luck_training.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)      260 2022-12-08 06:46:04.000000 dfktools-0.2.0/src/dfktools/quests/training/strength_training.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)      259 2022-12-08 06:45:11.000000 dfktools-0.2.0/src/dfktools/quests/training/vitality_training.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)      257 2022-12-08 06:44:57.000000 dfktools-0.2.0/src/dfktools/quests/training/wisdom_training.py
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2022-12-11 05:43:12.551573 dfktools-0.2.0/src/dfktools/quests/utils/
--rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 05:33:06.000000 dfktools-0.2.0/src/dfktools/quests/utils/__init__.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     3655 2022-07-21 14:45:27.000000 dfktools-0.2.0/src/dfktools/quests/utils/utils.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)    15405 2022-07-17 05:33:06.000000 dfktools-0.2.0/src/dfktools/quests/wishing_well.py
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2022-12-11 05:43:12.551573 dfktools-0.2.0/src/dfktools/raffle/
--rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 06:27:09.000000 dfktools-0.2.0/src/dfktools/raffle/__init__.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)    21592 2022-12-08 09:51:41.000000 dfktools-0.2.0/src/dfktools/raffle/raffle_master.py
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2022-12-11 05:43:12.551573 dfktools-0.2.0/src/dfktools/raffle/utils/
--rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 06:27:09.000000 dfktools-0.2.0/src/dfktools/raffle/utils/__init__.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)      738 2022-07-17 06:27:09.000000 dfktools-0.2.0/src/dfktools/raffle/utils/utils.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     2228 2022-12-08 09:51:41.000000 dfktools-0.2.0/src/dfktools/raffle_example.py
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2022-12-11 05:43:12.551573 dfktools-0.2.0/src/dfktools/stone_carver/
--rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-09-02 13:16:15.000000 dfktools-0.2.0/src/dfktools/stone_carver/__init__.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)    12804 2022-12-08 09:53:39.000000 dfktools-0.2.0/src/dfktools/stone_carver/stone_carver.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     1844 2022-12-08 09:53:39.000000 dfktools-0.2.0/src/dfktools/stone_carver_example.py
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2022-12-11 05:43:12.551573 dfktools-0.2.0/src/dfktools/summoning/
--rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 05:33:06.000000 dfktools-0.2.0/src/dfktools/summoning/__init__.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)    16133 2022-12-08 07:19:30.000000 dfktools-0.2.0/src/dfktools/summoning/assisting.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)    11172 2022-12-08 07:21:47.000000 dfktools-0.2.0/src/dfktools/summoning/crystals.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)    26791 2022-12-08 07:22:19.000000 dfktools-0.2.0/src/dfktools/summoning/crystals_v2.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)    10934 2022-08-13 04:50:15.000000 dfktools-0.2.0/src/dfktools/summoning/serendale_assisting.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)    26275 2022-12-08 07:23:16.000000 dfktools-0.2.0/src/dfktools/summoning/summoning.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     2930 2022-12-08 09:59:25.000000 dfktools-0.2.0/src/dfktools/summoning_example.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     1418 2022-07-17 05:33:06.000000 dfktools-0.2.0/src/dfktools/wishing_well_quest_example.py
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2022-12-11 05:43:12.543573 dfktools-0.2.0/src/dfktools.egg-info/
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     9965 2022-12-11 05:43:12.000000 dfktools-0.2.0/src/dfktools.egg-info/PKG-INFO
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     4337 2022-12-11 05:43:12.000000 dfktools-0.2.0/src/dfktools.egg-info/SOURCES.txt
--rw-rw-r--   0 ortis     (1000) ortis     (1000)        1 2022-12-11 05:43:12.000000 dfktools-0.2.0/src/dfktools.egg-info/dependency_links.txt
--rw-rw-r--   0 ortis     (1000) ortis     (1000)       60 2022-12-11 05:43:12.000000 dfktools-0.2.0/src/dfktools.egg-info/requires.txt
--rw-rw-r--   0 ortis     (1000) ortis     (1000)        9 2022-12-11 05:43:12.000000 dfktools-0.2.0/src/dfktools.egg-info/top_level.txt
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-05-27 14:19:42.828727 dfktools-0.3.0/
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     1098 2022-07-17 06:13:39.000000 dfktools-0.3.0/LICENSE
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     9848 2023-05-27 14:19:42.828727 dfktools-0.3.0/PKG-INFO
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     8304 2023-05-20 12:43:55.000000 dfktools-0.3.0/README.md
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)      563 2023-05-25 08:54:11.000000 dfktools-0.3.0/pyproject.toml
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)      579 2023-05-27 14:19:42.828727 dfktools-0.3.0/setup.cfg
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-05-27 14:19:42.780727 dfktools-0.3.0/src/
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-05-27 14:19:42.796727 dfktools-0.3.0/src/dfktools/
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 05:33:06.000000 dfktools-0.3.0/src/dfktools/__init__.py
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-05-27 14:19:42.796727 dfktools-0.3.0/src/dfktools/airdrop/
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-09-02 13:16:15.000000 dfktools-0.3.0/src/dfktools/airdrop/__init__.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     8867 2023-05-20 13:32:46.000000 dfktools-0.3.0/src/dfktools/airdrop/airdrop.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     1320 2023-05-17 06:47:32.000000 dfktools-0.3.0/src/dfktools/airdrop_example.py
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-05-27 14:19:42.796727 dfktools-0.3.0/src/dfktools/alchemist/
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 05:33:06.000000 dfktools-0.3.0/src/dfktools/alchemist/__init__.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)    10440 2023-05-20 13:33:08.000000 dfktools-0.3.0/src/dfktools/alchemist/alchemist.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     1791 2023-05-17 06:47:32.000000 dfktools-0.3.0/src/dfktools/alchemist_example.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)      681 2022-08-15 13:56:20.000000 dfktools-0.3.0/src/dfktools/assisting_example.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     3706 2023-05-17 06:47:32.000000 dfktools-0.3.0/src/dfktools/auction_example.py
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-05-27 14:19:42.796727 dfktools-0.3.0/src/dfktools/auctions/
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 05:33:06.000000 dfktools-0.3.0/src/dfktools/auctions/__init__.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     1918 2022-07-17 05:33:06.000000 dfktools-0.3.0/src/dfktools/auctions/auction.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)    17481 2023-05-17 09:17:55.000000 dfktools-0.3.0/src/dfktools/auctions/auction_core.py
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-05-27 14:19:42.800727 dfktools-0.3.0/src/dfktools/auctions/hero/
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 05:33:06.000000 dfktools-0.3.0/src/dfktools/auctions/hero/__init__.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     1874 2022-07-17 05:33:06.000000 dfktools-0.3.0/src/dfktools/auctions/hero/rent_auctions.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)    32597 2023-05-17 09:17:55.000000 dfktools-0.3.0/src/dfktools/auctions/hero/sale_auctions.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)      164 2022-12-08 06:49:54.000000 dfktools-0.3.0/src/dfktools/auctions/land.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)      248 2022-12-08 06:51:07.000000 dfktools-0.3.0/src/dfktools/auctions/pet.py
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-05-27 14:19:42.800727 dfktools-0.3.0/src/dfktools/auctions/utils/
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 05:33:06.000000 dfktools-0.3.0/src/dfktools/auctions/utils/__init__.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)      439 2022-07-17 14:24:54.000000 dfktools-0.3.0/src/dfktools/auctions/utils/utils.py
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-05-27 14:19:42.800727 dfktools-0.3.0/src/dfktools/bridge/
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-18 04:09:41.000000 dfktools-0.3.0/src/dfktools/bridge/__init__.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     6047 2023-05-17 09:17:55.000000 dfktools-0.3.0/src/dfktools/bridge/dfktears_bridge.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     8688 2023-05-17 09:17:55.000000 dfktools-0.3.0/src/dfktools/bridge/hero_bridge.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     1810 2023-05-17 06:47:32.000000 dfktools-0.3.0/src/dfktools/bridge_example.py
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-05-27 14:19:42.800727 dfktools-0.3.0/src/dfktools/consumable/
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 05:33:06.000000 dfktools-0.3.0/src/dfktools/consumable/__init__.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)    12941 2023-05-17 09:17:55.000000 dfktools-0.3.0/src/dfktools/consumable/consumable.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     1068 2023-05-17 06:47:32.000000 dfktools-0.3.0/src/dfktools/consumable_example.py
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-05-27 14:19:42.804727 dfktools-0.3.0/src/dfktools/dex/
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 05:33:06.000000 dfktools-0.3.0/src/dfktools/dex/__init__.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     3084 2023-05-17 09:17:55.000000 dfktools-0.3.0/src/dfktools/dex/crystal.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     5487 2023-05-17 06:28:12.000000 dfktools-0.3.0/src/dfktools/dex/erc1155.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)    34859 2023-05-20 13:02:18.000000 dfktools-0.3.0/src/dfktools/dex/erc20.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)    12438 2023-05-17 09:17:55.000000 dfktools-0.3.0/src/dfktools/dex/item_erc1155.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     3066 2023-05-17 09:17:55.000000 dfktools-0.3.0/src/dfktools/dex/jade.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     3070 2023-05-17 09:17:55.000000 dfktools-0.3.0/src/dfktools/dex/jewel.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)    21910 2023-05-17 06:28:12.000000 dfktools-0.3.0/src/dfktools/dex/master_gardener.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     3572 2023-05-17 06:28:12.000000 dfktools-0.3.0/src/dfktools/dex/uniswap_v2_factory.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)    14189 2023-05-17 09:17:55.000000 dfktools-0.3.0/src/dfktools/dex/uniswap_v2_pair.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)    18811 2023-05-17 09:17:55.000000 dfktools-0.3.0/src/dfktools/dex/uniswap_v2_router.py
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-05-27 14:19:42.804727 dfktools-0.3.0/src/dfktools/dex/utils/
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 05:33:06.000000 dfktools-0.3.0/src/dfktools/dex/utils/__init__.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     1078 2022-07-17 05:33:06.000000 dfktools-0.3.0/src/dfktools/dex/utils/utils.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     4400 2023-05-17 06:49:25.000000 dfktools-0.3.0/src/dfktools/dex_example.py
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-05-27 14:19:42.804727 dfktools-0.3.0/src/dfktools/duel/
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 06:15:15.000000 dfktools-0.3.0/src/dfktools/duel/__init__.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)    44461 2023-05-17 09:17:55.000000 dfktools-0.3.0/src/dfktools/duel/duel.py
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-05-27 14:19:42.808727 dfktools-0.3.0/src/dfktools/duel/utils/
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 06:15:15.000000 dfktools-0.3.0/src/dfktools/duel/utils/__init__.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)      934 2022-09-19 15:24:02.000000 dfktools-0.3.0/src/dfktools/duel/utils/utils.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     1798 2023-05-17 06:47:32.000000 dfktools-0.3.0/src/dfktools/duel_example.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     1066 2022-12-08 09:31:30.000000 dfktools-0.3.0/src/dfktools/erc20_example.py
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-05-27 14:19:42.808727 dfktools-0.3.0/src/dfktools/genes/
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 05:33:06.000000 dfktools-0.3.0/src/dfktools/genes/__init__.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     1828 2023-05-17 06:28:12.000000 dfktools-0.3.0/src/dfktools/genes/gene_science_v1.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     2168 2023-05-17 06:28:11.000000 dfktools-0.3.0/src/dfktools/genes/gene_science_v2.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     1885 2023-01-16 12:58:12.000000 dfktools-0.3.0/src/dfktools/genes_encode_example.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     1423 2022-07-17 11:30:49.000000 dfktools-0.3.0/src/dfktools/genes_example.py
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-05-27 14:19:42.808727 dfktools-0.3.0/src/dfktools/hero/
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 05:33:06.000000 dfktools-0.3.0/src/dfktools/hero/__init__.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)    85130 2023-05-24 13:11:07.000000 dfktools-0.3.0/src/dfktools/hero/hero_core.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     1808 2023-05-20 14:18:48.000000 dfktools-0.3.0/src/dfktools/hero/heroes.py
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-05-27 14:19:42.808727 dfktools-0.3.0/src/dfktools/hero/utils/
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 05:33:06.000000 dfktools-0.3.0/src/dfktools/hero/utils/__init__.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     7937 2023-05-21 13:34:56.000000 dfktools-0.3.0/src/dfktools/hero/utils/utils.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     2222 2023-05-21 13:28:44.000000 dfktools-0.3.0/src/dfktools/hero_example.py
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-05-27 14:19:42.808727 dfktools-0.3.0/src/dfktools/land/
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 05:33:06.000000 dfktools-0.3.0/src/dfktools/land/__init__.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)    16757 2023-05-17 09:17:55.000000 dfktools-0.3.0/src/dfktools/land/land.py
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-05-27 14:19:42.812727 dfktools-0.3.0/src/dfktools/land/utils/
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 05:33:06.000000 dfktools-0.3.0/src/dfktools/land/utils/__init__.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)      347 2022-07-17 05:33:06.000000 dfktools-0.3.0/src/dfktools/land/utils/utils.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     1218 2022-12-08 07:01:50.000000 dfktools-0.3.0/src/dfktools/land_example.py
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-05-27 14:19:42.812727 dfktools-0.3.0/src/dfktools/meditation/
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 05:33:06.000000 dfktools-0.3.0/src/dfktools/meditation/__init__.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)    32044 2023-05-17 09:17:55.000000 dfktools-0.3.0/src/dfktools/meditation/meditation.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     3691 2023-05-17 06:33:36.000000 dfktools-0.3.0/src/dfktools/meditation_example.py
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-05-27 14:19:42.812727 dfktools-0.3.0/src/dfktools/perilous_journey/
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 05:33:06.000000 dfktools-0.3.0/src/dfktools/perilous_journey/__init__.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)    10077 2022-07-17 05:33:06.000000 dfktools-0.3.0/src/dfktools/perilous_journey/perilous_journey.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     3043 2023-05-21 13:28:44.000000 dfktools-0.3.0/src/dfktools/pet_example.py
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-05-27 14:19:42.812727 dfktools-0.3.0/src/dfktools/pets/
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 13:32:00.000000 dfktools-0.3.0/src/dfktools/pets/__init__.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)    13128 2023-05-17 09:17:54.000000 dfktools-0.3.0/src/dfktools/pets/exchange.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)    15150 2023-05-17 09:17:54.000000 dfktools-0.3.0/src/dfktools/pets/hatchery.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)    48917 2023-05-24 13:26:25.000000 dfktools-0.3.0/src/dfktools/pets/pet_core.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     1479 2023-05-20 14:19:35.000000 dfktools-0.3.0/src/dfktools/pets/pets.py
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-05-27 14:19:42.812727 dfktools-0.3.0/src/dfktools/pets/utils/
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 14:45:38.000000 dfktools-0.3.0/src/dfktools/pets/utils/__init__.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     5642 2023-05-20 03:57:10.000000 dfktools-0.3.0/src/dfktools/pets/utils/utils.py
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-05-27 14:19:42.816727 dfktools-0.3.0/src/dfktools/profile/
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 05:33:06.000000 dfktools-0.3.0/src/dfktools/profile/__init__.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     7565 2023-05-17 06:28:12.000000 dfktools-0.3.0/src/dfktools/profile/profile.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)    11703 2023-05-17 06:28:12.000000 dfktools-0.3.0/src/dfktools/profile/profile_v2.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)      821 2023-02-02 10:29:02.000000 dfktools-0.3.0/src/dfktools/profile_example.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     5500 2023-05-25 00:04:40.000000 dfktools-0.3.0/src/dfktools/quest_example.py
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-05-27 14:19:42.820727 dfktools-0.3.0/src/dfktools/quests/
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 05:33:06.000000 dfktools-0.3.0/src/dfktools/quests/__init__.py
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-05-27 14:19:42.820727 dfktools-0.3.0/src/dfktools/quests/professions/
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 05:33:06.000000 dfktools-0.3.0/src/dfktools/quests/professions/__init__.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)      329 2022-12-08 06:24:10.000000 dfktools-0.3.0/src/dfktools/quests/professions/fishing.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)      329 2022-12-08 06:24:41.000000 dfktools-0.3.0/src/dfktools/quests/professions/foraging.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     3345 2022-12-08 07:25:12.000000 dfktools-0.3.0/src/dfktools/quests/professions/gardening.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)      521 2022-12-08 06:25:47.000000 dfktools-0.3.0/src/dfktools/quests/professions/mining.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)    40741 2023-05-17 09:17:55.000000 dfktools-0.3.0/src/dfktools/quests/quest_core_v1.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)    32248 2023-05-17 09:17:55.000000 dfktools-0.3.0/src/dfktools/quests/quest_core_v2.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)    29586 2023-05-24 14:31:32.000000 dfktools-0.3.0/src/dfktools/quests/quest_core_v3.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     2479 2022-07-18 04:06:28.000000 dfktools-0.3.0/src/dfktools/quests/quest_v1.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     2308 2022-09-19 15:00:40.000000 dfktools-0.3.0/src/dfktools/quests/quest_v2.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     2117 2023-05-21 12:28:14.000000 dfktools-0.3.0/src/dfktools/quests/quest_v3.py
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-05-27 14:19:42.824727 dfktools-0.3.0/src/dfktools/quests/training/
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 05:33:06.000000 dfktools-0.3.0/src/dfktools/quests/training/__init__.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)      259 2022-12-08 06:33:57.000000 dfktools-0.3.0/src/dfktools/quests/training/agility_training.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)      260 2022-12-08 06:44:01.000000 dfktools-0.3.0/src/dfktools/quests/training/dexterity_training.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)      260 2022-12-08 06:44:14.000000 dfktools-0.3.0/src/dfktools/quests/training/endurance_training.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)      263 2022-12-08 06:44:28.000000 dfktools-0.3.0/src/dfktools/quests/training/intelligence_training.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)      255 2022-12-08 06:44:45.000000 dfktools-0.3.0/src/dfktools/quests/training/luck_training.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)      260 2022-12-08 06:46:04.000000 dfktools-0.3.0/src/dfktools/quests/training/strength_training.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)      259 2022-12-08 06:45:11.000000 dfktools-0.3.0/src/dfktools/quests/training/vitality_training.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)      257 2022-12-08 06:44:57.000000 dfktools-0.3.0/src/dfktools/quests/training/wisdom_training.py
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-05-27 14:19:42.824727 dfktools-0.3.0/src/dfktools/quests/utils/
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 05:33:06.000000 dfktools-0.3.0/src/dfktools/quests/utils/__init__.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     5519 2023-05-23 22:26:44.000000 dfktools-0.3.0/src/dfktools/quests/utils/utils.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)    15405 2023-05-17 09:17:55.000000 dfktools-0.3.0/src/dfktools/quests/wishing_well.py
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-05-27 14:19:42.824727 dfktools-0.3.0/src/dfktools/raffle/
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 06:27:09.000000 dfktools-0.3.0/src/dfktools/raffle/__init__.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)    21612 2023-05-17 09:17:55.000000 dfktools-0.3.0/src/dfktools/raffle/raffle_master.py
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-05-27 14:19:42.824727 dfktools-0.3.0/src/dfktools/raffle/utils/
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 06:27:09.000000 dfktools-0.3.0/src/dfktools/raffle/utils/__init__.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)      738 2022-07-17 06:27:09.000000 dfktools-0.3.0/src/dfktools/raffle/utils/utils.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     2219 2023-05-17 06:47:32.000000 dfktools-0.3.0/src/dfktools/raffle_example.py
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-05-27 14:19:42.824727 dfktools-0.3.0/src/dfktools/stone_carver/
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-09-02 13:16:15.000000 dfktools-0.3.0/src/dfktools/stone_carver/__init__.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)    12747 2023-05-20 13:34:51.000000 dfktools-0.3.0/src/dfktools/stone_carver/stone_carver.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     1835 2023-05-17 06:47:32.000000 dfktools-0.3.0/src/dfktools/stone_carver_example.py
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-05-27 14:19:42.828727 dfktools-0.3.0/src/dfktools/summoning/
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2022-07-17 05:33:06.000000 dfktools-0.3.0/src/dfktools/summoning/__init__.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)    16129 2023-05-17 09:17:55.000000 dfktools-0.3.0/src/dfktools/summoning/assisting.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)    11172 2023-05-17 09:17:55.000000 dfktools-0.3.0/src/dfktools/summoning/crystals.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)    26787 2023-05-17 09:17:55.000000 dfktools-0.3.0/src/dfktools/summoning/crystals_v2.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)    10930 2023-05-17 09:17:55.000000 dfktools-0.3.0/src/dfktools/summoning/serendale_assisting.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)    26272 2023-05-17 09:17:55.000000 dfktools-0.3.0/src/dfktools/summoning/summoning.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     2934 2023-05-17 06:33:36.000000 dfktools-0.3.0/src/dfktools/summoning_example.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     1411 2023-05-17 06:47:32.000000 dfktools-0.3.0/src/dfktools/wishing_well_quest_example.py
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-05-27 14:19:42.796727 dfktools-0.3.0/src/dfktools.egg-info/
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     9848 2023-05-27 14:19:42.000000 dfktools-0.3.0/src/dfktools.egg-info/PKG-INFO
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     4471 2023-05-27 14:19:42.000000 dfktools-0.3.0/src/dfktools.egg-info/SOURCES.txt
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)        1 2023-05-27 14:19:42.000000 dfktools-0.3.0/src/dfktools.egg-info/dependency_links.txt
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)       60 2023-05-27 14:19:42.000000 dfktools-0.3.0/src/dfktools.egg-info/requires.txt
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)        9 2023-05-27 14:19:42.000000 dfktools-0.3.0/src/dfktools.egg-info/top_level.txt
```

### Comparing `dfktools-0.2.0/LICENSE` & `dfktools-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dfktools-0.2.0/PKG-INFO` & `dfktools-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dfktools
-Version: 0.2.0
+Version: 0.3.0
 Summary: A toolbox for DefiKingdoms
 Home-page: https://github.com/0rtis/dfktools
 Author: Ortis
 Author-email: Ortis <ortis@ortis.io>
 License: MIT License
         
         Copyright (c) 2022 Ortis (ortis@ortis.io)
@@ -40,42 +40,45 @@
 [![GitHub license](https://img.shields.io/github/license/0rtis/dfktools.svg?style=flat-square)](https://github.com/0rtis/dfktools/blob/master/LICENSE)
 [![GitHub stars](https://img.shields.io/github/stars/0rtis?style=flat-square)](https://github.com/0rtis)
 [![Join Discord](https://img.shields.io/discord/932350221256638564?label=discord&style=flat-square)](https://discord.gg/BMWKgZSXqJ)
 [![Join Discord](https://img.shields.io/discord/889216073906405507?label=discord&style=flat-square)](https://discord.gg/JvfPpV7but)
 [![Follow @twitter handle](https://img.shields.io/twitter/follow/Knockturn_io.svg?style=flat-square)](https://twitter.com/intent/follow?screen_name=ortis95)
 
 
-## DefiKingdoms contract
+Install with `pip install dfktools`
+
+https://pypi.org/project/dfktools/
+
+## DefiKingdoms toolbox
 
 This is a simple toolbox to interact with the contracts of [DefiKingdoms](https://defikingdoms.com/)
 
 *This software is not endorsed by, directly affiliated with, maintained, authorized, or sponsored by the DefiKingdoms team.
 All product and company names are the registered trademarks of their original owners.
 The use of any trade name or trademark is for identification and reference purposes only and does not imply any association with the trademark holder of their product brand.*
 
 <br/>
 
 **Like this project ? Consider supporting future developments by:**
 - Delegating AVAX to our Avalanche node **NodeID-4btZGj8TmrycK22kwgBK5wJEFighAFWiZ**
-- Delegating ADA to our [Cardano node [KTA]](https://pooltool.io/pool/991a64a6e3d866f4af4e0a2bfd61c15486a47ccc352e61e8a6b4fef8) **991a64a6e3d866f4af4e0a2bfd61c15486a47ccc352e61e8a6b4fef8**
 - Making a donation to **0xA68fBfa3E0c86D1f3fF071853df6DAe8753095E2**
 
 *Need help ? Join the [GameFi Developers Discord](https://discord.gg/JvfPpV7but)*
 
 ### Code guidelines
 1. Indent with Tab
 2. 1 empty line within a function, 2 empty lines between function
 3. Use *trait(s)* to name any or all of the 8 value `strength, agility, intelligence, wisdom, luck, vitality, endurance, dexterity`
 4. Use *ability(ies)* to name any or all of the 4 value `passive1, passive2, active1, active2`
 5. Use *stat(s)* as a generic term for any or all the characteristics of a hero (traits, abilities, HP, MP, stamina, etc)
 6. A function should support all realms, except if contracts differs across realms
 7. All hardcoded addresses should be [CheckSummed](https://ethsum.netlify.app/)
 8. Use `logging`, not `print`
 9. No other third-party libraries (if really needed, please explain why in the PR)
-10. A short & meaningful comment is superior to a long & unfathomable documentation
+10. A short & meaningful comment is better than a long & unfathomable documentation
 
 <br/>
 
 ### Hero contract
 The hero contract is accessible with [hero/hero.py](src/dfktools/hero/hero.py)
 
 #### Quickstart
```

### Comparing `dfktools-0.2.0/README.md` & `dfktools-0.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -3,42 +3,45 @@
 [![GitHub license](https://img.shields.io/github/license/0rtis/dfktools.svg?style=flat-square)](https://github.com/0rtis/dfktools/blob/master/LICENSE)
 [![GitHub stars](https://img.shields.io/github/stars/0rtis?style=flat-square)](https://github.com/0rtis)
 [![Join Discord](https://img.shields.io/discord/932350221256638564?label=discord&style=flat-square)](https://discord.gg/BMWKgZSXqJ)
 [![Join Discord](https://img.shields.io/discord/889216073906405507?label=discord&style=flat-square)](https://discord.gg/JvfPpV7but)
 [![Follow @twitter handle](https://img.shields.io/twitter/follow/Knockturn_io.svg?style=flat-square)](https://twitter.com/intent/follow?screen_name=ortis95)
 
 
-## DefiKingdoms contract
+Install with `pip install dfktools`
+
+https://pypi.org/project/dfktools/
+
+## DefiKingdoms toolbox
 
 This is a simple toolbox to interact with the contracts of [DefiKingdoms](https://defikingdoms.com/)
 
 *This software is not endorsed by, directly affiliated with, maintained, authorized, or sponsored by the DefiKingdoms team.
 All product and company names are the registered trademarks of their original owners.
 The use of any trade name or trademark is for identification and reference purposes only and does not imply any association with the trademark holder of their product brand.*
 
 <br/>
 
 **Like this project ? Consider supporting future developments by:**
 - Delegating AVAX to our Avalanche node **NodeID-4btZGj8TmrycK22kwgBK5wJEFighAFWiZ**
-- Delegating ADA to our [Cardano node [KTA]](https://pooltool.io/pool/991a64a6e3d866f4af4e0a2bfd61c15486a47ccc352e61e8a6b4fef8) **991a64a6e3d866f4af4e0a2bfd61c15486a47ccc352e61e8a6b4fef8**
 - Making a donation to **0xA68fBfa3E0c86D1f3fF071853df6DAe8753095E2**
 
 *Need help ? Join the [GameFi Developers Discord](https://discord.gg/JvfPpV7but)*
 
 ### Code guidelines
 1. Indent with Tab
 2. 1 empty line within a function, 2 empty lines between function
 3. Use *trait(s)* to name any or all of the 8 value `strength, agility, intelligence, wisdom, luck, vitality, endurance, dexterity`
 4. Use *ability(ies)* to name any or all of the 4 value `passive1, passive2, active1, active2`
 5. Use *stat(s)* as a generic term for any or all the characteristics of a hero (traits, abilities, HP, MP, stamina, etc)
 6. A function should support all realms, except if contracts differs across realms
 7. All hardcoded addresses should be [CheckSummed](https://ethsum.netlify.app/)
 8. Use `logging`, not `print`
 9. No other third-party libraries (if really needed, please explain why in the PR)
-10. A short & meaningful comment is superior to a long & unfathomable documentation
+10. A short & meaningful comment is better than a long & unfathomable documentation
 
 <br/>
 
 ### Hero contract
 The hero contract is accessible with [hero/hero.py](src/dfktools/hero/hero.py)
 
 #### Quickstart
```

### Comparing `dfktools-0.2.0/pyproject.toml` & `dfktools-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["setuptools>=57"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dfktools"
 description = "A toolbox for DefiKingdoms"
 authors = [{name = "Ortis", email = "ortis@ortis.io"}]
-version = "0.2.0"
+version = "0.3.0"
 readme = "README.md"
 keywords = ["blockchain", "web3", "NFT", "etherum", "game"]
 license = {file = "LICENSE"}
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
     "Programming Language :: Python :: 3",
```

### Comparing `dfktools-0.2.0/setup.cfg` & `dfktools-0.3.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dfktools
-version = 0.2.0
+version = 0.3.0
 author = Ortis
 author_email = ortis@ortis.io
 description = A toolbox for DefiKingdoms
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/0rtis/dfktools
 project_urls =
```

### Comparing `dfktools-0.2.0/src/dfktools/airdrop/airdrop.py` & `dfktools-0.3.0/src/dfktools/airdrop/airdrop.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,38 +45,39 @@
     else:
         return str(txid)
 
 
 def view_airdrops(contract_address, user_address, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-    contract = w3.eth.contract(Web3.toChecksumAddress(contract_address), abi=ABI)
+    contract = w3.eth.contract(Web3.to_checksum_address(contract_address), abi=ABI)
 
-    raw = contract.functions.viewAirdrops().call({'from': Web3.toChecksumAddress(user_address)})
+    raw = contract.functions.viewAirdrops().call({'from': Web3.to_checksum_address(user_address)})
     airdrops = []
     for r in raw:
         airdrops.append({'tokenAddress': r[0], 'amount': r[1], 'time': r[2], 'note': r[3]})
     return airdrops
 
 
 def claim_airdrop(contract_address, drop_id, private_key, nonce, gas_price_gwei, tx_timeout_seconds, rpc_address, logger):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
-    account = w3.eth.account.privateKeyToAccount(private_key)
+    account = w3.eth.account.from_key(private_key)
     w3.eth.default_account = account.address
 
-    contract_address = Web3.toChecksumAddress(contract_address)
+    contract_address = Web3.to_checksum_address(contract_address)
     contract = w3.eth.contract(contract_address, abi=ABI)
 
+    tx = contract.functions.claimAirdrop(drop_id)
+
     if isinstance(gas_price_gwei, dict):   # dynamic fee
-        tx = contract.functions.claimAirdrop(drop_id).buildTransaction(
-            {'maxFeePerGas': w3.toWei(gas_price_gwei['maxFeePerGas'], 'gwei'),
-             'maxPriorityFeePerGas': w3.toWei(gas_price_gwei['maxPriorityFeePerGas'], 'gwei'), 'nonce': nonce})
+        tx = tx.build_transaction(
+            {'maxFeePerGas': w3.to_wei(gas_price_gwei['maxFeePerGas'], 'gwei'),
+             'maxPriorityFeePerGas': w3.to_wei(gas_price_gwei['maxPriorityFeePerGas'], 'gwei'), 'nonce': nonce})
     else:   # legacy
-        tx = contract.functions.claimAirdrop(drop_id).buildTransaction(
-            {'gasPrice': w3.toWei(gas_price_gwei, 'gwei'), 'nonce': nonce})
+        tx = tx.build_transaction({'gasPrice': w3.to_wei(gas_price_gwei, 'gwei'), 'nonce': nonce})
 
     logger.debug("Signing transaction")
     signed_tx = w3.eth.account.sign_transaction(tx, private_key=private_key)
     logger.debug("Sending transaction " + str(tx))
     ret = w3.eth.send_raw_transaction(signed_tx.rawTransaction)
     logger.debug("Transaction successfully sent !")
     logger.info(
```

### Comparing `dfktools-0.2.0/src/dfktools/airdrop_example.py` & `dfktools-0.3.0/src/dfktools/airdrop_example.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,12 +20,12 @@
     for airdrop in airdrops:
         airdrop["tokenName"] = erc20.address2item(airdrop["tokenAddress"], 'serendale')[2]
     logger.info(airdrops)
 
     # Claim Airdrop
     w3 = Web3(Web3.HTTPProvider(rpc_server))
     private_key = None  # set private key
-    account_address = w3.eth.account.privateKeyToAccount(private_key).address
+    account_address = w3.eth.account.from_key(private_key).address
     gas_price_gwei = 100
     tx_timeout_seconds = 30
     airdrop_id = 0  # Use index from view_airdrops list
-    airdrop.claim_airdrop(airdrop.SERENDALE_CONTRACT_ADDRESS, airdrop_id, private_key, w3.eth.getTransactionCount(account_address), gas_price_gwei, tx_timeout_seconds, rpc_server, logger)
+    airdrop.claim_airdrop(airdrop.SERENDALE_CONTRACT_ADDRESS, airdrop_id, private_key, w3.eth.get_transaction_count(account_address), gas_price_gwei, tx_timeout_seconds, rpc_server, logger)
```

### Comparing `dfktools-0.2.0/src/dfktools/alchemist/alchemist.py` & `dfktools-0.3.0/src/dfktools/alchemist/alchemist.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,27 +46,28 @@
 		return 'https://subnets.avax.network/defi-kingdoms/dfk-chain/explorer/tx/' + str(txid)
 	else:
 		return str(txid)
 
 
 def create_potion(contract_address, potion_address, quantity, private_key, nonce, gas_price_gwei, tx_timeout_seconds, rpc_address, logger):
 	w3 = Web3(Web3.HTTPProvider(rpc_address))
-	account = w3.eth.account.privateKeyToAccount(private_key)
+	account = w3.eth.account.from_key(private_key)
 	w3.eth.default_account = account.address
 
-	contract_address = Web3.toChecksumAddress(contract_address)
+	contract_address = Web3.to_checksum_address(contract_address)
 	contract = w3.eth.contract(contract_address, abi=ABI)
 
+	tx = contract.functions.createPotion(potion_address, quantity)
+
 	if isinstance(gas_price_gwei, dict):  # dynamic fee
-		tx = contract.functions.createPotion(potion_address, quantity).buildTransaction(
-			{'maxFeePerGas': w3.toWei(gas_price_gwei['maxFeePerGas'], 'gwei'),
-			 'maxPriorityFeePerGas': w3.toWei(gas_price_gwei['maxPriorityFeePerGas'], 'gwei'), 'nonce': nonce})
+		tx = tx.build_transaction(
+			{'maxFeePerGas': w3.to_wei(gas_price_gwei['maxFeePerGas'], 'gwei'),
+			 'maxPriorityFeePerGas': w3.to_wei(gas_price_gwei['maxPriorityFeePerGas'], 'gwei'), 'nonce': nonce})
 	else:  # legacy
-		tx = contract.functions.createPotion(potion_address, quantity).buildTransaction(
-			{'gasPrice': w3.toWei(gas_price_gwei, 'gwei'), 'nonce': nonce})
+		tx = tx.build_transaction({'gasPrice': w3.to_wei(gas_price_gwei, 'gwei'), 'nonce': nonce})
 
 	logger.debug("Signing transaction")
 	signed_tx = w3.eth.account.sign_transaction(tx, private_key=private_key)
 	logger.debug("Sending transaction " + str(tx))
 	ret = w3.eth.send_raw_transaction(signed_tx.rawTransaction)
 	logger.debug("Transaction successfully sent !")
 	logger.info(
@@ -78,44 +79,44 @@
 
 	return tx_receipt
 
 
 def address_to_potion_id(contract_address, potion_address, rpc_address):
 	w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-	contract_address = Web3.toChecksumAddress(contract_address)
+	contract_address = Web3.to_checksum_address(contract_address)
 	contract = w3.eth.contract(contract_address, abi=ABI)
 
 	return contract.functions.addressToPotionId(potion_address).call()
 
 
 def potion_id_to_address_amount(contract_address, uint256, rpc_address):
 	w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-	contract_address = Web3.toChecksumAddress(contract_address)
+	contract_address = Web3.to_checksum_address(contract_address)
 	contract = w3.eth.contract(contract_address, abi=ABI)
 
 	raw = contract.functions.potions(uint256).call()
 	return {'address': raw[0], 'batchSize': raw[1]}
 
 
 def get_potion(contract_address, potion_address, rpc_address):
 	w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-	contract_address = Web3.toChecksumAddress(contract_address)
+	contract_address = Web3.to_checksum_address(contract_address)
 	contract = w3.eth.contract(contract_address, abi=ABI)
 
 	raw = contract.functions.getPotion(potion_address).call()
 	return {'address': raw[0], 'ingredientAddresses': raw[1], 'ingredientQuantities': raw[2], 'batchSize': raw[3]}
 
 
 def get_potions(contract_address, rpc_address):
 	w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-	contract_address = Web3.toChecksumAddress(contract_address)
+	contract_address = Web3.to_checksum_address(contract_address)
 	contract = w3.eth.contract(contract_address, abi=ABI)
 
 	raw = contract.functions.getPotions().call()
 	potions = []
 	for r in raw:
 		potions.append({'address': r[0], 'ingredientAddresses': r[1], 'ingredientQuantities': r[2], 'batchSize': r[3]})
```

### Comparing `dfktools-0.2.0/src/dfktools/alchemist_example.py` & `dfktools-0.3.0/src/dfktools/alchemist_example.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,11 +33,11 @@
     # potion id to address and batch size
     potion_addr_batch = alchemist.potion_id_to_address_amount(realm_contract, 1, rpc_server)
     logger.info("Potion id to address & batch size: " + str(potion_addr_batch))
 
     # crafting Stamina Vial
     w3 = Web3(Web3.HTTPProvider(rpc_server))
     private_key = None  # set private key
-    account_address = w3.eth.account.privateKeyToAccount(private_key).address
+    account_address = w3.eth.account.from_key(private_key).address
     gas_price_gwei = 40
     tx_timeout_seconds = 30
-    alchemist.create_potion(realm_contract, stamina_vial_address, 1, private_key, w3.eth.getTransactionCount(account_address), gas_price_gwei, tx_timeout_seconds, rpc_server, logger)
+    alchemist.create_potion(realm_contract, stamina_vial_address, 1, private_key, w3.eth.get_transaction_count(account_address), gas_price_gwei, tx_timeout_seconds, rpc_server, logger)
```

### Comparing `dfktools-0.2.0/src/dfktools/assisting_example.py` & `dfktools-0.3.0/src/dfktools/assisting_example.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.2.0/src/dfktools/auction_example.py` & `dfktools-0.3.0/src/dfktools/auction_example.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,24 +36,24 @@
     logger.info("Hero rental auctions:")
     auctions = hero_rental.get_open_auctions(graphql, 0, 10)
     for auction in auctions:
         logger.info(str(auction))
 
     #w3 = Web3(Web3.HTTPProvider(rpc_server))
     #private_key = ""  # set private key
-    #account_address = w3.eth.account.privateKeyToAccount(private_key).address
+    #account_address = w3.eth.account.from_key(private_key).address
 
     # serendale hero auction
     #logger.info(hero_sales.get_auction(hero_sales.SERENDALE_CONTRACT_ADDRESS, 181373, 'https://api.harmony.one'))
-    # hero_sales.bid_hero(hero_sales.SERENDALE_CONTRACT_ADDRESS, 181373, hero_sales.ether2wei(100), private_key, 'w3.eth.getTransactionCount(account_address), 50, 30)
+    # hero_sales.bid_hero(hero_sales.SERENDALE_CONTRACT_ADDRESS, 181373, hero_sales.ether2wei(100), private_key, 'w3.eth.get_transaction_count(account_address), 50, 30)
 
     # crystalvale hero auction
     #cv_hero_auctions = Auction(hero_sales.CRYSTALVALE_CONTRACT_ADDRESS, 'https://subnets.avax.network/defi-kingdoms/dfk-chain/rpc', logger)
     #logger.info(auction_utils.human_readable_auction(cv_hero_auctions.get_auction(hero_utils.sd2cv_cv_hero_id(250))))
-    # cv_hero_auctions.bid_hero(hero_utils.sd2cv_cv_hero_id(250), hero_sales.ether2wei(100), private_key, w3.eth.getTransactionCount(account_address), 50, 30)
+    # cv_hero_auctions.bid_hero(hero_utils.sd2cv_cv_hero_id(250), hero_sales.ether2wei(100), private_key, w3.eth.get_transaction_count(account_address), 50, 30)
 
     logger.info("\n")
 
     # lands
     user = '0x2E7669F61eA77F02445A015FBdcFe2DE47083E02'
 
     land_auction = Auction(realm_land_auction_contract, rpc_server, logger)
```

### Comparing `dfktools-0.2.0/src/dfktools/auctions/auction.py` & `dfktools-0.3.0/src/dfktools/auctions/auction.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.2.0/src/dfktools/auctions/auction_core.py` & `dfktools-0.3.0/src/dfktools/auctions/auction_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import requests
 from web3 import Web3
 
 ABI = """
     [
         {"anonymous":false,"inputs":[{"indexed":false,"internalType":"uint256","name":"auctionId","type":"uint256"},{"indexed":true,"internalType":"uint256","name":"tokenId","type":"uint256"}],"name":"AuctionCancelled","type":"event"},
         {"anonymous":false,"inputs":[{"indexed":false,"internalType":"uint256","name":"auctionId","type":"uint256"},{"indexed":true,"internalType":"address","name":"owner","type":"address"},{"indexed":true,"internalType":"uint256","name":"tokenId","type":"uint256"},{"indexed":false,"internalType":"uint256","name":"startingPrice","type":"uint256"},{"indexed":false,"internalType":"uint256","name":"endingPrice","type":"uint256"},{"indexed":false,"internalType":"uint256","name":"duration","type":"uint256"},{"indexed":false,"internalType":"address","name":"winner","type":"address"}],"name":"AuctionCreated","type":"event"},
         {"anonymous":false,"inputs":[{"indexed":false,"internalType":"uint256","name":"auctionId","type":"uint256"},{"indexed":true,"internalType":"uint256","name":"tokenId","type":"uint256"},{"indexed":false,"internalType":"uint256","name":"totalPrice","type":"uint256"},{"indexed":false,"internalType":"address","name":"winner","type":"address"}],"name":"AuctionSuccessful","type":"event"},
@@ -52,28 +51,28 @@
 
 def block_explorer_link(txid):
     return 'https://explorer.harmony.one/tx/' + str(txid) + ' or https://subnets.avax.network/defi-kingdoms/dfk-chain/explorer/tx/' + str(txid)
 
 
 def bid(auction_contract_address, token_id, bid_amount_wei, private_key, nonce, gas_price_gwei, tx_timeout_seconds, rpc_address, logger):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
-    account = w3.eth.account.privateKeyToAccount(private_key)
+    account = w3.eth.account.from_key(private_key)
     w3.eth.default_account = account.address
 
-    auction_contract_address = Web3.toChecksumAddress(auction_contract_address)
+    auction_contract_address = Web3.to_checksum_address(auction_contract_address)
     contract = w3.eth.contract(auction_contract_address, abi=ABI)
 
     tx = contract.functions.bid(token_id, bid_amount_wei)
 
     if isinstance(gas_price_gwei, dict):   # dynamic fee
-        tx = tx.buildTransaction(
-            {'maxFeePerGas': w3.toWei(gas_price_gwei['maxFeePerGas'], 'gwei'),
-             'maxPriorityFeePerGas': w3.toWei(gas_price_gwei['maxPriorityFeePerGas'], 'gwei'), 'nonce': nonce})
+        tx = tx.build_transaction(
+            {'maxFeePerGas': w3.to_wei(gas_price_gwei['maxFeePerGas'], 'gwei'),
+             'maxPriorityFeePerGas': w3.to_wei(gas_price_gwei['maxPriorityFeePerGas'], 'gwei'), 'nonce': nonce})
     else:   # legacy
-        tx = tx.buildTransaction({'gasPrice': w3.toWei(gas_price_gwei, 'gwei'), 'nonce': nonce})
+        tx = tx.build_transaction({'gasPrice': w3.to_wei(gas_price_gwei, 'gwei'), 'nonce': nonce})
 
     logger.info("Signing transaction")
     signed_tx = w3.eth.account.sign_transaction(tx, private_key=private_key)
     logger.info("Sending transaction " + str(tx))
     ret = w3.eth.send_raw_transaction(signed_tx.rawTransaction)
     logger.info("Transaction successfully sent !")
     logger.info("Waiting for transaction " + block_explorer_link(signed_tx.hash.hex()) + " to be mined")
@@ -81,22 +80,22 @@
                                                      poll_latency=2)
     logger.info("Transaction mined !")
     logger.info(str(tx_receipt))
 
 
 def create_auction(auction_address, token_id, starting_price_wei, ending_price_wei, duration, winner, private_key, nonce, gas_price_gwei, tx_timeout_seconds, rpc_address, logger):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
-    account = w3.eth.account.privateKeyToAccount(private_key)
+    account = w3.eth.account.from_key(private_key)
     w3.eth.default_account = account.address
 
-    auction_contract_address = Web3.toChecksumAddress(auction_address)
+    auction_contract_address = Web3.to_checksum_address(auction_address)
     auction_contract = w3.eth.contract(auction_contract_address, abi=ABI)
 
-    tx = auction_contract.functions.createAuction(token_id, starting_price_wei, ending_price_wei, duration, winner).buildTransaction(
-        {'gasPrice': w3.toWei(gas_price_gwei, 'gwei'), 'nonce': nonce})
+    tx = auction_contract.functions.createAuction(token_id, starting_price_wei, ending_price_wei, duration, winner).build_transaction(
+        {'gasPrice': w3.to_wei(gas_price_gwei, 'gwei'), 'nonce': nonce})
 
     logger.info("Signing transaction")
     signed_tx = w3.eth.account.sign_transaction(tx, private_key=private_key)
     logger.info("Sending transaction " + str(tx))
     ret = w3.eth.send_raw_transaction(signed_tx.rawTransaction)
     logger.info("Transaction successfully sent !")
     logger.info("Waiting for transaction " + block_explorer_link(signed_tx.hash.hex()) + " to be mined")
@@ -104,22 +103,22 @@
                                                      poll_latency=2)
     logger.info("Transaction mined !")
     logger.info(str(tx_receipt))
 
 
 def cancel_auction(auction_address, token_id, private_key, nonce, gas_price_gwei, tx_timeout_seconds, rpc_address, logger):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
-    account = w3.eth.account.privateKeyToAccount(private_key)
+    account = w3.eth.account.from_key(private_key)
     w3.eth.default_account = account.address
 
-    auction_contract_address = Web3.toChecksumAddress(auction_address)
+    auction_contract_address = Web3.to_checksum_address(auction_address)
     auction_contract = w3.eth.contract(auction_contract_address, abi=ABI)
 
-    tx = auction_contract.functions.cancelAuction(token_id).buildTransaction(
-        {'gasPrice': w3.toWei(gas_price_gwei, 'gwei'), 'nonce': nonce})
+    tx = auction_contract.functions.cancelAuction(token_id).build_transaction(
+        {'gasPrice': w3.to_wei(gas_price_gwei, 'gwei'), 'nonce': nonce})
 
     logger.info("Signing transaction")
     signed_tx = w3.eth.account.sign_transaction(tx, private_key=private_key)
     logger.info("Sending transaction " + str(tx))
     ret = w3.eth.send_raw_transaction(signed_tx.rawTransaction)
     logger.info("Transaction successfully sent !")
     logger.info("Waiting for transaction " + block_explorer_link(signed_tx.hash.hex()) + " to be mined")
@@ -128,51 +127,51 @@
     logger.info("Transaction mined !")
     logger.info(str(tx_receipt))
 
 
 def is_on_auction(auction_address, token_id, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-    auction_contract_address = Web3.toChecksumAddress(auction_address)
+    auction_contract_address = Web3.to_checksum_address(auction_address)
     auction_contract = w3.eth.contract(auction_contract_address, abi=ABI)
     return auction_contract.functions.isOnAuction(token_id).call()
 
 
 def get_auction(auction_address, token_id, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-    auction_contract_address = Web3.toChecksumAddress(auction_address)
+    auction_contract_address = Web3.to_checksum_address(auction_address)
     auction_contract = w3.eth.contract(auction_contract_address, abi=ABI)
     return auction_contract.functions.getAuction(token_id).call()
 
 
 def get_auctions(auction_address, token_ids, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-    auction_contract_address = Web3.toChecksumAddress(auction_address)
+    auction_contract_address = Web3.to_checksum_address(auction_address)
     auction_contract = w3.eth.contract(auction_contract_address, abi=ABI)
     return auction_contract.functions.getAuctions(token_ids).call()
 
 
 def total_auctions(auction_address, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-    auction_contract_address = Web3.toChecksumAddress(auction_address)
+    auction_contract_address = Web3.to_checksum_address(auction_address)
     auction_contract = w3.eth.contract(auction_contract_address, abi=ABI)
     return auction_contract.functions.totalAuctions().call()
 
 
 def get_user_auctions(auction_address, user, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-    auction_contract_address = Web3.toChecksumAddress(auction_address)
+    auction_contract_address = Web3.to_checksum_address(auction_address)
     auction_contract = w3.eth.contract(auction_contract_address, abi=ABI)
-    return auction_contract.functions.getUserAuctions(Web3.toChecksumAddress(user)).call()
+    return auction_contract.functions.getUserAuctions(Web3.to_checksum_address(user)).call()
 
 
 def auctions(auction_address, index, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-    auction_contract_address = Web3.toChecksumAddress(auction_address)
+    auction_contract_address = Web3.to_checksum_address(auction_address)
     auction_contract = w3.eth.contract(auction_contract_address, abi=ABI)
     return auction_contract.functions.auctions(index).call()
```

### Comparing `dfktools-0.2.0/src/dfktools/auctions/hero/rent_auctions.py` & `dfktools-0.3.0/src/dfktools/auctions/hero/rent_auctions.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.2.0/src/dfktools/auctions/hero/sale_auctions.py` & `dfktools-0.3.0/src/dfktools/auctions/hero/sale_auctions.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,170 +3,188 @@
 
 SERENDALE_CONTRACT_ADDRESS = '0x13a65B9F8039E2c032Bc022171Dc05B30c3f2892'
 CRYSTALVALE_CONTRACT_ADDRESS = '0xc390fAA4C7f66E4D62E59C231D5beD32Ff77BEf0'
 SERENDALE2_CONTRACT_ADDRESS = '0x7F2B66DB2D02f642a9eb8d13Bc998d441DDe17A8'
 
 
 ABI = """
-        [
-            {"inputs":[{"internalType":"address","name":"_heroCoreAddress","type":"address"},{"internalType":"address","name":"_geneScienceAddress","type":"address"},{"internalType":"address","name":"_jewelTokenAddress","type":"address"},{"internalType":"address","name":"_gaiaTearsAddress","type":"address"},{"internalType":"address","name":"_statScienceAddress","type":"address"},{"internalType":"uint256","name":"_cut","type":"uint256"}],"stateMutability":"nonpayable","type":"constructor"},
-            {"anonymous":false,"inputs":[{"indexed":false,"internalType":"uint256","name":"auctionId","type":"uint256"},{"indexed":true,"internalType":"uint256","name":"tokenId","type":"uint256"}],"name":"AuctionCancelled","type":"event"},
-            {"anonymous":false,"inputs":[{"indexed":false,"internalType":"uint256","name":"auctionId","type":"uint256"},{"indexed":true,"internalType":"address","name":"owner","type":"address"},{"indexed":true,"internalType":"uint256","name":"tokenId","type":"uint256"},{"indexed":false,"internalType":"uint256","name":"startingPrice","type":"uint256"},{"indexed":false,"internalType":"uint256","name":"endingPrice","type":"uint256"},{"indexed":false,"internalType":"uint256","name":"duration","type":"uint256"},{"indexed":false,"internalType":"address","name":"winner","type":"address"}],"name":"AuctionCreated","type":"event"},
-            {"anonymous":false,"inputs":[{"indexed":false,"internalType":"uint256","name":"auctionId","type":"uint256"},{"indexed":true,"internalType":"uint256","name":"tokenId","type":"uint256"},{"indexed":false,"internalType":"uint256","name":"totalPrice","type":"uint256"},{"indexed":false,"internalType":"address","name":"winner","type":"address"}],"name":"AuctionSuccessful","type":"event"},
-            {"anonymous":false,"inputs":[{"indexed":true,"internalType":"address","name":"owner","type":"address"},{"indexed":false,"internalType":"uint256","name":"crystalId","type":"uint256"},{"indexed":false,"internalType":"uint256","name":"heroId","type":"uint256"}],"name":"CrystalOpen","type":"event"},
-            {"anonymous":false,"inputs":[{"indexed":false,"internalType":"uint256","name":"crystalId","type":"uint256"},{"indexed":true,"internalType":"address","name":"owner","type":"address"},{"indexed":false,"internalType":"uint256","name":"summonerId","type":"uint256"},{"indexed":false,"internalType":"uint256","name":"assistantId","type":"uint256"},{"indexed":false,"internalType":"uint16","name":"generation","type":"uint16"},{"indexed":false,"internalType":"uint256","name":"createdBlock","type":"uint256"},{"indexed":false,"internalType":"uint8","name":"summonerTears","type":"uint8"},{"indexed":false,"internalType":"uint8","name":"assistantTears","type":"uint8"},{"indexed":false,"internalType":"address","name":"bonusItem","type":"address"}],"name":"CrystalSummoned","type":"event"},
-            {"anonymous":false,"inputs":[{"indexed":true,"internalType":"address","name":"previousOwner","type":"address"},{"indexed":true,"internalType":"address","name":"newOwner","type":"address"}],"name":"OwnershipTransferred","type":"event"},
-            {"anonymous":false,"inputs":[{"indexed":false,"internalType":"address","name":"account","type":"address"}],"name":"Paused","type":"event"},
-            {"anonymous":false,"inputs":[{"indexed":true,"internalType":"bytes32","name":"role","type":"bytes32"},{"indexed":true,"internalType":"bytes32","name":"previousAdminRole","type":"bytes32"},{"indexed":true,"internalType":"bytes32","name":"newAdminRole","type":"bytes32"}],"name":"RoleAdminChanged","type":"event"},
-            {"anonymous":false,"inputs":[{"indexed":true,"internalType":"bytes32","name":"role","type":"bytes32"},{"indexed":true,"internalType":"address","name":"account","type":"address"},{"indexed":true,"internalType":"address","name":"sender","type":"address"}],"name":"RoleGranted","type":"event"},
-            {"anonymous":false,"inputs":[{"indexed":true,"internalType":"bytes32","name":"role","type":"bytes32"},{"indexed":true,"internalType":"address","name":"account","type":"address"},{"indexed":true,"internalType":"address","name":"sender","type":"address"}],"name":"RoleRevoked","type":"event"},
-            {"anonymous":false,"inputs":[{"indexed":false,"internalType":"address","name":"account","type":"address"}],"name":"Unpaused","type":"event"},
-            {"inputs":[],"name":"DEFAULT_ADMIN_ROLE","outputs":[{"internalType":"bytes32","name":"","type":"bytes32"}],"stateMutability":"view","type":"function"},
-            {"inputs":[],"name":"MODERATOR_ROLE","outputs":[{"internalType":"bytes32","name":"","type":"bytes32"}],"stateMutability":"view","type":"function"},
-            {"inputs":[],"name":"auctionHeroCore","outputs":[{"internalType":"contract IHeroCore","name":"","type":"address"}],"stateMutability":"view","type":"function"},
-            {"inputs":[],"name":"baseCooldown","outputs":[{"internalType":"uint256","name":"","type":"uint256"}],"stateMutability":"view","type":"function"},
-            {"inputs":[],"name":"baseSummonFee","outputs":[{"internalType":"uint256","name":"","type":"uint256"}],"stateMutability":"view","type":"function"},
-            {"inputs":[{"internalType":"uint256","name":"_tokenId","type":"uint256"},{"internalType":"uint256","name":"_bidAmount","type":"uint256"}],"name":"bid","outputs":[],"stateMutability":"nonpayable","type":"function"},
-            {"inputs":[{"components":[{"internalType":"uint256","name":"id","type":"uint256"},{"components":[{"internalType":"uint256","name":"summonedTime","type":"uint256"},{"internalType":"uint256","name":"nextSummonTime","type":"uint256"},{"internalType":"uint256","name":"summonerId","type":"uint256"},{"internalType":"uint256","name":"assistantId","type":"uint256"},{"internalType":"uint32","name":"summons","type":"uint32"},{"internalType":"uint32","name":"maxSummons","type":"uint32"}],"internalType":"struct IHeroTypes.SummoningInfo","name":"summoningInfo","type":"tuple"},{"components":[{"internalType":"uint256","name":"statGenes","type":"uint256"},{"internalType":"uint256","name":"visualGenes","type":"uint256"},{"internalType":"enum IHeroTypes.Rarity","name":"rarity","type":"uint8"},{"internalType":"bool","name":"shiny","type":"bool"},{"internalType":"uint16","name":"generation","type":"uint16"},{"internalType":"uint32","name":"firstName","type":"uint32"},{"internalType":"uint32","name":"lastName","type":"uint32"},{"internalType":"uint8","name":"shinyStyle","type":"uint8"},{"internalType":"uint8","name":"class","type":"uint8"},{"internalType":"uint8","name":"subClass","type":"uint8"}],"internalType":"struct IHeroTypes.HeroInfo","name":"info","type":"tuple"},{"components":[{"internalType":"uint256","name":"staminaFullAt","type":"uint256"},{"internalType":"uint256","name":"hpFullAt","type":"uint256"},{"internalType":"uint256","name":"mpFullAt","type":"uint256"},{"internalType":"uint16","name":"level","type":"uint16"},{"internalType":"uint64","name":"xp","type":"uint64"},{"internalType":"address","name":"currentQuest","type":"address"},{"internalType":"uint8","name":"sp","type":"uint8"},{"internalType":"enum IHeroTypes.HeroStatus","name":"status","type":"uint8"}],"internalType":"struct IHeroTypes.HeroState","name":"state","type":"tuple"},{"components":[{"internalType":"uint16","name":"strength","type":"uint16"},{"internalType":"uint16","name":"intelligence","type":"uint16"},{"internalType":"uint16","name":"wisdom","type":"uint16"},{"internalType":"uint16","name":"luck","type":"uint16"},{"internalType":"uint16","name":"agility","type":"uint16"},{"internalType":"uint16","name":"vitality","type":"uint16"},{"internalType":"uint16","name":"endurance","type":"uint16"},{"internalType":"uint16","name":"dexterity","type":"uint16"},{"internalType":"uint16","name":"hp","type":"uint16"},{"internalType":"uint16","name":"mp","type":"uint16"},{"internalType":"uint16","name":"stamina","type":"uint16"}],"internalType":"struct IHeroTypes.HeroStats","name":"stats","type":"tuple"},{"components":[{"internalType":"uint16","name":"strength","type":"uint16"},{"internalType":"uint16","name":"intelligence","type":"uint16"},{"internalType":"uint16","name":"wisdom","type":"uint16"},{"internalType":"uint16","name":"luck","type":"uint16"},{"internalType":"uint16","name":"agility","type":"uint16"},{"internalType":"uint16","name":"vitality","type":"uint16"},{"internalType":"uint16","name":"endurance","type":"uint16"},{"internalType":"uint16","name":"dexterity","type":"uint16"},{"internalType":"uint16","name":"hpSm","type":"uint16"},{"internalType":"uint16","name":"hpRg","type":"uint16"},{"internalType":"uint16","name":"hpLg","type":"uint16"},{"internalType":"uint16","name":"mpSm","type":"uint16"},{"internalType":"uint16","name":"mpRg","type":"uint16"},{"internalType":"uint16","name":"mpLg","type":"uint16"}],"internalType":"struct IHeroTypes.HeroStatGrowth","name":"primaryStatGrowth","type":"tuple"},{"components":[{"internalType":"uint16","name":"strength","type":"uint16"},{"internalType":"uint16","name":"intelligence","type":"uint16"},{"internalType":"uint16","name":"wisdom","type":"uint16"},{"internalType":"uint16","name":"luck","type":"uint16"},{"internalType":"uint16","name":"agility","type":"uint16"},{"internalType":"uint16","name":"vitality","type":"uint16"},{"internalType":"uint16","name":"endurance","type":"uint16"},{"internalType":"uint16","name":"dexterity","type":"uint16"},{"internalType":"uint16","name":"hpSm","type":"uint16"},{"internalType":"uint16","name":"hpRg","type":"uint16"},{"internalType":"uint16","name":"hpLg","type":"uint16"},{"internalType":"uint16","name":"mpSm","type":"uint16"},{"internalType":"uint16","name":"mpRg","type":"uint16"},{"internalType":"uint16","name":"mpLg","type":"uint16"}],"internalType":"struct IHeroTypes.HeroStatGrowth","name":"secondaryStatGrowth","type":"tuple"},{"components":[{"internalType":"uint16","name":"mining","type":"uint16"},{"internalType":"uint16","name":"gardening","type":"uint16"},{"internalType":"uint16","name":"foraging","type":"uint16"},{"internalType":"uint16","name":"fishing","type":"uint16"}],"internalType":"struct IHeroTypes.HeroProfessions","name":"professions","type":"tuple"}],"internalType":"struct IHeroTypes.Hero","name":"_hero","type":"tuple"}],"name":"calculateSummoningCost","outputs":[{"internalType":"uint256","name":"","type":"uint256"}],"stateMutability":"view","type":"function"},
-            {"inputs":[{"internalType":"uint256","name":"_tokenId","type":"uint256"}],"name":"cancelAuction","outputs":[],"stateMutability":"nonpayable","type":"function"},
-            {"inputs":[{"internalType":"uint256","name":"_tokenId","type":"uint256"}],"name":"cancelAuctionWhenPaused","outputs":[],"stateMutability":"nonpayable","type":"function"},
-            {"inputs":[],"name":"cooldownPerGen","outputs":[{"internalType":"uint256","name":"","type":"uint256"}],"stateMutability":"view","type":"function"},
-            {"inputs":[{"internalType":"uint256","name":"_tokenId","type":"uint256"},{"internalType":"uint128","name":"_startingPrice","type":"uint128"},{"internalType":"uint128","name":"_endingPrice","type":"uint128"},{"internalType":"uint64","name":"_duration","type":"uint64"},{"internalType":"address","name":"_winner","type":"address"}],"name":"createAuction","outputs":[],"stateMutability":"nonpayable","type":"function"},
-            {"inputs":[{"internalType":"uint256","name":"","type":"uint256"}],"name":"crystals","outputs":[{"internalType":"address","name":"owner","type":"address"},{"internalType":"uint256","name":"summonerId","type":"uint256"},{"internalType":"uint256","name":"assistantId","type":"uint256"},{"internalType":"uint16","name":"generation","type":"uint16"},{"internalType":"uint256","name":"createdBlock","type":"uint256"},{"internalType":"uint256","name":"heroId","type":"uint256"},{"internalType":"uint8","name":"summonerTears","type":"uint8"},{"internalType":"uint8","name":"assistantTears","type":"uint8"},{"internalType":"address","name":"bonusItem","type":"address"},{"internalType":"uint32","name":"maxSummons","type":"uint32"},{"internalType":"uint32","name":"firstName","type":"uint32"},{"internalType":"uint32","name":"lastName","type":"uint32"},{"internalType":"uint8","name":"shinyStyle","type":"uint8"}],"stateMutability":"view","type":"function"},
-            {"inputs":[{"internalType":"uint256","name":"_rarityRoll","type":"uint256"},{"internalType":"uint256","name":"_rarityMod","type":"uint256"}],"name":"determineRarity","outputs":[{"internalType":"enum IHeroTypes.Rarity","name":"","type":"uint8"}],"stateMutability":"pure","type":"function"},
-            {"inputs":[],"name":"enabled","outputs":[{"internalType":"bool","name":"","type":"bool"}],"stateMutability":"view","type":"function"},
-            {"inputs":[{"internalType":"uint256","name":"randomNumber","type":"uint256"},{"internalType":"uint256","name":"digits","type":"uint256"},{"internalType":"uint256","name":"offset","type":"uint256"}],"name":"extractNumber","outputs":[{"internalType":"uint256","name":"result","type":"uint256"}],"stateMutability":"pure","type":"function"},
-            {"inputs":[{"internalType":"uint256","name":"_tokenId","type":"uint256"}],"name":"getAuction","outputs":[{"internalType":"uint256","name":"auctionId","type":"uint256"},{"internalType":"address","name":"seller","type":"address"},{"internalType":"uint256","name":"startingPrice","type":"uint256"},{"internalType":"uint256","name":"endingPrice","type":"uint256"},{"internalType":"uint256","name":"duration","type":"uint256"},{"internalType":"uint256","name":"startedAt","type":"uint256"}],"stateMutability":"view","type":"function"},
-            {"inputs":[{"internalType":"uint256","name":"_crystalId","type":"uint256"}],"name":"getCrystal","outputs":[{"components":[{"internalType":"address","name":"owner","type":"address"},{"internalType":"uint256","name":"summonerId","type":"uint256"},{"internalType":"uint256","name":"assistantId","type":"uint256"},{"internalType":"uint16","name":"generation","type":"uint16"},{"internalType":"uint256","name":"createdBlock","type":"uint256"},{"internalType":"uint256","name":"heroId","type":"uint256"},{"internalType":"uint8","name":"summonerTears","type":"uint8"},{"internalType":"uint8","name":"assistantTears","type":"uint8"},{"internalType":"address","name":"bonusItem","type":"address"},{"internalType":"uint32","name":"maxSummons","type":"uint32"},{"internalType":"uint32","name":"firstName","type":"uint32"},{"internalType":"uint32","name":"lastName","type":"uint32"},{"internalType":"uint8","name":"shinyStyle","type":"uint8"}],"internalType":"struct ICrystalTypes.HeroCrystal","name":"","type":"tuple"}],"stateMutability":"view","type":"function"},
-            {"inputs":[{"internalType":"uint256","name":"_tokenId","type":"uint256"}],"name":"getCurrentPrice","outputs":[{"internalType":"uint256","name":"","type":"uint256"}],"stateMutability":"view","type":"function"},
-            {"inputs":[{"internalType":"bytes32","name":"role","type":"bytes32"}],"name":"getRoleAdmin","outputs":[{"internalType":"bytes32","name":"","type":"bytes32"}],"stateMutability":"view","type":"function"},
-            {"inputs":[{"internalType":"address","name":"_address","type":"address"}],"name":"getUserAuctions","outputs":[{"internalType":"uint256[]","name":"","type":"uint256[]"}],"stateMutability":"view","type":"function"},
-            {"inputs":[{"internalType":"address","name":"_address","type":"address"}],"name":"getUserCrystals","outputs":[{"internalType":"uint256[]","name":"","type":"uint256[]"}],"stateMutability":"view","type":"function"},
-            {"inputs":[{"internalType":"bytes32","name":"role","type":"bytes32"},{"internalType":"address","name":"account","type":"address"}],"name":"grantRole","outputs":[],"stateMutability":"nonpayable","type":"function"},
-            {"inputs":[{"internalType":"bytes32","name":"role","type":"bytes32"},{"internalType":"address","name":"account","type":"address"}],"name":"hasRole","outputs":[{"internalType":"bool","name":"","type":"bool"}],"stateMutability":"view","type":"function"},
-            {"inputs":[],"name":"increasePerGen","outputs":[{"internalType":"uint256","name":"","type":"uint256"}],"stateMutability":"view","type":"function"},
-            {"inputs":[],"name":"increasePerSummon","outputs":[{"internalType":"uint256","name":"","type":"uint256"}],"stateMutability":"view","type":"function"},
-            {"inputs":[{"internalType":"uint256","name":"_tokenId","type":"uint256"}],"name":"isOnAuction","outputs":[{"internalType":"bool","name":"","type":"bool"}],"stateMutability":"nonpayable","type":"function"},
-            {"inputs":[],"name":"jewelToken","outputs":[{"internalType":"contract IJewelToken","name":"","type":"address"}],"stateMutability":"view","type":"function"},
-            {"inputs":[],"name":"newSummonCooldown","outputs":[{"internalType":"uint256","name":"","type":"uint256"}],"stateMutability":"view","type":"function"},
-            {"inputs":[{"internalType":"uint256","name":"_crystalId","type":"uint256"}],"name":"open","outputs":[{"internalType":"uint256","name":"","type":"uint256"}],"stateMutability":"nonpayable","type":"function"},
-            {"inputs":[],"name":"owner","outputs":[{"internalType":"address","name":"","type":"address"}],"stateMutability":"view","type":"function"},
-            {"inputs":[],"name":"ownerCut","outputs":[{"internalType":"uint256","name":"","type":"uint256"}],"stateMutability":"view","type":"function"},
-            {"inputs":[],"name":"paused","outputs":[{"internalType":"bool","name":"","type":"bool"}],"stateMutability":"view","type":"function"},
-            {"inputs":[{"internalType":"uint256","name":"_crystalId","type":"uint256"}],"name":"rechargeCrystal","outputs":[],"stateMutability":"nonpayable","type":"function"},
-            {"inputs":[],"name":"renounceOwnership","outputs":[],"stateMutability":"nonpayable","type":"function"},
-            {"inputs":[{"internalType":"bytes32","name":"role","type":"bytes32"},{"internalType":"address","name":"account","type":"address"}],"name":"renounceRole","outputs":[],"stateMutability":"nonpayable","type":"function"},
-            {"inputs":[{"internalType":"bytes32","name":"role","type":"bytes32"},{"internalType":"address","name":"account","type":"address"}],"name":"revokeRole","outputs":[],"stateMutability":"nonpayable","type":"function"},
-            {"inputs":[{"internalType":"address[]","name":"_feeAddresses","type":"address[]"},{"internalType":"uint256[]","name":"_feePercents","type":"uint256[]"}],"name":"setFees","outputs":[],"stateMutability":"nonpayable","type":"function"},
-            {"inputs":[{"internalType":"address","name":"_geneScienceAddress","type":"address"}],"name":"setGeneScienceAddress","outputs":[],"stateMutability":"nonpayable","type":"function"},
-            {"inputs":[{"internalType":"address","name":"_statScienceAddress","type":"address"}],"name":"setStatScienceAddress","outputs":[],"stateMutability":"nonpayable","type":"function"},
-            {"inputs":[{"internalType":"uint256","name":"_newSummonCooldown","type":"uint256"},{"internalType":"uint256","name":"_baseCooldown","type":"uint256"},{"internalType":"uint256","name":"_cooldownPerGen","type":"uint256"}],"name":"setSummonCooldowns","outputs":[],"stateMutability":"nonpayable","type":"function"},
-            {"inputs":[{"internalType":"uint256","name":"_baseSummonFee","type":"uint256"},{"internalType":"uint256","name":"_increasePerSummon","type":"uint256"},{"internalType":"uint256","name":"_increasePerGen","type":"uint256"}],"name":"setSummonFees","outputs":[],"stateMutability":"nonpayable","type":"function"},
-            {"inputs":[],"name":"statScience","outputs":[{"internalType":"contract IStatScience","name":"","type":"address"}],"stateMutability":"view","type":"function"},
-            {"inputs":[{"internalType":"uint256","name":"_summonerId","type":"uint256"},{"internalType":"uint256","name":"_assistantId","type":"uint256"},{"internalType":"uint16","name":"_summonerTears","type":"uint16"},{"internalType":"uint16","name":"_assistantTears","type":"uint16"},{"internalType":"address","name":"_bonusItem","type":"address"}],"name":"summonCrystal","outputs":[],"stateMutability":"nonpayable","type":"function"},
-            {"inputs":[{"internalType":"bytes4","name":"interfaceId","type":"bytes4"}],"name":"supportsInterface","outputs":[{"internalType":"bool","name":"","type":"bool"}],"stateMutability":"view","type":"function"},
-            {"inputs":[],"name":"toggleEnabled","outputs":[],"stateMutability":"nonpayable","type":"function"},
-            {"inputs":[{"internalType":"address","name":"newOwner","type":"address"}],"name":"transferOwnership","outputs":[],"stateMutability":"nonpayable","type":"function"},
-            {"inputs":[{"internalType":"address","name":"","type":"address"},{"internalType":"uint256","name":"","type":"uint256"}],"name":"userAuctions","outputs":[{"internalType":"uint256","name":"","type":"uint256"}],"stateMutability":"view","type":"function"},
-            {"inputs":[{"internalType":"address","name":"","type":"address"},{"internalType":"uint256","name":"","type":"uint256"}],"name":"userCrystals","outputs":[{"internalType":"uint256","name":"","type":"uint256"}],"stateMutability":"view","type":"function"},
-            {"inputs":[{"internalType":"uint256","name":"blockNumber","type":"uint256"}],"name":"vrf","outputs":[{"internalType":"bytes32","name":"result","type":"bytes32"}],"stateMutability":"view","type":"function"}
-        ]
-        """
+		[
+			{"inputs":[{"internalType":"address","name":"_heroCoreAddress","type":"address"},{"internalType":"address","name":"_geneScienceAddress","type":"address"},{"internalType":"address","name":"_jewelTokenAddress","type":"address"},{"internalType":"address","name":"_gaiaTearsAddress","type":"address"},{"internalType":"address","name":"_statScienceAddress","type":"address"},{"internalType":"uint256","name":"_cut","type":"uint256"}],"stateMutability":"nonpayable","type":"constructor"},
+			{"anonymous":false,"inputs":[{"indexed":false,"internalType":"uint256","name":"auctionId","type":"uint256"},{"indexed":true,"internalType":"uint256","name":"tokenId","type":"uint256"}],"name":"AuctionCancelled","type":"event"},
+			{"anonymous":false,"inputs":[{"indexed":false,"internalType":"uint256","name":"auctionId","type":"uint256"},{"indexed":true,"internalType":"address","name":"owner","type":"address"},{"indexed":true,"internalType":"uint256","name":"tokenId","type":"uint256"},{"indexed":false,"internalType":"uint256","name":"startingPrice","type":"uint256"},{"indexed":false,"internalType":"uint256","name":"endingPrice","type":"uint256"},{"indexed":false,"internalType":"uint256","name":"duration","type":"uint256"},{"indexed":false,"internalType":"address","name":"winner","type":"address"}],"name":"AuctionCreated","type":"event"},
+			{"anonymous":false,"inputs":[{"indexed":false,"internalType":"uint256","name":"auctionId","type":"uint256"},{"indexed":true,"internalType":"uint256","name":"tokenId","type":"uint256"},{"indexed":false,"internalType":"uint256","name":"totalPrice","type":"uint256"},{"indexed":false,"internalType":"address","name":"winner","type":"address"}],"name":"AuctionSuccessful","type":"event"},
+			{"anonymous":false,"inputs":[{"indexed":true,"internalType":"address","name":"owner","type":"address"},{"indexed":false,"internalType":"uint256","name":"crystalId","type":"uint256"},{"indexed":false,"internalType":"uint256","name":"heroId","type":"uint256"}],"name":"CrystalOpen","type":"event"},
+			{"anonymous":false,"inputs":[{"indexed":false,"internalType":"uint256","name":"crystalId","type":"uint256"},{"indexed":true,"internalType":"address","name":"owner","type":"address"},{"indexed":false,"internalType":"uint256","name":"summonerId","type":"uint256"},{"indexed":false,"internalType":"uint256","name":"assistantId","type":"uint256"},{"indexed":false,"internalType":"uint16","name":"generation","type":"uint16"},{"indexed":false,"internalType":"uint256","name":"createdBlock","type":"uint256"},{"indexed":false,"internalType":"uint8","name":"summonerTears","type":"uint8"},{"indexed":false,"internalType":"uint8","name":"assistantTears","type":"uint8"},{"indexed":false,"internalType":"address","name":"bonusItem","type":"address"}],"name":"CrystalSummoned","type":"event"},
+			{"anonymous":false,"inputs":[{"indexed":true,"internalType":"address","name":"previousOwner","type":"address"},{"indexed":true,"internalType":"address","name":"newOwner","type":"address"}],"name":"OwnershipTransferred","type":"event"},
+			{"anonymous":false,"inputs":[{"indexed":false,"internalType":"address","name":"account","type":"address"}],"name":"Paused","type":"event"},
+			{"anonymous":false,"inputs":[{"indexed":true,"internalType":"bytes32","name":"role","type":"bytes32"},{"indexed":true,"internalType":"bytes32","name":"previousAdminRole","type":"bytes32"},{"indexed":true,"internalType":"bytes32","name":"newAdminRole","type":"bytes32"}],"name":"RoleAdminChanged","type":"event"},
+			{"anonymous":false,"inputs":[{"indexed":true,"internalType":"bytes32","name":"role","type":"bytes32"},{"indexed":true,"internalType":"address","name":"account","type":"address"},{"indexed":true,"internalType":"address","name":"sender","type":"address"}],"name":"RoleGranted","type":"event"},
+			{"anonymous":false,"inputs":[{"indexed":true,"internalType":"bytes32","name":"role","type":"bytes32"},{"indexed":true,"internalType":"address","name":"account","type":"address"},{"indexed":true,"internalType":"address","name":"sender","type":"address"}],"name":"RoleRevoked","type":"event"},
+			{"anonymous":false,"inputs":[{"indexed":false,"internalType":"address","name":"account","type":"address"}],"name":"Unpaused","type":"event"},
+			{"inputs":[],"name":"DEFAULT_ADMIN_ROLE","outputs":[{"internalType":"bytes32","name":"","type":"bytes32"}],"stateMutability":"view","type":"function"},
+			{"inputs":[],"name":"MODERATOR_ROLE","outputs":[{"internalType":"bytes32","name":"","type":"bytes32"}],"stateMutability":"view","type":"function"},
+			{"inputs":[],"name":"auctionHeroCore","outputs":[{"internalType":"contract IHeroCore","name":"","type":"address"}],"stateMutability":"view","type":"function"},
+			{"inputs":[],"name":"baseCooldown","outputs":[{"internalType":"uint256","name":"","type":"uint256"}],"stateMutability":"view","type":"function"},
+			{"inputs":[],"name":"baseSummonFee","outputs":[{"internalType":"uint256","name":"","type":"uint256"}],"stateMutability":"view","type":"function"},
+			{"inputs":[{"internalType":"uint256","name":"_tokenId","type":"uint256"},{"internalType":"uint256","name":"_bidAmount","type":"uint256"}],"name":"bid","outputs":[],"stateMutability":"nonpayable","type":"function"},
+			{"inputs":[{"components":[{"internalType":"uint256","name":"id","type":"uint256"},{"components":[{"internalType":"uint256","name":"summonedTime","type":"uint256"},{"internalType":"uint256","name":"nextSummonTime","type":"uint256"},{"internalType":"uint256","name":"summonerId","type":"uint256"},{"internalType":"uint256","name":"assistantId","type":"uint256"},{"internalType":"uint32","name":"summons","type":"uint32"},{"internalType":"uint32","name":"maxSummons","type":"uint32"}],"internalType":"struct IHeroTypes.SummoningInfo","name":"summoningInfo","type":"tuple"},{"components":[{"internalType":"uint256","name":"statGenes","type":"uint256"},{"internalType":"uint256","name":"visualGenes","type":"uint256"},{"internalType":"enum IHeroTypes.Rarity","name":"rarity","type":"uint8"},{"internalType":"bool","name":"shiny","type":"bool"},{"internalType":"uint16","name":"generation","type":"uint16"},{"internalType":"uint32","name":"firstName","type":"uint32"},{"internalType":"uint32","name":"lastName","type":"uint32"},{"internalType":"uint8","name":"shinyStyle","type":"uint8"},{"internalType":"uint8","name":"class","type":"uint8"},{"internalType":"uint8","name":"subClass","type":"uint8"}],"internalType":"struct IHeroTypes.HeroInfo","name":"info","type":"tuple"},{"components":[{"internalType":"uint256","name":"staminaFullAt","type":"uint256"},{"internalType":"uint256","name":"hpFullAt","type":"uint256"},{"internalType":"uint256","name":"mpFullAt","type":"uint256"},{"internalType":"uint16","name":"level","type":"uint16"},{"internalType":"uint64","name":"xp","type":"uint64"},{"internalType":"address","name":"currentQuest","type":"address"},{"internalType":"uint8","name":"sp","type":"uint8"},{"internalType":"enum IHeroTypes.HeroStatus","name":"status","type":"uint8"}],"internalType":"struct IHeroTypes.HeroState","name":"state","type":"tuple"},{"components":[{"internalType":"uint16","name":"strength","type":"uint16"},{"internalType":"uint16","name":"intelligence","type":"uint16"},{"internalType":"uint16","name":"wisdom","type":"uint16"},{"internalType":"uint16","name":"luck","type":"uint16"},{"internalType":"uint16","name":"agility","type":"uint16"},{"internalType":"uint16","name":"vitality","type":"uint16"},{"internalType":"uint16","name":"endurance","type":"uint16"},{"internalType":"uint16","name":"dexterity","type":"uint16"},{"internalType":"uint16","name":"hp","type":"uint16"},{"internalType":"uint16","name":"mp","type":"uint16"},{"internalType":"uint16","name":"stamina","type":"uint16"}],"internalType":"struct IHeroTypes.HeroStats","name":"stats","type":"tuple"},{"components":[{"internalType":"uint16","name":"strength","type":"uint16"},{"internalType":"uint16","name":"intelligence","type":"uint16"},{"internalType":"uint16","name":"wisdom","type":"uint16"},{"internalType":"uint16","name":"luck","type":"uint16"},{"internalType":"uint16","name":"agility","type":"uint16"},{"internalType":"uint16","name":"vitality","type":"uint16"},{"internalType":"uint16","name":"endurance","type":"uint16"},{"internalType":"uint16","name":"dexterity","type":"uint16"},{"internalType":"uint16","name":"hpSm","type":"uint16"},{"internalType":"uint16","name":"hpRg","type":"uint16"},{"internalType":"uint16","name":"hpLg","type":"uint16"},{"internalType":"uint16","name":"mpSm","type":"uint16"},{"internalType":"uint16","name":"mpRg","type":"uint16"},{"internalType":"uint16","name":"mpLg","type":"uint16"}],"internalType":"struct IHeroTypes.HeroStatGrowth","name":"primaryStatGrowth","type":"tuple"},{"components":[{"internalType":"uint16","name":"strength","type":"uint16"},{"internalType":"uint16","name":"intelligence","type":"uint16"},{"internalType":"uint16","name":"wisdom","type":"uint16"},{"internalType":"uint16","name":"luck","type":"uint16"},{"internalType":"uint16","name":"agility","type":"uint16"},{"internalType":"uint16","name":"vitality","type":"uint16"},{"internalType":"uint16","name":"endurance","type":"uint16"},{"internalType":"uint16","name":"dexterity","type":"uint16"},{"internalType":"uint16","name":"hpSm","type":"uint16"},{"internalType":"uint16","name":"hpRg","type":"uint16"},{"internalType":"uint16","name":"hpLg","type":"uint16"},{"internalType":"uint16","name":"mpSm","type":"uint16"},{"internalType":"uint16","name":"mpRg","type":"uint16"},{"internalType":"uint16","name":"mpLg","type":"uint16"}],"internalType":"struct IHeroTypes.HeroStatGrowth","name":"secondaryStatGrowth","type":"tuple"},{"components":[{"internalType":"uint16","name":"mining","type":"uint16"},{"internalType":"uint16","name":"gardening","type":"uint16"},{"internalType":"uint16","name":"foraging","type":"uint16"},{"internalType":"uint16","name":"fishing","type":"uint16"}],"internalType":"struct IHeroTypes.HeroProfessions","name":"professions","type":"tuple"}],"internalType":"struct IHeroTypes.Hero","name":"_hero","type":"tuple"}],"name":"calculateSummoningCost","outputs":[{"internalType":"uint256","name":"","type":"uint256"}],"stateMutability":"view","type":"function"},
+			{"inputs":[{"internalType":"uint256","name":"_tokenId","type":"uint256"}],"name":"cancelAuction","outputs":[],"stateMutability":"nonpayable","type":"function"},
+			{"inputs":[{"internalType":"uint256","name":"_tokenId","type":"uint256"}],"name":"cancelAuctionWhenPaused","outputs":[],"stateMutability":"nonpayable","type":"function"},
+			{"inputs":[],"name":"cooldownPerGen","outputs":[{"internalType":"uint256","name":"","type":"uint256"}],"stateMutability":"view","type":"function"},
+			{"inputs":[{"internalType":"uint256","name":"_tokenId","type":"uint256"},{"internalType":"uint128","name":"_startingPrice","type":"uint128"},{"internalType":"uint128","name":"_endingPrice","type":"uint128"},{"internalType":"uint64","name":"_duration","type":"uint64"},{"internalType":"address","name":"_winner","type":"address"}],"name":"createAuction","outputs":[],"stateMutability":"nonpayable","type":"function"},
+			{"inputs":[{"internalType":"uint256","name":"","type":"uint256"}],"name":"crystals","outputs":[{"internalType":"address","name":"owner","type":"address"},{"internalType":"uint256","name":"summonerId","type":"uint256"},{"internalType":"uint256","name":"assistantId","type":"uint256"},{"internalType":"uint16","name":"generation","type":"uint16"},{"internalType":"uint256","name":"createdBlock","type":"uint256"},{"internalType":"uint256","name":"heroId","type":"uint256"},{"internalType":"uint8","name":"summonerTears","type":"uint8"},{"internalType":"uint8","name":"assistantTears","type":"uint8"},{"internalType":"address","name":"bonusItem","type":"address"},{"internalType":"uint32","name":"maxSummons","type":"uint32"},{"internalType":"uint32","name":"firstName","type":"uint32"},{"internalType":"uint32","name":"lastName","type":"uint32"},{"internalType":"uint8","name":"shinyStyle","type":"uint8"}],"stateMutability":"view","type":"function"},
+			{"inputs":[{"internalType":"uint256","name":"_rarityRoll","type":"uint256"},{"internalType":"uint256","name":"_rarityMod","type":"uint256"}],"name":"determineRarity","outputs":[{"internalType":"enum IHeroTypes.Rarity","name":"","type":"uint8"}],"stateMutability":"pure","type":"function"},
+			{"inputs":[],"name":"enabled","outputs":[{"internalType":"bool","name":"","type":"bool"}],"stateMutability":"view","type":"function"},
+			{"inputs":[{"internalType":"uint256","name":"randomNumber","type":"uint256"},{"internalType":"uint256","name":"digits","type":"uint256"},{"internalType":"uint256","name":"offset","type":"uint256"}],"name":"extractNumber","outputs":[{"internalType":"uint256","name":"result","type":"uint256"}],"stateMutability":"pure","type":"function"},
+			{"inputs":[{"internalType":"uint256","name":"_tokenId","type":"uint256"}],"name":"getAuction","outputs":[{"internalType":"uint256","name":"auctionId","type":"uint256"},{"internalType":"address","name":"seller","type":"address"},{"internalType":"uint256","name":"startingPrice","type":"uint256"},{"internalType":"uint256","name":"endingPrice","type":"uint256"},{"internalType":"uint256","name":"duration","type":"uint256"},{"internalType":"uint256","name":"startedAt","type":"uint256"}],"stateMutability":"view","type":"function"},
+			{"inputs":[{"internalType":"uint256","name":"_crystalId","type":"uint256"}],"name":"getCrystal","outputs":[{"components":[{"internalType":"address","name":"owner","type":"address"},{"internalType":"uint256","name":"summonerId","type":"uint256"},{"internalType":"uint256","name":"assistantId","type":"uint256"},{"internalType":"uint16","name":"generation","type":"uint16"},{"internalType":"uint256","name":"createdBlock","type":"uint256"},{"internalType":"uint256","name":"heroId","type":"uint256"},{"internalType":"uint8","name":"summonerTears","type":"uint8"},{"internalType":"uint8","name":"assistantTears","type":"uint8"},{"internalType":"address","name":"bonusItem","type":"address"},{"internalType":"uint32","name":"maxSummons","type":"uint32"},{"internalType":"uint32","name":"firstName","type":"uint32"},{"internalType":"uint32","name":"lastName","type":"uint32"},{"internalType":"uint8","name":"shinyStyle","type":"uint8"}],"internalType":"struct ICrystalTypes.HeroCrystal","name":"","type":"tuple"}],"stateMutability":"view","type":"function"},
+			{"inputs":[{"internalType":"uint256","name":"_tokenId","type":"uint256"}],"name":"getCurrentPrice","outputs":[{"internalType":"uint256","name":"","type":"uint256"}],"stateMutability":"view","type":"function"},
+			{"inputs":[{"internalType":"bytes32","name":"role","type":"bytes32"}],"name":"getRoleAdmin","outputs":[{"internalType":"bytes32","name":"","type":"bytes32"}],"stateMutability":"view","type":"function"},
+			{"inputs":[{"internalType":"address","name":"_address","type":"address"}],"name":"getUserAuctions","outputs":[{"internalType":"uint256[]","name":"","type":"uint256[]"}],"stateMutability":"view","type":"function"},
+			{"inputs":[{"internalType":"address","name":"_address","type":"address"}],"name":"getUserCrystals","outputs":[{"internalType":"uint256[]","name":"","type":"uint256[]"}],"stateMutability":"view","type":"function"},
+			{"inputs":[{"internalType":"bytes32","name":"role","type":"bytes32"},{"internalType":"address","name":"account","type":"address"}],"name":"grantRole","outputs":[],"stateMutability":"nonpayable","type":"function"},
+			{"inputs":[{"internalType":"bytes32","name":"role","type":"bytes32"},{"internalType":"address","name":"account","type":"address"}],"name":"hasRole","outputs":[{"internalType":"bool","name":"","type":"bool"}],"stateMutability":"view","type":"function"},
+			{"inputs":[],"name":"increasePerGen","outputs":[{"internalType":"uint256","name":"","type":"uint256"}],"stateMutability":"view","type":"function"},
+			{"inputs":[],"name":"increasePerSummon","outputs":[{"internalType":"uint256","name":"","type":"uint256"}],"stateMutability":"view","type":"function"},
+			{"inputs":[{"internalType":"uint256","name":"_tokenId","type":"uint256"}],"name":"isOnAuction","outputs":[{"internalType":"bool","name":"","type":"bool"}],"stateMutability":"nonpayable","type":"function"},
+			{"inputs":[],"name":"jewelToken","outputs":[{"internalType":"contract IJewelToken","name":"","type":"address"}],"stateMutability":"view","type":"function"},
+			{"inputs":[],"name":"newSummonCooldown","outputs":[{"internalType":"uint256","name":"","type":"uint256"}],"stateMutability":"view","type":"function"},
+			{"inputs":[{"internalType":"uint256","name":"_crystalId","type":"uint256"}],"name":"open","outputs":[{"internalType":"uint256","name":"","type":"uint256"}],"stateMutability":"nonpayable","type":"function"},
+			{"inputs":[],"name":"owner","outputs":[{"internalType":"address","name":"","type":"address"}],"stateMutability":"view","type":"function"},
+			{"inputs":[],"name":"ownerCut","outputs":[{"internalType":"uint256","name":"","type":"uint256"}],"stateMutability":"view","type":"function"},
+			{"inputs":[],"name":"paused","outputs":[{"internalType":"bool","name":"","type":"bool"}],"stateMutability":"view","type":"function"},
+			{"inputs":[{"internalType":"uint256","name":"_crystalId","type":"uint256"}],"name":"rechargeCrystal","outputs":[],"stateMutability":"nonpayable","type":"function"},
+			{"inputs":[],"name":"renounceOwnership","outputs":[],"stateMutability":"nonpayable","type":"function"},
+			{"inputs":[{"internalType":"bytes32","name":"role","type":"bytes32"},{"internalType":"address","name":"account","type":"address"}],"name":"renounceRole","outputs":[],"stateMutability":"nonpayable","type":"function"},
+			{"inputs":[{"internalType":"bytes32","name":"role","type":"bytes32"},{"internalType":"address","name":"account","type":"address"}],"name":"revokeRole","outputs":[],"stateMutability":"nonpayable","type":"function"},
+			{"inputs":[{"internalType":"address[]","name":"_feeAddresses","type":"address[]"},{"internalType":"uint256[]","name":"_feePercents","type":"uint256[]"}],"name":"setFees","outputs":[],"stateMutability":"nonpayable","type":"function"},
+			{"inputs":[{"internalType":"address","name":"_geneScienceAddress","type":"address"}],"name":"setGeneScienceAddress","outputs":[],"stateMutability":"nonpayable","type":"function"},
+			{"inputs":[{"internalType":"address","name":"_statScienceAddress","type":"address"}],"name":"setStatScienceAddress","outputs":[],"stateMutability":"nonpayable","type":"function"},
+			{"inputs":[{"internalType":"uint256","name":"_newSummonCooldown","type":"uint256"},{"internalType":"uint256","name":"_baseCooldown","type":"uint256"},{"internalType":"uint256","name":"_cooldownPerGen","type":"uint256"}],"name":"setSummonCooldowns","outputs":[],"stateMutability":"nonpayable","type":"function"},
+			{"inputs":[{"internalType":"uint256","name":"_baseSummonFee","type":"uint256"},{"internalType":"uint256","name":"_increasePerSummon","type":"uint256"},{"internalType":"uint256","name":"_increasePerGen","type":"uint256"}],"name":"setSummonFees","outputs":[],"stateMutability":"nonpayable","type":"function"},
+			{"inputs":[],"name":"statScience","outputs":[{"internalType":"contract IStatScience","name":"","type":"address"}],"stateMutability":"view","type":"function"},
+			{"inputs":[{"internalType":"uint256","name":"_summonerId","type":"uint256"},{"internalType":"uint256","name":"_assistantId","type":"uint256"},{"internalType":"uint16","name":"_summonerTears","type":"uint16"},{"internalType":"uint16","name":"_assistantTears","type":"uint16"},{"internalType":"address","name":"_bonusItem","type":"address"}],"name":"summonCrystal","outputs":[],"stateMutability":"nonpayable","type":"function"},
+			{"inputs":[{"internalType":"bytes4","name":"interfaceId","type":"bytes4"}],"name":"supportsInterface","outputs":[{"internalType":"bool","name":"","type":"bool"}],"stateMutability":"view","type":"function"},
+			{"inputs":[],"name":"toggleEnabled","outputs":[],"stateMutability":"nonpayable","type":"function"},
+			{"inputs":[{"internalType":"address","name":"newOwner","type":"address"}],"name":"transferOwnership","outputs":[],"stateMutability":"nonpayable","type":"function"},
+			{"inputs":[{"internalType":"address","name":"","type":"address"},{"internalType":"uint256","name":"","type":"uint256"}],"name":"userAuctions","outputs":[{"internalType":"uint256","name":"","type":"uint256"}],"stateMutability":"view","type":"function"},
+			{"inputs":[{"internalType":"address","name":"","type":"address"},{"internalType":"uint256","name":"","type":"uint256"}],"name":"userCrystals","outputs":[{"internalType":"uint256","name":"","type":"uint256"}],"stateMutability":"view","type":"function"},
+			{"inputs":[{"internalType":"uint256","name":"blockNumber","type":"uint256"}],"name":"vrf","outputs":[{"internalType":"bytes32","name":"result","type":"bytes32"}],"stateMutability":"view","type":"function"}
+		]
+		"""
 
 AUCTIONS_OPEN_GRAPHQL_QUERY = """
-                        query {
-                          saleAuctions(skip: %d, first: %d, orderBy: startedAt, orderDirection: desc, where: {open: true, winner: null}) {
-                            id
-                            seller {
-                                name
-                            }
-                            tokenId {
-                              id
-                              owner {
-                                owner
-                              }
-                              statGenes
-                              generation
-                              rarity
-                              mainClass
-                              subClass
-                              strength
-                              intelligence
-                              wisdom
-                              luck
-                              agility
-                              vitality
-                              endurance
-                              dexterity
-                              level
-                              summons
-                              maxSummons
-                              summonerId {
-                                id
-                              }
-                              assistantId {
-                                id
-                              }
-                            }
-                            startingPrice
-                            endingPrice
-                            startedAt
-                            duration
-                            winner {
-                              id
-                              name
-                            }
-                            open
-                            
-                          }
-                          
-                        }
-                        """
+						query {
+						  saleAuctions(skip: %d, first: %d, orderBy: startedAt, orderDirection: desc, where: {open: true, winner: null}) {
+							id
+							seller {
+								name
+							}
+							tokenId {
+							  id
+							  owner {
+								owner
+							  }
+							  statGenes
+							  visualGenes
+							  generation
+							  rarity
+							  mainClass
+							  subClass
+							  strength
+							  intelligence
+							  wisdom
+							  luck
+							  agility
+							  vitality
+							  endurance
+							  dexterity
+							  strengthGrowthP
+							  intelligenceGrowthP
+							  wisdomGrowthP
+							  luckGrowthP
+							  agilityGrowthP
+							  vitalityGrowthP
+							  enduranceGrowthP
+							  dexterityGrowthP
+							  strengthGrowthS
+							  intelligenceGrowthS
+							  wisdomGrowthS
+							  luckGrowthS
+							  agilityGrowthS
+							  vitalityGrowthS
+							  enduranceGrowthS
+							  dexterityGrowthS
+							  level
+							  summons
+							  maxSummons
+							  summonerId {
+								id
+							  }
+							  assistantId {
+								id
+							  }
+							}
+							startingPrice
+							endingPrice
+							startedAt
+							duration
+							winner {
+							  id
+							  name
+							}
+							open
+							
+						  }
+						  
+						}
+						"""
 
 AUCTIONS_TOKEN_IDS_GRAPHQL_QUERY = """
-                        query {
-                          saleAuctions(orderBy: startedAt, orderDirection: desc, where: {open: true, tokenId_in: %s }) {
-                            id
-                            seller {
-                                name
-                            }
-                            tokenId {
-                              id
-                              owner {
-                                owner
-                              }
-                              
-                              statGenes
-                              generation
-                              rarity
-                              mainClass
-                              subClass
-                              summons
-                              maxSummons
-                              summonerId {
-                                id
-                              }
-                              assistantId {
-                                id
-                              }
-                            }
-                            startingPrice
-                            endingPrice
-                            startedAt
-                            duration
-                            winner {
-                              id
-                              name
-                            }
-                            open
+						query {
+						  saleAuctions(orderBy: startedAt, orderDirection: desc, where: {open: true, tokenId_in: %s }) {
+							id
+							seller {
+								name
+							}
+							tokenId {
+							  id
+							  owner {
+								owner
+							  }
+							  
+							  statGenes
+							  visualGenes
+							  generation
+							  rarity
+							  mainClass
+							  subClass
+							  summons
+							  maxSummons
+							  summonerId {
+								id
+							  }
+							  assistantId {
+								id
+							  }
+							}
+							startingPrice
+							endingPrice
+							startedAt
+							duration
+							winner {
+							  id
+							  name
+							}
+							open
 
-                          }
+						  }
 
-                        }
-                        """
+						}
+						"""
 
 
 def block_explorer_link(contract_address, txid):
 	if hasattr(contract_address, 'address'):
 		contract_address = str(contract_address.address)
 	contract_address = str(contract_address).upper()
 	if contract_address == SERENDALE_CONTRACT_ADDRESS.upper():
@@ -174,178 +192,228 @@
 	elif contract_address == CRYSTALVALE_CONTRACT_ADDRESS.upper():
 		return 'https://subnets.avax.network/defi-kingdoms/dfk-chain/explorer/tx/' + str(txid)
 	else:
 		return str(txid)
 
 
 def bid_hero(contract_address, token_id, bid_amount_wei, private_key, nonce, gas_price_gwei, tx_timeout_seconds, rpc_address, logger=None):
-    w3 = Web3(Web3.HTTPProvider(rpc_address))
-    account = w3.eth.account.privateKeyToAccount(private_key)
-    w3.eth.default_account = account.address
-
-    sales_auction_contract_address = Web3.toChecksumAddress(contract_address)
-    sales_auction_contract = w3.eth.contract(sales_auction_contract_address, abi=ABI)
-
-    if logger is not None:
-        logger.info("Biding " + str(wei2ether(bid_amount_wei)) + " on hero id " + str(token_id))
-    tx = sales_auction_contract.functions.bid(token_id, bid_amount_wei).buildTransaction(
-        {'gasPrice': w3.toWei(gas_price_gwei, 'gwei'), 'nonce': nonce})
-
-    if logger is not None:
-        logger.info("Signing transaction")
-    signed_tx = w3.eth.account.sign_transaction(tx, private_key=private_key)
-    if logger is not None:
-        logger.info("Sending transaction " + str(tx))
-    ret = w3.eth.send_raw_transaction(signed_tx.rawTransaction)
-    if logger is not None:
-        logger.info("Transaction successfully sent !")
-        logger.info("Waiting for transaction " + block_explorer_link(contract_address, signed_tx.hash.hex()) + " to be mined")
-    tx_receipt = w3.eth.wait_for_transaction_receipt(transaction_hash=signed_tx.hash, timeout=tx_timeout_seconds, poll_latency=2)
-
-    if logger is not None:
-        logger.info("Transaction mined !")
-        logger.info(str(tx_receipt))
+	w3 = Web3(Web3.HTTPProvider(rpc_address))
+	account = w3.eth.account.from_key(private_key)
+	w3.eth.default_account = account.address
+
+	sales_auction_contract_address = Web3.to_checksum_address(contract_address)
+	sales_auction_contract = w3.eth.contract(sales_auction_contract_address, abi=ABI)
+
+	if logger is not None:
+		logger.info("Biding " + str(wei2ether(bid_amount_wei)) + " on hero id " + str(token_id))
+	tx = sales_auction_contract.functions.bid(token_id, bid_amount_wei).build_transaction(
+		{'gasPrice': w3.to_wei(gas_price_gwei, 'gwei'), 'nonce': nonce})
+
+	if logger is not None:
+		logger.info("Signing transaction")
+	signed_tx = w3.eth.account.sign_transaction(tx, private_key=private_key)
+	if logger is not None:
+		logger.info("Sending transaction " + str(tx))
+	ret = w3.eth.send_raw_transaction(signed_tx.rawTransaction)
+	if logger is not None:
+		logger.info("Transaction successfully sent !")
+		logger.info("Waiting for transaction " + block_explorer_link(contract_address, signed_tx.hash.hex()) + " to be mined")
+	tx_receipt = w3.eth.wait_for_transaction_receipt(transaction_hash=signed_tx.hash, timeout=tx_timeout_seconds, poll_latency=2)
+
+	if logger is not None:
+		logger.info("Transaction mined !")
+		logger.info(str(tx_receipt))
 
-    return tx_receipt
+	return tx_receipt
 
 
 def create_auction(contract_address, token_id, starting_price_wei, ending_price_wei, duration, winner, private_key, nonce, gas_price_gwei, tx_timeout_seconds, rpc_address, logger=None):
-    w3 = Web3(Web3.HTTPProvider(rpc_address))
-    account = w3.eth.account.privateKeyToAccount(private_key)
-    w3.eth.default_account = account.address
-
-    sales_auction_contract_address = Web3.toChecksumAddress(contract_address)
-    sales_auction_contract = w3.eth.contract(sales_auction_contract_address, abi=ABI)
-
-    if logger is not None:
-        logger.info("Auctioning " + str(token_id) + " (starting price=" + str(wei2ether(starting_price_wei)) + ", ending price=" + str(wei2ether(ending_price_wei)) + ", duration=" + str(duration) + ", private sale buyer=" + str(winner) + ")")
-    tx = sales_auction_contract.functions.createAuction(token_id, starting_price_wei, ending_price_wei, duration, winner).buildTransaction(
-        {'gasPrice': w3.toWei(gas_price_gwei, 'gwei'), 'nonce': nonce})
-    if logger is not None:
-        logger.info("Signing transaction")
-    signed_tx = w3.eth.account.sign_transaction(tx, private_key=private_key)
-    if logger is not None:
-        logger.info("Sending transaction " + str(tx))
-    ret = w3.eth.send_raw_transaction(signed_tx.rawTransaction)
-    if logger is not None:
-        logger.info("Transaction successfully sent !")
-        logger.info("Waiting for transaction " + block_explorer_link(contract_address, signed_tx.hash.hex()) + " to be mined")
-    tx_receipt = w3.eth.wait_for_transaction_receipt(transaction_hash=signed_tx.hash, timeout=tx_timeout_seconds, poll_latency=2)
-    if logger is not None:
-        logger.info("Transaction mined !")
-        logger.info(str(tx_receipt))
-    return tx_receipt
+	w3 = Web3(Web3.HTTPProvider(rpc_address))
+	account = w3.eth.account.from_key(private_key)
+	w3.eth.default_account = account.address
+
+	sales_auction_contract_address = Web3.to_checksum_address(contract_address)
+	sales_auction_contract = w3.eth.contract(sales_auction_contract_address, abi=ABI)
+
+	if logger is not None:
+		logger.info("Auctioning " + str(token_id) + " (starting price=" + str(wei2ether(starting_price_wei)) + ", ending price=" + str(wei2ether(ending_price_wei)) + ", duration=" + str(duration) + ", private sale buyer=" + str(winner) + ")")
+	tx = sales_auction_contract.functions.createAuction(token_id, starting_price_wei, ending_price_wei, duration, winner).build_transaction(
+		{'gasPrice': w3.to_wei(gas_price_gwei, 'gwei'), 'nonce': nonce})
+	if logger is not None:
+		logger.info("Signing transaction")
+	signed_tx = w3.eth.account.sign_transaction(tx, private_key=private_key)
+	if logger is not None:
+		logger.info("Sending transaction " + str(tx))
+	ret = w3.eth.send_raw_transaction(signed_tx.rawTransaction)
+	if logger is not None:
+		logger.info("Transaction successfully sent !")
+		logger.info("Waiting for transaction " + block_explorer_link(contract_address, signed_tx.hash.hex()) + " to be mined")
+	tx_receipt = w3.eth.wait_for_transaction_receipt(transaction_hash=signed_tx.hash, timeout=tx_timeout_seconds, poll_latency=2)
+	if logger is not None:
+		logger.info("Transaction mined !")
+		logger.info(str(tx_receipt))
+	return tx_receipt
 
 
 def cancel_auction(contract_address, token_id, private_key, nonce, gas_price_gwei, tx_timeout_seconds, rpc_address, logger=None):
-    w3 = Web3(Web3.HTTPProvider(rpc_address))
-    account = w3.eth.account.privateKeyToAccount(private_key)
-    w3.eth.default_account = account.address
-
-    sales_auction_contract_address = Web3.toChecksumAddress(contract_address)
-    sales_auction_contract = w3.eth.contract(sales_auction_contract_address, abi=ABI)
-
-    tx = sales_auction_contract.functions.cancelAuction(token_id).buildTransaction(
-        {'gasPrice': w3.toWei(gas_price_gwei, 'gwei'), 'nonce': nonce})
-    if logger is not None:
-        logger.info("Signing transaction")
-    signed_tx = w3.eth.account.sign_transaction(tx, private_key=private_key)
-    if logger is not None:
-        logger.info("Sending transaction " + str(tx))
-    ret = w3.eth.send_raw_transaction(signed_tx.rawTransaction)
-    if logger is not None:
-        logger.info("Transaction successfully sent !")
-        logger.info("Waiting for transaction " + block_explorer_link(contract_address, signed_tx.hash.hex()) + " to be mined")
-    tx_receipt = w3.eth.wait_for_transaction_receipt(transaction_hash=signed_tx.hash, timeout=tx_timeout_seconds, poll_latency=2)
-    if logger is not None:
-        logger.info("Transaction mined !")
-        logger.info(str(tx_receipt))
-    return tx_receipt
+	w3 = Web3(Web3.HTTPProvider(rpc_address))
+	account = w3.eth.account.from_key(private_key)
+	w3.eth.default_account = account.address
+
+	sales_auction_contract_address = Web3.to_checksum_address(contract_address)
+	sales_auction_contract = w3.eth.contract(sales_auction_contract_address, abi=ABI)
+
+	tx = sales_auction_contract.functions.cancelAuction(token_id).build_transaction(
+		{'gasPrice': w3.to_wei(gas_price_gwei, 'gwei'), 'nonce': nonce})
+	if logger is not None:
+		logger.info("Signing transaction")
+	signed_tx = w3.eth.account.sign_transaction(tx, private_key=private_key)
+	if logger is not None:
+		logger.info("Sending transaction " + str(tx))
+	ret = w3.eth.send_raw_transaction(signed_tx.rawTransaction)
+	if logger is not None:
+		logger.info("Transaction successfully sent !")
+		logger.info("Waiting for transaction " + block_explorer_link(contract_address, signed_tx.hash.hex()) + " to be mined")
+	tx_receipt = w3.eth.wait_for_transaction_receipt(transaction_hash=signed_tx.hash, timeout=tx_timeout_seconds, poll_latency=2)
+	if logger is not None:
+		logger.info("Transaction mined !")
+		logger.info(str(tx_receipt))
+	return tx_receipt
 
 
 def is_on_auction(contract_address, token_id, rpc_address):
-    w3 = Web3(Web3.HTTPProvider(rpc_address))
+	w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-    sales_auction_contract_address = Web3.toChecksumAddress(contract_address)
-    sales_auction_contract = w3.eth.contract(sales_auction_contract_address, abi=ABI)
-    return sales_auction_contract.functions.isOnAuction(token_id).call()
+	sales_auction_contract_address = Web3.to_checksum_address(contract_address)
+	sales_auction_contract = w3.eth.contract(sales_auction_contract_address, abi=ABI)
+	return sales_auction_contract.functions.isOnAuction(token_id).call()
 
 
 def get_auction(contract_address, token_id, rpc_address):
-    w3 = Web3(Web3.HTTPProvider(rpc_address))
+	w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-    sales_auction_contract_address = Web3.toChecksumAddress(contract_address)
-    sales_auction_contract = w3.eth.contract(sales_auction_contract_address, abi=ABI)
-    result = sales_auction_contract.functions.getAuction(token_id).call()
-    auction = {}
-    auction['id'] = result[0]
-    auction['owner'] = result[1]
-    auction['startingPrice'] = result[2]
-    auction['endingPrice'] = result[3]
-    auction['duration'] = result[4]
-    auction['startedAt'] = result[5]
+	sales_auction_contract_address = Web3.to_checksum_address(contract_address)
+	sales_auction_contract = w3.eth.contract(sales_auction_contract_address, abi=ABI)
+	result = sales_auction_contract.functions.getAuction(token_id).call()
+	auction = {}
+	auction['id'] = result[0]
+	auction['owner'] = result[1]
+	auction['startingPrice'] = result[2]
+	auction['endingPrice'] = result[3]
+	auction['duration'] = result[4]
+	auction['startedAt'] = result[5]
 
-    return auction
+	return auction
 
 
 def get_open_auctions(graphql_address, skip=0, count=1000):
 
-    r = requests.post(graphql_address, json={'query': AUCTIONS_OPEN_GRAPHQL_QUERY % (skip, count)})
+	r = requests.post(graphql_address, json={'query': AUCTIONS_OPEN_GRAPHQL_QUERY % (skip, count)})
 
-    if r.status_code != 200:
-        raise Exception("HTTP error " + str(r.status_code) + ": " + r.text)
-    data = r.json()
-    return data['data']['saleAuctions']
+	if r.status_code != 200:
+		raise Exception("HTTP error " + str(r.status_code) + ": " + r.text)
+	data = r.json()
+	return data['data']['saleAuctions']
 
 
 def get_hero_open_auctions(graphql_address, hero_ids):
-    str_hero_ids = "["
-    for id in hero_ids:
-        str_hero_ids = str_hero_ids + "\"" + str(id) + "\", "
-    str_hero_ids = str_hero_ids + "]"
-
-    r = requests.post(graphql_address, json={'query': AUCTIONS_TOKEN_IDS_GRAPHQL_QUERY % str_hero_ids})
-    if r.status_code != 200:
-        raise Exception("HTTP error " + str(r.status_code) + ": " + r.text)
-    data = r.json()
-    return data['data']['saleAuctions']
+	str_hero_ids = "["
+	for id in hero_ids:
+		str_hero_ids = str_hero_ids + "\"" + str(id) + "\", "
+	str_hero_ids = str_hero_ids + "]"
+
+	r = requests.post(graphql_address, json={'query': AUCTIONS_TOKEN_IDS_GRAPHQL_QUERY % str_hero_ids})
+	if r.status_code != 200:
+		raise Exception("HTTP error " + str(r.status_code) + ": " + r.text)
+	data = r.json()
+	return data['data']['saleAuctions']
 
 
 def auction2hero(auction):
-    ah = auction['tokenId']
+	_class = {
+		0: "warrior",
+		1: "knight",
+		2: "thief",
+		3: "archer",
+		4: "priest",
+		5: "wizard",
+		6: "monk",
+		7: "pirate",
+		8: "berserker",
+		9: "seer",
+		10: "legionnaire",
+		11: "scholar",
+		16: "paladin",
+		17: "darkknight",
+		18: "summoner",
+		19: "ninja",
+		20: "shapeshifter",
+		21: "bard",
+		24: "dragoon",
+		25: "sage",
+		26: "spellbow",
+		28: "dreadknight"
+	}
+
+	ah = auction['tokenId']
+
+	hero = {}
+	hero['id'] = ah['id']
+	hero['info'] = {}
+	hero['info']['class'] =  _class.get(ah['mainClass'], None)
+	if hero['info']['class'] is None:
+		raise Exception("Unknown class "  +str(ah['mainClass']))
+	hero['info']['subClass'] = _class.get(ah['subClass'], None)
+	if hero['info']['subClass'] is None:
+		raise Exception("Unknown subclass "  +str(ah['subClass']))
+	hero['info']['rarity'] = ah['rarity']
+	hero['info']['level'] = ah['level']
+	hero['info']['statGenes'] = ah['statGenes']
+	hero['info']['visualGenes'] = ah['visualGenes']
+	hero['info']['generation'] = ah['generation']
+
+	hero['stats'] = {}
+	hero['stats']['strength'] = ah['strength']
+	hero['stats']['agility'] = ah['agility']
+	hero['stats']['intelligence'] = ah['intelligence']
+	hero['stats']['wisdom'] = ah['wisdom']
+	hero['stats']['luck'] = ah['luck']
+	hero['stats']['vitality'] = ah['vitality']
+	hero['stats']['endurance'] = ah['endurance']
+	hero['stats']['dexterity'] = ah['dexterity']
+
+	hero['primaryStatGrowth'] = {}
+	hero['primaryStatGrowth']['strength'] = ah['strengthGrowthP']
+	hero['primaryStatGrowth']['agility'] = ah['agilityGrowthP']
+	hero['primaryStatGrowth']['intelligence'] = ah['intelligenceGrowthP']
+	hero['primaryStatGrowth']['wisdom'] = ah['wisdomGrowthP']
+	hero['primaryStatGrowth']['luck'] = ah['luckGrowthP']
+	hero['primaryStatGrowth']['vitality'] = ah['vitalityGrowthP']
+	hero['primaryStatGrowth']['endurance'] = ah['enduranceGrowthP']
+	hero['primaryStatGrowth']['dexterity'] = ah['dexterityGrowthP']
+
+	hero['secondaryStatGrowth'] = {}
+	hero['secondaryStatGrowth']['strength'] = ah['strengthGrowthS']
+	hero['secondaryStatGrowth']['agility'] = ah['agilityGrowthS']
+	hero['secondaryStatGrowth']['intelligence'] = ah['intelligenceGrowthS']
+	hero['secondaryStatGrowth']['wisdom'] = ah['wisdomGrowthS']
+	hero['secondaryStatGrowth']['luck'] = ah['luckGrowthS']
+	hero['secondaryStatGrowth']['vitality'] = ah['vitalityGrowthS']
+	hero['secondaryStatGrowth']['endurance'] = ah['enduranceGrowthS']
+	hero['secondaryStatGrowth']['dexterity'] = ah['dexterityGrowthS']
+
+	hero['summoningInfo'] = {}
+	hero['summoningInfo']['summonerId'] = ah['summonerId']
+	hero['summoningInfo']['assistantId'] = ah['assistantId']
+	hero['summoningInfo']['maxSummons'] = ah['maxSummons']
+	hero['summoningInfo']['summons'] = ah['summons']
 
-    hero = {}
-    hero['id'] = ah['id']
-    hero['info'] = {}
-    hero['info']['class'] = ah['mainClass'].lower()
-    hero['info']['subClass'] = ah['subClass'].lower()
-    hero['info']['rarity'] = ah['rarity']
-    hero['info']['level'] = ah['level']
-    hero['info']['statGenes'] = ah['statGenes']
-    hero['info']['generation'] = ah['generation']
-
-    hero['stats'] = {}
-    hero['stats']['strength'] = ah['strength']
-    hero['stats']['agility'] = ah['agility']
-    hero['stats']['intelligence'] = ah['intelligence']
-    hero['stats']['wisdom'] = ah['wisdom']
-    hero['stats']['luck'] = ah['luck']
-    hero['stats']['vitality'] = ah['vitality']
-    hero['stats']['endurance'] = ah['endurance']
-    hero['stats']['dexterity'] = ah['dexterity']
-
-    hero['summoningInfo'] = {}
-    hero['summoningInfo']['summonerId'] = ah['summonerId']
-    hero['summoningInfo']['assistantId'] = ah['assistantId']
-    hero['summoningInfo']['maxSummons'] = ah['maxSummons']
-    hero['summoningInfo']['summons'] = ah['summons']
-
-    return hero
+	return hero
 
 
 def wei2ether(wei):
-    return float(wei) / 1000000000000000000
+	return float(wei) / 1000000000000000000
 
 
 def ether2wei(ether):
-    return int(ether * 1000000000000000000)
+	return int(ether * 1000000000000000000)
```

### Comparing `dfktools-0.2.0/src/dfktools/bridge/dfktears_bridge.py` & `dfktools-0.3.0/src/dfktools/bridge/dfktears_bridge.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,37 +37,37 @@
     else:
         return str(txid)
 
 
 def gaia_tears(realm_contract, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-    contract = Web3.toChecksumAddress(realm_contract)
+    contract = Web3.to_checksum_address(realm_contract)
     contract = w3.eth.contract(contract, abi=ABI)
     result = contract.functions.gaiaTears().call()
 
     return result
 
 
 def send_tear(origin_realm_contract, amount, destination_chain_id, private_key, nonce, gas_price_gwei, tx_timeout_seconds, rpc_address, logger):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
-    account = w3.eth.account.privateKeyToAccount(private_key)
+    account = w3.eth.account.from_key(private_key)
     w3.eth.default_account = account.address
 
-    origin_realm_contract = Web3.toChecksumAddress(origin_realm_contract)
+    origin_realm_contract = Web3.to_checksum_address(origin_realm_contract)
     origin_realm_contract = w3.eth.contract(origin_realm_contract, abi=ABI)
 
     tx = origin_realm_contract.functions.sendTear(amount, destination_chain_id)
 
     if isinstance(gas_price_gwei, dict):  # dynamic fee
-        tx = tx.buildTransaction(
-            {'maxFeePerGas': w3.toWei(gas_price_gwei['maxFeePerGas'], 'gwei'),
-             'maxPriorityFeePerGas': w3.toWei(gas_price_gwei['maxPriorityFeePerGas'], 'gwei'), 'nonce': nonce})
+        tx = tx.build_transaction(
+            {'maxFeePerGas': w3.to_wei(gas_price_gwei['maxFeePerGas'], 'gwei'),
+             'maxPriorityFeePerGas': w3.to_wei(gas_price_gwei['maxPriorityFeePerGas'], 'gwei'), 'nonce': nonce})
     else:  # legacy
-        tx = tx.buildTransaction({'gasPrice': w3.toWei(gas_price_gwei, 'gwei'), 'nonce': nonce})
+        tx = tx.build_transaction({'gasPrice': w3.to_wei(gas_price_gwei, 'gwei'), 'nonce': nonce})
 
     logger.debug("Signing transaction")
     signed_tx = w3.eth.account.sign_transaction(tx, private_key=private_key)
     logger.debug("Sending transaction " + str(tx))
     ret = w3.eth.send_raw_transaction(signed_tx.rawTransaction)
     logger.debug("Transaction successfully sent !")
     logger.info(
```

### Comparing `dfktools-0.2.0/src/dfktools/bridge/hero_bridge.py` & `dfktools-0.3.0/src/dfktools/bridge/hero_bridge.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,49 +52,49 @@
     else:
         return str(txid)
 
 
 def assisting_auction(realm_contract, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-    contract = Web3.toChecksumAddress(realm_contract)
+    contract = Web3.to_checksum_address(realm_contract)
     contract = w3.eth.contract(contract, abi=ABI)
     result = contract.functions.assistingAuction().call()
 
     return result
 
 
 def heroes(realm_contract, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-    contract = Web3.toChecksumAddress(realm_contract)
+    contract = Web3.to_checksum_address(realm_contract)
     contract = w3.eth.contract(contract, abi=ABI)
     result = contract.functions.heroes().call()
 
     return result
 
 
 def send_hero(origin_realm_contract_address, hero_id, destination_chain_id, bridge_fee_in_wei, private_key, nonce, gas_price_gwei, tx_timeout_seconds, rpc_address, logger):
 
     w3 = Web3(Web3.HTTPProvider(rpc_address))
-    account = w3.eth.account.privateKeyToAccount(private_key)
+    account = w3.eth.account.from_key(private_key)
     w3.eth.default_account = account.address
 
-    origin_realm_contract_address = Web3.toChecksumAddress(origin_realm_contract_address)
+    origin_realm_contract_address = Web3.to_checksum_address(origin_realm_contract_address)
     contract = w3.eth.contract(origin_realm_contract_address, abi=ABI)
 
     tx = contract.functions.sendHero(hero_id, destination_chain_id)
 
     if isinstance(gas_price_gwei, dict):   # dynamic fee
-        tx = tx.buildTransaction(
-            {'maxFeePerGas': w3.toWei(gas_price_gwei['maxFeePerGas'], 'gwei'),
-             'maxPriorityFeePerGas': w3.toWei(gas_price_gwei['maxPriorityFeePerGas'], 'gwei'),
+        tx = tx.build_transaction(
+            {'maxFeePerGas': w3.to_wei(gas_price_gwei['maxFeePerGas'], 'gwei'),
+             'maxPriorityFeePerGas': w3.to_wei(gas_price_gwei['maxPriorityFeePerGas'], 'gwei'),
              'value': bridge_fee_in_wei, 'nonce': nonce})
     else:   # legacy
-        tx = tx.buildTransaction({'gasPrice': w3.toWei(gas_price_gwei, 'gwei'), 'value': bridge_fee_in_wei, 'nonce': nonce})
+        tx = tx.build_transaction({'gasPrice': w3.to_wei(gas_price_gwei, 'gwei'), 'value': bridge_fee_in_wei, 'nonce': nonce})
 
     logger.debug("Signing transaction")
     signed_tx = w3.eth.account.sign_transaction(tx, private_key=private_key)
     logger.debug("Sending transaction " + str(tx))
     ret = w3.eth.send_raw_transaction(signed_tx.rawTransaction)
     logger.debug("Transaction successfully sent !")
     logger.info(
```

### Comparing `dfktools-0.2.0/src/dfktools/bridge_example.py` & `dfktools-0.3.0/src/dfktools/bridge_example.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,20 +18,20 @@
     private_key = None  # set private key
     tx_timeout = 30
     hero_id = 404
 
     # Serendale to Crystalvale
     gas_price_gwei = 115
     w3 = Web3(Web3.HTTPProvider(serendale_rpc_server))
-    account_address = w3.eth.account.privateKeyToAccount(private_key).address
+    account_address = w3.eth.account.from_key(private_key).address
     hero_bridge.send_hero(hero_bridge.SERENDALE_CONTRACT_ADDRESS, hero_id, hero_bridge.CRYSTALVALE_CHAIN_ID,
-                          w3.toWei(0.004, "ether"), private_key, w3.eth.getTransactionCount(account_address),
+                          w3.to_wei(0.004, "ether"), private_key, w3.eth.get_transaction_count(account_address),
                           gas_price_gwei, tx_timeout, serendale_rpc_server, logger)
 
     # Crystalvale to Serendale
     gas_price_gwei = {'maxFeePerGas': 2, 'maxPriorityFeePerGas': 2}  # EIP-1559
     w3 = Web3(Web3.HTTPProvider(crystalvale_rpc_server))
-    account_address = w3.eth.account.privateKeyToAccount(private_key).address
+    account_address = w3.eth.account.from_key(private_key).address
     hero_bridge.send_hero(hero_bridge.CRYSTALVALE_CONTRACT_ADDRESS, hero_id, hero_bridge.SERENDALE_CHAIN_ID,
-                          w3.toWei(0.05, "ether"), private_key,
-                          Web3(Web3.HTTPProvider(crystalvale_rpc_server)).eth.getTransactionCount(account_address),
+                          w3.to_wei(0.05, "ether"), private_key,
+                          Web3(Web3.HTTPProvider(crystalvale_rpc_server)).eth.get_transaction_count(account_address),
                           gas_price_gwei, tx_timeout, crystalvale_rpc_server, logger)
```

### Comparing `dfktools-0.2.0/src/dfktools/consumable/consumable.py` & `dfktools-0.3.0/src/dfktools/consumable/consumable.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,28 +26,28 @@
     else:
         return str(txid)
 
 
 def consume_item(consumable_contract_address, consumable_address, hero_id, private_key, nonce, gas_price_gwei, tx_timeout_seconds, rpc_address,
                  logger):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
-    account = w3.eth.account.privateKeyToAccount(private_key)
+    account = w3.eth.account.from_key(private_key)
     w3.eth.default_account = account.address
 
-    contract_address = Web3.toChecksumAddress(consumable_contract_address)
+    contract_address = Web3.to_checksum_address(consumable_contract_address)
     contract = w3.eth.contract(contract_address, abi=ABI)
 
     tx = contract.functions.consumeItem(consumable_address, hero_id)
 
     if isinstance(gas_price_gwei, dict):  # dynamic fee
-        tx = tx.buildTransaction(
-            {'maxFeePerGas': w3.toWei(gas_price_gwei['maxFeePerGas'], 'gwei'),
-             'maxPriorityFeePerGas': w3.toWei(gas_price_gwei['maxPriorityFeePerGas'], 'gwei'), 'nonce': nonce})
+        tx = tx.build_transaction(
+            {'maxFeePerGas': w3.to_wei(gas_price_gwei['maxFeePerGas'], 'gwei'),
+             'maxPriorityFeePerGas': w3.to_wei(gas_price_gwei['maxPriorityFeePerGas'], 'gwei'), 'nonce': nonce})
     else:  # legacy
-        tx = tx.buildTransaction({'gasPrice': w3.toWei(gas_price_gwei, 'gwei'), 'nonce': nonce})
+        tx = tx.build_transaction({'gasPrice': w3.to_wei(gas_price_gwei, 'gwei'), 'nonce': nonce})
 
     logger.debug("Signing transaction")
     signed_tx = w3.eth.account.sign_transaction(tx, private_key=private_key)
     logger.debug("Sending transaction " + str(tx))
     ret = w3.eth.send_raw_transaction(signed_tx.rawTransaction)
     logger.debug("Transaction successfully sent !")
     logger.info("Waiting for transaction " + block_explorer_link(consumable_contract_address, signed_tx.hash.hex()) + " to be mined")
```

### Comparing `dfktools-0.2.0/src/dfktools/consumable_example.py` & `dfktools-0.3.0/src/dfktools/consumable_example.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,13 +15,13 @@
     logger.info("Using RPC server " + rpc_server)
 
     stamina_vial_address = erc20.symbol2address('DFKSTMNPTN', 'sd2')
     realm_consumable_contract_address = consumable.SERENDALE2_CONTRACT_ADDRESS
 
     w3 = Web3(Web3.HTTPProvider(rpc_server))
     private_key = None  # set private key
-    account_address = w3.eth.account.privateKeyToAccount(private_key).address
+    account_address = w3.eth.account.from_key(private_key).address
     gas_price_gwei = 40
     tx_timeout_seconds = 30
 
     hero_id = 1
-    consumable.consume_item(realm_consumable_contract_address, stamina_vial_address, hero_id, private_key, w3.eth.getTransactionCount(account_address), gas_price_gwei, tx_timeout_seconds, rpc_server, logger)
+    consumable.consume_item(realm_consumable_contract_address, stamina_vial_address, hero_id, private_key, w3.eth.get_transaction_count(account_address), gas_price_gwei, tx_timeout_seconds, rpc_server, logger)
```

### Comparing `dfktools-0.2.0/src/dfktools/dex/crystal.py` & `dfktools-0.3.0/src/dfktools/dex/crystal.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,37 +20,37 @@
 def balance_of(address, rpc_address):
     return erc20_balance_of(address, CONTRACT_ADDRESS, rpc_address)
 
 
 def lock_of(address, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-    contract_address = Web3.toChecksumAddress(CONTRACT_ADDRESS)
+    contract_address = Web3.to_checksum_address(CONTRACT_ADDRESS)
     contract = w3.eth.contract(contract_address, abi=ABI)
 
-    return contract.functions.lockOf(Web3.toChecksumAddress(address)).call()
+    return contract.functions.lockOf(Web3.to_checksum_address(address)).call()
 
 
 def transfer_all(destination, private_key, nonce, gas_price_gwei, tx_timeout_seconds, rpc_address, logger):
 
     w3 = Web3(Web3.HTTPProvider(rpc_address))
-    account = w3.eth.account.privateKeyToAccount(private_key)
+    account = w3.eth.account.from_key(private_key)
     w3.eth.default_account = account.address
 
-    contract_address = Web3.toChecksumAddress(CONTRACT_ADDRESS)
+    contract_address = Web3.to_checksum_address(CONTRACT_ADDRESS)
     contract = w3.eth.contract(contract_address, abi=ABI)
 
     tx = contract.functions.transferAll(destination)
 
     if isinstance(gas_price_gwei, dict):  # dynamic fee
-        tx = tx.buildTransaction(
-            {'maxFeePerGas': w3.toWei(gas_price_gwei['maxFeePerGas'], 'gwei'),
-             'maxPriorityFeePerGas': w3.toWei(gas_price_gwei['maxPriorityFeePerGas'], 'gwei'), 'nonce': nonce})
+        tx = tx.build_transaction(
+            {'maxFeePerGas': w3.to_wei(gas_price_gwei['maxFeePerGas'], 'gwei'),
+             'maxPriorityFeePerGas': w3.to_wei(gas_price_gwei['maxPriorityFeePerGas'], 'gwei'), 'nonce': nonce})
     else:  # legacy
-        tx = tx.buildTransaction({'gasPrice': w3.toWei(gas_price_gwei, 'gwei'), 'nonce': nonce})
+        tx = tx.build_transaction({'gasPrice': w3.to_wei(gas_price_gwei, 'gwei'), 'nonce': nonce})
 
     logger.debug("Signing transaction")
     signed_tx = w3.eth.account.sign_transaction(tx, private_key=private_key)
     logger.debug("Sending transaction " + str(tx))
     ret = w3.eth.send_raw_transaction(signed_tx.rawTransaction)
     logger.debug("Transaction successfully sent !")
     logger.info("Waiting for transaction " + block_explorer_link(signed_tx.hash.hex()) + " to be mined")
```

### Comparing `dfktools-0.2.0/src/dfktools/dex/erc1155.py` & `dfktools-0.3.0/src/dfktools/dex/erc1155.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,21 +65,21 @@
 
 def copy_items(items):
     return items.copy()
 
 
 def balance_of(token_address, account_address, id, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
-    contract_address = Web3.toChecksumAddress(token_address)
+    contract_address = Web3.to_checksum_address(token_address)
     contract = w3.eth.contract(contract_address, abi=ABI)
     result = contract.functions.balanceOf(account_address, id).call()
 
     return result
 
 
 def uri(token_address, id, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
-    contract_address = Web3.toChecksumAddress(token_address)
+    contract_address = Web3.to_checksum_address(token_address)
     contract = w3.eth.contract(contract_address, abi=ABI)
     result = contract.functions.uri(id).call()
 
     return result
```

### Comparing `dfktools-0.2.0/src/dfktools/dex/erc20.py` & `dfktools-0.3.0/src/dfktools/dex/erc20.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,26 +172,29 @@
     ("0x5e4Cf6907CB5fBe2F642E399F6d07E567155d1F8", "DFKLVGRCR", "Lesser Vigor Crystal"),
     ("0xA71a120931526fC98f1AcC9f769b6b0d690fB8f0", "DFKVGRST", "Vigor Stone"),
     ("0x63891e0fcfEe0cEB12dE5fb96F43ADf9DbEC20a3", "DFKLVGRST", "Lesser Vigor Stone"),
     ("0xAeb5b59c8B90D4F078046550Cc8F9f08dC127253", "DFKWITCR", "Wit Crystal"),
     ("0xC989c916F189D2A2BE0322c020942d7c43aEa830", "DFKLWITCR", "Lesser Wit Crystal"),
     ("0x3971212Ec22147EE8808cB84F743DD852Be92f9C", "DFKWITST", "Wit Stone"),
     ("0xFC943eBd19112D6c6098412238E4E8319641B3d8", "DFKLWITST", "Lesser Wit Stone"),
+    ("0xAcDa84fAb3d3cdB38078b04901a26c103C37E7F4", "DFKREGTRT", "Regular Pet Treat"),
+    ("0x8Df3fFa5a677ba9737CE8Afcb8dd15Bd74085adD", "DFKPRMTRT", "Premium Pet Treat")
 ]
 
 
 ITEMS_SERENDALE2 = [
     ("0xB3F5867E277798b50ba7A71C0b24FDcA03045eDF", "JADE", "Jade"),
     ("0x30c103f8f5a3a732dfe2dce1cc9446f545527b43", "JEWEL", "Jewel"),
     ("0xaA8548665bCC12C202d5d0C700093123F2463EA6", "SJEWEL", "sJEWEL"),
     ("0xe7a1B580942148451E47b92e95aEB8d31B0acA37", "DFKGOLD", "DFK Gold"),
     ("0x8Be0cbA3c8c8F392408364ef21dfCF714A918234", "DFKTEARS", "Gaia's Tears"),
     ("0x75E8D8676d774C9429FbB148b30E304b5542aC3d", "DFKAMBRTFY", "Ambertaffy"),
     ("0xDbd4fA2D2C62C6c60957a126970e412Ed6AC1bD6", "DFKBLUESTEM", "Bluestem"),
     ("0xEDFBe9EEf42FfAf8909EC9Ce0d79850BA0C232FE", "DFKDRKWD", "Darkweed"),
+    ("0xeaF833A0Ae97897f6F69a728C9c17916296cecCA", "DFKGLDVN", "Goldvein"),
     ("0xBcdD90034eB73e7Aec2598ea9082d381a285f63b", "DFKIRONSCALE", "Ironscale"),
     ("0x80A42Dc2909C0873294c5E359e8DF49cf21c74E4", "DFKLANTERNEYE", "Lanterneye"),
     ("0xE408814828f2b51649473c1a05B861495516B920", "DFKMILKWEED", "Milkweed"),
     ("0xf2D479DaEdE7F9e270a90615F8b1C52F3C487bC7", "DFKRCKRT", "Rockroot"),
     ("0xc6030Afa09EDec1fd8e63a1dE10fC00E0146DaF3", "DFKSAILFISH", "Sailfish"),
     ("0xa61Bac689AD6867a605633520D70C49e1dCce853", "DFKSHIMMERSKIN", "Shimmerskin"),
     ("0x874FC0015ece1d77ba3D5668F16c46ba72913239", "DFKSKNSHADE", "Skunk Shade"),
@@ -257,15 +260,17 @@
     ("0x14a9D5a75799E4C6B4BfA65C8293a75e02DD5339", "DFKVGRCR", "Vigor Crystal"),
     ("0x6C7AF7483b050a00b5fbC4241eD06944c5f0bD77", "DFKLVGRCR", "Lesser Vigor Crystal"),
     ("0xA0c89fB3cbb115cf86EdcB4319578312D026A07a", "DFKVGRST", "Vigor Stone"),
     ("0x50F683acefA41b226CEfAdc0dd2ea6fFBfED56A0", "DFKLVGRST", "Lesser Vigor Stone"),
     ("0xf30214D43E55BE1cbaC712b49A75d4D3220302a7", "DFKWITCR", "Wit Crystal"),
     ("0xf15035b5eD13Feb18f63D829ABc1c3139041e7C2", "DFKLWITCR", "Lesser Wit Crystal"),
     ("0x3BaEFAfF21Fa2F06Ad3899903B7A899a91B5915A", "DFKWITST", "Wit Stone"),
-    ("0x5903F478e456DD4Ce5387caBE3984DfEf93D0A46", "DFKLWITST", "Lesser Wit Stone")
+    ("0x5903F478e456DD4Ce5387caBE3984DfEf93D0A46", "DFKLWITST", "Lesser Wit Stone"),
+    ("0x2F11e335224C5aBd3418B99922A9fe442F5696E9", "DFKREGTRT", "Regular Pet Treat"),
+    ("0xEec86C39e061B3Dec44f608Ff0ADA8053B8fFaDb", "DFKPRMTRT", "Premium Pet Treat")
 ]
 
 ABI = """
         [
             {"inputs":[{"internalType":"string","name":"_name","type":"string"},{"internalType":"string","name":"_symbol","type":"string"}],"stateMutability":"nonpayable","type":"constructor"},
             {"anonymous":false,"inputs":[{"indexed":true,"internalType":"address","name":"owner","type":"address"},{"indexed":true,"internalType":"address","name":"spender","type":"address"},{"indexed":false,"internalType":"uint256","name":"value","type":"uint256"}],"name":"Approval","type":"event"},
             {"anonymous":false,"inputs":[{"indexed":false,"internalType":"address","name":"account","type":"address"}],"name":"Paused","type":"event"},
@@ -303,19 +308,19 @@
             {"inputs":[{"internalType":"address","name":"sender","type":"address"},{"internalType":"address","name":"recipient","type":"address"},{"internalType":"uint256","name":"amount","type":"uint256"}],"name":"transferFrom","outputs":[{"internalType":"bool","name":"","type":"bool"}],"stateMutability":"nonpayable","type":"function"},
             {"inputs":[],"name":"unpause","outputs":[],"stateMutability":"nonpayable","type":"function"}
         ]
         """
 
 
 def wei2eth(w3, wei):
-    return w3.fromWei(wei, 'ether')
+    return w3.from_wei(wei, 'ether')
 
 
 def eth2wei(w3, eth):
-    return w3.toWei(eth, 'ether')
+    return w3.to_wei(eth, 'ether')
 
 
 def block_explorer_link(token_address, txid):
         return str(txid)
 
 
 def get_realm_item_list(realm):
@@ -374,63 +379,63 @@
     items = get_realm_item_list(realm)
     return items.copy()
 
 
 def symbol(token_address, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-    contract_address = Web3.toChecksumAddress(token_address)
+    contract_address = Web3.to_checksum_address(token_address)
     contract = w3.eth.contract(contract_address, abi=ABI)
 
     return contract.functions.symbol().call()
 
 
 def name(token_address, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-    contract_address = Web3.toChecksumAddress(token_address)
+    contract_address = Web3.to_checksum_address(token_address)
     contract = w3.eth.contract(contract_address, abi=ABI)
 
     return contract.functions.name().call()
 
 
 def decimals(token_address, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-    contract_address = Web3.toChecksumAddress(token_address)
+    contract_address = Web3.to_checksum_address(token_address)
     contract = w3.eth.contract(contract_address, abi=ABI)
 
     return contract.functions.decimals().call()
 
 
 def balance_of(address, token_address, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
-    contract_address = Web3.toChecksumAddress(token_address)
+    contract_address = Web3.to_checksum_address(token_address)
     contract = w3.eth.contract(contract_address, abi=ABI)
     result = contract.functions.balanceOf(address).call()
 
     return result
 
 
 def approve(token_address, private_key, nonce, gas_price_gwei, tx_timeout_seconds, rpc_address, logger):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
-    account = w3.eth.account.privateKeyToAccount(private_key)
+    account = w3.eth.account.from_key(private_key)
     w3.eth.default_account = account.address
 
-    contract_address = Web3.toChecksumAddress(token_address)
+    contract_address = Web3.to_checksum_address(token_address)
     contract = w3.eth.contract(contract_address, abi=ABI)
 
     tx = contract.functions.approve(account.address, sys.maxsize)
 
     if isinstance(gas_price_gwei, dict):  # dynamic fee
-        tx = tx.buildTransaction(
-            {'maxFeePerGas': w3.toWei(gas_price_gwei['maxFeePerGas'], 'gwei'),
-             'maxPriorityFeePerGas': w3.toWei(gas_price_gwei['maxPriorityFeePerGas'], 'gwei'), 'nonce': nonce})
+        tx = tx.build_transaction(
+            {'maxFeePerGas': w3.to_wei(gas_price_gwei['maxFeePerGas'], 'gwei'),
+             'maxPriorityFeePerGas': w3.to_wei(gas_price_gwei['maxPriorityFeePerGas'], 'gwei'), 'nonce': nonce})
     else:  # legacy
-        tx = tx.buildTransaction({'gasPrice': w3.toWei(gas_price_gwei, 'gwei'), 'nonce': nonce})
+        tx = tx.build_transaction({'gasPrice': w3.to_wei(gas_price_gwei, 'gwei'), 'nonce': nonce})
 
     logger.debug("Signing transaction")
     
     signed_tx = w3.eth.account.sign_transaction(tx, private_key=private_key)
     logger.debug("Sending transaction " + str(tx))
     
     ret = w3.eth.send_raw_transaction(signed_tx.rawTransaction)
@@ -443,28 +448,28 @@
     logger.info("Transaction mined !")
 
     return tx_receipt
 
 
 def transfer(token_address, private_key, nonce, dest_address, amount, gas_price_gwei, tx_timeout_seconds, rpc_address, logger):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
-    account = w3.eth.account.privateKeyToAccount(private_key)
+    account = w3.eth.account.from_key(private_key)
     w3.eth.default_account = account.address
 
-    contract_address = Web3.toChecksumAddress(token_address)
+    contract_address = Web3.to_checksum_address(token_address)
     contract = w3.eth.contract(contract_address, abi=ABI)
 
     tx = contract.functions.transferFrom(account.address, dest_address, amount)
 
     if isinstance(gas_price_gwei, dict):  # dynamic fee
-        tx = tx.buildTransaction(
-            {'maxFeePerGas': w3.toWei(gas_price_gwei['maxFeePerGas'], 'gwei'),
-             'maxPriorityFeePerGas': w3.toWei(gas_price_gwei['maxPriorityFeePerGas'], 'gwei'), 'nonce': nonce})
+        tx = tx.build_transaction(
+            {'maxFeePerGas': w3.to_wei(gas_price_gwei['maxFeePerGas'], 'gwei'),
+             'maxPriorityFeePerGas': w3.to_wei(gas_price_gwei['maxPriorityFeePerGas'], 'gwei'), 'nonce': nonce})
     else:  # legacy
-        tx = tx.buildTransaction({'gasPrice': w3.toWei(gas_price_gwei, 'gwei'), 'nonce': nonce})
+        tx = tx.build_transaction({'gasPrice': w3.to_wei(gas_price_gwei, 'gwei'), 'nonce': nonce})
 
     logger.debug("Signing transaction")
     
     signed_tx = w3.eth.account.sign_transaction(tx, private_key=private_key)
     logger.debug("Sending transaction " + str(tx))
     
     ret = w3.eth.send_raw_transaction(signed_tx.rawTransaction)
```

### Comparing `dfktools-0.2.0/src/dfktools/dex/item_erc1155.py` & `dfktools-0.3.0/src/dfktools/dex/item_erc1155.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,57 +70,57 @@
 
 def block_explorer_link(txid):
     return 'https://explorer.harmony.one/tx/' + str(txid)
 
 
 def balance_of(token_address, account_address, token_id, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
-    contract_address = Web3.toChecksumAddress(token_address)
+    contract_address = Web3.to_checksum_address(token_address)
     contract = w3.eth.contract(contract_address, abi=ABI)
     result = contract.functions.balanceOf(account_address, token_id).call()
 
     return result
 
 
 def decimals(token_address, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
-    contract_address = Web3.toChecksumAddress(token_address)
+    contract_address = Web3.to_checksum_address(token_address)
     contract = w3.eth.contract(contract_address, abi=ABI)
     result = contract.functions.decimals().call()
 
     return result
 
 
 def symbol(token_address, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
-    contract_address = Web3.toChecksumAddress(token_address)
+    contract_address = Web3.to_checksum_address(token_address)
     contract = w3.eth.contract(contract_address, abi=ABI)
     result = contract.functions.symbol().call()
 
     return result
 
 
 def uri(token_address, token_id, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
-    contract_address = Web3.toChecksumAddress(token_address)
+    contract_address = Web3.to_checksum_address(token_address)
     contract = w3.eth.contract(contract_address, abi=ABI)
     result = contract.functions.uri(token_id).call()
 
     return result
 
 
 def mint(token_address, receiver_address, token_id, amount, data, private_key, nonce, gas_price_gwei, tx_timeout_seconds, rpc_address, logger):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
-    account = w3.eth.account.privateKeyToAccount(private_key)
+    account = w3.eth.account.from_key(private_key)
     w3.eth.default_account = account.address
 
-    contract_address = Web3.toChecksumAddress(token_address)
+    contract_address = Web3.to_checksum_address(token_address)
     contract = w3.eth.contract(contract_address, abi=ABI)
-    tx = contract.functions.mint(receiver_address, token_id, amount, data).buildTransaction(
-        {'gasPrice': w3.toWei(gas_price_gwei, 'gwei'), 'nonce': nonce})
+    tx = contract.functions.mint(receiver_address, token_id, amount, data).build_transaction(
+        {'gasPrice': w3.to_wei(gas_price_gwei, 'gwei'), 'nonce': nonce})
     logger.debug("Signing transaction")
     signed_tx = w3.eth.account.sign_transaction(tx, private_key=private_key)
     logger.debug("Sending transaction " + str(tx))
     ret = w3.eth.send_raw_transaction(signed_tx.rawTransaction)
     logger.debug("Transaction successfully sent !")
     logger.info("Waiting for transaction " + block_explorer_link(signed_tx.hash.hex()) + " to be mined")
     tx_receipt = w3.eth.wait_for_transaction_receipt(transaction_hash=signed_tx.hash, timeout=tx_timeout_seconds,
```

### Comparing `dfktools-0.2.0/src/dfktools/dex/jade.py` & `dfktools-0.3.0/src/dfktools/dex/jade.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,37 +20,37 @@
 def balance_of(address, rpc_address):
     return erc20_balance_of(address, CONTRACT_ADDRESS, rpc_address)
 
 
 def lock_of(address, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-    contract_address = Web3.toChecksumAddress(CONTRACT_ADDRESS)
+    contract_address = Web3.to_checksum_address(CONTRACT_ADDRESS)
     contract = w3.eth.contract(contract_address, abi=ABI)
 
-    return contract.functions.lockOf(Web3.toChecksumAddress(address)).call()
+    return contract.functions.lockOf(Web3.to_checksum_address(address)).call()
 
 
 def transfer_all(destination, private_key, nonce, gas_price_gwei, tx_timeout_seconds, rpc_address, logger):
 
     w3 = Web3(Web3.HTTPProvider(rpc_address))
-    account = w3.eth.account.privateKeyToAccount(private_key)
+    account = w3.eth.account.from_key(private_key)
     w3.eth.default_account = account.address
 
-    contract_address = Web3.toChecksumAddress(CONTRACT_ADDRESS)
+    contract_address = Web3.to_checksum_address(CONTRACT_ADDRESS)
     contract = w3.eth.contract(contract_address, abi=ABI)
 
     tx = contract.functions.transferAll(destination)
 
     if isinstance(gas_price_gwei, dict):  # dynamic fee
-        tx = tx.buildTransaction(
-            {'maxFeePerGas': w3.toWei(gas_price_gwei['maxFeePerGas'], 'gwei'),
-             'maxPriorityFeePerGas': w3.toWei(gas_price_gwei['maxPriorityFeePerGas'], 'gwei'), 'nonce': nonce})
+        tx = tx.build_transaction(
+            {'maxFeePerGas': w3.to_wei(gas_price_gwei['maxFeePerGas'], 'gwei'),
+             'maxPriorityFeePerGas': w3.to_wei(gas_price_gwei['maxPriorityFeePerGas'], 'gwei'), 'nonce': nonce})
     else:  # legacy
-        tx = tx.buildTransaction({'gasPrice': w3.toWei(gas_price_gwei, 'gwei'), 'nonce': nonce})
+        tx = tx.build_transaction({'gasPrice': w3.to_wei(gas_price_gwei, 'gwei'), 'nonce': nonce})
 
     logger.debug("Signing transaction")
     signed_tx = w3.eth.account.sign_transaction(tx, private_key=private_key)
     logger.debug("Sending transaction " + str(tx))
     ret = w3.eth.send_raw_transaction(signed_tx.rawTransaction)
     logger.debug("Transaction successfully sent !")
     logger.info("Waiting for transaction " + block_explorer_link(signed_tx.hash.hex()) + " to be mined")
```

### Comparing `dfktools-0.2.0/src/dfktools/dex/jewel.py` & `dfktools-0.3.0/src/dfktools/dex/jewel.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,37 +20,37 @@
 def balance_of(address, rpc_address):
     return erc20_balance_of(address, CONTRACT_ADDRESS, rpc_address)
 
 
 def lock_of(address, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-    contract_address = Web3.toChecksumAddress(CONTRACT_ADDRESS)
+    contract_address = Web3.to_checksum_address(CONTRACT_ADDRESS)
     contract = w3.eth.contract(contract_address, abi=ABI)
 
-    return contract.functions.lockOf(Web3.toChecksumAddress(address)).call()
+    return contract.functions.lockOf(Web3.to_checksum_address(address)).call()
 
 
 def transfer_all(destination, private_key, nonce, gas_price_gwei, tx_timeout_seconds, rpc_address, logger):
 
     w3 = Web3(Web3.HTTPProvider(rpc_address))
-    account = w3.eth.account.privateKeyToAccount(private_key)
+    account = w3.eth.account.from_key(private_key)
     w3.eth.default_account = account.address
 
-    contract_address = Web3.toChecksumAddress(CONTRACT_ADDRESS)
+    contract_address = Web3.to_checksum_address(CONTRACT_ADDRESS)
     contract = w3.eth.contract(contract_address, abi=ABI)
 
     tx = contract.functions.transferAll(destination)
 
     if isinstance(gas_price_gwei, dict):  # dynamic fee
-        tx = tx.buildTransaction(
-            {'maxFeePerGas': w3.toWei(gas_price_gwei['maxFeePerGas'], 'gwei'),
-             'maxPriorityFeePerGas': w3.toWei(gas_price_gwei['maxPriorityFeePerGas'], 'gwei'), 'nonce': nonce})
+        tx = tx.build_transaction(
+            {'maxFeePerGas': w3.to_wei(gas_price_gwei['maxFeePerGas'], 'gwei'),
+             'maxPriorityFeePerGas': w3.to_wei(gas_price_gwei['maxPriorityFeePerGas'], 'gwei'), 'nonce': nonce})
     else:  # legacy
-        tx = tx.buildTransaction({'gasPrice': w3.toWei(gas_price_gwei, 'gwei'), 'nonce': nonce})
+        tx = tx.build_transaction({'gasPrice': w3.to_wei(gas_price_gwei, 'gwei'), 'nonce': nonce})
 
     logger.debug("Signing transaction")
     signed_tx = w3.eth.account.sign_transaction(tx, private_key=private_key)
     logger.debug("Sending transaction " + str(tx))
     ret = w3.eth.send_raw_transaction(signed_tx.rawTransaction)
     logger.debug("Transaction successfully sent !")
     logger.info("Waiting for transaction " + block_explorer_link(signed_tx.hash.hex()) + " to be mined")
```

### Comparing `dfktools-0.2.0/src/dfktools/dex/master_gardener.py` & `dfktools-0.3.0/src/dfktools/dex/master_gardener.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,24 +90,24 @@
     ]
     '''
 
 
 def pool_length(contract_address, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-    contract_address = Web3.toChecksumAddress(contract_address)
+    contract_address = Web3.to_checksum_address(contract_address)
     contract = w3.eth.contract(contract_address, abi=ABI)
 
     return contract.functions.poolLength().call()
 
 
 def pool_info(contract_address, pool_id, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-    contract_address = Web3.toChecksumAddress(contract_address)
+    contract_address = Web3.to_checksum_address(contract_address)
     contract = w3.eth.contract(contract_address, abi=ABI)
 
     return contract.functions.poolInfo(pool_id).call()
 
 
 def pool_id1(contract_address, pool_address, rpc_address):
     """
@@ -115,24 +115,24 @@
     :param contract_address:
     :param pool_address:
     :param rpc_address:
     :return:
     """
     w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-    contract_address = Web3.toChecksumAddress(contract_address)
+    contract_address = Web3.to_checksum_address(contract_address)
     contract = w3.eth.contract(contract_address, abi=ABI)
 
     return contract.functions.poolId1(pool_address).call()
 
 
 def user_info(contract_address, pool_id, user_address, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-    contract_address = Web3.toChecksumAddress(contract_address)
+    contract_address = Web3.to_checksum_address(contract_address)
     contract = w3.eth.contract(contract_address, abi=ABI)
 
     return contract.functions.userInfo(pool_id, user_address).call()
 
 
 class Garden:
     def __init__(self, garden_contract_address, uniswap_v2_pair, rpc_address, logger):
```

### Comparing `dfktools-0.2.0/src/dfktools/dex/uniswap_v2_factory.py` & `dfktools-0.3.0/src/dfktools/dex/uniswap_v2_factory.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,35 +25,35 @@
     """
 
 
 def all_pairs_length(contract_address, rpc_address):
 
     w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-    contract_address = Web3.toChecksumAddress(contract_address)
+    contract_address = Web3.to_checksum_address(contract_address)
     contract = w3.eth.contract(contract_address, abi=ABI)
 
     return contract.functions.allPairsLength().call()
 
 
 def all_pairs(contract_address, index, rpc_address):
     '''
     Return the address of the liquidity pair at index
     :param index:
     :param rpc_address:
     :return:
     '''
     w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-    contract_address = Web3.toChecksumAddress(contract_address)
+    contract_address = Web3.to_checksum_address(contract_address)
     contract = w3.eth.contract(contract_address, abi=ABI)
 
     return contract.functions.allPairs(index).call()
 
 
 def get_pair(contract_address, token_address_1, token_address_2, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-    contract_address = Web3.toChecksumAddress(contract_address)
+    contract_address = Web3.to_checksum_address(contract_address)
     contract = w3.eth.contract(contract_address, abi=ABI)
 
     return contract.functions.getPair(token_address_1, token_address_2).call()
```

### Comparing `dfktools-0.2.0/src/dfktools/dex/uniswap_v2_pair.py` & `dfktools-0.3.0/src/dfktools/dex/uniswap_v2_pair.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,28 +47,28 @@
 
 def block_explorer_link(txid):
     return 'https://explorer.harmony.one/tx/' + str(txid)
 
 
 def swap(pool_address, amount0_out, amount1_out, to, private_key, nonce, gas_price_gwei, tx_timeout_seconds, rpc_address, logger):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
-    account = w3.eth.account.privateKeyToAccount(private_key)
+    account = w3.eth.account.from_key(private_key)
     w3.eth.default_account = account.address
 
-    contract_address = Web3.toChecksumAddress(pool_address)
+    contract_address = Web3.to_checksum_address(pool_address)
     contract = w3.eth.contract(contract_address, abi=ABI)
 
     tx = contract.functions.startQuestWithData(amount0_out, amount1_out, to, None)
 
     if isinstance(gas_price_gwei, dict):  # dynamic fee
-        tx = tx.buildTransaction(
-            {'maxFeePerGas': w3.toWei(gas_price_gwei['maxFeePerGas'], 'gwei'),
-             'maxPriorityFeePerGas': w3.toWei(gas_price_gwei['maxPriorityFeePerGas'], 'gwei'), 'nonce': nonce})
+        tx = tx.build_transaction(
+            {'maxFeePerGas': w3.to_wei(gas_price_gwei['maxFeePerGas'], 'gwei'),
+             'maxPriorityFeePerGas': w3.to_wei(gas_price_gwei['maxPriorityFeePerGas'], 'gwei'), 'nonce': nonce})
     else:  # legacy
-        tx = tx.buildTransaction({'gasPrice': w3.toWei(gas_price_gwei, 'gwei'), 'nonce': nonce})
+        tx = tx.build_transaction({'gasPrice': w3.to_wei(gas_price_gwei, 'gwei'), 'nonce': nonce})
 
     logger.debug("Signing transaction")
     signed_tx = w3.eth.account.sign_transaction(tx, private_key=private_key)
     logger.debug("Sending transaction " + str(tx))
     ret = w3.eth.send_raw_transaction(signed_tx.rawTransaction)
     logger.debug("Transaction successfully sent !")
     logger.info(
@@ -80,60 +80,60 @@
 
     return tx_receipt
 
 
 def name(pool_address, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-    contract_address = Web3.toChecksumAddress(pool_address)
+    contract_address = Web3.to_checksum_address(pool_address)
     contract = w3.eth.contract(contract_address, abi=ABI)
 
     return contract.functions.symbol().call()
 
 
 def symbol(pool_address, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-    contract_address = Web3.toChecksumAddress(pool_address)
+    contract_address = Web3.to_checksum_address(pool_address)
     contract = w3.eth.contract(contract_address, abi=ABI)
 
     return contract.functions.symbol().call()
 
 
 def token_0(pool_address, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-    contract_address = Web3.toChecksumAddress(pool_address)
+    contract_address = Web3.to_checksum_address(pool_address)
     contract = w3.eth.contract(contract_address, abi=ABI)
 
     return contract.functions.token0().call()
 
 
 def token_1(pool_address, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-    contract_address = Web3.toChecksumAddress(pool_address)
+    contract_address = Web3.to_checksum_address(pool_address)
     contract = w3.eth.contract(contract_address, abi=ABI)
 
     return contract.functions.token1().call()
 
 
 def decimals(pool_address, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-    contract_address = Web3.toChecksumAddress(pool_address)
+    contract_address = Web3.to_checksum_address(pool_address)
     contract = w3.eth.contract(contract_address, abi=ABI)
 
     return contract.functions.decimals().call()
 
 
 def total_supply(pool_address, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-    contract_address = Web3.toChecksumAddress(pool_address)
+    contract_address = Web3.to_checksum_address(pool_address)
     contract = w3.eth.contract(contract_address, abi=ABI)
 
     return contract.functions.totalSupply().call()
 
 
 def get_reserves(pool_address, rpc_address):
     '''
@@ -141,42 +141,42 @@
     Also returns the block.timestamp (mod 2**32) of the last block during which an interaction occurred for the pair.
     :param pool_address:
     :param rpc_address:
     :return: reserve0, reserve1, blockTimestampLast
     '''
     w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-    contract_address = Web3.toChecksumAddress(pool_address)
+    contract_address = Web3.to_checksum_address(pool_address)
     contract = w3.eth.contract(contract_address, abi=ABI)
 
     return contract.functions.getReserves().call()
 
 
 def balance_of(pool_address, owner_address, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-    contract_address = Web3.toChecksumAddress(pool_address)
+    contract_address = Web3.to_checksum_address(pool_address)
     contract = w3.eth.contract(contract_address, abi=ABI)
 
     return contract.functions.balanceOf(owner_address).call()
 
 
 def price_0_cumulative_last(pool_address, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-    contract_address = Web3.toChecksumAddress(pool_address)
+    contract_address = Web3.to_checksum_address(pool_address)
     contract = w3.eth.contract(contract_address, abi=ABI)
 
     return contract.functions.price0CumulativeLast().call()
 
 
 def price_1_cumulative_last(pool_address, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-    contract_address = Web3.toChecksumAddress(pool_address)
+    contract_address = Web3.to_checksum_address(pool_address)
     contract = w3.eth.contract(contract_address, abi=ABI)
 
     return contract.functions.price1CumulativeLast().call()
 
 
 class UniswapV2Pair:
     def __init__(self, pair_address, rpc_address, logger):
```

### Comparing `dfktools-0.2.0/src/dfktools/dex/uniswap_v2_router.py` & `dfktools-0.3.0/src/dfktools/dex/uniswap_v2_router.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,51 +47,51 @@
     :param router_contract_address:
     :param rpc_address:
     :return:
     """
 
     w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-    contract_address = Web3.toChecksumAddress(router_contract_address)
+    contract_address = Web3.to_checksum_address(router_contract_address)
     contract = w3.eth.contract(contract_address, abi=ABI)
 
     return contract.functions.WETH().call()
 
 
 def factory(router_contract_address, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-    contract_address = Web3.toChecksumAddress(router_contract_address)
+    contract_address = Web3.to_checksum_address(router_contract_address)
     contract = w3.eth.contract(contract_address, abi=ABI)
 
     return contract.functions.factory().call()
 
 
 def quote(router_contract_address, amount_a, reserve_a, reserve_b, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-    contract_address = Web3.toChecksumAddress(router_contract_address)
+    contract_address = Web3.to_checksum_address(router_contract_address)
     contract = w3.eth.contract(contract_address, abi=ABI)
 
     return contract.functions.quote(amount_a, reserve_a, reserve_b).call()
 
 
 def get_amount_in(router_contract_address, amount_out, reserve_in, reserve_out, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-    contract_address = Web3.toChecksumAddress(router_contract_address)
+    contract_address = Web3.to_checksum_address(router_contract_address)
     contract = w3.eth.contract(contract_address, abi=ABI)
 
     return contract.functions.getAmountIn(amount_out, reserve_in, reserve_out).call()
 
 
 def get_amount_out(router_contract_address, amount_in, reserve_in, reserve_out, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-    contract_address = Web3.toChecksumAddress(router_contract_address)
+    contract_address = Web3.to_checksum_address(router_contract_address)
     contract = w3.eth.contract(contract_address, abi=ABI)
 
     return contract.functions.getAmountOut(amount_in, reserve_in, reserve_out).call()
 
 
 def swap_exact_tokens_for_tokens(router_contract_address, amount_in, amount_out_min, path, to, deadline, private_key, nonce, gas_price_gwei, tx_timeout_seconds, rpc_address, logger):
     """
@@ -109,27 +109,27 @@
     :param gas_price_gwei:
     :param tx_timeout_seconds:
     :param rpc_address:
     :param logger:
     :return:
     """
     w3 = Web3(Web3.HTTPProvider(rpc_address))
-    account = w3.eth.account.privateKeyToAccount(private_key)
+    account = w3.eth.account.from_key(private_key)
     w3.eth.default_account = account.address
 
-    contract_address = Web3.toChecksumAddress(router_contract_address)
+    contract_address = Web3.to_checksum_address(router_contract_address)
     contract = w3.eth.contract(contract_address, abi=ABI)
     if isinstance(gas_price_gwei, dict):
-        tx = contract.functions.swapExactTokensForTokens(amount_in, amount_out_min, path, to, deadline).buildTransaction(
-            {'maxFeePerGas': w3.toWei(gas_price_gwei['maxFeePerGas'], 'gwei'),
-            'maxPriorityFeePerGas': w3.toWei(gas_price_gwei['maxPriorityFeePerGas'], 'gwei'),
+        tx = contract.functions.swapExactTokensForTokens(amount_in, amount_out_min, path, to, deadline).build_transaction(
+            {'maxFeePerGas': w3.to_wei(gas_price_gwei['maxFeePerGas'], 'gwei'),
+            'maxPriorityFeePerGas': w3.to_wei(gas_price_gwei['maxPriorityFeePerGas'], 'gwei'),
             'nonce': nonce})
     else: # legacy 
-        tx = contract.functions.swapExactTokensForTokens(amount_in, amount_out_min, path, to, deadline).buildTransaction(
-            {'gasPrice': w3.toWei(gas_price_gwei, 'gwei'), 'nonce': nonce})
+        tx = contract.functions.swapExactTokensForTokens(amount_in, amount_out_min, path, to, deadline).build_transaction(
+            {'gasPrice': w3.to_wei(gas_price_gwei, 'gwei'), 'nonce': nonce})
     logger.debug("Signing transaction")
     signed_tx = w3.eth.account.sign_transaction(tx, private_key=private_key)
     logger.debug("Sending transaction " + str(tx))
     ret = w3.eth.send_raw_transaction(signed_tx.rawTransaction)
     logger.debug("Transaction successfully sent !")
     logger.info(
         "Waiting for transaction " + block_explorer_link(signed_tx.hash.hex()) + " to be mined")
@@ -157,28 +157,28 @@
     :param gas_price_gwei:
     :param tx_timeout_seconds:
     :param rpc_address:
     :param logger:
     :return:
     """
     w3 = Web3(Web3.HTTPProvider(rpc_address))
-    account = w3.eth.account.privateKeyToAccount(private_key)
+    account = w3.eth.account.from_key(private_key)
     w3.eth.default_account = account.address
 
-    contract_address = Web3.toChecksumAddress(router_contract_address)
+    contract_address = Web3.to_checksum_address(router_contract_address)
     contract = w3.eth.contract(contract_address, abi=ABI)
 
     if isinstance(gas_price_gwei, dict):
-        tx = contract.functions.swapExactTokensForETH(amount_in, amount_out_min, path, to, deadline).buildTransaction(
-            {'maxFeePerGas': w3.toWei(gas_price_gwei['maxFeePerGas'], 'gwei'),
-            'maxPriorityFeePerGas': w3.toWei(gas_price_gwei['maxPriorityFeePerGas'], 'gwei'),
+        tx = contract.functions.swapExactTokensForETH(amount_in, amount_out_min, path, to, deadline).build_transaction(
+            {'maxFeePerGas': w3.to_wei(gas_price_gwei['maxFeePerGas'], 'gwei'),
+            'maxPriorityFeePerGas': w3.to_wei(gas_price_gwei['maxPriorityFeePerGas'], 'gwei'),
             'nonce': nonce})
     else: # legacy 
-        tx = contract.functions.swapExactTokensForETH(amount_in, amount_out_min, path, to, deadline).buildTransaction(
-            {'gasPrice': w3.toWei(gas_price_gwei, 'gwei'), 'nonce': nonce})
+        tx = contract.functions.swapExactTokensForETH(amount_in, amount_out_min, path, to, deadline).build_transaction(
+            {'gasPrice': w3.to_wei(gas_price_gwei, 'gwei'), 'nonce': nonce})
     logger.debug("Signing transaction")
     signed_tx = w3.eth.account.sign_transaction(tx, private_key=private_key)
     logger.debug("Sending transaction " + str(tx))
     ret = w3.eth.send_raw_transaction(signed_tx.rawTransaction)
     logger.debug("Transaction successfully sent !")
     logger.info(
         "Waiting for transaction " + block_explorer_link(signed_tx.hash.hex()) + " to be mined")
```

### Comparing `dfktools-0.2.0/src/dfktools/dex/utils/utils.py` & `dfktools-0.3.0/src/dfktools/dex/utils/utils.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.2.0/src/dfktools/dex_example.py` & `dfktools-0.3.0/src/dfktools/dex_example.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,11 +60,11 @@
     staking_pool_balance = gardens.Garden.user_info_lp_balance(staking_pool_user)
     staking_pool_share = staking_pool_balance/staking_pool_total_supply
     logger.info("LP staked user balance:\t" + str(
         erc20.wei2eth(w3, staking_pool_balance)) + " (pool share " + str(round(100 * staking_pool_share, 2)) + "%)")
 
     # Swap JEWEL for ONE
     #private_key = None #set private key of to swap coin from
-    #account_address = w3.eth.account.privateKeyToAccount(private_key).address
+    #account_address = w3.eth.account.from_key(private_key).address
     #market_place_router.swap_exact_tokens_for_eth(erc20.eth2wei(w3, 1), 60, [erc20.JEWEL, market_place_router.weth(rpc_server)], account_address,
-    #                                 int(time.time() + 60), private_key, w3.eth.getTransactionCount(account_address),
-    #                                 w3.fromWei(w3.eth.gas_price, 'gwei'), 30, rpc_server, logger)
+    #                                 int(time.time() + 60), private_key, w3.eth.get_transaction_count(account_address),
+    #                                 w3.from_wei(w3.eth.gas_price, 'gwei'), 30, rpc_server, logger)
```

### Comparing `dfktools-0.2.0/src/dfktools/duel/duel.py` & `dfktools-0.3.0/src/dfktools/duel/duel.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     #    return 'https://scope.klaytn.com/tx/' + str(txid)
     else:
         return str(txid)
 
 
 def get_duel(duel_id, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
-    contract_address = Web3.toChecksumAddress(SERENDALE_CONTRACT_ADDRESS)
+    contract_address = Web3.to_checksum_address(SERENDALE_CONTRACT_ADDRESS)
     contract = w3.eth.contract(contract_address, abi=ABI)
     contract_entry = contract.functions.getDuel(duel_id).call()
 
     duel = {}
     duel['id'] = contract_entry[0]
     duel['player1'] = str(contract_entry[1])
     duel['player2'] = str(contract_entry[2])
@@ -43,15 +43,15 @@
     duel['status'] = contract_entry[10]
 
     return duel
 
 
 def get_duel_entry(duel_entry_id, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
-    contract_address = Web3.toChecksumAddress(SERENDALE_CONTRACT_ADDRESS)
+    contract_address = Web3.to_checksum_address(SERENDALE_CONTRACT_ADDRESS)
     contract = w3.eth.contract(contract_address, abi=ABI)
     contract_entry = contract.functions.getDuelEntry(duel_entry_id).call()
 
     duel = {}
     duel['id'] = contract_entry[0]
     duel['player'] = str(contract_entry[1])
     duel['heroes'] = contract_entry[2]
@@ -66,17 +66,17 @@
     duel['status'] = contract_entry[11]
 
     return duel
 
 
 def get_duel_history(address, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
-    contract_address = Web3.toChecksumAddress(SERENDALE_CONTRACT_ADDRESS)
+    contract_address = Web3.to_checksum_address(SERENDALE_CONTRACT_ADDRESS)
     contract = w3.eth.contract(contract_address, abi=ABI)
-    contract_entry = contract.functions.getDuelHistory(Web3.toChecksumAddress(address)).call()
+    contract_entry = contract.functions.getDuelHistory(Web3.to_checksum_address(address)).call()
 
     duels = []
 
     for item in contract_entry:
         duel = {}
         if item[0] == 0:
             continue
@@ -95,17 +95,17 @@
         duels.append(duel)
 
     return duels
 
 
 def get_active_duels(address, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
-    contract_address = Web3.toChecksumAddress(SERENDALE_CONTRACT_ADDRESS)
+    contract_address = Web3.to_checksum_address(SERENDALE_CONTRACT_ADDRESS)
     contract = w3.eth.contract(contract_address, abi=ABI)
-    contract_entry = contract.functions.getActiveDuels(Web3.toChecksumAddress(address)).call()
+    contract_entry = contract.functions.getActiveDuels(Web3.to_checksum_address(address)).call()
 
     duels = []
 
     for item in contract_entry:
         duel = {}
         if item[0] == 0:
             continue
@@ -124,17 +124,17 @@
         duels.append(duel)
 
     return duels
 
 
 def get_challenges(address, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
-    contract_address = Web3.toChecksumAddress(SERENDALE_CONTRACT_ADDRESS)
+    contract_address = Web3.to_checksum_address(SERENDALE_CONTRACT_ADDRESS)
     contract = w3.eth.contract(contract_address, abi=ABI)
-    contract_entry = contract.functions.getChallenges(Web3.toChecksumAddress(address)).call()
+    contract_entry = contract.functions.getChallenges(Web3.to_checksum_address(address)).call()
 
     duels = []
 
     for item in contract_entry:
         duel = {}
         if item[0] == 0:
             continue
@@ -153,22 +153,22 @@
         duels.append(duel)
 
     return duels
 
 
 def get_duel_index_p1(duel_id, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
-    contract_address = Web3.toChecksumAddress(SERENDALE_CONTRACT_ADDRESS)
+    contract_address = Web3.to_checksum_address(SERENDALE_CONTRACT_ADDRESS)
     contract = w3.eth.contract(contract_address, abi=ABI)
     return contract.functions.getDuelIndexP1(duel_id).call()
 
 
 def get_duel_turns(duel_id, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
-    contract_address = Web3.toChecksumAddress(SERENDALE_CONTRACT_ADDRESS)
+    contract_address = Web3.to_checksum_address(SERENDALE_CONTRACT_ADDRESS)
     contract = w3.eth.contract(contract_address, abi=ABI)
     contract_entry = contract.functions.getDuelTurns(duel_id).call()
 
     duels = []
 
     for item in contract_entry:
         duel = {}
@@ -200,15 +200,15 @@
         duels.append(duel)
 
     return duels
 
 
 def get_hero_duel(hero_id, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
-    contract_address = Web3.toChecksumAddress(SERENDALE_CONTRACT_ADDRESS)
+    contract_address = Web3.to_checksum_address(SERENDALE_CONTRACT_ADDRESS)
     contract = w3.eth.contract(contract_address, abi=ABI)
     contract_entry = contract.functions.getHeroDuel(hero_id).call()
 
     duel = {}
     duel['id'] = contract_entry[0]
     duel['player1'] = str(contract_entry[1])
     duel['player2'] = str(contract_entry[2])
@@ -222,75 +222,75 @@
     duel['status'] = contract_entry[10]
 
     return duel
 
 
 def get_highest_score(rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
-    contract_address = Web3.toChecksumAddress(SERENDALE_CONTRACT_ADDRESS)
+    contract_address = Web3.to_checksum_address(SERENDALE_CONTRACT_ADDRESS)
     contract = w3.eth.contract(contract_address, abi=ABI)
     return contract.functions.getHighestScore().call()
 
 
 def get_player_score(address, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
-    contract_address = Web3.toChecksumAddress(SERENDALE_CONTRACT_ADDRESS)
+    contract_address = Web3.to_checksum_address(SERENDALE_CONTRACT_ADDRESS)
     contract = w3.eth.contract(contract_address, abi=ABI)
-    return contract.functions.getPlayerScore(Web3.toChecksumAddress(address)).call()
+    return contract.functions.getPlayerScore(Web3.to_checksum_address(address)).call()
 
 
 def get_total_duel_entries(rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
-    contract_address = Web3.toChecksumAddress(SERENDALE_CONTRACT_ADDRESS)
+    contract_address = Web3.to_checksum_address(SERENDALE_CONTRACT_ADDRESS)
     contract = w3.eth.contract(contract_address, abi=ABI)
     return contract.functions.getTotalDuelEntries().call()
 
 
 def get_total_duels(rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
-    contract_address = Web3.toChecksumAddress(SERENDALE_CONTRACT_ADDRESS)
+    contract_address = Web3.to_checksum_address(SERENDALE_CONTRACT_ADDRESS)
     contract = w3.eth.contract(contract_address, abi=ABI)
     return contract.functions.getTotalDuels().call()
 
 
 def get_total_open_duel_entries(lobby_id, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
-    contract_address = Web3.toChecksumAddress(SERENDALE_CONTRACT_ADDRESS)
+    contract_address = Web3.to_checksum_address(SERENDALE_CONTRACT_ADDRESS)
     contract = w3.eth.contract(contract_address, abi=ABI)
     return contract.functions.getTotalOpenDuelEntries(lobby_id).call()
 
 
 def get_total_player_duels(address, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
-    contract_address = Web3.toChecksumAddress(SERENDALE_CONTRACT_ADDRESS)
+    contract_address = Web3.to_checksum_address(SERENDALE_CONTRACT_ADDRESS)
     contract = w3.eth.contract(contract_address, abi=ABI)
-    return contract.functions.getTotalPlayerDuels(Web3.toChecksumAddress(address)).call()
+    return contract.functions.getTotalPlayerDuels(Web3.to_checksum_address(address)).call()
 
 
 def get_total_player_wins(address, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
-    contract_address = Web3.toChecksumAddress(SERENDALE_CONTRACT_ADDRESS)
+    contract_address = Web3.to_checksum_address(SERENDALE_CONTRACT_ADDRESS)
     contract = w3.eth.contract(contract_address, abi=ABI)
-    return contract.functions.getTotalPlayerWins(Web3.toChecksumAddress(address)).call()
+    return contract.functions.getTotalPlayerWins(Web3.to_checksum_address(address)).call()
 
 
 def start_private_duel(duel_type, hero_ids, opponent, background, stat, private_key, nonce, gas_price_gwei,
                        tx_timeout_seconds, rpc_address, logger):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
-    account = w3.eth.account.privateKeyToAccount(private_key)
+    account = w3.eth.account.from_key(private_key)
     w3.eth.default_account = account.address
 
-    contract_address = Web3.toChecksumAddress(SERENDALE_CONTRACT_ADDRESS)
+    contract_address = Web3.to_checksum_address(SERENDALE_CONTRACT_ADDRESS)
     contract = w3.eth.contract(contract_address, abi=ABI)
 
     tx = contract.functions.startPrivateDuel(duel_utils.string2id('type', duel_type), hero_ids, opponent,
                                              duel_utils.string2id('background', background),
                                              duel_utils.string2id('stat', stat)
-                                             ).buildTransaction(
-        {'gasPrice': w3.toWei(gas_price_gwei, 'gwei'), 'nonce': nonce})
+                                             ).build_transaction(
+        {'gasPrice': w3.to_wei(gas_price_gwei, 'gwei'), 'nonce': nonce})
 
     logger.debug("Signing transaction")
     signed_tx = w3.eth.account.sign_transaction(tx, private_key=private_key)
     logger.debug("Sending transaction " + str(tx))
     ret = w3.eth.send_raw_transaction(signed_tx.rawTransaction)
     logger.debug("Transaction successfully sent !")
     logger.info("Waiting for transaction " + block_explorer_link(signed_tx.hash.hex()) + " to be mined")
@@ -300,26 +300,26 @@
 
     return tx_receipt
 
 
 def enter_duel_lobby(duel_type, hero_ids, jewel_fee, background, stat, private_key, nonce, gas_price_gwei,
                      tx_timeout_seconds, rpc_address, logger):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
-    account = w3.eth.account.privateKeyToAccount(private_key)
+    account = w3.eth.account.from_key(private_key)
     w3.eth.default_account = account.address
 
-    contract_address = Web3.toChecksumAddress(SERENDALE_CONTRACT_ADDRESS)
+    contract_address = Web3.to_checksum_address(SERENDALE_CONTRACT_ADDRESS)
     contract = w3.eth.contract(contract_address, abi=ABI)
 
     tx = contract.functions.enterDuelLobby(duel_utils.string2id('type', duel_type), hero_ids,
-                                           w3.toWei(jewel_fee, 'ether'),
+                                           w3.to_wei(jewel_fee, 'ether'),
                                            duel_utils.string2id('background', background),
                                            duel_utils.string2id('stat', stat)
-                                           ).buildTransaction(
-        {'gasPrice': w3.toWei(gas_price_gwei, 'gwei'), 'nonce': nonce})
+                                           ).build_transaction(
+        {'gasPrice': w3.to_wei(gas_price_gwei, 'gwei'), 'nonce': nonce})
 
     logger.debug("Signing transaction")
     signed_tx = w3.eth.account.sign_transaction(tx, private_key=private_key)
     logger.debug("Sending transaction " + str(tx))
     ret = w3.eth.send_raw_transaction(signed_tx.rawTransaction)
     logger.debug("Transaction successfully sent !")
     logger.info("Waiting for transaction " + block_explorer_link(signed_tx.hash.hex()) + " to be mined")
@@ -328,22 +328,22 @@
     logger.info("Transaction mined !")
 
     return tx_receipt
 
 
 def complete_duel(duel_id, private_key, nonce, gas_price_gwei, tx_timeout_seconds, rpc_address, logger):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
-    account = w3.eth.account.privateKeyToAccount(private_key)
+    account = w3.eth.account.from_key(private_key)
     w3.eth.default_account = account.address
 
-    contract_address = Web3.toChecksumAddress(SERENDALE_CONTRACT_ADDRESS)
+    contract_address = Web3.to_checksum_address(SERENDALE_CONTRACT_ADDRESS)
     contract = w3.eth.contract(contract_address, abi=ABI)
 
-    tx = contract.functions.completeDuel(duel_id).buildTransaction(
-        {'gasPrice': w3.toWei(gas_price_gwei, 'gwei'), 'nonce': nonce})
+    tx = contract.functions.completeDuel(duel_id).build_transaction(
+        {'gasPrice': w3.to_wei(gas_price_gwei, 'gwei'), 'nonce': nonce})
 
     logger.debug("Signing transaction")
     signed_tx = w3.eth.account.sign_transaction(tx, private_key=private_key)
     logger.debug("Sending transaction " + str(tx))
     ret = w3.eth.send_raw_transaction(signed_tx.rawTransaction)
     logger.debug("Transaction successfully sent !")
     logger.info("Waiting for transaction " + block_explorer_link(signed_tx.hash.hex()) + " to be mined")
@@ -353,24 +353,24 @@
 
     return tx_receipt
 
 
 def accept_challenge(duel_id, hero_ids, background, stat, private_key, nonce, gas_price_gwei, tx_timeout_seconds,
                      rpc_address, logger):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
-    account = w3.eth.account.privateKeyToAccount(private_key)
+    account = w3.eth.account.from_key(private_key)
     w3.eth.default_account = account.address
 
-    contract_address = Web3.toChecksumAddress(SERENDALE_CONTRACT_ADDRESS)
+    contract_address = Web3.to_checksum_address(SERENDALE_CONTRACT_ADDRESS)
     contract = w3.eth.contract(contract_address, abi=ABI)
 
     tx = contract.functions.acceptChallenge(duel_id, hero_ids, duel_utils.string2id('background', background),
                                             duel_utils.string2id('stat', stat)
-                                            ).buildTransaction(
-        {'gasPrice': w3.toWei(gas_price_gwei, 'gwei'), 'nonce': nonce})
+                                            ).build_transaction(
+        {'gasPrice': w3.to_wei(gas_price_gwei, 'gwei'), 'nonce': nonce})
 
     logger.debug("Signing transaction")
     signed_tx = w3.eth.account.sign_transaction(tx, private_key=private_key)
     logger.debug("Sending transaction " + str(tx))
     ret = w3.eth.send_raw_transaction(signed_tx.rawTransaction)
     logger.debug("Transaction successfully sent !")
     logger.info("Waiting for transaction " + block_explorer_link(signed_tx.hash.hex()) + " to be mined")
```

### Comparing `dfktools-0.2.0/src/dfktools/duel/utils/utils.py` & `dfktools-0.3.0/src/dfktools/duel/utils/utils.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.2.0/src/dfktools/duel_example.py` & `dfktools-0.3.0/src/dfktools/duel_example.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,35 +15,35 @@
     logger.info("Using RPC server " + rpc_server)
 
     result = duels.get_duel(1, rpc_server)
     logger.info(json.dumps(result, indent=4, sort_keys=False))
 
     w3 = Web3(Web3.HTTPProvider(rpc_server))
     private_key = ""  # set private key
-    account_address = "0x"  # w3.eth.account.privateKeyToAccount(private_key).address
+    account_address = "0x"  # w3.eth.account.from_key(private_key).address
     gas_price_gwei = 120
     tx_timeout_seconds = 30
 
 
     # start ranked duel
     '''
     Ranked match jewel fees
     Solo: 0.1, 0.5, 1
     Squad: 0.3, 1.5, 3
     War: 1, 5, 10
     '''
     duels.enter_duel_lobby('solo', [241730], 0.1, 'forest', 'dexterity',
-                            private_key, w3.eth.getTransactionCount(account_address),
+                            private_key, w3.eth.get_transaction_count(account_address),
                             gas_price_gwei, tx_timeout_seconds, rpc_server, logger)
 
     # start private duel
     duels.start_private_duel('solo', [241730], '0x', 'forest', 'dexterity',
-                            private_key, w3.eth.getTransactionCount(account_address),
+                            private_key, w3.eth.get_transaction_count(account_address),
                             gas_price_gwei, tx_timeout_seconds, rpc_server, logger)
 
     # complete duel
     duels.complete_duel(40331,
-                        private_key, w3.eth.getTransactionCount(account_address),
+                        private_key, w3.eth.get_transaction_count(account_address),
                         gas_price_gwei, tx_timeout_seconds, rpc_server, logger)
 
     # result = duels.getDuelTurns(1,rpc_server) # get duels details based on Duel ID
     # result = duels.get_total_open_duel_entries(3, rpc_server) # 1-Solo,3-Squad,9-War
```

### Comparing `dfktools-0.2.0/src/dfktools/erc20_example.py` & `dfktools-0.3.0/src/dfktools/erc20_example.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.2.0/src/dfktools/genes/gene_science_v1.py` & `dfktools-0.3.0/src/dfktools/genes/gene_science_v1.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,18 +13,18 @@
          ]
         '''
 
 
 def mix_genes(genes1, genes2, block_number, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-    contract_address = Web3.toChecksumAddress(CONTRACT_ADDRESS)
+    contract_address = Web3.to_checksum_address(CONTRACT_ADDRESS)
     contract = w3.eth.contract(contract_address, abi=ABI)
     return contract.functions.mixGenes(genes1, genes2, block_number).call()
 
 
 def decode(genes, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-    contract_address = Web3.toChecksumAddress(CONTRACT_ADDRESS)
+    contract_address = Web3.to_checksum_address(CONTRACT_ADDRESS)
     contract = w3.eth.contract(contract_address, abi=ABI)
     return contract.functions.decode(genes).call()
```

### Comparing `dfktools-0.2.0/src/dfktools/genes/gene_science_v2.py` & `dfktools-0.3.0/src/dfktools/genes/gene_science_v2.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,26 +13,26 @@
          ]
         '''
 
 
 def mix_genes(genes1, genes2, block_number, crystal_id, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-    contract_address = Web3.toChecksumAddress(CONTRACT_ADDRESS)
+    contract_address = Web3.to_checksum_address(CONTRACT_ADDRESS)
     contract = w3.eth.contract(contract_address, abi=ABI)
     return contract.functions.mixGenes(genes1, genes2, crystal_id, block_number).call()
 
 
 def decode(genes, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-    contract_address = Web3.toChecksumAddress(CONTRACT_ADDRESS)
+    contract_address = Web3.to_checksum_address(CONTRACT_ADDRESS)
     contract = w3.eth.contract(contract_address, abi=ABI)
     return contract.functions.decode(genes).call()
 
 
 def expressing_traits(genes, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-    contract_address = Web3.toChecksumAddress(CONTRACT_ADDRESS)
+    contract_address = Web3.to_checksum_address(CONTRACT_ADDRESS)
     contract = w3.eth.contract(contract_address, abi=ABI)
     return contract.functions.expressingTraits(genes).call()
```

### Comparing `dfktools-0.2.0/src/dfktools/genes_example.py` & `dfktools-0.3.0/src/dfktools/genes_example.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.2.0/src/dfktools/hero/hero.py` & `dfktools-0.3.0/src/dfktools/hero/heroes.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 from . import hero_core
 
-
-class Hero:
+class Heroes:
     def __init__(self, contract_address, rpc_address, logger=None):
         self.contract_address = contract_address
         self.rpc_address = rpc_address
         self.logger = logger
 
-    def transfer(self, hero_id, owner_private_key, owner_nonce, receiver_address, gas_price_gwei, tx_timeout_seconds):
-        return hero_core.transfer(self.contract_address, hero_id, owner_private_key, owner_nonce, receiver_address, gas_price_gwei, tx_timeout_seconds, self.rpc_address, self.logger)
+    def transfer(self, hero_id, receiver_address, owner_private_key, owner_nonce, gas_price_gwei, tx_timeout_seconds):
+        return hero_core.transfer_from(self.contract_address, hero_id, receiver_address, owner_private_key, owner_nonce, gas_price_gwei, tx_timeout_seconds, self.rpc_address, self.logger)
+
+    def transfer_with_equipment(self, hero_id, receiver_address, owner_private_key, owner_nonce, gas_price_gwei, tx_timeout_seconds):
+        return hero_core.transfer_hero_and_equipment_from(self.contract_address, hero_id, receiver_address, owner_private_key, owner_nonce, gas_price_gwei, tx_timeout_seconds, self.rpc_address, self.logger)
 
     def get_owner(self, hero_id, block_identifier="latest"):
         return hero_core.get_owner(self.contract_address, hero_id, self.rpc_address, block_identifier)
 
     def get_users_heroes(self, user_address, block_identifier="latest"):
         return hero_core.get_users_heroes(self.contract_address, user_address, self.rpc_address, block_identifier)
 
     def is_approved_for_all(self, owner, operator):
         return hero_core.is_approved_for_all(self.contract_address, owner, operator, self.rpc_address)
 
     def get_hero(self, hero_id, block_identifier="latest"):
-        return hero_core.get_hero(self.contract_address, hero_id, self.rpc_address, block_identifier)
+        return hero_core.get_hero_v2(self.contract_address, hero_id, self.rpc_address, block_identifier)
 
     @staticmethod
     def human_readable_hero(raw_hero, hero_male_first_names=None, hero_female_first_names=None, hero_last_names=None):
         return hero_core.human_readable_hero(raw_hero, hero_male_first_names, hero_female_first_names, hero_last_names)
```

### Comparing `dfktools-0.2.0/src/dfktools/hero/utils/utils.py` & `dfktools-0.3.0/src/dfktools/hero/utils/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,27 +52,38 @@
     7: 'eyeColor',
     8: 'skinColor',
     9: 'appendageColor',
     10: 'backAppendageColor',
     11: 'visualUnknown2'
 }
 
+background = {
+    0: "desert",
+    2: "forest",
+    4: "plains",
+    6: "island",
+    8: "swamp",
+    10: "mountains",
+    12: "city",
+    14: "arctic"
+}
+
 stat_traits = {
     0: "class",
     1: "subClass",
     2: "profession",
     3: "passive1",
     4: "passive2",
     5: "active1",
     6: "active2",
     7: "statBoost1",
     8: "statBoost2",
-    9: "statsUnknown1",
+    9: "craft1",
     10: "element",
-    11: "statsUnknown2"
+    11: "craft2"
 }
 
 ability_traits = {
     0: "basic1",
     1: "basic2",
     2: "basic3",
     3: "basic4",
@@ -92,14 +103,26 @@
 professions = {
     0: 'mining',
     2: 'gardening',
     4: 'fishing',
     6: 'foraging',
 }
 
+
+crafts = {
+    0: 'blacksmithing',
+    2: 'goldsmithing',
+    4: 'armorsmithing',
+    6: 'woodworking',
+    8: 'leatherworking',
+    10: 'tailoring',
+    12: 'enchanting',
+    14: 'alchemy'
+}
+
 stats = {
     0: 'strength',
     2: 'agility',
     4: 'intelligence',
     6: 'wisdom',
     8: 'luck',
     10: 'vitality',
@@ -115,27 +138,27 @@
     8: 'lightning',
     10: 'ice',
     12: 'light',
     14: 'dark',
 }
 
 
-def cv2sd_cv_hero_id(cv_hero_id):
+def cv2norm_hero_id(cv_hero_id):
     return cv_hero_id - CRYSTALEVALE_HERO_OFFSET
 
 
-def sd2cv_cv_hero_id(cv_hero_id):
-    return cv_hero_id + CRYSTALEVALE_HERO_OFFSET
+def norm2cv_hero_id(norm_hero_id):
+    return norm_hero_id + CRYSTALEVALE_HERO_OFFSET
 
-def sd22sd_sd2_hero_id(sd2_hero_id):
+def sd2norm_hero_id(sd2_hero_id):
     return sd2_hero_id - SERENDALE2_HERO_OFFSET
 
 
-def sd2sd2_sd2_hero_id(sd2_hero_id):
-    return sd2_hero_id + SERENDALE2_HERO_OFFSET
+def norm2sd_hero_id(norm_hero_id):
+    return norm_hero_id + SERENDALE2_HERO_OFFSET
 
 
 def parse_rarity(id):
     value = rarity.get(id, None)
     if FAIL_ON_NOT_FOUND and value is None:
         raise Exception("Rarity not found")
     return value
@@ -151,14 +174,22 @@
 def parse_profession(id):
     value = professions.get(id, None)
     if FAIL_ON_NOT_FOUND and value is None:
         raise Exception("Profession not found")
     return value
 
 
+def parse_craft(id):
+    value = crafts.get(id, None)
+    if FAIL_ON_NOT_FOUND and value is None:
+        raise Exception("Craft not found")
+    return value
+
+
+
 def parse_stat(id):
     value = stats.get(id, None)
     if FAIL_ON_NOT_FOUND and value is None:
         raise Exception("Stat not found")
     return value
 
 
@@ -171,14 +202,20 @@
 
 def parse_element(id):
     value = elements.get(id, None)
     if FAIL_ON_NOT_FOUND and value is None:
         raise Exception("Element not found")
     return value
 
+def parse_background(id):
+    value = background.get(id, None)
+    if FAIL_ON_NOT_FOUND and value is None:
+        raise Exception("Background not found")
+    return value
+
 
 def genes2traits(genes):
     traits = []
 
     stat_raw_kai = "".join(__genesToKai(genes).split(' '))
     for ki in range(0, len(stat_raw_kai)):
         kai = stat_raw_kai[ki]
@@ -193,15 +230,15 @@
             arranged_traits[j].append(traits[index + j])
 
     arranged_traits.reverse()
     return arranged_traits
 
 
 def parse_stat_genes(genes):
-    traits = genes2traits(genes)
+    traits = genes2traits(int(genes))
     stats = parse_stat_trait(traits[0])
     r1 = parse_stat_trait(traits[1])
     r2 = parse_stat_trait(traits[2])
     r3 = parse_stat_trait(traits[3])
 
     stats['r1'] = r1
     stats['r2'] = r2
@@ -229,35 +266,37 @@
     stats['passive1'] = parse_ability(stats['passive1'])
     stats['passive2'] = parse_ability(stats['passive2'])
     stats['active1'] = parse_ability(stats['active1'])
     stats['active2'] = parse_ability(stats['active2'])
 
     stats['statBoost1'] = parse_stat(stats['statBoost1'])
     stats['statBoost2'] = parse_stat(stats['statBoost2'])
-    stats['statsUnknown1'] = stats.get(stats['statsUnknown1'], None)  # parse_stat(stat_genes['statsUnknown1'])
-    stats['statsUnknown2'] = stats.get(stats['statsUnknown2'], None)  # parse_stat(stat_genes['statsUnknown2'])
+    stats['craft1'] = parse_craft(stats['craft1'])
+    stats['craft2'] = parse_craft(stats['craft2'])
 
     stats['element'] = parse_element(stats['element'])
 
     return stats
 
 
 def parse_visual_genes(genes):
     visual_genes = {}
-    visual_genes['raw'] = genes
+    visual_genes['raw'] = int(genes)
 
     visual_raw_kai = "".join(__genesToKai(visual_genes['raw']).split(' '))
 
     for ki in range(0, len(visual_raw_kai)):
         stat_trait = visual_traits.get(int(ki / 4), None)
         kai = visual_raw_kai[ki]
         value_num = __kai2dec(kai)
         visual_genes[stat_trait] = value_num
 
     visual_genes['gender'] = 'male' if visual_genes['gender'] == 1 else 'female'
+    visual_genes['background'] = parse_background(visual_genes['background'])
+
     return visual_genes
 
 
 def hero2str(hero):
 
     if isinstance(hero['info']['class'], int):
         c = parse_class(hero['info']['class'])
@@ -292,14 +331,22 @@
     return ' '.join(buf[i:i + 4] for i in range(0, len(buf), 4))
 
 
 def __kai2dec(kai):
     return ALPHABET.index(kai)
 
 
+def _encode_traits(traits):
+    assert len(traits) == 48
+    genes = 0
+    for i  in range(48):
+        genes = genes << 5
+        genes = genes | traits[47 - i]
+    return genes
+
 def parse_names(names_raw_string):
     names_raw_string = names_raw_string\
         .replace("\\xf3", "ó") \
         .replace("\\xf2", "ò") \
         .replace("\\xe9", "é") \
         .replace("\\xe1", "á") \
         .replace("\\xc9", "É") \
```

### Comparing `dfktools-0.2.0/src/dfktools/hero_example.py` & `dfktools-0.3.0/src/dfktools/hero_example.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 import json
 import sys
 import hero.utils.utils as hero_utils
 import hero.hero_core as hero_core
-from hero.hero import Hero
+from hero.heroes import Heroes
 
 
 if __name__ == "__main__":
     log_format = '%(asctime)s|%(name)s|%(levelname)s: %(message)s'
 
     logger = logging.getLogger("DFK-hero")
     logger.setLevel(logging.DEBUG)
@@ -22,29 +22,29 @@
     logger.info("Male hero first name loaded")
 
     with open('hero/lastName.json', 'r') as f:
         last_names = hero_utils.parse_names(f.read())
     logger.info("Hero last name loaded")
 
 
-    serendale2_heroes = Hero(hero_core.SERENDALE2_CONTRACT_ADDRESS, 'https://klaytn.rpc.defikingdoms.com/', logger)
+    serendale2_heroes = Heroes(hero_core.SERENDALE2_CONTRACT_ADDRESS, 'https://klaytn.rpc.defikingdoms.com/', logger)
     #serendale2_heroes.transfer(1, 'private key of the owner', 'next nonce of owner account', 'receiver address', 45, 30)
 
     for i in range(1, 10):
         logger.info("Processing serendale 2 hero #"+str(i))
-        sd2_hero_id = hero_utils.sd2sd2_sd2_hero_id(i)
+        sd2_hero_id = hero_utils.norm2sd_hero_id(i)
         owner = serendale2_heroes.get_owner(sd2_hero_id)
         hero = serendale2_heroes.get_hero(sd2_hero_id)
         readable_hero = serendale2_heroes.human_readable_hero(hero, male_first_names, female_first_names, last_names)
         logger.info(json.dumps(readable_hero, indent=4, sort_keys=False) + "\n Owned by " + owner)
 
-    crystalvale_heroes = Hero(hero_core.CRYSTALVALE_CONTRACT_ADDRESS,
+    crystalvale_heroes = Heroes(hero_core.CRYSTALVALE_CONTRACT_ADDRESS,
                               'https://subnets.avax.network/defi-kingdoms/dfk-chain/rpc', logger)
 
 
     for i in range(1, 10):
         logger.info("Processing crystalvale hero #" + str(i))
-        cv_hero_id = hero_utils.sd2cv_cv_hero_id(i)
+        cv_hero_id = hero_utils.norm2cv_hero_id(i)
         owner = crystalvale_heroes.get_owner(cv_hero_id)
         hero = crystalvale_heroes.get_hero(cv_hero_id)
         readable_hero = crystalvale_heroes.human_readable_hero(hero, male_first_names, female_first_names, last_names)
         logger.info(json.dumps(readable_hero, indent=4, sort_keys=False) + "\n Owned by " + owner)
```

### Comparing `dfktools-0.2.0/src/dfktools/land/land.py` & `dfktools-0.3.0/src/dfktools/land/land.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,81 +68,81 @@
         return 'https://scope.klaytn.com/tx/' + str(txid)
     else:
         return str(txid)
 
 def get_account_lands(real_contract, account, rpc_address):
 	w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-	contract_address = Web3.toChecksumAddress(real_contract)
+	contract_address = Web3.to_checksum_address(real_contract)
 	contract = w3.eth.contract(contract_address, abi=ABI)
 
-	return contract.functions.getAccountLands(Web3.toChecksumAddress(account)).call()
+	return contract.functions.getAccountLands(Web3.to_checksum_address(account)).call()
 
 
 def get_land(real_contract, land_id, rpc_address):
 	w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-	contract_address = Web3.toChecksumAddress(real_contract)
+	contract_address = Web3.to_checksum_address(real_contract)
 	contract = w3.eth.contract(contract_address, abi=ABI)
 
 	return contract.functions.getLand(land_id).call()
 
 
 def get_lands_by_region(real_contract, region_id, rpc_address):
 	w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-	contract_address = Web3.toChecksumAddress(real_contract)
+	contract_address = Web3.to_checksum_address(real_contract)
 	contract = w3.eth.contract(contract_address, abi=ABI)
 
 	return contract.functions.getLandsByRegion(region_id).call()
 
 
 def get_all_lands(real_contract, rpc_address):
 	w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-	contract_address = Web3.toChecksumAddress(real_contract)
+	contract_address = Web3.to_checksum_address(real_contract)
 	contract = w3.eth.contract(contract_address, abi=ABI)
 
 	return contract.functions.getAllLands().call()
 
 
 def owner_of(real_contract, land_id, rpc_address):
 	w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-	contract_address = Web3.toChecksumAddress(real_contract)
+	contract_address = Web3.to_checksum_address(real_contract)
 	contract = w3.eth.contract(contract_address, abi=ABI)
 
 	return contract.functions.ownerOf(land_id).call()
 
 
 def total_supply(real_contract, rpc_address):
 	w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-	contract_address = Web3.toChecksumAddress(real_contract)
+	contract_address = Web3.to_checksum_address(real_contract)
 	contract = w3.eth.contract(contract_address, abi=ABI)
 
 	return contract.functions.totalSupply().call()
 
 
 def claim(real_contract, landId, private_key, nonce, gas_price_gwei, tx_timeout_seconds, rpc_address, logger):
 	w3 = Web3(Web3.HTTPProvider(rpc_address))
-	account = w3.eth.account.privateKeyToAccount(private_key)
+	account = w3.eth.account.from_key(private_key)
 	w3.eth.default_account = account.address
 
-	contract_address = Web3.toChecksumAddress(real_contract)
+	contract_address = Web3.to_checksum_address(real_contract)
 	contract = w3.eth.contract(contract_address, abi=ABI)
 
 	tx = contract.functions.claimLand(account.address, landId)
 
 	if isinstance(gas_price_gwei, dict):  # dynamic fee
-		tx = tx.buildTransaction(
-			{'maxFeePerGas': w3.toWei(gas_price_gwei['maxFeePerGas'], 'gwei'),
-			 'maxPriorityFeePerGas': w3.toWei(gas_price_gwei['maxPriorityFeePerGas'], 'gwei'), 'nonce': nonce})
+		tx = tx.build_transaction(
+			{'maxFeePerGas': w3.to_wei(gas_price_gwei['maxFeePerGas'], 'gwei'),
+			 'maxPriorityFeePerGas': w3.to_wei(gas_price_gwei['maxPriorityFeePerGas'], 'gwei'), 'nonce': nonce})
 	else:  # legacy
-		tx = tx.buildTransaction({'gasPrice': w3.toWei(gas_price_gwei, 'gwei'), 'nonce': nonce})
+		tx = tx.build_transaction({'gasPrice': w3.to_wei(gas_price_gwei, 'gwei'), 'nonce': nonce})
 
 	logger.debug("Signing transaction")
 	signed_tx = w3.eth.account.sign_transaction(tx, private_key=private_key)
 	logger.debug("Sending transaction " + str(tx))
 	ret = w3.eth.send_raw_transaction(signed_tx.rawTransaction)
 	logger.debug("Transaction successfully sent !")
 	logger.info("Waiting for transaction " + block_explorer_link(signed_tx.hash.hex()) + " to be mined")
```

### Comparing `dfktools-0.2.0/src/dfktools/land_example.py` & `dfktools-0.3.0/src/dfktools/land_example.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.2.0/src/dfktools/meditation/meditation.py` & `dfktools-0.3.0/src/dfktools/meditation/meditation.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,33 +65,33 @@
     else:
         return str(txid)
 
 
 def get_required_runes(contract_address, level, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-    contract_address = Web3.toChecksumAddress(contract_address)
+    contract_address = Web3.to_checksum_address(contract_address)
     contract = w3.eth.contract(contract_address, abi=ABI)
 
     return contract.functions._getRequiredRunes(level).call()
 
 
 def active_attunement_crystals(contract_address, address, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-    contract_address = Web3.toChecksumAddress(contract_address)
+    contract_address = Web3.to_checksum_address(contract_address)
     contract = w3.eth.contract(contract_address, abi=ABI)
 
     return contract.functions.activeAttunementCrystals(address).call()
 
 
 def add_attunement_crystal(contract_address, address, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-    contract_address = Web3.toChecksumAddress(contract_address)
+    contract_address = Web3.to_checksum_address(contract_address)
     contract = w3.eth.contract(contract_address, abi=ABI)
 
     return contract.functions.addAttunementCrystal(address).call()
 
 
 def start_meditation(contract_address, hero_id, trait1, trait2, trait3, attunement_crystal_address, private_key, nonce, gas_price_gwei, tx_timeout_seconds, rpc_address, logger):
 
@@ -101,28 +101,28 @@
     if type(trait2) == str:
         trait2 = trait2id(trait2)
 
     if type(trait3) == str:
         trait3 = trait2id(trait3)
 
     w3 = Web3(Web3.HTTPProvider(rpc_address))
-    account = w3.eth.account.privateKeyToAccount(private_key)
+    account = w3.eth.account.from_key(private_key)
     w3.eth.default_account = account.address
 
-    contract_address = Web3.toChecksumAddress(contract_address)
+    contract_address = Web3.to_checksum_address(contract_address)
     contract = w3.eth.contract(contract_address, abi=ABI)
 
     tx = contract.functions.startMeditation(hero_id, trait1, trait2, trait3, attunement_crystal_address)
 
     if isinstance(gas_price_gwei, dict):  # dynamic fee
-        tx = tx.buildTransaction(
-            {'maxFeePerGas': w3.toWei(gas_price_gwei['maxFeePerGas'], 'gwei'),
-             'maxPriorityFeePerGas': w3.toWei(gas_price_gwei['maxPriorityFeePerGas'], 'gwei'), 'nonce': nonce})
+        tx = tx.build_transaction(
+            {'maxFeePerGas': w3.to_wei(gas_price_gwei['maxFeePerGas'], 'gwei'),
+             'maxPriorityFeePerGas': w3.to_wei(gas_price_gwei['maxPriorityFeePerGas'], 'gwei'), 'nonce': nonce})
     else:  # legacy
-        tx = tx.buildTransaction({'gasPrice': w3.toWei(gas_price_gwei, 'gwei'), 'nonce': nonce})
+        tx = tx.build_transaction({'gasPrice': w3.to_wei(gas_price_gwei, 'gwei'), 'nonce': nonce})
 
     logger.debug("Signing transaction")
     signed_tx = w3.eth.account.sign_transaction(tx, private_key=private_key)
     logger.debug("Sending transaction " + str(tx))
     ret = w3.eth.send_raw_transaction(signed_tx.rawTransaction)
     logger.debug("Transaction successfully sent !")
     logger.info("Waiting for transaction " + block_explorer_link(contract_address, signed_tx.hash.hex()) + " to be mined")
@@ -131,28 +131,28 @@
     logger.info("Transaction mined !")
 
     return tx_receipt
 
 
 def complete_meditation(contract_address, hero_id, private_key, nonce, gas_price_gwei, tx_timeout_seconds, rpc_address, logger):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
-    account = w3.eth.account.privateKeyToAccount(private_key)
+    account = w3.eth.account.from_key(private_key)
     w3.eth.default_account = account.address
 
-    contract_address = Web3.toChecksumAddress(contract_address)
+    contract_address = Web3.to_checksum_address(contract_address)
     contract = w3.eth.contract(contract_address, abi=ABI)
 
     tx = contract.functions.completeMeditation(hero_id)
 
     if isinstance(gas_price_gwei, dict):  # dynamic fee
-        tx = tx.buildTransaction(
-            {'maxFeePerGas': w3.toWei(gas_price_gwei['maxFeePerGas'], 'gwei'),
-             'maxPriorityFeePerGas': w3.toWei(gas_price_gwei['maxPriorityFeePerGas'], 'gwei'), 'nonce': nonce})
+        tx = tx.build_transaction(
+            {'maxFeePerGas': w3.to_wei(gas_price_gwei['maxFeePerGas'], 'gwei'),
+             'maxPriorityFeePerGas': w3.to_wei(gas_price_gwei['maxPriorityFeePerGas'], 'gwei'), 'nonce': nonce})
     else:  # legacy
-        tx = tx.buildTransaction({'gasPrice': w3.toWei(gas_price_gwei, 'gwei'), 'nonce': nonce})
+        tx = tx.build_transaction({'gasPrice': w3.to_wei(gas_price_gwei, 'gwei'), 'nonce': nonce})
 
     logger.debug("Signing transaction")
     signed_tx = w3.eth.account.sign_transaction(tx, private_key=private_key)
     logger.debug("Sending transaction " + str(tx))
     ret = w3.eth.send_raw_transaction(signed_tx.rawTransaction)
     logger.debug("Transaction successfully sent !")
     logger.info("Waiting for transaction " + block_explorer_link(contract_address, signed_tx.hash.hex()) + " to be mined")
@@ -162,22 +162,22 @@
 
     return tx_receipt
 
 
 def parse_meditation_results(contract_address, tx_receipt, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-    contract_address = Web3.toChecksumAddress(contract_address)
+    contract_address = Web3.to_checksum_address(contract_address)
     contract = w3.eth.contract(contract_address, abi=ABI)
 
     meditation_result = {}
-    level_up = contract.events.LevelUp().processReceipt(tx_receipt, errors=DISCARD)
+    level_up = contract.events.LevelUp().process_receipt(tx_receipt, errors=DISCARD)
     new_level = level_up[0]['args']["hero"][3][3]
     
-    stat_up = contract.events.StatUp().processReceipt(tx_receipt, errors=DISCARD)
+    stat_up = contract.events.StatUp().process_receipt(tx_receipt, errors=DISCARD)
 
     hero_id = None
     for stat in stat_up:
         hero_id = stat['args']['heroId']
 
         if hero_id not in meditation_result:
             meditation_result[hero_id] = {}
@@ -192,57 +192,57 @@
     
     return meditation_result
 
 
 def get_active_meditations(contract_address, address, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-    contract_address = Web3.toChecksumAddress(contract_address)
+    contract_address = Web3.to_checksum_address(contract_address)
     contract = w3.eth.contract(contract_address, abi=ABI)
 
     return contract.functions.getActiveMeditations(address).call()
 
 
 def get_hero_meditation(contract_address, hero_id, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-    contract_address = Web3.toChecksumAddress(contract_address)
+    contract_address = Web3.to_checksum_address(contract_address)
     contract = w3.eth.contract(contract_address, abi=ABI)
 
     result = contract.functions.getHeroMeditation(hero_id).call()
     if result[0] == 0:
         return None
     return result
 
 
 def get_meditation(contract_address, meditation_id, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-    contract_address = Web3.toChecksumAddress(contract_address)
+    contract_address = Web3.to_checksum_address(contract_address)
     contract = w3.eth.contract(contract_address, abi=ABI)
 
     result = contract.functions.getMeditation(meditation_id).call()
     if result[0] == 0:
         return None
     return result
 
 
 def hero_to_meditation_id(contract_address, hero_id, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-    contract_address = Web3.toChecksumAddress(contract_address)
+    contract_address = Web3.to_checksum_address(contract_address)
     contract = w3.eth.contract(contract_address, abi=ABI)
 
     return contract.functions.heroToMeditation(hero_id).call()
 
 
 def profile_active_meditations(contract_address, address, id, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-    contract_address = Web3.toChecksumAddress(contract_address)
+    contract_address = Web3.to_checksum_address(contract_address)
     contract = w3.eth.contract(contract_address, abi=ABI)
 
     return contract.functions.profileActiveMeditations(address, id).call()
 
 
 def trait2id(label):
     stats = {
```

### Comparing `dfktools-0.2.0/src/dfktools/meditation_example.py` & `dfktools-0.3.0/src/dfktools/meditation_example.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,21 +44,21 @@
     # runes
     active_meditations = meditation.get_active_meditations(contract_address, account_address, rpc_server)
     logger.info("Pending meditation on address " + str(account_address) + ": "+str(active_meditations))
 
     
     required_runes = meditation.get_required_runes(contract_address, level, rpc_server)
     meditation.start_meditation(contract_address, hero_id, stat1, stat2, stat3,
-                                attunement_crystal_address, private_key, w3.eth.getTransactionCount(account_address),
+                                attunement_crystal_address, private_key, w3.eth.get_transaction_count(account_address),
                                 gas_price_gwei, tx_timeout_seconds, rpc_server, logger)
     hero_meditation = meditation.get_hero_meditation(contract_address, hero_id, rpc_server)
     logger.info("Pending meditation "+str(hero_meditation))
     logger.info("Waiting 20 seconds to complete meditation")
     time.sleep(20)
-    tx_receipt = meditation.complete_meditation(contract_address, hero_id, private_key, w3.eth.getTransactionCount(account_address),
+    tx_receipt = meditation.complete_meditation(contract_address, hero_id, private_key, w3.eth.get_transaction_count(account_address),
                                    gas_price_gwei, tx_timeout_seconds, rpc_server, logger)
 
     level_up = meditation.parse_meditation_results(contract_address, tx_receipt, rpc_server)
                 
     meditation_results_msg = ""
     for hero_id in level_up:
         inc = level_up[hero_id]
```

### Comparing `dfktools-0.2.0/src/dfktools/perilous_journey/perilous_journey.py` & `dfktools-0.3.0/src/dfktools/perilous_journey/perilous_journey.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.2.0/src/dfktools/pet_example.py` & `dfktools-0.3.0/src/dfktools/pet_example.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import logging
 import sys
+import json
 from web3 import Web3
 import pets.pet_core as pet_core
 import pets.hatchery as hatchery
 import pets.exchange as exchange
 import pets.utils.utils as pet_utils
+from pets.pets import Pets
 
 if __name__ == "__main__":
     log_format = '%(asctime)s|%(name)s|%(levelname)s: %(message)s'
 
     logger = logging.getLogger("DFK-pet")
     logger.setLevel(logging.DEBUG)
     logging.basicConfig(level=logging.INFO, format=log_format, stream=sys.stdout)
@@ -19,17 +21,26 @@
     user = '0x2E7669F61eA77F02445A015FBdcFe2DE47083E02'
 
     # pet NFT
     logger.info("Total existing pet: {}".format(str(pet_core.next_pet_id(pet_core.CRYSTALVALE_CONTRACT_ADDRESS, rpc_server))))
     user_balance = pet_core.balance_of(pet_core.CRYSTALVALE_CONTRACT_ADDRESS, user, rpc_server)
     logger.info("Player {} is owner of {} pets".format(user, user_balance))
 
-    user_pets = pet_core.get_user_pets(pet_core.CRYSTALVALE_CONTRACT_ADDRESS, user, rpc_server)
+    crystalvale_pets = Pets(pet_core.CRYSTALVALE_CONTRACT_ADDRESS, rpc_server, logger)
+    user_pets = crystalvale_pets.get_user_pets(user)
     for pet in user_pets:
-        logger.info(str(pet_utils.human_readable_pet(pet)))
+        logger.info(str(Pets.human_readable_pet(pet)))
+
+    for i in range(1, 10):
+        logger.info("Processing crystalvale pet {}".format(i))
+        cv_pet_id = pet_utils.norm2cv_pet_id(i)
+        owner = crystalvale_pets.get_owner(cv_pet_id)
+        pet = crystalvale_pets.get_pet(cv_pet_id)
+        readable_pet = crystalvale_pets.human_readable_pet(pet)
+        logger.info(json.dumps(readable_pet, indent=4, sort_keys=False) + "\n Owned by " + owner)
 
     # exchange
     logger.info("Total pet exchange: {}".format(exchange.total_exchanges(exchange.CRYSTALVALE_CONTRACT_ADDRESS, rpc_server)))
     logger.info("Player {} has {} pet exchange pending".format(user, len(
         exchange.get_user_pet_exchanges(exchange.CRYSTALVALE_CONTRACT_ADDRESS, user, rpc_server))))
 
     # hatching
@@ -41,12 +52,12 @@
     logger.info("Incubating cost of blue egg: {}".format(str(blue_egg_cost)))
     logger.info("Incubating cost of grey egg: {}".format(str(grey_egg_cost)))
 
     private_key = None  # set private key
     gas_price_gwei = 115
     tx_timeout = 30
     w3 = Web3(Web3.HTTPProvider(rpc_server))
-    account_address = w3.eth.account.privateKeyToAccount(private_key).address
+    account_address = w3.eth.account.from_key(private_key).address
 
-    hatchery.incubate_egg(hatchery.CRYSTALVALE_CONTRACT_ADDRESS,0, 2, private_key, w3.eth.getTransactionCount(account_address), gas_price_gwei, tx_timeout, rpc_server, logger)
-    hatchery.crack(hatchery.CRYSTALVALE_CONTRACT_ADDRESS, 404, private_key, w3.eth.getTransactionCount(account_address), gas_price_gwei, tx_timeout,
+    hatchery.incubate_egg(hatchery.CRYSTALVALE_CONTRACT_ADDRESS,0, 2, private_key, w3.eth.get_transaction_count(account_address), gas_price_gwei, tx_timeout, rpc_server, logger)
+    hatchery.crack(hatchery.CRYSTALVALE_CONTRACT_ADDRESS, 404, private_key, w3.eth.get_transaction_count(account_address), gas_price_gwei, tx_timeout,
                   rpc_server, logger)
```

### Comparing `dfktools-0.2.0/src/dfktools/pets/exchange.py` & `dfktools-0.3.0/src/dfktools/pets/exchange.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,54 +54,54 @@
     else:
         return str(txid)
 
 
 def get_pet_exchange(contract_address, exchange_id, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-    contract_address = Web3.toChecksumAddress(contract_address)
+    contract_address = Web3.to_checksum_address(contract_address)
     contract = w3.eth.contract(contract_address, abi=ABI)
 
     return contract.functions.getPetExchange(exchange_id).call()
 
 
 def get_user_pet_exchanges(contract_address, account, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-    contract_address = Web3.toChecksumAddress(contract_address)
+    contract_address = Web3.to_checksum_address(contract_address)
     contract = w3.eth.contract(contract_address, abi=ABI)
 
     return contract.functions.getUserPetExchanges(account).call()
 
 
 def total_exchanges(contract_address, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-    contract_address = Web3.toChecksumAddress(contract_address)
+    contract_address = Web3.to_checksum_address(contract_address)
     contract = w3.eth.contract(contract_address, abi=ABI)
 
     return contract.functions.totalExchanges().call()
 
 
 def start_exchange(contract_address, pet_id_1, pet_id_2, private_key, nonce, gas_price_gwei, tx_timeout_seconds, rpc_address, logger):
 
     w3 = Web3(Web3.HTTPProvider(rpc_address))
-    account = w3.eth.account.privateKeyToAccount(private_key)
+    account = w3.eth.account.from_key(private_key)
     w3.eth.default_account = account.address
-    contract_address = Web3.toChecksumAddress(contract_address)
+    contract_address = Web3.to_checksum_address(contract_address)
     contract = w3.eth.contract(contract_address, abi=ABI)
 
     tx = contract.functions.startExchange(pet_id_1, pet_id_2)
 
     if isinstance(gas_price_gwei, dict):  # dynamic fee
-        tx = tx.buildTransaction(
-            {'maxFeePerGas': w3.toWei(gas_price_gwei['maxFeePerGas'], 'gwei'),
-             'maxPriorityFeePerGas': w3.toWei(gas_price_gwei['maxPriorityFeePerGas'], 'gwei'), 'nonce': nonce})
+        tx = tx.build_transaction(
+            {'maxFeePerGas': w3.to_wei(gas_price_gwei['maxFeePerGas'], 'gwei'),
+             'maxPriorityFeePerGas': w3.to_wei(gas_price_gwei['maxPriorityFeePerGas'], 'gwei'), 'nonce': nonce})
     else:  # legacy
-        tx = tx.buildTransaction({'gasPrice': w3.toWei(gas_price_gwei, 'gwei'), 'nonce': nonce})
+        tx = tx.build_transaction({'gasPrice': w3.to_wei(gas_price_gwei, 'gwei'), 'nonce': nonce})
 
     logger.debug("Signing transaction")
     signed_tx = w3.eth.account.sign_transaction(tx, private_key=private_key)
     logger.debug("Sending transaction " + str(tx))
     ret = w3.eth.send_raw_transaction(signed_tx.rawTransaction)
     logger.debug("Transaction successfully sent !")
     logger.info("Waiting for transaction " + block_explorer_link(contract_address, signed_tx.hash.hex()) + " to be mined")
@@ -112,27 +112,27 @@
 
     return tx_receipt
 
 
 def complete_exchange(contract_address, exchange_id, private_key, nonce, gas_price_gwei, tx_timeout_seconds, rpc_address, logger):
 
     w3 = Web3(Web3.HTTPProvider(rpc_address))
-    account = w3.eth.account.privateKeyToAccount(private_key)
+    account = w3.eth.account.from_key(private_key)
     w3.eth.default_account = account.address
-    contract_address = Web3.toChecksumAddress(contract_address)
+    contract_address = Web3.to_checksum_address(contract_address)
     contract = w3.eth.contract(contract_address, abi=ABI)
 
     tx = contract.functions.completeExchange(exchange_id)
 
     if isinstance(gas_price_gwei, dict):  # dynamic fee
-        tx = tx.buildTransaction(
-            {'maxFeePerGas': w3.toWei(gas_price_gwei['maxFeePerGas'], 'gwei'),
-             'maxPriorityFeePerGas': w3.toWei(gas_price_gwei['maxPriorityFeePerGas'], 'gwei'), 'nonce': nonce})
+        tx = tx.build_transaction(
+            {'maxFeePerGas': w3.to_wei(gas_price_gwei['maxFeePerGas'], 'gwei'),
+             'maxPriorityFeePerGas': w3.to_wei(gas_price_gwei['maxPriorityFeePerGas'], 'gwei'), 'nonce': nonce})
     else:  # legacy
-        tx = tx.buildTransaction({'gasPrice': w3.toWei(gas_price_gwei, 'gwei'), 'nonce': nonce})
+        tx = tx.build_transaction({'gasPrice': w3.to_wei(gas_price_gwei, 'gwei'), 'nonce': nonce})
 
     logger.debug("Signing transaction")
     signed_tx = w3.eth.account.sign_transaction(tx, private_key=private_key)
     logger.debug("Sending transaction " + str(tx))
     ret = w3.eth.send_raw_transaction(signed_tx.rawTransaction)
     logger.debug("Transaction successfully sent !")
     logger.info("Waiting for transaction " + block_explorer_link(contract_address, signed_tx.hash.hex()) + " to be mined")
```

### Comparing `dfktools-0.2.0/src/dfktools/pets/hatchery.py` & `dfktools-0.3.0/src/dfktools/pets/hatchery.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,58 +59,58 @@
     else:
         return str(txid)
 
 
 def get_user_eggs(contract_address, account, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-    contract_address = Web3.toChecksumAddress(contract_address)
+    contract_address = Web3.to_checksum_address(contract_address)
     contract = w3.eth.contract(contract_address, abi=ABI)
 
-    return contract.functions.getUserEggs(Web3.toChecksumAddress(account)).call()
+    return contract.functions.getUserEggs(Web3.to_checksum_address(account)).call()
 
 
 def egg_type_costs(contract_address, egg_type, rpc_address):
     """
     :param contract_address:
     :param egg_type: color of the egg as int (0: )
     :param rpc_address:
     :return:
     """
 
     w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-    contract_address = Web3.toChecksumAddress(contract_address)
+    contract_address = Web3.to_checksum_address(contract_address)
     contract = w3.eth.contract(contract_address, abi=ABI)
 
     return contract.functions.eggTypeCosts(egg_type).call()
 
 
 def get_egg(contract_address, egg_id, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-    contract_address = Web3.toChecksumAddress(contract_address)
+    contract_address = Web3.to_checksum_address(contract_address)
     contract = w3.eth.contract(contract_address, abi=ABI)
 
     return contract.functions.getEgg(egg_id).call()
 
 
 def season(contract_address, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-    contract_address = Web3.toChecksumAddress(contract_address)
+    contract_address = Web3.to_checksum_address(contract_address)
     contract = w3.eth.contract(contract_address, abi=ABI)
 
     return contract.functions.season().call()
 
 
 def total_eggs(contract_address, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-    contract_address = Web3.toChecksumAddress(contract_address)
+    contract_address = Web3.to_checksum_address(contract_address)
     contract = w3.eth.contract(contract_address, abi=ABI)
 
     return contract.functions.totalEggs().call()
 
 
 def incubate_egg(contract_address, egg_type, tier, private_key, nonce, gas_price_gwei, tx_timeout_seconds, rpc_address, logger):
     """
@@ -123,27 +123,27 @@
     :param tx_timeout_seconds:
     :param rpc_address:
     :param logger:
     :return:
     """
 
     w3 = Web3(Web3.HTTPProvider(rpc_address))
-    account = w3.eth.account.privateKeyToAccount(private_key)
+    account = w3.eth.account.from_key(private_key)
     w3.eth.default_account = account.address
-    contract_address = Web3.toChecksumAddress(contract_address)
+    contract_address = Web3.to_checksum_address(contract_address)
     contract = w3.eth.contract(contract_address, abi=ABI)
 
     tx = contract.functions.incubateEgg(egg_type, tier)
 
     if isinstance(gas_price_gwei, dict):  # dynamic fee
-        tx = tx.buildTransaction(
-            {'maxFeePerGas': w3.toWei(gas_price_gwei['maxFeePerGas'], 'gwei'),
-             'maxPriorityFeePerGas': w3.toWei(gas_price_gwei['maxPriorityFeePerGas'], 'gwei'), 'nonce': nonce})
+        tx = tx.build_transaction(
+            {'maxFeePerGas': w3.to_wei(gas_price_gwei['maxFeePerGas'], 'gwei'),
+             'maxPriorityFeePerGas': w3.to_wei(gas_price_gwei['maxPriorityFeePerGas'], 'gwei'), 'nonce': nonce})
     else:  # legacy
-        tx = tx.buildTransaction({'gasPrice': w3.toWei(gas_price_gwei, 'gwei'), 'nonce': nonce})
+        tx = tx.build_transaction({'gasPrice': w3.to_wei(gas_price_gwei, 'gwei'), 'nonce': nonce})
 
     logger.debug("Signing transaction")
     signed_tx = w3.eth.account.sign_transaction(tx, private_key=private_key)
     logger.debug("Sending transaction " + str(tx))
     ret = w3.eth.send_raw_transaction(signed_tx.rawTransaction)
     logger.debug("Transaction successfully sent !")
     logger.info("Waiting for transaction " + block_explorer_link(contract_address, signed_tx.hash.hex()) + " to be mined")
@@ -153,27 +153,27 @@
     logger.info("Transaction mined !")
 
     return tx_receipt
 
 
 def crack(contract_address, egg_id, private_key, nonce, gas_price_gwei, tx_timeout_seconds, rpc_address, logger):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
-    account = w3.eth.account.privateKeyToAccount(private_key)
+    account = w3.eth.account.from_key(private_key)
     w3.eth.default_account = account.address
-    contract_address = Web3.toChecksumAddress(contract_address)
+    contract_address = Web3.to_checksum_address(contract_address)
     contract = w3.eth.contract(contract_address, abi=ABI)
 
     tx = contract.functions.crack(egg_id)
 
     if isinstance(gas_price_gwei, dict):  # dynamic fee
-        tx = tx.buildTransaction(
-            {'maxFeePerGas': w3.toWei(gas_price_gwei['maxFeePerGas'], 'gwei'),
-             'maxPriorityFeePerGas': w3.toWei(gas_price_gwei['maxPriorityFeePerGas'], 'gwei'), 'nonce': nonce})
+        tx = tx.build_transaction(
+            {'maxFeePerGas': w3.to_wei(gas_price_gwei['maxFeePerGas'], 'gwei'),
+             'maxPriorityFeePerGas': w3.to_wei(gas_price_gwei['maxPriorityFeePerGas'], 'gwei'), 'nonce': nonce})
     else:  # legacy
-        tx = tx.buildTransaction({'gasPrice': w3.toWei(gas_price_gwei, 'gwei'), 'nonce': nonce})
+        tx = tx.build_transaction({'gasPrice': w3.to_wei(gas_price_gwei, 'gwei'), 'nonce': nonce})
 
     logger.debug("Signing transaction")
     signed_tx = w3.eth.account.sign_transaction(tx, private_key=private_key)
     logger.debug("Sending transaction " + str(tx))
     ret = w3.eth.send_raw_transaction(signed_tx.rawTransaction)
     logger.debug("Transaction successfully sent !")
     logger.info("Waiting for transaction " + block_explorer_link(contract_address, signed_tx.hash.hex()) + " to be mined")
```

### Comparing `dfktools-0.2.0/src/dfktools/pets/pet_core.py` & `dfktools-0.3.0/src/dfktools/raffle/raffle_master.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,178 +1,128 @@
 from web3 import Web3
 
-SERENDALE_CONTRACT_ADDRESS = '0xAC9AFb5900C8A27B766bCad3A37423DC0F4C22d3'
-CRYSTALVALE_CONTRACT_ADDRESS = '0x1990F87d6BC9D9385917E3EDa0A7674411C3Cd7F'
-SERENDALE2_CONTRACT_ADDRESS = '0x6362b205b539afb5FC369277365441c1dC6fAa28'
-
-ABI = '''
-    [
-        {"anonymous":false,"inputs":[{"indexed":true,"internalType":"address","name":"owner","type":"address"},{"indexed":true,"internalType":"address","name":"approved","type":"address"},{"indexed":true,"internalType":"uint256","name":"tokenId","type":"uint256"}],"name":"Approval","type":"event"},
-        {"anonymous":false,"inputs":[{"indexed":true,"internalType":"address","name":"owner","type":"address"},{"indexed":true,"internalType":"address","name":"operator","type":"address"},{"indexed":false,"internalType":"bool","name":"approved","type":"bool"}],"name":"ApprovalForAll","type":"event"},
-        {"anonymous":false,"inputs":[{"indexed":false,"internalType":"uint8","name":"version","type":"uint8"}],"name":"Initialized","type":"event"},
-        {"anonymous":false,"inputs":[{"indexed":false,"internalType":"address","name":"account","type":"address"}],"name":"Paused","type":"event"},
-        {"anonymous":false,"inputs":[{"indexed":true,"internalType":"address","name":"owner","type":"address"},{"indexed":true,"internalType":"uint256","name":"petId","type":"uint256"},{"components":[{"internalType":"uint256","name":"id","type":"uint256"},{"internalType":"uint8","name":"originId","type":"uint8"},{"internalType":"string","name":"name","type":"string"},{"internalType":"uint8","name":"season","type":"uint8"},{"internalType":"uint8","name":"eggType","type":"uint8"},{"internalType":"uint8","name":"rarity","type":"uint8"},{"internalType":"uint8","name":"element","type":"uint8"},{"internalType":"uint8","name":"bonusCount","type":"uint8"},{"internalType":"uint8","name":"profBonus","type":"uint8"},{"internalType":"uint8","name":"profBonusScalar","type":"uint8"},{"internalType":"uint8","name":"craftBonus","type":"uint8"},{"internalType":"uint8","name":"craftBonusScalar","type":"uint8"},{"internalType":"uint8","name":"combatBonus","type":"uint8"},{"internalType":"uint8","name":"combatBonusScalar","type":"uint8"},{"internalType":"uint16","name":"appearance","type":"uint16"},{"internalType":"uint8","name":"background","type":"uint8"},{"internalType":"uint8","name":"shiny","type":"uint8"},{"internalType":"uint64","name":"hungryAt","type":"uint64"},{"internalType":"uint64","name":"equippableAt","type":"uint64"},{"internalType":"uint256","name":"equippedTo","type":"uint256"}],"indexed":false,"internalType":"struct Pet","name":"pet","type":"tuple"}],"name":"PetHatched","type":"event"},
-        {"anonymous":false,"inputs":[{"indexed":true,"internalType":"address","name":"owner","type":"address"},{"indexed":true,"internalType":"uint256","name":"petId","type":"uint256"},{"components":[{"internalType":"uint256","name":"id","type":"uint256"},{"internalType":"uint8","name":"originId","type":"uint8"},{"internalType":"string","name":"name","type":"string"},{"internalType":"uint8","name":"season","type":"uint8"},{"internalType":"uint8","name":"eggType","type":"uint8"},{"internalType":"uint8","name":"rarity","type":"uint8"},{"internalType":"uint8","name":"element","type":"uint8"},{"internalType":"uint8","name":"bonusCount","type":"uint8"},{"internalType":"uint8","name":"profBonus","type":"uint8"},{"internalType":"uint8","name":"profBonusScalar","type":"uint8"},{"internalType":"uint8","name":"craftBonus","type":"uint8"},{"internalType":"uint8","name":"craftBonusScalar","type":"uint8"},{"internalType":"uint8","name":"combatBonus","type":"uint8"},{"internalType":"uint8","name":"combatBonusScalar","type":"uint8"},{"internalType":"uint16","name":"appearance","type":"uint16"},{"internalType":"uint8","name":"background","type":"uint8"},{"internalType":"uint8","name":"shiny","type":"uint8"},{"internalType":"uint64","name":"hungryAt","type":"uint64"},{"internalType":"uint64","name":"equippableAt","type":"uint64"},{"internalType":"uint256","name":"equippedTo","type":"uint256"}],"indexed":false,"internalType":"struct Pet","name":"pet","type":"tuple"}],"name":"PetUpdated","type":"event"},
-        {"anonymous":false,"inputs":[{"indexed":true,"internalType":"bytes32","name":"role","type":"bytes32"},{"indexed":true,"internalType":"bytes32","name":"previousAdminRole","type":"bytes32"},{"indexed":true,"internalType":"bytes32","name":"newAdminRole","type":"bytes32"}],"name":"RoleAdminChanged","type":"event"},
-        {"anonymous":false,"inputs":[{"indexed":true,"internalType":"bytes32","name":"role","type":"bytes32"},{"indexed":true,"internalType":"address","name":"account","type":"address"},{"indexed":true,"internalType":"address","name":"sender","type":"address"}],"name":"RoleGranted","type":"event"},
-        {"anonymous":false,"inputs":[{"indexed":true,"internalType":"bytes32","name":"role","type":"bytes32"},{"indexed":true,"internalType":"address","name":"account","type":"address"},{"indexed":true,"internalType":"address","name":"sender","type":"address"}],"name":"RoleRevoked","type":"event"},
-        {"anonymous":false,"inputs":[{"indexed":true,"internalType":"address","name":"from","type":"address"},{"indexed":true,"internalType":"address","name":"to","type":"address"},{"indexed":true,"internalType":"uint256","name":"tokenId","type":"uint256"}],"name":"Transfer","type":"event"},
-        {"anonymous":false,"inputs":[{"indexed":false,"internalType":"address","name":"account","type":"address"}],"name":"Unpaused","type":"event"},
-        {"inputs":[],"name":"BRIDGE_ROLE","outputs":[{"internalType":"bytes32","name":"","type":"bytes32"}],"stateMutability":"view","type":"function"},
-        {"inputs":[],"name":"DEFAULT_ADMIN_ROLE","outputs":[{"internalType":"bytes32","name":"","type":"bytes32"}],"stateMutability":"view","type":"function"},
-        {"inputs":[],"name":"MINTER_ROLE","outputs":[{"internalType":"bytes32","name":"","type":"bytes32"}],"stateMutability":"view","type":"function"},
-        {"inputs":[],"name":"MODERATOR_ROLE","outputs":[{"internalType":"bytes32","name":"","type":"bytes32"}],"stateMutability":"view","type":"function"},
-        {"inputs":[],"name":"PET_MODERATOR_ROLE","outputs":[{"internalType":"bytes32","name":"","type":"bytes32"}],"stateMutability":"view","type":"function"},
-        {"inputs":[{"internalType":"address","name":"to","type":"address"},{"internalType":"uint256","name":"tokenId","type":"uint256"}],"name":"approve","outputs":[],"stateMutability":"nonpayable","type":"function"},
-        {"inputs":[{"internalType":"address","name":"owner","type":"address"}],"name":"balanceOf","outputs":[{"internalType":"uint256","name":"","type":"uint256"}],"stateMutability":"view","type":"function"},
-        {"inputs":[{"internalType":"uint256","name":"_id","type":"uint256"},{"internalType":"address","name":"_to","type":"address"}],"name":"bridgeMint","outputs":[],"stateMutability":"nonpayable","type":"function"},
-        {"inputs":[{"internalType":"uint256","name":"tokenId","type":"uint256"}],"name":"getApproved","outputs":[{"internalType":"address","name":"","type":"address"}],"stateMutability":"view","type":"function"},
-        {"inputs":[{"internalType":"uint256","name":"_id","type":"uint256"}],"name":"getPet","outputs":[{"components":[{"internalType":"uint256","name":"id","type":"uint256"},{"internalType":"uint8","name":"originId","type":"uint8"},{"internalType":"string","name":"name","type":"string"},{"internalType":"uint8","name":"season","type":"uint8"},{"internalType":"uint8","name":"eggType","type":"uint8"},{"internalType":"uint8","name":"rarity","type":"uint8"},{"internalType":"uint8","name":"element","type":"uint8"},{"internalType":"uint8","name":"bonusCount","type":"uint8"},{"internalType":"uint8","name":"profBonus","type":"uint8"},{"internalType":"uint8","name":"profBonusScalar","type":"uint8"},{"internalType":"uint8","name":"craftBonus","type":"uint8"},{"internalType":"uint8","name":"craftBonusScalar","type":"uint8"},{"internalType":"uint8","name":"combatBonus","type":"uint8"},{"internalType":"uint8","name":"combatBonusScalar","type":"uint8"},{"internalType":"uint16","name":"appearance","type":"uint16"},{"internalType":"uint8","name":"background","type":"uint8"},{"internalType":"uint8","name":"shiny","type":"uint8"},{"internalType":"uint64","name":"hungryAt","type":"uint64"},{"internalType":"uint64","name":"equippableAt","type":"uint64"},{"internalType":"uint256","name":"equippedTo","type":"uint256"}],"internalType":"struct Pet","name":"","type":"tuple"}],"stateMutability":"view","type":"function"},
-        {"inputs":[{"internalType":"bytes32","name":"role","type":"bytes32"}],"name":"getRoleAdmin","outputs":[{"internalType":"bytes32","name":"","type":"bytes32"}],"stateMutability":"view","type":"function"},
-        {"inputs":[{"internalType":"address","name":"_address","type":"address"}],"name":"getUserPets","outputs":[{"components":[{"internalType":"uint256","name":"id","type":"uint256"},{"internalType":"uint8","name":"originId","type":"uint8"},{"internalType":"string","name":"name","type":"string"},{"internalType":"uint8","name":"season","type":"uint8"},{"internalType":"uint8","name":"eggType","type":"uint8"},{"internalType":"uint8","name":"rarity","type":"uint8"},{"internalType":"uint8","name":"element","type":"uint8"},{"internalType":"uint8","name":"bonusCount","type":"uint8"},{"internalType":"uint8","name":"profBonus","type":"uint8"},{"internalType":"uint8","name":"profBonusScalar","type":"uint8"},{"internalType":"uint8","name":"craftBonus","type":"uint8"},{"internalType":"uint8","name":"craftBonusScalar","type":"uint8"},{"internalType":"uint8","name":"combatBonus","type":"uint8"},{"internalType":"uint8","name":"combatBonusScalar","type":"uint8"},{"internalType":"uint16","name":"appearance","type":"uint16"},{"internalType":"uint8","name":"background","type":"uint8"},{"internalType":"uint8","name":"shiny","type":"uint8"},{"internalType":"uint64","name":"hungryAt","type":"uint64"},{"internalType":"uint64","name":"equippableAt","type":"uint64"},{"internalType":"uint256","name":"equippedTo","type":"uint256"}],"internalType":"struct Pet[]","name":"","type":"tuple[]"}],"stateMutability":"view","type":"function"},
-        {"inputs":[{"internalType":"bytes32","name":"role","type":"bytes32"},{"internalType":"address","name":"account","type":"address"}],"name":"grantRole","outputs":[],"stateMutability":"nonpayable","type":"function"},
-        {"inputs":[{"internalType":"bytes32","name":"role","type":"bytes32"},{"internalType":"address","name":"account","type":"address"}],"name":"hasRole","outputs":[{"internalType":"bool","name":"","type":"bool"}],"stateMutability":"view","type":"function"},
-        {"inputs":[{"components":[{"internalType":"uint8","name":"originId","type":"uint8"},{"internalType":"string","name":"name","type":"string"},{"internalType":"uint8","name":"season","type":"uint8"},{"internalType":"uint8","name":"eggType","type":"uint8"},{"internalType":"uint8","name":"rarity","type":"uint8"},{"internalType":"uint8","name":"element","type":"uint8"},{"internalType":"uint8","name":"bonusCount","type":"uint8"},{"internalType":"uint8","name":"profBonus","type":"uint8"},{"internalType":"uint8","name":"profBonusScalar","type":"uint8"},{"internalType":"uint8","name":"craftBonus","type":"uint8"},{"internalType":"uint8","name":"craftBonusScalar","type":"uint8"},{"internalType":"uint8","name":"combatBonus","type":"uint8"},{"internalType":"uint8","name":"combatBonusScalar","type":"uint8"},{"internalType":"uint16","name":"appearance","type":"uint16"},{"internalType":"uint8","name":"background","type":"uint8"},{"internalType":"uint8","name":"shiny","type":"uint8"}],"internalType":"struct PetOptions","name":"_petOptions","type":"tuple"},{"internalType":"address","name":"owner","type":"address"}],"name":"hatchPet","outputs":[{"internalType":"uint256","name":"","type":"uint256"}],"stateMutability":"nonpayable","type":"function"},
-        {"inputs":[{"internalType":"string","name":"_name","type":"string"},{"internalType":"string","name":"_symbol","type":"string"}],"name":"initialize","outputs":[],"stateMutability":"nonpayable","type":"function"},
-        {"inputs":[{"internalType":"address","name":"owner","type":"address"},{"internalType":"address","name":"operator","type":"address"}],"name":"isApprovedForAll","outputs":[{"internalType":"bool","name":"","type":"bool"}],"stateMutability":"view","type":"function"},
-        {"inputs":[],"name":"name","outputs":[{"internalType":"string","name":"","type":"string"}],"stateMutability":"view","type":"function"},
-        {"inputs":[],"name":"nextPetId","outputs":[{"internalType":"uint256","name":"","type":"uint256"}],"stateMutability":"view","type":"function"},
-        {"inputs":[{"internalType":"uint256","name":"tokenId","type":"uint256"}],"name":"ownerOf","outputs":[{"internalType":"address","name":"","type":"address"}],"stateMutability":"view","type":"function"},
-        {"inputs":[],"name":"pause","outputs":[],"stateMutability":"nonpayable","type":"function"},
-        {"inputs":[],"name":"paused","outputs":[{"internalType":"bool","name":"","type":"bool"}],"stateMutability":"view","type":"function"},
-        {"inputs":[{"internalType":"bytes32","name":"role","type":"bytes32"},{"internalType":"address","name":"account","type":"address"}],"name":"renounceRole","outputs":[],"stateMutability":"nonpayable","type":"function"},
-        {"inputs":[{"internalType":"bytes32","name":"role","type":"bytes32"},{"internalType":"address","name":"account","type":"address"}],"name":"revokeRole","outputs":[],"stateMutability":"nonpayable","type":"function"},
-        {"inputs":[{"internalType":"address","name":"from","type":"address"},{"internalType":"address","name":"to","type":"address"},{"internalType":"uint256","name":"tokenId","type":"uint256"}],"name":"safeTransferFrom","outputs":[],"stateMutability":"nonpayable","type":"function"},
-        {"inputs":[{"internalType":"address","name":"from","type":"address"},{"internalType":"address","name":"to","type":"address"},{"internalType":"uint256","name":"tokenId","type":"uint256"},{"internalType":"bytes","name":"_data","type":"bytes"}],"name":"safeTransferFrom","outputs":[],"stateMutability":"nonpayable","type":"function"},
-        {"inputs":[{"internalType":"address","name":"operator","type":"address"},{"internalType":"bool","name":"approved","type":"bool"}],"name":"setApprovalForAll","outputs":[],"stateMutability":"nonpayable","type":"function"},
-        {"inputs":[{"internalType":"bytes4","name":"interfaceId","type":"bytes4"}],"name":"supportsInterface","outputs":[{"internalType":"bool","name":"","type":"bool"}],"stateMutability":"view","type":"function"},
-        {"inputs":[],"name":"symbol","outputs":[{"internalType":"string","name":"","type":"string"}],"stateMutability":"view","type":"function"},
-        {"inputs":[{"internalType":"uint256","name":"index","type":"uint256"}],"name":"tokenByIndex","outputs":[{"internalType":"uint256","name":"","type":"uint256"}],"stateMutability":"view","type":"function"},
-        {"inputs":[{"internalType":"address","name":"owner","type":"address"},{"internalType":"uint256","name":"index","type":"uint256"}],"name":"tokenOfOwnerByIndex","outputs":[{"internalType":"uint256","name":"","type":"uint256"}],"stateMutability":"view","type":"function"},
-        {"inputs":[{"internalType":"uint256","name":"tokenId","type":"uint256"}],"name":"tokenURI","outputs":[{"internalType":"string","name":"","type":"string"}],"stateMutability":"view","type":"function"},
-        {"inputs":[],"name":"totalSupply","outputs":[{"internalType":"uint256","name":"","type":"uint256"}],"stateMutability":"view","type":"function"},
-        {"inputs":[{"internalType":"address","name":"from","type":"address"},{"internalType":"address","name":"to","type":"address"},{"internalType":"uint256","name":"tokenId","type":"uint256"}],"name":"transferFrom","outputs":[],"stateMutability":"nonpayable","type":"function"},
-        {"inputs":[],"name":"unpause","outputs":[],"stateMutability":"nonpayable","type":"function"},
-        {"inputs":[{"components":[{"internalType":"uint256","name":"id","type":"uint256"},{"internalType":"uint8","name":"originId","type":"uint8"},{"internalType":"string","name":"name","type":"string"},{"internalType":"uint8","name":"season","type":"uint8"},{"internalType":"uint8","name":"eggType","type":"uint8"},{"internalType":"uint8","name":"rarity","type":"uint8"},{"internalType":"uint8","name":"element","type":"uint8"},{"internalType":"uint8","name":"bonusCount","type":"uint8"},{"internalType":"uint8","name":"profBonus","type":"uint8"},{"internalType":"uint8","name":"profBonusScalar","type":"uint8"},{"internalType":"uint8","name":"craftBonus","type":"uint8"},{"internalType":"uint8","name":"craftBonusScalar","type":"uint8"},{"internalType":"uint8","name":"combatBonus","type":"uint8"},{"internalType":"uint8","name":"combatBonusScalar","type":"uint8"},{"internalType":"uint16","name":"appearance","type":"uint16"},{"internalType":"uint8","name":"background","type":"uint8"},{"internalType":"uint8","name":"shiny","type":"uint8"},{"internalType":"uint64","name":"hungryAt","type":"uint64"},{"internalType":"uint64","name":"equippableAt","type":"uint64"},{"internalType":"uint256","name":"equippedTo","type":"uint256"}],"internalType":"struct Pet","name":"_pet","type":"tuple"}],"name":"updatePet","outputs":[],"stateMutability":"nonpayable","type":"function"}
-    ]
-    '''
+SERENDALE_CONTRACT_ADDRESS = '0x6a56222A67df18FC282CD58dCDF12e61Be812f97'
+CRYSTALVALE_CONTRACT_ADDRESS = '0xd8D7CE8921490b75EC489bd076AD0f27DC765675'
+
+ABI = """
+    [{"anonymous":false,"inputs":[{"indexed":false,"internalType":"uint8","name":"version","type":"uint8"}],"name":"Initialized","type":"event"},{"anonymous":false,"inputs":[{"indexed":false,"internalType":"address","name":"account","type":"address"}],"name":"Paused","type":"event"},{"anonymous":false,"inputs":[{"indexed":true,"internalType":"uint256","name":"raffleId","type":"uint256"}],"name":"RaffleClosed","type":"event"},{"anonymous":false,"inputs":[{"indexed":true,"internalType":"uint256","name":"raffleId","type":"uint256"},{"indexed":true,"internalType":"address","name":"winner","type":"address"}],"name":"RaffleDrawn","type":"event"},{"anonymous":false,"inputs":[{"indexed":true,"internalType":"address","name":"user","type":"address"},{"indexed":true,"internalType":"uint256","name":"raffleId","type":"uint256"},{"indexed":false,"internalType":"uint256","name":"tickets","type":"uint256"}],"name":"RaffleEntered","type":"event"},{"anonymous":false,"inputs":[{"indexed":true,"internalType":"uint256","name":"raffleId","type":"uint256"},{"components":[{"internalType":"uint256","name":"id","type":"uint256"},{"internalType":"address[]","name":"rewards","type":"address[]"},{"internalType":"uint256[]","name":"rewardAmounts","type":"uint256[]"},{"internalType":"uint256","name":"maxWinners","type":"uint256"},{"internalType":"uint64","name":"duration","type":"uint64"}],"indexed":false,"internalType":"struct RaffleMaster.RaffleType","name":"raffleType","type":"tuple"}],"name":"RaffleStarted","type":"event"},{"anonymous":false,"inputs":[{"indexed":true,"internalType":"uint256","name":"raffleTypeId","type":"uint256"},{"indexed":false,"internalType":"uint256","name":"bucket","type":"uint256"}],"name":"RaffleTypeActivated","type":"event"},{"anonymous":false,"inputs":[{"indexed":true,"internalType":"uint256","name":"id","type":"uint256"},{"components":[{"internalType":"uint256","name":"id","type":"uint256"},{"internalType":"address[]","name":"rewards","type":"address[]"},{"internalType":"uint256[]","name":"rewardAmounts","type":"uint256[]"},{"internalType":"uint256","name":"maxWinners","type":"uint256"},{"internalType":"uint64","name":"duration","type":"uint64"}],"indexed":false,"internalType":"struct RaffleMaster.RaffleType","name":"raffleType","type":"tuple"}],"name":"RaffleTypeAdded","type":"event"},{"anonymous":false,"inputs":[{"indexed":true,"internalType":"uint256","name":"raffleTypeId","type":"uint256"},{"indexed":false,"internalType":"uint256","name":"bucket","type":"uint256"}],"name":"RaffleTypeDeactivated","type":"event"},{"anonymous":false,"inputs":[{"indexed":true,"internalType":"bytes32","name":"role","type":"bytes32"},{"indexed":true,"internalType":"bytes32","name":"previousAdminRole","type":"bytes32"},{"indexed":true,"internalType":"bytes32","name":"newAdminRole","type":"bytes32"}],"name":"RoleAdminChanged","type":"event"},{"anonymous":false,"inputs":[{"indexed":true,"internalType":"bytes32","name":"role","type":"bytes32"},{"indexed":true,"internalType":"address","name":"account","type":"address"},{"indexed":true,"internalType":"address","name":"sender","type":"address"}],"name":"RoleGranted","type":"event"},{"anonymous":false,"inputs":[{"indexed":true,"internalType":"bytes32","name":"role","type":"bytes32"},{"indexed":true,"internalType":"address","name":"account","type":"address"},{"indexed":true,"internalType":"address","name":"sender","type":"address"}],"name":"RoleRevoked","type":"event"},{"anonymous":false,"inputs":[{"indexed":false,"internalType":"address","name":"account","type":"address"}],"name":"Unpaused","type":"event"},{"inputs":[],"name":"DEFAULT_ADMIN_ROLE","outputs":[{"internalType":"bytes32","name":"","type":"bytes32"}],"stateMutability":"view","type":"function"},{"inputs":[],"name":"MODERATOR_ROLE","outputs":[{"internalType":"bytes32","name":"","type":"bytes32"}],"stateMutability":"view","type":"function"},{"inputs":[{"internalType":"uint256","name":"","type":"uint256"},{"internalType":"uint256","name":"","type":"uint256"}],"name":"activeRaffleTypes","outputs":[{"internalType":"uint256","name":"","type":"uint256"}],"stateMutability":"view","type":"function"},{"inputs":[{"internalType":"uint256","name":"_id","type":"uint256"},{"internalType":"uint256","name":"_bucket","type":"uint256"}],"name":"addActiveRaffleType","outputs":[],"stateMutability":"nonpayable","type":"function"},{"inputs":[{"internalType":"address[]","name":"_rewards","type":"address[]"},{"internalType":"uint256[]","name":"_rewardAmounts","type":"uint256[]"},{"internalType":"uint256","name":"_maxWinners","type":"uint256"},{"internalType":"uint64","name":"_duration","type":"uint64"},{"internalType":"uint256[]","name":"_buckets","type":"uint256[]"}],"name":"addAndActivateRaffleType","outputs":[],"stateMutability":"nonpayable","type":"function"},{"inputs":[{"internalType":"address[]","name":"_rewards","type":"address[]"},{"internalType":"uint256[]","name":"_rewardAmounts","type":"uint256[]"},{"internalType":"uint256","name":"_maxWinners","type":"uint256"},{"internalType":"uint64","name":"_duration","type":"uint64"}],"name":"addRaffleType","outputs":[],"stateMutability":"nonpayable","type":"function"},{"inputs":[],"name":"closeRaffles","outputs":[],"stateMutability":"nonpayable","type":"function"},{"inputs":[{"internalType":"uint256","name":"_raffleTypeId","type":"uint256"},{"internalType":"uint256","name":"_bucket","type":"uint256"}],"name":"createRaffle","outputs":[],"stateMutability":"nonpayable","type":"function"},{"inputs":[{"internalType":"uint256","name":"","type":"uint256"}],"name":"currentRaffleBuckets","outputs":[{"internalType":"uint256","name":"","type":"uint256"}],"stateMutability":"view","type":"function"},{"inputs":[],"name":"drawWinners","outputs":[],"stateMutability":"nonpayable","type":"function"},{"inputs":[{"internalType":"uint256","name":"_raffleId","type":"uint256"},{"internalType":"uint256","name":"_tickets","type":"uint256"}],"name":"enterRaffle","outputs":[],"stateMutability":"nonpayable","type":"function"},{"inputs":[{"internalType":"uint256","name":"","type":"uint256"},{"internalType":"uint256","name":"","type":"uint256"}],"name":"entries","outputs":[{"internalType":"address","name":"","type":"address"}],"stateMutability":"view","type":"function"},{"inputs":[],"name":"getCurrentRaffleBuckets","outputs":[{"internalType":"uint256[]","name":"","type":"uint256[]"}],"stateMutability":"view","type":"function"},{"inputs":[],"name":"getCurrentRaffleData","outputs":[{"components":[{"internalType":"uint256","name":"id","type":"uint256"},{"internalType":"uint256","name":"raffleType","type":"uint256"},{"internalType":"uint256","name":"startTime","type":"uint256"},{"internalType":"uint256","name":"totalEntries","type":"uint256"},{"internalType":"uint256","name":"endTime","type":"uint256"},{"internalType":"uint256","name":"closedBlock","type":"uint256"},{"internalType":"address[]","name":"winners","type":"address[]"},{"internalType":"uint8","name":"status","type":"uint8"}],"internalType":"struct RaffleMaster.Raffle[]","name":"","type":"tuple[]"},{"components":[{"internalType":"uint256","name":"id","type":"uint256"},{"internalType":"address[]","name":"rewards","type":"address[]"},{"internalType":"uint256[]","name":"rewardAmounts","type":"uint256[]"},{"internalType":"uint256","name":"maxWinners","type":"uint256"},{"internalType":"uint64","name":"duration","type":"uint64"}],"internalType":"struct RaffleMaster.RaffleType[]","name":"","type":"tuple[]"},{"internalType":"uint256[]","name":"","type":"uint256[]"},{"internalType":"uint256[]","name":"","type":"uint256[]"}],"stateMutability":"view","type":"function"},{"inputs":[],"name":"getLastRaffleBuckets","outputs":[{"internalType":"uint256[]","name":"","type":"uint256[]"}],"stateMutability":"view","type":"function"},{"inputs":[],"name":"getPreviousRaffleData","outputs":[{"components":[{"internalType":"uint256","name":"id","type":"uint256"},{"internalType":"uint256","name":"raffleType","type":"uint256"},{"internalType":"uint256","name":"startTime","type":"uint256"},{"internalType":"uint256","name":"totalEntries","type":"uint256"},{"internalType":"uint256","name":"endTime","type":"uint256"},{"internalType":"uint256","name":"closedBlock","type":"uint256"},{"internalType":"address[]","name":"winners","type":"address[]"},{"internalType":"uint8","name":"status","type":"uint8"}],"internalType":"struct RaffleMaster.Raffle[]","name":"","type":"tuple[]"},{"components":[{"internalType":"uint256","name":"id","type":"uint256"},{"internalType":"address[]","name":"rewards","type":"address[]"},{"internalType":"uint256[]","name":"rewardAmounts","type":"uint256[]"},{"internalType":"uint256","name":"maxWinners","type":"uint256"},{"internalType":"uint64","name":"duration","type":"uint64"}],"internalType":"struct RaffleMaster.RaffleType[]","name":"","type":"tuple[]"},{"internalType":"uint256[]","name":"","type":"uint256[]"},{"internalType":"uint256[]","name":"","type":"uint256[]"}],"stateMutability":"view","type":"function"},{"inputs":[{"internalType":"uint256[]","name":"_raffleBuckets","type":"uint256[]"}],"name":"getRaffleList","outputs":[{"components":[{"internalType":"uint256","name":"id","type":"uint256"},{"internalType":"uint256","name":"raffleType","type":"uint256"},{"internalType":"uint256","name":"startTime","type":"uint256"},{"internalType":"uint256","name":"totalEntries","type":"uint256"},{"internalType":"uint256","name":"endTime","type":"uint256"},{"internalType":"uint256","name":"closedBlock","type":"uint256"},{"internalType":"address[]","name":"winners","type":"address[]"},{"internalType":"uint8","name":"status","type":"uint8"}],"internalType":"struct RaffleMaster.Raffle[]","name":"","type":"tuple[]"}],"stateMutability":"view","type":"function"},{"inputs":[{"internalType":"uint256[]","name":"_raffleBuckets","type":"uint256[]"}],"name":"getRaffleTicketsAllowanceList","outputs":[{"internalType":"uint256[]","name":"","type":"uint256[]"}],"stateMutability":"view","type":"function"},{"inputs":[{"internalType":"uint256[]","name":"_raffleBuckets","type":"uint256[]"}],"name":"getRaffleTicketsList","outputs":[{"internalType":"uint256[]","name":"","type":"uint256[]"}],"stateMutability":"view","type":"function"},{"inputs":[{"internalType":"uint256[]","name":"_raffleBuckets","type":"uint256[]"}],"name":"getRaffleTypesList","outputs":[{"components":[{"internalType":"uint256","name":"id","type":"uint256"},{"internalType":"address[]","name":"rewards","type":"address[]"},{"internalType":"uint256[]","name":"rewardAmounts","type":"uint256[]"},{"internalType":"uint256","name":"maxWinners","type":"uint256"},{"internalType":"uint64","name":"duration","type":"uint64"}],"internalType":"struct RaffleMaster.RaffleType[]","name":"","type":"tuple[]"}],"stateMutability":"view","type":"function"},{"inputs":[{"internalType":"bytes32","name":"role","type":"bytes32"}],"name":"getRoleAdmin","outputs":[{"internalType":"bytes32","name":"","type":"bytes32"}],"stateMutability":"view","type":"function"},{"inputs":[{"internalType":"address","name":"_user","type":"address"},{"internalType":"uint256","name":"_raffleId","type":"uint256"}],"name":"getTicketAllowance","outputs":[{"internalType":"uint256","name":"","type":"uint256"}],"stateMutability":"view","type":"function"},{"inputs":[{"internalType":"bytes32","name":"role","type":"bytes32"},{"internalType":"address","name":"account","type":"address"}],"name":"grantRole","outputs":[],"stateMutability":"nonpayable","type":"function"},{"inputs":[{"internalType":"bytes32","name":"role","type":"bytes32"},{"internalType":"address","name":"account","type":"address"}],"name":"hasRole","outputs":[{"internalType":"bool","name":"","type":"bool"}],"stateMutability":"view","type":"function"},{"inputs":[{"internalType":"uint256","name":"_buckets","type":"uint256"}],"name":"initRaffleBuckets","outputs":[],"stateMutability":"nonpayable","type":"function"},{"inputs":[{"internalType":"address","name":"_raffleTickets","type":"address"},{"internalType":"address","name":"_airdropClaim","type":"address"},{"internalType":"address","name":"_itemMinter","type":"address"}],"name":"initialize","outputs":[],"stateMutability":"nonpayable","type":"function"},{"inputs":[{"internalType":"uint256","name":"","type":"uint256"}],"name":"lastRaffleBuckets","outputs":[{"internalType":"uint256","name":"","type":"uint256"}],"stateMutability":"view","type":"function"},{"inputs":[],"name":"pause","outputs":[],"stateMutability":"nonpayable","type":"function"},{"inputs":[],"name":"paused","outputs":[{"internalType":"bool","name":"","type":"bool"}],"stateMutability":"view","type":"function"},{"inputs":[{"internalType":"uint256","name":"","type":"uint256"},{"internalType":"address","name":"","type":"address"}],"name":"playerEntries","outputs":[{"internalType":"uint256","name":"","type":"uint256"}],"stateMutability":"view","type":"function"},{"inputs":[{"internalType":"uint256","name":"","type":"uint256"}],"name":"raffleTypes","outputs":[{"internalType":"uint256","name":"id","type":"uint256"},{"internalType":"uint256","name":"maxWinners","type":"uint256"},{"internalType":"uint64","name":"duration","type":"uint64"}],"stateMutability":"view","type":"function"},{"inputs":[{"internalType":"uint256","name":"","type":"uint256"}],"name":"raffles","outputs":[{"internalType":"uint256","name":"id","type":"uint256"},{"internalType":"uint256","name":"raffleType","type":"uint256"},{"internalType":"uint256","name":"startTime","type":"uint256"},{"internalType":"uint256","name":"totalEntries","type":"uint256"},{"internalType":"uint256","name":"endTime","type":"uint256"},{"internalType":"uint256","name":"closedBlock","type":"uint256"},{"internalType":"uint8","name":"status","type":"uint8"}],"stateMutability":"view","type":"function"},{"inputs":[{"internalType":"uint256","name":"_index","type":"uint256"},{"internalType":"uint256","name":"_bucket","type":"uint256"}],"name":"removeActiveRaffleType","outputs":[],"stateMutability":"nonpayable","type":"function"},{"inputs":[{"internalType":"bytes32","name":"role","type":"bytes32"},{"internalType":"address","name":"account","type":"address"}],"name":"renounceRole","outputs":[],"stateMutability":"nonpayable","type":"function"},{"inputs":[{"internalType":"bytes32","name":"role","type":"bytes32"},{"internalType":"address","name":"account","type":"address"}],"name":"revokeRole","outputs":[],"stateMutability":"nonpayable","type":"function"},{"inputs":[{"internalType":"uint256","name":"_raffleTypeId","type":"uint256"},{"internalType":"address[]","name":"_rewards","type":"address[]"},{"internalType":"uint256[]","name":"_rewardAmounts","type":"uint256[]"},{"internalType":"uint256","name":"_maxWinners","type":"uint256"},{"internalType":"uint64","name":"_duration","type":"uint64"}],"name":"setRaffleType","outputs":[],"stateMutability":"nonpayable","type":"function"},{"inputs":[{"internalType":"uint256","name":"_bucket","type":"uint256"}],"name":"startRandomRaffle","outputs":[],"stateMutability":"nonpayable","type":"function"},{"inputs":[{"internalType":"uint256[]","name":"_buckets","type":"uint256[]"}],"name":"startRandomRaffles","outputs":[],"stateMutability":"nonpayable","type":"function"},{"inputs":[{"internalType":"bytes4","name":"interfaceId","type":"bytes4"}],"name":"supportsInterface","outputs":[{"internalType":"bool","name":"","type":"bool"}],"stateMutability":"view","type":"function"},{"inputs":[],"name":"timePerTicket","outputs":[{"internalType":"uint256","name":"","type":"uint256"}],"stateMutability":"view","type":"function"},{"inputs":[],"name":"totalRaffleTypes","outputs":[{"internalType":"uint256","name":"","type":"uint256"}],"stateMutability":"view","type":"function"},{"inputs":[],"name":"totalRaffles","outputs":[{"internalType":"uint256","name":"","type":"uint256"}],"stateMutability":"view","type":"function"},{"inputs":[],"name":"unpause","outputs":[],"stateMutability":"nonpayable","type":"function"}]
+    """
 
 
 def block_explorer_link(contract_address, txid):
     if hasattr(contract_address, 'address'):
         contract_address = str(contract_address.address)
     contract_address = str(contract_address).upper()
     if contract_address == SERENDALE_CONTRACT_ADDRESS.upper():
         return 'https://explorer.harmony.one/tx/' + str(txid)
     elif contract_address == CRYSTALVALE_CONTRACT_ADDRESS.upper():
-        return 'https://subnets.avax.network/defi-kingdoms/dfk-chain/explorer/tx/' + str(txid)
-    elif contract_address == SERENDALE2_CONTRACT_ADDRESS.upper():
-        return 'https://scope.klaytn.com/tx/' + str(txid)
+       return 'https://subnets.avax.network/defi-kingdoms/dfk-chain/explorer/tx/' + str(txid)
+    #elif contract_address == SERENDALE2_CONTRACT_ADDRESS.upper():
+    #    return 'https://scope.klaytn.com/tx/' + str(txid)
     else:
         return str(txid)
+    
+def get_current_raffle_buckets(contract_address, rpc_address):
+    w3 = Web3(Web3.HTTPProvider(rpc_address))
+    contract_address = Web3.to_checksum_address(contract_address)
+    contract = w3.eth.contract(contract_address, abi=ABI)
+    return contract.functions.getCurrentRaffleBuckets().call()
 
 
-def balance_of(contract_address, account, rpc_address):
+def get_current_raffle_data(contract_address, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
-
-    contract_address = Web3.toChecksumAddress(contract_address)
+    contract_address = Web3.to_checksum_address(contract_address)
     contract = w3.eth.contract(contract_address, abi=ABI)
-
-    return contract.functions.balanceOf(Web3.toChecksumAddress(account)).call()
+    return contract.functions.getCurrentRaffleData().call()
 
 
-def get_pet(contract_address, pet_id, rpc_address):
+def get_last_raffle_buckets(contract_address, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
-
-    contract_address = Web3.toChecksumAddress(contract_address)
+    contract_address = Web3.to_checksum_address(contract_address)
     contract = w3.eth.contract(contract_address, abi=ABI)
-
-    return contract.functions.getPet(pet_id).call()
+    return contract.functions.getLastRaffleBuckets().call()
 
 
-def get_user_pets(contract_address, account, rpc_address):
+def get_previous_raffle_data(rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
-
-    contract_address = Web3.toChecksumAddress(contract_address)
+    contract_address = Web3.to_checksum_address(SERENDALE_CONTRACT_ADDRESS)
     contract = w3.eth.contract(contract_address, abi=ABI)
-
-    return contract.functions.getUserPets(account).call()
+    return contract.functions.getPreviousRaffleData().call()
 
 
-def owner_of(contract_address, pet_id, rpc_address):
+def get_total_raffles(contract_address, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
-
-    contract_address = Web3.toChecksumAddress(contract_address)
+    contract_address = Web3.to_checksum_address(contract_address)
     contract = w3.eth.contract(contract_address, abi=ABI)
-
-    return contract.functions.ownerOf(pet_id).call()
+    return contract.functions.totalRaffles().call()
 
 
-def next_pet_id(contract_address, rpc_address):
+def get_ticket_allowance(contract_address, address, raffle_id, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
-
-    contract_address = Web3.toChecksumAddress(contract_address)
+    contract_address = Web3.to_checksum_address(contract_address)
     contract = w3.eth.contract(contract_address, abi=ABI)
+    return contract.functions.getTicketAllowance(Web3.to_checksum_address(address),raffle_id).call()
 
-    return contract.functions.nextPetId().call()
 
+def get_total_raffle_types(contract_address, rpc_address):
+    w3 = Web3(Web3.HTTPProvider(rpc_address))
+    contract_address = Web3.to_checksum_address(contract_address)
+    contract = w3.eth.contract(contract_address, abi=ABI)
+    return contract.functions.totalRaffleTypes().call()
 
-def safe_transfer_from(contract_address, _from, to, egg_id, private_key, nonce, gas_price_gwei, tx_timeout_seconds, rpc_address, logger):
 
+def get_raffle_list(contract_address, raffle_id, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
-    account = w3.eth.account.privateKeyToAccount(private_key)
-    w3.eth.default_account = account.address
-    contract_address = Web3.toChecksumAddress(contract_address)
+    contract_address = Web3.to_checksum_address(contract_address)
     contract = w3.eth.contract(contract_address, abi=ABI)
+    return contract.functions.getRaffleList(raffle_id).call()
 
-    tx = contract.functions.safeTransferFrom(_from, to, egg_id)
 
-    if isinstance(gas_price_gwei, dict):  # dynamic fee
-        tx = tx.buildTransaction(
-            {'maxFeePerGas': w3.toWei(gas_price_gwei['maxFeePerGas'], 'gwei'),
-             'maxPriorityFeePerGas': w3.toWei(gas_price_gwei['maxPriorityFeePerGas'], 'gwei'), 'nonce': nonce})
-    else:  # legacy
-        tx = tx.buildTransaction({'gasPrice': w3.toWei(gas_price_gwei, 'gwei'), 'nonce': nonce})
+def get_raffle_tickets_allowance_list(contract_address, raffle_id, rpc_address):
+    w3 = Web3(Web3.HTTPProvider(rpc_address))
+    contract_address = Web3.to_checksum_address(contract_address)
+    contract = w3.eth.contract(contract_address, abi=ABI)
+    return contract.functions.getRaffleTicketsAllowanceList(raffle_id).call()
 
-    logger.debug("Signing transaction")
-    signed_tx = w3.eth.account.sign_transaction(tx, private_key=private_key)
-    logger.debug("Sending transaction " + str(tx))
-    ret = w3.eth.send_raw_transaction(signed_tx.rawTransaction)
-    logger.debug("Transaction successfully sent !")
-    logger.info("Waiting for transaction " + block_explorer_link(contract_address, signed_tx.hash.hex()) + " to be mined")
 
-    tx_receipt = w3.eth.wait_for_transaction_receipt(transaction_hash=signed_tx.hash, timeout=tx_timeout_seconds,
-                                                     poll_latency=2)
-    logger.info("Transaction mined !")
+def get_raffle_tickets_list(contract_address, raffle_id, rpc_address):
+    w3 = Web3(Web3.HTTPProvider(rpc_address))
+    contract_address = Web3.to_checksum_address(contract_address)
+    contract = w3.eth.contract(contract_address, abi=ABI)
+    return contract.functions.getRaffleTicketsList(raffle_id).call()
 
-    return tx_receipt
 
+def get_raffle_types_list(contract_address, raffle_id, rpc_address):
+    w3 = Web3(Web3.HTTPProvider(rpc_address))
+    contract_address = Web3.to_checksum_address(contract_address)
+    contract = w3.eth.contract(contract_address, abi=ABI)
+    return contract.functions.getRaffleTypesList(raffle_id).call()
 
-def transfer_from(contract_address, _from, to, egg_id, private_key, nonce, gas_price_gwei, tx_timeout_seconds, rpc_address, logger):
 
+def enter_raffle(contract_address, raffle_id, tickets, private_key, nonce, gas_price_gwei, tx_timeout_seconds, rpc_address, logger):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
-    account = w3.eth.account.privateKeyToAccount(private_key)
+    account = w3.eth.account.from_key(private_key)
     w3.eth.default_account = account.address
-    contract_address = Web3.toChecksumAddress(contract_address)
+
+    contract_address = Web3.to_checksum_address(contract_address)
     contract = w3.eth.contract(contract_address, abi=ABI)
 
-    tx = contract.functions.transferFrom(_from, to, egg_id)
+    tx = contract.functions.enterRaffle(raffle_id, tickets)
 
     if isinstance(gas_price_gwei, dict):  # dynamic fee
-        tx = tx.buildTransaction(
-            {'maxFeePerGas': w3.toWei(gas_price_gwei['maxFeePerGas'], 'gwei'),
-             'maxPriorityFeePerGas': w3.toWei(gas_price_gwei['maxPriorityFeePerGas'], 'gwei'), 'nonce': nonce})
+        tx = tx.build_transaction(
+            {'maxFeePerGas': w3.to_wei(gas_price_gwei['maxFeePerGas'], 'gwei'),
+             'maxPriorityFeePerGas': w3.to_wei(gas_price_gwei['maxPriorityFeePerGas'], 'gwei'), 'nonce': nonce})
     else:  # legacy
-        tx = tx.buildTransaction({'gasPrice': w3.toWei(gas_price_gwei, 'gwei'), 'nonce': nonce})
+        tx = tx.build_transaction({'gasPrice': w3.to_wei(gas_price_gwei, 'gwei'), 'nonce': nonce})
 
     logger.debug("Signing transaction")
     signed_tx = w3.eth.account.sign_transaction(tx, private_key=private_key)
     logger.debug("Sending transaction " + str(tx))
     ret = w3.eth.send_raw_transaction(signed_tx.rawTransaction)
     logger.debug("Transaction successfully sent !")
-    logger.info("Waiting for transaction " + block_explorer_link(contract_address, signed_tx.hash.hex()) + " to be mined")
-
+    logger.info("Waiting for transaction " + block_explorer_link(signed_tx.hash.hex()) + " to be mined")
     tx_receipt = w3.eth.wait_for_transaction_receipt(transaction_hash=signed_tx.hash, timeout=tx_timeout_seconds,
                                                      poll_latency=2)
     logger.info("Transaction mined !")
 
-    return tx_receipt
+    return tx_receipt
```

### Comparing `dfktools-0.2.0/src/dfktools/profile/profile.py` & `dfktools-0.3.0/src/dfktools/profile/profile.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,17 +31,17 @@
             {"inputs":[{"internalType":"address","name":"newOwner","type":"address"}],"name":"transferOwnership","outputs":[],"stateMutability":"nonpayable","type":"function"}
         ]
         """
 
 
 def get_profile(address, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
-    contract_address = Web3.toChecksumAddress(CONTRACT_ADDRESS)
+    contract_address = Web3.to_checksum_address(CONTRACT_ADDRESS)
     contract = w3.eth.contract(contract_address, abi=ABI)
-    contract_entry = contract.functions.getProfileByAddress(Web3.toChecksumAddress(address)).call()
+    contract_entry = contract.functions.getProfileByAddress(Web3.to_checksum_address(address)).call()
 
     profile = {}
     profile['id'] = contract_entry[0]
     profile['address'] = str(contract_entry[1])
     profile['name'] = contract_entry[2]
     profile['creation_time'] = contract_entry[3]
     profile['pic_id'] = contract_entry[4]
```

### Comparing `dfktools-0.2.0/src/dfktools/profile/profile_v2.py` & `dfktools-0.3.0/src/dfktools/profile/profile_v2.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,17 +48,17 @@
             {"inputs":[{"internalType":"bytes4","name":"interfaceId","type":"bytes4"}],"name":"supportsInterface","outputs":[{"internalType":"bool","name":"","type":"bool"}],"stateMutability":"view","type":"function"}
         ]
         """
 
 
 def get_profile(contract_address, address, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
-    contract_address = Web3.toChecksumAddress(contract_address)
+    contract_address = Web3.to_checksum_address(contract_address)
     contract = w3.eth.contract(contract_address, abi=ABI)
-    contract_entry = contract.functions.getProfileByAddress(Web3.toChecksumAddress(address)).call()
+    contract_entry = contract.functions.getProfile(Web3.to_checksum_address(address)).call()
 
     profile = {}
     profile['id'] = contract_entry[0]
     profile['address'] = str(contract_entry[1])
     profile['name'] = contract_entry[2]
     profile['creation_time'] = contract_entry[3]
     profile['pic_id'] = contract_entry[4]
```

### Comparing `dfktools-0.2.0/src/dfktools/quest_example.py` & `dfktools-0.3.0/src/dfktools/quest_example.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 import sys
 import time
 from web3 import Web3
 import quests.professions.fishing as fishing
 import quests.professions.gardening as gardening
-import quests.quest_v2 as quest_v2, quests.quest_core_v2 as quest_core_v2, quests.quest_v1 as quest_v1
+import quests.quest_v3 as quest_v3, quests.quest_core_v3 as quest_core_v3, quests.quest_v2 as quest_v2, quests.quest_core_v2 as quest_core_v2, quests.quest_v1 as quest_v1
 import quests.utils.utils as quest_utils
 
 ZERO_ADDRESS = '0x0000000000000000000000000000000000000000'
 
 if __name__ == "__main__":
     log_format = '%(asctime)s|%(name)s|%(levelname)s: %(message)s'
 
@@ -20,81 +20,79 @@
     crystalvale_rpc_server = 'https://subnets.avax.network/defi-kingdoms/dfk-chain/rpc'
     logger.info("Using RPC servers " + serendale2_rpc_server + ", " + crystalvale_rpc_server)
 
     w3_serendale2 = Web3(Web3.HTTPProvider(serendale2_rpc_server))
     w3_crystalvale = Web3(Web3.HTTPProvider(crystalvale_rpc_server))
 
     # Parse completeQuest transaction receipt V2
-    tx_receipt = w3_serendale2.eth.getTransactionReceipt("0x7096f3742c27dedb5c9020d895f453524ec583b99a007238095e2cddce8e67aa")
+    tx_receipt = w3_serendale2.eth.get_transaction_receipt('0x7096f3742c27dedb5c9020d895f453524ec583b99a007238095e2cddce8e67aa')
     quest_result = quest_v2.Quest(quest_core_v2.SERENDALE2_CONTRACT_ADDRESS, serendale2_rpc_server, logger).parse_complete_quest_receipt(tx_receipt)
     quest_rewards = quest_utils.human_readable_quest_results(quest_result, very_human=True)
     logger.info("Rewards V2: {}".format(str(quest_rewards)))
 
     # Full quest flow
     private_key = None  # set private key
     gas_price_gwei_serendale = {'maxFeePerGas': 55, 'maxPriorityFeePerGas': 25}  # EIP-1559
     gas_price_gwei_crystalvale = {'maxFeePerGas': 2, 'maxPriorityFeePerGas': 2}  # EIP-1559
     tx_timeout = 30
 
-    account_address = w3_serendale2.eth.account.privateKeyToAccount(private_key).address
+    account_address = w3_serendale2.eth.account.from_key(private_key).address
 
     # Fishing in Crystalvale
-    questV2 = quest_v2.Quest(quest_core_v2.CRYSTALVALE_CONTRACT_ADDRESS, crystalvale_rpc_server, logger)
-    quest_contract = fishing.CRYSTALVALE_QUEST_CONTRACT_ADDRESS
+    questV3 = quest_v3.Quest(quest_core_v3.CRYSTALVALE_CONTRACT_ADDRESS, crystalvale_rpc_server, logger)
     my_heroes_id = [1, 2, 3, 4]
     attempts = 3
     level = 1
-    questV2.start_quest(quest_contract, my_heroes_id, attempts, level, private_key, w3_crystalvale.eth.getTransactionCount(account_address), gas_price_gwei_crystalvale, tx_timeout)
-    quest_info = quest_utils.human_readable_quest(questV2.get_hero_quest(my_heroes_id[0]))
+    questV3.start_quest(my_heroes_id, quest_core_v3.QUEST_TYPE_FISHING, attempts, level, 0, private_key, w3_crystalvale.eth.get_transaction_count(account_address), gas_price_gwei_crystalvale, tx_timeout)
+    quest_info = quest_utils.human_readable_quest(questV3.get_hero_quest(my_heroes_id[0]))
 
     logger.info(
         "Waiting " + str(quest_info['completeAtTime'] - time.time()) + " secs to complete quest " + str(quest_info))
     while time.time() < quest_info['completeAtTime']:
         time.sleep(2)
 
-    tx_receipt = questV2.complete_quest(my_heroes_id[0], private_key, w3_crystalvale.eth.getTransactionCount(account_address), gas_price_gwei_crystalvale, tx_timeout)
-    quest_result = questV2.parse_complete_quest_receipt(tx_receipt)
+    tx_receipt = questV3.complete_quest(my_heroes_id[0], private_key, w3_crystalvale.eth.get_transaction_count(account_address), gas_price_gwei_crystalvale, tx_timeout)
+    quest_result = questV3.parse_complete_quest_receipt(tx_receipt)
     quest_rewards = quest_utils.human_readable_quest_results(quest_result, very_human=True)
     logger.info("Rewards: {}".format(str(quest_rewards)))
 
     # Gardening in Serendale
-    pool_id = 0  # See gardens.master_gardener
-    questV2 = quest_v2.Quest(quest_core_v2.SERENDALE2_CONTRACT_ADDRESS, serendale2_rpc_server, logger)
-    quest_contract = gardening.get_pool_id_contract_address(gardening.SERENDALE2_QUEST_CONTRACT_ADDRESSES, 0) # 'wJEWEL-xJEWEL'
+    questV3 = quest_v3.Quest(quest_core_v3.SERENDALE2_CONTRACT_ADDRESS, serendale2_rpc_server, logger)
+    pool_id = 0 # 'wJEWEL-xJEWEL' (see gardens.master_gardener)
     quest_data = (pool_id, 0, 0, 0, 0, 0, '', '', ZERO_ADDRESS, ZERO_ADDRESS, ZERO_ADDRESS, ZERO_ADDRESS)
     my_gardener_heroes_id = [5]
     attempts = 1
     level = 0
-    questV2.start_quest(quest_contract, my_gardener_heroes_id, attempts, level, private_key,
-                        w3_serendale2.eth.getTransactionCount(account_address), gas_price_gwei_crystalvale, tx_timeout)
-    quest_info = quest_utils.human_readable_quest(questV2.get_hero_quest(my_heroes_id[0]))
+    questV3.start_quest(my_gardener_heroes_id, quest_core_v3.QUEST_TYPE_GARDENING, attempts, level, pool_id, private_key,
+                        w3_serendale2.eth.get_transaction_count(account_address), gas_price_gwei_crystalvale, tx_timeout)
+    quest_info = quest_utils.human_readable_quest(questV3.get_hero_quest(my_heroes_id[0]))
 
     logger.info(
         "Waiting " + str(quest_info['completeAtTime'] - time.time()) + " secs to complete quest " + str(quest_info))
     while time.time() < quest_info['completeAtTime']:
         time.sleep(2)
 
-    tx_receipt = questV2.complete_quest(my_heroes_id[0], private_key,
-                                        w3_serendale2.eth.getTransactionCount(account_address),
+    tx_receipt = questV3.complete_quest(my_heroes_id[0], private_key,
+                                        w3_serendale2.eth.get_transaction_count(account_address),
                                         gas_price_gwei_crystalvale, tx_timeout)
-    quest_result = questV2.parse_complete_quest_receipt(tx_receipt)
+    quest_result = questV3.parse_complete_quest_receipt(tx_receipt)
     quest_rewards = quest_utils.human_readable_quest_results(quest_result, very_human=True)
     logger.info("Rewards: {}".format(str(quest_rewards)))
 
     # Gardening in Crystalvale
-    questV2 = quest_v2.Quest(quest_core_v2.CRYSTALVALE_CONTRACT_ADDRESS, crystalvale_rpc_server, logger)
-    quest_contract = gardening.get_pool_id_contract_address(gardening.CRYSTALVALE_QUEST_CONTRACT_ADDRESSES_V2, 0) # 'wJEWEL-xJEWEL'
+    questV3 = quest_v3.Quest(quest_core_v3.CRYSTALVALE_CONTRACT_ADDRESS, crystalvale_rpc_server, logger)
+    pool_id = 0 # 'wJEWEL-xJEWEL'
     my_heroes_id = [1, 2]
     attempts = 1
     level = 0
-    questV2.start_quest(quest_contract, my_heroes_id, attempts, level, private_key, w3_crystalvale.eth.getTransactionCount(account_address), gas_price_gwei_crystalvale, tx_timeout)
-    quest_info = quest_utils.human_readable_quest(questV2.get_hero_quest(my_heroes_id[0]))
+    questV3.start_quest(my_heroes_id, quest_core_v3.QUEST_TYPE_GARDENING, attempts, level, pool_id, private_key, w3_crystalvale.eth.get_transaction_count(account_address), gas_price_gwei_crystalvale, tx_timeout)
+    quest_info = quest_utils.human_readable_quest(questV3.get_hero_quest(my_heroes_id[0]))
 
     logger.info(
         "Waiting " + str(quest_info['completeAtTime'] - time.time()) + " secs to complete quest " + str(quest_info))
     while time.time() < quest_info['completeAtTime']:
         time.sleep(2)
 
-    tx_receipt = questV2.complete_quest(my_heroes_id[0], private_key, w3_crystalvale.eth.getTransactionCount(account_address), gas_price_gwei_crystalvale, tx_timeout)
-    quest_result = questV2.parse_complete_quest_receipt(tx_receipt)
+    tx_receipt = questV3.complete_quest(my_heroes_id[0], private_key, w3_crystalvale.eth.get_transaction_count(account_address), gas_price_gwei_crystalvale, tx_timeout)
+    quest_result = questV3.parse_complete_quest_receipt(tx_receipt)
     quest_rewards = quest_utils.human_readable_quest_results(quest_result, very_human=True)
     logger.info("Rewards: {}".format(str(quest_rewards)))
```

### Comparing `dfktools-0.2.0/src/dfktools/quests/professions/gardening.py` & `dfktools-0.3.0/src/dfktools/quests/professions/gardening.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.2.0/src/dfktools/quests/professions/mining.py` & `dfktools-0.3.0/src/dfktools/quests/professions/mining.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.2.0/src/dfktools/quests/quest_core_v1.py` & `dfktools-0.3.0/src/dfktools/quests/quest_core_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,28 +60,28 @@
 
 def block_explorer_link(txid):
     return 'https://explorer.harmony.one/tx/' + str(txid)
 
 
 def start_quest(quest_address, hero_ids, attempts, private_key, nonce, gas_price_gwei, tx_timeout_seconds, rpc_address, logger):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
-    account = w3.eth.account.privateKeyToAccount(private_key)
+    account = w3.eth.account.from_key(private_key)
     w3.eth.default_account = account.address
 
-    contract_address = Web3.toChecksumAddress(CONTRACT_ADDRESS)
+    contract_address = Web3.to_checksum_address(CONTRACT_ADDRESS)
     contract = w3.eth.contract(contract_address, abi=ABI)
 
     tx = contract.functions.startQuest(hero_ids, quest_address, attempts)
 
     if isinstance(gas_price_gwei, dict):  # dynamic fee
-        tx = tx.buildTransaction(
-            {'maxFeePerGas': w3.toWei(gas_price_gwei['maxFeePerGas'], 'gwei'),
-             'maxPriorityFeePerGas': w3.toWei(gas_price_gwei['maxPriorityFeePerGas'], 'gwei'), 'nonce': nonce})
+        tx = tx.build_transaction(
+            {'maxFeePerGas': w3.to_wei(gas_price_gwei['maxFeePerGas'], 'gwei'),
+             'maxPriorityFeePerGas': w3.to_wei(gas_price_gwei['maxPriorityFeePerGas'], 'gwei'), 'nonce': nonce})
     else:  # legacy
-        tx = tx.buildTransaction({'gasPrice': w3.toWei(gas_price_gwei, 'gwei'), 'nonce': nonce})
+        tx = tx.build_transaction({'gasPrice': w3.to_wei(gas_price_gwei, 'gwei'), 'nonce': nonce})
 
     logger.debug("Signing transaction")
     signed_tx = w3.eth.account.sign_transaction(tx, private_key=private_key)
     logger.debug("Sending transaction " + str(tx))
     ret = w3.eth.send_raw_transaction(signed_tx.rawTransaction)
     logger.debug("Transaction successfully sent !")
     logger.info(
@@ -92,34 +92,34 @@
     logger.info("Transaction mined !")
 
     return tx_receipt
 
 
 def start_quest_with_data(quest_address, data, hero_ids, attempts, private_key, nonce, gas_price_gwei, tx_timeout_seconds, rpc_address, logger):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
-    account = w3.eth.account.privateKeyToAccount(private_key)
+    account = w3.eth.account.from_key(private_key)
     w3.eth.default_account = account.address
 
-    contract_address = Web3.toChecksumAddress(CONTRACT_ADDRESS)
+    contract_address = Web3.to_checksum_address(CONTRACT_ADDRESS)
     contract = w3.eth.contract(contract_address, abi=ABI)
 
     if type(data) != tuple:
         raise Exception("Quest data must be a tuple")
 
     if len(data) != 12:
         raise Exception("Invalid quest data length (expected 12 but was "+str(len(data))+")")
 
     tx = contract.functions.startQuestWithData(hero_ids, quest_address, attempts, data)
 
     if isinstance(gas_price_gwei, dict):  # dynamic fee
-        tx = tx.buildTransaction(
-            {'maxFeePerGas': w3.toWei(gas_price_gwei['maxFeePerGas'], 'gwei'),
-             'maxPriorityFeePerGas': w3.toWei(gas_price_gwei['maxPriorityFeePerGas'], 'gwei'), 'nonce': nonce})
+        tx = tx.build_transaction(
+            {'maxFeePerGas': w3.to_wei(gas_price_gwei['maxFeePerGas'], 'gwei'),
+             'maxPriorityFeePerGas': w3.to_wei(gas_price_gwei['maxPriorityFeePerGas'], 'gwei'), 'nonce': nonce})
     else:  # legacy
-        tx = tx.buildTransaction({'gasPrice': w3.toWei(gas_price_gwei, 'gwei'), 'nonce': nonce})
+        tx = tx.build_transaction({'gasPrice': w3.to_wei(gas_price_gwei, 'gwei'), 'nonce': nonce})
 
     logger.debug("Signing transaction")
     signed_tx = w3.eth.account.sign_transaction(tx, private_key=private_key)
     logger.debug("Sending transaction " + str(tx))
     ret = w3.eth.send_raw_transaction(signed_tx.rawTransaction)
     logger.debug("Transaction successfully sent !")
     logger.info(
@@ -130,28 +130,28 @@
     logger.info("Transaction mined !")
 
     return tx_receipt
 
 
 def complete_quest(hero_id, private_key, nonce, gas_price_gwei, tx_timeout_seconds, rpc_address, logger):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
-    account = w3.eth.account.privateKeyToAccount(private_key)
+    account = w3.eth.account.from_key(private_key)
     w3.eth.default_account = account.address
 
-    contract_address = Web3.toChecksumAddress(CONTRACT_ADDRESS)
+    contract_address = Web3.to_checksum_address(CONTRACT_ADDRESS)
     contract = w3.eth.contract(contract_address, abi=ABI)
 
     tx = contract.functions.completeQuest(hero_id)
 
     if isinstance(gas_price_gwei, dict):  # dynamic fee
-        tx = tx.buildTransaction(
-            {'maxFeePerGas': w3.toWei(gas_price_gwei['maxFeePerGas'], 'gwei'),
-             'maxPriorityFeePerGas': w3.toWei(gas_price_gwei['maxPriorityFeePerGas'], 'gwei'), 'nonce': nonce})
+        tx = tx.build_transaction(
+            {'maxFeePerGas': w3.to_wei(gas_price_gwei['maxFeePerGas'], 'gwei'),
+             'maxPriorityFeePerGas': w3.to_wei(gas_price_gwei['maxPriorityFeePerGas'], 'gwei'), 'nonce': nonce})
     else:  # legacy
-        tx = tx.buildTransaction({'gasPrice': w3.toWei(gas_price_gwei, 'gwei'), 'nonce': nonce})
+        tx = tx.build_transaction({'gasPrice': w3.to_wei(gas_price_gwei, 'gwei'), 'nonce': nonce})
 
     logger.debug("Signing transaction")
     signed_tx = w3.eth.account.sign_transaction(tx, private_key=private_key)
     logger.debug("Sending transaction " + str(tx))
     ret = w3.eth.send_raw_transaction(signed_tx.rawTransaction)
     logger.debug("Transaction successfully sent !")
     logger.info(
@@ -162,47 +162,47 @@
 
     return tx_receipt
 
 
 def parse_complete_quest_receipt(tx_receipt, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-    contract_address = Web3.toChecksumAddress(CONTRACT_ADDRESS)
+    contract_address = Web3.to_checksum_address(CONTRACT_ADDRESS)
     contract = w3.eth.contract(contract_address, abi=ABI)
 
     quest_result = {}
 
-    quest_reward = contract.events.QuestReward().processReceipt(tx_receipt)
+    quest_reward = contract.events.QuestReward().process_receipt(tx_receipt)
     quest_result['reward'] = quest_reward
 
-    quest_xp = contract.events.QuestXP().processReceipt(tx_receipt)
+    quest_xp = contract.events.QuestXP().process_receipt(tx_receipt)
     quest_result['xp'] = quest_xp
 
-    quest_skill_up = contract.events.QuestSkillUp().processReceipt(tx_receipt)
+    quest_skill_up = contract.events.QuestSkillUp().process_receipt(tx_receipt)
     quest_result['skillUp'] = quest_skill_up
 
     return quest_result
 
 
 def cancel_quest(hero_id, private_key, nonce, gas_price_gwei, tx_timeout_seconds, rpc_address, logger):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
-    account = w3.eth.account.privateKeyToAccount(private_key)
+    account = w3.eth.account.from_key(private_key)
     w3.eth.default_account = account.address
 
-    contract_address = Web3.toChecksumAddress(CONTRACT_ADDRESS)
+    contract_address = Web3.to_checksum_address(CONTRACT_ADDRESS)
     contract = w3.eth.contract(contract_address, abi=ABI)
 
     tx = contract.functions.cancelQuest(hero_id)
 
     if isinstance(gas_price_gwei, dict):  # dynamic fee
-        tx = tx.buildTransaction(
-            {'maxFeePerGas': w3.toWei(gas_price_gwei['maxFeePerGas'], 'gwei'),
-             'maxPriorityFeePerGas': w3.toWei(gas_price_gwei['maxPriorityFeePerGas'], 'gwei'), 'nonce': nonce})
+        tx = tx.build_transaction(
+            {'maxFeePerGas': w3.to_wei(gas_price_gwei['maxFeePerGas'], 'gwei'),
+             'maxPriorityFeePerGas': w3.to_wei(gas_price_gwei['maxPriorityFeePerGas'], 'gwei'), 'nonce': nonce})
     else:  # legacy
-        tx = tx.buildTransaction({'gasPrice': w3.toWei(gas_price_gwei, 'gwei'), 'nonce': nonce})
+        tx = tx.build_transaction({'gasPrice': w3.to_wei(gas_price_gwei, 'gwei'), 'nonce': nonce})
 
     logger.debug("Signing transaction")
     signed_tx = w3.eth.account.sign_transaction(tx, private_key=private_key)
     logger.debug("Sending transaction " + str(tx))
     ret = w3.eth.send_raw_transaction(signed_tx.rawTransaction)
     logger.debug("Transaction successfully sent !")
     logger.info(
@@ -212,81 +212,81 @@
     logger.info("Transaction mined !")
 
     return tx_receipt
 
 
 def hero_to_quest_id(hero_id, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
-    contract_address = Web3.toChecksumAddress(CONTRACT_ADDRESS)
+    contract_address = Web3.to_checksum_address(CONTRACT_ADDRESS)
     contract = w3.eth.contract(contract_address, abi=ABI)
     result = contract.functions.heroToQuest(hero_id).call()
 
     return result
 
 
 def get_active_quest(address, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-    contract_address = Web3.toChecksumAddress(CONTRACT_ADDRESS)
+    contract_address = Web3.to_checksum_address(CONTRACT_ADDRESS)
     contract = w3.eth.contract(contract_address, abi=ABI)
     result = contract.functions.getActiveQuests(address).call()
 
     return result
 
 
 def get_hero_quest(hero_id, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-    contract_address = Web3.toChecksumAddress(CONTRACT_ADDRESS)
+    contract_address = Web3.to_checksum_address(CONTRACT_ADDRESS)
     contract = w3.eth.contract(contract_address, abi=ABI)
     result = contract.functions.getHeroQuest(hero_id).call()
 
     if result[0] <= 0:
         return None
 
     return result
 
 
 def get_quest(quest_id, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-    contract_address = Web3.toChecksumAddress(CONTRACT_ADDRESS)
+    contract_address = Web3.to_checksum_address(CONTRACT_ADDRESS)
     contract = w3.eth.contract(contract_address, abi=ABI)
     result = contract.functions.getQuest(quest_id).call()
 
     if result[0] <= 0:
         return None
 
     return result
 
 
 def get_quest_data(quest_id, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-    contract_address = Web3.toChecksumAddress(CONTRACT_ADDRESS)
+    contract_address = Web3.to_checksum_address(CONTRACT_ADDRESS)
     contract = w3.eth.contract(contract_address, abi=ABI)
     result = contract.functions.getQuestData(quest_id).call()
 
     return result
 
 
 def quest_address_to_type(quest_address, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-    contract_address = Web3.toChecksumAddress(CONTRACT_ADDRESS)
+    contract_address = Web3.to_checksum_address(CONTRACT_ADDRESS)
     contract = w3.eth.contract(contract_address, abi=ABI)
     result = contract.functions.questAddressToType(quest_address).call()
 
     return result
 
 
 def get_current_stamina(hero_id, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-    contract_address = Web3.toChecksumAddress(CONTRACT_ADDRESS)
+    contract_address = Web3.to_checksum_address(CONTRACT_ADDRESS)
     contract = w3.eth.contract(contract_address, abi=ABI)
     result = contract.functions.getCurrentStamina(hero_id).call()
 
     return result
```

### Comparing `dfktools-0.2.0/src/dfktools/quests/quest_core_v2.py` & `dfktools-0.3.0/src/dfktools/quests/quest_core_v2.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,27 +76,27 @@
         return 'https://scope.klaytn.com/tx/' + str(txid)
     else:
         return str(txid)
 
 
 def start_quest(quest_core_contract_address, quest_address, hero_ids, attempts, level, private_key, nonce, gas_price_gwei, tx_timeout_seconds, rpc_address, logger):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
-    account = w3.eth.account.privateKeyToAccount(private_key)
+    account = w3.eth.account.from_key(private_key)
     w3.eth.default_account = account.address
 
-    quest_core_contract_address = Web3.toChecksumAddress(quest_core_contract_address)
+    quest_core_contract_address = Web3.to_checksum_address(quest_core_contract_address)
     contract = w3.eth.contract(quest_core_contract_address, abi=ABI)
 
     if isinstance(gas_price_gwei, dict):   # dynamic fee
-        tx = contract.functions.startQuest(hero_ids, quest_address, attempts, level).buildTransaction(
-            {'maxFeePerGas': w3.toWei(gas_price_gwei['maxFeePerGas'], 'gwei'),
-             'maxPriorityFeePerGas': w3.toWei(gas_price_gwei['maxPriorityFeePerGas'], 'gwei'), 'nonce': nonce})
+        tx = contract.functions.startQuest(hero_ids, quest_address, attempts, level).build_transaction(
+            {'maxFeePerGas': w3.to_wei(gas_price_gwei['maxFeePerGas'], 'gwei'),
+             'maxPriorityFeePerGas': w3.to_wei(gas_price_gwei['maxPriorityFeePerGas'], 'gwei'), 'nonce': nonce})
     else:   # legacy
-        tx = contract.functions.startQuest(hero_ids, quest_address, attempts, level).buildTransaction(
-            {'gasPrice': w3.toWei(gas_price_gwei, 'gwei'), 'nonce': nonce})
+        tx = contract.functions.startQuest(hero_ids, quest_address, attempts, level).build_transaction(
+            {'gasPrice': w3.to_wei(gas_price_gwei, 'gwei'), 'nonce': nonce})
 
     logger.debug("Signing transaction")
     signed_tx = w3.eth.account.sign_transaction(tx, private_key=private_key)
     logger.debug("Sending transaction " + str(tx))
     ret = w3.eth.send_raw_transaction(signed_tx.rawTransaction)
     logger.debug("Transaction successfully sent !")
     logger.info(
@@ -107,27 +107,27 @@
     logger.info("Transaction mined !")
 
     return tx_receipt
 
 
 def start_quests(quest_core_contract_address, quest_addresses, hero_idss, attempts, levels, private_key, nonce, gas_price_gwei, tx_timeout_seconds, rpc_address, logger):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
-    account = w3.eth.account.privateKeyToAccount(private_key)
+    account = w3.eth.account.from_key(private_key)
     w3.eth.default_account = account.address
 
-    quest_core_contract_address = Web3.toChecksumAddress(quest_core_contract_address)
+    quest_core_contract_address = Web3.to_checksum_address(quest_core_contract_address)
     contract = w3.eth.contract(quest_core_contract_address, abi=ABI)
 
     if isinstance(gas_price_gwei, dict):  # dynamic fee
-        tx = contract.functions.multiStartQuest(quest_addresses, hero_idss, attempts, levels).buildTransaction(
-            {'maxFeePerGas': w3.toWei(gas_price_gwei['maxFeePerGas'], 'gwei'),
-             'maxPriorityFeePerGas': w3.toWei(gas_price_gwei['maxPriorityFeePerGas'], 'gwei'), 'nonce': nonce})
+        tx = contract.functions.multiStartQuest(quest_addresses, hero_idss, attempts, levels).build_transaction(
+            {'maxFeePerGas': w3.to_wei(gas_price_gwei['maxFeePerGas'], 'gwei'),
+             'maxPriorityFeePerGas': w3.to_wei(gas_price_gwei['maxPriorityFeePerGas'], 'gwei'), 'nonce': nonce})
     else:  # legacy
-        tx = contract.functions.multiStartQuest(quest_addresses, hero_idss, attempts, levels).buildTransaction(
-            {'gasPrice': w3.toWei(gas_price_gwei, 'gwei'), 'nonce': nonce})
+        tx = contract.functions.multiStartQuest(quest_addresses, hero_idss, attempts, levels).build_transaction(
+            {'gasPrice': w3.to_wei(gas_price_gwei, 'gwei'), 'nonce': nonce})
 
     logger.debug("Signing transaction")
     signed_tx = w3.eth.account.sign_transaction(tx, private_key=private_key)
     logger.debug("Sending transaction " + str(tx))
     ret = w3.eth.send_raw_transaction(signed_tx.rawTransaction)
     logger.debug("Transaction successfully sent !")
     logger.info(
@@ -138,27 +138,27 @@
     logger.info("Transaction mined !")
 
     return tx_receipt
 
 
 def complete_quest(quest_core_contract_address, hero_id, private_key, nonce, gas_price_gwei, tx_timeout_seconds, rpc_address, logger):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
-    account = w3.eth.account.privateKeyToAccount(private_key)
+    account = w3.eth.account.from_key(private_key)
     w3.eth.default_account = account.address
 
-    quest_core_contract_address = Web3.toChecksumAddress(quest_core_contract_address)
+    quest_core_contract_address = Web3.to_checksum_address(quest_core_contract_address)
     contract = w3.eth.contract(quest_core_contract_address, abi=ABI)
 
     if isinstance(gas_price_gwei, dict):  # dynamic fee
-        tx = contract.functions.completeQuest(hero_id).buildTransaction(
-            {'maxFeePerGas': w3.toWei(gas_price_gwei['maxFeePerGas'], 'gwei'),
-             'maxPriorityFeePerGas': w3.toWei(gas_price_gwei['maxPriorityFeePerGas'], 'gwei'), 'nonce': nonce})
+        tx = contract.functions.completeQuest(hero_id).build_transaction(
+            {'maxFeePerGas': w3.to_wei(gas_price_gwei['maxFeePerGas'], 'gwei'),
+             'maxPriorityFeePerGas': w3.to_wei(gas_price_gwei['maxPriorityFeePerGas'], 'gwei'), 'nonce': nonce})
     else:  # legacy
-        tx = contract.functions.completeQuest(hero_id).buildTransaction(
-            {'gasPrice': w3.toWei(gas_price_gwei, 'gwei'), 'nonce': nonce})
+        tx = contract.functions.completeQuest(hero_id).build_transaction(
+            {'gasPrice': w3.to_wei(gas_price_gwei, 'gwei'), 'nonce': nonce})
 
     logger.debug("Signing transaction")
     signed_tx = w3.eth.account.sign_transaction(tx, private_key=private_key)
     logger.debug("Sending transaction " + str(tx))
     ret = w3.eth.send_raw_transaction(signed_tx.rawTransaction)
     logger.debug("Transaction successfully sent !")
     logger.info(
@@ -169,46 +169,46 @@
 
     return tx_receipt
 
 
 def parse_complete_quest_receipt(quest_core_contract_address, tx_receipt, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-    quest_core_contract_address = Web3.toChecksumAddress(quest_core_contract_address)
+    quest_core_contract_address = Web3.to_checksum_address(quest_core_contract_address)
     contract = w3.eth.contract(quest_core_contract_address, abi=ABI)
 
     quest_result = {}
 
-    quest_reward = contract.events.RewardMinted().processReceipt(tx_receipt)
+    quest_reward = contract.events.RewardMinted().process_receipt(tx_receipt)
     quest_result['reward'] = quest_reward
 
-    quest_xp = contract.events.QuestXP().processReceipt(tx_receipt)
+    quest_xp = contract.events.QuestXP().process_receipt(tx_receipt)
     quest_result['xp'] = quest_xp
 
-    quest_skill_up = contract.events.QuestSkillUp().processReceipt(tx_receipt)
+    quest_skill_up = contract.events.QuestSkillUp().process_receipt(tx_receipt)
     quest_result['skillUp'] = quest_skill_up
 
     return quest_result
 
 
 def cancel_quest(quest_core_contract_address, hero_id, private_key, nonce, gas_price_gwei, tx_timeout_seconds, rpc_address, logger):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
-    account = w3.eth.account.privateKeyToAccount(private_key)
+    account = w3.eth.account.from_key(private_key)
     w3.eth.default_account = account.address
 
-    quest_core_contract_address = Web3.toChecksumAddress(quest_core_contract_address)
+    quest_core_contract_address = Web3.to_checksum_address(quest_core_contract_address)
     contract = w3.eth.contract(quest_core_contract_address, abi=ABI)
 
     if isinstance(gas_price_gwei, dict):  # dynamic fee
-        tx = contract.functions.cancelQuest(hero_id).buildTransaction(
-            {'maxFeePerGas': w3.toWei(gas_price_gwei['maxFeePerGas'], 'gwei'),
-             'maxPriorityFeePerGas': w3.toWei(gas_price_gwei['maxPriorityFeePerGas'], 'gwei'), 'nonce': nonce})
+        tx = contract.functions.cancelQuest(hero_id).build_transaction(
+            {'maxFeePerGas': w3.to_wei(gas_price_gwei['maxFeePerGas'], 'gwei'),
+             'maxPriorityFeePerGas': w3.to_wei(gas_price_gwei['maxPriorityFeePerGas'], 'gwei'), 'nonce': nonce})
     else:  # legacy
-        tx = contract.functions.cancelQuest(hero_id).buildTransaction(
-            {'gasPrice': w3.toWei(gas_price_gwei, 'gwei'), 'nonce': nonce})
+        tx = contract.functions.cancelQuest(hero_id).build_transaction(
+            {'gasPrice': w3.to_wei(gas_price_gwei, 'gwei'), 'nonce': nonce})
 
     logger.debug("Signing transaction")
     signed_tx = w3.eth.account.sign_transaction(tx, private_key=private_key)
     logger.debug("Sending transaction " + str(tx))
     ret = w3.eth.send_raw_transaction(signed_tx.rawTransaction)
     logger.debug("Transaction successfully sent !")
     logger.info(
@@ -218,27 +218,27 @@
     logger.info("Transaction mined !")
 
     return tx_receipt
 
 
 def cancel_quests(quest_core_contract_address, hero_ids, private_key, nonce, gas_price_gwei, tx_timeout_seconds, rpc_address, logger):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
-    account = w3.eth.account.privateKeyToAccount(private_key)
+    account = w3.eth.account.from_key(private_key)
     w3.eth.default_account = account.address
 
-    quest_core_contract_address = Web3.toChecksumAddress(quest_core_contract_address)
+    quest_core_contract_address = Web3.to_checksum_address(quest_core_contract_address)
     contract = w3.eth.contract(quest_core_contract_address, abi=ABI)
 
     if isinstance(gas_price_gwei, dict):  # dynamic fee
-        tx = contract.functions.multiCancelQuest(hero_ids).buildTransaction(
-            {'maxFeePerGas': w3.toWei(gas_price_gwei['maxFeePerGas'], 'gwei'),
-             'maxPriorityFeePerGas': w3.toWei(gas_price_gwei['maxPriorityFeePerGas'], 'gwei'), 'nonce': nonce})
+        tx = contract.functions.multiCancelQuest(hero_ids).build_transaction(
+            {'maxFeePerGas': w3.to_wei(gas_price_gwei['maxFeePerGas'], 'gwei'),
+             'maxPriorityFeePerGas': w3.to_wei(gas_price_gwei['maxPriorityFeePerGas'], 'gwei'), 'nonce': nonce})
     else:  # legacy
-        tx = contract.functions.multiCancelQuest(hero_ids).buildTransaction(
-            {'gasPrice': w3.toWei(gas_price_gwei, 'gwei'), 'nonce': nonce})
+        tx = contract.functions.multiCancelQuest(hero_ids).build_transaction(
+            {'gasPrice': w3.to_wei(gas_price_gwei, 'gwei'), 'nonce': nonce})
 
     logger.debug("Signing transaction")
     signed_tx = w3.eth.account.sign_transaction(tx, private_key=private_key)
     logger.debug("Sending transaction " + str(tx))
     ret = w3.eth.send_raw_transaction(signed_tx.rawTransaction)
     logger.debug("Transaction successfully sent !")
     logger.info(
@@ -248,77 +248,77 @@
     logger.info("Transaction mined !")
 
     return tx_receipt
 
 
 def hero_to_quest_id(quest_core_contract_address, hero_id, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
-    quest_core_contract_address = Web3.toChecksumAddress(quest_core_contract_address)
+    quest_core_contract_address = Web3.to_checksum_address(quest_core_contract_address)
     contract = w3.eth.contract(quest_core_contract_address, abi=ABI)
     result = contract.functions.heroToQuest(hero_id).call()
 
     return result
 
 
 def get_active_quest(quest_core_contract_address, address, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-    quest_core_contract_address = Web3.toChecksumAddress(quest_core_contract_address)
+    quest_core_contract_address = Web3.to_checksum_address(quest_core_contract_address)
     contract = w3.eth.contract(quest_core_contract_address, abi=ABI)
     result = contract.functions.getAccountActiveQuests(address).call()
 
     return result
 
 
 def get_hero_quest(contract_address, hero_id, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-    contract_address = Web3.toChecksumAddress(contract_address)
+    contract_address = Web3.to_checksum_address(contract_address)
     contract = w3.eth.contract(contract_address, abi=ABI)
     result = contract.functions.getHeroQuest(hero_id).call()
 
     if result[0] <= 0:
         return None
 
     return result
 
 
 def get_quests(quest_core_contract_address, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-    quest_core_contract_address = Web3.toChecksumAddress(quest_core_contract_address)
+    quest_core_contract_address = Web3.to_checksum_address(quest_core_contract_address)
     contract = w3.eth.contract(quest_core_contract_address, abi=ABI)
     result = contract.functions.getQuestContracts().call()
 
     return result
 
 
 def is_quest(quest_core_contract_address, address, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-    quest_core_contract_address = Web3.toChecksumAddress(quest_core_contract_address)
+    quest_core_contract_address = Web3.to_checksum_address(quest_core_contract_address)
     contract = w3.eth.contract(quest_core_contract_address, abi=ABI)
     result = contract.functions.isQuest(address).call()
 
     return result
 
 
 def quest_address_to_type(quest_core_contract_address, quest_address, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-    quest_core_contract_address = Web3.toChecksumAddress(quest_core_contract_address)
+    quest_core_contract_address = Web3.to_checksum_address(quest_core_contract_address)
     contract = w3.eth.contract(quest_core_contract_address, abi=ABI)
     result = contract.functions.questAddressToType(quest_address).call()
 
     return result
 
 
 def get_current_stamina(quest_core_contract_address, hero_id, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-    quest_core_contract_address = Web3.toChecksumAddress(quest_core_contract_address)
+    quest_core_contract_address = Web3.to_checksum_address(quest_core_contract_address)
     contract = w3.eth.contract(quest_core_contract_address, abi=ABI)
     result = contract.functions.getCurrentStamina(hero_id).call()
 
     return result
```

### Comparing `dfktools-0.2.0/src/dfktools/quests/quest_v1.py` & `dfktools-0.3.0/src/dfktools/quests/quest_v1.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.2.0/src/dfktools/quests/quest_v2.py` & `dfktools-0.3.0/src/dfktools/quests/quest_v2.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.2.0/src/dfktools/quests/wishing_well.py` & `dfktools-0.3.0/src/dfktools/quests/wishing_well.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,23 +51,23 @@
 
 def block_explorer_link(txid):
     return 'https://explorer.harmony.one/tx/' + str(txid)
 
 
 def start_quest(hero_id, attempts, private_key, nonce, gas_price_gwei, tx_timeout_seconds, rpc_address, logger):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
-    account = w3.eth.account.privateKeyToAccount(private_key)
+    account = w3.eth.account.from_key(private_key)
     w3.eth.default_account = account.address
 
-    contract_address = Web3.toChecksumAddress(CONTRACT_ADDRESS)
+    contract_address = Web3.to_checksum_address(CONTRACT_ADDRESS)
     contract = w3.eth.contract(contract_address, abi=ABI)
 
     logger.info("Starting quest with hero id " + str(hero_id))
-    tx = contract.functions.startQuest(hero_id, attempts).buildTransaction(
-        {'gasPrice': w3.toWei(gas_price_gwei, 'gwei'), 'nonce': nonce})
+    tx = contract.functions.startQuest(hero_id, attempts).build_transaction(
+        {'gasPrice': w3.to_wei(gas_price_gwei, 'gwei'), 'nonce': nonce})
 
     logger.debug("Signing transaction")
     signed_tx = w3.eth.account.sign_transaction(tx, private_key=private_key)
     logger.debug("Sending transaction " + str(tx))
     ret = w3.eth.send_raw_transaction(signed_tx.rawTransaction)
     logger.debug("Transaction successfully sent !")
     logger.info(
@@ -77,23 +77,23 @@
                                                      poll_latency=2)
     logger.info("Transaction mined !")
     logger.info(str(tx_receipt))
 
 
 def complete_quest(hero_id, private_key, nonce, gas_price_gwei, tx_timeout_seconds, rpc_address, logger):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
-    account = w3.eth.account.privateKeyToAccount(private_key)
+    account = w3.eth.account.from_key(private_key)
     w3.eth.default_account = account.address
 
-    contract_address = Web3.toChecksumAddress(CONTRACT_ADDRESS)
+    contract_address = Web3.to_checksum_address(CONTRACT_ADDRESS)
     contract = w3.eth.contract(contract_address, abi=ABI)
 
     logger.debug("Completing quest with hero id " + str(hero_id))
-    tx = contract.functions.completeQuest(hero_id).buildTransaction(
-        {'gasPrice': w3.toWei(gas_price_gwei, 'gwei'), 'nonce': nonce})
+    tx = contract.functions.completeQuest(hero_id).build_transaction(
+        {'gasPrice': w3.to_wei(gas_price_gwei, 'gwei'), 'nonce': nonce})
 
     logger.debug("Signing transaction")
     signed_tx = w3.eth.account.sign_transaction(tx, private_key=private_key)
     logger.debug("Sending transaction " + str(tx))
     ret = w3.eth.send_raw_transaction(signed_tx.rawTransaction)
     logger.debug("Transaction successfully sent !")
     logger.info(
@@ -105,66 +105,66 @@
 
     return tx_receipt
 
 
 def parse_complete_quest_receipt(tx_receipt, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-    contract_address = Web3.toChecksumAddress(CONTRACT_ADDRESS)
+    contract_address = Web3.to_checksum_address(CONTRACT_ADDRESS)
     contract = w3.eth.contract(contract_address, abi=ABI)
 
     quest_result = {}
 
-    quest_reward = contract.events.QuestReward().processReceipt(tx_receipt)
+    quest_reward = contract.events.QuestReward().process_receipt(tx_receipt)
     quest_result['tear'] = sum([result.args.itemQuantity for result in quest_reward])
 
-    quest_xp = contract.events.QuestXP().processReceipt(tx_receipt)
+    quest_xp = contract.events.QuestXP().process_receipt(tx_receipt)
     quest_result['xp'] = sum([result.args.xpEarned for result in quest_xp])
 
     return quest_result
 
 
 def quest_level(rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
-    contract_address = Web3.toChecksumAddress(CONTRACT_ADDRESS)
+    contract_address = Web3.to_checksum_address(CONTRACT_ADDRESS)
     contract = w3.eth.contract(contract_address, abi=ABI)
     result = contract.functions.questLevel().call()
 
     return result
 
 
 def rewards(quest_id, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
-    contract_address = Web3.toChecksumAddress(CONTRACT_ADDRESS)
+    contract_address = Web3.to_checksum_address(CONTRACT_ADDRESS)
     contract = w3.eth.contract(contract_address, abi=ABI)
     result = contract.functions.rewardItems(quest_id).call()
 
     return result
 
 
 def last_reward_index(rpc_address):
 
     w3 = Web3(Web3.HTTPProvider(rpc_address))
-    contract_address = Web3.toChecksumAddress(CONTRACT_ADDRESS)
+    contract_address = Web3.to_checksum_address(CONTRACT_ADDRESS)
     contract = w3.eth.contract(contract_address, abi=ABI)
     result = contract.functions.lastRewardIndex().call()
 
     return result
 
 
 def hero_to_quest(hero_id, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
-    contract_address = Web3.toChecksumAddress(CONTRACT_ADDRESS)
+    contract_address = Web3.to_checksum_address(CONTRACT_ADDRESS)
     contract = w3.eth.contract(contract_address, abi=ABI)
     result = contract.functions.heroToQuest(hero_id).call()
 
     return result
 
 
 def get_current_stamina(hero_id, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-    contract_address = Web3.toChecksumAddress(CONTRACT_ADDRESS)
+    contract_address = Web3.to_checksum_address(CONTRACT_ADDRESS)
     contract = w3.eth.contract(contract_address, abi=ABI)
     result = contract.functions.getCurrentStamina(hero_id).call()
 
     return result
```

### Comparing `dfktools-0.2.0/src/dfktools/raffle/utils/utils.py` & `dfktools-0.3.0/src/dfktools/raffle/utils/utils.py`

 * *Files identical despite different names*

### Comparing `dfktools-0.2.0/src/dfktools/raffle_example.py` & `dfktools-0.3.0/src/dfktools/raffle_example.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
     rpc_server = 'https://subnets.avax.network/defi-kingdoms/dfk-chain/rpc'
     logger.info("Using RPC server " + rpc_server)
     realm_contract_address = raffle_master.CRYSTALVALE_CONTRACT_ADDRESS
 
     w3 = Web3(Web3.HTTPProvider(rpc_server))
     private_key = ""  # set private key
-    account_address = "0x"  # w3.eth.account.privateKeyToAccount(private_key).address
+    account_address = "0x"  # w3.eth.account.from_key(private_key).address
     gas_price_gwei = 115
     tx_timeout_seconds = 30
 
     # Get current raffles
     current_raffle = raffle_master.get_current_raffle_data(realm_contract_address, rpc_server)
 
     raffle_log = "Current raffle:"
@@ -44,9 +44,9 @@
     # Get raffle allowed maximum entries
     raffle_id = [current_raffle[0][0][0]]
     raffle_max_entries = raffle_master.get_raffle_tickets_allowance_list(realm_contract_address, raffle_id, rpc_server)
     logger.info("Maximum allowed entries for raffle {} : {}".format(raffle_id[0],  raffle_max_entries[0]))
 
     # Enter raffle
     raffle_master.enter_raffle(realm_contract_address, 3555, 1,
-                               private_key, w3.eth.getTransactionCount(account_address),
+                               private_key, w3.eth.get_transaction_count(account_address),
                                gas_price_gwei, tx_timeout_seconds, rpc_server, logger)
```

### Comparing `dfktools-0.2.0/src/dfktools/stone_carver/stone_carver.py` & `dfktools-0.3.0/src/dfktools/stone_carver/stone_carver.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,34 +56,35 @@
 		return 'https://subnets.avax.network/defi-kingdoms/dfk-chain/explorer/tx/' + str(txid)
 	else:
 		return str(txid)
 
 
 def away_until(contract_address, rpc_address):
 	w3 = Web3(Web3.HTTPProvider(rpc_address))
-	contract = w3.eth.contract(Web3.toChecksumAddress(contract_address), abi=ABI)
+	contract = w3.eth.contract(Web3.to_checksum_address(contract_address), abi=ABI)
 	return contract.functions.awayUntil().call()
 
 
 def carve_stone(contract_address, item_address, quantity, private_key, nonce, gas_price_gwei, tx_timeout_seconds,
 				rpc_address, logger):
 	w3 = Web3(Web3.HTTPProvider(rpc_address))
-	account = w3.eth.account.privateKeyToAccount(private_key)
+	account = w3.eth.account.from_key(private_key)
 	w3.eth.default_account = account.address
 
-	contract_address = Web3.toChecksumAddress(contract_address)
+	contract_address = Web3.to_checksum_address(contract_address)
 	contract = w3.eth.contract(contract_address, abi=ABI)
 
+	tx = contract.functions.carveStone(item_address, quantity)
+
 	if isinstance(gas_price_gwei, dict):  # dynamic fee
-		tx = contract.functions.carveStone(item_address, quantity).buildTransaction(
-			{'maxFeePerGas': w3.toWei(gas_price_gwei['maxFeePerGas'], 'gwei'),
-			 'maxPriorityFeePerGas': w3.toWei(gas_price_gwei['maxPriorityFeePerGas'], 'gwei'), 'nonce': nonce})
+		tx = tx.build_transaction(
+			{'maxFeePerGas': w3.to_wei(gas_price_gwei['maxFeePerGas'], 'gwei'),
+			 'maxPriorityFeePerGas': w3.to_wei(gas_price_gwei['maxPriorityFeePerGas'], 'gwei'), 'nonce': nonce})
 	else:  # legacy
-		tx = contract.functions.carveStone(item_address, quantity).buildTransaction(
-			{'gasPrice': w3.toWei(gas_price_gwei, 'gwei'), 'nonce': nonce})
+		tx = tx.build_transaction({'gasPrice': w3.to_wei(gas_price_gwei, 'gwei'), 'nonce': nonce})
 
 	logger.debug("Signing transaction")
 	signed_tx = w3.eth.account.sign_transaction(tx, private_key=private_key)
 	logger.debug("Sending transaction " + str(tx))
 	ret = w3.eth.send_raw_transaction(signed_tx.rawTransaction)
 	logger.debug("Transaction successfully sent !")
 	logger.info(
@@ -92,57 +93,58 @@
 													 poll_latency=2)
 	logger.info("Transaction mined !")
 	return tx_receipt
 
 
 def get_availability(contract_address, rpc_address):
 	w3 = Web3(Web3.HTTPProvider(rpc_address))
-	contract = w3.eth.contract(Web3.toChecksumAddress(contract_address), abi=ABI)
+	contract = w3.eth.contract(Web3.to_checksum_address(contract_address), abi=ABI)
 	return contract.functions.getAvailability().call()
 
 
 def get_recipe(contract_address, item_address, rpc_address):
 	w3 = Web3(Web3.HTTPProvider(rpc_address))
-	contract = w3.eth.contract(Web3.toChecksumAddress(contract_address), abi=ABI)
+	contract = w3.eth.contract(Web3.to_checksum_address(contract_address), abi=ABI)
 	return contract.functions.getRecipe(item_address).call()
 
 
 def min_closed_time(contract_address, rpc_address):
 	w3 = Web3(Web3.HTTPProvider(rpc_address))
-	contract = w3.eth.contract(Web3.toChecksumAddress(contract_address), abi=ABI)
+	contract = w3.eth.contract(Web3.to_checksum_address(contract_address), abi=ABI)
 	return contract.functions.minClosedTime().call()
 
 
 def min_open_time(contract_address, rpc_address):
 	w3 = Web3(Web3.HTTPProvider(rpc_address))
-	contract = w3.eth.contract(Web3.toChecksumAddress(contract_address), abi=ABI)
+	contract = w3.eth.contract(Web3.to_checksum_address(contract_address), abi=ABI)
 	return contract.functions.minOpenTime().call()
 
 
 def recipes(item_address, contract_address, rpc_address):
 	w3 = Web3(Web3.HTTPProvider(rpc_address))
-	contract = w3.eth.contract(Web3.toChecksumAddress(contract_address), abi=ABI)
+	contract = w3.eth.contract(Web3.to_checksum_address(contract_address), abi=ABI)
 	return contract.functions.recipes(item_address).call()
 
 
 def set_up_shop(contract_address, private_key, nonce, gas_price_gwei, tx_timeout_seconds, rpc_address, logger):
 	w3 = Web3(Web3.HTTPProvider(rpc_address))
-	account = w3.eth.account.privateKeyToAccount(private_key)
+	account = w3.eth.account.from_key(private_key)
 	w3.eth.default_account = account.address
 
-	contract_address = Web3.toChecksumAddress(contract_address)
+	contract_address = Web3.to_checksum_address(contract_address)
 	contract = w3.eth.contract(contract_address, abi=ABI)
 
+	tx = contract.functions.setUpShop()
+
 	if isinstance(gas_price_gwei, dict):  # dynamic fee
-		tx = contract.functions.setUpShop().buildTransaction(
-			{'maxFeePerGas': w3.toWei(gas_price_gwei['maxFeePerGas'], 'gwei'),
-			 'maxPriorityFeePerGas': w3.toWei(gas_price_gwei['maxPriorityFeePerGas'], 'gwei'), 'nonce': nonce})
+		tx = tx.build_transaction(
+			{'maxFeePerGas': w3.to_wei(gas_price_gwei['maxFeePerGas'], 'gwei'),
+			 'maxPriorityFeePerGas': w3.to_wei(gas_price_gwei['maxPriorityFeePerGas'], 'gwei'), 'nonce': nonce})
 	else:  # legacy
-		tx = contract.functions.setUpShop().buildTransaction(
-			{'gasPrice': w3.toWei(gas_price_gwei, 'gwei'), 'nonce': nonce})
+		tx = tx.build_transaction({'gasPrice': w3.to_wei(gas_price_gwei, 'gwei'), 'nonce': nonce})
 
 	logger.debug("Signing transaction")
 	signed_tx = w3.eth.account.sign_transaction(tx, private_key=private_key)
 	logger.debug("Sending transaction " + str(tx))
 	ret = w3.eth.send_raw_transaction(signed_tx.rawTransaction)
 	logger.debug("Transaction successfully sent !")
 	logger.info(
@@ -151,21 +153,21 @@
 													 poll_latency=2)
 	logger.info("Transaction mined !")
 	return tx_receipt
 
 
 def var_closed_time(contract_address, rpc_address):
 	w3 = Web3(Web3.HTTPProvider(rpc_address))
-	contract = w3.eth.contract(Web3.toChecksumAddress(contract_address), abi=ABI)
+	contract = w3.eth.contract(Web3.to_checksum_address(contract_address), abi=ABI)
 	return contract.functions.varClosedTime().call()
 
 
 def var_open_time(contract_address, rpc_address):
 	w3 = Web3(Web3.HTTPProvider(rpc_address))
-	contract = w3.eth.contract(Web3.toChecksumAddress(contract_address), abi=ABI)
+	contract = w3.eth.contract(Web3.to_checksum_address(contract_address), abi=ABI)
 	return contract.functions.varOpenTime().call()
 
 
 def working_until(contract_address, rpc_address):
 	w3 = Web3(Web3.HTTPProvider(rpc_address))
-	contract = w3.eth.contract(Web3.toChecksumAddress(contract_address), abi=ABI)
+	contract = w3.eth.contract(Web3.to_checksum_address(contract_address), abi=ABI)
 	return contract.functions.workingUntil().call()
```

### Comparing `dfktools-0.2.0/src/dfktools/stone_carver_example.py` & `dfktools-0.3.0/src/dfktools/stone_carver_example.py`

 * *Files 12% similar despite different names*

```diff
@@ -30,11 +30,11 @@
     # Displays Working until Timestamp / whether SC is currently working
     working = stone_carver.working_until(realm_contract_address, rpc_server)
     logger.info(f"Working until: {working} / Currently Working: {True if time.time() < working else False}")
 
     # Crafting Lesser Chaos Stone
     w3 = Web3(Web3.HTTPProvider(rpc_server))
     private_key = None  # set private key
-    account_address = w3.eth.account.privateKeyToAccount(private_key).address
+    account_address = w3.eth.account.from_key(private_key).address
     gas_price_gwei = 100
     tx_timeout_seconds = 30
-    stone_carver.carve_stone(realm_contract_address, lesser_chaos_stone_address, 1, private_key, w3.eth.getTransactionCount(account_address), gas_price_gwei, tx_timeout_seconds, rpc_server, logger)
+    stone_carver.carve_stone(realm_contract_address, lesser_chaos_stone_address, 1, private_key, w3.eth.get_transaction_count(account_address), gas_price_gwei, tx_timeout_seconds, rpc_server, logger)
```

### Comparing `dfktools-0.2.0/src/dfktools/summoning/assisting.py` & `dfktools-0.3.0/src/dfktools/summoning/assisting.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,25 +64,25 @@
         return str(txid)
 
 
 def is_on_rent(contract_address, hero_id, rpc_address):
 
     w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-    contract_address = Web3.toChecksumAddress(contract_address)
+    contract_address = Web3.to_checksum_address(contract_address)
     contract = w3.eth.contract(contract_address, abi=ABI)
 
     return contract.functions.isOnAuction(hero_id).call()
 
 
 def get_rent_auction(contract_address, hero_id, rpc_address):
 
     w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-    contract_address = Web3.toChecksumAddress(contract_address)
+    contract_address = Web3.to_checksum_address(contract_address)
     contract = w3.eth.contract(contract_address, abi=ABI)
 
     ret = contract.functions.getAuction(hero_id).call()
 
     auction = {}
     auction['auctionId'] = ret[0]
     auction['seller'] = ret[1]
@@ -92,27 +92,27 @@
     auction['startedAt'] = ret[5]
 
     return auction
 
 
 def put_hero_for_rent(contract_address, hero_id, price_gwei, private_key, nonce, gas_price_gwei, tx_timeout_seconds, rpc_address, logger=None):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
-    account = w3.eth.account.privateKeyToAccount(private_key)
+    account = w3.eth.account.from_key(private_key)
     w3.eth.default_account = account.address
 
-    contract_address = Web3.toChecksumAddress(contract_address)
+    contract_address = Web3.to_checksum_address(contract_address)
     contract = w3.eth.contract(contract_address, abi=ABI)
 
     tx = contract.functions.createAuction(hero_id, price_gwei, price_gwei, 60, '0x0000000000000000000000000000000000000000')
     if isinstance(gas_price_gwei, dict):  # dynamic fee
-        tx = tx.buildTransaction(
-            {'maxFeePerGas': w3.toWei(gas_price_gwei['maxFeePerGas'], 'gwei'),
-             'maxPriorityFeePerGas': w3.toWei(gas_price_gwei['maxPriorityFeePerGas'], 'gwei'), 'nonce': nonce})
+        tx = tx.build_transaction(
+            {'maxFeePerGas': w3.to_wei(gas_price_gwei['maxFeePerGas'], 'gwei'),
+             'maxPriorityFeePerGas': w3.to_wei(gas_price_gwei['maxPriorityFeePerGas'], 'gwei'), 'nonce': nonce})
     else:  # legacy
-        tx = tx.buildTransaction({'gasPrice': w3.toWei(gas_price_gwei, 'gwei'), 'nonce': nonce})
+        tx = tx.build_transaction({'gasPrice': w3.to_wei(gas_price_gwei, 'gwei'), 'nonce': nonce})
     if logger is not None:
         logger.debug("Signing transaction")
     signed_tx = w3.eth.account.sign_transaction(tx, private_key=private_key)
     if logger is not None:
         logger.debug("Sending transaction " + str(tx))
     ret = w3.eth.send_raw_transaction(signed_tx.rawTransaction)
     if logger is not None:
@@ -125,29 +125,29 @@
         logger.info("Transaction mined !")
         logger.info(str(tx_receipt))
     return tx_receipt
 
 
 def cancel_rent(contract_address, hero_id, private_key, nonce, gas_price_gwei, tx_timeout_seconds, rpc_address, logger=None):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
-    account = w3.eth.account.privateKeyToAccount(private_key)
+    account = w3.eth.account.from_key(private_key)
     w3.eth.default_account = account.address
 
-    contract_address = Web3.toChecksumAddress(contract_address)
+    contract_address = Web3.to_checksum_address(contract_address)
     contract = w3.eth.contract(contract_address, abi=ABI)
     if logger is not None:
         logger.info("Cancel renting of hero " + str(hero_id))
 
     tx = contract.functions.cancelAuction(hero_id)
     if isinstance(gas_price_gwei, dict):  # dynamic fee
-        tx = tx.buildTransaction(
-            {'maxFeePerGas': w3.toWei(gas_price_gwei['maxFeePerGas'], 'gwei'),
-             'maxPriorityFeePerGas': w3.toWei(gas_price_gwei['maxPriorityFeePerGas'], 'gwei'), 'nonce': nonce})
+        tx = tx.build_transaction(
+            {'maxFeePerGas': w3.to_wei(gas_price_gwei['maxFeePerGas'], 'gwei'),
+             'maxPriorityFeePerGas': w3.to_wei(gas_price_gwei['maxPriorityFeePerGas'], 'gwei'), 'nonce': nonce})
     else:  # legacy
-        tx = tx.buildTransaction({'gasPrice': w3.toWei(gas_price_gwei, 'gwei'), 'nonce': nonce})
+        tx = tx.build_transaction({'gasPrice': w3.to_wei(gas_price_gwei, 'gwei'), 'nonce': nonce})
     if logger is not None:
         logger.debug("Signing transaction")
     signed_tx = w3.eth.account.sign_transaction(tx, private_key=private_key)
     if logger is not None:
         logger.debug("Sending transaction " + str(tx))
     ret = w3.eth.send_raw_transaction(signed_tx.rawTransaction)
     if logger is not None:
```

### Comparing `dfktools-0.2.0/src/dfktools/summoning/crystals.py` & `dfktools-0.3.0/src/dfktools/summoning/crystals.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,39 +33,39 @@
         ]
         """
 
 
 def get_user_crystal_ids(user_address, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-    contract_address = Web3.toChecksumAddress(SERENDALE_CONTRACT_ADDRESS)
+    contract_address = Web3.to_checksum_address(SERENDALE_CONTRACT_ADDRESS)
     contract = w3.eth.contract(contract_address, abi=ABI)
 
-    return contract.functions.getUserCrystals(Web3.toChecksumAddress(user_address)).call()
+    return contract.functions.getUserCrystals(Web3.to_checksum_address(user_address)).call()
 
 
 def open_crystal(crystal_id, owner_private_key, owner_nonce, gas_price_gwei, rpc_address, contract_abi, logger):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
-    account = w3.eth.account.privateKeyToAccount(owner_private_key)
+    account = w3.eth.account.from_key(owner_private_key)
 
-    contract_address = Web3.toChecksumAddress(SERENDALE_CONTRACT_ADDRESS)
+    contract_address = Web3.to_checksum_address(SERENDALE_CONTRACT_ADDRESS)
     contract = w3.eth.contract(contract_address, abi=ABI)
 
     fast_open_crystal(crystal_id, account.address, owner_private_key, owner_nonce, gas_price_gwei, contract, w3, logger)
 
 
 def fast_open_crystal(crystal_id, owner_address, private_key, nonce, gas_price_gwei, contract, w3, logger):
     w3.eth.default_account = owner_address
     tx = contract.functions.open(crystal_id)
     if isinstance(gas_price_gwei, dict):  # dynamic fee
-        tx = tx.buildTransaction(
-            {'maxFeePerGas': w3.toWei(gas_price_gwei['maxFeePerGas'], 'gwei'),
-             'maxPriorityFeePerGas': w3.toWei(gas_price_gwei['maxPriorityFeePerGas'], 'gwei'), 'nonce': nonce})
+        tx = tx.build_transaction(
+            {'maxFeePerGas': w3.to_wei(gas_price_gwei['maxFeePerGas'], 'gwei'),
+             'maxPriorityFeePerGas': w3.to_wei(gas_price_gwei['maxPriorityFeePerGas'], 'gwei'), 'nonce': nonce})
     else:  # legacy
-        tx = tx.buildTransaction({'gasPrice': w3.toWei(gas_price_gwei, 'gwei'), 'nonce': nonce})
+        tx = tx.build_transaction({'gasPrice': w3.to_wei(gas_price_gwei, 'gwei'), 'nonce': nonce})
     logger.debug("Signing transaction")
     signed_tx = w3.eth.account.sign_transaction(tx, private_key=private_key)
     logger.debug("Sending transaction " + str(tx))
     ret = w3.eth.send_raw_transaction(signed_tx.rawTransaction)
     logger.debug("Transaction successfully sent !")
     logger.info(
         "Waiting for transaction https://explorer.harmony.one/tx/" + str(signed_tx.hash.hex()) + " to be mined")
```

### Comparing `dfktools-0.2.0/src/dfktools/summoning/crystals_v2.py` & `dfktools-0.3.0/src/dfktools/summoning/crystals_v2.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,36 +86,36 @@
         return 'https://scope.klaytn.com/tx/' + str(txid)
     else:
         return str(txid)
 
 def get_user_crystal_ids(contract_address, user_address, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-    contract_address = Web3.toChecksumAddress(contract_address)
+    contract_address = Web3.to_checksum_address(contract_address)
     contract = w3.eth.contract(contract_address, abi=ABI)
 
-    return contract.functions.getUserCrystals(Web3.toChecksumAddress(user_address)).call()
+    return contract.functions.getUserCrystals(Web3.to_checksum_address(user_address)).call()
 
 
 def summon_crystal(contract_address, summoner_id, assistant_id, summoner_tears, assistant_tears, private_key, nonce, gas_price_gwei, tx_timeout_seconds, rpc_address, logger=None):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
-    account = w3.eth.account.privateKeyToAccount(private_key)
+    account = w3.eth.account.from_key(private_key)
     w3.eth.default_account = account.address
 
-    contract_address = Web3.toChecksumAddress(contract_address)
+    contract_address = Web3.to_checksum_address(contract_address)
     contract = w3.eth.contract(contract_address, abi=ABI)
     if logger is not None:
         logger.info("Summoning with " + str(summoner_id) + " & "+str(assistant_id))
     tx = contract.functions.summonCrystal(summoner_id, assistant_id, summoner_tears, assistant_tears, '0x0000000000000000000000000000000000000000')
     if isinstance(gas_price_gwei, dict):  # dynamic fee
-        tx = tx.buildTransaction(
-            {'maxFeePerGas': w3.toWei(gas_price_gwei['maxFeePerGas'], 'gwei'),
-             'maxPriorityFeePerGas': w3.toWei(gas_price_gwei['maxPriorityFeePerGas'], 'gwei'), 'nonce': nonce})
+        tx = tx.build_transaction(
+            {'maxFeePerGas': w3.to_wei(gas_price_gwei['maxFeePerGas'], 'gwei'),
+             'maxPriorityFeePerGas': w3.to_wei(gas_price_gwei['maxPriorityFeePerGas'], 'gwei'), 'nonce': nonce})
     else:  # legacy
-        tx = tx.buildTransaction({'gasPrice': w3.toWei(gas_price_gwei, 'gwei'), 'nonce': nonce})
+        tx = tx.build_transaction({'gasPrice': w3.to_wei(gas_price_gwei, 'gwei'), 'nonce': nonce})
     if logger is not None:
         logger.debug("Signing transaction")
     signed_tx = w3.eth.account.sign_transaction(tx, private_key=private_key)
     if logger is not None:
         logger.debug("Sending transaction " + str(tx))
     ret = w3.eth.send_raw_transaction(signed_tx.rawTransaction)
     if logger is not None:
@@ -128,28 +128,28 @@
         logger.info("Transaction mined !")
         logger.info(str(tx_receipt))
     return tx_receipt
 
 
 def open_crystal(contract_address, crystal_id, private_key, nonce, gas_price_gwei, tx_timeout_seconds, rpc_address, logger):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
-    account = w3.eth.account.privateKeyToAccount(private_key)
+    account = w3.eth.account.from_key(private_key)
     w3.eth.default_account = account.address
 
-    contract_address = Web3.toChecksumAddress(contract_address)
+    contract_address = Web3.to_checksum_address(contract_address)
     contract = w3.eth.contract(contract_address, abi=ABI)
     if logger is not None:
         logger.info("Opening crystal "+str(crystal_id))
     tx = contract.functions.open(crystal_id)
     if isinstance(gas_price_gwei, dict):  # dynamic fee
-        tx = tx.buildTransaction(
-            {'maxFeePerGas': w3.toWei(gas_price_gwei['maxFeePerGas'], 'gwei'),
-             'maxPriorityFeePerGas': w3.toWei(gas_price_gwei['maxPriorityFeePerGas'], 'gwei'), 'nonce': nonce})
+        tx = tx.build_transaction(
+            {'maxFeePerGas': w3.to_wei(gas_price_gwei['maxFeePerGas'], 'gwei'),
+             'maxPriorityFeePerGas': w3.to_wei(gas_price_gwei['maxPriorityFeePerGas'], 'gwei'), 'nonce': nonce})
     else:  # legacy
-        tx = tx.buildTransaction({'gasPrice': w3.toWei(gas_price_gwei, 'gwei'), 'nonce': nonce})
+        tx = tx.build_transaction({'gasPrice': w3.to_wei(gas_price_gwei, 'gwei'), 'nonce': nonce})
     if logger is not None:
         logger.debug("Signing transaction")
     signed_tx = w3.eth.account.sign_transaction(tx, private_key=private_key)
     if logger is not None:
         logger.debug("Sending transaction " + str(tx))
     ret = w3.eth.send_raw_transaction(signed_tx.rawTransaction)
     if logger is not None:
```

### Comparing `dfktools-0.2.0/src/dfktools/summoning/serendale_assisting.py` & `dfktools-0.3.0/src/dfktools/summoning/serendale_assisting.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,25 +33,25 @@
     return 'https://explorer.harmony.one/tx/' + str(txid)
 
 
 def is_on_rent(hero_id, rpc_address):
 
     w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-    contract_address = Web3.toChecksumAddress(SERENDALE_CONTRACT_ADDRESS)
+    contract_address = Web3.to_checksum_address(SERENDALE_CONTRACT_ADDRESS)
     contract = w3.eth.contract(contract_address, abi=ABI)
 
     return contract.functions.isOnAuction(hero_id).call()
 
 
 def get_rent_auction(hero_id, rpc_address):
 
     w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-    contract_address = Web3.toChecksumAddress(SERENDALE_CONTRACT_ADDRESS)
+    contract_address = Web3.to_checksum_address(SERENDALE_CONTRACT_ADDRESS)
     contract = w3.eth.contract(contract_address, abi=ABI)
 
     ret = contract.functions.getAuction(hero_id).call()
 
     auction = {}
     auction['auctionId'] = ret[0]
     auction['seller'] = ret[1]
@@ -61,29 +61,29 @@
     auction['startedAt'] = ret[5]
 
     return auction
 
 
 def put_hero_for_rent(hero_id, price_gwei, private_key, nonce, gas_price_gwei, tx_timeout_seconds, rpc_address, logger=None):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
-    account = w3.eth.account.privateKeyToAccount(private_key)
+    account = w3.eth.account.from_key(private_key)
     w3.eth.default_account = account.address
 
-    contract_address = Web3.toChecksumAddress(SERENDALE_CONTRACT_ADDRESS)
+    contract_address = Web3.to_checksum_address(SERENDALE_CONTRACT_ADDRESS)
     contract = w3.eth.contract(contract_address, abi=ABI)
     if logger is not None:
         logger.info("Renting hero " + str(hero_id) + " for " + str(price_gwei/1000000000000000000) + " JEWEL")
 
     tx = contract.functions.createAuction(hero_id, price_gwei, price_gwei, 60, '0x0000000000000000000000000000000000000000')
     if isinstance(gas_price_gwei, dict):  # dynamic fee
-        tx = tx.buildTransaction(
-            {'maxFeePerGas': w3.toWei(gas_price_gwei['maxFeePerGas'], 'gwei'),
-             'maxPriorityFeePerGas': w3.toWei(gas_price_gwei['maxPriorityFeePerGas'], 'gwei'), 'nonce': nonce})
+        tx = tx.build_transaction(
+            {'maxFeePerGas': w3.to_wei(gas_price_gwei['maxFeePerGas'], 'gwei'),
+             'maxPriorityFeePerGas': w3.to_wei(gas_price_gwei['maxPriorityFeePerGas'], 'gwei'), 'nonce': nonce})
     else:  # legacy
-        tx = tx.buildTransaction({'gasPrice': w3.toWei(gas_price_gwei, 'gwei'), 'nonce': nonce})
+        tx = tx.build_transaction({'gasPrice': w3.to_wei(gas_price_gwei, 'gwei'), 'nonce': nonce})
     if logger is not None:
         logger.debug("Signing transaction")
     signed_tx = w3.eth.account.sign_transaction(tx, private_key=private_key)
     if logger is not None:
         logger.debug("Sending transaction " + str(tx))
     ret = w3.eth.send_raw_transaction(signed_tx.rawTransaction)
     if logger is not None:
@@ -96,29 +96,29 @@
         logger.info("Transaction mined !")
         logger.info(str(tx_receipt))
     return tx_receipt
 
 
 def cancel_rent(hero_id, private_key, nonce, gas_price_gwei, tx_timeout_seconds, rpc_address, logger=None):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
-    account = w3.eth.account.privateKeyToAccount(private_key)
+    account = w3.eth.account.from_key(private_key)
     w3.eth.default_account = account.address
 
-    contract_address = Web3.toChecksumAddress(SERENDALE_CONTRACT_ADDRESS)
+    contract_address = Web3.to_checksum_address(SERENDALE_CONTRACT_ADDRESS)
     contract = w3.eth.contract(contract_address, abi=ABI)
     if logger is not None:
         logger.info("Cancel renting of hero " + str(hero_id))
 
     tx = contract.functions.cancelAuction(hero_id)
     if isinstance(gas_price_gwei, dict):  # dynamic fee
-        tx = tx.buildTransaction(
-            {'maxFeePerGas': w3.toWei(gas_price_gwei['maxFeePerGas'], 'gwei'),
-             'maxPriorityFeePerGas': w3.toWei(gas_price_gwei['maxPriorityFeePerGas'], 'gwei'), 'nonce': nonce})
+        tx = tx.build_transaction(
+            {'maxFeePerGas': w3.to_wei(gas_price_gwei['maxFeePerGas'], 'gwei'),
+             'maxPriorityFeePerGas': w3.to_wei(gas_price_gwei['maxPriorityFeePerGas'], 'gwei'), 'nonce': nonce})
     else:  # legacy
-        tx = tx.buildTransaction({'gasPrice': w3.toWei(gas_price_gwei, 'gwei'), 'nonce': nonce})
+        tx = tx.build_transaction({'gasPrice': w3.to_wei(gas_price_gwei, 'gwei'), 'nonce': nonce})
     if logger is not None:
         logger.debug("Signing transaction")
     signed_tx = w3.eth.account.sign_transaction(tx, private_key=private_key)
     if logger is not None:
         logger.debug("Sending transaction " + str(tx))
     ret = w3.eth.send_raw_transaction(signed_tx.rawTransaction)
     if logger is not None:
```

### Comparing `dfktools-0.2.0/src/dfktools/summoning/summoning.py` & `dfktools-0.3.0/src/dfktools/summoning/summoning.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,36 +75,36 @@
     else:
         return str(txid)
 
 
 def get_user_crystal_ids(contract_address, user_address, rpc_address):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
 
-    contract_address = Web3.toChecksumAddress(contract_address)
+    contract_address = Web3.to_checksum_address(contract_address)
     contract = w3.eth.contract(contract_address, abi=ABI)
 
-    return contract.functions.getUserCrystals(Web3.toChecksumAddress(user_address)).call()
+    return contract.functions.getUserCrystals(Web3.to_checksum_address(user_address)).call()
 
 
 def summon_crystal(contract_address, summoner_id, assistant_id, summoner_tears, assistant_tears, private_key, nonce, gas_price_gwei, tx_timeout_seconds, rpc_address, logger=None):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
-    account = w3.eth.account.privateKeyToAccount(private_key)
+    account = w3.eth.account.from_key(private_key)
     w3.eth.default_account = account.address
 
-    contract_address = Web3.toChecksumAddress(contract_address)
+    contract_address = Web3.to_checksum_address(contract_address)
     contract = w3.eth.contract(contract_address, abi=ABI)
     if logger is not None:
         logger.info("Summoning with " + str(summoner_id) + " & "+str(assistant_id))
     tx = contract.functions.summonCrystal(summoner_id, assistant_id, summoner_tears, assistant_tears, '0x0000000000000000000000000000000000000000')
     if isinstance(gas_price_gwei, dict):  # dynamic fee
-        tx = tx.buildTransaction(
-            {'maxFeePerGas': w3.toWei(gas_price_gwei['maxFeePerGas'], 'gwei'),
-             'maxPriorityFeePerGas': w3.toWei(gas_price_gwei['maxPriorityFeePerGas'], 'gwei'), 'nonce': nonce})
+        tx = tx.build_transaction(
+            {'maxFeePerGas': w3.to_wei(gas_price_gwei['maxFeePerGas'], 'gwei'),
+             'maxPriorityFeePerGas': w3.to_wei(gas_price_gwei['maxPriorityFeePerGas'], 'gwei'), 'nonce': nonce})
     else:  # legacy
-        tx = tx.buildTransaction({'gasPrice': w3.toWei(gas_price_gwei, 'gwei'), 'nonce': nonce})
+        tx = tx.build_transaction({'gasPrice': w3.to_wei(gas_price_gwei, 'gwei'), 'nonce': nonce})
     if logger is not None:
         logger.debug("Signing transaction")
     signed_tx = w3.eth.account.sign_transaction(tx, private_key=private_key)
     if logger is not None:
         logger.debug("Sending transaction " + str(tx))
     ret = w3.eth.send_raw_transaction(signed_tx.rawTransaction)
     if logger is not None:
@@ -117,28 +117,28 @@
         logger.info("Transaction mined !")
         logger.info(str(tx_receipt))
     return tx_receipt
 
 
 def open_crystal(contract_address, crystal_id, private_key, nonce, gas_price_gwei, tx_timeout_seconds, rpc_address, logger=None):
     w3 = Web3(Web3.HTTPProvider(rpc_address))
-    account = w3.eth.account.privateKeyToAccount(private_key)
+    account = w3.eth.account.from_key(private_key)
     w3.eth.default_account = account.address
 
-    contract_address = Web3.toChecksumAddress(contract_address)
+    contract_address = Web3.to_checksum_address(contract_address)
     contract = w3.eth.contract(contract_address, abi=ABI)
     if logger is not None:
         logger.info("Opening crystal "+str(crystal_id))
     tx = contract.functions.open(crystal_id)
     if isinstance(gas_price_gwei, dict):  # dynamic fee
-        tx = tx.buildTransaction(
-            {'maxFeePerGas': w3.toWei(gas_price_gwei['maxFeePerGas'], 'gwei'),
-             'maxPriorityFeePerGas': w3.toWei(gas_price_gwei['maxPriorityFeePerGas'], 'gwei'), 'nonce': nonce})
+        tx = tx.build_transaction(
+            {'maxFeePerGas': w3.to_wei(gas_price_gwei['maxFeePerGas'], 'gwei'),
+             'maxPriorityFeePerGas': w3.to_wei(gas_price_gwei['maxPriorityFeePerGas'], 'gwei'), 'nonce': nonce})
     else:  # legacy
-        tx = tx.buildTransaction({'gasPrice': w3.toWei(gas_price_gwei, 'gwei'), 'nonce': nonce})
+        tx = tx.build_transaction({'gasPrice': w3.to_wei(gas_price_gwei, 'gwei'), 'nonce': nonce})
     if logger is not None:
         logger.debug("Signing transaction")
     signed_tx = w3.eth.account.sign_transaction(tx, private_key=private_key)
     if logger is not None:
         logger.debug("Sending transaction " + str(tx))
     ret = w3.eth.send_raw_transaction(signed_tx.rawTransaction)
     if logger is not None:
@@ -153,12 +153,12 @@
     return tx_receipt
 
 
 def parse_opened_crystal(contract_address, tx_receipt, rpc_address):
     # Given the receipt from opening a crystal, return the id of the new hero
     w3 = Web3(Web3.HTTPProvider(rpc_address))
     contract = w3.eth.contract(contract_address, abi=ABI)
-    opened_info = contract.events.CrystalOpen().processReceipt(tx_receipt)
+    opened_info = contract.events.CrystalOpen().process_receipt(tx_receipt)
     hero_id = opened_info[0].args.heroId
     return hero_id
```

### Comparing `dfktools-0.2.0/src/dfktools/summoning_example.py` & `dfktools-0.3.0/src/dfktools/summoning_example.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,16 +64,16 @@
     hero_rank_2 = 'basic'
 
     hero_1_tears = tears_for_hero(hero_level_1, hero_rank_1, add_extra_tears=True)
     hero_2_tears = tears_for_hero(hero_level_2, hero_rank_2, add_extra_tears=True)
 
     w3 = Web3(Web3.HTTPProvider(rpc_server))
 
-    summoning.summon_crystal(contract_address, hero_id_1, hero_id_2, hero_1_tears, hero_2_tears, private_key, w3.eth.getTransactionCount(address), gas_price_gwei, tx_timeout, rpc_server, logger)
+    summoning.summon_crystal(contract_address, hero_id_1, hero_id_2, hero_1_tears, hero_2_tears, private_key, w3.eth.get_transaction_count(address), gas_price_gwei, tx_timeout, rpc_server, logger)
 
     crystals = summoning.get_user_crystal_ids(contract_address, address, rpc_server)
     if crystals:
         logger.info(f"Waiting 20 seconds before opening crystal {crystals[0]}")
         time.sleep(20)
-        tx_receipt = summoning.open_crystal(contract_address, crystals[0], private_key, w3.eth.getTransactionCount(address), gas_price_gwei, tx_timeout, rpc_server, logger)
+        tx_receipt = summoning.open_crystal(contract_address, crystals[0], private_key, w3.eth.get_transaction_count(address), gas_price_gwei, tx_timeout, rpc_server, logger)
         hero_id = summoning.parse_opened_crystal(contract_address, tx_receipt, rpc_server)
         logger.info("Summoned hero: " + str(hero_id))
```

### Comparing `dfktools-0.2.0/src/dfktools/wishing_well_quest_example.py` & `dfktools-0.3.0/src/dfktools/wishing_well_quest_example.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,17 +18,17 @@
     hero_id = 1  # <your hero id here>
     stamina = wishing_well.get_current_stamina(hero_id, rpc_server)
     logger.info("Current stamina on hero " + str(hero_id) + ": " + str(stamina))
 
     #w3 = Web3(Web3.HTTPProvider(rpc_server))
     #gas_price_gwei = 10
     #private_key = # set private key
-    #account_address = w3.eth.account.privateKeyToAccount(private_key).address
-    #wishing_well.start_quest(hero_id, 5, private_key, w3.eth.getTransactionCount(account_address), gas_price_gwei, 30, rpc_server, logger)
+    #account_address = w3.eth.account.from_key(private_key).address
+    #wishing_well.start_quest(hero_id, 5, private_key, w3.eth.get_transaction_count(account_address), gas_price_gwei, 30, rpc_server, logger)
     #time.sleep(60)
-    #tx_receipt = wishing_well.complete_quest(hero_id, private_key, w3.eth.getTransactionCount(account_address), gas_price_gwei, 30, rpc_server, logger)
+    #tx_receipt = wishing_well.complete_quest(hero_id, private_key, w3.eth.get_transaction_count(account_address), gas_price_gwei, 30, rpc_server, logger)
 
     #quest_result = wishing_well.parse_complete_quest_receipt(tx_receipt, rpc_server)
     #logger.info("Quest earned " + str(quest_result['tear']) + " tears and " + str(quest_result['xp']) + " xp")
```

### Comparing `dfktools-0.2.0/src/dfktools.egg-info/PKG-INFO` & `dfktools-0.3.0/src/dfktools.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dfktools
-Version: 0.2.0
+Version: 0.3.0
 Summary: A toolbox for DefiKingdoms
 Home-page: https://github.com/0rtis/dfktools
 Author: Ortis
 Author-email: Ortis <ortis@ortis.io>
 License: MIT License
         
         Copyright (c) 2022 Ortis (ortis@ortis.io)
@@ -40,42 +40,45 @@
 [![GitHub license](https://img.shields.io/github/license/0rtis/dfktools.svg?style=flat-square)](https://github.com/0rtis/dfktools/blob/master/LICENSE)
 [![GitHub stars](https://img.shields.io/github/stars/0rtis?style=flat-square)](https://github.com/0rtis)
 [![Join Discord](https://img.shields.io/discord/932350221256638564?label=discord&style=flat-square)](https://discord.gg/BMWKgZSXqJ)
 [![Join Discord](https://img.shields.io/discord/889216073906405507?label=discord&style=flat-square)](https://discord.gg/JvfPpV7but)
 [![Follow @twitter handle](https://img.shields.io/twitter/follow/Knockturn_io.svg?style=flat-square)](https://twitter.com/intent/follow?screen_name=ortis95)
 
 
-## DefiKingdoms contract
+Install with `pip install dfktools`
+
+https://pypi.org/project/dfktools/
+
+## DefiKingdoms toolbox
 
 This is a simple toolbox to interact with the contracts of [DefiKingdoms](https://defikingdoms.com/)
 
 *This software is not endorsed by, directly affiliated with, maintained, authorized, or sponsored by the DefiKingdoms team.
 All product and company names are the registered trademarks of their original owners.
 The use of any trade name or trademark is for identification and reference purposes only and does not imply any association with the trademark holder of their product brand.*
 
 <br/>
 
 **Like this project ? Consider supporting future developments by:**
 - Delegating AVAX to our Avalanche node **NodeID-4btZGj8TmrycK22kwgBK5wJEFighAFWiZ**
-- Delegating ADA to our [Cardano node [KTA]](https://pooltool.io/pool/991a64a6e3d866f4af4e0a2bfd61c15486a47ccc352e61e8a6b4fef8) **991a64a6e3d866f4af4e0a2bfd61c15486a47ccc352e61e8a6b4fef8**
 - Making a donation to **0xA68fBfa3E0c86D1f3fF071853df6DAe8753095E2**
 
 *Need help ? Join the [GameFi Developers Discord](https://discord.gg/JvfPpV7but)*
 
 ### Code guidelines
 1. Indent with Tab
 2. 1 empty line within a function, 2 empty lines between function
 3. Use *trait(s)* to name any or all of the 8 value `strength, agility, intelligence, wisdom, luck, vitality, endurance, dexterity`
 4. Use *ability(ies)* to name any or all of the 4 value `passive1, passive2, active1, active2`
 5. Use *stat(s)* as a generic term for any or all the characteristics of a hero (traits, abilities, HP, MP, stamina, etc)
 6. A function should support all realms, except if contracts differs across realms
 7. All hardcoded addresses should be [CheckSummed](https://ethsum.netlify.app/)
 8. Use `logging`, not `print`
 9. No other third-party libraries (if really needed, please explain why in the PR)
-10. A short & meaningful comment is superior to a long & unfathomable documentation
+10. A short & meaningful comment is better than a long & unfathomable documentation
 
 <br/>
 
 ### Hero contract
 The hero contract is accessible with [hero/hero.py](src/dfktools/hero/hero.py)
 
 #### Quickstart
```

### Comparing `dfktools-0.2.0/src/dfktools.egg-info/SOURCES.txt` & `dfktools-0.3.0/src/dfktools.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 src/dfktools/assisting_example.py
 src/dfktools/auction_example.py
 src/dfktools/bridge_example.py
 src/dfktools/consumable_example.py
 src/dfktools/dex_example.py
 src/dfktools/duel_example.py
 src/dfktools/erc20_example.py
+src/dfktools/genes_encode_example.py
 src/dfktools/genes_example.py
 src/dfktools/hero_example.py
 src/dfktools/land_example.py
 src/dfktools/meditation_example.py
 src/dfktools/pet_example.py
 src/dfktools/profile_example.py
 src/dfktools/quest_example.py
@@ -64,40 +65,43 @@
 src/dfktools/duel/duel.py
 src/dfktools/duel/utils/__init__.py
 src/dfktools/duel/utils/utils.py
 src/dfktools/genes/__init__.py
 src/dfktools/genes/gene_science_v1.py
 src/dfktools/genes/gene_science_v2.py
 src/dfktools/hero/__init__.py
-src/dfktools/hero/hero.py
 src/dfktools/hero/hero_core.py
+src/dfktools/hero/heroes.py
 src/dfktools/hero/utils/__init__.py
 src/dfktools/hero/utils/utils.py
 src/dfktools/land/__init__.py
 src/dfktools/land/land.py
 src/dfktools/land/utils/__init__.py
 src/dfktools/land/utils/utils.py
 src/dfktools/meditation/__init__.py
 src/dfktools/meditation/meditation.py
 src/dfktools/perilous_journey/__init__.py
 src/dfktools/perilous_journey/perilous_journey.py
 src/dfktools/pets/__init__.py
 src/dfktools/pets/exchange.py
 src/dfktools/pets/hatchery.py
 src/dfktools/pets/pet_core.py
+src/dfktools/pets/pets.py
 src/dfktools/pets/utils/__init__.py
 src/dfktools/pets/utils/utils.py
 src/dfktools/profile/__init__.py
 src/dfktools/profile/profile.py
 src/dfktools/profile/profile_v2.py
 src/dfktools/quests/__init__.py
 src/dfktools/quests/quest_core_v1.py
 src/dfktools/quests/quest_core_v2.py
+src/dfktools/quests/quest_core_v3.py
 src/dfktools/quests/quest_v1.py
 src/dfktools/quests/quest_v2.py
+src/dfktools/quests/quest_v3.py
 src/dfktools/quests/wishing_well.py
 src/dfktools/quests/professions/__init__.py
 src/dfktools/quests/professions/fishing.py
 src/dfktools/quests/professions/foraging.py
 src/dfktools/quests/professions/gardening.py
 src/dfktools/quests/professions/mining.py
 src/dfktools/quests/training/__init__.py
```

