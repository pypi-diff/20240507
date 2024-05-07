# Comparing `tmp/receptor_digger-0.7.1.tar.gz` & `tmp/receptor_digger-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "receptor_digger-0.7.1.tar", last modified: Fri Mar 29 15:44:39 2024, max compression
+gzip compressed data, was "receptor_digger-0.7.2.tar", last modified: Tue May  7 10:55:38 2024, max compression
```

## Comparing `receptor_digger-0.7.1.tar` & `receptor_digger-0.7.2.tar`

### file list

```diff
@@ -1,215 +1,215 @@
-drwxrwxrwx   0        0        0        0 2024-03-29 15:44:39.136551 receptor_digger-0.7.1/
--rw-rw-rw-   0        0        0     1401 2024-03-24 10:26:23.000000 receptor_digger-0.7.1/MANIFEST.in
--rw-rw-rw-   0        0        0      936 2024-03-29 15:44:39.136551 receptor_digger-0.7.1/PKG-INFO
--rw-rw-rw-   0        0        0      227 2024-03-24 10:26:23.000000 receptor_digger-0.7.1/README.md
--rw-rw-rw-   0        0        0      452 2024-03-24 10:26:23.000000 receptor_digger-0.7.1/license.txt
--rw-rw-rw-   0        0        0      110 2021-12-29 13:39:50.000000 receptor_digger-0.7.1/pyproject.toml
--rw-rw-rw-   0        0        0     1232 2024-03-29 15:44:39.138551 receptor_digger-0.7.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-29 15:44:38.748607 receptor_digger-0.7.1/src/
-drwxrwxrwx   0        0        0        0 2024-03-29 15:44:38.778609 receptor_digger-0.7.1/src/digger/
--rw-rw-rw-   0        0        0        0 2023-03-13 09:47:31.000000 receptor_digger-0.7.1/src/digger/__init__.py
--rw-rw-rw-   0        0        0     1364 2023-03-29 15:03:23.000000 receptor_digger-0.7.1/src/digger/blastresults_to_csv.py
--rw-rw-rw-   0        0        0     7746 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/calc_motifs.py
--rw-rw-rw-   0        0        0     2169 2023-02-06 16:38:59.000000 receptor_digger-0.7.1/src/digger/cirelli_contig_matches.py
--rw-rw-rw-   0        0        0      344 2023-02-06 16:38:59.000000 receptor_digger-0.7.1/src/digger/cirelli_to_fasta.py
--rw-rw-rw-   0        0        0    15097 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/compare_annotations.py
--rw-rw-rw-   0        0        0     9988 2024-03-24 10:26:23.000000 receptor_digger-0.7.1/src/digger/dig_sequence.py
--rw-rw-rw-   0        0        0    15908 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/dig_utils.py
--rw-rw-rw-   0        0        0     8470 2024-03-29 13:36:52.000000 receptor_digger-0.7.1/src/digger/digger.py
--rw-rw-rw-   0        0        0    20283 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/find_alignments.py
--rw-rw-rw-   0        0        0     4287 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motif.py
-drwxrwxrwx   0        0        0        0 2024-03-29 15:44:38.746605 receptor_digger-0.7.1/src/digger/motifs/
-drwxrwxrwx   0        0        0        0 2024-03-29 15:44:38.746605 receptor_digger-0.7.1/src/digger/motifs/human/
-drwxrwxrwx   0        0        0        0 2024-03-29 15:44:38.805605 receptor_digger-0.7.1/src/digger/motifs/human/IGH/
--rw-rw-rw-   0        0        0      223 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/IGH/3'D-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      272 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/IGH/3'D-NONAMER_prob.csv
--rw-rw-rw-   0        0        0      226 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/IGH/5'D-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      267 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/IGH/5'D-NONAMER_prob.csv
--rw-rw-rw-   0        0        0      220 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/IGH/J-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      278 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/IGH/J-NONAMER_prob.csv
--rw-rw-rw-   0        0        0     1814 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/IGH/L-PART1_1_48_prob.csv
--rw-rw-rw-   0        0        0     1417 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/IGH/L-PART1_2_48_prob.csv
--rw-rw-rw-   0        0        0     1819 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/IGH/L-PART1_3_48_prob.csv
--rw-rw-rw-   0        0        0     1825 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/IGH/L-PART1_4_48_prob.csv
--rw-rw-rw-   0        0        0     1694 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/IGH/L-PART1_5_51_prob.csv
--rw-rw-rw-   0        0        0     2005 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/IGH/L-PART1_6_63_prob.csv
--rw-rw-rw-   0        0        0      340 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/IGH/L-PART2_1_11_prob.csv
--rw-rw-rw-   0        0        0      255 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/IGH/OCTAMER_prob.csv
--rw-rw-rw-   0        0        0      222 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/IGH/V-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      266 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/IGH/V-NONAMER_prob.csv
--rw-rw-rw-   0        0        0      117 2023-04-06 10:56:41.000000 receptor_digger-0.7.1/src/digger/motifs/human/IGH/conserved_motifs.fasta
--rw-rw-rw-   0        0        0      246 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/IGH/motif_params.json
-drwxrwxrwx   0        0        0        0 2024-03-29 15:44:38.916646 receptor_digger-0.7.1/src/digger/motifs/human/IGK/
--rw-rw-rw-   0        0        0      226 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/IGK/J-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      284 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/IGK/J-NONAMER_prob.csv
--rw-rw-rw-   0        0        0     1540 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/IGK/L-PART1_1_48_prob.csv
--rw-rw-rw-   0        0        0     1817 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/IGK/L-PART1_2_57_prob.csv
--rw-rw-rw-   0        0        0     1739 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/IGK/L-PART1_3_51_prob.csv
--rw-rw-rw-   0        0        0     1739 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/IGK/L-PART1_4_51_prob.csv
--rw-rw-rw-   0        0        0     1739 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/IGK/L-PART1_5_51_prob.csv
--rw-rw-rw-   0        0        0     1739 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/IGK/L-PART1_6_51_prob.csv
--rw-rw-rw-   0        0        0     1448 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/IGK/L-PART1_prob.csv
--rw-rw-rw-   0        0        0      322 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/IGK/L-PART2_1_11_prob.csv
--rw-rw-rw-   0        0        0      251 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/IGK/L-PART2_prob.csv
--rw-rw-rw-   0        0        0      255 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/IGK/OCTAMER_prob.csv
--rw-rw-rw-   0        0        0      226 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/IGK/V-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      284 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/IGK/V-NONAMER_prob.csv
--rw-rw-rw-   0        0        0      117 2023-03-26 18:09:48.000000 receptor_digger-0.7.1/src/digger/motifs/human/IGK/conserved_motifs.fasta
--rw-rw-rw-   0        0        0      245 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/IGK/motif_params.json
-drwxrwxrwx   0        0        0        0 2024-03-29 15:44:38.942552 receptor_digger-0.7.1/src/digger/motifs/human/IGL/
--rw-rw-rw-   0        0        0      226 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/IGL/J-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      284 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/IGL/J-NONAMER_prob.csv
--rw-rw-rw-   0        0        0     1363 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/IGL/L-PART1_1_42_prob.csv
--rw-rw-rw-   0        0        0     1499 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/IGL/L-PART1_2_47_prob.csv
--rw-rw-rw-   0        0        0     1749 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/IGL/L-PART1_3_48_prob.csv
--rw-rw-rw-   0        0        0     1759 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/IGL/L-PART1_4_48_prob.csv
--rw-rw-rw-   0        0        0     1783 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/IGL/L-PART1_5_48_prob.csv
--rw-rw-rw-   0        0        0     1733 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/IGL/L-PART1_6_48_prob.csv
--rw-rw-rw-   0        0        0     1564 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/IGL/L-PART1_7_49_prob.csv
--rw-rw-rw-   0        0        0     1659 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/IGL/L-PART1_8_51_prob.csv
--rw-rw-rw-   0        0        0     1803 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/IGL/L-PART1_9_54_prob.csv
--rw-rw-rw-   0        0        0      330 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/IGL/L-PART2_1_11_prob.csv
--rw-rw-rw-   0        0        0      255 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/IGL/OCTAMER_prob.csv
--rw-rw-rw-   0        0        0      226 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/IGL/V-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      271 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/IGL/V-NONAMER_prob.csv
--rw-rw-rw-   0        0        0      117 2023-03-26 18:09:48.000000 receptor_digger-0.7.1/src/digger/motifs/human/IGL/conserved_motifs.fasta
--rw-rw-rw-   0        0        0      245 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/IGL/motif_params.json
-drwxrwxrwx   0        0        0        0 2024-03-29 15:44:38.986550 receptor_digger-0.7.1/src/digger/motifs/human/TRA/
--rw-rw-rw-   0        0        0    21121 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/TRA/IMGT000024_genes_lpart1.csv
--rw-rw-rw-   0        0        0     4251 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/TRA/IMGT000024_genes_lpart2.csv
--rw-rw-rw-   0        0        0      223 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/TRA/J-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      277 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/TRA/J-NONAMER_prob.csv
--rw-rw-rw-   0        0        0     1834 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/TRA/L-PART1_10_51_prob.csv
--rw-rw-rw-   0        0        0     1834 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/TRA/L-PART1_11_51_prob.csv
--rw-rw-rw-   0        0        0     1834 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/TRA/L-PART1_12_51_prob.csv
--rw-rw-rw-   0        0        0     1834 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/TRA/L-PART1_13_51_prob.csv
--rw-rw-rw-   0        0        0     2063 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/TRA/L-PART1_14_54_prob.csv
--rw-rw-rw-   0        0        0     2063 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/TRA/L-PART1_15_54_prob.csv
--rw-rw-rw-   0        0        0     2063 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/TRA/L-PART1_16_54_prob.csv
--rw-rw-rw-   0        0        0     1989 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/TRA/L-PART1_17_54_prob.csv
--rw-rw-rw-   0        0        0     1817 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/TRA/L-PART1_18_57_prob.csv
--rw-rw-rw-   0        0        0     1397 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/TRA/L-PART1_1_42_prob.csv
--rw-rw-rw-   0        0        0     1397 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/TRA/L-PART1_2_42_prob.csv
--rw-rw-rw-   0        0        0     1571 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/TRA/L-PART1_3_45_prob.csv
--rw-rw-rw-   0        0        0     1571 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/TRA/L-PART1_4_45_prob.csv
--rw-rw-rw-   0        0        0     1571 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/TRA/L-PART1_5_45_prob.csv
--rw-rw-rw-   0        0        0     1824 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/TRA/L-PART1_6_48_prob.csv
--rw-rw-rw-   0        0        0     1808 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/TRA/L-PART1_7_48_prob.csv
--rw-rw-rw-   0        0        0     1850 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/TRA/L-PART1_8_48_prob.csv
--rw-rw-rw-   0        0        0     1850 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/TRA/L-PART1_9_48_prob.csv
--rw-rw-rw-   0        0        0      951 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/TRA/L-PART2_1_32_prob.csv
--rw-rw-rw-   0        0        0      252 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/TRA/L-PART2_2_8_prob.csv
--rw-rw-rw-   0        0        0      303 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/TRA/L-PART2_3_11_prob.csv
--rw-rw-rw-   0        0        0      429 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/TRA/L-PART2_4_14_prob.csv
--rw-rw-rw-   0        0        0      777 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/TRA/L-PART2_5_26_prob.csv
--rw-rw-rw-   0        0        0      225 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/TRA/V-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      275 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/TRA/V-NONAMER_prob.csv
--rw-rw-rw-   0        0        0      255 2024-03-24 10:26:23.000000 receptor_digger-0.7.1/src/digger/motifs/human/TRA/motif_params.json
-drwxrwxrwx   0        0        0        0 2024-03-29 15:44:39.015551 receptor_digger-0.7.1/src/digger/motifs/human/TRB/
--rw-rw-rw-   0        0        0      226 2024-03-24 10:26:23.000000 receptor_digger-0.7.1/src/digger/motifs/human/TRB/3'D-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      284 2024-03-24 10:26:23.000000 receptor_digger-0.7.1/src/digger/motifs/human/TRB/3'D-NONAMER_prob.csv
--rw-rw-rw-   0        0        0      226 2024-03-24 10:26:23.000000 receptor_digger-0.7.1/src/digger/motifs/human/TRB/5'D-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      284 2024-03-24 10:26:23.000000 receptor_digger-0.7.1/src/digger/motifs/human/TRB/5'D-NONAMER_prob.csv
--rw-rw-rw-   0        0        0      226 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/TRB/J-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      274 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/TRB/J-NONAMER_prob.csv
--rw-rw-rw-   0        0        0     1159 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/TRB/L-PART1_1_36_prob.csv
--rw-rw-rw-   0        0        0     2569 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/TRB/L-PART1_2_81_prob.csv
--rw-rw-rw-   0        0        0     1883 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/TRB/L-PART1_3_51_prob.csv
--rw-rw-rw-   0        0        0     1910 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/TRB/L-PART1_4_51_prob.csv
--rw-rw-rw-   0        0        0     1916 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/TRB/L-PART1_5_51_prob.csv
--rw-rw-rw-   0        0        0     1805 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/TRB/L-PART1_6_51_prob.csv
--rw-rw-rw-   0        0        0     1698 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/TRB/L-PART1_7_52_prob.csv
--rw-rw-rw-   0        0        0     1911 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/TRB/L-PART1_8_60_prob.csv
--rw-rw-rw-   0        0        0     2005 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/TRB/L-PART1_9_63_prob.csv
--rw-rw-rw-   0        0        0      243 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/TRB/L-PART2_1_8_prob.csv
--rw-rw-rw-   0        0        0      342 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/TRB/L-PART2_2_11_prob.csv
--rw-rw-rw-   0        0        0      226 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/TRB/V-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      284 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/TRB/V-NONAMER_prob.csv
--rw-rw-rw-   0        0        0      188 2024-03-24 10:26:23.000000 receptor_digger-0.7.1/src/digger/motifs/human/TRB/motif_params.json
-drwxrwxrwx   0        0        0        0 2024-03-29 15:44:39.035550 receptor_digger-0.7.1/src/digger/motifs/human/TRD/
--rw-rw-rw-   0        0        0      226 2024-03-24 10:26:23.000000 receptor_digger-0.7.1/src/digger/motifs/human/TRD/3'D-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      284 2024-03-24 10:26:23.000000 receptor_digger-0.7.1/src/digger/motifs/human/TRD/3'D-NONAMER_prob.csv
--rw-rw-rw-   0        0        0      226 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/TRD/5'D-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      284 2024-03-24 10:26:23.000000 receptor_digger-0.7.1/src/digger/motifs/human/TRD/5'D-NONAMER_prob.csv
--rw-rw-rw-   0        0        0      214 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/TRD/J-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      270 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/TRD/J-NONAMER_prob.csv
--rw-rw-rw-   0        0        0     1535 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/TRD/L-PART1_1_48_prob.csv
--rw-rw-rw-   0        0        0     1629 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/TRD/L-PART1_2_51_prob.csv
--rw-rw-rw-   0        0        0      342 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/TRD/L-PART2_1_11_prob.csv
--rw-rw-rw-   0        0        0      429 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/TRD/L-PART2_2_14_prob.csv
--rw-rw-rw-   0        0        0      226 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/TRD/V-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      284 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/TRD/V-NONAMER_prob.csv
--rw-rw-rw-   0        0        0      188 2024-03-24 10:26:23.000000 receptor_digger-0.7.1/src/digger/motifs/human/TRD/motif_params.json
-drwxrwxrwx   0        0        0        0 2024-03-29 15:44:39.049551 receptor_digger-0.7.1/src/digger/motifs/human/TRG/
--rw-rw-rw-   0        0        0      216 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/TRG/J-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      284 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/TRG/J-NONAMER_prob.csv
--rw-rw-rw-   0        0        0     1535 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/TRG/L-PART1_1_48_prob.csv
--rw-rw-rw-   0        0        0     1471 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/TRG/L-PART1_2_45_prob.csv
--rw-rw-rw-   0        0        0      342 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/TRG/L-PART2_1_11_prob.csv
--rw-rw-rw-   0        0        0      429 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/TRG/L-PART2_2_14_prob.csv
--rw-rw-rw-   0        0        0      226 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/TRG/V-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      284 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/human/TRG/V-NONAMER_prob.csv
--rw-rw-rw-   0        0        0      255 2024-03-24 10:26:23.000000 receptor_digger-0.7.1/src/digger/motifs/human/TRG/motif_params.json
-drwxrwxrwx   0        0        0        0 2024-03-29 15:44:38.748607 receptor_digger-0.7.1/src/digger/motifs/rhesus_macaque/
-drwxrwxrwx   0        0        0        0 2024-03-29 15:44:39.077551 receptor_digger-0.7.1/src/digger/motifs/rhesus_macaque/IGH/
--rw-rw-rw-   0        0        0      226 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/rhesus_macaque/IGH/3'D-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      200 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/rhesus_macaque/IGH/3'D-NONAMER_prob.csv
--rw-rw-rw-   0        0        0      226 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/rhesus_macaque/IGH/5'D-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      284 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/rhesus_macaque/IGH/5'D-NONAMER_prob.csv
--rw-rw-rw-   0        0        0      220 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/rhesus_macaque/IGH/J-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      275 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/rhesus_macaque/IGH/J-NONAMER_prob.csv
--rw-rw-rw-   0        0        0     1799 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/rhesus_macaque/IGH/L-PART1_1_48_prob.csv
--rw-rw-rw-   0        0        0     1815 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/rhesus_macaque/IGH/L-PART1_2_48_prob.csv
--rw-rw-rw-   0        0        0     1811 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/rhesus_macaque/IGH/L-PART1_3_48_prob.csv
--rw-rw-rw-   0        0        0     1815 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/rhesus_macaque/IGH/L-PART1_4_48_prob.csv
--rw-rw-rw-   0        0        0     1699 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/rhesus_macaque/IGH/L-PART1_5_51_prob.csv
--rw-rw-rw-   0        0        0     1288 2023-02-06 16:38:59.000000 receptor_digger-0.7.1/src/digger/motifs/rhesus_macaque/IGH/L-PART1_prob.csv
--rw-rw-rw-   0        0        0      516 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/rhesus_macaque/IGH/L-PART2_1_17_prob.csv
--rw-rw-rw-   0        0        0      240 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/rhesus_macaque/IGH/L-PART2_2_11_prob.csv
--rw-rw-rw-   0        0        0      320 2023-02-06 16:38:59.000000 receptor_digger-0.7.1/src/digger/motifs/rhesus_macaque/IGH/L-PART2_prob.csv
--rw-rw-rw-   0        0        0      220 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/rhesus_macaque/IGH/V-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      278 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/rhesus_macaque/IGH/V-NONAMER_prob.csv
--rw-rw-rw-   0        0        0      165 2023-04-04 14:13:25.000000 receptor_digger-0.7.1/src/digger/motifs/rhesus_macaque/IGH/conserved_motifs.fasta
--rw-rw-rw-   0        0        0      246 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/rhesus_macaque/IGH/motif_params.json
-drwxrwxrwx   0        0        0        0 2024-03-29 15:44:39.097551 receptor_digger-0.7.1/src/digger/motifs/rhesus_macaque/IGK/
--rw-rw-rw-   0        0        0      226 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/rhesus_macaque/IGK/J-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      284 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/rhesus_macaque/IGK/J-NONAMER_prob.csv
--rw-rw-rw-   0        0        0     1875 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/rhesus_macaque/IGK/L-PART1_1_57_prob.csv
--rw-rw-rw-   0        0        0     1830 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/rhesus_macaque/IGK/L-PART1_2_51_prob.csv
--rw-rw-rw-   0        0        0     1834 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/rhesus_macaque/IGK/L-PART1_3_51_prob.csv
--rw-rw-rw-   0        0        0     1831 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/rhesus_macaque/IGK/L-PART1_4_51_prob.csv
--rw-rw-rw-   0        0        0     1783 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/rhesus_macaque/IGK/L-PART1_5_51_prob.csv
--rw-rw-rw-   0        0        0      327 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/rhesus_macaque/IGK/L-PART2_1_11_prob.csv
--rw-rw-rw-   0        0        0      226 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/rhesus_macaque/IGK/V-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      284 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/rhesus_macaque/IGK/V-NONAMER_prob.csv
--rw-rw-rw-   0        0        0       90 2023-04-04 10:42:00.000000 receptor_digger-0.7.1/src/digger/motifs/rhesus_macaque/IGK/conserved_motifs.fasta
--rw-rw-rw-   0        0        0      245 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/rhesus_macaque/IGK/motif_params.json
-drwxrwxrwx   0        0        0        0 2024-03-29 15:44:39.122551 receptor_digger-0.7.1/src/digger/motifs/rhesus_macaque/IGL/
--rw-rw-rw-   0        0        0      226 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/rhesus_macaque/IGL/J-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      276 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/rhesus_macaque/IGL/J-NONAMER_prob.csv
--rw-rw-rw-   0        0        0     1253 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/rhesus_macaque/IGL/L-PART1_1_39_prob.csv
--rw-rw-rw-   0        0        0     1347 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/rhesus_macaque/IGL/L-PART1_2_42_prob.csv
--rw-rw-rw-   0        0        0     1476 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/rhesus_macaque/IGL/L-PART1_3_45_prob.csv
--rw-rw-rw-   0        0        0     1783 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/rhesus_macaque/IGL/L-PART1_4_48_prob.csv
--rw-rw-rw-   0        0        0     1792 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/rhesus_macaque/IGL/L-PART1_5_48_prob.csv
--rw-rw-rw-   0        0        0     1767 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/rhesus_macaque/IGL/L-PART1_6_48_prob.csv
--rw-rw-rw-   0        0        0     1800 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/rhesus_macaque/IGL/L-PART1_7_48_prob.csv
--rw-rw-rw-   0        0        0     1629 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/rhesus_macaque/IGL/L-PART1_8_51_prob.csv
--rw-rw-rw-   0        0        0     1817 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/rhesus_macaque/IGL/L-PART1_9_57_prob.csv
--rw-rw-rw-   0        0        0      339 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/rhesus_macaque/IGL/L-PART2_1_11_prob.csv
--rw-rw-rw-   0        0        0      224 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/rhesus_macaque/IGL/V-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      284 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/rhesus_macaque/IGL/V-NONAMER_prob.csv
--rw-rw-rw-   0        0        0       90 2023-04-04 11:10:35.000000 receptor_digger-0.7.1/src/digger/motifs/rhesus_macaque/IGL/conserved_motifs.fasta
--rw-rw-rw-   0        0        0      245 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/motifs/rhesus_macaque/IGL/motif_params.json
--rw-rw-rw-   0        0        0    52622 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/parse_genes.py
--rw-rw-rw-   0        0        0    15126 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/parse_imgt_annotations.py
--rw-rw-rw-   0        0        0    13030 2024-03-25 11:25:58.000000 receptor_digger-0.7.1/src/digger/search_motifs.py
--rw-rw-rw-   0        0        0     2187 2024-03-24 10:26:23.000000 receptor_digger-0.7.1/src/digger/setup_motif_params.py
--rw-rw-rw-   0        0        0      856 2023-02-06 16:38:59.000000 receptor_digger-0.7.1/src/digger/slugify.py
-drwxrwxrwx   0        0        0        0 2024-03-29 15:44:39.134550 receptor_digger-0.7.1/src/receptor_digger.egg-info/
--rw-rw-rw-   0        0        0      936 2024-03-29 15:44:38.000000 receptor_digger-0.7.1/src/receptor_digger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     9536 2024-03-29 15:44:38.000000 receptor_digger-0.7.1/src/receptor_digger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-29 15:44:38.000000 receptor_digger-0.7.1/src/receptor_digger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      338 2024-03-29 15:44:38.000000 receptor_digger-0.7.1/src/receptor_digger.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       55 2024-03-29 15:44:38.000000 receptor_digger-0.7.1/src/receptor_digger.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-03-29 15:44:38.000000 receptor_digger-0.7.1/src/receptor_digger.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-07 10:55:38.050549 receptor_digger-0.7.2/
+-rw-rw-rw-   0        0        0     1401 2024-03-24 10:26:23.000000 receptor_digger-0.7.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      936 2024-05-07 10:55:38.047550 receptor_digger-0.7.2/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2024-03-24 10:26:23.000000 receptor_digger-0.7.2/README.md
+-rw-rw-rw-   0        0        0      452 2024-03-24 10:26:23.000000 receptor_digger-0.7.2/license.txt
+-rw-rw-rw-   0        0        0      110 2021-12-29 13:39:50.000000 receptor_digger-0.7.2/pyproject.toml
+-rw-rw-rw-   0        0        0     1242 2024-05-07 10:55:38.053048 receptor_digger-0.7.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-07 10:55:37.421801 receptor_digger-0.7.2/src/
+drwxrwxrwx   0        0        0        0 2024-05-07 10:55:37.639701 receptor_digger-0.7.2/src/digger/
+-rw-rw-rw-   0        0        0        0 2023-03-13 09:47:31.000000 receptor_digger-0.7.2/src/digger/__init__.py
+-rw-rw-rw-   0        0        0     1364 2023-03-29 15:03:23.000000 receptor_digger-0.7.2/src/digger/blastresults_to_csv.py
+-rw-rw-rw-   0        0        0     7746 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/calc_motifs.py
+-rw-rw-rw-   0        0        0     2169 2023-02-06 16:38:59.000000 receptor_digger-0.7.2/src/digger/cirelli_contig_matches.py
+-rw-rw-rw-   0        0        0      344 2023-02-06 16:38:59.000000 receptor_digger-0.7.2/src/digger/cirelli_to_fasta.py
+-rw-rw-rw-   0        0        0    15097 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/compare_annotations.py
+-rw-rw-rw-   0        0        0     9988 2024-03-24 10:26:23.000000 receptor_digger-0.7.2/src/digger/dig_sequence.py
+-rw-rw-rw-   0        0        0    15908 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/dig_utils.py
+-rw-rw-rw-   0        0        0     8542 2024-04-01 14:18:10.000000 receptor_digger-0.7.2/src/digger/digger.py
+-rw-rw-rw-   0        0        0    20180 2024-05-07 08:04:12.000000 receptor_digger-0.7.2/src/digger/find_alignments.py
+-rw-rw-rw-   0        0        0     4287 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motif.py
+drwxrwxrwx   0        0        0        0 2024-05-07 10:55:37.419801 receptor_digger-0.7.2/src/digger/motifs/
+drwxrwxrwx   0        0        0        0 2024-05-07 10:55:37.419301 receptor_digger-0.7.2/src/digger/motifs/human/
+drwxrwxrwx   0        0        0        0 2024-05-07 10:55:37.673971 receptor_digger-0.7.2/src/digger/motifs/human/IGH/
+-rw-rw-rw-   0        0        0      223 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/IGH/3'D-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      272 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/IGH/3'D-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0      226 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/IGH/5'D-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      267 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/IGH/5'D-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0      220 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/IGH/J-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      278 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/IGH/J-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0     1814 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/IGH/L-PART1_1_48_prob.csv
+-rw-rw-rw-   0        0        0     1417 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/IGH/L-PART1_2_48_prob.csv
+-rw-rw-rw-   0        0        0     1819 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/IGH/L-PART1_3_48_prob.csv
+-rw-rw-rw-   0        0        0     1825 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/IGH/L-PART1_4_48_prob.csv
+-rw-rw-rw-   0        0        0     1694 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/IGH/L-PART1_5_51_prob.csv
+-rw-rw-rw-   0        0        0     2005 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/IGH/L-PART1_6_63_prob.csv
+-rw-rw-rw-   0        0        0      340 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/IGH/L-PART2_1_11_prob.csv
+-rw-rw-rw-   0        0        0      255 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/IGH/OCTAMER_prob.csv
+-rw-rw-rw-   0        0        0      222 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/IGH/V-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      266 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/IGH/V-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0      117 2023-04-06 10:56:41.000000 receptor_digger-0.7.2/src/digger/motifs/human/IGH/conserved_motifs.fasta
+-rw-rw-rw-   0        0        0      246 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/IGH/motif_params.json
+drwxrwxrwx   0        0        0        0 2024-05-07 10:55:37.705490 receptor_digger-0.7.2/src/digger/motifs/human/IGK/
+-rw-rw-rw-   0        0        0      226 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/IGK/J-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      284 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/IGK/J-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0     1540 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/IGK/L-PART1_1_48_prob.csv
+-rw-rw-rw-   0        0        0     1817 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/IGK/L-PART1_2_57_prob.csv
+-rw-rw-rw-   0        0        0     1739 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/IGK/L-PART1_3_51_prob.csv
+-rw-rw-rw-   0        0        0     1739 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/IGK/L-PART1_4_51_prob.csv
+-rw-rw-rw-   0        0        0     1739 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/IGK/L-PART1_5_51_prob.csv
+-rw-rw-rw-   0        0        0     1739 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/IGK/L-PART1_6_51_prob.csv
+-rw-rw-rw-   0        0        0     1448 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/IGK/L-PART1_prob.csv
+-rw-rw-rw-   0        0        0      322 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/IGK/L-PART2_1_11_prob.csv
+-rw-rw-rw-   0        0        0      251 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/IGK/L-PART2_prob.csv
+-rw-rw-rw-   0        0        0      255 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/IGK/OCTAMER_prob.csv
+-rw-rw-rw-   0        0        0      226 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/IGK/V-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      284 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/IGK/V-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0      117 2023-03-26 18:09:48.000000 receptor_digger-0.7.2/src/digger/motifs/human/IGK/conserved_motifs.fasta
+-rw-rw-rw-   0        0        0      245 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/IGK/motif_params.json
+drwxrwxrwx   0        0        0        0 2024-05-07 10:55:37.737989 receptor_digger-0.7.2/src/digger/motifs/human/IGL/
+-rw-rw-rw-   0        0        0      226 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/IGL/J-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      284 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/IGL/J-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0     1363 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/IGL/L-PART1_1_42_prob.csv
+-rw-rw-rw-   0        0        0     1499 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/IGL/L-PART1_2_47_prob.csv
+-rw-rw-rw-   0        0        0     1749 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/IGL/L-PART1_3_48_prob.csv
+-rw-rw-rw-   0        0        0     1759 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/IGL/L-PART1_4_48_prob.csv
+-rw-rw-rw-   0        0        0     1783 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/IGL/L-PART1_5_48_prob.csv
+-rw-rw-rw-   0        0        0     1733 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/IGL/L-PART1_6_48_prob.csv
+-rw-rw-rw-   0        0        0     1564 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/IGL/L-PART1_7_49_prob.csv
+-rw-rw-rw-   0        0        0     1659 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/IGL/L-PART1_8_51_prob.csv
+-rw-rw-rw-   0        0        0     1803 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/IGL/L-PART1_9_54_prob.csv
+-rw-rw-rw-   0        0        0      330 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/IGL/L-PART2_1_11_prob.csv
+-rw-rw-rw-   0        0        0      255 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/IGL/OCTAMER_prob.csv
+-rw-rw-rw-   0        0        0      226 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/IGL/V-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      271 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/IGL/V-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0      117 2023-03-26 18:09:48.000000 receptor_digger-0.7.2/src/digger/motifs/human/IGL/conserved_motifs.fasta
+-rw-rw-rw-   0        0        0      245 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/IGL/motif_params.json
+drwxrwxrwx   0        0        0        0 2024-05-07 10:55:37.798278 receptor_digger-0.7.2/src/digger/motifs/human/TRA/
+-rw-rw-rw-   0        0        0    21121 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/TRA/IMGT000024_genes_lpart1.csv
+-rw-rw-rw-   0        0        0     4251 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/TRA/IMGT000024_genes_lpart2.csv
+-rw-rw-rw-   0        0        0      223 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/TRA/J-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      277 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/TRA/J-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0     1834 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/TRA/L-PART1_10_51_prob.csv
+-rw-rw-rw-   0        0        0     1834 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/TRA/L-PART1_11_51_prob.csv
+-rw-rw-rw-   0        0        0     1834 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/TRA/L-PART1_12_51_prob.csv
+-rw-rw-rw-   0        0        0     1834 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/TRA/L-PART1_13_51_prob.csv
+-rw-rw-rw-   0        0        0     2063 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/TRA/L-PART1_14_54_prob.csv
+-rw-rw-rw-   0        0        0     2063 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/TRA/L-PART1_15_54_prob.csv
+-rw-rw-rw-   0        0        0     2063 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/TRA/L-PART1_16_54_prob.csv
+-rw-rw-rw-   0        0        0     1989 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/TRA/L-PART1_17_54_prob.csv
+-rw-rw-rw-   0        0        0     1817 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/TRA/L-PART1_18_57_prob.csv
+-rw-rw-rw-   0        0        0     1397 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/TRA/L-PART1_1_42_prob.csv
+-rw-rw-rw-   0        0        0     1397 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/TRA/L-PART1_2_42_prob.csv
+-rw-rw-rw-   0        0        0     1571 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/TRA/L-PART1_3_45_prob.csv
+-rw-rw-rw-   0        0        0     1571 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/TRA/L-PART1_4_45_prob.csv
+-rw-rw-rw-   0        0        0     1571 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/TRA/L-PART1_5_45_prob.csv
+-rw-rw-rw-   0        0        0     1824 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/TRA/L-PART1_6_48_prob.csv
+-rw-rw-rw-   0        0        0     1808 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/TRA/L-PART1_7_48_prob.csv
+-rw-rw-rw-   0        0        0     1850 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/TRA/L-PART1_8_48_prob.csv
+-rw-rw-rw-   0        0        0     1850 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/TRA/L-PART1_9_48_prob.csv
+-rw-rw-rw-   0        0        0      951 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/TRA/L-PART2_1_32_prob.csv
+-rw-rw-rw-   0        0        0      252 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/TRA/L-PART2_2_8_prob.csv
+-rw-rw-rw-   0        0        0      303 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/TRA/L-PART2_3_11_prob.csv
+-rw-rw-rw-   0        0        0      429 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/TRA/L-PART2_4_14_prob.csv
+-rw-rw-rw-   0        0        0      777 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/TRA/L-PART2_5_26_prob.csv
+-rw-rw-rw-   0        0        0      225 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/TRA/V-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      275 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/TRA/V-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0      255 2024-03-24 10:26:23.000000 receptor_digger-0.7.2/src/digger/motifs/human/TRA/motif_params.json
+drwxrwxrwx   0        0        0        0 2024-05-07 10:55:37.838861 receptor_digger-0.7.2/src/digger/motifs/human/TRB/
+-rw-rw-rw-   0        0        0      226 2024-03-24 10:26:23.000000 receptor_digger-0.7.2/src/digger/motifs/human/TRB/3'D-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      284 2024-03-24 10:26:23.000000 receptor_digger-0.7.2/src/digger/motifs/human/TRB/3'D-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0      226 2024-03-24 10:26:23.000000 receptor_digger-0.7.2/src/digger/motifs/human/TRB/5'D-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      284 2024-03-24 10:26:23.000000 receptor_digger-0.7.2/src/digger/motifs/human/TRB/5'D-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0      226 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/TRB/J-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      274 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/TRB/J-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0     1159 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/TRB/L-PART1_1_36_prob.csv
+-rw-rw-rw-   0        0        0     2569 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/TRB/L-PART1_2_81_prob.csv
+-rw-rw-rw-   0        0        0     1883 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/TRB/L-PART1_3_51_prob.csv
+-rw-rw-rw-   0        0        0     1910 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/TRB/L-PART1_4_51_prob.csv
+-rw-rw-rw-   0        0        0     1916 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/TRB/L-PART1_5_51_prob.csv
+-rw-rw-rw-   0        0        0     1805 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/TRB/L-PART1_6_51_prob.csv
+-rw-rw-rw-   0        0        0     1698 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/TRB/L-PART1_7_52_prob.csv
+-rw-rw-rw-   0        0        0     1911 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/TRB/L-PART1_8_60_prob.csv
+-rw-rw-rw-   0        0        0     2005 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/TRB/L-PART1_9_63_prob.csv
+-rw-rw-rw-   0        0        0      243 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/TRB/L-PART2_1_8_prob.csv
+-rw-rw-rw-   0        0        0      342 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/TRB/L-PART2_2_11_prob.csv
+-rw-rw-rw-   0        0        0      226 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/TRB/V-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      284 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/TRB/V-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0      188 2024-03-24 10:26:23.000000 receptor_digger-0.7.2/src/digger/motifs/human/TRB/motif_params.json
+drwxrwxrwx   0        0        0        0 2024-05-07 10:55:37.864361 receptor_digger-0.7.2/src/digger/motifs/human/TRD/
+-rw-rw-rw-   0        0        0      226 2024-03-24 10:26:23.000000 receptor_digger-0.7.2/src/digger/motifs/human/TRD/3'D-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      284 2024-03-24 10:26:23.000000 receptor_digger-0.7.2/src/digger/motifs/human/TRD/3'D-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0      226 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/TRD/5'D-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      284 2024-03-24 10:26:23.000000 receptor_digger-0.7.2/src/digger/motifs/human/TRD/5'D-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0      214 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/TRD/J-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      270 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/TRD/J-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0     1535 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/TRD/L-PART1_1_48_prob.csv
+-rw-rw-rw-   0        0        0     1629 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/TRD/L-PART1_2_51_prob.csv
+-rw-rw-rw-   0        0        0      342 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/TRD/L-PART2_1_11_prob.csv
+-rw-rw-rw-   0        0        0      429 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/TRD/L-PART2_2_14_prob.csv
+-rw-rw-rw-   0        0        0      226 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/TRD/V-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      284 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/TRD/V-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0      188 2024-03-24 10:26:23.000000 receptor_digger-0.7.2/src/digger/motifs/human/TRD/motif_params.json
+drwxrwxrwx   0        0        0        0 2024-05-07 10:55:37.890529 receptor_digger-0.7.2/src/digger/motifs/human/TRG/
+-rw-rw-rw-   0        0        0      216 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/TRG/J-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      284 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/TRG/J-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0     1535 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/TRG/L-PART1_1_48_prob.csv
+-rw-rw-rw-   0        0        0     1471 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/TRG/L-PART1_2_45_prob.csv
+-rw-rw-rw-   0        0        0      342 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/TRG/L-PART2_1_11_prob.csv
+-rw-rw-rw-   0        0        0      429 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/TRG/L-PART2_2_14_prob.csv
+-rw-rw-rw-   0        0        0      226 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/TRG/V-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      284 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/human/TRG/V-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0      255 2024-03-24 10:26:23.000000 receptor_digger-0.7.2/src/digger/motifs/human/TRG/motif_params.json
+drwxrwxrwx   0        0        0        0 2024-05-07 10:55:37.421320 receptor_digger-0.7.2/src/digger/motifs/rhesus_macaque/
+drwxrwxrwx   0        0        0        0 2024-05-07 10:55:37.944021 receptor_digger-0.7.2/src/digger/motifs/rhesus_macaque/IGH/
+-rw-rw-rw-   0        0        0      226 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/rhesus_macaque/IGH/3'D-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      200 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/rhesus_macaque/IGH/3'D-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0      226 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/rhesus_macaque/IGH/5'D-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      284 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/rhesus_macaque/IGH/5'D-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0      220 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/rhesus_macaque/IGH/J-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      275 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/rhesus_macaque/IGH/J-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0     1799 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/rhesus_macaque/IGH/L-PART1_1_48_prob.csv
+-rw-rw-rw-   0        0        0     1815 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/rhesus_macaque/IGH/L-PART1_2_48_prob.csv
+-rw-rw-rw-   0        0        0     1811 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/rhesus_macaque/IGH/L-PART1_3_48_prob.csv
+-rw-rw-rw-   0        0        0     1815 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/rhesus_macaque/IGH/L-PART1_4_48_prob.csv
+-rw-rw-rw-   0        0        0     1699 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/rhesus_macaque/IGH/L-PART1_5_51_prob.csv
+-rw-rw-rw-   0        0        0     1288 2023-02-06 16:38:59.000000 receptor_digger-0.7.2/src/digger/motifs/rhesus_macaque/IGH/L-PART1_prob.csv
+-rw-rw-rw-   0        0        0      516 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/rhesus_macaque/IGH/L-PART2_1_17_prob.csv
+-rw-rw-rw-   0        0        0      240 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/rhesus_macaque/IGH/L-PART2_2_11_prob.csv
+-rw-rw-rw-   0        0        0      320 2023-02-06 16:38:59.000000 receptor_digger-0.7.2/src/digger/motifs/rhesus_macaque/IGH/L-PART2_prob.csv
+-rw-rw-rw-   0        0        0      220 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/rhesus_macaque/IGH/V-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      278 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/rhesus_macaque/IGH/V-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0      165 2023-04-04 14:13:25.000000 receptor_digger-0.7.2/src/digger/motifs/rhesus_macaque/IGH/conserved_motifs.fasta
+-rw-rw-rw-   0        0        0      246 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/rhesus_macaque/IGH/motif_params.json
+drwxrwxrwx   0        0        0        0 2024-05-07 10:55:37.973547 receptor_digger-0.7.2/src/digger/motifs/rhesus_macaque/IGK/
+-rw-rw-rw-   0        0        0      226 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/rhesus_macaque/IGK/J-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      284 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/rhesus_macaque/IGK/J-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0     1875 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/rhesus_macaque/IGK/L-PART1_1_57_prob.csv
+-rw-rw-rw-   0        0        0     1830 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/rhesus_macaque/IGK/L-PART1_2_51_prob.csv
+-rw-rw-rw-   0        0        0     1834 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/rhesus_macaque/IGK/L-PART1_3_51_prob.csv
+-rw-rw-rw-   0        0        0     1831 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/rhesus_macaque/IGK/L-PART1_4_51_prob.csv
+-rw-rw-rw-   0        0        0     1783 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/rhesus_macaque/IGK/L-PART1_5_51_prob.csv
+-rw-rw-rw-   0        0        0      327 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/rhesus_macaque/IGK/L-PART2_1_11_prob.csv
+-rw-rw-rw-   0        0        0      226 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/rhesus_macaque/IGK/V-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      284 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/rhesus_macaque/IGK/V-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0       90 2023-04-04 10:42:00.000000 receptor_digger-0.7.2/src/digger/motifs/rhesus_macaque/IGK/conserved_motifs.fasta
+-rw-rw-rw-   0        0        0      245 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/rhesus_macaque/IGK/motif_params.json
+drwxrwxrwx   0        0        0        0 2024-05-07 10:55:38.010557 receptor_digger-0.7.2/src/digger/motifs/rhesus_macaque/IGL/
+-rw-rw-rw-   0        0        0      226 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/rhesus_macaque/IGL/J-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      276 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/rhesus_macaque/IGL/J-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0     1253 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/rhesus_macaque/IGL/L-PART1_1_39_prob.csv
+-rw-rw-rw-   0        0        0     1347 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/rhesus_macaque/IGL/L-PART1_2_42_prob.csv
+-rw-rw-rw-   0        0        0     1476 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/rhesus_macaque/IGL/L-PART1_3_45_prob.csv
+-rw-rw-rw-   0        0        0     1783 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/rhesus_macaque/IGL/L-PART1_4_48_prob.csv
+-rw-rw-rw-   0        0        0     1792 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/rhesus_macaque/IGL/L-PART1_5_48_prob.csv
+-rw-rw-rw-   0        0        0     1767 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/rhesus_macaque/IGL/L-PART1_6_48_prob.csv
+-rw-rw-rw-   0        0        0     1800 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/rhesus_macaque/IGL/L-PART1_7_48_prob.csv
+-rw-rw-rw-   0        0        0     1629 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/rhesus_macaque/IGL/L-PART1_8_51_prob.csv
+-rw-rw-rw-   0        0        0     1817 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/rhesus_macaque/IGL/L-PART1_9_57_prob.csv
+-rw-rw-rw-   0        0        0      339 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/rhesus_macaque/IGL/L-PART2_1_11_prob.csv
+-rw-rw-rw-   0        0        0      224 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/rhesus_macaque/IGL/V-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      284 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/rhesus_macaque/IGL/V-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0       90 2023-04-04 11:10:35.000000 receptor_digger-0.7.2/src/digger/motifs/rhesus_macaque/IGL/conserved_motifs.fasta
+-rw-rw-rw-   0        0        0      245 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/motifs/rhesus_macaque/IGL/motif_params.json
+-rw-rw-rw-   0        0        0    52622 2024-04-01 09:46:16.000000 receptor_digger-0.7.2/src/digger/parse_genes.py
+-rw-rw-rw-   0        0        0    15126 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/parse_imgt_annotations.py
+-rw-rw-rw-   0        0        0    13030 2024-03-25 11:25:58.000000 receptor_digger-0.7.2/src/digger/search_motifs.py
+-rw-rw-rw-   0        0        0     2187 2024-03-24 10:26:23.000000 receptor_digger-0.7.2/src/digger/setup_motif_params.py
+-rw-rw-rw-   0        0        0      856 2023-02-06 16:38:59.000000 receptor_digger-0.7.2/src/digger/slugify.py
+drwxrwxrwx   0        0        0        0 2024-05-07 10:55:38.042549 receptor_digger-0.7.2/src/receptor_digger.egg-info/
+-rw-rw-rw-   0        0        0      936 2024-05-07 10:55:37.000000 receptor_digger-0.7.2/src/receptor_digger.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     9536 2024-05-07 10:55:37.000000 receptor_digger-0.7.2/src/receptor_digger.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 10:55:37.000000 receptor_digger-0.7.2/src/receptor_digger.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      338 2024-05-07 10:55:37.000000 receptor_digger-0.7.2/src/receptor_digger.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       55 2024-05-07 10:55:37.000000 receptor_digger-0.7.2/src/receptor_digger.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-07 10:55:37.000000 receptor_digger-0.7.2/src/receptor_digger.egg-info/top_level.txt
```

### Comparing `receptor_digger-0.7.1/MANIFEST.in` & `receptor_digger-0.7.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/PKG-INFO` & `receptor_digger-0.7.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: receptor_digger
-Version: 0.7.1
+Version: 0.7.2
 Summary: Tools for de novo discovery of genomic germline IG and TR receptor sequences
 Home-page: https://github.com/williamdlees/digger
 Author: William Lees
 Author-email: william@lees.org.uk
 Project-URL: Bug Tracker, https://github.com/williamdlees/digger/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
