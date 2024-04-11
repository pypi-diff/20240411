# Comparing `tmp/BioSAK-1.83.1.tar.gz` & `tmp/BioSAK-1.83.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BioSAK-1.83.1.tar", last modified: Tue Apr  9 11:41:54 2024, max compression
+gzip compressed data, was "BioSAK-1.83.2.tar", last modified: Thu Apr 11 13:05:26 2024, max compression
```

## Comparing `BioSAK-1.83.1.tar` & `BioSAK-1.83.2.tar`

### file list

```diff
@@ -1,161 +1,161 @@
-drwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2024-04-09 11:41:54.153462 BioSAK-1.83.1/
-drwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2024-04-09 11:41:54.150986 BioSAK-1.83.1/BioSAK/
--rw-r--r--   0 songweizhi   (501) staff       (20)     3653 2024-01-16 05:10:59.000000 BioSAK-1.83.1/BioSAK/BLCA_op_parser.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2031 2023-05-31 05:26:00.000000 BioSAK-1.83.1/BioSAK/BioSAK_config.py
--rwxr-xr-x   0 songweizhi   (501) staff       (20)    39300 2024-03-22 00:45:31.000000 BioSAK-1.83.1/BioSAK/COG2020.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3615 2023-05-09 01:09:35.000000 BioSAK-1.83.1/BioSAK/COG_boxplot_last1row.R
--rw-r--r--   0 songweizhi   (501) staff       (20)     6974 2023-05-09 01:09:35.000000 BioSAK-1.83.1/BioSAK/COG_boxplot_last2row.R
--rwxr-xr-x   0 songweizhi   (501) staff       (20)     6067 2024-01-16 05:00:13.000000 BioSAK-1.83.1/BioSAK/CheckM.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     5891 2024-01-16 05:10:59.000000 BioSAK-1.83.1/BioSAK/ConvertMSA.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    16671 2023-05-09 01:09:35.000000 BioSAK-1.83.1/BioSAK/DnaFeaturesViewer.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2292 2023-05-09 01:09:35.000000 BioSAK-1.83.1/BioSAK/FastaSplitler_by_num.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2485 2023-05-09 01:09:35.000000 BioSAK-1.83.1/BioSAK/FastaSplitler_by_size.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2190 2023-05-09 01:09:35.000000 BioSAK-1.83.1/BioSAK/GTDB_for_BLCA.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1321 2023-05-09 01:09:35.000000 BioSAK-1.83.1/BioSAK/Gene2Ctg.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    45147 2024-03-23 14:54:03.000000 BioSAK-1.83.1/BioSAK/KEGG.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3484 2023-05-09 01:09:35.000000 BioSAK-1.83.1/BioSAK/KEGG_boxplot_last1row.R
--rw-r--r--   0 songweizhi   (501) staff       (20)      269 2023-05-09 01:09:35.000000 BioSAK-1.83.1/BioSAK/KEGG_get_eukaryotic_kos.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3077 2023-08-22 09:31:28.000000 BioSAK-1.83.1/BioSAK/KeepRemovingTmp.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2620 2024-01-16 05:10:59.000000 BioSAK-1.83.1/BioSAK/MeanMappingDepth.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3682 2024-01-16 12:39:58.000000 BioSAK-1.83.1/BioSAK/MetaBiosample.py
--rw-r--r--   0 songweizhi   (501) staff       (20)  3297822 2023-05-09 01:09:35.000000 BioSAK-1.83.1/BioSAK/MetaCHIP_phylo.hmm
--rw-r--r--   0 songweizhi   (501) staff       (20)  1206805 2023-05-09 01:09:35.000000 BioSAK-1.83.1/BioSAK/MetaCyc_reactions_with_ec.txt
--rw-r--r--   0 songweizhi   (501) staff       (20)    16960 2023-05-09 01:09:35.000000 BioSAK-1.83.1/BioSAK/NetEnzymes.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3713 2023-05-09 01:09:35.000000 BioSAK-1.83.1/BioSAK/Newick_tree_plotter.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1659 2024-01-16 05:10:59.000000 BioSAK-1.83.1/BioSAK/OneLineAln.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    10448 2023-05-09 01:09:35.000000 BioSAK-1.83.1/BioSAK/Prodigal.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     6048 2023-05-09 01:09:35.000000 BioSAK-1.83.1/BioSAK/Reads_simulator.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3573 2024-01-16 05:10:59.000000 BioSAK-1.83.1/BioSAK/RunGraphMB.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3833 2024-01-16 05:10:59.000000 BioSAK-1.83.1/BioSAK/SILVA_for_BLCA.py
--rwxr-xr-x   0 songweizhi   (501) staff       (20)     6255 2023-05-09 01:09:35.000000 BioSAK-1.83.1/BioSAK/SankeyTaxon.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     5678 2024-01-16 05:10:59.000000 BioSAK-1.83.1/BioSAK/SliceMSA.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3173 2024-01-16 05:10:59.000000 BioSAK-1.83.1/BioSAK/SubsampleLongReads.py
--rwxr-xr-x   0 songweizhi   (501) staff       (20)     1696 2024-01-16 05:10:59.000000 BioSAK-1.83.1/BioSAK/Tax4Fun2IndOTU.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3499 2024-04-09 11:41:51.000000 BioSAK-1.83.1/BioSAK/VERSION
--rw-r--r--   0 songweizhi   (501) staff       (20)      467 2023-05-09 01:09:35.000000 BioSAK-1.83.1/BioSAK/VisBlastOp.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     9944 2023-05-09 01:09:35.000000 BioSAK-1.83.1/BioSAK/VisGeneFlk.py
--rwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2023-05-09 01:09:35.000000 BioSAK-1.83.1/BioSAK/__init__.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2526 2024-03-25 14:00:14.000000 BioSAK-1.83.1/BioSAK/add_desc.py
--rwxr-xr-x   0 songweizhi   (501) staff       (20)    38577 2024-03-22 00:45:31.000000 BioSAK-1.83.1/BioSAK/arCOG.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     6985 2024-01-16 05:00:13.000000 BioSAK-1.83.1/BioSAK/bam2reads.py
--rwxr-xr-x   0 songweizhi   (501) staff       (20)     2630 2024-03-22 13:23:45.000000 BioSAK-1.83.1/BioSAK/boxplot.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3312 2023-05-09 01:09:35.000000 BioSAK-1.83.1/BioSAK/boxplot_last1row.R
--rw-r--r--   0 songweizhi   (501) staff       (20)     6104 2023-05-09 01:09:35.000000 BioSAK-1.83.1/BioSAK/boxplot_matrix_COG.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     5403 2023-05-09 01:09:35.000000 BioSAK-1.83.1/BioSAK/boxplot_matrix_COG_backup.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     6984 2023-05-09 01:09:35.000000 BioSAK-1.83.1/BioSAK/boxplot_matrix_KEGG.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     5747 2023-05-09 01:09:35.000000 BioSAK-1.83.1/BioSAK/boxplot_matrix_dbCAN.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1695 2023-05-09 01:09:35.000000 BioSAK-1.83.1/BioSAK/cat_fa.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    13440 2023-05-09 01:09:35.000000 BioSAK-1.83.1/BioSAK/cdd2cog.pl
--rw-r--r--   0 songweizhi   (501) staff       (20)     1186 2023-05-09 01:09:35.000000 BioSAK-1.83.1/BioSAK/checkm_marker.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1076 2023-05-09 01:09:35.000000 BioSAK-1.83.1/BioSAK/compare_trees.R
--rw-r--r--   0 songweizhi   (501) staff       (20)     9745 2024-01-16 05:10:59.000000 BioSAK-1.83.1/BioSAK/compare_trees.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     6592 2023-05-09 01:09:35.000000 BioSAK-1.83.1/BioSAK/cross_link_seqs.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    24033 2024-03-22 00:45:31.000000 BioSAK-1.83.1/BioSAK/dbCAN.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1936 2023-05-09 01:09:35.000000 BioSAK-1.83.1/BioSAK/download_GenBank_genome_subset_prokaryotes_csv.py
--rw-r--r--   0 songweizhi   (501) staff       (20)      767 2023-05-09 01:09:35.000000 BioSAK-1.83.1/BioSAK/dwnld_sra_reads.py
--rwxr-xr-x   0 songweizhi   (501) staff       (20)    13250 2024-03-22 08:01:22.000000 BioSAK-1.83.1/BioSAK/enrich.py
--rw-r--r--   0 songweizhi   (501) staff       (20)      929 2023-05-09 01:09:35.000000 BioSAK-1.83.1/BioSAK/exe_cmds.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1508 2023-12-05 01:06:39.000000 BioSAK-1.83.1/BioSAK/ezaai2mat.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1396 2023-12-05 01:02:55.000000 BioSAK-1.83.1/BioSAK/fa2id.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1195 2023-05-17 06:14:50.000000 BioSAK-1.83.1/BioSAK/fa2phy.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1363 2023-05-09 01:09:35.000000 BioSAK-1.83.1/BioSAK/fa2tree.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     6280 2023-05-09 01:09:35.000000 BioSAK-1.83.1/BioSAK/format_converter.py
--rwxr-xr-x   0 songweizhi   (501) staff       (20)     2861 2023-05-09 01:09:35.000000 BioSAK-1.83.1/BioSAK/format_leaf_name.py
--rw-r--r--   0 songweizhi   (501) staff       (20)      639 2023-05-09 01:09:35.000000 BioSAK-1.83.1/BioSAK/fq2fa.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3190 2024-04-09 11:41:51.000000 BioSAK-1.83.1/BioSAK/gapseq.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2846 2023-06-14 10:08:30.000000 BioSAK-1.83.1/BioSAK/gbk2faa.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3342 2023-06-14 10:14:13.000000 BioSAK-1.83.1/BioSAK/gbk2ffn.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2528 2023-05-09 01:09:35.000000 BioSAK-1.83.1/BioSAK/gbk2fna.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3726 2023-05-09 01:09:35.000000 BioSAK-1.83.1/BioSAK/gbk_to_ffn_faa.py
--rw-r--r--   0 songweizhi   (501) staff       (20)      813 2023-05-09 01:09:35.000000 BioSAK-1.83.1/BioSAK/get_EC_from_ko_stats_D.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     7477 2023-05-09 01:09:35.000000 BioSAK-1.83.1/BioSAK/get_GTDB_taxon_gnm.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     5428 2023-06-15 03:03:02.000000 BioSAK-1.83.1/BioSAK/get_MAG_reads_long.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3991 2023-05-09 01:09:35.000000 BioSAK-1.83.1/BioSAK/get_Pfam_hmms.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    29246 2023-05-09 01:09:35.000000 BioSAK-1.83.1/BioSAK/get_SCG_tree.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1784 2023-05-09 01:09:35.000000 BioSAK-1.83.1/BioSAK/get_TopHits_taxonomy.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2247 2023-05-09 01:09:35.000000 BioSAK-1.83.1/BioSAK/get_aa_composition.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    12066 2023-05-09 01:09:35.000000 BioSAK-1.83.1/BioSAK/get_bin_abundance copy.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2139 2024-01-23 11:57:14.000000 BioSAK-1.83.1/BioSAK/get_data_matrix.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1339 2023-05-09 01:09:35.000000 BioSAK-1.83.1/BioSAK/get_gc.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     5523 2023-05-09 01:09:35.000000 BioSAK-1.83.1/BioSAK/get_gene_depth.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3591 2024-01-16 05:10:59.000000 BioSAK-1.83.1/BioSAK/get_genome_GTDB.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     6070 2024-01-16 04:57:23.000000 BioSAK-1.83.1/BioSAK/get_genome_NCBI.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    11209 2023-05-09 01:09:35.000000 BioSAK-1.83.1/BioSAK/get_genome_NCBI_v1.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    12620 2023-05-09 01:09:35.000000 BioSAK-1.83.1/BioSAK/get_genome_NCBI_v2.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3048 2023-05-09 01:09:35.000000 BioSAK-1.83.1/BioSAK/get_gnm_size.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     4834 2023-05-09 01:09:35.000000 BioSAK-1.83.1/BioSAK/get_ko_gene_seqs.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1192 2023-09-21 08:44:42.000000 BioSAK-1.83.1/BioSAK/get_krona_plot.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1559 2023-05-09 01:09:35.000000 BioSAK-1.83.1/BioSAK/get_reads_from_sam.py
--rw-r--r--   0 songweizhi   (501) staff       (20)      792 2023-05-09 01:09:35.000000 BioSAK-1.83.1/BioSAK/get_reads_id_in_sam.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2386 2023-05-09 01:09:35.000000 BioSAK-1.83.1/BioSAK/get_sankey_plot.R
--rw-r--r--   0 songweizhi   (501) staff       (20)     4242 2023-05-09 01:09:35.000000 BioSAK-1.83.1/BioSAK/get_top_hit.py
--rw-r--r--   0 songweizhi   (501) staff       (20)      820 2023-05-09 01:09:35.000000 BioSAK-1.83.1/BioSAK/get_total_length.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     4643 2023-05-18 01:37:58.000000 BioSAK-1.83.1/BioSAK/global_functions.py
--rwxr-xr-x   0 songweizhi   (501) staff       (20)     2910 2024-03-11 00:57:02.000000 BioSAK-1.83.1/BioSAK/hpc3.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    26258 2024-03-23 15:17:20.000000 BioSAK-1.83.1/BioSAK/iTOL.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3337 2024-03-07 03:01:35.000000 BioSAK-1.83.1/BioSAK/js_cmds.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3281 2024-04-08 09:48:49.000000 BioSAK-1.83.1/BioSAK/js_hpc3.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1643 2023-05-09 01:09:35.000000 BioSAK-1.83.1/BioSAK/keep_best_hit.py
--rw-r--r--   0 songweizhi   (501) staff       (20)  3361029 2023-05-09 01:09:35.000000 BioSAK-1.83.1/BioSAK/ko00001.keg
--rw-r--r--   0 songweizhi   (501) staff       (20)     1848 2024-03-10 15:18:30.000000 BioSAK-1.83.1/BioSAK/koala.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2772 2023-05-09 01:09:35.000000 BioSAK-1.83.1/BioSAK/label_tree.R
--rw-r--r--   0 songweizhi   (501) staff       (20)     4788 2024-01-16 05:10:59.000000 BioSAK-1.83.1/BioSAK/label_tree.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    35857 2023-05-09 01:09:35.000000 BioSAK-1.83.1/BioSAK/link_16S_MAG.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    12349 2023-05-09 01:09:35.000000 BioSAK-1.83.1/BioSAK/magabund.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    19855 2023-05-09 01:09:35.000000 BioSAK-1.83.1/BioSAK/magabund2.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1224 2023-05-09 01:09:35.000000 BioSAK-1.83.1/BioSAK/manipulator_fasta.py
--rw-r--r--   0 songweizhi   (501) staff       (20)        0 2023-05-09 01:09:35.000000 BioSAK-1.83.1/BioSAK/manipulator_msa.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3659 2023-05-09 01:09:35.000000 BioSAK-1.83.1/BioSAK/manipulator_newick.py
--rw-r--r--   0 songweizhi   (501) staff       (20)        0 2023-05-09 01:09:35.000000 BioSAK-1.83.1/BioSAK/manipulator_sam.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2433 2023-05-30 01:59:44.000000 BioSAK-1.83.1/BioSAK/mean_MAG_cov.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1880 2024-03-25 06:45:20.000000 BioSAK-1.83.1/BioSAK/merge_df.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2405 2024-01-16 05:10:59.000000 BioSAK-1.83.1/BioSAK/merge_seq.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     6742 2024-01-23 07:37:01.000000 BioSAK-1.83.1/BioSAK/metaAssembly.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1327 2023-06-11 13:56:21.000000 BioSAK-1.83.1/BioSAK/metabat2concoct.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1612 2023-06-11 16:00:51.000000 BioSAK-1.83.1/BioSAK/metabat2maxbin.py
--rw-r--r--   0 songweizhi   (501) staff       (20)        0 2023-05-09 01:09:35.000000 BioSAK-1.83.1/BioSAK/msa_to_distance_matrix.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1759 2023-05-09 01:09:35.000000 BioSAK-1.83.1/BioSAK/ncbi_dataset.py
--rw-r--r--   0 songweizhi   (501) staff       (20)        0 2024-03-03 11:00:02.000000 BioSAK-1.83.1/BioSAK/odp.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2820 2023-05-09 01:09:35.000000 BioSAK-1.83.1/BioSAK/parse_MetaCyc_RxnDB.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1460 2023-09-18 14:42:31.000000 BioSAK-1.83.1/BioSAK/parse_mmseqs_tsv.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     8633 2024-01-16 05:10:59.000000 BioSAK-1.83.1/BioSAK/plot_mag.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     7332 2023-05-09 01:09:35.000000 BioSAK-1.83.1/BioSAK/plot_sam_depth.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1638 2023-05-09 01:09:35.000000 BioSAK-1.83.1/BioSAK/plot_tree.R
--rw-r--r--   0 songweizhi   (501) staff       (20)     2256 2023-07-22 00:36:16.000000 BioSAK-1.83.1/BioSAK/prefix_file.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     4221 2024-01-16 05:10:59.000000 BioSAK-1.83.1/BioSAK/prokka.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     5057 2023-08-03 02:58:56.000000 BioSAK-1.83.1/BioSAK/reads2bam.py
--rwxr-xr-x   0 songweizhi   (501) staff       (20)     2534 2023-05-09 01:09:35.000000 BioSAK-1.83.1/BioSAK/rename_leaves.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2005 2023-05-09 01:09:35.000000 BioSAK-1.83.1/BioSAK/rename_reads_for_Reago.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     6801 2023-10-26 11:55:44.000000 BioSAK-1.83.1/BioSAK/rename_seq.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2210 2024-01-16 05:10:59.000000 BioSAK-1.83.1/BioSAK/rename_seqs.py
--rw-r--r--   0 songweizhi   (501) staff       (20)      144 2024-03-03 10:34:33.000000 BioSAK-1.83.1/BioSAK/ribbon.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1996 2023-05-09 01:09:35.000000 BioSAK-1.83.1/BioSAK/sam2bam.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     6877 2023-05-13 11:01:19.000000 BioSAK-1.83.1/BioSAK/sampling_GTDB_gnms.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3603 2024-01-16 05:10:59.000000 BioSAK-1.83.1/BioSAK/select_seq.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3167 2023-05-09 01:09:35.000000 BioSAK-1.83.1/BioSAK/sep_reads_by_barcode.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2671 2024-01-16 05:10:59.000000 BioSAK-1.83.1/BioSAK/slice_seq.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3788 2023-05-09 01:09:35.000000 BioSAK-1.83.1/BioSAK/split_fasta.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1998 2024-01-16 05:10:59.000000 BioSAK-1.83.1/BioSAK/split_folder.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     4561 2023-05-09 01:09:35.000000 BioSAK-1.83.1/BioSAK/split_sam.py
--rwxr-xr-x   0 songweizhi   (501) staff       (20)     1204 2024-01-16 05:10:59.000000 BioSAK-1.83.1/BioSAK/submitHPC.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2011 2024-01-16 05:10:59.000000 BioSAK-1.83.1/BioSAK/subset_GTDB_meta.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     4585 2024-04-09 03:15:33.000000 BioSAK-1.83.1/BioSAK/subset_df.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     7296 2024-01-16 05:10:59.000000 BioSAK-1.83.1/BioSAK/subset_tree.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     7844 2024-01-16 05:10:59.000000 BioSAK-1.83.1/BioSAK/top_16S_hits.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2106 2023-05-09 01:09:35.000000 BioSAK-1.83.1/BioSAK/top_hits_in_a_group.py
--rw-r--r--   0 songweizhi   (501) staff       (20)      831 2024-04-09 06:05:51.000000 BioSAK-1.83.1/BioSAK/transpose.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2252 2024-01-16 05:10:59.000000 BioSAK-1.83.1/BioSAK/usearch_uc.py
-drwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2024-04-09 11:41:54.152892 BioSAK-1.83.1/BioSAK.egg-info/
--rw-r--r--   0 songweizhi   (501) staff       (20)      508 2024-04-09 11:41:54.000000 BioSAK-1.83.1/BioSAK.egg-info/PKG-INFO
--rw-r--r--   0 songweizhi   (501) staff       (20)     3630 2024-04-09 11:41:54.000000 BioSAK-1.83.1/BioSAK.egg-info/SOURCES.txt
--rw-r--r--   0 songweizhi   (501) staff       (20)        1 2024-04-09 11:41:54.000000 BioSAK-1.83.1/BioSAK.egg-info/dependency_links.txt
--rw-r--r--   0 songweizhi   (501) staff       (20)       95 2024-04-09 11:41:54.000000 BioSAK-1.83.1/BioSAK.egg-info/requires.txt
--rw-r--r--   0 songweizhi   (501) staff       (20)        7 2024-04-09 11:41:54.000000 BioSAK-1.83.1/BioSAK.egg-info/top_level.txt
--rw-r--r--   0 songweizhi   (501) staff       (20)    35141 2023-05-09 01:09:36.000000 BioSAK-1.83.1/LICENSE
--rwxr-xr-x   0 songweizhi   (501) staff       (20)      300 2023-05-09 01:09:36.000000 BioSAK-1.83.1/MANIFEST.in
--rw-r--r--   0 songweizhi   (501) staff       (20)      508 2024-04-09 11:41:54.153193 BioSAK-1.83.1/PKG-INFO
--rw-r--r--   0 songweizhi   (501) staff       (20)     1533 2024-01-23 07:37:01.000000 BioSAK-1.83.1/README.md
-drwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2024-04-09 11:41:54.152065 BioSAK-1.83.1/bin/
--rwxr-xr-x   0 songweizhi   (501) staff       (20)    72931 2024-04-09 06:05:51.000000 BioSAK-1.83.1/bin/BioSAK
--rw-r--r--   0 songweizhi   (501) staff       (20)       38 2024-04-09 11:41:54.153530 BioSAK-1.83.1/setup.cfg
--rw-r--r--   0 songweizhi   (501) staff       (20)      915 2024-01-15 11:41:11.000000 BioSAK-1.83.1/setup.py
+drwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2024-04-11 13:05:26.862743 BioSAK-1.83.2/
+drwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2024-04-11 13:05:26.860031 BioSAK-1.83.2/BioSAK/
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3653 2024-01-16 05:10:59.000000 BioSAK-1.83.2/BioSAK/BLCA_op_parser.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2031 2023-05-31 05:26:00.000000 BioSAK-1.83.2/BioSAK/BioSAK_config.py
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)    39300 2024-03-22 00:45:31.000000 BioSAK-1.83.2/BioSAK/COG2020.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3615 2023-05-09 01:09:35.000000 BioSAK-1.83.2/BioSAK/COG_boxplot_last1row.R
+-rw-r--r--   0 songweizhi   (501) staff       (20)     6974 2023-05-09 01:09:35.000000 BioSAK-1.83.2/BioSAK/COG_boxplot_last2row.R
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)     6067 2024-01-16 05:00:13.000000 BioSAK-1.83.2/BioSAK/CheckM.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     5891 2024-01-16 05:10:59.000000 BioSAK-1.83.2/BioSAK/ConvertMSA.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    16671 2023-05-09 01:09:35.000000 BioSAK-1.83.2/BioSAK/DnaFeaturesViewer.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2292 2023-05-09 01:09:35.000000 BioSAK-1.83.2/BioSAK/FastaSplitler_by_num.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2485 2023-05-09 01:09:35.000000 BioSAK-1.83.2/BioSAK/FastaSplitler_by_size.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2190 2023-05-09 01:09:35.000000 BioSAK-1.83.2/BioSAK/GTDB_for_BLCA.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1321 2023-05-09 01:09:35.000000 BioSAK-1.83.2/BioSAK/Gene2Ctg.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    45147 2024-03-23 14:54:03.000000 BioSAK-1.83.2/BioSAK/KEGG.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3484 2023-05-09 01:09:35.000000 BioSAK-1.83.2/BioSAK/KEGG_boxplot_last1row.R
+-rw-r--r--   0 songweizhi   (501) staff       (20)      269 2023-05-09 01:09:35.000000 BioSAK-1.83.2/BioSAK/KEGG_get_eukaryotic_kos.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3077 2023-08-22 09:31:28.000000 BioSAK-1.83.2/BioSAK/KeepRemovingTmp.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2620 2024-01-16 05:10:59.000000 BioSAK-1.83.2/BioSAK/MeanMappingDepth.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3682 2024-01-16 12:39:58.000000 BioSAK-1.83.2/BioSAK/MetaBiosample.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)  3297822 2023-05-09 01:09:35.000000 BioSAK-1.83.2/BioSAK/MetaCHIP_phylo.hmm
+-rw-r--r--   0 songweizhi   (501) staff       (20)  1206805 2023-05-09 01:09:35.000000 BioSAK-1.83.2/BioSAK/MetaCyc_reactions_with_ec.txt
+-rw-r--r--   0 songweizhi   (501) staff       (20)    16960 2023-05-09 01:09:35.000000 BioSAK-1.83.2/BioSAK/NetEnzymes.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3713 2023-05-09 01:09:35.000000 BioSAK-1.83.2/BioSAK/Newick_tree_plotter.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1659 2024-01-16 05:10:59.000000 BioSAK-1.83.2/BioSAK/OneLineAln.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    10448 2023-05-09 01:09:35.000000 BioSAK-1.83.2/BioSAK/Prodigal.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     6048 2023-05-09 01:09:35.000000 BioSAK-1.83.2/BioSAK/Reads_simulator.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3573 2024-01-16 05:10:59.000000 BioSAK-1.83.2/BioSAK/RunGraphMB.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3833 2024-01-16 05:10:59.000000 BioSAK-1.83.2/BioSAK/SILVA_for_BLCA.py
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)     6255 2023-05-09 01:09:35.000000 BioSAK-1.83.2/BioSAK/SankeyTaxon.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     5678 2024-01-16 05:10:59.000000 BioSAK-1.83.2/BioSAK/SliceMSA.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3173 2024-01-16 05:10:59.000000 BioSAK-1.83.2/BioSAK/SubsampleLongReads.py
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)     1696 2024-01-16 05:10:59.000000 BioSAK-1.83.2/BioSAK/Tax4Fun2IndOTU.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3499 2024-04-11 13:05:22.000000 BioSAK-1.83.2/BioSAK/VERSION
+-rw-r--r--   0 songweizhi   (501) staff       (20)      467 2023-05-09 01:09:35.000000 BioSAK-1.83.2/BioSAK/VisBlastOp.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     9944 2023-05-09 01:09:35.000000 BioSAK-1.83.2/BioSAK/VisGeneFlk.py
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2023-05-09 01:09:35.000000 BioSAK-1.83.2/BioSAK/__init__.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2526 2024-03-25 14:00:14.000000 BioSAK-1.83.2/BioSAK/add_desc.py
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)    38577 2024-03-22 00:45:31.000000 BioSAK-1.83.2/BioSAK/arCOG.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     6985 2024-01-16 05:00:13.000000 BioSAK-1.83.2/BioSAK/bam2reads.py
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)     2630 2024-03-22 13:23:45.000000 BioSAK-1.83.2/BioSAK/boxplot.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3312 2023-05-09 01:09:35.000000 BioSAK-1.83.2/BioSAK/boxplot_last1row.R
+-rw-r--r--   0 songweizhi   (501) staff       (20)     6104 2023-05-09 01:09:35.000000 BioSAK-1.83.2/BioSAK/boxplot_matrix_COG.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     5403 2023-05-09 01:09:35.000000 BioSAK-1.83.2/BioSAK/boxplot_matrix_COG_backup.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     6984 2023-05-09 01:09:35.000000 BioSAK-1.83.2/BioSAK/boxplot_matrix_KEGG.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     5747 2023-05-09 01:09:35.000000 BioSAK-1.83.2/BioSAK/boxplot_matrix_dbCAN.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1695 2023-05-09 01:09:35.000000 BioSAK-1.83.2/BioSAK/cat_fa.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    13440 2023-05-09 01:09:35.000000 BioSAK-1.83.2/BioSAK/cdd2cog.pl
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1186 2023-05-09 01:09:35.000000 BioSAK-1.83.2/BioSAK/checkm_marker.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1076 2023-05-09 01:09:35.000000 BioSAK-1.83.2/BioSAK/compare_trees.R
+-rw-r--r--   0 songweizhi   (501) staff       (20)     9745 2024-01-16 05:10:59.000000 BioSAK-1.83.2/BioSAK/compare_trees.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     6592 2023-05-09 01:09:35.000000 BioSAK-1.83.2/BioSAK/cross_link_seqs.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    24033 2024-03-22 00:45:31.000000 BioSAK-1.83.2/BioSAK/dbCAN.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1936 2023-05-09 01:09:35.000000 BioSAK-1.83.2/BioSAK/download_GenBank_genome_subset_prokaryotes_csv.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)      767 2023-05-09 01:09:35.000000 BioSAK-1.83.2/BioSAK/dwnld_sra_reads.py
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)    13250 2024-03-22 08:01:22.000000 BioSAK-1.83.2/BioSAK/enrich.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)      929 2023-05-09 01:09:35.000000 BioSAK-1.83.2/BioSAK/exe_cmds.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1508 2023-12-05 01:06:39.000000 BioSAK-1.83.2/BioSAK/ezaai2mat.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1396 2023-12-05 01:02:55.000000 BioSAK-1.83.2/BioSAK/fa2id.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1195 2023-05-17 06:14:50.000000 BioSAK-1.83.2/BioSAK/fa2phy.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1363 2023-05-09 01:09:35.000000 BioSAK-1.83.2/BioSAK/fa2tree.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     6280 2023-05-09 01:09:35.000000 BioSAK-1.83.2/BioSAK/format_converter.py
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)     2861 2023-05-09 01:09:35.000000 BioSAK-1.83.2/BioSAK/format_leaf_name.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)      639 2023-05-09 01:09:35.000000 BioSAK-1.83.2/BioSAK/fq2fa.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3190 2024-04-09 11:41:51.000000 BioSAK-1.83.2/BioSAK/gapseq.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2846 2023-06-14 10:08:30.000000 BioSAK-1.83.2/BioSAK/gbk2faa.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3342 2023-06-14 10:14:13.000000 BioSAK-1.83.2/BioSAK/gbk2ffn.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2528 2023-05-09 01:09:35.000000 BioSAK-1.83.2/BioSAK/gbk2fna.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3726 2023-05-09 01:09:35.000000 BioSAK-1.83.2/BioSAK/gbk_to_ffn_faa.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)      813 2023-05-09 01:09:35.000000 BioSAK-1.83.2/BioSAK/get_EC_from_ko_stats_D.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     7477 2023-05-09 01:09:35.000000 BioSAK-1.83.2/BioSAK/get_GTDB_taxon_gnm.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     5428 2023-06-15 03:03:02.000000 BioSAK-1.83.2/BioSAK/get_MAG_reads_long.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3991 2023-05-09 01:09:35.000000 BioSAK-1.83.2/BioSAK/get_Pfam_hmms.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    29246 2023-05-09 01:09:35.000000 BioSAK-1.83.2/BioSAK/get_SCG_tree.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1784 2023-05-09 01:09:35.000000 BioSAK-1.83.2/BioSAK/get_TopHits_taxonomy.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2247 2023-05-09 01:09:35.000000 BioSAK-1.83.2/BioSAK/get_aa_composition.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    12066 2023-05-09 01:09:35.000000 BioSAK-1.83.2/BioSAK/get_bin_abundance copy.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2139 2024-01-23 11:57:14.000000 BioSAK-1.83.2/BioSAK/get_data_matrix.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1339 2023-05-09 01:09:35.000000 BioSAK-1.83.2/BioSAK/get_gc.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     5523 2023-05-09 01:09:35.000000 BioSAK-1.83.2/BioSAK/get_gene_depth.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3591 2024-01-16 05:10:59.000000 BioSAK-1.83.2/BioSAK/get_genome_GTDB.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     6070 2024-01-16 04:57:23.000000 BioSAK-1.83.2/BioSAK/get_genome_NCBI.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    11209 2023-05-09 01:09:35.000000 BioSAK-1.83.2/BioSAK/get_genome_NCBI_v1.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    12620 2023-05-09 01:09:35.000000 BioSAK-1.83.2/BioSAK/get_genome_NCBI_v2.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3048 2023-05-09 01:09:35.000000 BioSAK-1.83.2/BioSAK/get_gnm_size.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     4834 2023-05-09 01:09:35.000000 BioSAK-1.83.2/BioSAK/get_ko_gene_seqs.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1192 2023-09-21 08:44:42.000000 BioSAK-1.83.2/BioSAK/get_krona_plot.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1559 2023-05-09 01:09:35.000000 BioSAK-1.83.2/BioSAK/get_reads_from_sam.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)      792 2023-05-09 01:09:35.000000 BioSAK-1.83.2/BioSAK/get_reads_id_in_sam.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2386 2023-05-09 01:09:35.000000 BioSAK-1.83.2/BioSAK/get_sankey_plot.R
+-rw-r--r--   0 songweizhi   (501) staff       (20)     4242 2023-05-09 01:09:35.000000 BioSAK-1.83.2/BioSAK/get_top_hit.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)      820 2023-05-09 01:09:35.000000 BioSAK-1.83.2/BioSAK/get_total_length.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     4643 2023-05-18 01:37:58.000000 BioSAK-1.83.2/BioSAK/global_functions.py
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)     2910 2024-03-11 00:57:02.000000 BioSAK-1.83.2/BioSAK/hpc3.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    26816 2024-04-11 13:05:22.000000 BioSAK-1.83.2/BioSAK/iTOL.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3337 2024-03-07 03:01:35.000000 BioSAK-1.83.2/BioSAK/js_cmds.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3281 2024-04-08 09:48:49.000000 BioSAK-1.83.2/BioSAK/js_hpc3.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1643 2023-05-09 01:09:35.000000 BioSAK-1.83.2/BioSAK/keep_best_hit.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)  3361029 2023-05-09 01:09:35.000000 BioSAK-1.83.2/BioSAK/ko00001.keg
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1848 2024-03-10 15:18:30.000000 BioSAK-1.83.2/BioSAK/koala.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2772 2023-05-09 01:09:35.000000 BioSAK-1.83.2/BioSAK/label_tree.R
+-rw-r--r--   0 songweizhi   (501) staff       (20)     4788 2024-01-16 05:10:59.000000 BioSAK-1.83.2/BioSAK/label_tree.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    35857 2023-05-09 01:09:35.000000 BioSAK-1.83.2/BioSAK/link_16S_MAG.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    12349 2023-05-09 01:09:35.000000 BioSAK-1.83.2/BioSAK/magabund.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    19855 2023-05-09 01:09:35.000000 BioSAK-1.83.2/BioSAK/magabund2.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1224 2023-05-09 01:09:35.000000 BioSAK-1.83.2/BioSAK/manipulator_fasta.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)        0 2023-05-09 01:09:35.000000 BioSAK-1.83.2/BioSAK/manipulator_msa.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3659 2023-05-09 01:09:35.000000 BioSAK-1.83.2/BioSAK/manipulator_newick.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)        0 2023-05-09 01:09:35.000000 BioSAK-1.83.2/BioSAK/manipulator_sam.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2433 2023-05-30 01:59:44.000000 BioSAK-1.83.2/BioSAK/mean_MAG_cov.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1880 2024-03-25 06:45:20.000000 BioSAK-1.83.2/BioSAK/merge_df.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2405 2024-01-16 05:10:59.000000 BioSAK-1.83.2/BioSAK/merge_seq.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     6742 2024-01-23 07:37:01.000000 BioSAK-1.83.2/BioSAK/metaAssembly.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1327 2023-06-11 13:56:21.000000 BioSAK-1.83.2/BioSAK/metabat2concoct.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1612 2023-06-11 16:00:51.000000 BioSAK-1.83.2/BioSAK/metabat2maxbin.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)        0 2023-05-09 01:09:35.000000 BioSAK-1.83.2/BioSAK/msa_to_distance_matrix.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1759 2023-05-09 01:09:35.000000 BioSAK-1.83.2/BioSAK/ncbi_dataset.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)        0 2024-03-03 11:00:02.000000 BioSAK-1.83.2/BioSAK/odp.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2820 2023-05-09 01:09:35.000000 BioSAK-1.83.2/BioSAK/parse_MetaCyc_RxnDB.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1460 2023-09-18 14:42:31.000000 BioSAK-1.83.2/BioSAK/parse_mmseqs_tsv.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     8633 2024-01-16 05:10:59.000000 BioSAK-1.83.2/BioSAK/plot_mag.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     7332 2023-05-09 01:09:35.000000 BioSAK-1.83.2/BioSAK/plot_sam_depth.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1638 2023-05-09 01:09:35.000000 BioSAK-1.83.2/BioSAK/plot_tree.R
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2256 2023-07-22 00:36:16.000000 BioSAK-1.83.2/BioSAK/prefix_file.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     4221 2024-01-16 05:10:59.000000 BioSAK-1.83.2/BioSAK/prokka.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     5057 2023-08-03 02:58:56.000000 BioSAK-1.83.2/BioSAK/reads2bam.py
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)     2534 2023-05-09 01:09:35.000000 BioSAK-1.83.2/BioSAK/rename_leaves.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2005 2023-05-09 01:09:35.000000 BioSAK-1.83.2/BioSAK/rename_reads_for_Reago.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     6801 2023-10-26 11:55:44.000000 BioSAK-1.83.2/BioSAK/rename_seq.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2210 2024-01-16 05:10:59.000000 BioSAK-1.83.2/BioSAK/rename_seqs.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)      144 2024-03-03 10:34:33.000000 BioSAK-1.83.2/BioSAK/ribbon.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1996 2023-05-09 01:09:35.000000 BioSAK-1.83.2/BioSAK/sam2bam.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     6877 2023-05-13 11:01:19.000000 BioSAK-1.83.2/BioSAK/sampling_GTDB_gnms.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3603 2024-01-16 05:10:59.000000 BioSAK-1.83.2/BioSAK/select_seq.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3167 2023-05-09 01:09:35.000000 BioSAK-1.83.2/BioSAK/sep_reads_by_barcode.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2671 2024-01-16 05:10:59.000000 BioSAK-1.83.2/BioSAK/slice_seq.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3788 2023-05-09 01:09:35.000000 BioSAK-1.83.2/BioSAK/split_fasta.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1998 2024-01-16 05:10:59.000000 BioSAK-1.83.2/BioSAK/split_folder.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     4561 2023-05-09 01:09:35.000000 BioSAK-1.83.2/BioSAK/split_sam.py
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)     1204 2024-01-16 05:10:59.000000 BioSAK-1.83.2/BioSAK/submitHPC.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2011 2024-01-16 05:10:59.000000 BioSAK-1.83.2/BioSAK/subset_GTDB_meta.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     4585 2024-04-09 03:15:33.000000 BioSAK-1.83.2/BioSAK/subset_df.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     7296 2024-01-16 05:10:59.000000 BioSAK-1.83.2/BioSAK/subset_tree.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     7844 2024-01-16 05:10:59.000000 BioSAK-1.83.2/BioSAK/top_16S_hits.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2106 2023-05-09 01:09:35.000000 BioSAK-1.83.2/BioSAK/top_hits_in_a_group.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)      831 2024-04-09 06:05:51.000000 BioSAK-1.83.2/BioSAK/transpose.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2252 2024-01-16 05:10:59.000000 BioSAK-1.83.2/BioSAK/usearch_uc.py
+drwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2024-04-11 13:05:26.862193 BioSAK-1.83.2/BioSAK.egg-info/
+-rw-r--r--   0 songweizhi   (501) staff       (20)      508 2024-04-11 13:05:26.000000 BioSAK-1.83.2/BioSAK.egg-info/PKG-INFO
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3630 2024-04-11 13:05:26.000000 BioSAK-1.83.2/BioSAK.egg-info/SOURCES.txt
+-rw-r--r--   0 songweizhi   (501) staff       (20)        1 2024-04-11 13:05:26.000000 BioSAK-1.83.2/BioSAK.egg-info/dependency_links.txt
+-rw-r--r--   0 songweizhi   (501) staff       (20)       95 2024-04-11 13:05:26.000000 BioSAK-1.83.2/BioSAK.egg-info/requires.txt
+-rw-r--r--   0 songweizhi   (501) staff       (20)        7 2024-04-11 13:05:26.000000 BioSAK-1.83.2/BioSAK.egg-info/top_level.txt
+-rw-r--r--   0 songweizhi   (501) staff       (20)    35141 2023-05-09 01:09:36.000000 BioSAK-1.83.2/LICENSE
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)      300 2023-05-09 01:09:36.000000 BioSAK-1.83.2/MANIFEST.in
+-rw-r--r--   0 songweizhi   (501) staff       (20)      508 2024-04-11 13:05:26.862493 BioSAK-1.83.2/PKG-INFO
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1533 2024-01-23 07:37:01.000000 BioSAK-1.83.2/README.md
+drwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2024-04-11 13:05:26.860834 BioSAK-1.83.2/bin/
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)    72931 2024-04-09 06:05:51.000000 BioSAK-1.83.2/bin/BioSAK
+-rw-r--r--   0 songweizhi   (501) staff       (20)       38 2024-04-11 13:05:26.862791 BioSAK-1.83.2/setup.cfg
+-rw-r--r--   0 songweizhi   (501) staff       (20)      915 2024-01-15 11:41:11.000000 BioSAK-1.83.2/setup.py
```

### Comparing `BioSAK-1.83.1/BioSAK/BLCA_op_parser.py` & `BioSAK-1.83.2/BioSAK/BLCA_op_parser.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/BioSAK_config.py` & `BioSAK-1.83.2/BioSAK/BioSAK_config.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/COG2020.py` & `BioSAK-1.83.2/BioSAK/COG2020.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/COG_boxplot_last1row.R` & `BioSAK-1.83.2/BioSAK/COG_boxplot_last1row.R`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/COG_boxplot_last2row.R` & `BioSAK-1.83.2/BioSAK/COG_boxplot_last2row.R`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/CheckM.py` & `BioSAK-1.83.2/BioSAK/CheckM.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/ConvertMSA.py` & `BioSAK-1.83.2/BioSAK/ConvertMSA.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/DnaFeaturesViewer.py` & `BioSAK-1.83.2/BioSAK/DnaFeaturesViewer.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/FastaSplitler_by_num.py` & `BioSAK-1.83.2/BioSAK/FastaSplitler_by_num.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/FastaSplitler_by_size.py` & `BioSAK-1.83.2/BioSAK/FastaSplitler_by_size.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/GTDB_for_BLCA.py` & `BioSAK-1.83.2/BioSAK/GTDB_for_BLCA.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/Gene2Ctg.py` & `BioSAK-1.83.2/BioSAK/Gene2Ctg.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/KEGG.py` & `BioSAK-1.83.2/BioSAK/KEGG.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/KEGG_boxplot_last1row.R` & `BioSAK-1.83.2/BioSAK/KEGG_boxplot_last1row.R`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/KeepRemovingTmp.py` & `BioSAK-1.83.2/BioSAK/KeepRemovingTmp.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/MeanMappingDepth.py` & `BioSAK-1.83.2/BioSAK/MeanMappingDepth.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/MetaBiosample.py` & `BioSAK-1.83.2/BioSAK/MetaBiosample.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/MetaCHIP_phylo.hmm` & `BioSAK-1.83.2/BioSAK/MetaCHIP_phylo.hmm`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/MetaCyc_reactions_with_ec.txt` & `BioSAK-1.83.2/BioSAK/MetaCyc_reactions_with_ec.txt`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/NetEnzymes.py` & `BioSAK-1.83.2/BioSAK/NetEnzymes.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/Newick_tree_plotter.py` & `BioSAK-1.83.2/BioSAK/Newick_tree_plotter.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/OneLineAln.py` & `BioSAK-1.83.2/BioSAK/OneLineAln.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/Prodigal.py` & `BioSAK-1.83.2/BioSAK/Prodigal.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/Reads_simulator.py` & `BioSAK-1.83.2/BioSAK/Reads_simulator.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/RunGraphMB.py` & `BioSAK-1.83.2/BioSAK/RunGraphMB.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/SILVA_for_BLCA.py` & `BioSAK-1.83.2/BioSAK/SILVA_for_BLCA.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/SankeyTaxon.py` & `BioSAK-1.83.2/BioSAK/SankeyTaxon.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/SliceMSA.py` & `BioSAK-1.83.2/BioSAK/SliceMSA.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/SubsampleLongReads.py` & `BioSAK-1.83.2/BioSAK/SubsampleLongReads.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/Tax4Fun2IndOTU.py` & `BioSAK-1.83.2/BioSAK/Tax4Fun2IndOTU.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/VERSION` & `BioSAK-1.83.2/BioSAK/VERSION`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-1.83.1
+1.83.2
 - fixed bugs
 
 1.83.0
 - new module added: transpose
 
 1.82.0
 - new module added: gapseq
