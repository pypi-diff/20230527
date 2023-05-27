# Comparing `tmp/cg-32.2.4.tar.gz` & `tmp/cg-32.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cg-32.2.4.tar", last modified: Fri May 26 12:06:16 2023, max compression
+gzip compressed data, was "dist/cg-32.2.5.tar", last modified: Sat May 27 11:20:57 2023, max compression
```

## Comparing `cg-32.2.4.tar` & `cg-32.2.5.tar`

### file list

```diff
@@ -1,1263 +1,1263 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-26 12:06:07.000000 cg-32.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-05-26 12:06:16.000000 cg-32.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-05-26 12:06:07.000000 cg-32.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-26 12:06:07.000000 cg-32.2.4/cg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/apps/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/apps/cgstats/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/cgstats/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/apps/cgstats/crud/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/cgstats/crud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15866 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/cgstats/crud/create.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/cgstats/crud/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     8001 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/cgstats/crud/find.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/apps/cgstats/db/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/cgstats/db/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/apps/cgstats/db/models/
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/cgstats/db/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/cgstats/db/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/cgstats/db/models/datasource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/cgstats/db/models/demux.py
--rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/cgstats/db/models/demux_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/cgstats/db/models/dragen_demux_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/cgstats/db/models/flowcell.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/cgstats/db/models/project.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/cgstats/db/models/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/cgstats/db/models/support_params.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/cgstats/db/models/unaligned.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/cgstats/db/models/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/apps/cgstats/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/cgstats/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/cgstats/parsers/adapter_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    11317 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/cgstats/parsers/conversion_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/cgstats/parsers/demux_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/cgstats/parsers/dragen_demultiplexing_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/cgstats/parsers/quality_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/cgstats/parsers/run_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     6315 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/cgstats/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/apps/coverage/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/coverage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/coverage/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/apps/crunchy/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/crunchy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12884 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/crunchy/crunchy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/crunchy/files.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/crunchy/sbatch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/apps/demultiplex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/demultiplex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11469 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/demultiplex/demultiplex_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/demultiplex/demux_report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/apps/demultiplex/sample_sheet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/demultiplex/sample_sheet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/demultiplex/sample_sheet/create.py
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/demultiplex/sample_sheet/dummy_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     5171 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/demultiplex/sample_sheet/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/demultiplex/sample_sheet/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5802 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/demultiplex/sample_sheet/novaseq_sample_sheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/demultiplex/sample_sheet/validate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/demultiplex/sbatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/environ.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/gens.py
--rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/gt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/apps/hermes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/hermes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/hermes/hermes_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/hermes/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/apps/housekeeper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/housekeeper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17538 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/housekeeper/hk.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/housekeeper/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/apps/invoice/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/invoice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/invoice/render.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/apps/invoice/templates/
--rw-r--r--   0 runner    (1001) docker     (123)   113439 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/invoice/templates/KI_pool_invoice.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    81032 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/invoice/templates/KI_sample_invoice.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   113363 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/invoice/templates/KTH_pool_invoice.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    80886 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/invoice/templates/KTH_sample_invoice.xlsx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/apps/lims/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/lims/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16393 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/lims/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/lims/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     8243 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/lims/order.py
--rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/lims/samplesheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/loqus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/apps/madeline/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/madeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/madeline/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/apps/mip/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/mip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/mip/confighandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/mutacc_auto.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/apps/orderform/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/orderform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9233 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/orderform/excel_orderform_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/orderform/json_orderform_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/orderform/orderform_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/osticket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/apps/scout/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/scout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/scout/scout_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     9882 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/scout/scoutapi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/apps/sequencing_metrics_parser/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/sequencing_metrics_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/sequencing_metrics_parser/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/apps/sequencing_metrics_parser/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/sequencing_metrics_parser/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/sequencing_metrics_parser/models/bcl2fastq_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/sequencing_metrics_parser/models/bcl_convert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/apps/sequencing_metrics_parser/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/sequencing_metrics_parser/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/sequencing_metrics_parser/parsers/bcl2fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/sequencing_metrics_parser/parsers/bcl2fastq_to_sequencing_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     7657 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/sequencing_metrics_parser/parsers/bcl_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/sequencing_metrics_parser/parsers/bcl_convert_to_sequencing_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/sequencing_metrics_parser/sequencing_metrics_calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/apps/slurm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/slurm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/slurm/sbatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/slurm/slurm_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/apps/tb/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/tb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8319 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/tb/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/tb/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-05-26 12:06:07.000000 cg-32.2.4/cg/apps/vogue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10329 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     7057 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    19665 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/clean.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/cli/compress/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/compress/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/compress/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6669 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/compress/fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     8507 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/compress/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/cli/delete/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/delete/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/delete/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/delete/case.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/delete/cases.py
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/delete/observations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/cli/deliver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/deliver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/deliver/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/cli/demultiplex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/demultiplex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/demultiplex/add.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/demultiplex/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7354 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/demultiplex/demux.py
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/demultiplex/finish.py
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/demultiplex/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/demultiplex/sample_sheet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/cli/generate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/generate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/generate/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/cli/generate/report/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/generate/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/generate/report/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/generate/report/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/generate/report/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8386 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/cli/set/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/set/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9868 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/set/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/set/case.py
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/set/cases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/cli/store/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/store/fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/store/store.py
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/transfer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/cli/upload/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/upload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/upload/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/upload/clinical_delivery.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/upload/coverage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/upload/delivery_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/upload/fohm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/upload/genotype.py
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/upload/gens.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/upload/gisaid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/upload/mutacc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/cli/upload/nipt/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/upload/nipt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/upload/nipt/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/upload/nipt/ftp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/upload/nipt/statina.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/cli/upload/observations/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/upload/observations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/upload/observations/observations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/upload/observations/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9563 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/upload/scout.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/upload/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/upload/validate.py
--rw-r--r--   0 runner    (1001) docker     (123)    11932 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/upload/vogue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/cli/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/workflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/cli/workflow/balsamic/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/workflow/balsamic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8860 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/workflow/balsamic/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/workflow/balsamic/options.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/workflow/balsamic/pon.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/workflow/balsamic/qc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/workflow/balsamic/umi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/workflow/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12622 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/workflow/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/cli/workflow/fastq/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/workflow/fastq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/workflow/fastq/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/cli/workflow/fluffy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/workflow/fluffy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/workflow/fluffy/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/cli/workflow/microsalt/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/workflow/microsalt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11101 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/workflow/microsalt/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/cli/workflow/mip/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/workflow/mip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6224 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/workflow/mip/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/workflow/mip/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/cli/workflow/mip_dna/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/workflow/mip_dna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/workflow/mip_dna/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/cli/workflow/mip_rna/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/workflow/mip_rna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/workflow/mip_rna/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/cli/workflow/mutant/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/workflow/mutant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/workflow/mutant/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/cli/workflow/nextflow/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/workflow/nextflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/workflow/nextflow/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/cli/workflow/rnafusion/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/workflow/rnafusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12229 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/workflow/rnafusion/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/workflow/rnafusion/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/cli/workflow/taxprofiler/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/workflow/taxprofiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/workflow/taxprofiler/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/cli/workflow/tower/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/workflow/tower/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-26 12:06:07.000000 cg-32.2.4/cg/cli/workflow/tower/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/constants/
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-05-26 12:06:07.000000 cg-32.2.4/cg/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-26 12:06:07.000000 cg-32.2.4/cg/constants/backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-26 12:06:07.000000 cg-32.2.4/cg/constants/bcl_convert_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-26 12:06:07.000000 cg-32.2.4/cg/constants/cgstats.py
--rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-05-26 12:06:07.000000 cg-32.2.4/cg/constants/compression.py
--rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-05-26 12:06:07.000000 cg-32.2.4/cg/constants/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-05-26 12:06:07.000000 cg-32.2.4/cg/constants/delivery.py
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-05-26 12:06:07.000000 cg-32.2.4/cg/constants/demultiplexing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-26 12:06:07.000000 cg-32.2.4/cg/constants/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-26 12:06:07.000000 cg-32.2.4/cg/constants/extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-26 12:06:07.000000 cg-32.2.4/cg/constants/gene_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-05-26 12:06:07.000000 cg-32.2.4/cg/constants/housekeeper_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-26 12:06:07.000000 cg-32.2.4/cg/constants/indexes.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-26 12:06:07.000000 cg-32.2.4/cg/constants/invoice.py
--rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-05-26 12:06:07.000000 cg-32.2.4/cg/constants/lims.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-26 12:06:07.000000 cg-32.2.4/cg/constants/nextflow.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-26 12:06:07.000000 cg-32.2.4/cg/constants/nipt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-05-26 12:06:07.000000 cg-32.2.4/cg/constants/observations.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-26 12:06:07.000000 cg-32.2.4/cg/constants/orderforms.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 12:06:07.000000 cg-32.2.4/cg/constants/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-26 12:06:07.000000 cg-32.2.4/cg/constants/pdc.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-26 12:06:07.000000 cg-32.2.4/cg/constants/pedigree.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-26 12:06:07.000000 cg-32.2.4/cg/constants/priority.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-26 12:06:07.000000 cg-32.2.4/cg/constants/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-05-26 12:06:07.000000 cg-32.2.4/cg/constants/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-26 12:06:07.000000 cg-32.2.4/cg/constants/rnafusion.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-26 12:06:07.000000 cg-32.2.4/cg/constants/sample_sources.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-05-26 12:06:07.000000 cg-32.2.4/cg/constants/scout_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-05-26 12:06:07.000000 cg-32.2.4/cg/constants/sequencing.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-26 12:06:07.000000 cg-32.2.4/cg/constants/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-26 12:06:07.000000 cg-32.2.4/cg/constants/subject.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-26 12:06:07.000000 cg-32.2.4/cg/constants/symbols.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-26 12:06:07.000000 cg-32.2.4/cg/constants/tb.py
--rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-05-26 12:06:07.000000 cg-32.2.4/cg/exc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/cg/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-26 12:06:07.000000 cg-32.2.4/cg/io/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-26 12:06:07.000000 cg-32.2.4/cg/io/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-05-26 12:06:07.000000 cg-32.2.4/cg/io/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-26 12:06:07.000000 cg-32.2.4/cg/io/json.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-26 12:06:07.000000 cg-32.2.4/cg/io/validate_path.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-26 12:06:07.000000 cg-32.2.4/cg/io/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/meta/archive/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/archive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8577 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/archive/ddn_dataflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/meta/backup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/backup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18893 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/backup/backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/backup/pdc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/meta/clean/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/clean/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/clean/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    14404 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/clean/demultiplexed_flow_cells.py
--rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/clean/flow_cell_run_directories.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/meta/compress/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/compress/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12476 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/compress/compress.py
--rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/compress/files.py
--rw-r--r--   0 runner    (1001) docker     (123)    13049 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/deliver.py
--rw-r--r--   0 runner    (1001) docker     (123)     8032 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/deliver_ticket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/meta/demultiplex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/demultiplex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11077 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/demultiplex/delete_demultiplex_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    15622 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/demultiplex/demux_post_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/demultiplex/files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/meta/encryption/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/encryption/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10747 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/encryption/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)    10954 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/invoice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/meta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/meta/observations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/observations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/observations/balsamic_observations_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/observations/mip_dna_observations_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5463 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/observations/observations_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/meta/orders/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/orders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/orders/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/orders/balsamic_qc_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/orders/balsamic_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/orders/balsamic_umi_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)    15376 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/orders/case_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/orders/fastq_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/orders/fluffy_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/orders/lims.py
--rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/orders/metagenome_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/orders/microbial_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/orders/microsalt_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/orders/mip_dna_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/orders/mip_rna_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/orders/pool_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/orders/rml_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/orders/sars_cov_2_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/orders/submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/orders/ticket_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/meta/report/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9732 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/report/balsamic.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/report/balsamic_umi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/report/field_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     7012 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/report/mip_dna.py
--rw-r--r--   0 runner    (1001) docker     (123)    17821 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/report/report_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/meta/report/templates/
--rw-r--r--   0 runner    (1001) docker     (123)    78964 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/report/templates/balsamic_report.html
--rw-r--r--   0 runner    (1001) docker     (123)   151463 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/report/templates/bootstrap.html
--rw-r--r--   0 runner    (1001) docker     (123)    77831 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/report/templates/mip-dna_report.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/meta/rsync/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/rsync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12066 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/rsync/rsync_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/rsync/sbatch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/meta/tar/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/tar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/tar/tar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/meta/transfer/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/transfer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10070 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/transfer/external_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     8417 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/transfer/flowcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/transfer/lims.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/meta/upload/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/upload/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/meta/upload/balsamic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/upload/balsamic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/upload/balsamic/balsamic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/upload/coverage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/meta/upload/fohm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/upload/fohm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12140 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/upload/fohm/fohm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/meta/upload/gisaid/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/upload/gisaid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/upload/gisaid/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    13572 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/upload/gisaid/gisaid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/upload/gisaid/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/upload/gt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/meta/upload/mip/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/upload/mip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/upload/mip/mip_dna.py
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/upload/mip/mip_rna.py
--rw-r--r--   0 runner    (1001) docker     (123)     7491 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/upload/mutacc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/meta/upload/nipt/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/upload/nipt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/upload/nipt/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     7542 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/upload/nipt/nipt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/meta/upload/rnafusion/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/upload/rnafusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/upload/rnafusion/rnafusion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/meta/upload/scout/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/upload/scout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/upload/scout/balsamic_config_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/upload/scout/balsamic_umi_config_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/upload/scout/hk_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/upload/scout/mip_config_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/upload/scout/rnafusion_config_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/upload/scout/scout_config_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    19045 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/upload/scout/uploadscoutapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/upload/upload_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/upload/vogue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/meta/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20004 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/workflow/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    28453 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/workflow/balsamic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/workflow/balsamic_pon.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/workflow/balsamic_qc.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/workflow/balsamic_umi.py
--rw-r--r--   0 runner    (1001) docker     (123)    10959 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/workflow/fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)    13390 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/workflow/fluffy.py
--rw-r--r--   0 runner    (1001) docker     (123)    18121 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/workflow/microsalt.py
--rw-r--r--   0 runner    (1001) docker     (123)    14337 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/workflow/mip.py
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/workflow/mip_dna.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/workflow/mip_rna.py
--rw-r--r--   0 runner    (1001) docker     (123)    10762 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/workflow/mutant.py
--rw-r--r--   0 runner    (1001) docker     (123)    11044 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/workflow/nextflow_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/workflow/prepare_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)    17110 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/workflow/rnafusion.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/workflow/taxprofiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-05-26 12:06:07.000000 cg-32.2.4/cg/meta/workflow/tower_common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/models/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-26 12:06:07.000000 cg-32.2.4/cg/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-26 12:06:07.000000 cg-32.2.4/cg/models/analysis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/models/balsamic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/cg/models/balsamic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-26 12:06:07.000000 cg-32.2.4/cg/models/balsamic/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-05-26 12:06:07.000000 cg-32.2.4/cg/models/balsamic/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-05-26 12:06:07.000000 cg-32.2.4/cg/models/balsamic/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    12924 2023-05-26 12:06:07.000000 cg-32.2.4/cg/models/cg_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/models/cgstats/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/cg/models/cgstats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-26 12:06:07.000000 cg-32.2.4/cg/models/cgstats/flowcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-26 12:06:07.000000 cg-32.2.4/cg/models/cgstats/stats_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-05-26 12:06:07.000000 cg-32.2.4/cg/models/compression_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/models/deliverables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/cg/models/deliverables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-05-26 12:06:07.000000 cg-32.2.4/cg/models/deliverables/metric_deliverables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/models/demultiplex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/cg/models/demultiplex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10905 2023-05-26 12:06:07.000000 cg-32.2.4/cg/models/demultiplex/demux_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     8513 2023-05-26 12:06:07.000000 cg-32.2.4/cg/models/demultiplex/flow_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-05-26 12:06:07.000000 cg-32.2.4/cg/models/demultiplex/run_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-26 12:06:07.000000 cg-32.2.4/cg/models/demultiplex/sbatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-26 12:06:07.000000 cg-32.2.4/cg/models/email.py
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-05-26 12:06:07.000000 cg-32.2.4/cg/models/file_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/models/invoice/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/cg/models/invoice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-05-26 12:06:07.000000 cg-32.2.4/cg/models/invoice/invoice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/models/lims/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/cg/models/lims/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-05-26 12:06:07.000000 cg-32.2.4/cg/models/lims/sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/models/mip/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/cg/models/mip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-26 12:06:07.000000 cg-32.2.4/cg/models/mip/mip_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-05-26 12:06:07.000000 cg-32.2.4/cg/models/mip/mip_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-05-26 12:06:07.000000 cg-32.2.4/cg/models/mip/mip_metrics_deliverables.py
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-05-26 12:06:07.000000 cg-32.2.4/cg/models/mip/mip_sample_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/models/nextflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/cg/models/nextflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-26 12:06:07.000000 cg-32.2.4/cg/models/nextflow/deliverables.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-26 12:06:07.000000 cg-32.2.4/cg/models/nextflow/sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/models/observations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/cg/models/observations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-05-26 12:06:07.000000 cg-32.2.4/cg/models/observations/input_files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/models/orders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/cg/models/orders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-26 12:06:07.000000 cg-32.2.4/cg/models/orders/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6002 2023-05-26 12:06:07.000000 cg-32.2.4/cg/models/orders/excel_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-26 12:06:07.000000 cg-32.2.4/cg/models/orders/json_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-26 12:06:07.000000 cg-32.2.4/cg/models/orders/order.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-26 12:06:07.000000 cg-32.2.4/cg/models/orders/orderform_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-05-26 12:06:07.000000 cg-32.2.4/cg/models/orders/sample_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9856 2023-05-26 12:06:07.000000 cg-32.2.4/cg/models/orders/samples.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/models/report/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/cg/models/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-05-26 12:06:07.000000 cg-32.2.4/cg/models/report/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-05-26 12:06:07.000000 cg-32.2.4/cg/models/report/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-05-26 12:06:07.000000 cg-32.2.4/cg/models/report/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-05-26 12:06:07.000000 cg-32.2.4/cg/models/report/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/models/rnafusion/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/cg/models/rnafusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-26 12:06:07.000000 cg-32.2.4/cg/models/rnafusion/rnafusion_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/models/scout/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/cg/models/scout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-05-26 12:06:07.000000 cg-32.2.4/cg/models/scout/scout_load_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/models/slurm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/cg/models/slurm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-26 12:06:07.000000 cg-32.2.4/cg/models/slurm/sbatch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/models/taxprofiler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/cg/models/taxprofiler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/models/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/cg/models/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-26 12:06:07.000000 cg-32.2.4/cg/models/workflow/mutant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/resources/
--rw-r--r--   0 runner    (1001) docker     (123)    25590 2023-05-26 12:06:07.000000 cg-32.2.4/cg/resources/20181012_Indices.csv
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-26 12:06:07.000000 cg-32.2.4/cg/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-05-26 12:06:07.000000 cg-32.2.4/cg/resources/rnafusion_bundle_filenames.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/cg/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16964 2023-05-26 12:06:07.000000 cg-32.2.4/cg/server/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)    19037 2023-05-26 12:06:07.000000 cg-32.2.4/cg/server/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-05-26 12:06:07.000000 cg-32.2.4/cg/server/app.py
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-26 12:06:07.000000 cg-32.2.4/cg/server/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-26 12:06:07.000000 cg-32.2.4/cg/server/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-26 12:06:07.000000 cg-32.2.4/cg/server/ext.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/server/invoices/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-26 12:06:07.000000 cg-32.2.4/cg/server/invoices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/server/invoices/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/server/invoices/templates/invoices/
--rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-05-26 12:06:07.000000 cg-32.2.4/cg/server/invoices/templates/invoices/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-05-26 12:06:07.000000 cg-32.2.4/cg/server/invoices/templates/invoices/invoice.html
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-05-26 12:06:07.000000 cg-32.2.4/cg/server/invoices/templates/invoices/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-05-26 12:06:07.000000 cg-32.2.4/cg/server/invoices/templates/invoices/new.html
--rw-r--r--   0 runner    (1001) docker     (123)     7794 2023-05-26 12:06:07.000000 cg-32.2.4/cg/server/invoices/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/server/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/server/templates/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-26 12:06:07.000000 cg-32.2.4/cg/server/templates/admin/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/store/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-26 12:06:07.000000 cg-32.2.4/cg/store/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/store/api/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-26 12:06:07.000000 cg-32.2.4/cg/store/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10616 2023-05-26 12:06:07.000000 cg-32.2.4/cg/store/api/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     6942 2023-05-26 12:06:07.000000 cg-32.2.4/cg/store/api/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-05-26 12:06:07.000000 cg-32.2.4/cg/store/api/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-26 12:06:07.000000 cg-32.2.4/cg/store/api/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     8530 2023-05-26 12:06:07.000000 cg-32.2.4/cg/store/api/find_basic_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    32466 2023-05-26 12:06:07.000000 cg-32.2.4/cg/store/api/find_business_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    39188 2023-05-26 12:06:07.000000 cg-32.2.4/cg/store/api/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/store/filters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/cg/store/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7005 2023-05-26 12:06:07.000000 cg-32.2.4/cg/store/filters/status_analysis_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-05-26 12:06:07.000000 cg-32.2.4/cg/store/filters/status_application_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-05-26 12:06:07.000000 cg-32.2.4/cg/store/filters/status_application_version_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-05-26 12:06:07.000000 cg-32.2.4/cg/store/filters/status_bed_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-26 12:06:07.000000 cg-32.2.4/cg/store/filters/status_bed_version_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    10718 2023-05-26 12:06:07.000000 cg-32.2.4/cg/store/filters/status_case_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-05-26 12:06:07.000000 cg-32.2.4/cg/store/filters/status_case_sample_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-26 12:06:07.000000 cg-32.2.4/cg/store/filters/status_collaboration_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-05-26 12:06:07.000000 cg-32.2.4/cg/store/filters/status_customer_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-26 12:06:07.000000 cg-32.2.4/cg/store/filters/status_flow_cell_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-26 12:06:07.000000 cg-32.2.4/cg/store/filters/status_invoice_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-26 12:06:07.000000 cg-32.2.4/cg/store/filters/status_organism_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-26 12:06:07.000000 cg-32.2.4/cg/store/filters/status_panel_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-05-26 12:06:07.000000 cg-32.2.4/cg/store/filters/status_pool_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     9943 2023-05-26 12:06:07.000000 cg-32.2.4/cg/store/filters/status_sample_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-26 12:06:07.000000 cg-32.2.4/cg/store/filters/status_user_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    29946 2023-05-26 12:06:07.000000 cg-32.2.4/cg/store/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-26 12:06:07.000000 cg-32.2.4/cg/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/utils/checksum/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/cg/utils/checksum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-26 12:06:07.000000 cg-32.2.4/cg/utils/checksum/checksum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/utils/click/
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-05-26 12:06:07.000000 cg-32.2.4/cg/utils/click/EnumChoice.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/cg/utils/click/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-05-26 12:06:07.000000 cg-32.2.4/cg/utils/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-05-26 12:06:07.000000 cg-32.2.4/cg/utils/date.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-26 12:06:07.000000 cg-32.2.4/cg/utils/dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-05-26 12:06:07.000000 cg-32.2.4/cg/utils/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-26 12:06:07.000000 cg-32.2.4/cg/utils/email.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-26 12:06:07.000000 cg-32.2.4/cg/utils/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-26 12:06:07.000000 cg-32.2.4/cg/utils/files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg/utils/flask/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/cg/utils/flask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-05-26 12:06:07.000000 cg-32.2.4/cg/utils/flask/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-26 12:06:07.000000 cg-32.2.4/cg/utils/time.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-26 12:06:07.000000 cg-32.2.4/cg/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/cg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-05-26 12:06:16.000000 cg-32.2.4/cg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    40436 2023-05-26 12:06:16.000000 cg-32.2.4/cg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 12:06:16.000000 cg-32.2.4/cg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-26 12:06:16.000000 cg-32.2.4/cg.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 12:06:16.000000 cg-32.2.4/cg.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-26 12:06:16.000000 cg-32.2.4/cg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-26 12:06:16.000000 cg-32.2.4/cg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-26 12:06:07.000000 cg-32.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-26 12:06:07.000000 cg-32.2.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 12:06:16.000000 cg-32.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-26 12:06:07.000000 cg-32.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/apps/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/apps/cgstats/
--rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-05-26 12:06:07.000000 cg-32.2.4/tests/apps/cgstats/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/apps/cgstats/crud/
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-05-26 12:06:07.000000 cg-32.2.4/tests/apps/cgstats/crud/test_create_novaseq.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-26 12:06:07.000000 cg-32.2.4/tests/apps/cgstats/crud/test_delete.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/apps/cgstats/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 12:06:07.000000 cg-32.2.4/tests/apps/cgstats/parsers/test_adapter_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-26 12:06:07.000000 cg-32.2.4/tests/apps/cgstats/parsers/test_conversion_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-26 12:06:07.000000 cg-32.2.4/tests/apps/cgstats/parsers/test_demux_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 12:06:07.000000 cg-32.2.4/tests/apps/cgstats/parsers/test_quality_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-26 12:06:07.000000 cg-32.2.4/tests/apps/cgstats/parsers/test_run_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-05-26 12:06:07.000000 cg-32.2.4/tests/apps/cgstats/test_cgstats_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-05-26 12:06:07.000000 cg-32.2.4/tests/apps/cgstats/test_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-26 12:06:07.000000 cg-32.2.4/tests/apps/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/apps/coverage/
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-26 12:06:07.000000 cg-32.2.4/tests/apps/coverage/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-05-26 12:06:07.000000 cg-32.2.4/tests/apps/coverage/test_coverage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/apps/crunchy/
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-05-26 12:06:07.000000 cg-32.2.4/tests/apps/crunchy/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-05-26 12:06:07.000000 cg-32.2.4/tests/apps/crunchy/test_compress_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-05-26 12:06:07.000000 cg-32.2.4/tests/apps/crunchy/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    14590 2023-05-26 12:06:07.000000 cg-32.2.4/tests/apps/crunchy/test_crunchy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9107 2023-05-26 12:06:07.000000 cg-32.2.4/tests/apps/crunchy/test_spring_decompression.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/apps/demultiplex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/tests/apps/demultiplex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10019 2023-05-26 12:06:07.000000 cg-32.2.4/tests/apps/demultiplex/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-26 12:06:07.000000 cg-32.2.4/tests/apps/demultiplex/test_convert_to_sample_sheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-26 12:06:07.000000 cg-32.2.4/tests/apps/demultiplex/test_demultiplex_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-05-26 12:06:07.000000 cg-32.2.4/tests/apps/demultiplex/test_sample_sheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6258 2023-05-26 12:06:07.000000 cg-32.2.4/tests/apps/demultiplex/test_validate_sample_sheet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/apps/gens/
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-05-26 12:06:07.000000 cg-32.2.4/tests/apps/gens/test_gens_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/apps/gt/
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-05-26 12:06:07.000000 cg-32.2.4/tests/apps/gt/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-05-26 12:06:07.000000 cg-32.2.4/tests/apps/gt/test_gt_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/apps/hk/
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-05-26 12:06:07.000000 cg-32.2.4/tests/apps/hk/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-26 12:06:07.000000 cg-32.2.4/tests/apps/hk/test__getattr__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-26 12:06:07.000000 cg-32.2.4/tests/apps/hk/test_add_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-05-26 12:06:07.000000 cg-32.2.4/tests/apps/hk/test_bundles.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-26 12:06:07.000000 cg-32.2.4/tests/apps/hk/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    24046 2023-05-26 12:06:07.000000 cg-32.2.4/tests/apps/hk/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-05-26 12:06:07.000000 cg-32.2.4/tests/apps/hk/test_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/apps/lims/
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-26 12:06:07.000000 cg-32.2.4/tests/apps/lims/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-05-26 12:06:07.000000 cg-32.2.4/tests/apps/lims/test_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/apps/loqus/
--rw-r--r--   0 runner    (1001) docker     (123)     9785 2023-05-26 12:06:07.000000 cg-32.2.4/tests/apps/loqus/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-05-26 12:06:07.000000 cg-32.2.4/tests/apps/loqus/test_loqusdb_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/apps/madeline/
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-05-26 12:06:07.000000 cg-32.2.4/tests/apps/madeline/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-05-26 12:06:07.000000 cg-32.2.4/tests/apps/madeline/test_madeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/apps/mip/
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-05-26 12:06:07.000000 cg-32.2.4/tests/apps/mip/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-26 12:06:07.000000 cg-32.2.4/tests/apps/mip/test_config_mip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/apps/mutacc_auto/
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-26 12:06:07.000000 cg-32.2.4/tests/apps/mutacc_auto/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-05-26 12:06:07.000000 cg-32.2.4/tests/apps/mutacc_auto/test_mutacc_auto.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/apps/orderform/
--rw-r--r--   0 runner    (1001) docker     (123)    11900 2023-05-26 12:06:07.000000 cg-32.2.4/tests/apps/orderform/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-05-26 12:06:07.000000 cg-32.2.4/tests/apps/orderform/test_excel_orderform_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-05-26 12:06:07.000000 cg-32.2.4/tests/apps/orderform/test_excel_sample_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-26 12:06:07.000000 cg-32.2.4/tests/apps/orderform/test_json_orderform_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-05-26 12:06:07.000000 cg-32.2.4/tests/apps/orderform/test_orderform_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/apps/scout/
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-05-26 12:06:07.000000 cg-32.2.4/tests/apps/scout/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-05-26 12:06:07.000000 cg-32.2.4/tests/apps/scout/test_get_causative_variants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-05-26 12:06:07.000000 cg-32.2.4/tests/apps/scout/test_get_scout_cases.py
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-05-26 12:06:07.000000 cg-32.2.4/tests/apps/scout/test_scout_load_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-05-26 12:06:07.000000 cg-32.2.4/tests/apps/scout/test_scout_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/apps/sequencing_metrics_parser/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/tests/apps/sequencing_metrics_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6678 2023-05-26 12:06:07.000000 cg-32.2.4/tests/apps/sequencing_metrics_parser/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/apps/sequencing_metrics_parser/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-05-26 12:06:07.000000 cg-32.2.4/tests/apps/sequencing_metrics_parser/parsers/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-26 12:06:07.000000 cg-32.2.4/tests/apps/sequencing_metrics_parser/parsers/test_bcl2fastq_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-26 12:06:07.000000 cg-32.2.4/tests/apps/sequencing_metrics_parser/parsers/test_bcl2fastq_to_sequencing_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-26 12:06:07.000000 cg-32.2.4/tests/apps/sequencing_metrics_parser/parsers/test_bcl_convert_to_sequencing_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)    10043 2023-05-26 12:06:07.000000 cg-32.2.4/tests/apps/sequencing_metrics_parser/parsers/test_bclconvert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-26 12:06:07.000000 cg-32.2.4/tests/apps/sequencing_metrics_parser/test_sequencing_metrics_calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/apps/slurm/
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-26 12:06:07.000000 cg-32.2.4/tests/apps/slurm/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-05-26 12:06:07.000000 cg-32.2.4/tests/apps/slurm/test_slurm_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-05-26 12:06:07.000000 cg-32.2.4/tests/apps/test_apps_environ.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-26 12:06:07.000000 cg-32.2.4/tests/apps/test_osticket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/apps/vogue/
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-26 12:06:07.000000 cg-32.2.4/tests/apps/vogue/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-05-26 12:06:07.000000 cg-32.2.4/tests/apps/vogue/test_vogue_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/cli/add/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/add/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/add/test_cli_add.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/add/test_cli_add_customer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/add/test_cli_add_family.py
--rw-r--r--   0 runner    (1001) docker     (123)     7565 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/add/test_cli_add_relationship.py
--rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/add/test_cli_add_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/cli/backup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/backup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/backup/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/backup/test_backup_command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/cli/clean/
--rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/clean/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5535 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/clean/test_balsamic_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/clean/test_clean_hk_bundle_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/clean/test_hk_bundle_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/clean/test_hk_case_bundle_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/clean/test_microbial_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/clean/test_rsync_past_run_dirs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/cli/compress/
--rw-r--r--   0 runner    (1001) docker     (123)    10311 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/compress/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6929 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/compress/test_cli_compress_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/compress/test_cli_decompress_spring.py
--rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/compress/test_compress_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/compress/test_store_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/cli/delete/
--rw-r--r--   0 runner    (1001) docker     (123)    12781 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/delete/test_cli_delete_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/delete/test_cli_delete_cases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/cli/deliver/
--rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/deliver/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/deliver/test_deliver_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/deliver/test_rsync_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8562 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/deliver/test_run_deliver_cmd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/cli/demultiplex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/demultiplex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11372 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/demultiplex/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/demultiplex/test_add_flowcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     4175 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/demultiplex/test_create_sample_sheet.py
--rw-r--r--   0 runner    (1001) docker     (123)    11412 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/demultiplex/test_demultiplex_flowcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/demultiplex/test_finish_demux.py
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/demultiplex/test_stats_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/demultiplex/test_validate_sample_sheet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/cli/generate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/generate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/cli/generate/report/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/generate/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/generate/report/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/generate/report/test_cli_delivery_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/generate/report/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/generate/test_cli_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/cli/get/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/get/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/get/test_cli_get.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/get/test_cli_get_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/get/test_cli_get_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/get/test_cli_get_flow_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     8862 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/get/test_cli_get_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/cli/set/
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/set/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7320 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/set/test_cli_set_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/set/test_cli_set_cases.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/set/test_cli_set_flowcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/set/test_cli_set_list_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)    12516 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/set/test_cli_set_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/set/test_cli_set_samples.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/cli/store/
--rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/store/test_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/test_clean.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/cli/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/cli/tests/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/cli/tests/fixtures/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/tests/fixtures/data/fastq.fastq.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/cli/upload/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/upload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10414 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/upload/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/upload/test_cli_scout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/upload/test_cli_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/upload/test_cli_upload_auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/upload/test_cli_upload_delivery_report.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/upload/test_cli_upload_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/upload/test_cli_upload_genotype.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/upload/test_cli_upload_gens.py
--rw-r--r--   0 runner    (1001) docker     (123)     9971 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/upload/test_cli_upload_nipt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/upload/test_cli_upload_nipt_ftp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/upload/test_cli_upload_nipt_statina.py
--rw-r--r--   0 runner    (1001) docker     (123)     5963 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/upload/test_cli_upload_observations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/upload/test_cli_upload_vogue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/cli/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/workflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/cli/workflow/balsamic/
--rw-r--r--   0 runner    (1001) docker     (123)    30801 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/workflow/balsamic/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    15328 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/workflow/balsamic/test_cli_balsamic_config_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/workflow/balsamic/test_compound_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/workflow/balsamic/test_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/workflow/balsamic/test_report_deliver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6369 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/workflow/balsamic/test_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/workflow/balsamic/test_store_housekeeper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7787 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/workflow/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/cli/workflow/fastq/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/workflow/fastq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/workflow/fastq/test_fastq_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/cli/workflow/fluffy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/workflow/fluffy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/workflow/fluffy/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/workflow/fluffy/test_cli_create_samplesheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/workflow/fluffy/test_cli_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/workflow/fluffy/test_cli_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/workflow/fluffy/test_cli_start.py
--rw-r--r--   0 runner    (1001) docker     (123)     7878 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/workflow/fluffy/test_cli_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/cli/workflow/microsalt/
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/workflow/microsalt/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/cli/workflow/microsalt/snapshots/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/workflow/microsalt/snapshots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/workflow/microsalt/snapshots/snap_test_microsalt_case_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7185 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/workflow/microsalt/test_microsalt_case_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/workflow/microsalt/test_microsalt_run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/cli/workflow/mip/
--rw-r--r--   0 runner    (1001) docker     (123)     6965 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/workflow/mip/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6951 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/workflow/mip/test_cli_mip_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/workflow/mip/test_cli_mip_dna_config_case.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/workflow/mip/test_cli_mip_dna_link.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/workflow/mip/test_cli_mip_dna_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/workflow/mip/test_cli_mip_dna_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/workflow/mip/test_cli_mip_dna_start.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/workflow/mip/test_cli_mip_rna_config_case.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/workflow/mip/test_cli_mip_rna_link.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/workflow/mip/test_cli_mip_rna_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     8558 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/workflow/mip/test_cli_mip_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/cli/workflow/rnafusion/
--rw-r--r--   0 runner    (1001) docker     (123)     8350 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/workflow/rnafusion/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/workflow/rnafusion/test_cli_rnafusion_compound_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     5254 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/workflow/rnafusion/test_cli_rnafusion_config_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/workflow/rnafusion/test_cli_rnafusion_metrics_deliver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/workflow/rnafusion/test_cli_rnafusion_report_deliver.py
--rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/workflow/rnafusion/test_cli_rnafusion_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     8449 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/workflow/rnafusion/test_cli_rnafusion_store_housekeeper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/cli/workflow/taxprofiler/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/workflow/taxprofiler/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/workflow/taxprofiler/test_cli_taxprofiler_compound_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/workflow/test_cli_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-05-26 12:06:07.000000 cg-32.2.4/tests/cli/workflow/test_cli_workflow_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)    62393 2023-05-26 12:06:07.000000 cg-32.2.4/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/fixtures/DEMUX/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/ADM1136A3_XTC08_AGTGGTCA_L001_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/ADM1136A3_XTC08_AGTGGTCA_L001_R2_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/ADM1136A3_XTC08_AGTGGTCA_L002_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/ADM1136A3_XTC08_AGTGGTCA_L002_R2_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/runParameters.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/fixtures/analysis/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/fixtures/analysis/balsamic/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/fixtures/analysis/balsamic/tn_wgs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/analysis/balsamic/tn_wgs/adm1.cram
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/analysis/balsamic/tn_wgs/ascat.output.pdf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/analysis/balsamic/tn_wgs/snv.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/analysis/balsamic/tn_wgs/sv.vcf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/fixtures/analysis/microsalt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/
--rw-r--r--   0 runner    (1001) docker     (123)    14644 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/ACC11111_qc_fail.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/
--rw-r--r--   0 runner    (1001) docker     (123)    15713 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/ACC22222_qc_pass.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/fixtures/analysis/mip/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/fixtures/analysis/mip/dna/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/analysis/mip/dna/ADM1.baf.bed.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/analysis/mip/dna/ADM1.cov.bed.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/analysis/mip/dna/ADM2.cram
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/analysis/mip/dna/ADM3.cram
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/analysis/mip/dna/adm1.cram
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/analysis/mip/dna/adm1.mt.bam
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/analysis/mip/dna/multiqc.html
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/analysis/mip/dna/report.pdf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/analysis/mip/dna/smn.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/analysis/mip/dna/snv.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/analysis/mip/dna/snv_research.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/analysis/mip/dna/str.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/analysis/mip/dna/sv.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/analysis/mip/dna/sv_research.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/analysis/mip/dna/vcf2cytosure.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/fixtures/analysis/rnafusion/
--rw-r--r--   0 runner    (1001) docker     (123)     5587 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/analysis/rnafusion/multiqc_data.json
--rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/analysis/sample_coverage.bed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/fixtures/apps/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/fixtures/apps/balsamic/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/fixtures/apps/balsamic/case/
--rw-r--r--   0 runner    (1001) docker     (123)     9948 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/balsamic/case/config.json
--rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/balsamic/case/metadata.yml
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/balsamic/case/metadata_directory.yml
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/balsamic/case/metadata_file_tags.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/balsamic/case/metrics_deliverables.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/fixtures/apps/crunchy/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/crunchy/spring_metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/fixtures/apps/demultiplexing/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/
--rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml
--rw-r--r--   0 runner    (1001) docker     (123)    53877 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv
--rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/demultiplexing/RunParameters_different_index_cycles.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/demultiplexing/SampleSheetS2_Bcl2Fastq.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/demultiplexing/SampleSheetS2_Dragen.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/HN3FKDSXY_AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/HN3FKDSXY_AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R2_001.fastq.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/
--rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/Adapter_Metrics.csv
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/Quality_Metrics.csv
--rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/RunInfo.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/dummy_run_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/dummy_run_R1_001.fastq.gz.md5
--rw-r--r--   0 runner    (1001) docker     (123)   338370 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R1_001.fastq.gz.md5
--rw-r--r--   0 runner    (1001) docker     (123)   338349 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R2_001.fastq.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R2_001.fastq.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L001_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L001_R2_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L002_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L002_R2_001.fastq.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/fixtures/apps/demultiplexing/flow-cell-runs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/fixtures/apps/demultiplexing/flow-cell-runs/201203_A00689_0200_AHVKJCDRXX/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/demultiplexing/flow-cell-runs/201203_A00689_0200_AHVKJCDRXX/CopyComplete.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/demultiplexing/flow-cell-runs/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/demultiplexing/flow-cell-runs/201203_A00689_0200_AHVKJCDRXX/RTAComplete.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/demultiplexing/flow-cell-runs/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/demultiplexing/flow-cell-runs/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/demultiplexing/flow-cell-runs/201203_A00689_0200_AHVKJCDRXX/demuxstarted.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/fixtures/apps/demultiplexing/flow-cell-runs/211101_A00187_0615_AHLG5GDRXY/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/demultiplexing/flow-cell-runs/211101_A00187_0615_AHLG5GDRXY/CopyComplete.txt
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/demultiplexing/flow-cell-runs/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stderr
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/demultiplexing/flow-cell-runs/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/demultiplexing/flow-cell-runs/211101_A00187_0615_AHLG5GDRXY/RTAComplete.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/demultiplexing/flow-cell-runs/211101_A00187_0615_AHLG5GDRXY/RunParameters.xml
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/demultiplexing/flow-cell-runs/211101_A00187_0615_AHLG5GDRXY/SampleSheet.csv
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/demultiplexing/flow-cell-runs/211101_A00187_0615_AHLG5GDRXY/demuxstarted.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/fixtures/apps/demultiplexing/hiseq_run/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/fixtures/apps/demultiplexing/hiseq_run/201203_A00689_0200_AHVKJCDRXX/
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/demultiplexing/hiseq_run/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/demultiplexing/hiseq_run/201203_A00689_0200_AHVKJCDRXX/RTAComplete.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/demultiplexing/hiseq_run/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/demultiplexing/hiseq_run/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/demultiplexing/hiseq_run/201203_A00689_0200_AHVKJCDRXX/copycomplete.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/demultiplexing/hiseq_run/201203_A00689_0200_AHVKJCDRXX/demuxstarted.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/demultiplexing/hiseq_run/runParameters.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/fixtures/apps/demultiplexing/raw_lims_samples/
--rw-r--r--   0 runner    (1001) docker     (123)    92887 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/demultiplexing/raw_lims_samples/raw_samplesheet_novaseq.json
--rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/demultiplexing/runParameters_missing_flowcell_run_field.xml
--rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/demultiplexing/unknown_run_parameters.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/fixtures/apps/fluffy/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/fixtures/apps/fluffy/2020-23219-05/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/fluffy/2020-23219-05/2020-23219-05.WCXpredict_aberrations.filt.bed
--rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/fluffy/SampleSheet.csv
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/fluffy/deliverables.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/fluffy/fluffy_fastq.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/fluffy/multiqc_report.html
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/fluffy/summary.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/fixtures/apps/gt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/gt/yellowhog.bcf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/fixtures/apps/madeline/
--rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/madeline/madeline.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/fixtures/apps/mip/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/mip/case_file.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/mip/case_metrics_deliverables.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/fixtures/apps/mip/dna/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/fixtures/apps/mip/dna/store/
--rw-r--r--   0 runner    (1001) docker     (123)    21811 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/mip/dna/store/case_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    23364 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/mip/dna/store/case_id_deliverables.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    37367 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/mip/dna/store/case_qc_sample_info.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/mip/dna/store/empty_case_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/mip/dna/store/empty_case_metrics_deliverables.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/mip/dna/store/empty_case_qc_sample_info.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/mip/dna/store/empty_delivery_report.html
--rw-r--r--   0 runner    (1001) docker     (123)    62741 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/mip/dna/store/yellowhog_clinical_selected.vcf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/fixtures/apps/mip/rna/
--rw-r--r--   0 runner    (1001) docker     (123)    11242 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/mip/rna/case_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    12164 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/mip/rna/case_qc_sampleinfo.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/fixtures/apps/mip/rna/store/
--rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/mip/rna/store/bundle_data.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     9774 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/mip/rna/store/case_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/mip/rna/store/case_id_deliverables.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13666 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/mip/rna/store/case_qc_sample_info.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/mip/sample_file.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/fixtures/apps/scout/
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/scout/643594.config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/scout/case_export.json
--rw-r--r--   0 runner    (1001) docker     (123)     9349 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/scout/export_causatives.json
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/scout/none_case_export.json
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/scout/other_sex_case.json
--rw-r--r--   0 runner    (1001) docker     (123)     8874 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/scout/panel_export.bed
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/scout/panel_export.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/fixtures/apps/sequencing_metrics_parser/
--rw-r--r--   0 runner    (1001) docker     (123)    63569 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/sequencing_metrics_parser/Adapter_Metrics.csv
--rw-r--r--   0 runner    (1001) docker     (123)    42478 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/sequencing_metrics_parser/Demultiplex_Stats.csv
--rw-r--r--   0 runner    (1001) docker     (123)    69862 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/sequencing_metrics_parser/Quality_Metrics.csv
--rw-r--r--   0 runner    (1001) docker     (123)     8623 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/sequencing_metrics_parser/RunInfo.xml
--rw-r--r--   0 runner    (1001) docker     (123)    42872 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/sequencing_metrics_parser/SampleSheet.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/fixtures/apps/shipping/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/apps/shipping/scout-deploy.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/fixtures/cgweb_orders/
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/cgweb_orders/balsamic.json
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/cgweb_orders/fastq.json
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/cgweb_orders/metagenome.json
--rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/cgweb_orders/microsalt.json
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/cgweb_orders/mip.json
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/cgweb_orders/mip_rna.json
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/cgweb_orders/rml.json
--rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/cgweb_orders/sarscov2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/fixtures/data/
--rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/data/SampleSheet.csv
--rw-r--r--   0 runner    (1001) docker     (123)   258048 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/data/cgfixture.db
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/data/fastq.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)    49152 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/data/hkstore.db
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/fixtures/data/yellowhog/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/data/yellowhog/pedigree.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/fixtures/io/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/io/example_csv.csv
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/io/example_json.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/fixtures/orderforms/
--rw-r--r--   0 runner    (1001) docker     (123)   257271 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/orderforms/1508.27.balsamic.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   256694 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/orderforms/1508.27.balsamic_qc.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   257319 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/orderforms/1508.27.balsamic_umi.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   256733 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/orderforms/1508.27.fastq.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   257317 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/orderforms/1508.27.mip.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   257230 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/orderforms/1508.27.mip_rna.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    95490 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/orderforms/1603.11.microbial.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   158941 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/orderforms/1604.15.rml.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    88438 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/orderforms/1605.10.metagenome.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   228196 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/orderforms/2184.7.sarscov2.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    18639 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/orderforms/NIPT-json.json
--rw-r--r--   0 runner    (1001) docker     (123)     6052 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/orderforms/balsamic_uploaded_json_orderform.json
--rw-r--r--   0 runner    (1001) docker     (123)     6611 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/orderforms/mip_uploaded_json_orderform.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/fixtures/report/
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/report/case_data.json
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/report/lims_exported_samples.json
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-26 12:06:07.000000 cg-32.2.4/tests/fixtures/report/lims_family.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/io/
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-05-26 12:06:07.000000 cg-32.2.4/tests/io/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7743 2023-05-26 12:06:07.000000 cg-32.2.4/tests/io/test_io_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-26 12:06:07.000000 cg-32.2.4/tests/io/test_io_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-05-26 12:06:07.000000 cg-32.2.4/tests/io/test_io_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-05-26 12:06:07.000000 cg-32.2.4/tests/io/test_io_yaml.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-05-26 12:06:07.000000 cg-32.2.4/tests/io/test_validate_path.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/meta/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/tests/meta/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/meta/archive/
--rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-05-26 12:06:07.000000 cg-32.2.4/tests/meta/archive/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    12864 2023-05-26 12:06:07.000000 cg-32.2.4/tests/meta/archive/test_archiving.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/meta/backup/
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-26 12:06:07.000000 cg-32.2.4/tests/meta/backup/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    24493 2023-05-26 12:06:07.000000 cg-32.2.4/tests/meta/backup/test_meta_backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-05-26 12:06:07.000000 cg-32.2.4/tests/meta/backup/test_meta_pdc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/meta/clean/
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-05-26 12:06:07.000000 cg-32.2.4/tests/meta/clean/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-05-26 12:06:07.000000 cg-32.2.4/tests/meta/clean/test_clean_demultiplexed_runs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-05-26 12:06:07.000000 cg-32.2.4/tests/meta/clean/test_clean_flow_cell_run_directories.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/meta/compress/
--rw-r--r--   0 runner    (1001) docker     (123)     7793 2023-05-26 12:06:07.000000 cg-32.2.4/tests/meta/compress/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7115 2023-05-26 12:06:07.000000 cg-32.2.4/tests/meta/compress/test_clean_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-05-26 12:06:07.000000 cg-32.2.4/tests/meta/compress/test_compress_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-05-26 12:06:07.000000 cg-32.2.4/tests/meta/compress/test_compress_meta_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-26 12:06:07.000000 cg-32.2.4/tests/meta/compress/test_decompress_spring_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-05-26 12:06:07.000000 cg-32.2.4/tests/meta/compress/test_meta_compress_update_hk.py
--rw-r--r--   0 runner    (1001) docker     (123)     9965 2023-05-26 12:06:07.000000 cg-32.2.4/tests/meta/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/meta/deliver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/tests/meta/deliver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-05-26 12:06:07.000000 cg-32.2.4/tests/meta/deliver/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8874 2023-05-26 12:06:07.000000 cg-32.2.4/tests/meta/deliver/test_deliver_ticket.py
--rw-r--r--   0 runner    (1001) docker     (123)    10178 2023-05-26 12:06:07.000000 cg-32.2.4/tests/meta/deliver/test_delivery_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/meta/demultiplex/
--rw-r--r--   0 runner    (1001) docker     (123)    11200 2023-05-26 12:06:07.000000 cg-32.2.4/tests/meta/demultiplex/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    13452 2023-05-26 12:06:07.000000 cg-32.2.4/tests/meta/demultiplex/test_delete_demultiplex_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    14245 2023-05-26 12:06:07.000000 cg-32.2.4/tests/meta/demultiplex/test_demux_post_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-26 12:06:07.000000 cg-32.2.4/tests/meta/demultiplex/test_rename_files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/meta/encryption/
--rw-r--r--   0 runner    (1001) docker     (123)     6011 2023-05-26 12:06:07.000000 cg-32.2.4/tests/meta/encryption/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    12823 2023-05-26 12:06:07.000000 cg-32.2.4/tests/meta/encryption/test_encryption.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/meta/observations/
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-05-26 12:06:07.000000 cg-32.2.4/tests/meta/observations/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    16497 2023-05-26 12:06:07.000000 cg-32.2.4/tests/meta/observations/test_meta_upload_observations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/meta/orders/
--rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-05-26 12:06:07.000000 cg-32.2.4/tests/meta/orders/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-05-26 12:06:07.000000 cg-32.2.4/tests/meta/orders/test_PoolSubmitter_validate_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-26 12:06:07.000000 cg-32.2.4/tests/meta/orders/test_SarsCov2Submitter_order_to_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-05-26 12:06:07.000000 cg-32.2.4/tests/meta/orders/test_SarsCov2Submitter_store_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-05-26 12:06:07.000000 cg-32.2.4/tests/meta/orders/test_SarsCov2Submitter_validate_order.py
--rw-r--r--   0 runner    (1001) docker     (123)    19748 2023-05-26 12:06:07.000000 cg-32.2.4/tests/meta/orders/test_meta_orders_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7123 2023-05-26 12:06:07.000000 cg-32.2.4/tests/meta/orders/test_meta_orders_lims.py
--rw-r--r--   0 runner    (1001) docker     (123)    29645 2023-05-26 12:06:07.000000 cg-32.2.4/tests/meta/orders/test_meta_orders_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-26 12:06:07.000000 cg-32.2.4/tests/meta/orders/test_ticket_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/meta/report/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/tests/meta/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-05-26 12:06:07.000000 cg-32.2.4/tests/meta/report/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-26 12:06:07.000000 cg-32.2.4/tests/meta/report/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-05-26 12:06:07.000000 cg-32.2.4/tests/meta/report/test_balsamic_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-05-26 12:06:07.000000 cg-32.2.4/tests/meta/report/test_field_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-05-26 12:06:07.000000 cg-32.2.4/tests/meta/report/test_mip_dna_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    13311 2023-05-26 12:06:07.000000 cg-32.2.4/tests/meta/report/test_report_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/meta/rsync/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/tests/meta/rsync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-26 12:06:07.000000 cg-32.2.4/tests/meta/rsync/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8811 2023-05-26 12:06:07.000000 cg-32.2.4/tests/meta/rsync/test_rsync.py
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-05-26 12:06:07.000000 cg-32.2.4/tests/meta/test_invoice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/meta/transfer/
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-05-26 12:06:07.000000 cg-32.2.4/tests/meta/transfer/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    10019 2023-05-26 12:06:07.000000 cg-32.2.4/tests/meta/transfer/test_external_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    16507 2023-05-26 12:06:07.000000 cg-32.2.4/tests/meta/transfer/test_meta_transfer_flowcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-05-26 12:06:07.000000 cg-32.2.4/tests/meta/transfer/test_meta_transfer_lims.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/meta/upload/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/tests/meta/upload/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/meta/upload/balsamic/
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-05-26 12:06:07.000000 cg-32.2.4/tests/meta/upload/balsamic/test_balsamic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-05-26 12:06:07.000000 cg-32.2.4/tests/meta/upload/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/meta/upload/gisaid/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/tests/meta/upload/gisaid/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/meta/upload/gisaid/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-26 12:06:07.000000 cg-32.2.4/tests/meta/upload/gisaid/fixtures/four_samples.csv
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/tests/meta/upload/gisaid/fixtures/invalid_housekeeper.fasta
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-26 12:06:07.000000 cg-32.2.4/tests/meta/upload/gisaid/fixtures/valid_gisaid.fasta
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-26 12:06:07.000000 cg-32.2.4/tests/meta/upload/gisaid/fixtures/valid_housekeeper.fasta
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/meta/upload/mutacc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/tests/meta/upload/mutacc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-05-26 12:06:07.000000 cg-32.2.4/tests/meta/upload/mutacc/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-05-26 12:06:07.000000 cg-32.2.4/tests/meta/upload/mutacc/test_meta_upload_mutacc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/meta/upload/nipt/
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-05-26 12:06:07.000000 cg-32.2.4/tests/meta/upload/nipt/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-26 12:06:07.000000 cg-32.2.4/tests/meta/upload/nipt/test_nipt_upload_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/meta/upload/scout/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/tests/meta/upload/scout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23429 2023-05-26 12:06:07.000000 cg-32.2.4/tests/meta/upload/scout/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-05-26 12:06:07.000000 cg-32.2.4/tests/meta/upload/scout/test_generate_load_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-05-26 12:06:07.000000 cg-32.2.4/tests/meta/upload/scout/test_meta_upload_scoutapi.py
--rw-r--r--   0 runner    (1001) docker     (123)    32103 2023-05-26 12:06:07.000000 cg-32.2.4/tests/meta/upload/scout/test_meta_upload_scoutapi_rna.py
--rw-r--r--   0 runner    (1001) docker     (123)     7857 2023-05-26 12:06:07.000000 cg-32.2.4/tests/meta/upload/scout/test_scout_config_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-05-26 12:06:07.000000 cg-32.2.4/tests/meta/upload/test_meta_upload_coverage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-05-26 12:06:07.000000 cg-32.2.4/tests/meta/upload/test_upload_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-05-26 12:06:07.000000 cg-32.2.4/tests/meta/upload/test_upload_genotypes_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/meta/upload/vogue/
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-05-26 12:06:07.000000 cg-32.2.4/tests/meta/upload/vogue/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-05-26 12:06:07.000000 cg-32.2.4/tests/meta/upload/vogue/test_upload_vogue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/meta/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/tests/meta/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6953 2023-05-26 12:06:07.000000 cg-32.2.4/tests/meta/workflow/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-05-26 12:06:07.000000 cg-32.2.4/tests/meta/workflow/test_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-05-26 12:06:07.000000 cg-32.2.4/tests/meta/workflow/test_balsamic.py
--rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-05-26 12:06:07.000000 cg-32.2.4/tests/meta/workflow/test_microsalt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-05-26 12:06:07.000000 cg-32.2.4/tests/meta/workflow/test_prepare_fastq_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/mocks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/tests/mocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-26 12:06:07.000000 cg-32.2.4/tests/mocks/balsamic_analysis_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-05-26 12:06:07.000000 cg-32.2.4/tests/mocks/crunchy.py
--rw-r--r--   0 runner    (1001) docker     (123)    20596 2023-05-26 12:06:07.000000 cg-32.2.4/tests/mocks/hk_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-05-26 12:06:07.000000 cg-32.2.4/tests/mocks/limsmock.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-26 12:06:07.000000 cg-32.2.4/tests/mocks/madeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-05-26 12:06:07.000000 cg-32.2.4/tests/mocks/mip_analysis_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-26 12:06:07.000000 cg-32.2.4/tests/mocks/osticket.py
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-05-26 12:06:07.000000 cg-32.2.4/tests/mocks/process_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-05-26 12:06:07.000000 cg-32.2.4/tests/mocks/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-05-26 12:06:07.000000 cg-32.2.4/tests/mocks/scout.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-26 12:06:07.000000 cg-32.2.4/tests/mocks/store_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-26 12:06:07.000000 cg-32.2.4/tests/mocks/tb_mock.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/tests/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/models/balsamic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/tests/models/balsamic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-26 12:06:07.000000 cg-32.2.4/tests/models/balsamic/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-26 12:06:07.000000 cg-32.2.4/tests/models/balsamic/test_balsamic_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-26 12:06:07.000000 cg-32.2.4/tests/models/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/models/demultiplexing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/tests/models/demultiplexing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-26 12:06:07.000000 cg-32.2.4/tests/models/demultiplexing/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-26 12:06:07.000000 cg-32.2.4/tests/models/demultiplexing/test_demux_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-05-26 12:06:07.000000 cg-32.2.4/tests/models/demultiplexing/test_flowcell_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4894 2023-05-26 12:06:07.000000 cg-32.2.4/tests/models/demultiplexing/test_run_parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/models/mip/
--rw-r--r--   0 runner    (1001) docker     (123)     6707 2023-05-26 12:06:07.000000 cg-32.2.4/tests/models/mip/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-26 12:06:07.000000 cg-32.2.4/tests/models/mip/test_mip_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-05-26 12:06:07.000000 cg-32.2.4/tests/models/mip/test_mip_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-05-26 12:06:07.000000 cg-32.2.4/tests/models/mip/test_mip_metrics_deliverables.py
--rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-05-26 12:06:07.000000 cg-32.2.4/tests/models/mip/test_mip_sample_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/models/nextflow/
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-26 12:06:07.000000 cg-32.2.4/tests/models/nextflow/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-26 12:06:07.000000 cg-32.2.4/tests/models/nextflow/test_nextflow_deliver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/models/observations/
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-26 12:06:07.000000 cg-32.2.4/tests/models/observations/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-05-26 12:06:07.000000 cg-32.2.4/tests/models/observations/test_observations_input_files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/models/report/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/tests/models/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-05-26 12:06:07.000000 cg-32.2.4/tests/models/report/test_validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/models/rnafusion/
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-05-26 12:06:07.000000 cg-32.2.4/tests/models/rnafusion/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-05-26 12:06:07.000000 cg-32.2.4/tests/models/rnafusion/test_rnafusion_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-26 12:06:07.000000 cg-32.2.4/tests/models/test_cg_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-26 12:06:07.000000 cg-32.2.4/tests/models/test_compression_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-05-26 12:06:07.000000 cg-32.2.4/tests/models/test_file_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-26 12:06:07.000000 cg-32.2.4/tests/models/test_flowcell_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/server/
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-26 12:06:07.000000 cg-32.2.4/tests/server/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-26 12:06:07.000000 cg-32.2.4/tests/server/test_server_app.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-26 12:06:07.000000 cg-32.2.4/tests/server/test_server_auto.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-26 12:06:07.000000 cg-32.2.4/tests/small_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/store/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/tests/store/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/store/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/tests/store/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/store/api/add/
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-05-26 12:06:07.000000 cg-32.2.4/tests/store/api/add/test_store_add_application_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-05-26 12:06:07.000000 cg-32.2.4/tests/store/api/add/test_store_add_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-05-26 12:06:07.000000 cg-32.2.4/tests/store/api/add/test_store_add_customer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-05-26 12:06:07.000000 cg-32.2.4/tests/store/api/add/test_store_add_flow_celll.py
--rw-r--r--   0 runner    (1001) docker     (123)    17919 2023-05-26 12:06:07.000000 cg-32.2.4/tests/store/api/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/store/api/delete/
--rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-05-26 12:06:07.000000 cg-32.2.4/tests/store/api/delete/test_store_api_delete.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/store/api/find/
--rw-r--r--   0 runner    (1001) docker     (123)    10138 2023-05-26 12:06:07.000000 cg-32.2.4/tests/store/api/find/test_find_basic_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-05-26 12:06:07.000000 cg-32.2.4/tests/store/api/find/test_find_basic_data_application_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    30667 2023-05-26 12:06:07.000000 cg-32.2.4/tests/store/api/find/test_find_business_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5488 2023-05-26 12:06:07.000000 cg-32.2.4/tests/store/api/find/test_find_business_data_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-05-26 12:06:07.000000 cg-32.2.4/tests/store/api/find/test_find_business_data_case.py
--rw-r--r--   0 runner    (1001) docker     (123)    14143 2023-05-26 12:06:07.000000 cg-32.2.4/tests/store/api/find/test_find_business_data_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/store/api/status/
--rw-r--r--   0 runner    (1001) docker     (123)     5019 2023-05-26 12:06:07.000000 cg-32.2.4/tests/store/api/status/test_analyses_to_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-05-26 12:06:07.000000 cg-32.2.4/tests/store/api/status/test_analyses_to_delivery_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     9780 2023-05-26 12:06:07.000000 cg-32.2.4/tests/store/api/status/test_store_api_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    15265 2023-05-26 12:06:07.000000 cg-32.2.4/tests/store/api/status/test_store_api_status_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    54170 2023-05-26 12:06:07.000000 cg-32.2.4/tests/store/api/status/test_store_api_status_cases.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-26 12:06:07.000000 cg-32.2.4/tests/store/api/status/test_store_api_status_customer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-26 12:06:07.000000 cg-32.2.4/tests/store/api/status/test_store_api_status_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     8763 2023-05-26 12:06:07.000000 cg-32.2.4/tests/store/api/status/test_store_api_status_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-05-26 12:06:07.000000 cg-32.2.4/tests/store/api/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    16197 2023-05-26 12:06:07.000000 cg-32.2.4/tests/store/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/store/filters/
--rw-r--r--   0 runner    (1001) docker     (123)    15180 2023-05-26 12:06:07.000000 cg-32.2.4/tests/store/filters/test_status_analyses_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-05-26 12:06:07.000000 cg-32.2.4/tests/store/filters/test_status_application_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    13358 2023-05-26 12:06:07.000000 cg-32.2.4/tests/store/filters/test_status_application_version_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-05-26 12:06:07.000000 cg-32.2.4/tests/store/filters/test_status_bed_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-05-26 12:06:07.000000 cg-32.2.4/tests/store/filters/test_status_bed_version_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5146 2023-05-26 12:06:07.000000 cg-32.2.4/tests/store/filters/test_status_case_sample_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    39481 2023-05-26 12:06:07.000000 cg-32.2.4/tests/store/filters/test_status_cases_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-26 12:06:07.000000 cg-32.2.4/tests/store/filters/test_status_collaboration_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-05-26 12:06:07.000000 cg-32.2.4/tests/store/filters/test_status_customer_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-05-26 12:06:07.000000 cg-32.2.4/tests/store/filters/test_status_flow_cell_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-05-26 12:06:07.000000 cg-32.2.4/tests/store/filters/test_status_invoice_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-05-26 12:06:07.000000 cg-32.2.4/tests/store/filters/test_status_organism_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-26 12:06:07.000000 cg-32.2.4/tests/store/filters/test_status_panel_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     9637 2023-05-26 12:06:07.000000 cg-32.2.4/tests/store/filters/test_status_pool_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    25770 2023-05-26 12:06:07.000000 cg-32.2.4/tests/store/filters/test_status_samples_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-26 12:06:07.000000 cg-32.2.4/tests/store/filters/test_status_user_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-05-26 12:06:07.000000 cg-32.2.4/tests/store/test_delivery.py
--rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-05-26 12:06:07.000000 cg-32.2.4/tests/store/test_store_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    30278 2023-05-26 12:06:07.000000 cg-32.2.4/tests/store_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-26 12:06:07.000000 cg-32.2.4/tests/test_store_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/tests/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/tests/fixtures/apps/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/tests/fixtures/apps/demultiplexing/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/tests/fixtures/apps/demultiplexing/flowcell-runs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/tests/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/copycomplete.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/tests/fixtures/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/tests/tests/fixtures/data/fastq.fastq.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:16.000000 cg-32.2.4/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:06:07.000000 cg-32.2.4/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-26 12:06:07.000000 cg-32.2.4/tests/utils/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-05-26 12:06:07.000000 cg-32.2.4/tests/utils/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-26 12:06:07.000000 cg-32.2.4/tests/utils/test_date.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-05-26 12:06:07.000000 cg-32.2.4/tests/utils/test_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-05-26 12:06:07.000000 cg-32.2.4/tests/utils/test_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-26 12:06:07.000000 cg-32.2.4/tests/utils/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-27 11:20:49.000000 cg-32.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-05-27 11:20:57.000000 cg-32.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-05-27 11:20:49.000000 cg-32.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-27 11:20:49.000000 cg-32.2.5/cg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/apps/cgstats/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/cgstats/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/apps/cgstats/crud/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/cgstats/crud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15866 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/cgstats/crud/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/cgstats/crud/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8001 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/cgstats/crud/find.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/apps/cgstats/db/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/cgstats/db/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/apps/cgstats/db/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/cgstats/db/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/cgstats/db/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/cgstats/db/models/datasource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/cgstats/db/models/demux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/cgstats/db/models/demux_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/cgstats/db/models/dragen_demux_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/cgstats/db/models/flowcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/cgstats/db/models/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/cgstats/db/models/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/cgstats/db/models/support_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/cgstats/db/models/unaligned.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/cgstats/db/models/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/apps/cgstats/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/cgstats/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/cgstats/parsers/adapter_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11317 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/cgstats/parsers/conversion_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/cgstats/parsers/demux_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/cgstats/parsers/dragen_demultiplexing_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/cgstats/parsers/quality_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/cgstats/parsers/run_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6315 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/cgstats/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/apps/coverage/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/coverage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/coverage/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/apps/crunchy/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/crunchy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12884 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/crunchy/crunchy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/crunchy/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/crunchy/sbatch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/apps/demultiplex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/demultiplex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11469 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/demultiplex/demultiplex_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/demultiplex/demux_report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/apps/demultiplex/sample_sheet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/demultiplex/sample_sheet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/demultiplex/sample_sheet/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/demultiplex/sample_sheet/dummy_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5171 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/demultiplex/sample_sheet/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/demultiplex/sample_sheet/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5802 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/demultiplex/sample_sheet/novaseq_sample_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/demultiplex/sample_sheet/validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/demultiplex/sbatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/environ.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/gens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/gt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/apps/hermes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/hermes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/hermes/hermes_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/hermes/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/apps/housekeeper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/housekeeper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17304 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/housekeeper/hk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/housekeeper/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/apps/invoice/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/invoice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/invoice/render.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/apps/invoice/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)   113439 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/invoice/templates/KI_pool_invoice.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    81032 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/invoice/templates/KI_sample_invoice.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   113363 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/invoice/templates/KTH_pool_invoice.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    80886 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/invoice/templates/KTH_sample_invoice.xlsx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/apps/lims/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/lims/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16393 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/lims/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/lims/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8243 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/lims/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/lims/samplesheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/loqus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/apps/madeline/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/madeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/madeline/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/apps/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/mip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/mip/confighandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/mutacc_auto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/apps/orderform/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/orderform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9233 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/orderform/excel_orderform_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/orderform/json_orderform_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6387 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/orderform/orderform_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/osticket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/apps/scout/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/scout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/scout/scout_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9438 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/scout/scoutapi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/apps/sequencing_metrics_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/sequencing_metrics_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/sequencing_metrics_parser/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/apps/sequencing_metrics_parser/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/sequencing_metrics_parser/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/sequencing_metrics_parser/models/bcl2fastq_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/sequencing_metrics_parser/models/bcl_convert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/apps/sequencing_metrics_parser/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/sequencing_metrics_parser/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/sequencing_metrics_parser/parsers/bcl2fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/sequencing_metrics_parser/parsers/bcl2fastq_to_sequencing_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7657 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/sequencing_metrics_parser/parsers/bcl_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/sequencing_metrics_parser/parsers/bcl_convert_to_sequencing_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/sequencing_metrics_parser/sequencing_metrics_calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/apps/slurm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/slurm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/slurm/sbatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/slurm/slurm_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/apps/tb/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/tb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7646 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/tb/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/tb/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-05-27 11:20:49.000000 cg-32.2.5/cg/apps/vogue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10329 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7057 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19665 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/clean.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/cli/compress/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/compress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/compress/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6669 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/compress/fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8507 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/compress/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/cli/delete/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/delete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/delete/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/delete/case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/delete/cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/delete/observations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/cli/deliver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/deliver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/deliver/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/cli/demultiplex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/demultiplex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/demultiplex/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/demultiplex/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7354 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/demultiplex/demux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/demultiplex/finish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/demultiplex/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/demultiplex/sample_sheet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/cli/generate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/generate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/generate/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/cli/generate/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/generate/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/generate/report/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/generate/report/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/generate/report/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8386 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/cli/set/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/set/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9868 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/set/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/set/case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/set/cases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/cli/store/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/store/fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/store/store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/transfer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/cli/upload/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/upload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/upload/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/upload/clinical_delivery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/upload/coverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/upload/delivery_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/upload/fohm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/upload/genotype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/upload/gens.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/upload/gisaid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/upload/mutacc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/cli/upload/nipt/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/upload/nipt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/upload/nipt/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/upload/nipt/ftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/upload/nipt/statina.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/cli/upload/observations/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/upload/observations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/upload/observations/observations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/upload/observations/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9563 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/upload/scout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/upload/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/upload/validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11932 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/upload/vogue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/cli/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/workflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/cli/workflow/balsamic/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/workflow/balsamic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8860 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/workflow/balsamic/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/workflow/balsamic/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/workflow/balsamic/pon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/workflow/balsamic/qc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/workflow/balsamic/umi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/workflow/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12622 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/workflow/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/cli/workflow/fastq/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/workflow/fastq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/workflow/fastq/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/cli/workflow/fluffy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/workflow/fluffy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/workflow/fluffy/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/cli/workflow/microsalt/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/workflow/microsalt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11101 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/workflow/microsalt/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/cli/workflow/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/workflow/mip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6224 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/workflow/mip/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/workflow/mip/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/cli/workflow/mip_dna/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/workflow/mip_dna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/workflow/mip_dna/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/cli/workflow/mip_rna/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/workflow/mip_rna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/workflow/mip_rna/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/cli/workflow/mutant/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/workflow/mutant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/workflow/mutant/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/cli/workflow/nextflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/workflow/nextflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/workflow/nextflow/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/cli/workflow/rnafusion/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/workflow/rnafusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12229 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/workflow/rnafusion/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/workflow/rnafusion/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/cli/workflow/taxprofiler/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/workflow/taxprofiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/workflow/taxprofiler/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/cli/workflow/tower/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/workflow/tower/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-27 11:20:49.000000 cg-32.2.5/cg/cli/workflow/tower/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/constants/
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-05-27 11:20:49.000000 cg-32.2.5/cg/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-27 11:20:49.000000 cg-32.2.5/cg/constants/backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-27 11:20:49.000000 cg-32.2.5/cg/constants/bcl_convert_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-27 11:20:49.000000 cg-32.2.5/cg/constants/cgstats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-05-27 11:20:49.000000 cg-32.2.5/cg/constants/compression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-05-27 11:20:49.000000 cg-32.2.5/cg/constants/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-05-27 11:20:49.000000 cg-32.2.5/cg/constants/delivery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-05-27 11:20:49.000000 cg-32.2.5/cg/constants/demultiplexing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-27 11:20:49.000000 cg-32.2.5/cg/constants/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-27 11:20:49.000000 cg-32.2.5/cg/constants/extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-27 11:20:49.000000 cg-32.2.5/cg/constants/gene_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-05-27 11:20:49.000000 cg-32.2.5/cg/constants/housekeeper_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-27 11:20:49.000000 cg-32.2.5/cg/constants/indexes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-27 11:20:49.000000 cg-32.2.5/cg/constants/invoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-05-27 11:20:49.000000 cg-32.2.5/cg/constants/lims.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-27 11:20:49.000000 cg-32.2.5/cg/constants/nextflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-27 11:20:49.000000 cg-32.2.5/cg/constants/nipt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-05-27 11:20:49.000000 cg-32.2.5/cg/constants/observations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-27 11:20:49.000000 cg-32.2.5/cg/constants/orderforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-27 11:20:49.000000 cg-32.2.5/cg/constants/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-27 11:20:49.000000 cg-32.2.5/cg/constants/pdc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-27 11:20:49.000000 cg-32.2.5/cg/constants/pedigree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-27 11:20:49.000000 cg-32.2.5/cg/constants/priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-27 11:20:49.000000 cg-32.2.5/cg/constants/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-05-27 11:20:49.000000 cg-32.2.5/cg/constants/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-27 11:20:49.000000 cg-32.2.5/cg/constants/rnafusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-27 11:20:49.000000 cg-32.2.5/cg/constants/sample_sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-05-27 11:20:49.000000 cg-32.2.5/cg/constants/scout_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-05-27 11:20:49.000000 cg-32.2.5/cg/constants/sequencing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-27 11:20:49.000000 cg-32.2.5/cg/constants/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-27 11:20:49.000000 cg-32.2.5/cg/constants/subject.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-27 11:20:49.000000 cg-32.2.5/cg/constants/symbols.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-27 11:20:49.000000 cg-32.2.5/cg/constants/tb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-05-27 11:20:49.000000 cg-32.2.5/cg/exc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-27 11:20:49.000000 cg-32.2.5/cg/io/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-27 11:20:49.000000 cg-32.2.5/cg/io/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-05-27 11:20:49.000000 cg-32.2.5/cg/io/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-27 11:20:49.000000 cg-32.2.5/cg/io/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-27 11:20:49.000000 cg-32.2.5/cg/io/validate_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-27 11:20:49.000000 cg-32.2.5/cg/io/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/meta/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/archive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8577 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/archive/ddn_dataflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/meta/backup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/backup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18893 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/backup/backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/backup/pdc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/meta/clean/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/clean/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/clean/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14404 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/clean/demultiplexed_flow_cells.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/clean/flow_cell_run_directories.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/meta/compress/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/compress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12476 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/compress/compress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/compress/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13049 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/deliver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8032 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/deliver_ticket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/meta/demultiplex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/demultiplex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11077 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/demultiplex/delete_demultiplex_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15622 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/demultiplex/demux_post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/demultiplex/files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/meta/encryption/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/encryption/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10256 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/encryption/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10954 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/invoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/meta/observations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/observations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/observations/balsamic_observations_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/observations/mip_dna_observations_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5463 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/observations/observations_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/meta/orders/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/orders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/orders/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/orders/balsamic_qc_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/orders/balsamic_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/orders/balsamic_umi_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15376 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/orders/case_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/orders/fastq_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/orders/fluffy_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/orders/lims.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/orders/metagenome_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/orders/microbial_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/orders/microsalt_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/orders/mip_dna_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/orders/mip_rna_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/orders/pool_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/orders/rml_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/orders/sars_cov_2_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/orders/submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/orders/ticket_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/meta/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9732 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/report/balsamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/report/balsamic_umi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/report/field_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7012 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/report/mip_dna.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17821 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/report/report_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/meta/report/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)    78964 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/report/templates/balsamic_report.html
+-rw-r--r--   0 runner    (1001) docker     (123)   151463 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/report/templates/bootstrap.html
+-rw-r--r--   0 runner    (1001) docker     (123)    77831 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/report/templates/mip-dna_report.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/meta/rsync/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/rsync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12066 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/rsync/rsync_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/rsync/sbatch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/meta/tar/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/tar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/tar/tar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/meta/transfer/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/transfer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10070 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/transfer/external_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8417 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/transfer/flowcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6046 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/transfer/lims.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/meta/upload/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/upload/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/meta/upload/balsamic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/upload/balsamic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/upload/balsamic/balsamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/upload/coverage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/meta/upload/fohm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/upload/fohm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12140 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/upload/fohm/fohm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/meta/upload/gisaid/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/upload/gisaid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/upload/gisaid/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13572 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/upload/gisaid/gisaid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/upload/gisaid/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/upload/gt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/meta/upload/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/upload/mip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/upload/mip/mip_dna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/upload/mip/mip_rna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7308 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/upload/mutacc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/meta/upload/nipt/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/upload/nipt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/upload/nipt/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7542 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/upload/nipt/nipt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/meta/upload/rnafusion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/upload/rnafusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/upload/rnafusion/rnafusion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/meta/upload/scout/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/upload/scout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/upload/scout/balsamic_config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/upload/scout/balsamic_umi_config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/upload/scout/hk_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/upload/scout/mip_config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/upload/scout/rnafusion_config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/upload/scout/scout_config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18719 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/upload/scout/uploadscoutapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/upload/upload_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/upload/vogue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/meta/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20004 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/workflow/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26519 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/workflow/balsamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/workflow/balsamic_pon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/workflow/balsamic_qc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/workflow/balsamic_umi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10959 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/workflow/fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13390 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/workflow/fluffy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18121 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/workflow/microsalt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14033 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/workflow/mip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/workflow/mip_dna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/workflow/mip_rna.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10762 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/workflow/mutant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10249 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/workflow/nextflow_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/workflow/prepare_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17110 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/workflow/rnafusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/workflow/taxprofiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-05-27 11:20:49.000000 cg-32.2.5/cg/meta/workflow/tower_common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/models/balsamic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/balsamic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/balsamic/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/balsamic/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/balsamic/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12924 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/cg_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/models/cgstats/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/cgstats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/cgstats/flowcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/cgstats/stats_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/compression_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/models/deliverables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/deliverables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/deliverables/metric_deliverables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/models/demultiplex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/demultiplex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10905 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/demultiplex/demux_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8513 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/demultiplex/flow_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/demultiplex/run_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/demultiplex/sbatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/file_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/models/invoice/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/invoice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/invoice/invoice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/models/lims/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/lims/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/lims/sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/models/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/mip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/mip/mip_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/mip/mip_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/mip/mip_metrics_deliverables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/mip/mip_sample_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/models/nextflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/nextflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/nextflow/deliverables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/nextflow/sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/models/observations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/observations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/observations/input_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/models/orders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/orders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/orders/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6002 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/orders/excel_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/orders/json_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/orders/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/orders/orderform_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/orders/sample_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9856 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/orders/samples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/models/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/report/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/report/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/report/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/report/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/models/rnafusion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/rnafusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/rnafusion/rnafusion_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/models/scout/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/scout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/scout/scout_load_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/models/slurm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/slurm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/slurm/sbatch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/models/taxprofiler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/taxprofiler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/models/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-27 11:20:49.000000 cg-32.2.5/cg/models/workflow/mutant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)    25590 2023-05-27 11:20:49.000000 cg-32.2.5/cg/resources/20181012_Indices.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-27 11:20:49.000000 cg-32.2.5/cg/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-05-27 11:20:49.000000 cg-32.2.5/cg/resources/rnafusion_bundle_filenames.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16964 2023-05-27 11:20:49.000000 cg-32.2.5/cg/server/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19037 2023-05-27 11:20:49.000000 cg-32.2.5/cg/server/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-05-27 11:20:49.000000 cg-32.2.5/cg/server/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-27 11:20:49.000000 cg-32.2.5/cg/server/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-27 11:20:49.000000 cg-32.2.5/cg/server/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-27 11:20:49.000000 cg-32.2.5/cg/server/ext.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/server/invoices/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-27 11:20:49.000000 cg-32.2.5/cg/server/invoices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/server/invoices/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/server/invoices/templates/invoices/
+-rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-05-27 11:20:49.000000 cg-32.2.5/cg/server/invoices/templates/invoices/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-05-27 11:20:49.000000 cg-32.2.5/cg/server/invoices/templates/invoices/invoice.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-05-27 11:20:49.000000 cg-32.2.5/cg/server/invoices/templates/invoices/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-05-27 11:20:49.000000 cg-32.2.5/cg/server/invoices/templates/invoices/new.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7794 2023-05-27 11:20:49.000000 cg-32.2.5/cg/server/invoices/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/server/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/server/templates/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-27 11:20:49.000000 cg-32.2.5/cg/server/templates/admin/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/store/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-27 11:20:49.000000 cg-32.2.5/cg/store/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/store/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-27 11:20:49.000000 cg-32.2.5/cg/store/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10616 2023-05-27 11:20:49.000000 cg-32.2.5/cg/store/api/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6942 2023-05-27 11:20:49.000000 cg-32.2.5/cg/store/api/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-05-27 11:20:49.000000 cg-32.2.5/cg/store/api/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-27 11:20:49.000000 cg-32.2.5/cg/store/api/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-05-27 11:20:49.000000 cg-32.2.5/cg/store/api/find_basic_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28994 2023-05-27 11:20:49.000000 cg-32.2.5/cg/store/api/find_business_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38700 2023-05-27 11:20:49.000000 cg-32.2.5/cg/store/api/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/store/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/store/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-05-27 11:20:49.000000 cg-32.2.5/cg/store/filters/status_analysis_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-27 11:20:49.000000 cg-32.2.5/cg/store/filters/status_application_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-05-27 11:20:49.000000 cg-32.2.5/cg/store/filters/status_application_version_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-27 11:20:49.000000 cg-32.2.5/cg/store/filters/status_bed_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-27 11:20:49.000000 cg-32.2.5/cg/store/filters/status_bed_version_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10388 2023-05-27 11:20:49.000000 cg-32.2.5/cg/store/filters/status_case_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-27 11:20:49.000000 cg-32.2.5/cg/store/filters/status_case_sample_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-27 11:20:49.000000 cg-32.2.5/cg/store/filters/status_collaboration_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-05-27 11:20:49.000000 cg-32.2.5/cg/store/filters/status_customer_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-27 11:20:49.000000 cg-32.2.5/cg/store/filters/status_flow_cell_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-27 11:20:49.000000 cg-32.2.5/cg/store/filters/status_invoice_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-27 11:20:49.000000 cg-32.2.5/cg/store/filters/status_organism_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-27 11:20:49.000000 cg-32.2.5/cg/store/filters/status_panel_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-05-27 11:20:49.000000 cg-32.2.5/cg/store/filters/status_pool_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8892 2023-05-27 11:20:49.000000 cg-32.2.5/cg/store/filters/status_sample_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-27 11:20:49.000000 cg-32.2.5/cg/store/filters/status_user_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29946 2023-05-27 11:20:49.000000 cg-32.2.5/cg/store/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-27 11:20:49.000000 cg-32.2.5/cg/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/utils/checksum/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/utils/checksum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-27 11:20:49.000000 cg-32.2.5/cg/utils/checksum/checksum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/utils/click/
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-27 11:20:49.000000 cg-32.2.5/cg/utils/click/EnumChoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/utils/click/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-05-27 11:20:49.000000 cg-32.2.5/cg/utils/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-05-27 11:20:49.000000 cg-32.2.5/cg/utils/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-27 11:20:49.000000 cg-32.2.5/cg/utils/dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-05-27 11:20:49.000000 cg-32.2.5/cg/utils/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-27 11:20:49.000000 cg-32.2.5/cg/utils/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-27 11:20:49.000000 cg-32.2.5/cg/utils/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-27 11:20:49.000000 cg-32.2.5/cg/utils/files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg/utils/flask/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/cg/utils/flask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-27 11:20:49.000000 cg-32.2.5/cg/utils/flask/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-27 11:20:49.000000 cg-32.2.5/cg/utils/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-27 11:20:49.000000 cg-32.2.5/cg/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/cg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-05-27 11:20:56.000000 cg-32.2.5/cg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    40436 2023-05-27 11:20:57.000000 cg-32.2.5/cg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 11:20:56.000000 cg-32.2.5/cg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-27 11:20:56.000000 cg-32.2.5/cg.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 11:20:56.000000 cg-32.2.5/cg.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-27 11:20:56.000000 cg-32.2.5/cg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-27 11:20:56.000000 cg-32.2.5/cg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-27 11:20:49.000000 cg-32.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-27 11:20:49.000000 cg-32.2.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 11:20:57.000000 cg-32.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-27 11:20:49.000000 cg-32.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/apps/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/apps/cgstats/
+-rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/cgstats/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/apps/cgstats/crud/
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/cgstats/crud/test_create_novaseq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/cgstats/crud/test_delete.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/apps/cgstats/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/cgstats/parsers/test_adapter_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/cgstats/parsers/test_conversion_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/cgstats/parsers/test_demux_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/cgstats/parsers/test_quality_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/cgstats/parsers/test_run_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/cgstats/test_cgstats_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/cgstats/test_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/apps/coverage/
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/coverage/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/coverage/test_coverage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/apps/crunchy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/crunchy/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/crunchy/test_compress_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/crunchy/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14590 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/crunchy/test_crunchy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9107 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/crunchy/test_spring_decompression.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/apps/demultiplex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/demultiplex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10019 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/demultiplex/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/demultiplex/test_convert_to_sample_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/demultiplex/test_demultiplex_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/demultiplex/test_sample_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6258 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/demultiplex/test_validate_sample_sheet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/apps/gens/
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/gens/test_gens_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/apps/gt/
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/gt/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/gt/test_gt_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/apps/hk/
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/hk/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/hk/test__getattr__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/hk/test_add_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/hk/test_bundles.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/hk/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24046 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/hk/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/hk/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/apps/lims/
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/lims/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/lims/test_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/apps/loqus/
+-rw-r--r--   0 runner    (1001) docker     (123)     9785 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/loqus/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/loqus/test_loqusdb_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/apps/madeline/
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/madeline/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/madeline/test_madeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/apps/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/mip/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/mip/test_config_mip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/apps/mutacc_auto/
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/mutacc_auto/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/mutacc_auto/test_mutacc_auto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/apps/orderform/
+-rw-r--r--   0 runner    (1001) docker     (123)    11900 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/orderform/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/orderform/test_excel_orderform_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/orderform/test_excel_sample_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/orderform/test_json_orderform_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/orderform/test_orderform_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/apps/scout/
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/scout/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/scout/test_get_causative_variants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/scout/test_get_scout_cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/scout/test_scout_load_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/scout/test_scout_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/apps/sequencing_metrics_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/sequencing_metrics_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6678 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/sequencing_metrics_parser/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/apps/sequencing_metrics_parser/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/sequencing_metrics_parser/parsers/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/sequencing_metrics_parser/parsers/test_bcl2fastq_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/sequencing_metrics_parser/parsers/test_bcl2fastq_to_sequencing_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/sequencing_metrics_parser/parsers/test_bcl_convert_to_sequencing_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10043 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/sequencing_metrics_parser/parsers/test_bclconvert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/sequencing_metrics_parser/test_sequencing_metrics_calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/apps/slurm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/slurm/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/slurm/test_slurm_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/test_apps_environ.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/test_osticket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/apps/vogue/
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/vogue/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-05-27 11:20:49.000000 cg-32.2.5/tests/apps/vogue/test_vogue_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/cli/add/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/add/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/add/test_cli_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/add/test_cli_add_customer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/add/test_cli_add_family.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7565 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/add/test_cli_add_relationship.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/add/test_cli_add_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/cli/backup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/backup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/backup/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/backup/test_backup_command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/cli/clean/
+-rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/clean/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5535 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/clean/test_balsamic_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/clean/test_clean_hk_bundle_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/clean/test_hk_bundle_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/clean/test_hk_case_bundle_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/clean/test_microbial_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/clean/test_rsync_past_run_dirs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/cli/compress/
+-rw-r--r--   0 runner    (1001) docker     (123)    10311 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/compress/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6929 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/compress/test_cli_compress_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/compress/test_cli_decompress_spring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/compress/test_compress_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/compress/test_store_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/cli/delete/
+-rw-r--r--   0 runner    (1001) docker     (123)    12781 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/delete/test_cli_delete_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/delete/test_cli_delete_cases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/cli/deliver/
+-rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/deliver/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/deliver/test_deliver_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/deliver/test_rsync_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8562 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/deliver/test_run_deliver_cmd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/cli/demultiplex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/demultiplex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11372 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/demultiplex/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/demultiplex/test_add_flowcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4175 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/demultiplex/test_create_sample_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11412 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/demultiplex/test_demultiplex_flowcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/demultiplex/test_finish_demux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/demultiplex/test_stats_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/demultiplex/test_validate_sample_sheet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/cli/generate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/generate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/cli/generate/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/generate/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/generate/report/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/generate/report/test_cli_delivery_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/generate/report/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/generate/test_cli_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/cli/get/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/get/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/get/test_cli_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/get/test_cli_get_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/get/test_cli_get_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/get/test_cli_get_flow_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8862 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/get/test_cli_get_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/cli/set/
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/set/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7320 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/set/test_cli_set_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/set/test_cli_set_cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/set/test_cli_set_flowcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/set/test_cli_set_list_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12516 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/set/test_cli_set_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/set/test_cli_set_samples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/cli/store/
+-rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/store/test_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/test_clean.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/cli/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/cli/tests/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/cli/tests/fixtures/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/tests/fixtures/data/fastq.fastq.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/cli/upload/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/upload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10414 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/upload/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/upload/test_cli_scout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/upload/test_cli_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/upload/test_cli_upload_auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/upload/test_cli_upload_delivery_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/upload/test_cli_upload_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/upload/test_cli_upload_genotype.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/upload/test_cli_upload_gens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9971 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/upload/test_cli_upload_nipt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/upload/test_cli_upload_nipt_ftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/upload/test_cli_upload_nipt_statina.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5963 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/upload/test_cli_upload_observations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/upload/test_cli_upload_vogue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/cli/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/cli/workflow/balsamic/
+-rw-r--r--   0 runner    (1001) docker     (123)    30801 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/balsamic/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15328 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/balsamic/test_cli_balsamic_config_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/balsamic/test_compound_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/balsamic/test_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/balsamic/test_report_deliver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6369 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/balsamic/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/balsamic/test_store_housekeeper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7787 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/cli/workflow/fastq/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/fastq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/fastq/test_fastq_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/cli/workflow/fluffy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/fluffy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/fluffy/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/fluffy/test_cli_create_samplesheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/fluffy/test_cli_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/fluffy/test_cli_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/fluffy/test_cli_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7878 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/fluffy/test_cli_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/cli/workflow/microsalt/
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/microsalt/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/cli/workflow/microsalt/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/microsalt/snapshots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/microsalt/snapshots/snap_test_microsalt_case_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7185 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/microsalt/test_microsalt_case_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/microsalt/test_microsalt_run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/cli/workflow/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/mip/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6796 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/mip/test_cli_mip_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/mip/test_cli_mip_dna_config_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/mip/test_cli_mip_dna_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/mip/test_cli_mip_dna_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/mip/test_cli_mip_dna_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/mip/test_cli_mip_dna_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/mip/test_cli_mip_rna_config_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/mip/test_cli_mip_rna_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/mip/test_cli_mip_rna_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8558 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/mip/test_cli_mip_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/cli/workflow/rnafusion/
+-rw-r--r--   0 runner    (1001) docker     (123)     8350 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/rnafusion/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/rnafusion/test_cli_rnafusion_compound_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5254 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/rnafusion/test_cli_rnafusion_config_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/rnafusion/test_cli_rnafusion_metrics_deliver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/rnafusion/test_cli_rnafusion_report_deliver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/rnafusion/test_cli_rnafusion_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8449 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/rnafusion/test_cli_rnafusion_store_housekeeper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/cli/workflow/taxprofiler/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/taxprofiler/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/taxprofiler/test_cli_taxprofiler_compound_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/test_cli_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-05-27 11:20:49.000000 cg-32.2.5/tests/cli/workflow/test_cli_workflow_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62393 2023-05-27 11:20:49.000000 cg-32.2.5/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/DEMUX/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/ADM1136A3_XTC08_AGTGGTCA_L001_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/ADM1136A3_XTC08_AGTGGTCA_L001_R2_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/ADM1136A3_XTC08_AGTGGTCA_L002_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/ADM1136A3_XTC08_AGTGGTCA_L002_R2_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/runParameters.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/analysis/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/analysis/balsamic/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/analysis/balsamic/tn_wgs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/analysis/balsamic/tn_wgs/adm1.cram
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/analysis/balsamic/tn_wgs/ascat.output.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/analysis/balsamic/tn_wgs/snv.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/analysis/balsamic/tn_wgs/sv.vcf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/analysis/microsalt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/
+-rw-r--r--   0 runner    (1001) docker     (123)    14644 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/ACC11111_qc_fail.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/
+-rw-r--r--   0 runner    (1001) docker     (123)    15713 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/ACC22222_qc_pass.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/analysis/mip/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/analysis/mip/dna/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/analysis/mip/dna/ADM1.baf.bed.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/analysis/mip/dna/ADM1.cov.bed.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/analysis/mip/dna/ADM2.cram
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/analysis/mip/dna/ADM3.cram
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/analysis/mip/dna/adm1.cram
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/analysis/mip/dna/adm1.mt.bam
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/analysis/mip/dna/multiqc.html
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/analysis/mip/dna/report.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/analysis/mip/dna/smn.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/analysis/mip/dna/snv.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/analysis/mip/dna/snv_research.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/analysis/mip/dna/str.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/analysis/mip/dna/sv.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/analysis/mip/dna/sv_research.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/analysis/mip/dna/vcf2cytosure.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/analysis/rnafusion/
+-rw-r--r--   0 runner    (1001) docker     (123)     5587 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/analysis/rnafusion/multiqc_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/analysis/sample_coverage.bed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/apps/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/apps/balsamic/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/apps/balsamic/case/
+-rw-r--r--   0 runner    (1001) docker     (123)     9948 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/balsamic/case/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/balsamic/case/metadata.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/balsamic/case/metadata_directory.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/balsamic/case/metadata_file_tags.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/balsamic/case/metrics_deliverables.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/apps/crunchy/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/crunchy/spring_metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/
+-rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    53877 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/RunParameters_different_index_cycles.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/SampleSheetS2_Bcl2Fastq.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/SampleSheetS2_Dragen.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/HN3FKDSXY_AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/HN3FKDSXY_AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R2_001.fastq.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/
+-rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/Adapter_Metrics.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/Quality_Metrics.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/RunInfo.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/dummy_run_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/dummy_run_R1_001.fastq.gz.md5
+-rw-r--r--   0 runner    (1001) docker     (123)   338370 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R1_001.fastq.gz.md5
+-rw-r--r--   0 runner    (1001) docker     (123)   338349 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R2_001.fastq.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R2_001.fastq.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L001_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L001_R2_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L002_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L002_R2_001.fastq.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/flow-cell-runs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/flow-cell-runs/201203_A00689_0200_AHVKJCDRXX/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/flow-cell-runs/201203_A00689_0200_AHVKJCDRXX/CopyComplete.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/flow-cell-runs/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/flow-cell-runs/201203_A00689_0200_AHVKJCDRXX/RTAComplete.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/flow-cell-runs/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/flow-cell-runs/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/flow-cell-runs/201203_A00689_0200_AHVKJCDRXX/demuxstarted.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/flow-cell-runs/211101_A00187_0615_AHLG5GDRXY/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/flow-cell-runs/211101_A00187_0615_AHLG5GDRXY/CopyComplete.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/flow-cell-runs/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stderr
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/flow-cell-runs/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/flow-cell-runs/211101_A00187_0615_AHLG5GDRXY/RTAComplete.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/flow-cell-runs/211101_A00187_0615_AHLG5GDRXY/RunParameters.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/flow-cell-runs/211101_A00187_0615_AHLG5GDRXY/SampleSheet.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/flow-cell-runs/211101_A00187_0615_AHLG5GDRXY/demuxstarted.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/hiseq_run/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/hiseq_run/201203_A00689_0200_AHVKJCDRXX/
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/hiseq_run/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/hiseq_run/201203_A00689_0200_AHVKJCDRXX/RTAComplete.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/hiseq_run/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/hiseq_run/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/hiseq_run/201203_A00689_0200_AHVKJCDRXX/copycomplete.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/hiseq_run/201203_A00689_0200_AHVKJCDRXX/demuxstarted.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/hiseq_run/runParameters.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/raw_lims_samples/
+-rw-r--r--   0 runner    (1001) docker     (123)    92887 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/raw_lims_samples/raw_samplesheet_novaseq.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/runParameters_missing_flowcell_run_field.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/demultiplexing/unknown_run_parameters.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/apps/fluffy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/apps/fluffy/2020-23219-05/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/fluffy/2020-23219-05/2020-23219-05.WCXpredict_aberrations.filt.bed
+-rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/fluffy/SampleSheet.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/fluffy/deliverables.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/fluffy/fluffy_fastq.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/fluffy/multiqc_report.html
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/fluffy/summary.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/apps/gt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/gt/yellowhog.bcf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/apps/madeline/
+-rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/madeline/madeline.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/apps/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/mip/case_file.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/mip/case_metrics_deliverables.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/apps/mip/dna/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/apps/mip/dna/store/
+-rw-r--r--   0 runner    (1001) docker     (123)    21811 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/mip/dna/store/case_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    23364 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/mip/dna/store/case_id_deliverables.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    37367 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/mip/dna/store/case_qc_sample_info.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/mip/dna/store/empty_case_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/mip/dna/store/empty_case_metrics_deliverables.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/mip/dna/store/empty_case_qc_sample_info.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/mip/dna/store/empty_delivery_report.html
+-rw-r--r--   0 runner    (1001) docker     (123)    62741 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/mip/dna/store/yellowhog_clinical_selected.vcf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/apps/mip/rna/
+-rw-r--r--   0 runner    (1001) docker     (123)    11242 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/mip/rna/case_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    12164 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/mip/rna/case_qc_sampleinfo.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/apps/mip/rna/store/
+-rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/mip/rna/store/bundle_data.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9774 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/mip/rna/store/case_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/mip/rna/store/case_id_deliverables.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13666 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/mip/rna/store/case_qc_sample_info.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/mip/sample_file.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/apps/scout/
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/scout/643594.config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/scout/case_export.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9349 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/scout/export_causatives.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/scout/none_case_export.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/scout/other_sex_case.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8874 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/scout/panel_export.bed
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/scout/panel_export.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/apps/sequencing_metrics_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)    63569 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/sequencing_metrics_parser/Adapter_Metrics.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    42478 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/sequencing_metrics_parser/Demultiplex_Stats.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    69862 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/sequencing_metrics_parser/Quality_Metrics.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     8623 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/sequencing_metrics_parser/RunInfo.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    42872 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/sequencing_metrics_parser/SampleSheet.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/apps/shipping/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/apps/shipping/scout-deploy.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/cgweb_orders/
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/cgweb_orders/balsamic.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/cgweb_orders/fastq.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/cgweb_orders/metagenome.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/cgweb_orders/microsalt.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/cgweb_orders/mip.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/cgweb_orders/mip_rna.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/cgweb_orders/rml.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/cgweb_orders/sarscov2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/data/SampleSheet.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   258048 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/data/cgfixture.db
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/data/fastq.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    49152 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/data/hkstore.db
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/data/yellowhog/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/data/yellowhog/pedigree.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/io/example_csv.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/io/example_json.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/orderforms/
+-rw-r--r--   0 runner    (1001) docker     (123)   257271 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/orderforms/1508.27.balsamic.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   256694 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/orderforms/1508.27.balsamic_qc.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   257319 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/orderforms/1508.27.balsamic_umi.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   256733 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/orderforms/1508.27.fastq.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   257317 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/orderforms/1508.27.mip.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   257230 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/orderforms/1508.27.mip_rna.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    95490 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/orderforms/1603.11.microbial.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   158941 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/orderforms/1604.15.rml.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    88438 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/orderforms/1605.10.metagenome.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   228196 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/orderforms/2184.7.sarscov2.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    18639 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/orderforms/NIPT-json.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6052 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/orderforms/balsamic_uploaded_json_orderform.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6611 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/orderforms/mip_uploaded_json_orderform.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/fixtures/report/
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/report/case_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/report/lims_exported_samples.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-27 11:20:49.000000 cg-32.2.5/tests/fixtures/report/lims_family.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/io/
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-05-27 11:20:49.000000 cg-32.2.5/tests/io/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7743 2023-05-27 11:20:49.000000 cg-32.2.5/tests/io/test_io_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-27 11:20:49.000000 cg-32.2.5/tests/io/test_io_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-05-27 11:20:49.000000 cg-32.2.5/tests/io/test_io_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-05-27 11:20:49.000000 cg-32.2.5/tests/io/test_io_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-05-27 11:20:49.000000 cg-32.2.5/tests/io/test_validate_path.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/meta/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/archive/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12864 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/archive/test_archiving.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/meta/backup/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/backup/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24493 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/backup/test_meta_backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/backup/test_meta_pdc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/meta/clean/
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/clean/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/clean/test_clean_demultiplexed_runs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/clean/test_clean_flow_cell_run_directories.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/meta/compress/
+-rw-r--r--   0 runner    (1001) docker     (123)     7793 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/compress/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7115 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/compress/test_clean_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/compress/test_compress_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/compress/test_compress_meta_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/compress/test_decompress_spring_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/compress/test_meta_compress_update_hk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9965 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/meta/deliver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/deliver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/deliver/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8874 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/deliver/test_deliver_ticket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10178 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/deliver/test_delivery_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/meta/demultiplex/
+-rw-r--r--   0 runner    (1001) docker     (123)    11200 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/demultiplex/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13452 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/demultiplex/test_delete_demultiplex_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14245 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/demultiplex/test_demux_post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/demultiplex/test_rename_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/meta/encryption/
+-rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/encryption/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11132 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/encryption/test_encryption.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/meta/observations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/observations/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16497 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/observations/test_meta_upload_observations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/meta/orders/
+-rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/orders/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/orders/test_PoolSubmitter_validate_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/orders/test_SarsCov2Submitter_order_to_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/orders/test_SarsCov2Submitter_store_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/orders/test_SarsCov2Submitter_validate_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19748 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/orders/test_meta_orders_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7123 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/orders/test_meta_orders_lims.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29658 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/orders/test_meta_orders_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/orders/test_ticket_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/meta/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/report/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/report/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/report/test_balsamic_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/report/test_field_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/report/test_mip_dna_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13311 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/report/test_report_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/meta/rsync/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/rsync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/rsync/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8811 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/rsync/test_rsync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/test_invoice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/meta/transfer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/transfer/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10019 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/transfer/test_external_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16507 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/transfer/test_meta_transfer_flowcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/transfer/test_meta_transfer_lims.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/meta/upload/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/upload/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/meta/upload/balsamic/
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/upload/balsamic/test_balsamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/upload/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/meta/upload/gisaid/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/upload/gisaid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/meta/upload/gisaid/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/upload/gisaid/fixtures/four_samples.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/upload/gisaid/fixtures/invalid_housekeeper.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/upload/gisaid/fixtures/valid_gisaid.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/upload/gisaid/fixtures/valid_housekeeper.fasta
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/meta/upload/mutacc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/upload/mutacc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/upload/mutacc/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/upload/mutacc/test_meta_upload_mutacc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/meta/upload/nipt/
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/upload/nipt/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/upload/nipt/test_nipt_upload_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/meta/upload/scout/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/upload/scout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23429 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/upload/scout/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/upload/scout/test_generate_load_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/upload/scout/test_meta_upload_scoutapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32141 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/upload/scout/test_meta_upload_scoutapi_rna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7857 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/upload/scout/test_scout_config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/upload/test_meta_upload_coverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/upload/test_upload_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/upload/test_upload_genotypes_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/meta/upload/vogue/
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/upload/vogue/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/upload/vogue/test_upload_vogue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/meta/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6953 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/workflow/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/workflow/test_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/workflow/test_balsamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/workflow/test_microsalt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-05-27 11:20:49.000000 cg-32.2.5/tests/meta/workflow/test_prepare_fastq_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/mocks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/mocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-27 11:20:49.000000 cg-32.2.5/tests/mocks/balsamic_analysis_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-05-27 11:20:49.000000 cg-32.2.5/tests/mocks/crunchy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20596 2023-05-27 11:20:49.000000 cg-32.2.5/tests/mocks/hk_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-05-27 11:20:49.000000 cg-32.2.5/tests/mocks/limsmock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-27 11:20:49.000000 cg-32.2.5/tests/mocks/madeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-05-27 11:20:49.000000 cg-32.2.5/tests/mocks/mip_analysis_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-27 11:20:49.000000 cg-32.2.5/tests/mocks/osticket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-05-27 11:20:49.000000 cg-32.2.5/tests/mocks/process_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-05-27 11:20:49.000000 cg-32.2.5/tests/mocks/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-05-27 11:20:49.000000 cg-32.2.5/tests/mocks/scout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-27 11:20:49.000000 cg-32.2.5/tests/mocks/store_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-27 11:20:49.000000 cg-32.2.5/tests/mocks/tb_mock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/models/balsamic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/models/balsamic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-27 11:20:49.000000 cg-32.2.5/tests/models/balsamic/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-27 11:20:49.000000 cg-32.2.5/tests/models/balsamic/test_balsamic_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-27 11:20:49.000000 cg-32.2.5/tests/models/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/models/demultiplexing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/models/demultiplexing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-27 11:20:49.000000 cg-32.2.5/tests/models/demultiplexing/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-27 11:20:49.000000 cg-32.2.5/tests/models/demultiplexing/test_demux_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-05-27 11:20:49.000000 cg-32.2.5/tests/models/demultiplexing/test_flowcell_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4894 2023-05-27 11:20:49.000000 cg-32.2.5/tests/models/demultiplexing/test_run_parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/models/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)     6707 2023-05-27 11:20:49.000000 cg-32.2.5/tests/models/mip/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-27 11:20:49.000000 cg-32.2.5/tests/models/mip/test_mip_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-05-27 11:20:49.000000 cg-32.2.5/tests/models/mip/test_mip_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-05-27 11:20:49.000000 cg-32.2.5/tests/models/mip/test_mip_metrics_deliverables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-05-27 11:20:49.000000 cg-32.2.5/tests/models/mip/test_mip_sample_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/models/nextflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-27 11:20:49.000000 cg-32.2.5/tests/models/nextflow/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-27 11:20:49.000000 cg-32.2.5/tests/models/nextflow/test_nextflow_deliver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/models/observations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-27 11:20:49.000000 cg-32.2.5/tests/models/observations/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-05-27 11:20:49.000000 cg-32.2.5/tests/models/observations/test_observations_input_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/models/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/models/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-05-27 11:20:49.000000 cg-32.2.5/tests/models/report/test_validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/models/rnafusion/
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-05-27 11:20:49.000000 cg-32.2.5/tests/models/rnafusion/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-05-27 11:20:49.000000 cg-32.2.5/tests/models/rnafusion/test_rnafusion_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-27 11:20:49.000000 cg-32.2.5/tests/models/test_cg_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-27 11:20:49.000000 cg-32.2.5/tests/models/test_compression_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-05-27 11:20:49.000000 cg-32.2.5/tests/models/test_file_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-27 11:20:49.000000 cg-32.2.5/tests/models/test_flowcell_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/server/
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-27 11:20:49.000000 cg-32.2.5/tests/server/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-27 11:20:49.000000 cg-32.2.5/tests/server/test_server_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-27 11:20:49.000000 cg-32.2.5/tests/server/test_server_auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-27 11:20:49.000000 cg-32.2.5/tests/small_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/store/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/store/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/store/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/store/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/store/api/add/
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-27 11:20:49.000000 cg-32.2.5/tests/store/api/add/test_store_add_application_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-05-27 11:20:49.000000 cg-32.2.5/tests/store/api/add/test_store_add_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-05-27 11:20:49.000000 cg-32.2.5/tests/store/api/add/test_store_add_customer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-05-27 11:20:49.000000 cg-32.2.5/tests/store/api/add/test_store_add_flow_celll.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17674 2023-05-27 11:20:49.000000 cg-32.2.5/tests/store/api/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/store/api/delete/
+-rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-05-27 11:20:49.000000 cg-32.2.5/tests/store/api/delete/test_store_api_delete.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/store/api/find/
+-rw-r--r--   0 runner    (1001) docker     (123)     8342 2023-05-27 11:20:49.000000 cg-32.2.5/tests/store/api/find/test_find_basic_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-05-27 11:20:49.000000 cg-32.2.5/tests/store/api/find/test_find_basic_data_application_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27415 2023-05-27 11:20:49.000000 cg-32.2.5/tests/store/api/find/test_find_business_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-05-27 11:20:49.000000 cg-32.2.5/tests/store/api/find/test_find_business_data_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-05-27 11:20:49.000000 cg-32.2.5/tests/store/api/find/test_find_business_data_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12223 2023-05-27 11:20:49.000000 cg-32.2.5/tests/store/api/find/test_find_business_data_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/store/api/status/
+-rw-r--r--   0 runner    (1001) docker     (123)     5019 2023-05-27 11:20:49.000000 cg-32.2.5/tests/store/api/status/test_analyses_to_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-05-27 11:20:49.000000 cg-32.2.5/tests/store/api/status/test_analyses_to_delivery_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9780 2023-05-27 11:20:49.000000 cg-32.2.5/tests/store/api/status/test_store_api_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15265 2023-05-27 11:20:49.000000 cg-32.2.5/tests/store/api/status/test_store_api_status_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54170 2023-05-27 11:20:49.000000 cg-32.2.5/tests/store/api/status/test_store_api_status_cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-27 11:20:49.000000 cg-32.2.5/tests/store/api/status/test_store_api_status_customer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-27 11:20:49.000000 cg-32.2.5/tests/store/api/status/test_store_api_status_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8763 2023-05-27 11:20:49.000000 cg-32.2.5/tests/store/api/status/test_store_api_status_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-05-27 11:20:49.000000 cg-32.2.5/tests/store/api/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15566 2023-05-27 11:20:49.000000 cg-32.2.5/tests/store/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/store/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)    14547 2023-05-27 11:20:49.000000 cg-32.2.5/tests/store/filters/test_status_analyses_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-05-27 11:20:49.000000 cg-32.2.5/tests/store/filters/test_status_application_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10505 2023-05-27 11:20:49.000000 cg-32.2.5/tests/store/filters/test_status_application_version_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-05-27 11:20:49.000000 cg-32.2.5/tests/store/filters/test_status_bed_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-05-27 11:20:49.000000 cg-32.2.5/tests/store/filters/test_status_bed_version_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-05-27 11:20:49.000000 cg-32.2.5/tests/store/filters/test_status_case_sample_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38171 2023-05-27 11:20:49.000000 cg-32.2.5/tests/store/filters/test_status_cases_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-27 11:20:49.000000 cg-32.2.5/tests/store/filters/test_status_collaboration_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-05-27 11:20:49.000000 cg-32.2.5/tests/store/filters/test_status_customer_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-05-27 11:20:49.000000 cg-32.2.5/tests/store/filters/test_status_flow_cell_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-05-27 11:20:49.000000 cg-32.2.5/tests/store/filters/test_status_invoice_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-05-27 11:20:49.000000 cg-32.2.5/tests/store/filters/test_status_organism_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-27 11:20:49.000000 cg-32.2.5/tests/store/filters/test_status_panel_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8713 2023-05-27 11:20:49.000000 cg-32.2.5/tests/store/filters/test_status_pool_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22968 2023-05-27 11:20:49.000000 cg-32.2.5/tests/store/filters/test_status_samples_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-27 11:20:49.000000 cg-32.2.5/tests/store/filters/test_status_user_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-05-27 11:20:49.000000 cg-32.2.5/tests/store/test_delivery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-05-27 11:20:49.000000 cg-32.2.5/tests/store/test_store_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30182 2023-05-27 11:20:49.000000 cg-32.2.5/tests/store_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-27 11:20:49.000000 cg-32.2.5/tests/test_store_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/tests/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/tests/fixtures/apps/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/tests/fixtures/apps/demultiplexing/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/tests/fixtures/apps/demultiplexing/flowcell-runs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/copycomplete.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/tests/fixtures/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/tests/fixtures/data/fastq.fastq.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:57.000000 cg-32.2.5/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 11:20:49.000000 cg-32.2.5/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-27 11:20:49.000000 cg-32.2.5/tests/utils/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-05-27 11:20:49.000000 cg-32.2.5/tests/utils/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-27 11:20:49.000000 cg-32.2.5/tests/utils/test_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-05-27 11:20:49.000000 cg-32.2.5/tests/utils/test_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7176 2023-05-27 11:20:49.000000 cg-32.2.5/tests/utils/test_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-27 11:20:49.000000 cg-32.2.5/tests/utils/test_utils.py
```

### Comparing `cg-32.2.4/PKG-INFO` & `cg-32.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cg
-Version: 32.2.4
+Version: 32.2.5
 Summary: Clinical Genomics command center
 Home-page: https://github.com/Clinical-Genomics/cg
 Author: Clinical Genomics
 Author-email: support@clinicalgenomics.se
 License: UNKNOWN
 Description: 
         # cg