```

### Comparing `receptor_digger-0.7.1/setup.cfg` & `receptor_digger-0.7.2/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2072 6563 6570 746f 725f 6469 6767   = receptor_digg
 00000020: 6572 0d0a 7665 7273 696f 6e20 3d20 302e  er..version = 0.
-00000030: 372e 310d 0a61 7574 686f 7220 3d20 5769  7.1..author = Wi
+00000030: 372e 320d 0a61 7574 686f 7220 3d20 5769  7.2..author = Wi
 00000040: 6c6c 6961 6d20 4c65 6573 0d0a 6175 7468  lliam Lees..auth
 00000050: 6f72 5f65 6d61 696c 203d 2077 696c 6c69  or_email = willi
 00000060: 616d 406c 6565 732e 6f72 672e 756b 0d0a  am@lees.org.uk..
 00000070: 6465 7363 7269 7074 696f 6e20 3d20 546f  description = To
 00000080: 6f6c 7320 666f 7220 6465 206e 6f76 6f20  ols for de novo 
 00000090: 6469 7363 6f76 6572 7920 6f66 2067 656e  discovery of gen
 000000a0: 6f6d 6963 2067 6572 6d6c 696e 6520 4947  omic germline IG
@@ -31,47 +31,48 @@
 000001e0: 4920 4170 7072 6f76 6564 203a 3a20 4575  I Approved :: Eu
 000001f0: 726f 7065 616e 2055 6e69 6f6e 2050 7562  ropean Union Pub
 00000200: 6c69 6320 4c69 6365 6e63 6520 312e 3220  lic Licence 1.2 
 00000210: 2845 5550 4c20 312e 3229 0d0a 094f 7065  (EUPL 1.2)...Ope
 00000220: 7261 7469 6e67 2053 7973 7465 6d20 3a3a  rating System ::
 00000230: 204f 5320 496e 6465 7065 6e64 656e 740d   OS Independent.
 00000240: 0a0d 0a5b 6f70 7469 6f6e 735d 0d0a 7061  ...[options]..pa
