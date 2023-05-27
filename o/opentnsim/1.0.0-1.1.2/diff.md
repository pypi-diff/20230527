# Comparing `tmp/opentnsim-1.0.0.tar.gz` & `tmp/opentnsim-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\opentnsim-1.0.0.tar", last modified: Thu May  7 18:46:34 2020, max compression
+gzip compressed data, was "opentnsim-1.1.2.tar", last modified: Sat May 27 12:33:59 2023, max compression
```

## Comparing `opentnsim-1.0.0.tar` & `opentnsim-1.1.2.tar`

### file list

```diff
@@ -1,55 +1,98 @@
-drwxrwxrwx   0        0        0        0 2020-05-07 18:46:34.000000 opentnsim-1.0.0/
-drwxrwxrwx   0        0        0        0 2020-05-07 18:46:33.000000 opentnsim-1.0.0/.circleci/
--rw-rw-rw-   0        0        0     1308 2020-05-07 18:46:06.000000 opentnsim-1.0.0/.circleci/config.yml
--rw-rw-rw-   0        0        0       78 2019-07-18 12:16:26.000000 opentnsim-1.0.0/.coveragerc
--rw-rw-rw-   0        0        0      101 2019-01-24 11:41:01.000000 opentnsim-1.0.0/.dockerignore
--rw-rw-rw-   0        0        0      596 2019-07-18 12:16:26.000000 opentnsim-1.0.0/.gitignore
--rw-rw-rw-   0        0        0     1537 2019-07-18 12:16:26.000000 opentnsim-1.0.0/AUTHORS.rst
--rw-rw-rw-   0        0        0     4077 2019-07-18 12:16:26.000000 opentnsim-1.0.0/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0      213 2019-07-18 12:16:26.000000 opentnsim-1.0.0/Dockerfile
--rw-rw-rw-   0        0        0      219 2020-05-07 18:46:06.000000 opentnsim-1.0.0/HISTORY.rst
--rw-rw-rw-   0        0        0     1122 2019-01-31 12:05:59.000000 opentnsim-1.0.0/LICENSE.txt
--rw-rw-rw-   0        0        0     2919 2020-05-07 18:46:34.000000 opentnsim-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2018 2020-05-07 18:46:06.000000 opentnsim-1.0.0/README.md
--rw-rw-rw-   0        0        0      233 2019-07-18 12:16:26.000000 opentnsim-1.0.0/docker-compose.yml
-drwxrwxrwx   0        0        0        0 2020-05-07 18:46:33.000000 opentnsim-1.0.0/docs/
--rw-rw-rw-   0        0        0     7829 2019-01-03 10:07:50.000000 opentnsim-1.0.0/docs/Makefile
--rw-rw-rw-   0        0        0     6810 2019-07-18 12:16:26.000000 opentnsim-1.0.0/docs/OpenTNSim.png
-drwxrwxrwx   0        0        0        0 2020-05-07 18:46:33.000000 opentnsim-1.0.0/docs/_static/
--rw-rw-rw-   0        0        0       19 2019-01-03 10:07:50.000000 opentnsim-1.0.0/docs/_static/.gitignore
--rw-rw-rw-   0        0        0       43 2019-01-03 10:07:50.000000 opentnsim-1.0.0/docs/authors.rst
--rw-rw-rw-   0        0        0       45 2019-01-03 10:07:50.000000 opentnsim-1.0.0/docs/changelog.rst
--rw-rw-rw-   0        0        0     5058 2019-07-18 12:16:26.000000 opentnsim-1.0.0/docs/conf.py
--rw-rw-rw-   0        0        0       34 2019-07-18 12:16:26.000000 opentnsim-1.0.0/docs/contributing.rst
--rw-rw-rw-   0        0        0       29 2019-07-18 12:16:26.000000 opentnsim-1.0.0/docs/history.rst
--rw-rw-rw-   0        0        0      928 2020-05-07 18:46:06.000000 opentnsim-1.0.0/docs/index.rst
--rw-rw-rw-   0        0        0     1314 2019-09-05 14:19:19.000000 opentnsim-1.0.0/docs/installation.rst
--rw-rw-rw-   0        0        0       74 2019-01-03 10:07:50.000000 opentnsim-1.0.0/docs/license.rst
--rw-rw-rw-   0        0        0      842 2019-09-05 14:19:19.000000 opentnsim-1.0.0/docs/opentnsim.rst
--rw-rw-rw-   0        0        0     1180 2020-05-07 18:46:06.000000 opentnsim-1.0.0/docs/version-conventions.rst
-drwxrwxrwx   0        0        0        0 2020-05-07 18:46:33.000000 opentnsim-1.0.0/opentnsim/
--rw-rw-rw-   0        0        0      176 2020-05-07 18:46:06.000000 opentnsim-1.0.0/opentnsim/__init__.py
--rw-rw-rw-   0        0        0      775 2019-07-18 12:16:26.000000 opentnsim-1.0.0/opentnsim/cli.py
--rw-rw-rw-   0        0        0    21422 2019-07-18 12:16:26.000000 opentnsim-1.0.0/opentnsim/core.py
--rw-rw-rw-   0        0        0     4687 2019-07-18 12:16:26.000000 opentnsim-1.0.0/opentnsim/graph_module.py
--rw-rw-rw-   0        0        0     7775 2019-07-18 12:16:26.000000 opentnsim-1.0.0/opentnsim/model.py
--rw-rw-rw-   0        0        0    13761 2020-05-07 18:46:06.000000 opentnsim-1.0.0/opentnsim/plot.py
-drwxrwxrwx   0        0        0        0 2020-05-07 18:46:33.000000 opentnsim-1.0.0/opentnsim.egg-info/
--rw-rw-rw-   0        0        0     2919 2020-05-07 18:46:32.000000 opentnsim-1.0.0/opentnsim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      952 2020-05-07 18:46:32.000000 opentnsim-1.0.0/opentnsim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-05-07 18:46:32.000000 opentnsim-1.0.0/opentnsim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2020-05-07 18:46:32.000000 opentnsim-1.0.0/opentnsim.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2019-07-18 09:00:07.000000 opentnsim-1.0.0/opentnsim.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      189 2020-05-07 18:46:32.000000 opentnsim-1.0.0/opentnsim.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2020-05-07 18:46:32.000000 opentnsim-1.0.0/opentnsim.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1285 2020-05-07 18:46:34.000000 opentnsim-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     2150 2020-05-07 18:46:06.000000 opentnsim-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2020-05-07 18:46:34.000000 opentnsim-1.0.0/tests/
--rw-rw-rw-   0        0        0      261 2019-07-18 12:16:26.000000 opentnsim-1.0.0/tests/conftest.py
--rw-rw-rw-   0        0        0     1806 2019-07-18 12:16:26.000000 opentnsim-1.0.0/tests/test_make_graph.py
--rw-rw-rw-   0        0        0     2156 2019-07-18 12:16:26.000000 opentnsim-1.0.0/tests/test_make_vessel.py
--rw-rw-rw-   0        0        0     5443 2019-07-18 12:16:26.000000 opentnsim-1.0.0/tests/test_route_selection.py
--rw-rw-rw-   0        0        0     6088 2019-07-18 12:16:26.000000 opentnsim-1.0.0/tests/test_sailing_times.py
--rw-rw-rw-   0        0        0     5047 2019-07-18 12:16:26.000000 opentnsim-1.0.0/tests/test_vessel_generator.py
-drwxrwxrwx   0        0        0        0 2020-05-07 18:46:34.000000 opentnsim-1.0.0/tests/vessels/
--rw-rw-rw-   0        0        0      596 2019-07-18 07:24:27.000000 opentnsim-1.0.0/tests/vessels/vessels.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 12:33:59.273583 opentnsim-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-27 12:33:41.000000 opentnsim-1.1.2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-05-27 12:33:41.000000 opentnsim-1.1.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-27 12:33:41.000000 opentnsim-1.1.2/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-27 12:33:41.000000 opentnsim-1.1.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-27 12:33:41.000000 opentnsim-1.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-05-27 12:33:59.273583 opentnsim-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-05-27 12:33:41.000000 opentnsim-1.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 12:33:59.261583 opentnsim-1.1.2/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-05-27 12:33:41.000000 opentnsim-1.1.2/data/Correctionfactors.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-05-27 12:33:41.000000 opentnsim-1.1.2/data/KarpovSmoothCurves.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   212529 2023-05-27 12:33:41.000000 opentnsim-1.1.2/data/ais.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 12:33:59.261583 opentnsim-1.1.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7598 2023-05-27 12:33:41.000000 opentnsim-1.1.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     6810 2023-05-27 12:33:41.000000 opentnsim-1.1.2/docs/OpenTNSim.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 12:33:59.261583 opentnsim-1.1.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)   785084 2023-05-27 12:33:41.000000 opentnsim-1.1.2/docs/_static/book.png
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-27 12:33:41.000000 opentnsim-1.1.2/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-27 12:33:41.000000 opentnsim-1.1.2/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4894 2023-05-27 12:33:41.000000 opentnsim-1.1.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-27 12:33:41.000000 opentnsim-1.1.2/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-27 12:33:41.000000 opentnsim-1.1.2/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-27 12:33:41.000000 opentnsim-1.1.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-05-27 12:33:41.000000 opentnsim-1.1.2/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-27 12:33:41.000000 opentnsim-1.1.2/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-27 12:33:41.000000 opentnsim-1.1.2/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-27 12:33:41.000000 opentnsim-1.1.2/docs/opentnsim.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-27 12:33:41.000000 opentnsim-1.1.2/docs/version-conventions.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 12:33:59.265583 opentnsim-1.1.2/opentnsim/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-27 12:33:42.000000 opentnsim-1.1.2/opentnsim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-27 12:33:42.000000 opentnsim-1.1.2/opentnsim/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20866 2023-05-27 12:33:42.000000 opentnsim-1.1.2/opentnsim/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80195 2023-05-27 12:33:42.000000 opentnsim-1.1.2/opentnsim/energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9524 2023-05-27 12:33:42.000000 opentnsim-1.1.2/opentnsim/graph_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69590 2023-05-27 12:33:42.000000 opentnsim-1.1.2/opentnsim/lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6434 2023-05-27 12:33:42.000000 opentnsim-1.1.2/opentnsim/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13353 2023-05-27 12:33:42.000000 opentnsim-1.1.2/opentnsim/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14357 2023-05-27 12:33:42.000000 opentnsim-1.1.2/opentnsim/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14991 2023-05-27 12:33:42.000000 opentnsim-1.1.2/opentnsim/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 12:33:59.265583 opentnsim-1.1.2/opentnsim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-05-27 12:33:59.000000 opentnsim-1.1.2/opentnsim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-05-27 12:33:59.000000 opentnsim-1.1.2/opentnsim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 12:33:59.000000 opentnsim-1.1.2/opentnsim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-27 12:33:59.000000 opentnsim-1.1.2/opentnsim.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 12:33:59.000000 opentnsim-1.1.2/opentnsim.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-27 12:33:59.000000 opentnsim-1.1.2/opentnsim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-27 12:33:59.000000 opentnsim-1.1.2/opentnsim.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-27 12:33:42.000000 opentnsim-1.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-27 12:33:59.273583 opentnsim-1.1.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2642 2023-05-27 12:33:42.000000 opentnsim-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 12:33:59.269583 opentnsim-1.1.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 12:33:59.269583 opentnsim-1.1.2/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)  2888448 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/data/ect-bctn.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7603 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/test_ManJiang_et_al_2022_current_influence_limiting_depth_single_and_round_trips.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/test_ManJiang_et_al_2022_current_influence_limiting_depth_single_and_round_trips_expected.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/test_ManJiang_et_al_2022_emission_rates_v_depth_engine_age.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/test_ManJiang_et_al_2022_emission_rates_v_depth_engine_age_expected.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     7661 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/test_ManJiang_et_al_2022_fuel_use_and_emissions_along_limiting_depth_route.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/test_ManJiang_et_al_2022_fuel_use_and_emissions_along_limiting_depth_route_expected.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     7498 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/test_ManJiang_et_al_2022_fuel_use_and_emissions_along_uniform_depth_route.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/test_ManJiang_et_al_2022_fuel_use_and_emissions_along_uniform_depth_route_expected.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     7862 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/test_ManJiang_et_al_2022_fuel_use_and_emissions_along_varying_depth_route.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/test_ManJiang_et_al_2022_fuel_use_and_emissions_along_varying_depth_route_expected.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     7740 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/test_ManJiang_et_al_2022_fuel_use_and_emissions_given_engine_age_round_trip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/test_ManJiang_et_al_2022_fuel_use_and_emissions_given_engine_age_round_trip_expected.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     6751 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/test_ManJiang_et_al_2022_power2v_limiting_depth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/test_ManJiang_et_al_2022_power2v_limiting_depth_expected.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     6801 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/test_ManJiang_et_al_2022_power2v_uniform_depth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/test_ManJiang_et_al_2022_power2v_uniform_depth_expected.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/test_ManJiang_et_al_2022_power2v_varying_depth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/test_ManJiang_et_al_2022_power2v_varying_depth_expected.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4785 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/test_ManJiang_et_al_2022_resistance_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/test_ManJiang_et_al_2022_resistance_components_expected.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/test_ManJiang_et_al_2022_squat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/test_ManJiang_et_al_2022_squat_expected.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/test_ManJiang_et_al_2022_total_power.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/test_ManJiang_et_al_2022_total_power_expected.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     7166 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/test_ManJiang_et_al_2022_v113_diesel_use_along_validation_route_with_C_year_without_C_year.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/test_ManJiang_et_al_2022_v113_diesel_use_along_validation_route_with_C_year_without_C_year_expected.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     7224 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/test_ManJiang_et_al_2022_v113_emissions_along_validation_route.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/test_ManJiang_et_al_2022_v113_emissions_along_validation_route_expected.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    10117 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/test_ManJiang_et_al_2022_v113_renewable_energy_sources_use_along_validation_route.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4806 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/test_ManJiang_et_al_2022_v113_renewable_energy_sources_use_along_validation_route_expected.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/test_Van_Dorsser_et_al_2020_draught_payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/test_Van_Dorsser_et_al_2020_draught_payload_expected.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/test_basic_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8211 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/test_single_vessel_with_pre-conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6652 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/test_single_vessel_without_pre-conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10023 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/test_two_vessels_bidirectional_simultaneous_arrival_with_pre-conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9263 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/test_two_vessels_bidirectional_simultaneous_arrival_without_pre-conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10320 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/test_two_vessels_unidirectional_simultaneous_arrival_separate_locking_with_pre-conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9022 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/test_two_vessels_unidirectional_simultaneous_arrival_separate_locking_without_pre-conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9678 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/test_two_vessels_unidirectional_simultaneous_arrival_simultaneous_locking_with_pre-conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8814 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/test_two_vessels_unidirectional_simultaneous_arrival_simultaneous_locking_without_pre-conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 12:33:59.273583 opentnsim-1.1.2/tests/vessels/
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/vessels/vessels.csv
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `opentnsim-1.0.0/AUTHORS.rst` & `opentnsim-1.1.2/AUTHORS.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,26 @@
-=======
-Credits
-=======
-
-Development Lead
-----------------
-* `Mark van Koningsveld`_
-* `Joris den Uijl`_
-
-.. _Mark van Koningsveld: https://www.tudelft.nl/citg/over-faculteit/afdelingen/hydraulic-engineering/sections/rivers-ports-waterways-and-dredging-engineering/staff/van-koningsveld-m/
-.. _Joris den Uijl: https://github.com/uijl
-
-Contributors
-------------
-
-Various MSc projects
-
-* `Jeroen van der Does de Willebois`_, 2019. **Assessing the impact of quay-wall renovations on the nautical traffic in Amsterdam: A simulation study.** MSc thesis. Delft University of Technology, Civil Engineering and Geosciences, Hydraulic Engineering - Ports and Waterways. Delft, the Netherlands.
-* `Leonore Vehmeijer`_, 2019. **Measures for the reduction of CO2 emissions, by the inland shipping fleet, on the Rotterdam-Antwerp corridor.** MSc thesis. Delft University of Technology, Civil Engineering and Geosciences, Hydraulic Engineering - Ports and Waterways. Delft, the Netherlands.
-* `Sophie Ensing`_, 2019. **Agent-based modeling and simulation of public transport to identify effects of network changes on passenger flows.** MSc thesis. University of Amsterdam, Faculty of Science, Data Science, Information Studies. Amsterdam, the Netherlands.
-
-
-.. _Jeroen van der Does de Willebois: http://resolver.tudelft.nl/uuid:22eddd89-21a2-4819-ba1f-ee905a829364
-.. _Leonore Vehmeijer: http://resolver.tudelft.nl/uuid:1abd88e0-9ab6-47fd-a503-2f19ba13bbff
-.. _Sophie Ensing: http://scriptiesonline.uba.uva.nl/scriptie/690471
+=======
+Credits
+=======
+
+Development Lead
+----------------
+* `Mark van Koningsveld`_
+* `Fedor Baart`_
+
+.. _Mark van Koningsveld: https://www.tudelft.nl/citg/over-faculteit/afdelingen/hydraulic-engineering/sections/rivers-ports-waterways-and-dredging-engineering/staff/van-koningsveld-m/
+.. _Fedor Baart: https://www.deltares.nl/en/experts/fedor-baart-3/
+
+Contributors
+------------
+
+Various MSc projects
+
+* `Jeroen van der Does de Willebois`_, 2019. **Assessing the impact of quay-wall renovations on the nautical traffic in Amsterdam: A simulation study.** MSc thesis. Delft University of Technology, Civil Engineering and Geosciences, Hydraulic Engineering - Ports and Waterways. Delft, the Netherlands.
+* `Leonore Vehmeijer`_, 2019. **Measures for the reduction of CO2 emissions, by the inland shipping fleet, on the Rotterdam-Antwerp corridor.** MSc thesis. Delft University of Technology, Civil Engineering and Geosciences, Hydraulic Engineering - Ports and Waterways. Delft, the Netherlands.
+* `Sophie Ensing`_, 2019. **Agent-based modeling and simulation of public transport to identify effects of network changes on passenger flows.** MSc thesis. University of Amsterdam, Faculty of Science, Data Science, Information Studies. Amsterdam, the Netherlands.
+* `Loes Segers`_, 2021. **Mapping inland shipping emissions in time and space for the benefit of emission policy development: A case study on the Rotterdam-Antwerp corridor.** MSc thesis. Delft University of Technology, Civil Engineering and Geosciences, Hydraulic Engineering - Ports and Waterways. Delft, the Netherlands.
+
+.. _Jeroen van der Does de Willebois: http://resolver.tudelft.nl/uuid:22eddd89-21a2-4819-ba1f-ee905a829364
+.. _Leonore Vehmeijer: http://resolver.tudelft.nl/uuid:1abd88e0-9ab6-47fd-a503-2f19ba13bbff
+.. _Sophie Ensing: http://scriptiesonline.uba.uva.nl/scriptie/690471
+.. _Loes Segers: http://resolver.tudelft.nl/uuid:a260bc48-c6ce-4f7c-b14a-e681d2e528e3
```