```

### Comparing `BioSAK-1.83.1/BioSAK/VisGeneFlk.py` & `BioSAK-1.83.2/BioSAK/VisGeneFlk.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/add_desc.py` & `BioSAK-1.83.2/BioSAK/add_desc.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/arCOG.py` & `BioSAK-1.83.2/BioSAK/arCOG.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/bam2reads.py` & `BioSAK-1.83.2/BioSAK/bam2reads.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/boxplot.py` & `BioSAK-1.83.2/BioSAK/boxplot.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/boxplot_last1row.R` & `BioSAK-1.83.2/BioSAK/boxplot_last1row.R`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/boxplot_matrix_COG.py` & `BioSAK-1.83.2/BioSAK/boxplot_matrix_COG.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/boxplot_matrix_COG_backup.py` & `BioSAK-1.83.2/BioSAK/boxplot_matrix_COG_backup.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/boxplot_matrix_KEGG.py` & `BioSAK-1.83.2/BioSAK/boxplot_matrix_KEGG.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/boxplot_matrix_dbCAN.py` & `BioSAK-1.83.2/BioSAK/boxplot_matrix_dbCAN.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/cat_fa.py` & `BioSAK-1.83.2/BioSAK/cat_fa.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/cdd2cog.pl` & `BioSAK-1.83.2/BioSAK/cdd2cog.pl`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/checkm_marker.py` & `BioSAK-1.83.2/BioSAK/checkm_marker.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/compare_trees.R` & `BioSAK-1.83.2/BioSAK/compare_trees.R`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/compare_trees.py` & `BioSAK-1.83.2/BioSAK/compare_trees.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/cross_link_seqs.py` & `BioSAK-1.83.2/BioSAK/cross_link_seqs.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/dbCAN.py` & `BioSAK-1.83.2/BioSAK/dbCAN.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/download_GenBank_genome_subset_prokaryotes_csv.py` & `BioSAK-1.83.2/BioSAK/download_GenBank_genome_subset_prokaryotes_csv.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/dwnld_sra_reads.py` & `BioSAK-1.83.2/BioSAK/dwnld_sra_reads.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/enrich.py` & `BioSAK-1.83.2/BioSAK/enrich.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/exe_cmds.py` & `BioSAK-1.83.2/BioSAK/exe_cmds.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/ezaai2mat.py` & `BioSAK-1.83.2/BioSAK/ezaai2mat.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/fa2id.py` & `BioSAK-1.83.2/BioSAK/fa2id.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/fa2phy.py` & `BioSAK-1.83.2/BioSAK/fa2phy.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/fa2tree.py` & `BioSAK-1.83.2/BioSAK/fa2tree.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/format_converter.py` & `BioSAK-1.83.2/BioSAK/format_converter.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/format_leaf_name.py` & `BioSAK-1.83.2/BioSAK/format_leaf_name.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/fq2fa.py` & `BioSAK-1.83.2/BioSAK/fq2fa.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/gapseq.py` & `BioSAK-1.83.2/BioSAK/gapseq.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/gbk2faa.py` & `BioSAK-1.83.2/BioSAK/gbk2faa.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/gbk2ffn.py` & `BioSAK-1.83.2/BioSAK/gbk2ffn.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/gbk2fna.py` & `BioSAK-1.83.2/BioSAK/gbk2fna.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/gbk_to_ffn_faa.py` & `BioSAK-1.83.2/BioSAK/gbk_to_ffn_faa.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/get_EC_from_ko_stats_D.py` & `BioSAK-1.83.2/BioSAK/get_EC_from_ko_stats_D.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/get_GTDB_taxon_gnm.py` & `BioSAK-1.83.2/BioSAK/get_GTDB_taxon_gnm.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/get_MAG_reads_long.py` & `BioSAK-1.83.2/BioSAK/get_MAG_reads_long.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/get_Pfam_hmms.py` & `BioSAK-1.83.2/BioSAK/get_Pfam_hmms.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/get_SCG_tree.py` & `BioSAK-1.83.2/BioSAK/get_SCG_tree.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/get_TopHits_taxonomy.py` & `BioSAK-1.83.2/BioSAK/get_TopHits_taxonomy.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/get_aa_composition.py` & `BioSAK-1.83.2/BioSAK/get_aa_composition.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/get_bin_abundance copy.py` & `BioSAK-1.83.2/BioSAK/get_bin_abundance copy.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/get_data_matrix.py` & `BioSAK-1.83.2/BioSAK/get_data_matrix.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/get_gc.py` & `BioSAK-1.83.2/BioSAK/get_gc.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/get_gene_depth.py` & `BioSAK-1.83.2/BioSAK/get_gene_depth.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/get_genome_GTDB.py` & `BioSAK-1.83.2/BioSAK/get_genome_GTDB.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/get_genome_NCBI.py` & `BioSAK-1.83.2/BioSAK/get_genome_NCBI.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/get_genome_NCBI_v1.py` & `BioSAK-1.83.2/BioSAK/get_genome_NCBI_v1.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/get_genome_NCBI_v2.py` & `BioSAK-1.83.2/BioSAK/get_genome_NCBI_v2.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/get_gnm_size.py` & `BioSAK-1.83.2/BioSAK/get_gnm_size.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/get_ko_gene_seqs.py` & `BioSAK-1.83.2/BioSAK/get_ko_gene_seqs.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/get_krona_plot.py` & `BioSAK-1.83.2/BioSAK/get_krona_plot.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/get_reads_from_sam.py` & `BioSAK-1.83.2/BioSAK/get_reads_from_sam.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/get_reads_id_in_sam.py` & `BioSAK-1.83.2/BioSAK/get_reads_id_in_sam.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/get_sankey_plot.R` & `BioSAK-1.83.2/BioSAK/get_sankey_plot.R`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/get_top_hit.py` & `BioSAK-1.83.2/BioSAK/get_top_hit.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/get_total_length.py` & `BioSAK-1.83.2/BioSAK/get_total_length.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/global_functions.py` & `BioSAK-1.83.2/BioSAK/global_functions.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/hpc3.py` & `BioSAK-1.83.2/BioSAK/hpc3.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/iTOL.py` & `BioSAK-1.83.2/BioSAK/iTOL.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 BioSAK iTOL -Binary -lm Binary_matrix.txt -lt Enzyme -o Presence_Absence_iTOL.txt
 BioSAK iTOL -Heatmap -lm MagAbundance.txt -lt Abundance -o Heatmap_abundance.txt
 BioSAK iTOL -SimpleBar -lv MagSize.txt -scale 0-3-6-9 -lt Size -o SimpleBar_size.txt
 BioSAK iTOL -ColorStrip -lg MagTaxon.txt -lt Phylum -o ColorStrip_taxon.txt
 BioSAK iTOL -ColorRange -lg MagTaxon.txt -lt Phylum -o ColorRange_taxon.txt
 BioSAK iTOL -ColorRange -taxon Taxonomy.txt -rank f -lt Family -o ColorRange_taxon.txt
 BioSAK iTOL -ExternalShape -lm identity_matrix.txt -lt Identity -scale 25-50-75-100 -o ExternalShape_identity.txt