-00000250: 636b 6167 6573 203d 2066 696e 643a 0d0a  ckages = find:..
-00000260: 7061 636b 6167 655f 6469 7220 3d20 0d0a  package_dir = ..
-00000270: 093d 2073 7263 0d0a 696e 636c 7564 655f  .= src..include_
-00000280: 7061 636b 6167 655f 6461 7461 203d 2054  package_data = T
-00000290: 7275 650d 0a70 7974 686f 6e5f 7265 7175  rue..python_requ
-000002a0: 6972 6573 203d 203e 3d33 2e39 0d0a 696e  ires = >=3.9..in
-000002b0: 7374 616c 6c5f 7265 7175 6972 6573 203d  stall_requires =
-000002c0: 200d 0a09 6269 6f70 7974 686f 6e3e 3d31   ...biopython>=1
-000002d0: 2e38 310d 0a09 7265 6365 7074 6f72 5f75  .81...receptor_u
-000002e0: 7469 6c73 3e3d 302e 302e 3436 0d0a 096d  tils>=0.0.46...m
-000002f0: 6174 706c 6f74 6c69 622d 7665 6e6e 0d0a  atplotlib-venn..
-00000300: 0d0a 5b6f 7074 696f 6e73 2e70 6163 6b61  ..[options.packa
-00000310: 6765 732e 6669 6e64 5d0d 0a77 6865 7265  ges.find]..where
-00000320: 203d 2073 7263 0d0a 0d0a 5b6f 7074 696f   = src....[optio
-00000330: 6e73 2e65 6e74 7279 5f70 6f69 6e74 735d  ns.entry_points]
-00000340: 0d0a 636f 6e73 6f6c 655f 7363 7269 7074  ..console_script
-00000350: 7320 3d20 0d0a 0962 6c61 7374 7265 7375  s = ...blastresu
-00000360: 6c74 735f 746f 5f63 7376 203d 2064 6967  lts_to_csv = dig
-00000370: 6765 722e 626c 6173 7472 6573 756c 7473  ger.blastresults
-00000380: 5f74 6f5f 6373 763a 6d61 696e 0d0a 0963  _to_csv:main...c
-00000390: 6f6d 7061 7265 5f61 6e6e 6f74 6174 696f  ompare_annotatio
-000003a0: 6e73 203d 2064 6967 6765 722e 636f 6d70  ns = digger.comp
-000003b0: 6172 655f 616e 6e6f 7461 7469 6f6e 733a  are_annotations:
-000003c0: 6d61 696e 0d0a 0964 6967 6765 7220 3d20  main...digger = 
-000003d0: 6469 6767 6572 2e64 6967 6765 723a 6d61  digger.digger:ma
-000003e0: 696e 0d0a 0966 696e 645f 616c 6967 6e6d  in...find_alignm
-000003f0: 656e 7473 203d 2064 6967 6765 722e 6669  ents = digger.fi
-00000400: 6e64 5f61 6c69 676e 6d65 6e74 733a 6d61  nd_alignments:ma
-00000410: 696e 0d0a 0970 6172 7365 5f69 6d67 745f  in...parse_imgt_
-00000420: 616e 6e6f 7461 7469 6f6e 7320 3d20 6469  annotations = di
-00000430: 6767 6572 2e70 6172 7365 5f69 6d67 745f  gger.parse_imgt_
-00000440: 616e 6e6f 7461 7469 6f6e 733a 6d61 696e  annotations:main
-00000450: 0d0a 0963 616c 635f 6d6f 7469 6673 203d  ...calc_motifs =
-00000460: 2064 6967 6765 722e 6361 6c63 5f6d 6f74   digger.calc_mot
-00000470: 6966 733a 6d61 696e 0d0a 0964 6967 5f73  ifs:main...dig_s
-00000480: 6571 7565 6e63 6520 3d20 6469 6767 6572  equence = digger
-00000490: 2e64 6967 5f73 6571 7565 6e63 653a 6d61  .dig_sequence:ma
-000004a0: 696e 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d  in....[egg_info]
-000004b0: 0d0a 7461 675f 6275 696c 6420 3d20 0d0a  ..tag_build = ..
-000004c0: 7461 675f 6461 7465 203d 2030 0d0a 0d0a  tag_date = 0....
+00000250: 636b 6167 6573 203d 2066 696e 645f 6e61  ckages = find_na
+00000260: 6d65 7370 6163 653a 0d0a 7061 636b 6167  mespace:..packag
+00000270: 655f 6469 7220 3d20 0d0a 093d 2073 7263  e_dir = ...= src
+00000280: 0d0a 696e 636c 7564 655f 7061 636b 6167  ..include_packag
+00000290: 655f 6461 7461 203d 2054 7275 650d 0a70  e_data = True..p
+000002a0: 7974 686f 6e5f 7265 7175 6972 6573 203d  ython_requires =
+000002b0: 203e 3d33 2e39 0d0a 696e 7374 616c 6c5f   >=3.9..install_
+000002c0: 7265 7175 6972 6573 203d 200d 0a09 6269  requires = ...bi
+000002d0: 6f70 7974 686f 6e3e 3d31 2e38 310d 0a09  opython>=1.81...
+000002e0: 7265 6365 7074 6f72 5f75 7469 6c73 3e3d  receptor_utils>=
+000002f0: 302e 302e 3436 0d0a 096d 6174 706c 6f74  0.0.46...matplot
+00000300: 6c69 622d 7665 6e6e 0d0a 0d0a 5b6f 7074  lib-venn....[opt
+00000310: 696f 6e73 2e70 6163 6b61 6765 732e 6669  ions.packages.fi
+00000320: 6e64 5d0d 0a77 6865 7265 203d 2073 7263  nd]..where = src
+00000330: 0d0a 0d0a 5b6f 7074 696f 6e73 2e65 6e74  ....[options.ent
+00000340: 7279 5f70 6f69 6e74 735d 0d0a 636f 6e73  ry_points]..cons
+00000350: 6f6c 655f 7363 7269 7074 7320 3d20 0d0a  ole_scripts = ..
+00000360: 0962 6c61 7374 7265 7375 6c74 735f 746f  .blastresults_to
+00000370: 5f63 7376 203d 2064 6967 6765 722e 626c  _csv = digger.bl
+00000380: 6173 7472 6573 756c 7473 5f74 6f5f 6373  astresults_to_cs
+00000390: 763a 6d61 696e 0d0a 0963 6f6d 7061 7265  v:main...compare
+000003a0: 5f61 6e6e 6f74 6174 696f 6e73 203d 2064  _annotations = d
+000003b0: 6967 6765 722e 636f 6d70 6172 655f 616e  igger.compare_an
+000003c0: 6e6f 7461 7469 6f6e 733a 6d61 696e 0d0a  notations:main..
+000003d0: 0964 6967 6765 7220 3d20 6469 6767 6572  .digger = digger
+000003e0: 2e64 6967 6765 723a 6d61 696e 0d0a 0966  .digger:main...f
+000003f0: 696e 645f 616c 6967 6e6d 656e 7473 203d  ind_alignments =
+00000400: 2064 6967 6765 722e 6669 6e64 5f61 6c69   digger.find_ali
+00000410: 676e 6d65 6e74 733a 6d61 696e 0d0a 0970  gnments:main...p
+00000420: 6172 7365 5f69 6d67 745f 616e 6e6f 7461  arse_imgt_annota
+00000430: 7469 6f6e 7320 3d20 6469 6767 6572 2e70  tions = digger.p
+00000440: 6172 7365 5f69 6d67 745f 616e 6e6f 7461  arse_imgt_annota
+00000450: 7469 6f6e 733a 6d61 696e 0d0a 0963 616c  tions:main...cal
+00000460: 635f 6d6f 7469 6673 203d 2064 6967 6765  c_motifs = digge
+00000470: 722e 6361 6c63 5f6d 6f74 6966 733a 6d61  r.calc_motifs:ma
+00000480: 696e 0d0a 0964 6967 5f73 6571 7565 6e63  in...dig_sequenc
+00000490: 6520 3d20 6469 6767 6572 2e64 6967 5f73  e = digger.dig_s
+000004a0: 6571 7565 6e63 653a 6d61 696e 0d0a 0d0a  equence:main....
+000004b0: 5b65 6767 5f69 6e66 6f5d 0d0a 7461 675f  [egg_info]..tag_
+000004c0: 6275 696c 6420 3d20 0d0a 7461 675f 6461  build = ..tag_da
+000004d0: 7465 203d 2030 0d0a 0d0a                 te = 0....
```

### Comparing `receptor_digger-0.7.1/src/digger/blastresults_to_csv.py` & `receptor_digger-0.7.2/src/digger/blastresults_to_csv.py`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/calc_motifs.py` & `receptor_digger-0.7.2/src/digger/calc_motifs.py`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/cirelli_contig_matches.py` & `receptor_digger-0.7.2/src/digger/cirelli_contig_matches.py`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/compare_annotations.py` & `receptor_digger-0.7.2/src/digger/compare_annotations.py`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/dig_sequence.py` & `receptor_digger-0.7.2/src/digger/dig_sequence.py`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/dig_utils.py` & `receptor_digger-0.7.2/src/digger/dig_utils.py`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/digger.py` & `receptor_digger-0.7.2/src/digger/digger.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,14 +63,18 @@
     remove_working_files()
 
     if os.path.isfile(args.output_file):
         os.remove(args.output_file)
 
     # check arguments
 