### Comparing `opentnsim-1.0.0/CONTRIBUTING.rst` & `opentnsim-1.1.2/CONTRIBUTING.rst`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,157 +1,157 @@
-.. highlight:: shell
-
-============
-Contributing
-============
-
-Contributions are welcome, and they are greatly appreciated! Every little bit
-helps, and credit will always be given.
-
-You can contribute in many ways:
-
-Types of Contributions
-----------------------
-
-Report Bugs
-~~~~~~~~~~~
-
-Report bugs at https://github.com/TUDelft-CITG/OpenTNSim/issues.
-
-If you are reporting a bug, please include:
-
-* Your operating system name and version.
-* Any details about your local setup that might be helpful in troubleshooting.
-* Detailed steps to reproduce the bug.
-
-Fix Bugs
-~~~~~~~~
-
-Look through the GitHub issues for bugs. Anything tagged with "bug" and "help
-wanted" is open to whoever wants to implement it.
-
-Implement Features
-~~~~~~~~~~~~~~~~~~
-
-Look through the GitHub issues for features. Anything tagged with "enhancement"
-and "help wanted" is open to whoever wants to implement it.
-
-Write Documentation
-~~~~~~~~~~~~~~~~~~~
-
-OpenTNSim could always use more documentation, whether as part of the
-official OpenTNSim docs, in docstrings, or even on the web in blog posts,
-articles, and such.
-
-Submit Feedback
-~~~~~~~~~~~~~~~
-
-The best way to send feedback is to file an issue at https://github.com/TUDelft-CITG/OpenTNSim/issues.
-
-If you are proposing a feature:
-
-* Explain in detail how it would work.
-* Keep the scope as narrow as possible, to make it easier to implement.
-* Remember that this is a volunteer-driven project, and that contributions
-  are welcome :)
-
-Get Started!
-------------
-
-Ready to contribute? Here's how to set up `OpenTNSim` for local development.
-
-1. Fork the `OpenTNSim` repository on GitHub.
-
-
-2. Clone your fork locally::
-
-    $ git clone git@github.com:your_name_here/OpenTNSim.git
-
-
-3. Install your local copy into a virtualenv. Assuming you have virtualenvwrapper installed, this is how you set up your fork for local development::
-
-    $ mkvirtualenv opentnsim
-    $ cd opentnsim/
-    $ python setup.py develop
-
-
-4. Create a branch for local development::
-
-    $ git checkout -b name-of-your-bugfix-or-feature
-
-
-   Now you can make your changes locally.
-
-
-5. When you're done making changes, check that your changes pass flake8 and the
-   tests, including testing other Python versions with tox::
-
-    $ flake8 opentnsim tests
-    $ python setup.py test or py.test
-    $ tox
-
-
-   To get flake8 and tox, just pip install them into your virtualenv.
-
-
-6. The style of OpenTNSim is according to Black. Format your code using 
-   Black witht the following lines of code::
-
-    $ black opentnsim
-    $ black tests
-
-
-   You can install black using pip.
-
-
-7. Commit your changes and push your branch to GitHub::
-
-    $ git add .
-    $ git commit -m "Your detailed description of your changes."
-    $ git push origin name-of-your-bugfix-or-feature
-
-
-8. Submit a pull request through the GitHub website.
-
-Pull Request Guidelines
------------------------
-
-Before you submit a pull request, check that it meets these guidelines:
-
-1. The pull request should include tests.
-2. If the pull request adds functionality, the docs should be updated. Put
-   your new functionality into a function with a docstring, and add the
-   feature to the list in README.rst.
-3. The pull request should work for Python 3.4, 3.5 and 3.6, and for PyPy. Check
-   CircleCI and make sure that the tests pass for all supported Python versions.
-
-Tips
-----
-
-To run a subset of tests::
-
-$ py.test tests.test_opentnsim
-
-To make the documentation pages
-$ make docs # for linux/osx
-
-For windows
-$ del docs\opentnsim.rst
-$ del docs\modules.rst
-$ sphinx-apidoc -o docs/ opentnsim
-$ cd docs
-$ make html
-$ start explorer _build\html\index.html
-
-
-Deploying
----------
-
-A reminder for the maintainers on how to deploy.
-Make sure all your changes are committed (including an entry in HISTORY.rst).
-Then run::
-
-$ bumpversion patch # possible: major / minor / patch
-$ git push
-$ git push --tags
-
-Travis will then deploy to PyPI if tests pass.
+.. highlight:: shell
+
+============
+Contributing
+============
+
+Contributions are welcome, and they are greatly appreciated! Every little bit
+helps, and credit will always be given.
+
+You can contribute in many ways:
+
+Types of Contributions
+----------------------
+
+Report Bugs
+~~~~~~~~~~~
+
+Report bugs at https://github.com/TUDelft-CITG/OpenTNSim/issues.
+
+If you are reporting a bug, please include:
+
+* Your operating system name and version.
+* Any details about your local setup that might be helpful in troubleshooting.
+* Detailed steps to reproduce the bug.
+
+Fix Bugs
+~~~~~~~~
+
+Look through the GitHub issues for bugs. Anything tagged with "bug" and "help
+wanted" is open to whoever wants to implement it.
+
+Implement Features
+~~~~~~~~~~~~~~~~~~
+
+Look through the GitHub issues for features. Anything tagged with "enhancement"
+and "help wanted" is open to whoever wants to implement it.
+
+Write Documentation
+~~~~~~~~~~~~~~~~~~~
+
+OpenTNSim could always use more documentation, whether as part of the
+official OpenTNSim docs, in docstrings, or even on the web in blog posts,
+articles, and such.
+
+Submit Feedback
+~~~~~~~~~~~~~~~
+
+The best way to send feedback is to file an issue at https://github.com/TUDelft-CITG/OpenTNSim/issues.
+
+If you are proposing a feature:
+
+* Explain in detail how it would work.
+* Keep the scope as narrow as possible, to make it easier to implement.
+* Remember that this is a volunteer-driven project, and that contributions
+  are welcome :)
+
+Get Started!
+------------
+
+Ready to contribute? Here's how to set up `OpenTNSim` for local development.
+
+1. Fork the `OpenTNSim` repository on GitHub.
+
+
+2. Clone your fork locally::
+
+    $ git clone git@github.com:your_name_here/OpenTNSim.git
+
+
+3. Install your local copy into a virtualenv. Assuming you have virtualenvwrapper installed, this is how you set up your fork for local development::
+
+    $ mkvirtualenv opentnsim
+    $ cd opentnsim/
+    $ python setup.py develop
+
+
+4. Create a branch for local development::
+
+    $ git checkout -b name-of-your-bugfix-or-feature
+
+
+   Now you can make your changes locally.
+
+
+5. When you're done making changes, check that your changes pass flake8 and the
+   tests, including testing other Python versions with tox::
+
+    $ flake8 opentnsim tests
+    $ python setup.py test or py.test
+    $ tox
+
+
+   To get flake8 and tox, just pip install them into your virtualenv.
+
+
+6. The style of OpenTNSim is according to Black. Format your code using 
+   Black witht the following lines of code::
+
+    $ black opentnsim
+    $ black tests
+
+
+   You can install black using pip.
+
+
+7. Commit your changes and push your branch to GitHub::
+
+    $ git add .
+    $ git commit -m "Your detailed description of your changes."
+    $ git push origin name-of-your-bugfix-or-feature
+
+
+8. Submit a pull request through the GitHub website.
+
+Pull Request Guidelines
+-----------------------
+
+Before you submit a pull request, check that it meets these guidelines:
+
+1. The pull request should include tests.
+2. If the pull request adds functionality, the docs should be updated. Put
+   your new functionality into a function with a docstring, and add the
+   feature to the list in README.rst.
+3. The pull request should work for Python 3.4, 3.5 and 3.6, and for PyPy. Check
+   CircleCI and make sure that the tests pass for all supported Python versions.
+
+Tips
+----
+
+To run a subset of tests::
+
+$ py.test tests.test_opentnsim
+
+To make the documentation pages
+$ make docs # for linux/osx
+
+For windows
+$ del docs\opentnsim.rst
+$ del docs\modules.rst
+$ sphinx-apidoc -o docs/ opentnsim
+$ cd docs
+$ make html
+$ start explorer _build\html\index.html
+
+
+Deploying
+---------
+
+A reminder for the maintainers on how to deploy.
+Make sure all your changes are committed (including an entry in HISTORY.rst).
+Then run::
+
+$ bumpversion patch # possible: major / minor / patch
+$ git push
+$ git push --tags
+
+Travis will then deploy to PyPI if tests pass.
```

### Comparing `opentnsim-1.0.0/LICENSE.txt` & `opentnsim-1.1.2/LICENSE.txt`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-The MIT License (MIT)
-
-Copyright (c) 2018 TUDelft / CITG-Ports and Waterways
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+The MIT License (MIT)
+
+Copyright (c) 2018 TUDelft / CITG-Ports and Waterways
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `opentnsim-1.0.0/docs/OpenTNSim.png` & `opentnsim-1.1.2/docs/OpenTNSim.png`

 * *Files identical despite different names*

### Comparing `opentnsim-1.0.0/docs/conf.py` & `opentnsim-1.1.2/docs/conf.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,164 +1,164 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-#
-# opentnsim documentation build configuration file, created by
-# sphinx-quickstart on Fri Jun  9 13:47:02 2017.
-#
-# This file is execfile()d with the current directory set to its
-# containing dir.
-#
-# Note that not all possible configuration values are present in this
-# autogenerated file.
-#
-# All configuration values have a default; values that are commented out
-# serve to show the default.
-
-# If extensions (or modules to document with autodoc) are in another
-# directory, add these directories to sys.path here. If the directory is
-# relative to the documentation root, use os.path.abspath to make it
-# absolute, like shown here.
-#
-import os
-import sys
-sys.path.insert(0, os.path.abspath('..'))
-
-import opentnsim
-
-# -- General configuration ---------------------------------------------
-
-# If your documentation needs a minimal Sphinx version, state it here.
-#
-# needs_sphinx = '1.0'
-
-# Add any Sphinx extension module names here, as strings. They can be
-# extensions coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
-extensions = ['sphinx.ext.autodoc', 'sphinx.ext.viewcode']
-
-# Add any paths that contain templates here, relative to this directory.
-templates_path = ['_templates']
-
-# The suffix(es) of source filenames.
-# You can specify multiple suffix as a list of string:
-#
-# source_suffix = ['.rst', '.md']
-source_suffix = '.rst'
-
-# The master toctree document.
-master_doc = 'index'
-
-# General information about the project.
-project = u'OpenTNSim'
-copyright = u"2019, TU Delft"
-author = u"Mark van Koningsveld"
-
-# The version info for the project you're documenting, acts as replacement
-# for |version| and |release|, also used in various other places throughout
-# the built documents.
-#
-# The short X.Y version.
-version = opentnsim.__version__
-# The full version, including alpha/beta/rc tags.
-release = opentnsim.__version__
-
-# The language for content autogenerated by Sphinx. Refer to documentation
-# for a list of supported languages.
-#
-# This is also used if you do content translation via gettext catalogs.
-# Usually you set "language" from the command line for these cases.
-language = None
-
-# List of patterns, relative to source directory, that match files and
-# directories to ignore when looking for source files.
-# This patterns also effect to html_static_path and html_extra_path
-exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
-
-# The name of the Pygments (syntax highlighting) style to use.
-pygments_style = 'sphinx'
-
-# If true, `todo` and `todoList` produce output, else they produce nothing.
-todo_include_todos = False
-
-
-# -- Options for HTML output -------------------------------------------
-
-# Add a logo
-html_logo = "OpenTNSim.png"
-
-# The theme to use for HTML and HTML Help pages.  See the documentation for
-# a list of builtin themes.
-#
-html_theme = "sphinx_rtd_theme"
-
-
-# Theme options are theme-specific and customize the look and feel of a
-# theme further.  For a list of options available for each theme, see the
-# documentation.
-#
-# html_theme_options = {}
-
-# Add any paths that contain custom static files (such as style sheets) here,
-# relative to this directory. They are copied after the builtin static files,
-# so a file named "default.css" will overwrite the builtin "default.css".
-html_static_path = ['_static']
-
-
-# -- Options for HTMLHelp output ---------------------------------------
-
-# Output file base name for HTML help builder.
-htmlhelp_basename = 'opentnsimdoc'
-
-
-# -- Options for LaTeX output ------------------------------------------
-
-latex_elements = {
-    # The paper size ('letterpaper' or 'a4paper').
-    #
-    # 'papersize': 'letterpaper',
-
-    # The font size ('10pt', '11pt' or '12pt').
-    #
-    # 'pointsize': '10pt',
-
-    # Additional stuff for the LaTeX preamble.
-    #
-    # 'preamble': '',
-
-    # Latex figure (float) alignment
-    #
-    # 'figure_align': 'htbp',
-}
-
-# Grouping the document tree into LaTeX files. List of tuples
-# (source start file, target name, title, author, documentclass
-# [howto, manual, or own class]).
-latex_documents = [
-    (master_doc, 'opentnsim.tex',
-     u'OpenTNSim Documentation',
-     u'Mark van Koningsveld', 'manual'),
-]
-
-
-# -- Options for manual page output ------------------------------------
-
-# One entry per manual page. List of tuples
-# (source start file, name, description, authors, manual section).
-man_pages = [
-    (master_doc, 'opentnsim',
-     u'OpenTNSim Documentation',
-     [author], 1)
-]
-
-
-# -- Options for Texinfo output ----------------------------------------
-
-# Grouping the document tree into Texinfo files. List of tuples
-# (source start file, target name, title, author,
-#  dir menu entry, description, category)
-texinfo_documents = [
-    (master_doc, 'opentnsim',
-     u'OpenTNSim Documentation',
-     author,
-     'opentnsim',
-     'One line description of project.',
-     'Miscellaneous'),
-]
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+#
+# opentnsim documentation build configuration file, created by
+# sphinx-quickstart on Fri Jun  9 13:47:02 2017.
+#
+# This file is execfile()d with the current directory set to its
+# containing dir.
+#
+# Note that not all possible configuration values are present in this
+# autogenerated file.
+#
+# All configuration values have a default; values that are commented out
+# serve to show the default.
+
+# If extensions (or modules to document with autodoc) are in another
+# directory, add these directories to sys.path here. If the directory is
+# relative to the documentation root, use os.path.abspath to make it
+# absolute, like shown here.
+#
+import os
+import sys
+sys.path.insert(0, os.path.abspath('..'))
+
+import opentnsim
+
+# -- General configuration ---------------------------------------------
+
+# If your documentation needs a minimal Sphinx version, state it here.
+#
+# needs_sphinx = '1.0'
+
+# Add any Sphinx extension module names here, as strings. They can be
+# extensions coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
+extensions = ['sphinx.ext.autodoc', 'sphinx.ext.viewcode']
+
+# Add any paths that contain templates here, relative to this directory.
+templates_path = ['_templates']
+
+# The suffix(es) of source filenames.
+# You can specify multiple suffix as a list of string:
+#
+# source_suffix = ['.rst', '.md']
+source_suffix = '.rst'
+
+# The master toctree document.
+master_doc = 'index'
+
+# General information about the project.
+project = u'OpenTNSim'
+copyright = u"2019, TU Delft"
+author = u"Mark van Koningsveld"
+
+# The version info for the project you're documenting, acts as replacement
+# for |version| and |release|, also used in various other places throughout
+# the built documents.
+#
+# The short X.Y version.
+version = opentnsim.__version__
+# The full version, including alpha/beta/rc tags.
+release = opentnsim.__version__
+
+# The language for content autogenerated by Sphinx. Refer to documentation
+# for a list of supported languages.
+#
+# This is also used if you do content translation via gettext catalogs.
+# Usually you set "language" from the command line for these cases.
+language = None
+
+# List of patterns, relative to source directory, that match files and
+# directories to ignore when looking for source files.
+# This patterns also effect to html_static_path and html_extra_path
+exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
+
+# The name of the Pygments (syntax highlighting) style to use.
+pygments_style = 'sphinx'
+
+# If true, `todo` and `todoList` produce output, else they produce nothing.
+todo_include_todos = False
+
+
+# -- Options for HTML output -------------------------------------------
+
+# Add a logo
+html_logo = "OpenTNSim.png"
+
+# The theme to use for HTML and HTML Help pages.  See the documentation for
+# a list of builtin themes.
+#
+html_theme = "sphinx_rtd_theme"
+
+
+# Theme options are theme-specific and customize the look and feel of a
+# theme further.  For a list of options available for each theme, see the
+# documentation.
+#
+# html_theme_options = {}
+
+# Add any paths that contain custom static files (such as style sheets) here,
+# relative to this directory. They are copied after the builtin static files,
+# so a file named "default.css" will overwrite the builtin "default.css".
+html_static_path = ['_static']
+
+
+# -- Options for HTMLHelp output ---------------------------------------
+
+# Output file base name for HTML help builder.
+htmlhelp_basename = 'opentnsimdoc'
+
+
+# -- Options for LaTeX output ------------------------------------------
+
+latex_elements = {
+    # The paper size ('letterpaper' or 'a4paper').
+    #
+    # 'papersize': 'letterpaper',
+
+    # The font size ('10pt', '11pt' or '12pt').
+    #
+    # 'pointsize': '10pt',
+
+    # Additional stuff for the LaTeX preamble.
+    #
+    # 'preamble': '',
+
+    # Latex figure (float) alignment
+    #
+    # 'figure_align': 'htbp',
+}
+
+# Grouping the document tree into LaTeX files. List of tuples
+# (source start file, target name, title, author, documentclass
+# [howto, manual, or own class]).
+latex_documents = [
+    (master_doc, 'opentnsim.tex',
+     u'OpenTNSim Documentation',
+     u'Mark van Koningsveld', 'manual'),
+]
+
+
+# -- Options for manual page output ------------------------------------
+
+# One entry per manual page. List of tuples
+# (source start file, name, description, authors, manual section).
+man_pages = [
+    (master_doc, 'opentnsim',
+     u'OpenTNSim Documentation',
+     [author], 1)
+]
+
+
+# -- Options for Texinfo output ----------------------------------------
+
+# Grouping the document tree into Texinfo files. List of tuples
+# (source start file, target name, title, author,
+#  dir menu entry, description, category)
+texinfo_documents = [
+    (master_doc, 'opentnsim',
+     u'OpenTNSim Documentation',
+     author,
+     'opentnsim',
+     'One line description of project.',
+     'Miscellaneous'),
+]
```

### Comparing `opentnsim-1.0.0/docs/index.rst` & `opentnsim-1.1.2/docs/index.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,31 @@
-Open source Transport Network Simulation
-========================================
-
-OpenTNSim is a python package for the investigation of traffic behaviour on networks to compare the consequences of different traffic scenarios and network configurations.
-
-Welcome to OpenTNSim documentation! Please check the contents below for information on installation, getting started and actual example code. If you want to dive straight into the code you can check out our `GitHub`_ page or the working examples presented in `Jupyter Notebooks`_.
-
-.. toctree::
-   :maxdepth: 1
-   :caption: Contents:
-
-   installation
-   opentnsim
-   contributing
-   authors
-   history
-   version-conventions
-
-Indices and tables
-==================
-
-* :ref:`genindex`
-* :ref:`modindex`
-* :ref:`search`
-
-.. _GitHub: https://github.com/TUDelft-CITG/OpenTNSim
-.. _Jupyter Notebooks: https://github.com/TUDelft-CITG/OpenTNSim-Notebooks
+Open source Transport Network Simulation
+========================================
+
+OpenTNSim is a python package for the investigation of traffic behaviour on networks to compare the consequences of different traffic scenarios and network configurations.
+
+Welcome to OpenTNSim documentation! Please check the contents below for information on installation, getting started and actual example code. If you want to dive straight into the code you can check out our `GitHub`_ page or the working examples presented in `Jupyter Notebooks`_. The examples in the notebooks directory are also available as an online book.
+
+.. image:: _static/book.png
+   :target: https://happy-bush-0c5d10603.1.azurestaticapps.net
+   :width: 600
+
+.. toctree::
+   :maxdepth: 1
+   :caption: Contents:
+
+   installation
+   opentnsim
+   contributing
+   authors
+   history
+   version-conventions
+
+Indices and tables
+==================
+
+* :ref:`genindex`
+* :ref:`modindex`
+* :ref:`search`
+
+.. _GitHub: https://github.com/TUDelft-CITG/OpenTNSim
+.. _Jupyter Notebooks: https://github.com/TUDelft-CITG/OpenTNSim/notebooks
```

### Comparing `opentnsim-1.0.0/docs/installation.rst` & `opentnsim-1.1.2/docs/installation.rst`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,57 +1,57 @@
-.. highlight:: shell
-
-============
-Installation
-============
-
-
-Stable release
---------------
-
-To install OpenTNSim, run this command in your terminal:
-
-.. code-block:: bash
-
-    # Use pip to install OpenTNSim
-    pip install opentnsim
-
-This is the preferred method to install OpenTNSim, as it will always install the most recent stable release.
-
-If you do not `pip`_ installed, this `Python installation guide`_ can guide
-you through the process.
-
-.. _pip: https://pip.pypa.io
-.. _Python installation guide: http://docs.python-guide.org/en/latest/starting/installation/
-
-
-From sources
-------------
-
-The sources for OpenTNSim can be downloaded from the `Github repo`_.
-
-You can either clone the public repository:
-
-.. code-block:: bash
-
-    # Use git to clone OpenTNSim
-    git clone git://github.com/TUDelft-CITG/OpenTNSim
-
-
-Or download the `tarball`_:
-
-.. code-block:: bash
-
-    # Use curl to obtain the tarball
-    curl  -OL https://github.com/TUDelft-CITG/OpenTNSim/tarball/master
-
-
-Once you have a copy of the source, you can install it with:
-
-.. code-block:: bash
-
-    # Use python to install
-    python setup.py install
-
-
-.. _Github repo: https://github.com/TUDelft-CITG/OpenCLSim
-.. _tarball: https://github.com/TUDelft-CITG/OpenCLSim/tarball/master
+.. highlight:: shell
+
+============
+Installation
+============
+
+
+Stable release
+--------------
+
+To install OpenTNSim, run this command in your terminal:
+
+.. code-block:: bash
+
+    # Use pip to install OpenTNSim
+    pip install opentnsim
+
+This is the preferred method to install OpenTNSim, as it will always install the most recent stable release.
+
+If you do not `pip`_ installed, this `Python installation guide`_ can guide
+you through the process.
+
+.. _pip: https://pip.pypa.io
+.. _Python installation guide: http://docs.python-guide.org/en/latest/starting/installation/
+
+
+From sources
+------------
+
+The sources for OpenTNSim can be downloaded from the `Github repo`_.
+
+You can either clone the public repository:
+
+.. code-block:: bash
+
+    # Use git to clone OpenTNSim
+    git clone git://github.com/TUDelft-CITG/OpenTNSim
+
+
+Or download the `tarball`_:
+
+.. code-block:: bash
+
+    # Use curl to obtain the tarball
+    curl  -OL https://github.com/TUDelft-CITG/OpenTNSim/tarball/master
+
+
+Once you have a copy of the source, you can install it with:
+
+.. code-block:: bash
+
+    # Use python to install
+    python setup.py install
+
+
+.. _Github repo: https://github.com/TUDelft-CITG/OpenCLSim
+.. _tarball: https://github.com/TUDelft-CITG/OpenCLSim/tarball/master
```

