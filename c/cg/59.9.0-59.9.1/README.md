# Comparing `tmp/cg-59.9.0.tar.gz` & `tmp/cg-59.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cg-59.9.0.tar", max compression
+gzip compressed data, was "cg-59.9.1.tar", max compression
```

## Comparing `cg-59.9.0.tar` & `cg-59.9.1.tar`

### file list

```diff
@@ -1,1296 +1,1296 @@
--rw-r--r--   0        0        0     2686 2024-03-01 09:19:24.066125 cg-59.9.0/README.md
--rw-r--r--   0        0        0       40 2024-03-01 09:19:24.066125 cg-59.9.0/cg/__init__.py
--rw-r--r--   0        0        0      315 2024-03-01 09:19:24.066125 cg-59.9.0/cg/apps/__init__.py
--rw-r--r--   0        0        0       27 2024-03-01 09:19:24.066125 cg-59.9.0/cg/apps/coverage/__init__.py
--rw-r--r--   0        0        0     2940 2024-03-01 09:19:24.066125 cg-59.9.0/cg/apps/coverage/api.py
--rw-r--r--   0        0        0       56 2024-03-01 09:19:24.066125 cg-59.9.0/cg/apps/crunchy/__init__.py
--rw-r--r--   0        0        0    12783 2024-03-01 09:19:24.066125 cg-59.9.0/cg/apps/crunchy/crunchy.py
--rw-r--r--   0        0        0     4502 2024-03-01 09:19:24.066125 cg-59.9.0/cg/apps/crunchy/files.py
--rw-r--r--   0        0        0      430 2024-03-01 09:19:24.066125 cg-59.9.0/cg/apps/crunchy/models.py
--rw-r--r--   0        0        0      910 2024-03-01 09:19:24.066125 cg-59.9.0/cg/apps/crunchy/sbatch.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.070125 cg-59.9.0/cg/apps/demultiplex/__init__.py
--rw-r--r--   0        0        0    12262 2024-03-01 09:19:24.070125 cg-59.9.0/cg/apps/demultiplex/demultiplex_api.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.070125 cg-59.9.0/cg/apps/demultiplex/sample_sheet/__init__.py
--rw-r--r--   0        0        0     8576 2024-03-01 09:19:24.070125 cg-59.9.0/cg/apps/demultiplex/sample_sheet/api.py
--rw-r--r--   0        0        0     1581 2024-03-01 09:19:24.070125 cg-59.9.0/cg/apps/demultiplex/sample_sheet/create.py
--rw-r--r--   0        0        0     4227 2024-03-01 09:19:24.070125 cg-59.9.0/cg/apps/demultiplex/sample_sheet/index.py
--rw-r--r--   0        0        0     7341 2024-03-01 09:19:24.070125 cg-59.9.0/cg/apps/demultiplex/sample_sheet/override_cycles_validator.py
--rw-r--r--   0        0        0     4166 2024-03-01 09:19:24.070125 cg-59.9.0/cg/apps/demultiplex/sample_sheet/read_sample_sheet.py
--rw-r--r--   0        0        0    10542 2024-03-01 09:19:24.070125 cg-59.9.0/cg/apps/demultiplex/sample_sheet/sample_models.py
--rw-r--r--   0        0        0     9851 2024-03-01 09:19:24.070125 cg-59.9.0/cg/apps/demultiplex/sample_sheet/sample_sheet_creator.py
--rw-r--r--   0        0        0     1614 2024-03-01 09:19:24.070125 cg-59.9.0/cg/apps/demultiplex/sample_sheet/sample_sheet_models.py
--rw-r--r--   0        0        0     9644 2024-03-01 09:19:24.070125 cg-59.9.0/cg/apps/demultiplex/sample_sheet/sample_sheet_validator.py
--rw-r--r--   0        0        0      824 2024-03-01 09:19:24.070125 cg-59.9.0/cg/apps/demultiplex/sample_sheet/validators.py
--rw-r--r--   0        0        0     1943 2024-03-01 09:19:24.070125 cg-59.9.0/cg/apps/demultiplex/sbatch.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.070125 cg-59.9.0/cg/apps/downsample/__init__.py
--rw-r--r--   0        0        0     6160 2024-03-01 09:19:24.070125 cg-59.9.0/cg/apps/downsample/downsample.py
--rw-r--r--   0        0        0     2125 2024-03-01 09:19:24.070125 cg-59.9.0/cg/apps/downsample/utils.py
--rw-r--r--   0        0        0      298 2024-03-01 09:19:24.070125 cg-59.9.0/cg/apps/environ.py
--rw-r--r--   0        0        0     1741 2024-03-01 09:19:24.070125 cg-59.9.0/cg/apps/gens.py
--rw-r--r--   0        0        0     3419 2024-03-01 09:19:24.070125 cg-59.9.0/cg/apps/gt.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.070125 cg-59.9.0/cg/apps/hermes/__init__.py
--rw-r--r--   0        0        0     2249 2024-03-01 09:19:24.070125 cg-59.9.0/cg/apps/hermes/hermes_api.py
--rw-r--r--   0        0        0     1298 2024-03-01 09:19:24.070125 cg-59.9.0/cg/apps/hermes/models.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.070125 cg-59.9.0/cg/apps/housekeeper/__init__.py
--rw-r--r--   0        0        0    28681 2024-03-01 09:19:24.070125 cg-59.9.0/cg/apps/housekeeper/hk.py
--rw-r--r--   0        0        0      326 2024-03-01 09:19:24.070125 cg-59.9.0/cg/apps/housekeeper/models.py
--rw-r--r--   0        0        0       32 2024-03-01 09:19:24.070125 cg-59.9.0/cg/apps/invoice/__init__.py
--rw-r--r--   0        0        0     4804 2024-03-01 09:19:24.070125 cg-59.9.0/cg/apps/invoice/render.py
--rw-r--r--   0        0        0   113439 2024-03-01 09:19:24.070125 cg-59.9.0/cg/apps/invoice/templates/KI_pool_invoice.xlsx
--rw-r--r--   0        0        0    81032 2024-03-01 09:19:24.070125 cg-59.9.0/cg/apps/invoice/templates/KI_sample_invoice.xlsx
--rw-r--r--   0        0        0   113363 2024-03-01 09:19:24.070125 cg-59.9.0/cg/apps/invoice/templates/KTH_pool_invoice.xlsx
--rw-r--r--   0        0        0    80886 2024-03-01 09:19:24.070125 cg-59.9.0/cg/apps/invoice/templates/KTH_sample_invoice.xlsx
--rw-r--r--   0        0        0       25 2024-03-01 09:19:24.070125 cg-59.9.0/cg/apps/lims/__init__.py
--rw-r--r--   0        0        0    16539 2024-03-01 09:19:24.070125 cg-59.9.0/cg/apps/lims/api.py
--rw-r--r--   0        0        0     2652 2024-03-01 09:19:24.070125 cg-59.9.0/cg/apps/lims/batch.py
--rw-r--r--   0        0        0     8129 2024-03-01 09:19:24.070125 cg-59.9.0/cg/apps/lims/order.py
--rw-r--r--   0        0        0     3302 2024-03-01 09:19:24.070125 cg-59.9.0/cg/apps/lims/sample_sheet.py
--rw-r--r--   0        0        0     4866 2024-03-01 09:19:24.070125 cg-59.9.0/cg/apps/loqus.py
--rw-r--r--   0        0        0       35 2024-03-01 09:19:24.070125 cg-59.9.0/cg/apps/madeline/__init__.py
--rw-r--r--   0        0        0     3213 2024-03-01 09:19:24.070125 cg-59.9.0/cg/apps/madeline/api.py
--rw-r--r--   0        0        0       23 2024-03-01 09:19:24.070125 cg-59.9.0/cg/apps/mip/__init__.py
--rw-r--r--   0        0        0     3564 2024-03-01 09:19:24.070125 cg-59.9.0/cg/apps/mip/confighandler.py
--rw-r--r--   0        0        0     2207 2024-03-01 09:19:24.070125 cg-59.9.0/cg/apps/mutacc_auto.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.070125 cg-59.9.0/cg/apps/orderform/__init__.py
--rw-r--r--   0        0        0     9498 2024-03-01 09:19:24.070125 cg-59.9.0/cg/apps/orderform/excel_orderform_parser.py
--rw-r--r--   0        0        0     3051 2024-03-01 09:19:24.070125 cg-59.9.0/cg/apps/orderform/json_orderform_parser.py
--rw-r--r--   0        0        0     6419 2024-03-01 09:19:24.070125 cg-59.9.0/cg/apps/orderform/orderform_parser.py
--rw-r--r--   0        0        0      252 2024-03-01 09:19:24.070125 cg-59.9.0/cg/apps/orderform/utils.py
--rw-r--r--   0        0        0     2537 2024-03-01 09:19:24.070125 cg-59.9.0/cg/apps/osticket.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.074125 cg-59.9.0/cg/apps/scout/__init__.py
--rw-r--r--   0        0        0     3177 2024-03-01 09:19:24.074125 cg-59.9.0/cg/apps/scout/scout_export.py
--rw-r--r--   0        0        0    11054 2024-03-01 09:19:24.074125 cg-59.9.0/cg/apps/scout/scoutapi.py
--rw-r--r--   0        0        0      444 2024-03-01 09:19:24.074125 cg-59.9.0/cg/apps/scout/validators.py
--rw-r--r--   0        0        0       78 2024-03-01 09:19:24.074125 cg-59.9.0/cg/apps/sequencing_metrics_parser/__init__.py
--rw-r--r--   0        0        0     1854 2024-03-01 09:19:24.074125 cg-59.9.0/cg/apps/sequencing_metrics_parser/api.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.074125 cg-59.9.0/cg/apps/sequencing_metrics_parser/models/__init__.py
--rw-r--r--   0        0        0     1871 2024-03-01 09:19:24.074125 cg-59.9.0/cg/apps/sequencing_metrics_parser/models/bcl2fastq_metrics.py
--rw-r--r--   0        0        0     1076 2024-03-01 09:19:24.074125 cg-59.9.0/cg/apps/sequencing_metrics_parser/models/bcl_convert.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.074125 cg-59.9.0/cg/apps/sequencing_metrics_parser/parsers/__init__.py
--rw-r--r--   0        0        0     7312 2024-03-01 09:19:24.074125 cg-59.9.0/cg/apps/sequencing_metrics_parser/parsers/bcl2fastq.py
--rw-r--r--   0        0        0     2641 2024-03-01 09:19:24.074125 cg-59.9.0/cg/apps/sequencing_metrics_parser/parsers/bcl2fastq_to_sequencing_statistics.py
--rw-r--r--   0        0        0     6806 2024-03-01 09:19:24.074125 cg-59.9.0/cg/apps/sequencing_metrics_parser/parsers/bcl_convert.py
--rw-r--r--   0        0        0     3559 2024-03-01 09:19:24.074125 cg-59.9.0/cg/apps/sequencing_metrics_parser/parsers/bcl_convert_to_sequencing_statistics.py
--rw-r--r--   0        0        0      172 2024-03-01 09:19:24.074125 cg-59.9.0/cg/apps/sequencing_metrics_parser/parsers/utils.py
--rw-r--r--   0        0        0      836 2024-03-01 09:19:24.074125 cg-59.9.0/cg/apps/sequencing_metrics_parser/sequencing_metrics_calculator.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.074125 cg-59.9.0/cg/apps/slurm/__init__.py
--rw-r--r--   0        0        0     1277 2024-03-01 09:19:24.074125 cg-59.9.0/cg/apps/slurm/sbatch.py
--rw-r--r--   0        0        0     3559 2024-03-01 09:19:24.074125 cg-59.9.0/cg/apps/slurm/slurm_api.py
--rw-r--r--   0        0        0       32 2024-03-01 09:19:24.074125 cg-59.9.0/cg/apps/tb/__init__.py
--rw-r--r--   0        0        0     7501 2024-03-01 09:19:24.074125 cg-59.9.0/cg/apps/tb/api.py
--rw-r--r--   0        0        0      152 2024-03-01 09:19:24.074125 cg-59.9.0/cg/apps/tb/dto/create_job_request.py
--rw-r--r--   0        0        0      287 2024-03-01 09:19:24.074125 cg-59.9.0/cg/apps/tb/dto/summary_response.py
--rw-r--r--   0        0        0     1305 2024-03-01 09:19:24.074125 cg-59.9.0/cg/apps/tb/models.py
--rw-r--r--   0        0        0      305 2024-03-01 09:19:24.074125 cg-59.9.0/cg/apps/tb/validators.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.074125 cg-59.9.0/cg/cli/__init__.py
--rw-r--r--   0        0        0    10945 2024-03-01 09:19:24.074125 cg-59.9.0/cg/cli/add.py
--rw-r--r--   0        0        0     2653 2024-03-01 09:19:24.074125 cg-59.9.0/cg/cli/archive.py
--rw-r--r--   0        0        0    10118 2024-03-01 09:19:24.074125 cg-59.9.0/cg/cli/backup.py
--rw-r--r--   0        0        0     3853 2024-03-01 09:19:24.074125 cg-59.9.0/cg/cli/base.py
--rw-r--r--   0        0        0    10506 2024-03-01 09:19:24.074125 cg-59.9.0/cg/cli/clean.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.074125 cg-59.9.0/cg/cli/compress/__init__.py
--rw-r--r--   0        0        0     2135 2024-03-01 09:19:24.074125 cg-59.9.0/cg/cli/compress/base.py
--rw-r--r--   0        0        0     6706 2024-03-01 09:19:24.074125 cg-59.9.0/cg/cli/compress/fastq.py
--rw-r--r--   0        0        0     8163 2024-03-01 09:19:24.074125 cg-59.9.0/cg/cli/compress/helpers.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.074125 cg-59.9.0/cg/cli/delete/__init__.py
--rw-r--r--   0        0        0      564 2024-03-01 09:19:24.074125 cg-59.9.0/cg/cli/delete/base.py
--rw-r--r--   0        0        0     4603 2024-03-01 09:19:24.074125 cg-59.9.0/cg/cli/delete/case.py
--rw-r--r--   0        0        0     1884 2024-03-01 09:19:24.074125 cg-59.9.0/cg/cli/delete/cases.py
--rw-r--r--   0        0        0     2633 2024-03-01 09:19:24.074125 cg-59.9.0/cg/cli/delete/observations.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.074125 cg-59.9.0/cg/cli/deliver/__init__.py
--rw-r--r--   0        0        0     6270 2024-03-01 09:19:24.074125 cg-59.9.0/cg/cli/deliver/base.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.074125 cg-59.9.0/cg/cli/demultiplex/__init__.py
--rw-r--r--   0        0        0      829 2024-03-01 09:19:24.074125 cg-59.9.0/cg/cli/demultiplex/base.py
--rw-r--r--   0        0        0     4905 2024-03-01 09:19:24.074125 cg-59.9.0/cg/cli/demultiplex/copy_novaseqx_demultiplex_data.py
--rw-r--r--   0        0        0     8016 2024-03-01 09:19:24.074125 cg-59.9.0/cg/cli/demultiplex/demux.py
--rw-r--r--   0        0        0     1619 2024-03-01 09:19:24.074125 cg-59.9.0/cg/cli/demultiplex/finish.py
--rw-r--r--   0        0        0     2683 2024-03-01 09:19:24.074125 cg-59.9.0/cg/cli/demultiplex/sample_sheet.py
--rw-r--r--   0        0        0     2995 2024-03-01 09:19:24.074125 cg-59.9.0/cg/cli/downsample.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.074125 cg-59.9.0/cg/cli/generate/__init__.py
--rw-r--r--   0        0        0      356 2024-03-01 09:19:24.074125 cg-59.9.0/cg/cli/generate/base.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.074125 cg-59.9.0/cg/cli/generate/report/__init__.py
--rw-r--r--   0        0        0     4636 2024-03-01 09:19:24.074125 cg-59.9.0/cg/cli/generate/report/base.py
--rw-r--r--   0        0        0      854 2024-03-01 09:19:24.074125 cg-59.9.0/cg/cli/generate/report/options.py
--rw-r--r--   0        0        0     5107 2024-03-01 09:19:24.074125 cg-59.9.0/cg/cli/generate/report/utils.py
--rw-r--r--   0        0        0     8326 2024-03-01 09:19:24.074125 cg-59.9.0/cg/cli/get.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.074125 cg-59.9.0/cg/cli/set/__init__.py
--rw-r--r--   0        0        0     9856 2024-03-01 09:19:24.074125 cg-59.9.0/cg/cli/set/base.py
--rw-r--r--   0        0        0     4384 2024-03-01 09:19:24.074125 cg-59.9.0/cg/cli/set/case.py
--rw-r--r--   0        0        0     2595 2024-03-01 09:19:24.074125 cg-59.9.0/cg/cli/set/cases.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.074125 cg-59.9.0/cg/cli/store/__init__.py
--rw-r--r--   0        0        0     5340 2024-03-01 09:19:24.074125 cg-59.9.0/cg/cli/store/fastq.py
--rw-r--r--   0        0        0     1049 2024-03-01 09:19:24.074125 cg-59.9.0/cg/cli/store/store.py
--rw-r--r--   0        0        0     1761 2024-03-01 09:19:24.074125 cg-59.9.0/cg/cli/transfer.py
--rw-r--r--   0        0        0        1 2024-03-01 09:19:24.074125 cg-59.9.0/cg/cli/upload/__init__.py
--rw-r--r--   0        0        0     5652 2024-03-01 09:19:24.074125 cg-59.9.0/cg/cli/upload/base.py
--rw-r--r--   0        0        0     5238 2024-03-01 09:19:24.074125 cg-59.9.0/cg/cli/upload/clinical_delivery.py
--rw-r--r--   0        0        0     1175 2024-03-01 09:19:24.074125 cg-59.9.0/cg/cli/upload/coverage.py
--rw-r--r--   0        0        0     1528 2024-03-01 09:19:24.074125 cg-59.9.0/cg/cli/upload/delivery_report.py
--rw-r--r--   0        0        0     4022 2024-03-01 09:19:24.074125 cg-59.9.0/cg/cli/upload/fohm.py
--rw-r--r--   0        0        0     1463 2024-03-01 09:19:24.074125 cg-59.9.0/cg/cli/upload/genotype.py
--rw-r--r--   0        0        0     1885 2024-03-01 09:19:24.074125 cg-59.9.0/cg/cli/upload/gens.py
--rw-r--r--   0        0        0      584 2024-03-01 09:19:24.074125 cg-59.9.0/cg/cli/upload/gisaid.py
--rw-r--r--   0        0        0     2645 2024-03-01 09:19:24.074125 cg-59.9.0/cg/cli/upload/mutacc.py
--rw-r--r--   0        0        0       23 2024-03-01 09:19:24.074125 cg-59.9.0/cg/cli/upload/nipt/__init__.py
--rw-r--r--   0        0        0     3006 2024-03-01 09:19:24.074125 cg-59.9.0/cg/cli/upload/nipt/base.py
--rw-r--r--   0        0        0     2275 2024-03-01 09:19:24.074125 cg-59.9.0/cg/cli/upload/nipt/ftp.py
--rw-r--r--   0        0        0     1596 2024-03-01 09:19:24.074125 cg-59.9.0/cg/cli/upload/nipt/statina.py
--rw-r--r--   0        0        0      112 2024-03-01 09:19:24.074125 cg-59.9.0/cg/cli/upload/observations/__init__.py
--rw-r--r--   0        0        0     2672 2024-03-01 09:19:24.074125 cg-59.9.0/cg/cli/upload/observations/observations.py
--rw-r--r--   0        0        0     2904 2024-03-01 09:19:24.074125 cg-59.9.0/cg/cli/upload/observations/utils.py
--rw-r--r--   0        0        0     9970 2024-03-01 09:19:24.074125 cg-59.9.0/cg/cli/upload/scout.py
--rw-r--r--   0        0        0      650 2024-03-01 09:19:24.074125 cg-59.9.0/cg/cli/upload/utils.py
--rw-r--r--   0        0        0     1667 2024-03-01 09:19:24.074125 cg-59.9.0/cg/cli/upload/validate.py
--rw-r--r--   0        0        0      105 2024-03-01 09:19:24.074125 cg-59.9.0/cg/cli/utils.py
--rw-r--r--   0        0        0       18 2024-03-01 09:19:24.078125 cg-59.9.0/cg/cli/workflow/__init__.py
--rw-r--r--   0        0        0       22 2024-03-01 09:19:24.078125 cg-59.9.0/cg/cli/workflow/balsamic/__init__.py
--rw-r--r--   0        0        0     8925 2024-03-01 09:19:24.078125 cg-59.9.0/cg/cli/workflow/balsamic/base.py
--rw-r--r--   0        0        0     1980 2024-03-01 09:19:24.078125 cg-59.9.0/cg/cli/workflow/balsamic/options.py
--rw-r--r--   0        0        0      881 2024-03-01 09:19:24.078125 cg-59.9.0/cg/cli/workflow/balsamic/pon.py
--rw-r--r--   0        0        0     1162 2024-03-01 09:19:24.078125 cg-59.9.0/cg/cli/workflow/balsamic/qc.py
--rw-r--r--   0        0        0     1177 2024-03-01 09:19:24.078125 cg-59.9.0/cg/cli/workflow/balsamic/umi.py
--rw-r--r--   0        0        0     1196 2024-03-01 09:19:24.078125 cg-59.9.0/cg/cli/workflow/base.py
--rw-r--r--   0        0        0    12379 2024-03-01 09:19:24.078125 cg-59.9.0/cg/cli/workflow/commands.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.078125 cg-59.9.0/cg/cli/workflow/fastq/__init__.py
--rw-r--r--   0        0        0     1367 2024-03-01 09:19:24.078125 cg-59.9.0/cg/cli/workflow/fastq/base.py
--rw-r--r--   0        0        0     1787 2024-03-01 09:19:24.078125 cg-59.9.0/cg/cli/workflow/fastq/fastq_service.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.078125 cg-59.9.0/cg/cli/workflow/fluffy/__init__.py
--rw-r--r--   0        0        0     4177 2024-03-01 09:19:24.078125 cg-59.9.0/cg/cli/workflow/fluffy/base.py
--rw-r--r--   0        0        0       22 2024-03-01 09:19:24.078125 cg-59.9.0/cg/cli/workflow/microsalt/__init__.py
--rw-r--r--   0        0        0     7810 2024-03-01 09:19:24.078125 cg-59.9.0/cg/cli/workflow/microsalt/base.py
--rw-r--r--   0        0        0       22 2024-03-01 09:19:24.078125 cg-59.9.0/cg/cli/workflow/mip/__init__.py
--rw-r--r--   0        0        0     6596 2024-03-01 09:19:24.078125 cg-59.9.0/cg/cli/workflow/mip/base.py
--rw-r--r--   0        0        0     1268 2024-03-01 09:19:24.078125 cg-59.9.0/cg/cli/workflow/mip/options.py
--rw-r--r--   0        0        0       22 2024-03-01 09:19:24.078125 cg-59.9.0/cg/cli/workflow/mip_dna/__init__.py
--rw-r--r--   0        0        0     1013 2024-03-01 09:19:24.078125 cg-59.9.0/cg/cli/workflow/mip_dna/base.py
--rw-r--r--   0        0        0       22 2024-03-01 09:19:24.078125 cg-59.9.0/cg/cli/workflow/mip_rna/__init__.py
--rw-r--r--   0        0        0      916 2024-03-01 09:19:24.078125 cg-59.9.0/cg/cli/workflow/mip_rna/base.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.078125 cg-59.9.0/cg/cli/workflow/mutant/__init__.py
--rw-r--r--   0        0        0     3413 2024-03-01 09:19:24.078125 cg-59.9.0/cg/cli/workflow/mutant/base.py
--rw-r--r--   0        0        0     3532 2024-03-01 09:19:24.078125 cg-59.9.0/cg/cli/workflow/nf_analysis.py
--rw-r--r--   0        0        0       22 2024-03-01 09:19:24.078125 cg-59.9.0/cg/cli/workflow/raredisease/__init__.py
--rw-r--r--   0        0        0     1865 2024-03-01 09:19:24.078125 cg-59.9.0/cg/cli/workflow/raredisease/base.py
--rw-r--r--   0        0        0       22 2024-03-01 09:19:24.078125 cg-59.9.0/cg/cli/workflow/rnafusion/__init__.py
--rw-r--r--   0        0        0    10391 2024-03-01 09:19:24.078125 cg-59.9.0/cg/cli/workflow/rnafusion/base.py
--rw-r--r--   0        0        0      554 2024-03-01 09:19:24.078125 cg-59.9.0/cg/cli/workflow/rnafusion/options.py
--rw-r--r--   0        0        0       22 2024-03-01 09:19:24.078125 cg-59.9.0/cg/cli/workflow/taxprofiler/__init__.py
--rw-r--r--   0        0        0     6512 2024-03-01 09:19:24.078125 cg-59.9.0/cg/cli/workflow/taxprofiler/base.py
--rw-r--r--   0        0        0      531 2024-03-01 09:19:24.078125 cg-59.9.0/cg/cli/workflow/taxprofiler/options.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.078125 cg-59.9.0/cg/clients/__init__.py
--rw-r--r--   0        0        0      147 2024-03-01 09:19:24.078125 cg-59.9.0/cg/clients/arnold/api.py
--rw-r--r--   0        0        0      125 2024-03-01 09:19:24.078125 cg-59.9.0/cg/clients/arnold/dto/create_case_request.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.078125 cg-59.9.0/cg/clients/janus/__init__.py
--rw-r--r--   0        0        0     1078 2024-03-01 09:19:24.078125 cg-59.9.0/cg/clients/janus/api.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.078125 cg-59.9.0/cg/clients/janus/dto/__init__.py
--rw-r--r--   0        0        0      503 2024-03-01 09:19:24.078125 cg-59.9.0/cg/clients/janus/dto/create_qc_metrics_request.py
--rw-r--r--   0        0        0      420 2024-03-01 09:19:24.078125 cg-59.9.0/cg/clients/janus/exceptions.py
--rw-r--r--   0        0        0      937 2024-03-01 09:19:24.078125 cg-59.9.0/cg/constants/__init__.py
--rw-r--r--   0        0        0      253 2024-03-01 09:19:24.078125 cg-59.9.0/cg/constants/archiving.py
--rw-r--r--   0        0        0       35 2024-03-01 09:19:24.078125 cg-59.9.0/cg/constants/backup.py
--rw-r--r--   0        0        0     1411 2024-03-01 09:19:24.078125 cg-59.9.0/cg/constants/bcl_convert_metrics.py
--rw-r--r--   0        0        0      469 2024-03-01 09:19:24.078125 cg-59.9.0/cg/constants/compression.py
--rw-r--r--   0        0        0     6285 2024-03-01 09:19:24.078125 cg-59.9.0/cg/constants/constants.py
--rw-r--r--   0        0        0     5615 2024-03-01 09:19:24.078125 cg-59.9.0/cg/constants/delivery.py
--rw-r--r--   0        0        0     9650 2024-03-01 09:19:24.078125 cg-59.9.0/cg/constants/demultiplexing.py
--rw-r--r--   0        0        0     1422 2024-03-01 09:19:24.078125 cg-59.9.0/cg/constants/encryption.py
--rw-r--r--   0        0        0      372 2024-03-01 09:19:24.078125 cg-59.9.0/cg/constants/extraction.py
--rw-r--r--   0        0        0     2047 2024-03-01 09:19:24.078125 cg-59.9.0/cg/constants/gene_panel.py
--rw-r--r--   0        0        0     6396 2024-03-01 09:19:24.078125 cg-59.9.0/cg/constants/housekeeper_tags.py
--rw-r--r--   0        0        0       95 2024-03-01 09:19:24.078125 cg-59.9.0/cg/constants/invoice.py
--rw-r--r--   0        0        0     5815 2024-03-01 09:19:24.078125 cg-59.9.0/cg/constants/lims.py
--rw-r--r--   0        0        0      231 2024-03-01 09:19:24.078125 cg-59.9.0/cg/constants/nanopore_files.py
--rw-r--r--   0        0        0      650 2024-03-01 09:19:24.078125 cg-59.9.0/cg/constants/nextflow.py
--rw-r--r--   0        0        0      862 2024-03-01 09:19:24.078125 cg-59.9.0/cg/constants/nf_analysis.py
--rw-r--r--   0        0        0       19 2024-03-01 09:19:24.078125 cg-59.9.0/cg/constants/nipt.py
--rw-r--r--   0        0        0     2257 2024-03-01 09:19:24.078125 cg-59.9.0/cg/constants/observations.py
--rw-r--r--   0        0        0     1216 2024-03-01 09:19:24.078125 cg-59.9.0/cg/constants/orderforms.py
--rw-r--r--   0        0        0       96 2024-03-01 09:19:24.078125 cg-59.9.0/cg/constants/paths.py
--rw-r--r--   0        0        0      266 2024-03-01 09:19:24.078125 cg-59.9.0/cg/constants/pdc.py
--rw-r--r--   0        0        0      160 2024-03-01 09:19:24.078125 cg-59.9.0/cg/constants/pedigree.py
--rw-r--r--   0        0        0     1044 2024-03-01 09:19:24.082125 cg-59.9.0/cg/constants/priority.py
--rw-r--r--   0        0        0       79 2024-03-01 09:19:24.082125 cg-59.9.0/cg/constants/process.py
--rw-r--r--   0        0        0     4506 2024-03-01 09:19:24.082125 cg-59.9.0/cg/constants/report.py
--rw-r--r--   0        0        0      485 2024-03-01 09:19:24.082125 cg-59.9.0/cg/constants/sample_sources.py
--rw-r--r--   0        0        0     3111 2024-03-01 09:19:24.082125 cg-59.9.0/cg/constants/scout.py
--rw-r--r--   0        0        0     1669 2024-03-01 09:19:24.082125 cg-59.9.0/cg/constants/sequencing.py
--rw-r--r--   0        0        0      313 2024-03-01 09:19:24.082125 cg-59.9.0/cg/constants/slurm.py
--rw-r--r--   0        0        0      529 2024-03-01 09:19:24.082125 cg-59.9.0/cg/constants/subject.py
--rw-r--r--   0        0        0       55 2024-03-01 09:19:24.082125 cg-59.9.0/cg/constants/symbols.py
--rw-r--r--   0        0        0      435 2024-03-01 09:19:24.082125 cg-59.9.0/cg/constants/tb.py
--rw-r--r--   0        0        0      161 2024-03-01 09:19:24.082125 cg-59.9.0/cg/constants/time.py
--rw-r--r--   0        0        0     6014 2024-03-01 09:19:24.082125 cg-59.9.0/cg/exc.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.082125 cg-59.9.0/cg/io/__init__.py
--rw-r--r--   0        0        0     1037 2024-03-01 09:19:24.082125 cg-59.9.0/cg/io/api.py
--rw-r--r--   0        0        0     2913 2024-03-01 09:19:24.082125 cg-59.9.0/cg/io/controller.py
--rw-r--r--   0        0        0     1763 2024-03-01 09:19:24.082125 cg-59.9.0/cg/io/csv.py
--rw-r--r--   0        0        0      210 2024-03-01 09:19:24.082125 cg-59.9.0/cg/io/gzip.py
--rw-r--r--   0        0        0      616 2024-03-01 09:19:24.082125 cg-59.9.0/cg/io/json.py
--rw-r--r--   0        0        0      601 2024-03-01 09:19:24.082125 cg-59.9.0/cg/io/txt.py
--rw-r--r--   0        0        0      552 2024-03-01 09:19:24.082125 cg-59.9.0/cg/io/validate_path.py
--rw-r--r--   0        0        0     1289 2024-03-01 09:19:24.082125 cg-59.9.0/cg/io/xml.py
--rw-r--r--   0        0        0     1153 2024-03-01 09:19:24.082125 cg-59.9.0/cg/io/yaml.py
--rw-r--r--   0        0        0      281 2024-03-01 09:19:24.082125 cg-59.9.0/cg/meta/__init__.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.082125 cg-59.9.0/cg/meta/archive/__init__.py
--rw-r--r--   0        0        0    15193 2024-03-01 09:19:24.082125 cg-59.9.0/cg/meta/archive/archive.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.082125 cg-59.9.0/cg/meta/archive/ddn/__init__.py
--rw-r--r--   0        0        0     1727 2024-03-01 09:19:24.082125 cg-59.9.0/cg/meta/archive/ddn/constants.py
--rw-r--r--   0        0        0    10853 2024-03-01 09:19:24.082125 cg-59.9.0/cg/meta/archive/ddn/ddn_data_flow_client.py
--rw-r--r--   0        0        0     3704 2024-03-01 09:19:24.082125 cg-59.9.0/cg/meta/archive/ddn/models.py
--rw-r--r--   0        0        0     1250 2024-03-01 09:19:24.082125 cg-59.9.0/cg/meta/archive/ddn/utils.py
--rw-r--r--   0        0        0     2024 2024-03-01 09:19:24.082125 cg-59.9.0/cg/meta/archive/models.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.082125 cg-59.9.0/cg/meta/backup/__init__.py
--rw-r--r--   0        0        0    17530 2024-03-01 09:19:24.082125 cg-59.9.0/cg/meta/backup/backup.py
--rw-r--r--   0        0        0     5397 2024-03-01 09:19:24.082125 cg-59.9.0/cg/meta/backup/pdc.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.082125 cg-59.9.0/cg/meta/clean/__init__.py
--rw-r--r--   0        0        0     3901 2024-03-01 09:19:24.082125 cg-59.9.0/cg/meta/clean/api.py
--rw-r--r--   0        0        0     7744 2024-03-01 09:19:24.082125 cg-59.9.0/cg/meta/clean/clean_flow_cells.py
--rw-r--r--   0        0        0     1841 2024-03-01 09:19:24.082125 cg-59.9.0/cg/meta/clean/clean_retrieved_spring_files.py
--rw-r--r--   0        0        0       34 2024-03-01 09:19:24.082125 cg-59.9.0/cg/meta/compress/__init__.py
--rw-r--r--   0        0        0    14557 2024-03-01 09:19:24.082125 cg-59.9.0/cg/meta/compress/compress.py
--rw-r--r--   0        0        0     4947 2024-03-01 09:19:24.082125 cg-59.9.0/cg/meta/compress/files.py
--rw-r--r--   0        0        0    14247 2024-03-01 09:19:24.082125 cg-59.9.0/cg/meta/deliver.py
--rw-r--r--   0        0        0     7886 2024-03-01 09:19:24.082125 cg-59.9.0/cg/meta/deliver_ticket.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.082125 cg-59.9.0/cg/meta/demultiplex/__init__.py
--rw-r--r--   0        0        0     2592 2024-03-01 09:19:24.082125 cg-59.9.0/cg/meta/demultiplex/combine_sequencing_metrics.py
--rw-r--r--   0        0        0     5915 2024-03-01 09:19:24.082125 cg-59.9.0/cg/meta/demultiplex/demux_post_processing.py
--rw-r--r--   0        0        0     4135 2024-03-01 09:19:24.082125 cg-59.9.0/cg/meta/demultiplex/files.py
--rw-r--r--   0        0        0     7777 2024-03-01 09:19:24.082125 cg-59.9.0/cg/meta/demultiplex/housekeeper_storage_functions.py
--rw-r--r--   0        0        0     6941 2024-03-01 09:19:24.082125 cg-59.9.0/cg/meta/demultiplex/status_db_storage_functions.py
--rw-r--r--   0        0        0    11951 2024-03-01 09:19:24.082125 cg-59.9.0/cg/meta/demultiplex/utils.py
--rw-r--r--   0        0        0     2855 2024-03-01 09:19:24.082125 cg-59.9.0/cg/meta/demultiplex/validation.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.082125 cg-59.9.0/cg/meta/encryption/__init__.py
--rw-r--r--   0        0        0    19578 2024-03-01 09:19:24.086125 cg-59.9.0/cg/meta/encryption/encryption.py
--rw-r--r--   0        0        0      464 2024-03-01 09:19:24.086125 cg-59.9.0/cg/meta/encryption/sbatch.py
--rw-r--r--   0        0        0    10922 2024-03-01 09:19:24.086125 cg-59.9.0/cg/meta/invoice.py
--rw-r--r--   0        0        0     2249 2024-03-01 09:19:24.086125 cg-59.9.0/cg/meta/meta.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.086125 cg-59.9.0/cg/meta/observations/__init__.py
--rw-r--r--   0        0        0     6008 2024-03-01 09:19:24.086125 cg-59.9.0/cg/meta/observations/balsamic_observations_api.py
--rw-r--r--   0        0        0     5277 2024-03-01 09:19:24.086125 cg-59.9.0/cg/meta/observations/mip_dna_observations_api.py
--rw-r--r--   0        0        0     5364 2024-03-01 09:19:24.086125 cg-59.9.0/cg/meta/observations/observations_api.py
--rw-r--r--   0        0        0       27 2024-03-01 09:19:24.086125 cg-59.9.0/cg/meta/orders/__init__.py
--rw-r--r--   0        0        0     3637 2024-03-01 09:19:24.086125 cg-59.9.0/cg/meta/orders/api.py
--rw-r--r--   0        0        0      121 2024-03-01 09:19:24.086125 cg-59.9.0/cg/meta/orders/balsamic_qc_submitter.py
--rw-r--r--   0        0        0      107 2024-03-01 09:19:24.086125 cg-59.9.0/cg/meta/orders/balsamic_submitter.py
--rw-r--r--   0        0        0      122 2024-03-01 09:19:24.086125 cg-59.9.0/cg/meta/orders/balsamic_umi_submitter.py
--rw-r--r--   0        0        0    15262 2024-03-01 09:19:24.086125 cg-59.9.0/cg/meta/orders/case_submitter.py
--rw-r--r--   0        0        0     6102 2024-03-01 09:19:24.086125 cg-59.9.0/cg/meta/orders/fastq_submitter.py
--rw-r--r--   0        0        0      105 2024-03-01 09:19:24.086125 cg-59.9.0/cg/meta/orders/fluffy_submitter.py
--rw-r--r--   0        0        0     1254 2024-03-01 09:19:24.086125 cg-59.9.0/cg/meta/orders/lims.py
--rw-r--r--   0        0        0     5782 2024-03-01 09:19:24.086125 cg-59.9.0/cg/meta/orders/metagenome_submitter.py
--rw-r--r--   0        0        0     6337 2024-03-01 09:19:24.086125 cg-59.9.0/cg/meta/orders/microbial_submitter.py
--rw-r--r--   0        0        0      123 2024-03-01 09:19:24.086125 cg-59.9.0/cg/meta/orders/microsalt_submitter.py
--rw-r--r--   0        0        0      105 2024-03-01 09:19:24.086125 cg-59.9.0/cg/meta/orders/mip_dna_submitter.py
--rw-r--r--   0        0        0      105 2024-03-01 09:19:24.086125 cg-59.9.0/cg/meta/orders/mip_rna_submitter.py
--rw-r--r--   0        0        0     7761 2024-03-01 09:19:24.086125 cg-59.9.0/cg/meta/orders/pool_submitter.py
--rw-r--r--   0        0        0      102 2024-03-01 09:19:24.086125 cg-59.9.0/cg/meta/orders/rml_submitter.py
--rw-r--r--   0        0        0      718 2024-03-01 09:19:24.086125 cg-59.9.0/cg/meta/orders/rnafusion_submitter.py
--rw-r--r--   0        0        0     1268 2024-03-01 09:19:24.086125 cg-59.9.0/cg/meta/orders/sars_cov_2_submitter.py
--rw-r--r--   0        0        0     1754 2024-03-01 09:19:24.086125 cg-59.9.0/cg/meta/orders/submitter.py
--rw-r--r--   0        0        0     7880 2024-03-01 09:19:24.086125 cg-59.9.0/cg/meta/orders/ticket_handler.py
--rw-r--r--   0        0        0     3608 2024-03-01 09:19:24.086125 cg-59.9.0/cg/meta/qc_metrics/collect_qc_metrics.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.086125 cg-59.9.0/cg/meta/report/__init__.py
--rw-r--r--   0        0        0    10372 2024-03-01 09:19:24.086125 cg-59.9.0/cg/meta/report/balsamic.py
--rw-r--r--   0        0        0      562 2024-03-01 09:19:24.086125 cg-59.9.0/cg/meta/report/balsamic_qc.py
--rw-r--r--   0        0        0      717 2024-03-01 09:19:24.086125 cg-59.9.0/cg/meta/report/balsamic_umi.py
--rw-r--r--   0        0        0     4171 2024-03-01 09:19:24.086125 cg-59.9.0/cg/meta/report/field_validators.py
--rw-r--r--   0        0        0     7160 2024-03-01 09:19:24.086125 cg-59.9.0/cg/meta/report/mip_dna.py
--rw-r--r--   0        0        0    19056 2024-03-01 09:19:24.086125 cg-59.9.0/cg/meta/report/report_api.py
--rw-r--r--   0        0        0     5403 2024-03-01 09:19:24.086125 cg-59.9.0/cg/meta/report/rnafusion.py
--rw-r--r--   0        0        0    80176 2024-03-01 09:19:24.086125 cg-59.9.0/cg/meta/report/templates/balsamic_report.html
--rw-r--r--   0        0        0   151463 2024-03-01 09:19:24.086125 cg-59.9.0/cg/meta/report/templates/bootstrap.html
--rw-r--r--   0        0        0    78094 2024-03-01 09:19:24.086125 cg-59.9.0/cg/meta/report/templates/mip-dna_report.html
--rw-r--r--   0        0        0    79169 2024-03-01 09:19:24.086125 cg-59.9.0/cg/meta/report/templates/rnafusion_report.html
--rw-r--r--   0        0        0       32 2024-03-01 09:19:24.086125 cg-59.9.0/cg/meta/rsync/__init__.py
--rw-r--r--   0        0        0    12141 2024-03-01 09:19:24.086125 cg-59.9.0/cg/meta/rsync/rsync_api.py
--rw-r--r--   0        0        0      387 2024-03-01 09:19:24.086125 cg-59.9.0/cg/meta/rsync/sbatch.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.086125 cg-59.9.0/cg/meta/tar/__init__.py
--rw-r--r--   0        0        0     1694 2024-03-01 09:19:24.086125 cg-59.9.0/cg/meta/tar/tar.py
--rw-r--r--   0        0        0       71 2024-03-01 09:19:24.086125 cg-59.9.0/cg/meta/transfer/__init__.py
--rw-r--r--   0        0        0    10013 2024-03-01 09:19:24.086125 cg-59.9.0/cg/meta/transfer/external_data.py
--rw-r--r--   0        0        0     5814 2024-03-01 09:19:24.086125 cg-59.9.0/cg/meta/transfer/lims.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.086125 cg-59.9.0/cg/meta/upload/__init__.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.086125 cg-59.9.0/cg/meta/upload/balsamic/__init__.py
--rw-r--r--   0        0        0     3107 2024-03-01 09:19:24.090125 cg-59.9.0/cg/meta/upload/balsamic/balsamic.py
--rw-r--r--   0        0        0     2224 2024-03-01 09:19:24.090125 cg-59.9.0/cg/meta/upload/coverage.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.090125 cg-59.9.0/cg/meta/upload/fohm/__init__.py
--rw-r--r--   0        0        0    12102 2024-03-01 09:19:24.090125 cg-59.9.0/cg/meta/upload/fohm/fohm.py
--rw-r--r--   0        0        0       30 2024-03-01 09:19:24.090125 cg-59.9.0/cg/meta/upload/gisaid/__init__.py
--rw-r--r--   0        0        0      928 2024-03-01 09:19:24.090125 cg-59.9.0/cg/meta/upload/gisaid/constants.py
--rw-r--r--   0        0        0    13521 2024-03-01 09:19:24.090125 cg-59.9.0/cg/meta/upload/gisaid/gisaid.py
--rw-r--r--   0        0        0     3312 2024-03-01 09:19:24.090125 cg-59.9.0/cg/meta/upload/gisaid/models.py
--rw-r--r--   0        0        0     5310 2024-03-01 09:19:24.090125 cg-59.9.0/cg/meta/upload/gt.py
--rw-r--r--   0        0        0      898 2024-03-01 09:19:24.090125 cg-59.9.0/cg/meta/upload/microsalt/microsalt_upload_api.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.090125 cg-59.9.0/cg/meta/upload/mip/__init__.py
--rw-r--r--   0        0        0     2546 2024-03-01 09:19:24.090125 cg-59.9.0/cg/meta/upload/mip/mip_dna.py
--rw-r--r--   0        0        0     1400 2024-03-01 09:19:24.090125 cg-59.9.0/cg/meta/upload/mip/mip_rna.py
--rw-r--r--   0        0        0     7294 2024-03-01 09:19:24.090125 cg-59.9.0/cg/meta/upload/mutacc.py
--rw-r--r--   0        0        0       32 2024-03-01 09:19:24.090125 cg-59.9.0/cg/meta/upload/nipt/__init__.py
--rw-r--r--   0        0        0      696 2024-03-01 09:19:24.090125 cg-59.9.0/cg/meta/upload/nipt/models.py
--rw-r--r--   0        0        0     8106 2024-03-01 09:19:24.090125 cg-59.9.0/cg/meta/upload/nipt/nipt.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.090125 cg-59.9.0/cg/meta/upload/rnafusion/__init__.py
--rw-r--r--   0        0        0     1698 2024-03-01 09:19:24.090125 cg-59.9.0/cg/meta/upload/rnafusion/rnafusion.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.090125 cg-59.9.0/cg/meta/upload/scout/__init__.py
--rw-r--r--   0        0        0     4009 2024-03-01 09:19:24.090125 cg-59.9.0/cg/meta/upload/scout/balsamic_config_builder.py
--rw-r--r--   0        0        0     1491 2024-03-01 09:19:24.090125 cg-59.9.0/cg/meta/upload/scout/balsamic_umi_config_builder.py
--rw-r--r--   0        0        0     3322 2024-03-01 09:19:24.090125 cg-59.9.0/cg/meta/upload/scout/hk_tags.py
--rw-r--r--   0        0        0     9103 2024-03-01 09:19:24.090125 cg-59.9.0/cg/meta/upload/scout/mip_config_builder.py
--rw-r--r--   0        0        0     3495 2024-03-01 09:19:24.090125 cg-59.9.0/cg/meta/upload/scout/rnafusion_config_builder.py
--rw-r--r--   0        0        0     7516 2024-03-01 09:19:24.090125 cg-59.9.0/cg/meta/upload/scout/scout_config_builder.py
--rw-r--r--   0        0        0    23146 2024-03-01 09:19:24.090125 cg-59.9.0/cg/meta/upload/scout/uploadscoutapi.py
--rw-r--r--   0        0        0     3197 2024-03-01 09:19:24.090125 cg-59.9.0/cg/meta/upload/upload_api.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.090125 cg-59.9.0/cg/meta/workflow/__init__.py
--rw-r--r--   0        0        0    26334 2024-03-01 09:19:24.090125 cg-59.9.0/cg/meta/workflow/analysis.py
--rw-r--r--   0        0        0    26074 2024-03-01 09:19:24.090125 cg-59.9.0/cg/meta/workflow/balsamic.py
--rw-r--r--   0        0        0     2700 2024-03-01 09:19:24.090125 cg-59.9.0/cg/meta/workflow/balsamic_pon.py
--rw-r--r--   0        0        0      553 2024-03-01 09:19:24.090125 cg-59.9.0/cg/meta/workflow/balsamic_qc.py
--rw-r--r--   0        0        0      556 2024-03-01 09:19:24.090125 cg-59.9.0/cg/meta/workflow/balsamic_umi.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.090125 cg-59.9.0/cg/meta/workflow/downsample/__init__.py
--rw-r--r--   0        0        0     3922 2024-03-01 09:19:24.090125 cg-59.9.0/cg/meta/workflow/downsample/downsample.py
--rw-r--r--   0        0        0      711 2024-03-01 09:19:24.090125 cg-59.9.0/cg/meta/workflow/downsample/sbatch.py
--rw-r--r--   0        0        0     8913 2024-03-01 09:19:24.090125 cg-59.9.0/cg/meta/workflow/fastq.py
--rw-r--r--   0        0        0    10687 2024-03-01 09:19:24.090125 cg-59.9.0/cg/meta/workflow/fluffy.py
--rw-r--r--   0        0        0       70 2024-03-01 09:19:24.090125 cg-59.9.0/cg/meta/workflow/microsalt/__init__.py
--rw-r--r--   0        0        0      116 2024-03-01 09:19:24.090125 cg-59.9.0/cg/meta/workflow/microsalt/constants.py
--rw-r--r--   0        0        0      174 2024-03-01 09:19:24.090125 cg-59.9.0/cg/meta/workflow/microsalt/metrics_parser/__init__.py
--rw-r--r--   0        0        0      366 2024-03-01 09:19:24.090125 cg-59.9.0/cg/meta/workflow/microsalt/metrics_parser/metrics_parser.py
--rw-r--r--   0        0        0      903 2024-03-01 09:19:24.090125 cg-59.9.0/cg/meta/workflow/microsalt/metrics_parser/models.py
--rw-r--r--   0        0        0    13171 2024-03-01 09:19:24.090125 cg-59.9.0/cg/meta/workflow/microsalt/microsalt.py
--rw-r--r--   0        0        0       95 2024-03-01 09:19:24.090125 cg-59.9.0/cg/meta/workflow/microsalt/quality_controller/__init__.py
--rw-r--r--   0        0        0      712 2024-03-01 09:19:24.090125 cg-59.9.0/cg/meta/workflow/microsalt/quality_controller/models.py
--rw-r--r--   0        0        0     5688 2024-03-01 09:19:24.090125 cg-59.9.0/cg/meta/workflow/microsalt/quality_controller/quality_controller.py
--rw-r--r--   0        0        0     1217 2024-03-01 09:19:24.090125 cg-59.9.0/cg/meta/workflow/microsalt/quality_controller/report_generator.py
--rw-r--r--   0        0        0     2373 2024-03-01 09:19:24.090125 cg-59.9.0/cg/meta/workflow/microsalt/quality_controller/result_logger.py
--rw-r--r--   0        0        0     5641 2024-03-01 09:19:24.090125 cg-59.9.0/cg/meta/workflow/microsalt/quality_controller/utils.py
--rw-r--r--   0        0        0     1220 2024-03-01 09:19:24.090125 cg-59.9.0/cg/meta/workflow/microsalt/utils.py
--rw-r--r--   0        0        0    13833 2024-03-01 09:19:24.090125 cg-59.9.0/cg/meta/workflow/mip.py
--rw-r--r--   0        0        0     2686 2024-03-01 09:19:24.090125 cg-59.9.0/cg/meta/workflow/mip_dna.py
--rw-r--r--   0        0        0     2167 2024-03-01 09:19:24.090125 cg-59.9.0/cg/meta/workflow/mip_rna.py
--rw-r--r--   0        0        0    10587 2024-03-01 09:19:24.090125 cg-59.9.0/cg/meta/workflow/mutant.py
--rw-r--r--   0        0        0    19362 2024-03-01 09:19:24.090125 cg-59.9.0/cg/meta/workflow/nf_analysis.py
--rw-r--r--   0        0        0     6161 2024-03-01 09:19:24.090125 cg-59.9.0/cg/meta/workflow/nf_handlers.py
--rw-r--r--   0        0        0     6394 2024-03-01 09:19:24.090125 cg-59.9.0/cg/meta/workflow/prepare_fastq.py
--rw-r--r--   0        0        0     2318 2024-03-01 09:19:24.090125 cg-59.9.0/cg/meta/workflow/raredisease.py
--rw-r--r--   0        0        0     8987 2024-03-01 09:19:24.090125 cg-59.9.0/cg/meta/workflow/rnafusion.py
--rw-r--r--   0        0        0     7652 2024-03-01 09:19:24.090125 cg-59.9.0/cg/meta/workflow/taxprofiler.py
--rw-r--r--   0        0        0      113 2024-03-01 09:19:24.090125 cg-59.9.0/cg/models/__init__.py
--rw-r--r--   0        0        0      102 2024-03-01 09:19:24.090125 cg-59.9.0/cg/models/analysis.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.090125 cg-59.9.0/cg/models/balsamic/__init__.py
--rw-r--r--   0        0        0      459 2024-03-01 09:19:24.090125 cg-59.9.0/cg/models/balsamic/analysis.py
--rw-r--r--   0        0        0     4550 2024-03-01 09:19:24.090125 cg-59.9.0/cg/models/balsamic/config.py
--rw-r--r--   0        0        0     1954 2024-03-01 09:19:24.090125 cg-59.9.0/cg/models/balsamic/metrics.py
--rw-r--r--   0        0        0    16013 2024-03-01 09:19:24.090125 cg-59.9.0/cg/models/cg_config.py
--rw-r--r--   0        0        0     4302 2024-03-01 09:19:24.090125 cg-59.9.0/cg/models/compression_data.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.090125 cg-59.9.0/cg/models/deliverables/__init__.py
--rw-r--r--   0        0        0     5170 2024-03-01 09:19:24.090125 cg-59.9.0/cg/models/deliverables/metric_deliverables.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.094125 cg-59.9.0/cg/models/demultiplex/__init__.py
--rw-r--r--   0        0        0    12040 2024-03-01 09:19:24.094125 cg-59.9.0/cg/models/demultiplex/run_parameters.py
--rw-r--r--   0        0        0      539 2024-03-01 09:19:24.094125 cg-59.9.0/cg/models/demultiplex/sbatch.py
--rw-r--r--   0        0        0     6823 2024-03-01 09:19:24.094125 cg-59.9.0/cg/models/downsample/downsample_data.py
--rw-r--r--   0        0        0      255 2024-03-01 09:19:24.094125 cg-59.9.0/cg/models/email.py
--rw-r--r--   0        0        0     1046 2024-03-01 09:19:24.094125 cg-59.9.0/cg/models/fastq.py
--rw-r--r--   0        0        0     2157 2024-03-01 09:19:24.094125 cg-59.9.0/cg/models/file_data.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.094125 cg-59.9.0/cg/models/flow_cell/__init__.py
--rw-r--r--   0        0        0    10976 2024-03-01 09:19:24.094125 cg-59.9.0/cg/models/flow_cell/flow_cell.py
--rw-r--r--   0        0        0      317 2024-03-01 09:19:24.094125 cg-59.9.0/cg/models/flow_cell/utils.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.094125 cg-59.9.0/cg/models/invoice/__init__.py
--rw-r--r--   0        0        0     1254 2024-03-01 09:19:24.094125 cg-59.9.0/cg/models/invoice/invoice.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.094125 cg-59.9.0/cg/models/lims/__init__.py
--rw-r--r--   0        0        0     2019 2024-03-01 09:19:24.094125 cg-59.9.0/cg/models/lims/sample.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.094125 cg-59.9.0/cg/models/mip/__init__.py
--rw-r--r--   0        0        0      337 2024-03-01 09:19:24.094125 cg-59.9.0/cg/models/mip/mip_analysis.py
--rw-r--r--   0        0        0     1564 2024-03-01 09:19:24.094125 cg-59.9.0/cg/models/mip/mip_config.py
--rw-r--r--   0        0        0     4696 2024-03-01 09:19:24.094125 cg-59.9.0/cg/models/mip/mip_metrics_deliverables.py
--rw-r--r--   0        0        0     2550 2024-03-01 09:19:24.094125 cg-59.9.0/cg/models/mip/mip_sample_info.py
--rw-r--r--   0        0        0     2076 2024-03-01 09:19:24.094125 cg-59.9.0/cg/models/nf_analysis.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.094125 cg-59.9.0/cg/models/observations/__init__.py
--rw-r--r--   0        0        0      688 2024-03-01 09:19:24.094125 cg-59.9.0/cg/models/observations/input_files.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.094125 cg-59.9.0/cg/models/orders/__init__.py
--rw-r--r--   0        0        0     2659 2024-03-01 09:19:24.094125 cg-59.9.0/cg/models/orders/constants.py
--rw-r--r--   0        0        0     5604 2024-03-01 09:19:24.094125 cg-59.9.0/cg/models/orders/excel_sample.py
--rw-r--r--   0        0        0      898 2024-03-01 09:19:24.094125 cg-59.9.0/cg/models/orders/json_sample.py
--rw-r--r--   0        0        0     1449 2024-03-01 09:19:24.094125 cg-59.9.0/cg/models/orders/order.py
--rw-r--r--   0        0        0      811 2024-03-01 09:19:24.094125 cg-59.9.0/cg/models/orders/orderform_schema.py
--rw-r--r--   0        0        0     4212 2024-03-01 09:19:24.094125 cg-59.9.0/cg/models/orders/sample_base.py
--rw-r--r--   0        0        0     9549 2024-03-01 09:19:24.094125 cg-59.9.0/cg/models/orders/samples.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.094125 cg-59.9.0/cg/models/orders/validators/__init__.py
--rw-r--r--   0        0        0     2300 2024-03-01 09:19:24.094125 cg-59.9.0/cg/models/orders/validators/excel_sample_validators.py
--rw-r--r--   0        0        0      576 2024-03-01 09:19:24.094125 cg-59.9.0/cg/models/orders/validators/json_sample_validators.py
--rw-r--r--   0        0        0       71 2024-03-01 09:19:24.094125 cg-59.9.0/cg/models/orders/validators/sample_base_validators.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.094125 cg-59.9.0/cg/models/raredisease/__init__.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.094125 cg-59.9.0/cg/models/report/__init__.py
--rw-r--r--   0        0        0     6785 2024-03-01 09:19:24.094125 cg-59.9.0/cg/models/report/metadata.py
--rw-r--r--   0        0        0     5951 2024-03-01 09:19:24.094125 cg-59.9.0/cg/models/report/report.py
--rw-r--r--   0        0        0     4724 2024-03-01 09:19:24.094125 cg-59.9.0/cg/models/report/sample.py
--rw-r--r--   0        0        0     2669 2024-03-01 09:19:24.094125 cg-59.9.0/cg/models/report/validators.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.094125 cg-59.9.0/cg/models/rnafusion/__init__.py
--rw-r--r--   0        0        0     2633 2024-03-01 09:19:24.094125 cg-59.9.0/cg/models/rnafusion/rnafusion.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.094125 cg-59.9.0/cg/models/scout/__init__.py
--rw-r--r--   0        0        0     4783 2024-03-01 09:19:24.094125 cg-59.9.0/cg/models/scout/scout_load_config.py
--rw-r--r--   0        0        0      116 2024-03-01 09:19:24.094125 cg-59.9.0/cg/models/scout/validators.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.094125 cg-59.9.0/cg/models/slurm/__init__.py
--rw-r--r--   0        0        0      617 2024-03-01 09:19:24.094125 cg-59.9.0/cg/models/slurm/sbatch.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.094125 cg-59.9.0/cg/models/taxprofiler/__init__.py
--rw-r--r--   0        0        0     2433 2024-03-01 09:19:24.094125 cg-59.9.0/cg/models/taxprofiler/taxprofiler.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.094125 cg-59.9.0/cg/models/workflow/__init__.py
--rw-r--r--   0        0        0      685 2024-03-01 09:19:24.094125 cg-59.9.0/cg/models/workflow/mutant.py
--rw-r--r--   0        0        0       70 2024-03-01 09:19:24.094125 cg-59.9.0/cg/models/workflow/validators.py
--rw-r--r--   0        0        0    25590 2024-03-01 09:19:24.094125 cg-59.9.0/cg/resources/20181012_Indices.csv
--rw-r--r--   0        0        0      661 2024-03-01 09:19:24.094125 cg-59.9.0/cg/resources/__init__.py
--rw-r--r--   0        0        0     2590 2024-03-01 09:19:24.094125 cg-59.9.0/cg/resources/rnafusion_bundle_filenames.csv
--rw-r--r--   0        0        0     2583 2024-03-01 09:19:24.094125 cg-59.9.0/cg/resources/taxprofiler_bundle_filenames.csv
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.094125 cg-59.9.0/cg/server/__init__.py
--rw-r--r--   0        0        0    20077 2024-03-01 09:19:24.094125 cg-59.9.0/cg/server/admin.py
--rw-r--r--   0        0        0    19972 2024-03-01 09:19:24.094125 cg-59.9.0/cg/server/api.py
--rw-r--r--   0        0        0     4813 2024-03-01 09:19:24.094125 cg-59.9.0/cg/server/app.py
--rw-r--r--   0        0        0       48 2024-03-01 09:19:24.094125 cg-59.9.0/cg/server/auto.py
--rw-r--r--   0        0        0     1184 2024-03-01 09:19:24.094125 cg-59.9.0/cg/server/config.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.094125 cg-59.9.0/cg/server/dto/__init__.py
--rw-r--r--   0        0        0       92 2024-03-01 09:19:24.094125 cg-59.9.0/cg/server/dto/delivery_message_response.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.094125 cg-59.9.0/cg/server/dto/orders/__init__.py
--rw-r--r--   0        0        0      671 2024-03-01 09:19:24.094125 cg-59.9.0/cg/server/dto/orders/orders_request.py
--rw-r--r--   0        0        0      397 2024-03-01 09:19:24.094125 cg-59.9.0/cg/server/dto/orders/orders_response.py
--rw-r--r--   0        0        0     2404 2024-03-01 09:19:24.094125 cg-59.9.0/cg/server/ext.py
--rw-r--r--   0        0        0       29 2024-03-01 09:19:24.094125 cg-59.9.0/cg/server/invoices/__init__.py
--rw-r--r--   0        0        0     4793 2024-03-01 09:19:24.094125 cg-59.9.0/cg/server/invoices/templates/invoices/index.html
--rw-r--r--   0        0        0     8171 2024-03-01 09:19:24.094125 cg-59.9.0/cg/server/invoices/templates/invoices/invoice.html
--rw-r--r--   0        0        0     2838 2024-03-01 09:19:24.094125 cg-59.9.0/cg/server/invoices/templates/invoices/layout.html
--rw-r--r--   0        0        0     4956 2024-03-01 09:19:24.094125 cg-59.9.0/cg/server/invoices/templates/invoices/new.html
--rw-r--r--   0        0        0     7715 2024-03-01 09:19:24.094125 cg-59.9.0/cg/server/invoices/views.py
--rw-r--r--   0        0        0      354 2024-03-01 09:19:24.094125 cg-59.9.0/cg/server/templates/admin/index.html
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.094125 cg-59.9.0/cg/services/__init__.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.094125 cg-59.9.0/cg/services/delivery_message/__init__.py
--rw-r--r--   0        0        0      607 2024-03-01 09:19:24.094125 cg-59.9.0/cg/services/delivery_message/delivery_message_service.py
--rw-r--r--   0        0        0      792 2024-03-01 09:19:24.098125 cg-59.9.0/cg/services/delivery_message/messages/__init__.py
--rw-r--r--   0        0        0      706 2024-03-01 09:19:24.098125 cg-59.9.0/cg/services/delivery_message/messages/analysis_scout_message.py
--rw-r--r--   0        0        0      777 2024-03-01 09:19:24.098125 cg-59.9.0/cg/services/delivery_message/messages/covid_message.py
--rw-r--r--   0        0        0      182 2024-03-01 09:19:24.098125 cg-59.9.0/cg/services/delivery_message/messages/delivery_message.py
--rw-r--r--   0        0        0      721 2024-03-01 09:19:24.098125 cg-59.9.0/cg/services/delivery_message/messages/fastq_analysis_scout_message.py
--rw-r--r--   0        0        0      525 2024-03-01 09:19:24.098125 cg-59.9.0/cg/services/delivery_message/messages/fastq_message.py
--rw-r--r--   0        0        0      701 2024-03-01 09:19:24.098125 cg-59.9.0/cg/services/delivery_message/messages/fastq_scout_message.py
--rw-r--r--   0        0        0      594 2024-03-01 09:19:24.098125 cg-59.9.0/cg/services/delivery_message/messages/microsalt_mwr_message.py
--rw-r--r--   0        0        0      582 2024-03-01 09:19:24.098125 cg-59.9.0/cg/services/delivery_message/messages/microsalt_mwx_message.py
--rw-r--r--   0        0        0      415 2024-03-01 09:19:24.098125 cg-59.9.0/cg/services/delivery_message/messages/scout_message.py
--rw-r--r--   0        0        0      408 2024-03-01 09:19:24.098125 cg-59.9.0/cg/services/delivery_message/messages/statina_message.py
--rw-r--r--   0        0        0      737 2024-03-01 09:19:24.098125 cg-59.9.0/cg/services/delivery_message/messages/utils.py
--rw-r--r--   0        0        0     2346 2024-03-01 09:19:24.098125 cg-59.9.0/cg/services/delivery_message/utils.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.098125 cg-59.9.0/cg/services/fastq_file_service/__init__.py
--rw-r--r--   0        0        0      101 2024-03-01 09:19:24.098125 cg-59.9.0/cg/services/fastq_file_service/exceptions.py
--rw-r--r--   0        0        0      868 2024-03-01 09:19:24.098125 cg-59.9.0/cg/services/fastq_file_service/fastq_file_service.py
--rw-r--r--   0        0        0     2780 2024-03-01 09:19:24.098125 cg-59.9.0/cg/services/fastq_file_service/utils.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.098125 cg-59.9.0/cg/services/orders/__init__.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.098125 cg-59.9.0/cg/services/orders/order_service/__init__.py
--rw-r--r--   0        0        0      101 2024-03-01 09:19:24.098125 cg-59.9.0/cg/services/orders/order_service/exceptions.py
--rw-r--r--   0        0        0     2116 2024-03-01 09:19:24.098125 cg-59.9.0/cg/services/orders/order_service/order_service.py
--rw-r--r--   0        0        0     1053 2024-03-01 09:19:24.098125 cg-59.9.0/cg/services/orders/order_service/utils.py
--rw-r--r--   0        0        0       92 2024-03-01 09:19:24.098125 cg-59.9.0/cg/services/orders/order_status_service/__init__.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.098125 cg-59.9.0/cg/services/orders/order_status_service/dto/__init__.py
--rw-r--r--   0        0        0      275 2024-03-01 09:19:24.098125 cg-59.9.0/cg/services/orders/order_status_service/dto/order_status_summary.py
--rw-r--r--   0        0        0      981 2024-03-01 09:19:24.098125 cg-59.9.0/cg/services/orders/order_status_service/order_status_service.py
--rw-r--r--   0        0        0     2316 2024-03-01 09:19:24.098125 cg-59.9.0/cg/services/orders/order_status_service/utils.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.098125 cg-59.9.0/cg/services/slurm_service/__init__.py
--rw-r--r--   0        0        0      703 2024-03-01 09:19:24.098125 cg-59.9.0/cg/services/slurm_service/slurm_cli_service.py
--rw-r--r--   0        0        0      242 2024-03-01 09:19:24.098125 cg-59.9.0/cg/services/slurm_service/slurm_service.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.098125 cg-59.9.0/cg/services/slurm_upload_service/__init__.py
--rw-r--r--   0        0        0      175 2024-03-01 09:19:24.098125 cg-59.9.0/cg/services/slurm_upload_service/slurm_upload_config.py
--rw-r--r--   0        0        0     2074 2024-03-01 09:19:24.098125 cg-59.9.0/cg/services/slurm_upload_service/slurm_upload_service.py
--rw-r--r--   0        0        0      203 2024-03-01 09:19:24.098125 cg-59.9.0/cg/services/slurm_upload_service/utils.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.098125 cg-59.9.0/cg/store/__init__.py
--rw-r--r--   0        0        0     7245 2024-03-01 09:19:24.098125 cg-59.9.0/cg/store/base.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.098125 cg-59.9.0/cg/store/crud/__init__.py
--rw-r--r--   0        0        0    12932 2024-03-01 09:19:24.098125 cg-59.9.0/cg/store/crud/create.py
--rw-r--r--   0        0        0     2144 2024-03-01 09:19:24.098125 cg-59.9.0/cg/store/crud/delete.py
--rw-r--r--   0        0        0    77317 2024-03-01 09:19:24.098125 cg-59.9.0/cg/store/crud/read.py
--rw-r--r--   0        0        0      837 2024-03-01 09:19:24.098125 cg-59.9.0/cg/store/crud/update.py
--rw-r--r--   0        0        0     1662 2024-03-01 09:19:24.098125 cg-59.9.0/cg/store/database.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.098125 cg-59.9.0/cg/store/filters/__init__.py
--rw-r--r--   0        0        0     5371 2024-03-01 09:19:24.098125 cg-59.9.0/cg/store/filters/status_analysis_filters.py
--rw-r--r--   0        0        0     1712 2024-03-01 09:19:24.098125 cg-59.9.0/cg/store/filters/status_application_filters.py
--rw-r--r--   0        0        0     1440 2024-03-01 09:19:24.098125 cg-59.9.0/cg/store/filters/status_application_limitations_filters.py
--rw-r--r--   0        0        0     2523 2024-03-01 09:19:24.098125 cg-59.9.0/cg/store/filters/status_application_version_filters.py
--rw-r--r--   0        0        0     1390 2024-03-01 09:19:24.098125 cg-59.9.0/cg/store/filters/status_bed_filters.py
--rw-r--r--   0        0        0     1317 2024-03-01 09:19:24.098125 cg-59.9.0/cg/store/filters/status_bed_version_filters.py
--rw-r--r--   0        0        0    10384 2024-03-01 09:19:24.098125 cg-59.9.0/cg/store/filters/status_case_filters.py
--rw-r--r--   0        0        0     1461 2024-03-01 09:19:24.098125 cg-59.9.0/cg/store/filters/status_case_sample_filters.py
--rw-r--r--   0        0        0      903 2024-03-01 09:19:24.098125 cg-59.9.0/cg/store/filters/status_collaboration_filters.py
--rw-r--r--   0        0        0     1412 2024-03-01 09:19:24.098125 cg-59.9.0/cg/store/filters/status_customer_filters.py
--rw-r--r--   0        0        0     1880 2024-03-01 09:19:24.098125 cg-59.9.0/cg/store/filters/status_flow_cell_filters.py
--rw-r--r--   0        0        0     1255 2024-03-01 09:19:24.098125 cg-59.9.0/cg/store/filters/status_invoice_filters.py
--rw-r--r--   0        0        0     2792 2024-03-01 09:19:24.098125 cg-59.9.0/cg/store/filters/status_metrics_filters.py
--rw-r--r--   0        0        0     2323 2024-03-01 09:19:24.098125 cg-59.9.0/cg/store/filters/status_order_filters.py
--rw-r--r--   0        0        0      851 2024-03-01 09:19:24.098125 cg-59.9.0/cg/store/filters/status_organism_filters.py
--rw-r--r--   0        0        0      783 2024-03-01 09:19:24.098125 cg-59.9.0/cg/store/filters/status_panel_filters.py
--rw-r--r--   0        0        0     3923 2024-03-01 09:19:24.098125 cg-59.9.0/cg/store/filters/status_pool_filters.py
--rw-r--r--   0        0        0     8660 2024-03-01 09:19:24.098125 cg-59.9.0/cg/store/filters/status_sample_filters.py
--rw-r--r--   0        0        0      731 2024-03-01 09:19:24.098125 cg-59.9.0/cg/store/filters/status_user_filters.py
--rw-r--r--   0        0        0    37068 2024-03-01 09:19:24.098125 cg-59.9.0/cg/store/models.py
--rw-r--r--   0        0        0      593 2024-03-01 09:19:24.098125 cg-59.9.0/cg/store/store.py
--rw-r--r--   0        0        0       30 2024-03-01 09:19:24.098125 cg-59.9.0/cg/utils/__init__.py
--rw-r--r--   0        0        0      187 2024-03-01 09:19:24.098125 cg-59.9.0/cg/utils/calculations.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.098125 cg-59.9.0/cg/utils/checksum/__init__.py
--rw-r--r--   0        0        0     1579 2024-03-01 09:19:24.098125 cg-59.9.0/cg/utils/checksum/checksum.py
--rw-r--r--   0        0        0     1655 2024-03-01 09:19:24.098125 cg-59.9.0/cg/utils/click/EnumChoice.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.098125 cg-59.9.0/cg/utils/click/__init__.py
--rw-r--r--   0        0        0     4910 2024-03-01 09:19:24.098125 cg-59.9.0/cg/utils/commands.py
--rw-r--r--   0        0        0     1811 2024-03-01 09:19:24.098125 cg-59.9.0/cg/utils/date.py
--rw-r--r--   0        0        0      635 2024-03-01 09:19:24.098125 cg-59.9.0/cg/utils/dict.py
--rw-r--r--   0        0        0     2111 2024-03-01 09:19:24.098125 cg-59.9.0/cg/utils/dispatcher.py
--rw-r--r--   0        0        0     1251 2024-03-01 09:19:24.098125 cg-59.9.0/cg/utils/email.py
--rw-r--r--   0        0        0      134 2024-03-01 09:19:24.098125 cg-59.9.0/cg/utils/enums.py
--rw-r--r--   0        0        0     3178 2024-03-01 09:19:24.098125 cg-59.9.0/cg/utils/files.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.098125 cg-59.9.0/cg/utils/flask/__init__.py
--rw-r--r--   0        0        0     1052 2024-03-01 09:19:24.098125 cg-59.9.0/cg/utils/flask/enum.py
--rw-r--r--   0        0        0      834 2024-03-01 09:19:24.098125 cg-59.9.0/cg/utils/time.py
--rw-r--r--   0        0        0     1224 2024-03-01 09:19:24.098125 cg-59.9.0/cg/utils/utils.py
--rw-r--r--   0        0        0     1721 2024-03-01 09:19:24.102125 cg-59.9.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.102125 cg-59.9.0/tests/__init__.py
--rw-r--r--   0        0        0     1158 2024-03-01 09:19:24.102125 cg-59.9.0/tests/apps/conftest.py
--rw-r--r--   0        0        0      231 2024-03-01 09:19:24.102125 cg-59.9.0/tests/apps/coverage/conftest.py
--rw-r--r--   0        0        0     6188 2024-03-01 09:19:24.102125 cg-59.9.0/tests/apps/coverage/test_coverage.py
--rw-r--r--   0        0        0     1693 2024-03-01 09:19:24.102125 cg-59.9.0/tests/apps/crunchy/conftest.py
--rw-r--r--   0        0        0     5438 2024-03-01 09:19:24.102125 cg-59.9.0/tests/apps/crunchy/test_compress_fastq.py
--rw-r--r--   0        0        0     2283 2024-03-01 09:19:24.102125 cg-59.9.0/tests/apps/crunchy/test_config.py
--rw-r--r--   0        0        0    14032 2024-03-01 09:19:24.102125 cg-59.9.0/tests/apps/crunchy/test_crunchy.py
--rw-r--r--   0        0        0     9109 2024-03-01 09:19:24.102125 cg-59.9.0/tests/apps/crunchy/test_spring_decompression.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.102125 cg-59.9.0/tests/apps/demultiplex/__init__.py
--rw-r--r--   0        0        0    10776 2024-03-01 09:19:24.102125 cg-59.9.0/tests/apps/demultiplex/conftest.py
--rw-r--r--   0        0        0     8944 2024-03-01 09:19:24.102125 cg-59.9.0/tests/apps/demultiplex/test_demultiplex_api.py
--rw-r--r--   0        0        0     6098 2024-03-01 09:19:24.102125 cg-59.9.0/tests/apps/demultiplex/test_index.py
--rw-r--r--   0        0        0     9468 2024-03-01 09:19:24.102125 cg-59.9.0/tests/apps/demultiplex/test_override_cycles_validator.py
--rw-r--r--   0        0        0     6074 2024-03-01 09:19:24.102125 cg-59.9.0/tests/apps/demultiplex/test_read_sample_sheet.py
--rw-r--r--   0        0        0    15738 2024-03-01 09:19:24.102125 cg-59.9.0/tests/apps/demultiplex/test_sample_models.py
--rw-r--r--   0        0        0     4516 2024-03-01 09:19:24.102125 cg-59.9.0/tests/apps/demultiplex/test_sample_sheet_creator.py
--rw-r--r--   0        0        0     2244 2024-03-01 09:19:24.102125 cg-59.9.0/tests/apps/demultiplex/test_sample_sheet_creator_factory.py
--rw-r--r--   0        0        0     3271 2024-03-01 09:19:24.102125 cg-59.9.0/tests/apps/demultiplex/test_sample_sheet_models.py
--rw-r--r--   0        0        0    11331 2024-03-01 09:19:24.106124 cg-59.9.0/tests/apps/demultiplex/test_sample_sheet_validator.py
--rw-r--r--   0        0        0     1495 2024-03-01 09:19:24.106124 cg-59.9.0/tests/apps/demultiplex/test_validate.py
--rw-r--r--   0        0        0     5094 2024-03-01 09:19:24.106124 cg-59.9.0/tests/apps/downsample/test_downsample.py
--rw-r--r--   0        0        0     1419 2024-03-01 09:19:24.106124 cg-59.9.0/tests/apps/downsample/test_downsample_utils.py
--rw-r--r--   0        0        0     1716 2024-03-01 09:19:24.106124 cg-59.9.0/tests/apps/gens/test_gens_api.py
--rw-r--r--   0        0        0     1950 2024-03-01 09:19:24.106124 cg-59.9.0/tests/apps/gt/conftest.py
--rw-r--r--   0        0        0     4276 2024-03-01 09:19:24.106124 cg-59.9.0/tests/apps/gt/test_gt_api.py
--rw-r--r--   0        0        0     1453 2024-03-01 09:19:24.106124 cg-59.9.0/tests/apps/hk/conftest.py
--rw-r--r--   0        0        0      684 2024-03-01 09:19:24.106124 cg-59.9.0/tests/apps/hk/test__getattr__.py
--rw-r--r--   0        0        0     1593 2024-03-01 09:19:24.106124 cg-59.9.0/tests/apps/hk/test_add_file.py
--rw-r--r--   0        0        0     3523 2024-03-01 09:19:24.106124 cg-59.9.0/tests/apps/hk/test_bundles.py
--rw-r--r--   0        0        0      871 2024-03-01 09:19:24.106124 cg-59.9.0/tests/apps/hk/test_core.py
--rw-r--r--   0        0        0    24975 2024-03-01 09:19:24.106124 cg-59.9.0/tests/apps/hk/test_file.py
--rw-r--r--   0        0        0     5080 2024-03-01 09:19:24.106124 cg-59.9.0/tests/apps/hk/test_version.py
--rw-r--r--   0        0        0     1840 2024-03-01 09:19:24.106124 cg-59.9.0/tests/apps/lims/conftest.py
--rw-r--r--   0        0        0     3197 2024-03-01 09:19:24.106124 cg-59.9.0/tests/apps/lims/test_api.py
--rw-r--r--   0        0        0     1451 2024-03-01 09:19:24.106124 cg-59.9.0/tests/apps/lims/test_sample_sheet.py
--rw-r--r--   0        0        0     9223 2024-03-01 09:19:24.106124 cg-59.9.0/tests/apps/loqus/conftest.py
--rw-r--r--   0        0        0     8994 2024-03-01 09:19:24.106124 cg-59.9.0/tests/apps/loqus/test_loqusdb_api.py
--rw-r--r--   0        0        0     2439 2024-03-01 09:19:24.106124 cg-59.9.0/tests/apps/madeline/conftest.py
--rw-r--r--   0        0        0     4653 2024-03-01 09:19:24.106124 cg-59.9.0/tests/apps/madeline/test_madeline.py
--rw-r--r--   0        0        0     3328 2024-03-01 09:19:24.106124 cg-59.9.0/tests/apps/mip/conftest.py
--rw-r--r--   0        0        0     2487 2024-03-01 09:19:24.106124 cg-59.9.0/tests/apps/mip/test_config_mip.py
--rw-r--r--   0        0        0      883 2024-03-01 09:19:24.106124 cg-59.9.0/tests/apps/mutacc_auto/conftest.py
--rw-r--r--   0        0        0     2473 2024-03-01 09:19:24.106124 cg-59.9.0/tests/apps/mutacc_auto/test_mutacc_auto.py
--rw-r--r--   0        0        0    11930 2024-03-01 09:19:24.106124 cg-59.9.0/tests/apps/orderform/conftest.py
--rw-r--r--   0        0        0     9484 2024-03-01 09:19:24.106124 cg-59.9.0/tests/apps/orderform/test_excel_orderform_parser.py
--rw-r--r--   0        0        0     4351 2024-03-01 09:19:24.106124 cg-59.9.0/tests/apps/orderform/test_excel_sample_schema.py
--rw-r--r--   0        0        0     1032 2024-03-01 09:19:24.106124 cg-59.9.0/tests/apps/orderform/test_json_orderform_parser.py
--rw-r--r--   0        0        0     2474 2024-03-01 09:19:24.106124 cg-59.9.0/tests/apps/orderform/test_orderform_parser.py
--rw-r--r--   0        0        0    16002 2024-03-01 09:19:24.106124 cg-59.9.0/tests/apps/orderform/validators/test_excel_sample_validators.py
--rw-r--r--   0        0        0     3670 2024-03-01 09:19:24.106124 cg-59.9.0/tests/apps/scout/conftest.py
--rw-r--r--   0        0        0     2269 2024-03-01 09:19:24.106124 cg-59.9.0/tests/apps/scout/test_get_causative_variants.py
--rw-r--r--   0        0        0     1376 2024-03-01 09:19:24.106124 cg-59.9.0/tests/apps/scout/test_get_scout_cases.py
--rw-r--r--   0        0        0     1840 2024-03-01 09:19:24.106124 cg-59.9.0/tests/apps/scout/test_scout_load_config.py
--rw-r--r--   0        0        0     7047 2024-03-01 09:19:24.106124 cg-59.9.0/tests/apps/scout/test_scout_models.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.106124 cg-59.9.0/tests/apps/sequencing_metrics_parser/__init__.py
--rw-r--r--   0        0        0     2861 2024-03-01 09:19:24.106124 cg-59.9.0/tests/apps/sequencing_metrics_parser/conftest.py
--rw-r--r--   0        0        0     2010 2024-03-01 09:19:24.106124 cg-59.9.0/tests/apps/sequencing_metrics_parser/parsers/conftest.py
--rw-r--r--   0        0        0     1820 2024-03-01 09:19:24.106124 cg-59.9.0/tests/apps/sequencing_metrics_parser/parsers/test_bcl2fastq_parser.py
--rw-r--r--   0        0        0     1908 2024-03-01 09:19:24.106124 cg-59.9.0/tests/apps/sequencing_metrics_parser/parsers/test_bcl2fastq_to_sequencing_statistics.py
--rw-r--r--   0        0        0     2997 2024-03-01 09:19:24.106124 cg-59.9.0/tests/apps/sequencing_metrics_parser/parsers/test_bcl_convert_to_sequencing_statistics.py
--rw-r--r--   0        0        0     7322 2024-03-01 09:19:24.106124 cg-59.9.0/tests/apps/sequencing_metrics_parser/parsers/test_bclconvert.py
--rw-r--r--   0        0        0     1458 2024-03-01 09:19:24.106124 cg-59.9.0/tests/apps/sequencing_metrics_parser/test_sequencing_metrics_calculator.py
--rw-r--r--   0        0        0     1131 2024-03-01 09:19:24.106124 cg-59.9.0/tests/apps/slurm/conftest.py
--rw-r--r--   0        0        0     4412 2024-03-01 09:19:24.106124 cg-59.9.0/tests/apps/slurm/test_slurm_api.py
--rw-r--r--   0        0        0      831 2024-03-01 09:19:24.106124 cg-59.9.0/tests/apps/test_apps_environ.py
--rw-r--r--   0        0        0      957 2024-03-01 09:19:24.106124 cg-59.9.0/tests/apps/test_osticket.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.106124 cg-59.9.0/tests/cli/__init__.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.106124 cg-59.9.0/tests/cli/add/__init__.py
--rw-r--r--   0        0        0     1174 2024-03-01 09:19:24.106124 cg-59.9.0/tests/cli/add/test_cli_add.py
--rw-r--r--   0        0        0     2471 2024-03-01 09:19:24.106124 cg-59.9.0/tests/cli/add/test_cli_add_customer.py
--rw-r--r--   0        0        0     6747 2024-03-01 09:19:24.106124 cg-59.9.0/tests/cli/add/test_cli_add_family.py
--rw-r--r--   0        0        0     7588 2024-03-01 09:19:24.106124 cg-59.9.0/tests/cli/add/test_cli_add_relationship.py
--rw-r--r--   0        0        0     7694 2024-03-01 09:19:24.106124 cg-59.9.0/tests/cli/add/test_cli_add_sample.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.106124 cg-59.9.0/tests/cli/backup/__init__.py
--rw-r--r--   0        0        0      705 2024-03-01 09:19:24.106124 cg-59.9.0/tests/cli/backup/conftest.py
--rw-r--r--   0        0        0    11101 2024-03-01 09:19:24.106124 cg-59.9.0/tests/cli/backup/test_backup_command.py
--rw-r--r--   0        0        0     6865 2024-03-01 09:19:24.106124 cg-59.9.0/tests/cli/clean/conftest.py
--rw-r--r--   0        0        0     5536 2024-03-01 09:19:24.106124 cg-59.9.0/tests/cli/clean/test_balsamic_clean.py
--rw-r--r--   0        0        0     2557 2024-03-01 09:19:24.106124 cg-59.9.0/tests/cli/clean/test_clean_flow_cell.py
--rw-r--r--   0        0        0     1830 2024-03-01 09:19:24.106124 cg-59.9.0/tests/cli/clean/test_clean_hk_bundle_files.py
--rw-r--r--   0        0        0     2098 2024-03-01 09:19:24.106124 cg-59.9.0/tests/cli/clean/test_hk_bundle_files.py
--rw-r--r--   0        0        0     4610 2024-03-01 09:19:24.106124 cg-59.9.0/tests/cli/clean/test_hk_case_bundle_files.py
--rw-r--r--   0        0        0     3585 2024-03-01 09:19:24.106124 cg-59.9.0/tests/cli/clean/test_microbial_clean.py
--rw-r--r--   0        0        0     1881 2024-03-01 09:19:24.106124 cg-59.9.0/tests/cli/clean/test_rsync_past_run_dirs.py
--rw-r--r--   0        0        0     9707 2024-03-01 09:19:24.106124 cg-59.9.0/tests/cli/compress/conftest.py
--rw-r--r--   0        0        0     7709 2024-03-01 09:19:24.106124 cg-59.9.0/tests/cli/compress/test_cli_compress_fastq.py
--rw-r--r--   0        0        0     1416 2024-03-01 09:19:24.106124 cg-59.9.0/tests/cli/compress/test_cli_decompress_spring.py
--rw-r--r--   0        0        0     5205 2024-03-01 09:19:24.106124 cg-59.9.0/tests/cli/compress/test_compress_helpers.py
--rw-r--r--   0        0        0     1239 2024-03-01 09:19:24.106124 cg-59.9.0/tests/cli/compress/test_store_fastq.py
--rw-r--r--   0        0        0     7558 2024-03-01 09:19:24.106124 cg-59.9.0/tests/cli/conftest.py
--rw-r--r--   0        0        0    12747 2024-03-01 09:19:24.106124 cg-59.9.0/tests/cli/delete/test_cli_delete_case.py
--rw-r--r--   0        0        0     1873 2024-03-01 09:19:24.110125 cg-59.9.0/tests/cli/delete/test_cli_delete_cases.py
--rw-r--r--   0        0        0     3794 2024-03-01 09:19:24.110125 cg-59.9.0/tests/cli/deliver/conftest.py
--rw-r--r--   0        0        0     4630 2024-03-01 09:19:24.110125 cg-59.9.0/tests/cli/deliver/test_deliver_base.py
--rw-r--r--   0        0        0     1166 2024-03-01 09:19:24.110125 cg-59.9.0/tests/cli/deliver/test_rsync_base.py
--rw-r--r--   0        0        0     8569 2024-03-01 09:19:24.110125 cg-59.9.0/tests/cli/deliver/test_run_deliver_cmd.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.110125 cg-59.9.0/tests/cli/demultiplex/__init__.py
--rw-r--r--   0        0        0     9244 2024-03-01 09:19:24.110125 cg-59.9.0/tests/cli/demultiplex/test_create_sample_sheet.py
--rw-r--r--   0        0        0     8683 2024-03-01 09:19:24.110125 cg-59.9.0/tests/cli/demultiplex/test_demultiplex_flowcell.py
--rw-r--r--   0        0        0     1607 2024-03-01 09:19:24.110125 cg-59.9.0/tests/cli/demultiplex/test_finish_demux.py
--rw-r--r--   0        0        0     3704 2024-03-01 09:19:24.110125 cg-59.9.0/tests/cli/demultiplex/test_validate_sample_sheet.py
--rw-r--r--   0        0        0     4423 2024-03-01 09:19:24.110125 cg-59.9.0/tests/cli/demultiplex/test_verify_syncing.py
--rw-r--r--   0        0        0     1585 2024-03-01 09:19:24.110125 cg-59.9.0/tests/cli/downsample/test_cli_downsample.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.110125 cg-59.9.0/tests/cli/generate/__init__.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.110125 cg-59.9.0/tests/cli/generate/report/__init__.py
--rw-r--r--   0        0        0     1622 2024-03-01 09:19:24.110125 cg-59.9.0/tests/cli/generate/report/conftest.py
--rw-r--r--   0        0        0     2477 2024-03-01 09:19:24.110125 cg-59.9.0/tests/cli/generate/report/test_cli_delivery_report.py
--rw-r--r--   0        0        0     2760 2024-03-01 09:19:24.110125 cg-59.9.0/tests/cli/generate/report/test_utils.py
--rw-r--r--   0        0        0      563 2024-03-01 09:19:24.110125 cg-59.9.0/tests/cli/generate/test_cli_base.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.110125 cg-59.9.0/tests/cli/get/__init__.py
--rw-r--r--   0        0        0      863 2024-03-01 09:19:24.110125 cg-59.9.0/tests/cli/get/test_cli_get.py
--rw-r--r--   0        0        0     1526 2024-03-01 09:19:24.110125 cg-59.9.0/tests/cli/get/test_cli_get_analysis.py
--rw-r--r--   0        0        0     1242 2024-03-01 09:19:24.110125 cg-59.9.0/tests/cli/get/test_cli_get_case.py
--rw-r--r--   0        0        0     6208 2024-03-01 09:19:24.110125 cg-59.9.0/tests/cli/get/test_cli_get_flow_cell.py
--rw-r--r--   0        0        0     8835 2024-03-01 09:19:24.110125 cg-59.9.0/tests/cli/get/test_cli_get_sample.py
--rw-r--r--   0        0        0     1364 2024-03-01 09:19:24.110125 cg-59.9.0/tests/cli/set/conftest.py
--rw-r--r--   0        0        0     7311 2024-03-01 09:19:24.110125 cg-59.9.0/tests/cli/set/test_cli_set_case.py
--rw-r--r--   0        0        0     1460 2024-03-01 09:19:24.110125 cg-59.9.0/tests/cli/set/test_cli_set_cases.py
--rw-r--r--   0        0        0     2016 2024-03-01 09:19:24.110125 cg-59.9.0/tests/cli/set/test_cli_set_flowcell.py
--rw-r--r--   0        0        0     1685 2024-03-01 09:19:24.110125 cg-59.9.0/tests/cli/set/test_cli_set_list_keys.py
--rw-r--r--   0        0        0    12450 2024-03-01 09:19:24.110125 cg-59.9.0/tests/cli/set/test_cli_set_sample.py
--rw-r--r--   0        0        0     6124 2024-03-01 09:19:24.110125 cg-59.9.0/tests/cli/set/test_cli_set_samples.py
--rw-r--r--   0        0        0     6934 2024-03-01 09:19:24.110125 cg-59.9.0/tests/cli/store/test_fastq.py
--rw-r--r--   0        0        0     2332 2024-03-01 09:19:24.110125 cg-59.9.0/tests/cli/test_base.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.110125 cg-59.9.0/tests/cli/upload/__init__.py
--rw-r--r--   0        0        0    10003 2024-03-01 09:19:24.110125 cg-59.9.0/tests/cli/upload/conftest.py
--rw-r--r--   0        0        0     2295 2024-03-01 09:19:24.110125 cg-59.9.0/tests/cli/upload/test_cli_scout.py
--rw-r--r--   0        0        0     1789 2024-03-01 09:19:24.110125 cg-59.9.0/tests/cli/upload/test_cli_upload.py
--rw-r--r--   0        0        0      971 2024-03-01 09:19:24.110125 cg-59.9.0/tests/cli/upload/test_cli_upload_auto.py
--rw-r--r--   0        0        0     1669 2024-03-01 09:19:24.110125 cg-59.9.0/tests/cli/upload/test_cli_upload_delivery_report.py
--rw-r--r--   0        0        0      895 2024-03-01 09:19:24.110125 cg-59.9.0/tests/cli/upload/test_cli_upload_fastq.py
--rw-r--r--   0        0        0     1199 2024-03-01 09:19:24.110125 cg-59.9.0/tests/cli/upload/test_cli_upload_genotype.py
--rw-r--r--   0        0        0      694 2024-03-01 09:19:24.110125 cg-59.9.0/tests/cli/upload/test_cli_upload_gens.py
--rw-r--r--   0        0        0     9965 2024-03-01 09:19:24.110125 cg-59.9.0/tests/cli/upload/test_cli_upload_nipt.py
--rw-r--r--   0        0        0     4684 2024-03-01 09:19:24.110125 cg-59.9.0/tests/cli/upload/test_cli_upload_nipt_ftp.py
--rw-r--r--   0        0        0     1839 2024-03-01 09:19:24.110125 cg-59.9.0/tests/cli/upload/test_cli_upload_nipt_statina.py
--rw-r--r--   0        0        0     6177 2024-03-01 09:19:24.110125 cg-59.9.0/tests/cli/upload/test_cli_upload_observations.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.110125 cg-59.9.0/tests/cli/workflow/__init__.py
--rw-r--r--   0        0        0    30612 2024-03-01 09:19:24.110125 cg-59.9.0/tests/cli/workflow/balsamic/conftest.py
--rw-r--r--   0        0        0    13938 2024-03-01 09:19:24.110125 cg-59.9.0/tests/cli/workflow/balsamic/test_cli_balsamic_config_case.py
--rw-r--r--   0        0        0     7957 2024-03-01 09:19:24.110125 cg-59.9.0/tests/cli/workflow/balsamic/test_compound_commands.py
--rw-r--r--   0        0        0     2336 2024-03-01 09:19:24.110125 cg-59.9.0/tests/cli/workflow/balsamic/test_link.py
--rw-r--r--   0        0        0     3554 2024-03-01 09:19:24.110125 cg-59.9.0/tests/cli/workflow/balsamic/test_report_deliver.py
--rw-r--r--   0        0        0     6209 2024-03-01 09:19:24.110125 cg-59.9.0/tests/cli/workflow/balsamic/test_run.py
--rw-r--r--   0        0        0     6934 2024-03-01 09:19:24.110125 cg-59.9.0/tests/cli/workflow/balsamic/test_store_housekeeper.py
--rw-r--r--   0        0        0     8458 2024-03-01 09:19:24.110125 cg-59.9.0/tests/cli/workflow/conftest.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.110125 cg-59.9.0/tests/cli/workflow/fastq/__init__.py
--rw-r--r--   0        0        0     2298 2024-03-01 09:19:24.110125 cg-59.9.0/tests/cli/workflow/fastq/test_fastq_base.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.110125 cg-59.9.0/tests/cli/workflow/fluffy/__init__.py
--rw-r--r--   0        0        0     5291 2024-03-01 09:19:24.110125 cg-59.9.0/tests/cli/workflow/fluffy/conftest.py
--rw-r--r--   0        0        0     5687 2024-03-01 09:19:24.110125 cg-59.9.0/tests/cli/workflow/fluffy/test_cli_create_samplesheet.py
--rw-r--r--   0        0        0     3302 2024-03-01 09:19:24.110125 cg-59.9.0/tests/cli/workflow/fluffy/test_cli_link.py
--rw-r--r--   0        0        0     1896 2024-03-01 09:19:24.110125 cg-59.9.0/tests/cli/workflow/fluffy/test_cli_run.py
--rw-r--r--   0        0        0     2968 2024-03-01 09:19:24.110125 cg-59.9.0/tests/cli/workflow/fluffy/test_cli_start.py
--rw-r--r--   0        0        0     7815 2024-03-01 09:19:24.110125 cg-59.9.0/tests/cli/workflow/fluffy/test_cli_store.py
--rw-r--r--   0        0        0     2775 2024-03-01 09:19:24.110125 cg-59.9.0/tests/cli/workflow/microsalt/conftest.py
--rw-r--r--   0        0        0     6926 2024-03-01 09:19:24.110125 cg-59.9.0/tests/cli/workflow/microsalt/test_microsalt_case_config.py
--rw-r--r--   0        0        0     1000 2024-03-01 09:19:24.110125 cg-59.9.0/tests/cli/workflow/microsalt/test_microsalt_run.py
--rw-r--r--   0        0        0     6544 2024-03-01 09:19:24.110125 cg-59.9.0/tests/cli/workflow/mip/conftest.py
--rw-r--r--   0        0        0     7011 2024-03-01 09:19:24.110125 cg-59.9.0/tests/cli/workflow/mip/test_cli_mip_base.py
--rw-r--r--   0        0        0     1542 2024-03-01 09:19:24.110125 cg-59.9.0/tests/cli/workflow/mip/test_cli_mip_dna_config_case.py
--rw-r--r--   0        0        0      431 2024-03-01 09:19:24.110125 cg-59.9.0/tests/cli/workflow/mip/test_cli_mip_dna_link.py
--rw-r--r--   0        0        0     2108 2024-03-01 09:19:24.110125 cg-59.9.0/tests/cli/workflow/mip/test_cli_mip_dna_manged_variants.py
--rw-r--r--   0        0        0     1273 2024-03-01 09:19:24.110125 cg-59.9.0/tests/cli/workflow/mip/test_cli_mip_dna_panel.py
--rw-r--r--   0        0        0     3595 2024-03-01 09:19:24.110125 cg-59.9.0/tests/cli/workflow/mip/test_cli_mip_dna_run.py
--rw-r--r--   0        0        0     3884 2024-03-01 09:19:24.110125 cg-59.9.0/tests/cli/workflow/mip/test_cli_mip_dna_start.py
--rw-r--r--   0        0        0     1004 2024-03-01 09:19:24.110125 cg-59.9.0/tests/cli/workflow/mip/test_cli_mip_rna_config_case.py
--rw-r--r--   0        0        0      527 2024-03-01 09:19:24.110125 cg-59.9.0/tests/cli/workflow/mip/test_cli_mip_rna_link.py
--rw-r--r--   0        0        0      716 2024-03-01 09:19:24.110125 cg-59.9.0/tests/cli/workflow/mip/test_cli_mip_rna_run.py
--rw-r--r--   0        0        0     8559 2024-03-01 09:19:24.110125 cg-59.9.0/tests/cli/workflow/mip/test_cli_mip_store.py
--rw-r--r--   0        0        0     1864 2024-03-01 09:19:24.110125 cg-59.9.0/tests/cli/workflow/nf_analysis/test_cli_config_case.py
--rw-r--r--   0        0        0     1927 2024-03-01 09:19:24.114125 cg-59.9.0/tests/cli/workflow/nf_analysis/test_cli_metrics_deliver.py
--rw-r--r--   0        0        0     5075 2024-03-01 09:19:24.114125 cg-59.9.0/tests/cli/workflow/nf_analysis/test_cli_report_deliver.py
--rw-r--r--   0        0        0     4498 2024-03-01 09:19:24.114125 cg-59.9.0/tests/cli/workflow/raredisease/test_cli_raredisease_compound_commands.py
--rw-r--r--   0        0        0     9843 2024-03-01 09:19:24.114125 cg-59.9.0/tests/cli/workflow/rnafusion/test_cli_rnafusion_compound_commands.py
--rw-r--r--   0        0        0     5887 2024-03-01 09:19:24.114125 cg-59.9.0/tests/cli/workflow/rnafusion/test_cli_rnafusion_config_case.py
--rw-r--r--   0        0        0     1602 2024-03-01 09:19:24.114125 cg-59.9.0/tests/cli/workflow/rnafusion/test_cli_rnafusion_metrics_deliver.py
--rw-r--r--   0        0        0     7899 2024-03-01 09:19:24.114125 cg-59.9.0/tests/cli/workflow/rnafusion/test_cli_rnafusion_run.py
--rw-r--r--   0        0        0     8710 2024-03-01 09:19:24.114125 cg-59.9.0/tests/cli/workflow/rnafusion/test_cli_rnafusion_store_housekeeper.py
--rw-r--r--   0        0        0     2409 2024-03-01 09:19:24.114125 cg-59.9.0/tests/cli/workflow/taxprofiler/test_cli_taxprofiler_compound_commands.py
--rw-r--r--   0        0        0     3302 2024-03-01 09:19:24.114125 cg-59.9.0/tests/cli/workflow/taxprofiler/test_cli_taxprofiler_config_case.py
--rw-r--r--   0        0        0     1521 2024-03-01 09:19:24.114125 cg-59.9.0/tests/cli/workflow/taxprofiler/test_cli_taxprofiler_metrics_deliver.py
--rw-r--r--   0        0        0     3933 2024-03-01 09:19:24.114125 cg-59.9.0/tests/cli/workflow/taxprofiler/test_cli_taxprofiler_run.py
--rw-r--r--   0        0        0      837 2024-03-01 09:19:24.114125 cg-59.9.0/tests/cli/workflow/test_cli_workflow.py
--rw-r--r--   0        0        0     4310 2024-03-01 09:19:24.114125 cg-59.9.0/tests/cli/workflow/test_cli_workflow_clean.py
--rw-r--r--   0        0        0     2346 2024-03-01 09:19:24.114125 cg-59.9.0/tests/clients/conftest.py
--rw-r--r--   0        0        0     1812 2024-03-01 09:19:24.114125 cg-59.9.0/tests/clients/janus/test_janus_api_client.py
--rw-r--r--   0        0        0   100013 2024-03-01 09:19:24.114125 cg-59.9.0/tests/conftest.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.114125 cg-59.9.0/tests/fixture_plugins/__init__.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.114125 cg-59.9.0/tests/fixture_plugins/demultiplex_fixtures/__init__.py
--rw-r--r--   0        0        0     4867 2024-03-01 09:19:24.114125 cg-59.9.0/tests/fixture_plugins/demultiplex_fixtures/flow_cell_fixtures.py
--rw-r--r--   0        0        0     3686 2024-03-01 09:19:24.114125 cg-59.9.0/tests/fixture_plugins/demultiplex_fixtures/name_fixtures.py
--rw-r--r--   0        0        0    21233 2024-03-01 09:19:24.114125 cg-59.9.0/tests/fixture_plugins/demultiplex_fixtures/path_fixtures.py
--rw-r--r--   0        0        0     3699 2024-03-01 09:19:24.114125 cg-59.9.0/tests/fixture_plugins/demultiplex_fixtures/run_parameters_fixtures.py
--rw-r--r--   0        0        0     4385 2024-03-01 09:19:24.114125 cg-59.9.0/tests/fixture_plugins/demultiplex_fixtures/sample_fixtures.py
--rw-r--r--   0        0        0     5824 2024-03-01 09:19:24.114125 cg-59.9.0/tests/fixture_plugins/demultiplex_fixtures/sample_sheet_fixtures.py
--rw-r--r--   0        0        0     1304 2024-03-01 09:19:24.114125 cg-59.9.0/tests/fixture_plugins/timestamp_fixtures.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.114125 cg-59.9.0/tests/fixtures/analysis/balsamic/tn_wgs/adm1.cram
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.114125 cg-59.9.0/tests/fixtures/analysis/balsamic/tn_wgs/ascat.output.pdf
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.114125 cg-59.9.0/tests/fixtures/analysis/balsamic/tn_wgs/snv.vcf
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.114125 cg-59.9.0/tests/fixtures/analysis/balsamic/tn_wgs/sv.vcf
--rw-r--r--   0        0        0    14644 2024-03-01 09:19:24.114125 cg-59.9.0/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/ACC11111_qc_fail.json
--rw-r--r--   0        0        0    15921 2024-03-01 09:19:24.114125 cg-59.9.0/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/ACC22222_qc_pass.json
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.114125 cg-59.9.0/tests/fixtures/analysis/mip/dna/ADM1.baf.bed.gz
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.114125 cg-59.9.0/tests/fixtures/analysis/mip/dna/ADM1.cov.bed.gz
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.114125 cg-59.9.0/tests/fixtures/analysis/mip/dna/ADM2.cram
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.114125 cg-59.9.0/tests/fixtures/analysis/mip/dna/ADM3.cram
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.114125 cg-59.9.0/tests/fixtures/analysis/mip/dna/adm1.cram
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.114125 cg-59.9.0/tests/fixtures/analysis/mip/dna/adm1.mt.bam
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.114125 cg-59.9.0/tests/fixtures/analysis/mip/dna/multiqc.html
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.114125 cg-59.9.0/tests/fixtures/analysis/mip/dna/report.pdf
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.114125 cg-59.9.0/tests/fixtures/analysis/mip/dna/smn.vcf
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.114125 cg-59.9.0/tests/fixtures/analysis/mip/dna/snv.vcf
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.114125 cg-59.9.0/tests/fixtures/analysis/mip/dna/snv_research.vcf
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.114125 cg-59.9.0/tests/fixtures/analysis/mip/dna/str.vcf
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.114125 cg-59.9.0/tests/fixtures/analysis/mip/dna/sv.vcf
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.114125 cg-59.9.0/tests/fixtures/analysis/mip/dna/sv_research.vcf
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.114125 cg-59.9.0/tests/fixtures/analysis/mip/dna/vcf2cytosure.txt
--rw-r--r--   0        0        0     5497 2024-03-01 09:19:24.114125 cg-59.9.0/tests/fixtures/analysis/rnafusion/multiqc_data.json
--rw-r--r--   0        0        0    11711 2024-03-01 09:19:24.114125 cg-59.9.0/tests/fixtures/analysis/rnafusion/rnafusion_case_enough_reads_metrics_deliverables.yaml
--rw-r--r--   0        0        0     2873 2024-03-01 09:19:24.114125 cg-59.9.0/tests/fixtures/analysis/sample_coverage.bed
--rw-r--r--   0        0        0     6506 2024-03-01 09:19:24.114125 cg-59.9.0/tests/fixtures/analysis/taxprofiler/multiqc_data.json
--rw-r--r--   0        0        0    10513 2024-03-01 09:19:24.114125 cg-59.9.0/tests/fixtures/analysis/taxprofiler/taxprofiler_case_metrics_deliverables.yaml
--rw-r--r--   0        0        0    10961 2024-03-01 09:19:24.114125 cg-59.9.0/tests/fixtures/apps/balsamic/case/config.json
--rw-r--r--   0        0        0     3465 2024-03-01 09:19:24.114125 cg-59.9.0/tests/fixtures/apps/balsamic/case/metadata.yml
--rw-r--r--   0        0        0       63 2024-03-01 09:19:24.114125 cg-59.9.0/tests/fixtures/apps/balsamic/case/metadata_directory.yml
--rw-r--r--   0        0        0      165 2024-03-01 09:19:24.114125 cg-59.9.0/tests/fixtures/apps/balsamic/case/metadata_file_tags.yml
--rw-r--r--   0        0        0     2705 2024-03-01 09:19:24.114125 cg-59.9.0/tests/fixtures/apps/balsamic/case/metrics_deliverables.yaml
--rw-r--r--   0        0        0      692 2024-03-01 09:19:24.114125 cg-59.9.0/tests/fixtures/apps/crunchy/spring_metadata.json
--rw-r--r--   0        0        0      156 2024-03-01 09:19:24.114125 cg-59.9.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/SampleSheet.csv
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.114125 cg-59.9.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/Unaligned/Project_150031/Sample_SVE2528A1_CTGAAGCT/HHKVCALXX-l1t11_150031_S5_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.114125 cg-59.9.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/Unaligned/Project_150031/Sample_SVE2528A1_CTGAAGCT/HHKVCALXX-l1t11_150031_S5_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.118125 cg-59.9.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/Unaligned/Project_150031/Sample_SVE2528A1_CTGAAGCT/HHKVCALXX-l1t21_150031_S5_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.118125 cg-59.9.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/Unaligned/Project_150031/Sample_SVE2528A1_CTGAAGCT/HHKVCALXX-l1t21_150031_S5_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.118125 cg-59.9.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/Undetermined_S0_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.118125 cg-59.9.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/Undetermined_S0_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.118125 cg-59.9.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/demuxcomplete.txt
--rw-r--r--   0        0        0     1781 2024-03-01 09:19:24.118125 cg-59.9.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/l1t11/Stats/Stats.json
--rw-r--r--   0        0        0     2532 2024-03-01 09:19:24.118125 cg-59.9.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/l1t21/Stats/Stats.json
--rw-r--r--   0        0        0     1757 2024-03-01 09:19:24.118125 cg-59.9.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
--rw-r--r--   0        0        0        7 2024-03-01 09:19:24.118125 cg-59.9.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/SampleSheet.csv
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.118125 cg-59.9.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/HN3FKDSXY_AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.118125 cg-59.9.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/HN3FKDSXY_AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0     6034 2024-03-01 09:19:24.118125 cg-59.9.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml
--rw-r--r--   0        0        0     1172 2024-03-01 09:19:24.118125 cg-59.9.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml
--rw-r--r--   0        0        0        7 2024-03-01 09:19:24.118125 cg-59.9.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/fastq_1.fastq.gz
--rw-r--r--   0        0        0        7 2024-03-01 09:19:24.118125 cg-59.9.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/fastq_2.fastq.gz
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.118125 cg-59.9.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/BCLConvert/fastq/ACC11927A2_S1_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.118125 cg-59.9.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/BCLConvert/fastq/ACC11927A2_S1_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.118125 cg-59.9.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/BCLConvert/fastq/ACC11927A2_S1_L002_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.118125 cg-59.9.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/BCLConvert/fastq/ACC11927A2_S1_L002_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.118125 cg-59.9.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/BCLConvert/fastq/ACC11927A5_S1_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.118125 cg-59.9.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/BCLConvert/fastq/ACC11927A5_S1_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.118125 cg-59.9.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/BCLConvert/fastq/ACC11927A5_S1_L002_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.118125 cg-59.9.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/BCLConvert/fastq/ACC11927A5_S1_L002_R2_001.fastq.gz
--rw-r--r--   0        0        0      345 2024-03-01 09:19:24.118125 cg-59.9.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/Reports/Adapter_Metrics.csv
--rw-r--r--   0        0        0      650 2024-03-01 09:19:24.118125 cg-59.9.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/Reports/Demultiplex_Stats.csv
--rw-r--r--   0        0        0      896 2024-03-01 09:19:24.118125 cg-59.9.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/Reports/Quality_Metrics.csv
--rw-r--r--   0        0        0      602 2024-03-01 09:19:24.118125 cg-59.9.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/SampleSheet.csv
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.118125 cg-59.9.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/demuxcomplete.txt
--rw-r--r--   0        0        0      315 2024-03-01 09:19:24.118125 cg-59.9.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRZZ/Unaligned/Reports/Adapter_Metrics.csv
--rw-r--r--   0        0        0      434 2024-03-01 09:19:24.118125 cg-59.9.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRZZ/Unaligned/Reports/Quality_Metrics.csv
--rw-r--r--   0        0        0     8624 2024-03-01 09:19:24.118125 cg-59.9.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRZZ/Unaligned/Reports/RunInfo.xml
--rw-r--r--   0        0        0      568 2024-03-01 09:19:24.118125 cg-59.9.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/SampleSheet.csv
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.118125 cg-59.9.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A2/HY7FFDRX2_ACC11927A2_S1_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.118125 cg-59.9.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A2/HY7FFDRX2_ACC11927A2_S1_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.118125 cg-59.9.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A2/HY7FFDRX2_ACC11927A2_S1_L002_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.118125 cg-59.9.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A2/HY7FFDRX2_ACC11927A2_S1_L002_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.118125 cg-59.9.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A5/HY7FFDRX2_ACC11927A5_S1_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.118125 cg-59.9.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A5/HY7FFDRX2_ACC11927A5_S1_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.118125 cg-59.9.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A5/HY7FFDRX2_ACC11927A5_S1_L002_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.118125 cg-59.9.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A5/HY7FFDRX2_ACC11927A5_S1_L002_R2_001.fastq.gz
--rw-r--r--   0        0        0      220 2024-03-01 09:19:24.118125 cg-59.9.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Reports/Adapter_Metrics.csv
--rw-r--r--   0        0        0      463 2024-03-01 09:19:24.118125 cg-59.9.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Reports/Demultiplex_Stats.csv
--rw-r--r--   0        0        0      622 2024-03-01 09:19:24.118125 cg-59.9.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Reports/Quality_Metrics.csv
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.118125 cg-59.9.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Undetermined_S0_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.118125 cg-59.9.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/demuxcomplete.txt
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.118125 cg-59.9.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A2_S1_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.118125 cg-59.9.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A2_S1_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.118125 cg-59.9.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A2_S1_L002_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.118125 cg-59.9.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A2_S1_L002_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.118125 cg-59.9.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A5_S1_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.118125 cg-59.9.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A5_S1_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.118125 cg-59.9.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A5_S1_L002_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.118125 cg-59.9.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A5_S1_L002_R2_001.fastq.gz
--rw-r--r--   0        0        0      345 2024-03-01 09:19:24.118125 cg-59.9.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/Reports/Adapter_Metrics.csv
--rw-r--r--   0        0        0      650 2024-03-01 09:19:24.118125 cg-59.9.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/Reports/Demultiplex_Stats.csv
--rw-r--r--   0        0        0      896 2024-03-01 09:19:24.118125 cg-59.9.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/Reports/Quality_Metrics.csv
--rw-r--r--   0        0        0      619 2024-03-01 09:19:24.118125 cg-59.9.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/SampleSheet.csv
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.118125 cg-59.9.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/demuxcomplete.txt
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.114125 cg-59.9.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.114125 cg-59.9.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0     4439 2024-03-01 09:19:24.114125 cg-59.9.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml
--rw-r--r--   0        0        0     1172 2024-03-01 09:19:24.114125 cg-59.9.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.114125 cg-59.9.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L001_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.114125 cg-59.9.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L001_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.114125 cg-59.9.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L002_R1_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.114125 cg-59.9.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L002_R2_001.fastq.gz
--rw-r--r--   0        0        0       43 2024-03-01 09:19:24.118125 cg-59.9.0/tests/fixtures/apps/demultiplexing/fastq/dummy_run_R1_001.fastq.gz
--rw-r--r--   0        0        0       67 2024-03-01 09:19:24.118125 cg-59.9.0/tests/fixtures/apps/demultiplexing/fastq/dummy_run_R1_001.fastq.gz.md5
--rw-r--r--   0        0        0   338370 2024-03-01 09:19:24.118125 cg-59.9.0/tests/fixtures/apps/demultiplexing/fastq/fastq_run_R1_001.fastq.gz
--rw-r--r--   0        0        0       67 2024-03-01 09:19:24.118125 cg-59.9.0/tests/fixtures/apps/demultiplexing/fastq/fastq_run_R1_001.fastq.gz.md5
--rw-r--r--   0        0        0   338349 2024-03-01 09:19:24.118125 cg-59.9.0/tests/fixtures/apps/demultiplexing/fastq/fastq_run_R2_001.fastq.gz
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.118125 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/CopyComplete.txt
--rw-r--r--   0        0        0     2126 2024-03-01 09:19:24.122125 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/HJCFFALXX_bcl2fastq_raw.json
--rw-r--r--   0        0        0     1827 2024-03-01 09:19:24.122125 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/HJCFFALXX_bcl_convert_raw.json
--rw-r--r--   0        0        0       90 2024-03-01 09:19:24.122125 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/README.txt
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.122125 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTAComplete.txt
--rw-r--r--   0        0        0     6895 2024-03-01 09:19:24.122125 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTAConfiguration.xml
--rw-r--r--   0        0        0       37 2024-03-01 09:19:24.122125 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTARead1Complete.txt
--rw-r--r--   0        0        0       36 2024-03-01 09:19:24.122125 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTARead2Complete.txt
--rw-r--r--   0        0        0       36 2024-03-01 09:19:24.122125 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTARead3Complete.txt
--rw-r--r--   0        0        0    24755 2024-03-01 09:19:24.122125 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RunInfo.xml
--rw-r--r--   0        0        0      692 2024-03-01 09:19:24.122125 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet.csv
--rw-r--r--   0        0        0      724 2024-03-01 09:19:24.122125 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet_bcl2fastq.csv
--rw-r--r--   0        0        0       61 2024-03-01 09:19:24.122125 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/SequencingComplete.txt
--rw-r--r--   0        0        0     5775 2024-03-01 09:19:24.122125 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/runParameters.xml
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.122125 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/CopyComplete.txt
--rw-r--r--   0        0        0     2282 2024-03-01 09:19:24.122125 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/HL32LCCXY_bcl2fastq_raw.json
--rw-r--r--   0        0        0     1632 2024-03-01 09:19:24.122125 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/HL32LCCXY_bcl_convert_raw.json
--rw-r--r--   0        0        0       75 2024-03-01 09:19:24.122125 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/README.txt
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.122125 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTAComplete.txt
--rw-r--r--   0        0        0     6912 2024-03-01 09:19:24.122125 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTAConfiguration.xml
--rw-r--r--   0        0        0       36 2024-03-01 09:19:24.122125 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTARead1Complete.txt
--rw-r--r--   0        0        0       36 2024-03-01 09:19:24.122125 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTARead2Complete.txt
--rw-r--r--   0        0        0       36 2024-03-01 09:19:24.122125 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTARead3Complete.txt
--rw-r--r--   0        0        0       36 2024-03-01 09:19:24.122125 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTARead4Complete.txt
--rw-r--r--   0        0        0    24814 2024-03-01 09:19:24.122125 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RunInfo.xml
--rw-r--r--   0        0        0      814 2024-03-01 09:19:24.122125 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/SampleSheet.csv
--rw-r--r--   0        0        0      660 2024-03-01 09:19:24.122125 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/SampleSheet_bcl2fastq.csv
--rw-r--r--   0        0        0       61 2024-03-01 09:19:24.122125 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/SequencingComplete.txt
--rw-r--r--   0        0        0     5853 2024-03-01 09:19:24.122125 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/runParameters.xml
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.122125 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/CopyComplete.txt
--rw-r--r--   0        0        0    21848 2024-03-01 09:19:24.122125 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/HGYFNBCX2_bcl2fastq_raw.json
--rw-r--r--   0        0        0    15512 2024-03-01 09:19:24.122125 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/HGYFNBCX2_bcl_convert_raw.json
--rw-r--r--   0        0        0       79 2024-03-01 09:19:24.122125 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/README.txt
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.122125 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/RTAComplete.txt
--rw-r--r--   0        0        0      756 2024-03-01 09:19:24.122125 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/RunInfo.xml
--rw-r--r--   0        0        0     4118 2024-03-01 09:19:24.122125 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/SampleSheet.csv
--rw-r--r--   0        0        0     1408 2024-03-01 09:19:24.122125 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/SampleSheet_bcl2fastq.csv
--rw-r--r--   0        0        0     5326 2024-03-01 09:19:24.122125 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/runParameters.xml
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.122125 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/CopyComplete.txt
--rw-r--r--   0        0        0    15041 2024-03-01 09:19:24.122125 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/HM2LNBCX2_bcl2fastq_raw.json
--rw-r--r--   0        0        0    10649 2024-03-01 09:19:24.122125 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/HM2LNBCX2_bcl_convert_raw.json
--rw-r--r--   0        0        0       80 2024-03-01 09:19:24.122125 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/README.txt
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.122125 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/RTAComplete.txt
--rw-r--r--   0        0        0      755 2024-03-01 09:19:24.122125 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/RunInfo.xml
--rw-r--r--   0        0        0     2878 2024-03-01 09:19:24.122125 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/SampleSheet.csv
--rw-r--r--   0        0        0      928 2024-03-01 09:19:24.122125 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/SampleSheet_bcl2fastq.csv
--rw-r--r--   0        0        0     5359 2024-03-01 09:19:24.122125 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/runParameters.xml
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.122125 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/CopyComplete.txt
--rw-r--r--   0        0        0    27887 2024-03-01 09:19:24.122125 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/CorrectSampleSheet.csv
--rw-r--r--   0        0        0   141870 2024-03-01 09:19:24.122125 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/HLYWYDSXX_bcl2fastq_raw.json
--rwxr-xr-x   0        0        0   122682 2024-03-01 09:19:24.122125 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/HLYWYDSXX_bcl_convert_raw.json
--rw-r--r--   0        0        0      243 2024-03-01 09:19:24.122125 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/README.txt
--rw-r--r--   0        0        0    28230 2024-03-01 09:19:24.122125 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RTA3.cfg
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.122125 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RTAComplete.txt
--rw-r--r--   0        0        0    94426 2024-03-01 09:19:24.122125 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RunInfo.xml
--rw-r--r--   0        0        0     5819 2024-03-01 09:19:24.122125 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RunParameters.xml
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.122125 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/SequenceComplete.txt
--rw-r--r--   0        0        0     1757 2024-03-01 09:19:24.122125 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/HVKJCDRXX_demultiplex.stderr
--rw-r--r--   0        0        0     1757 2024-03-01 09:19:24.122125 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/HVKJCDRXX_demultiplex.stdout
--rw-r--r--   0        0        0       12 2024-03-01 09:19:24.122125 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/README.txt
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.122125 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/RTAComplete.txt
--rw-r--r--   0        0        0     5945 2024-03-01 09:19:24.122125 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/RunParameters.xml
--rw-r--r--   0        0        0      260 2024-03-01 09:19:24.122125 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/SampleSheet.csv
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.122125 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/copycomplete.txt
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.122125 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/demuxstarted.txt
--rw-r--r--   0        0        0     1757 2024-03-01 09:19:24.122125 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
--rw-r--r--   0        0        0     1757 2024-03-01 09:19:24.122125 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stdout
--rw-r--r--   0        0        0    47522 2024-03-01 09:19:24.122125 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_raw.json
--rw-r--r--   0        0        0       12 2024-03-01 09:19:24.122125 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/README.txt
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.122125 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/RTAComplete.txt
--rw-r--r--   0        0        0     6666 2024-03-01 09:19:24.122125 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/RunParameters.xml
--rw-r--r--   0        0        0      254 2024-03-01 09:19:24.122125 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/SampleSheet.csv
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.126124 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/copycomplete.txt
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.126124 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/delivery.txt
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.126124 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/demuxstarted.txt
--rwxr-xr-x   0        0        0    47434 2024-03-01 09:19:24.126124 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/22F52TLT3_raw.json
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.126124 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/CopyComplete.txt
--rw-r--r--   0        0        0    10950 2024-03-01 09:19:24.126124 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/CorrectSampleSheet.csv
--rw-r--r--   0        0        0      225 2024-03-01 09:19:24.126124 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/Manifest.tsv
--rw-r--r--   0        0        0       55 2024-03-01 09:19:24.126124 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/README.txt
--rwxr-xr-x   0        0        0     2493 2024-03-01 09:19:24.126124 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RTA.cfg
--rwxr-xr-x   0        0        0        1 2024-03-01 09:19:24.126124 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RTAComplete.txt
--rwxr-xr-x   0        0        0        2 2024-03-01 09:19:24.126124 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RTAExited.txt
--rwxr-xr-x   0        0        0      730 2024-03-01 09:19:24.126124 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunCompletionStatus.xml
--rwxr-xr-x   0        0        0    79277 2024-03-01 09:19:24.126124 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunInfo.xml
--rwxr-xr-x   0        0        0     2694 2024-03-01 09:19:24.126124 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunParameters.xml
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.126124 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/CopyComplete.txt
--rw-r--r--   0        0        0      509 2024-03-01 09:19:24.126124 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stderr
--rw-r--r--   0        0        0     2229 2024-03-01 09:19:24.126124 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stdout
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.126124 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/RTAComplete.txt
--rw-r--r--   0        0        0     6665 2024-03-01 09:19:24.126124 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/RunParameters.xml
--rw-r--r--   0        0        0      619 2024-03-01 09:19:24.126124 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/SampleSheet.csv
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.126124 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/CopyComplete.txt
--rw-r--r--   0        0        0      509 2024-03-01 09:19:24.126124 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stderr
--rw-r--r--   0        0        0     2229 2024-03-01 09:19:24.126124 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout
--rw-r--r--   0        0        0       12 2024-03-01 09:19:24.126124 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/README.txt
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.126124 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/RTAComplete.txt
--rw-r--r--   0        0        0     6665 2024-03-01 09:19:24.126124 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/RunParameters.xml
--rw-r--r--   0        0        0      399 2024-03-01 09:19:24.126124 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/SampleSheet.csv
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.126124 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/CopyComplete.txt
--rw-r--r--   0        0        0     4941 2024-03-01 09:19:24.126124 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/CorrectSampleSheet.csv
--rwxr-xr-x   0        0        0    20050 2024-03-01 09:19:24.126124 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/HK33MDRX3_bcl_convert_raw.json
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.126124 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/HK33MDRX3_demultiplex.stderr
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.126124 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/HK33MDRX3_demultiplex.stdout
--rw-r--r--   0        0        0      244 2024-03-01 09:19:24.126124 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/README.txt
--rw-r--r--   0        0        0     6391 2024-03-01 09:19:24.126124 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RTA3.cfg
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.126124 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RTAComplete.txt
--rw-r--r--   0        0        0    16428 2024-03-01 09:19:24.126124 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RunInfo.xml
--rw-r--r--   0        0        0     6728 2024-03-01 09:19:24.126124 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RunParameters.xml
--rw-r--r--   0        0        0     5127 2024-03-01 09:19:24.126124 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/SampleSheet.csv
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.126124 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/SequenceComplete.txt
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.126124 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/demuxstarted.txt
--rw-r--r--   0        0        0      124 2024-03-01 09:19:24.126124 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells_broken/180509_D00450_0598_BHGYFNBCX2/README.txt
--rw-r--r--   0        0        0      310 2024-03-01 09:19:24.126124 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells_broken/190927_A00689_0069_BHLYWYDSXX/README.txt
--rw-r--r--   0        0        0     5819 2024-03-01 09:19:24.126124 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells_broken/190927_A00689_0069_BHLYWYDSXX/RunParameters.xml
--rw-r--r--   0        0        0      122 2024-03-01 09:19:24.126124 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells_broken/20231108_LH00188_0028_B22F52TLT3/README.txt
--rwxr-xr-x   0        0        0     2694 2024-03-01 09:19:24.126124 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells_broken/20231108_LH00188_0028_B22F52TLT3/RunParameters.xml
--rw-r--r--   0        0        0      311 2024-03-01 09:19:24.126124 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells_broken/230912_A00187_1009_AHK33MDRX3/README.txt
--rw-r--r--   0        0        0     6728 2024-03-01 09:19:24.126124 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells_broken/230912_A00187_1009_AHK33MDRX3/RunParameters.xml
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.126124 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/CopyComplete.txt
--rw-r--r--   0        0        0      509 2024-03-01 09:19:24.126124 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stderr
--rw-r--r--   0        0        0     2229 2024-03-01 09:19:24.126124 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.126124 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/RTAComplete.txt
--rw-r--r--   0        0        0     6665 2024-03-01 09:19:24.126124 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/RunParameters.xml
--rw-r--r--   0        0        0      399 2024-03-01 09:19:24.126124 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/SampleSheet.csv
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.126124 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/CopyComplete.txt
--rw-r--r--   0        0        0      509 2024-03-01 09:19:24.126124 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stderr
--rw-r--r--   0        0        0     2229 2024-03-01 09:19:24.126124 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stdout
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.126124 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/RTAComplete.txt
--rw-r--r--   0        0        0     6665 2024-03-01 09:19:24.126124 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/RunParameters.xml
--rw-r--r--   0        0        0      399 2024-03-01 09:19:24.126124 cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/SampleSheet.csv
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.126124 cg-59.9.0/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_1/20231205_1618_3B_PAS86456_72d9fceb/fastq_pass/PAS86456_pass_72d9fceb_8a4fd683_0.fastq.gz
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.126124 cg-59.9.0/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_1/20231205_1618_3B_PAS86456_72d9fceb/fastq_pass/PAS86456_pass_72d9fceb_8a4fd683_1.fastq.gz
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.126124 cg-59.9.0/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_1/20231205_1618_3B_PAS86456_72d9fceb/final_summary_PAS86456_72d9fceb_8a4fd683.txt
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.126124 cg-59.9.0/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_1/20231205_1618_3B_PAS86456_72d9fceb/pod5_pass/PAS86456_pass_72d9fceb_8a4fd683_0.pod5
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.126124 cg-59.9.0/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_1/20231205_1618_3B_PAS86456_72d9fceb/pod5_pass/PAS86456_pass_72d9fceb_8a4fd683_1.pod5
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.126124 cg-59.9.0/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_2/20231205_1618_3D_PAS97781_595b5663/fastq_pass/PAS97781_pass_595b5663_efc7f02e_0.fastq.gz
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.126124 cg-59.9.0/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_2/20231205_1618_3D_PAS97781_595b5663/fastq_pass/PAS97781_pass_595b5663_efc7f02e_1.fastq.gz
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.126124 cg-59.9.0/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_2/20231205_1618_3D_PAS97781_595b5663/final_summary_PAS97781_595b5663_efc7f02e.txt
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.126124 cg-59.9.0/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_2/20231205_1618_3D_PAS97781_595b5663/pod5_pass/PAS97781_pass_595b5663_efc7f02e_0.pod5
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.126124 cg-59.9.0/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_2/20231205_1618_3D_PAS97781_595b5663/pod5_pass/PAS97781_pass_595b5663_efc7f02e_1.pod5
--rw-r--r--   0        0        0   111989 2024-03-01 09:19:24.126124 cg-59.9.0/tests/fixtures/apps/demultiplexing/raw_lims_samples/raw_samplesheet_novaseq.json
--rw-r--r--   0        0        0     5319 2024-03-01 09:19:24.126124 cg-59.9.0/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_hiseq_2500_different_index_cycles.xml
--rw-r--r--   0        0        0     5944 2024-03-01 09:19:24.126124 cg-59.9.0/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_6000_different_index_cycles.xml
--rwxr-xr-x   0        0        0     2481 2024-03-01 09:19:24.126124 cg-59.9.0/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_X_different_index_cycles.xml
--rwxr-xr-x   0        0        0     2474 2024-03-01 09:19:24.126124 cg-59.9.0/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_X_wrong_instrument.xml
--rw-r--r--   0        0        0     5899 2024-03-01 09:19:24.126124 cg-59.9.0/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_no_software_nor_reagent_version.xml
--rw-r--r--   0        0        0     4941 2024-03-01 09:19:24.126124 cg-59.9.0/tests/fixtures/apps/demultiplexing/sample_sheets/novaseq_6000_sample_sheet_with_reversed_cycles.csv
--rw-r--r--   0        0        0    10950 2024-03-01 09:19:24.130124 cg-59.9.0/tests/fixtures/apps/demultiplexing/sample_sheets/novaseq_x_sample_sheet_with_forward_cycles.csv
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.130124 cg-59.9.0/tests/fixtures/apps/demultiplexing/spring/dummy_run_001.spring
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.130124 cg-59.9.0/tests/fixtures/apps/demultiplexing/spring/dummy_run_002.spring
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.130124 cg-59.9.0/tests/fixtures/apps/demultiplexing/spring/dummy_spring_meta_data.json
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.130124 cg-59.9.0/tests/fixtures/apps/fluffy/2020-23219-05/2020-23219-05.WCXpredict_aberrations.filt.bed
--rw-r--r--   0        0        0     5554 2024-03-01 09:19:24.130124 cg-59.9.0/tests/fixtures/apps/fluffy/SampleSheet.csv
--rw-r--r--   0        0        0      901 2024-03-01 09:19:24.130124 cg-59.9.0/tests/fixtures/apps/fluffy/deliverables.yaml
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.130124 cg-59.9.0/tests/fixtures/apps/fluffy/fluffy_fastq.fastq.gz
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.130124 cg-59.9.0/tests/fixtures/apps/fluffy/multiqc_report.html
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.130124 cg-59.9.0/tests/fixtures/apps/fluffy/summary.csv
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.130124 cg-59.9.0/tests/fixtures/apps/gt/yellowhog.bcf
--rw-r--r--   0        0        0     5114 2024-03-01 09:19:24.130124 cg-59.9.0/tests/fixtures/apps/madeline/madeline.xml
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.130124 cg-59.9.0/tests/fixtures/apps/mip/case_file.txt
--rw-r--r--   0        0        0     3241 2024-03-01 09:19:24.130124 cg-59.9.0/tests/fixtures/apps/mip/case_metrics_deliverables.yaml
--rw-r--r--   0        0        0    21811 2024-03-01 09:19:24.130124 cg-59.9.0/tests/fixtures/apps/mip/dna/store/case_config.yaml
--rw-r--r--   0        0        0    23364 2024-03-01 09:19:24.130124 cg-59.9.0/tests/fixtures/apps/mip/dna/store/case_id_deliverables.yaml
--rw-r--r--   0        0        0    37367 2024-03-01 09:19:24.130124 cg-59.9.0/tests/fixtures/apps/mip/dna/store/case_qc_sample_info.yaml
--rw-r--r--   0        0        0       16 2024-03-01 09:19:24.130124 cg-59.9.0/tests/fixtures/apps/mip/dna/store/empty_case_config.yaml
--rw-r--r--   0        0        0       16 2024-03-01 09:19:24.130124 cg-59.9.0/tests/fixtures/apps/mip/dna/store/empty_case_metrics_deliverables.yaml
--rw-r--r--   0        0        0       16 2024-03-01 09:19:24.130124 cg-59.9.0/tests/fixtures/apps/mip/dna/store/empty_case_qc_sample_info.yaml
--rw-r--r--   0        0        0      123 2024-03-01 09:19:24.130124 cg-59.9.0/tests/fixtures/apps/mip/dna/store/empty_delivery_report.html
--rw-r--r--   0        0        0    62741 2024-03-01 09:19:24.130124 cg-59.9.0/tests/fixtures/apps/mip/dna/store/yellowhog_clinical_selected.vcf
--rw-r--r--   0        0        0    11242 2024-03-01 09:19:24.130124 cg-59.9.0/tests/fixtures/apps/mip/rna/case_config.yaml
--rw-r--r--   0        0        0    12164 2024-03-01 09:19:24.130124 cg-59.9.0/tests/fixtures/apps/mip/rna/case_qc_sampleinfo.yaml
--rw-r--r--   0        0        0     5231 2024-03-01 09:19:24.130124 cg-59.9.0/tests/fixtures/apps/mip/rna/store/bundle_data.yaml
--rw-r--r--   0        0        0     9774 2024-03-01 09:19:24.130124 cg-59.9.0/tests/fixtures/apps/mip/rna/store/case_config.yaml
--rw-r--r--   0        0        0     4624 2024-03-01 09:19:24.130124 cg-59.9.0/tests/fixtures/apps/mip/rna/store/case_id_deliverables.yaml
--rw-r--r--   0        0        0    13666 2024-03-01 09:19:24.130124 cg-59.9.0/tests/fixtures/apps/mip/rna/store/case_qc_sample_info.yaml
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.130124 cg-59.9.0/tests/fixtures/apps/mip/sample_file.txt
--rw-r--r--   0        0        0     1885 2024-03-01 09:19:24.130124 cg-59.9.0/tests/fixtures/apps/scout/643594.config.yaml
--rw-r--r--   0        0        0     6027 2024-03-01 09:19:24.130124 cg-59.9.0/tests/fixtures/apps/scout/case_export.json
--rw-r--r--   0        0        0     9349 2024-03-01 09:19:24.130124 cg-59.9.0/tests/fixtures/apps/scout/export_causatives.json
--rw-r--r--   0        0        0     1315 2024-03-01 09:19:24.130124 cg-59.9.0/tests/fixtures/apps/scout/none_case_export.json
--rw-r--r--   0        0        0     3518 2024-03-01 09:19:24.130124 cg-59.9.0/tests/fixtures/apps/scout/other_sex_case.json
--rw-r--r--   0        0        0     8874 2024-03-01 09:19:24.130124 cg-59.9.0/tests/fixtures/apps/scout/panel_export.bed
--rw-r--r--   0        0        0     4169 2024-03-01 09:19:24.130124 cg-59.9.0/tests/fixtures/apps/scout/panel_export.csv
--rw-r--r--   0        0        0    63569 2024-03-01 09:19:24.130124 cg-59.9.0/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Adapter_Metrics.csv
--rw-r--r--   0        0        0    42478 2024-03-01 09:19:24.130124 cg-59.9.0/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Demultiplex_Stats.csv
--rw-r--r--   0        0        0    69708 2024-03-01 09:19:24.130124 cg-59.9.0/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Quality_Metrics.csv
--rw-r--r--   0        0        0      582 2024-03-01 09:19:24.130124 cg-59.9.0/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/SampleSheet.csv
--rw-r--r--   0        0        0       42 2024-03-01 09:19:24.130124 cg-59.9.0/tests/fixtures/apps/shipping/scout-deploy.yaml
--rw-r--r--   0        0        0     1036 2024-03-01 09:19:24.130124 cg-59.9.0/tests/fixtures/cgweb_orders/balsamic.json
--rw-r--r--   0        0        0     1104 2024-03-01 09:19:24.130124 cg-59.9.0/tests/fixtures/cgweb_orders/fastq.json
--rw-r--r--   0        0        0     1313 2024-03-01 09:19:24.130124 cg-59.9.0/tests/fixtures/cgweb_orders/metagenome.json
--rw-r--r--   0        0        0     3038 2024-03-01 09:19:24.130124 cg-59.9.0/tests/fixtures/cgweb_orders/microsalt.json
--rw-r--r--   0        0        0     3705 2024-03-01 09:19:24.130124 cg-59.9.0/tests/fixtures/cgweb_orders/mip.json
--rw-r--r--   0        0        0     1364 2024-03-01 09:19:24.130124 cg-59.9.0/tests/fixtures/cgweb_orders/mip_rna.json
--rw-r--r--   0        0        0     2125 2024-03-01 09:19:24.130124 cg-59.9.0/tests/fixtures/cgweb_orders/rml.json
--rw-r--r--   0        0        0     1368 2024-03-01 09:19:24.130124 cg-59.9.0/tests/fixtures/cgweb_orders/rnafusion.json
--rw-r--r--   0        0        0     4684 2024-03-01 09:19:24.130124 cg-59.9.0/tests/fixtures/cgweb_orders/sarscov2.json
--rw-r--r--   0        0        0     5609 2024-03-01 09:19:24.130124 cg-59.9.0/tests/fixtures/data/SampleSheet.csv
--rw-r--r--   0        0        0      511 2024-03-01 09:19:24.130124 cg-59.9.0/tests/fixtures/data/bcl_convert_sample_sheet.csv
--rw-r--r--   0        0        0   258048 2024-03-01 09:19:24.134125 cg-59.9.0/tests/fixtures/data/cgfixture.db
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.134125 cg-59.9.0/tests/fixtures/data/fastq.fastq.gz
--rw-r--r--   0        0        0    49152 2024-03-01 09:19:24.134125 cg-59.9.0/tests/fixtures/data/hkstore.db
--rw-r--r--   0        0        0       73 2024-03-01 09:19:24.134125 cg-59.9.0/tests/fixtures/data/yellowhog/pedigree.yaml
--rw-r--r--   0        0        0       76 2024-03-01 09:19:24.134125 cg-59.9.0/tests/fixtures/io/casava_five_parts.fastq.gz
--rw-r--r--   0        0        0       90 2024-03-01 09:19:24.134125 cg-59.9.0/tests/fixtures/io/casava_seven_parts.fastq.gz
--rw-r--r--   0        0        0       96 2024-03-01 09:19:24.134125 cg-59.9.0/tests/fixtures/io/casava_ten_parts.fastq.gz
--rw-r--r--   0        0        0      153 2024-03-01 09:19:24.134125 cg-59.9.0/tests/fixtures/io/example.csv
--rw-r--r--   0        0        0       46 2024-03-01 09:19:24.134125 cg-59.9.0/tests/fixtures/io/example.gz
--rw-r--r--   0        0        0      147 2024-03-01 09:19:24.134125 cg-59.9.0/tests/fixtures/io/example.tsv
--rw-r--r--   0        0        0       20 2024-03-01 09:19:24.134125 cg-59.9.0/tests/fixtures/io/example.txt
--rw-r--r--   0        0        0      582 2024-03-01 09:19:24.134125 cg-59.9.0/tests/fixtures/io/example_json.json
--rw-r--r--   0        0        0      103 2024-03-01 09:19:24.134125 cg-59.9.0/tests/fixtures/io/example_xml.xml
--rw-r--r--   0        0        0       20 2024-03-01 09:19:24.134125 cg-59.9.0/tests/fixtures/meta/qc_metrics/file_with_right_tags.json
--rw-r--r--   0        0        0       20 2024-03-01 09:19:24.134125 cg-59.9.0/tests/fixtures/meta/qc_metrics/file_without_right_tags.json
--rw-r--r--   0        0        0   156910 2024-03-01 09:19:24.134125 cg-59.9.0/tests/fixtures/orderforms/1508.30.balsamic.xlsx
--rw-r--r--   0        0        0   156770 2024-03-01 09:19:24.134125 cg-59.9.0/tests/fixtures/orderforms/1508.30.balsamic_qc.xlsx
--rw-r--r--   0        0        0   156737 2024-03-01 09:19:24.134125 cg-59.9.0/tests/fixtures/orderforms/1508.30.balsamic_umi.xlsx
--rw-r--r--   0        0        0   156582 2024-03-01 09:19:24.134125 cg-59.9.0/tests/fixtures/orderforms/1508.30.fastq.xlsx
--rw-r--r--   0        0        0   155627 2024-03-01 09:19:24.138125 cg-59.9.0/tests/fixtures/orderforms/1508.30.metagenome.xlsx
--rw-r--r--   0        0        0   156850 2024-03-01 09:19:24.138125 cg-59.9.0/tests/fixtures/orderforms/1508.30.mip.xlsx
--rw-r--r--   0        0        0   258580 2024-03-01 09:19:24.138125 cg-59.9.0/tests/fixtures/orderforms/1508.30.mip_rna.xlsx
--rw-r--r--   0        0        0   258342 2024-03-01 09:19:24.138125 cg-59.9.0/tests/fixtures/orderforms/1508.30.rnafusion.xlsx
--rw-r--r--   0        0        0    82677 2024-03-01 09:19:24.138125 cg-59.9.0/tests/fixtures/orderforms/1603.11.microbial.xlsx
--rw-r--r--   0        0        0   149394 2024-03-01 09:19:24.138125 cg-59.9.0/tests/fixtures/orderforms/1604.17.rml.xlsx
--rw-r--r--   0        0        0   227887 2024-03-01 09:19:24.142125 cg-59.9.0/tests/fixtures/orderforms/2184.8.sarscov2.xlsx
--rw-r--r--   0        0        0    18639 2024-03-01 09:19:24.142125 cg-59.9.0/tests/fixtures/orderforms/NIPT-json.json
--rw-r--r--   0        0        0     6052 2024-03-01 09:19:24.142125 cg-59.9.0/tests/fixtures/orderforms/balsamic_uploaded_json_orderform.json
--rw-r--r--   0        0        0     6611 2024-03-01 09:19:24.142125 cg-59.9.0/tests/fixtures/orderforms/mip_uploaded_json_orderform.json
--rw-r--r--   0        0        0     1417 2024-03-01 09:19:24.142125 cg-59.9.0/tests/fixtures/report/case_data.json
--rw-r--r--   0        0        0     1109 2024-03-01 09:19:24.142125 cg-59.9.0/tests/fixtures/report/lims_exported_samples.json
--rw-r--r--   0        0        0     1562 2024-03-01 09:19:24.142125 cg-59.9.0/tests/fixtures/report/lims_family.json
--rw-r--r--   0        0        0     2948 2024-03-01 09:19:24.142125 cg-59.9.0/tests/io/conftest.py
--rw-r--r--   0        0        0     8639 2024-03-01 09:19:24.142125 cg-59.9.0/tests/io/test_io_controller.py
--rw-r--r--   0        0        0     3877 2024-03-01 09:19:24.142125 cg-59.9.0/tests/io/test_io_csv.py
--rw-r--r--   0        0        0      482 2024-03-01 09:19:24.142125 cg-59.9.0/tests/io/test_io_gzip.py
--rw-r--r--   0        0        0     1779 2024-03-01 09:19:24.142125 cg-59.9.0/tests/io/test_io_json.py
--rw-r--r--   0        0        0     1828 2024-03-01 09:19:24.142125 cg-59.9.0/tests/io/test_io_txt.py
--rw-r--r--   0        0        0     1027 2024-03-01 09:19:24.142125 cg-59.9.0/tests/io/test_io_xml.py
--rw-r--r--   0        0        0     2131 2024-03-01 09:19:24.142125 cg-59.9.0/tests/io/test_io_yaml.py
--rw-r--r--   0        0        0     1233 2024-03-01 09:19:24.142125 cg-59.9.0/tests/io/test_validate_path.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.142125 cg-59.9.0/tests/meta/__init__.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.142125 cg-59.9.0/tests/meta/archive/__init__.py
--rw-r--r--   0        0        0    13131 2024-03-01 09:19:24.142125 cg-59.9.0/tests/meta/archive/conftest.py
--rw-r--r--   0        0        0    16858 2024-03-01 09:19:24.142125 cg-59.9.0/tests/meta/archive/test_archive_api.py
--rw-r--r--   0        0        0    10246 2024-03-01 09:19:24.142125 cg-59.9.0/tests/meta/archive/test_archive_cli.py
--rw-r--r--   0        0        0    15766 2024-03-01 09:19:24.142125 cg-59.9.0/tests/meta/archive/test_archiving.py
--rw-r--r--   0        0        0     3807 2024-03-01 09:19:24.142125 cg-59.9.0/tests/meta/backup/conftest.py
--rw-r--r--   0        0        0    26536 2024-03-01 09:19:24.142125 cg-59.9.0/tests/meta/backup/test_meta_backup.py
--rw-r--r--   0        0        0    10055 2024-03-01 09:19:24.142125 cg-59.9.0/tests/meta/backup/test_meta_pdc.py
--rw-r--r--   0        0        0    12654 2024-03-01 09:19:24.142125 cg-59.9.0/tests/meta/clean/conftest.py
--rw-r--r--   0        0        0    16961 2024-03-01 09:19:24.142125 cg-59.9.0/tests/meta/clean/test_clean_flow_cells_api.py
--rw-r--r--   0        0        0     2286 2024-03-01 09:19:24.142125 cg-59.9.0/tests/meta/clean/test_clean_retrieved_spring_files.py
--rw-r--r--   0        0        0     7691 2024-03-01 09:19:24.142125 cg-59.9.0/tests/meta/compress/conftest.py
--rw-r--r--   0        0        0     7961 2024-03-01 09:19:24.142125 cg-59.9.0/tests/meta/compress/test_clean_fastq.py
--rw-r--r--   0        0        0     1778 2024-03-01 09:19:24.142125 cg-59.9.0/tests/meta/compress/test_compress_files.py
--rw-r--r--   0        0        0     3644 2024-03-01 09:19:24.142125 cg-59.9.0/tests/meta/compress/test_compress_meta_fastq.py
--rw-r--r--   0        0        0     1180 2024-03-01 09:19:24.142125 cg-59.9.0/tests/meta/compress/test_decompress_spring_meta.py
--rw-r--r--   0        0        0     6902 2024-03-01 09:19:24.142125 cg-59.9.0/tests/meta/compress/test_meta_compress_update_hk.py
--rw-r--r--   0        0        0     8207 2024-03-01 09:19:24.142125 cg-59.9.0/tests/meta/conftest.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.142125 cg-59.9.0/tests/meta/deliver/__init__.py
--rw-r--r--   0        0        0     3471 2024-03-01 09:19:24.142125 cg-59.9.0/tests/meta/deliver/conftest.py
--rw-r--r--   0        0        0     8874 2024-03-01 09:19:24.142125 cg-59.9.0/tests/meta/deliver/test_deliver_ticket.py
--rw-r--r--   0        0        0    10277 2024-03-01 09:19:24.142125 cg-59.9.0/tests/meta/deliver/test_delivery_api.py
--rw-r--r--   0        0        0    13489 2024-03-01 09:19:24.142125 cg-59.9.0/tests/meta/demultiplex/conftest.py
--rw-r--r--   0        0        0     5382 2024-03-01 09:19:24.142125 cg-59.9.0/tests/meta/demultiplex/test_combine_sequencing_metrics.py
--rw-r--r--   0        0        0    10786 2024-03-01 09:19:24.142125 cg-59.9.0/tests/meta/demultiplex/test_demux_post_processing.py
--rw-r--r--   0        0        0    12330 2024-03-01 09:19:24.142125 cg-59.9.0/tests/meta/demultiplex/test_housekeeper_storage_functions.py
--rw-r--r--   0        0        0     5219 2024-03-01 09:19:24.142125 cg-59.9.0/tests/meta/demultiplex/test_status_db_storage_functions.py
--rw-r--r--   0        0        0    22708 2024-03-01 09:19:24.142125 cg-59.9.0/tests/meta/demultiplex/test_utils.py
--rw-r--r--   0        0        0     6193 2024-03-01 09:19:24.142125 cg-59.9.0/tests/meta/demultiplex/test_validation.py
--rw-r--r--   0        0        0     4943 2024-03-01 09:19:24.142125 cg-59.9.0/tests/meta/encryption/conftest.py
--rw-r--r--   0        0        0    18133 2024-03-01 09:19:24.142125 cg-59.9.0/tests/meta/encryption/test_encryption.py
--rw-r--r--   0        0        0     3122 2024-03-01 09:19:24.142125 cg-59.9.0/tests/meta/observations/conftest.py
--rw-r--r--   0        0        0    16164 2024-03-01 09:19:24.142125 cg-59.9.0/tests/meta/observations/test_meta_upload_observations.py
--rw-r--r--   0        0        0     4974 2024-03-01 09:19:24.142125 cg-59.9.0/tests/meta/orders/conftest.py
--rw-r--r--   0        0        0     1749 2024-03-01 09:19:24.142125 cg-59.9.0/tests/meta/orders/test_PoolSubmitter_validate_order.py
--rw-r--r--   0        0        0     1470 2024-03-01 09:19:24.142125 cg-59.9.0/tests/meta/orders/test_SarsCov2Submitter_order_to_status.py
--rw-r--r--   0        0        0     1768 2024-03-01 09:19:24.142125 cg-59.9.0/tests/meta/orders/test_SarsCov2Submitter_store_order.py
--rw-r--r--   0        0        0     2032 2024-03-01 09:19:24.142125 cg-59.9.0/tests/meta/orders/test_SarsCov2Submitter_validate_order.py
--rw-r--r--   0        0        0    19783 2024-03-01 09:19:24.142125 cg-59.9.0/tests/meta/orders/test_meta_orders_api.py
--rw-r--r--   0        0        0     7083 2024-03-01 09:19:24.142125 cg-59.9.0/tests/meta/orders/test_meta_orders_lims.py
--rw-r--r--   0        0        0    29515 2024-03-01 09:19:24.142125 cg-59.9.0/tests/meta/orders/test_meta_orders_status.py
--rw-r--r--   0        0        0     1677 2024-03-01 09:19:24.142125 cg-59.9.0/tests/meta/orders/test_rnafusion_submitter.py
--rw-r--r--   0        0        0     1068 2024-03-01 09:19:24.142125 cg-59.9.0/tests/meta/orders/test_ticket_handler.py
--rw-r--r--   0        0        0     3907 2024-03-01 09:19:24.142125 cg-59.9.0/tests/meta/qc_metrics/conftest.py
--rw-r--r--   0        0        0     1247 2024-03-01 09:19:24.142125 cg-59.9.0/tests/meta/qc_metrics/test_collect_qc_metrics.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.146124 cg-59.9.0/tests/meta/report/__init__.py
--rw-r--r--   0        0        0     5354 2024-03-01 09:19:24.146124 cg-59.9.0/tests/meta/report/conftest.py
--rw-r--r--   0        0        0      434 2024-03-01 09:19:24.146124 cg-59.9.0/tests/meta/report/helper.py
--rw-r--r--   0        0        0     4106 2024-03-01 09:19:24.146124 cg-59.9.0/tests/meta/report/test_balsamic_api.py
--rw-r--r--   0        0        0     4056 2024-03-01 09:19:24.146124 cg-59.9.0/tests/meta/report/test_field_validators.py
--rw-r--r--   0        0        0     2834 2024-03-01 09:19:24.146124 cg-59.9.0/tests/meta/report/test_mip_dna_api.py
--rw-r--r--   0        0        0    16698 2024-03-01 09:19:24.146124 cg-59.9.0/tests/meta/report/test_report_api.py
--rw-r--r--   0        0        0     2546 2024-03-01 09:19:24.146124 cg-59.9.0/tests/meta/report/test_rnafusion_api.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.146124 cg-59.9.0/tests/meta/rsync/__init__.py
--rw-r--r--   0        0        0      916 2024-03-01 09:19:24.146124 cg-59.9.0/tests/meta/rsync/conftest.py
--rw-r--r--   0        0        0     9442 2024-03-01 09:19:24.146124 cg-59.9.0/tests/meta/rsync/test_rsync.py
--rw-r--r--   0        0        0     3147 2024-03-01 09:19:24.146124 cg-59.9.0/tests/meta/test_invoice.py
--rw-r--r--   0        0        0     1787 2024-03-01 09:19:24.146124 cg-59.9.0/tests/meta/transfer/conftest.py
--rw-r--r--   0        0        0     9995 2024-03-01 09:19:24.146124 cg-59.9.0/tests/meta/transfer/test_external_data.py
--rw-r--r--   0        0        0     4395 2024-03-01 09:19:24.146124 cg-59.9.0/tests/meta/transfer/test_meta_transfer_lims.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.146124 cg-59.9.0/tests/meta/upload/__init__.py
--rw-r--r--   0        0        0     2210 2024-03-01 09:19:24.146124 cg-59.9.0/tests/meta/upload/balsamic/test_balsamic.py
--rw-r--r--   0        0        0     4002 2024-03-01 09:19:24.146124 cg-59.9.0/tests/meta/upload/conftest.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.146124 cg-59.9.0/tests/meta/upload/gisaid/__init__.py
--rw-r--r--   0        0        0     2557 2024-03-01 09:19:24.146124 cg-59.9.0/tests/meta/upload/gisaid/fixtures/four_samples.csv
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.146124 cg-59.9.0/tests/meta/upload/gisaid/fixtures/invalid_housekeeper.fasta
--rw-r--r--   0        0        0      211 2024-03-01 09:19:24.146124 cg-59.9.0/tests/meta/upload/gisaid/fixtures/valid_gisaid.fasta
--rw-r--r--   0        0        0      371 2024-03-01 09:19:24.146124 cg-59.9.0/tests/meta/upload/gisaid/fixtures/valid_housekeeper.fasta
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.146124 cg-59.9.0/tests/meta/upload/mutacc/__init__.py
--rw-r--r--   0        0        0     3684 2024-03-01 09:19:24.146124 cg-59.9.0/tests/meta/upload/mutacc/conftest.py
--rw-r--r--   0        0        0     4188 2024-03-01 09:19:24.146124 cg-59.9.0/tests/meta/upload/mutacc/test_meta_upload_mutacc.py
--rw-r--r--   0        0        0     1149 2024-03-01 09:19:24.146124 cg-59.9.0/tests/meta/upload/nipt/conftest.py
--rw-r--r--   0        0        0     1683 2024-03-01 09:19:24.146124 cg-59.9.0/tests/meta/upload/nipt/test_models.py
--rw-r--r--   0        0        0     1242 2024-03-01 09:19:24.146124 cg-59.9.0/tests/meta/upload/nipt/test_nipt_upload_api.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.146124 cg-59.9.0/tests/meta/upload/scout/__init__.py
--rw-r--r--   0        0        0    24071 2024-03-01 09:19:24.146124 cg-59.9.0/tests/meta/upload/scout/conftest.py
--rw-r--r--   0        0        0     4734 2024-03-01 09:19:24.146124 cg-59.9.0/tests/meta/upload/scout/test_generate_load_config.py
--rw-r--r--   0        0        0     4182 2024-03-01 09:19:24.146124 cg-59.9.0/tests/meta/upload/scout/test_meta_upload_scoutapi.py
--rw-r--r--   0        0        0    33260 2024-03-01 09:19:24.146124 cg-59.9.0/tests/meta/upload/scout/test_meta_upload_scoutapi_rna.py
--rw-r--r--   0        0        0     7372 2024-03-01 09:19:24.146124 cg-59.9.0/tests/meta/upload/scout/test_scout_config_builder.py
--rw-r--r--   0        0        0     2511 2024-03-01 09:19:24.146124 cg-59.9.0/tests/meta/upload/test_meta_upload_coverage.py
--rw-r--r--   0        0        0     1473 2024-03-01 09:19:24.146124 cg-59.9.0/tests/meta/upload/test_upload_api.py
--rw-r--r--   0        0        0     2547 2024-03-01 09:19:24.146124 cg-59.9.0/tests/meta/upload/test_upload_genotypes_api.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.146124 cg-59.9.0/tests/meta/workflow/__init__.py
--rw-r--r--   0        0        0    10066 2024-03-01 09:19:24.146124 cg-59.9.0/tests/meta/workflow/conftest.py
--rw-r--r--   0        0        0     3652 2024-03-01 09:19:24.146124 cg-59.9.0/tests/meta/workflow/microsalt/conftest.py
--rw-r--r--   0        0        0      318 2024-03-01 09:19:24.146124 cg-59.9.0/tests/meta/workflow/microsalt/test_parsing_metrics.py
--rw-r--r--   0        0        0     3714 2024-03-01 09:19:24.146124 cg-59.9.0/tests/meta/workflow/microsalt/test_quality_controller.py
--rw-r--r--   0        0        0    14367 2024-03-01 09:19:24.146124 cg-59.9.0/tests/meta/workflow/microsalt/test_quality_controller_utils.py
--rw-r--r--   0        0        0      825 2024-03-01 09:19:24.146124 cg-59.9.0/tests/meta/workflow/microsalt/test_report_generation.py
--rw-r--r--   0        0        0    20886 2024-03-01 09:19:24.146124 cg-59.9.0/tests/meta/workflow/test_analysis.py
--rw-r--r--   0        0        0     6190 2024-03-01 09:19:24.146124 cg-59.9.0/tests/meta/workflow/test_balsamic.py
--rw-r--r--   0        0        0     3034 2024-03-01 09:19:24.146124 cg-59.9.0/tests/meta/workflow/test_fastq.py
--rw-r--r--   0        0        0     1532 2024-03-01 09:19:24.146124 cg-59.9.0/tests/meta/workflow/test_microsalt.py
--rw-r--r--   0        0        0     3123 2024-03-01 09:19:24.146124 cg-59.9.0/tests/meta/workflow/test_nf_analysis.py
--rw-r--r--   0        0        0     7741 2024-03-01 09:19:24.146124 cg-59.9.0/tests/meta/workflow/test_prepare_fastq_api.py
--rw-r--r--   0        0        0     1688 2024-03-01 09:19:24.146124 cg-59.9.0/tests/meta/workflow/test_rnafusion.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.146124 cg-59.9.0/tests/mocks/__init__.py
--rw-r--r--   0        0        0     1161 2024-03-01 09:19:24.146124 cg-59.9.0/tests/mocks/balsamic_analysis_mock.py
--rw-r--r--   0        0        0     3500 2024-03-01 09:19:24.146124 cg-59.9.0/tests/mocks/crunchy.py
--rw-r--r--   0        0        0    21569 2024-03-01 09:19:24.146124 cg-59.9.0/tests/mocks/hk_mock.py
--rw-r--r--   0        0        0     3802 2024-03-01 09:19:24.146124 cg-59.9.0/tests/mocks/limsmock.py
--rw-r--r--   0        0        0      572 2024-03-01 09:19:24.146124 cg-59.9.0/tests/mocks/madeline.py
--rw-r--r--   0        0        0     1297 2024-03-01 09:19:24.146124 cg-59.9.0/tests/mocks/mip_analysis_mock.py
--rw-r--r--   0        0        0     1525 2024-03-01 09:19:24.146124 cg-59.9.0/tests/mocks/osticket.py
--rw-r--r--   0        0        0     3239 2024-03-01 09:19:24.146124 cg-59.9.0/tests/mocks/process_mock.py
--rw-r--r--   0        0        0     3718 2024-03-01 09:19:24.146124 cg-59.9.0/tests/mocks/report.py
--rw-r--r--   0        0        0     3915 2024-03-01 09:19:24.146124 cg-59.9.0/tests/mocks/scout.py
--rw-r--r--   0        0        0      750 2024-03-01 09:19:24.146124 cg-59.9.0/tests/mocks/store_model.py
--rw-r--r--   0        0        0     1532 2024-03-01 09:19:24.146124 cg-59.9.0/tests/mocks/tb_mock.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.146124 cg-59.9.0/tests/models/__init__.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.146124 cg-59.9.0/tests/models/balsamic/__init__.py
--rw-r--r--   0        0        0     1194 2024-03-01 09:19:24.146124 cg-59.9.0/tests/models/balsamic/conftest.py
--rw-r--r--   0        0        0     1030 2024-03-01 09:19:24.146124 cg-59.9.0/tests/models/balsamic/test_balsamic_analysis.py
--rw-r--r--   0        0        0     1050 2024-03-01 09:19:24.146124 cg-59.9.0/tests/models/conftest.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.146124 cg-59.9.0/tests/models/demultiplexing/__init__.py
--rw-r--r--   0        0        0      284 2024-03-01 09:19:24.146124 cg-59.9.0/tests/models/demultiplexing/conftest.py
--rw-r--r--   0        0        0    11446 2024-03-01 09:19:24.146124 cg-59.9.0/tests/models/demultiplexing/test_run_parameters.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.146124 cg-59.9.0/tests/models/downsample/__init__.py
--rw-r--r--   0        0        0     2096 2024-03-01 09:19:24.146124 cg-59.9.0/tests/models/downsample/test_down_sample_meta_data.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.146124 cg-59.9.0/tests/models/flow_cell/__init__.py
--rw-r--r--   0        0        0     8715 2024-03-01 09:19:24.146124 cg-59.9.0/tests/models/flow_cell/test_flowcell_model.py
--rw-r--r--   0        0        0     6637 2024-03-01 09:19:24.146124 cg-59.9.0/tests/models/mip/conftest.py
--rw-r--r--   0        0        0     1239 2024-03-01 09:19:24.150124 cg-59.9.0/tests/models/mip/test_mip_analysis.py
--rw-r--r--   0        0        0     2348 2024-03-01 09:19:24.150124 cg-59.9.0/tests/models/mip/test_mip_config.py
--rw-r--r--   0        0        0     6392 2024-03-01 09:19:24.150124 cg-59.9.0/tests/models/mip/test_mip_metrics_deliverables.py
--rw-r--r--   0        0        0     3959 2024-03-01 09:19:24.150124 cg-59.9.0/tests/models/mip/test_mip_sample_info.py
--rw-r--r--   0        0        0     3314 2024-03-01 09:19:24.150124 cg-59.9.0/tests/models/nextflow/test_nextflow_deliver.py
--rw-r--r--   0        0        0     1602 2024-03-01 09:19:24.150124 cg-59.9.0/tests/models/observations/conftest.py
--rw-r--r--   0        0        0     2579 2024-03-01 09:19:24.150124 cg-59.9.0/tests/models/observations/test_observations_input_files.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.150124 cg-59.9.0/tests/models/report/__init__.py
--rw-r--r--   0        0        0     6722 2024-03-01 09:19:24.150124 cg-59.9.0/tests/models/report/test_validators.py
--rw-r--r--   0        0        0     3855 2024-03-01 09:19:24.150124 cg-59.9.0/tests/models/rnafusion/test_rnafusion_sample.py
--rw-r--r--   0        0        0     1374 2024-03-01 09:19:24.150124 cg-59.9.0/tests/models/test_cg_models.py
--rw-r--r--   0        0        0      990 2024-03-01 09:19:24.150124 cg-59.9.0/tests/models/test_compression_data.py
--rw-r--r--   0        0        0      729 2024-03-01 09:19:24.150124 cg-59.9.0/tests/models/test_fastq.py
--rw-r--r--   0        0        0     2860 2024-03-01 09:19:24.150124 cg-59.9.0/tests/models/test_file_data.py
--rw-r--r--   0        0        0     3114 2024-03-01 09:19:24.150124 cg-59.9.0/tests/server/conftest.py
--rw-r--r--   0        0        0      509 2024-03-01 09:19:24.150124 cg-59.9.0/tests/server/endpoints/test_delivery_message_endpoint.py
--rw-r--r--   0        0        0     2943 2024-03-01 09:19:24.150124 cg-59.9.0/tests/server/endpoints/test_orders_endpoint.py
--rw-r--r--   0        0        0      271 2024-03-01 09:19:24.150124 cg-59.9.0/tests/server/test_server_auto.py
--rw-r--r--   0        0        0     1047 2024-03-01 09:19:24.150124 cg-59.9.0/tests/services/fastq_file_service/conftest.py
--rw-r--r--   0        0        0     3435 2024-03-01 09:19:24.150124 cg-59.9.0/tests/services/fastq_file_service/test_fastq_file_service.py
--rw-r--r--   0        0        0     1055 2024-03-01 09:19:24.150124 cg-59.9.0/tests/services/orders/order_status_service/conftest.py
--rw-r--r--   0        0        0      872 2024-03-01 09:19:24.150124 cg-59.9.0/tests/services/orders/order_status_service/test_order_status_service.py
--rw-r--r--   0        0        0      318 2024-03-01 09:19:24.150124 cg-59.9.0/tests/small_helpers.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.150124 cg-59.9.0/tests/store/__init__.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.150124 cg-59.9.0/tests/store/api/__init__.py
--rw-r--r--   0        0        0     2981 2024-03-01 09:19:24.150124 cg-59.9.0/tests/store/api/conftest.py
--rw-r--r--   0        0        0     1557 2024-03-01 09:19:24.150124 cg-59.9.0/tests/store/api/test_base.py
--rw-r--r--   0        0        0    20311 2024-03-01 09:19:24.150124 cg-59.9.0/tests/store/conftest.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.150124 cg-59.9.0/tests/store/crud/__init__.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.150124 cg-59.9.0/tests/store/crud/add/__init__.py
--rw-r--r--   0        0        0     1497 2024-03-01 09:19:24.150124 cg-59.9.0/tests/store/crud/add/test_store_add_application_version.py
--rw-r--r--   0        0        0     3958 2024-03-01 09:19:24.150124 cg-59.9.0/tests/store/crud/add/test_store_add_base.py
--rw-r--r--   0        0        0     2502 2024-03-01 09:19:24.150124 cg-59.9.0/tests/store/crud/add/test_store_add_customer.py
--rw-r--r--   0        0        0     1640 2024-03-01 09:19:24.150124 cg-59.9.0/tests/store/crud/add/test_store_add_flow_celll.py
--rw-r--r--   0        0        0    12209 2024-03-01 09:19:24.150124 cg-59.9.0/tests/store/crud/conftest.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.150124 cg-59.9.0/tests/store/crud/delete/__init__.py
--rw-r--r--   0        0        0     5541 2024-03-01 09:19:24.150124 cg-59.9.0/tests/store/crud/delete/test_delete.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.150124 cg-59.9.0/tests/store/crud/read/__init__.py
--rw-r--r--   0        0        0    57211 2024-03-01 09:19:24.150124 cg-59.9.0/tests/store/crud/read/test_read.py
--rw-r--r--   0        0        0     5461 2024-03-01 09:19:24.150124 cg-59.9.0/tests/store/crud/read/test_read_analyses_to_clean.py
--rw-r--r--   0        0        0     3553 2024-03-01 09:19:24.150124 cg-59.9.0/tests/store/crud/read/test_read_analyses_to_delivery_report.py
--rw-r--r--   0        0        0    18463 2024-03-01 09:19:24.150124 cg-59.9.0/tests/store/crud/read/test_read_analysis.py
--rw-r--r--   0        0        0     2743 2024-03-01 09:19:24.150124 cg-59.9.0/tests/store/crud/read/test_read_application_version.py
--rw-r--r--   0        0        0    59704 2024-03-01 09:19:24.150124 cg-59.9.0/tests/store/crud/read/test_read_case.py
--rw-r--r--   0        0        0     1105 2024-03-01 09:19:24.150124 cg-59.9.0/tests/store/crud/read/test_read_customer.py
--rw-r--r--   0        0        0     1530 2024-03-01 09:19:24.150124 cg-59.9.0/tests/store/crud/read/test_read_pool.py
--rw-r--r--   0        0        0    21602 2024-03-01 09:19:24.150124 cg-59.9.0/tests/store/crud/read/test_read_sample.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.150124 cg-59.9.0/tests/store/crud/update/__init__.py
--rw-r--r--   0        0        0      737 2024-03-01 09:19:24.150124 cg-59.9.0/tests/store/crud/update/test_update.py
--rw-r--r--   0        0        0    11693 2024-03-01 09:19:24.150124 cg-59.9.0/tests/store/filters/test_status_analyses_filters.py
--rw-r--r--   0        0        0     3397 2024-03-01 09:19:24.150124 cg-59.9.0/tests/store/filters/test_status_application_filters.py
--rw-r--r--   0        0        0     2073 2024-03-01 09:19:24.150124 cg-59.9.0/tests/store/filters/test_status_application_limitations_filters.py
--rw-r--r--   0        0        0    10452 2024-03-01 09:19:24.150124 cg-59.9.0/tests/store/filters/test_status_application_version_filters.py
--rw-r--r--   0        0        0     2804 2024-03-01 09:19:24.150124 cg-59.9.0/tests/store/filters/test_status_bed_filters.py
--rw-r--r--   0        0        0     2362 2024-03-01 09:19:24.150124 cg-59.9.0/tests/store/filters/test_status_bed_version_filters.py
--rw-r--r--   0        0        0     3495 2024-03-01 09:19:24.150124 cg-59.9.0/tests/store/filters/test_status_case_sample_filters.py
--rw-r--r--   0        0        0    39100 2024-03-01 09:19:24.150124 cg-59.9.0/tests/store/filters/test_status_cases_filters.py
--rw-r--r--   0        0        0     1345 2024-03-01 09:19:24.150124 cg-59.9.0/tests/store/filters/test_status_collaboration_filters.py
--rw-r--r--   0        0        0     2482 2024-03-01 09:19:24.150124 cg-59.9.0/tests/store/filters/test_status_customer_filters.py
--rw-r--r--   0        0        0     4907 2024-03-01 09:19:24.150124 cg-59.9.0/tests/store/filters/test_status_flow_cell_filters.py
--rw-r--r--   0        0        0     2226 2024-03-01 09:19:24.150124 cg-59.9.0/tests/store/filters/test_status_invoice_filters.py
--rw-r--r--   0        0        0     5970 2024-03-01 09:19:24.150124 cg-59.9.0/tests/store/filters/test_status_metrics_filters.py
--rw-r--r--   0        0        0     2404 2024-03-01 09:19:24.150124 cg-59.9.0/tests/store/filters/test_status_organism_filters.py
--rw-r--r--   0        0        0     1804 2024-03-01 09:19:24.150124 cg-59.9.0/tests/store/filters/test_status_panel_filters.py
--rw-r--r--   0        0        0     8720 2024-03-01 09:19:24.150124 cg-59.9.0/tests/store/filters/test_status_pool_filters.py
--rw-r--r--   0        0        0    22967 2024-03-01 09:19:24.150124 cg-59.9.0/tests/store/filters/test_status_samples_filters.py
--rw-r--r--   0        0        0     1576 2024-03-01 09:19:24.150124 cg-59.9.0/tests/store/filters/test_status_user_filters.py
--rw-r--r--   0        0        0     2147 2024-03-01 09:19:24.150124 cg-59.9.0/tests/store/test_delivery.py
--rw-r--r--   0        0        0     4127 2024-03-01 09:19:24.150124 cg-59.9.0/tests/store/test_store_models.py
--rw-r--r--   0        0        0    35256 2024-03-01 09:19:24.154125 cg-59.9.0/tests/store_helpers.py
--rw-r--r--   0        0        0     4930 2024-03-01 09:19:24.154125 cg-59.9.0/tests/test_copy_novaseqx_flow_cell.py
--rw-r--r--   0        0        0      911 2024-03-01 09:19:24.154125 cg-59.9.0/tests/test_store_helpers.py
--rw-r--r--   0        0        0        0 2024-03-01 09:19:24.154125 cg-59.9.0/tests/utils/__init__.py
--rw-r--r--   0        0        0     1754 2024-03-01 09:19:24.154125 cg-59.9.0/tests/utils/conftest.py
--rw-r--r--   0        0        0      371 2024-03-01 09:19:24.154125 cg-59.9.0/tests/utils/test_calculations.py
--rw-r--r--   0        0        0     2920 2024-03-01 09:19:24.154125 cg-59.9.0/tests/utils/test_commands.py
--rw-r--r--   0        0        0      953 2024-03-01 09:19:24.154125 cg-59.9.0/tests/utils/test_date.py
--rw-r--r--   0        0        0     1508 2024-03-01 09:19:24.154125 cg-59.9.0/tests/utils/test_dict.py
--rw-r--r--   0        0        0     7154 2024-03-01 09:19:24.154125 cg-59.9.0/tests/utils/test_dispatcher.py
--rw-r--r--   0        0        0     4100 2024-03-01 09:19:24.154125 cg-59.9.0/tests/utils/test_files.py
--rw-r--r--   0        0        0     1170 2024-03-01 09:19:24.154125 cg-59.9.0/tests/utils/test_time.py
--rw-r--r--   0        0        0     2366 2024-03-01 09:19:24.154125 cg-59.9.0/tests/utils/test_utils.py
--rw-r--r--   0        0        0     4341 1970-01-01 00:00:00.000000 cg-59.9.0/PKG-INFO
+-rw-r--r--   0        0        0     2686 2024-03-04 07:52:11.681385 cg-59.9.1/README.md
+-rw-r--r--   0        0        0       40 2024-03-04 07:52:11.685385 cg-59.9.1/cg/__init__.py
+-rw-r--r--   0        0        0      315 2024-03-04 07:52:11.685385 cg-59.9.1/cg/apps/__init__.py
+-rw-r--r--   0        0        0       27 2024-03-04 07:52:11.685385 cg-59.9.1/cg/apps/coverage/__init__.py
+-rw-r--r--   0        0        0     2940 2024-03-04 07:52:11.685385 cg-59.9.1/cg/apps/coverage/api.py
+-rw-r--r--   0        0        0       56 2024-03-04 07:52:11.685385 cg-59.9.1/cg/apps/crunchy/__init__.py
+-rw-r--r--   0        0        0    12783 2024-03-04 07:52:11.685385 cg-59.9.1/cg/apps/crunchy/crunchy.py
+-rw-r--r--   0        0        0     4502 2024-03-04 07:52:11.685385 cg-59.9.1/cg/apps/crunchy/files.py
+-rw-r--r--   0        0        0      430 2024-03-04 07:52:11.685385 cg-59.9.1/cg/apps/crunchy/models.py
+-rw-r--r--   0        0        0      910 2024-03-04 07:52:11.685385 cg-59.9.1/cg/apps/crunchy/sbatch.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.685385 cg-59.9.1/cg/apps/demultiplex/__init__.py
+-rw-r--r--   0        0        0    12262 2024-03-04 07:52:11.685385 cg-59.9.1/cg/apps/demultiplex/demultiplex_api.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.685385 cg-59.9.1/cg/apps/demultiplex/sample_sheet/__init__.py
+-rw-r--r--   0        0        0     8576 2024-03-04 07:52:11.685385 cg-59.9.1/cg/apps/demultiplex/sample_sheet/api.py
+-rw-r--r--   0        0        0     1581 2024-03-04 07:52:11.685385 cg-59.9.1/cg/apps/demultiplex/sample_sheet/create.py
+-rw-r--r--   0        0        0     4227 2024-03-04 07:52:11.685385 cg-59.9.1/cg/apps/demultiplex/sample_sheet/index.py
+-rw-r--r--   0        0        0     7341 2024-03-04 07:52:11.685385 cg-59.9.1/cg/apps/demultiplex/sample_sheet/override_cycles_validator.py
+-rw-r--r--   0        0        0     4166 2024-03-04 07:52:11.685385 cg-59.9.1/cg/apps/demultiplex/sample_sheet/read_sample_sheet.py
+-rw-r--r--   0        0        0    10542 2024-03-04 07:52:11.685385 cg-59.9.1/cg/apps/demultiplex/sample_sheet/sample_models.py
+-rw-r--r--   0        0        0     9851 2024-03-04 07:52:11.685385 cg-59.9.1/cg/apps/demultiplex/sample_sheet/sample_sheet_creator.py
+-rw-r--r--   0        0        0     1614 2024-03-04 07:52:11.685385 cg-59.9.1/cg/apps/demultiplex/sample_sheet/sample_sheet_models.py
+-rw-r--r--   0        0        0     9644 2024-03-04 07:52:11.685385 cg-59.9.1/cg/apps/demultiplex/sample_sheet/sample_sheet_validator.py
+-rw-r--r--   0        0        0      824 2024-03-04 07:52:11.685385 cg-59.9.1/cg/apps/demultiplex/sample_sheet/validators.py
+-rw-r--r--   0        0        0     1943 2024-03-04 07:52:11.685385 cg-59.9.1/cg/apps/demultiplex/sbatch.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.685385 cg-59.9.1/cg/apps/downsample/__init__.py
+-rw-r--r--   0        0        0     6160 2024-03-04 07:52:11.685385 cg-59.9.1/cg/apps/downsample/downsample.py
+-rw-r--r--   0        0        0     2125 2024-03-04 07:52:11.685385 cg-59.9.1/cg/apps/downsample/utils.py
+-rw-r--r--   0        0        0      298 2024-03-04 07:52:11.685385 cg-59.9.1/cg/apps/environ.py
+-rw-r--r--   0        0        0     1741 2024-03-04 07:52:11.685385 cg-59.9.1/cg/apps/gens.py
+-rw-r--r--   0        0        0     3419 2024-03-04 07:52:11.685385 cg-59.9.1/cg/apps/gt.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.685385 cg-59.9.1/cg/apps/hermes/__init__.py
+-rw-r--r--   0        0        0     2249 2024-03-04 07:52:11.685385 cg-59.9.1/cg/apps/hermes/hermes_api.py
+-rw-r--r--   0        0        0     1298 2024-03-04 07:52:11.685385 cg-59.9.1/cg/apps/hermes/models.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.685385 cg-59.9.1/cg/apps/housekeeper/__init__.py
+-rw-r--r--   0        0        0    28681 2024-03-04 07:52:11.685385 cg-59.9.1/cg/apps/housekeeper/hk.py
+-rw-r--r--   0        0        0      326 2024-03-04 07:52:11.685385 cg-59.9.1/cg/apps/housekeeper/models.py
+-rw-r--r--   0        0        0       32 2024-03-04 07:52:11.685385 cg-59.9.1/cg/apps/invoice/__init__.py
+-rw-r--r--   0        0        0     4804 2024-03-04 07:52:11.685385 cg-59.9.1/cg/apps/invoice/render.py
+-rw-r--r--   0        0        0   113439 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/invoice/templates/KI_pool_invoice.xlsx
+-rw-r--r--   0        0        0    81032 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/invoice/templates/KI_sample_invoice.xlsx
+-rw-r--r--   0        0        0   113363 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/invoice/templates/KTH_pool_invoice.xlsx
+-rw-r--r--   0        0        0    80886 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/invoice/templates/KTH_sample_invoice.xlsx
+-rw-r--r--   0        0        0       25 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/lims/__init__.py
+-rw-r--r--   0        0        0    16539 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/lims/api.py
+-rw-r--r--   0        0        0     2652 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/lims/batch.py
+-rw-r--r--   0        0        0     8129 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/lims/order.py
+-rw-r--r--   0        0        0     3302 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/lims/sample_sheet.py
+-rw-r--r--   0        0        0     4866 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/loqus.py
+-rw-r--r--   0        0        0       35 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/madeline/__init__.py
+-rw-r--r--   0        0        0     3213 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/madeline/api.py
+-rw-r--r--   0        0        0       23 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/mip/__init__.py
+-rw-r--r--   0        0        0     3564 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/mip/confighandler.py
+-rw-r--r--   0        0        0     2207 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/mutacc_auto.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/orderform/__init__.py
+-rw-r--r--   0        0        0     9498 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/orderform/excel_orderform_parser.py
+-rw-r--r--   0        0        0     3051 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/orderform/json_orderform_parser.py
+-rw-r--r--   0        0        0     6419 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/orderform/orderform_parser.py
+-rw-r--r--   0        0        0      252 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/orderform/utils.py
+-rw-r--r--   0        0        0     2537 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/osticket.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/scout/__init__.py
+-rw-r--r--   0        0        0     3177 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/scout/scout_export.py
+-rw-r--r--   0        0        0    11054 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/scout/scoutapi.py
+-rw-r--r--   0        0        0      444 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/scout/validators.py
+-rw-r--r--   0        0        0       78 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/sequencing_metrics_parser/__init__.py
+-rw-r--r--   0        0        0     1854 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/sequencing_metrics_parser/api.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/sequencing_metrics_parser/models/__init__.py
+-rw-r--r--   0        0        0     1871 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/sequencing_metrics_parser/models/bcl2fastq_metrics.py
+-rw-r--r--   0        0        0     1076 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/sequencing_metrics_parser/models/bcl_convert.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/sequencing_metrics_parser/parsers/__init__.py
+-rw-r--r--   0        0        0     7312 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/sequencing_metrics_parser/parsers/bcl2fastq.py
+-rw-r--r--   0        0        0     2641 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/sequencing_metrics_parser/parsers/bcl2fastq_to_sequencing_statistics.py
+-rw-r--r--   0        0        0     6806 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/sequencing_metrics_parser/parsers/bcl_convert.py
+-rw-r--r--   0        0        0     3559 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/sequencing_metrics_parser/parsers/bcl_convert_to_sequencing_statistics.py
+-rw-r--r--   0        0        0      172 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/sequencing_metrics_parser/parsers/utils.py
+-rw-r--r--   0        0        0      836 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/sequencing_metrics_parser/sequencing_metrics_calculator.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/slurm/__init__.py
+-rw-r--r--   0        0        0     1277 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/slurm/sbatch.py
+-rw-r--r--   0        0        0     3559 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/slurm/slurm_api.py
+-rw-r--r--   0        0        0       32 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/tb/__init__.py
+-rw-r--r--   0        0        0     7501 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/tb/api.py
+-rw-r--r--   0        0        0      152 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/tb/dto/create_job_request.py
+-rw-r--r--   0        0        0      287 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/tb/dto/summary_response.py
+-rw-r--r--   0        0        0     1305 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/tb/models.py
+-rw-r--r--   0        0        0      305 2024-03-04 07:52:11.689385 cg-59.9.1/cg/apps/tb/validators.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.689385 cg-59.9.1/cg/cli/__init__.py
+-rw-r--r--   0        0        0    10945 2024-03-04 07:52:11.689385 cg-59.9.1/cg/cli/add.py
+-rw-r--r--   0        0        0     2653 2024-03-04 07:52:11.689385 cg-59.9.1/cg/cli/archive.py
+-rw-r--r--   0        0        0    10118 2024-03-04 07:52:11.689385 cg-59.9.1/cg/cli/backup.py
+-rw-r--r--   0        0        0     3853 2024-03-04 07:52:11.689385 cg-59.9.1/cg/cli/base.py
+-rw-r--r--   0        0        0    10506 2024-03-04 07:52:11.689385 cg-59.9.1/cg/cli/clean.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.689385 cg-59.9.1/cg/cli/compress/__init__.py
+-rw-r--r--   0        0        0     2135 2024-03-04 07:52:11.689385 cg-59.9.1/cg/cli/compress/base.py
+-rw-r--r--   0        0        0     6706 2024-03-04 07:52:11.689385 cg-59.9.1/cg/cli/compress/fastq.py
+-rw-r--r--   0        0        0     8163 2024-03-04 07:52:11.689385 cg-59.9.1/cg/cli/compress/helpers.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/delete/__init__.py
+-rw-r--r--   0        0        0      564 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/delete/base.py
+-rw-r--r--   0        0        0     4603 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/delete/case.py
+-rw-r--r--   0        0        0     1884 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/delete/cases.py
+-rw-r--r--   0        0        0     2633 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/delete/observations.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/deliver/__init__.py
+-rw-r--r--   0        0        0     6270 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/deliver/base.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/demultiplex/__init__.py
+-rw-r--r--   0        0        0      829 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/demultiplex/base.py
+-rw-r--r--   0        0        0     4905 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/demultiplex/copy_novaseqx_demultiplex_data.py
+-rw-r--r--   0        0        0     8016 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/demultiplex/demux.py
+-rw-r--r--   0        0        0     1619 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/demultiplex/finish.py
+-rw-r--r--   0        0        0     2683 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/demultiplex/sample_sheet.py
+-rw-r--r--   0        0        0     2995 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/downsample.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/generate/__init__.py
+-rw-r--r--   0        0        0      356 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/generate/base.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/generate/report/__init__.py
+-rw-r--r--   0        0        0     4636 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/generate/report/base.py
+-rw-r--r--   0        0        0      854 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/generate/report/options.py
+-rw-r--r--   0        0        0     5107 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/generate/report/utils.py
+-rw-r--r--   0        0        0     8326 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/get.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/set/__init__.py
+-rw-r--r--   0        0        0     9856 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/set/base.py
+-rw-r--r--   0        0        0     4384 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/set/case.py
+-rw-r--r--   0        0        0     2595 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/set/cases.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/store/__init__.py
+-rw-r--r--   0        0        0     5340 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/store/fastq.py
+-rw-r--r--   0        0        0     1049 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/store/store.py
+-rw-r--r--   0        0        0     1761 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/transfer.py
+-rw-r--r--   0        0        0        1 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/upload/__init__.py
+-rw-r--r--   0        0        0     5652 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/upload/base.py
+-rw-r--r--   0        0        0     5238 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/upload/clinical_delivery.py
+-rw-r--r--   0        0        0     1175 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/upload/coverage.py
+-rw-r--r--   0        0        0     1528 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/upload/delivery_report.py
+-rw-r--r--   0        0        0     4022 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/upload/fohm.py
+-rw-r--r--   0        0        0     1463 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/upload/genotype.py
+-rw-r--r--   0        0        0     1885 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/upload/gens.py
+-rw-r--r--   0        0        0      584 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/upload/gisaid.py
+-rw-r--r--   0        0        0     2645 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/upload/mutacc.py
+-rw-r--r--   0        0        0       23 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/upload/nipt/__init__.py
+-rw-r--r--   0        0        0     3006 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/upload/nipt/base.py
+-rw-r--r--   0        0        0     2275 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/upload/nipt/ftp.py
+-rw-r--r--   0        0        0     1596 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/upload/nipt/statina.py
+-rw-r--r--   0        0        0      112 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/upload/observations/__init__.py
+-rw-r--r--   0        0        0     2672 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/upload/observations/observations.py
+-rw-r--r--   0        0        0     2904 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/upload/observations/utils.py
+-rw-r--r--   0        0        0     9970 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/upload/scout.py
+-rw-r--r--   0        0        0      650 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/upload/utils.py
+-rw-r--r--   0        0        0     1667 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/upload/validate.py
+-rw-r--r--   0        0        0      105 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/utils.py
+-rw-r--r--   0        0        0       18 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/workflow/__init__.py
+-rw-r--r--   0        0        0       22 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/workflow/balsamic/__init__.py
+-rw-r--r--   0        0        0     8925 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/workflow/balsamic/base.py
+-rw-r--r--   0        0        0     1980 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/workflow/balsamic/options.py
+-rw-r--r--   0        0        0      881 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/workflow/balsamic/pon.py
+-rw-r--r--   0        0        0     1162 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/workflow/balsamic/qc.py
+-rw-r--r--   0        0        0     1177 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/workflow/balsamic/umi.py
+-rw-r--r--   0        0        0     1196 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/workflow/base.py
+-rw-r--r--   0        0        0    12379 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/workflow/commands.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/workflow/fastq/__init__.py
+-rw-r--r--   0        0        0     1367 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/workflow/fastq/base.py
+-rw-r--r--   0        0        0     1787 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/workflow/fastq/fastq_service.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/workflow/fluffy/__init__.py
+-rw-r--r--   0        0        0     4177 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/workflow/fluffy/base.py
+-rw-r--r--   0        0        0       22 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/workflow/microsalt/__init__.py
+-rw-r--r--   0        0        0     7810 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/workflow/microsalt/base.py
+-rw-r--r--   0        0        0       22 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/workflow/mip/__init__.py
+-rw-r--r--   0        0        0     6596 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/workflow/mip/base.py
+-rw-r--r--   0        0        0     1268 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/workflow/mip/options.py
+-rw-r--r--   0        0        0       22 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/workflow/mip_dna/__init__.py
+-rw-r--r--   0        0        0     1013 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/workflow/mip_dna/base.py
+-rw-r--r--   0        0        0       22 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/workflow/mip_rna/__init__.py
+-rw-r--r--   0        0        0      916 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/workflow/mip_rna/base.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/workflow/mutant/__init__.py
+-rw-r--r--   0        0        0     3413 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/workflow/mutant/base.py
+-rw-r--r--   0        0        0     3532 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/workflow/nf_analysis.py
+-rw-r--r--   0        0        0       22 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/workflow/raredisease/__init__.py
+-rw-r--r--   0        0        0     1865 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/workflow/raredisease/base.py
+-rw-r--r--   0        0        0       22 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/workflow/rnafusion/__init__.py
+-rw-r--r--   0        0        0    10391 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/workflow/rnafusion/base.py
+-rw-r--r--   0        0        0      554 2024-03-04 07:52:11.693385 cg-59.9.1/cg/cli/workflow/rnafusion/options.py
+-rw-r--r--   0        0        0       22 2024-03-04 07:52:11.697385 cg-59.9.1/cg/cli/workflow/taxprofiler/__init__.py
+-rw-r--r--   0        0        0     6512 2024-03-04 07:52:11.697385 cg-59.9.1/cg/cli/workflow/taxprofiler/base.py
+-rw-r--r--   0        0        0      531 2024-03-04 07:52:11.697385 cg-59.9.1/cg/cli/workflow/taxprofiler/options.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.697385 cg-59.9.1/cg/clients/__init__.py
+-rw-r--r--   0        0        0      147 2024-03-04 07:52:11.697385 cg-59.9.1/cg/clients/arnold/api.py
+-rw-r--r--   0        0        0      125 2024-03-04 07:52:11.697385 cg-59.9.1/cg/clients/arnold/dto/create_case_request.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.697385 cg-59.9.1/cg/clients/janus/__init__.py
+-rw-r--r--   0        0        0     1078 2024-03-04 07:52:11.697385 cg-59.9.1/cg/clients/janus/api.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.697385 cg-59.9.1/cg/clients/janus/dto/__init__.py
+-rw-r--r--   0        0        0      503 2024-03-04 07:52:11.697385 cg-59.9.1/cg/clients/janus/dto/create_qc_metrics_request.py
+-rw-r--r--   0        0        0      420 2024-03-04 07:52:11.697385 cg-59.9.1/cg/clients/janus/exceptions.py
+-rw-r--r--   0        0        0      937 2024-03-04 07:52:11.697385 cg-59.9.1/cg/constants/__init__.py
+-rw-r--r--   0        0        0      253 2024-03-04 07:52:11.697385 cg-59.9.1/cg/constants/archiving.py
+-rw-r--r--   0        0        0       35 2024-03-04 07:52:11.697385 cg-59.9.1/cg/constants/backup.py
+-rw-r--r--   0        0        0     1411 2024-03-04 07:52:11.697385 cg-59.9.1/cg/constants/bcl_convert_metrics.py
+-rw-r--r--   0        0        0      469 2024-03-04 07:52:11.697385 cg-59.9.1/cg/constants/compression.py
+-rw-r--r--   0        0        0     6285 2024-03-04 07:52:11.697385 cg-59.9.1/cg/constants/constants.py
+-rw-r--r--   0        0        0     5615 2024-03-04 07:52:11.697385 cg-59.9.1/cg/constants/delivery.py
+-rw-r--r--   0        0        0     9650 2024-03-04 07:52:11.697385 cg-59.9.1/cg/constants/demultiplexing.py
+-rw-r--r--   0        0        0     1422 2024-03-04 07:52:11.697385 cg-59.9.1/cg/constants/encryption.py
+-rw-r--r--   0        0        0      372 2024-03-04 07:52:11.697385 cg-59.9.1/cg/constants/extraction.py
+-rw-r--r--   0        0        0     2047 2024-03-04 07:52:11.697385 cg-59.9.1/cg/constants/gene_panel.py
+-rw-r--r--   0        0        0     6396 2024-03-04 07:52:11.697385 cg-59.9.1/cg/constants/housekeeper_tags.py
+-rw-r--r--   0        0        0       95 2024-03-04 07:52:11.697385 cg-59.9.1/cg/constants/invoice.py
+-rw-r--r--   0        0        0     5815 2024-03-04 07:52:11.697385 cg-59.9.1/cg/constants/lims.py
+-rw-r--r--   0        0        0      231 2024-03-04 07:52:11.697385 cg-59.9.1/cg/constants/nanopore_files.py
+-rw-r--r--   0        0        0      650 2024-03-04 07:52:11.697385 cg-59.9.1/cg/constants/nextflow.py
+-rw-r--r--   0        0        0      862 2024-03-04 07:52:11.697385 cg-59.9.1/cg/constants/nf_analysis.py
+-rw-r--r--   0        0        0       19 2024-03-04 07:52:11.697385 cg-59.9.1/cg/constants/nipt.py
+-rw-r--r--   0        0        0     2257 2024-03-04 07:52:11.697385 cg-59.9.1/cg/constants/observations.py
+-rw-r--r--   0        0        0     1216 2024-03-04 07:52:11.697385 cg-59.9.1/cg/constants/orderforms.py
+-rw-r--r--   0        0        0       96 2024-03-04 07:52:11.697385 cg-59.9.1/cg/constants/paths.py
+-rw-r--r--   0        0        0      266 2024-03-04 07:52:11.697385 cg-59.9.1/cg/constants/pdc.py
+-rw-r--r--   0        0        0      160 2024-03-04 07:52:11.697385 cg-59.9.1/cg/constants/pedigree.py
+-rw-r--r--   0        0        0     1044 2024-03-04 07:52:11.697385 cg-59.9.1/cg/constants/priority.py
+-rw-r--r--   0        0        0       79 2024-03-04 07:52:11.697385 cg-59.9.1/cg/constants/process.py
+-rw-r--r--   0        0        0     4506 2024-03-04 07:52:11.697385 cg-59.9.1/cg/constants/report.py
+-rw-r--r--   0        0        0      485 2024-03-04 07:52:11.697385 cg-59.9.1/cg/constants/sample_sources.py
+-rw-r--r--   0        0        0     3111 2024-03-04 07:52:11.697385 cg-59.9.1/cg/constants/scout.py
+-rw-r--r--   0        0        0     1669 2024-03-04 07:52:11.697385 cg-59.9.1/cg/constants/sequencing.py
+-rw-r--r--   0        0        0      313 2024-03-04 07:52:11.697385 cg-59.9.1/cg/constants/slurm.py
+-rw-r--r--   0        0        0      529 2024-03-04 07:52:11.697385 cg-59.9.1/cg/constants/subject.py
+-rw-r--r--   0        0        0       55 2024-03-04 07:52:11.697385 cg-59.9.1/cg/constants/symbols.py
+-rw-r--r--   0        0        0      435 2024-03-04 07:52:11.697385 cg-59.9.1/cg/constants/tb.py
+-rw-r--r--   0        0        0      161 2024-03-04 07:52:11.697385 cg-59.9.1/cg/constants/time.py
+-rw-r--r--   0        0        0     6014 2024-03-04 07:52:11.697385 cg-59.9.1/cg/exc.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.697385 cg-59.9.1/cg/io/__init__.py
+-rw-r--r--   0        0        0     1037 2024-03-04 07:52:11.697385 cg-59.9.1/cg/io/api.py
+-rw-r--r--   0        0        0     2913 2024-03-04 07:52:11.697385 cg-59.9.1/cg/io/controller.py
+-rw-r--r--   0        0        0     1763 2024-03-04 07:52:11.697385 cg-59.9.1/cg/io/csv.py
+-rw-r--r--   0        0        0      210 2024-03-04 07:52:11.697385 cg-59.9.1/cg/io/gzip.py
+-rw-r--r--   0        0        0      616 2024-03-04 07:52:11.697385 cg-59.9.1/cg/io/json.py
+-rw-r--r--   0        0        0      601 2024-03-04 07:52:11.697385 cg-59.9.1/cg/io/txt.py
+-rw-r--r--   0        0        0      552 2024-03-04 07:52:11.697385 cg-59.9.1/cg/io/validate_path.py
+-rw-r--r--   0        0        0     1289 2024-03-04 07:52:11.697385 cg-59.9.1/cg/io/xml.py
+-rw-r--r--   0        0        0     1153 2024-03-04 07:52:11.697385 cg-59.9.1/cg/io/yaml.py
+-rw-r--r--   0        0        0      281 2024-03-04 07:52:11.697385 cg-59.9.1/cg/meta/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.697385 cg-59.9.1/cg/meta/archive/__init__.py
+-rw-r--r--   0        0        0    15193 2024-03-04 07:52:11.697385 cg-59.9.1/cg/meta/archive/archive.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.697385 cg-59.9.1/cg/meta/archive/ddn/__init__.py
+-rw-r--r--   0        0        0     1727 2024-03-04 07:52:11.697385 cg-59.9.1/cg/meta/archive/ddn/constants.py
+-rw-r--r--   0        0        0    10853 2024-03-04 07:52:11.697385 cg-59.9.1/cg/meta/archive/ddn/ddn_data_flow_client.py
+-rw-r--r--   0        0        0     3704 2024-03-04 07:52:11.697385 cg-59.9.1/cg/meta/archive/ddn/models.py
+-rw-r--r--   0        0        0     1250 2024-03-04 07:52:11.697385 cg-59.9.1/cg/meta/archive/ddn/utils.py
+-rw-r--r--   0        0        0     2024 2024-03-04 07:52:11.697385 cg-59.9.1/cg/meta/archive/models.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.697385 cg-59.9.1/cg/meta/backup/__init__.py
+-rw-r--r--   0        0        0    17530 2024-03-04 07:52:11.697385 cg-59.9.1/cg/meta/backup/backup.py
+-rw-r--r--   0        0        0     5397 2024-03-04 07:52:11.697385 cg-59.9.1/cg/meta/backup/pdc.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.697385 cg-59.9.1/cg/meta/clean/__init__.py
+-rw-r--r--   0        0        0     3901 2024-03-04 07:52:11.697385 cg-59.9.1/cg/meta/clean/api.py
+-rw-r--r--   0        0        0     7744 2024-03-04 07:52:11.697385 cg-59.9.1/cg/meta/clean/clean_flow_cells.py
+-rw-r--r--   0        0        0     1841 2024-03-04 07:52:11.697385 cg-59.9.1/cg/meta/clean/clean_retrieved_spring_files.py
+-rw-r--r--   0        0        0       34 2024-03-04 07:52:11.697385 cg-59.9.1/cg/meta/compress/__init__.py
+-rw-r--r--   0        0        0    14557 2024-03-04 07:52:11.697385 cg-59.9.1/cg/meta/compress/compress.py
+-rw-r--r--   0        0        0     4947 2024-03-04 07:52:11.697385 cg-59.9.1/cg/meta/compress/files.py
+-rw-r--r--   0        0        0    14247 2024-03-04 07:52:11.697385 cg-59.9.1/cg/meta/deliver.py
+-rw-r--r--   0        0        0     7886 2024-03-04 07:52:11.697385 cg-59.9.1/cg/meta/deliver_ticket.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.697385 cg-59.9.1/cg/meta/demultiplex/__init__.py
+-rw-r--r--   0        0        0     2592 2024-03-04 07:52:11.697385 cg-59.9.1/cg/meta/demultiplex/combine_sequencing_metrics.py
+-rw-r--r--   0        0        0     5915 2024-03-04 07:52:11.697385 cg-59.9.1/cg/meta/demultiplex/demux_post_processing.py
+-rw-r--r--   0        0        0     4135 2024-03-04 07:52:11.697385 cg-59.9.1/cg/meta/demultiplex/files.py
+-rw-r--r--   0        0        0     7777 2024-03-04 07:52:11.697385 cg-59.9.1/cg/meta/demultiplex/housekeeper_storage_functions.py
+-rw-r--r--   0        0        0     6941 2024-03-04 07:52:11.697385 cg-59.9.1/cg/meta/demultiplex/status_db_storage_functions.py
+-rw-r--r--   0        0        0    11951 2024-03-04 07:52:11.697385 cg-59.9.1/cg/meta/demultiplex/utils.py
+-rw-r--r--   0        0        0     2855 2024-03-04 07:52:11.697385 cg-59.9.1/cg/meta/demultiplex/validation.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.697385 cg-59.9.1/cg/meta/encryption/__init__.py
+-rw-r--r--   0        0        0    19578 2024-03-04 07:52:11.697385 cg-59.9.1/cg/meta/encryption/encryption.py
+-rw-r--r--   0        0        0      464 2024-03-04 07:52:11.697385 cg-59.9.1/cg/meta/encryption/sbatch.py
+-rw-r--r--   0        0        0    10922 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/invoice.py
+-rw-r--r--   0        0        0     2249 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/meta.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/observations/__init__.py
+-rw-r--r--   0        0        0     6008 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/observations/balsamic_observations_api.py
+-rw-r--r--   0        0        0     5277 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/observations/mip_dna_observations_api.py
+-rw-r--r--   0        0        0     5364 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/observations/observations_api.py
+-rw-r--r--   0        0        0       27 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/orders/__init__.py
+-rw-r--r--   0        0        0     3637 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/orders/api.py
+-rw-r--r--   0        0        0      121 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/orders/balsamic_qc_submitter.py
+-rw-r--r--   0        0        0      107 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/orders/balsamic_submitter.py
+-rw-r--r--   0        0        0      122 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/orders/balsamic_umi_submitter.py
+-rw-r--r--   0        0        0    15262 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/orders/case_submitter.py
+-rw-r--r--   0        0        0     6102 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/orders/fastq_submitter.py
+-rw-r--r--   0        0        0      105 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/orders/fluffy_submitter.py
+-rw-r--r--   0        0        0     1254 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/orders/lims.py
+-rw-r--r--   0        0        0     5782 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/orders/metagenome_submitter.py
+-rw-r--r--   0        0        0     6337 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/orders/microbial_submitter.py
+-rw-r--r--   0        0        0      123 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/orders/microsalt_submitter.py
+-rw-r--r--   0        0        0      105 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/orders/mip_dna_submitter.py
+-rw-r--r--   0        0        0      105 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/orders/mip_rna_submitter.py
+-rw-r--r--   0        0        0     7761 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/orders/pool_submitter.py
+-rw-r--r--   0        0        0      102 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/orders/rml_submitter.py
+-rw-r--r--   0        0        0      718 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/orders/rnafusion_submitter.py
+-rw-r--r--   0        0        0     1268 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/orders/sars_cov_2_submitter.py
+-rw-r--r--   0        0        0     1754 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/orders/submitter.py
+-rw-r--r--   0        0        0     7880 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/orders/ticket_handler.py
+-rw-r--r--   0        0        0     3608 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/qc_metrics/collect_qc_metrics.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/report/__init__.py
+-rw-r--r--   0        0        0    10372 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/report/balsamic.py
+-rw-r--r--   0        0        0      562 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/report/balsamic_qc.py
+-rw-r--r--   0        0        0      717 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/report/balsamic_umi.py
+-rw-r--r--   0        0        0     4171 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/report/field_validators.py
+-rw-r--r--   0        0        0     7160 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/report/mip_dna.py
+-rw-r--r--   0        0        0    19056 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/report/report_api.py
+-rw-r--r--   0        0        0     5403 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/report/rnafusion.py
+-rw-r--r--   0        0        0    80176 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/report/templates/balsamic_report.html
+-rw-r--r--   0        0        0   151463 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/report/templates/bootstrap.html
+-rw-r--r--   0        0        0    78094 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/report/templates/mip-dna_report.html
+-rw-r--r--   0        0        0    79169 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/report/templates/rnafusion_report.html
+-rw-r--r--   0        0        0       32 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/rsync/__init__.py
+-rw-r--r--   0        0        0    12141 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/rsync/rsync_api.py
+-rw-r--r--   0        0        0      387 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/rsync/sbatch.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/tar/__init__.py
+-rw-r--r--   0        0        0     1694 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/tar/tar.py
+-rw-r--r--   0        0        0       71 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/transfer/__init__.py
+-rw-r--r--   0        0        0    10013 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/transfer/external_data.py
+-rw-r--r--   0        0        0     5814 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/transfer/lims.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/upload/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/upload/balsamic/__init__.py
+-rw-r--r--   0        0        0     3107 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/upload/balsamic/balsamic.py
+-rw-r--r--   0        0        0     2224 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/upload/coverage.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/upload/fohm/__init__.py
+-rw-r--r--   0        0        0    12102 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/upload/fohm/fohm.py
+-rw-r--r--   0        0        0       30 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/upload/gisaid/__init__.py
+-rw-r--r--   0        0        0      928 2024-03-04 07:52:11.701385 cg-59.9.1/cg/meta/upload/gisaid/constants.py
+-rw-r--r--   0        0        0    13521 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/upload/gisaid/gisaid.py
+-rw-r--r--   0        0        0     3312 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/upload/gisaid/models.py
+-rw-r--r--   0        0        0     5310 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/upload/gt.py
+-rw-r--r--   0        0        0      898 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/upload/microsalt/microsalt_upload_api.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/upload/mip/__init__.py
+-rw-r--r--   0        0        0     2546 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/upload/mip/mip_dna.py
+-rw-r--r--   0        0        0     1400 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/upload/mip/mip_rna.py
+-rw-r--r--   0        0        0     7294 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/upload/mutacc.py
+-rw-r--r--   0        0        0       32 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/upload/nipt/__init__.py
+-rw-r--r--   0        0        0      696 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/upload/nipt/models.py
+-rw-r--r--   0        0        0     8106 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/upload/nipt/nipt.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/upload/rnafusion/__init__.py
+-rw-r--r--   0        0        0     1698 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/upload/rnafusion/rnafusion.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/upload/scout/__init__.py
+-rw-r--r--   0        0        0     4009 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/upload/scout/balsamic_config_builder.py
+-rw-r--r--   0        0        0     1491 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/upload/scout/balsamic_umi_config_builder.py
+-rw-r--r--   0        0        0     3322 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/upload/scout/hk_tags.py
+-rw-r--r--   0        0        0     9103 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/upload/scout/mip_config_builder.py
+-rw-r--r--   0        0        0     3495 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/upload/scout/rnafusion_config_builder.py
+-rw-r--r--   0        0        0     7516 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/upload/scout/scout_config_builder.py
+-rw-r--r--   0        0        0    23146 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/upload/scout/uploadscoutapi.py
+-rw-r--r--   0        0        0     3197 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/upload/upload_api.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/workflow/__init__.py
+-rw-r--r--   0        0        0    26334 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/workflow/analysis.py
+-rw-r--r--   0        0        0    26074 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/workflow/balsamic.py
+-rw-r--r--   0        0        0     2700 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/workflow/balsamic_pon.py
+-rw-r--r--   0        0        0      553 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/workflow/balsamic_qc.py
+-rw-r--r--   0        0        0      556 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/workflow/balsamic_umi.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/workflow/downsample/__init__.py
+-rw-r--r--   0        0        0     3922 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/workflow/downsample/downsample.py
+-rw-r--r--   0        0        0      711 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/workflow/downsample/sbatch.py
+-rw-r--r--   0        0        0     8913 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/workflow/fastq.py
+-rw-r--r--   0        0        0    10687 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/workflow/fluffy.py
+-rw-r--r--   0        0        0       70 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/workflow/microsalt/__init__.py
+-rw-r--r--   0        0        0      116 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/workflow/microsalt/constants.py
+-rw-r--r--   0        0        0      174 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/workflow/microsalt/metrics_parser/__init__.py
+-rw-r--r--   0        0        0      366 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/workflow/microsalt/metrics_parser/metrics_parser.py
+-rw-r--r--   0        0        0      903 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/workflow/microsalt/metrics_parser/models.py
+-rw-r--r--   0        0        0    13171 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/workflow/microsalt/microsalt.py
+-rw-r--r--   0        0        0       95 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/workflow/microsalt/quality_controller/__init__.py
+-rw-r--r--   0        0        0      712 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/workflow/microsalt/quality_controller/models.py
+-rw-r--r--   0        0        0     5688 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/workflow/microsalt/quality_controller/quality_controller.py
+-rw-r--r--   0        0        0     1217 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/workflow/microsalt/quality_controller/report_generator.py
+-rw-r--r--   0        0        0     2373 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/workflow/microsalt/quality_controller/result_logger.py
+-rw-r--r--   0        0        0     5641 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/workflow/microsalt/quality_controller/utils.py
+-rw-r--r--   0        0        0     1220 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/workflow/microsalt/utils.py
+-rw-r--r--   0        0        0    13833 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/workflow/mip.py
+-rw-r--r--   0        0        0     2686 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/workflow/mip_dna.py
+-rw-r--r--   0        0        0     2167 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/workflow/mip_rna.py
+-rw-r--r--   0        0        0    10587 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/workflow/mutant.py
+-rw-r--r--   0        0        0    19362 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/workflow/nf_analysis.py
+-rw-r--r--   0        0        0     6161 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/workflow/nf_handlers.py
+-rw-r--r--   0        0        0     6394 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/workflow/prepare_fastq.py
+-rw-r--r--   0        0        0     2318 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/workflow/raredisease.py
+-rw-r--r--   0        0        0     8987 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/workflow/rnafusion.py
+-rw-r--r--   0        0        0     7652 2024-03-04 07:52:11.705385 cg-59.9.1/cg/meta/workflow/taxprofiler.py
+-rw-r--r--   0        0        0      113 2024-03-04 07:52:11.705385 cg-59.9.1/cg/models/__init__.py
+-rw-r--r--   0        0        0      102 2024-03-04 07:52:11.705385 cg-59.9.1/cg/models/analysis.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.705385 cg-59.9.1/cg/models/balsamic/__init__.py
+-rw-r--r--   0        0        0      459 2024-03-04 07:52:11.705385 cg-59.9.1/cg/models/balsamic/analysis.py
+-rw-r--r--   0        0        0     4550 2024-03-04 07:52:11.705385 cg-59.9.1/cg/models/balsamic/config.py
+-rw-r--r--   0        0        0     1954 2024-03-04 07:52:11.705385 cg-59.9.1/cg/models/balsamic/metrics.py
+-rw-r--r--   0        0        0    16013 2024-03-04 07:52:11.705385 cg-59.9.1/cg/models/cg_config.py
+-rw-r--r--   0        0        0     4302 2024-03-04 07:52:11.705385 cg-59.9.1/cg/models/compression_data.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.705385 cg-59.9.1/cg/models/deliverables/__init__.py
+-rw-r--r--   0        0        0     5170 2024-03-04 07:52:11.705385 cg-59.9.1/cg/models/deliverables/metric_deliverables.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.705385 cg-59.9.1/cg/models/demultiplex/__init__.py
+-rw-r--r--   0        0        0    12040 2024-03-04 07:52:11.705385 cg-59.9.1/cg/models/demultiplex/run_parameters.py
+-rw-r--r--   0        0        0      539 2024-03-04 07:52:11.705385 cg-59.9.1/cg/models/demultiplex/sbatch.py
+-rw-r--r--   0        0        0     6823 2024-03-04 07:52:11.705385 cg-59.9.1/cg/models/downsample/downsample_data.py
+-rw-r--r--   0        0        0      255 2024-03-04 07:52:11.705385 cg-59.9.1/cg/models/email.py
+-rw-r--r--   0        0        0     1046 2024-03-04 07:52:11.705385 cg-59.9.1/cg/models/fastq.py
+-rw-r--r--   0        0        0     2157 2024-03-04 07:52:11.705385 cg-59.9.1/cg/models/file_data.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.705385 cg-59.9.1/cg/models/flow_cell/__init__.py
+-rw-r--r--   0        0        0    10976 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/flow_cell/flow_cell.py
+-rw-r--r--   0        0        0      317 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/flow_cell/utils.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/invoice/__init__.py
+-rw-r--r--   0        0        0     1254 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/invoice/invoice.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/lims/__init__.py
+-rw-r--r--   0        0        0     2019 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/lims/sample.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/mip/__init__.py
+-rw-r--r--   0        0        0      337 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/mip/mip_analysis.py
+-rw-r--r--   0        0        0     1564 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/mip/mip_config.py
+-rw-r--r--   0        0        0     4696 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/mip/mip_metrics_deliverables.py
+-rw-r--r--   0        0        0     2550 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/mip/mip_sample_info.py
+-rw-r--r--   0        0        0     2076 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/nf_analysis.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/observations/__init__.py
+-rw-r--r--   0        0        0      688 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/observations/input_files.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/orders/__init__.py
+-rw-r--r--   0        0        0     2659 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/orders/constants.py
+-rw-r--r--   0        0        0     5604 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/orders/excel_sample.py
+-rw-r--r--   0        0        0      898 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/orders/json_sample.py
+-rw-r--r--   0        0        0     1449 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/orders/order.py
+-rw-r--r--   0        0        0      811 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/orders/orderform_schema.py
+-rw-r--r--   0        0        0     4212 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/orders/sample_base.py
+-rw-r--r--   0        0        0     9549 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/orders/samples.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/orders/validators/__init__.py
+-rw-r--r--   0        0        0     2300 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/orders/validators/excel_sample_validators.py
+-rw-r--r--   0        0        0      576 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/orders/validators/json_sample_validators.py
+-rw-r--r--   0        0        0       71 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/orders/validators/sample_base_validators.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/raredisease/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/report/__init__.py
+-rw-r--r--   0        0        0     6785 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/report/metadata.py
+-rw-r--r--   0        0        0     5951 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/report/report.py
+-rw-r--r--   0        0        0     4724 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/report/sample.py
+-rw-r--r--   0        0        0     2669 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/report/validators.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/rnafusion/__init__.py
+-rw-r--r--   0        0        0     2633 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/rnafusion/rnafusion.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/scout/__init__.py
+-rw-r--r--   0        0        0     4783 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/scout/scout_load_config.py
+-rw-r--r--   0        0        0      116 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/scout/validators.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/slurm/__init__.py
+-rw-r--r--   0        0        0      617 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/slurm/sbatch.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/taxprofiler/__init__.py
+-rw-r--r--   0        0        0     2433 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/taxprofiler/taxprofiler.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/workflow/__init__.py
+-rw-r--r--   0        0        0      685 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/workflow/mutant.py
+-rw-r--r--   0        0        0       70 2024-03-04 07:52:11.709385 cg-59.9.1/cg/models/workflow/validators.py
+-rw-r--r--   0        0        0    25590 2024-03-04 07:52:11.709385 cg-59.9.1/cg/resources/20181012_Indices.csv
+-rw-r--r--   0        0        0      661 2024-03-04 07:52:11.709385 cg-59.9.1/cg/resources/__init__.py
+-rw-r--r--   0        0        0     2590 2024-03-04 07:52:11.709385 cg-59.9.1/cg/resources/rnafusion_bundle_filenames.csv
+-rw-r--r--   0        0        0     2583 2024-03-04 07:52:11.709385 cg-59.9.1/cg/resources/taxprofiler_bundle_filenames.csv
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.709385 cg-59.9.1/cg/server/__init__.py
+-rw-r--r--   0        0        0    20077 2024-03-04 07:52:11.709385 cg-59.9.1/cg/server/admin.py
+-rw-r--r--   0        0        0    19972 2024-03-04 07:52:11.709385 cg-59.9.1/cg/server/api.py
+-rw-r--r--   0        0        0     4813 2024-03-04 07:52:11.709385 cg-59.9.1/cg/server/app.py
+-rw-r--r--   0        0        0       48 2024-03-04 07:52:11.709385 cg-59.9.1/cg/server/auto.py
+-rw-r--r--   0        0        0     1184 2024-03-04 07:52:11.709385 cg-59.9.1/cg/server/config.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.709385 cg-59.9.1/cg/server/dto/__init__.py
+-rw-r--r--   0        0        0       92 2024-03-04 07:52:11.709385 cg-59.9.1/cg/server/dto/delivery_message_response.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.709385 cg-59.9.1/cg/server/dto/orders/__init__.py
+-rw-r--r--   0        0        0      598 2024-03-04 07:52:11.709385 cg-59.9.1/cg/server/dto/orders/orders_request.py
+-rw-r--r--   0        0        0      397 2024-03-04 07:52:11.709385 cg-59.9.1/cg/server/dto/orders/orders_response.py
+-rw-r--r--   0        0        0     2404 2024-03-04 07:52:11.709385 cg-59.9.1/cg/server/ext.py
+-rw-r--r--   0        0        0       29 2024-03-04 07:52:11.709385 cg-59.9.1/cg/server/invoices/__init__.py
+-rw-r--r--   0        0        0     4793 2024-03-04 07:52:11.709385 cg-59.9.1/cg/server/invoices/templates/invoices/index.html
+-rw-r--r--   0        0        0     8171 2024-03-04 07:52:11.709385 cg-59.9.1/cg/server/invoices/templates/invoices/invoice.html
+-rw-r--r--   0        0        0     2838 2024-03-04 07:52:11.709385 cg-59.9.1/cg/server/invoices/templates/invoices/layout.html
+-rw-r--r--   0        0        0     4956 2024-03-04 07:52:11.709385 cg-59.9.1/cg/server/invoices/templates/invoices/new.html
+-rw-r--r--   0        0        0     7715 2024-03-04 07:52:11.709385 cg-59.9.1/cg/server/invoices/views.py
+-rw-r--r--   0        0        0      354 2024-03-04 07:52:11.709385 cg-59.9.1/cg/server/templates/admin/index.html
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.709385 cg-59.9.1/cg/services/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.709385 cg-59.9.1/cg/services/delivery_message/__init__.py
+-rw-r--r--   0        0        0      607 2024-03-04 07:52:11.709385 cg-59.9.1/cg/services/delivery_message/delivery_message_service.py
+-rw-r--r--   0        0        0      792 2024-03-04 07:52:11.709385 cg-59.9.1/cg/services/delivery_message/messages/__init__.py
+-rw-r--r--   0        0        0      706 2024-03-04 07:52:11.709385 cg-59.9.1/cg/services/delivery_message/messages/analysis_scout_message.py
+-rw-r--r--   0        0        0      777 2024-03-04 07:52:11.709385 cg-59.9.1/cg/services/delivery_message/messages/covid_message.py
+-rw-r--r--   0        0        0      182 2024-03-04 07:52:11.709385 cg-59.9.1/cg/services/delivery_message/messages/delivery_message.py
+-rw-r--r--   0        0        0      721 2024-03-04 07:52:11.709385 cg-59.9.1/cg/services/delivery_message/messages/fastq_analysis_scout_message.py
+-rw-r--r--   0        0        0      525 2024-03-04 07:52:11.709385 cg-59.9.1/cg/services/delivery_message/messages/fastq_message.py
+-rw-r--r--   0        0        0      701 2024-03-04 07:52:11.709385 cg-59.9.1/cg/services/delivery_message/messages/fastq_scout_message.py
+-rw-r--r--   0        0        0      594 2024-03-04 07:52:11.709385 cg-59.9.1/cg/services/delivery_message/messages/microsalt_mwr_message.py
+-rw-r--r--   0        0        0      582 2024-03-04 07:52:11.709385 cg-59.9.1/cg/services/delivery_message/messages/microsalt_mwx_message.py
+-rw-r--r--   0        0        0      415 2024-03-04 07:52:11.709385 cg-59.9.1/cg/services/delivery_message/messages/scout_message.py
+-rw-r--r--   0        0        0      408 2024-03-04 07:52:11.709385 cg-59.9.1/cg/services/delivery_message/messages/statina_message.py
+-rw-r--r--   0        0        0      737 2024-03-04 07:52:11.709385 cg-59.9.1/cg/services/delivery_message/messages/utils.py
+-rw-r--r--   0        0        0     2346 2024-03-04 07:52:11.709385 cg-59.9.1/cg/services/delivery_message/utils.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.709385 cg-59.9.1/cg/services/fastq_file_service/__init__.py
+-rw-r--r--   0        0        0      101 2024-03-04 07:52:11.709385 cg-59.9.1/cg/services/fastq_file_service/exceptions.py
+-rw-r--r--   0        0        0      868 2024-03-04 07:52:11.713385 cg-59.9.1/cg/services/fastq_file_service/fastq_file_service.py
+-rw-r--r--   0        0        0     2780 2024-03-04 07:52:11.713385 cg-59.9.1/cg/services/fastq_file_service/utils.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.713385 cg-59.9.1/cg/services/orders/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.713385 cg-59.9.1/cg/services/orders/order_service/__init__.py
+-rw-r--r--   0        0        0      101 2024-03-04 07:52:11.713385 cg-59.9.1/cg/services/orders/order_service/exceptions.py
+-rw-r--r--   0        0        0     2020 2024-03-04 07:52:11.713385 cg-59.9.1/cg/services/orders/order_service/order_service.py
+-rw-r--r--   0        0        0     1053 2024-03-04 07:52:11.713385 cg-59.9.1/cg/services/orders/order_service/utils.py
+-rw-r--r--   0        0        0       92 2024-03-04 07:52:11.713385 cg-59.9.1/cg/services/orders/order_status_service/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.713385 cg-59.9.1/cg/services/orders/order_status_service/dto/__init__.py
+-rw-r--r--   0        0        0      275 2024-03-04 07:52:11.713385 cg-59.9.1/cg/services/orders/order_status_service/dto/order_status_summary.py
+-rw-r--r--   0        0        0      972 2024-03-04 07:52:11.713385 cg-59.9.1/cg/services/orders/order_status_service/order_status_service.py
+-rw-r--r--   0        0        0     2316 2024-03-04 07:52:11.713385 cg-59.9.1/cg/services/orders/order_status_service/utils.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.713385 cg-59.9.1/cg/services/slurm_service/__init__.py
+-rw-r--r--   0        0        0      703 2024-03-04 07:52:11.713385 cg-59.9.1/cg/services/slurm_service/slurm_cli_service.py
+-rw-r--r--   0        0        0      242 2024-03-04 07:52:11.713385 cg-59.9.1/cg/services/slurm_service/slurm_service.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.713385 cg-59.9.1/cg/services/slurm_upload_service/__init__.py
+-rw-r--r--   0        0        0      175 2024-03-04 07:52:11.713385 cg-59.9.1/cg/services/slurm_upload_service/slurm_upload_config.py
+-rw-r--r--   0        0        0     2074 2024-03-04 07:52:11.713385 cg-59.9.1/cg/services/slurm_upload_service/slurm_upload_service.py
+-rw-r--r--   0        0        0      203 2024-03-04 07:52:11.713385 cg-59.9.1/cg/services/slurm_upload_service/utils.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.713385 cg-59.9.1/cg/store/__init__.py
+-rw-r--r--   0        0        0     7245 2024-03-04 07:52:11.713385 cg-59.9.1/cg/store/base.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.713385 cg-59.9.1/cg/store/crud/__init__.py
+-rw-r--r--   0        0        0    12932 2024-03-04 07:52:11.713385 cg-59.9.1/cg/store/crud/create.py
+-rw-r--r--   0        0        0     2144 2024-03-04 07:52:11.713385 cg-59.9.1/cg/store/crud/delete.py
+-rw-r--r--   0        0        0    77317 2024-03-04 07:52:11.713385 cg-59.9.1/cg/store/crud/read.py
+-rw-r--r--   0        0        0      837 2024-03-04 07:52:11.713385 cg-59.9.1/cg/store/crud/update.py
+-rw-r--r--   0        0        0     1662 2024-03-04 07:52:11.713385 cg-59.9.1/cg/store/database.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.713385 cg-59.9.1/cg/store/filters/__init__.py
+-rw-r--r--   0        0        0     5371 2024-03-04 07:52:11.713385 cg-59.9.1/cg/store/filters/status_analysis_filters.py
+-rw-r--r--   0        0        0     1712 2024-03-04 07:52:11.713385 cg-59.9.1/cg/store/filters/status_application_filters.py
+-rw-r--r--   0        0        0     1440 2024-03-04 07:52:11.713385 cg-59.9.1/cg/store/filters/status_application_limitations_filters.py
+-rw-r--r--   0        0        0     2523 2024-03-04 07:52:11.713385 cg-59.9.1/cg/store/filters/status_application_version_filters.py
+-rw-r--r--   0        0        0     1390 2024-03-04 07:52:11.713385 cg-59.9.1/cg/store/filters/status_bed_filters.py
+-rw-r--r--   0        0        0     1317 2024-03-04 07:52:11.713385 cg-59.9.1/cg/store/filters/status_bed_version_filters.py
+-rw-r--r--   0        0        0    10384 2024-03-04 07:52:11.713385 cg-59.9.1/cg/store/filters/status_case_filters.py
+-rw-r--r--   0        0        0     1461 2024-03-04 07:52:11.713385 cg-59.9.1/cg/store/filters/status_case_sample_filters.py
+-rw-r--r--   0        0        0      903 2024-03-04 07:52:11.713385 cg-59.9.1/cg/store/filters/status_collaboration_filters.py
+-rw-r--r--   0        0        0     1412 2024-03-04 07:52:11.713385 cg-59.9.1/cg/store/filters/status_customer_filters.py
+-rw-r--r--   0        0        0     1880 2024-03-04 07:52:11.713385 cg-59.9.1/cg/store/filters/status_flow_cell_filters.py
+-rw-r--r--   0        0        0     1255 2024-03-04 07:52:11.713385 cg-59.9.1/cg/store/filters/status_invoice_filters.py
+-rw-r--r--   0        0        0     2792 2024-03-04 07:52:11.713385 cg-59.9.1/cg/store/filters/status_metrics_filters.py
+-rw-r--r--   0        0        0     2304 2024-03-04 07:52:11.713385 cg-59.9.1/cg/store/filters/status_order_filters.py
+-rw-r--r--   0        0        0      851 2024-03-04 07:52:11.713385 cg-59.9.1/cg/store/filters/status_organism_filters.py
+-rw-r--r--   0        0        0      783 2024-03-04 07:52:11.713385 cg-59.9.1/cg/store/filters/status_panel_filters.py
+-rw-r--r--   0        0        0     3923 2024-03-04 07:52:11.713385 cg-59.9.1/cg/store/filters/status_pool_filters.py
+-rw-r--r--   0        0        0     8660 2024-03-04 07:52:11.713385 cg-59.9.1/cg/store/filters/status_sample_filters.py
+-rw-r--r--   0        0        0      731 2024-03-04 07:52:11.713385 cg-59.9.1/cg/store/filters/status_user_filters.py
+-rw-r--r--   0        0        0    37068 2024-03-04 07:52:11.713385 cg-59.9.1/cg/store/models.py
+-rw-r--r--   0        0        0      593 2024-03-04 07:52:11.713385 cg-59.9.1/cg/store/store.py
+-rw-r--r--   0        0        0       30 2024-03-04 07:52:11.713385 cg-59.9.1/cg/utils/__init__.py
+-rw-r--r--   0        0        0      187 2024-03-04 07:52:11.713385 cg-59.9.1/cg/utils/calculations.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.713385 cg-59.9.1/cg/utils/checksum/__init__.py
+-rw-r--r--   0        0        0     1579 2024-03-04 07:52:11.713385 cg-59.9.1/cg/utils/checksum/checksum.py
+-rw-r--r--   0        0        0     1655 2024-03-04 07:52:11.713385 cg-59.9.1/cg/utils/click/EnumChoice.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.713385 cg-59.9.1/cg/utils/click/__init__.py
+-rw-r--r--   0        0        0     4910 2024-03-04 07:52:11.713385 cg-59.9.1/cg/utils/commands.py
+-rw-r--r--   0        0        0     1811 2024-03-04 07:52:11.713385 cg-59.9.1/cg/utils/date.py
+-rw-r--r--   0        0        0      635 2024-03-04 07:52:11.713385 cg-59.9.1/cg/utils/dict.py
+-rw-r--r--   0        0        0     2111 2024-03-04 07:52:11.713385 cg-59.9.1/cg/utils/dispatcher.py
+-rw-r--r--   0        0        0     1251 2024-03-04 07:52:11.713385 cg-59.9.1/cg/utils/email.py
+-rw-r--r--   0        0        0      134 2024-03-04 07:52:11.713385 cg-59.9.1/cg/utils/enums.py
+-rw-r--r--   0        0        0     3178 2024-03-04 07:52:11.713385 cg-59.9.1/cg/utils/files.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.713385 cg-59.9.1/cg/utils/flask/__init__.py
+-rw-r--r--   0        0        0     1052 2024-03-04 07:52:11.713385 cg-59.9.1/cg/utils/flask/enum.py
+-rw-r--r--   0        0        0      834 2024-03-04 07:52:11.713385 cg-59.9.1/cg/utils/time.py
+-rw-r--r--   0        0        0     1224 2024-03-04 07:52:11.713385 cg-59.9.1/cg/utils/utils.py
+-rw-r--r--   0        0        0     1678 2024-03-04 07:52:11.717385 cg-59.9.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.717385 cg-59.9.1/tests/__init__.py
+-rw-r--r--   0        0        0     1158 2024-03-04 07:52:11.717385 cg-59.9.1/tests/apps/conftest.py
+-rw-r--r--   0        0        0      231 2024-03-04 07:52:11.717385 cg-59.9.1/tests/apps/coverage/conftest.py
+-rw-r--r--   0        0        0     6188 2024-03-04 07:52:11.717385 cg-59.9.1/tests/apps/coverage/test_coverage.py
+-rw-r--r--   0        0        0     1693 2024-03-04 07:52:11.717385 cg-59.9.1/tests/apps/crunchy/conftest.py
+-rw-r--r--   0        0        0     5438 2024-03-04 07:52:11.717385 cg-59.9.1/tests/apps/crunchy/test_compress_fastq.py
+-rw-r--r--   0        0        0     2283 2024-03-04 07:52:11.717385 cg-59.9.1/tests/apps/crunchy/test_config.py
+-rw-r--r--   0        0        0    14032 2024-03-04 07:52:11.717385 cg-59.9.1/tests/apps/crunchy/test_crunchy.py
+-rw-r--r--   0        0        0     9109 2024-03-04 07:52:11.717385 cg-59.9.1/tests/apps/crunchy/test_spring_decompression.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.717385 cg-59.9.1/tests/apps/demultiplex/__init__.py
+-rw-r--r--   0        0        0    10776 2024-03-04 07:52:11.717385 cg-59.9.1/tests/apps/demultiplex/conftest.py
+-rw-r--r--   0        0        0     8944 2024-03-04 07:52:11.717385 cg-59.9.1/tests/apps/demultiplex/test_demultiplex_api.py
+-rw-r--r--   0        0        0     6098 2024-03-04 07:52:11.717385 cg-59.9.1/tests/apps/demultiplex/test_index.py
+-rw-r--r--   0        0        0     9468 2024-03-04 07:52:11.717385 cg-59.9.1/tests/apps/demultiplex/test_override_cycles_validator.py
+-rw-r--r--   0        0        0     6074 2024-03-04 07:52:11.717385 cg-59.9.1/tests/apps/demultiplex/test_read_sample_sheet.py
+-rw-r--r--   0        0        0    15738 2024-03-04 07:52:11.717385 cg-59.9.1/tests/apps/demultiplex/test_sample_models.py
+-rw-r--r--   0        0        0     4516 2024-03-04 07:52:11.717385 cg-59.9.1/tests/apps/demultiplex/test_sample_sheet_creator.py
+-rw-r--r--   0        0        0     2244 2024-03-04 07:52:11.717385 cg-59.9.1/tests/apps/demultiplex/test_sample_sheet_creator_factory.py
+-rw-r--r--   0        0        0     3271 2024-03-04 07:52:11.717385 cg-59.9.1/tests/apps/demultiplex/test_sample_sheet_models.py
+-rw-r--r--   0        0        0    11331 2024-03-04 07:52:11.717385 cg-59.9.1/tests/apps/demultiplex/test_sample_sheet_validator.py
+-rw-r--r--   0        0        0     1495 2024-03-04 07:52:11.717385 cg-59.9.1/tests/apps/demultiplex/test_validate.py
+-rw-r--r--   0        0        0     5094 2024-03-04 07:52:11.717385 cg-59.9.1/tests/apps/downsample/test_downsample.py
+-rw-r--r--   0        0        0     1419 2024-03-04 07:52:11.717385 cg-59.9.1/tests/apps/downsample/test_downsample_utils.py
+-rw-r--r--   0        0        0     1716 2024-03-04 07:52:11.717385 cg-59.9.1/tests/apps/gens/test_gens_api.py
+-rw-r--r--   0        0        0     1950 2024-03-04 07:52:11.717385 cg-59.9.1/tests/apps/gt/conftest.py
+-rw-r--r--   0        0        0     4276 2024-03-04 07:52:11.717385 cg-59.9.1/tests/apps/gt/test_gt_api.py
+-rw-r--r--   0        0        0     1453 2024-03-04 07:52:11.717385 cg-59.9.1/tests/apps/hk/conftest.py
+-rw-r--r--   0        0        0      684 2024-03-04 07:52:11.717385 cg-59.9.1/tests/apps/hk/test__getattr__.py
+-rw-r--r--   0        0        0     1593 2024-03-04 07:52:11.717385 cg-59.9.1/tests/apps/hk/test_add_file.py
+-rw-r--r--   0        0        0     3523 2024-03-04 07:52:11.717385 cg-59.9.1/tests/apps/hk/test_bundles.py
+-rw-r--r--   0        0        0      871 2024-03-04 07:52:11.717385 cg-59.9.1/tests/apps/hk/test_core.py
+-rw-r--r--   0        0        0    24975 2024-03-04 07:52:11.717385 cg-59.9.1/tests/apps/hk/test_file.py
+-rw-r--r--   0        0        0     5080 2024-03-04 07:52:11.717385 cg-59.9.1/tests/apps/hk/test_version.py
+-rw-r--r--   0        0        0     1840 2024-03-04 07:52:11.717385 cg-59.9.1/tests/apps/lims/conftest.py
+-rw-r--r--   0        0        0     3197 2024-03-04 07:52:11.717385 cg-59.9.1/tests/apps/lims/test_api.py
+-rw-r--r--   0        0        0     1451 2024-03-04 07:52:11.717385 cg-59.9.1/tests/apps/lims/test_sample_sheet.py
+-rw-r--r--   0        0        0     9223 2024-03-04 07:52:11.717385 cg-59.9.1/tests/apps/loqus/conftest.py
+-rw-r--r--   0        0        0     8994 2024-03-04 07:52:11.717385 cg-59.9.1/tests/apps/loqus/test_loqusdb_api.py
+-rw-r--r--   0        0        0     2439 2024-03-04 07:52:11.717385 cg-59.9.1/tests/apps/madeline/conftest.py
+-rw-r--r--   0        0        0     4653 2024-03-04 07:52:11.717385 cg-59.9.1/tests/apps/madeline/test_madeline.py
+-rw-r--r--   0        0        0     3328 2024-03-04 07:52:11.717385 cg-59.9.1/tests/apps/mip/conftest.py
+-rw-r--r--   0        0        0     2487 2024-03-04 07:52:11.717385 cg-59.9.1/tests/apps/mip/test_config_mip.py
+-rw-r--r--   0        0        0      883 2024-03-04 07:52:11.721385 cg-59.9.1/tests/apps/mutacc_auto/conftest.py
+-rw-r--r--   0        0        0     2473 2024-03-04 07:52:11.721385 cg-59.9.1/tests/apps/mutacc_auto/test_mutacc_auto.py
+-rw-r--r--   0        0        0    11930 2024-03-04 07:52:11.721385 cg-59.9.1/tests/apps/orderform/conftest.py
+-rw-r--r--   0        0        0     9484 2024-03-04 07:52:11.721385 cg-59.9.1/tests/apps/orderform/test_excel_orderform_parser.py
+-rw-r--r--   0        0        0     4351 2024-03-04 07:52:11.721385 cg-59.9.1/tests/apps/orderform/test_excel_sample_schema.py
+-rw-r--r--   0        0        0     1032 2024-03-04 07:52:11.721385 cg-59.9.1/tests/apps/orderform/test_json_orderform_parser.py
+-rw-r--r--   0        0        0     2474 2024-03-04 07:52:11.721385 cg-59.9.1/tests/apps/orderform/test_orderform_parser.py
+-rw-r--r--   0        0        0    16002 2024-03-04 07:52:11.721385 cg-59.9.1/tests/apps/orderform/validators/test_excel_sample_validators.py
+-rw-r--r--   0        0        0     3670 2024-03-04 07:52:11.721385 cg-59.9.1/tests/apps/scout/conftest.py
+-rw-r--r--   0        0        0     2269 2024-03-04 07:52:11.721385 cg-59.9.1/tests/apps/scout/test_get_causative_variants.py
+-rw-r--r--   0        0        0     1376 2024-03-04 07:52:11.721385 cg-59.9.1/tests/apps/scout/test_get_scout_cases.py
+-rw-r--r--   0        0        0     1840 2024-03-04 07:52:11.721385 cg-59.9.1/tests/apps/scout/test_scout_load_config.py
+-rw-r--r--   0        0        0     7047 2024-03-04 07:52:11.721385 cg-59.9.1/tests/apps/scout/test_scout_models.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.721385 cg-59.9.1/tests/apps/sequencing_metrics_parser/__init__.py
+-rw-r--r--   0        0        0     2861 2024-03-04 07:52:11.721385 cg-59.9.1/tests/apps/sequencing_metrics_parser/conftest.py
+-rw-r--r--   0        0        0     2010 2024-03-04 07:52:11.721385 cg-59.9.1/tests/apps/sequencing_metrics_parser/parsers/conftest.py
+-rw-r--r--   0        0        0     1820 2024-03-04 07:52:11.721385 cg-59.9.1/tests/apps/sequencing_metrics_parser/parsers/test_bcl2fastq_parser.py
+-rw-r--r--   0        0        0     1908 2024-03-04 07:52:11.721385 cg-59.9.1/tests/apps/sequencing_metrics_parser/parsers/test_bcl2fastq_to_sequencing_statistics.py
+-rw-r--r--   0        0        0     2997 2024-03-04 07:52:11.721385 cg-59.9.1/tests/apps/sequencing_metrics_parser/parsers/test_bcl_convert_to_sequencing_statistics.py
+-rw-r--r--   0        0        0     7322 2024-03-04 07:52:11.721385 cg-59.9.1/tests/apps/sequencing_metrics_parser/parsers/test_bclconvert.py
+-rw-r--r--   0        0        0     1458 2024-03-04 07:52:11.721385 cg-59.9.1/tests/apps/sequencing_metrics_parser/test_sequencing_metrics_calculator.py
+-rw-r--r--   0        0        0     1131 2024-03-04 07:52:11.721385 cg-59.9.1/tests/apps/slurm/conftest.py
+-rw-r--r--   0        0        0     4412 2024-03-04 07:52:11.721385 cg-59.9.1/tests/apps/slurm/test_slurm_api.py
+-rw-r--r--   0        0        0      831 2024-03-04 07:52:11.721385 cg-59.9.1/tests/apps/test_apps_environ.py
+-rw-r--r--   0        0        0      957 2024-03-04 07:52:11.721385 cg-59.9.1/tests/apps/test_osticket.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/add/__init__.py
+-rw-r--r--   0        0        0     1174 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/add/test_cli_add.py
+-rw-r--r--   0        0        0     2471 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/add/test_cli_add_customer.py
+-rw-r--r--   0        0        0     6747 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/add/test_cli_add_family.py
+-rw-r--r--   0        0        0     7588 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/add/test_cli_add_relationship.py
+-rw-r--r--   0        0        0     7694 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/add/test_cli_add_sample.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/backup/__init__.py
+-rw-r--r--   0        0        0      705 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/backup/conftest.py
+-rw-r--r--   0        0        0    11101 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/backup/test_backup_command.py
+-rw-r--r--   0        0        0     6865 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/clean/conftest.py
+-rw-r--r--   0        0        0     5536 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/clean/test_balsamic_clean.py
+-rw-r--r--   0        0        0     2557 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/clean/test_clean_flow_cell.py
+-rw-r--r--   0        0        0     1830 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/clean/test_clean_hk_bundle_files.py
+-rw-r--r--   0        0        0     2098 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/clean/test_hk_bundle_files.py
+-rw-r--r--   0        0        0     4610 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/clean/test_hk_case_bundle_files.py
+-rw-r--r--   0        0        0     3585 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/clean/test_microbial_clean.py
+-rw-r--r--   0        0        0     1881 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/clean/test_rsync_past_run_dirs.py
+-rw-r--r--   0        0        0     9707 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/compress/conftest.py
+-rw-r--r--   0        0        0     7709 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/compress/test_cli_compress_fastq.py
+-rw-r--r--   0        0        0     1416 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/compress/test_cli_decompress_spring.py
+-rw-r--r--   0        0        0     5205 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/compress/test_compress_helpers.py
+-rw-r--r--   0        0        0     1239 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/compress/test_store_fastq.py
+-rw-r--r--   0        0        0     7558 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/conftest.py
+-rw-r--r--   0        0        0    12747 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/delete/test_cli_delete_case.py
+-rw-r--r--   0        0        0     1873 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/delete/test_cli_delete_cases.py
+-rw-r--r--   0        0        0     3794 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/deliver/conftest.py
+-rw-r--r--   0        0        0     4630 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/deliver/test_deliver_base.py
+-rw-r--r--   0        0        0     1166 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/deliver/test_rsync_base.py
+-rw-r--r--   0        0        0     8569 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/deliver/test_run_deliver_cmd.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/demultiplex/__init__.py
+-rw-r--r--   0        0        0     9244 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/demultiplex/test_create_sample_sheet.py
+-rw-r--r--   0        0        0     8683 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/demultiplex/test_demultiplex_flowcell.py
+-rw-r--r--   0        0        0     1607 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/demultiplex/test_finish_demux.py
+-rw-r--r--   0        0        0     3704 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/demultiplex/test_validate_sample_sheet.py
+-rw-r--r--   0        0        0     4423 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/demultiplex/test_verify_syncing.py
+-rw-r--r--   0        0        0     1585 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/downsample/test_cli_downsample.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/generate/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/generate/report/__init__.py
+-rw-r--r--   0        0        0     1622 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/generate/report/conftest.py
+-rw-r--r--   0        0        0     2477 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/generate/report/test_cli_delivery_report.py
+-rw-r--r--   0        0        0     2760 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/generate/report/test_utils.py
+-rw-r--r--   0        0        0      563 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/generate/test_cli_base.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/get/__init__.py
+-rw-r--r--   0        0        0      863 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/get/test_cli_get.py
+-rw-r--r--   0        0        0     1526 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/get/test_cli_get_analysis.py
+-rw-r--r--   0        0        0     1242 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/get/test_cli_get_case.py
+-rw-r--r--   0        0        0     6208 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/get/test_cli_get_flow_cell.py
+-rw-r--r--   0        0        0     8835 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/get/test_cli_get_sample.py
+-rw-r--r--   0        0        0     1364 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/set/conftest.py
+-rw-r--r--   0        0        0     7311 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/set/test_cli_set_case.py
+-rw-r--r--   0        0        0     1460 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/set/test_cli_set_cases.py
+-rw-r--r--   0        0        0     2016 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/set/test_cli_set_flowcell.py
+-rw-r--r--   0        0        0     1685 2024-03-04 07:52:11.721385 cg-59.9.1/tests/cli/set/test_cli_set_list_keys.py
+-rw-r--r--   0        0        0    12450 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/set/test_cli_set_sample.py
+-rw-r--r--   0        0        0     6124 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/set/test_cli_set_samples.py
+-rw-r--r--   0        0        0     6934 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/store/test_fastq.py
+-rw-r--r--   0        0        0     2332 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/test_base.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/upload/__init__.py
+-rw-r--r--   0        0        0    10003 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/upload/conftest.py
+-rw-r--r--   0        0        0     2295 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/upload/test_cli_scout.py
+-rw-r--r--   0        0        0     1789 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/upload/test_cli_upload.py
+-rw-r--r--   0        0        0      971 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/upload/test_cli_upload_auto.py
+-rw-r--r--   0        0        0     1669 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/upload/test_cli_upload_delivery_report.py
+-rw-r--r--   0        0        0      895 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/upload/test_cli_upload_fastq.py
+-rw-r--r--   0        0        0     1199 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/upload/test_cli_upload_genotype.py
+-rw-r--r--   0        0        0      694 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/upload/test_cli_upload_gens.py
+-rw-r--r--   0        0        0     9965 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/upload/test_cli_upload_nipt.py
+-rw-r--r--   0        0        0     4684 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/upload/test_cli_upload_nipt_ftp.py
+-rw-r--r--   0        0        0     1839 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/upload/test_cli_upload_nipt_statina.py
+-rw-r--r--   0        0        0     6177 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/upload/test_cli_upload_observations.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/__init__.py
+-rw-r--r--   0        0        0    30612 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/balsamic/conftest.py
+-rw-r--r--   0        0        0    13938 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/balsamic/test_cli_balsamic_config_case.py
+-rw-r--r--   0        0        0     7957 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/balsamic/test_compound_commands.py
+-rw-r--r--   0        0        0     2336 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/balsamic/test_link.py
+-rw-r--r--   0        0        0     3554 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/balsamic/test_report_deliver.py
+-rw-r--r--   0        0        0     6209 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/balsamic/test_run.py
+-rw-r--r--   0        0        0     6934 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/balsamic/test_store_housekeeper.py
+-rw-r--r--   0        0        0     8458 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/conftest.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/fastq/__init__.py
+-rw-r--r--   0        0        0     2298 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/fastq/test_fastq_base.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/fluffy/__init__.py
+-rw-r--r--   0        0        0     5291 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/fluffy/conftest.py
+-rw-r--r--   0        0        0     5687 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/fluffy/test_cli_create_samplesheet.py
+-rw-r--r--   0        0        0     3302 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/fluffy/test_cli_link.py
+-rw-r--r--   0        0        0     1896 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/fluffy/test_cli_run.py
+-rw-r--r--   0        0        0     2968 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/fluffy/test_cli_start.py
+-rw-r--r--   0        0        0     7815 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/fluffy/test_cli_store.py
+-rw-r--r--   0        0        0     2775 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/microsalt/conftest.py
+-rw-r--r--   0        0        0     6926 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/microsalt/test_microsalt_case_config.py
+-rw-r--r--   0        0        0     1000 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/microsalt/test_microsalt_run.py
+-rw-r--r--   0        0        0     6544 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/mip/conftest.py
+-rw-r--r--   0        0        0     7011 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/mip/test_cli_mip_base.py
+-rw-r--r--   0        0        0     1542 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/mip/test_cli_mip_dna_config_case.py
+-rw-r--r--   0        0        0      431 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/mip/test_cli_mip_dna_link.py
+-rw-r--r--   0        0        0     2108 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/mip/test_cli_mip_dna_manged_variants.py
+-rw-r--r--   0        0        0     1273 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/mip/test_cli_mip_dna_panel.py
+-rw-r--r--   0        0        0     3595 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/mip/test_cli_mip_dna_run.py
+-rw-r--r--   0        0        0     3884 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/mip/test_cli_mip_dna_start.py
+-rw-r--r--   0        0        0     1004 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/mip/test_cli_mip_rna_config_case.py
+-rw-r--r--   0        0        0      527 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/mip/test_cli_mip_rna_link.py
+-rw-r--r--   0        0        0      716 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/mip/test_cli_mip_rna_run.py
+-rw-r--r--   0        0        0     8559 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/mip/test_cli_mip_store.py
+-rw-r--r--   0        0        0     1864 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/nf_analysis/test_cli_config_case.py
+-rw-r--r--   0        0        0     1927 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/nf_analysis/test_cli_metrics_deliver.py
+-rw-r--r--   0        0        0     5075 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/nf_analysis/test_cli_report_deliver.py
+-rw-r--r--   0        0        0     4498 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/raredisease/test_cli_raredisease_compound_commands.py
+-rw-r--r--   0        0        0     9843 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/rnafusion/test_cli_rnafusion_compound_commands.py
+-rw-r--r--   0        0        0     5887 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/rnafusion/test_cli_rnafusion_config_case.py
+-rw-r--r--   0        0        0     1602 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/rnafusion/test_cli_rnafusion_metrics_deliver.py
+-rw-r--r--   0        0        0     7899 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/rnafusion/test_cli_rnafusion_run.py
+-rw-r--r--   0        0        0     8710 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/rnafusion/test_cli_rnafusion_store_housekeeper.py
+-rw-r--r--   0        0        0     2409 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/taxprofiler/test_cli_taxprofiler_compound_commands.py
+-rw-r--r--   0        0        0     3302 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/taxprofiler/test_cli_taxprofiler_config_case.py
+-rw-r--r--   0        0        0     1521 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/taxprofiler/test_cli_taxprofiler_metrics_deliver.py
+-rw-r--r--   0        0        0     3933 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/taxprofiler/test_cli_taxprofiler_run.py
+-rw-r--r--   0        0        0      837 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/test_cli_workflow.py
+-rw-r--r--   0        0        0     4310 2024-03-04 07:52:11.725385 cg-59.9.1/tests/cli/workflow/test_cli_workflow_clean.py
+-rw-r--r--   0        0        0     2346 2024-03-04 07:52:11.725385 cg-59.9.1/tests/clients/conftest.py
+-rw-r--r--   0        0        0     1812 2024-03-04 07:52:11.725385 cg-59.9.1/tests/clients/janus/test_janus_api_client.py
+-rw-r--r--   0        0        0   100013 2024-03-04 07:52:11.725385 cg-59.9.1/tests/conftest.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.725385 cg-59.9.1/tests/fixture_plugins/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.725385 cg-59.9.1/tests/fixture_plugins/demultiplex_fixtures/__init__.py
+-rw-r--r--   0        0        0     4867 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixture_plugins/demultiplex_fixtures/flow_cell_fixtures.py
+-rw-r--r--   0        0        0     3686 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixture_plugins/demultiplex_fixtures/name_fixtures.py
+-rw-r--r--   0        0        0    21233 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixture_plugins/demultiplex_fixtures/path_fixtures.py
+-rw-r--r--   0        0        0     3699 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixture_plugins/demultiplex_fixtures/run_parameters_fixtures.py
+-rw-r--r--   0        0        0     4385 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixture_plugins/demultiplex_fixtures/sample_fixtures.py
+-rw-r--r--   0        0        0     5824 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixture_plugins/demultiplex_fixtures/sample_sheet_fixtures.py
+-rw-r--r--   0        0        0     1304 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixture_plugins/timestamp_fixtures.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/analysis/balsamic/tn_wgs/adm1.cram
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/analysis/balsamic/tn_wgs/ascat.output.pdf
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/analysis/balsamic/tn_wgs/snv.vcf
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/analysis/balsamic/tn_wgs/sv.vcf
+-rw-r--r--   0        0        0    14644 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/ACC11111_qc_fail.json
+-rw-r--r--   0        0        0    15921 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/ACC22222_qc_pass.json
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/analysis/mip/dna/ADM1.baf.bed.gz
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/analysis/mip/dna/ADM1.cov.bed.gz
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/analysis/mip/dna/ADM2.cram
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/analysis/mip/dna/ADM3.cram
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/analysis/mip/dna/adm1.cram
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/analysis/mip/dna/adm1.mt.bam
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/analysis/mip/dna/multiqc.html
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/analysis/mip/dna/report.pdf
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/analysis/mip/dna/smn.vcf
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/analysis/mip/dna/snv.vcf
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/analysis/mip/dna/snv_research.vcf
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/analysis/mip/dna/str.vcf
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/analysis/mip/dna/sv.vcf
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/analysis/mip/dna/sv_research.vcf
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/analysis/mip/dna/vcf2cytosure.txt
+-rw-r--r--   0        0        0     5497 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/analysis/rnafusion/multiqc_data.json
+-rw-r--r--   0        0        0    11711 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/analysis/rnafusion/rnafusion_case_enough_reads_metrics_deliverables.yaml
+-rw-r--r--   0        0        0     2873 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/analysis/sample_coverage.bed
+-rw-r--r--   0        0        0     6506 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/analysis/taxprofiler/multiqc_data.json
+-rw-r--r--   0        0        0    10513 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/analysis/taxprofiler/taxprofiler_case_metrics_deliverables.yaml
+-rw-r--r--   0        0        0    10961 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/balsamic/case/config.json
+-rw-r--r--   0        0        0     3465 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/balsamic/case/metadata.yml
+-rw-r--r--   0        0        0       63 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/balsamic/case/metadata_directory.yml
+-rw-r--r--   0        0        0      165 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/balsamic/case/metadata_file_tags.yml
+-rw-r--r--   0        0        0     2705 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/balsamic/case/metrics_deliverables.yaml
+-rw-r--r--   0        0        0      692 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/crunchy/spring_metadata.json
+-rw-r--r--   0        0        0      156 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/SampleSheet.csv
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/Unaligned/Project_150031/Sample_SVE2528A1_CTGAAGCT/HHKVCALXX-l1t11_150031_S5_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/Unaligned/Project_150031/Sample_SVE2528A1_CTGAAGCT/HHKVCALXX-l1t11_150031_S5_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/Unaligned/Project_150031/Sample_SVE2528A1_CTGAAGCT/HHKVCALXX-l1t21_150031_S5_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/Unaligned/Project_150031/Sample_SVE2528A1_CTGAAGCT/HHKVCALXX-l1t21_150031_S5_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/Undetermined_S0_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/Undetermined_S0_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/demuxcomplete.txt
+-rw-r--r--   0        0        0     1781 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/l1t11/Stats/Stats.json
+-rw-r--r--   0        0        0     2532 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/l1t21/Stats/Stats.json
+-rw-r--r--   0        0        0     1757 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
+-rw-r--r--   0        0        0        7 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/SampleSheet.csv
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/HN3FKDSXY_AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/HN3FKDSXY_AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0     6034 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml
+-rw-r--r--   0        0        0     1172 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml
+-rw-r--r--   0        0        0        7 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/fastq_1.fastq.gz
+-rw-r--r--   0        0        0        7 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/fastq_2.fastq.gz
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/BCLConvert/fastq/ACC11927A2_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/BCLConvert/fastq/ACC11927A2_S1_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/BCLConvert/fastq/ACC11927A2_S1_L002_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/BCLConvert/fastq/ACC11927A2_S1_L002_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/BCLConvert/fastq/ACC11927A5_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/BCLConvert/fastq/ACC11927A5_S1_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/BCLConvert/fastq/ACC11927A5_S1_L002_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/BCLConvert/fastq/ACC11927A5_S1_L002_R2_001.fastq.gz
+-rw-r--r--   0        0        0      345 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/Reports/Adapter_Metrics.csv
+-rw-r--r--   0        0        0      650 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/Reports/Demultiplex_Stats.csv
+-rw-r--r--   0        0        0      896 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/Reports/Quality_Metrics.csv
+-rw-r--r--   0        0        0      602 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/SampleSheet.csv
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/demuxcomplete.txt
+-rw-r--r--   0        0        0      315 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRZZ/Unaligned/Reports/Adapter_Metrics.csv
+-rw-r--r--   0        0        0      434 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRZZ/Unaligned/Reports/Quality_Metrics.csv
+-rw-r--r--   0        0        0     8624 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRZZ/Unaligned/Reports/RunInfo.xml
+-rw-r--r--   0        0        0      568 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/SampleSheet.csv
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A2/HY7FFDRX2_ACC11927A2_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A2/HY7FFDRX2_ACC11927A2_S1_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A2/HY7FFDRX2_ACC11927A2_S1_L002_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A2/HY7FFDRX2_ACC11927A2_S1_L002_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A5/HY7FFDRX2_ACC11927A5_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A5/HY7FFDRX2_ACC11927A5_S1_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A5/HY7FFDRX2_ACC11927A5_S1_L002_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Project_405887/Sample_ACC11927A5/HY7FFDRX2_ACC11927A5_S1_L002_R2_001.fastq.gz
+-rw-r--r--   0        0        0      220 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Reports/Adapter_Metrics.csv
+-rw-r--r--   0        0        0      463 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Reports/Demultiplex_Stats.csv
+-rw-r--r--   0        0        0      622 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Reports/Quality_Metrics.csv
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Undetermined_S0_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/demuxcomplete.txt
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A2_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A2_S1_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A2_S1_L002_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A2_S1_L002_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A5_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A5_S1_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A5_S1_L002_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/BCLConvert/fastq/ACC11927A5_S1_L002_R2_001.fastq.gz
+-rw-r--r--   0        0        0      345 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/Reports/Adapter_Metrics.csv
+-rw-r--r--   0        0        0      650 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/Reports/Demultiplex_Stats.csv
+-rw-r--r--   0        0        0      896 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/Reports/Quality_Metrics.csv
+-rw-r--r--   0        0        0      619 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/SampleSheet.csv
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/demuxcomplete.txt
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0     4439 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml
+-rw-r--r--   0        0        0     1172 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L001_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L001_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L002_R1_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.729385 cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L002_R2_001.fastq.gz
+-rw-r--r--   0        0        0       43 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/fastq/dummy_run_R1_001.fastq.gz
+-rw-r--r--   0        0        0       67 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/fastq/dummy_run_R1_001.fastq.gz.md5
+-rw-r--r--   0        0        0   338370 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/fastq/fastq_run_R1_001.fastq.gz
+-rw-r--r--   0        0        0       67 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/fastq/fastq_run_R1_001.fastq.gz.md5
+-rw-r--r--   0        0        0   338349 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/fastq/fastq_run_R2_001.fastq.gz
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/CopyComplete.txt
+-rw-r--r--   0        0        0     2126 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/HJCFFALXX_bcl2fastq_raw.json
+-rw-r--r--   0        0        0     1827 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/HJCFFALXX_bcl_convert_raw.json
+-rw-r--r--   0        0        0       90 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/README.txt
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTAComplete.txt
+-rw-r--r--   0        0        0     6895 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTAConfiguration.xml
+-rw-r--r--   0        0        0       37 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTARead1Complete.txt
+-rw-r--r--   0        0        0       36 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTARead2Complete.txt
+-rw-r--r--   0        0        0       36 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTARead3Complete.txt
+-rw-r--r--   0        0        0    24755 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RunInfo.xml
+-rw-r--r--   0        0        0      692 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet.csv
+-rw-r--r--   0        0        0      724 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet_bcl2fastq.csv
+-rw-r--r--   0        0        0       61 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/SequencingComplete.txt
+-rw-r--r--   0        0        0     5775 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/runParameters.xml
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/CopyComplete.txt
+-rw-r--r--   0        0        0     2282 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/HL32LCCXY_bcl2fastq_raw.json
+-rw-r--r--   0        0        0     1632 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/HL32LCCXY_bcl_convert_raw.json
+-rw-r--r--   0        0        0       75 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/README.txt
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTAComplete.txt
+-rw-r--r--   0        0        0     6912 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTAConfiguration.xml
+-rw-r--r--   0        0        0       36 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTARead1Complete.txt
+-rw-r--r--   0        0        0       36 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTARead2Complete.txt
+-rw-r--r--   0        0        0       36 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTARead3Complete.txt
+-rw-r--r--   0        0        0       36 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTARead4Complete.txt
+-rw-r--r--   0        0        0    24814 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RunInfo.xml
+-rw-r--r--   0        0        0      814 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/SampleSheet.csv
+-rw-r--r--   0        0        0      660 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/SampleSheet_bcl2fastq.csv
+-rw-r--r--   0        0        0       61 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/SequencingComplete.txt
+-rw-r--r--   0        0        0     5853 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/runParameters.xml
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/CopyComplete.txt
+-rw-r--r--   0        0        0    21848 2024-03-04 07:52:11.733385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/HGYFNBCX2_bcl2fastq_raw.json
+-rw-r--r--   0        0        0    15512 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/HGYFNBCX2_bcl_convert_raw.json
+-rw-r--r--   0        0        0       79 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/README.txt
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/RTAComplete.txt
+-rw-r--r--   0        0        0      756 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/RunInfo.xml
+-rw-r--r--   0        0        0     4118 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/SampleSheet.csv
+-rw-r--r--   0        0        0     1408 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/SampleSheet_bcl2fastq.csv
+-rw-r--r--   0        0        0     5326 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/runParameters.xml
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/CopyComplete.txt
+-rw-r--r--   0        0        0    15041 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/HM2LNBCX2_bcl2fastq_raw.json
+-rw-r--r--   0        0        0    10649 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/HM2LNBCX2_bcl_convert_raw.json
+-rw-r--r--   0        0        0       80 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/README.txt
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/RTAComplete.txt
+-rw-r--r--   0        0        0      755 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/RunInfo.xml
+-rw-r--r--   0        0        0     2878 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/SampleSheet.csv
+-rw-r--r--   0        0        0      928 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/SampleSheet_bcl2fastq.csv
+-rw-r--r--   0        0        0     5359 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/runParameters.xml
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/CopyComplete.txt
+-rw-r--r--   0        0        0    27887 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/CorrectSampleSheet.csv
+-rw-r--r--   0        0        0   141870 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/HLYWYDSXX_bcl2fastq_raw.json
+-rwxr-xr-x   0        0        0   122682 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/HLYWYDSXX_bcl_convert_raw.json
+-rw-r--r--   0        0        0      243 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/README.txt
+-rw-r--r--   0        0        0    28230 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RTA3.cfg
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RTAComplete.txt
+-rw-r--r--   0        0        0    94426 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RunInfo.xml
+-rw-r--r--   0        0        0     5819 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RunParameters.xml
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/SequenceComplete.txt
+-rw-r--r--   0        0        0     1757 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/HVKJCDRXX_demultiplex.stderr
+-rw-r--r--   0        0        0     1757 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/HVKJCDRXX_demultiplex.stdout
+-rw-r--r--   0        0        0       12 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/README.txt
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/RTAComplete.txt
+-rw-r--r--   0        0        0     5945 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/RunParameters.xml
+-rw-r--r--   0        0        0      260 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/SampleSheet.csv
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/copycomplete.txt
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/demuxstarted.txt
+-rw-r--r--   0        0        0     1757 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
+-rw-r--r--   0        0        0     1757 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stdout
+-rw-r--r--   0        0        0    47522 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_raw.json
+-rw-r--r--   0        0        0       12 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/README.txt
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/RTAComplete.txt
+-rw-r--r--   0        0        0     6666 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/RunParameters.xml
+-rw-r--r--   0        0        0      254 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/SampleSheet.csv
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/copycomplete.txt
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/delivery.txt
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/demuxstarted.txt
+-rwxr-xr-x   0        0        0    47434 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/22F52TLT3_raw.json
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/CopyComplete.txt
+-rw-r--r--   0        0        0    10950 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/CorrectSampleSheet.csv
+-rw-r--r--   0        0        0      225 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/Manifest.tsv
+-rw-r--r--   0        0        0       55 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/README.txt
+-rwxr-xr-x   0        0        0     2493 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RTA.cfg
+-rwxr-xr-x   0        0        0        1 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RTAComplete.txt
+-rwxr-xr-x   0        0        0        2 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RTAExited.txt
+-rwxr-xr-x   0        0        0      730 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunCompletionStatus.xml
+-rwxr-xr-x   0        0        0    79277 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunInfo.xml
+-rwxr-xr-x   0        0        0     2694 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunParameters.xml
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/CopyComplete.txt
+-rw-r--r--   0        0        0      509 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stderr
+-rw-r--r--   0        0        0     2229 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stdout
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/RTAComplete.txt
+-rw-r--r--   0        0        0     6665 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/RunParameters.xml
+-rw-r--r--   0        0        0      619 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/SampleSheet.csv
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/CopyComplete.txt
+-rw-r--r--   0        0        0      509 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stderr
+-rw-r--r--   0        0        0     2229 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout
+-rw-r--r--   0        0        0       12 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/README.txt
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/RTAComplete.txt
+-rw-r--r--   0        0        0     6665 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/RunParameters.xml
+-rw-r--r--   0        0        0      399 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/SampleSheet.csv
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/CopyComplete.txt
+-rw-r--r--   0        0        0     4941 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/CorrectSampleSheet.csv
+-rwxr-xr-x   0        0        0    20050 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/HK33MDRX3_bcl_convert_raw.json
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/HK33MDRX3_demultiplex.stderr
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/HK33MDRX3_demultiplex.stdout
+-rw-r--r--   0        0        0      244 2024-03-04 07:52:11.737385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/README.txt
+-rw-r--r--   0        0        0     6391 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RTA3.cfg
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RTAComplete.txt
+-rw-r--r--   0        0        0    16428 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RunInfo.xml
+-rw-r--r--   0        0        0     6728 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RunParameters.xml
+-rw-r--r--   0        0        0     5127 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/SampleSheet.csv
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/SequenceComplete.txt
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/demuxstarted.txt
+-rw-r--r--   0        0        0      124 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/180509_D00450_0598_BHGYFNBCX2/README.txt
+-rw-r--r--   0        0        0      310 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/190927_A00689_0069_BHLYWYDSXX/README.txt
+-rw-r--r--   0        0        0     5819 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/190927_A00689_0069_BHLYWYDSXX/RunParameters.xml
+-rw-r--r--   0        0        0      122 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/20231108_LH00188_0028_B22F52TLT3/README.txt
+-rwxr-xr-x   0        0        0     2694 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/20231108_LH00188_0028_B22F52TLT3/RunParameters.xml
+-rw-r--r--   0        0        0      311 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/230912_A00187_1009_AHK33MDRX3/README.txt
+-rw-r--r--   0        0        0     6728 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/230912_A00187_1009_AHK33MDRX3/RunParameters.xml
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/CopyComplete.txt
+-rw-r--r--   0        0        0      509 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stderr
+-rw-r--r--   0        0        0     2229 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/RTAComplete.txt
+-rw-r--r--   0        0        0     6665 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/RunParameters.xml
+-rw-r--r--   0        0        0      399 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/SampleSheet.csv
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/CopyComplete.txt
+-rw-r--r--   0        0        0      509 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stderr
+-rw-r--r--   0        0        0     2229 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stdout
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/RTAComplete.txt
+-rw-r--r--   0        0        0     6665 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/RunParameters.xml
+-rw-r--r--   0        0        0      399 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/SampleSheet.csv
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_1/20231205_1618_3B_PAS86456_72d9fceb/fastq_pass/PAS86456_pass_72d9fceb_8a4fd683_0.fastq.gz
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_1/20231205_1618_3B_PAS86456_72d9fceb/fastq_pass/PAS86456_pass_72d9fceb_8a4fd683_1.fastq.gz
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_1/20231205_1618_3B_PAS86456_72d9fceb/final_summary_PAS86456_72d9fceb_8a4fd683.txt
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_1/20231205_1618_3B_PAS86456_72d9fceb/pod5_pass/PAS86456_pass_72d9fceb_8a4fd683_0.pod5
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_1/20231205_1618_3B_PAS86456_72d9fceb/pod5_pass/PAS86456_pass_72d9fceb_8a4fd683_1.pod5
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_2/20231205_1618_3D_PAS97781_595b5663/fastq_pass/PAS97781_pass_595b5663_efc7f02e_0.fastq.gz
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_2/20231205_1618_3D_PAS97781_595b5663/fastq_pass/PAS97781_pass_595b5663_efc7f02e_1.fastq.gz
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_2/20231205_1618_3D_PAS97781_595b5663/final_summary_PAS97781_595b5663_efc7f02e.txt
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_2/20231205_1618_3D_PAS97781_595b5663/pod5_pass/PAS97781_pass_595b5663_efc7f02e_0.pod5
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/nanopore/experiment_name/sample_2/20231205_1618_3D_PAS97781_595b5663/pod5_pass/PAS97781_pass_595b5663_efc7f02e_1.pod5
+-rw-r--r--   0        0        0   111989 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/raw_lims_samples/raw_samplesheet_novaseq.json
+-rw-r--r--   0        0        0     5319 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_hiseq_2500_different_index_cycles.xml
+-rw-r--r--   0        0        0     5944 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_6000_different_index_cycles.xml
+-rwxr-xr-x   0        0        0     2481 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_X_different_index_cycles.xml
+-rwxr-xr-x   0        0        0     2474 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_X_wrong_instrument.xml
+-rw-r--r--   0        0        0     5899 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_no_software_nor_reagent_version.xml
+-rw-r--r--   0        0        0     4941 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/sample_sheets/novaseq_6000_sample_sheet_with_reversed_cycles.csv
+-rw-r--r--   0        0        0    10950 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/sample_sheets/novaseq_x_sample_sheet_with_forward_cycles.csv
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/spring/dummy_run_001.spring
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/spring/dummy_run_002.spring
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/demultiplexing/spring/dummy_spring_meta_data.json
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/fluffy/2020-23219-05/2020-23219-05.WCXpredict_aberrations.filt.bed
+-rw-r--r--   0        0        0     5554 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/fluffy/SampleSheet.csv
+-rw-r--r--   0        0        0      901 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/fluffy/deliverables.yaml
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/fluffy/fluffy_fastq.fastq.gz
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/fluffy/multiqc_report.html
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/fluffy/summary.csv
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/gt/yellowhog.bcf
+-rw-r--r--   0        0        0     5114 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/madeline/madeline.xml
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/mip/case_file.txt
+-rw-r--r--   0        0        0     3241 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/mip/case_metrics_deliverables.yaml
+-rw-r--r--   0        0        0    21811 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/mip/dna/store/case_config.yaml
+-rw-r--r--   0        0        0    23364 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/mip/dna/store/case_id_deliverables.yaml
+-rw-r--r--   0        0        0    37367 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/mip/dna/store/case_qc_sample_info.yaml
+-rw-r--r--   0        0        0       16 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/mip/dna/store/empty_case_config.yaml
+-rw-r--r--   0        0        0       16 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/mip/dna/store/empty_case_metrics_deliverables.yaml
+-rw-r--r--   0        0        0       16 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/mip/dna/store/empty_case_qc_sample_info.yaml
+-rw-r--r--   0        0        0      123 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/mip/dna/store/empty_delivery_report.html
+-rw-r--r--   0        0        0    62741 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/mip/dna/store/yellowhog_clinical_selected.vcf
+-rw-r--r--   0        0        0    11242 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/mip/rna/case_config.yaml
+-rw-r--r--   0        0        0    12164 2024-03-04 07:52:11.741385 cg-59.9.1/tests/fixtures/apps/mip/rna/case_qc_sampleinfo.yaml
+-rw-r--r--   0        0        0     5231 2024-03-04 07:52:11.745385 cg-59.9.1/tests/fixtures/apps/mip/rna/store/bundle_data.yaml
+-rw-r--r--   0        0        0     9774 2024-03-04 07:52:11.745385 cg-59.9.1/tests/fixtures/apps/mip/rna/store/case_config.yaml
+-rw-r--r--   0        0        0     4624 2024-03-04 07:52:11.745385 cg-59.9.1/tests/fixtures/apps/mip/rna/store/case_id_deliverables.yaml
+-rw-r--r--   0        0        0    13666 2024-03-04 07:52:11.745385 cg-59.9.1/tests/fixtures/apps/mip/rna/store/case_qc_sample_info.yaml
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.745385 cg-59.9.1/tests/fixtures/apps/mip/sample_file.txt
+-rw-r--r--   0        0        0     1885 2024-03-04 07:52:11.745385 cg-59.9.1/tests/fixtures/apps/scout/643594.config.yaml
+-rw-r--r--   0        0        0     6027 2024-03-04 07:52:11.745385 cg-59.9.1/tests/fixtures/apps/scout/case_export.json
+-rw-r--r--   0        0        0     9349 2024-03-04 07:52:11.745385 cg-59.9.1/tests/fixtures/apps/scout/export_causatives.json
+-rw-r--r--   0        0        0     1315 2024-03-04 07:52:11.745385 cg-59.9.1/tests/fixtures/apps/scout/none_case_export.json
+-rw-r--r--   0        0        0     3518 2024-03-04 07:52:11.745385 cg-59.9.1/tests/fixtures/apps/scout/other_sex_case.json
+-rw-r--r--   0        0        0     8874 2024-03-04 07:52:11.745385 cg-59.9.1/tests/fixtures/apps/scout/panel_export.bed
+-rw-r--r--   0        0        0     4169 2024-03-04 07:52:11.745385 cg-59.9.1/tests/fixtures/apps/scout/panel_export.csv
+-rw-r--r--   0        0        0    63569 2024-03-04 07:52:11.745385 cg-59.9.1/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Adapter_Metrics.csv
+-rw-r--r--   0        0        0    42478 2024-03-04 07:52:11.745385 cg-59.9.1/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Demultiplex_Stats.csv
+-rw-r--r--   0        0        0    69708 2024-03-04 07:52:11.745385 cg-59.9.1/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Quality_Metrics.csv
+-rw-r--r--   0        0        0      582 2024-03-04 07:52:11.745385 cg-59.9.1/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/SampleSheet.csv
+-rw-r--r--   0        0        0       42 2024-03-04 07:52:11.745385 cg-59.9.1/tests/fixtures/apps/shipping/scout-deploy.yaml
+-rw-r--r--   0        0        0     1036 2024-03-04 07:52:11.745385 cg-59.9.1/tests/fixtures/cgweb_orders/balsamic.json
+-rw-r--r--   0        0        0     1104 2024-03-04 07:52:11.745385 cg-59.9.1/tests/fixtures/cgweb_orders/fastq.json
+-rw-r--r--   0        0        0     1313 2024-03-04 07:52:11.745385 cg-59.9.1/tests/fixtures/cgweb_orders/metagenome.json
+-rw-r--r--   0        0        0     3038 2024-03-04 07:52:11.745385 cg-59.9.1/tests/fixtures/cgweb_orders/microsalt.json
+-rw-r--r--   0        0        0     3705 2024-03-04 07:52:11.745385 cg-59.9.1/tests/fixtures/cgweb_orders/mip.json
+-rw-r--r--   0        0        0     1364 2024-03-04 07:52:11.745385 cg-59.9.1/tests/fixtures/cgweb_orders/mip_rna.json
+-rw-r--r--   0        0        0     2125 2024-03-04 07:52:11.745385 cg-59.9.1/tests/fixtures/cgweb_orders/rml.json
+-rw-r--r--   0        0        0     1368 2024-03-04 07:52:11.745385 cg-59.9.1/tests/fixtures/cgweb_orders/rnafusion.json
+-rw-r--r--   0        0        0     4684 2024-03-04 07:52:11.745385 cg-59.9.1/tests/fixtures/cgweb_orders/sarscov2.json
+-rw-r--r--   0        0        0     5609 2024-03-04 07:52:11.745385 cg-59.9.1/tests/fixtures/data/SampleSheet.csv
+-rw-r--r--   0        0        0      511 2024-03-04 07:52:11.745385 cg-59.9.1/tests/fixtures/data/bcl_convert_sample_sheet.csv
+-rw-r--r--   0        0        0   258048 2024-03-04 07:52:11.745385 cg-59.9.1/tests/fixtures/data/cgfixture.db
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.745385 cg-59.9.1/tests/fixtures/data/fastq.fastq.gz
+-rw-r--r--   0        0        0    49152 2024-03-04 07:52:11.745385 cg-59.9.1/tests/fixtures/data/hkstore.db
+-rw-r--r--   0        0        0       73 2024-03-04 07:52:11.745385 cg-59.9.1/tests/fixtures/data/yellowhog/pedigree.yaml
+-rw-r--r--   0        0        0       76 2024-03-04 07:52:11.745385 cg-59.9.1/tests/fixtures/io/casava_five_parts.fastq.gz
+-rw-r--r--   0        0        0       90 2024-03-04 07:52:11.745385 cg-59.9.1/tests/fixtures/io/casava_seven_parts.fastq.gz
+-rw-r--r--   0        0        0       96 2024-03-04 07:52:11.745385 cg-59.9.1/tests/fixtures/io/casava_ten_parts.fastq.gz
+-rw-r--r--   0        0        0      153 2024-03-04 07:52:11.745385 cg-59.9.1/tests/fixtures/io/example.csv
+-rw-r--r--   0        0        0       46 2024-03-04 07:52:11.745385 cg-59.9.1/tests/fixtures/io/example.gz
+-rw-r--r--   0        0        0      147 2024-03-04 07:52:11.745385 cg-59.9.1/tests/fixtures/io/example.tsv
+-rw-r--r--   0        0        0       20 2024-03-04 07:52:11.749385 cg-59.9.1/tests/fixtures/io/example.txt
+-rw-r--r--   0        0        0      582 2024-03-04 07:52:11.749385 cg-59.9.1/tests/fixtures/io/example_json.json
+-rw-r--r--   0        0        0      103 2024-03-04 07:52:11.749385 cg-59.9.1/tests/fixtures/io/example_xml.xml
+-rw-r--r--   0        0        0       20 2024-03-04 07:52:11.749385 cg-59.9.1/tests/fixtures/meta/qc_metrics/file_with_right_tags.json
+-rw-r--r--   0        0        0       20 2024-03-04 07:52:11.749385 cg-59.9.1/tests/fixtures/meta/qc_metrics/file_without_right_tags.json
+-rw-r--r--   0        0        0   156910 2024-03-04 07:52:11.749385 cg-59.9.1/tests/fixtures/orderforms/1508.30.balsamic.xlsx
+-rw-r--r--   0        0        0   156770 2024-03-04 07:52:11.749385 cg-59.9.1/tests/fixtures/orderforms/1508.30.balsamic_qc.xlsx
+-rw-r--r--   0        0        0   156737 2024-03-04 07:52:11.749385 cg-59.9.1/tests/fixtures/orderforms/1508.30.balsamic_umi.xlsx
+-rw-r--r--   0        0        0   156582 2024-03-04 07:52:11.749385 cg-59.9.1/tests/fixtures/orderforms/1508.30.fastq.xlsx
+-rw-r--r--   0        0        0   155627 2024-03-04 07:52:11.749385 cg-59.9.1/tests/fixtures/orderforms/1508.30.metagenome.xlsx
+-rw-r--r--   0        0        0   156850 2024-03-04 07:52:11.749385 cg-59.9.1/tests/fixtures/orderforms/1508.30.mip.xlsx
+-rw-r--r--   0        0        0   258580 2024-03-04 07:52:11.753385 cg-59.9.1/tests/fixtures/orderforms/1508.30.mip_rna.xlsx
+-rw-r--r--   0        0        0   258342 2024-03-04 07:52:11.753385 cg-59.9.1/tests/fixtures/orderforms/1508.30.rnafusion.xlsx
+-rw-r--r--   0        0        0    82677 2024-03-04 07:52:11.753385 cg-59.9.1/tests/fixtures/orderforms/1603.11.microbial.xlsx
+-rw-r--r--   0        0        0   149394 2024-03-04 07:52:11.753385 cg-59.9.1/tests/fixtures/orderforms/1604.17.rml.xlsx
+-rw-r--r--   0        0        0   227887 2024-03-04 07:52:11.753385 cg-59.9.1/tests/fixtures/orderforms/2184.8.sarscov2.xlsx
+-rw-r--r--   0        0        0    18639 2024-03-04 07:52:11.753385 cg-59.9.1/tests/fixtures/orderforms/NIPT-json.json
+-rw-r--r--   0        0        0     6052 2024-03-04 07:52:11.753385 cg-59.9.1/tests/fixtures/orderforms/balsamic_uploaded_json_orderform.json
+-rw-r--r--   0        0        0     6611 2024-03-04 07:52:11.753385 cg-59.9.1/tests/fixtures/orderforms/mip_uploaded_json_orderform.json
+-rw-r--r--   0        0        0     1417 2024-03-04 07:52:11.753385 cg-59.9.1/tests/fixtures/report/case_data.json
+-rw-r--r--   0        0        0     1109 2024-03-04 07:52:11.753385 cg-59.9.1/tests/fixtures/report/lims_exported_samples.json
+-rw-r--r--   0        0        0     1562 2024-03-04 07:52:11.753385 cg-59.9.1/tests/fixtures/report/lims_family.json
+-rw-r--r--   0        0        0     2948 2024-03-04 07:52:11.753385 cg-59.9.1/tests/io/conftest.py
+-rw-r--r--   0        0        0     8639 2024-03-04 07:52:11.753385 cg-59.9.1/tests/io/test_io_controller.py
+-rw-r--r--   0        0        0     3877 2024-03-04 07:52:11.753385 cg-59.9.1/tests/io/test_io_csv.py
+-rw-r--r--   0        0        0      482 2024-03-04 07:52:11.753385 cg-59.9.1/tests/io/test_io_gzip.py
+-rw-r--r--   0        0        0     1779 2024-03-04 07:52:11.753385 cg-59.9.1/tests/io/test_io_json.py
+-rw-r--r--   0        0        0     1828 2024-03-04 07:52:11.753385 cg-59.9.1/tests/io/test_io_txt.py
+-rw-r--r--   0        0        0     1027 2024-03-04 07:52:11.753385 cg-59.9.1/tests/io/test_io_xml.py
+-rw-r--r--   0        0        0     2131 2024-03-04 07:52:11.753385 cg-59.9.1/tests/io/test_io_yaml.py
+-rw-r--r--   0        0        0     1233 2024-03-04 07:52:11.753385 cg-59.9.1/tests/io/test_validate_path.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.753385 cg-59.9.1/tests/meta/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.753385 cg-59.9.1/tests/meta/archive/__init__.py
+-rw-r--r--   0        0        0    13131 2024-03-04 07:52:11.753385 cg-59.9.1/tests/meta/archive/conftest.py
+-rw-r--r--   0        0        0    16858 2024-03-04 07:52:11.753385 cg-59.9.1/tests/meta/archive/test_archive_api.py
+-rw-r--r--   0        0        0    10246 2024-03-04 07:52:11.753385 cg-59.9.1/tests/meta/archive/test_archive_cli.py
+-rw-r--r--   0        0        0    15766 2024-03-04 07:52:11.753385 cg-59.9.1/tests/meta/archive/test_archiving.py
+-rw-r--r--   0        0        0     3807 2024-03-04 07:52:11.753385 cg-59.9.1/tests/meta/backup/conftest.py
+-rw-r--r--   0        0        0    26536 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/backup/test_meta_backup.py
+-rw-r--r--   0        0        0    10055 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/backup/test_meta_pdc.py
+-rw-r--r--   0        0        0    12654 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/clean/conftest.py
+-rw-r--r--   0        0        0    16961 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/clean/test_clean_flow_cells_api.py
+-rw-r--r--   0        0        0     2286 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/clean/test_clean_retrieved_spring_files.py
+-rw-r--r--   0        0        0     7691 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/compress/conftest.py
+-rw-r--r--   0        0        0     7961 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/compress/test_clean_fastq.py
+-rw-r--r--   0        0        0     1778 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/compress/test_compress_files.py
+-rw-r--r--   0        0        0     3644 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/compress/test_compress_meta_fastq.py
+-rw-r--r--   0        0        0     1180 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/compress/test_decompress_spring_meta.py
+-rw-r--r--   0        0        0     6902 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/compress/test_meta_compress_update_hk.py
+-rw-r--r--   0        0        0     8207 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/conftest.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/deliver/__init__.py
+-rw-r--r--   0        0        0     3471 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/deliver/conftest.py
+-rw-r--r--   0        0        0     8874 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/deliver/test_deliver_ticket.py
+-rw-r--r--   0        0        0    10277 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/deliver/test_delivery_api.py
+-rw-r--r--   0        0        0    13489 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/demultiplex/conftest.py
+-rw-r--r--   0        0        0     5382 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/demultiplex/test_combine_sequencing_metrics.py
+-rw-r--r--   0        0        0    10786 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/demultiplex/test_demux_post_processing.py
+-rw-r--r--   0        0        0    12330 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/demultiplex/test_housekeeper_storage_functions.py
+-rw-r--r--   0        0        0     5219 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/demultiplex/test_status_db_storage_functions.py
+-rw-r--r--   0        0        0    22708 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/demultiplex/test_utils.py
+-rw-r--r--   0        0        0     6193 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/demultiplex/test_validation.py
+-rw-r--r--   0        0        0     4943 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/encryption/conftest.py
+-rw-r--r--   0        0        0    18133 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/encryption/test_encryption.py
+-rw-r--r--   0        0        0     3122 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/observations/conftest.py
+-rw-r--r--   0        0        0    16164 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/observations/test_meta_upload_observations.py
+-rw-r--r--   0        0        0     4974 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/orders/conftest.py
+-rw-r--r--   0        0        0     1749 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/orders/test_PoolSubmitter_validate_order.py
+-rw-r--r--   0        0        0     1470 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/orders/test_SarsCov2Submitter_order_to_status.py
+-rw-r--r--   0        0        0     1768 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/orders/test_SarsCov2Submitter_store_order.py
+-rw-r--r--   0        0        0     2032 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/orders/test_SarsCov2Submitter_validate_order.py
+-rw-r--r--   0        0        0    19783 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/orders/test_meta_orders_api.py
+-rw-r--r--   0        0        0     7083 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/orders/test_meta_orders_lims.py
+-rw-r--r--   0        0        0    29515 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/orders/test_meta_orders_status.py
+-rw-r--r--   0        0        0     1677 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/orders/test_rnafusion_submitter.py
+-rw-r--r--   0        0        0     1068 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/orders/test_ticket_handler.py
+-rw-r--r--   0        0        0     3907 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/qc_metrics/conftest.py
+-rw-r--r--   0        0        0     1247 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/qc_metrics/test_collect_qc_metrics.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/report/__init__.py
+-rw-r--r--   0        0        0     5354 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/report/conftest.py
+-rw-r--r--   0        0        0      434 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/report/helper.py
+-rw-r--r--   0        0        0     4106 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/report/test_balsamic_api.py
+-rw-r--r--   0        0        0     4056 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/report/test_field_validators.py
+-rw-r--r--   0        0        0     2834 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/report/test_mip_dna_api.py
+-rw-r--r--   0        0        0    16698 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/report/test_report_api.py
+-rw-r--r--   0        0        0     2546 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/report/test_rnafusion_api.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/rsync/__init__.py
+-rw-r--r--   0        0        0      916 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/rsync/conftest.py
+-rw-r--r--   0        0        0     9442 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/rsync/test_rsync.py
+-rw-r--r--   0        0        0     3147 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/test_invoice.py
+-rw-r--r--   0        0        0     1787 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/transfer/conftest.py
+-rw-r--r--   0        0        0     9995 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/transfer/test_external_data.py
+-rw-r--r--   0        0        0     4395 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/transfer/test_meta_transfer_lims.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/upload/__init__.py
+-rw-r--r--   0        0        0     2210 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/upload/balsamic/test_balsamic.py
+-rw-r--r--   0        0        0     4002 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/upload/conftest.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/upload/gisaid/__init__.py
+-rw-r--r--   0        0        0     2557 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/upload/gisaid/fixtures/four_samples.csv
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/upload/gisaid/fixtures/invalid_housekeeper.fasta
+-rw-r--r--   0        0        0      211 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/upload/gisaid/fixtures/valid_gisaid.fasta
+-rw-r--r--   0        0        0      371 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/upload/gisaid/fixtures/valid_housekeeper.fasta
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/upload/mutacc/__init__.py
+-rw-r--r--   0        0        0     3684 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/upload/mutacc/conftest.py
+-rw-r--r--   0        0        0     4188 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/upload/mutacc/test_meta_upload_mutacc.py
+-rw-r--r--   0        0        0     1149 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/upload/nipt/conftest.py
+-rw-r--r--   0        0        0     1683 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/upload/nipt/test_models.py
+-rw-r--r--   0        0        0     1242 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/upload/nipt/test_nipt_upload_api.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.757385 cg-59.9.1/tests/meta/upload/scout/__init__.py
+-rw-r--r--   0        0        0    24071 2024-03-04 07:52:11.761385 cg-59.9.1/tests/meta/upload/scout/conftest.py
+-rw-r--r--   0        0        0     4734 2024-03-04 07:52:11.761385 cg-59.9.1/tests/meta/upload/scout/test_generate_load_config.py
+-rw-r--r--   0        0        0     4182 2024-03-04 07:52:11.761385 cg-59.9.1/tests/meta/upload/scout/test_meta_upload_scoutapi.py
+-rw-r--r--   0        0        0    33260 2024-03-04 07:52:11.761385 cg-59.9.1/tests/meta/upload/scout/test_meta_upload_scoutapi_rna.py
+-rw-r--r--   0        0        0     7372 2024-03-04 07:52:11.761385 cg-59.9.1/tests/meta/upload/scout/test_scout_config_builder.py
+-rw-r--r--   0        0        0     2511 2024-03-04 07:52:11.761385 cg-59.9.1/tests/meta/upload/test_meta_upload_coverage.py
+-rw-r--r--   0        0        0     1473 2024-03-04 07:52:11.761385 cg-59.9.1/tests/meta/upload/test_upload_api.py
+-rw-r--r--   0        0        0     2547 2024-03-04 07:52:11.761385 cg-59.9.1/tests/meta/upload/test_upload_genotypes_api.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.761385 cg-59.9.1/tests/meta/workflow/__init__.py
+-rw-r--r--   0        0        0    10066 2024-03-04 07:52:11.761385 cg-59.9.1/tests/meta/workflow/conftest.py
+-rw-r--r--   0        0        0     3652 2024-03-04 07:52:11.761385 cg-59.9.1/tests/meta/workflow/microsalt/conftest.py
+-rw-r--r--   0        0        0      318 2024-03-04 07:52:11.761385 cg-59.9.1/tests/meta/workflow/microsalt/test_parsing_metrics.py
+-rw-r--r--   0        0        0     3714 2024-03-04 07:52:11.761385 cg-59.9.1/tests/meta/workflow/microsalt/test_quality_controller.py
+-rw-r--r--   0        0        0    14367 2024-03-04 07:52:11.761385 cg-59.9.1/tests/meta/workflow/microsalt/test_quality_controller_utils.py
+-rw-r--r--   0        0        0      825 2024-03-04 07:52:11.761385 cg-59.9.1/tests/meta/workflow/microsalt/test_report_generation.py
+-rw-r--r--   0        0        0    20886 2024-03-04 07:52:11.761385 cg-59.9.1/tests/meta/workflow/test_analysis.py
+-rw-r--r--   0        0        0     6190 2024-03-04 07:52:11.761385 cg-59.9.1/tests/meta/workflow/test_balsamic.py
+-rw-r--r--   0        0        0     3034 2024-03-04 07:52:11.761385 cg-59.9.1/tests/meta/workflow/test_fastq.py
+-rw-r--r--   0        0        0     1532 2024-03-04 07:52:11.761385 cg-59.9.1/tests/meta/workflow/test_microsalt.py
+-rw-r--r--   0        0        0     3123 2024-03-04 07:52:11.761385 cg-59.9.1/tests/meta/workflow/test_nf_analysis.py
+-rw-r--r--   0        0        0     7741 2024-03-04 07:52:11.761385 cg-59.9.1/tests/meta/workflow/test_prepare_fastq_api.py
+-rw-r--r--   0        0        0     1688 2024-03-04 07:52:11.761385 cg-59.9.1/tests/meta/workflow/test_rnafusion.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.761385 cg-59.9.1/tests/mocks/__init__.py
+-rw-r--r--   0        0        0     1161 2024-03-04 07:52:11.761385 cg-59.9.1/tests/mocks/balsamic_analysis_mock.py
+-rw-r--r--   0        0        0     3500 2024-03-04 07:52:11.761385 cg-59.9.1/tests/mocks/crunchy.py
+-rw-r--r--   0        0        0    21569 2024-03-04 07:52:11.761385 cg-59.9.1/tests/mocks/hk_mock.py
+-rw-r--r--   0        0        0     3802 2024-03-04 07:52:11.761385 cg-59.9.1/tests/mocks/limsmock.py
+-rw-r--r--   0        0        0      572 2024-03-04 07:52:11.761385 cg-59.9.1/tests/mocks/madeline.py
+-rw-r--r--   0        0        0     1297 2024-03-04 07:52:11.761385 cg-59.9.1/tests/mocks/mip_analysis_mock.py
+-rw-r--r--   0        0        0     1525 2024-03-04 07:52:11.761385 cg-59.9.1/tests/mocks/osticket.py
+-rw-r--r--   0        0        0     3239 2024-03-04 07:52:11.761385 cg-59.9.1/tests/mocks/process_mock.py
+-rw-r--r--   0        0        0     3718 2024-03-04 07:52:11.761385 cg-59.9.1/tests/mocks/report.py
+-rw-r--r--   0        0        0     3915 2024-03-04 07:52:11.761385 cg-59.9.1/tests/mocks/scout.py
+-rw-r--r--   0        0        0      750 2024-03-04 07:52:11.761385 cg-59.9.1/tests/mocks/store_model.py
+-rw-r--r--   0        0        0     1532 2024-03-04 07:52:11.761385 cg-59.9.1/tests/mocks/tb_mock.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.761385 cg-59.9.1/tests/models/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.761385 cg-59.9.1/tests/models/balsamic/__init__.py
+-rw-r--r--   0        0        0     1194 2024-03-04 07:52:11.761385 cg-59.9.1/tests/models/balsamic/conftest.py
+-rw-r--r--   0        0        0     1030 2024-03-04 07:52:11.761385 cg-59.9.1/tests/models/balsamic/test_balsamic_analysis.py
+-rw-r--r--   0        0        0     1050 2024-03-04 07:52:11.761385 cg-59.9.1/tests/models/conftest.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.761385 cg-59.9.1/tests/models/demultiplexing/__init__.py
+-rw-r--r--   0        0        0      284 2024-03-04 07:52:11.761385 cg-59.9.1/tests/models/demultiplexing/conftest.py
+-rw-r--r--   0        0        0    11446 2024-03-04 07:52:11.761385 cg-59.9.1/tests/models/demultiplexing/test_run_parameters.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.761385 cg-59.9.1/tests/models/downsample/__init__.py
+-rw-r--r--   0        0        0     2096 2024-03-04 07:52:11.761385 cg-59.9.1/tests/models/downsample/test_down_sample_meta_data.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.761385 cg-59.9.1/tests/models/flow_cell/__init__.py
+-rw-r--r--   0        0        0     8715 2024-03-04 07:52:11.761385 cg-59.9.1/tests/models/flow_cell/test_flowcell_model.py
+-rw-r--r--   0        0        0     6637 2024-03-04 07:52:11.761385 cg-59.9.1/tests/models/mip/conftest.py
+-rw-r--r--   0        0        0     1239 2024-03-04 07:52:11.761385 cg-59.9.1/tests/models/mip/test_mip_analysis.py
+-rw-r--r--   0        0        0     2348 2024-03-04 07:52:11.761385 cg-59.9.1/tests/models/mip/test_mip_config.py
+-rw-r--r--   0        0        0     6392 2024-03-04 07:52:11.761385 cg-59.9.1/tests/models/mip/test_mip_metrics_deliverables.py
+-rw-r--r--   0        0        0     3959 2024-03-04 07:52:11.761385 cg-59.9.1/tests/models/mip/test_mip_sample_info.py
+-rw-r--r--   0        0        0     3314 2024-03-04 07:52:11.761385 cg-59.9.1/tests/models/nextflow/test_nextflow_deliver.py
+-rw-r--r--   0        0        0     1602 2024-03-04 07:52:11.761385 cg-59.9.1/tests/models/observations/conftest.py
+-rw-r--r--   0        0        0     2579 2024-03-04 07:52:11.761385 cg-59.9.1/tests/models/observations/test_observations_input_files.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.761385 cg-59.9.1/tests/models/report/__init__.py
+-rw-r--r--   0        0        0     6722 2024-03-04 07:52:11.761385 cg-59.9.1/tests/models/report/test_validators.py
+-rw-r--r--   0        0        0     3855 2024-03-04 07:52:11.761385 cg-59.9.1/tests/models/rnafusion/test_rnafusion_sample.py
+-rw-r--r--   0        0        0     1374 2024-03-04 07:52:11.761385 cg-59.9.1/tests/models/test_cg_models.py
+-rw-r--r--   0        0        0      990 2024-03-04 07:52:11.761385 cg-59.9.1/tests/models/test_compression_data.py
+-rw-r--r--   0        0        0      729 2024-03-04 07:52:11.761385 cg-59.9.1/tests/models/test_fastq.py
+-rw-r--r--   0        0        0     2860 2024-03-04 07:52:11.761385 cg-59.9.1/tests/models/test_file_data.py
+-rw-r--r--   0        0        0     3114 2024-03-04 07:52:11.761385 cg-59.9.1/tests/server/conftest.py
+-rw-r--r--   0        0        0      509 2024-03-04 07:52:11.761385 cg-59.9.1/tests/server/endpoints/test_delivery_message_endpoint.py
+-rw-r--r--   0        0        0     3047 2024-03-04 07:52:11.761385 cg-59.9.1/tests/server/endpoints/test_orders_endpoint.py
+-rw-r--r--   0        0        0      271 2024-03-04 07:52:11.761385 cg-59.9.1/tests/server/test_server_auto.py
+-rw-r--r--   0        0        0     1047 2024-03-04 07:52:11.761385 cg-59.9.1/tests/services/fastq_file_service/conftest.py
+-rw-r--r--   0        0        0     3435 2024-03-04 07:52:11.761385 cg-59.9.1/tests/services/fastq_file_service/test_fastq_file_service.py
+-rw-r--r--   0        0        0     1055 2024-03-04 07:52:11.761385 cg-59.9.1/tests/services/orders/order_status_service/conftest.py
+-rw-r--r--   0        0        0      872 2024-03-04 07:52:11.761385 cg-59.9.1/tests/services/orders/order_status_service/test_order_status_service.py
+-rw-r--r--   0        0        0      318 2024-03-04 07:52:11.761385 cg-59.9.1/tests/small_helpers.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.761385 cg-59.9.1/tests/store/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.761385 cg-59.9.1/tests/store/api/__init__.py
+-rw-r--r--   0        0        0     2981 2024-03-04 07:52:11.761385 cg-59.9.1/tests/store/api/conftest.py
+-rw-r--r--   0        0        0     1557 2024-03-04 07:52:11.761385 cg-59.9.1/tests/store/api/test_base.py
+-rw-r--r--   0        0        0    20311 2024-03-04 07:52:11.761385 cg-59.9.1/tests/store/conftest.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.765385 cg-59.9.1/tests/store/crud/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.765385 cg-59.9.1/tests/store/crud/add/__init__.py
+-rw-r--r--   0        0        0     1497 2024-03-04 07:52:11.765385 cg-59.9.1/tests/store/crud/add/test_store_add_application_version.py
+-rw-r--r--   0        0        0     3958 2024-03-04 07:52:11.765385 cg-59.9.1/tests/store/crud/add/test_store_add_base.py
+-rw-r--r--   0        0        0     2502 2024-03-04 07:52:11.765385 cg-59.9.1/tests/store/crud/add/test_store_add_customer.py
+-rw-r--r--   0        0        0     1640 2024-03-04 07:52:11.765385 cg-59.9.1/tests/store/crud/add/test_store_add_flow_celll.py
+-rw-r--r--   0        0        0    12209 2024-03-04 07:52:11.765385 cg-59.9.1/tests/store/crud/conftest.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.765385 cg-59.9.1/tests/store/crud/delete/__init__.py
+-rw-r--r--   0        0        0     5541 2024-03-04 07:52:11.765385 cg-59.9.1/tests/store/crud/delete/test_delete.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.765385 cg-59.9.1/tests/store/crud/read/__init__.py
+-rw-r--r--   0        0        0    57211 2024-03-04 07:52:11.765385 cg-59.9.1/tests/store/crud/read/test_read.py
+-rw-r--r--   0        0        0     5461 2024-03-04 07:52:11.765385 cg-59.9.1/tests/store/crud/read/test_read_analyses_to_clean.py
+-rw-r--r--   0        0        0     3553 2024-03-04 07:52:11.765385 cg-59.9.1/tests/store/crud/read/test_read_analyses_to_delivery_report.py
+-rw-r--r--   0        0        0    18463 2024-03-04 07:52:11.765385 cg-59.9.1/tests/store/crud/read/test_read_analysis.py
+-rw-r--r--   0        0        0     2743 2024-03-04 07:52:11.765385 cg-59.9.1/tests/store/crud/read/test_read_application_version.py
+-rw-r--r--   0        0        0    59704 2024-03-04 07:52:11.765385 cg-59.9.1/tests/store/crud/read/test_read_case.py
+-rw-r--r--   0        0        0     1105 2024-03-04 07:52:11.765385 cg-59.9.1/tests/store/crud/read/test_read_customer.py
+-rw-r--r--   0        0        0     1530 2024-03-04 07:52:11.765385 cg-59.9.1/tests/store/crud/read/test_read_pool.py
+-rw-r--r--   0        0        0    21602 2024-03-04 07:52:11.765385 cg-59.9.1/tests/store/crud/read/test_read_sample.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.765385 cg-59.9.1/tests/store/crud/update/__init__.py
+-rw-r--r--   0        0        0      737 2024-03-04 07:52:11.765385 cg-59.9.1/tests/store/crud/update/test_update.py
+-rw-r--r--   0        0        0    11693 2024-03-04 07:52:11.765385 cg-59.9.1/tests/store/filters/test_status_analyses_filters.py
+-rw-r--r--   0        0        0     3397 2024-03-04 07:52:11.765385 cg-59.9.1/tests/store/filters/test_status_application_filters.py
+-rw-r--r--   0        0        0     2073 2024-03-04 07:52:11.765385 cg-59.9.1/tests/store/filters/test_status_application_limitations_filters.py
+-rw-r--r--   0        0        0    10452 2024-03-04 07:52:11.765385 cg-59.9.1/tests/store/filters/test_status_application_version_filters.py
+-rw-r--r--   0        0        0     2804 2024-03-04 07:52:11.765385 cg-59.9.1/tests/store/filters/test_status_bed_filters.py
+-rw-r--r--   0        0        0     2362 2024-03-04 07:52:11.765385 cg-59.9.1/tests/store/filters/test_status_bed_version_filters.py
+-rw-r--r--   0        0        0     3495 2024-03-04 07:52:11.765385 cg-59.9.1/tests/store/filters/test_status_case_sample_filters.py
+-rw-r--r--   0        0        0    39100 2024-03-04 07:52:11.765385 cg-59.9.1/tests/store/filters/test_status_cases_filters.py
+-rw-r--r--   0        0        0     1345 2024-03-04 07:52:11.765385 cg-59.9.1/tests/store/filters/test_status_collaboration_filters.py
+-rw-r--r--   0        0        0     2482 2024-03-04 07:52:11.765385 cg-59.9.1/tests/store/filters/test_status_customer_filters.py
+-rw-r--r--   0        0        0     4907 2024-03-04 07:52:11.765385 cg-59.9.1/tests/store/filters/test_status_flow_cell_filters.py
+-rw-r--r--   0        0        0     2226 2024-03-04 07:52:11.765385 cg-59.9.1/tests/store/filters/test_status_invoice_filters.py
+-rw-r--r--   0        0        0     5970 2024-03-04 07:52:11.765385 cg-59.9.1/tests/store/filters/test_status_metrics_filters.py
+-rw-r--r--   0        0        0     2404 2024-03-04 07:52:11.765385 cg-59.9.1/tests/store/filters/test_status_organism_filters.py
+-rw-r--r--   0        0        0     1804 2024-03-04 07:52:11.765385 cg-59.9.1/tests/store/filters/test_status_panel_filters.py
+-rw-r--r--   0        0        0     8720 2024-03-04 07:52:11.765385 cg-59.9.1/tests/store/filters/test_status_pool_filters.py
+-rw-r--r--   0        0        0    22967 2024-03-04 07:52:11.765385 cg-59.9.1/tests/store/filters/test_status_samples_filters.py
+-rw-r--r--   0        0        0     1576 2024-03-04 07:52:11.765385 cg-59.9.1/tests/store/filters/test_status_user_filters.py
+-rw-r--r--   0        0        0     2147 2024-03-04 07:52:11.765385 cg-59.9.1/tests/store/test_delivery.py
+-rw-r--r--   0        0        0     4127 2024-03-04 07:52:11.765385 cg-59.9.1/tests/store/test_store_models.py
+-rw-r--r--   0        0        0    35256 2024-03-04 07:52:11.765385 cg-59.9.1/tests/store_helpers.py
+-rw-r--r--   0        0        0     4930 2024-03-04 07:52:11.765385 cg-59.9.1/tests/test_copy_novaseqx_flow_cell.py
+-rw-r--r--   0        0        0      911 2024-03-04 07:52:11.765385 cg-59.9.1/tests/test_store_helpers.py
+-rw-r--r--   0        0        0        0 2024-03-04 07:52:11.765385 cg-59.9.1/tests/utils/__init__.py
+-rw-r--r--   0        0        0     1754 2024-03-04 07:52:11.765385 cg-59.9.1/tests/utils/conftest.py
+-rw-r--r--   0        0        0      371 2024-03-04 07:52:11.765385 cg-59.9.1/tests/utils/test_calculations.py
+-rw-r--r--   0        0        0     2920 2024-03-04 07:52:11.765385 cg-59.9.1/tests/utils/test_commands.py
+-rw-r--r--   0        0        0      953 2024-03-04 07:52:11.765385 cg-59.9.1/tests/utils/test_date.py
+-rw-r--r--   0        0        0     1508 2024-03-04 07:52:11.765385 cg-59.9.1/tests/utils/test_dict.py
+-rw-r--r--   0        0        0     7154 2024-03-04 07:52:11.765385 cg-59.9.1/tests/utils/test_dispatcher.py
+-rw-r--r--   0        0        0     4100 2024-03-04 07:52:11.765385 cg-59.9.1/tests/utils/test_files.py
+-rw-r--r--   0        0        0     1170 2024-03-04 07:52:11.765385 cg-59.9.1/tests/utils/test_time.py
+-rw-r--r--   0        0        0     2366 2024-03-04 07:52:11.765385 cg-59.9.1/tests/utils/test_utils.py
+-rw-r--r--   0        0        0     4341 1970-01-01 00:00:00.000000 cg-59.9.1/PKG-INFO
```

### Comparing `cg-59.9.0/README.md` & `cg-59.9.1/README.md`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/apps/coverage/api.py` & `cg-59.9.1/cg/apps/coverage/api.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/apps/crunchy/crunchy.py` & `cg-59.9.1/cg/apps/crunchy/crunchy.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/apps/crunchy/files.py` & `cg-59.9.1/cg/apps/crunchy/files.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/apps/crunchy/sbatch.py` & `cg-59.9.1/cg/apps/crunchy/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/apps/demultiplex/demultiplex_api.py` & `cg-59.9.1/cg/apps/demultiplex/demultiplex_api.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/apps/demultiplex/sample_sheet/api.py` & `cg-59.9.1/cg/apps/demultiplex/sample_sheet/api.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/apps/demultiplex/sample_sheet/create.py` & `cg-59.9.1/cg/apps/demultiplex/sample_sheet/create.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/apps/demultiplex/sample_sheet/index.py` & `cg-59.9.1/cg/apps/demultiplex/sample_sheet/index.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/apps/demultiplex/sample_sheet/override_cycles_validator.py` & `cg-59.9.1/cg/apps/demultiplex/sample_sheet/override_cycles_validator.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/apps/demultiplex/sample_sheet/read_sample_sheet.py` & `cg-59.9.1/cg/apps/demultiplex/sample_sheet/read_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/apps/demultiplex/sample_sheet/sample_models.py` & `cg-59.9.1/cg/apps/demultiplex/sample_sheet/sample_models.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/apps/demultiplex/sample_sheet/sample_sheet_creator.py` & `cg-59.9.1/cg/apps/demultiplex/sample_sheet/sample_sheet_creator.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/apps/demultiplex/sample_sheet/sample_sheet_models.py` & `cg-59.9.1/cg/apps/demultiplex/sample_sheet/sample_sheet_models.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/apps/demultiplex/sample_sheet/sample_sheet_validator.py` & `cg-59.9.1/cg/apps/demultiplex/sample_sheet/sample_sheet_validator.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/apps/demultiplex/sample_sheet/validators.py` & `cg-59.9.1/cg/apps/demultiplex/sample_sheet/validators.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/apps/demultiplex/sbatch.py` & `cg-59.9.1/cg/apps/demultiplex/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/apps/downsample/downsample.py` & `cg-59.9.1/cg/apps/downsample/downsample.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/apps/downsample/utils.py` & `cg-59.9.1/cg/apps/downsample/utils.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/apps/gens.py` & `cg-59.9.1/cg/apps/gens.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/apps/gt.py` & `cg-59.9.1/cg/apps/gt.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/apps/hermes/hermes_api.py` & `cg-59.9.1/cg/apps/hermes/hermes_api.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/apps/hermes/models.py` & `cg-59.9.1/cg/apps/hermes/models.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/apps/housekeeper/hk.py` & `cg-59.9.1/cg/apps/housekeeper/hk.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/apps/invoice/render.py` & `cg-59.9.1/cg/apps/invoice/render.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/apps/invoice/templates/KI_pool_invoice.xlsx` & `cg-59.9.1/cg/apps/invoice/templates/KI_pool_invoice.xlsx`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/apps/invoice/templates/KI_sample_invoice.xlsx` & `cg-59.9.1/cg/apps/invoice/templates/KI_sample_invoice.xlsx`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/apps/invoice/templates/KTH_pool_invoice.xlsx` & `cg-59.9.1/cg/apps/invoice/templates/KTH_pool_invoice.xlsx`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/apps/invoice/templates/KTH_sample_invoice.xlsx` & `cg-59.9.1/cg/apps/invoice/templates/KTH_sample_invoice.xlsx`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/apps/lims/api.py` & `cg-59.9.1/cg/apps/lims/api.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/apps/lims/batch.py` & `cg-59.9.1/cg/apps/lims/batch.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/apps/lims/order.py` & `cg-59.9.1/cg/apps/lims/order.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/apps/lims/sample_sheet.py` & `cg-59.9.1/cg/apps/lims/sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/apps/loqus.py` & `cg-59.9.1/cg/apps/loqus.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/apps/madeline/api.py` & `cg-59.9.1/cg/apps/madeline/api.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/apps/mip/confighandler.py` & `cg-59.9.1/cg/apps/mip/confighandler.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/apps/mutacc_auto.py` & `cg-59.9.1/cg/apps/mutacc_auto.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/apps/orderform/excel_orderform_parser.py` & `cg-59.9.1/cg/apps/orderform/excel_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/apps/orderform/json_orderform_parser.py` & `cg-59.9.1/cg/apps/orderform/json_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/apps/orderform/orderform_parser.py` & `cg-59.9.1/cg/apps/orderform/orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/apps/osticket.py` & `cg-59.9.1/cg/apps/osticket.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/apps/scout/scout_export.py` & `cg-59.9.1/cg/apps/scout/scout_export.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/apps/scout/scoutapi.py` & `cg-59.9.1/cg/apps/scout/scoutapi.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/apps/sequencing_metrics_parser/api.py` & `cg-59.9.1/cg/apps/sequencing_metrics_parser/api.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/apps/sequencing_metrics_parser/models/bcl2fastq_metrics.py` & `cg-59.9.1/cg/apps/sequencing_metrics_parser/models/bcl2fastq_metrics.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/apps/sequencing_metrics_parser/models/bcl_convert.py` & `cg-59.9.1/cg/apps/sequencing_metrics_parser/models/bcl_convert.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/apps/sequencing_metrics_parser/parsers/bcl2fastq.py` & `cg-59.9.1/cg/apps/sequencing_metrics_parser/parsers/bcl2fastq.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/apps/sequencing_metrics_parser/parsers/bcl2fastq_to_sequencing_statistics.py` & `cg-59.9.1/cg/apps/sequencing_metrics_parser/parsers/bcl2fastq_to_sequencing_statistics.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/apps/sequencing_metrics_parser/parsers/bcl_convert.py` & `cg-59.9.1/cg/apps/sequencing_metrics_parser/parsers/bcl_convert.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/apps/sequencing_metrics_parser/parsers/bcl_convert_to_sequencing_statistics.py` & `cg-59.9.1/cg/apps/sequencing_metrics_parser/parsers/bcl_convert_to_sequencing_statistics.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/apps/sequencing_metrics_parser/sequencing_metrics_calculator.py` & `cg-59.9.1/cg/apps/sequencing_metrics_parser/sequencing_metrics_calculator.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/apps/slurm/sbatch.py` & `cg-59.9.1/cg/apps/slurm/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/apps/slurm/slurm_api.py` & `cg-59.9.1/cg/apps/slurm/slurm_api.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/apps/tb/api.py` & `cg-59.9.1/cg/apps/tb/api.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/apps/tb/models.py` & `cg-59.9.1/cg/apps/tb/models.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/cli/add.py` & `cg-59.9.1/cg/cli/add.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/cli/archive.py` & `cg-59.9.1/cg/cli/archive.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/cli/backup.py` & `cg-59.9.1/cg/cli/backup.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/cli/base.py` & `cg-59.9.1/cg/cli/base.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/cli/clean.py` & `cg-59.9.1/cg/cli/clean.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/cli/compress/base.py` & `cg-59.9.1/cg/cli/compress/base.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/cli/compress/fastq.py` & `cg-59.9.1/cg/cli/compress/fastq.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/cli/compress/helpers.py` & `cg-59.9.1/cg/cli/compress/helpers.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/cli/delete/base.py` & `cg-59.9.1/cg/cli/delete/base.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/cli/delete/case.py` & `cg-59.9.1/cg/cli/delete/case.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/cli/delete/cases.py` & `cg-59.9.1/cg/cli/delete/cases.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/cli/delete/observations.py` & `cg-59.9.1/cg/cli/delete/observations.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/cli/deliver/base.py` & `cg-59.9.1/cg/cli/deliver/base.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/cli/demultiplex/base.py` & `cg-59.9.1/cg/cli/demultiplex/base.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/cli/demultiplex/copy_novaseqx_demultiplex_data.py` & `cg-59.9.1/cg/cli/demultiplex/copy_novaseqx_demultiplex_data.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/cli/demultiplex/demux.py` & `cg-59.9.1/cg/cli/demultiplex/demux.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/cli/demultiplex/finish.py` & `cg-59.9.1/cg/cli/demultiplex/finish.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/cli/demultiplex/sample_sheet.py` & `cg-59.9.1/cg/cli/demultiplex/sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/cli/downsample.py` & `cg-59.9.1/cg/cli/downsample.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/cli/generate/report/base.py` & `cg-59.9.1/cg/cli/generate/report/base.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/cli/generate/report/options.py` & `cg-59.9.1/cg/cli/generate/report/options.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/cli/generate/report/utils.py` & `cg-59.9.1/cg/cli/generate/report/utils.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/cli/get.py` & `cg-59.9.1/cg/cli/get.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/cli/set/base.py` & `cg-59.9.1/cg/cli/set/base.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/cli/set/case.py` & `cg-59.9.1/cg/cli/set/case.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/cli/set/cases.py` & `cg-59.9.1/cg/cli/set/cases.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/cli/store/fastq.py` & `cg-59.9.1/cg/cli/store/fastq.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/cli/store/store.py` & `cg-59.9.1/cg/cli/store/store.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/cli/transfer.py` & `cg-59.9.1/cg/cli/transfer.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/cli/upload/base.py` & `cg-59.9.1/cg/cli/upload/base.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/cli/upload/clinical_delivery.py` & `cg-59.9.1/cg/cli/upload/clinical_delivery.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/cli/upload/coverage.py` & `cg-59.9.1/cg/cli/upload/coverage.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/cli/upload/delivery_report.py` & `cg-59.9.1/cg/cli/upload/delivery_report.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/cli/upload/fohm.py` & `cg-59.9.1/cg/cli/upload/fohm.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/cli/upload/genotype.py` & `cg-59.9.1/cg/cli/upload/genotype.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/cli/upload/gens.py` & `cg-59.9.1/cg/cli/upload/gens.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/cli/upload/gisaid.py` & `cg-59.9.1/cg/cli/upload/gisaid.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/cli/upload/mutacc.py` & `cg-59.9.1/cg/cli/upload/mutacc.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/cli/upload/nipt/base.py` & `cg-59.9.1/cg/cli/upload/nipt/base.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/cli/upload/nipt/ftp.py` & `cg-59.9.1/cg/cli/upload/nipt/ftp.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/cli/upload/nipt/statina.py` & `cg-59.9.1/cg/cli/upload/nipt/statina.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/cli/upload/observations/observations.py` & `cg-59.9.1/cg/cli/upload/observations/observations.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/cli/upload/observations/utils.py` & `cg-59.9.1/cg/cli/upload/observations/utils.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/cli/upload/scout.py` & `cg-59.9.1/cg/cli/upload/scout.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/cli/upload/utils.py` & `cg-59.9.1/cg/cli/upload/utils.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/cli/upload/validate.py` & `cg-59.9.1/cg/cli/upload/validate.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/cli/workflow/balsamic/base.py` & `cg-59.9.1/cg/cli/workflow/balsamic/base.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/cli/workflow/balsamic/options.py` & `cg-59.9.1/cg/cli/workflow/balsamic/options.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/cli/workflow/balsamic/pon.py` & `cg-59.9.1/cg/cli/workflow/balsamic/pon.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/cli/workflow/balsamic/qc.py` & `cg-59.9.1/cg/cli/workflow/balsamic/qc.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/cli/workflow/balsamic/umi.py` & `cg-59.9.1/cg/cli/workflow/balsamic/umi.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/cli/workflow/base.py` & `cg-59.9.1/cg/cli/workflow/base.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/cli/workflow/commands.py` & `cg-59.9.1/cg/cli/workflow/commands.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/cli/workflow/fastq/base.py` & `cg-59.9.1/cg/cli/workflow/fastq/base.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/cli/workflow/fastq/fastq_service.py` & `cg-59.9.1/cg/cli/workflow/fastq/fastq_service.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/cli/workflow/fluffy/base.py` & `cg-59.9.1/cg/cli/workflow/fluffy/base.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/cli/workflow/microsalt/base.py` & `cg-59.9.1/cg/cli/workflow/microsalt/base.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/cli/workflow/mip/base.py` & `cg-59.9.1/cg/cli/workflow/mip/base.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/cli/workflow/mip/options.py` & `cg-59.9.1/cg/cli/workflow/mip/options.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/cli/workflow/mip_dna/base.py` & `cg-59.9.1/cg/cli/workflow/mip_dna/base.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/cli/workflow/mip_rna/base.py` & `cg-59.9.1/cg/cli/workflow/mip_rna/base.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/cli/workflow/mutant/base.py` & `cg-59.9.1/cg/cli/workflow/mutant/base.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/cli/workflow/nf_analysis.py` & `cg-59.9.1/cg/cli/workflow/nf_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/cli/workflow/raredisease/base.py` & `cg-59.9.1/cg/cli/workflow/raredisease/base.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/cli/workflow/rnafusion/base.py` & `cg-59.9.1/cg/cli/workflow/rnafusion/base.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/cli/workflow/rnafusion/options.py` & `cg-59.9.1/cg/cli/workflow/rnafusion/options.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/cli/workflow/taxprofiler/base.py` & `cg-59.9.1/cg/cli/workflow/taxprofiler/base.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/cli/workflow/taxprofiler/options.py` & `cg-59.9.1/cg/cli/workflow/taxprofiler/options.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/clients/janus/api.py` & `cg-59.9.1/cg/clients/janus/api.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/constants/__init__.py` & `cg-59.9.1/cg/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/constants/bcl_convert_metrics.py` & `cg-59.9.1/cg/constants/bcl_convert_metrics.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/constants/constants.py` & `cg-59.9.1/cg/constants/constants.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/constants/delivery.py` & `cg-59.9.1/cg/constants/delivery.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/constants/demultiplexing.py` & `cg-59.9.1/cg/constants/demultiplexing.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/constants/encryption.py` & `cg-59.9.1/cg/constants/encryption.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/constants/gene_panel.py` & `cg-59.9.1/cg/constants/gene_panel.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/constants/housekeeper_tags.py` & `cg-59.9.1/cg/constants/housekeeper_tags.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/constants/lims.py` & `cg-59.9.1/cg/constants/lims.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/constants/nextflow.py` & `cg-59.9.1/cg/constants/nextflow.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/constants/nf_analysis.py` & `cg-59.9.1/cg/constants/nf_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/constants/observations.py` & `cg-59.9.1/cg/constants/observations.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/constants/orderforms.py` & `cg-59.9.1/cg/constants/orderforms.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/constants/priority.py` & `cg-59.9.1/cg/constants/priority.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/constants/report.py` & `cg-59.9.1/cg/constants/report.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/constants/scout.py` & `cg-59.9.1/cg/constants/scout.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/constants/sequencing.py` & `cg-59.9.1/cg/constants/sequencing.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/constants/subject.py` & `cg-59.9.1/cg/constants/subject.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/exc.py` & `cg-59.9.1/cg/exc.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/io/api.py` & `cg-59.9.1/cg/io/api.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/io/controller.py` & `cg-59.9.1/cg/io/controller.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/io/csv.py` & `cg-59.9.1/cg/io/csv.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/io/json.py` & `cg-59.9.1/cg/io/json.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/io/txt.py` & `cg-59.9.1/cg/io/txt.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/io/validate_path.py` & `cg-59.9.1/cg/io/validate_path.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/io/xml.py` & `cg-59.9.1/cg/io/xml.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/io/yaml.py` & `cg-59.9.1/cg/io/yaml.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/archive/archive.py` & `cg-59.9.1/cg/meta/archive/archive.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/archive/ddn/constants.py` & `cg-59.9.1/cg/meta/archive/ddn/constants.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/archive/ddn/ddn_data_flow_client.py` & `cg-59.9.1/cg/meta/archive/ddn/ddn_data_flow_client.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/archive/ddn/models.py` & `cg-59.9.1/cg/meta/archive/ddn/models.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/archive/ddn/utils.py` & `cg-59.9.1/cg/meta/archive/ddn/utils.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/archive/models.py` & `cg-59.9.1/cg/meta/archive/models.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/backup/backup.py` & `cg-59.9.1/cg/meta/backup/backup.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/backup/pdc.py` & `cg-59.9.1/cg/meta/backup/pdc.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/clean/api.py` & `cg-59.9.1/cg/meta/clean/api.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/clean/clean_flow_cells.py` & `cg-59.9.1/cg/meta/clean/clean_flow_cells.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/clean/clean_retrieved_spring_files.py` & `cg-59.9.1/cg/meta/clean/clean_retrieved_spring_files.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/compress/compress.py` & `cg-59.9.1/cg/meta/compress/compress.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/compress/files.py` & `cg-59.9.1/cg/meta/compress/files.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/deliver.py` & `cg-59.9.1/cg/meta/deliver.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/deliver_ticket.py` & `cg-59.9.1/cg/meta/deliver_ticket.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/demultiplex/combine_sequencing_metrics.py` & `cg-59.9.1/cg/meta/demultiplex/combine_sequencing_metrics.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/demultiplex/demux_post_processing.py` & `cg-59.9.1/cg/meta/demultiplex/demux_post_processing.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/demultiplex/files.py` & `cg-59.9.1/cg/meta/demultiplex/files.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/demultiplex/housekeeper_storage_functions.py` & `cg-59.9.1/cg/meta/demultiplex/housekeeper_storage_functions.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/demultiplex/status_db_storage_functions.py` & `cg-59.9.1/cg/meta/demultiplex/status_db_storage_functions.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/demultiplex/utils.py` & `cg-59.9.1/cg/meta/demultiplex/utils.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/demultiplex/validation.py` & `cg-59.9.1/cg/meta/demultiplex/validation.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/encryption/encryption.py` & `cg-59.9.1/cg/meta/encryption/encryption.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/invoice.py` & `cg-59.9.1/cg/meta/invoice.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/meta.py` & `cg-59.9.1/cg/meta/meta.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/observations/balsamic_observations_api.py` & `cg-59.9.1/cg/meta/observations/balsamic_observations_api.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/observations/mip_dna_observations_api.py` & `cg-59.9.1/cg/meta/observations/mip_dna_observations_api.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/observations/observations_api.py` & `cg-59.9.1/cg/meta/observations/observations_api.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/orders/api.py` & `cg-59.9.1/cg/meta/orders/api.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/orders/case_submitter.py` & `cg-59.9.1/cg/meta/orders/case_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/orders/fastq_submitter.py` & `cg-59.9.1/cg/meta/orders/fastq_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/orders/lims.py` & `cg-59.9.1/cg/meta/orders/lims.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/orders/metagenome_submitter.py` & `cg-59.9.1/cg/meta/orders/metagenome_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/orders/microbial_submitter.py` & `cg-59.9.1/cg/meta/orders/microbial_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/orders/pool_submitter.py` & `cg-59.9.1/cg/meta/orders/pool_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/orders/rnafusion_submitter.py` & `cg-59.9.1/cg/meta/orders/rnafusion_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/orders/sars_cov_2_submitter.py` & `cg-59.9.1/cg/meta/orders/sars_cov_2_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/orders/submitter.py` & `cg-59.9.1/cg/meta/orders/submitter.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/orders/ticket_handler.py` & `cg-59.9.1/cg/meta/orders/ticket_handler.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/qc_metrics/collect_qc_metrics.py` & `cg-59.9.1/cg/meta/qc_metrics/collect_qc_metrics.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/report/balsamic.py` & `cg-59.9.1/cg/meta/report/balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/report/balsamic_qc.py` & `cg-59.9.1/cg/meta/report/balsamic_qc.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/report/balsamic_umi.py` & `cg-59.9.1/cg/meta/report/balsamic_umi.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/report/field_validators.py` & `cg-59.9.1/cg/meta/report/field_validators.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/report/mip_dna.py` & `cg-59.9.1/cg/meta/report/mip_dna.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/report/report_api.py` & `cg-59.9.1/cg/meta/report/report_api.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/report/rnafusion.py` & `cg-59.9.1/cg/meta/report/rnafusion.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/report/templates/balsamic_report.html` & `cg-59.9.1/cg/meta/report/templates/balsamic_report.html`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/report/templates/bootstrap.html` & `cg-59.9.1/cg/meta/report/templates/bootstrap.html`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/report/templates/mip-dna_report.html` & `cg-59.9.1/cg/meta/report/templates/mip-dna_report.html`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/report/templates/rnafusion_report.html` & `cg-59.9.1/cg/meta/report/templates/rnafusion_report.html`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/rsync/rsync_api.py` & `cg-59.9.1/cg/meta/rsync/rsync_api.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/tar/tar.py` & `cg-59.9.1/cg/meta/tar/tar.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/transfer/external_data.py` & `cg-59.9.1/cg/meta/transfer/external_data.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/transfer/lims.py` & `cg-59.9.1/cg/meta/transfer/lims.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/upload/balsamic/balsamic.py` & `cg-59.9.1/cg/meta/upload/balsamic/balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/upload/coverage.py` & `cg-59.9.1/cg/meta/upload/coverage.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/upload/fohm/fohm.py` & `cg-59.9.1/cg/meta/upload/fohm/fohm.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/upload/gisaid/constants.py` & `cg-59.9.1/cg/meta/upload/gisaid/constants.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/upload/gisaid/gisaid.py` & `cg-59.9.1/cg/meta/upload/gisaid/gisaid.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/upload/gisaid/models.py` & `cg-59.9.1/cg/meta/upload/gisaid/models.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/upload/gt.py` & `cg-59.9.1/cg/meta/upload/gt.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/upload/microsalt/microsalt_upload_api.py` & `cg-59.9.1/cg/meta/upload/microsalt/microsalt_upload_api.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/upload/mip/mip_dna.py` & `cg-59.9.1/cg/meta/upload/mip/mip_dna.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/upload/mip/mip_rna.py` & `cg-59.9.1/cg/meta/upload/mip/mip_rna.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/upload/mutacc.py` & `cg-59.9.1/cg/meta/upload/mutacc.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/upload/nipt/models.py` & `cg-59.9.1/cg/meta/upload/nipt/models.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/upload/nipt/nipt.py` & `cg-59.9.1/cg/meta/upload/nipt/nipt.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/upload/rnafusion/rnafusion.py` & `cg-59.9.1/cg/meta/upload/rnafusion/rnafusion.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/upload/scout/balsamic_config_builder.py` & `cg-59.9.1/cg/meta/upload/scout/balsamic_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/upload/scout/balsamic_umi_config_builder.py` & `cg-59.9.1/cg/meta/upload/scout/balsamic_umi_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/upload/scout/hk_tags.py` & `cg-59.9.1/cg/meta/upload/scout/hk_tags.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/upload/scout/mip_config_builder.py` & `cg-59.9.1/cg/meta/upload/scout/mip_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/upload/scout/rnafusion_config_builder.py` & `cg-59.9.1/cg/meta/upload/scout/rnafusion_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/upload/scout/scout_config_builder.py` & `cg-59.9.1/cg/meta/upload/scout/scout_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/upload/scout/uploadscoutapi.py` & `cg-59.9.1/cg/meta/upload/scout/uploadscoutapi.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/upload/upload_api.py` & `cg-59.9.1/cg/meta/upload/upload_api.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/workflow/analysis.py` & `cg-59.9.1/cg/meta/workflow/analysis.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/workflow/balsamic.py` & `cg-59.9.1/cg/meta/workflow/balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/workflow/balsamic_pon.py` & `cg-59.9.1/cg/meta/workflow/balsamic_pon.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/workflow/balsamic_qc.py` & `cg-59.9.1/cg/meta/workflow/balsamic_qc.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/workflow/balsamic_umi.py` & `cg-59.9.1/cg/meta/workflow/balsamic_umi.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/workflow/downsample/downsample.py` & `cg-59.9.1/cg/meta/workflow/downsample/downsample.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/workflow/downsample/sbatch.py` & `cg-59.9.1/cg/meta/workflow/downsample/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/workflow/fastq.py` & `cg-59.9.1/cg/meta/workflow/fastq.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/workflow/fluffy.py` & `cg-59.9.1/cg/meta/workflow/fluffy.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/workflow/microsalt/metrics_parser/models.py` & `cg-59.9.1/cg/meta/workflow/microsalt/metrics_parser/models.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/workflow/microsalt/microsalt.py` & `cg-59.9.1/cg/meta/workflow/microsalt/microsalt.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/workflow/microsalt/quality_controller/models.py` & `cg-59.9.1/cg/meta/workflow/microsalt/quality_controller/models.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/workflow/microsalt/quality_controller/quality_controller.py` & `cg-59.9.1/cg/meta/workflow/microsalt/quality_controller/quality_controller.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/workflow/microsalt/quality_controller/report_generator.py` & `cg-59.9.1/cg/meta/workflow/microsalt/quality_controller/report_generator.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/workflow/microsalt/quality_controller/result_logger.py` & `cg-59.9.1/cg/meta/workflow/microsalt/quality_controller/result_logger.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/workflow/microsalt/quality_controller/utils.py` & `cg-59.9.1/cg/meta/workflow/microsalt/quality_controller/utils.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/workflow/microsalt/utils.py` & `cg-59.9.1/cg/meta/workflow/microsalt/utils.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/workflow/mip.py` & `cg-59.9.1/cg/meta/workflow/mip.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/workflow/mip_dna.py` & `cg-59.9.1/cg/meta/workflow/mip_dna.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/workflow/mip_rna.py` & `cg-59.9.1/cg/meta/workflow/mip_rna.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/workflow/mutant.py` & `cg-59.9.1/cg/meta/workflow/mutant.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/workflow/nf_analysis.py` & `cg-59.9.1/cg/meta/workflow/nf_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/workflow/nf_handlers.py` & `cg-59.9.1/cg/meta/workflow/nf_handlers.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/workflow/prepare_fastq.py` & `cg-59.9.1/cg/meta/workflow/prepare_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/workflow/raredisease.py` & `cg-59.9.1/cg/meta/workflow/raredisease.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/workflow/rnafusion.py` & `cg-59.9.1/cg/meta/workflow/rnafusion.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/meta/workflow/taxprofiler.py` & `cg-59.9.1/cg/meta/workflow/taxprofiler.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/models/balsamic/config.py` & `cg-59.9.1/cg/models/balsamic/config.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/models/balsamic/metrics.py` & `cg-59.9.1/cg/models/balsamic/metrics.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/models/cg_config.py` & `cg-59.9.1/cg/models/cg_config.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/models/compression_data.py` & `cg-59.9.1/cg/models/compression_data.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/models/deliverables/metric_deliverables.py` & `cg-59.9.1/cg/models/deliverables/metric_deliverables.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/models/demultiplex/run_parameters.py` & `cg-59.9.1/cg/models/demultiplex/run_parameters.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/models/demultiplex/sbatch.py` & `cg-59.9.1/cg/models/demultiplex/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/models/downsample/downsample_data.py` & `cg-59.9.1/cg/models/downsample/downsample_data.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/models/fastq.py` & `cg-59.9.1/cg/models/fastq.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/models/file_data.py` & `cg-59.9.1/cg/models/file_data.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/models/flow_cell/flow_cell.py` & `cg-59.9.1/cg/models/flow_cell/flow_cell.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/models/invoice/invoice.py` & `cg-59.9.1/cg/models/invoice/invoice.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/models/lims/sample.py` & `cg-59.9.1/cg/models/lims/sample.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/models/mip/mip_config.py` & `cg-59.9.1/cg/models/mip/mip_config.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/models/mip/mip_metrics_deliverables.py` & `cg-59.9.1/cg/models/mip/mip_metrics_deliverables.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/models/mip/mip_sample_info.py` & `cg-59.9.1/cg/models/mip/mip_sample_info.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/models/nf_analysis.py` & `cg-59.9.1/cg/models/nf_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/models/observations/input_files.py` & `cg-59.9.1/cg/models/observations/input_files.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/models/orders/constants.py` & `cg-59.9.1/cg/models/orders/constants.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/models/orders/excel_sample.py` & `cg-59.9.1/cg/models/orders/excel_sample.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/models/orders/json_sample.py` & `cg-59.9.1/cg/models/orders/json_sample.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/models/orders/order.py` & `cg-59.9.1/cg/models/orders/order.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/models/orders/orderform_schema.py` & `cg-59.9.1/cg/models/orders/orderform_schema.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/models/orders/sample_base.py` & `cg-59.9.1/cg/models/orders/sample_base.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/models/orders/samples.py` & `cg-59.9.1/cg/models/orders/samples.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/models/orders/validators/excel_sample_validators.py` & `cg-59.9.1/cg/models/orders/validators/excel_sample_validators.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/models/orders/validators/json_sample_validators.py` & `cg-59.9.1/cg/models/orders/validators/json_sample_validators.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/models/report/metadata.py` & `cg-59.9.1/cg/models/report/metadata.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/models/report/report.py` & `cg-59.9.1/cg/models/report/report.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/models/report/sample.py` & `cg-59.9.1/cg/models/report/sample.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/models/report/validators.py` & `cg-59.9.1/cg/models/report/validators.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/models/rnafusion/rnafusion.py` & `cg-59.9.1/cg/models/rnafusion/rnafusion.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/models/scout/scout_load_config.py` & `cg-59.9.1/cg/models/scout/scout_load_config.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/models/slurm/sbatch.py` & `cg-59.9.1/cg/models/slurm/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/models/taxprofiler/taxprofiler.py` & `cg-59.9.1/cg/models/taxprofiler/taxprofiler.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/models/workflow/mutant.py` & `cg-59.9.1/cg/models/workflow/mutant.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/resources/20181012_Indices.csv` & `cg-59.9.1/cg/resources/20181012_Indices.csv`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/resources/__init__.py` & `cg-59.9.1/cg/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/resources/rnafusion_bundle_filenames.csv` & `cg-59.9.1/cg/resources/rnafusion_bundle_filenames.csv`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/resources/taxprofiler_bundle_filenames.csv` & `cg-59.9.1/cg/resources/taxprofiler_bundle_filenames.csv`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/server/admin.py` & `cg-59.9.1/cg/server/admin.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/server/api.py` & `cg-59.9.1/cg/server/api.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/server/app.py` & `cg-59.9.1/cg/server/app.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/server/config.py` & `cg-59.9.1/cg/server/config.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/server/dto/orders/orders_request.py` & `cg-59.9.1/cg/server/dto/orders/orders_request.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,8 +15,7 @@
 
 class OrdersRequest(BaseModel):
     page_size: int | None = Field(alias="pageSize", default=50)
     page: int | None = 1
     sort_field: OrderSortField | None = Field(alias="sortField", default=OrderSortField.ORDER_DATE)
     sort_order: SortOrder | None = Field(alias="sortOrder", default=SortOrder.DESC)
     workflow: str | None = None
-    include_summary: bool = Field(default=False, alias="includeSummary")
```

### Comparing `cg-59.9.0/cg/server/ext.py` & `cg-59.9.1/cg/server/ext.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/server/invoices/templates/invoices/index.html` & `cg-59.9.1/cg/server/invoices/templates/invoices/index.html`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/server/invoices/templates/invoices/invoice.html` & `cg-59.9.1/cg/server/invoices/templates/invoices/invoice.html`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/server/invoices/templates/invoices/layout.html` & `cg-59.9.1/cg/server/invoices/templates/invoices/layout.html`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/server/invoices/templates/invoices/new.html` & `cg-59.9.1/cg/server/invoices/templates/invoices/new.html`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/server/invoices/views.py` & `cg-59.9.1/cg/server/invoices/views.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/services/delivery_message/delivery_message_service.py` & `cg-59.9.1/cg/services/delivery_message/delivery_message_service.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/services/delivery_message/messages/__init__.py` & `cg-59.9.1/cg/services/delivery_message/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/services/delivery_message/messages/analysis_scout_message.py` & `cg-59.9.1/cg/services/delivery_message/messages/analysis_scout_message.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/services/delivery_message/messages/covid_message.py` & `cg-59.9.1/cg/services/delivery_message/messages/covid_message.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/services/delivery_message/messages/fastq_analysis_scout_message.py` & `cg-59.9.1/cg/services/delivery_message/messages/fastq_analysis_scout_message.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/services/delivery_message/messages/fastq_message.py` & `cg-59.9.1/cg/services/delivery_message/messages/fastq_message.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/services/delivery_message/messages/fastq_scout_message.py` & `cg-59.9.1/cg/services/delivery_message/messages/fastq_scout_message.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/services/delivery_message/messages/microsalt_mwr_message.py` & `cg-59.9.1/cg/services/delivery_message/messages/microsalt_mwr_message.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/services/delivery_message/messages/microsalt_mwx_message.py` & `cg-59.9.1/cg/services/delivery_message/messages/microsalt_mwx_message.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/services/delivery_message/messages/utils.py` & `cg-59.9.1/cg/services/delivery_message/messages/utils.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/services/delivery_message/utils.py` & `cg-59.9.1/cg/services/delivery_message/utils.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/services/fastq_file_service/fastq_file_service.py` & `cg-59.9.1/cg/services/fastq_file_service/fastq_file_service.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/services/fastq_file_service/utils.py` & `cg-59.9.1/cg/services/fastq_file_service/utils.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/services/orders/order_service/order_service.py` & `cg-59.9.1/cg/services/orders/order_service/order_service.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,20 +25,16 @@
         if not order:
             raise OrderNotFoundError(f"Order {order_id} not found.")
         summary: OrderSummary = self.summary_service.get_status_summary(order_id)
         return create_order_response(order=order, summary=summary)
 
     def get_orders(self, orders_request: OrdersRequest) -> OrdersResponse:
         orders, total_count = self.store.get_orders(orders_request)
-
-        summaries: list[OrderSummary] = []
-        if orders_request.include_summary:
-            order_ids: list[int] = [order.id for order in orders]
-            summaries: list[OrderSummary] = self.summary_service.get_status_summaries(order_ids)
-
+        order_ids: list[int] = [order.id for order in orders]
+        summaries: list[OrderSummary] = self.summary_service.get_status_summaries(order_ids)
         return create_orders_response(orders=orders, summaries=summaries, total=total_count)
 
     def create_order(self, order_data: OrderIn) -> OrderResponse:
         """Creates an order and links it to the given cases."""
         order: Order = self.store.add_order(order_data)
         cases: list[Case] = self.store.get_cases_by_ticket_id(order_data.ticket)
         for case in cases:
```

### Comparing `cg-59.9.0/cg/services/orders/order_service/utils.py` & `cg-59.9.1/cg/services/orders/order_service/utils.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/services/orders/order_status_service/order_status_service.py` & `cg-59.9.1/cg/services/orders/order_status_service/order_status_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 from cg.apps.tb.api import TrailblazerAPI
 from cg.apps.tb.dto.summary_response import AnalysisSummary
-from cg.services.orders.order_status_service.dto.order_status_summary import (
-    OrderSummary,
-)
+from cg.services.orders.order_status_service.dto.order_status_summary import OrderSummary
 from cg.services.orders.order_status_service.utils import create_summaries
 from cg.store.models import Order
 from cg.store.store import Store
 
 
 class OrderStatusService:
     def __init__(self, analysis_client: TrailblazerAPI, store: Store) -> None:
```

### Comparing `cg-59.9.0/cg/services/orders/order_status_service/utils.py` & `cg-59.9.1/cg/services/orders/order_status_service/utils.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/services/slurm_service/slurm_cli_service.py` & `cg-59.9.1/cg/services/slurm_service/slurm_cli_service.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/services/slurm_upload_service/slurm_upload_service.py` & `cg-59.9.1/cg/services/slurm_upload_service/slurm_upload_service.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/store/base.py` & `cg-59.9.1/cg/store/base.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/store/crud/create.py` & `cg-59.9.1/cg/store/crud/create.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/store/crud/delete.py` & `cg-59.9.1/cg/store/crud/delete.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/store/crud/read.py` & `cg-59.9.1/cg/store/crud/read.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/store/crud/update.py` & `cg-59.9.1/cg/store/crud/update.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/store/database.py` & `cg-59.9.1/cg/store/database.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/store/filters/status_analysis_filters.py` & `cg-59.9.1/cg/store/filters/status_analysis_filters.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/store/filters/status_application_filters.py` & `cg-59.9.1/cg/store/filters/status_application_filters.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/store/filters/status_application_limitations_filters.py` & `cg-59.9.1/cg/store/filters/status_application_limitations_filters.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/store/filters/status_application_version_filters.py` & `cg-59.9.1/cg/store/filters/status_application_version_filters.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/store/filters/status_bed_filters.py` & `cg-59.9.1/cg/store/filters/status_bed_filters.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/store/filters/status_bed_version_filters.py` & `cg-59.9.1/cg/store/filters/status_bed_version_filters.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/store/filters/status_case_filters.py` & `cg-59.9.1/cg/store/filters/status_case_filters.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/store/filters/status_case_sample_filters.py` & `cg-59.9.1/cg/store/filters/status_case_sample_filters.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/store/filters/status_collaboration_filters.py` & `cg-59.9.1/cg/store/filters/status_collaboration_filters.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/store/filters/status_customer_filters.py` & `cg-59.9.1/cg/store/filters/status_customer_filters.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/store/filters/status_flow_cell_filters.py` & `cg-59.9.1/cg/store/filters/status_flow_cell_filters.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/store/filters/status_invoice_filters.py` & `cg-59.9.1/cg/store/filters/status_invoice_filters.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/store/filters/status_metrics_filters.py` & `cg-59.9.1/cg/store/filters/status_metrics_filters.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/store/filters/status_order_filters.py` & `cg-59.9.1/cg/store/filters/status_order_filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 def filter_orders_by_id(orders: Query, id: int | None, **kwargs) -> Query:
     return orders.filter(Order.id == id) if id else orders
 
 
 def filter_orders_by_ids(orders: Query, ids: list[int] | None, **kwargs) -> Query:
-    return orders.filter(Order.id.in_(ids)) if ids else orders
+    return orders.filter(Order.id.in_(ids))
 
 
 def apply_pagination(orders: Query, page: int | None, page_size: int | None, **kwargs) -> Query:
     return orders.limit(page_size).offset((page - 1) * page_size) if page and page_size else orders
 
 
 def filter_orders_by_ticket_id(orders: Query, ticket_id: int | None, **kwargs) -> Query:
```

### Comparing `cg-59.9.0/cg/store/filters/status_organism_filters.py` & `cg-59.9.1/cg/store/filters/status_organism_filters.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/store/filters/status_panel_filters.py` & `cg-59.9.1/cg/store/filters/status_panel_filters.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/store/filters/status_pool_filters.py` & `cg-59.9.1/cg/store/filters/status_pool_filters.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/store/filters/status_sample_filters.py` & `cg-59.9.1/cg/store/filters/status_sample_filters.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/store/filters/status_user_filters.py` & `cg-59.9.1/cg/store/filters/status_user_filters.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/store/models.py` & `cg-59.9.1/cg/store/models.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/store/store.py` & `cg-59.9.1/cg/store/store.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/utils/checksum/checksum.py` & `cg-59.9.1/cg/utils/checksum/checksum.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/utils/click/EnumChoice.py` & `cg-59.9.1/cg/utils/click/EnumChoice.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/utils/commands.py` & `cg-59.9.1/cg/utils/commands.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/utils/date.py` & `cg-59.9.1/cg/utils/date.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/utils/dict.py` & `cg-59.9.1/cg/utils/dict.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/utils/dispatcher.py` & `cg-59.9.1/cg/utils/dispatcher.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/utils/email.py` & `cg-59.9.1/cg/utils/email.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/utils/files.py` & `cg-59.9.1/cg/utils/files.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/utils/flask/enum.py` & `cg-59.9.1/cg/utils/flask/enum.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/utils/time.py` & `cg-59.9.1/cg/utils/time.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/cg/utils/utils.py` & `cg-59.9.1/cg/utils/utils.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/pyproject.toml` & `cg-59.9.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "cg"
-version = "59.9.0"
+version = "59.9.1"
 description = "Clinical Genomics command center"
 authors = ["Clinical Genomics <support@clinicalgenomics.se>"]
 readme = "README.md"
 homepage = "https://github.com/Clinical-Genomics/cg"
 repository = "https://github.com/Clinical-Genomics/cg"
 classifiers = [
   "Programming Language :: Python",
@@ -76,24 +76,22 @@
 coveralls = "*"
 mock = "*"
 pre-commit = "*"
 pytest-cov = "*"
 pytest-mock = "*"
 pytest = "*"
 ruff = "*"
+pytest-xdist = "*"
 
 [tool.poetry.scripts]
 cg = "cg.cli.base:base"
 
 
 # Configurations
 
-[tool.poetry.group.dev.dependencies]
-pytest-xdist = "^3.5.0"
-
 [tool.black]
 line-length = 100
 
 [tool.isort]
 profile = "black"
 
 [tool.ruff]
```

### Comparing `cg-59.9.0/tests/apps/conftest.py` & `cg-59.9.1/tests/apps/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/apps/coverage/test_coverage.py` & `cg-59.9.1/tests/apps/coverage/test_coverage.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/apps/crunchy/conftest.py` & `cg-59.9.1/tests/apps/crunchy/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/apps/crunchy/test_compress_fastq.py` & `cg-59.9.1/tests/apps/crunchy/test_compress_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/apps/crunchy/test_config.py` & `cg-59.9.1/tests/apps/crunchy/test_config.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/apps/crunchy/test_crunchy.py` & `cg-59.9.1/tests/apps/crunchy/test_crunchy.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/apps/crunchy/test_spring_decompression.py` & `cg-59.9.1/tests/apps/crunchy/test_spring_decompression.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/apps/demultiplex/conftest.py` & `cg-59.9.1/tests/apps/demultiplex/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/apps/demultiplex/test_demultiplex_api.py` & `cg-59.9.1/tests/apps/demultiplex/test_demultiplex_api.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/apps/demultiplex/test_index.py` & `cg-59.9.1/tests/apps/demultiplex/test_index.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/apps/demultiplex/test_override_cycles_validator.py` & `cg-59.9.1/tests/apps/demultiplex/test_override_cycles_validator.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/apps/demultiplex/test_read_sample_sheet.py` & `cg-59.9.1/tests/apps/demultiplex/test_read_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/apps/demultiplex/test_sample_models.py` & `cg-59.9.1/tests/apps/demultiplex/test_sample_models.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/apps/demultiplex/test_sample_sheet_creator.py` & `cg-59.9.1/tests/apps/demultiplex/test_sample_sheet_creator.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/apps/demultiplex/test_sample_sheet_creator_factory.py` & `cg-59.9.1/tests/apps/demultiplex/test_sample_sheet_creator_factory.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/apps/demultiplex/test_sample_sheet_models.py` & `cg-59.9.1/tests/apps/demultiplex/test_sample_sheet_models.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/apps/demultiplex/test_sample_sheet_validator.py` & `cg-59.9.1/tests/apps/demultiplex/test_sample_sheet_validator.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/apps/demultiplex/test_validate.py` & `cg-59.9.1/tests/apps/demultiplex/test_validate.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/apps/downsample/test_downsample.py` & `cg-59.9.1/tests/apps/downsample/test_downsample.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/apps/downsample/test_downsample_utils.py` & `cg-59.9.1/tests/apps/downsample/test_downsample_utils.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/apps/gens/test_gens_api.py` & `cg-59.9.1/tests/apps/gens/test_gens_api.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/apps/gt/conftest.py` & `cg-59.9.1/tests/apps/gt/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/apps/gt/test_gt_api.py` & `cg-59.9.1/tests/apps/gt/test_gt_api.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/apps/hk/conftest.py` & `cg-59.9.1/tests/apps/hk/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/apps/hk/test__getattr__.py` & `cg-59.9.1/tests/apps/hk/test__getattr__.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/apps/hk/test_add_file.py` & `cg-59.9.1/tests/apps/hk/test_add_file.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/apps/hk/test_bundles.py` & `cg-59.9.1/tests/apps/hk/test_bundles.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/apps/hk/test_core.py` & `cg-59.9.1/tests/apps/hk/test_core.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/apps/hk/test_file.py` & `cg-59.9.1/tests/apps/hk/test_file.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/apps/hk/test_version.py` & `cg-59.9.1/tests/apps/hk/test_version.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/apps/lims/conftest.py` & `cg-59.9.1/tests/apps/lims/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/apps/lims/test_api.py` & `cg-59.9.1/tests/apps/lims/test_api.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/apps/lims/test_sample_sheet.py` & `cg-59.9.1/tests/apps/lims/test_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/apps/loqus/conftest.py` & `cg-59.9.1/tests/apps/loqus/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/apps/loqus/test_loqusdb_api.py` & `cg-59.9.1/tests/apps/loqus/test_loqusdb_api.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/apps/madeline/conftest.py` & `cg-59.9.1/tests/apps/madeline/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/apps/madeline/test_madeline.py` & `cg-59.9.1/tests/apps/madeline/test_madeline.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/apps/mip/conftest.py` & `cg-59.9.1/tests/apps/mip/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/apps/mip/test_config_mip.py` & `cg-59.9.1/tests/apps/mip/test_config_mip.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/apps/mutacc_auto/conftest.py` & `cg-59.9.1/tests/apps/mutacc_auto/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/apps/mutacc_auto/test_mutacc_auto.py` & `cg-59.9.1/tests/apps/mutacc_auto/test_mutacc_auto.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/apps/orderform/conftest.py` & `cg-59.9.1/tests/apps/orderform/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/apps/orderform/test_excel_orderform_parser.py` & `cg-59.9.1/tests/apps/orderform/test_excel_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/apps/orderform/test_excel_sample_schema.py` & `cg-59.9.1/tests/apps/orderform/test_excel_sample_schema.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/apps/orderform/test_json_orderform_parser.py` & `cg-59.9.1/tests/apps/orderform/test_json_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/apps/orderform/test_orderform_parser.py` & `cg-59.9.1/tests/apps/orderform/test_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/apps/orderform/validators/test_excel_sample_validators.py` & `cg-59.9.1/tests/apps/orderform/validators/test_excel_sample_validators.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/apps/scout/conftest.py` & `cg-59.9.1/tests/apps/scout/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/apps/scout/test_get_causative_variants.py` & `cg-59.9.1/tests/apps/scout/test_get_causative_variants.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/apps/scout/test_get_scout_cases.py` & `cg-59.9.1/tests/apps/scout/test_get_scout_cases.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/apps/scout/test_scout_load_config.py` & `cg-59.9.1/tests/apps/scout/test_scout_load_config.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/apps/scout/test_scout_models.py` & `cg-59.9.1/tests/apps/scout/test_scout_models.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/apps/sequencing_metrics_parser/conftest.py` & `cg-59.9.1/tests/apps/sequencing_metrics_parser/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/apps/sequencing_metrics_parser/parsers/conftest.py` & `cg-59.9.1/tests/apps/sequencing_metrics_parser/parsers/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/apps/sequencing_metrics_parser/parsers/test_bcl2fastq_parser.py` & `cg-59.9.1/tests/apps/sequencing_metrics_parser/parsers/test_bcl2fastq_parser.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/apps/sequencing_metrics_parser/parsers/test_bcl2fastq_to_sequencing_statistics.py` & `cg-59.9.1/tests/apps/sequencing_metrics_parser/parsers/test_bcl2fastq_to_sequencing_statistics.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/apps/sequencing_metrics_parser/parsers/test_bcl_convert_to_sequencing_statistics.py` & `cg-59.9.1/tests/apps/sequencing_metrics_parser/parsers/test_bcl_convert_to_sequencing_statistics.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/apps/sequencing_metrics_parser/parsers/test_bclconvert.py` & `cg-59.9.1/tests/apps/sequencing_metrics_parser/parsers/test_bclconvert.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/apps/sequencing_metrics_parser/test_sequencing_metrics_calculator.py` & `cg-59.9.1/tests/apps/sequencing_metrics_parser/test_sequencing_metrics_calculator.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/apps/slurm/conftest.py` & `cg-59.9.1/tests/apps/slurm/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/apps/slurm/test_slurm_api.py` & `cg-59.9.1/tests/apps/slurm/test_slurm_api.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/apps/test_apps_environ.py` & `cg-59.9.1/tests/apps/test_apps_environ.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/apps/test_osticket.py` & `cg-59.9.1/tests/apps/test_osticket.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/add/test_cli_add.py` & `cg-59.9.1/tests/cli/add/test_cli_add.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/add/test_cli_add_customer.py` & `cg-59.9.1/tests/cli/add/test_cli_add_customer.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/add/test_cli_add_family.py` & `cg-59.9.1/tests/cli/add/test_cli_add_family.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/add/test_cli_add_relationship.py` & `cg-59.9.1/tests/cli/add/test_cli_add_relationship.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/add/test_cli_add_sample.py` & `cg-59.9.1/tests/cli/add/test_cli_add_sample.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/backup/conftest.py` & `cg-59.9.1/tests/cli/backup/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/backup/test_backup_command.py` & `cg-59.9.1/tests/cli/backup/test_backup_command.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/clean/conftest.py` & `cg-59.9.1/tests/cli/clean/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/clean/test_balsamic_clean.py` & `cg-59.9.1/tests/cli/clean/test_balsamic_clean.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/clean/test_clean_flow_cell.py` & `cg-59.9.1/tests/cli/clean/test_clean_flow_cell.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/clean/test_clean_hk_bundle_files.py` & `cg-59.9.1/tests/cli/clean/test_clean_hk_bundle_files.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/clean/test_hk_bundle_files.py` & `cg-59.9.1/tests/cli/clean/test_hk_bundle_files.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/clean/test_hk_case_bundle_files.py` & `cg-59.9.1/tests/cli/clean/test_hk_case_bundle_files.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/clean/test_microbial_clean.py` & `cg-59.9.1/tests/cli/clean/test_microbial_clean.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/clean/test_rsync_past_run_dirs.py` & `cg-59.9.1/tests/cli/clean/test_rsync_past_run_dirs.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/compress/conftest.py` & `cg-59.9.1/tests/cli/compress/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/compress/test_cli_compress_fastq.py` & `cg-59.9.1/tests/cli/compress/test_cli_compress_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/compress/test_cli_decompress_spring.py` & `cg-59.9.1/tests/cli/compress/test_cli_decompress_spring.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/compress/test_compress_helpers.py` & `cg-59.9.1/tests/cli/compress/test_compress_helpers.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/compress/test_store_fastq.py` & `cg-59.9.1/tests/cli/compress/test_store_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/conftest.py` & `cg-59.9.1/tests/cli/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/delete/test_cli_delete_case.py` & `cg-59.9.1/tests/cli/delete/test_cli_delete_case.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/delete/test_cli_delete_cases.py` & `cg-59.9.1/tests/cli/delete/test_cli_delete_cases.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/deliver/conftest.py` & `cg-59.9.1/tests/cli/deliver/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/deliver/test_deliver_base.py` & `cg-59.9.1/tests/cli/deliver/test_deliver_base.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/deliver/test_rsync_base.py` & `cg-59.9.1/tests/cli/deliver/test_rsync_base.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/deliver/test_run_deliver_cmd.py` & `cg-59.9.1/tests/cli/deliver/test_run_deliver_cmd.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/demultiplex/test_create_sample_sheet.py` & `cg-59.9.1/tests/cli/demultiplex/test_create_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/demultiplex/test_demultiplex_flowcell.py` & `cg-59.9.1/tests/cli/demultiplex/test_demultiplex_flowcell.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/demultiplex/test_finish_demux.py` & `cg-59.9.1/tests/cli/demultiplex/test_finish_demux.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/demultiplex/test_validate_sample_sheet.py` & `cg-59.9.1/tests/cli/demultiplex/test_validate_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/demultiplex/test_verify_syncing.py` & `cg-59.9.1/tests/cli/demultiplex/test_verify_syncing.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/downsample/test_cli_downsample.py` & `cg-59.9.1/tests/cli/downsample/test_cli_downsample.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/generate/report/conftest.py` & `cg-59.9.1/tests/cli/generate/report/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/generate/report/test_cli_delivery_report.py` & `cg-59.9.1/tests/cli/generate/report/test_cli_delivery_report.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/generate/report/test_utils.py` & `cg-59.9.1/tests/cli/generate/report/test_utils.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/generate/test_cli_base.py` & `cg-59.9.1/tests/cli/generate/test_cli_base.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/get/test_cli_get.py` & `cg-59.9.1/tests/cli/get/test_cli_get.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/get/test_cli_get_analysis.py` & `cg-59.9.1/tests/cli/get/test_cli_get_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/get/test_cli_get_case.py` & `cg-59.9.1/tests/cli/get/test_cli_get_case.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/get/test_cli_get_flow_cell.py` & `cg-59.9.1/tests/cli/get/test_cli_get_flow_cell.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/get/test_cli_get_sample.py` & `cg-59.9.1/tests/cli/get/test_cli_get_sample.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/set/conftest.py` & `cg-59.9.1/tests/cli/set/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/set/test_cli_set_case.py` & `cg-59.9.1/tests/cli/set/test_cli_set_case.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/set/test_cli_set_cases.py` & `cg-59.9.1/tests/cli/set/test_cli_set_cases.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/set/test_cli_set_flowcell.py` & `cg-59.9.1/tests/cli/set/test_cli_set_flowcell.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/set/test_cli_set_list_keys.py` & `cg-59.9.1/tests/cli/set/test_cli_set_list_keys.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/set/test_cli_set_sample.py` & `cg-59.9.1/tests/cli/set/test_cli_set_sample.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/set/test_cli_set_samples.py` & `cg-59.9.1/tests/cli/set/test_cli_set_samples.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/store/test_fastq.py` & `cg-59.9.1/tests/cli/store/test_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/test_base.py` & `cg-59.9.1/tests/cli/test_base.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/upload/conftest.py` & `cg-59.9.1/tests/cli/upload/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/upload/test_cli_scout.py` & `cg-59.9.1/tests/cli/upload/test_cli_scout.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/upload/test_cli_upload.py` & `cg-59.9.1/tests/cli/upload/test_cli_upload.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/upload/test_cli_upload_auto.py` & `cg-59.9.1/tests/cli/upload/test_cli_upload_auto.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/upload/test_cli_upload_delivery_report.py` & `cg-59.9.1/tests/cli/upload/test_cli_upload_delivery_report.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/upload/test_cli_upload_fastq.py` & `cg-59.9.1/tests/cli/upload/test_cli_upload_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/upload/test_cli_upload_genotype.py` & `cg-59.9.1/tests/cli/upload/test_cli_upload_genotype.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/upload/test_cli_upload_gens.py` & `cg-59.9.1/tests/cli/upload/test_cli_upload_gens.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/upload/test_cli_upload_nipt.py` & `cg-59.9.1/tests/cli/upload/test_cli_upload_nipt.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/upload/test_cli_upload_nipt_ftp.py` & `cg-59.9.1/tests/cli/upload/test_cli_upload_nipt_ftp.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/upload/test_cli_upload_nipt_statina.py` & `cg-59.9.1/tests/cli/upload/test_cli_upload_nipt_statina.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/upload/test_cli_upload_observations.py` & `cg-59.9.1/tests/cli/upload/test_cli_upload_observations.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/workflow/balsamic/conftest.py` & `cg-59.9.1/tests/cli/workflow/balsamic/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/workflow/balsamic/test_cli_balsamic_config_case.py` & `cg-59.9.1/tests/cli/workflow/balsamic/test_cli_balsamic_config_case.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/workflow/balsamic/test_compound_commands.py` & `cg-59.9.1/tests/cli/workflow/balsamic/test_compound_commands.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/workflow/balsamic/test_link.py` & `cg-59.9.1/tests/cli/workflow/balsamic/test_link.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/workflow/balsamic/test_report_deliver.py` & `cg-59.9.1/tests/cli/workflow/balsamic/test_report_deliver.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/workflow/balsamic/test_run.py` & `cg-59.9.1/tests/cli/workflow/balsamic/test_run.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/workflow/balsamic/test_store_housekeeper.py` & `cg-59.9.1/tests/cli/workflow/balsamic/test_store_housekeeper.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/workflow/conftest.py` & `cg-59.9.1/tests/cli/workflow/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/workflow/fastq/test_fastq_base.py` & `cg-59.9.1/tests/cli/workflow/fastq/test_fastq_base.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/workflow/fluffy/conftest.py` & `cg-59.9.1/tests/cli/workflow/fluffy/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/workflow/fluffy/test_cli_create_samplesheet.py` & `cg-59.9.1/tests/cli/workflow/fluffy/test_cli_create_samplesheet.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/workflow/fluffy/test_cli_link.py` & `cg-59.9.1/tests/cli/workflow/fluffy/test_cli_link.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/workflow/fluffy/test_cli_run.py` & `cg-59.9.1/tests/cli/workflow/fluffy/test_cli_run.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/workflow/fluffy/test_cli_start.py` & `cg-59.9.1/tests/cli/workflow/fluffy/test_cli_start.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/workflow/fluffy/test_cli_store.py` & `cg-59.9.1/tests/cli/workflow/fluffy/test_cli_store.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/workflow/microsalt/conftest.py` & `cg-59.9.1/tests/cli/workflow/microsalt/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/workflow/microsalt/test_microsalt_case_config.py` & `cg-59.9.1/tests/cli/workflow/microsalt/test_microsalt_case_config.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/workflow/microsalt/test_microsalt_run.py` & `cg-59.9.1/tests/cli/workflow/microsalt/test_microsalt_run.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/workflow/mip/conftest.py` & `cg-59.9.1/tests/cli/workflow/mip/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/workflow/mip/test_cli_mip_base.py` & `cg-59.9.1/tests/cli/workflow/mip/test_cli_mip_base.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/workflow/mip/test_cli_mip_dna_config_case.py` & `cg-59.9.1/tests/cli/workflow/mip/test_cli_mip_dna_config_case.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/workflow/mip/test_cli_mip_dna_manged_variants.py` & `cg-59.9.1/tests/cli/workflow/mip/test_cli_mip_dna_manged_variants.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/workflow/mip/test_cli_mip_dna_panel.py` & `cg-59.9.1/tests/cli/workflow/mip/test_cli_mip_dna_panel.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/workflow/mip/test_cli_mip_dna_run.py` & `cg-59.9.1/tests/cli/workflow/mip/test_cli_mip_dna_run.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/workflow/mip/test_cli_mip_dna_start.py` & `cg-59.9.1/tests/cli/workflow/mip/test_cli_mip_dna_start.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/workflow/mip/test_cli_mip_rna_config_case.py` & `cg-59.9.1/tests/cli/workflow/mip/test_cli_mip_rna_config_case.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/workflow/mip/test_cli_mip_rna_link.py` & `cg-59.9.1/tests/cli/workflow/mip/test_cli_mip_rna_link.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/workflow/mip/test_cli_mip_rna_run.py` & `cg-59.9.1/tests/cli/workflow/mip/test_cli_mip_rna_run.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/workflow/mip/test_cli_mip_store.py` & `cg-59.9.1/tests/cli/workflow/mip/test_cli_mip_store.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/workflow/nf_analysis/test_cli_config_case.py` & `cg-59.9.1/tests/cli/workflow/nf_analysis/test_cli_config_case.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/workflow/nf_analysis/test_cli_metrics_deliver.py` & `cg-59.9.1/tests/cli/workflow/nf_analysis/test_cli_metrics_deliver.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/workflow/nf_analysis/test_cli_report_deliver.py` & `cg-59.9.1/tests/cli/workflow/nf_analysis/test_cli_report_deliver.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/workflow/raredisease/test_cli_raredisease_compound_commands.py` & `cg-59.9.1/tests/cli/workflow/raredisease/test_cli_raredisease_compound_commands.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/workflow/rnafusion/test_cli_rnafusion_compound_commands.py` & `cg-59.9.1/tests/cli/workflow/rnafusion/test_cli_rnafusion_compound_commands.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/workflow/rnafusion/test_cli_rnafusion_config_case.py` & `cg-59.9.1/tests/cli/workflow/rnafusion/test_cli_rnafusion_config_case.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/workflow/rnafusion/test_cli_rnafusion_metrics_deliver.py` & `cg-59.9.1/tests/cli/workflow/rnafusion/test_cli_rnafusion_metrics_deliver.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/workflow/rnafusion/test_cli_rnafusion_run.py` & `cg-59.9.1/tests/cli/workflow/rnafusion/test_cli_rnafusion_run.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/workflow/rnafusion/test_cli_rnafusion_store_housekeeper.py` & `cg-59.9.1/tests/cli/workflow/rnafusion/test_cli_rnafusion_store_housekeeper.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/workflow/taxprofiler/test_cli_taxprofiler_compound_commands.py` & `cg-59.9.1/tests/cli/workflow/taxprofiler/test_cli_taxprofiler_compound_commands.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/workflow/taxprofiler/test_cli_taxprofiler_config_case.py` & `cg-59.9.1/tests/cli/workflow/taxprofiler/test_cli_taxprofiler_config_case.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/workflow/taxprofiler/test_cli_taxprofiler_metrics_deliver.py` & `cg-59.9.1/tests/cli/workflow/taxprofiler/test_cli_taxprofiler_metrics_deliver.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/workflow/taxprofiler/test_cli_taxprofiler_run.py` & `cg-59.9.1/tests/cli/workflow/taxprofiler/test_cli_taxprofiler_run.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/workflow/test_cli_workflow.py` & `cg-59.9.1/tests/cli/workflow/test_cli_workflow.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/cli/workflow/test_cli_workflow_clean.py` & `cg-59.9.1/tests/cli/workflow/test_cli_workflow_clean.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/clients/conftest.py` & `cg-59.9.1/tests/clients/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/clients/janus/test_janus_api_client.py` & `cg-59.9.1/tests/clients/janus/test_janus_api_client.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/conftest.py` & `cg-59.9.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixture_plugins/demultiplex_fixtures/flow_cell_fixtures.py` & `cg-59.9.1/tests/fixture_plugins/demultiplex_fixtures/flow_cell_fixtures.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixture_plugins/demultiplex_fixtures/name_fixtures.py` & `cg-59.9.1/tests/fixture_plugins/demultiplex_fixtures/name_fixtures.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixture_plugins/demultiplex_fixtures/path_fixtures.py` & `cg-59.9.1/tests/fixture_plugins/demultiplex_fixtures/path_fixtures.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixture_plugins/demultiplex_fixtures/run_parameters_fixtures.py` & `cg-59.9.1/tests/fixture_plugins/demultiplex_fixtures/run_parameters_fixtures.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixture_plugins/demultiplex_fixtures/sample_fixtures.py` & `cg-59.9.1/tests/fixture_plugins/demultiplex_fixtures/sample_fixtures.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixture_plugins/demultiplex_fixtures/sample_sheet_fixtures.py` & `cg-59.9.1/tests/fixture_plugins/demultiplex_fixtures/sample_sheet_fixtures.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixture_plugins/timestamp_fixtures.py` & `cg-59.9.1/tests/fixture_plugins/timestamp_fixtures.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/ACC11111_qc_fail.json` & `cg-59.9.1/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/ACC11111_qc_fail.json`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/ACC22222_qc_pass.json` & `cg-59.9.1/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/ACC22222_qc_pass.json`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/analysis/rnafusion/multiqc_data.json` & `cg-59.9.1/tests/fixtures/analysis/rnafusion/multiqc_data.json`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/analysis/rnafusion/rnafusion_case_enough_reads_metrics_deliverables.yaml` & `cg-59.9.1/tests/fixtures/analysis/rnafusion/rnafusion_case_enough_reads_metrics_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/analysis/sample_coverage.bed` & `cg-59.9.1/tests/fixtures/analysis/sample_coverage.bed`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/analysis/taxprofiler/multiqc_data.json` & `cg-59.9.1/tests/fixtures/analysis/taxprofiler/multiqc_data.json`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/analysis/taxprofiler/taxprofiler_case_metrics_deliverables.yaml` & `cg-59.9.1/tests/fixtures/analysis/taxprofiler/taxprofiler_case_metrics_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/balsamic/case/config.json` & `cg-59.9.1/tests/fixtures/apps/balsamic/case/config.json`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/balsamic/case/metadata.yml` & `cg-59.9.1/tests/fixtures/apps/balsamic/case/metadata.yml`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/balsamic/case/metrics_deliverables.yaml` & `cg-59.9.1/tests/fixtures/apps/balsamic/case/metrics_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/crunchy/spring_metadata.json` & `cg-59.9.1/tests/fixtures/apps/crunchy/spring_metadata.json`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/l1t11/Stats/Stats.json` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/l1t11/Stats/Stats.json`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/l1t21/Stats/Stats.json` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/170407_ST-E00198_0209_BHHKVCALXX/l1t21/Stats/Stats.json`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/Reports/Demultiplex_Stats.csv` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/Reports/Demultiplex_Stats.csv`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/Reports/Quality_Metrics.csv` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/Reports/Quality_Metrics.csv`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/SampleSheet.csv` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/20230508_LH00188_0003_A22522YLT3/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRZZ/Unaligned/Reports/RunInfo.xml` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRZZ/Unaligned/Reports/RunInfo.xml`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/SampleSheet.csv` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Reports/Quality_Metrics.csv` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230504_A00689_0804_BHY7FFDRX2/Unaligned/Reports/Quality_Metrics.csv`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/Reports/Demultiplex_Stats.csv` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/Reports/Demultiplex_Stats.csv`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/Reports/Quality_Metrics.csv` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/Reports/Quality_Metrics.csv`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/SampleSheet.csv` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/230505_A00689_0804_BHY7FFDRX2/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_D00483_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/fastq/fastq_run_R1_001.fastq.gz` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/fastq/fastq_run_R1_001.fastq.gz`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/fastq/fastq_run_R2_001.fastq.gz` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/fastq/fastq_run_R2_001.fastq.gz`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/HJCFFALXX_bcl2fastq_raw.json` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/HJCFFALXX_bcl2fastq_raw.json`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/HJCFFALXX_bcl_convert_raw.json` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/HJCFFALXX_bcl_convert_raw.json`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTAConfiguration.xml` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RTAConfiguration.xml`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RunInfo.xml` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/RunInfo.xml`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet.csv` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet_bcl2fastq.csv` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/SampleSheet_bcl2fastq.csv`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/runParameters.xml` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/170517_ST-E00266_0210_BHJCFFALXX/runParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/HL32LCCXY_bcl2fastq_raw.json` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/HL32LCCXY_bcl2fastq_raw.json`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/HL32LCCXY_bcl_convert_raw.json` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/HL32LCCXY_bcl_convert_raw.json`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTAConfiguration.xml` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RTAConfiguration.xml`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RunInfo.xml` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/RunInfo.xml`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/SampleSheet.csv` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/SampleSheet_bcl2fastq.csv` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/SampleSheet_bcl2fastq.csv`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/runParameters.xml` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180508_ST-E00269_0269_AHL32LCCXY/runParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/HGYFNBCX2_bcl2fastq_raw.json` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/HGYFNBCX2_bcl2fastq_raw.json`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/HGYFNBCX2_bcl_convert_raw.json` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/HGYFNBCX2_bcl_convert_raw.json`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/RunInfo.xml` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/RunInfo.xml`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/SampleSheet.csv` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/SampleSheet_bcl2fastq.csv` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/SampleSheet_bcl2fastq.csv`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/runParameters.xml` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/180509_D00450_0598_BHGYFNBCX2/runParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/HM2LNBCX2_bcl2fastq_raw.json` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/HM2LNBCX2_bcl2fastq_raw.json`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/HM2LNBCX2_bcl_convert_raw.json` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/HM2LNBCX2_bcl_convert_raw.json`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/RunInfo.xml` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/RunInfo.xml`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/SampleSheet.csv` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/SampleSheet_bcl2fastq.csv` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/SampleSheet_bcl2fastq.csv`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/runParameters.xml` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/181005_D00410_0735_BHM2LNBCX2/runParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/CorrectSampleSheet.csv` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/CorrectSampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/HLYWYDSXX_bcl2fastq_raw.json` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/HLYWYDSXX_bcl2fastq_raw.json`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/HLYWYDSXX_bcl_convert_raw.json` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/HLYWYDSXX_bcl_convert_raw.json`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RTA3.cfg` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RTA3.cfg`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RunInfo.xml` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RunInfo.xml`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RunParameters.xml` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/190927_A00689_0069_BHLYWYDSXX/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/HVKJCDRXX_demultiplex.stderr` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/HVKJCDRXX_demultiplex.stderr`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/HVKJCDRXX_demultiplex.stdout` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/HVKJCDRXX_demultiplex.stdout`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/RunParameters.xml` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_A00689_0200_AHVKJCDRXY/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stdout` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stdout`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_raw.json` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/HVKJCDRXX_raw.json`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/RunParameters.xml` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/201203_D00483_0200_AHVKJCDRXX/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/22F52TLT3_raw.json` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/22F52TLT3_raw.json`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/CorrectSampleSheet.csv` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/CorrectSampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RTA.cfg` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RTA.cfg`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunCompletionStatus.xml` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunCompletionStatus.xml`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunInfo.xml` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunInfo.xml`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunParameters.xml` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/20231108_LH00188_0028_B22F52TLT3/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stdout` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stdout`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/RunParameters.xml` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/SampleSheet.csv` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_A00187_0615_AHLG5GDRZZ/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/RunParameters.xml` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/211101_D00483_0615_AHLG5GDRXY/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/CorrectSampleSheet.csv` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/CorrectSampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/HK33MDRX3_bcl_convert_raw.json` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/HK33MDRX3_bcl_convert_raw.json`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RTA3.cfg` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RTA3.cfg`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RunInfo.xml` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RunInfo.xml`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RunParameters.xml` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/SampleSheet.csv` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells/230912_A00187_1009_AHK33MDRX3/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells_broken/190927_A00689_0069_BHLYWYDSXX/RunParameters.xml` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/190927_A00689_0069_BHLYWYDSXX/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells_broken/20231108_LH00188_0028_B22F52TLT3/RunParameters.xml` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/20231108_LH00188_0028_B22F52TLT3/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells_broken/230912_A00187_1009_AHK33MDRX3/RunParameters.xml` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells_broken/230912_A00187_1009_AHK33MDRX3/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/RunParameters.xml` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRXY/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stdout` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/HLG5GDRZZ_demultiplex.stdout`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/RunParameters.xml` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/flow_cells_demux_all/211101_A00187_0615_AHLG5GDRZZ/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/raw_lims_samples/raw_samplesheet_novaseq.json` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/raw_lims_samples/raw_samplesheet_novaseq.json`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_hiseq_2500_different_index_cycles.xml` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_hiseq_2500_different_index_cycles.xml`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_6000_different_index_cycles.xml` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_6000_different_index_cycles.xml`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_X_different_index_cycles.xml` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_X_different_index_cycles.xml`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_X_wrong_instrument.xml` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_X_wrong_instrument.xml`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_no_software_nor_reagent_version.xml` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/run_parameters/RunParameters_novaseq_no_software_nor_reagent_version.xml`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/sample_sheets/novaseq_6000_sample_sheet_with_reversed_cycles.csv` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/sample_sheets/novaseq_6000_sample_sheet_with_reversed_cycles.csv`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/demultiplexing/sample_sheets/novaseq_x_sample_sheet_with_forward_cycles.csv` & `cg-59.9.1/tests/fixtures/apps/demultiplexing/sample_sheets/novaseq_x_sample_sheet_with_forward_cycles.csv`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/fluffy/SampleSheet.csv` & `cg-59.9.1/tests/fixtures/apps/fluffy/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/fluffy/deliverables.yaml` & `cg-59.9.1/tests/fixtures/apps/fluffy/deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/madeline/madeline.xml` & `cg-59.9.1/tests/fixtures/apps/madeline/madeline.xml`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/mip/case_metrics_deliverables.yaml` & `cg-59.9.1/tests/fixtures/apps/mip/case_metrics_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/mip/dna/store/case_config.yaml` & `cg-59.9.1/tests/fixtures/apps/mip/dna/store/case_config.yaml`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/mip/dna/store/case_id_deliverables.yaml` & `cg-59.9.1/tests/fixtures/apps/mip/dna/store/case_id_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/mip/dna/store/case_qc_sample_info.yaml` & `cg-59.9.1/tests/fixtures/apps/mip/dna/store/case_qc_sample_info.yaml`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/mip/dna/store/yellowhog_clinical_selected.vcf` & `cg-59.9.1/tests/fixtures/apps/mip/dna/store/yellowhog_clinical_selected.vcf`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/mip/rna/case_config.yaml` & `cg-59.9.1/tests/fixtures/apps/mip/rna/case_config.yaml`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/mip/rna/case_qc_sampleinfo.yaml` & `cg-59.9.1/tests/fixtures/apps/mip/rna/case_qc_sampleinfo.yaml`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/mip/rna/store/bundle_data.yaml` & `cg-59.9.1/tests/fixtures/apps/mip/rna/store/bundle_data.yaml`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/mip/rna/store/case_config.yaml` & `cg-59.9.1/tests/fixtures/apps/mip/rna/store/case_config.yaml`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/mip/rna/store/case_id_deliverables.yaml` & `cg-59.9.1/tests/fixtures/apps/mip/rna/store/case_id_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/mip/rna/store/case_qc_sample_info.yaml` & `cg-59.9.1/tests/fixtures/apps/mip/rna/store/case_qc_sample_info.yaml`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/scout/643594.config.yaml` & `cg-59.9.1/tests/fixtures/apps/scout/643594.config.yaml`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/scout/case_export.json` & `cg-59.9.1/tests/fixtures/apps/scout/case_export.json`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/scout/export_causatives.json` & `cg-59.9.1/tests/fixtures/apps/scout/export_causatives.json`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/scout/none_case_export.json` & `cg-59.9.1/tests/fixtures/apps/scout/none_case_export.json`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/scout/other_sex_case.json` & `cg-59.9.1/tests/fixtures/apps/scout/other_sex_case.json`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/scout/panel_export.bed` & `cg-59.9.1/tests/fixtures/apps/scout/panel_export.bed`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/scout/panel_export.csv` & `cg-59.9.1/tests/fixtures/apps/scout/panel_export.csv`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Adapter_Metrics.csv` & `cg-59.9.1/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Adapter_Metrics.csv`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Demultiplex_Stats.csv` & `cg-59.9.1/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Demultiplex_Stats.csv`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Quality_Metrics.csv` & `cg-59.9.1/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/Quality_Metrics.csv`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/SampleSheet.csv` & `cg-59.9.1/tests/fixtures/apps/sequencing_metrics_parser/230622_A00621_0864_AHY7FFDRX2/Unaligned/Reports/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/cgweb_orders/balsamic.json` & `cg-59.9.1/tests/fixtures/cgweb_orders/balsamic.json`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/cgweb_orders/fastq.json` & `cg-59.9.1/tests/fixtures/cgweb_orders/fastq.json`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/cgweb_orders/metagenome.json` & `cg-59.9.1/tests/fixtures/cgweb_orders/metagenome.json`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/cgweb_orders/microsalt.json` & `cg-59.9.1/tests/fixtures/cgweb_orders/microsalt.json`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/cgweb_orders/mip.json` & `cg-59.9.1/tests/fixtures/cgweb_orders/mip.json`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/cgweb_orders/mip_rna.json` & `cg-59.9.1/tests/fixtures/cgweb_orders/mip_rna.json`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/cgweb_orders/rml.json` & `cg-59.9.1/tests/fixtures/cgweb_orders/rml.json`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/cgweb_orders/rnafusion.json` & `cg-59.9.1/tests/fixtures/cgweb_orders/rnafusion.json`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/cgweb_orders/sarscov2.json` & `cg-59.9.1/tests/fixtures/cgweb_orders/sarscov2.json`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/data/SampleSheet.csv` & `cg-59.9.1/tests/fixtures/data/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/data/cgfixture.db` & `cg-59.9.1/tests/fixtures/data/cgfixture.db`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/data/hkstore.db` & `cg-59.9.1/tests/fixtures/data/hkstore.db`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/io/example_json.json` & `cg-59.9.1/tests/fixtures/io/example_json.json`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/orderforms/1508.30.balsamic.xlsx` & `cg-59.9.1/tests/fixtures/orderforms/1508.30.balsamic.xlsx`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/orderforms/1508.30.balsamic_qc.xlsx` & `cg-59.9.1/tests/fixtures/orderforms/1508.30.balsamic_qc.xlsx`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/orderforms/1508.30.balsamic_umi.xlsx` & `cg-59.9.1/tests/fixtures/orderforms/1508.30.balsamic_umi.xlsx`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/orderforms/1508.30.fastq.xlsx` & `cg-59.9.1/tests/fixtures/orderforms/1508.30.fastq.xlsx`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/orderforms/1508.30.metagenome.xlsx` & `cg-59.9.1/tests/fixtures/orderforms/1508.30.metagenome.xlsx`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/orderforms/1508.30.mip.xlsx` & `cg-59.9.1/tests/fixtures/orderforms/1508.30.mip.xlsx`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/orderforms/1508.30.mip_rna.xlsx` & `cg-59.9.1/tests/fixtures/orderforms/1508.30.mip_rna.xlsx`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/orderforms/1508.30.rnafusion.xlsx` & `cg-59.9.1/tests/fixtures/orderforms/1508.30.rnafusion.xlsx`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/orderforms/1603.11.microbial.xlsx` & `cg-59.9.1/tests/fixtures/orderforms/1603.11.microbial.xlsx`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/orderforms/1604.17.rml.xlsx` & `cg-59.9.1/tests/fixtures/orderforms/1604.17.rml.xlsx`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/orderforms/2184.8.sarscov2.xlsx` & `cg-59.9.1/tests/fixtures/orderforms/2184.8.sarscov2.xlsx`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/orderforms/NIPT-json.json` & `cg-59.9.1/tests/fixtures/orderforms/NIPT-json.json`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/orderforms/balsamic_uploaded_json_orderform.json` & `cg-59.9.1/tests/fixtures/orderforms/balsamic_uploaded_json_orderform.json`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/orderforms/mip_uploaded_json_orderform.json` & `cg-59.9.1/tests/fixtures/orderforms/mip_uploaded_json_orderform.json`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/report/case_data.json` & `cg-59.9.1/tests/fixtures/report/case_data.json`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/report/lims_exported_samples.json` & `cg-59.9.1/tests/fixtures/report/lims_exported_samples.json`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/fixtures/report/lims_family.json` & `cg-59.9.1/tests/fixtures/report/lims_family.json`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/io/conftest.py` & `cg-59.9.1/tests/io/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/io/test_io_controller.py` & `cg-59.9.1/tests/io/test_io_controller.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/io/test_io_csv.py` & `cg-59.9.1/tests/io/test_io_csv.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/io/test_io_json.py` & `cg-59.9.1/tests/io/test_io_json.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/io/test_io_txt.py` & `cg-59.9.1/tests/io/test_io_txt.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/io/test_io_xml.py` & `cg-59.9.1/tests/io/test_io_xml.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/io/test_io_yaml.py` & `cg-59.9.1/tests/io/test_io_yaml.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/io/test_validate_path.py` & `cg-59.9.1/tests/io/test_validate_path.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/meta/archive/conftest.py` & `cg-59.9.1/tests/meta/archive/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/meta/archive/test_archive_api.py` & `cg-59.9.1/tests/meta/archive/test_archive_api.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/meta/archive/test_archive_cli.py` & `cg-59.9.1/tests/meta/archive/test_archive_cli.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/meta/archive/test_archiving.py` & `cg-59.9.1/tests/meta/archive/test_archiving.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/meta/backup/conftest.py` & `cg-59.9.1/tests/meta/backup/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/meta/backup/test_meta_backup.py` & `cg-59.9.1/tests/meta/backup/test_meta_backup.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/meta/backup/test_meta_pdc.py` & `cg-59.9.1/tests/meta/backup/test_meta_pdc.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/meta/clean/conftest.py` & `cg-59.9.1/tests/meta/clean/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/meta/clean/test_clean_flow_cells_api.py` & `cg-59.9.1/tests/meta/clean/test_clean_flow_cells_api.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/meta/clean/test_clean_retrieved_spring_files.py` & `cg-59.9.1/tests/meta/clean/test_clean_retrieved_spring_files.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/meta/compress/conftest.py` & `cg-59.9.1/tests/meta/compress/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/meta/compress/test_clean_fastq.py` & `cg-59.9.1/tests/meta/compress/test_clean_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/meta/compress/test_compress_files.py` & `cg-59.9.1/tests/meta/compress/test_compress_files.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/meta/compress/test_compress_meta_fastq.py` & `cg-59.9.1/tests/meta/compress/test_compress_meta_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/meta/compress/test_decompress_spring_meta.py` & `cg-59.9.1/tests/meta/compress/test_decompress_spring_meta.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/meta/compress/test_meta_compress_update_hk.py` & `cg-59.9.1/tests/meta/compress/test_meta_compress_update_hk.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/meta/conftest.py` & `cg-59.9.1/tests/meta/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/meta/deliver/conftest.py` & `cg-59.9.1/tests/meta/deliver/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/meta/deliver/test_deliver_ticket.py` & `cg-59.9.1/tests/meta/deliver/test_deliver_ticket.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/meta/deliver/test_delivery_api.py` & `cg-59.9.1/tests/meta/deliver/test_delivery_api.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/meta/demultiplex/conftest.py` & `cg-59.9.1/tests/meta/demultiplex/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/meta/demultiplex/test_combine_sequencing_metrics.py` & `cg-59.9.1/tests/meta/demultiplex/test_combine_sequencing_metrics.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/meta/demultiplex/test_demux_post_processing.py` & `cg-59.9.1/tests/meta/demultiplex/test_demux_post_processing.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/meta/demultiplex/test_housekeeper_storage_functions.py` & `cg-59.9.1/tests/meta/demultiplex/test_housekeeper_storage_functions.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/meta/demultiplex/test_status_db_storage_functions.py` & `cg-59.9.1/tests/meta/demultiplex/test_status_db_storage_functions.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/meta/demultiplex/test_utils.py` & `cg-59.9.1/tests/meta/demultiplex/test_utils.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/meta/demultiplex/test_validation.py` & `cg-59.9.1/tests/meta/demultiplex/test_validation.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/meta/encryption/conftest.py` & `cg-59.9.1/tests/meta/encryption/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/meta/encryption/test_encryption.py` & `cg-59.9.1/tests/meta/encryption/test_encryption.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/meta/observations/conftest.py` & `cg-59.9.1/tests/meta/observations/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/meta/observations/test_meta_upload_observations.py` & `cg-59.9.1/tests/meta/observations/test_meta_upload_observations.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/meta/orders/conftest.py` & `cg-59.9.1/tests/meta/orders/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/meta/orders/test_PoolSubmitter_validate_order.py` & `cg-59.9.1/tests/meta/orders/test_PoolSubmitter_validate_order.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/meta/orders/test_SarsCov2Submitter_order_to_status.py` & `cg-59.9.1/tests/meta/orders/test_SarsCov2Submitter_order_to_status.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/meta/orders/test_SarsCov2Submitter_store_order.py` & `cg-59.9.1/tests/meta/orders/test_SarsCov2Submitter_store_order.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/meta/orders/test_SarsCov2Submitter_validate_order.py` & `cg-59.9.1/tests/meta/orders/test_SarsCov2Submitter_validate_order.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/meta/orders/test_meta_orders_api.py` & `cg-59.9.1/tests/meta/orders/test_meta_orders_api.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/meta/orders/test_meta_orders_lims.py` & `cg-59.9.1/tests/meta/orders/test_meta_orders_lims.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/meta/orders/test_meta_orders_status.py` & `cg-59.9.1/tests/meta/orders/test_meta_orders_status.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/meta/orders/test_rnafusion_submitter.py` & `cg-59.9.1/tests/meta/orders/test_rnafusion_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/meta/orders/test_ticket_handler.py` & `cg-59.9.1/tests/meta/orders/test_ticket_handler.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/meta/qc_metrics/conftest.py` & `cg-59.9.1/tests/meta/qc_metrics/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/meta/qc_metrics/test_collect_qc_metrics.py` & `cg-59.9.1/tests/meta/qc_metrics/test_collect_qc_metrics.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/meta/report/conftest.py` & `cg-59.9.1/tests/meta/report/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/meta/report/test_balsamic_api.py` & `cg-59.9.1/tests/meta/report/test_balsamic_api.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/meta/report/test_field_validators.py` & `cg-59.9.1/tests/meta/report/test_field_validators.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/meta/report/test_mip_dna_api.py` & `cg-59.9.1/tests/meta/report/test_mip_dna_api.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/meta/report/test_report_api.py` & `cg-59.9.1/tests/meta/report/test_report_api.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/meta/report/test_rnafusion_api.py` & `cg-59.9.1/tests/meta/report/test_rnafusion_api.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/meta/rsync/conftest.py` & `cg-59.9.1/tests/meta/rsync/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/meta/rsync/test_rsync.py` & `cg-59.9.1/tests/meta/rsync/test_rsync.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/meta/test_invoice.py` & `cg-59.9.1/tests/meta/test_invoice.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/meta/transfer/conftest.py` & `cg-59.9.1/tests/meta/transfer/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/meta/transfer/test_external_data.py` & `cg-59.9.1/tests/meta/transfer/test_external_data.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/meta/transfer/test_meta_transfer_lims.py` & `cg-59.9.1/tests/meta/transfer/test_meta_transfer_lims.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/meta/upload/balsamic/test_balsamic.py` & `cg-59.9.1/tests/meta/upload/balsamic/test_balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/meta/upload/conftest.py` & `cg-59.9.1/tests/meta/upload/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/meta/upload/gisaid/fixtures/four_samples.csv` & `cg-59.9.1/tests/meta/upload/gisaid/fixtures/four_samples.csv`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/meta/upload/mutacc/conftest.py` & `cg-59.9.1/tests/meta/upload/mutacc/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/meta/upload/mutacc/test_meta_upload_mutacc.py` & `cg-59.9.1/tests/meta/upload/mutacc/test_meta_upload_mutacc.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/meta/upload/nipt/conftest.py` & `cg-59.9.1/tests/meta/upload/nipt/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/meta/upload/nipt/test_models.py` & `cg-59.9.1/tests/meta/upload/nipt/test_models.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/meta/upload/nipt/test_nipt_upload_api.py` & `cg-59.9.1/tests/meta/upload/nipt/test_nipt_upload_api.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/meta/upload/scout/conftest.py` & `cg-59.9.1/tests/meta/upload/scout/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/meta/upload/scout/test_generate_load_config.py` & `cg-59.9.1/tests/meta/upload/scout/test_generate_load_config.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/meta/upload/scout/test_meta_upload_scoutapi.py` & `cg-59.9.1/tests/meta/upload/scout/test_meta_upload_scoutapi.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/meta/upload/scout/test_meta_upload_scoutapi_rna.py` & `cg-59.9.1/tests/meta/upload/scout/test_meta_upload_scoutapi_rna.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/meta/upload/scout/test_scout_config_builder.py` & `cg-59.9.1/tests/meta/upload/scout/test_scout_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/meta/upload/test_meta_upload_coverage.py` & `cg-59.9.1/tests/meta/upload/test_meta_upload_coverage.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/meta/upload/test_upload_api.py` & `cg-59.9.1/tests/meta/upload/test_upload_api.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/meta/upload/test_upload_genotypes_api.py` & `cg-59.9.1/tests/meta/upload/test_upload_genotypes_api.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/meta/workflow/conftest.py` & `cg-59.9.1/tests/meta/workflow/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/meta/workflow/microsalt/conftest.py` & `cg-59.9.1/tests/meta/workflow/microsalt/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/meta/workflow/microsalt/test_quality_controller.py` & `cg-59.9.1/tests/meta/workflow/microsalt/test_quality_controller.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/meta/workflow/microsalt/test_quality_controller_utils.py` & `cg-59.9.1/tests/meta/workflow/microsalt/test_quality_controller_utils.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/meta/workflow/microsalt/test_report_generation.py` & `cg-59.9.1/tests/meta/workflow/microsalt/test_report_generation.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/meta/workflow/test_analysis.py` & `cg-59.9.1/tests/meta/workflow/test_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/meta/workflow/test_balsamic.py` & `cg-59.9.1/tests/meta/workflow/test_balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/meta/workflow/test_fastq.py` & `cg-59.9.1/tests/meta/workflow/test_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/meta/workflow/test_microsalt.py` & `cg-59.9.1/tests/meta/workflow/test_microsalt.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/meta/workflow/test_nf_analysis.py` & `cg-59.9.1/tests/meta/workflow/test_nf_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/meta/workflow/test_prepare_fastq_api.py` & `cg-59.9.1/tests/meta/workflow/test_prepare_fastq_api.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/meta/workflow/test_rnafusion.py` & `cg-59.9.1/tests/meta/workflow/test_rnafusion.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/mocks/balsamic_analysis_mock.py` & `cg-59.9.1/tests/mocks/balsamic_analysis_mock.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/mocks/crunchy.py` & `cg-59.9.1/tests/mocks/crunchy.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/mocks/hk_mock.py` & `cg-59.9.1/tests/mocks/hk_mock.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/mocks/limsmock.py` & `cg-59.9.1/tests/mocks/limsmock.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/mocks/madeline.py` & `cg-59.9.1/tests/mocks/madeline.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/mocks/mip_analysis_mock.py` & `cg-59.9.1/tests/mocks/mip_analysis_mock.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/mocks/osticket.py` & `cg-59.9.1/tests/mocks/osticket.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/mocks/process_mock.py` & `cg-59.9.1/tests/mocks/process_mock.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/mocks/report.py` & `cg-59.9.1/tests/mocks/report.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/mocks/scout.py` & `cg-59.9.1/tests/mocks/scout.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/mocks/store_model.py` & `cg-59.9.1/tests/mocks/store_model.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/mocks/tb_mock.py` & `cg-59.9.1/tests/mocks/tb_mock.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/models/balsamic/conftest.py` & `cg-59.9.1/tests/models/balsamic/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/models/balsamic/test_balsamic_analysis.py` & `cg-59.9.1/tests/models/balsamic/test_balsamic_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/models/conftest.py` & `cg-59.9.1/tests/models/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/models/demultiplexing/test_run_parameters.py` & `cg-59.9.1/tests/models/demultiplexing/test_run_parameters.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/models/downsample/test_down_sample_meta_data.py` & `cg-59.9.1/tests/models/downsample/test_down_sample_meta_data.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/models/flow_cell/test_flowcell_model.py` & `cg-59.9.1/tests/models/flow_cell/test_flowcell_model.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/models/mip/conftest.py` & `cg-59.9.1/tests/models/mip/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/models/mip/test_mip_analysis.py` & `cg-59.9.1/tests/models/mip/test_mip_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/models/mip/test_mip_config.py` & `cg-59.9.1/tests/models/mip/test_mip_config.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/models/mip/test_mip_metrics_deliverables.py` & `cg-59.9.1/tests/models/mip/test_mip_metrics_deliverables.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/models/mip/test_mip_sample_info.py` & `cg-59.9.1/tests/models/mip/test_mip_sample_info.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/models/nextflow/test_nextflow_deliver.py` & `cg-59.9.1/tests/models/nextflow/test_nextflow_deliver.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/models/observations/conftest.py` & `cg-59.9.1/tests/models/observations/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/models/observations/test_observations_input_files.py` & `cg-59.9.1/tests/models/observations/test_observations_input_files.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/models/report/test_validators.py` & `cg-59.9.1/tests/models/report/test_validators.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/models/rnafusion/test_rnafusion_sample.py` & `cg-59.9.1/tests/models/rnafusion/test_rnafusion_sample.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/models/test_cg_models.py` & `cg-59.9.1/tests/models/test_cg_models.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/models/test_compression_data.py` & `cg-59.9.1/tests/models/test_compression_data.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/models/test_fastq.py` & `cg-59.9.1/tests/models/test_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/models/test_file_data.py` & `cg-59.9.1/tests/models/test_file_data.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/server/conftest.py` & `cg-59.9.1/tests/server/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/server/endpoints/test_orders_endpoint.py` & `cg-59.9.1/tests/server/endpoints/test_orders_endpoint.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,21 +30,23 @@
     client: FlaskClient,
     order: Order,
     order_another: Order,
     order_balsamic: Order,
     limit: int | None,
     workflow: str,
     expected_orders: int,
+    analysis_summary,
 ):
     """Tests that orders are returned from the orders endpoint"""
     # GIVEN a store with three orders, two of which are MIP-DNA and the last is BALSAMIC
 
     # WHEN a request is made to get all orders
     endpoint: str = "/api/v1/orders"
-    response = client.get(endpoint, query_string={"pageSize": limit, "workflow": workflow})
+    with mock.patch.object(TrailblazerAPI, "get_summaries", return_value=[]):
+        response = client.get(endpoint, query_string={"pageSize": limit, "workflow": workflow})
 
     # THEN the response should be successful
     assert response.status_code == HTTPStatus.OK
 
     # THEN the response contains the correct number of orders
     assert len(response.json["orders"]) == expected_orders
```

### Comparing `cg-59.9.0/tests/services/fastq_file_service/conftest.py` & `cg-59.9.1/tests/services/fastq_file_service/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/services/fastq_file_service/test_fastq_file_service.py` & `cg-59.9.1/tests/services/fastq_file_service/test_fastq_file_service.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/services/orders/order_status_service/conftest.py` & `cg-59.9.1/tests/services/orders/order_status_service/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/services/orders/order_status_service/test_order_status_service.py` & `cg-59.9.1/tests/services/orders/order_status_service/test_order_status_service.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/store/api/conftest.py` & `cg-59.9.1/tests/store/api/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/store/api/test_base.py` & `cg-59.9.1/tests/store/api/test_base.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/store/conftest.py` & `cg-59.9.1/tests/store/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/store/crud/add/test_store_add_application_version.py` & `cg-59.9.1/tests/store/crud/add/test_store_add_application_version.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/store/crud/add/test_store_add_base.py` & `cg-59.9.1/tests/store/crud/add/test_store_add_base.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/store/crud/add/test_store_add_customer.py` & `cg-59.9.1/tests/store/crud/add/test_store_add_customer.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/store/crud/add/test_store_add_flow_celll.py` & `cg-59.9.1/tests/store/crud/add/test_store_add_flow_celll.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/store/crud/conftest.py` & `cg-59.9.1/tests/store/crud/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/store/crud/delete/test_delete.py` & `cg-59.9.1/tests/store/crud/delete/test_delete.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/store/crud/read/test_read.py` & `cg-59.9.1/tests/store/crud/read/test_read.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/store/crud/read/test_read_analyses_to_clean.py` & `cg-59.9.1/tests/store/crud/read/test_read_analyses_to_clean.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/store/crud/read/test_read_analyses_to_delivery_report.py` & `cg-59.9.1/tests/store/crud/read/test_read_analyses_to_delivery_report.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/store/crud/read/test_read_analysis.py` & `cg-59.9.1/tests/store/crud/read/test_read_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/store/crud/read/test_read_application_version.py` & `cg-59.9.1/tests/store/crud/read/test_read_application_version.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/store/crud/read/test_read_case.py` & `cg-59.9.1/tests/store/crud/read/test_read_case.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/store/crud/read/test_read_customer.py` & `cg-59.9.1/tests/store/crud/read/test_read_customer.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/store/crud/read/test_read_pool.py` & `cg-59.9.1/tests/store/crud/read/test_read_pool.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/store/crud/read/test_read_sample.py` & `cg-59.9.1/tests/store/crud/read/test_read_sample.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/store/crud/update/test_update.py` & `cg-59.9.1/tests/store/crud/update/test_update.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/store/filters/test_status_analyses_filters.py` & `cg-59.9.1/tests/store/filters/test_status_analyses_filters.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/store/filters/test_status_application_filters.py` & `cg-59.9.1/tests/store/filters/test_status_application_filters.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/store/filters/test_status_application_limitations_filters.py` & `cg-59.9.1/tests/store/filters/test_status_application_limitations_filters.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/store/filters/test_status_application_version_filters.py` & `cg-59.9.1/tests/store/filters/test_status_application_version_filters.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/store/filters/test_status_bed_filters.py` & `cg-59.9.1/tests/store/filters/test_status_bed_filters.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/store/filters/test_status_bed_version_filters.py` & `cg-59.9.1/tests/store/filters/test_status_bed_version_filters.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/store/filters/test_status_case_sample_filters.py` & `cg-59.9.1/tests/store/filters/test_status_case_sample_filters.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/store/filters/test_status_cases_filters.py` & `cg-59.9.1/tests/store/filters/test_status_cases_filters.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/store/filters/test_status_collaboration_filters.py` & `cg-59.9.1/tests/store/filters/test_status_collaboration_filters.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/store/filters/test_status_customer_filters.py` & `cg-59.9.1/tests/store/filters/test_status_customer_filters.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/store/filters/test_status_flow_cell_filters.py` & `cg-59.9.1/tests/store/filters/test_status_flow_cell_filters.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/store/filters/test_status_invoice_filters.py` & `cg-59.9.1/tests/store/filters/test_status_invoice_filters.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/store/filters/test_status_metrics_filters.py` & `cg-59.9.1/tests/store/filters/test_status_metrics_filters.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/store/filters/test_status_organism_filters.py` & `cg-59.9.1/tests/store/filters/test_status_organism_filters.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/store/filters/test_status_panel_filters.py` & `cg-59.9.1/tests/store/filters/test_status_panel_filters.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/store/filters/test_status_pool_filters.py` & `cg-59.9.1/tests/store/filters/test_status_pool_filters.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/store/filters/test_status_samples_filters.py` & `cg-59.9.1/tests/store/filters/test_status_samples_filters.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/store/filters/test_status_user_filters.py` & `cg-59.9.1/tests/store/filters/test_status_user_filters.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/store/test_delivery.py` & `cg-59.9.1/tests/store/test_delivery.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/store/test_store_models.py` & `cg-59.9.1/tests/store/test_store_models.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/store_helpers.py` & `cg-59.9.1/tests/store_helpers.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/test_copy_novaseqx_flow_cell.py` & `cg-59.9.1/tests/test_copy_novaseqx_flow_cell.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/test_store_helpers.py` & `cg-59.9.1/tests/test_store_helpers.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/utils/conftest.py` & `cg-59.9.1/tests/utils/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/utils/test_commands.py` & `cg-59.9.1/tests/utils/test_commands.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/utils/test_date.py` & `cg-59.9.1/tests/utils/test_date.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/utils/test_dict.py` & `cg-59.9.1/tests/utils/test_dict.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/utils/test_dispatcher.py` & `cg-59.9.1/tests/utils/test_dispatcher.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/utils/test_files.py` & `cg-59.9.1/tests/utils/test_files.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/utils/test_time.py` & `cg-59.9.1/tests/utils/test_time.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/tests/utils/test_utils.py` & `cg-59.9.1/tests/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `cg-59.9.0/PKG-INFO` & `cg-59.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cg
-Version: 59.9.0
+Version: 59.9.1
 Summary: Clinical Genomics command center
 Home-page: https://github.com/Clinical-Genomics/cg
 Author: Clinical Genomics
 Author-email: support@clinicalgenomics.se
 Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