```

### Comparing `cg-32.2.4/README.md` & `cg-32.2.5/README.md`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/apps/cgstats/crud/create.py` & `cg-32.2.5/cg/apps/cgstats/crud/create.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/apps/cgstats/crud/delete.py` & `cg-32.2.5/cg/apps/cgstats/crud/delete.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/apps/cgstats/crud/find.py` & `cg-32.2.5/cg/apps/cgstats/crud/find.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/apps/cgstats/db/models/base.py` & `cg-32.2.5/cg/apps/cgstats/db/models/base.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/apps/cgstats/db/models/datasource.py` & `cg-32.2.5/cg/apps/cgstats/db/models/datasource.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/apps/cgstats/db/models/demux.py` & `cg-32.2.5/cg/apps/cgstats/db/models/demux.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/apps/cgstats/db/models/demux_sample.py` & `cg-32.2.5/cg/apps/cgstats/db/models/demux_sample.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/apps/cgstats/db/models/dragen_demux_sample.py` & `cg-32.2.5/cg/apps/cgstats/db/models/dragen_demux_sample.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/apps/cgstats/db/models/sample.py` & `cg-32.2.5/cg/apps/cgstats/db/models/sample.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/apps/cgstats/db/models/support_params.py` & `cg-32.2.5/cg/apps/cgstats/db/models/support_params.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/apps/cgstats/db/models/unaligned.py` & `cg-32.2.5/cg/apps/cgstats/db/models/unaligned.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/apps/cgstats/db/models/version.py` & `cg-32.2.5/cg/apps/cgstats/db/models/version.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/apps/cgstats/parsers/adapter_metrics.py` & `cg-32.2.5/cg/apps/cgstats/parsers/adapter_metrics.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/apps/cgstats/parsers/conversion_stats.py` & `cg-32.2.5/cg/apps/cgstats/parsers/conversion_stats.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/apps/cgstats/parsers/demux_stats.py` & `cg-32.2.5/cg/apps/cgstats/parsers/demux_stats.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/apps/cgstats/parsers/dragen_demultiplexing_stats.py` & `cg-32.2.5/cg/apps/cgstats/parsers/dragen_demultiplexing_stats.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/apps/cgstats/parsers/quality_metrics.py` & `cg-32.2.5/cg/apps/cgstats/parsers/quality_metrics.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/apps/cgstats/parsers/run_info.py` & `cg-32.2.5/cg/apps/cgstats/parsers/run_info.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/apps/cgstats/stats.py` & `cg-32.2.5/cg/apps/cgstats/stats.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/apps/coverage/api.py` & `cg-32.2.5/cg/apps/coverage/api.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/apps/crunchy/crunchy.py` & `cg-32.2.5/cg/apps/crunchy/crunchy.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/apps/crunchy/files.py` & `cg-32.2.5/cg/apps/crunchy/files.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/apps/crunchy/sbatch.py` & `cg-32.2.5/cg/apps/crunchy/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/apps/demultiplex/demultiplex_api.py` & `cg-32.2.5/cg/apps/demultiplex/demultiplex_api.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/apps/demultiplex/demux_report.py` & `cg-32.2.5/cg/apps/demultiplex/demux_report.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/apps/demultiplex/sample_sheet/create.py` & `cg-32.2.5/cg/apps/demultiplex/sample_sheet/create.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/apps/demultiplex/sample_sheet/dummy_sample.py` & `cg-32.2.5/cg/apps/demultiplex/sample_sheet/dummy_sample.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/apps/demultiplex/sample_sheet/index.py` & `cg-32.2.5/cg/apps/demultiplex/sample_sheet/index.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/apps/demultiplex/sample_sheet/models.py` & `cg-32.2.5/cg/apps/demultiplex/sample_sheet/models.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/apps/demultiplex/sample_sheet/novaseq_sample_sheet.py` & `cg-32.2.5/cg/apps/demultiplex/sample_sheet/novaseq_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/apps/demultiplex/sample_sheet/validate.py` & `cg-32.2.5/cg/apps/demultiplex/sample_sheet/validate.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/apps/demultiplex/sbatch.py` & `cg-32.2.5/cg/apps/demultiplex/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/apps/gens.py` & `cg-32.2.5/cg/apps/gens.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/apps/gt.py` & `cg-32.2.5/cg/apps/gt.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/apps/hermes/hermes_api.py` & `cg-32.2.5/cg/apps/hermes/hermes_api.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/apps/hermes/models.py` & `cg-32.2.5/cg/apps/hermes/models.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/apps/housekeeper/hk.py` & `cg-32.2.5/cg/apps/housekeeper/hk.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,18 +89,14 @@
 
         LOG.info(f"Deleting file {file_id} from housekeeper")
         self._store.session.delete(file_obj)
         self.commit()
 
         return file_obj
 
-    def check_for_files(self, bundle: str = None, tags=None, version=None) -> bool:
-        """Check if there are files for a bundle, tags, and/or version."""
-        return any(self.files(bundle=bundle, tags=tags, version=version))
-
     def add_file(self, path, version_obj: Version, tags: list, to_archive: bool = False) -> File:
         """Add a file to the database."""
         if isinstance(tags, str):
             tags: List[str] = [tags]
         for tag_name in tags:
             if not self.get_tag(tag_name):
                 self.add_tag(tag_name)
```