### Comparing `opentnsim-1.0.0/docs/opentnsim.rst` & `opentnsim-1.1.2/docs/opentnsim.rst`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-=========
-OpenTNSim
-=========
-
-This page lists all functions and classes available in the OpenTNSim.model and OpenTNSim.core modules. For examples on how to use these submodules please check out the Examples page, information on installing OpenCLSim can be found on the Installation page.
-
-Submodules
-----------
-
-The main components are the Model module and the Core module. All of their components are listed below. 
-
-opentnsim\.model module
---------------------------
-
-.. automodule:: opentnsim.model
-   :members:
-   :undoc-members:
-   :show-inheritance:
-
-opentnsim\.core module
---------------------------
-
-.. automodule:: opentnsim.core
-   :members:
-   :undoc-members:
-   :show-inheritance:
-
-Module contents
----------------
-
-.. automodule:: opentnsim
-   :members:
-   :undoc-members:
-   :show-inheritance:
+=========
+OpenTNSim
+=========
+
+This page lists all functions and classes available in the OpenTNSim.model and OpenTNSim.core modules. For examples on how to use these submodules please check out the Examples page, information on installing OpenCLSim can be found on the Installation page.
+
+Submodules
+----------
+
+The main components are the Model module and the Core module. All of their components are listed below. 
+
+opentnsim\.model module
+--------------------------
+
+.. automodule:: opentnsim.model
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
+opentnsim\.core module
+--------------------------
+
+.. automodule:: opentnsim.core
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
+Module contents
+---------------
+
+.. automodule:: opentnsim
+   :members:
+   :undoc-members:
+   :show-inheritance:
```

### Comparing `opentnsim-1.0.0/docs/version-conventions.rst` & `opentnsim-1.1.2/docs/version-conventions.rst`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-===================
-Version conventions
-===================
-
-This package is being developed continuously. Branch protection is turned on for the master branch. Useful new features and bugfixes can be developed in a separate branch or fork. Pull requests can be made to integrate updates into the master branch. To keep track of versions, every change to the master branch will receive a version tag. This page outlines the version tags' naming convention.
-
-Each change to the master branch is stamped with a unique version identifier. We use sequence based version identifiers, that consist of a sequence of three numbers: the first number is a major change identifier, followed by a minor change idenfier and finally a maintenance identifier. This leads to version identifiers of the form:
-
-major.minor.maintenance (example: 1.2.2)
-
-The following guideline gives an idea what types of changes are considered major changes, minor changes and maintenance:
-
-- Major changes (typically breaking changes)  -> major + 1
-- Minor changes (typically adding of new features) -> minor + 1
-- Maintenance (typically bug fixes and updates in documentation -> maintenance + 1
-
+===================
+Version conventions
+===================
+
+This package is being developed continuously. Branch protection is turned on for the master branch. Useful new features and bugfixes can be developed in a separate branch or fork. Pull requests can be made to integrate updates into the master branch. To keep track of versions, every change to the master branch will receive a version tag. This page outlines the version tags' naming convention.
+
+Each change to the master branch is stamped with a unique version identifier. We use sequence based version identifiers, that consist of a sequence of three numbers: the first number is a major change identifier, followed by a minor change idenfier and finally a maintenance identifier. This leads to version identifiers of the form:
+
+major.minor.maintenance (example: 1.2.2)
+
+The following guideline gives an idea what types of changes are considered major changes, minor changes and maintenance:
+
+- Major changes (typically breaking changes)  -> major + 1
+- Minor changes (typically adding of new features) -> minor + 1
+- Maintenance (typically bug fixes and updates in documentation -> maintenance + 1
+
```