+BioSAK iTOL -PieChart -lv MagCompleteness.txt -lt Completeness -o PieChart_completeness.txt
 
 # Leaf-to-Group file format (-lg, tab separated, no header)
 genome_1	Bacteria
 genome_2	Archaea
 
 # taxonomy file format (-taxon, tab separated, GTDB-format taxononomy string)
 genome_1	d__Bacteria;p__Proteobacteria;c__Alphaproteobacteria;o__Dongiales;f__Dongiaceae;g__Dongia;s__Dongia mobilis
@@ -54,15 +55,14 @@
         color_list_combined = ['#3787c0', '#39399f', '#ffb939', '#399f39', '#9f399f', '#fb694a', '#9f9f39', '#959595']
 
     elif 8 < color_num <= 16:
         color_list_combined = ['#2b7bba', '#89bedc', '#2e2e99', '#8a8acc', '#ffa500', '#ffc55c', '#2e992e', '#8acc8a', '#992e99', '#cc8acc', '#d52221', '#fc8161', '#99992e', '#cccc8a', '#5c5c5c', '#adadad']
 
     else:
         color_num_each = math.ceil(color_num/8) + 2
-
         color_list_1 = sns.color_palette('Blues',  n_colors=color_num_each).as_hex()
         color_list_2 = sns.light_palette('navy',   n_colors=color_num_each).as_hex()
         color_list_3 = sns.light_palette('orange', n_colors=color_num_each).as_hex()
         color_list_4 = sns.light_palette('green',  n_colors=color_num_each).as_hex()
         color_list_5 = sns.light_palette('purple', n_colors=color_num_each).as_hex()
         color_list_6 = sns.color_palette('Reds',   n_colors=color_num_each).as_hex()
         color_list_7 = sns.light_palette('olive',  n_colors=color_num_each).as_hex()