### Comparing `cg-32.2.4/cg/apps/invoice/render.py` & `cg-32.2.5/cg/apps/invoice/render.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/apps/invoice/templates/KI_pool_invoice.xlsx` & `cg-32.2.5/cg/apps/invoice/templates/KI_pool_invoice.xlsx`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/apps/invoice/templates/KI_sample_invoice.xlsx` & `cg-32.2.5/cg/apps/invoice/templates/KI_sample_invoice.xlsx`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/apps/invoice/templates/KTH_pool_invoice.xlsx` & `cg-32.2.5/cg/apps/invoice/templates/KTH_pool_invoice.xlsx`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/apps/invoice/templates/KTH_sample_invoice.xlsx` & `cg-32.2.5/cg/apps/invoice/templates/KTH_sample_invoice.xlsx`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/apps/lims/api.py` & `cg-32.2.5/cg/apps/lims/api.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/apps/lims/batch.py` & `cg-32.2.5/cg/apps/lims/batch.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/apps/lims/order.py` & `cg-32.2.5/cg/apps/lims/order.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/apps/lims/samplesheet.py` & `cg-32.2.5/cg/apps/lims/samplesheet.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/apps/loqus.py` & `cg-32.2.5/cg/apps/loqus.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/apps/madeline/api.py` & `cg-32.2.5/cg/apps/madeline/api.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/apps/mip/confighandler.py` & `cg-32.2.5/cg/apps/mip/confighandler.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/apps/mutacc_auto.py` & `cg-32.2.5/cg/apps/mutacc_auto.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/apps/orderform/excel_orderform_parser.py` & `cg-32.2.5/cg/apps/orderform/excel_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/apps/orderform/json_orderform_parser.py` & `cg-32.2.5/cg/apps/orderform/json_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/apps/orderform/orderform_parser.py` & `cg-32.2.5/cg/apps/orderform/orderform_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,17 +22,14 @@
     delivery_type: Optional[DataDelivery] = None
     customer_id: constr(
         min_length=1, max_length=Customer.internal_id.property.columns[0].type.length
     ) = None
     order_comment: Optional[str] = None
     order_name: Optional[str] = None
 