### Comparing `opentnsim-1.0.0/opentnsim/cli.py` & `opentnsim-1.1.2/opentnsim/cli.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-# -*- coding: utf-8 -*-
-
-"""Console script for opentnsim."""
-import sys
-import click
-
-import opentnsim.server
-
-
-@click.group()
-def cli(args=None):
-    """OpenTNSim simulation."""
-    click.echo("Replace this message by putting your code into " "opentnsim.cli.main")
-    click.echo("See click documentation at http://click.pocoo.org/")
-    return 0
-
-
-@cli.command()
-@click.option("--host", default="0.0.0.0")
-@click.option("--port", default=5000, type=int)
-@click.option("--debug/--no-debug", default=False)
-def serve(host, port, debug, args=None):
-    """Run a flask server with the backend code"""
-    app = opentnsim.server.app
-    app.run(host=host, debug=debug, port=port)
-
-
-if __name__ == "__main__":
-    sys.exit(cli())  # pragma: no cover
+# -*- coding: utf-8 -*-
+
+"""Console script for opentnsim."""
+import sys
+import click
+
+import opentnsim.server
+
+
+@click.group()
+def cli(args=None):
+    """OpenTNSim simulation."""
+    click.echo("Replace this message by putting your code into " "opentnsim.cli.main")
+    click.echo("See click documentation at http://click.pocoo.org/")
+    return 0
+
+
+@cli.command()
+@click.option("--host", default="0.0.0.0")
+@click.option("--port", default=5000, type=int)
+@click.option("--debug/--no-debug", default=False)
+def serve(host, port, debug, args=None):
+    """Run a flask server with the backend code"""
+    app = opentnsim.server.app
+    app.run(host=host, debug=debug, port=port)
+
+
+if __name__ == "__main__":
+    sys.exit(cli())  # pragma: no cover
```

### Comparing `opentnsim-1.0.0/opentnsim/plot.py` & `opentnsim-1.1.2/opentnsim/plot.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,412 +1,404 @@
-import pandas as pd
-import numpy as np
-import datetime
-
-# plotting libraries
-from plotly.offline import init_notebook_mode, iplot
-import plotly.graph_objs as go
-import matplotlib.pyplot as plt
-
-# spatial libraries
-import pyproj
-import shapely.geometry
-from simplekml import Kml, Style
-
-import networkx as nx
-
-
-def vessel_planning(vessels, activities, colors, web=False):
-    """create a plot of the planning of vessels"""
-
-    def get_segments(series, activity, y_val):
-        """extract 'start' and 'stop' of activities from log"""
-        x = []
-        y = []
-        for i, v in series.iteritems():
-            if v == activity + " start":
-                start = i
-            if v == activity + " stop":
-                x.extend((start, start, i, i, i))
-                y.extend((y_val, y_val, y_val, y_val, None))
-        return x, y
-
-    # organise logdata into 'dataframes'
-    dataframes = []
-    for vessel in vessels:
-        df = pd.DataFrame(
-            {"log_value": vessel.log["Value"], "log_string": vessel.log["Message"]},
-            vessel.log["Timestamp"],
-        )
-        dataframes.append(df)
-    df = dataframes[0]
-
-    # prepare traces for each of the activities
-    traces = []
-    for i, activity in enumerate(activities):
-        x_combined = []
-        y_combined = []
-        for k, df in enumerate(dataframes):
-            y_val = vessels[k].name
-            x, y = get_segments(df["log_string"], activity=activity, y_val=y_val)
-            x_combined.extend(x)
-            y_combined.extend(y)
-        traces.append(
-            go.Scatter(
-                name=activity,
-                x=x_combined,
-                y=y_combined,
-                mode="lines",
-                hoverinfo="y+name",
-                line=dict(color=colors[i], width=10),
-                connectgaps=False,
-            )
-        )
-
-    # prepare layout of figure
-    layout = go.Layout(
-        title="Vessel planning",
-        hovermode="closest",
-        legend=dict(x=0, y=-0.2, orientation="h"),
-        xaxis=dict(
-            title="Time",
-            titlefont=dict(family="Courier New, monospace", size=18, color="#7f7f7f"),
-            range=[0, vessel.log["Timestamp"][-1]],
-        ),
-        yaxis=dict(
-            title="Vessels",
-            titlefont=dict(family="Courier New, monospace", size=18, color="#7f7f7f"),
-        ),
-    )
-
-    # plot figure
-    init_notebook_mode(connected=True)
-    fig = go.Figure(data=traces, layout=layout)
-    return iplot(fig, filename="news-source")
-
-
-def vessel_kml(
-        env,
-        vessels,
-        fname="vessel_movements.kml",
-        icon="http://maps.google.com/mapfiles/kml/shapes/sailing.png",
-        size=1,
-        scale=1,
-        stepsize=120,
-):
-    """Create a kml visualisation of vessels. Env variable needs to contain 
-        epoch to enable conversion of simulation time to real time. Vessels need
-        logs that contain geometries in lat, lon as a function of time."""
-
-    # create a kml file containing the visualisation
-    kml = Kml()
-    fol = kml.newfolder(name="Vessels")
-
-    shared_style = Style()
-    shared_style.labelstyle.color = "ffffffff"  # White
-    shared_style.labelstyle.scale = size
-    shared_style.iconstyle.color = "ffff0000"  # Blue
-    shared_style.iconstyle.scale = scale
-    shared_style.iconstyle.icon.href = icon
-
-    # each timestep will be represented as a single point
-    for vessel in vessels:
-        geom_x = []
-        geom_y = []
-
-        for geom in vessel.log["Geometry"]:
-            geom_x.append(geom.x)
-            geom_y.append(geom.y)
-
-        vessel.log["Geometry - x"] = geom_x
-        vessel.log["Geometry - y"] = geom_y
-
-        time_stamp_min = min(vessel.log["Timestamp"]).timestamp()
-        time_stamp_max = max(vessel.log["Timestamp"]).timestamp()
-
-        steps = int(np.floor((time_stamp_max - time_stamp_min) / stepsize))
-        timestamps_t = np.linspace(time_stamp_min, time_stamp_max, steps)
-
-        times = []
-        for t in vessel.log["Timestamp"]:
-            times.append(t.timestamp())
-
-        vessel.log["timestamps_t"] = timestamps_t
-        vessel.log["timestamps_x"] = np.interp(
-            timestamps_t, times, vessel.log["Geometry - x"]
-        )
-        vessel.log["timestamps_y"] = np.interp(
-            timestamps_t, times, vessel.log["Geometry - y"]
-        )
-
-        for log_index, value in enumerate(vessel.log["timestamps_t"][:-1]):
-            begin = datetime.datetime.fromtimestamp(
-                vessel.log["timestamps_t"][log_index]
-            )
-            end = datetime.datetime.fromtimestamp(
-                vessel.log["timestamps_t"][log_index + 1]
-            )
-
-            pnt = fol.newpoint(
-                name=vessel.name,
-                coords=[
-                    (
-                        vessel.log["timestamps_x"][log_index],
-                        vessel.log["timestamps_y"][log_index],
-                    )
-                ],
-            )
-            pnt.timespan.begin = begin.isoformat()
-            pnt.timespan.end = end.isoformat()
-            pnt.style = shared_style
-
-        # include last point as well
-        begin = datetime.datetime.fromtimestamp(
-            vessel.log["timestamps_t"][log_index + 1]
-        )
-        # end = datetime.datetime.fromtimestamp(vessel.log["timestamps_t"][log_index + 1])
-
-        pnt = fol.newpoint(
-            name=vessel.name,
-            coords=[
-                (
-                    vessel.log["timestamps_x"][log_index + 1],
-                    vessel.log["timestamps_y"][log_index + 1],
-                )
-            ],
-        )
-        pnt.timespan.begin = begin.isoformat()
-        # pnt.timespan.end = end.isoformat()
-        pnt.style = shared_style
-
-    kml.save(fname)
-
-
-def site_kml(
-        env,
-        sites,
-        fname="site_development.kml",
-        icon="http://maps.google.com/mapfiles/kml/shapes/square.png",
-        size=1,
-        scale=3,
-        stepsize=120,
-):
-    """Create a kml visualisation of vessels. Env variable needs to contain 
-        epoch to enable conversion of simulation time to real time. Vessels need
-        logs that contain geometries in lat, lon as a function of time."""
-
-    # create a kml file containing the visualisation
-    kml = Kml()
-    fol = kml.newfolder(name="Sites")
-
-    # each timestep will be represented as a single point
-    for site in sites:
-        for log_index, value in enumerate(site.log["Timestamp"][:-1]):
-            style = Style()
-            style.labelstyle.color = "ffffffff"  # White
-            style.labelstyle.scale = 1
-            style.iconstyle.color = "ff00ffff"  # Yellow
-            style.iconstyle.scale = scale * (
-                    site.log["Value"][log_index] / site.container.capacity
-            )
-            style.iconstyle.icon.href = icon
-
-            begin = site.log["Timestamp"][log_index]
-            end = site.log["Timestamp"][log_index + 1]
-
-            pnt = fol.newpoint(
-                name=site.name,
-                coords=[
-                    (
-                        site.log["Geometry"][log_index].x,
-                        site.log["Geometry"][log_index].y,
-                    )
-                ],
-            )
-            pnt.timespan.begin = begin.isoformat()
-            pnt.timespan.end = end.isoformat()
-            pnt.style = style
-
-        # include last point as well
-        style = Style()
-        style.labelstyle.color = "ffffffff"  # White
-        style.labelstyle.scale = 1
-        style.iconstyle.color = "ff00ffff"  # Yellow
-        style.iconstyle.scale = scale * (
-                site.log["Value"][log_index + 1] / site.container.capacity
-        )
-        style.iconstyle.icon.href = icon
-
-        begin = site.log["Timestamp"][log_index + 1]
-        # end = site.log["Timestamp"][log_index + 1]
-
-        pnt = fol.newpoint(
-            name=site.name,
-            coords=[
-                (
-                    site.log["Geometry"][log_index + 1].x,
-                    site.log["Geometry"][log_index + 1].y,
-                )
-            ],
-        )
-        pnt.timespan.begin = begin.isoformat()
-        # pnt.timespan.end = end.isoformat()
-        pnt.style = style
-
-    kml.save(fname)
-
-
-def graph_kml(
-        env,
-        fname="graph.kml",
-        icon="http://maps.google.com/mapfiles/kml/shapes/donut.png",
-        size=0.5,
-        scale=0.5,
-        width=5,
-):
-    """Create a kml visualisation of graph. Env variable needs to contain 
-        graph."""
-
-    # create a kml file containing the visualisation
-    kml = Kml()
-    fol = kml.newfolder(name="Vessels")
-
-    shared_style = Style()
-    shared_style.labelstyle.color = "ffffffff"  # White
-    shared_style.labelstyle.scale = size
-    shared_style.iconstyle.color = "ffffffff"  # White
-    shared_style.iconstyle.scale = scale
-    shared_style.iconstyle.icon.href = icon
-    shared_style.linestyle.color = "ff0055ff"  # Red
-    shared_style.linestyle.width = width
-
-    nodes = list(env.FG.nodes)
-
-    # each timestep will be represented as a single point
-    for log_index, value in enumerate(list(env.FG.nodes)[0: -1 - 1]):
-        pnt = fol.newpoint(
-            name="",
-            coords=[
-                (
-                    nx.get_node_attributes(env.FG, "geometry")[nodes[log_index]].x,
-                    nx.get_node_attributes(env.FG, "geometry")[nodes[log_index]].y,
-                )
-            ],
-        )
-        pnt.style = shared_style
-
-    edges = list(env.FG.edges)
-    for log_index, value in enumerate(list(env.FG.edges)[0: -1 - 1]):
-        lne = fol.newlinestring(
-            name="",
-            coords=[
-                (
-                    nx.get_node_attributes(env.FG, "geometry")[edges[log_index][0]].x,
-                    nx.get_node_attributes(env.FG, "geometry")[edges[log_index][0]].y,
-                ),
-                (
-                    nx.get_node_attributes(env.FG, "geometry")[edges[log_index][1]].x,
-                    nx.get_node_attributes(env.FG, "geometry")[edges[log_index][1]].y,
-                ),
-            ],
-        )
-        lne.style = shared_style
-
-    kml.save(fname)
-
-
-def energy_use(vessel, testing=False):
-    energy_use_loading = 0  # concumption between loading start and loading stop
-    energy_use_sailing_full = (
-        0
-    )  # concumption between sailing full start and sailing full stop
-    energy_use_unloading = 0  # concumption between unloading  start and unloading  stop
-    energy_use_sailing_empty = (
-        0
-    )  # concumption between sailing empty start and sailing empty stop
-    energy_use_waiting = 0  # concumption between waiting start and waiting stop
-
-    for i in range(len(vessel.log["Message"])):
-        if vessel.log["Message"][i] == "Energy use loading":
-            energy_use_loading += vessel.log["Value"][i]
-
-        elif vessel.log["Message"][i] == "Energy use sailing full":
-            energy_use_sailing_full += vessel.log["Value"][i]
-
-        elif vessel.log["Message"][i] == "Energy use unloading":
-            energy_use_unloading += vessel.log["Value"][i]
-
-        elif vessel.log["Message"][i] == "Energy use sailing empty":
-            energy_use_sailing_empty += vessel.log["Value"][i]
-
-        elif vessel.log["Message"][i] == "Energy use waiting":
-            energy_use_waiting += vessel.log["Value"][i]
-
-    # For the total plot
-    fig, ax1 = plt.subplots(figsize=[15, 10])
-
-    # For the barchart
-    height = [
-        energy_use_loading,
-        energy_use_unloading,
-        energy_use_sailing_full,
-        energy_use_sailing_empty,
-        energy_use_waiting,
-    ]
-    labels = ["Loading", "Unloading", "Sailing full", "Sailing empty", "Waiting"]
-    colors = [
-        (55 / 255, 126 / 255, 184 / 255),
-        (98 / 255, 192 / 255, 122 / 255),
-        (255 / 255, 150 / 255, 0 / 255),
-        (98 / 255, 141 / 255, 122 / 255),
-        (124 / 255, 10 / 255, 2 / 255),
-    ]
-
-    positions = np.arange(len(labels))
-    ax1.bar(positions, height, color=colors)
-
-    # For the cumulative percentages
-    total_use = sum(
-        [
-            energy_use_loading,
-            energy_use_unloading,
-            energy_use_sailing_full,
-            energy_use_sailing_empty,
-            energy_use_waiting,
-        ]
-    )
-
-    energy_use_unloading += energy_use_loading
-    energy_use_sailing_full += energy_use_unloading
-    energy_use_sailing_empty += energy_use_sailing_full
-    energy_use_waiting += energy_use_sailing_empty
-    y = [
-        energy_use_loading,
-        energy_use_unloading,
-        energy_use_sailing_full,
-        energy_use_sailing_empty,
-        energy_use_waiting,
-    ]
-    n = [
-        energy_use_loading / total_use,
-        energy_use_unloading / total_use,
-        energy_use_sailing_full / total_use,
-        energy_use_sailing_empty / total_use,
-        energy_use_waiting / total_use,
-    ]
-
-    ax1.plot(positions, y, "ko", markersize=10)
-    ax1.plot(positions, y, "k")
-
-    for i, txt in enumerate(n):
-        x_txt = positions[i] + 0.1
-        y_txt = y[i] * 0.95
-        ax1.annotate("{:02.1f}%".format(txt * 100), (x_txt, y_txt), size=12)
-
-    # Further markup
-    plt.ylabel("Energy useage in KWH", size=12)
-    ax1.set_xticks(positions)
-    ax1.set_xticklabels(labels, size=12)
-    plt.title("Energy use - {}".format(vessel.name), size=15)
-
-    if testing == False:
-        plt.show()
+import pandas as pd
+import numpy as np
+import datetime
+
+# plotting libraries
+from plotly.offline import init_notebook_mode, iplot
+import plotly.graph_objs as go
+import matplotlib.pyplot as plt
+
+# spatial libraries
+import pyproj
+import shapely.geometry
+from simplekml import Kml, Style
+
+import networkx as nx
+
+
+def vessel_planning(vessels, activities, colors, web=False):
+    """create a plot of the planning of vessels"""
+
+    def get_segments(series, activity, y_val):
+        """extract 'start' and 'stop' of activities from log"""
+        x = []
+        y = []
+        for i, v in series.iteritems():
+            if v == activity + " start":
+                start = i
+            if v == activity + " stop":
+                x.extend((start, start, i, i, i))
+                y.extend((y_val, y_val, y_val, y_val, None))
+        return x, y
+
+    # organise logdata into 'dataframes'
+    dataframes = []
+    for vessel in vessels:
+        rename = {"Value": "log_value", "Message": "log_string"}
+        df = pd.DataFrame(vessel.logbook)
+        df = df.set_index("Timestamp").rename(columns=rename)
+
+        dataframes.append(df)
+    df = dataframes[0]
+
+    # prepare traces for each of the activities
+    traces = []
+    for i, activity in enumerate(activities):
+        x_combined = []
+        y_combined = []
+        for k, df in enumerate(dataframes):
+            y_val = vessels[k].name
+            x, y = get_segments(df["log_string"], activity=activity, y_val=y_val)
+            x_combined.extend(x)
+            y_combined.extend(y)
+        traces.append(
+            go.Scatter(
+                name=activity,
+                x=x_combined,
+                y=y_combined,
+                mode="lines",
+                hoverinfo="y+name",
+                line=dict(color=colors[i], width=10),
+                connectgaps=False,
+            )
+        )
+
+    # prepare layout of figure
+    layout = go.Layout(
+        title="Vessel planning",
+        hovermode="closest",
+        legend=dict(x=0, y=-0.2, orientation="h"),
+        xaxis=dict(
+            title="Time",
+            titlefont=dict(family="Courier New, monospace", size=18, color="#7f7f7f"),
+            range=[0, df.index[-1]],
+        ),
+        yaxis=dict(
+            title="Vessels",
+            titlefont=dict(family="Courier New, monospace", size=18, color="#7f7f7f"),
+        ),
+    )
+
+    # plot figure
+    init_notebook_mode(connected=True)
+    fig = go.Figure(data=traces, layout=layout)
+    return iplot(fig, filename="news-source")
+
+
+def vessel_kml(
+    env,
+    vessels,
+    fname="vessel_movements.kml",
+    icon="http://maps.google.com/mapfiles/kml/shapes/sailing.png",
+    size=1,
+    scale=1,
+    stepsize=120,
+):
+    """Create a kml visualisation of vessels. Env variable needs to contain
+    epoch to enable conversion of simulation time to real time. Vessels need
+    logs that contain geometries in lat, lon as a function of time."""
+
+    # create a kml file containing the visualisation
+    kml = Kml()
+    fol = kml.newfolder(name="Vessels")
+
+    shared_style = Style()
+    shared_style.labelstyle.color = "ffffffff"  # White
+    shared_style.labelstyle.scale = size
+    shared_style.iconstyle.color = "ffff0000"  # Blue
+    shared_style.iconstyle.scale = scale
+    shared_style.iconstyle.icon.href = icon
+
+    # each timestep will be represented as a single point
+    # todo: create a tmpvessel to log info. Do not attach it to the original vessel log!
+    for vessel in vessels:
+        tmp_vessel = {
+            "Geometry - x": [],
+            "Geometry - y": [],
+            "timestamps_t": [],
+            "timestamps_x": [],
+        }
+        geom_x = []
+        geom_y = []
+
+        vessel_log = pd.DataFrame(vessel.logbook)
+
+        for geom in vessel_log["Geometry"]:
+            geom_x.append(geom.x)
+            geom_y.append(geom.y)
+
+        tmp_vessel["Geometry - x"] = geom_x
+        tmp_vessel["Geometry - y"] = geom_y
+
+        time_stamp_min = min(vessel_log["Timestamp"]).timestamp()
+        time_stamp_max = max(vessel_log["Timestamp"]).timestamp()
+
+        steps = int(np.floor((time_stamp_max - time_stamp_min) / stepsize))
+        timestamps_t = np.linspace(time_stamp_min, time_stamp_max, steps)
+
+        times = []
+        for row in vessel.logbook:
+            t = row["Timestamp"]
+            times.append(t.timestamp())
+
+        tmp_vessel["timestamps_t"] = timestamps_t
+        tmp_vessel["timestamps_x"] = np.interp(timestamps_t, times, tmp_vessel["Geometry - x"])
+        tmp_vessel["timestamps_y"] = np.interp(timestamps_t, times, tmp_vessel["Geometry - y"])
+
+        for log_index, value in enumerate(tmp_vessel["timestamps_t"][:-1]):
+            begin = datetime.datetime.fromtimestamp(tmp_vessel["timestamps_t"][log_index])
+            end = datetime.datetime.fromtimestamp(tmp_vessel["timestamps_t"][log_index + 1])
+
+            pnt = fol.newpoint(
+                name=vessel.name,
+                coords=[
+                    (
+                        tmp_vessel["timestamps_x"][log_index],
+                        tmp_vessel["timestamps_y"][log_index],
+                    )
+                ],
+            )
+            pnt.timespan.begin = begin.isoformat()
+            pnt.timespan.end = end.isoformat()
+            pnt.style = shared_style
+
+        # include last point as well
+        begin = datetime.datetime.fromtimestamp(tmp_vessel["timestamps_t"][log_index + 1])
+        # end = datetime.datetime.fromtimestamp(vessel.log["timestamps_t"][log_index + 1])
+
+        pnt = fol.newpoint(
+            name=vessel.name,
+            coords=[
+                (
+                    tmp_vessel["timestamps_x"][log_index + 1],
+                    tmp_vessel["timestamps_y"][log_index + 1],
+                )
+            ],
+        )
+        pnt.timespan.begin = begin.isoformat()
+        # pnt.timespan.end = end.isoformat()
+        pnt.style = shared_style
+
+    kml.save(fname)
+
+
+def site_kml(
+    env,
+    sites,
+    fname="site_development.kml",
+    icon="http://maps.google.com/mapfiles/kml/shapes/square.png",
+    size=1,
+    scale=3,
+    stepsize=120,
+):
+    """Create a kml visualisation of vessels. Env variable needs to contain
+    epoch to enable conversion of simulation time to real time. Vessels need
+    logs that contain geometries in lat, lon as a function of time."""
+
+    # create a kml file containing the visualisation
+    kml = Kml()
+    fol = kml.newfolder(name="Sites")
+
+    # each timestep will be represented as a single point
+    for site in sites:
+        for log_index, value in enumerate(site.log["Timestamp"][:-1]):
+            style = Style()
+            style.labelstyle.color = "ffffffff"  # White
+            style.labelstyle.scale = 1
+            style.iconstyle.color = "ff00ffff"  # Yellow
+            style.iconstyle.scale = scale * (site.log["Value"][log_index] / site.container.capacity)
+            style.iconstyle.icon.href = icon
+
+            begin = site.log["Timestamp"][log_index]
+            end = site.log["Timestamp"][log_index + 1]
+
+            pnt = fol.newpoint(
+                name=site.name,
+                coords=[
+                    (
+                        site.log["Geometry"][log_index].x,
+                        site.log["Geometry"][log_index].y,
+                    )
+                ],
+            )
+            pnt.timespan.begin = begin.isoformat()
+            pnt.timespan.end = end.isoformat()
+            pnt.style = style
+
+        # include last point as well
+        style = Style()
+        style.labelstyle.color = "ffffffff"  # White
+        style.labelstyle.scale = 1
+        style.iconstyle.color = "ff00ffff"  # Yellow
+        style.iconstyle.scale = scale * (site.log["Value"][log_index + 1] / site.container.capacity)
+        style.iconstyle.icon.href = icon
+
+        begin = site.log["Timestamp"][log_index + 1]
+        # end = site.log["Timestamp"][log_index + 1]
+
+        pnt = fol.newpoint(
+            name=site.name,
+            coords=[
+                (
+                    site.log["Geometry"][log_index + 1].x,
+                    site.log["Geometry"][log_index + 1].y,
+                )
+            ],
+        )
+        pnt.timespan.begin = begin.isoformat()
+        # pnt.timespan.end = end.isoformat()
+        pnt.style = style
+
+    kml.save(fname)
+
+
+def graph_kml(
+    env,
+    fname="graph.kml",
+    icon="http://maps.google.com/mapfiles/kml/shapes/donut.png",
+    size=0.5,
+    scale=0.5,
+    width=5,
+):
+    """Create a kml visualisation of graph. Env variable needs to contain
+    graph."""
+
+    # create a kml file containing the visualisation
+    kml = Kml()
+    fol = kml.newfolder(name="Vessels")
+
+    shared_style = Style()
+    shared_style.labelstyle.color = "ffffffff"  # White
+    shared_style.labelstyle.scale = size
+    shared_style.iconstyle.color = "ffffffff"  # White
+    shared_style.iconstyle.scale = scale
+    shared_style.iconstyle.icon.href = icon
+    shared_style.linestyle.color = "ff0055ff"  # Red
+    shared_style.linestyle.width = width
+
+    nodes = list(env.FG.nodes)
+
+    # each timestep will be represented as a single point
+    for log_index, value in enumerate(list(env.FG.nodes)[0 : -1 - 1]):
+        pnt = fol.newpoint(
+            name="",
+            coords=[
+                (
+                    nx.get_node_attributes(env.FG, "geometry")[nodes[log_index]].x,
+                    nx.get_node_attributes(env.FG, "geometry")[nodes[log_index]].y,
+                )
+            ],
+        )
+        pnt.style = shared_style
+
+    edges = list(env.FG.edges)
+    for log_index, value in enumerate(list(env.FG.edges)[0 : -1 - 1]):
+        lne = fol.newlinestring(
+            name="",
+            coords=[
+                (
+                    nx.get_node_attributes(env.FG, "geometry")[edges[log_index][0]].x,
+                    nx.get_node_attributes(env.FG, "geometry")[edges[log_index][0]].y,
+                ),
+                (
+                    nx.get_node_attributes(env.FG, "geometry")[edges[log_index][1]].x,
+                    nx.get_node_attributes(env.FG, "geometry")[edges[log_index][1]].y,
+                ),
+            ],
+        )
+        lne.style = shared_style
+
+    kml.save(fname)
+
+
+def energy_use(vessel, testing=False):
+    energy_use_loading = 0  # concumption between loading start and loading stop
+    energy_use_sailing_full = 0  # concumption between sailing full start and sailing full stop
+    energy_use_unloading = 0  # concumption between unloading  start and unloading  stop
+    energy_use_sailing_empty = 0  # concumption between sailing empty start and sailing empty stop
+    energy_use_waiting = 0  # concumption between waiting start and waiting stop
+
+    for i in range(len(vessel.log["Message"])):
+        if vessel.log["Message"][i] == "Energy use loading":
+            energy_use_loading += vessel.log["Value"][i]
+
+        elif vessel.log["Message"][i] == "Energy use sailing full":
+            energy_use_sailing_full += vessel.log["Value"][i]
+
+        elif vessel.log["Message"][i] == "Energy use unloading":
+            energy_use_unloading += vessel.log["Value"][i]
+
+        elif vessel.log["Message"][i] == "Energy use sailing empty":
+            energy_use_sailing_empty += vessel.log["Value"][i]
+
+        elif vessel.log["Message"][i] == "Energy use waiting":
+            energy_use_waiting += vessel.log["Value"][i]
+
+    # For the total plot
+    fig, ax1 = plt.subplots(figsize=[15, 10])
+
+    # For the barchart
+    height = [
+        energy_use_loading,
+        energy_use_unloading,
+        energy_use_sailing_full,
+        energy_use_sailing_empty,
+        energy_use_waiting,
+    ]
+    labels = ["Loading", "Unloading", "Sailing full", "Sailing empty", "Waiting"]
+    colors = [
+        (55 / 255, 126 / 255, 184 / 255),
+        (98 / 255, 192 / 255, 122 / 255),
+        (255 / 255, 150 / 255, 0 / 255),
+        (98 / 255, 141 / 255, 122 / 255),
+        (124 / 255, 10 / 255, 2 / 255),
+    ]
+
+    positions = np.arange(len(labels))
+    ax1.bar(positions, height, color=colors)
+
+    # For the cumulative percentages
+    total_use = sum(
+        [
+            energy_use_loading,
+            energy_use_unloading,
+            energy_use_sailing_full,
+            energy_use_sailing_empty,
+            energy_use_waiting,
+        ]
+    )
+
+    energy_use_unloading += energy_use_loading
+    energy_use_sailing_full += energy_use_unloading
+    energy_use_sailing_empty += energy_use_sailing_full
+    energy_use_waiting += energy_use_sailing_empty
+    y = [
+        energy_use_loading,
+        energy_use_unloading,
+        energy_use_sailing_full,
+        energy_use_sailing_empty,
+        energy_use_waiting,
+    ]
+    n = [
+        energy_use_loading / total_use,
+        energy_use_unloading / total_use,
+        energy_use_sailing_full / total_use,
+        energy_use_sailing_empty / total_use,
+        energy_use_waiting / total_use,
+    ]
+
+    ax1.plot(positions, y, "ko", markersize=10)
+    ax1.plot(positions, y, "k")
+
+    for i, txt in enumerate(n):
+        x_txt = positions[i] + 0.1
+        y_txt = y[i] * 0.95
+        ax1.annotate("{:02.1f}%".format(txt * 100), (x_txt, y_txt), size=12)
+
+    # Further markup
+    plt.ylabel("Energy useage in KWH", size=12)
+    ax1.set_xticks(positions)
+    ax1.set_xticklabels(labels, size=12)
+    plt.title("Energy use - {}".format(vessel.name), size=15)
+
+    if testing == False:
+        plt.show()
```

### Comparing `opentnsim-1.0.0/setup.cfg` & `opentnsim-1.1.2/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,81 +1,80 @@
-00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
-00000010: 203d 204f 7065 6e54 4e53 696d 0d0a 6465   = OpenTNSim..de
-00000020: 7363 7269 7074 696f 6e20 3d20 5472 616e  scription = Tran
-00000030: 7370 6f72 7420 4e65 7477 6f72 6b20 416e  sport Network An
-00000040: 616c 7973 6973 202d 2066 6163 696c 6974  alysis - facilit
-00000050: 6174 6520 6261 7369 6320 6e61 7574 6963  ate basic nautic
-00000060: 616c 2074 7261 6666 6963 2073 696d 756c  al traffic simul
-00000070: 6174 696f 6e73 2e0d 0a61 7574 686f 7220  ations...author 
-00000080: 3d20 5455 2044 656c 6674 202f 2043 4954  = TU Delft / CIT
-00000090: 470d 0a61 7574 686f 722d 656d 6169 6c20  G..author-email 
-000000a0: 3d20 6d2e 7661 6e6b 6f6e 696e 6773 7665  = m.vankoningsve
-000000b0: 6c64 4074 7564 656c 6674 2e6e 6c0d 0a6c  ld@tudelft.nl..l
-000000c0: 6963 656e 7365 203d 206d 6974 0d0a 7572  icense = mit..ur
-000000d0: 6c20 3d20 6874 7470 733a 2f2f 7079 7363  l = https://pysc
-000000e0: 6166 666f 6c64 2e6f 7267 2f0d 0a6c 6f6e  affold.org/..lon
-000000f0: 672d 6465 7363 7269 7074 696f 6e20 3d20  g-description = 
-00000100: 6669 6c65 3a20 5245 4144 4d45 2e6d 640d  file: README.md.
-00000110: 0a70 6c61 7466 6f72 6d73 203d 2061 6e79  .platforms = any
-00000120: 0d0a 636c 6173 7369 6669 6572 7320 3d20  ..classifiers = 
-00000130: 0d0a 090d 0a09 4465 7665 6c6f 706d 656e  ......Developmen
-00000140: 7420 5374 6174 7573 203a 3a20 3420 2d20  t Status :: 4 - 
-00000150: 4265 7461 0d0a 090d 0a09 5072 6f67 7261  Beta......Progra
-00000160: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-00000170: 3a20 5079 7468 6f6e 0d0a 0d0a 5b6f 7074  : Python....[opt
-00000180: 696f 6e73 5d0d 0a7a 6970 5f73 6166 6520  ions]..zip_safe 
-00000190: 3d20 4661 6c73 650d 0a70 6163 6b61 6765  = False..package
-000001a0: 7320 3d20 6669 6e64 3a0d 0a69 6e63 6c75  s = find:..inclu
-000001b0: 6465 5f70 6163 6b61 6765 5f64 6174 6120  de_package_data 
-000001c0: 3d20 5472 7565 0d0a 7365 7475 705f 7265  = True..setup_re
-000001d0: 7175 6972 6573 203d 2070 7973 6361 6666  quires = pyscaff
-000001e0: 6f6c 643e 3d33 2e31 6130 2c3c 332e 3261  old>=3.1a0,<3.2a
-000001f0: 300d 0a69 6e73 7461 6c6c 5f72 6571 7569  0..install_requi
-00000200: 7265 7320 3d20 0d0a 0973 696d 7079 0d0a  res = ...simpy..
-00000210: 096e 6574 776f 726b 780d 0a09 6861 6c65  .networkx...hale
-00000220: 6d0d 0a09 7368 6170 656c 790d 0a09 7363  m...shapely...sc
-00000230: 6970 790d 0a09 706c 6f74 6c79 0d0a 0970  ipy...plotly...p
-00000240: 7973 6361 6666 6f6c 640d 0a09 7369 6d70  yscaffold...simp
-00000250: 6c65 6b6d 6c0d 0a09 6d61 7470 6c6f 746c  lekml...matplotl
-00000260: 6962 0d0a 0963 6c69 636b 0d0a 096e 6f73  ib...click...nos
-00000270: 650d 0a09 666c 6173 6b0d 0a09 666c 6173  e...flask...flas
-00000280: 6b5f 636f 7273 0d0a 0d0a 5b6f 7074 696f  k_cors....[optio
-00000290: 6e73 2e70 6163 6b61 6765 732e 6669 6e64  ns.packages.find
-000002a0: 5d0d 0a77 6865 7265 203d 2054 7261 6e73  ]..where = Trans
-000002b0: 706f 7274 2d4e 6574 776f 726b 2d41 6e61  port-Network-Ana
-000002c0: 6c79 7369 730d 0a0d 0a5b 6f70 7469 6f6e  lysis....[option
-000002d0: 732e 6578 7472 6173 5f72 6571 7569 7265  s.extras_require
-000002e0: 5d0d 0a74 6573 7469 6e67 203d 200d 0a09  ]..testing = ...
-000002f0: 7079 7465 7374 0d0a 0970 7974 6573 742d  pytest...pytest-
-00000300: 636f 760d 0a09 7079 7465 7374 2d74 696d  cov...pytest-tim
-00000310: 656f 7574 0d0a 0d0a 5b6f 7074 696f 6e73  eout....[options
-00000320: 2e65 6e74 7279 5f70 6f69 6e74 735d 0d0a  .entry_points]..
-00000330: 0d0a 5b74 6f6f 6c3a 7079 7465 7374 5d0d  ..[tool:pytest].
-00000340: 0a61 6464 6f70 7473 203d 200d 0a09 2d2d  .addopts = ...--
-00000350: 636f 7620 2d2d 636f 762d 7265 706f 7274  cov --cov-report
-00000360: 2074 6572 6d2d 6d69 7373 696e 6720 2d2d   term-missing --
-00000370: 636f 762d 7265 706f 7274 2068 746d 6c0d  cov-report html.
-00000380: 0a09 2d2d 7665 7262 6f73 650d 0a6e 6f72  ..--verbose..nor
-00000390: 6563 7572 7365 6469 7273 203d 200d 0a09  ecursedirs = ...
-000003a0: 6469 7374 0d0a 0962 7569 6c64 0d0a 092e  dist...build....
-000003b0: 746f 780d 0a09 2e65 6767 730d 0a74 6573  tox....eggs..tes
-000003c0: 7470 6174 6873 203d 2074 6573 7473 0d0a  tpaths = tests..
-000003d0: 0d0a 5b61 6c69 6173 6573 5d0d 0a64 6f63  ..[aliases]..doc
-000003e0: 7320 3d20 6275 696c 645f 7370 6869 6e78  s = build_sphinx
-000003f0: 0d0a 7465 7374 203d 2070 7974 6573 740d  ..test = pytest.
-00000400: 0a0d 0a5b 6264 6973 745f 7768 6565 6c5d  ...[bdist_wheel]
-00000410: 0d0a 756e 6976 6572 7361 6c20 3d20 310d  ..universal = 1.
-00000420: 0a0d 0a5b 6275 696c 645f 7370 6869 6e78  ...[build_sphinx
-00000430: 5d0d 0a73 6f75 7263 655f 6469 7220 3d20  ]..source_dir = 
-00000440: 646f 6373 0d0a 6275 696c 645f 6469 7220  docs..build_dir 
-00000450: 3d20 646f 6373 2f5f 6275 696c 640d 0a0d  = docs/_build...
-00000460: 0a5b 6465 7670 693a 7570 6c6f 6164 5d0d  .[devpi:upload].
-00000470: 0a6e 6f2d 7663 7320 3d20 310d 0a66 6f72  .no-vcs = 1..for
-00000480: 6d61 7473 203d 2062 6469 7374 5f77 6865  mats = bdist_whe
-00000490: 656c 0d0a 0d0a 5b66 6c61 6b65 385d 0d0a  el....[flake8]..
-000004a0: 6578 636c 7564 6520 3d20 0d0a 092e 746f  exclude = ....to
-000004b0: 780d 0a09 6275 696c 640d 0a09 6469 7374  x...build...dist
-000004c0: 0d0a 092e 6567 6773 0d0a 0964 6f63 732f  ....eggs...docs/
-000004d0: 636f 6e66 2e70 790d 0a0d 0a5b 6567 675f  conf.py....[egg_
-000004e0: 696e 666f 5d0d 0a74 6167 5f62 7569 6c64  info]..tag_build
-000004f0: 203d 200d 0a74 6167 5f64 6174 6520 3d20   = ..tag_date = 
-00000500: 300d 0a0d 0a                             0....
+00000000: 5b6d 6574 6164 6174 615d 0a6e 616d 6520  [metadata].name 
+00000010: 3d20 4f70 656e 544e 5369 6d0a 6465 7363  = OpenTNSim.desc
+00000020: 7269 7074 696f 6e20 3d20 5472 616e 7370  ription = Transp
+00000030: 6f72 7420 4e65 7477 6f72 6b20 416e 616c  ort Network Anal
+00000040: 7973 6973 202d 2066 6163 696c 6974 6174  ysis - facilitat
+00000050: 6520 6261 7369 6320 6e61 7574 6963 616c  e basic nautical
+00000060: 2074 7261 6666 6963 2073 696d 756c 6174   traffic simulat
+00000070: 696f 6e73 2e0a 6175 7468 6f72 203d 2054  ions..author = T
+00000080: 5520 4465 6c66 7420 2f20 4349 5447 0a61  U Delft / CITG.a
+00000090: 7574 686f 722d 656d 6169 6c20 3d20 6d2e  uthor-email = m.
+000000a0: 7661 6e6b 6f6e 696e 6773 7665 6c64 4074  vankoningsveld@t
+000000b0: 7564 656c 6674 2e6e 6c0a 6c69 6365 6e73  udelft.nl.licens
+000000c0: 6520 3d20 6d69 740a 7572 6c20 3d20 6874  e = mit.url = ht
+000000d0: 7470 733a 2f2f 7079 7363 6166 666f 6c64  tps://pyscaffold
+000000e0: 2e6f 7267 2f0a 6c6f 6e67 2d64 6573 6372  .org/.long-descr
+000000f0: 6970 7469 6f6e 203d 2066 696c 653a 2052  iption = file: R
+00000100: 4541 444d 452e 6d64 0a70 6c61 7466 6f72  EADME.md.platfor
+00000110: 6d73 203d 2061 6e79 0a63 6c61 7373 6966  ms = any.classif
+00000120: 6965 7273 203d 200a 090a 0944 6576 656c  iers = ....Devel
+00000130: 6f70 6d65 6e74 2053 7461 7475 7320 3a3a  opment Status ::
+00000140: 2034 202d 2042 6574 610a 090a 0950 726f   4 - Beta....Pro
+00000150: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+00000160: 6520 3a3a 2050 7974 686f 6e0a 0a5b 6f70  e :: Python..[op
+00000170: 7469 6f6e 735d 0a7a 6970 5f73 6166 6520  tions].zip_safe 
+00000180: 3d20 4661 6c73 650a 7061 636b 6167 6573  = False.packages
+00000190: 203d 2066 696e 643a 0a69 6e63 6c75 6465   = find:.include
+000001a0: 5f70 6163 6b61 6765 5f64 6174 6120 3d20  _package_data = 
+000001b0: 5472 7565 0a73 6574 7570 5f72 6571 7569  True.setup_requi
+000001c0: 7265 7320 3d20 7079 7363 6166 666f 6c64  res = pyscaffold
+000001d0: 3e3d 332e 3161 302c 3c33 2e32 6130 0a69  >=3.1a0,<3.2a0.i
+000001e0: 6e73 7461 6c6c 5f72 6571 7569 7265 7320  nstall_requires 
+000001f0: 3d20 0a09 4465 7072 6563 6174 6564 0a09  = ..Deprecated..
+00000200: 7369 6d70 790a 096e 6574 776f 726b 780a  simpy..networkx.
+00000210: 0968 616c 656d 0a09 7368 6170 656c 793e  .halem..shapely>
+00000220: 3d32 0a09 7363 6970 790a 0970 6c6f 746c  =2..scipy..plotl
+00000230: 790a 0970 7973 6361 6666 6f6c 640a 0973  y..pyscaffold..s
+00000240: 696d 706c 656b 6d6c 0a09 6d61 7470 6c6f  implekml..matplo
+00000250: 746c 6962 0a09 636c 6963 6b0a 096e 6f73  tlib..click..nos
+00000260: 650a 0966 6c61 736b 0a09 666c 6173 6b5f  e..flask..flask_
+00000270: 636f 7273 0a09 7471 646d 0a0a 5b6f 7074  cors..tqdm..[opt
+00000280: 696f 6e73 2e70 6163 6b61 6765 732e 6669  ions.packages.fi
+00000290: 6e64 5d0a 7768 6572 6520 3d20 5472 616e  nd].where = Tran
+000002a0: 7370 6f72 742d 4e65 7477 6f72 6b2d 416e  sport-Network-An
+000002b0: 616c 7973 6973 0a0a 5b6f 7074 696f 6e73  alysis..[options
+000002c0: 2e65 7874 7261 735f 7265 7175 6972 655d  .extras_require]
+000002d0: 0a74 6573 7469 6e67 203d 200a 0967 656f  .testing = ..geo
+000002e0: 7061 6e64 6173 0a09 7079 7465 7374 0a09  pandas..pytest..
+000002f0: 7079 7465 7374 2d63 6f76 0a09 7079 7465  pytest-cov..pyte
+00000300: 7374 2d74 696d 656f 7574 0a0a 5b6f 7074  st-timeout..[opt
+00000310: 696f 6e73 2e65 6e74 7279 5f70 6f69 6e74  ions.entry_point
+00000320: 735d 0a0a 5b74 6f6f 6c3a 7079 7465 7374  s]..[tool:pytest
+00000330: 5d0a 6164 646f 7074 7320 3d20 0a09 2d2d  ].addopts = ..--
+00000340: 636f 7620 2d2d 636f 762d 7265 706f 7274  cov --cov-report
+00000350: 2074 6572 6d2d 6d69 7373 696e 6720 2d2d   term-missing --
+00000360: 636f 762d 7265 706f 7274 2068 746d 6c0a  cov-report html.
+00000370: 092d 2d76 6572 626f 7365 0a6e 6f72 6563  .--verbose.norec
+00000380: 7572 7365 6469 7273 203d 200a 0964 6973  ursedirs = ..dis
+00000390: 740a 0962 7569 6c64 0a09 2e74 6f78 0a09  t..build...tox..
+000003a0: 2e65 6767 730a 7465 7374 7061 7468 7320  .eggs.testpaths 
+000003b0: 3d20 7465 7374 730a 0a5b 616c 6961 7365  = tests..[aliase
+000003c0: 735d 0a64 6f63 7320 3d20 6275 696c 645f  s].docs = build_
+000003d0: 7370 6869 6e78 0a74 6573 7420 3d20 7079  sphinx.test = py
+000003e0: 7465 7374 0a0a 5b62 6469 7374 5f77 6865  test..[bdist_whe
+000003f0: 656c 5d0a 756e 6976 6572 7361 6c20 3d20  el].universal = 
+00000400: 310a 0a5b 6275 696c 645f 7370 6869 6e78  1..[build_sphinx
+00000410: 5d0a 736f 7572 6365 5f64 6972 203d 2064  ].source_dir = d
+00000420: 6f63 730a 6275 696c 645f 6469 7220 3d20  ocs.build_dir = 
+00000430: 646f 6373 2f5f 6275 696c 640a 0a5b 6465  docs/_build..[de
+00000440: 7670 693a 7570 6c6f 6164 5d0a 6e6f 2d76  vpi:upload].no-v
+00000450: 6373 203d 2031 0a66 6f72 6d61 7473 203d  cs = 1.formats =
+00000460: 2062 6469 7374 5f77 6865 656c 0a0a 5b66   bdist_wheel..[f
+00000470: 6c61 6b65 385d 0a6d 6178 2d6c 696e 652d  lake8].max-line-
+00000480: 6c65 6e67 7468 203d 2031 3332 0a65 7874  length = 132.ext
+00000490: 656e 642d 6967 6e6f 7265 203d 2045 3230  end-ignore = E20
+000004a0: 330a 6578 636c 7564 6520 3d20 0a09 2e74  3.exclude = ...t
+000004b0: 6f78 0a09 6275 696c 640a 0964 6973 740a  ox..build..dist.
+000004c0: 092e 6567 6773 0a09 646f 6373 2f63 6f6e  ..eggs..docs/con
+000004d0: 662e 7079 0a0a 5b65 6767 5f69 6e66 6f5d  f.py..[egg_info]
+000004e0: 0a74 6167 5f62 7569 6c64 203d 200a 7461  .tag_build = .ta
+000004f0: 675f 6461 7465 203d 2030 0a0a            g_date = 0..
```

### Comparing `opentnsim-1.0.0/tests/vessels/vessels.csv` & `opentnsim-1.1.2/tests/vessels/vessels.csv`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-﻿vessel_id,vessel_type,width,length,height_empty,height_full,draught_empty,draught_full,capacity,installed_power
-12ad8a02-4aef-11e9-9940-b469212bff5b,CEMT - I,5.05,38.5,4.65,3.35,1.2,2.5,365,175
-17746aee-4aef-11e9-8ebf-b469212bff5b,CEMT - II,6.6,55,5.8,4.6,1.4,2.6,615,250
-1be5fb2e-4aef-11e9-9bfb-b469212bff5b,CEMT - III,8.2,85,6.3,5.1,1.5,2.7,1250,435
-208a5aca-4aef-11e9-b7e9-b469212bff5b,CEMT - IV,9.5,105,6.7,5.3,1.6,3,2040,690
-24f93100-4aef-11e9-8ff9-b469212bff5b,CEMT - Va,11.4,135,7.1,5.4,1.8,3.5,3735,1425
-289b8492-4aef-11e9-b34f-b469212bff5b,CEMT - VIa,17,135,10,8,2,4,6000,2015
+﻿vessel_id,vessel_type,width,length,height_empty,height_full,draught_empty,draught_full,capacity,installed_power
+12ad8a02-4aef-11e9-9940-b469212bff5b,CEMT - I,5.05,38.5,4.65,3.35,1.2,2.5,365,175
+17746aee-4aef-11e9-8ebf-b469212bff5b,CEMT - II,6.6,55,5.8,4.6,1.4,2.6,615,250
+1be5fb2e-4aef-11e9-9bfb-b469212bff5b,CEMT - III,8.2,85,6.3,5.1,1.5,2.7,1250,435
+208a5aca-4aef-11e9-b7e9-b469212bff5b,CEMT - IV,9.5,105,6.7,5.3,1.6,3,2040,690
+24f93100-4aef-11e9-8ff9-b469212bff5b,CEMT - Va,11.4,135,7.1,5.4,1.8,3.5,3735,1425
+289b8492-4aef-11e9-b34f-b469212bff5b,CEMT - VIa,17,135,10,8,2,4,6000,2015
```