@@ -118,14 +118,15 @@
     ColorStrip      = args['ColorStrip']
     ColorRange      = args['ColorRange']
     SimpleBar       = args['SimpleBar']
     Heatmap         = args['Heatmap']
     ExternalShape   = args['ExternalShape']
     Binary          = args['Binary']
     Connection      = args['Connection']
+    PieChart        = args['PieChart']
     LeafGroup       = args['lg']
     GroupColor      = args['gc']
     ColumnColor     = args['cc']
     LeafValue       = args['lv']
     LeafLabel       = args['ll']
     LeafMatrix      = args['lm']
     d2r             = args['dr']
@@ -146,19 +147,17 @@
     SimpleBar_SCALE_WIDTH       = 1
     SimpleBar_SCALE_DASHED      = 1
     SimpleBar_SCALE_FontSize    = 2
 
     # Heatmap
     Heatmap_STRIP_WIDTH         = 60
 
-    # ExternalShape
-
     # check the number of specified file type
     True_num = 0
-    for file_type in [Labels, ColorStrip, ColorRange, SimpleBar, Heatmap, ExternalShape, Binary]:
+    for file_type in [Labels, ColorStrip, ColorRange, SimpleBar, Heatmap, ExternalShape, Binary, PieChart]:
         if file_type is True:
             True_num += 1
 
     if True_num == 0:
         print('Please specify one file type, choose from -ColorStrip, -ColorRange, -SimpleBar, -Heatmap, -ExternalShape or -Binary')
         exit()
     if True_num > 1:
@@ -230,26 +229,23 @@
 
         # write out legend info
         FileOut_handle.write('\n# customize legend here\n')
         FileOut_handle.write('LEGEND_TITLE\t%s\n' % LegendTitle)
         FileOut_handle.write('LEGEND_SHAPES\t%s\n' % '\t'.join(['1' for i in Group_to_Color_dict]))
         FileOut_handle.write('LEGEND_COLORS\t%s\n' % '\t'.join(color_list))
         FileOut_handle.write('LEGEND_LABELS\t%s\n' % '\t'.join(group_list))
-
-        # write out data info
         FileOut_handle.write('\n# provide data here\nDATA\n')
         for leaf in Leaf_to_Group_dict:
             leaf_group = Leaf_to_Group_dict[leaf]
             leaf_color = Group_to_Color_dict[leaf_group]
 
             if ColorStrip is True:
                 FileOut_handle.write('%s\t%s\t%s\n' % (leaf, leaf_color, leaf_group))
             if ColorRange is True:
                 FileOut_handle.write('%s\trange\t%s\t%s\n' % (leaf, leaf_color, leaf_group))
-
         FileOut_handle.close()
 
     ####################################################################################################################
 
     # Prepare SimpleBar file
     if SimpleBar is True:
 
@@ -268,21 +264,17 @@
             if max_value == None:
                 max_value = float(leaf_value_split[1])
             else:
                 if float(leaf_value_split[1]) > max_value:
                     max_value = float(leaf_value_split[1])
 
         SimpleBar_FileOut_handle = open(FileOut, 'w')