+    if not (args.v_ref or args.d_ref or args.j_ref):
+        print('Please specify at least one starting point reference set')
+        exit(1)
+
     for fn in [args.assembly_file, args.v_ref]:
         if not os.path.isfile(fn):
             print(f"{fn} - file not found")
             exit(1)
 
     if not args.motif_dir and not args.species:
         print('Error - please specify either -motif_dir or -species')
@@ -103,18 +107,14 @@
     if args.ref_comp:
         for ref_arg in args.ref_comp:
             ref_name, fn = ref_arg.split(',')
             if not os.path.isfile(fn):
                 print(f"{fn} - file not found")
                 exit(1)
 
-    if not (args.v_ref or args.d_ref or args.j_ref):
-        print('Please specify at least one starting point reference set')
-        exit(1)
-
     locus = 'IGH'
 
     if args.locus:
         if args.locus not in ['IGH', 'IGK', 'IGL', 'TRA', 'TRB', 'TRD', 'TRG']:
             print(f"locus must be one of {','.join(['IGH', 'IGK', 'IGL', 'TRA', 'TRB', 'TRD', 'TRG'])}")
             exit(1)
         locus = args.locus
@@ -211,14 +211,16 @@
             '-species', f'{args.species}',
             '-locus', locus,
             ]
 
     if args.ref_comp:
         for ref_arg in args.ref_comp:
             cmd.extend(['-ref', ref_arg])