-    class Config:
-        validate_assignment = True
-
     def parse_orderform(self, orderform_file: Path) -> None:
         """Parse the orderform information"""
         raise NotImplementedError
 
     def group_cases(self) -> Dict[str, List[OrderSample]]:
         """Group samples in cases."""
         LOG.info("Group samples under respective case")
```

### Comparing `cg-32.2.4/cg/apps/osticket.py` & `cg-32.2.5/cg/apps/osticket.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/apps/scout/scout_export.py` & `cg-32.2.5/cg/apps/scout/scout_export.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/apps/scout/scoutapi.py` & `cg-32.2.5/cg/apps/scout/scoutapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,28 +45,14 @@
                 existing_date = existing_case.analysis_date.date()
                 LOG.warning(f"Analysis of case already loaded: {existing_date}")
                 return
         LOG.debug("load new Scout case")
         self.process.run_command(load_command)
         LOG.debug("Case loaded successfully to Scout")
 
-    def update_alignment_file(self, case_id: str, sample_id: str, alignment_path: Path):
-        """Update alignment file for individual in case"""
-        parameters = [
-            "update",
-            "individual",
-            "--case-id",
-            case_id,
-            "--ind-id",
-            sample_id,
-            "--alignment-path",
-            str(alignment_path),
-        ]
-        self.process.run_command(parameters=parameters)
-
     def export_panels(self, panels: List[str], build: str = GENOME_BUILD_37) -> List[str]:
         """Pass through to export of a list of gene panels.
 
         Return list of lines in bed format
         """
         export_panels_command = ["export", "panel", "--bed"]
         export_panels_command.extend(iter(panels))
```

### Comparing `cg-32.2.4/cg/apps/sequencing_metrics_parser/models/bcl2fastq_metrics.py` & `cg-32.2.5/cg/apps/sequencing_metrics_parser/models/bcl2fastq_metrics.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/apps/sequencing_metrics_parser/models/bcl_convert.py` & `cg-32.2.5/cg/apps/sequencing_metrics_parser/models/bcl_convert.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/apps/sequencing_metrics_parser/parsers/bcl2fastq_to_sequencing_statistics.py` & `cg-32.2.5/cg/apps/sequencing_metrics_parser/parsers/bcl2fastq_to_sequencing_statistics.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/apps/sequencing_metrics_parser/parsers/bcl_convert.py` & `cg-32.2.5/cg/apps/sequencing_metrics_parser/parsers/bcl_convert.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/apps/sequencing_metrics_parser/parsers/bcl_convert_to_sequencing_statistics.py` & `cg-32.2.5/cg/apps/sequencing_metrics_parser/parsers/bcl_convert_to_sequencing_statistics.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/apps/sequencing_metrics_parser/sequencing_metrics_calculator.py` & `cg-32.2.5/cg/apps/sequencing_metrics_parser/sequencing_metrics_calculator.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/apps/slurm/sbatch.py` & `cg-32.2.5/cg/apps/slurm/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/apps/slurm/slurm_api.py` & `cg-32.2.5/cg/apps/slurm/slurm_api.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/apps/tb/api.py` & `cg-32.2.5/cg/apps/tb/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,22 +102,14 @@
         request_body = {
             "case_id": case_id,
         }
         response = self.query_trailblazer(command="get-latest-analysis", request_body=request_body)
         if response:
             return TrailblazerAnalysis.parse_obj(response)
 
-    def find_analysis(
-        self, case_id: str, started_at: dt.datetime, status: str
-    ) -> Optional[TrailblazerAnalysis]:
-        request_body = {"case_id": case_id, "started_at": str(started_at), "status": status}
-        response = self.query_trailblazer(command="find-analysis", request_body=request_body)
-        if response:
-            return TrailblazerAnalysis.parse_obj(response)
-
     def get_latest_analysis_status(self, case_id: str) -> Optional[str]:
         latest_analysis = self.get_latest_analysis(case_id=case_id)
         if latest_analysis:
             return latest_analysis.status
 
     def has_latest_analysis_started(self, case_id: str) -> bool:
         return self.get_latest_analysis_status(case_id=case_id) in self.__STARTED_STATUSES
@@ -127,19 +119,14 @@
 
     def is_latest_analysis_completed(self, case_id: str) -> bool:
         return self.get_latest_analysis_status(case_id=case_id) == AnalysisStatus.COMPLETED
 
     def is_latest_analysis_qc(self, case_id: str) -> bool:
         return self.get_latest_analysis_status(case_id=case_id) == AnalysisStatus.QC
 