-
-        # write out header
         SimpleBar_FileOut_handle.write('DATASET_SIMPLEBAR\n')
         SimpleBar_FileOut_handle.write('# Reference: https://itol.embl.de/help/dataset_simplebar_template.txt\n')
         SimpleBar_FileOut_handle.write('\nSEPARATOR TAB\n')
-
-        # write out SimpleBar attributes
         SimpleBar_FileOut_handle.write('\n# customize barchart attributes here\n')
         SimpleBar_FileOut_handle.write('DATASET_LABEL\t%s\n'    % LegendTitle)
         SimpleBar_FileOut_handle.write('COLOR\t%s\n'            % SimpleBar_COLOR)
         SimpleBar_FileOut_handle.write('WIDTH\t%s\n'            % SimpleBar_WIDTH)
         SimpleBar_FileOut_handle.write('MARGIN\t%s\n'           % MARGIN)
         SimpleBar_FileOut_handle.write('HEIGHT_FACTOR\t%s\n'    % SimpleBar_HEIGHT_FACTOR)
         SimpleBar_FileOut_handle.write('BORDER_WIDTH\t%s\n'     % SimpleBar_BORDER_WIDTH)
@@ -292,16 +284,14 @@
         for scale_value in scale_str.split('-'):
             scale_attributes = '%s-%s-%s-%s-%s-%s' % (scale_value, scale_value, SimpleBar_SCALE_COLOR, SimpleBar_SCALE_WIDTH, SimpleBar_SCALE_DASHED, SimpleBar_SCALE_FontSize)
             scale_attributes_list.append(scale_attributes)
 
         SimpleBar_FileOut_handle.write('\n# customize scale attributes here\n')
         SimpleBar_FileOut_handle.write('# format: VALUE-LABEL-COLOR-WIDTH-DASHED-LABEL_SCALE_FACTOR, LABEL_SCALE_FACTOR controls font size\n')
         SimpleBar_FileOut_handle.write('DATASET_SCALE\t%s\n' % '\t'.join(scale_attributes_list))