+    else:
+        cmd.extend(['-ref', 'ref,full_germline_set.fasta'])
 
     if args.sense:
         cmd.extend(['-sense', args.sense])
 
     if args.v_ref_gapped:
         cmd.extend(['-align', args.v_ref_gapped])
```

### Comparing `receptor_digger-0.7.1/src/digger/find_alignments.py` & `receptor_digger-0.7.2/src/digger/find_alignments.py`

 * *Files 1% similar despite different names*

```diff
@@ -236,15 +236,15 @@
             if locus + 'C' not in best['subject']:
                 gene_type = locus + best['subject'].split(locus)[1][0]
             else:
                 gene_type = locus + 'C'
 
             start = best['q start']
 
-            #print('processing match to %s at %d' % (best['subject'], best['q start']))
+            # print('processing match to %s at %d' % (best['subject'], best['q start']))
 
             add_rows = True
 
             if 'V' in gene_type:
                 # don't process obviously very truncated records
                 if abs(end - start) < 250 or start < 1 or end > assembly_length:
                     continue
@@ -280,17 +280,14 @@
                             result_length = result['start'] - result['end'] + 1
 
                         # if this row overlaps with one already stored in results, keep the one that is functional
                         # if both are functional or both nonfunctional, keep the one that most closely matches a reference, if we have reference sets
                         # Otherwise keep the longer sequence
 
                         if row['start'] < row['end'] and (result['start'] <= row['start'] <= result['end'] or result['start'] <= row['end'] <= result['end']):