-    def delete_analysis(self, analysis_id: str, force: bool = False) -> None:
-        """Raises TrailblazerAPIHTTPError"""
-        request_body = {"analysis_id": analysis_id, "force": force}
-        self.query_trailblazer(command="delete-analysis", request_body=request_body)
-
     def mark_analyses_deleted(self, case_id: str) -> Optional[list]:
         """Mark all analyses for case deleted without removing analysis files"""
         request_body = {
             "case_id": case_id,
         }
         response = self.query_trailblazer(
             command="mark-analyses-deleted", request_body=request_body
```

### Comparing `cg-32.2.4/cg/apps/tb/models.py` & `cg-32.2.5/cg/apps/tb/models.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/apps/vogue.py` & `cg-32.2.5/cg/apps/vogue.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/cli/add.py` & `cg-32.2.5/cg/cli/add.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/cli/backup.py` & `cg-32.2.5/cg/cli/backup.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/cli/base.py` & `cg-32.2.5/cg/cli/base.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/cli/clean.py` & `cg-32.2.5/cg/cli/clean.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/cli/compress/base.py` & `cg-32.2.5/cg/cli/compress/base.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/cli/compress/fastq.py` & `cg-32.2.5/cg/cli/compress/fastq.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/cli/compress/helpers.py` & `cg-32.2.5/cg/cli/compress/helpers.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/cli/delete/base.py` & `cg-32.2.5/cg/cli/delete/base.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/cli/delete/case.py` & `cg-32.2.5/cg/cli/delete/case.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/cli/delete/cases.py` & `cg-32.2.5/cg/cli/delete/cases.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/cli/delete/observations.py` & `cg-32.2.5/cg/cli/delete/observations.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/cli/deliver/base.py` & `cg-32.2.5/cg/cli/deliver/base.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/cli/demultiplex/add.py` & `cg-32.2.5/cg/cli/demultiplex/add.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/cli/demultiplex/base.py` & `cg-32.2.5/cg/cli/demultiplex/base.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/cli/demultiplex/demux.py` & `cg-32.2.5/cg/cli/demultiplex/demux.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/cli/demultiplex/finish.py` & `cg-32.2.5/cg/cli/demultiplex/finish.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/cli/demultiplex/report.py` & `cg-32.2.5/cg/cli/demultiplex/report.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/cli/demultiplex/sample_sheet.py` & `cg-32.2.5/cg/cli/demultiplex/sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/cli/generate/report/base.py` & `cg-32.2.5/cg/cli/generate/report/base.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/cli/generate/report/options.py` & `cg-32.2.5/cg/cli/generate/report/options.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/cli/generate/report/utils.py` & `cg-32.2.5/cg/cli/generate/report/utils.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/cli/get.py` & `cg-32.2.5/cg/cli/get.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/cli/set/base.py` & `cg-32.2.5/cg/cli/set/base.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/cli/set/case.py` & `cg-32.2.5/cg/cli/set/case.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/cli/set/cases.py` & `cg-32.2.5/cg/cli/set/cases.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/cli/store/fastq.py` & `cg-32.2.5/cg/cli/store/fastq.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/cli/store/store.py` & `cg-32.2.5/cg/cli/store/store.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/cli/transfer.py` & `cg-32.2.5/cg/cli/transfer.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/cli/upload/base.py` & `cg-32.2.5/cg/cli/upload/base.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/cli/upload/clinical_delivery.py` & `cg-32.2.5/cg/cli/upload/clinical_delivery.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/cli/upload/coverage.py` & `cg-32.2.5/cg/cli/upload/coverage.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/cli/upload/delivery_report.py` & `cg-32.2.5/cg/cli/upload/delivery_report.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/cli/upload/fohm.py` & `cg-32.2.5/cg/cli/upload/fohm.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/cli/upload/genotype.py` & `cg-32.2.5/cg/cli/upload/genotype.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/cli/upload/gens.py` & `cg-32.2.5/cg/cli/upload/gens.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/cli/upload/gisaid.py` & `cg-32.2.5/cg/cli/upload/gisaid.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/cli/upload/mutacc.py` & `cg-32.2.5/cg/cli/upload/mutacc.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/cli/upload/nipt/base.py` & `cg-32.2.5/cg/cli/upload/nipt/base.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/cli/upload/nipt/ftp.py` & `cg-32.2.5/cg/cli/upload/nipt/ftp.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/cli/upload/nipt/statina.py` & `cg-32.2.5/cg/cli/upload/nipt/statina.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/cli/upload/observations/observations.py` & `cg-32.2.5/cg/cli/upload/observations/observations.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/cli/upload/observations/utils.py` & `cg-32.2.5/cg/cli/upload/observations/utils.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/cli/upload/scout.py` & `cg-32.2.5/cg/cli/upload/scout.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/cli/upload/utils.py` & `cg-32.2.5/cg/cli/upload/utils.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/cli/upload/validate.py` & `cg-32.2.5/cg/cli/upload/validate.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/cli/upload/vogue.py` & `cg-32.2.5/cg/cli/upload/vogue.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/cli/workflow/balsamic/base.py` & `cg-32.2.5/cg/cli/workflow/balsamic/base.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/cli/workflow/balsamic/options.py` & `cg-32.2.5/cg/cli/workflow/balsamic/options.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/cli/workflow/balsamic/pon.py` & `cg-32.2.5/cg/cli/workflow/balsamic/pon.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/cli/workflow/balsamic/qc.py` & `cg-32.2.5/cg/cli/workflow/balsamic/qc.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/cli/workflow/balsamic/umi.py` & `cg-32.2.5/cg/cli/workflow/balsamic/umi.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/cli/workflow/base.py` & `cg-32.2.5/cg/cli/workflow/base.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/cli/workflow/commands.py` & `cg-32.2.5/cg/cli/workflow/commands.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/cli/workflow/fastq/base.py` & `cg-32.2.5/cg/cli/workflow/fastq/base.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/cli/workflow/fluffy/base.py` & `cg-32.2.5/cg/cli/workflow/fluffy/base.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/cli/workflow/microsalt/base.py` & `cg-32.2.5/cg/cli/workflow/microsalt/base.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/cli/workflow/mip/base.py` & `cg-32.2.5/cg/cli/workflow/mip/base.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/cli/workflow/mip/options.py` & `cg-32.2.5/cg/cli/workflow/mip/options.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/cli/workflow/mip_dna/base.py` & `cg-32.2.5/cg/cli/workflow/mip_dna/base.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/cli/workflow/mip_rna/base.py` & `cg-32.2.5/cg/cli/workflow/mip_rna/base.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/cli/workflow/mutant/base.py` & `cg-32.2.5/cg/cli/workflow/mutant/base.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/cli/workflow/nextflow/options.py` & `cg-32.2.5/cg/cli/workflow/nextflow/options.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/cli/workflow/rnafusion/base.py` & `cg-32.2.5/cg/cli/workflow/rnafusion/base.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/cli/workflow/rnafusion/options.py` & `cg-32.2.5/cg/cli/workflow/rnafusion/options.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/cli/workflow/taxprofiler/base.py` & `cg-32.2.5/cg/cli/workflow/taxprofiler/base.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/constants/__init__.py` & `cg-32.2.5/cg/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/constants/bcl_convert_metrics.py` & `cg-32.2.5/cg/constants/bcl_convert_metrics.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/constants/compression.py` & `cg-32.2.5/cg/constants/compression.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/constants/constants.py` & `cg-32.2.5/cg/constants/constants.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/constants/delivery.py` & `cg-32.2.5/cg/constants/delivery.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/constants/demultiplexing.py` & `cg-32.2.5/cg/constants/demultiplexing.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/constants/encryption.py` & `cg-32.2.5/cg/constants/encryption.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/constants/gene_panel.py` & `cg-32.2.5/cg/constants/gene_panel.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/constants/housekeeper_tags.py` & `cg-32.2.5/cg/constants/housekeeper_tags.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/constants/lims.py` & `cg-32.2.5/cg/constants/lims.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/constants/nextflow.py` & `cg-32.2.5/cg/constants/nextflow.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/constants/observations.py` & `cg-32.2.5/cg/constants/observations.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/constants/orderforms.py` & `cg-32.2.5/cg/constants/orderforms.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/constants/priority.py` & `cg-32.2.5/cg/constants/priority.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/constants/report.py` & `cg-32.2.5/cg/constants/report.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/constants/rnafusion.py` & `cg-32.2.5/cg/constants/rnafusion.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/constants/scout_upload.py` & `cg-32.2.5/cg/constants/scout_upload.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/constants/sequencing.py` & `cg-32.2.5/cg/constants/sequencing.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/constants/subject.py` & `cg-32.2.5/cg/constants/subject.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/exc.py` & `cg-32.2.5/cg/exc.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/io/api.py` & `cg-32.2.5/cg/io/api.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/io/controller.py` & `cg-32.2.5/cg/io/controller.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/io/csv.py` & `cg-32.2.5/cg/io/csv.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/io/json.py` & `cg-32.2.5/cg/io/json.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/io/validate_path.py` & `cg-32.2.5/cg/io/validate_path.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/io/yaml.py` & `cg-32.2.5/cg/io/yaml.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/meta/archive/ddn_dataflow.py` & `cg-32.2.5/cg/meta/archive/ddn_dataflow.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/meta/backup/backup.py` & `cg-32.2.5/cg/meta/backup/backup.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/meta/backup/pdc.py` & `cg-32.2.5/cg/meta/backup/pdc.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/meta/clean/api.py` & `cg-32.2.5/cg/meta/clean/api.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/meta/clean/demultiplexed_flow_cells.py` & `cg-32.2.5/cg/meta/clean/demultiplexed_flow_cells.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/meta/clean/flow_cell_run_directories.py` & `cg-32.2.5/cg/meta/clean/flow_cell_run_directories.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/meta/compress/compress.py` & `cg-32.2.5/cg/meta/compress/compress.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/meta/compress/files.py` & `cg-32.2.5/cg/meta/compress/files.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/meta/deliver.py` & `cg-32.2.5/cg/meta/deliver.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/meta/deliver_ticket.py` & `cg-32.2.5/cg/meta/deliver_ticket.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/meta/demultiplex/delete_demultiplex_api.py` & `cg-32.2.5/cg/meta/demultiplex/delete_demultiplex_api.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/meta/demultiplex/demux_post_processing.py` & `cg-32.2.5/cg/meta/demultiplex/demux_post_processing.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/meta/demultiplex/files.py` & `cg-32.2.5/cg/meta/demultiplex/files.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/meta/encryption/encryption.py` & `cg-32.2.5/cg/meta/encryption/encryption.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,23 +52,14 @@
         self.run_passhprase_process(
             passphrase_file=passphrase_file, quality_level=quality_level, count=count
         )
         LOG.debug(f"Temporary passphrase file generated: {passphrase_file.name}")
 
         return Path(passphrase_file.name)
 
-    def compare_file_checksums(self, original_file: Path, decrypted_file_checksum: Path) -> bool:
-        """Performs a checksum by decrypting an encrypted file and comparing it to the original file"""
-        is_checksum_equal = sha512_checksum(original_file) == sha512_checksum(
-            decrypted_file_checksum
-        )
-        if not is_checksum_equal:
-            raise ChecksumFailedError(message="Checksum comparison failed!")
-        LOG.info("Checksum comparison successful!")
-
     def get_asymmetric_encryption_command(self, input_file: Path, output_file: Path) -> List[str]:
         """Generates the gpg command for asymmetric encryption"""
         encryption_parameters: list = GPGParameters.ASYMMETRIC_ENCRYPTION.copy()
         output_parameter: list = GPGParameters.OUTPUT_PARAMETER.copy()
         output_parameter.extend([str(output_file), str(input_file)])
         encryption_parameters.extend(output_parameter)
         return encryption_parameters
```

### Comparing `cg-32.2.4/cg/meta/invoice.py` & `cg-32.2.5/cg/meta/invoice.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/meta/meta.py` & `cg-32.2.5/cg/meta/meta.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/meta/observations/balsamic_observations_api.py` & `cg-32.2.5/cg/meta/observations/balsamic_observations_api.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/meta/observations/mip_dna_observations_api.py` & `cg-32.2.5/cg/meta/observations/mip_dna_observations_api.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/meta/observations/observations_api.py` & `cg-32.2.5/cg/meta/observations/observations_api.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/meta/orders/api.py` & `cg-32.2.5/cg/meta/orders/api.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/meta/orders/case_submitter.py` & `cg-32.2.5/cg/meta/orders/case_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/meta/orders/fastq_submitter.py` & `cg-32.2.5/cg/meta/orders/fastq_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/meta/orders/lims.py` & `cg-32.2.5/cg/meta/orders/lims.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/meta/orders/metagenome_submitter.py` & `cg-32.2.5/cg/meta/orders/metagenome_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/meta/orders/microbial_submitter.py` & `cg-32.2.5/cg/meta/orders/microbial_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/meta/orders/pool_submitter.py` & `cg-32.2.5/cg/meta/orders/pool_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/meta/orders/sars_cov_2_submitter.py` & `cg-32.2.5/cg/meta/orders/sars_cov_2_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/meta/orders/submitter.py` & `cg-32.2.5/cg/meta/orders/submitter.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/meta/orders/ticket_handler.py` & `cg-32.2.5/cg/meta/orders/ticket_handler.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/meta/report/balsamic.py` & `cg-32.2.5/cg/meta/report/balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/meta/report/balsamic_umi.py` & `cg-32.2.5/cg/meta/report/balsamic_umi.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/meta/report/field_validators.py` & `cg-32.2.5/cg/meta/report/field_validators.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/meta/report/mip_dna.py` & `cg-32.2.5/cg/meta/report/mip_dna.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/meta/report/report_api.py` & `cg-32.2.5/cg/meta/report/report_api.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/meta/report/templates/balsamic_report.html` & `cg-32.2.5/cg/meta/report/templates/balsamic_report.html`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/meta/report/templates/bootstrap.html` & `cg-32.2.5/cg/meta/report/templates/bootstrap.html`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/meta/report/templates/mip-dna_report.html` & `cg-32.2.5/cg/meta/report/templates/mip-dna_report.html`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/meta/rsync/rsync_api.py` & `cg-32.2.5/cg/meta/rsync/rsync_api.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/meta/tar/tar.py` & `cg-32.2.5/cg/meta/tar/tar.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/meta/transfer/external_data.py` & `cg-32.2.5/cg/meta/transfer/external_data.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/meta/transfer/flowcell.py` & `cg-32.2.5/cg/meta/transfer/flowcell.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/meta/transfer/lims.py` & `cg-32.2.5/cg/meta/transfer/lims.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,21 +17,14 @@
 
 
 class PoolState(Enum):
     RECEIVED = "received"
     DELIVERED = "delivered"
 
 
-class MicrobialState(Enum):
-    RECEIVED = "received"
-    PREPARED = "prepared"
-    SEQUENCED = "sequenced"
-    DELIVERED = "delivered"
-
-
 class IncludeOptions(Enum):
     UNSET = "unset"
     NOTINVOICED = "not-invoiced"
     ALL = "all"
 
 
 class TransferLims(object):
@@ -54,17 +47,14 @@
             SampleState.RECEIVED: self.lims.get_received_date,
             SampleState.PREPARED: self.lims.get_prepared_date,
             SampleState.DELIVERED: self.lims.get_delivery_date,
             PoolState.RECEIVED: self.lims.get_received_date,
             PoolState.DELIVERED: self.lims.get_delivery_date,
         }
 
-    def _get_samples_not_yet_delivered(self):
-        return self.status.get_samples_not_delivered()
-
     def transfer_samples(
         self, status_type: SampleState, include: str = "unset", sample_id: str = None
     ):
         """Transfer information about samples."""
 
         if sample_id:
             samples: List[Sample] = self.status.get_samples_by_internal_id(internal_id=sample_id)
```

### Comparing `cg-32.2.4/cg/meta/upload/balsamic/balsamic.py` & `cg-32.2.5/cg/meta/upload/balsamic/balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/meta/upload/coverage.py` & `cg-32.2.5/cg/meta/upload/coverage.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/meta/upload/fohm/fohm.py` & `cg-32.2.5/cg/meta/upload/fohm/fohm.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/meta/upload/gisaid/constants.py` & `cg-32.2.5/cg/meta/upload/gisaid/constants.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/meta/upload/gisaid/gisaid.py` & `cg-32.2.5/cg/meta/upload/gisaid/gisaid.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/meta/upload/gisaid/models.py` & `cg-32.2.5/cg/meta/upload/gisaid/models.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/meta/upload/gt.py` & `cg-32.2.5/cg/meta/upload/gt.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/meta/upload/mip/mip_dna.py` & `cg-32.2.5/cg/meta/upload/mip/mip_dna.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/meta/upload/mip/mip_rna.py` & `cg-32.2.5/cg/meta/upload/mip/mip_rna.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/meta/upload/mutacc.py` & `cg-32.2.5/cg/meta/upload/mutacc.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,19 +25,14 @@
     def extract_reads(self, case: scout_export.ScoutExportCase):
         """Use mutacc API to extract reads from case"""
         data: dict = self.data(case)
         if data:
             LOG.info("Extracting reads from case %s", case.id)
             self.mutacc_auto.extract_reads(case=data["case"], variants=data["causatives"])
 
-    def import_cases(self):
-        """Use mutacc API to import cases to database"""
-        LOG.info("importing cases into mutacc database")
-        self.mutacc_auto.import_reads()
-
     def data(self, case: scout_export.ScoutExportCase) -> Dict[str, dict]:
         """
         Find the necessary data for the case
 
         Args:
             case (dict): case dictionary from scout
```

### Comparing `cg-32.2.4/cg/meta/upload/nipt/nipt.py` & `cg-32.2.5/cg/meta/upload/nipt/nipt.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/meta/upload/rnafusion/rnafusion.py` & `cg-32.2.5/cg/meta/upload/rnafusion/rnafusion.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/meta/upload/scout/balsamic_config_builder.py` & `cg-32.2.5/cg/meta/upload/scout/balsamic_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/meta/upload/scout/balsamic_umi_config_builder.py` & `cg-32.2.5/cg/meta/upload/scout/balsamic_umi_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/meta/upload/scout/hk_tags.py` & `cg-32.2.5/cg/meta/upload/scout/hk_tags.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/meta/upload/scout/mip_config_builder.py` & `cg-32.2.5/cg/meta/upload/scout/mip_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/meta/upload/scout/rnafusion_config_builder.py` & `cg-32.2.5/cg/meta/upload/scout/rnafusion_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/meta/upload/scout/scout_config_builder.py` & `cg-32.2.5/cg/meta/upload/scout/scout_config_builder.py`

 * *Files 10% similar despite different names*

```diff
@@ -116,21 +116,14 @@
                     phenotype_group,
                     sample_obj.internal_id,
                 )
                 phenotype_groups.add(phenotype_group)
         if phenotype_groups:
             self.load_config.phenotype_groups = list(phenotype_groups)
 
-    def include_synopsis(self) -> None:
-        LOG.info("Adding synopsis string to scout load config")
-        synopsis_string: str = self.analysis_obj.family.synopsis
-        if synopsis_string:
-            LOG.debug("Adding synopsis string %s", synopsis_string)
-            self.load_config.synopsis = synopsis_string
-
     def include_cohorts(self) -> None:
         LOG.info("Including cohorts to scout load config")
         cohorts: List[str] = self.analysis_obj.family.cohorts
         if cohorts:
             LOG.debug("Adding cohorts %s", ", ".join(cohorts))
             self.load_config.cohorts = cohorts
```

### Comparing `cg-32.2.4/cg/meta/upload/scout/uploadscoutapi.py` & `cg-32.2.5/cg/meta/upload/scout/uploadscoutapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -320,24 +320,14 @@
         LOG.info("Upload splice junctions bed file finished!")
 
     def upload_rna_junctions_to_scout(self, dry_run: bool, case_id: str) -> None:
         """Upload RNA junctions splice files to Scout."""
         self.upload_splice_junctions_bed_to_scout(dry_run=dry_run, case_id=case_id)
         self.upload_rna_coverage_bigwig_to_scout(case_id=case_id, dry_run=dry_run)
 
-    @staticmethod
-    def _get_sample(case: Family, subject_id: str) -> Optional[Sample]:
-        """Return sample of a case for a subject_id."""
-
-        link: FamilySample
-        for link in case.links:
-            sample: Sample = link.sample
-            if sample.subject_id == subject_id:
-                return sample
-
     def get_config_builder(self, analysis, hk_version) -> ScoutConfigBuilder:
         config_builders = {
             Pipeline.BALSAMIC: BalsamicConfigBuilder(
                 hk_version_obj=hk_version, analysis_obj=analysis, lims_api=self.lims
             ),
             Pipeline.BALSAMIC_UMI: BalsamicUmiConfigBuilder(
                 hk_version_obj=hk_version, analysis_obj=analysis, lims_api=self.lims
```

### Comparing `cg-32.2.4/cg/meta/upload/upload_api.py` & `cg-32.2.5/cg/meta/upload/upload_api.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/meta/upload/vogue.py` & `cg-32.2.5/cg/meta/upload/vogue.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/meta/workflow/analysis.py` & `cg-32.2.5/cg/meta/workflow/analysis.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/meta/workflow/balsamic.py` & `cg-32.2.5/cg/meta/workflow/balsamic.py`

 * *Files 4% similar despite different names*

```diff
@@ -498,51 +498,14 @@
                 case_id=case_id, sample_data=sample_data, force_normal=force_normal
             )
         )
         config_case.update(self.get_parsed_observation_file_paths(observations))
 
         return config_case
 
-    def build_sample_id_map_string(self, case_id: str) -> str:
-        """Creates sample info string for balsamic with format lims_id:tumor/normal:customer_sample_id"""
-
-        tumor_sample_lims_id = self.get_tumor_sample_name(case_id=case_id)
-        tumor_string = f"{tumor_sample_lims_id}:tumor:{self.status_db.get_sample_by_internal_id(internal_id=tumor_sample_lims_id).name}"
-        normal_sample_lims_id = self.get_normal_sample_name(case_id=case_id)
-        if normal_sample_lims_id:
-            normal_string = f"{normal_sample_lims_id}:normal:{self.status_db.get_sample_by_internal_id(internal_id=normal_sample_lims_id).name}"
-            return ",".join([tumor_string, normal_string])
-        return tumor_string
-
-    def build_case_id_map_string(self, case_id: str) -> Optional[str]:
-        """Creates case info string for balsamic with format panel_shortname:case_name:application_tag."""
-
-        case: Family = self.status_db.get_case_by_internal_id(internal_id=case_id)
-        sample: Sample = case.links[0].sample
-        if sample.from_sample:
-            sample: Sample = self.status_db.get_sample_by_internal_id(
-                internal_id=sample.from_sample
-            )
-        capture_kit: Optional[str] = self.lims_api.capture_kit(lims_id=sample.internal_id)
-        if capture_kit:
-            panel_shortname: str = self.status_db.get_bed_version_by_short_name(
-                bed_version_short_name=capture_kit
-            ).shortname
-        elif (
-            self.get_application_type(case.links[0].sample) == AnalysisType.WHOLE_GENOME_SEQUENCING
-        ):
-            panel_shortname: str = "Whole_Genome"
-        else:
-            return
-
-        application_tag = self.status_db.get_application_tag_by_application_version_entry_id(
-            application_version_entry_id=case.links[0].sample.application_version_id
-        )
-        return f"{panel_shortname}:{case.name}:{application_tag}"
-
     @staticmethod
     def print_sample_params(case_id: str, sample_data: dict) -> None:
         """Outputs a table of samples to be displayed in log"""
 
         LOG.info(f"Case {case_id} has following BALSAMIC samples:")
         LOG.info(
             "{:<20} {:<20} {:<20} {:<20}".format(
```

### Comparing `cg-32.2.4/cg/meta/workflow/balsamic_pon.py` & `cg-32.2.5/cg/meta/workflow/balsamic_pon.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/meta/workflow/balsamic_qc.py` & `cg-32.2.5/cg/meta/workflow/balsamic_qc.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/meta/workflow/balsamic_umi.py` & `cg-32.2.5/cg/meta/workflow/balsamic_umi.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/meta/workflow/fastq.py` & `cg-32.2.5/cg/meta/workflow/fastq.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/meta/workflow/fluffy.py` & `cg-32.2.5/cg/meta/workflow/fluffy.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/meta/workflow/microsalt.py` & `cg-32.2.5/cg/meta/workflow/microsalt.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/meta/workflow/mip.py` & `cg-32.2.5/cg/meta/workflow/mip.py`

 * *Files 1% similar despite different names*

```diff
@@ -261,23 +261,14 @@
             sample_id_metrics=qc_metrics.sample_id_metrics,
             mip_version=sample_info.mip_version,
             rank_model_version=sample_info.rank_model_version,
             sample_ids=mip_config.sample_ids,
             sv_rank_model_version=sample_info.sv_rank_model_version,
         )
 
-    @staticmethod
-    def is_dna_only_case(case_obj: Family) -> bool:
-        """Returns True if all samples of a case has DNA application type."""
-
-        return all(
-            _link.sample.application_version.application.analysis_type not in "wts"
-            for _link in case_obj.links
-        )
-
     def get_skip_evaluation_flag(self, case_id: str, skip_evaluation: bool) -> bool:
         """If any sample in this case is downsampled or external, returns true"""
         if skip_evaluation:
             return True
         case_obj = self.status_db.get_case_by_internal_id(internal_id=case_id)
         for link_obj in case_obj.links:
             downsampled = isinstance(link_obj.sample.downsampled_to, int)
```

### Comparing `cg-32.2.4/cg/meta/workflow/mip_dna.py` & `cg-32.2.5/cg/meta/workflow/mip_dna.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/meta/workflow/mip_rna.py` & `cg-32.2.5/cg/meta/workflow/mip_rna.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/meta/workflow/mutant.py` & `cg-32.2.5/cg/meta/workflow/mutant.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/meta/workflow/nextflow_common.py` & `cg-32.2.5/cg/meta/workflow/nextflow_common.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,23 +67,14 @@
     @classmethod
     def get_nextflow_config_path(cls, nextflow_config: Optional[str] = None) -> Optional[Path]:
         """Generates a path where the Nextflow configurations should be located."""
         if nextflow_config:
             return Path(nextflow_config).absolute()
 
     @classmethod
-    def get_case_nextflow_pid_path(cls, case_id: str, root_dir: str) -> Path:
-        """Generates a path where the Nextflow pid file for the case_id should be located."""
-        # If not specified with the NXF_PID_FILE variable, a .nextflow.pid is created in the launch directory when
-        # running nextflow in the background (with the bg option)
-        return Path(
-            (cls.get_case_path(case_id=case_id, root_dir=root_dir)), f"{case_id}_nextflow.pid"
-        )
-
-    @classmethod
     def get_software_version_path(cls, case_id: str, root_dir: str) -> Path:
         return Path(
             (cls.get_case_path(case_id, root_dir)), "pipeline_info", "software_versions.yml"
         )
 
     @classmethod
     def get_pipeline_version(cls, case_id: str, root_dir: str, pipeline: str) -> str:
@@ -196,21 +187,14 @@
     @classmethod
     def get_outdir_path(cls, case_id: str, root_dir: str, outdir: str = None) -> Path:
         if outdir:
             return outdir
         return Path(cls.get_case_path(case_id, root_dir))
 
     @classmethod
-    def get_nextflow_stdout_stderr(cls, case_id: str, root_dir: str) -> List[str]:
-        case_path = cls.get_case_path(case_id, root_dir).as_posix()
-        return [
-            f" > {case_path}/{case_id}-stdout.log 2> {case_path}/{case_id}-stdout.err < /dev/null & "
-        ]
-
-    @classmethod
     def get_replace_map(cls, case_id: str, root_dir: str) -> dict:
         return {
             "PATHTOCASE": str(cls.get_case_path(case_id, root_dir)),
             "CASEID": case_id,
         }
 
     @classmethod
```

### Comparing `cg-32.2.4/cg/meta/workflow/prepare_fastq.py` & `cg-32.2.5/cg/meta/workflow/prepare_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/meta/workflow/rnafusion.py` & `cg-32.2.5/cg/meta/workflow/rnafusion.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/meta/workflow/taxprofiler.py` & `cg-32.2.5/cg/meta/workflow/taxprofiler.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/meta/workflow/tower_common.py` & `cg-32.2.5/cg/meta/workflow/tower_common.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/models/balsamic/config.py` & `cg-32.2.5/cg/models/balsamic/config.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/models/balsamic/metrics.py` & `cg-32.2.5/cg/models/balsamic/metrics.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/models/cg_config.py` & `cg-32.2.5/cg/models/cg_config.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/models/cgstats/stats_sample.py` & `cg-32.2.5/cg/models/cgstats/stats_sample.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/models/compression_data.py` & `cg-32.2.5/cg/models/compression_data.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/models/deliverables/metric_deliverables.py` & `cg-32.2.5/cg/models/deliverables/metric_deliverables.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/models/demultiplex/demux_results.py` & `cg-32.2.5/cg/models/demultiplex/demux_results.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/models/demultiplex/flow_cell.py` & `cg-32.2.5/cg/models/demultiplex/flow_cell.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/models/demultiplex/run_parameters.py` & `cg-32.2.5/cg/models/demultiplex/run_parameters.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/models/demultiplex/sbatch.py` & `cg-32.2.5/cg/models/demultiplex/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/models/file_data.py` & `cg-32.2.5/cg/models/file_data.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/models/invoice/invoice.py` & `cg-32.2.5/cg/models/invoice/invoice.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/models/lims/sample.py` & `cg-32.2.5/cg/models/lims/sample.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/models/mip/mip_config.py` & `cg-32.2.5/cg/models/mip/mip_config.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/models/mip/mip_metrics_deliverables.py` & `cg-32.2.5/cg/models/mip/mip_metrics_deliverables.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/models/mip/mip_sample_info.py` & `cg-32.2.5/cg/models/mip/mip_sample_info.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/models/nextflow/deliverables.py` & `cg-32.2.5/cg/models/nextflow/deliverables.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/models/nextflow/sample.py` & `cg-32.2.5/cg/models/nextflow/sample.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/models/observations/input_files.py` & `cg-32.2.5/cg/models/observations/input_files.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/models/orders/constants.py` & `cg-32.2.5/cg/models/orders/constants.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/models/orders/excel_sample.py` & `cg-32.2.5/cg/models/orders/excel_sample.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/models/orders/json_sample.py` & `cg-32.2.5/cg/models/orders/json_sample.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/models/orders/order.py` & `cg-32.2.5/cg/models/orders/order.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/models/orders/orderform_schema.py` & `cg-32.2.5/cg/models/orders/orderform_schema.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/models/orders/sample_base.py` & `cg-32.2.5/cg/models/orders/sample_base.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/models/orders/samples.py` & `cg-32.2.5/cg/models/orders/samples.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/models/report/metadata.py` & `cg-32.2.5/cg/models/report/metadata.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/models/report/report.py` & `cg-32.2.5/cg/models/report/report.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/models/report/sample.py` & `cg-32.2.5/cg/models/report/sample.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/models/report/validators.py` & `cg-32.2.5/cg/models/report/validators.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/models/rnafusion/rnafusion_sample.py` & `cg-32.2.5/cg/models/rnafusion/rnafusion_sample.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/models/scout/scout_load_config.py` & `cg-32.2.5/cg/models/scout/scout_load_config.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/models/slurm/sbatch.py` & `cg-32.2.5/cg/models/slurm/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/models/workflow/mutant.py` & `cg-32.2.5/cg/models/workflow/mutant.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/resources/20181012_Indices.csv` & `cg-32.2.5/cg/resources/20181012_Indices.csv`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/resources/rnafusion_bundle_filenames.csv` & `cg-32.2.5/cg/resources/rnafusion_bundle_filenames.csv`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/server/admin.py` & `cg-32.2.5/cg/server/admin.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/server/api.py` & `cg-32.2.5/cg/server/api.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/server/app.py` & `cg-32.2.5/cg/server/app.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/server/config.py` & `cg-32.2.5/cg/server/config.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/server/ext.py` & `cg-32.2.5/cg/server/ext.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/server/invoices/templates/invoices/index.html` & `cg-32.2.5/cg/server/invoices/templates/invoices/index.html`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/server/invoices/templates/invoices/invoice.html` & `cg-32.2.5/cg/server/invoices/templates/invoices/invoice.html`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/server/invoices/templates/invoices/layout.html` & `cg-32.2.5/cg/server/invoices/templates/invoices/layout.html`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/server/invoices/templates/invoices/new.html` & `cg-32.2.5/cg/server/invoices/templates/invoices/new.html`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/server/invoices/views.py` & `cg-32.2.5/cg/server/invoices/views.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/store/api/add.py` & `cg-32.2.5/cg/store/api/add.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/store/api/base.py` & `cg-32.2.5/cg/store/api/base.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/store/api/core.py` & `cg-32.2.5/cg/store/api/core.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/store/api/delete.py` & `cg-32.2.5/cg/store/api/delete.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/store/api/find_basic_data.py` & `cg-32.2.5/cg/store/api/find_basic_data.py`

 * *Files 26% similar despite different names*

```diff
@@ -43,73 +43,33 @@
         """Return an application by tag."""
         return apply_application_filter(
             applications=self._get_query(table=Application),
             filter_functions=[ApplicationFilter.FILTER_BY_TAG],
             tag=tag,
         ).first()
 
-    def get_applications_by_prep_category(self, prep_category: str) -> List[Application]:
-        """Return applications by prep category."""
-        return (
-            apply_application_filter(
-                applications=self._get_query(table=Application),
-                filter_functions=[ApplicationFilter.FILTER_BY_PREP_CATEGORY],
-                prep_category=prep_category,
-            )
-            .order_by(Application.prep_category, Application.tag)
-            .all()
-        )
-
     def get_applications_is_not_archived(self) -> List[Application]:
         """Return applications that are not archived."""
         return (
             apply_application_filter(
                 applications=self._get_query(table=Application),
                 filter_functions=[ApplicationFilter.FILTER_IS_NOT_ARCHIVED],
             )
             .order_by(Application.prep_category, Application.tag)
             .all()
         )
 
-    def get_applications_by_prep_category_and_is_archived(
-        self, prep_category: str
-    ) -> List[Application]:
-        """Return applications by prep category that are archived."""
-        return (
-            apply_application_filter(
-                applications=self._get_query(table=Application),
-                filter_functions=[
-                    ApplicationFilter.FILTER_BY_PREP_CATEGORY,
-                    ApplicationFilter.FILTER_IS_ARCHIVED,
-                ],
-                prep_category=prep_category,
-            )
-            .order_by(Application.prep_category, Application.tag)
-            .all()
-        )
-
     def get_applications(self) -> List[Application]:
         """Return all applications."""
         return (
             self._get_query(table=Application)
             .order_by(Application.prep_category, Application.tag)
             .all()
         )
 
-    def get_application_version_by_application_entry_id(
-        self, application_entry_id: int
-    ) -> ApplicationVersion:
-        """Return an application version by application entry id."""
-        application_versions = self._get_query(table=ApplicationVersion)
-        return apply_application_versions_filter(
-            application_versions=application_versions,
-            filter_functions=[ApplicationVersionFilter.FILTER_BY_APPLICATION_ENTRY_ID],
-            application_entry_id=application_entry_id,
-        ).first()
-
     def get_current_application_version_by_tag(self, tag: str) -> Optional[ApplicationVersion]:
         """Return the current application version for an application tag."""
         application = self.get_application_by_tag(tag=tag)
         if not application:
             return None
         return apply_application_versions_filter(
             filter_functions=[
@@ -118,49 +78,32 @@
                 ApplicationVersionFilter.ORDER_BY_VALID_FROM_DESC,
             ],
             application_versions=self._get_query(table=ApplicationVersion),
             application_entry_id=application.id,
             valid_from=dt.datetime.now(),
         ).first()
 
-    def get_application_versions(self) -> List[ApplicationVersion]:
-        """Return all application versions."""
-        return self._get_query(table=ApplicationVersion).all()
-
     def get_bed_version_by_short_name(self, bed_version_short_name: str) -> BedVersion:
         """Return bed version with short name."""
         return apply_bed_version_filter(
             bed_versions=self._get_query(table=BedVersion),
             bed_version_short_name=bed_version_short_name,
             filter_functions=[BedVersionFilter.FILTER_BY_SHORT_NAME],
         ).first()
 
-    def get_bed_by_name(self, bed_name: str) -> Optional[Bed]:
-        """Return bed by name."""
-        return apply_bed_filter(
-            beds=self._get_query(table=Bed),
-            bed_name=bed_name,
-            filter_functions=[BedFilter.FILTER_BY_NAME],
-        ).first()
-
     def get_active_beds(self) -> Query:
         """Get all beds which are not archived."""
         bed_filter_functions: List[BedFilter] = [
             BedFilter.FILTER_NOT_ARCHIVED,
             BedFilter.ORDER_BY_NAME,
         ]
         return apply_bed_filter(
             beds=self._get_query(table=Bed), filter_functions=bed_filter_functions
         )
 
-    def get_latest_bed_version(self, bed_name: str) -> Optional[BedVersion]:
-        """Return the latest bed version for a bed by supplied name."""
-        bed: Optional[Bed] = self.get_bed_by_name(bed_name=bed_name)
-        return bed.versions[-1] if bed and bed.versions else None
-
     def get_customer_by_internal_id(self, customer_internal_id: str) -> Customer:
         """Return customer with customer id."""
         return apply_customer_filter(
             filter_functions=[CustomerFilter.FILTER_BY_INTERNAL_ID],
             customers=self._get_query(table=Customer),
             customer_internal_id=customer_internal_id,
         ).first()
```

### Comparing `cg-32.2.4/cg/store/api/find_business_data.py` & `cg-32.2.5/cg/store/api/find_business_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,22 +45,14 @@
 
 class FindBusinessDataHandler(BaseHandler):
     """Contains methods to find business data model instances"""
 
     def __init__(self, session: Session):
         super().__init__(session=session)
 
-    def get_analyses_by_case_entry_id(self, case_entry_id: int) -> List[Analysis]:
-        """Return analysis by case entry id."""
-        return apply_analysis_filter(
-            analyses=self._get_query(Analysis),
-            case_entry_id=case_entry_id,
-            filter_functions=[AnalysisFilter.FILTER_BY_CASE_ENTRY_ID],
-        ).all()
-
     def get_case_by_entry_id(self, entry_id: str) -> Family:
         """Return a case by entry id."""
         cases_query: Query = self._get_query(table=Family)
         return apply_case_filter(
             cases=cases_query, filter_functions=[CaseFilter.FILTER_BY_ENTRY_ID], entry_id=entry_id
         ).first()
 
@@ -81,29 +73,14 @@
 
         return (
             self.get_case_by_internal_id(internal_id=case_id)
             .links[ListIndexes.FIRST.value]
             .sample.application_version.application
         )
 
-    def get_application_tag_by_application_version_entry_id(
-        self,
-        application_version_entry_id: str,
-    ) -> Optional[str]:
-        """Return the application tag of an application version."""
-
-        application_version: ApplicationVersion = apply_application_versions_filter(
-            application_versions=self._get_query(ApplicationVersion),
-            filter_functions=[ApplicationVersionFilter.FILTER_BY_ENTRY_ID],
-            application_version_entry_id=application_version_entry_id,
-        ).first()
-
-        if application_version and application_version.application:
-            return application_version.application.tag
-
     def get_analysis_for_vogue_upload_completed_after(self, completed_at_after: dt.datetime):
         """Return all cases completed after a given date that have not been uploaded to Vogue."""
         filter_functions = [
             AnalysisFilter.FILTER_NOT_UPLOADED_TO_VOGUE,
             AnalysisFilter.FILTER_COMPLETED_AT_AFTER,
         ]
         return apply_analysis_filter(
@@ -158,23 +135,14 @@
         return apply_analysis_filter(
             analyses=self._get_query(Analysis),
             case_entry_id=case_entry_id,
             started_at_date=started_at_date,
             filter_functions=filter_functions,
         ).first()
 
-    def get_cases_created_within_days(self, days: int) -> List[Family]:
-        """Fetch all cases created within the past days."""
-        newer_than_date = dt.datetime.now() - dt.timedelta(days=days)
-        return apply_case_filter(
-            filter_functions=[CaseFilter.GET_NEW_BY_CREATION_DATE],
-            cases=self._get_query(table=Family),
-            creation_date=newer_than_date,
-        ).all()
-
     def get_cases_by_customer_and_case_name_search(
         self, customer: Customer, case_name_search: str
     ) -> List[Family]:
         """
         Retrieve a list of cases filtered by a customer and matching names.
 
         Args:
@@ -281,22 +249,14 @@
         """Return the case-sample links associated with a case."""
         return apply_case_sample_filter(
             filter_functions=[CaseSampleFilter.GET_SAMPLES_IN_CASE_BY_INTERNAL_ID],
             case_internal_id=case_internal_id,
             case_samples=self._get_join_case_sample_query(),
         ).all()
 
-    def get_case_samples_from_sample_entry_id(self, sample_entry_id: str) -> Query:
-        """Return cases related to a given sample."""
-        return apply_case_sample_filter(
-            filter_functions=[CaseSampleFilter.GET_CASES_WITH_SAMPLE_BY_ENTRY_ID],
-            sample_entry_id=sample_entry_id,
-            case_samples=self._get_join_case_sample_query(),
-        )
-
     def filter_cases_with_samples(self, case_ids: List[str]) -> List[str]:
         """Return case id:s associated with samples."""
         cases_with_samples = set()
         for case_id in case_ids:
             case: Family = self.get_case_by_internal_id(internal_id=case_id)
             if case and case.links:
                 cases_with_samples.add(case_id)
@@ -353,20 +313,14 @@
     def get_sample_ids_by_case_id(self, case_id: str = None) -> Iterator[str]:
         """Return sample ids from case id."""
         case: Family = self.get_case_by_internal_id(internal_id=case_id)
         self._is_case_found(case=case, case_id=case_id)
         for link in case.links:
             yield link.sample.internal_id
 
-    def get_sequenced_samples(self, family_id: str) -> List[Sample]:
-        """Get sequenced samples by family_id."""
-
-        samples: List[Sample] = self.get_samples_by_case_id(family_id)
-        return [sample for sample in samples if sample.sequencing_qc]
-
     def get_case_by_name_and_customer(self, customer: Customer, case_name: str) -> Family:
         """Find a case by case name within a customer."""
         return apply_case_filter(
             cases=self._get_query(table=Family),
             filter_functions=[CaseFilter.FILTER_BY_CUSTOMER_ENTRY_ID, CaseFilter.FILTER_BY_NAME],
             customer_entry_id=customer.id,
             name=case_name,
@@ -400,22 +354,14 @@
         """Return flow cell by flow cell name."""
         return apply_flow_cell_filter(
             flow_cells=self._get_query(table=Flowcell),
             flow_cell_name=flow_cell_name,
             filter_functions=[FlowCellFilter.GET_BY_NAME],
         ).first()
 
-    def get_flow_cell_by_name_pattern(self, name_pattern: str) -> Flowcell:
-        """Return flow cell by name pattern."""
-        return apply_flow_cell_filter(
-            flow_cells=self._get_query(table=Flowcell),
-            name_search=name_pattern,
-            filter_functions=[FlowCellFilter.GET_BY_NAME_SEARCH],
-        ).first()
-
     def get_flow_cells_by_statuses(self, flow_cell_statuses: List[str]) -> Optional[List[Flowcell]]:
         """Return flow cells with supplied statuses."""
         return apply_flow_cell_filter(
             flow_cells=self._get_query(table=Flowcell),
             flow_cell_statuses=flow_cell_statuses,
             filter_functions=[FlowCellFilter.GET_WITH_STATUSES],
         ).all()
@@ -588,22 +534,14 @@
         if application.prep_category != PrepCategory.READY_MADE_LIBRARY.value:
             raise ValueError(
                 f"{case_id} is not a ready made library, found prep category: "
                 f"{application.prep_category}"
             )
         return application.expected_reads
 
-    def get_samples_by_name_pattern(self, name_pattern: str) -> List[Sample]:
-        """Return all samples with a name fitting the pattern."""
-        return apply_sample_filter(
-            samples=self._get_query(table=Sample),
-            name_pattern=name_pattern,
-            filter_functions=[SampleFilter.FILTER_BY_NAME_PATTERN],
-        ).all()
-
     def get_samples_by_customer_id_and_pattern(
         self, *, customers: Optional[List[Customer]] = None, pattern: str = None
     ) -> List[Sample]:
         """Get samples by customer and sample internal id  or sample name pattern."""
         samples: Query = self._get_query(table=Sample)
         customer_entry_ids: List[int] = []
         filter_functions: List[SampleFilter] = []
@@ -641,30 +579,14 @@
         self, customer_internal_id: str, subject_id: str
     ) -> List[Sample]:
         """Get samples of customer with given subject id."""
         return self._get_samples_by_customer_and_subject_id_query(
             customer_internal_id=customer_internal_id, subject_id=subject_id
         ).all()
 
-    def get_samples_by_customer_subject_id_and_is_tumour(
-        self, customer_internal_id: str, subject_id: str, is_tumour: bool
-    ) -> List[Sample]:
-        """Get samples of customer with given subject id and is tumour."""
-        samples: Query = self._get_samples_by_customer_and_subject_id_query(
-            customer_internal_id=customer_internal_id, subject_id=subject_id
-        )
-        if is_tumour:
-            return apply_sample_filter(
-                samples=samples, filter_functions=[SampleFilter.FILTER_IS_TUMOUR]
-            ).all()
-        else:
-            return apply_sample_filter(
-                samples=samples, filter_functions=[SampleFilter.FILTER_IS_NOT_TUMOUR]
-            ).all()
-
     def get_samples_by_customer_id_list_and_subject_id_and_is_tumour(
         self, customer_ids: List[int], subject_id: str, is_tumour: bool
     ) -> List[Sample]:
         """Return a list of samples matching a list of customers with given subject id and is a tumour or not."""
         samples = self._get_query(table=Sample)
         filter_functions = [
             SampleFilter.FILTER_BY_CUSTOMER_ENTRY_IDS,
```

### Comparing `cg-32.2.4/cg/store/api/status.py` & `cg-32.2.5/cg/store/api/status.py`

 * *Files 3% similar despite different names*

```diff
@@ -725,28 +725,14 @@
         records: Query = apply_sample_filter(
             filter_functions=sample_filter_functions,
             samples=records,
         )
 
         return records.all()
 
-    def get_samples_not_delivered(self) -> List[Sample]:
-        """Return samples not delivered."""
-        records = self._get_query(table=Sample)
-        sample_filter_functions: List[SampleFilter] = [
-            SampleFilter.FILTER_IS_NOT_DOWN_SAMPLED,
-            SampleFilter.FILTER_IS_NOT_DELIVERED,
-        ]
-
-        records: Query = apply_sample_filter(
-            filter_functions=sample_filter_functions,
-            samples=records,
-        )
-        return records.all()
-
     def get_samples_not_invoiced(self) -> List[Sample]:
         """Return all samples that have  not been invoiced, excluding those that
         have been down sampled."""
         records = self._get_query(table=Sample)
         sample_filter_functions: List[SampleFilter] = [
             SampleFilter.FILTER_HAS_NO_INVOICE_ID,
             SampleFilter.FILTER_IS_NOT_DOWN_SAMPLED,
```

### Comparing `cg-32.2.4/cg/store/filters/status_analysis_filters.py` & `cg-32.2.5/cg/store/filters/status_analysis_filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,19 +21,14 @@
 
 
 def filter_completed_analyses(analyses: Query, **kwargs) -> Query:
     """Return analyses that have been completed."""
     return analyses.filter(Analysis.completed_at.isnot(None))
 
 
-def filter_not_completed_analyses(analyses: Query, **kwargs) -> Query:
-    """Return not completed analyses."""
-    return analyses.filter(Analysis.completed_at.is_(None))
-
-
 def filter_uploaded_analyses(analyses: Query, **kwargs) -> Query:
     """Return analyses that have been already uploaded."""
     return analyses.filter(Analysis.uploaded_at.isnot(None))
 
 
 def filter_not_uploaded_analyses(analyses: Query, **kwargs) -> Query:
     """Return analyses that have not been uploaded."""
@@ -101,19 +96,14 @@
 
 
 def filter_analyses_by_started_at(analyses: Query, started_at_date: datetime, **kwargs) -> Query:
     """Return a query of analyses started at a certain date."""
     return analyses.filter(Analysis.started_at == started_at_date)
 
 
-def order_analyses_by_started_at_desc(analyses: Query, **kwargs) -> Query:
-    """Return a query of ordered analyses (from old to new) by the started_at field."""
-    return analyses.order_by(Analysis.started_at.desc())
-
-
 def filter_analyses_not_cleaned(analyses: Query, **kwargs) -> Query:
     """Return a query of analyses that have not been cleaned."""
     return analyses.filter(Analysis.cleaned_at.is_(None))
 
 
 def filter_analysis_case_action_is_none(analyses: Query, **kwargs) -> Query:
     """Return a query of analyses that do not have active cases."""
@@ -143,15 +133,14 @@
 
 class AnalysisFilter(Enum):
     """Define Analysis filter functions."""
 
     FILTER_VALID_IN_PRODUCTION: Callable = filter_valid_analyses_in_production
     FILTER_WITH_PIPELINE: Callable = filter_analyses_with_pipeline
     FILTER_COMPLETED: Callable = filter_completed_analyses
-    FILTER_NOT_COMPLETED: Callable = filter_not_completed_analyses
     FILTER_IS_UPLOADED: Callable = filter_uploaded_analyses
     FILTER_IS_NOT_UPLOADED: Callable = filter_not_uploaded_analyses
     FILTER_WITH_DELIVERY_REPORT: Callable = filter_analyses_with_delivery_report
     FILTER_WITHOUT_DELIVERY_REPORT: Callable = filter_analyses_without_delivery_report
     FILTER_REPORT_BY_PIPELINE: Callable = filter_report_analyses_by_pipeline
     FILTER_BY_CASE_ENTRY_ID: Callable = filter_analyses_by_case_entry_id
     FILTER_COMPLETED_AT_AFTER: Callable = filter_analyses_completed_after
@@ -159,8 +148,7 @@
     FILTER_NOT_UPLOADED_TO_VOGUE: Callable = filter_analyses_not_uploaded_to_vogue
     FILTER_IS_NOT_CLEANED: Callable = filter_analyses_not_cleaned
     FILTER_STARTED_AT_BEFORE: Callable = filter_analyses_started_before
     FILTER_BY_STARTED_AT: Callable = filter_analyses_by_started_at
     FILTER_CASE_ACTION_IS_NONE: Callable = filter_analysis_case_action_is_none
     ORDER_BY_UPLOADED_AT: Callable = order_analyses_by_uploaded_at_asc
     ORDER_BY_COMPLETED_AT: Callable = order_analyses_by_completed_at_asc
-    ORDER_BY_STARTED_AT_DESC: Callable = order_analyses_by_started_at_desc
```

### Comparing `cg-32.2.4/cg/store/filters/status_application_filters.py` & `cg-32.2.5/cg/store/filters/status_application_filters.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,36 +6,19 @@
 
 
 def filter_applications_by_tag(applications: Query, tag: str, **kwargs) -> Query:
     """Return application by tag."""
     return applications.filter(Application.tag == tag)
 
 
-def filter_applications_by_prep_category(
-    applications: Query, prep_category: str, **kwargs
-) -> Query:
-    """Return application by prep category."""
-    return applications.filter(Application.prep_category == prep_category)
-
-
-def filter_applications_is_archived(applications: Query, **kwargs) -> Query:
-    """Return application which is archived."""
-    return applications.filter(Application.is_archived.is_(True))
-
-
 def filter_applications_is_not_archived(applications: Query, **kwargs) -> Query:
     """Return application which is not archived."""
     return applications.filter(Application.is_archived.is_(False))
 
 
-def filter_applications_by_entry_id(applications: Query, entry_id: int, **kwargs) -> Query:
-    """Return application by entry id."""
-    return applications.filter(Application.id == entry_id)
-
-
 def filter_applications_is_external(applications: Query, **kwargs) -> Query:
     """Return application which is external."""
     return applications.filter(Application.is_external == True)
 
 
 def filter_applications_is_not_external(applications: Query, **kwargs) -> Query:
     """Return application which is not external."""
@@ -63,11 +46,8 @@
 
 class ApplicationFilter(Enum):
     """Define Application filter functions."""
 
     FILTER_IS_EXTERNAL = filter_applications_is_external
     FILTER_IS_NOT_EXTERNAL = filter_applications_is_not_external
     FILTER_BY_TAG = filter_applications_by_tag
-    FILTER_BY_PREP_CATEGORY = filter_applications_by_prep_category
-    FILTER_IS_ARCHIVED = filter_applications_is_archived
     FILTER_IS_NOT_ARCHIVED = filter_applications_is_not_archived
-    FILTER_BY_ID = filter_applications_by_entry_id
```

### Comparing `cg-32.2.4/cg/store/filters/status_application_version_filters.py` & `cg-32.2.5/cg/store/filters/status_application_version_filters.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,21 +9,14 @@
 def filter_application_versions_by_application_entry_id(
     application_versions: Query, application_entry_id: int, **kwargs
 ) -> Query:
     """Return the application versions given an application entry id."""
     return application_versions.filter(ApplicationVersion.application_id == application_entry_id)
 
 
-def filter_application_versions_by_version(
-    application_versions: Query, version: int, **kwargs
-) -> Query:
-    """Return the application versions given a version."""
-    return application_versions.filter(ApplicationVersion.version == version)
-
-
 def filter_application_versions_before_valid_from(
     application_versions: Query, valid_from: datetime, **kwargs
 ) -> Query:
     """Return the application versions with valid_from before a given valid_from date."""
     return application_versions.filter(ApplicationVersion.valid_from < valid_from)
 
 
@@ -63,9 +56,8 @@
 
 class ApplicationVersionFilter(Enum):
     """Define Application Version filter functions."""
 
     FILTER_BY_APPLICATION_ENTRY_ID = filter_application_versions_by_application_entry_id
     FILTER_BY_ENTRY_ID = filter_application_versions_by_application_version_entry_id
     FILTER_BY_VALID_FROM_BEFORE = filter_application_versions_before_valid_from
-    FILTER_BY_VERSION = filter_application_versions_by_version
     ORDER_BY_VALID_FROM_DESC = order_application_versions_by_valid_from_desc
```

### Comparing `cg-32.2.4/cg/store/filters/status_bed_filters.py` & `cg-32.2.5/cg/store/filters/status_bed_filters.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,33 +2,27 @@
 from typing import List, Optional, Callable
 
 from sqlalchemy.orm import Query
 
 from cg.store.models import Bed
 
 
-def get_beds_by_name(beds: Query, bed_name: str, **kwargs) -> Query:
-    """Return beds by name."""
-    return beds.filter(Bed.name == bed_name)
-
-
 def get_not_archived_beds(beds: Query, **kwargs) -> Query:
     """Return beds not archived."""
     return beds.filter(Bed.is_archived.is_(False))
 
 
 def order_beds_by_name(beds: Query, **kwargs) -> Query:
     """Return beds ordered by name."""
     return beds.order_by(Bed.name)
 
 
 class BedFilter(Enum):
     """Define BED filter functions."""
 
-    FILTER_BY_NAME: Callable = get_beds_by_name
     FILTER_NOT_ARCHIVED: Callable = get_not_archived_beds
     ORDER_BY_NAME: Callable = order_beds_by_name
 
 
 def apply_bed_filter(
     beds: Query,
     filter_functions: List[Callable],
```

### Comparing `cg-32.2.4/cg/store/filters/status_bed_version_filters.py` & `cg-32.2.5/cg/store/filters/status_bed_version_filters.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/store/filters/status_case_filters.py` & `cg-32.2.5/cg/store/filters/status_case_filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,20 +37,14 @@
 
 def get_older_cases_by_creation_date(cases: Query, creation_date: datetime, **kwargs) -> Query:
     """Return older cases compared to date."""
     cases = cases.filter(Family.created_at < creation_date)
     return cases.order_by(Family.created_at.asc())
 
 
-def get_newer_cases_by_creation_date(cases: Query, creation_date: datetime, **kwargs) -> Query:
-    """Return newer cases compared to date."""
-    cases = cases.filter(Family.created_at > creation_date)
-    return cases.order_by(Family.created_at.asc())
-
-
 def get_cases_with_pipeline(cases: Query, pipeline: Pipeline = None, **kwargs) -> Query:
     """Return cases with pipeline."""
     return cases.filter(Family.data_analysis == pipeline) if pipeline else cases
 
 
 def get_cases_with_loqusdb_supported_pipeline(
     cases: Query, pipeline: Pipeline = None, **kwargs
@@ -246,15 +240,14 @@
 
 class CaseFilter(Enum):
     """Define case filters."""
 
     GET_HAS_SEQUENCE: Callable = get_cases_has_sequence
     GET_HAS_INACTIVE_ANALYSIS: Callable = get_inactive_analysis_cases
     GET_OLD_BY_CREATION_DATE: Callable = get_older_cases_by_creation_date
-    GET_NEW_BY_CREATION_DATE: Callable = get_newer_cases_by_creation_date
     GET_NEW_BY_ORDER_DATE: Callable = get_newer_cases_by_order_date
     GET_WITH_PIPELINE: Callable = get_cases_with_pipeline
     GET_WITH_LOQUSDB_SUPPORTED_PIPELINE: Callable = get_cases_with_loqusdb_supported_pipeline
     GET_WITH_LOQUSDB_SUPPORTED_SEQUENCING_METHOD: Callable = (
         get_cases_with_loqusdb_supported_sequencing_method
     )
     GET_FOR_ANALYSIS: Callable = get_cases_for_analysis
```

### Comparing `cg-32.2.4/cg/store/filters/status_case_sample_filters.py` & `cg-32.2.5/cg/store/filters/status_case_sample_filters.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,19 +13,14 @@
 
 
 def get_cases_with_sample_by_internal_id(case_samples: Query, sample_internal_id: str, **kwargs):
     """Return cases associated with a sample internal id."""
     return case_samples.filter(Sample.internal_id == sample_internal_id)
 
 
-def get_cases_with_sample_by_entry_id(case_samples: Query, sample_entry_id: int, **kwargs) -> Query:
-    """Return cases associated with a sample entry id."""
-    return case_samples.filter(Sample.id == sample_entry_id)
-
-
 def apply_case_sample_filter(
     filter_functions: List[Callable],
     case_samples: Query,
     case_internal_id: Optional[str] = None,
     sample_entry_id: Optional[int] = None,
     sample_internal_id: Optional[str] = None,
 ) -> Query:
@@ -42,8 +37,7 @@
 
 
 class CaseSampleFilter(Enum):
     """Define CaseSample filter functions."""
 
     GET_SAMPLES_IN_CASE_BY_INTERNAL_ID: Callable = get_samples_in_case_by_internal_id
     GET_CASES_WITH_SAMPLE_BY_INTERNAL_ID: Callable = get_cases_with_sample_by_internal_id
-    GET_CASES_WITH_SAMPLE_BY_ENTRY_ID: Callable = get_cases_with_sample_by_entry_id
```

### Comparing `cg-32.2.4/cg/store/filters/status_collaboration_filters.py` & `cg-32.2.5/cg/store/filters/status_collaboration_filters.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/store/filters/status_customer_filters.py` & `cg-32.2.5/cg/store/filters/status_customer_filters.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/store/filters/status_flow_cell_filters.py` & `cg-32.2.5/cg/store/filters/status_flow_cell_filters.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/store/filters/status_invoice_filters.py` & `cg-32.2.5/cg/store/filters/status_invoice_filters.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/store/filters/status_organism_filters.py` & `cg-32.2.5/cg/store/filters/status_organism_filters.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/store/filters/status_panel_filters.py` & `cg-32.2.5/cg/store/filters/status_panel_filters.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/store/filters/status_pool_filters.py` & `cg-32.2.5/cg/store/filters/status_pool_filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,19 +60,14 @@
 
 
 def filter_pools_do_invoice(pools: Query, **kwargs) -> Query:
     """Return pools marked for invoicing."""
     return pools.filter(Pool.no_invoice.is_(False))
 
 
-def filter_pools_do_not_invoice(pools: Query, **kwargs) -> Query:
-    """Return pools marked to skip invoicing."""
-    return pools.filter(Pool.no_invoice.is_(True))
-
-
 def filter_pools_by_customer(pools: Query, customer: Customer, **kwargs) -> Query:
     """Return pools by customer id."""
     return pools.filter(Pool.customer == customer)
 
 
 def apply_pool_filter(
     filter_functions: List[Callable],
@@ -109,12 +104,11 @@
     FILTER_IS_RECEIVED: Callable = filter_pools_is_received
     FILTER_IS_NOT_RECEIVED: Callable = filter_pools_is_not_received
     FILTER_IS_DELIVERED: Callable = filter_pools_is_delivered
     FILTER_IS_NOT_DELIVERED: Callable = filter_pools_is_not_delivered
     FILTER_BY_INVOICE_ID: Callable = filter_pools_by_invoice_id
     FILTER_WITHOUT_INVOICE_ID: Callable = filter_pools_without_invoice_id
     FILTER_DO_INVOICE: Callable = filter_pools_do_invoice
-    FILTER_DO_NOT_INVOICE: Callable = filter_pools_do_not_invoice
     FILTER_BY_CUSTOMER_ID: Callable = filter_pools_by_customer_id
     FILTER_BY_NAME_ENQUIRY: Callable = filter_pools_by_name_enquiry
     FILTER_BY_ORDER_ENQUIRY: Callable = filter_pools_by_order_enquiry
     FILTER_BY_CUSTOMER: Callable = filter_pools_by_customer
```

### Comparing `cg-32.2.4/cg/store/filters/status_sample_filters.py` & `cg-32.2.5/cg/store/filters/status_sample_filters.py`

 * *Files 12% similar despite different names*

```diff
@@ -59,19 +59,14 @@
 
 
 def filter_samples_is_not_down_sampled(samples: Query, **kwargs) -> Query:
     """Return samples that are not down sampled."""
     return samples.filter(Sample.downsampled_to.is_(None))
 
 
-def filter_samples_is_down_sampled(samples: Query, **kwargs) -> Query:
-    """Return samples that are down sampled."""
-    return samples.filter(Sample.downsampled_to.isnot(None))
-
-
 def filter_samples_is_sequenced(samples: Query, **kwargs) -> Query:
     """Return samples that are sequenced."""
     return samples.filter(Sample.sequenced_at.isnot(None))
 
 
 def filter_samples_is_not_sequenced(samples: Query, **kwargs) -> Query:
     """Return samples that are not sequenced."""
@@ -79,31 +74,21 @@
 
 
 def filter_samples_do_invoice(samples: Query, **kwargs) -> Query:
     """Return samples that should be invoiced."""
     return samples.filter(Sample.no_invoice.is_(False))
 
 
-def filter_samples_do_not_invoice(samples: Query, **kwargs) -> Query:
-    """Return samples marked to skip invoicing."""
-    return samples.filter(Sample.no_invoice.is_(True))
-
-
 def filter_samples_by_entry_customer_ids(
     samples: Query, customer_entry_ids: List[int], **kwargs
 ) -> Query:
     """Return samples by customer id."""
     return samples.filter(Sample.customer_id.in_(customer_entry_ids))
 
 
-def filter_samples_by_customer_name(samples: Query, customer_name: str, **kwargs) -> Query:
-    """Return samples by customer name."""
-    return samples.filter(Sample.customer_name == customer_name)
-
-
 def filter_samples_is_received(samples: Query, **kwargs) -> Query:
     """Return samples that are received."""
     return samples.filter(Sample.received_at.isnot(None))
 
 
 def filter_samples_is_not_received(samples: Query, **kwargs) -> Query:
     """Return samples that are not received."""
@@ -131,19 +116,14 @@
 
 
 def filter_samples_is_not_tumour(samples: Query, **kwargs) -> Query:
     """Return samples that are not tumour."""
     return samples.filter(Sample.is_tumour.is_(False))
 
 
-def filter_samples_by_name_pattern(samples: Query, name_pattern: str, **kwargs) -> Query:
-    """Return samples matching the name pattern."""
-    return samples.filter(Sample.name.like(f"%{name_pattern}%"))
-
-
 def filter_samples_by_internal_id_pattern(
     samples: Query, internal_id_pattern: str, **kwargs
 ) -> Query:
     """Return samples matching the internal id pattern."""
     return samples.filter(Sample.internal_id.like(f"%{internal_id_pattern}%"))
 
 
@@ -226,28 +206,24 @@
     FILTER_WITHOUT_LOQUSDB_ID: Callable = filter_samples_without_loqusdb_id
     FILTER_BY_ENTRY_ID: Callable = filter_samples_by_entry_id
     FILTER_IS_DELIVERED: Callable = filter_samples_is_delivered
     FILTER_IS_NOT_DELIVERED: Callable = filter_samples_is_not_delivered
     FILTER_BY_INVOICE_ID: Callable = filter_samples_by_invoice_id
     FILTER_HAS_NO_INVOICE_ID: Callable = filter_samples_without_invoice_id
     FILTER_IS_NOT_DOWN_SAMPLED: Callable = filter_samples_is_not_down_sampled
-    FILTER_IS_DOWN_SAMPLED: Callable = filter_samples_is_down_sampled
     FILTER_IS_SEQUENCED: Callable = filter_samples_is_sequenced
     FILTER_IS_NOT_SEQUENCED: Callable = filter_samples_is_not_sequenced
     FILTER_DO_INVOICE: Callable = filter_samples_do_invoice
-    FILTER_DO_NOT_INVOICE: Callable = filter_samples_do_not_invoice
-    FILTER_BY_CUSTOMER_NAME: Callable = filter_samples_by_customer_name
     FILTER_BY_CUSTOMER_ENTRY_IDS: Callable = filter_samples_by_entry_customer_ids
     FILTER_IS_RECEIVED: Callable = filter_samples_is_received
     FILTER_IS_NOT_RECEIVED: Callable = filter_samples_is_not_received
     FILTER_IS_PREPARED: Callable = filter_samples_is_prepared
     FILTER_IS_NOT_PREPARED: Callable = filter_samples_is_not_prepared
     FILTER_BY_SAMPLE_NAME: Callable = filter_samples_by_name
     FILTER_BY_SUBJECT_ID: Callable = filter_samples_by_subject_id
     FILTER_IS_TUMOUR: Callable = filter_samples_is_tumour
     FILTER_IS_NOT_TUMOUR: Callable = filter_samples_is_not_tumour
-    FILTER_BY_NAME_PATTERN: Callable = filter_samples_by_name_pattern
     FILTER_BY_INTERNAL_ID_PATTERN: Callable = filter_samples_by_internal_id_pattern
     FILTER_BY_CUSTOMER: Callable = filter_samples_by_customer
     FILTER_BY_INTERNAL_ID_OR_NAME_SEARCH: Callable = filter_samples_by_internal_id_or_name_search
     FILTER_BY_IDENTIFIER_NAME_AND_VALUE: Callable = filter_samples_by_identifier_name_and_value
     ORDER_BY_CREATED_AT_DESC: Callable = order_samples_by_created_at_desc
```

### Comparing `cg-32.2.4/cg/store/filters/status_user_filters.py` & `cg-32.2.5/cg/store/filters/status_user_filters.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/store/models.py` & `cg-32.2.5/cg/store/models.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/utils/checksum/checksum.py` & `cg-32.2.5/cg/utils/checksum/checksum.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/utils/commands.py` & `cg-32.2.5/cg/utils/commands.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/utils/date.py` & `cg-32.2.5/cg/utils/date.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/utils/dict.py` & `cg-32.2.5/cg/utils/dict.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/utils/dispatcher.py` & `cg-32.2.5/cg/utils/dispatcher.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/utils/email.py` & `cg-32.2.5/cg/utils/email.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg/utils/flask/enum.py` & `cg-32.2.5/cg/utils/flask/enum.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,14 @@
 from enum import Enum, EnumMeta
 
 from flask_admin.form import Select2Field
 
 
 class EnumField:
     @staticmethod
-    def get_name(enum_instance):
-        return enum_instance.name
-
-    @staticmethod
     def get_value(enum_instance):
         return enum_instance.value
 
     default_label_function = get_value
 
     def apply_choices(
         self, enum_class: EnumMeta, label_function=default_label_function, kwargs=None
```

### Comparing `cg-32.2.4/cg/utils/utils.py` & `cg-32.2.5/cg/utils/utils.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/cg.egg-info/PKG-INFO` & `cg-32.2.5/cg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cg
-Version: 32.2.4
+Version: 32.2.5
 Summary: Clinical Genomics command center
 Home-page: https://github.com/Clinical-Genomics/cg
 Author: Clinical Genomics
 Author-email: support@clinicalgenomics.se
 License: UNKNOWN
 Description: 
         # cg
```

### Comparing `cg-32.2.4/cg.egg-info/SOURCES.txt` & `cg-32.2.5/cg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/requirements.txt` & `cg-32.2.5/requirements.txt`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/setup.py` & `cg-32.2.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     with io.open(os.path.join(HERE, "README.md"), encoding="utf-8") as f:
         LONG_DESCRIPTION = "\n" + f.read()
 except FileNotFoundError:
     LONG_DESCRIPTION = DESCRIPTION
 
 setup(
     name=NAME,
-    version="32.2.4",
+    version="32.2.5",
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     author=AUTHOR,
     author_email=EMAIL,
     url=URL,
     include_package_data=True,
```

### Comparing `cg-32.2.4/tests/apps/cgstats/conftest.py` & `cg-32.2.5/tests/apps/cgstats/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/apps/cgstats/crud/test_create_novaseq.py` & `cg-32.2.5/tests/apps/cgstats/crud/test_create_novaseq.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/apps/cgstats/crud/test_delete.py` & `cg-32.2.5/tests/apps/cgstats/crud/test_delete.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/apps/cgstats/parsers/test_conversion_stats.py` & `cg-32.2.5/tests/apps/cgstats/parsers/test_conversion_stats.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/apps/cgstats/parsers/test_demux_stats.py` & `cg-32.2.5/tests/apps/cgstats/parsers/test_demux_stats.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/apps/cgstats/parsers/test_run_info.py` & `cg-32.2.5/tests/apps/cgstats/parsers/test_run_info.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/apps/cgstats/test_cgstats_create.py` & `cg-32.2.5/tests/apps/cgstats/test_cgstats_create.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/apps/cgstats/test_stats.py` & `cg-32.2.5/tests/apps/cgstats/test_stats.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/apps/conftest.py` & `cg-32.2.5/tests/apps/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/apps/coverage/test_coverage.py` & `cg-32.2.5/tests/apps/coverage/test_coverage.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/apps/crunchy/conftest.py` & `cg-32.2.5/tests/apps/crunchy/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/apps/crunchy/test_compress_fastq.py` & `cg-32.2.5/tests/apps/crunchy/test_compress_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/apps/crunchy/test_config.py` & `cg-32.2.5/tests/apps/crunchy/test_config.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/apps/crunchy/test_crunchy.py` & `cg-32.2.5/tests/apps/crunchy/test_crunchy.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/apps/crunchy/test_spring_decompression.py` & `cg-32.2.5/tests/apps/crunchy/test_spring_decompression.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/apps/demultiplex/conftest.py` & `cg-32.2.5/tests/apps/demultiplex/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/apps/demultiplex/test_convert_to_sample_sheet.py` & `cg-32.2.5/tests/apps/demultiplex/test_convert_to_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/apps/demultiplex/test_demultiplex_api.py` & `cg-32.2.5/tests/apps/demultiplex/test_demultiplex_api.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/apps/demultiplex/test_sample_sheet.py` & `cg-32.2.5/tests/apps/demultiplex/test_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/apps/demultiplex/test_validate_sample_sheet.py` & `cg-32.2.5/tests/apps/demultiplex/test_validate_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/apps/gens/test_gens_api.py` & `cg-32.2.5/tests/apps/gens/test_gens_api.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/apps/gt/conftest.py` & `cg-32.2.5/tests/apps/gt/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/apps/gt/test_gt_api.py` & `cg-32.2.5/tests/apps/gt/test_gt_api.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/apps/hk/conftest.py` & `cg-32.2.5/tests/apps/hk/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/apps/hk/test__getattr__.py` & `cg-32.2.5/tests/apps/hk/test__getattr__.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/apps/hk/test_add_file.py` & `cg-32.2.5/tests/apps/hk/test_add_file.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/apps/hk/test_bundles.py` & `cg-32.2.5/tests/apps/hk/test_bundles.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/apps/hk/test_core.py` & `cg-32.2.5/tests/apps/hk/test_core.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/apps/hk/test_file.py` & `cg-32.2.5/tests/apps/hk/test_file.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/apps/hk/test_version.py` & `cg-32.2.5/tests/apps/hk/test_version.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/apps/lims/conftest.py` & `cg-32.2.5/tests/apps/lims/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/apps/lims/test_api.py` & `cg-32.2.5/tests/apps/lims/test_api.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/apps/loqus/conftest.py` & `cg-32.2.5/tests/apps/loqus/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/apps/loqus/test_loqusdb_api.py` & `cg-32.2.5/tests/apps/loqus/test_loqusdb_api.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/apps/madeline/conftest.py` & `cg-32.2.5/tests/apps/madeline/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/apps/madeline/test_madeline.py` & `cg-32.2.5/tests/apps/madeline/test_madeline.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/apps/mip/conftest.py` & `cg-32.2.5/tests/apps/mip/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/apps/mip/test_config_mip.py` & `cg-32.2.5/tests/apps/mip/test_config_mip.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/apps/mutacc_auto/conftest.py` & `cg-32.2.5/tests/apps/mutacc_auto/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/apps/mutacc_auto/test_mutacc_auto.py` & `cg-32.2.5/tests/apps/mutacc_auto/test_mutacc_auto.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/apps/orderform/conftest.py` & `cg-32.2.5/tests/apps/orderform/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/apps/orderform/test_excel_orderform_parser.py` & `cg-32.2.5/tests/apps/orderform/test_excel_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/apps/orderform/test_excel_sample_schema.py` & `cg-32.2.5/tests/apps/orderform/test_excel_sample_schema.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/apps/orderform/test_json_orderform_parser.py` & `cg-32.2.5/tests/apps/orderform/test_json_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/apps/orderform/test_orderform_parser.py` & `cg-32.2.5/tests/apps/orderform/test_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/apps/scout/conftest.py` & `cg-32.2.5/tests/apps/scout/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/apps/scout/test_get_causative_variants.py` & `cg-32.2.5/tests/apps/scout/test_get_causative_variants.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/apps/scout/test_get_scout_cases.py` & `cg-32.2.5/tests/apps/scout/test_get_scout_cases.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/apps/scout/test_scout_load_config.py` & `cg-32.2.5/tests/apps/scout/test_scout_load_config.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/apps/scout/test_scout_models.py` & `cg-32.2.5/tests/apps/scout/test_scout_models.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/apps/sequencing_metrics_parser/conftest.py` & `cg-32.2.5/tests/apps/sequencing_metrics_parser/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/apps/sequencing_metrics_parser/parsers/conftest.py` & `cg-32.2.5/tests/apps/sequencing_metrics_parser/parsers/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/apps/sequencing_metrics_parser/parsers/test_bcl2fastq_parser.py` & `cg-32.2.5/tests/apps/sequencing_metrics_parser/parsers/test_bcl2fastq_parser.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/apps/sequencing_metrics_parser/parsers/test_bcl2fastq_to_sequencing_statistics.py` & `cg-32.2.5/tests/apps/sequencing_metrics_parser/parsers/test_bcl2fastq_to_sequencing_statistics.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/apps/sequencing_metrics_parser/parsers/test_bcl_convert_to_sequencing_statistics.py` & `cg-32.2.5/tests/apps/sequencing_metrics_parser/parsers/test_bcl_convert_to_sequencing_statistics.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/apps/sequencing_metrics_parser/parsers/test_bclconvert.py` & `cg-32.2.5/tests/apps/sequencing_metrics_parser/parsers/test_bclconvert.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/apps/sequencing_metrics_parser/test_sequencing_metrics_calculator.py` & `cg-32.2.5/tests/apps/sequencing_metrics_parser/test_sequencing_metrics_calculator.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/apps/slurm/conftest.py` & `cg-32.2.5/tests/apps/slurm/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/apps/slurm/test_slurm_api.py` & `cg-32.2.5/tests/apps/slurm/test_slurm_api.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/apps/test_apps_environ.py` & `cg-32.2.5/tests/apps/test_apps_environ.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/apps/test_osticket.py` & `cg-32.2.5/tests/apps/test_osticket.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/apps/vogue/conftest.py` & `cg-32.2.5/tests/apps/vogue/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/apps/vogue/test_vogue_api.py` & `cg-32.2.5/tests/apps/vogue/test_vogue_api.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/add/test_cli_add.py` & `cg-32.2.5/tests/cli/add/test_cli_add.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/add/test_cli_add_customer.py` & `cg-32.2.5/tests/cli/add/test_cli_add_customer.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/add/test_cli_add_family.py` & `cg-32.2.5/tests/cli/add/test_cli_add_family.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/add/test_cli_add_relationship.py` & `cg-32.2.5/tests/cli/add/test_cli_add_relationship.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/add/test_cli_add_sample.py` & `cg-32.2.5/tests/cli/add/test_cli_add_sample.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/backup/conftest.py` & `cg-32.2.5/tests/cli/backup/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/backup/test_backup_command.py` & `cg-32.2.5/tests/cli/backup/test_backup_command.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/clean/conftest.py` & `cg-32.2.5/tests/cli/clean/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/clean/test_balsamic_clean.py` & `cg-32.2.5/tests/cli/clean/test_balsamic_clean.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/clean/test_clean_hk_bundle_files.py` & `cg-32.2.5/tests/cli/clean/test_clean_hk_bundle_files.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/clean/test_hk_bundle_files.py` & `cg-32.2.5/tests/cli/clean/test_hk_bundle_files.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/clean/test_hk_case_bundle_files.py` & `cg-32.2.5/tests/cli/clean/test_hk_case_bundle_files.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/clean/test_microbial_clean.py` & `cg-32.2.5/tests/cli/clean/test_microbial_clean.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/clean/test_rsync_past_run_dirs.py` & `cg-32.2.5/tests/cli/clean/test_rsync_past_run_dirs.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/compress/conftest.py` & `cg-32.2.5/tests/cli/compress/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/compress/test_cli_compress_fastq.py` & `cg-32.2.5/tests/cli/compress/test_cli_compress_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/compress/test_cli_decompress_spring.py` & `cg-32.2.5/tests/cli/compress/test_cli_decompress_spring.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/compress/test_compress_helpers.py` & `cg-32.2.5/tests/cli/compress/test_compress_helpers.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/compress/test_store_fastq.py` & `cg-32.2.5/tests/cli/compress/test_store_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/conftest.py` & `cg-32.2.5/tests/cli/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/delete/test_cli_delete_case.py` & `cg-32.2.5/tests/cli/delete/test_cli_delete_case.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/delete/test_cli_delete_cases.py` & `cg-32.2.5/tests/cli/delete/test_cli_delete_cases.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/deliver/conftest.py` & `cg-32.2.5/tests/cli/deliver/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/deliver/test_deliver_base.py` & `cg-32.2.5/tests/cli/deliver/test_deliver_base.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/deliver/test_rsync_base.py` & `cg-32.2.5/tests/cli/deliver/test_rsync_base.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/deliver/test_run_deliver_cmd.py` & `cg-32.2.5/tests/cli/deliver/test_run_deliver_cmd.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/demultiplex/conftest.py` & `cg-32.2.5/tests/cli/demultiplex/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/demultiplex/test_add_flowcell.py` & `cg-32.2.5/tests/cli/demultiplex/test_add_flowcell.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/demultiplex/test_create_sample_sheet.py` & `cg-32.2.5/tests/cli/demultiplex/test_create_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/demultiplex/test_demultiplex_flowcell.py` & `cg-32.2.5/tests/cli/demultiplex/test_demultiplex_flowcell.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/demultiplex/test_finish_demux.py` & `cg-32.2.5/tests/cli/demultiplex/test_finish_demux.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/demultiplex/test_stats_command.py` & `cg-32.2.5/tests/cli/demultiplex/test_stats_command.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/demultiplex/test_validate_sample_sheet.py` & `cg-32.2.5/tests/cli/demultiplex/test_validate_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/generate/report/conftest.py` & `cg-32.2.5/tests/cli/generate/report/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/generate/report/test_cli_delivery_report.py` & `cg-32.2.5/tests/cli/generate/report/test_cli_delivery_report.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/generate/report/test_utils.py` & `cg-32.2.5/tests/cli/generate/report/test_utils.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/generate/test_cli_base.py` & `cg-32.2.5/tests/cli/generate/test_cli_base.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/get/test_cli_get.py` & `cg-32.2.5/tests/cli/get/test_cli_get.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/get/test_cli_get_analysis.py` & `cg-32.2.5/tests/cli/get/test_cli_get_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/get/test_cli_get_case.py` & `cg-32.2.5/tests/cli/get/test_cli_get_case.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/get/test_cli_get_flow_cell.py` & `cg-32.2.5/tests/cli/get/test_cli_get_flow_cell.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/get/test_cli_get_sample.py` & `cg-32.2.5/tests/cli/get/test_cli_get_sample.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/set/conftest.py` & `cg-32.2.5/tests/cli/set/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/set/test_cli_set_case.py` & `cg-32.2.5/tests/cli/set/test_cli_set_case.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/set/test_cli_set_cases.py` & `cg-32.2.5/tests/cli/set/test_cli_set_cases.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/set/test_cli_set_flowcell.py` & `cg-32.2.5/tests/cli/set/test_cli_set_flowcell.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/set/test_cli_set_list_keys.py` & `cg-32.2.5/tests/cli/set/test_cli_set_list_keys.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/set/test_cli_set_sample.py` & `cg-32.2.5/tests/cli/set/test_cli_set_sample.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/set/test_cli_set_samples.py` & `cg-32.2.5/tests/cli/set/test_cli_set_samples.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/store/test_fastq.py` & `cg-32.2.5/tests/cli/store/test_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/test_base.py` & `cg-32.2.5/tests/cli/test_base.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/test_clean.py` & `cg-32.2.5/tests/cli/test_clean.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/upload/conftest.py` & `cg-32.2.5/tests/cli/upload/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/upload/test_cli_scout.py` & `cg-32.2.5/tests/cli/upload/test_cli_scout.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/upload/test_cli_upload.py` & `cg-32.2.5/tests/cli/upload/test_cli_upload.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/upload/test_cli_upload_auto.py` & `cg-32.2.5/tests/cli/upload/test_cli_upload_auto.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/upload/test_cli_upload_delivery_report.py` & `cg-32.2.5/tests/cli/upload/test_cli_upload_delivery_report.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/upload/test_cli_upload_fastq.py` & `cg-32.2.5/tests/cli/upload/test_cli_upload_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/upload/test_cli_upload_genotype.py` & `cg-32.2.5/tests/cli/upload/test_cli_upload_genotype.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/upload/test_cli_upload_gens.py` & `cg-32.2.5/tests/cli/upload/test_cli_upload_gens.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/upload/test_cli_upload_nipt.py` & `cg-32.2.5/tests/cli/upload/test_cli_upload_nipt.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/upload/test_cli_upload_nipt_ftp.py` & `cg-32.2.5/tests/cli/upload/test_cli_upload_nipt_ftp.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/upload/test_cli_upload_nipt_statina.py` & `cg-32.2.5/tests/cli/upload/test_cli_upload_nipt_statina.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/upload/test_cli_upload_observations.py` & `cg-32.2.5/tests/cli/upload/test_cli_upload_observations.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/upload/test_cli_upload_vogue.py` & `cg-32.2.5/tests/cli/upload/test_cli_upload_vogue.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/workflow/balsamic/conftest.py` & `cg-32.2.5/tests/cli/workflow/balsamic/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/workflow/balsamic/test_cli_balsamic_config_case.py` & `cg-32.2.5/tests/cli/workflow/balsamic/test_cli_balsamic_config_case.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/workflow/balsamic/test_compound_commands.py` & `cg-32.2.5/tests/cli/workflow/balsamic/test_compound_commands.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/workflow/balsamic/test_link.py` & `cg-32.2.5/tests/cli/workflow/balsamic/test_link.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/workflow/balsamic/test_report_deliver.py` & `cg-32.2.5/tests/cli/workflow/balsamic/test_report_deliver.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/workflow/balsamic/test_run.py` & `cg-32.2.5/tests/cli/workflow/balsamic/test_run.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/workflow/balsamic/test_store_housekeeper.py` & `cg-32.2.5/tests/cli/workflow/balsamic/test_store_housekeeper.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/workflow/conftest.py` & `cg-32.2.5/tests/cli/workflow/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/workflow/fastq/test_fastq_base.py` & `cg-32.2.5/tests/cli/workflow/fastq/test_fastq_base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,33 @@
 import logging
 from datetime import datetime
 
 from cg.cli.workflow.fastq.base import store_fastq_analysis, store_available_fastq_analysis
-from cg.store.models import Family, Sample
+from cg.store.models import Analysis, Family, Sample
 
 
 def test_store_fastq_analysis(caplog, case_id: str, cli_runner, fastq_context):
     """Test for CLI command creating an analysis object for a fastq case"""
     # GIVEN a fastq context
     caplog.set_level(logging.INFO)
     case_obj: Family = fastq_context.status_db.get_case_by_internal_id(internal_id=case_id)
     case_obj.analyses = []
 
     # WHEN the store_fastq_analysis command is invoked
     cli_runner.invoke(store_fastq_analysis, [case_id], obj=fastq_context)
 
     # THEN the run command should be reached
-    assert len(fastq_context.status_db.get_analyses_by_case_entry_id(case_entry_id=case_obj.id)) > 0
+    assert (
+        len(
+            fastq_context.status_db._get_query(table=Analysis)
+            .filter(Analysis.family_id == case_obj.id)
+            .all()
+        )
+        > 0
+    )
 
 
 def test_store_available_fastq_analysis(
     caplog, case_id: str, cli_runner, fastq_context, sample_id: str
 ):
     """Test for CLI command creating an analysis object for all fastq cases to be delivered"""
     caplog.set_level(logging.INFO)
```

### Comparing `cg-32.2.4/tests/cli/workflow/fluffy/conftest.py` & `cg-32.2.5/tests/cli/workflow/fluffy/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/workflow/fluffy/test_cli_create_samplesheet.py` & `cg-32.2.5/tests/cli/workflow/fluffy/test_cli_create_samplesheet.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/workflow/fluffy/test_cli_link.py` & `cg-32.2.5/tests/cli/workflow/fluffy/test_cli_link.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/workflow/fluffy/test_cli_run.py` & `cg-32.2.5/tests/cli/workflow/fluffy/test_cli_run.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/workflow/fluffy/test_cli_start.py` & `cg-32.2.5/tests/cli/workflow/fluffy/test_cli_start.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/workflow/fluffy/test_cli_store.py` & `cg-32.2.5/tests/cli/workflow/fluffy/test_cli_store.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/workflow/microsalt/conftest.py` & `cg-32.2.5/tests/cli/workflow/microsalt/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/workflow/microsalt/snapshots/snap_test_microsalt_case_config.py` & `cg-32.2.5/tests/cli/workflow/microsalt/snapshots/snap_test_microsalt_case_config.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/workflow/microsalt/test_microsalt_case_config.py` & `cg-32.2.5/tests/cli/workflow/microsalt/test_microsalt_case_config.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/workflow/microsalt/test_microsalt_run.py` & `cg-32.2.5/tests/cli/workflow/microsalt/test_microsalt_run.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/workflow/mip/conftest.py` & `cg-32.2.5/tests/cli/workflow/mip/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,28 +157,24 @@
 
 def setup_mocks(
     mocker,
     can_at_least_one_sample_be_decompressed: bool = False,
     case_to_analyze: Family = None,
     decompress_spring: bool = False,
     has_latest_analysis_started: bool = False,
-    is_dna_only_case: bool = False,
     is_spring_decompression_needed: bool = False,
     is_spring_decompression_running: bool = False,
 ) -> None:
     """Helper function to setup the necessary mocks for the decompression logics."""
     mocker.patch.object(StatusHandler, "cases_to_analyze")
     StatusHandler.cases_to_analyze.return_value = [case_to_analyze]
 
     mocker.patch.object(PrepareFastqAPI, "is_spring_decompression_needed")
     PrepareFastqAPI.is_spring_decompression_needed.return_value = is_spring_decompression_needed
 
-    mocker.patch.object(MipAnalysisAPI, "is_dna_only_case")
-    MipAnalysisAPI.is_dna_only_case.return_value = is_dna_only_case
-
     mocker.patch.object(TrailblazerAPI, "has_latest_analysis_started")
     TrailblazerAPI.has_latest_analysis_started.return_value = has_latest_analysis_started
 
     mocker.patch.object(PrepareFastqAPI, "can_at_least_one_sample_be_decompressed")
     PrepareFastqAPI.can_at_least_one_sample_be_decompressed.return_value = (
         can_at_least_one_sample_be_decompressed
     )
```

### Comparing `cg-32.2.4/tests/cli/workflow/mip/test_cli_mip_base.py` & `cg-32.2.5/tests/cli/workflow/mip/test_cli_mip_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,14 @@
     # GIVEN there is spring files that can be decompressed
     # GIVEN there is flow cells for the case
     setup_mocks(
         can_at_least_one_sample_be_decompressed=True,
         case_to_analyze=case,
         decompress_spring=True,
         has_latest_analysis_started=False,
-        is_dna_only_case=True,
         is_spring_decompression_needed=True,
         mocker=mocker,
     )
 
     # WHEN an MIP analysis is started
     result = cli_runner.invoke(start_available, obj=mip_dna_context)
 
@@ -67,15 +66,14 @@
     # GIVEN there is spring files that can be decompressed
     # GIVEN there is flow cells for the case
     setup_mocks(
         can_at_least_one_sample_be_decompressed=True,
         case_to_analyze=case,
         decompress_spring=False,
         has_latest_analysis_started=False,
-        is_dna_only_case=True,
         is_spring_decompression_needed=True,
         mocker=mocker,
     )
 
     # WHEN an MIP analysis is started
     result = cli_runner.invoke(start_available, obj=mip_dna_context)
 
@@ -104,15 +102,14 @@
     # GIVEN spring decompression is not running
     # GIVEN there is flow cells for the case
     setup_mocks(
         can_at_least_one_sample_be_decompressed=False,
         case_to_analyze=case,
         decompress_spring=False,
         has_latest_analysis_started=False,
-        is_dna_only_case=True,
         is_spring_decompression_needed=True,
         is_spring_decompression_running=False,
         mocker=mocker,
     )
 
     # WHEN an MIP analysis is started
     result = cli_runner.invoke(start_available, obj=mip_dna_context)
@@ -142,15 +139,14 @@
     # GIVEN spring decompression is running
     # GIVEN there is flow cells for the case
     setup_mocks(
         can_at_least_one_sample_be_decompressed=False,
         case_to_analyze=case,
         decompress_spring=False,
         has_latest_analysis_started=False,
-        is_dna_only_case=True,
         is_spring_decompression_needed=True,
         is_spring_decompression_running=True,
         mocker=mocker,
     )
 
     # WHEN an MIP analysis is started
     result = cli_runner.invoke(start_available, obj=mip_dna_context)
@@ -181,15 +177,14 @@
     # GIVEN a panel file is created
     # GIVEN there is flow cells for the case
     setup_mocks(
         can_at_least_one_sample_be_decompressed=False,
         case_to_analyze=case,
         decompress_spring=False,
         has_latest_analysis_started=False,
-        is_dna_only_case=True,
         is_spring_decompression_needed=False,
         is_spring_decompression_running=False,
         mocker=mocker,
     )
 
     # WHEN MIP analysis is started
     result = cli_runner.invoke(start, [case.internal_id, "--dry-run"], obj=mip_dna_context)
```

### Comparing `cg-32.2.4/tests/cli/workflow/mip/test_cli_mip_dna_config_case.py` & `cg-32.2.5/tests/cli/workflow/mip/test_cli_mip_dna_config_case.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/workflow/mip/test_cli_mip_dna_run.py` & `cg-32.2.5/tests/cli/workflow/mip/test_cli_mip_dna_run.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/workflow/mip/test_cli_mip_dna_start.py` & `cg-32.2.5/tests/cli/workflow/mip/test_cli_mip_dna_start.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/workflow/mip/test_cli_mip_rna_config_case.py` & `cg-32.2.5/tests/cli/workflow/mip/test_cli_mip_rna_config_case.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/workflow/mip/test_cli_mip_rna_link.py` & `cg-32.2.5/tests/cli/workflow/mip/test_cli_mip_rna_link.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/workflow/mip/test_cli_mip_rna_run.py` & `cg-32.2.5/tests/cli/workflow/mip/test_cli_mip_rna_run.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/workflow/mip/test_cli_mip_store.py` & `cg-32.2.5/tests/cli/workflow/mip/test_cli_mip_store.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/workflow/rnafusion/conftest.py` & `cg-32.2.5/tests/cli/workflow/rnafusion/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/workflow/rnafusion/test_cli_rnafusion_compound_commands.py` & `cg-32.2.5/tests/cli/workflow/rnafusion/test_cli_rnafusion_compound_commands.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/workflow/rnafusion/test_cli_rnafusion_config_case.py` & `cg-32.2.5/tests/cli/workflow/rnafusion/test_cli_rnafusion_config_case.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/workflow/rnafusion/test_cli_rnafusion_metrics_deliver.py` & `cg-32.2.5/tests/cli/workflow/rnafusion/test_cli_rnafusion_metrics_deliver.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/workflow/rnafusion/test_cli_rnafusion_report_deliver.py` & `cg-32.2.5/tests/cli/workflow/rnafusion/test_cli_rnafusion_report_deliver.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/workflow/rnafusion/test_cli_rnafusion_run.py` & `cg-32.2.5/tests/cli/workflow/rnafusion/test_cli_rnafusion_run.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/workflow/rnafusion/test_cli_rnafusion_store_housekeeper.py` & `cg-32.2.5/tests/cli/workflow/rnafusion/test_cli_rnafusion_store_housekeeper.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/workflow/taxprofiler/test_cli_taxprofiler_compound_commands.py` & `cg-32.2.5/tests/cli/workflow/taxprofiler/test_cli_taxprofiler_compound_commands.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/workflow/test_cli_workflow.py` & `cg-32.2.5/tests/cli/workflow/test_cli_workflow.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/cli/workflow/test_cli_workflow_clean.py` & `cg-32.2.5/tests/cli/workflow/test_cli_workflow_clean.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/conftest.py` & `cg-32.2.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/runParameters.xml` & `cg-32.2.5/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/runParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/ACC11111_qc_fail.json` & `cg-32.2.5/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/ACC11111_qc_fail.json`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/ACC22222_qc_pass.json` & `cg-32.2.5/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/ACC22222_qc_pass.json`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/fixtures/analysis/rnafusion/multiqc_data.json` & `cg-32.2.5/tests/fixtures/analysis/rnafusion/multiqc_data.json`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/fixtures/analysis/sample_coverage.bed` & `cg-32.2.5/tests/fixtures/analysis/sample_coverage.bed`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/fixtures/apps/balsamic/case/config.json` & `cg-32.2.5/tests/fixtures/apps/balsamic/case/config.json`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/fixtures/apps/balsamic/case/metadata.yml` & `cg-32.2.5/tests/fixtures/apps/balsamic/case/metadata.yml`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/fixtures/apps/balsamic/case/metrics_deliverables.yaml` & `cg-32.2.5/tests/fixtures/apps/balsamic/case/metrics_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/fixtures/apps/crunchy/spring_metadata.json` & `cg-32.2.5/tests/fixtures/apps/crunchy/spring_metadata.json`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml` & `cg-32.2.5/tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv` & `cg-32.2.5/tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/fixtures/apps/demultiplexing/RunParameters_different_index_cycles.xml` & `cg-32.2.5/tests/fixtures/apps/demultiplexing/RunParameters_different_index_cycles.xml`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/fixtures/apps/demultiplexing/SampleSheetS2_Bcl2Fastq.csv` & `cg-32.2.5/tests/fixtures/apps/demultiplexing/SampleSheetS2_Bcl2Fastq.csv`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/fixtures/apps/demultiplexing/SampleSheetS2_Dragen.csv` & `cg-32.2.5/tests/fixtures/apps/demultiplexing/SampleSheetS2_Dragen.csv`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr` & `cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml` & `cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml` & `cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/RunInfo.xml` & `cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/RunInfo.xml`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R1_001.fastq.gz` & `cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R1_001.fastq.gz`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R2_001.fastq.gz` & `cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R2_001.fastq.gz`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml` & `cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml` & `cg-32.2.5/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/fixtures/apps/demultiplexing/flow-cell-runs/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr` & `cg-32.2.5/tests/fixtures/apps/demultiplexing/flow-cell-runs/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/fixtures/apps/demultiplexing/flow-cell-runs/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml` & `cg-32.2.5/tests/fixtures/apps/demultiplexing/flow-cell-runs/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/fixtures/apps/demultiplexing/flow-cell-runs/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout` & `cg-32.2.5/tests/fixtures/apps/demultiplexing/flow-cell-runs/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/fixtures/apps/demultiplexing/flow-cell-runs/211101_A00187_0615_AHLG5GDRXY/RunParameters.xml` & `cg-32.2.5/tests/fixtures/apps/demultiplexing/flow-cell-runs/211101_A00187_0615_AHLG5GDRXY/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/fixtures/apps/demultiplexing/hiseq_run/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr` & `cg-32.2.5/tests/fixtures/apps/demultiplexing/hiseq_run/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/fixtures/apps/demultiplexing/hiseq_run/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml` & `cg-32.2.5/tests/fixtures/apps/demultiplexing/hiseq_run/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/fixtures/apps/demultiplexing/hiseq_run/runParameters.xml` & `cg-32.2.5/tests/fixtures/apps/demultiplexing/hiseq_run/runParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/fixtures/apps/demultiplexing/raw_lims_samples/raw_samplesheet_novaseq.json` & `cg-32.2.5/tests/fixtures/apps/demultiplexing/raw_lims_samples/raw_samplesheet_novaseq.json`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/fixtures/apps/demultiplexing/runParameters_missing_flowcell_run_field.xml` & `cg-32.2.5/tests/fixtures/apps/demultiplexing/runParameters_missing_flowcell_run_field.xml`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/fixtures/apps/demultiplexing/unknown_run_parameters.xml` & `cg-32.2.5/tests/fixtures/apps/demultiplexing/unknown_run_parameters.xml`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/fixtures/apps/fluffy/SampleSheet.csv` & `cg-32.2.5/tests/fixtures/apps/fluffy/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/fixtures/apps/fluffy/deliverables.yaml` & `cg-32.2.5/tests/fixtures/apps/fluffy/deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/fixtures/apps/madeline/madeline.xml` & `cg-32.2.5/tests/fixtures/apps/madeline/madeline.xml`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/fixtures/apps/mip/case_metrics_deliverables.yaml` & `cg-32.2.5/tests/fixtures/apps/mip/case_metrics_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/fixtures/apps/mip/dna/store/case_config.yaml` & `cg-32.2.5/tests/fixtures/apps/mip/dna/store/case_config.yaml`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/fixtures/apps/mip/dna/store/case_id_deliverables.yaml` & `cg-32.2.5/tests/fixtures/apps/mip/dna/store/case_id_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/fixtures/apps/mip/dna/store/case_qc_sample_info.yaml` & `cg-32.2.5/tests/fixtures/apps/mip/dna/store/case_qc_sample_info.yaml`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/fixtures/apps/mip/dna/store/yellowhog_clinical_selected.vcf` & `cg-32.2.5/tests/fixtures/apps/mip/dna/store/yellowhog_clinical_selected.vcf`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/fixtures/apps/mip/rna/case_config.yaml` & `cg-32.2.5/tests/fixtures/apps/mip/rna/case_config.yaml`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/fixtures/apps/mip/rna/case_qc_sampleinfo.yaml` & `cg-32.2.5/tests/fixtures/apps/mip/rna/case_qc_sampleinfo.yaml`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/fixtures/apps/mip/rna/store/bundle_data.yaml` & `cg-32.2.5/tests/fixtures/apps/mip/rna/store/bundle_data.yaml`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/fixtures/apps/mip/rna/store/case_config.yaml` & `cg-32.2.5/tests/fixtures/apps/mip/rna/store/case_config.yaml`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/fixtures/apps/mip/rna/store/case_id_deliverables.yaml` & `cg-32.2.5/tests/fixtures/apps/mip/rna/store/case_id_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/fixtures/apps/mip/rna/store/case_qc_sample_info.yaml` & `cg-32.2.5/tests/fixtures/apps/mip/rna/store/case_qc_sample_info.yaml`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/fixtures/apps/scout/643594.config.yaml` & `cg-32.2.5/tests/fixtures/apps/scout/643594.config.yaml`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/fixtures/apps/scout/case_export.json` & `cg-32.2.5/tests/fixtures/apps/scout/case_export.json`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/fixtures/apps/scout/export_causatives.json` & `cg-32.2.5/tests/fixtures/apps/scout/export_causatives.json`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/fixtures/apps/scout/none_case_export.json` & `cg-32.2.5/tests/fixtures/apps/scout/none_case_export.json`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/fixtures/apps/scout/other_sex_case.json` & `cg-32.2.5/tests/fixtures/apps/scout/other_sex_case.json`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/fixtures/apps/scout/panel_export.bed` & `cg-32.2.5/tests/fixtures/apps/scout/panel_export.bed`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/fixtures/apps/scout/panel_export.csv` & `cg-32.2.5/tests/fixtures/apps/scout/panel_export.csv`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/fixtures/apps/sequencing_metrics_parser/Adapter_Metrics.csv` & `cg-32.2.5/tests/fixtures/apps/sequencing_metrics_parser/Adapter_Metrics.csv`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/fixtures/apps/sequencing_metrics_parser/Demultiplex_Stats.csv` & `cg-32.2.5/tests/fixtures/apps/sequencing_metrics_parser/Demultiplex_Stats.csv`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/fixtures/apps/sequencing_metrics_parser/Quality_Metrics.csv` & `cg-32.2.5/tests/fixtures/apps/sequencing_metrics_parser/Quality_Metrics.csv`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/fixtures/apps/sequencing_metrics_parser/RunInfo.xml` & `cg-32.2.5/tests/fixtures/apps/sequencing_metrics_parser/RunInfo.xml`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/fixtures/apps/sequencing_metrics_parser/SampleSheet.csv` & `cg-32.2.5/tests/fixtures/apps/sequencing_metrics_parser/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/fixtures/cgweb_orders/balsamic.json` & `cg-32.2.5/tests/fixtures/cgweb_orders/balsamic.json`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/fixtures/cgweb_orders/fastq.json` & `cg-32.2.5/tests/fixtures/cgweb_orders/fastq.json`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/fixtures/cgweb_orders/metagenome.json` & `cg-32.2.5/tests/fixtures/cgweb_orders/metagenome.json`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/fixtures/cgweb_orders/microsalt.json` & `cg-32.2.5/tests/fixtures/cgweb_orders/microsalt.json`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/fixtures/cgweb_orders/mip.json` & `cg-32.2.5/tests/fixtures/cgweb_orders/mip.json`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/fixtures/cgweb_orders/mip_rna.json` & `cg-32.2.5/tests/fixtures/cgweb_orders/mip_rna.json`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/fixtures/cgweb_orders/rml.json` & `cg-32.2.5/tests/fixtures/cgweb_orders/rml.json`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/fixtures/cgweb_orders/sarscov2.json` & `cg-32.2.5/tests/fixtures/cgweb_orders/sarscov2.json`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/fixtures/data/SampleSheet.csv` & `cg-32.2.5/tests/fixtures/data/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/fixtures/data/cgfixture.db` & `cg-32.2.5/tests/fixtures/data/cgfixture.db`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/fixtures/data/hkstore.db` & `cg-32.2.5/tests/fixtures/data/hkstore.db`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/fixtures/io/example_json.json` & `cg-32.2.5/tests/fixtures/io/example_json.json`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/fixtures/orderforms/1508.27.balsamic.xlsx` & `cg-32.2.5/tests/fixtures/orderforms/1508.27.balsamic.xlsx`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/fixtures/orderforms/1508.27.balsamic_qc.xlsx` & `cg-32.2.5/tests/fixtures/orderforms/1508.27.balsamic_qc.xlsx`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/fixtures/orderforms/1508.27.balsamic_umi.xlsx` & `cg-32.2.5/tests/fixtures/orderforms/1508.27.balsamic_umi.xlsx`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/fixtures/orderforms/1508.27.fastq.xlsx` & `cg-32.2.5/tests/fixtures/orderforms/1508.27.fastq.xlsx`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/fixtures/orderforms/1508.27.mip.xlsx` & `cg-32.2.5/tests/fixtures/orderforms/1508.27.mip.xlsx`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/fixtures/orderforms/1508.27.mip_rna.xlsx` & `cg-32.2.5/tests/fixtures/orderforms/1508.27.mip_rna.xlsx`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/fixtures/orderforms/1603.11.microbial.xlsx` & `cg-32.2.5/tests/fixtures/orderforms/1603.11.microbial.xlsx`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/fixtures/orderforms/1604.15.rml.xlsx` & `cg-32.2.5/tests/fixtures/orderforms/1604.15.rml.xlsx`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/fixtures/orderforms/1605.10.metagenome.xlsx` & `cg-32.2.5/tests/fixtures/orderforms/1605.10.metagenome.xlsx`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/fixtures/orderforms/2184.7.sarscov2.xlsx` & `cg-32.2.5/tests/fixtures/orderforms/2184.7.sarscov2.xlsx`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/fixtures/orderforms/NIPT-json.json` & `cg-32.2.5/tests/fixtures/orderforms/NIPT-json.json`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/fixtures/orderforms/balsamic_uploaded_json_orderform.json` & `cg-32.2.5/tests/fixtures/orderforms/balsamic_uploaded_json_orderform.json`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/fixtures/orderforms/mip_uploaded_json_orderform.json` & `cg-32.2.5/tests/fixtures/orderforms/mip_uploaded_json_orderform.json`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/fixtures/report/case_data.json` & `cg-32.2.5/tests/fixtures/report/case_data.json`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/fixtures/report/lims_exported_samples.json` & `cg-32.2.5/tests/fixtures/report/lims_exported_samples.json`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/fixtures/report/lims_family.json` & `cg-32.2.5/tests/fixtures/report/lims_family.json`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/io/conftest.py` & `cg-32.2.5/tests/io/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/io/test_io_controller.py` & `cg-32.2.5/tests/io/test_io_controller.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/io/test_io_csv.py` & `cg-32.2.5/tests/io/test_io_csv.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/io/test_io_json.py` & `cg-32.2.5/tests/io/test_io_json.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/io/test_io_yaml.py` & `cg-32.2.5/tests/io/test_io_yaml.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/io/test_validate_path.py` & `cg-32.2.5/tests/io/test_validate_path.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/meta/archive/conftest.py` & `cg-32.2.5/tests/meta/archive/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/meta/archive/test_archiving.py` & `cg-32.2.5/tests/meta/archive/test_archiving.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/meta/backup/conftest.py` & `cg-32.2.5/tests/meta/backup/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/meta/backup/test_meta_backup.py` & `cg-32.2.5/tests/meta/backup/test_meta_backup.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/meta/backup/test_meta_pdc.py` & `cg-32.2.5/tests/meta/backup/test_meta_pdc.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/meta/clean/conftest.py` & `cg-32.2.5/tests/meta/clean/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/meta/clean/test_clean_demultiplexed_runs.py` & `cg-32.2.5/tests/meta/clean/test_clean_demultiplexed_runs.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/meta/clean/test_clean_flow_cell_run_directories.py` & `cg-32.2.5/tests/meta/clean/test_clean_flow_cell_run_directories.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/meta/compress/conftest.py` & `cg-32.2.5/tests/meta/compress/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/meta/compress/test_clean_fastq.py` & `cg-32.2.5/tests/meta/compress/test_clean_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/meta/compress/test_compress_files.py` & `cg-32.2.5/tests/meta/compress/test_compress_files.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/meta/compress/test_compress_meta_fastq.py` & `cg-32.2.5/tests/meta/compress/test_compress_meta_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/meta/compress/test_decompress_spring_meta.py` & `cg-32.2.5/tests/meta/compress/test_decompress_spring_meta.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/meta/compress/test_meta_compress_update_hk.py` & `cg-32.2.5/tests/meta/compress/test_meta_compress_update_hk.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/meta/conftest.py` & `cg-32.2.5/tests/meta/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/meta/deliver/conftest.py` & `cg-32.2.5/tests/meta/deliver/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/meta/deliver/test_deliver_ticket.py` & `cg-32.2.5/tests/meta/deliver/test_deliver_ticket.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/meta/deliver/test_delivery_api.py` & `cg-32.2.5/tests/meta/deliver/test_delivery_api.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/meta/demultiplex/conftest.py` & `cg-32.2.5/tests/meta/demultiplex/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/meta/demultiplex/test_delete_demultiplex_api.py` & `cg-32.2.5/tests/meta/demultiplex/test_delete_demultiplex_api.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/meta/demultiplex/test_demux_post_processing.py` & `cg-32.2.5/tests/meta/demultiplex/test_demux_post_processing.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/meta/demultiplex/test_rename_files.py` & `cg-32.2.5/tests/meta/demultiplex/test_rename_files.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/meta/encryption/conftest.py` & `cg-32.2.5/tests/meta/encryption/conftest.py`

 * *Files 10% similar despite different names*

```diff
@@ -42,38 +42,20 @@
 
 @pytest.fixture(name="spring_file_path")
 def fixture_spring_file_path() -> Path:
     """Return an spring file Path object"""
     return Path("/path/to/file.spring")
 
 
-@pytest.fixture(name="checksum_spring_file_path")
-def fixture_checksum_spring_file_path() -> Path:
-    """Return an spring file Path object"""
-    return Path("/path/to/file.spring.tmp")
-
-
 @pytest.fixture(name="encrypted_spring_file_path")
 def fixture_encrypted_spring_file_path() -> Path:
     """Return an encrypted spring file Path object"""
     return Path("/path/to/file.spring.gpg")
 
 
-@pytest.fixture(name="checksum_result_1")
-def fixture_checksum_result_1() -> str:
-    """fixture that can be used as a checksum result"""
-    return "a1b2c3"
-
-
-@pytest.fixture(name="checksum_result_2")
-def fixture_checksum_result_2() -> str:
-    """fixture that can be used as a checksum result"""
-    return "x7y8z9"
-
-
 @pytest.fixture(name="encryption_user_id")
 def fixture_encryption_user_id() -> str:
     """Encryption user ID fixture"""
     return "Clinical Genomics"
 
 
 @pytest.fixture(name="cipher_algorithm")
```

### Comparing `cg-32.2.4/tests/meta/encryption/test_encryption.py` & `cg-32.2.5/tests/meta/encryption/test_encryption.py`

 * *Files 10% similar despite different names*

```diff
@@ -50,64 +50,14 @@
     result = encryption_api.generate_temporary_passphrase_file()
 
     # THEN the passphrase file should be generated as a temporary file
     assert type(result) is pathlib.PosixPath
     assert result.exists()
 
 
-@mock.patch("cg.meta.encryption.encryption.sha512_checksum")
-def test_compare_file_checksums_equal(
-    mock_file_checksum,
-    binary_path,
-    spring_file_path,
-    checksum_spring_file_path,
-    checksum_result_1,
-    caplog,
-):
-    """Tests the compare_file_checksum method"""
-    # GIVEN two identical checksum results
-    caplog.set_level(logging.INFO)
-    encryption_api = SpringEncryptionAPI(binary_path=binary_path)
-
-    mock_file_checksum.side_effect = [checksum_result_1, checksum_result_1]
-
-    # WHEN comparing the checksums of those files
-    encryption_api.compare_file_checksums(
-        original_file=spring_file_path, decrypted_file_checksum=checksum_spring_file_path
-    )
-
-    # THEN the checksum comparison should pass
-    assert "Checksum comparison successful!" in caplog.text
-
-
-@mock.patch("cg.meta.encryption.encryption.sha512_checksum")
-def test_compare_file_checksums_not_equal(
-    mock_file_checksum,
-    binary_path,
-    spring_file_path,
-    checksum_spring_file_path,
-    checksum_result_1,
-    checksum_result_2,
-):
-    """Tests the compare_file_checksum method"""
-    # GIVEN two nonidentical checksum results
-    encryption_api = SpringEncryptionAPI(binary_path=binary_path)
-
-    mock_file_checksum.side_effect = [checksum_result_1, checksum_result_2]
-
-    # WHEN comparing the checksums of those files
-    with pytest.raises(ChecksumFailedError) as error:
-        encryption_api.compare_file_checksums(
-            original_file=spring_file_path, decrypted_file_checksum=checksum_spring_file_path
-        )
-
-    # THEN the checksum comparison should fail and an exception should be raised
-    assert error.value.args[0] == "Checksum comparison failed!"
-
-
 def test_get_asymmetric_encryption_command(
     binary_path, input_file, output_file, asymmetric_encryption_command
 ):
     """Tests creating the asymmetric encryption command"""
     # GIVEN an input file and an output file for a gpg command
     encryption_api = SpringEncryptionAPI(binary_path=binary_path)
```

### Comparing `cg-32.2.4/tests/meta/observations/conftest.py` & `cg-32.2.5/tests/meta/observations/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/meta/observations/test_meta_upload_observations.py` & `cg-32.2.5/tests/meta/observations/test_meta_upload_observations.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/meta/orders/conftest.py` & `cg-32.2.5/tests/meta/orders/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/meta/orders/test_PoolSubmitter_validate_order.py` & `cg-32.2.5/tests/meta/orders/test_PoolSubmitter_validate_order.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/meta/orders/test_SarsCov2Submitter_order_to_status.py` & `cg-32.2.5/tests/meta/orders/test_SarsCov2Submitter_order_to_status.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/meta/orders/test_SarsCov2Submitter_store_order.py` & `cg-32.2.5/tests/meta/orders/test_SarsCov2Submitter_store_order.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/meta/orders/test_SarsCov2Submitter_validate_order.py` & `cg-32.2.5/tests/meta/orders/test_SarsCov2Submitter_validate_order.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/meta/orders/test_meta_orders_api.py` & `cg-32.2.5/tests/meta/orders/test_meta_orders_api.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/meta/orders/test_meta_orders_lims.py` & `cg-32.2.5/tests/meta/orders/test_meta_orders_lims.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/meta/orders/test_meta_orders_status.py` & `cg-32.2.5/tests/meta/orders/test_meta_orders_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from cg.meta.orders.mip_rna_submitter import MipRnaSubmitter
 from cg.meta.orders.rml_submitter import RmlSubmitter
 from cg.meta.orders.sars_cov_2_submitter import SarsCov2Submitter
 from cg.meta.orders.submitter import Submitter
 from cg.models.orders.order import OrderIn, OrderType
 from cg.meta.orders import OrdersAPI
 from cg.store import Store
-from cg.store.models import Delivery, Family, Pool, Sample
+from cg.store.models import Application, Delivery, Family, Pool, Sample
 from cg.constants import Priority
 
 
 def test_pools_to_status(rml_order_to_submit):
     # GIVEN a rml order with three samples in one pool
     order = OrderIn.parse_obj(rml_order_to_submit, OrderType.RML)
 
@@ -350,19 +350,23 @@
 def test_store_fastq_samples_non_wgs_as_fastq(
     orders_api, base_store, fastq_status_data, ticket_id: str
 ):
     # GIVEN a basic store with no samples and a fastq order as non wgs
     assert not base_store._get_query(table=Sample).first()
     assert base_store._get_query(table=Family).count() == 0
     non_wgs_prep_category = PrepCategory.WHOLE_EXOME_SEQUENCING
-    assert base_store.get_applications_by_prep_category(prep_category=non_wgs_prep_category)
+
+    non_wgs_applications = base_store._get_query(table=Application).filter(
+        Application.prep_category == non_wgs_prep_category
+    )
+
+    assert non_wgs_applications
+
     for sample in fastq_status_data["samples"]:
-        sample["application"] = base_store.get_applications_by_prep_category(
-            prep_category=non_wgs_prep_category
-        )[0].tag
+        sample["application"] = non_wgs_applications[0].tag
 
     submitter = FastqSubmitter(lims=orders_api.lims, status=orders_api.status)
 
     # WHEN storing the order
     new_samples = submitter.store_items_in_status(
         customer_id=fastq_status_data["customer"],
         order=fastq_status_data["order"],
```

### Comparing `cg-32.2.4/tests/meta/orders/test_ticket_handler.py` & `cg-32.2.5/tests/meta/orders/test_ticket_handler.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/meta/report/conftest.py` & `cg-32.2.5/tests/meta/report/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/meta/report/test_balsamic_api.py` & `cg-32.2.5/tests/meta/report/test_balsamic_api.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/meta/report/test_field_validators.py` & `cg-32.2.5/tests/meta/report/test_field_validators.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/meta/report/test_mip_dna_api.py` & `cg-32.2.5/tests/meta/report/test_mip_dna_api.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/meta/report/test_report_api.py` & `cg-32.2.5/tests/meta/report/test_report_api.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/meta/rsync/conftest.py` & `cg-32.2.5/tests/meta/rsync/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/meta/rsync/test_rsync.py` & `cg-32.2.5/tests/meta/rsync/test_rsync.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/meta/test_invoice.py` & `cg-32.2.5/tests/meta/test_invoice.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/meta/transfer/conftest.py` & `cg-32.2.5/tests/meta/transfer/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/meta/transfer/test_external_data.py` & `cg-32.2.5/tests/meta/transfer/test_external_data.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/meta/transfer/test_meta_transfer_flowcell.py` & `cg-32.2.5/tests/meta/transfer/test_meta_transfer_flowcell.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/meta/transfer/test_meta_transfer_lims.py` & `cg-32.2.5/tests/meta/transfer/test_meta_transfer_lims.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/meta/upload/balsamic/test_balsamic.py` & `cg-32.2.5/tests/meta/upload/balsamic/test_balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/meta/upload/conftest.py` & `cg-32.2.5/tests/meta/upload/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/meta/upload/gisaid/fixtures/four_samples.csv` & `cg-32.2.5/tests/meta/upload/gisaid/fixtures/four_samples.csv`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/meta/upload/mutacc/conftest.py` & `cg-32.2.5/tests/meta/upload/mutacc/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/meta/upload/mutacc/test_meta_upload_mutacc.py` & `cg-32.2.5/tests/meta/upload/mutacc/test_meta_upload_mutacc.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/meta/upload/nipt/conftest.py` & `cg-32.2.5/tests/meta/upload/nipt/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/meta/upload/nipt/test_nipt_upload_api.py` & `cg-32.2.5/tests/meta/upload/nipt/test_nipt_upload_api.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/meta/upload/scout/conftest.py` & `cg-32.2.5/tests/meta/upload/scout/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/meta/upload/scout/test_generate_load_config.py` & `cg-32.2.5/tests/meta/upload/scout/test_generate_load_config.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/meta/upload/scout/test_meta_upload_scoutapi.py` & `cg-32.2.5/tests/meta/upload/scout/test_meta_upload_scoutapi.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/meta/upload/scout/test_meta_upload_scoutapi_rna.py` & `cg-32.2.5/tests/meta/upload/scout/test_meta_upload_scoutapi_rna.py`

 * *Files 0% similar despite different names*

```diff
@@ -535,15 +535,17 @@
     rna_store: Store,
     upload_scout_api: UploadScoutAPI,
 ):
     """Test that for a given RNA case the RNA samples are added to the rna_dna_case_map."""
 
     # GIVEN an RNA case and the associated RNA samples
     rna_case: Family = rna_store.get_case_by_internal_id(internal_id=rna_case_id)
-    rna_sample_list: List[Sample] = rna_store.get_samples_by_name_pattern(name_pattern="rna")
+    rna_sample_list: List[Sample] = (
+        rna_store._get_query(table=Sample).filter(Sample.internal_id.like("rna")).all()
+    )
 
     # WHEN running the method to create a nested dictionary with the relationships between RNA/DNA samples and DNA cases
     rna_dna_case_map: dict = upload_scout_api.create_rna_dna_sample_case_map(rna_case=rna_case)
 
     # THEN the resulting dictionary should contain all RNA samples in the case
     for key in rna_sample_list:
         assert key.internal_id in list(rna_dna_case_map.keys())
```

### Comparing `cg-32.2.4/tests/meta/upload/scout/test_scout_config_builder.py` & `cg-32.2.5/tests/meta/upload/scout/test_scout_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/meta/upload/test_meta_upload_coverage.py` & `cg-32.2.5/tests/meta/upload/test_meta_upload_coverage.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/meta/upload/test_upload_api.py` & `cg-32.2.5/tests/meta/upload/test_upload_api.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/meta/upload/test_upload_genotypes_api.py` & `cg-32.2.5/tests/meta/upload/test_upload_genotypes_api.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/meta/upload/vogue/conftest.py` & `cg-32.2.5/tests/meta/upload/vogue/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/meta/upload/vogue/test_upload_vogue.py` & `cg-32.2.5/tests/meta/upload/vogue/test_upload_vogue.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/meta/workflow/conftest.py` & `cg-32.2.5/tests/meta/workflow/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/meta/workflow/test_analysis.py` & `cg-32.2.5/tests/meta/workflow/test_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/meta/workflow/test_balsamic.py` & `cg-32.2.5/tests/meta/workflow/test_balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/meta/workflow/test_microsalt.py` & `cg-32.2.5/tests/meta/workflow/test_microsalt.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/meta/workflow/test_prepare_fastq_api.py` & `cg-32.2.5/tests/meta/workflow/test_prepare_fastq_api.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/mocks/balsamic_analysis_mock.py` & `cg-32.2.5/tests/mocks/balsamic_analysis_mock.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/mocks/crunchy.py` & `cg-32.2.5/tests/mocks/crunchy.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/mocks/hk_mock.py` & `cg-32.2.5/tests/mocks/hk_mock.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/mocks/limsmock.py` & `cg-32.2.5/tests/mocks/limsmock.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/mocks/madeline.py` & `cg-32.2.5/tests/mocks/madeline.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/mocks/mip_analysis_mock.py` & `cg-32.2.5/tests/mocks/mip_analysis_mock.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/mocks/osticket.py` & `cg-32.2.5/tests/mocks/osticket.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/mocks/process_mock.py` & `cg-32.2.5/tests/mocks/process_mock.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/mocks/report.py` & `cg-32.2.5/tests/mocks/report.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/mocks/scout.py` & `cg-32.2.5/tests/mocks/scout.py`

 * *Files 11% similar despite different names*

```diff
@@ -77,18 +77,14 @@
 
     # Overridden functions
 
     def upload(self, data: dict, force: bool = False):
         """Load analysis of a new case into Scout."""
         LOG.debug("Case loaded successfully to Scout")
 
-    def update_alignment_file(self, case_id: str, sample_id: str, alignment_path: Path):
-        """Update alignment file for individual in case"""
-        self._alignment_file_updated += 1
-
     def export_panels(self, panels: List[str], versions=None):
         """Pass through to export of a list of gene panels."""
         return self._panels
 
     def get_genes(self, panel_id: str, version: str = None) -> list:
         """Fetch panel genes.
```

### Comparing `cg-32.2.4/tests/mocks/store_model.py` & `cg-32.2.5/tests/mocks/store_model.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/mocks/tb_mock.py` & `cg-32.2.5/tests/mocks/tb_mock.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/models/balsamic/conftest.py` & `cg-32.2.5/tests/models/balsamic/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/models/balsamic/test_balsamic_analysis.py` & `cg-32.2.5/tests/models/balsamic/test_balsamic_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/models/conftest.py` & `cg-32.2.5/tests/models/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/models/demultiplexing/conftest.py` & `cg-32.2.5/tests/models/demultiplexing/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/models/demultiplexing/test_demux_results.py` & `cg-32.2.5/tests/models/demultiplexing/test_demux_results.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/models/demultiplexing/test_flowcell_model.py` & `cg-32.2.5/tests/models/demultiplexing/test_flowcell_model.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/models/demultiplexing/test_run_parameters.py` & `cg-32.2.5/tests/models/demultiplexing/test_run_parameters.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/models/mip/conftest.py` & `cg-32.2.5/tests/models/mip/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/models/mip/test_mip_analysis.py` & `cg-32.2.5/tests/models/mip/test_mip_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/models/mip/test_mip_config.py` & `cg-32.2.5/tests/models/mip/test_mip_config.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/models/mip/test_mip_metrics_deliverables.py` & `cg-32.2.5/tests/models/mip/test_mip_metrics_deliverables.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/models/mip/test_mip_sample_info.py` & `cg-32.2.5/tests/models/mip/test_mip_sample_info.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/models/nextflow/conftest.py` & `cg-32.2.5/tests/models/nextflow/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/models/nextflow/test_nextflow_deliver.py` & `cg-32.2.5/tests/models/nextflow/test_nextflow_deliver.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/models/observations/conftest.py` & `cg-32.2.5/tests/models/observations/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/models/observations/test_observations_input_files.py` & `cg-32.2.5/tests/models/observations/test_observations_input_files.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/models/report/test_validators.py` & `cg-32.2.5/tests/models/report/test_validators.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/models/rnafusion/conftest.py` & `cg-32.2.5/tests/models/rnafusion/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/models/rnafusion/test_rnafusion_sample.py` & `cg-32.2.5/tests/models/rnafusion/test_rnafusion_sample.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/models/test_cg_models.py` & `cg-32.2.5/tests/models/test_cg_models.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/models/test_compression_data.py` & `cg-32.2.5/tests/models/test_compression_data.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/models/test_file_data.py` & `cg-32.2.5/tests/models/test_file_data.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/models/test_flowcell_class.py` & `cg-32.2.5/tests/models/test_flowcell_class.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/server/conftest.py` & `cg-32.2.5/tests/server/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/store/api/add/test_store_add_application_version.py` & `cg-32.2.5/tests/store/api/add/test_store_add_application_version.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,24 +11,32 @@
     version: int = 1,
 ):
     """Test that the functions returns an application version."""
     # GIVEN a store with applications but without application versions
     applications: List[
         Application
     ] = store_with_an_application_with_and_without_attributes.get_applications()
-    store_with_an_application_with_and_without_attributes.get_application_versions()
+    store_with_an_application_with_and_without_attributes._get_query(table=ApplicationVersion).all()
     assert len(applications) > 0
     assert (
-        len(store_with_an_application_with_and_without_attributes.get_application_versions()) == 0
+        len(
+            store_with_an_application_with_and_without_attributes._get_query(
+                table=ApplicationVersion
+            ).all()
+        )
+        == 0
     )
 
     # WHEN adding a new application version
-    application_version: ApplicationVersion = (
-        store_with_an_application_with_and_without_attributes.add_application_version(
-            application=applications[0], version=version, valid_from=timestamp, prices=prices
-        )
+    store_with_an_application_with_and_without_attributes.add_application_version(
+        application=applications[0], version=version, valid_from=timestamp, prices=prices
     )
 
     # THEN the store has one application version
     assert (
-        len(store_with_an_application_with_and_without_attributes.get_application_versions()) == 1
+        len(
+            store_with_an_application_with_and_without_attributes._get_query(
+                table=ApplicationVersion
+            ).all()
+        )
+        == 1
     )
```

### Comparing `cg-32.2.4/tests/store/api/add/test_store_add_base.py` & `cg-32.2.5/tests/store/api/add/test_store_add_base.py`

 * *Files 8% similar despite different names*

```diff
@@ -82,16 +82,18 @@
 
 
 def test_add_pool(rml_pool_store: Store):
     """Tests whether new pools are invoiced as default."""
     # GIVEN a valid customer and a valid application_version
     customer: Customer = rml_pool_store.get_customers()[0]
     application = rml_pool_store.get_application_by_tag(tag="RMLP05R800")
-    app_version = rml_pool_store.get_application_version_by_application_entry_id(
-        application_entry_id=application.id
+    app_version = (
+        rml_pool_store._get_query(table=ApplicationVersion)
+        .filter(ApplicationVersion.application_id == application.id)
+        .first()
     )
 
     # WHEN adding a new pool
     new_pool = rml_pool_store.add_pool(
         customer=customer,
         name="pool2",
         order="123456",
```

### Comparing `cg-32.2.4/tests/store/api/add/test_store_add_customer.py` & `cg-32.2.5/tests/store/api/add/test_store_add_customer.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/store/api/add/test_store_add_flow_celll.py` & `cg-32.2.5/tests/store/api/add/test_store_add_flow_celll.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/store/api/conftest.py` & `cg-32.2.5/tests/store/api/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,20 +172,14 @@
 
 @pytest.fixture(name="EXPECTED_NUMBER_OF_NOT_ARCHIVED_APPLICATIONS")
 def fixture_expected_number_of_not_archived_applications() -> int:
     """Return the number of expected number of not archived applications"""
     return 4
 
 
-@pytest.fixture(name="EXPECTED_NUMBER_OF_APPLICATIONS_WITH_PREP_CATEGORY")
-def fixture_expected_number_of_applications_with_prep_category() -> int:
-    """Return the number of expected number of applications with prep category"""
-    return 7
-
-
 @pytest.fixture(name="EXPECTED_NUMBER_OF_APPLICATIONS")
 def fixture_expected_number_of_applications() -> int:
     """Return the number of expected number of applications with prep category"""
     return 7
 
 
 @pytest.fixture(name="store_with_samples_that_have_names")
```

### Comparing `cg-32.2.4/tests/store/api/delete/test_store_api_delete.py` & `cg-32.2.5/tests/store/api/delete/test_store_api_delete.py`

 * *Files 9% similar despite different names*

```diff
@@ -44,24 +44,24 @@
     assert sample_in_single_case
     assert sample_in_multiple_cases
 
     # WHEN removing the relationships between one sample and its cases
     store_with_multiple_cases_and_samples.delete_relationships_sample(sample=sample_in_single_case)
 
     # THEN it should no longer be associated with any cases, but other relationships should remain
-    results: List[
-        FamilySample
-    ] = store_with_multiple_cases_and_samples.get_case_samples_from_sample_entry_id(
-        sample_entry_id=sample_in_single_case.id
-    ).all()
-    existing_relationships: List[
-        FamilySample
-    ] = store_with_multiple_cases_and_samples.get_case_samples_from_sample_entry_id(
-        sample_entry_id=sample_in_multiple_cases.id
-    ).all()
+    results: List[FamilySample] = (
+        store_with_multiple_cases_and_samples._get_query(table=FamilySample)
+        .filter(FamilySample.sample_id == sample_in_single_case.id)
+        .all()
+    )
+    existing_relationships: List[FamilySample] = (
+        store_with_multiple_cases_and_samples._get_query(table=FamilySample)
+        .filter(FamilySample.sample_id == sample_in_multiple_cases.id)
+        .all()
+    )
 
     assert not results
     assert existing_relationships
 
 
 def test_store_api_delete_all_empty_cases(
     case_id_without_samples: str,
```

### Comparing `cg-32.2.4/tests/store/api/find/test_find_basic_data.py` & `cg-32.2.5/tests/store/api/find/test_find_basic_data.py`

 * *Files 16% similar despite different names*

```diff
@@ -42,53 +42,14 @@
     # WHEN fetching beds
     active_beds: Query = base_store.get_active_beds()
 
     # THEN return no beds
     assert not list(active_beds)
 
 
-def test_get_bed_by_name(base_store: Store, bed_name: str):
-    """Test returning a bed record by name from the database."""
-
-    # GIVEN a store with beds
-
-    # WHEN fetching beds
-    bed: Optional[Bed] = base_store.get_bed_by_name(bed_name=bed_name)
-
-    # THEN return a bed
-    assert bed
-
-    # THEN return a bed with the supplied bed name
-    assert bed.name == bed_name
-
-
-def test_get_bed_by_name_when_no_match(base_store: Store):
-    """Test returning a bed record by name from the database when no match."""
-
-    # GIVEN a store with beds
-
-    # WHEN fetching beds
-    bed: Optional[Bed] = base_store.get_bed_by_name(bed_name="does_not_exist")
-
-    # THEN do not return a bed
-    assert not bed
-
-
-def test_get_latest_bed_version(base_store: Store, bed_name: str):
-    """Test returning a bed version by bed name from the database."""
-
-    # GIVEN a store with beds
-
-    # WHEN fetching beds
-    bed_version: BedVersion = base_store.get_latest_bed_version(bed_name=bed_name)
-
-    # THEN return a bed version with the supplied bed name
-    assert bed_version.version == 1
-
-
 def test_get_application_by_tag(microbial_store: Store, tag: str = MicrosaltAppTags.MWRNXTR003):
     """Test function to return the application by tag."""
 
     # GIVEN a store with application records
 
     # WHEN getting the query for the flow cells
     application: Application = microbial_store.get_application_by_tag(tag=tag)
@@ -108,33 +69,14 @@
     applications: List[Application] = microbial_store.get_applications_is_not_archived()
 
     # THEN return a application with the supplied application tag
     assert len(applications) == EXPECTED_NUMBER_OF_NOT_ARCHIVED_APPLICATIONS
     assert (application.is_archived is False for application in applications)
 
 
-def test_get_applications_by_prep_category(
-    microbial_store: Store,
-    EXPECTED_NUMBER_OF_APPLICATIONS_WITH_PREP_CATEGORY,
-    prep_category=MicrosaltAppTags.PREP_CATEGORY,
-):
-    """Test function to return the application by prep category."""
-
-    # GIVEN a store with application records
-
-    # WHEN getting the query for the flow cells
-    applications: List[Application] = microbial_store.get_applications_by_prep_category(
-        prep_category=prep_category
-    )
-
-    # THEN return a application with the supplied application tag
-    assert len(applications) == EXPECTED_NUMBER_OF_APPLICATIONS_WITH_PREP_CATEGORY
-    assert (application.prep_category == prep_category for application in applications)
-
-
 def test_get_applications(microbial_store: Store, EXPECTED_NUMBER_OF_APPLICATIONS):
     """Test function to return the applications."""
 
     # GIVEN a store with application records
 
     # WHEN getting the query for the flow cells
     applications: List[Application] = microbial_store.get_applications()
```

### Comparing `cg-32.2.4/tests/store/api/find/test_find_basic_data_application_version.py` & `cg-32.2.5/tests/store/api/find/test_find_basic_data_application_version.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,52 +1,12 @@
 from typing import Optional, List
 from cg.store import Store
 from cg.store.models import Application, ApplicationVersion
 
 
-def test_get_application_version_by_application_id_existing_id(
-    base_store: Store,
-):
-    """Test that the correct application version is returned when using a correct application id."""
-    # GIVEN a store with an application
-    application: Application = base_store.get_applications()[0]
-    assert application
-
-    # WHEN getting the application version by application id
-    application_version: ApplicationVersion = (
-        base_store.get_application_version_by_application_entry_id(
-            application_entry_id=application.id
-        )
-    )
-
-    # THEN the id of the application is the same as the application version
-    assert application_version.application_id == application.id
-
-
-def test_get_application_version_by_application_id_invalid_id(
-    base_store: Store,
-    invalid_application_id: int,
-):
-    """Test that the correct application version is returned when using a correct application id."""
-    # GIVEN a store with applications and an invalid application id
-    applications: List[Application] = base_store.get_applications()
-    ids: List[str] = [application.id for application in applications]
-    assert invalid_application_id not in ids
-
-    # WHEN getting an application version by the invalid id
-    application_version: Optional[
-        ApplicationVersion
-    ] = base_store.get_application_version_by_application_entry_id(
-        application_entry_id=invalid_application_id
-    )
-
-    # THEN the application version is None
-    assert application_version is None
-
-
 def test_get_current_application_version_by_tag_existing_tag(base_store: Store):
     """Test that giving an existing tag returns the correct application version."""
     # GIVEN an application in store with a valid tag
     application: Application = base_store.get_applications()[0]
     tag: str = application.tag
     assert tag
 
@@ -81,15 +41,15 @@
 def test_get_current_application_version_by_tag_latest_version(
     store_with_different_application_versions: Store,
 ):
     """Test that the returned application version is the most recent."""
     # GIVEN a store with applications versions with different 'valid_from' attributes
     application_versions: List[
         ApplicationVersion
-    ] = store_with_different_application_versions.get_application_versions()
+    ] = store_with_different_application_versions._get_query(table=ApplicationVersion).all()
     assert application_versions[0].valid_from != application_versions[-1].valid_from
 
     # GIVEN a valid application tag
     tag: str = store_with_different_application_versions.get_applications()[0].tag
     application_versions_with_tag: List[ApplicationVersion] = [
         app_ver for app_ver in application_versions if app_ver.application.tag == tag
     ]
```

### Comparing `cg-32.2.4/tests/store/api/find/test_find_business_data.py` & `cg-32.2.5/tests/store/api/find/test_find_business_data.py`

 * *Files 9% similar despite different names*

```diff
@@ -78,30 +78,14 @@
         flow_cell_name=bcl2fastq_flow_cell_id
     )
 
     # THEN the returned flow cell should have the same name as the one in the database
     assert flow_cell.name == bcl2fastq_flow_cell_id
 
 
-def test_get_flow_cell_by_name_pattern(
-    bcl2fastq_flow_cell_id: str, re_sequenced_sample_store: Store
-):
-    """Test returning the latest flow cell from the database by enquiry."""
-
-    # GIVEN a store with two flow cells
-
-    # WHEN fetching the latest flow cell
-    flow_cell: List[Flowcell] = re_sequenced_sample_store.get_flow_cell_by_name_pattern(
-        name_pattern=bcl2fastq_flow_cell_id[:4]
-    )
-
-    # THEN the returned flow cell should have the same name as the one in the database
-    assert flow_cell.name == bcl2fastq_flow_cell_id
-
-
 def test_get_flow_cells_by_case(
     base_store: Store,
     bcl2fastq_flow_cell_id: str,
     another_flow_cell_id: str,
     case: Family,
     helpers: StoreHelpers,
     sample: Sample,
@@ -448,57 +432,14 @@
     # THEN the returned element is a FamilySample object
     assert isinstance(case_sample, FamilySample)
     # THEN the returned family sample has the correct case and sample internal ids
     assert case_sample.family.internal_id == case_id
     assert case_sample.sample.internal_id == sample_id
 
 
-def test_find_single_case_for_sample(
-    sample_id_in_single_case: str, store_with_multiple_cases_and_samples: Store
-):
-    """Test that cases associated with a sample can be found."""
-
-    # GIVEN a database containing a sample associated with a single case
-    sample: Sample = store_with_multiple_cases_and_samples.get_sample_by_internal_id(
-        internal_id=sample_id_in_single_case
-    )
-
-    assert sample
-
-    # WHEN the cases associated with the sample is fetched
-    cases: List[
-        FamilySample
-    ] = store_with_multiple_cases_and_samples.get_case_samples_from_sample_entry_id(
-        sample_entry_id=sample.id
-    ).all()
-
-    # THEN only one case is found
-    assert cases and len(cases) == 1
-
-
-def test_find_multiple_cases_for_sample(
-    sample_id_in_multiple_cases: str, store_with_multiple_cases_and_samples: Store
-):
-    # GIVEN a database containing a sample associated with multiple cases
-    sample: Sample = store_with_multiple_cases_and_samples.get_sample_by_internal_id(
-        internal_id=sample_id_in_multiple_cases
-    )
-    assert sample
-
-    # WHEN the cases associated with the sample is fetched
-    cases: List[
-        FamilySample
-    ] = store_with_multiple_cases_and_samples.get_case_samples_from_sample_entry_id(
-        sample_entry_id=sample.id
-    ).all()
-
-    # THEN multiple cases are found
-    assert cases and len(cases) > 1
-
-
 def test_find_cases_for_non_existing_case(store_with_multiple_cases_and_samples: Store):
     """Test that nothing happens when trying to find a case that does not exist."""
 
     # GIVEN a database containing some cases but not a specific case
     case_id: str = "some_case"
     case: Family = store_with_multiple_cases_and_samples.get_case_by_internal_id(
         internal_id=case_id
@@ -709,16 +650,14 @@
 
     # THEN one pool should be returned
     assert len(pools) == 1
 
 
 def test_get_pools_to_render_with(
     store_with_multiple_pools_for_customer: Store,
-    pool_name_1: str,
-    pool_order_1: str,
 ):
     """Test that pools can be fetched from the store by customer id."""
     # GIVEN a database with two pools
 
     # WHEN fetching pools with no customer or enquiry
     pools: List[Pool] = store_with_multiple_pools_for_customer.get_pools_to_render()
 
@@ -827,36 +766,7 @@
     # THEN multiple cases should be returned
     assert len(cases) > 1
 
     # Check that all returned cases have the matching sample and are not analysed
     for case in cases:
         assert not case.analyses
         assert any(sample.internal_id == sample_id_in_multiple_cases for sample in case.samples)
-
-
-def test_fetch_cases_newer_than_date_no_cases(store_with_multiple_cases_and_samples: Store):
-    """Test that no cases are returned when there are no cases newer than the given date."""
-    # GIVEN a store with cases older than 7 days
-    older_than_date = datetime.now() - timedelta(days=10)
-    for case in store_with_multiple_cases_and_samples._get_query(table=Family):
-        case.created_at = older_than_date
-
-    # WHEN fetching cases newer than 7 days
-    cases = store_with_multiple_cases_and_samples.get_cases_created_within_days(days=7)
-
-    # THEN no cases should be returned
-    assert len(cases) == 0
-
-
-def test_fetch_cases_newer_than_date_all_cases(store_with_multiple_cases_and_samples: Store):
-    """Test that all cases are returned when all cases newer than the given date."""
-    # GIVEN a store with cases newer than 7 days
-    older_than_date = datetime.now() - timedelta(days=5)
-    all_cases = store_with_multiple_cases_and_samples._get_query(table=Family).all()
-    for case in all_cases:
-        case.created_at = older_than_date
-
-    # WHEN fetching cases newer than 7 days
-    cases = store_with_multiple_cases_and_samples.get_cases_created_within_days(days=7)
-
-    # THEN all cases should be returned
-    assert len(cases) == len(all_cases)
```

### Comparing `cg-32.2.4/tests/store/api/find/test_find_business_data_analysis.py` & `cg-32.2.5/tests/store/api/find/test_find_business_data_analysis.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,34 +4,15 @@
 from cg.store import Store
 from cg.store.models import (
     Analysis,
 )
 from cg.constants import Pipeline
 
 
-def test_get_analysis_by_case(
-    store_with_case_and_analysis: Store, case_id: str = "test_case_internal_id"
-):
-    """Test that an analysis can be fetched by case."""
-    # GIVEN a database with an analysis and case
-    case = store_with_case_and_analysis.get_case_by_internal_id(internal_id=case_id)
-    assert case
-    # WHEN fetching the analysis by case
-    analyses: List[Analysis] = store_with_case_and_analysis.get_analyses_by_case_entry_id(
-        case_entry_id=case.id
-    )
-    # THEN one analysis should be returned
-    for analysis in analyses:
-        assert analysis
-        assert analysis.family == case
-
-
-def test_get_analyses_uploaded_to_vogue(
-    store_with_analyses_for_cases: Store, case_id: str = "test_case_internal_id"
-):
+def test_get_analyses_uploaded_to_vogue(store_with_analyses_for_cases: Store):
     """Test that an analysis can be fetched by case."""
     # GIVEN a database with an analysis and case
 
     # WHEN fetching the latest analysis to upload to vogue
     analyses: List[Analysis] = store_with_analyses_for_cases.get_analyses_for_vogue_upload()
 
     # THEN the analyses should not have been uploaded to Vogue
@@ -121,15 +102,14 @@
         assert analysis.started_at == timestamp_now
         assert analysis.uploaded_at is None
         assert analysis.pipeline == pipeline
 
 
 def test_get_analyses_to_deliver_for_pipeline(
     store_with_analyses_for_cases_to_deliver: Store,
-    timestamp_now: datetime,
     pipeline: Pipeline = Pipeline.FLUFFY,
 ):
     # GIVEN a store with multiple analyses to deliver
 
     # WHEN fetching the latest analysis to upload to nipt
     analyses = store_with_analyses_for_cases_to_deliver.get_analyses_to_deliver_for_pipeline(
         pipeline=pipeline
```

### Comparing `cg-32.2.4/tests/store/api/find/test_find_business_data_case.py` & `cg-32.2.5/tests/store/api/find/test_find_business_data_case.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/store/api/find/test_find_business_data_sample.py` & `cg-32.2.5/tests/store/api/find/test_find_business_data_sample.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,14 @@
     # THEN the pool and sample should be returned
     assert pool in records
     assert sample in records
 
 
 def test_get_samples_by_customer_and_subject_id_query(
     store_with_samples_subject_id_and_tumour_status: Store,
-    helpers: StoreHelpers,
     cust123: str,
     test_subject: str,
 ):
     """Test that samples can be fetched by subject id."""
     # GIVEN a database with two samples that have a subject ID but only one is tumour
 
     # GIVEN that there are two samples in the store
@@ -56,15 +55,14 @@
     assert samples.count() == 2
     # THEN the fetched samples have the subject id used for filtering
     assert all(fetched_sample.subject_id == test_subject for fetched_sample in samples.all())
 
 
 def test_get_samples_by_customer_and_subject_id_query_missing_subject_id(
     store_with_samples_and_tumour_status_missing_subject_id: Store,
-    helpers: StoreHelpers,
     cust123: str,
     test_subject: str,
 ):
     """Test that samples can be fetched by subject id."""
     # GIVEN a database with two samples that have a subject ID but only one is tumour
 
     # GIVEN that there are two samples in the store
@@ -85,15 +83,14 @@
 
     # THEN two samples should be returned
     assert samples.count() == 0
 
 
 def test_get_samples_by_subject_id(
     store_with_samples_subject_id_and_tumour_status: Store,
-    helpers: StoreHelpers,
     cust123: str,
     test_subject: str,
 ):
     """Test that samples can be fetched by subject id."""
     # GIVEN a database with two samples that have a subject ID but only one is tumour
 
     # ASSERT that there are two samples in the store
@@ -111,42 +108,14 @@
         )
     )
 
     # THEN two samples should be returned
     assert samples and len(samples) == 2
 
 
-def test_get_samples_by_subject_id_and_is_tumour(
-    store_with_samples_subject_id_and_tumour_status: Store,
-    helpers: StoreHelpers,
-    cust123: str,
-    test_subject: str,
-    is_tumour: bool = True,
-):
-    """Test that samples can be fetched by subject id."""
-    # GIVEN a database with two samples that have a subject ID but only one is tumour
-
-    # ASSERT that there are two samples in the store
-    assert len(store_with_samples_subject_id_and_tumour_status._get_query(table=Sample).all()) == 2
-
-    # ASSERT that there is a customer with the given customer id
-    assert store_with_samples_subject_id_and_tumour_status.get_customer_by_internal_id(
-        customer_internal_id=cust123
-    )
-    # WHEN fetching the sample by subject id and customer_id
-    samples: List[
-        Sample
-    ] = store_with_samples_subject_id_and_tumour_status.get_samples_by_customer_subject_id_and_is_tumour(
-        subject_id=test_subject, customer_internal_id=cust123, is_tumour=is_tumour
-    )
-
-    # THEN two samples should be returned
-    assert samples and len(samples) == 1
-
-
 def test_get_samples_by_customer_id_list_and_subject_id_and_is_tumour(
     store_with_samples_customer_id_and_subject_id_and_tumour_status: Store,
     customer_ids: List[int] = [1, 2],
     subject_id: str = "test_subject",
     is_tumour: bool = True,
 ):
     """Test that samples can be fetched by customer ID, subject ID, and tumour status."""
@@ -174,15 +143,14 @@
         assert sample.customer_id == customer_id
         assert sample.subject_id == subject_id
         assert sample.is_tumour == is_tumour
 
 
 def test_get_samples_by_customer_id_list_and_subject_id_and_is_tumour_with_non_existing_customer_id(
     store_with_samples_customer_id_and_subject_id_and_tumour_status: Store,
-    helpers: StoreHelpers,
 ):
     """Test that no samples are returned when filtering on non-existing customer ID."""
     # GIVEN a database with four samples, two with customer ID 1 and two with customer ID 2
 
     # ASSERT that there are no customers with the given customer IDs
     customer_ids = [1, 2, 3]
     for customer_id in customer_ids:
@@ -219,65 +187,44 @@
     # WHEN fetching the sample by name
     samples: Sample = store_with_samples_that_have_names.get_sample_by_name(name=name)
 
     # THEN one sample should be returned
     assert samples and samples.name == name
 
 
-def test_get_samples_by_name_pattern(
-    store_with_samples_that_have_names: Store, name_pattern="sample"
-):
-    """Test that samples can be fetched by name."""
-    # GIVEN a database with two samples of which one has a name
-
-    # ASSERT that there are two samples in the store
-    assert len(store_with_samples_that_have_names._get_query(table=Sample).all()) == 4
-
-    # WHEN fetching the sample by name
-    samples: List[Sample] = store_with_samples_that_have_names.get_samples_by_name_pattern(
-        name_pattern=name_pattern
-    )
-
-    # THEN one sample should be returned
-    assert samples and len(samples) == 3
-
-
 def test_has_active_cases_for_sample_analyze(
     store_with_active_sample_analyze: Store,
-    helpers: StoreHelpers,
     sample_internal_id: str = "test_sample_internal_id",
 ):
     """Test that a sample is active."""
     # GIVEN a store with an active case
 
     # THEN the sample should be active
     assert (
         store_with_active_sample_analyze.has_active_cases_for_sample(internal_id=sample_internal_id)
         is True
     )
 
 
 def test_has_active_cases_for_sample_running(
     store_with_active_sample_running: Store,
-    helpers: StoreHelpers,
     sample_internal_id: str = "test_sample_internal_id",
 ):
     """Test that a sample is active."""
     # GIVEN a store with an active case
 
     # THEN the sample should be active
     assert (
         store_with_active_sample_running.has_active_cases_for_sample(internal_id=sample_internal_id)
         is True
     )
 
 
 def test_get_samples_by_customer_and_name(
     store_with_samples_that_have_names: Store,
-    helpers: StoreHelpers,
     name: str = "test_sample_1",
     customer_id="cust000",
 ):
     """Test that samples can be fetched by name."""
     # GIVEN a database with samples
     # WHEN getting a customer from the store
     customer: Customer = store_with_samples_that_have_names.get_customer_by_internal_id(
@@ -293,15 +240,14 @@
     assert sample
     assert sample.name == name
     assert sample.customer == customer
 
 
 def test_get_samples_by_customer_and_name_invalid_customer(
     store_with_samples_that_have_names: Store,
-    helpers: StoreHelpers,
     name: str = "test_sample_1",
     customer_id="unrelated_customer",
 ):
     """Test that samples can be fetched by name does not return a sample when invalid customer is supplied."""
     # GIVEN a database with two samples
 
     # WHEN getting a customer from the store
```

### Comparing `cg-32.2.4/tests/store/api/status/test_analyses_to_clean.py` & `cg-32.2.5/tests/store/api/status/test_analyses_to_clean.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/store/api/status/test_analyses_to_delivery_report.py` & `cg-32.2.5/tests/store/api/status/test_analyses_to_delivery_report.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/store/api/status/test_store_api_status.py` & `cg-32.2.5/tests/store/api/status/test_store_api_status.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/store/api/status/test_store_api_status_analysis.py` & `cg-32.2.5/tests/store/api/status/test_store_api_status_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/store/api/status/test_store_api_status_cases.py` & `cg-32.2.5/tests/store/api/status/test_store_api_status_cases.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/store/api/status/test_store_api_status_customer.py` & `cg-32.2.5/tests/store/api/status/test_store_api_status_customer.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/store/api/status/test_store_api_status_pool.py` & `cg-32.2.5/tests/store/api/status/test_store_api_status_pool.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/store/api/status/test_store_api_status_sample.py` & `cg-32.2.5/tests/store/api/status/test_store_api_status_sample.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/store/api/test_base.py` & `cg-32.2.5/tests/store/api/test_base.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/store/conftest.py` & `cg-32.2.5/tests/store/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -183,20 +183,14 @@
 
 @pytest.fixture(name="invalid_application_tag")
 def fixture_invalid_application_tag() -> str:
     """Return an invalid application tag."""
     return "invalid-tag"
 
 
-@pytest.fixture(name="invalid_application_version_version")
-def fixture_invalid_application_version_version() -> int:
-    """Return an invalid version of an Application Version."""
-    return -1
-
-
 @pytest.fixture(name="store_with_a_sample_that_has_many_attributes_and_one_without")
 def fixture_store_with_a_sample_that_has_many_attributes_and_one_without(
     store: Store,
     helpers: StoreHelpers,
     timestamp_now=dt.datetime.now(),
 ) -> Store:
     """Return a store with a sample that has many attributes and one without."""
@@ -359,25 +353,14 @@
         store=store,
         invoice_id=StoreConstants.INVOICE_ID_INVOICE_WITHOUT_ATTRIBUTES.value,
         invoiced_at=None,
     )
     return store
 
 
-@pytest.fixture(name="store_with_case_and_analysis")
-def fixture_store_with_case_and_analysis(
-    store: Store, helpers: StoreHelpers, analysis_type: str = "wgs"
-) -> Store:
-    """Return a store with a case and analysis."""
-    # GIVEN a store with a case and analysis
-    case = helpers.add_case(store=store, name="test_case", internal_id="test_case_internal_id")
-    helpers.add_analysis(store=store, case=case)
-    yield store
-
-
 @pytest.fixture(name="store_with_older_and_newer_analyses")
 def fixture_store_with_older_and_newer_analyses(
     base_store: Store,
     helpers: StoreHelpers,
     case: Family,
     timestamp_now: dt.datetime,
     timestamp_yesterday: dt.datetime,
```

### Comparing `cg-32.2.4/tests/store/filters/test_status_analyses_filters.py` & `cg-32.2.5/tests/store/filters/test_status_analyses_filters.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,14 @@
     filter_analyses_not_cleaned,
     filter_analyses_not_uploaded_to_vogue,
     filter_analyses_started_before,
     filter_analyses_with_delivery_report,
     filter_analyses_with_pipeline,
     filter_analyses_without_delivery_report,
     filter_completed_analyses,
-    filter_not_completed_analyses,
     filter_not_uploaded_analyses,
     filter_report_analyses_by_pipeline,
     filter_uploaded_analyses,
     filter_valid_analyses_in_production,
     order_analyses_by_completed_at_asc,
     order_analyses_by_uploaded_at_asc,
 )
@@ -91,30 +90,14 @@
     # ASSERT that analyses is a query
     assert isinstance(analyses, Query)
 
     # THEN the completed analysis should be obtained
     assert analysis in analyses
 
 
-def test_filter_not_completed_analyses(base_store: Store, helpers: StoreHelpers):
-    """Test filtering of ongoing analyses."""
-
-    # GIVEN a mock not completed analysis
-    analysis_not_completed: Analysis = helpers.add_analysis(store=base_store, completed_at=None)
-
-    # WHEN retrieving the not completed analyses
-    analyses: Query = filter_not_completed_analyses(analyses=base_store._get_query(table=Analysis))
-
-    # ASSERT that analyses is a query
-    assert isinstance(analyses, Query)
-
-    # THEN the expected analysis should be retrieved
-    assert analysis_not_completed in analyses
-
-
 def test_filter_filter_uploaded_analyses(
     base_store: Store, helpers: StoreHelpers, timestamp_now: datetime
 ):
     """Test filtering of analysis with an uploaded_at field."""
 
     # GIVEN a mock uploaded analysis
     analysis: Analysis = helpers.add_analysis(store=base_store, uploaded_at=timestamp_now)
```

### Comparing `cg-32.2.4/tests/store/filters/test_status_application_filters.py` & `cg-32.2.5/tests/store/filters/test_status_application_filters.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,9 @@
 from cg.store.filters.status_application_filters import (
-    filter_applications_by_entry_id,
-    filter_applications_by_prep_category,
     filter_applications_by_tag,
-    filter_applications_is_archived,
     filter_applications_is_external,
     filter_applications_is_not_external,
     filter_applications_is_not_archived,
 )
 
 from cg.store import Store
 from cg.store.models import Application
@@ -32,64 +29,14 @@
     # ASSERT that application is a query
     assert isinstance(application, Query)
 
     # THEN assert the application was found
     assert application.all() and len(application.all()) == 1 and application.all()[0].tag == tag
 
 
-def test_filter_get_applications_by_prep_category(
-    store_with_an_application_with_and_without_attributes: Store,
-    prep_category=StoreConstants.PREP_CATEGORY_APPLICATION_WITH_ATTRIBUTES.value,
-) -> None:
-    """Test to get application by prep category."""
-    #  GIVEN a store with two applications of which one is of a prep category
-
-    # WHEN getting an application by prep category
-    application: Query = filter_applications_by_prep_category(
-        applications=store_with_an_application_with_and_without_attributes._get_query(
-            table=Application
-        ),
-        prep_category=prep_category,
-    )
-
-    # ASSERT that application is a query
-    assert isinstance(application, Query)
-
-    # THEN assert the application was found
-    assert (
-        application.all()
-        and len(application.all()) == 1
-        and application.all()[0].prep_category == prep_category
-    )
-
-
-def test_filter_get_applications_is_archived(
-    store_with_an_application_with_and_without_attributes: Store,
-) -> None:
-    """Test to get application by is_archived."""
-    # GIVEN a store with two applications of which one is archived
-
-    # WHEN getting an application by is_archived
-    application: Query = filter_applications_is_archived(
-        applications=store_with_an_application_with_and_without_attributes._get_query(
-            table=Application
-        )
-    )
-
-    # ASSERT that application is a query
-    assert isinstance(application, Query)
-
-    # THEN assert the application was found
-    assert (
-        application.all()
-        and len(application.all()) == 1
-        and application.all()[0].is_archived is True
-    )
-
-
 def test_filter_application_is_not_archived(
     store_with_an_application_with_and_without_attributes: Store,
 ) -> None:
     """Test to get application when no archived."""
     # GIVEN a store with two applications of which one is archived
 
     # WHEN getting an application that is not archived
@@ -152,29 +99,7 @@
 
     # THEN assert the application was found
     assert (
         application.all()
         and len(application.all()) == 1
         and application.all()[0].is_external is False
     )
-
-
-def test_filter_get_applications_by_entry_id(
-    store_with_an_application_with_and_without_attributes: Store,
-    entry_id: int = 1,
-) -> None:
-    """Test to get application by id."""
-    # GIVEN a database with an application two applications
-
-    # WHEN getting an application by id
-    application: Query = filter_applications_by_entry_id(
-        applications=store_with_an_application_with_and_without_attributes._get_query(
-            table=Application
-        ),
-        entry_id=entry_id,
-    )
-
-    # ASSERT that applications is a query
-    assert isinstance(application, Query)
-
-    # THEN assert the application was found
-    assert application.all() and len(application.all()) == 1 and application.all()[0].id == entry_id
```

### Comparing `cg-32.2.4/tests/store/filters/test_status_application_version_filters.py` & `cg-32.2.5/tests/store/filters/test_status_application_version_filters.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,25 +4,23 @@
 from sqlalchemy.orm import Query
 
 from cg.store import Store
 from cg.store.filters.status_application_version_filters import (
     filter_application_versions_by_application_entry_id,
     filter_application_versions_before_valid_from,
     filter_application_versions_by_application_version_entry_id,
-    filter_application_versions_by_version,
     order_application_versions_by_valid_from_desc,
 )
 from cg.store.models import Application, ApplicationVersion
 
 from tests.store_helpers import StoreHelpers
 
 
 def test_filter_application_version_by_application_entry_id_correct_id(
     base_store: Store,
-    helpers: StoreHelpers,
 ):
     """Test that the correct application version is returned when using a correct application entry id."""
     # GIVEN a store with application versions
     app_version_query: Query = base_store._get_query(table=ApplicationVersion)
 
     # GIVEN an application in store different in id from at least another application in store
     application: Application = base_store.get_applications()[0]
@@ -43,15 +41,14 @@
         for application_version in filtered_app_version_query.all()
     ]
     assert all(application_id == application.id for application_id in application_ids)
 
 
 def test_filter_application_version_by_application_entry_id_wrong_id(
     base_store: Store,
-    helpers: StoreHelpers,
     invalid_application_id: int,
 ):
     """Test that an empty query is returned when using an incorrect application id."""
     # GIVEN a store with application versions
     app_version_query: Query = base_store._get_query(table=ApplicationVersion)
 
     # WHEN filtering with an invalid application id
@@ -166,78 +163,14 @@
     )
 
     # THEN the function returns an empty query
     assert isinstance(filtered_app_version_query, Query)
     assert filtered_app_version_query.count() == 0
 
 
-def test_filter_application_version_by_version_correct_version(
-    store_with_different_application_versions: Store,
-):
-    """Test that filtering by a valid version returns an application version with the correct version."""
-    # GIVEN a store with application versions with different versions
-    app_version_query: Query = store_with_different_application_versions._get_query(
-        table=ApplicationVersion
-    ).order_by(ApplicationVersion.version)
-    version_to_filter: int = app_version_query.first().version
-    version_to_exclude: int = app_version_query.offset(1).first().version
-    assert version_to_filter != version_to_exclude
-
-    # WHEN filtering the application version query using the valid version
-    filtered_app_version_query: Query = filter_application_versions_by_version(
-        application_versions=app_version_query,
-        version=version_to_filter,
-    )
-
-    # THEN the filtered query has fewer elements than the unfiltered query
-    assert filtered_app_version_query.count() < app_version_query.count()
-    # THEN the version of all the filtered query entries is equal to the version used to filter
-    versions: List[int] = [
-        application_version.version for application_version in filtered_app_version_query.all()
-    ]
-    assert all(version == version_to_filter for version in versions)
-
-
-def test_filter_application_version_by_version_invalid_version_returns_empty(
-    base_store: Store,
-    invalid_application_version_version: int,
-):
-    """Test that an empty query is returned if a non-existent version is used to filter."""
-    # GIVEN a store with application versions
-    app_version_query: Query = base_store._get_query(
-        table=ApplicationVersion,
-    )
-
-    # WHEN filtering by version using an invalid version
-    filtered_app_version_query: Query = filter_application_versions_by_version(
-        application_versions=app_version_query,
-        version=invalid_application_version_version,
-    )
-
-    # THEN the filtered query is empty
-    assert filtered_app_version_query.count() == 0
-
-
-def test_filter_application_version_by_version_empty_query(store: Store, version: int = 1):
-    """Test that filtering an empty query by version returns an empty query."""
-    # GIVEN a store without any application version
-    app_version_query: Query = store._get_query(table=ApplicationVersion)
-    assert app_version_query.count() == 0
-
-    # WHEN filtering by application id
-    filtered_app_version_query: Query = filter_application_versions_by_version(
-        application_versions=app_version_query,
-        version=version,
-    )
-
-    # THEN the function returns an empty query
-    assert isinstance(filtered_app_version_query, Query)
-    assert filtered_app_version_query.count() == 0
-
-
 def test_order_application_versions_by_valid_from_desc(
     base_store: Store,
 ):
     """Test that ordering an application version query returns a query ordered by 'valid_from'."""
     # GIVEN a store with application versions with different dates
     app_version_query: Query = base_store._get_query(table=ApplicationVersion)
```

### Comparing `cg-32.2.4/tests/store/filters/test_status_bed_filters.py` & `cg-32.2.5/tests/store/filters/test_status_bed_filters.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/store/filters/test_status_bed_version_filters.py` & `cg-32.2.5/tests/store/filters/test_status_bed_version_filters.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/store/filters/test_status_cases_filters.py` & `cg-32.2.5/tests/store/filters/test_status_cases_filters.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
     filter_cases_by_customer_entry_ids,
     filter_cases_by_entry_id,
     filter_case_by_internal_id,
     filter_cases_by_name,
     filter_cases_by_pipeline_search,
     filter_cases_by_priority,
     filter_cases_not_analysed,
-    get_newer_cases_by_creation_date,
     get_newer_cases_by_order_date,
     get_running_cases,
     filter_cases_by_ticket_id,
     get_cases_with_pipeline,
     get_cases_has_sequence,
     get_cases_for_analysis,
     get_cases_with_scout_data_delivery,
@@ -559,53 +558,14 @@
     # ASSERT that cases is a query
     assert isinstance(cases, Query)
 
     # THEN cases should not contain the test case
     assert not cases.all()
 
 
-def test_get_newer_cases_none_when_all_cases_older(
-    base_store: Store, helpers: StoreHelpers, timestamp_in_2_weeks: datetime
-):
-    """Test that no cases are returned when all cases are older than the given date."""
-
-    # GIVEN a cases Query
-    helpers.add_case(base_store)
-    cases: Query = base_store._get_query(table=Family)
-
-    # WHEN getting newer cases
-    cases: Query = get_newer_cases_by_creation_date(cases=cases, creation_date=timestamp_in_2_weeks)
-
-    # ASSERT that cases is a query
-    assert isinstance(cases, Query)
-
-    # THEN no cases should be returned
-    assert not cases.all()
-
-
-def test_get_newer_cases_all_when_all_cases_newer(
-    base_store: Store, helpers: StoreHelpers, timestamp_yesterday: datetime
-):
-    """Test that all cases are returned when all cases are newer than the given date."""
-    # GIVEN a cases Query
-    helpers.add_case(base_store)
-    cases: Query = base_store._get_query(table=Family)
-
-    # WHEN getting newer cases
-    filtered_cases: Query = get_newer_cases_by_creation_date(
-        cases=cases, creation_date=timestamp_yesterday
-    )
-
-    # ASSERT that cases is a query
-    assert isinstance(filtered_cases, Query)
-
-    # THEN all cases should be returned
-    assert filtered_cases.count() == cases.count()
-
-
 def test_filter_case_by_existing_entry_id(store_with_multiple_cases_and_samples: Store):
     # GIVEN a store containing a case with an entry id
     cases_query: Query = store_with_multiple_cases_and_samples._get_query(table=Family)
     entry_id: int = cases_query.first().id
     assert entry_id
 
     # WHEN filtering for cases with the entry_id
```

### Comparing `cg-32.2.4/tests/store/filters/test_status_collaboration_filters.py` & `cg-32.2.5/tests/store/filters/test_status_collaboration_filters.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/store/filters/test_status_customer_filters.py` & `cg-32.2.5/tests/store/filters/test_status_customer_filters.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/store/filters/test_status_flow_cell_filters.py` & `cg-32.2.5/tests/store/filters/test_status_flow_cell_filters.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/store/filters/test_status_invoice_filters.py` & `cg-32.2.5/tests/store/filters/test_status_invoice_filters.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/store/filters/test_status_organism_filters.py` & `cg-32.2.5/tests/store/filters/test_status_organism_filters.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/store/filters/test_status_panel_filters.py` & `cg-32.2.5/tests/store/filters/test_status_panel_filters.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/store/filters/test_status_pool_filters.py` & `cg-32.2.5/tests/store/filters/test_status_pool_filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from cg.store.filters.status_pool_filters import (
     filter_pools_is_received,
     filter_pools_is_not_received,
     filter_pools_is_delivered,
     filter_pools_is_not_delivered,
     filter_pools_without_invoice_id,
     filter_pools_do_invoice,
-    filter_pools_do_not_invoice,
     filter_pools_by_invoice_id,
     filter_pools_by_order_enquiry,
     filter_pools_by_name_enquiry,
     filter_pools_by_customer_id,
 )
 from tests.store.conftest import StoreConstants
 
@@ -117,40 +116,14 @@
     # THEN only one pool should be returned
     assert len(pools.all()) == 1
 
     # THEN the pool should have the expected name
     assert pools.all()[0].name == name
 
 
-def test_filter_pools_do_not_invoice(
-    store_with_a_pool_with_and_without_attributes: Store,
-    name=StoreConstants.NAME_POOL_WITHOUT_ATTRIBUTES.value,
-):
-    """Test that a pool is returned when there is a pool that should not be invoiced."""
-
-    # GIVEN a pool marked to skip invoicing and one not marked to skip invoicing
-
-    # WHEN getting pools marked to skip invoicing
-    pools: Query = filter_pools_do_not_invoice(
-        pools=store_with_a_pool_with_and_without_attributes._get_query(table=Pool)
-    )
-
-    # ASSERT that the query is a Query
-    assert isinstance(pools, Query)
-
-    # THEN pools should contain the test pool
-    assert pools.all()
-
-    # THEN only one pool should be returned
-    assert len(pools.all()) == 1
-
-    # THEN the pool should have the expected name
-    assert pools.all()[0].name == name
-
-
 def test_filter_pools_do_invoice(
     store_with_a_pool_with_and_without_attributes: Store,
     name=StoreConstants.NAME_POOL_WITH_ATTRIBUTES.value,
 ):
     """Test that a pool is returned when there is a pool that should be invoiced."""
 
     # GIVEN a pool marked for invoicing and one not marked for invoicing
@@ -279,15 +252,14 @@
 
     # THEN the pool should have the expected name
     assert pools.all()[0].name == name
 
 
 def test_filter_pools_by_customer_id(
     store_with_a_pool_with_and_without_attributes: Store,
-    name=StoreConstants.NAME_POOL_WITH_ATTRIBUTES.value,
 ):
     """Test that a pool is returned when there is a pool with a specific customer id."""
 
     # GIVEN a store with two pools of with the same customer
 
     # WHEN getting pools with customer id
     pools: Query = filter_pools_by_customer_id(
```

### Comparing `cg-32.2.4/tests/store/filters/test_status_samples_filters.py` & `cg-32.2.5/tests/store/filters/test_status_samples_filters.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,32 +7,29 @@
 
 from cg.store.filters.status_sample_filters import (
     filter_samples_with_loqusdb_id,
     filter_samples_without_loqusdb_id,
     filter_samples_is_delivered,
     filter_samples_is_not_delivered,
     filter_samples_without_invoice_id,
-    filter_samples_is_down_sampled,
     filter_samples_is_not_down_sampled,
     filter_samples_is_sequenced,
     filter_samples_is_not_sequenced,
     filter_samples_do_invoice,
-    filter_samples_do_not_invoice,
     filter_samples_by_invoice_id,
     filter_samples_by_internal_id,
     filter_samples_by_entry_id,
     filter_samples_with_type,
     filter_samples_is_prepared,
     filter_samples_is_not_prepared,
     filter_samples_is_received,
     filter_samples_is_not_received,
     filter_samples_by_name,
     filter_samples_by_subject_id,
     filter_samples_by_entry_customer_ids,
-    filter_samples_by_name_pattern,
     filter_samples_by_internal_id_pattern,
     filter_samples_by_identifier_name_and_value,
 )
 from tests.store.conftest import StoreConstants
 
 
 def test_get_samples_with_loqusdb_id(helpers, store, sample_store, sample_id, loqusdb_id):
@@ -185,41 +182,14 @@
     # THEN samples should contain one sample
     assert len(samples.all()) == 1
 
     # THEN the sample should not have an invoice id
     assert samples.all()[0].invoice_id is None
 
 
-def test_filter_samples_down_sampled(
-    store_with_a_sample_that_has_many_attributes_and_one_without: Store,
-):
-    """Test that a sample is returned when there is a sample that is not down sampled."""
-
-    # GIVEN a store with two samples of which one is not sequenced
-
-    # WHEN getting not sequenced samples
-    samples: Query = filter_samples_is_down_sampled(
-        samples=store_with_a_sample_that_has_many_attributes_and_one_without._get_query(
-            table=Sample
-        )
-    )
-
-    # ASSERT that samples is a query
-    assert isinstance(samples, Query)
-
-    # THEN samples should contain the test sample
-    assert samples.all()
-
-    # THEN samples should contain one sample
-    assert len(samples.all()) == 1
-
-    # THEN the sample should have a down sampled to value
-    assert samples.all()[0].downsampled_to is not None
-
-
 def test_filter_samples_not_down_sampled(
     store_with_a_sample_that_has_many_attributes_and_one_without: Store,
 ):
     """Test that a sample is returned when there is a sample that is not down sampled."""
 
     # GIVEN a store with two samples of which one is not sequenced
 
@@ -320,41 +290,14 @@
     # THEN samples should contain one sample
     assert len(samples.all()) == 1
 
     # THEN the sample should have a no invoice indicator that is set to False
     assert samples.all()[0].no_invoice is False
 
 
-def test_filter_samples_do_not_invoice(
-    store_with_a_sample_that_has_many_attributes_and_one_without: Store,
-):
-    """Test that a sample is returned when there is not a sample that should be invoiced."""
-
-    # GIVEN a  store with two samples of which one is marked to skip invoicing
-
-    # WHEN getting samples that are marked to skip invoicing
-    samples: Query = filter_samples_do_not_invoice(
-        samples=store_with_a_sample_that_has_many_attributes_and_one_without._get_query(
-            table=Sample
-        )
-    )
-
-    # ASSERT that samples is a query
-    assert isinstance(samples, Query)
-
-    # THEN samples should contain the test sample
-    assert samples.all()
-
-    # THEN samples should contain one sample
-    assert len(samples.all()) == 1
-
-    # THEN the sample should have a no invoice indicator that is set to True
-    assert samples.all()[0].no_invoice is True
-
-
 def test_filter_samples_is_received(
     store_with_a_sample_that_has_many_attributes_and_one_without: Store,
 ):
     """Test that a sample is returned when there is a sample that is received."""
 
     # GIVEN a store with two samples of which one is received
 
@@ -622,42 +565,14 @@
     # THEN the filtered query has fewer elements than the unfiltered query
     assert filtered_query.count() < samples.count()
 
     # THEN a sample in the filtered query should have the correct customer id
     assert filtered_query.first().customer_id == customer_id
 
 
-def test_filter_get_samples_by_name_pattern(
-    store_with_a_sample_that_has_many_attributes_and_one_without: Store,
-    name_pattern: str = StoreConstants.NAME_SAMPLE_WITH_ATTRIBUTES.value,
-):
-    """Test that a sample is returned when there is a sample with the given name pattern."""
-    # GIVEN a store with two samples of which one has a name name pattern
-
-    # WHEN getting a sample by name pattern
-    samples: Query = filter_samples_by_name_pattern(
-        samples=store_with_a_sample_that_has_many_attributes_and_one_without._get_query(
-            table=Sample
-        ),
-        name_pattern=name_pattern,
-    )
-
-    # ASSERT that samples is a query
-    assert isinstance(samples, Query)
-
-    # THEN samples should contain the test sample
-    assert samples.all()
-
-    # THEN samples should contain one sample
-    assert len(samples.all()) == 1
-
-    # THEN the sample should have the correct name
-    assert samples[0].name == name_pattern
-
-
 def test_filter_get_samples_by_internal_id_pattern(
     store_with_a_sample_that_has_many_attributes_and_one_without: Store,
     internal_id_pattern: str = "with_attributes",
 ):
     """Test that a sample is returned when there is a sample with the given internal id pattern."""
     # GIVEN a store with two samples of which one has a name name pattern
```

### Comparing `cg-32.2.4/tests/store/filters/test_status_user_filters.py` & `cg-32.2.5/tests/store/filters/test_status_user_filters.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/store/test_delivery.py` & `cg-32.2.5/tests/store/test_delivery.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/store/test_store_models.py` & `cg-32.2.5/tests/store/test_store_models.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/store_helpers.py` & `cg-32.2.5/tests/store_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,16 +118,18 @@
         store: Store,
         application: Application,
         prices: Dict,
         version: int = 1,
         valid_from: datetime = datetime.now(),
     ) -> ApplicationVersion:
         """Add an application version to store."""
-        new_record: ApplicationVersion = store.get_application_version_by_application_entry_id(
-            application_entry_id=application.id
+        new_record = (
+            store._get_query(table=ApplicationVersion)
+            .filter(ApplicationVersion.application_id == application.id)
+            .first()
         )
         if not new_record:
             new_record: ApplicationVersion = store.add_application_version(
                 application=application,
                 version=version,
                 valid_from=valid_from,
                 prices=prices,
@@ -193,26 +195,24 @@
         store.session.add(application)
         store.session.commit()
         return application
 
     @staticmethod
     def ensure_bed_version(store: Store, bed_name: str = "dummy_bed") -> BedVersion:
         """Return existing or create and return bed version for tests."""
-        bed: Optional[Bed] = store.get_bed_by_name(bed_name=bed_name)
+        bed: Optional[Bed] = store._get_query(table=Bed).filter(Bed.name == bed_name)
         if not bed:
             bed: Bed = store.add_bed(name=bed_name)
             store.session.add(bed)
 
-        bed_version: Optional[BedVersion] = store.get_latest_bed_version(bed_name=bed_name)
-        if not bed_version:
-            bed_version: BedVersion = store.add_bed_version(
-                bed=bed, version=1, filename="dummy_filename", shortname=bed_name
-            )
-            store.session.add(bed_version)
-            store.session.commit()
+        bed_version: BedVersion = store.add_bed_version(
+            bed=bed, version=1, filename="dummy_filename", shortname=bed_name
+        )
+        store.session.add(bed_version)
+        store.session.commit()
         return bed_version
 
     @staticmethod
     def ensure_collaboration(store: Store, collaboration_id: str = "all_customers"):
         collaboration = store.get_collaboration_by_internal_id(collaboration_id)
         if not collaboration:
             collaboration = store.add_collaboration(collaboration_id, collaboration_id)
```

### Comparing `cg-32.2.4/tests/test_store_helpers.py` & `cg-32.2.5/tests/test_store_helpers.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/utils/conftest.py` & `cg-32.2.5/tests/utils/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/utils/test_commands.py` & `cg-32.2.5/tests/utils/test_commands.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/utils/test_date.py` & `cg-32.2.5/tests/utils/test_date.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/utils/test_dict.py` & `cg-32.2.5/tests/utils/test_dict.py`

 * *Files identical despite different names*

### Comparing `cg-32.2.4/tests/utils/test_dispatcher.py` & `cg-32.2.5/tests/utils/test_dispatcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,20 +146,18 @@
     helpers.add_sample(store, subject_id=test_subject)
     helpers.add_sample(store, subject_id=test_subject, is_tumour=False)
 
     # WHEN calling the dispatcher with the customer and subject id
     dispatcher = Dispatcher(
         functions=[
             store.get_samples_by_customer_and_subject_id,
-            store.get_samples_by_customer_subject_id_and_is_tumour,
         ],
         input_dict={
             "customer_internal_id": customer_internal_id,
             "subject_id": test_subject,
-            "is_tumour": is_tumour,
         },
     )
     # THEN the dispatcher should return the correct samples
     samples: List[Sample] = dispatcher()
     for sample in samples:
         assert sample.customer.internal_id == customer_internal_id
         assert sample.subject_id == test_subject
```

### Comparing `cg-32.2.4/tests/utils/test_utils.py` & `cg-32.2.5/tests/utils/test_utils.py`

 * *Files identical despite different names*