-
-        # write out data info
         SimpleBar_FileOut_handle.write('\n# provide data here\n')
         SimpleBar_FileOut_handle.write('DATA\n')
 
         for leaf in leaf_value_dict:
             SimpleBar_FileOut_handle.write('%s\t%s\n' % (leaf, leaf_value_dict[leaf]))
 
         SimpleBar_FileOut_handle.close()
@@ -374,46 +364,37 @@
             if n == 0:
                 col_name_list = leaf_matrix_split[1:]
             else:
                 leaf_matrix_dict[leaf_matrix_split[0]] = leaf_matrix_split[1:]
             n += 1
 
         Heatmap_FileOut_handle = open(FileOut, 'w')
-
-        # write out header
         Heatmap_FileOut_handle.write('DATASET_HEATMAP\n')
         Heatmap_FileOut_handle.write('# Reference https://itol.embl.de/help/dataset_heatmap_template.txt\n')
         Heatmap_FileOut_handle.write('\nSEPARATOR TAB\n')
-
-        # write out heatmap attributes
         Heatmap_FileOut_handle.write('\n# customize heatmap attributes here\n')
         Heatmap_FileOut_handle.write('MARGIN\t%s\n'          % MARGIN)
         Heatmap_FileOut_handle.write('STRIP_WIDTH\t%s\n'     % Heatmap_STRIP_WIDTH)
-
-        # write out legend info
         Heatmap_FileOut_handle.write('\n# customize legend here\n')
         Heatmap_FileOut_handle.write('AUTO_LEGEND\t1\n')
         Heatmap_FileOut_handle.write('DATASET_LABEL\t%s\n' % LegendTitle)
         Heatmap_FileOut_handle.write('USE_MID_COLOR\t1\n')
         Heatmap_FileOut_handle.write('COLOR_MIN\t#2980B9\n')
         Heatmap_FileOut_handle.write('COLOR_MID\t#ECF0F1\n')
         Heatmap_FileOut_handle.write('COLOR_MAX\t#E74C3C\n')
         Heatmap_FileOut_handle.write('\n# customize value range here. By default, color gradients will be calculated based on dataset values\n')
         Heatmap_FileOut_handle.write('# USER_MIN_VALUE	0\n')
         Heatmap_FileOut_handle.write('# USER_MID_VALUE	5\n')
         Heatmap_FileOut_handle.write('# USER_MAX_VALUE	10\n')
         Heatmap_FileOut_handle.write('\n# customize column name here\n')
         Heatmap_FileOut_handle.write('FIELD_LABELS\t%s\n' % '\t'.join(col_name_list))
-
-        # write out data info
         Heatmap_FileOut_handle.write('\n# Provide data here\n')
         Heatmap_FileOut_handle.write('DATA\n')
         for leaf in leaf_matrix_dict:
             Heatmap_FileOut_handle.write('%s\t%s\n' % (leaf, '\t'.join(leaf_matrix_dict[leaf])))
-
         Heatmap_FileOut_handle.close()
 
     ####################################################################################################################
 
     if Labels is True:
 
         if os.path.isfile(LeafLabel) is False:
@@ -441,14 +422,33 @@
         Connection_FileOut_handle.write('MAXIMUM_LINE_WIDTH\t10\nCURVE_ANGLE\t45\nCENTER_CURVES\t1\nALIGN_TO_LABELS\t0\nDATA\n')
         for each_connection in open(d2r):
             Connection_FileOut_handle.write(each_connection)
         Connection_FileOut_handle.close()
 
     ####################################################################################################################
 
+    # Prepare PieChart file
+    if PieChart is True:
+        PieChart_FileOut_handle = open(FileOut, 'w')
+        PieChart_FileOut_handle.write('DATASET_PIECHART\n')
+        PieChart_FileOut_handle.write('SEPARATOR TAB\n')
+        PieChart_FileOut_handle.write('DATASET_LABEL\tCompleteness\n')
+        PieChart_FileOut_handle.write('COLOR\t#ff0000\n')
+        PieChart_FileOut_handle.write('FIELD_COLORS\t#5DADE2\t#FFFFFF\n')
+        PieChart_FileOut_handle.write('FIELD_LABELS\tf1\tf2\n')
+        PieChart_FileOut_handle.write('DATA\n')
+        for each in open(LeafValue):
+            each_split = each.strip().split('\t')
+            node_id = each_split[0]
+            node_value = float(each_split[1])
+            PieChart_FileOut_handle.write('%s\t-1\t1\t%s\t%s\n' % (node_id, node_value, (100 - node_value)))
+        PieChart_FileOut_handle.close()
+
+    ####################################################################################################################
+
     # Prepare ExternalShape file
     if ExternalShape is True:
 
         # read in leaf matrix into dict
         n = 0
         col_name_list = []
         leaf_matrix_dict = {}
@@ -474,16 +474,14 @@
                     unfound_cols.append(each_col_header)
             if len(unfound_cols) > 0:
                 print('Color code for the following columns are not provided, program exited!')
                 print(','.join(unfound_cols))
                 exit()
 
         ExternalShape_FileOut_handle = open(FileOut, 'w')
-
-        # write out header
         ExternalShape_FileOut_handle.write('DATASET_EXTERNALSHAPE\n')
         ExternalShape_FileOut_handle.write('# Reference https://itol.embl.de/help/dataset_external_shapes_template.txt\n')
         ExternalShape_FileOut_handle.write('\nSEPARATOR TAB\n')
 
         # define scale here
         if scale_str is None:
             print('Please provide scale values for ExternalShapes, e.g., 25-50-75-100, 2-4-6-8-10')