-                            #if row['start'] == 5087:
-                            #    breakpoint()
-
                             replace = False
 
                             if row['functional'] != 'Functional' and result['functional'] == 'Functional':
                                 replace = False
                             elif row['functional'] == 'Functional' and result['functional'] != 'Functional':
                                 replace = True
                             else:
```

### Comparing `receptor_digger-0.7.1/src/digger/motif.py` & `receptor_digger-0.7.2/src/digger/motif.py`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/motifs/human/IGH/L-PART1_1_48_prob.csv` & `receptor_digger-0.7.2/src/digger/motifs/human/IGH/L-PART1_1_48_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/motifs/human/IGH/L-PART1_2_48_prob.csv` & `receptor_digger-0.7.2/src/digger/motifs/human/IGH/L-PART1_2_48_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/motifs/human/IGH/L-PART1_3_48_prob.csv` & `receptor_digger-0.7.2/src/digger/motifs/human/IGH/L-PART1_3_48_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/motifs/human/IGH/L-PART1_4_48_prob.csv` & `receptor_digger-0.7.2/src/digger/motifs/human/IGH/L-PART1_4_48_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/motifs/human/IGH/L-PART1_5_51_prob.csv` & `receptor_digger-0.7.2/src/digger/motifs/human/IGH/L-PART1_5_51_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/motifs/human/IGH/L-PART1_6_63_prob.csv` & `receptor_digger-0.7.2/src/digger/motifs/human/IGH/L-PART1_6_63_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/motifs/human/IGK/L-PART1_1_48_prob.csv` & `receptor_digger-0.7.2/src/digger/motifs/human/IGK/L-PART1_1_48_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/motifs/human/IGK/L-PART1_2_57_prob.csv` & `receptor_digger-0.7.2/src/digger/motifs/human/IGK/L-PART1_2_57_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/motifs/human/IGK/L-PART1_3_51_prob.csv` & `receptor_digger-0.7.2/src/digger/motifs/human/IGK/L-PART1_3_51_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/motifs/human/IGK/L-PART1_4_51_prob.csv` & `receptor_digger-0.7.2/src/digger/motifs/human/IGK/L-PART1_4_51_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/motifs/human/IGK/L-PART1_5_51_prob.csv` & `receptor_digger-0.7.2/src/digger/motifs/human/IGK/L-PART1_5_51_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/motifs/human/IGK/L-PART1_6_51_prob.csv` & `receptor_digger-0.7.2/src/digger/motifs/human/IGK/L-PART1_6_51_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/motifs/human/IGK/L-PART1_prob.csv` & `receptor_digger-0.7.2/src/digger/motifs/human/IGK/L-PART1_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/motifs/human/IGL/L-PART1_1_42_prob.csv` & `receptor_digger-0.7.2/src/digger/motifs/human/IGL/L-PART1_1_42_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/motifs/human/IGL/L-PART1_2_47_prob.csv` & `receptor_digger-0.7.2/src/digger/motifs/human/IGL/L-PART1_2_47_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/motifs/human/IGL/L-PART1_3_48_prob.csv` & `receptor_digger-0.7.2/src/digger/motifs/human/IGL/L-PART1_3_48_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/motifs/human/IGL/L-PART1_4_48_prob.csv` & `receptor_digger-0.7.2/src/digger/motifs/human/IGL/L-PART1_4_48_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/motifs/human/IGL/L-PART1_5_48_prob.csv` & `receptor_digger-0.7.2/src/digger/motifs/human/IGL/L-PART1_5_48_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/motifs/human/IGL/L-PART1_6_48_prob.csv` & `receptor_digger-0.7.2/src/digger/motifs/human/IGL/L-PART1_6_48_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/motifs/human/IGL/L-PART1_7_49_prob.csv` & `receptor_digger-0.7.2/src/digger/motifs/human/IGL/L-PART1_7_49_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/motifs/human/IGL/L-PART1_8_51_prob.csv` & `receptor_digger-0.7.2/src/digger/motifs/human/IGL/L-PART1_8_51_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/motifs/human/IGL/L-PART1_9_54_prob.csv` & `receptor_digger-0.7.2/src/digger/motifs/human/IGL/L-PART1_9_54_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/motifs/human/TRA/IMGT000024_genes_lpart1.csv` & `receptor_digger-0.7.2/src/digger/motifs/human/TRA/IMGT000024_genes_lpart1.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/motifs/human/TRA/IMGT000024_genes_lpart2.csv` & `receptor_digger-0.7.2/src/digger/motifs/human/TRA/IMGT000024_genes_lpart2.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/motifs/human/TRA/L-PART1_10_51_prob.csv` & `receptor_digger-0.7.2/src/digger/motifs/human/TRA/L-PART1_10_51_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/motifs/human/TRA/L-PART1_11_51_prob.csv` & `receptor_digger-0.7.2/src/digger/motifs/human/TRA/L-PART1_11_51_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/motifs/human/TRA/L-PART1_12_51_prob.csv` & `receptor_digger-0.7.2/src/digger/motifs/human/TRA/L-PART1_12_51_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/motifs/human/TRA/L-PART1_13_51_prob.csv` & `receptor_digger-0.7.2/src/digger/motifs/human/TRA/L-PART1_13_51_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/motifs/human/TRA/L-PART1_14_54_prob.csv` & `receptor_digger-0.7.2/src/digger/motifs/human/TRA/L-PART1_14_54_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/motifs/human/TRA/L-PART1_15_54_prob.csv` & `receptor_digger-0.7.2/src/digger/motifs/human/TRA/L-PART1_15_54_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/motifs/human/TRA/L-PART1_16_54_prob.csv` & `receptor_digger-0.7.2/src/digger/motifs/human/TRA/L-PART1_16_54_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/motifs/human/TRA/L-PART1_17_54_prob.csv` & `receptor_digger-0.7.2/src/digger/motifs/human/TRA/L-PART1_17_54_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/motifs/human/TRA/L-PART1_18_57_prob.csv` & `receptor_digger-0.7.2/src/digger/motifs/human/TRA/L-PART1_18_57_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/motifs/human/TRA/L-PART1_1_42_prob.csv` & `receptor_digger-0.7.2/src/digger/motifs/human/TRA/L-PART1_1_42_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/motifs/human/TRA/L-PART1_2_42_prob.csv` & `receptor_digger-0.7.2/src/digger/motifs/human/TRA/L-PART1_2_42_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/motifs/human/TRA/L-PART1_3_45_prob.csv` & `receptor_digger-0.7.2/src/digger/motifs/human/TRA/L-PART1_3_45_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/motifs/human/TRA/L-PART1_4_45_prob.csv` & `receptor_digger-0.7.2/src/digger/motifs/human/TRA/L-PART1_4_45_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/motifs/human/TRA/L-PART1_5_45_prob.csv` & `receptor_digger-0.7.2/src/digger/motifs/human/TRA/L-PART1_5_45_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/motifs/human/TRA/L-PART1_6_48_prob.csv` & `receptor_digger-0.7.2/src/digger/motifs/human/TRA/L-PART1_6_48_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/motifs/human/TRA/L-PART1_7_48_prob.csv` & `receptor_digger-0.7.2/src/digger/motifs/human/TRA/L-PART1_7_48_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/motifs/human/TRA/L-PART1_8_48_prob.csv` & `receptor_digger-0.7.2/src/digger/motifs/human/TRA/L-PART1_8_48_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/motifs/human/TRA/L-PART1_9_48_prob.csv` & `receptor_digger-0.7.2/src/digger/motifs/human/TRA/L-PART1_9_48_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/motifs/human/TRA/L-PART2_1_32_prob.csv` & `receptor_digger-0.7.2/src/digger/motifs/human/TRA/L-PART2_1_32_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/motifs/human/TRA/L-PART2_5_26_prob.csv` & `receptor_digger-0.7.2/src/digger/motifs/human/TRA/L-PART2_5_26_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/motifs/human/TRB/L-PART1_1_36_prob.csv` & `receptor_digger-0.7.2/src/digger/motifs/human/TRB/L-PART1_1_36_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/motifs/human/TRB/L-PART1_2_81_prob.csv` & `receptor_digger-0.7.2/src/digger/motifs/human/TRB/L-PART1_2_81_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/motifs/human/TRB/L-PART1_3_51_prob.csv` & `receptor_digger-0.7.2/src/digger/motifs/human/TRB/L-PART1_3_51_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/motifs/human/TRB/L-PART1_4_51_prob.csv` & `receptor_digger-0.7.2/src/digger/motifs/human/TRB/L-PART1_4_51_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/motifs/human/TRB/L-PART1_5_51_prob.csv` & `receptor_digger-0.7.2/src/digger/motifs/human/TRB/L-PART1_5_51_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/motifs/human/TRB/L-PART1_6_51_prob.csv` & `receptor_digger-0.7.2/src/digger/motifs/human/TRB/L-PART1_6_51_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/motifs/human/TRB/L-PART1_7_52_prob.csv` & `receptor_digger-0.7.2/src/digger/motifs/human/TRB/L-PART1_7_52_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/motifs/human/TRB/L-PART1_8_60_prob.csv` & `receptor_digger-0.7.2/src/digger/motifs/human/TRB/L-PART1_8_60_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/motifs/human/TRB/L-PART1_9_63_prob.csv` & `receptor_digger-0.7.2/src/digger/motifs/human/TRB/L-PART1_9_63_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/motifs/human/TRD/L-PART1_1_48_prob.csv` & `receptor_digger-0.7.2/src/digger/motifs/human/TRD/L-PART1_1_48_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/motifs/human/TRD/L-PART1_2_51_prob.csv` & `receptor_digger-0.7.2/src/digger/motifs/human/TRD/L-PART1_2_51_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/motifs/human/TRG/L-PART1_1_48_prob.csv` & `receptor_digger-0.7.2/src/digger/motifs/human/TRG/L-PART1_1_48_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/motifs/human/TRG/L-PART1_2_45_prob.csv` & `receptor_digger-0.7.2/src/digger/motifs/human/TRG/L-PART1_2_45_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/motifs/rhesus_macaque/IGH/L-PART1_1_48_prob.csv` & `receptor_digger-0.7.2/src/digger/motifs/rhesus_macaque/IGH/L-PART1_1_48_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/motifs/rhesus_macaque/IGH/L-PART1_2_48_prob.csv` & `receptor_digger-0.7.2/src/digger/motifs/rhesus_macaque/IGH/L-PART1_2_48_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/motifs/rhesus_macaque/IGH/L-PART1_3_48_prob.csv` & `receptor_digger-0.7.2/src/digger/motifs/rhesus_macaque/IGH/L-PART1_3_48_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/motifs/rhesus_macaque/IGH/L-PART1_4_48_prob.csv` & `receptor_digger-0.7.2/src/digger/motifs/rhesus_macaque/IGH/L-PART1_4_48_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/motifs/rhesus_macaque/IGH/L-PART1_5_51_prob.csv` & `receptor_digger-0.7.2/src/digger/motifs/rhesus_macaque/IGH/L-PART1_5_51_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/motifs/rhesus_macaque/IGH/L-PART1_prob.csv` & `receptor_digger-0.7.2/src/digger/motifs/rhesus_macaque/IGH/L-PART1_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/motifs/rhesus_macaque/IGH/L-PART2_1_17_prob.csv` & `receptor_digger-0.7.2/src/digger/motifs/rhesus_macaque/IGH/L-PART2_1_17_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/motifs/rhesus_macaque/IGK/L-PART1_1_57_prob.csv` & `receptor_digger-0.7.2/src/digger/motifs/rhesus_macaque/IGK/L-PART1_1_57_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/motifs/rhesus_macaque/IGK/L-PART1_2_51_prob.csv` & `receptor_digger-0.7.2/src/digger/motifs/rhesus_macaque/IGK/L-PART1_2_51_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/motifs/rhesus_macaque/IGK/L-PART1_3_51_prob.csv` & `receptor_digger-0.7.2/src/digger/motifs/rhesus_macaque/IGK/L-PART1_3_51_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/motifs/rhesus_macaque/IGK/L-PART1_4_51_prob.csv` & `receptor_digger-0.7.2/src/digger/motifs/rhesus_macaque/IGK/L-PART1_4_51_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/motifs/rhesus_macaque/IGK/L-PART1_5_51_prob.csv` & `receptor_digger-0.7.2/src/digger/motifs/rhesus_macaque/IGK/L-PART1_5_51_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/motifs/rhesus_macaque/IGL/L-PART1_1_39_prob.csv` & `receptor_digger-0.7.2/src/digger/motifs/rhesus_macaque/IGL/L-PART1_1_39_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/motifs/rhesus_macaque/IGL/L-PART1_2_42_prob.csv` & `receptor_digger-0.7.2/src/digger/motifs/rhesus_macaque/IGL/L-PART1_2_42_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/motifs/rhesus_macaque/IGL/L-PART1_3_45_prob.csv` & `receptor_digger-0.7.2/src/digger/motifs/rhesus_macaque/IGL/L-PART1_3_45_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/motifs/rhesus_macaque/IGL/L-PART1_4_48_prob.csv` & `receptor_digger-0.7.2/src/digger/motifs/rhesus_macaque/IGL/L-PART1_4_48_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/motifs/rhesus_macaque/IGL/L-PART1_5_48_prob.csv` & `receptor_digger-0.7.2/src/digger/motifs/rhesus_macaque/IGL/L-PART1_5_48_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/motifs/rhesus_macaque/IGL/L-PART1_6_48_prob.csv` & `receptor_digger-0.7.2/src/digger/motifs/rhesus_macaque/IGL/L-PART1_6_48_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/motifs/rhesus_macaque/IGL/L-PART1_7_48_prob.csv` & `receptor_digger-0.7.2/src/digger/motifs/rhesus_macaque/IGL/L-PART1_7_48_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/motifs/rhesus_macaque/IGL/L-PART1_8_51_prob.csv` & `receptor_digger-0.7.2/src/digger/motifs/rhesus_macaque/IGL/L-PART1_8_51_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/motifs/rhesus_macaque/IGL/L-PART1_9_57_prob.csv` & `receptor_digger-0.7.2/src/digger/motifs/rhesus_macaque/IGL/L-PART1_9_57_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/parse_genes.py` & `receptor_digger-0.7.2/src/digger/parse_genes.py`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/parse_imgt_annotations.py` & `receptor_digger-0.7.2/src/digger/parse_imgt_annotations.py`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/search_motifs.py` & `receptor_digger-0.7.2/src/digger/search_motifs.py`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/setup_motif_params.py` & `receptor_digger-0.7.2/src/digger/setup_motif_params.py`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/digger/slugify.py` & `receptor_digger-0.7.2/src/digger/slugify.py`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.7.1/src/receptor_digger.egg-info/PKG-INFO` & `receptor_digger-0.7.2/src/receptor_digger.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: receptor_digger
-Version: 0.7.1
+Version: 0.7.2
 Summary: Tools for de novo discovery of genomic germline IG and TR receptor sequences
 Home-page: https://github.com/williamdlees/digger
 Author: William Lees
 Author-email: william@lees.org.uk
 Project-URL: Bug Tracker, https://github.com/williamdlees/digger/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
```

### Comparing `receptor_digger-0.7.1/src/receptor_digger.egg-info/SOURCES.txt` & `receptor_digger-0.7.2/src/receptor_digger.egg-info/SOURCES.txt`

 * *Files identical despite different names*