@@ -495,16 +493,14 @@
         SHAPE_SCALES_list = scale_str_to_size_list(scale_str)
 
         ExternalShape_FileOut_handle.write('LEGEND_TITLE\t%s\n' % LegendTitle)
         ExternalShape_FileOut_handle.write('LEGEND_SHAPES\t%s\n' % '\t'.join(LEGEND_SHAPES_list))
         ExternalShape_FileOut_handle.write('LEGEND_COLORS\t%s\n' % '\t'.join(LEGEND_COLORS_list))
         ExternalShape_FileOut_handle.write('LEGEND_LABELS\t%s\n' % '\t'.join(scale_list))
         ExternalShape_FileOut_handle.write('LEGEND_SHAPE_SCALES\t%s\n' % '\t'.join(str(i) for i in SHAPE_SCALES_list))
-
-        # write out ExternalShape attributes
         ExternalShape_FileOut_handle.write('\n# customize attributes here\n')
         ExternalShape_FileOut_handle.write('VERTICAL_GRID\t0\n')
         ExternalShape_FileOut_handle.write('HORIZONTAL_GRID\t0\n')
         ExternalShape_FileOut_handle.write('SHAPE_TYPE\t2\n')
         ExternalShape_FileOut_handle.write('COLOR_FILL\t1\n')
         ExternalShape_FileOut_handle.write('SHAPE_SPACING\t1\n')
         ExternalShape_FileOut_handle.write('SHOW_LABELS\t0\n')
@@ -521,16 +517,14 @@
         ExternalShape_FileOut_handle.write('FIELD_LABELS\t%s\n' % '\t'.join(col_name_list))
 
         color_list = get_color_list(len(col_name_list))
         random.shuffle(color_list)
         if ColumnColor is not None:
             color_list = [Column_to_Color_dict[i] for i in col_name_list]
         ExternalShape_FileOut_handle.write('FIELD_COLORS\t%s\n' % '\t'.join(color_list))
-
-        # write out data info
         ExternalShape_FileOut_handle.write('\n# Provide data here\n')
         ExternalShape_FileOut_handle.write('DATA\n')
         for leaf in leaf_matrix_dict:
             ExternalShape_FileOut_handle.write('%s\t%s\n' % (leaf, '\t'.join(leaf_matrix_dict[leaf])))
 
         ExternalShape_FileOut_handle.close()
 
@@ -545,24 +539,20 @@
     parser.add_argument('-ColorStrip',      required=False, action='store_true',   help='ColorStrip')
     parser.add_argument('-ColorRange',      required=False, action='store_true',   help='ColorRange')
     parser.add_argument('-SimpleBar',       required=False, action='store_true',   help='SimpleBar')
     parser.add_argument('-Heatmap',         required=False, action='store_true',   help='Heatmap')
     parser.add_argument('-ExternalShape',   required=False, action='store_true',   help='ExternalShape')
     parser.add_argument('-Binary',          required=False, action='store_true',   help='Binary')
     parser.add_argument('-Connection',      required=False, action='store_true',   help='Connection')
+    parser.add_argument('-PieChart',        required=False, action='store_true',   help='PieChart')
     parser.add_argument('-ll',              required=False, default=None,          help='Leaf Label')
     parser.add_argument('-lg',              required=False, default=None,          help='Leaf Group')
     parser.add_argument('-gc',              required=False, default=None,          help='Specify Group/column Color (optional)')
     parser.add_argument('-cc',              required=False, default=None,          help='Specify Column Color (for ExternalShape format) (optional)')
     parser.add_argument('-lv',              required=False, default=None,          help='Leaf Value')
     parser.add_argument('-lm',              required=False, default=None,          help='Leaf Matrix')
     parser.add_argument('-dr',              required=False, default=None,          help='Donor to Recipient')
     parser.add_argument('-scale',           required=False, default=None,          help='Scale Values, in format 0-3-6-9')
     parser.add_argument('-lt',              required=False, default=None,          help='Legend Title')
     parser.add_argument('-o',               required=True,                         help='Output filename')
     args = vars(parser.parse_args())
     iTOL(args)
-
-
-# parser.add_argument('-taxon',           required=False, default=None,          help='Leaf taxonomy, gtdb format')
-# parser.add_argument('-rank',            required=False, default=None,          help='Taxonomy rank, select from p, c, o, f, g or s')
-# LABELS Labels
```

### Comparing `BioSAK-1.83.1/BioSAK/js_cmds.py` & `BioSAK-1.83.2/BioSAK/js_cmds.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/js_hpc3.py` & `BioSAK-1.83.2/BioSAK/js_hpc3.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/keep_best_hit.py` & `BioSAK-1.83.2/BioSAK/keep_best_hit.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/ko00001.keg` & `BioSAK-1.83.2/BioSAK/ko00001.keg`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/koala.py` & `BioSAK-1.83.2/BioSAK/koala.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/label_tree.R` & `BioSAK-1.83.2/BioSAK/label_tree.R`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/label_tree.py` & `BioSAK-1.83.2/BioSAK/label_tree.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/link_16S_MAG.py` & `BioSAK-1.83.2/BioSAK/link_16S_MAG.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/magabund.py` & `BioSAK-1.83.2/BioSAK/magabund.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/magabund2.py` & `BioSAK-1.83.2/BioSAK/magabund2.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/manipulator_fasta.py` & `BioSAK-1.83.2/BioSAK/manipulator_fasta.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/manipulator_newick.py` & `BioSAK-1.83.2/BioSAK/manipulator_newick.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/mean_MAG_cov.py` & `BioSAK-1.83.2/BioSAK/mean_MAG_cov.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/merge_df.py` & `BioSAK-1.83.2/BioSAK/merge_df.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/merge_seq.py` & `BioSAK-1.83.2/BioSAK/merge_seq.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/metaAssembly.py` & `BioSAK-1.83.2/BioSAK/metaAssembly.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/metabat2concoct.py` & `BioSAK-1.83.2/BioSAK/metabat2concoct.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/metabat2maxbin.py` & `BioSAK-1.83.2/BioSAK/metabat2maxbin.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/ncbi_dataset.py` & `BioSAK-1.83.2/BioSAK/ncbi_dataset.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/parse_MetaCyc_RxnDB.py` & `BioSAK-1.83.2/BioSAK/parse_MetaCyc_RxnDB.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/parse_mmseqs_tsv.py` & `BioSAK-1.83.2/BioSAK/parse_mmseqs_tsv.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/plot_mag.py` & `BioSAK-1.83.2/BioSAK/plot_mag.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/plot_sam_depth.py` & `BioSAK-1.83.2/BioSAK/plot_sam_depth.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/plot_tree.R` & `BioSAK-1.83.2/BioSAK/plot_tree.R`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/prefix_file.py` & `BioSAK-1.83.2/BioSAK/prefix_file.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/prokka.py` & `BioSAK-1.83.2/BioSAK/prokka.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/reads2bam.py` & `BioSAK-1.83.2/BioSAK/reads2bam.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/rename_leaves.py` & `BioSAK-1.83.2/BioSAK/rename_leaves.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/rename_reads_for_Reago.py` & `BioSAK-1.83.2/BioSAK/rename_reads_for_Reago.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/rename_seq.py` & `BioSAK-1.83.2/BioSAK/rename_seq.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/rename_seqs.py` & `BioSAK-1.83.2/BioSAK/rename_seqs.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/sam2bam.py` & `BioSAK-1.83.2/BioSAK/sam2bam.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/sampling_GTDB_gnms.py` & `BioSAK-1.83.2/BioSAK/sampling_GTDB_gnms.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/select_seq.py` & `BioSAK-1.83.2/BioSAK/select_seq.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/sep_reads_by_barcode.py` & `BioSAK-1.83.2/BioSAK/sep_reads_by_barcode.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/slice_seq.py` & `BioSAK-1.83.2/BioSAK/slice_seq.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/split_fasta.py` & `BioSAK-1.83.2/BioSAK/split_fasta.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/split_folder.py` & `BioSAK-1.83.2/BioSAK/split_folder.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/split_sam.py` & `BioSAK-1.83.2/BioSAK/split_sam.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/submitHPC.py` & `BioSAK-1.83.2/BioSAK/submitHPC.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/subset_GTDB_meta.py` & `BioSAK-1.83.2/BioSAK/subset_GTDB_meta.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/subset_df.py` & `BioSAK-1.83.2/BioSAK/subset_df.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/subset_tree.py` & `BioSAK-1.83.2/BioSAK/subset_tree.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/top_16S_hits.py` & `BioSAK-1.83.2/BioSAK/top_16S_hits.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/top_hits_in_a_group.py` & `BioSAK-1.83.2/BioSAK/top_hits_in_a_group.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/transpose.py` & `BioSAK-1.83.2/BioSAK/transpose.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK/usearch_uc.py` & `BioSAK-1.83.2/BioSAK/usearch_uc.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/BioSAK.egg-info/SOURCES.txt` & `BioSAK-1.83.2/BioSAK.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/LICENSE` & `BioSAK-1.83.2/LICENSE`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/README.md` & `BioSAK-1.83.2/README.md`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/bin/BioSAK` & `BioSAK-1.83.2/bin/BioSAK`

 * *Files identical despite different names*

### Comparing `BioSAK-1.83.1/setup.py` & `BioSAK-1.83.2/setup.py`

 * *Files identical despite different names*

