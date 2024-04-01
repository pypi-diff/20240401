# Comparing `tmp/cgat-0.6.5.tar.gz` & `tmp/cgat-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cgat-0.6.5.tar", last modified: Wed Nov 24 14:58:33 2021, max compression
+gzip compressed data, was "cgat-0.7.0.tar", last modified: Mon Apr  1 21:18:17 2024, max compression
```

## Comparing `cgat-0.6.5.tar` & `cgat-0.7.0.tar`

### file list

```diff
@@ -1,189 +1,174 @@
-drwxr-xr-x   0 adamcribbs   (501) staff       (20)        0 2021-11-24 14:58:33.670501 cgat-0.6.5/
--rw-r--r--   0 adamcribbs   (501) staff       (20)     1188 2021-07-21 21:50:52.000000 cgat-0.6.5/LICENSE
--rw-r--r--   0 adamcribbs   (501) staff       (20)      680 2021-07-21 21:50:52.000000 cgat-0.6.5/MANIFEST.in
--rw-r--r--   0 adamcribbs   (501) staff       (20)      751 2021-11-24 14:58:33.670257 cgat-0.6.5/PKG-INFO
--rw-r--r--   0 adamcribbs   (501) staff       (20)     2721 2021-07-21 21:50:52.000000 cgat-0.6.5/README.md
--rw-r--r--   0 adamcribbs   (501) staff       (20)      734 2021-07-21 21:50:52.000000 cgat-0.6.5/THANKS.txt
-drwxr-xr-x   0 adamcribbs   (501) staff       (20)        0 2021-11-24 14:58:33.641976 cgat-0.6.5/cgat/
--rw-r--r--   0 adamcribbs   (501) staff       (20)     2378 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/AGP.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     2018 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/AString.py
-drwxr-xr-x   0 adamcribbs   (501) staff       (20)        0 2021-11-24 14:58:33.643506 cgat-0.6.5/cgat/BamTools/
--rw-r--r--   0 adamcribbs   (501) staff       (20)    84081 2021-11-24 14:57:56.000000 cgat-0.6.5/cgat/BamTools/bamtools.pyx
--rw-r--r--   0 adamcribbs   (501) staff       (20)    73635 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/BamTools/geneprofile.pyx
--rw-r--r--   0 adamcribbs   (501) staff       (20)    13452 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/BamTools/peakshape.pyx
--rw-r--r--   0 adamcribbs   (501) staff       (20)    17233 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/Bed.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)    28840 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/Blat.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)    39690 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/CBioPortal.py
-drwxr-xr-x   0 adamcribbs   (501) staff       (20)        0 2021-11-24 14:58:33.643985 cgat-0.6.5/cgat/Components/
--rw-r--r--   0 adamcribbs   (501) staff       (20)     4766 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/Components/Components.pyx
--rw-r--r--   0 adamcribbs   (501) staff       (20)     3847 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/Components/connected_components.cpp
--rw-r--r--   0 adamcribbs   (501) staff       (20)     1734 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/Components/connected_components.h
--rw-r--r--   0 adamcribbs   (501) staff       (20)     3878 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/FastaIterator.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)    12895 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/Fastq.py
-drwxr-xr-x   0 adamcribbs   (501) staff       (20)        0 2021-11-24 14:58:33.644136 cgat-0.6.5/cgat/FastqTools/
--rw-r--r--   0 adamcribbs   (501) staff       (20)     3528 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/FastqTools/fastqtools.pyx
--rw-r--r--   0 adamcribbs   (501) staff       (20)     3108 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/GFF3.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)    31953 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/GTF.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)   185296 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/GeneModelAnalysis.pyx
--rw-r--r--   0 adamcribbs   (501) staff       (20)    49911 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/Genomics.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     1053 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/Glam2.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     1492 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/Glam2Scan.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)    19547 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/Histogram.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     1395 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/Histogram2D.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     4581 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/IGV.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)    41390 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/IndexedFasta.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     4570 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/IndexedGenome.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)    11505 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/Intervals.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     1756 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/Iterators.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     5499 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/MEME.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     7369 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/Masker.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)    12147 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/MatrixTools.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     2312 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/Motifs.py
-drwxr-xr-x   0 adamcribbs   (501) staff       (20)        0 2021-11-24 14:58:33.645164 cgat-0.6.5/cgat/NCL/
--rw-r--r--   0 adamcribbs   (501) staff       (20)     5656 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/NCL/__init__.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     4148 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/NCL/_cnestedlist.pxd
--rw-r--r--   0 adamcribbs   (501) staff       (20)    19606 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/NCL/cnestedlist.pyx
--rw-r--r--   0 adamcribbs   (501) staff       (20)     3933 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/NCL/default.h
--rw-r--r--   0 adamcribbs   (501) staff       (20)    32028 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/NCL/intervaldb.c
--rw-r--r--   0 adamcribbs   (501) staff       (20)     4921 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/NCL/intervaldb.h
--rw-r--r--   0 adamcribbs   (501) staff       (20)     1563 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/RLE.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     5705 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/RateEstimation.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)    36488 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/SVGdraw.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     8356 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/SequencePairProperties.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)    40104 2021-11-24 14:57:56.000000 cgat-0.6.5/cgat/SequenceProperties.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     6139 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/SetTools.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     7596 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/Sra.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)    34490 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/Stats.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)    20140 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/Tree.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)    44920 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/TreeTools.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     3137 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/VCF.py
-drwxr-xr-x   0 adamcribbs   (501) staff       (20)        0 2021-11-24 14:58:33.645326 cgat-0.6.5/cgat/VCFTools/
--rw-r--r--   0 adamcribbs   (501) staff       (20)    25310 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/VCFTools/vcftools.pyx
--rw-r--r--   0 adamcribbs   (501) staff       (20)    19027 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/Variants.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)   107936 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/WrapperCodeML.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)        0 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/__init__.py
--rwxr-xr-x   0 adamcribbs   (501) staff       (20)     3480 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/cgat.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)    28781 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/dictzip.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     7542 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/makeGeneset.py
-drwxr-xr-x   0 adamcribbs   (501) staff       (20)        0 2021-11-24 14:58:33.669910 cgat-0.6.5/cgat/tools/
--rw-r--r--   0 adamcribbs   (501) staff       (20)        0 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/tools/__init__.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     4332 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/tools/bam2UniquePairs.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)    25343 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/tools/bam2bam.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     1895 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/tools/bam2bam_split_reads.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     6227 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/tools/bam2bed.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     3410 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/tools/bam2depth.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)    16746 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/tools/bam2fasta.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     4895 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/tools/bam2fastq.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)    38204 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/tools/bam2geneprofile.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     4716 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/tools/bam2libtype.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)    22958 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/tools/bam2peakshape.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)    37840 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/tools/bam2stats.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)    16966 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/tools/bam2wiggle.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     2502 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/tools/bam2window_stats.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     9672 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/tools/bam_compare_alignments.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     9070 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/tools/bam_pileup2tsv.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     3866 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/tools/bam_vs_bam.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     8170 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/tools/bam_vs_bed.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     9174 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/tools/bam_vs_gtf.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     8328 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/tools/bams2bam.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     3208 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/tools/bcl2fastq.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     5283 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/tools/bed2annotator.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)    22414 2021-11-24 14:57:56.000000 cgat-0.6.5/cgat/tools/bed2bed.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     5688 2021-11-24 14:57:56.000000 cgat-0.6.5/cgat/tools/bed2fasta.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     4029 2021-11-24 14:57:56.000000 cgat-0.6.5/cgat/tools/bed2gff.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     2181 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/tools/bed2graph.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     7537 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/tools/bed2plot.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     5363 2021-11-24 14:57:56.000000 cgat-0.6.5/cgat/tools/bed2stats.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)    24191 2021-11-24 14:57:56.000000 cgat-0.6.5/cgat/tools/bed2table.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     4857 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/tools/bed_vs_bed.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)    10208 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/tools/beds2beds.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     4295 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/tools/beds2counts.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     1605 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/tools/cat_tables.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)    10672 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/tools/cgat2dot.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)    25196 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/tools/cgat2rdf.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     1611 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/tools/cgat_fasta2cDNA.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     5393 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/tools/cgat_get_options.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     2586 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/tools/cgat_rebuild_extensions.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     1033 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/tools/cgat_script_template.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     4384 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/tools/chain2psl.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)      720 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/tools/combine_tables.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     1470 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/tools/csv2csv.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)      826 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/tools/csv2db.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     4535 2021-11-24 14:57:56.000000 cgat-0.6.5/cgat/tools/csv_cut.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     2882 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/tools/csv_intersection.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     2173 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/tools/csv_rename.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     3010 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/tools/csv_select.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     3975 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/tools/csv_set.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)    10096 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/tools/csvs2csv.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     9275 2021-11-24 14:57:56.000000 cgat-0.6.5/cgat/tools/data2histogram.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     7781 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/tools/diff_bam.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)    11700 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/tools/diff_bed.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)    15078 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/tools/diff_chains.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     9500 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/tools/diff_fasta.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)    14424 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/tools/diff_gtf.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     6238 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/tools/extract_stats.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)    10207 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/tools/fasta2bed.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)    21392 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/tools/fasta2fasta.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)    14562 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/tools/fasta2fastq.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     5500 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/tools/fasta2kmercontent.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     2682 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/tools/fasta2stats.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)    12477 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/tools/fasta2table.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     3771 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/tools/fasta2variants.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     2536 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/tools/fasta2vcf.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     2281 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/tools/fastas2fasta.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     1884 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/tools/fastq2fasta.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)    17342 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/tools/fastq2fastq.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     5343 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/tools/fastq2summary.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     6364 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/tools/fastq2table.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)    12133 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/tools/fastq2tpm.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     1337 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/tools/fastq2tsv.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     5041 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/tools/fastqs2fasta.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     3534 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/tools/fastqs2fastq.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     9491 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/tools/fastqs2fastqs.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     2597 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/tools/genome_bed.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     5443 2021-11-24 14:57:56.000000 cgat-0.6.5/cgat/tools/gff2bed.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)    11034 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/tools/gff2coverage.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)    14023 2021-11-24 14:57:56.000000 cgat-0.6.5/cgat/tools/gff2fasta.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)    30534 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/tools/gff2gff.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     9967 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/tools/gff2histogram.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     4265 2021-11-24 14:57:56.000000 cgat-0.6.5/cgat/tools/gff2psl.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     7200 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/tools/gff2stats.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)    14982 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/tools/gff2table.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)    12848 2021-11-24 14:57:56.000000 cgat-0.6.5/cgat/tools/gff32gtf.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)    18199 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/tools/gtf2fasta.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)    40355 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/tools/gtf2gff.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)    52205 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/tools/gtf2gtf.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)    39563 2021-11-24 14:57:56.000000 cgat-0.6.5/cgat/tools/gtf2table.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)    11698 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/tools/gtf2tsv.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)    11190 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/tools/gtfs2tsv.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     4123 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/tools/index2bed.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)    12772 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/tools/index_fasta.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     8116 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/tools/medip_merge_intervals.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     1464 2021-11-24 14:57:56.000000 cgat-0.6.5/cgat/tools/randomize_lines.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     6507 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/tools/rnaseq_junction_bam2bam.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     6509 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/tools/split_fasta.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     7956 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/tools/split_file.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     4570 2021-11-24 14:57:56.000000 cgat-0.6.5/cgat/tools/split_gff.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     3071 2021-11-24 14:57:56.000000 cgat-0.6.5/cgat/tools/table2stats.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     2346 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/tools/table2table.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     9522 2021-11-24 14:57:56.000000 cgat-0.6.5/cgat/tools/tables2table.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     3088 2021-11-24 14:57:56.000000 cgat-0.6.5/cgat/tools/transfac2transfac.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)    11183 2021-11-24 14:57:56.000000 cgat-0.6.5/cgat/tools/vcf2tsv.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)    14736 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/tools/vcf2vcf.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     8970 2021-11-24 14:57:56.000000 cgat-0.6.5/cgat/tools/vcf_compare_phase.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     6901 2021-11-24 14:57:56.000000 cgat-0.6.5/cgat/tools/vcf_stats.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     3447 2021-11-24 14:57:56.000000 cgat-0.6.5/cgat/tools/vcf_vs_vcf.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     6581 2021-07-21 21:50:52.000000 cgat-0.6.5/cgat/tools/vcfstats2db.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)     6204 2021-11-24 14:57:56.000000 cgat-0.6.5/cgat/tools/wig2bed.py
--rw-r--r--   0 adamcribbs   (501) staff       (20)       22 2021-11-24 14:57:56.000000 cgat-0.6.5/cgat/version.py
-drwxr-xr-x   0 adamcribbs   (501) staff       (20)        0 2021-11-24 14:58:33.642713 cgat-0.6.5/cgat.egg-info/
--rw-r--r--   0 adamcribbs   (501) staff       (20)      751 2021-11-24 14:58:33.000000 cgat-0.6.5/cgat.egg-info/PKG-INFO
--rw-r--r--   0 adamcribbs   (501) staff       (20)     4163 2021-11-24 14:58:33.000000 cgat-0.6.5/cgat.egg-info/SOURCES.txt
--rw-r--r--   0 adamcribbs   (501) staff       (20)        1 2021-11-24 14:58:33.000000 cgat-0.6.5/cgat.egg-info/dependency_links.txt
--rw-r--r--   0 adamcribbs   (501) staff       (20)       41 2021-11-24 14:58:33.000000 cgat-0.6.5/cgat.egg-info/entry_points.txt
--rw-r--r--   0 adamcribbs   (501) staff       (20)        1 2021-11-24 14:58:33.000000 cgat-0.6.5/cgat.egg-info/not-zip-safe
--rw-r--r--   0 adamcribbs   (501) staff       (20)        5 2021-11-24 14:58:33.000000 cgat-0.6.5/cgat.egg-info/top_level.txt
--rwxr-xr-x   0 adamcribbs   (501) staff       (20)    26056 2021-07-21 21:50:52.000000 cgat-0.6.5/install.sh
--rw-r--r--   0 adamcribbs   (501) staff       (20)        0 2021-11-24 14:57:56.000000 cgat-0.6.5/requires.txt
--rw-r--r--   0 adamcribbs   (501) staff       (20)       38 2021-11-24 14:58:33.670553 cgat-0.6.5/setup.cfg
--rw-r--r--   0 adamcribbs   (501) staff       (20)    10750 2021-11-24 14:57:56.000000 cgat-0.6.5/setup.py
+drwxrwxr-x   0 caeruleus  (1000) caeruleus  (1000)        0 2024-04-01 21:18:17.087669 cgat-0.7.0/
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     1273 2024-04-01 08:10:13.000000 cgat-0.7.0/COPYING
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     1188 2024-04-01 08:10:13.000000 cgat-0.7.0/LICENSE
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)      680 2024-04-01 08:10:13.000000 cgat-0.7.0/MANIFEST.in
+-rw-r--r--   0 caeruleus  (1000) caeruleus  (1000)      783 2024-04-01 21:18:17.087669 cgat-0.7.0/PKG-INFO
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     2721 2024-04-01 08:10:13.000000 cgat-0.7.0/README.md
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)      734 2024-04-01 08:10:13.000000 cgat-0.7.0/THANKS.txt
+drwxrwxr-x   0 caeruleus  (1000) caeruleus  (1000)        0 2024-04-01 21:18:17.075668 cgat-0.7.0/cgat/
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     2378 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/AGP.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     2016 2024-04-01 20:22:36.000000 cgat-0.7.0/cgat/AString.py
+drwxrwxr-x   0 caeruleus  (1000) caeruleus  (1000)        0 2024-04-01 21:18:17.079668 cgat-0.7.0/cgat/BamTools/
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    84091 2024-04-01 19:44:25.000000 cgat-0.7.0/cgat/BamTools/bamtools.pyx
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    73647 2024-04-01 12:48:18.000000 cgat-0.7.0/cgat/BamTools/geneprofile.pyx
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    13457 2024-04-01 12:48:18.000000 cgat-0.7.0/cgat/BamTools/peakshape.pyx
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    17233 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/Bed.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    28840 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/Blat.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    39690 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/CBioPortal.py
+drwxrwxr-x   0 caeruleus  (1000) caeruleus  (1000)        0 2024-04-01 21:18:17.079668 cgat-0.7.0/cgat/Components/
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     4766 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/Components/Components.pyx
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     3847 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/Components/connected_components.cpp
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     1734 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/Components/connected_components.h
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     3878 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/FastaIterator.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    12895 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/Fastq.py
+drwxrwxr-x   0 caeruleus  (1000) caeruleus  (1000)        0 2024-04-01 21:18:17.079668 cgat-0.7.0/cgat/FastqTools/
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     3528 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/FastqTools/fastqtools.pyx
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     3108 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/GFF3.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    31953 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/GTF.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)   185318 2024-04-01 12:48:18.000000 cgat-0.7.0/cgat/GeneModelAnalysis.pyx
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    49913 2024-04-01 12:48:18.000000 cgat-0.7.0/cgat/Genomics.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     1053 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/Glam2.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     1492 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/Glam2Scan.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    19547 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/Histogram.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     1395 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/Histogram2D.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     4581 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/IGV.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    41375 2024-04-01 20:17:59.000000 cgat-0.7.0/cgat/IndexedFasta.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     4570 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/IndexedGenome.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    11505 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/Intervals.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     1756 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/Iterators.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     5499 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/MEME.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     7369 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/Masker.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    12153 2024-04-01 12:48:18.000000 cgat-0.7.0/cgat/MatrixTools.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     2312 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/Motifs.py
+drwxrwxr-x   0 caeruleus  (1000) caeruleus  (1000)        0 2024-04-01 21:18:17.079668 cgat-0.7.0/cgat/NCL/
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     5656 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/NCL/__init__.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     4148 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/NCL/_cnestedlist.pxd
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    19606 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/NCL/cnestedlist.pyx
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     3933 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/NCL/default.h
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    32028 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/NCL/intervaldb.c
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     4921 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/NCL/intervaldb.h
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     1563 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/RLE.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     5705 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/RateEstimation.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    36488 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/SVGdraw.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    40103 2024-04-01 15:50:46.000000 cgat-0.7.0/cgat/SequenceProperties.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     6141 2024-04-01 12:48:18.000000 cgat-0.7.0/cgat/SetTools.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     7596 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/Sra.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    34513 2024-04-01 18:24:35.000000 cgat-0.7.0/cgat/Stats.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    20140 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/Tree.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    44920 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/TreeTools.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     3137 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/VCF.py
+drwxrwxr-x   0 caeruleus  (1000) caeruleus  (1000)        0 2024-04-01 21:18:17.079668 cgat-0.7.0/cgat/VCFTools/
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    25310 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/VCFTools/vcftools.pyx
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    19027 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/Variants.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)        0 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/__init__.py
+-rwxrwxr-x   0 caeruleus  (1000) caeruleus  (1000)     3480 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/cgat.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    28781 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/dictzip.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     7542 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/makeGeneset.py
+drwxrwxr-x   0 caeruleus  (1000) caeruleus  (1000)        0 2024-04-01 21:18:17.087669 cgat-0.7.0/cgat/tools/
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)        0 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/__init__.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    25343 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/bam2bam.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     1895 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/bam2bam_split_reads.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     6227 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/bam2bed.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     3410 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/bam2depth.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    16746 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/bam2fasta.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     4895 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/bam2fastq.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    38204 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/bam2geneprofile.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    37840 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/bam2stats.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    16966 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/bam2wiggle.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     2502 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/bam2window_stats.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     9672 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/bam_compare_alignments.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     9070 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/bam_pileup2tsv.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     3866 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/bam_vs_bam.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     8170 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/bam_vs_bed.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     9174 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/bam_vs_gtf.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     8328 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/bams2bam.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     3208 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/bcl2fastq.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    22414 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/bed2bed.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     5688 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/bed2fasta.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     4029 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/bed2gff.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     2181 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/bed2graph.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     5363 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/bed2stats.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    24191 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/bed2table.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     4857 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/bed_vs_bed.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    10208 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/beds2beds.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     4295 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/beds2counts.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    10672 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/cgat2dot.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     5393 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/cgat_get_options.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     2586 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/cgat_rebuild_extensions.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     1033 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/cgat_script_template.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     1470 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/csv2csv.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    10096 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/csvs2csv.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     9275 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/data2histogram.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     7781 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/diff_bam.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    11704 2024-04-01 12:48:18.000000 cgat-0.7.0/cgat/tools/diff_bed.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    15078 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/diff_chains.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     9500 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/diff_fasta.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    14426 2024-04-01 12:48:18.000000 cgat-0.7.0/cgat/tools/diff_gtf.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     6238 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/extract_stats.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    10207 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/fasta2bed.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    21393 2024-04-01 12:48:18.000000 cgat-0.7.0/cgat/tools/fasta2fasta.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    14562 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/fasta2fastq.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     5500 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/fasta2kmercontent.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     2682 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/fasta2stats.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    12477 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/fasta2table.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     3771 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/fasta2variants.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     2536 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/fasta2vcf.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     2281 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/fastas2fasta.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     1884 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/fastq2fasta.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    17342 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/fastq2fastq.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     5343 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/fastq2summary.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     6364 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/fastq2table.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    12133 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/fastq2tpm.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     1337 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/fastq2tsv.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     5041 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/fastqs2fasta.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     3534 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/fastqs2fastq.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     9491 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/fastqs2fastqs.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     2597 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/genome_bed.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     5443 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/gff2bed.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    11034 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/gff2coverage.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    14023 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/gff2fasta.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    30534 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/gff2gff.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     9967 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/gff2histogram.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     4265 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/gff2psl.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     7200 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/gff2stats.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    14982 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/gff2table.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    12848 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/gff32gtf.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    18122 2024-04-01 20:23:32.000000 cgat-0.7.0/cgat/tools/gtf2fasta.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    40355 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/gtf2gff.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    52205 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/gtf2gtf.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    39563 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/gtf2table.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    11698 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/gtf2tsv.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    11190 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/gtfs2tsv.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     4123 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/index2bed.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    12771 2024-04-01 13:26:07.000000 cgat-0.7.0/cgat/tools/index_fasta.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     6509 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/split_fasta.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     7956 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/split_file.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     4570 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/split_gff.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     3071 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/table2stats.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     2346 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/table2table.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     9522 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/tables2table.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    11183 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/vcf2tsv.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    14736 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/vcf2vcf.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     8970 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/vcf_compare_phase.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     6901 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/vcf_stats.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     3447 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/vcf_vs_vcf.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     6581 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/vcfstats2db.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     6204 2024-04-01 08:10:13.000000 cgat-0.7.0/cgat/tools/wig2bed.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)       22 2024-04-01 20:35:56.000000 cgat-0.7.0/cgat/version.py
+drwxrwxr-x   0 caeruleus  (1000) caeruleus  (1000)        0 2024-04-01 21:18:17.087669 cgat-0.7.0/cgat.egg-info/
+-rw-r--r--   0 caeruleus  (1000) caeruleus  (1000)      783 2024-04-01 21:18:17.000000 cgat-0.7.0/cgat.egg-info/PKG-INFO
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     3683 2024-04-01 21:18:17.000000 cgat-0.7.0/cgat.egg-info/SOURCES.txt
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)        1 2024-04-01 21:18:17.000000 cgat-0.7.0/cgat.egg-info/dependency_links.txt
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)       40 2024-04-01 21:18:17.000000 cgat-0.7.0/cgat.egg-info/entry_points.txt
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)        1 2024-04-01 08:12:17.000000 cgat-0.7.0/cgat.egg-info/not-zip-safe
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)        5 2024-04-01 21:18:17.000000 cgat-0.7.0/cgat.egg-info/top_level.txt
+-rwxrwxr-x   0 caeruleus  (1000) caeruleus  (1000)    26056 2024-04-01 08:10:13.000000 cgat-0.7.0/install.sh
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)        0 2024-04-01 08:10:13.000000 cgat-0.7.0/requires.txt
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)       38 2024-04-01 21:18:17.087669 cgat-0.7.0/setup.cfg
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    10750 2024-04-01 08:10:13.000000 cgat-0.7.0/setup.py
+drwxrwxr-x   0 caeruleus  (1000) caeruleus  (1000)        0 2024-04-01 21:18:17.087669 cgat-0.7.0/tests/
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)      795 2024-04-01 08:10:14.000000 cgat-0.7.0/tests/testComponents.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     6974 2024-04-01 08:10:14.000000 cgat-0.7.0/tests/test_commandline.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     3267 2024-04-01 08:10:14.000000 cgat-0.7.0/tests/test_import.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)    11530 2024-04-01 08:10:14.000000 cgat-0.7.0/tests/test_scripts.py
+-rw-rw-r--   0 caeruleus  (1000) caeruleus  (1000)     2277 2024-04-01 08:10:14.000000 cgat-0.7.0/tests/test_style.py
```

### Comparing `cgat-0.6.5/LICENSE` & `cgat-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/MANIFEST.in` & `cgat-0.7.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/PKG-INFO` & `cgat-0.7.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,24 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: cgat
-Version: 0.6.5
+Version: 0.7.0
 Summary: cgat : the Computational Genomics Analysis Toolkit
 Home-page: http://www.cgat.org/cgat/Tools/
 Author: Andreas Heger
 Author-email: andreas.heger@gmail.com
 License: MIT
-Description: cgat : the Computational Genomics Analysis Toolkit
 Keywords: computational genomics
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
+License-File: LICENSE
+License-File: COPYING
+
+cgat : the Computational Genomics Analysis Toolkit
```

### Comparing `cgat-0.6.5/README.md` & `cgat-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/THANKS.txt` & `cgat-0.7.0/THANKS.txt`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/AGP.py` & `cgat-0.7.0/cgat/AGP.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/AString.py` & `cgat-0.7.0/cgat/AString.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,22 +51,22 @@
         else:
             return AString(str(self).lower())
 
     def __getitem__(self, *args):
         """return slice as a string."""
 
         if IS_PY3:
-            return array.__getitem__(self, *args).tostring().decode("ascii")
+            return array.__getitem__(self, *args).tobytes().decode("ascii")
         else:
             return array.__getitem__(self, *args).tostring()
 
     def __setitem__(self, start, end, sub):
         """set slice start:end from a string sub."""
         return array.__setitem__(self,
                                  start, end,
                                  array("b", sub))
 
     def __str__(self):
         if IS_PY3:
-            return self.tostring().decode("ascii")
+            return self.tobytes().decode("ascii")
         else:
             return self.tostring()
```

### Comparing `cgat-0.6.5/cgat/BamTools/bamtools.pyx` & `cgat-0.7.0/cgat/BamTools/bamtools.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -274,15 +274,15 @@
             md5 = hashlib.md5(read_name).digest()[:hash_size]
             if md5 not in reads:
                 reads[md5] = fastq_nreads
                 fastq_nreads += 1
                 if outfile_readmap:
                     outfile_readmap.write("{}\t{}\n".format(
                         read_name,
-                        base64.encodestring(md5)[:-1]))
+                        base64.encodebytes(md5)[:-1]))
 
         samfile.seek(old_pos)
         nalignments = iteration
     else:
         count_fastq = False
         E.info("simple counting only")
 
@@ -662,20 +662,20 @@
         counter.total_read2 = fastq_nreads
         counter.total_read2_is_mapped_uniq = total_read2_is_mapped_uniquely
         counter.total_read2_is_mmap = total_read2_is_mapped_multiply
         counter.total_read2_is_mapped = counter.total_read2_is_mapped_uniq + counter.total_read2_is_mmap
         counter.total_read2_is_unmapped = total_read2_is_unmapped
         counter.total_read2_is_missing = total_read2_is_missing
 
-        substitution_rates = numpy.zeros(fastq_nreads, dtype=numpy.float)
-        insertion_rates = numpy.zeros(fastq_nreads, dtype=numpy.float)
-        deletion_rates = numpy.zeros(fastq_nreads, dtype=numpy.float)
-        error_rates = numpy.zeros(fastq_nreads, dtype=numpy.float)
-        coverages = numpy.zeros(fastq_nreads, dtype=numpy.float)
-        mask = numpy.ones(fastq_nreads, dtype=numpy.int)
+        substitution_rates = numpy.zeros(fastq_nreads, dtype=numpy.float64)
+        insertion_rates = numpy.zeros(fastq_nreads, dtype=numpy.float64)
+        deletion_rates = numpy.zeros(fastq_nreads, dtype=numpy.float64)
+        error_rates = numpy.zeros(fastq_nreads, dtype=numpy.float64)
+        coverages = numpy.zeros(fastq_nreads, dtype=numpy.float64)
+        mask = numpy.ones(fastq_nreads, dtype=numpy.int64)
 
         if outfile_details:
             header = ["read_md5",
                       "read_length",
                       "alignments",
                       "mean_quality",
                       "median_quality",
@@ -707,15 +707,15 @@
             if outfile_details != sys.stdout:
                 # later: get access FILE * object
                 outfile_details.write("\t".join(header) + "\n")
                 for qname, read_index in reads.items():
                     fastq_count = &fastq_counts[read_index]
                     # remove "\n" from base64 encoded md5
                     outfile_details.write("%s\t%s" % (
-                        base64.encodestring(qname)[:-1].decode("ascii"),
+                        base64.encodebytes(qname)[:-1].decode("ascii"),
                         "\t".join( \
                                    map(str,
                                        (fastq_count.read_length,
                                         fastq_count.alignments,
                                         "{:5.2f}".format(fastq_count.mean_quality / 1000.0),
                                         "{:5.2f}".format(fastq_count.median_quality / 1000.0),
                                         fastq_count.is_unmapped,
@@ -1554,27 +1554,27 @@
     else:
         itr = samfile.fetch()
 
     cdef uint32_t total_length = sum(lengths) + _window_size * len(lengths)
     cdef uint32_t ncontigs = len(contigs)
     cdef int ncolumns = len(columns)
     cdef numpy.ndarray offsets = numpy.zeros(
-        ncontigs + 1, dtype=numpy.int32)
+        ncontigs + 1, dtype=numpy.int64)
 
     for idx, length in enumerate(lengths):
         offsets[idx] = offset
         if length > 0:
             offset += (length + _window_size) // _window_size
 
     cdef uint32_t total_windows = offset
     offsets[idx + 1] = offset
 
     cdef numpy.ndarray window_counts = numpy.zeros(
         (total_windows, ncolumns),
-        dtype=numpy.int32)
+        dtype=numpy.int64)
 
     cdef int32_t [:, :] window_counts_view = window_counts
 
     E.debug("total_windows={}, total_length={}, nflags={}, ncolumns={}, ncontigs={}".format(
             total_windows, total_length, nflags, ncolumns, ncontigs))
 
     E.info("computing read counts in windows")
```

### Comparing `cgat-0.6.5/cgat/BamTools/geneprofile.pyx` & `cgat-0.7.0/cgat/BamTools/geneprofile.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -556,17 +556,17 @@
 
         '''
         self.counts.append(0)
         self.lengths.append([])
         self.fields.append(field)
         self.nbins.append(length)
         if self.normalization in ("max", "sum", "total-max", "total-sum"):
-            self.dtype = numpy.float
+            self.dtype = numpy.float64
         else:
-            self.dtype = numpy.int
+            self.dtype = numpy.int64
         self.aggregate_counts.append(numpy.zeros(length, dtype=self.dtype))
 
     def setOutputProfiles(self, outfile_profiles):
         if outfile_profiles:
             self.outfile_profiles = outfile_profiles
             sum_counts = sum([len(x) for x in self.aggregate_counts])
             self.outfile_profiles.write(
@@ -580,18 +580,18 @@
         if self.outfile_profiles:
             self.outfile_profiles.close()
 
     def setNormalization( self, normalization ):
         self.normalization = normalization
 
         if self.normalization in ("max", "sum", "total-max", "total-sum" ):
-            self.dtype = numpy.float
+            self.dtype = numpy.float64
             self.format = "%6.4f"
         else:
-            self.dtype = numpy.int
+            self.dtype = numpy.int64
             self.format = "%i"
 
         for x,c in enumerate(self.aggregate_counts):
             self.aggregate_counts[x] = numpy.zeros( len(c), dtype = self.dtype )
 
     def addName( self, name ):
         '''record name currently being processed.'''
@@ -667,15 +667,15 @@
 
         '''
         if normalize is None or normalize == "none":
             profile = numpy.concatenate(self.aggregate_counts)
 
         elif normalize in ("area", "background"):
             profile = numpy.concatenate(self.aggregate_counts)
-            profile = numpy.array(profile, dtype=numpy.float)
+            profile = numpy.array(profile, dtype=numpy.float64)
 
             if normalize == "area":
                 background = profile.sum()
 
             elif normalize == "background":
                 # take counts at either end of profile
                 background_counts = numpy.concatenate(
@@ -684,15 +684,15 @@
                 # compute mean()
                 background = numpy.mean(background_counts)
 
             profile /= background
 
         elif normalize == "counts":
             profile = numpy.concatenate(
-                [numpy.array(x, dtype=numpy.float) / y
+                [numpy.array(x, dtype=numpy.float64) / y
                  for x, y in zip(self.aggregate_counts,
                                  self.counts)])
 
         return profile
 
     def writeLengthStats(self, outfile):
         '''output length stats to outfile.'''
```

### Comparing `cgat-0.6.5/cgat/BamTools/peakshape.pyx` & `cgat-0.7.0/cgat/BamTools/peakshape.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         nreads, counts = self.coverageInInterval(infile, 
                                                  contig, 
                                                  max(0, pos + bins[0]),
                                                  pos + bins[-1],
                                                  **kwargs )
 
         nbins = len(bins) - 1
-        hist = numpy.zeros(nbins, dtype=numpy.int)
+        hist = numpy.zeros(nbins, dtype=numpy.int64)
         cdef int lcounts = len(counts)
 
         if self.smooth_method is not None:
             smoothed_counts = self.smooth_method(counts)
 
         offset = -bins[0]
         xstart = offset + bins[0] 
@@ -192,15 +192,15 @@
                                      right_last - peak_center)
         cdef int closest_dist = min(peak_center - left_last,
                                     right_first - peak_center)
 
         #################################################
         # compute histogram
         nbins = len(bins) - 1
-        hist = numpy.zeros(nbins, dtype = numpy.int)
+        hist = numpy.zeros(nbins, dtype = numpy.int64)
 
         # decide in which region to count - interval or window
         if use_interval:
             counts = counts_in_interval
             # offset = peak
             offset = peak_center
         else:
@@ -333,15 +333,15 @@
                     # read is unmapped but has still a coordinate
                     # assigned.
                     continue
 
                 for i from rstart <= i < rend: ccounts[i] += 1
 
         # transfer to numpy count object
-        counts = numpy.zeros( interval_width, dtype = numpy.int )
+        counts = numpy.zeros( interval_width, dtype = numpy.int64)
         for i from 0 <= i < interval_width: counts[i] = ccounts[i]
 
         free( ccounts )
 
         return nreads, counts
 
 cdef class CounterBigwig(Counter):
```

### Comparing `cgat-0.6.5/cgat/Bed.py` & `cgat-0.7.0/cgat/Bed.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/Blat.py` & `cgat-0.7.0/cgat/Blat.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/CBioPortal.py` & `cgat-0.7.0/cgat/CBioPortal.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/Components/Components.pyx` & `cgat-0.7.0/cgat/Components/Components.pyx`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/Components/connected_components.cpp` & `cgat-0.7.0/cgat/Components/connected_components.cpp`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/Components/connected_components.h` & `cgat-0.7.0/cgat/Components/connected_components.h`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/FastaIterator.py` & `cgat-0.7.0/cgat/FastaIterator.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/Fastq.py` & `cgat-0.7.0/cgat/Fastq.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/FastqTools/fastqtools.pyx` & `cgat-0.7.0/cgat/FastqTools/fastqtools.pyx`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/GFF3.py` & `cgat-0.7.0/cgat/GFF3.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/GTF.py` & `cgat-0.7.0/cgat/GTF.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/GeneModelAnalysis.pyx` & `cgat-0.7.0/cgat/GeneModelAnalysis.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -303,17 +303,17 @@
                 else:
                     utr3.append( (start,end) )
         if strand == "-":
             utr5, utr3 = utr3, utr5
         return utr5, utr3
     
 cimport numpy
-DTYPE_INT = numpy.int
+DTYPE_INT = numpy.int64
 ctypedef numpy.int_t DTYPE_INT_t
-DTYPE_FLOAT = numpy.float
+DTYPE_FLOAT = numpy.float64
 ctypedef numpy.float_t DTYPE_FLOAT_t
 
 
 cdef __add( numpy.ndarray[DTYPE_INT_t, ndim=1]counts, positions, int offset, int length ):
     '''add positions to counts vector'''
     cdef int p, pos
     for p in positions:
@@ -356,16 +356,16 @@
         segments = [ x for x in segments if (x[1] - x[0]) < self.max_length ]
 
         if len(segments) == 0: 
             self.length = 0
             return
 
         cdef int length = sum( [x[1] - x[0] for x in segments ] )
-        cdef numpy.ndarray[DTYPE_INT_t, ndim=1] counts_sense = numpy.zeros( length, dtype = numpy.int )
-        cdef numpy.ndarray[DTYPE_INT_t, ndim=1] counts_antisense = numpy.zeros( length, dtype = numpy.int )
+        cdef numpy.ndarray[DTYPE_INT_t, ndim=1] counts_sense = numpy.zeros( length, dtype = numpy.int64)
+        cdef numpy.ndarray[DTYPE_INT_t, ndim=1] counts_antisense = numpy.zeros( length, dtype = numpy.int64)
         cdef int p, pos, offset
 
         reads_sense, reads_antisense = set(), set()
 
         contig = self.getContig()
         if self.getStrand() == "+":
             is_reverse = False
@@ -889,19 +889,19 @@
         cdef AlignedSegment read
 
         # define counters, add 1 for quality filtered reads
         def get_counters(n=ncounters,
                          x=ndirection_status, 
                          y=nexons_status,
                          z=nspliced_status):
-            counters = numpy.zeros(n, dtype=numpy.float)
+            counters = numpy.zeros(n, dtype=numpy.float64)
             counters.shape = (x,y,z)
             return counters
             
-        # counters = numpy.zeros(ncounters, dtype=numpy.float)
+        # counters = numpy.zeros(ncounters, dtype=numpy.float64)
         # counters.shape = (ndirection_status,
         #                   nexons_status,
         #                   nspliced_status)
 
         # retrieve all reads
         reads = []
 
@@ -1068,15 +1068,15 @@
         if use_barcodes:
             counters = get_counters()
             for key, value in barcode_counters.iteritems():
                 counters += value
 
         if not weight_multi_mapping:
             # convert to full counts
-            counters = numpy.array(counters, dtype=numpy.int)
+            counters = numpy.array(counters, dtype=numpy.int64)
 
         self.counters = counters
         self.reads_below_quality = quality_read_status
 
     def __str__(self):
         return "\t".join(map(str, (self.counters.flat) )) +\
             "\t" +\
@@ -1411,15 +1411,15 @@
         for ix from 0 <= ix < nexons:
             exon_starts[ix] = exons[ix][0]
             exon_ends[ix] = exons[ix][1]
             
         cdef AlignedSegment read1
 
         # define counters, add 1 for quality filtered reads
-        counters = numpy.zeros(ncounters, dtype=numpy.float)
+        counters = numpy.zeros(ncounters, dtype=numpy.float64)
         counters.shape = (npair_status,
                           ndirection_status,
                           nexons_status,
                           nspliced_status)
 
         # retrieve all reads
         reads = []
@@ -1663,15 +1663,15 @@
         free(block_starts)
         free(block_ends)
         free(exon_starts)
         free(exon_ends)
 
         if not weight_multi_mapping:
             # convert to full counts
-            counters = numpy.array(counters, dtype=numpy.int)
+            counters = numpy.array(counters, dtype=numpy.int64)
 
         self.counters = counters
         
         self.reads_below_quality = quality_read_status
         self.pairs_below_quality = quality_pair_status
 
     def __str__(self):
@@ -2304,15 +2304,15 @@
             map_genome2transcript.addDiagonal(start,
                                               end,
                                               x - start)
             x += end - start
 
         l = sum([x[1] - x[0] for x in segments])
 
-        counts = numpy.zeros(l, numpy.int)
+        counts = numpy.zeros(l, numpy.int64)
 
         intervals = set()
         if contig in self.mIntersectors:
             for start, end in segments:
                 r = self.mIntersectors[contig].find(quicksect.Interval(start, end))
                 for x in r:
                     intervals.add((x.start, x.end))
@@ -4860,16 +4860,16 @@
         for region in regions:
             if region:
                 start, end = region
             else:
                 # create dummy counts vector
                 start, end = 0, 1
 
-            counts.append([numpy.zeros(end - start, numpy.int),
-                           numpy.zeros(end - start, numpy.int)])
+            counts.append([numpy.zeros(end - start, numpy.int64),
+                           numpy.zeros(end - start, numpy.int64)])
 
         def __add(counts, positions, offset):
             l = len(counts)
             for p in positions:
                 pos = p - offset
                 if 0 <= pos < l:
                     counts[pos] += 1
```

### Comparing `cgat-0.6.5/cgat/Genomics.py` & `cgat-0.7.0/cgat/Genomics.py`

 * *Files 0% similar despite different names*

```diff
@@ -1471,15 +1471,15 @@
     """given a pair of sequences, calculate
     a substitution matrix for the given alphabet.
     """
     if len(seq1) != len(seq2):
         raise ValueError("two sequences of unequal length submitted")
 
     nchars = len(alphabet)
-    matrix = numpy.zeros((nchars, nchars), numpy.int)
+    matrix = numpy.zeros((nchars, nchars), numpy.int64)
 
     map_char2pos = {}
     for x in alphabet:
         map_char2pos[x] = len(map_char2pos)
 
     for x in range(len(seq1)):
         try:
```

### Comparing `cgat-0.6.5/cgat/Glam2.py` & `cgat-0.7.0/cgat/Glam2.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/Glam2Scan.py` & `cgat-0.7.0/cgat/Glam2Scan.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/Histogram.py` & `cgat-0.7.0/cgat/Histogram.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/Histogram2D.py` & `cgat-0.7.0/cgat/Histogram2D.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/IGV.py` & `cgat-0.7.0/cgat/IGV.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/IndexedFasta.py` & `cgat-0.7.0/cgat/IndexedFasta.py`

 * *Files 1% similar despite different names*

```diff
@@ -483,15 +483,14 @@
             return
 
         if not result:
             break
 
         is_new, identifier, fragment = result
 
-        print(is_new, identifier, fragment)
         if is_new:
             # check for duplicate identifiers
             if identifier in identifiers:
                 if ignore_duplicates:
                     raise ValueError("ignore duplicates not implemented")
                 elif allow_duplicates:
                     # the current implementation will fail if the same
@@ -898,33 +897,33 @@
             "first position %i is larger than last position %i " % \
             (first_pos, last_pos)
 
         p = AString()
 
         if self.mNoSeek:
             # read directly from position
-            p.fromstring(
+            p.frombytes(
                 self.mDatabaseFile.read(block_size, data[3],
-                                        first_pos, last_pos))
+                                        first_pos, last_pos).encode('utf-8'))
         else:
             first_pos += pos_seq
             last_pos += pos_seq
 
             self.mDatabaseFile.seek(first_pos)
-            p.fromstring(self.mDatabaseFile.read(last_pos - first_pos))
+            p.frombytes(self.mDatabaseFile.read(last_pos - first_pos).encode('utf-8'))
 
         if str(strand) in ("-", "0", "-1"):
             p = AString(Genomics.reverse_complement(str(p)))
 
         if self.mTranslator:
             return self.mTranslator.translate(p)
         elif as_array:
             return p
         else:
-            return p.tostring().decode("ascii")
+            return p.tobytes().decode("ascii")
 
     def getRandomCoordinates(self, size):
         """returns coordinates for a random fragment of size #.
 
         The coordinates are forward/reverse.
 
         Default sampling mode:
```

### Comparing `cgat-0.6.5/cgat/IndexedGenome.py` & `cgat-0.7.0/cgat/IndexedGenome.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/Intervals.py` & `cgat-0.7.0/cgat/Intervals.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/Iterators.py` & `cgat-0.7.0/cgat/Iterators.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/MEME.py` & `cgat-0.7.0/cgat/MEME.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/Masker.py` & `cgat-0.7.0/cgat/Masker.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/MatrixTools.py` & `cgat-0.7.0/cgat/MatrixTools.py`

 * *Files 0% similar despite different names*

```diff
@@ -206,15 +206,15 @@
         m.mMapCol2Token = col_tokens
         m.mMapToken2Row = map_token2row
         m.mMapToken2Col = map_token2col
 
     return matrix
 
 
-def buildMatrixFromLists(lists, dtype=numpy.float, default=None):
+def buildMatrixFromLists(lists, dtype=numpy.float64, default=None):
     '''build a matrix from a list of lists.
 
     Each list is a list of tuples (row, value).
     The columns are given by order of the lists.
 
     Returns matrix, row_headers
     '''
@@ -231,15 +231,15 @@
 
     for col, l in enumerate(lists):
         for row, value in l:
             matrix[all_rows[row], col] = value
     return matrix, list(all_rows.keys())
 
 
-def buildMatrixFromTables(infiles, column, column_header=0, dtype=numpy.float,
+def buildMatrixFromTables(infiles, column, column_header=0, dtype=numpy.float64,
                           default=None):
     '''build a matrix from a column called *column* in a series of input files.
 
     If column_value is None, the first column is taken as the name of the row.
 
     The columns are given by order of the input files.
 
@@ -256,15 +256,15 @@
 
 def buildMatrixFromEdges(edges,
                          in_map_token2row={},
                          in_map_token2col={},
                          is_symmetric=False,
                          missing_value=0,
                          diagonal_value=0,
-                         dtype=numpy.int):
+                         dtype=numpy.int64):
     """build a matrix from an edge-list representation.
 
     For example, the following list of tuples::
 
        [('A', 'B', 1),
         ('A', 'C', 2),
         ('B', 'C', 3)]
```

### Comparing `cgat-0.6.5/cgat/Motifs.py` & `cgat-0.7.0/cgat/Motifs.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/NCL/__init__.py` & `cgat-0.7.0/cgat/NCL/__init__.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/NCL/_cnestedlist.pxd` & `cgat-0.7.0/cgat/NCL/_cnestedlist.pxd`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/NCL/cnestedlist.pyx` & `cgat-0.7.0/cgat/NCL/cnestedlist.pyx`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/NCL/default.h` & `cgat-0.7.0/cgat/NCL/default.h`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/NCL/intervaldb.c` & `cgat-0.7.0/cgat/NCL/intervaldb.c`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/NCL/intervaldb.h` & `cgat-0.7.0/cgat/NCL/intervaldb.h`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/RLE.py` & `cgat-0.7.0/cgat/RLE.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/RateEstimation.py` & `cgat-0.7.0/cgat/RateEstimation.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/SVGdraw.py` & `cgat-0.7.0/cgat/SVGdraw.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/SequenceProperties.py` & `cgat-0.7.0/cgat/SequenceProperties.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,15 +137,15 @@
         SequenceProperties.loadSequence(self, sequence, seqtype)
 
         # do the encryption
         h = hashlib.md5(six.b(sequence)).digest()
         # map to printable letters: hid has length 22, so the padded '=' are
         # truncated. You have to add them, if you ever want to decode,
         # but who would do such a thing :=)
-        r = base64.encodestring(h)[0:22].decode("ascii")
+        r = base64.encodebytes(h)[0:22].decode("ascii")
 
         # finally substitute some characters:
         # '/' for '_', so we have legal file names
         # '[' for '+' and ']' for '=' for internet-applications
         hid = r.replace('/', '_').replace('+', '[').replace('=', ']')
 
         self.mHid = hid
```

### Comparing `cgat-0.6.5/cgat/SetTools.py` & `cgat-0.7.0/cgat/SetTools.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,15 @@
         The matrix is a list of lists. The upper diagonal of the
         matrix contains the size of the union of two sets and the
         lower diagonal the intersection of two sets.
 
     '''
 
     l = len(list_of_sets)
-    matrix = numpy.zeros((l, l), dtype=numpy.int)
+    matrix = numpy.zeros((l, l), dtype=numpy.int64)
     for x in range(l):
         xx = list_of_sets[x]
         for y in range(x):
             yy = list_of_sets[y]
             union = xx.union(yy)
             inter = xx.intersection(yy)
             matrix[x][y] = len(union)
```

### Comparing `cgat-0.6.5/cgat/Sra.py` & `cgat-0.7.0/cgat/Sra.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/Stats.py` & `cgat-0.7.0/cgat/Stats.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 Code
 ----
 
 '''
 import math
 import numpy
 import scipy
-import scipy.stats
+from scipy import stats
 import scipy.interpolate
 import collections
 from functools import reduce
 
 
 def getSignificance(pvalue, thresholds=[0.05, 0.01, 0.001]):
     """return cartoon of significance of a p-Value."""
@@ -308,17 +308,17 @@
         n.sort()
         self.mQ1 = n[len(n) / 4]
         self.mQ3 = n[len(n) * 3 / 4]
 
         self.mCounts = len(n)
         self.mMin = min(n)
         self.mMax = max(n)
-        self.mMean = scipy.mean(n)
-        self.mMedian = scipy.median(n)
-        self.mSampleStd = scipy.std(n)
+        self.mMean = numpy.mean(n)
+        self.mMedian = numpy.median(n)
+        self.mSampleStd = numpy.std(n)
         self.mSum = reduce(lambda x, y: x + y, n)
 
     def getZScore(self, value):
         """return zscore for value."""
         if self.mSampleStd > 0:
             return (value - self.mMean) / self.mSampleStd
         else:
@@ -437,17 +437,17 @@
                 self.q3 = n[len(n) * 3 // 4]
             else:
                 self.q1 = self.q3 = 0
 
             self.counts = len(n)
             self.min = min(n)
             self.max = max(n)
-            self.mean = scipy.mean(n)
-            self.median = scipy.median(n)
-            self.samplestd = scipy.std(n)
+            self.mean = numpy.mean(n)
+            self.median = numpy.median(n)
+            self.samplestd = numpy.std(n)
             self.sum = reduce(lambda x, y: x + y, n)
 
     def getHeaders(self):
         """returns header of column separated values."""
         return self.fields
 
     def getHeader(self):
@@ -498,15 +498,15 @@
         raise ValueError("p-values out of range")
 
     # set to default of qvalue method
     if vlambda is None:
         vlambda = numpy.arange(0, 0.95, 0.05)
 
     m = len(pvalues)
-    pvalues = numpy.array(pvalues, dtype=numpy.float)
+    pvalues = numpy.array(pvalues, dtype=numpy.float64)
 
     if pi0 is None:
         if type(vlambda) == float:
             vlambda = (vlambda,)
 
         if len(vlambda) > 1 and len(vlambda) < 4:
             raise ValueError(
@@ -521,15 +521,15 @@
             if vlambda < 0 or vlambda >= 1:
                 raise ValueError("vlambda must be within [0, 1).")
 
             pi0 = numpy.mean([x >= vlambda for x in pvalues]) / (1.0 - vlambda)
             pi0 = min(pi0, 1.0)
         else:
 
-            pi0 = numpy.zeros(len(vlambda), numpy.float)
+            pi0 = numpy.zeros(len(vlambda), numpy.float64)
 
             for i in range(len(vlambda)):
                 pi0[i] = numpy.mean([x >= vlambda[i]
                                      for x in pvalues]) / (1.0 - vlambda[i])
 
             if pi0_method == "smoother":
 
@@ -554,16 +554,16 @@
                 if smooth_log_pi0:
                     pi0 = math.exp(pi0)
 
             elif pi0_method == "bootstrap":
 
                 minpi0 = min(pi0)
 
-                mse = numpy.zeros(len(vlambda), numpy.float)
-                pi0_boot = numpy.zeros(len(vlambda), numpy.float)
+                mse = numpy.zeros(len(vlambda), numpy.float64)
+                pi0_boot = numpy.zeros(len(vlambda), numpy.float64)
 
                 for i in range(100):
                     # sample pvalues
                     idx_boot = numpy.random.random_integers(0, m - 1, m)
                     pvalues_boot = pvalues[idx_boot]
 
                     for x in range(len(vlambda)):
@@ -590,15 +590,15 @@
     idx = numpy.argsort(pvalues)
     # monotonically decreasing bins, so that bins[i-1] > x >=  bins[i]
     bins = numpy.unique(pvalues)[::-1]
 
     # v[i] = number of observations less than or equal to pvalue[i]
     # could this be done more elegantly?
     val2bin = len(bins) - numpy.digitize(pvalues, bins)
-    v = numpy.zeros(m, dtype=numpy.int)
+    v = numpy.zeros(m, dtype=numpy.int64)
     lastbin = None
     for x in range(m - 1, -1, -1):
         bin = val2bin[idx[x]]
         if bin != lastbin:
             c = x
         v[idx[x]] = c + 1
         lastbin = bin
@@ -670,15 +670,15 @@
     @classmethod
     def getHeaders(cls):
         return ("coeff", "pvalue", "significance", "observations",
                 "method", "alternative")
 
 
 def filterMasked(xvals, yvals, missing=("na", "Nan", None, ""),
-                 dtype=numpy.float):
+                 dtype=numpy.float64):
     """convert xvals and yvals to numpy array skipping pairs with
     one or more missing values."""
     xmask = [i in missing for i in xvals]
     ymask = [i in missing for i in yvals]
     return (numpy.array([xvals[i] for i in range(len(xvals))
                          if not xmask[i]], dtype=dtype),
             numpy.array([yvals[i] for i in range(len(yvals))
@@ -1037,15 +1037,15 @@
     if n is None:
         n = len(pvalues)
 
     if method == "fdr":
         method = "BH"
 
     # optional, remove NA values
-    p = numpy.array(pvalues, dtype=numpy.float)
+    p = numpy.array(pvalues, dtype=numpy.float64)
     lp = len(p)
 
     assert n <= lp
 
     if n <= 1:
         return p
     if n == 2 and method == "hommel":
@@ -1151,16 +1151,16 @@
        Chemistry, 1964, 36 (8), pp 1627-1639.
     .. [2] Numerical Recipes 3rd Edition: The Art of Scientific Computing
        W.H. Press, S.A. Teukolsky, W.T. Vetterling, B.P. Flannery
        Cambridge University Press ISBN-13: 9780521880688
     """
 
     try:
-        window_size = numpy.abs(numpy.int(window_size))
-        order = numpy.abs(numpy.int(order))
+        window_size = numpy.abs(numpy.int64(window_size))
+        order = numpy.abs(numpy.int64(order))
     except ValueError:
         raise ValueError("window_size and order have to be of type int")
     if window_size % 2 != 1 or window_size < 1:
         raise TypeError("window_size size must be a positive odd number")
     if window_size < order + 2:
         raise TypeError("window_size is too small for the polynomials order")
     order_range = list(range(order + 1))
```

### Comparing `cgat-0.6.5/cgat/Tree.py` & `cgat-0.7.0/cgat/Tree.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/TreeTools.py` & `cgat-0.7.0/cgat/TreeTools.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/VCF.py` & `cgat-0.7.0/cgat/VCF.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/VCFTools/vcftools.pyx` & `cgat-0.7.0/cgat/VCFTools/vcftools.pyx`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/Variants.py` & `cgat-0.7.0/cgat/Variants.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/cgat.py` & `cgat-0.7.0/cgat/cgat.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/dictzip.py` & `cgat-0.7.0/cgat/dictzip.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/makeGeneset.py` & `cgat-0.7.0/cgat/makeGeneset.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/tools/bam2bam.py` & `cgat-0.7.0/cgat/tools/bam2bam.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/tools/bam2bam_split_reads.py` & `cgat-0.7.0/cgat/tools/bam2bam_split_reads.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/tools/bam2bed.py` & `cgat-0.7.0/cgat/tools/bam2bed.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/tools/bam2depth.py` & `cgat-0.7.0/cgat/tools/bam2depth.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/tools/bam2fasta.py` & `cgat-0.7.0/cgat/tools/bam2fasta.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/tools/bam2fastq.py` & `cgat-0.7.0/cgat/tools/bam2fastq.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/tools/bam2geneprofile.py` & `cgat-0.7.0/cgat/tools/bam2geneprofile.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/tools/bam2peakshape.py` & `cgat-0.7.0/cgat/tools/bed2bed.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,658 +1,690 @@
-'''bam2peakshape.py - compute peak shape features from a bam-file
-==============================================================
-
-:Tags: Genomics NGS Intervals BAM BED Summary
+'''
+bed2bed - manipulate bed files
+=================================
 
 Purpose
 -------
 
-This script takes a :term:`bed` formatted file with regions of
-interest, for example binding intervals from a ChIP-Seq
-experiment. Using a collection of aligned reads is a :term:`bam`
-formatted file or :term:`bigwig` formatted file, the script outputs a
-collection of features describing the peak shape.
-
-This script is designed with a slight emphasis on ChIP-Seq datasets.
-The main reason that this script is better suited for ChIP-Seq is
-that(1) it is able to center the counting window at the summit of
-every individual peak; (2) it is also able to use the control ChIP-Seq
-library to enable side-by-side comparison of treatment vs control;(3)
-it can randomly shift the set of input regions to generate a
-artificial set of regions, in the absence of real ChIP-Seq control
-library, the random regions can provide a peaks profile that can be
-used as the control.
-
-For example, given the peaks regions defined by analyzing some
-ChIP-Seq dataset (e.g. by using MACS), and without the need to use any
-additional genomic annotations (e.g. ENSEMBL, refseq), we can
-visualise the binding profiles of transcriptionfactors ChIP-Seq data
-relative to the center of each peak regions.
-
-The script outputs a tab-separated table on stdout containing features
-for each interval. A peak is defined as the location of the highest
-density in an interval. The width of the peak (peak_width) is defined
-as the region around the peak in which the density does not drop below
-a threshold of peak_heigt * 90%.
+This script provides various methods for merging (by position, by name
+or by score), filtering and moving bed formatted intervals and
+outputting the results as a bed file
 
-Usage
------
+Methods
+-------
 
-Detailed usage example
-++++++++++++++++++++++
+This script provides several methods, each with a set of options
+to control behavoir:
 
-The following command will generate the peak shape plot for the peak
-regions defined in :file:`onepeak.bed`, using the reads stored in
-:file:`small.bam`.  The command will also create a profile for the
-control library.  The control library in this example is re-using the
-same reads file :file:`small.bam`, however, in your actual experiment,
-it should be a different library (the input library for this ChIP-Seq
-experiment).::
-
-    python ./scripts/bam2peakshape.py \
-        ./tests/bam2peakshape.py/small.bam \
-        ./tests/bam2peakshape.py/onepeak.bed \
-        --control-bam-file=./tests/bam2peakshape.py/small.bam \
-        --use-interval \
-        --normalize-transcript
+merge
++++++
 
+Merge together overlapping or adjacent intervals. The basic
+functionality is similar to bedtools merge, but with some additions:
 
-Output files
-++++++++++++
+* Merging by name: specifying the --merge-by-name option will mean
+  that only overlaping (or adjacent intervals) with the same value in
+  the 4th column of the bed will be merged
 
-Among the features output are:
+* Removing overlapping intervals with inconsistent names: set the
+   ``--remove-inconsistent-names`` option.
 
-+-------------------+---------------------------------------------------------+
-|*Column*           |*Content*                                                |
-+-------------------+---------------------------------------------------------+
-|peak_height        |number of reads at peak                                  |
-+-------------------+---------------------------------------------------------+
-|peak_median        |median coverage compared to peak height                  |
-+-------------------+---------------------------------------------------------+
-|interval_width     |width of interval                                        |
-+-------------------+---------------------------------------------------------+
-|peak_width         |width of peak                                            |
-+-------------------+---------------------------------------------------------+
-|bins               |bins for a histogram of densities within the interval.   |
-+-------------------+---------------------------------------------------------+
-|npeaks             |number of density peaks in interval.                     |
-+-------------------+---------------------------------------------------------+
-|peak_center        |point of highest density in interval                     |
-+-------------------+---------------------------------------------------------+
-|peak_relative_pos  |point of highest density in interval coordinates         |
-+-------------------+---------------------------------------------------------+
-|counts             |counts for a histogram of densities within the interval  |
-+-------------------+---------------------------------------------------------+
-|furthest_half_heigh|Distance of peak center to furthest half-height position |
-+-------------------+---------------------------------------------------------+
-|closest_half_height|Distance of peak center to closest half-height position  |
-+-------------------+---------------------------------------------------------+
-
-
-Additionally, the script outputs a set of matrixes with densities over
-intervals that can be used for plotting. The default filenames are
-``(matrix|control)_<sortorder>.tsv.gz``, The names can be controlled
-with the ``--output-filename-pattern`` option.
+.. caution::
+   Intervals of the same name will only be merged if they
+   are consecutive in the bed file.
 
+* Only output merged intervals: By specifiying the --merge-min-intervals=n
+  options, only those intervals that were created by merging at least n
+  intervals together will be output
 
-Type::
+Intervals that are close but not overlapping can be merged by setting
+--merge-distance to a non-zero value
 
-   python bam2peakshape.py --help
+bins
+++++
 
-for command line help.
+Merges together overlapping or adjecent intervals only if they have
+"similar" scores. Score similarity is assessed by creating a number of
+score bins and assigning each interval to a bin. If two adjacent
+intervals are in the same bin, the intervals are merged. Note that in
+contrast to merge-by-name above, two intervals do not need to be
+overlapping or within a certain distance to be merged.
 
+There are several methods to create the bins:
 
-Options
--------
+* equal-bases: Bins are created to that they contain the same number of bases.
+  Specified by passing "equal-bases" to --binning-method. This is the default.
+
+* equal-intervals: Score bins are create so that each bin contains the
+  same number of intervals. Specified by passing "equal-intervals" to
+  --binning-method.
+
+* equal-range: Score bins are created so that
+  each bin covers the same fraction of the total range of
+  scores. Specified by passing "equal-range" to --binning-method.
 
-Option: Shift
+* bin-edges: Score binds can be specified by manually passing a comma
+  seperated list of bin edges to --bin-edges.
+
+The number of bins is specified by the --num-bins options, and the
+default is 5.
+
+block
++++++
+
+Creates blocked bed12 outputs from a bed6, where intervals with the
+same name are merged together to create a single bed12 entry.
+
+.. Caution:: Input must be sorted so that entries of the same
+name are together.
+
+filter-genome
 +++++++++++++
 
-shift the each read by a certain distance, because in a ChIP-Seq
-experment, the read is always at the edge of an sonicated fragment,
-the actual binding site is usually L/2 distance away from the read,
-where L is the length of sonicated fragment (determined either
-experimentally or computationally).
+Removes intervals that are on unknown contigs or extend off the 3' or
+5' end of the contig.  Requires a tab seperated input file to -g which
+lists the contigs in the genome, plus their lengths.
+
+sanitize-genome
++++++++++++++++
 
-This option is used only if the input reads are in :term:`bam` formatted file.
-If input reads are :term:`bigwig` formatted file, this option is ignored.
+As above, but instead of removing intervals overlapping the ends of
+contigs, truncates them.  Also removes empty intervals.
 
-Option: Random shift
-++++++++++++++++++++
+filter-names
+++++++++++++
 
-randomly shift the set of input regions to generate a artificial set
-of regions. In the absence of real ChIP-Seq control library, the
-random regions can provide a peaks profile that can be used as the
-control.
+Output intervals whose names are in list of desired names. Names are
+supplied as a file with one name on each line.
 
-Option: Centring method
-+++++++++++++++++++++++
+shift
++++++
 
-"reads" will output in the way that the summit of the peaks are
-aligned. "middle" will output in the way that the middle of the input
-bed intervals are aligned.
+Moves intervals by the specified amount, but will not allow them to be
+shifted off the end of contigs. Thus if a shift will shift the start
+of end of the contig, the interval is only moved as much as is
+possible without doing this.
+
+rename-chr
+++++++++++
+
+Renames chromosome names. Source and target names are supplied as a file
+with two columns. Examples are available at:
+https://github.com/dpryan79/ChromosomeMappings
+Note that unmapped chromosomes are dropped from the output file.
 
-Option: Only interval
-+++++++++++++++++++++
+Other options
++++++++++++++
 
-Only count reads that are in the interval as defined by the input bed file.
+-g/--genome-file, -b/--bam-file:
+   the filter-genome, sanitize-genome and shift methods require a genome in
+   order to ensure they are not placing intervals outside the limits of
+   contigs. This genome can be supplied either as a samtools or cgat indexed
+   genome, or extracted from the header of a bam file.
 
-Option: normalization=sum
-+++++++++++++++++++++++++
+Examples
+--------
 
-normalize counts such that the sum of all counts in all features are
-exactly 1000000.
+Merge overlapping or adjectent peaks from a CHiP-seq experiment where the
+intervals have the same name:
 
-The detail normalization algorithm as follows: norm = sum(all counts
-in all features)/1000000.0 normalized count = normalized count / norm
+    cat chip-peaks.bed | cgat bed2bed --method=merge --merge-by-name > chip-peaks-merged.bed
 
-.. todo::
+Merge adjected ChIP-seq peaks if their scores are in the same quartile of
+all scores:
 
-   paired-endedness is not fully implemented.
+    cat chip-peaks.bed | cgat bed2bed --method=bins --binning-method=equal-intervals --num-bins=4
+
+Remove intervals that overlap the ends of a contig and those that are on a
+non-standard contig. Take the input intervals from a file rather than stdin.
+Note that hg19.fasta has been indexed with `index_genome`:
+
+    cgat bed2bed --method=filter-genome --genome-file=hg19.fasta -I chip-peaks.bed -O chip-peaks-sanitized.bed
+
+Convert a bed file contain gene structures with one line per exon to a bed12
+with linked block representing the gene structure. Note the transparent use
+of compressed input and output files:
+
+    cgat bed2bed --method=block -I transcripts.bed.gz -O transcripts.blocked.bed.gz
+
+Rename UCSC chromosomes to ENSEMBL.
+
+    cat ucsc.bed | cgat bed2bed --method=rename-chr --rename-chr-file=ucsc2ensembl.txt > ensembl.bed
+
+Usage
+-----
+
+   cgat bed2bed --method=[METHOD] [OPTIONS]
+
+Will read bed file from stdin and apply the specified method
 
 Command line options
 --------------------
-
 '''
 
 import sys
-import os
-import re
 import cgatcore.experiment as E
-import cgatcore.iotools as iotools
-import pysam
+import cgat.IndexedFasta as IndexedFasta
 import cgat.Bed as Bed
-import numpy
-import collections
-import pyBigWig
+import cgat.Intervals as Intervals
+from collections import defaultdict as defaultdict
+import pysam
+import csv
 
-import cgat.BamTools.peakshape as bam2peakshape
 
+def filterNames(iterator, names):
+    """ Select only those intervals whose name is in names """
 
-def buildArgumentParser(argv):
+    for bed in iterator:
+        if bed.name in names:
+            yield bed
 
-    if not argv:
-        argv = sys.argv
 
-    # setup command line parser
-    parser = E.ArgumentParser(description=__doc__)
+def merge(iterator,
+          max_distance=0,
+          by_name=False,
+          min_intervals=1,
+          remove_inconsistent=False,
+          resolve_blocks=False,
+          stranded=False):
+    """iterator for merging adjacent bed entries.
 
-    parser.add_argument("--version", action='version', version="1.0")
+    *max_distance* > 0 permits merging of intervals that are
+    not directly adjacent.
 
-    parser.add_argument("-f", "--format", dest="format", type=str,
-                        choices=("bam", "bigwig"),
-                        help="format of genomic input files for densities "
-                        )
+    If *by_name = True*, only entries with the same name are merged.
 
-    parser.add_argument(
-        "-o", "--use-interval", dest="use_interval", action="store_true",
-        help="only count tags that are in interval given "
-        "in bed file. Otherwise, use a fixed width window (see --window-size) "
-        "around peak ")
+    If *remove_inconsistent*, overlapping intervals where the names
+    are inconsistent will be removed.
 
-    parser.add_argument(
-        "-w", "--window-size", dest="window_size", type=int,
-        help="window size in bp on either side of a peak used for getting "
-        "read densities. If ``--window-size`` is 1000, the actual window size"
-        "will be 2kb, 1kb on either side of the peak in an interval"
-        )
+    The score gives the number of intervals that have been merged.
+    """
 
-    parser.add_argument(
-        "-b", "--bin-size", dest="bin_size", type=int,
-        help="bin-size in bp for computing read densities. "
-        "If ``--window-size`` is set to 1000 and ``--bin-size`` to 10, "
-        "there will be 100 bins on either side of a peak. "
-        )
+    if remove_inconsistent and by_name:
+        assert ValueError(
+            "using both remove_inconsistent and by_name makes no sense")
+
+    def iterate_chunks(iterator):
+        max_end = defaultdict(int)
+        to_join = defaultdict(list)
+        last_name = defaultdict(str)
 
-    parser.add_argument(
-        "--smooth-method", dest="smooth_method", type=str,
-        choices=("none", "sum", "sg"),
-        help="smooting method to apply to density data before sampling "
-        "according to ``bin-size``. sg=SavitzkyGolay, sum=sum density in bin, "
-        "none=no smoothing "
-        )
+        last = next(iterator)
 
-    parser.add_argument("-s", "--sort-order", dest="sort_orders",
-                        type=str,
-                        action="append",
-                        choices=("peak-height", "peak-width", "unsorted",
-                                 "interval-width", "interval-score"),
-                        help="output sort order for matrices. "
-                        )
+        if not stranded:
+            strand = "."
+        else:
+            strand = last.strand
 
-    parser.add_argument(
-        "-c", "--control-bam-file", "--control-bigwig-file",
-        action="append",
-        dest="control_files",
-        type=str,
-        help="control file. If given, two peakshapes are computed, "
-        "one for the primary data and one for the control data. "
-        "The control file is centered around the same "
-        "base as the primary file and output in the same "
-        "sort order as the primary profile to all side-by-side. "
-        "comparisons. Multiple control files can be given. The "
-        "control files should have the same format as the "
-        "principal input file "
-        )
+        max_end[strand] = last.end
+        to_join[strand] = [last]
 
-    parser.add_argument(
-        "-r", "--random-shift", dest="random_shift", action="store_true",
-        help="shift intervals in random direction up/downstream of interval "
-        )
+        for bed in iterator:
 
-    parser.add_argument(
-        "-e", "--centring-method", dest="centring_method", type=str,
-        choices=("reads", "middle"),
-        help="centring method. Available are: "
-        "reads=use density to determine peak, "
-        "middle=use middle of interval "
-        )
+            if not stranded:
+                strand = "."
+            else:
+                strand = bed.strand
 
-    parser.add_argument(
-        "-n", "--normalize-matrix", dest="normalization", type=str,
-        choices=("none", "sum"),
-        help="matrix normalisation to perform. "
-        )
+            d = bed.start - max_end[strand]
 
-    parser.add_argument(
-        "--use-strand", dest="strand_specific", action="store_true",
-        help="use strand information in intervals. Intervals on the "
-        "negative strand are flipped "
-        )
+            if bed.contig == last.contig:
+                assert bed.start >= last.start, \
+                    "input file should be sorted by contig and position: d=%i:\n%s\n%s\n" \
+                    % (d, last, bed)
+
+            if bed.contig != last.contig:
+
+                for s in to_join:
+                    if to_join[s]:
+                        yield to_join[s]
+                    to_join[s] = []
+                    max_end[s] = 0
+
+            elif (d > max_distance or
+                  (by_name and last_name[strand] and last_name[strand] != bed.name)):
+
+                if to_join[strand]:
+                    yield to_join[strand]
+
+                to_join[strand] = list()
+
+            last = bed
+            last_name[strand] = last.name
+            max_end[strand] = max(bed.end, max_end[strand])
+            to_join[strand].append(bed)
+
+        for strand in sorted(to_join):
+                if to_join[strand]:
+                    try:
+                        yield to_join[strand]
+                    except:
+                        return
 
-    parser.add_argument(
-        "-i", "--shift-size", dest="shift", type=int,
-        help="shift for reads. When processing bam files, "
-        "reads will be shifted upstream/downstream by this amount. "
-        )
-
-    parser.set_defaults(
-        bin_size=10,
-        shift=0,
-        window_size=1000,
-        sort_orders=[],
-        centring_method="reads",
-        control_files=[],
-        random_shift=False,
-        strand_specific=False,
-        format="bam",
-        report_step=100,
-        use_interval=False,
-        smooth_method=None,
-    )
-
-    return parser
-
-
-IntervalData = collections.namedtuple(
-    "IntervalData",
-    "foreground interval controls shifted")
-
-
-def outputFeatureTable(outfile, features_per_interval, bins):
-    '''ouput results from density profiles.'''
-
-    outfile.write("\t".join(
-        ("contig",
-         "start",
-         "end",
-         "name",
-         "\t".join(bam2peakshape.PeakShapeResult._fields))) + "\n")
-
-    # output principal table
-    n = 0
-    for foreground, bed, controls, shifted in features_per_interval:
-        n += 1
-        if "name" in bed:
-            name = bed.name
-        else:
-            name = str(n)
-        outfile.write("%s\t%i\t%i\t%s\t" %
-                      (bed.contig, bed.start, bed.end, name))
-
-        outfile.write("\t".join(map(str, foreground[:-2])))
-        bins, counts = foreground[-2], foreground[-1]
-        outfile.write("\t%s" % ",".join(map(str, bins)))
-        outfile.write("\t%s" % ",".join(map(str, counts)))
-        outfile.write("\n")
-
-
-def writeMatricesForSortOrder(features_per_interval,
-                              bins,
-                              foreground_track,
-                              control_tracks,
-                              shifted,
-                              sort_order):
-    '''output one or more matrices for each sort sorder.
-
-    For each sort order output the forerground. If there
-    are additional controls and shifted section, output
-    these as well
-
-    The files will named:
-    matrix_<track>_<sortorder>
-
-    '''
-    if "name" in features_per_interval[0].interval:
-        names = [x.interval.name for x in features_per_interval]
-    else:
-        names = list(map(str, list(range(1, len(features_per_interval) + 1))))
-
-    bins = ["%i" % x for x in bins]
-    sort_order = re.sub("-", "_", sort_order)
-
-    # write foreground
-    iotools.write_matrix(
-        E.open_output_file("matrix_%s_%s.gz" % (foreground_track, sort_order)),
-        [x.foreground.counts for x in features_per_interval],
-        row_headers=names,
-        col_headers=bins,
-        row_header="name")
-
-    # write controls
-    for idx, track in enumerate(control_tracks):
-        iotools.write_matrix(
-            E.open_output_file("matrix_%s_%s.gz" % (track, sort_order)),
-            [x.controls[idx].counts for x in features_per_interval],
-            row_headers=names,
-            col_headers=bins,
-            row_header="name")
-
-    # write shifted matrix
-    if shifted:
-        iotools.write_matrix(
-            E.open_output_file("matrix_shift_%s.gz" % (sort_order)),
-            [x.shifted.counts for x in features_per_interval],
-            row_headers=names,
-            col_headers=bins,
-            row_header="name")
-
-    # output a combined matrix
-    if len(control_tracks) > 0 or shifted:
-        rows = []
-        for row in features_per_interval:
-            l = [row.foreground.counts]
-            l.extend([row.controls[x].counts for x in
-                      range(len(control_tracks))])
-            if shifted:
-                l.append(row.shifted.counts)
-            rows.append(numpy.concatenate(l))
-
-        n = 1 + len(control_tracks)
-        if shifted:
-            n += 1
-
-        # make column names unique and make sure they can be sorted
-        # lexicographically
-        all_bins = []
-        for x in range(n):
-            all_bins.extend(["%i:%s" % (x, b) for b in bins])
-
-        iotools.write_matrix(
-            E.open_output_file("matrix_sidebyside_%s.gz" % (sort_order)),
-            rows,
-            row_headers=names,
-            col_headers=all_bins,
-            row_header="name")
-
-
-def outputMatrices(features_per_interval,
-                   bins,
-                   foreground_track,
-                   control_tracks=None,
-                   shifted=False,
-                   sort_orders=None):
-    '''ouput matrices from density profiles
-    in one or more sort_orders.
-    '''
-
-    # output sorted matrices
-    if not sort_orders:
-        writeMatricesForSortOrder(features_per_interval,
-                                  bins,
-                                  foreground_track,
-                                  control_tracks,
-                                  shifted,
-                                  "unsorted")
-
-    for sort_order in sort_orders:
-
-        if sort_order == "peak-height":
-            features_per_interval.sort(
-                key=lambda x: x.foreground.peak_height)
-
-        elif sort_order == "peak-width":
-            features_per_interval.sort(
-                key=lambda x: x.foreground.peak_width)
-
-        elif sort_order == "interval-width":
-            features_per_interval.sort(
-                key=lambda x: x.interval.end - x.interval.start)
-
-        elif sort_order == "interval-score":
-            try:
-                features_per_interval.sort(
-                    key=lambda x: float(x.interval.score))
-            except IndexError:
-                E.warn("score field not present - no output")
+    c = E.Counter()
+
+    for to_join in iterate_chunks(iterator):
+
+        c.input += 1
+
+        if remove_inconsistent:
+            names = set([x.name for x in to_join])
+            if len(names) > 1:
+                c.skipped_inconsistent_intervals += 1
                 continue
-            except TypeError:
-                E.warn("score field not a valid number - no output")
+
+        if resolve_blocks:
+            # keep track of number of intervals in each entry
+            for bed in to_join:
+                bed["score"] = 1
+            merged = True
+            while merged:
+                joined = []
+                not_joined = []
+                merged = False
+
+                while len(to_join) > 0:
+                    bed1, to_join = to_join[0], to_join[1:]
+                    intervals1 = bed1.toIntervals()
+                    for bed2 in to_join:
+                        intervals2 = bed2.toIntervals()
+                        if Intervals.calculateOverlap(intervals1, intervals2) > 0:
+                            intervals = Intervals.combine(intervals1 +
+                                                          intervals2)
+                            bed1.fromIntervals(intervals)
+                            bed1["score"] += bed2["score"]
+                            merged = True
+                        else:
+                            not_joined.append(bed2)
+
+                    joined.append(bed1)
+                    to_join = not_joined
+                    not_joined = []
+
+                to_join = joined
+                joined = []
+
+            to_join = sorted(to_join, key=lambda x: int(x.start))
+
+            # keep only those with the created from the merge of the minimum
+            # number of intervals
+
+            for bed in to_join:
+
+                if bed["score"] < min_intervals:
+                    c.skipped_min_intervals += 1
+                    continue
+
+                yield bed
+                c.output += 1
+        else:
+
+            if len(to_join) < min_intervals:
+                c.skipped_min_intervals += 1
                 continue
 
-        writeMatricesForSortOrder(features_per_interval,
-                                  bins,
-                                  foreground_track,
-                                  control_tracks,
-                                  shifted,
-                                  sort_order)
-
-
-def buildDensityMatrices(bedfile,
-                         fg_file,
-                         control_files,
-                         counter,
-                         window_size=1000,
-                         bin_size=10,
-                         strand_specific=False,
-                         centring_method="reads",
-                         use_interval=False,
-                         random_shift=False,
-                         smooth_method="none",
-                         report_step=1000):
-    '''compute densities and peakshape parameters
-    in intervals given by *bedfile* using reads in *fg_file*.
-
-    If *control_files* are given, densities are produced for
-    these as well.
-
-    Returns a list of results for each interval in *bedfile* of
-    type IntervalData and an array of bin-values.
-    '''
-
-    if window_size:
-        # bins are centered at peak-center and then stretching outwards.
-        bins = numpy.arange(-window_size + bin_size // 2,
-                            +window_size,
-                            bin_size)
+            a = to_join[0]
+            a.end = max([entry.end for entry in to_join])
+            a.score = len(to_join)
+            yield a
+            c.output += 1
 
-    result = []
-    c = E.Counter()
-    c.input = 0
+    E.info(str(c))
 
-    for bed in bedfile:
-        c.input += 1
 
-        # if bed.contig not in contigs:
-        #    c.skipped += 1
-        #    continue
-
-        if c.input % report_step == 0:
-            E.info("iteration: %i" % c.input)
-
-        features = counter.countInInterval(
-            fg_file,
-            bed.contig, bed.start, bed.end,
-            window_size=window_size,
-            bins=bins,
-            use_interval=use_interval,
-            centring_method=centring_method)
-
-        if features is None:
-            c.skipped += 1
-            continue
-
-        if control_files:
-            control = []
-            for control_file in control_files:
-                control.append(counter.countAroundPos(
-                    control_file,
-                    bed.contig,
-                    features.peak_center,
-                    bins=features.bins))
+def filterGenome(iterator, contigs):
+    """remove bed intervals that are outside of contigs.
 
-        else:
-            control = None
+    contigs is a dictionary of contig sizes."""
 
-        if random_shift:
-            direction = numpy.random.randint(0, 2)
-            if direction:
-                pos = features.peak_center + 2 * bins[0]
-            else:
-                pos = features.peak_center + 2 * bins[-1]
-            shifted = counter.countAroundPos(fg_file,
-                                             bed.contig,
-                                             pos,
-                                             bins=features.bins)
+    ninput, noutput = 0, 0
+    nskipped_contig, nskipped_range, nskipped_endzero = 0, 0, 0
+
+    for bed in iterator:
+        ninput += 1
+        if bed.contig not in contigs:
+            nskipped_contig += 1
+            continue
+        # IMS: add filtering for filtering <0 co-ordinates
+        if bed.start < 0 or bed.end < 0:
+            nskipped_range += 1
+            continue
+        # should this not be just >, as co-ordinates are half-closed, so
+        # if end = contigs[bed.contig], then interval ends on last base?
+        if bed.end > contigs[bed.contig]:
+            nskipped_range += 1
+            continue
+        if bed.end == 0:
+            nskipped_endzero += 1
+            continue
+        noutput += 1
+        yield bed
+
+    E.info("ninput=%i, noutput=%i, nskipped_contig=%i, nskipped_range=%i, nskipped_endzero=%i" %
+           (ninput, noutput, nskipped_contig, nskipped_range, nskipped_endzero))
+
+
+def sanitizeGenome(iterator, contigs):
+    """truncate bed intervals that extend beyond contigs.
+
+    removes empty intervals (start == end).
+
+    throws an error if start > end.
+    """
+
+    ninput, noutput = 0, 0
+    ntruncated_contig, nskipped_contig, nskipped_empty = 0, 0, 0
+
+    for bed in iterator:
+        ninput += 1
+        if bed.contig not in contigs:
+            nskipped_contig += 1
+            continue
+        # IMS: changing >= to > in if statement: next line sets bed.end = contigs[bed.contig]
+        # this shouldn't count as a truncation.
+        if bed.end > contigs[bed.contig]:
+            bed.end = contigs[bed.contig]
+            ntruncated_contig += 1
+        if bed.start < 0:
+            bed.start = 0
+            ntruncated_contig += 1
+        if bed.start == bed.end:
+            nskipped_empty += 1
+            continue
+        elif bed.start > bed.end:
+            raise ValueError("invalid interval: start > end for %s" % str(bed))
+
+        noutput += 1
+        yield bed
+
+    E.info("ninput=%i, noutput=%i, nskipped_contig=%i, ntruncated=%i, nskipped_empty=%i" %
+           (ninput, noutput, nskipped_contig, ntruncated_contig, nskipped_empty))
+
+
+def shiftIntervals(iterator, contigs, offset):
+    """shift intervals by a certain offset and ensure size is maintaned even id contig end reached.
+
+    contigs is a dictionary of contig sizes."""
+
+    ninput, noutput = 0, 0
+    nskipped_contig, nskipped_range = 0, 0
+
+    for bed in iterator:
+        ninput += 1
+        if bed.contig not in contigs:
+            nskipped_contig += 1
+            continue
+        # IMS: if we skip intervals off the end of the contig we should skipp ones
+        # off the start as well
+        if bed.start < 0 or bed.end < 0:
+            nskipped_range += 1
+            continue
+        # IMS: changing >= to > as bed is half-open
+        if bed.end > contigs[bed.contig]:
+            nskipped_range += 1
+            continue
+        noutput += 1
+
+        # add offset to each start and end, and adjust for contig length
+        l = bed.end - bed.start
+        newstart = bed.start + offset
+        newend = bed.end + offset
+        if newstart < 0:
+            newstart = 0
+            newend = l
+        if newend > contigs[bed.contig]:
+            newstart = contigs[bed.contig] - l
+            newend = contigs[bed.contig]
+
+        bed.start = newstart
+        bed.end = newend
+
+        yield bed
+
+    E.info("ninput=%i, noutput=%i, nskipped_contig=%i, nskipped_range=%i" %
+           (ninput, noutput, nskipped_contig, nskipped_range))
+
+
+def extendInterval(iterator, contigs, distance):
+
+    ninput, noutput, nskipped = 0, 0, 0
+    for bed in iterator:
+        ninput += 1
+
+        if bed.contig not in contigs:
+            nskipped += 1
+            continue
+        if bed.start < 0 or bed.end < 0:
+            nskipped += 1
+            continue
+        if bed.end > contigs[bed.contig]:
+            nskipped += 1
+            continue
+
+        newstart = bed.start - distance
+        newend = bed.end + distance
+
+        if newstart < 0:
+            newstart = 0
+
+        if newend > contigs[bed.contig]:
+            newend = contigs[bed.contig]
+
+        bed.start = newstart
+        bed.end = newend
+
+        noutput += 1
+        yield bed
+
+    E.info("ninput = %i, noutput=%i, nskipped=%i" %
+           (ninput, noutput, nskipped))
+
+
+def renameChromosomes(iterator, chr_map):
+
+    ninput, noutput, nskipped = 0, 0, 0
+
+    for bed in iterator:
+        ninput += 1
+
+        if bed.contig in chr_map.keys():
+            bed.contig = chr_map[bed.contig]
         else:
-            shifted = None
+            nskipped += 1
+            continue
 
-        if strand_specific and bed.strand == "-":
-            features._replace(hist=features.hist[::-1])
-            if control:
-                for c in control:
-                    c._replace(hist=c.hist[::-1])
-            if shifted:
-                shifted._replace(hist=shifted.hist[::-1])
+        noutput += 1
+        yield bed
 
-        result.append(IntervalData._make((features, bed, control, shifted)))
-        c.added += 1
+    E.info("ninput = %i, noutput=%i, nskipped=%i" %
+           (ninput, noutput, nskipped))
 
-    E.info("interval processing: %s" % c)
 
-    return result, bins
+def main(argv=sys.argv):
 
+    parser = E.ArgumentParser(description=__doc__)
 
-def main(argv=None):
-    """script main.
+    parser.add_argument("--version", action='version', version="1.0")
 
-    parses command line options in sys.argv, unless *argv* is given.
-    """
+    # IMS: new method: extend intervals by set amount
+    parser.add_argument("-m", "--method", dest="methods", type=str,
+                        action="append",
+                        choices=("merge", "filter-genome", "bins",
+                                 "block", "sanitize-genome", "shift", "extend",
+                                 "filter-names", "rename-chr"),
+                        help="method to apply")
+
+    parser.add_argument("--num-bins", dest="num_bins", type=int,
+                        help="number of bins into which to merge (used for "
+                        "method `bins)")
+
+    parser.add_argument("--bin-edges", dest="bin_edges", type=str,
+                        help="bin_edges for binning method")
 
-    parser = buildArgumentParser(argv)
+    parser.add_argument(
+        "--binning-method", dest="binning_method", type=str,
+        choices=(
+            "equal-bases", "equal-intervals", "equal-range"),
+        help="method used for binning (used for method `bins` if no "
+        "bin_edges is given)")
 
-    # add common options (-h/--help, ...) and parse command line
-    (args, unknown) = E.start(parser, argv=argv, add_output_options=True, unknowns=True)
+    parser.add_argument(
+        "--merge-distance", dest="merge_distance", type=int,
+        help="distance in bases over which to merge that are not "
+        "directly adjacent")
+
+    parser.add_argument(
+        "--merge-min-intervals", dest="merge_min_intervals", type=int,
+        help="only output merged intervals that are build from at least "
+        "x intervals")
+
+    parser.add_argument(
+        "--merge-by-name", dest="merge_by_name",
+        action="store_true",
+        help="only merge intervals with the same name")
+
+    parser.add_argument(
+        "--merge-and-resolve-blocks", dest="resolve_blocks",
+        action="store_true",
+        help="When merging bed12 entrys, should blocks be resolved?")
+
+    parser.add_argument(
+        "--merge-stranded", dest="stranded",
+        action="store_true",
+        help="Only merge intervals on the same strand")
+
+    parser.add_argument(
+        "--remove-inconsistent-names", dest="remove_inconsistent_names",
+        action="store_true",
+        help="when merging, do not output intervals where the names of "
+        "overlapping intervals do not match")
+
+    parser.add_argument(
+        "--offset", dest="offset",  type=int,
+        help="offset for shifting intervals")
+
+    parser.add_argument("-g", "--genome-file", dest="genome_file", type=str,
+                        help="filename with genome.")
+
+    parser.add_argument("-b", "--bam-file", dest="bam_file", type=str,
+                        help="bam-formatted filename with genome.")
+
+    parser.add_argument("--filter-names-file", dest="names", type=str,
+                        help="list of names to keep. One per line")
+
+    parser.add_argument("--rename-chr-file", dest="rename_chr_file", type=str,
+                        help="mapping table between old and new chromosome names."
+                        "TAB separated 2-column file.")
+
+    parser.set_defaults(methods=[],
+                        merge_distance=0,
+                        binning_method="equal-bases",
+                        merge_by_name=False,
+                        genome_file=None,
+                        rename_chr_file=None,
+                        bam_file=None,
+                        num_bins=5,
+                        merge_min_intervals=1,
+                        bin_edges=None,
+                        offset=10000,
+                        test=None,
+                        extend_distance=1000,
+                        remove_inconsistent_names=False,
+                        resolve_blocks=False)
+
+    (args) = E.start(parser, add_pipe_options=True)
+
+    contigs = None
+    chr_map = None
+
+    # Why provide full indexed genome, when a tsv of contig sizes would do?
+    if args.genome_file:
+        genome_fasta = IndexedFasta.IndexedFasta(args.genome_file)
+        contigs = genome_fasta.getContigSizes()
+
+    if args.bam_file:
+        samfile = pysam.AlignmentFile(args.bam_file)
+        contigs = dict(list(zip(samfile.references, samfile.lengths)))
+
+    if args.rename_chr_file:
+        chr_map = {}
+        with open(args.rename_chr_file, 'r') as filein:
+            reader = csv.reader(filein, delimiter='\t')
+            for row in reader:
+                if len(row) != 2:
+                    raise ValueError("Mapping table must have exactly two columns")
+                chr_map[row[0]] = row[1]
+        if not len(chr_map.keys()) > 0:
+            raise ValueError("Empty mapping dictionnary")
+
+    processor = Bed.iterator(args.stdin)
+
+    for method in args.methods:
+        if method == "filter-genome":
+            if not contigs:
+                raise ValueError("please supply contig sizes")
+            processor = filterGenome(processor, contigs)
+        elif method == "sanitize-genome":
+            if not contigs:
+                raise ValueError("please supply contig sizes")
+            processor = sanitizeGenome(processor, contigs)
+        elif method == "merge":
+            processor = merge(
+                processor,
+                args.merge_distance,
+                by_name=args.merge_by_name,
+                min_intervals=args.merge_min_intervals,
+                remove_inconsistent=args.remove_inconsistent_names,
+                resolve_blocks=args.resolve_blocks,
+                stranded=args.stranded)
+        elif method == "bins":
+            if args.bin_edges:
+                bin_edges = list(map(float, args.bin_edges.split(",")))
+                # IMS: check bin edges are valid
+                if not(len(bin_edges) == args.num_bins + 1):
+                    raise ValueError(
+                        "Number of bin edge must be one more than "
+                        "number of bins")
+            else:
+                bin_edges = None
+            processor, bin_edges = Bed.binIntervals(
+                processor,
+                num_bins=args.num_bins,
+                method=args.binning_method,
+                bin_edges=bin_edges)
+            E.info("# split bed: bin_edges=%s" % (str(bin_edges)))
+
+        elif method == "block":
+            processor = Bed.blocked_iterator(processor)
+        elif method == "shift":
+            # IMS: test that contig sizes are availible
+            if not contigs:
+                raise ValueError("please supply genome file")
+            processor = shiftIntervals(
+                processor, contigs, offset=args.offset)
+        # IMS: new method: extend intervals by set amount
+        elif method == "extend":
+            if not contigs:
+                raise ValueError("please supply genome file")
+            processor = extendInterval(processor, contigs, args.offset)
+        elif method == "filter-names":
+            if not args.names:
+                raise ValueError("please supply list of names to filter")
+            names = [name.strip() for name in open(args.names)]
+            processor = filterNames(processor, names)
+        elif method == "rename-chr":
+            if not chr_map:
+                raise ValueError("please supply mapping file")
+            processor = renameChromosomes(processor, chr_map)
+
+    noutput = 0
+    for bed in processor:
+        args.stdout.write(str(bed) + "\n")
+        noutput += 1
 
-    if len(unknown) != 2:
-        raise ValueError(
-            "please specify one bam- or wig-file and one bed file")
-
-    if args.control_files:
-        E.info("using control files: %s" % ",".join(args.control_files))
-
-    infile, bedfile = unknown
-    control_files = []
-
-    if args.format == "bigwig":
-        fg_file = pyBigWig.open(infile)
-        for control_file in args.control_files:
-            control_files.append(pyBigWig.open(control_file))
-        counter = bam2peakshape.CounterBigwig(
-            smooth_method=args.smooth_method)
-
-    elif args.format == "bam":
-        fg_file = pysam.AlignmentFile(infile, "rb")
-        for control_file in args.control_files:
-            control_files.append(pysam.AlignmentFile(control_file, "rb"))
-        counter = bam2peakshape.CounterBam(
-            shift=args.shift,
-            smooth_method=args.smooth_method)
-
-    features_per_interval, bins = buildDensityMatrices(
-        Bed.iterator(iotools.open_file(bedfile)),
-        fg_file,
-        control_files,
-        counter,
-        window_size=args.window_size,
-        bin_size=args.bin_size,
-        strand_specific=args.strand_specific,
-        centring_method=args.centring_method,
-        use_interval=args.use_interval,
-        random_shift=args.random_shift,
-        smooth_method=args.smooth_method,
-        report_step=args.report_step)
-
-    if len(features_per_interval) == 0:
-        E.warn("no data - no output")
-        E.stop()
-        return
-
-    outputFeatureTable(args.stdout, features_per_interval, bins)
-
-    # apply normalization
-    # Note: does not normalize control?
-    # Needs reworking, currently it does not normalize across
-    # all samples nor does the work "sum" reflect the per million
-    # normalization.
-    if args.normalization == "sum":
-        E.info("starting sum normalization")
-        # get total counts across all intervals
-        norm = 0.0
-        for foreground, bed, controls, shifted in features_per_interval:
-            norm += sum(foreground.counts)
-        # per million
-        norm /= float(1000000)
-        E.info("sum/million normalization with %f" % norm)
-
-        # normalise
-        new_data = []
-        for foreground, bed, controls, shifted in features_per_interval:
-            foreground = foreground._replace(
-                counts=numpy.array(foreground.counts,
-                                   dtype=numpy.float) / norm)
-            new_controls = []
-            for control in controls:
-                new_controls.append(
-                    control._replace(
-                        counts=numpy.array(control.counts,
-                                           dtype=numpy.float) / norm))
-            if shifted:
-                shifted = shifted._replace(
-                    counts=numpy.array(shifted.counts,
-                                       dtype=numpy.float) / norm)
-            new_data.append(IntervalData._make((
-                foreground, bed, new_controls, shifted)))
-        features_per_interval = new_data
-    else:
-        E.info("no normalization performed")
-
-    # center bins
-    out_bins = bins[:-1] + args.bin_size
-
-    # build tracks
-    def _toTrack(filename):
-        return os.path.splitext(os.path.basename(filename))[0]
-
-    outputMatrices(features_per_interval,
-                   out_bins,
-                   foreground_track=_toTrack(infile),
-                   control_tracks=[_toTrack(x) for x in args.control_files],
-                   shifted=args.random_shift,
-                   sort_orders=args.sort_orders)
+    E.info("noutput=%i" % (noutput))
 
-    # write footer and output benchmark information.
     E.stop()
 
 
 if __name__ == "__main__":
     sys.exit(main(sys.argv))
```

### Comparing `cgat-0.6.5/cgat/tools/bam2stats.py` & `cgat-0.7.0/cgat/tools/bam2stats.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/tools/bam2wiggle.py` & `cgat-0.7.0/cgat/tools/bam2wiggle.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/tools/bam2window_stats.py` & `cgat-0.7.0/cgat/tools/bam2window_stats.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/tools/bam_compare_alignments.py` & `cgat-0.7.0/cgat/tools/bam_compare_alignments.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/tools/bam_pileup2tsv.py` & `cgat-0.7.0/cgat/tools/bam_pileup2tsv.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/tools/bam_vs_bam.py` & `cgat-0.7.0/cgat/tools/bam_vs_bam.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/tools/bam_vs_bed.py` & `cgat-0.7.0/cgat/tools/bam_vs_bed.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/tools/bam_vs_gtf.py` & `cgat-0.7.0/cgat/tools/bam_vs_gtf.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/tools/bams2bam.py` & `cgat-0.7.0/cgat/tools/bams2bam.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/tools/bcl2fastq.py` & `cgat-0.7.0/cgat/tools/bcl2fastq.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/tools/bed2fasta.py` & `cgat-0.7.0/cgat/tools/bed2fasta.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/tools/bed2gff.py` & `cgat-0.7.0/cgat/tools/bed2gff.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/tools/bed2graph.py` & `cgat-0.7.0/cgat/tools/bed2graph.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/tools/bed2stats.py` & `cgat-0.7.0/cgat/tools/bed2stats.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/tools/bed2table.py` & `cgat-0.7.0/cgat/tools/bed2table.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/tools/bed_vs_bed.py` & `cgat-0.7.0/cgat/tools/bed_vs_bed.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/tools/beds2beds.py` & `cgat-0.7.0/cgat/tools/beds2beds.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/tools/beds2counts.py` & `cgat-0.7.0/cgat/tools/beds2counts.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/tools/cat_tables.py` & `cgat-0.7.0/cgat/tools/cgat_script_template.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,83 +1,59 @@
-"""
-cat_tables.py - concatenate tables
-==================================
+'''
+cgat_script_template.py - template for cgat scripts
+====================================================
 
+:Author:
 :Tags: Python
 
 Purpose
 -------
 
-concatenate tables. Headers of subsequent files are ignored.
+.. Overall purpose and function of the script>
 
 Usage
 -----
 
+.. Example use case
+
+Example::
+
+   python cgat_script_template.py
+
 Type::
 
-   python <script_name>.py --help
+   python cgat_script_template.py --help
 
 for command line help.
 
 Command line options
 --------------------
 
-"""
+'''
 
 import sys
-import fileinput
-
 import cgatcore.experiment as E
 
 
 def main(argv=None):
     """script main.
-
     parses command line options in sys.argv, unless *argv* is given.
     """
 
-    if not argv:
+    if argv is None:
         argv = sys.argv
 
     # setup command line parser
     parser = E.ArgumentParser(description=__doc__)
 
-    parser.add_argument("--version", action='version', version="1.0")
-
-    parser.set_defaults(
-    )
+    parser.add_argument("-t", "--test", dest="test", type=str,
+                        help="supply help")
 
     # add common options (-h/--help, ...) and parse command line
-    (args, unknown) = E.start(parser,
-                              argv=argv,
-                              unknowns=True)
-
-    if len(unknown) == 0 or (len(unknown) == 1 and unknown[0] == "-"):
-        infile = args.stdin
-    else:
-        infile = fileinput.FileInput(args)
-
-    # do sth
-    ninput, nskipped, noutput = 0, 0, 0
-
-    header = False
-
-    for line in infile:
-        ninput += 1
-        if line.startswith("#"):
-            pass
-        elif not header:
-            header = line
-        elif line == header:
-            nskipped += 1
-            continue
-
-        args.stdout.write(line)
-        noutput += 1
-
-    E.info("ninput=%i, noutput=%i, nskipped=%i" % (ninput, noutput, nskipped))
+    (args) = E.start(parser, argv=argv)
 
     # write footer and output benchmark information.
     E.stop()
 
+
 if __name__ == "__main__":
     sys.exit(main(sys.argv))
```

### Comparing `cgat-0.6.5/cgat/tools/cgat2dot.py` & `cgat-0.7.0/cgat/tools/cgat2dot.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/tools/cgat_fasta2cDNA.py` & `cgat-0.7.0/cgat/tools/csv2csv.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,76 +1,76 @@
 '''
-cgat_fasta2cDNA.py - converting multi-fasta of exon features into a multi-fasta of spliced cDNAs/RNAs
-======================================================================================================
+csv2csv.py - operate on tables
+==============================
 
 :Tags: Python
 
 Purpose
 -------
 
+operate on tables.
+
 Usage
 -----
 
-.. Example use case
-
 Example::
 
-   python cgat_fasta2cDNA.py
+   python csv2csv.py --help
 
 Type::
 
-   python cgat_fasta2cDNA.py --help
+   python csv2csv.py --help
 
 for command line help.
 
 Command line options
 --------------------
 
 '''
-
 import sys
+import csv
 import cgatcore.experiment as E
 import cgatcore.iotools as iotools
 
 
-def makeSplicedFasta(infile):
-    '''
-    Merge fasta sequences together into a single
-    spliced transcript sequence
-    '''
-
-    fasta_dict = {}
-    with iotools.open_file(infile) as fafile:
-        for line in fafile.readlines():
-            if line[0] == '>':
-                header = line.rstrip("\n")
-                fasta_dict[header] = ''
-            else:
-                fasta_dict[header] += line.rstrip("\n")
-
-    for key, value in sorted(fasta_dict.items()):
-        yield "%s\n%s\n" % (key, value)
-
-
 def main(argv=None):
     """script main.
+
     parses command line options in sys.argv, unless *argv* is given.
     """
 
     if argv is None:
         argv = sys.argv
 
-    # setup command line parser
     parser = E.ArgumentParser(description=__doc__)
 
-    # add common options (-h/--help, ...) and parse command line
-    (args) = E.start(parser, argv=argv)
+    parser.add_argument("--version", action='version', version="1.0")
+
+    parser.add_argument(
+        "-s", "--method=sort --sort-order", dest="sort", type=str,
+        help="fields to take (in sorted order).")
+
+    (args) = E.start(parser, add_csv_options=True)
+
+    reader = csv.DictReader(E.stdin, dialect=args.csv_dialect)
+
+    if args.sort:
+        fields = args.sort.split(",")
+    else:
+        fields = None
+
+    writer = csv.DictWriter(E.stdout,
+                            fields,
+                            dialect=args.csv_dialect,
+                            lineterminator=args.csv_lineterminator,
+                            extrasaction='ignore')
+
+    E.stdout.write("\t".join(fields) + "\n")
 
-    infile = argv[-1]
-    for record in makeSplicedFasta(infile):
-        options.stdout.write(record)
+    for row in reader:
+        row = iotools.convertDictionary(row)
+        writer.writerow(row)
 
-    # write footer and output benchmark information.
     E.stop()
 
 if __name__ == "__main__":
     sys.exit(main(sys.argv))
```

### Comparing `cgat-0.6.5/cgat/tools/cgat_get_options.py` & `cgat-0.7.0/cgat/tools/cgat_get_options.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/tools/cgat_rebuild_extensions.py` & `cgat-0.7.0/cgat/tools/cgat_rebuild_extensions.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/tools/csvs2csv.py` & `cgat-0.7.0/cgat/tools/csvs2csv.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/tools/data2histogram.py` & `cgat-0.7.0/cgat/tools/data2histogram.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/tools/diff_bam.py` & `cgat-0.7.0/cgat/tools/diff_bam.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/tools/diff_bed.py` & `cgat-0.7.0/cgat/tools/diff_bed.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,15 +113,15 @@
                 raise Exception(
                     "error while processing %s, msg=%s" % (filename, msg))
             if len(intervals) == 0:
                 continue
 
             nexons_overlapping += 1
             start, end = this.start, this.end
-            counts = numpy.zeros(end - start, numpy.int)
+            counts = numpy.zeros(end - start, numpy.int64)
             for other_start, other_end, other_value in intervals:
                 for x in range(max(start, other_start) - start, min(end, other_end) - start):
                     counts[x] += 1
             nbases_overlapping += sum([1 for x in counts if x > 0])
 
         infile.close()
 
@@ -199,15 +199,15 @@
                 except KeyError:
                     continue
 
                 if len(intervals) == 0:
                     continue
 
                 nexons_overlapping += 1
-                counts = numpy.zeros(end - start, numpy.int)
+                counts = numpy.zeros(end - start, numpy.int64)
                 for other_start, other_end, other_value in intervals:
                     for x in range(max(start, other_start) - start, min(end, other_end) - start):
                         counts[x] += 1
                 nbases_overlapping += sum([1 for x in counts if x > 0])
 
         return nexons, nexons_overlapping, nbases, nbases_overlapping
```

### Comparing `cgat-0.6.5/cgat/tools/diff_chains.py` & `cgat-0.7.0/cgat/tools/diff_chains.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/tools/diff_fasta.py` & `cgat-0.7.0/cgat/tools/diff_fasta.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/tools/diff_gtf.py` & `cgat-0.7.0/cgat/tools/diff_gtf.py`

 * *Files 0% similar despite different names*

```diff
@@ -190,15 +190,15 @@
 
             if len(intervals) == 0:
                 continue
 
             overlapping_genes.add(this.gene_id)
             nexons_overlapping += 1
             start, end = this.start, this.end
-            counts = numpy.zeros(end - start, numpy.int)
+            counts = numpy.zeros(end - start, numpy.int64)
             for other_start, other_end, other_value in intervals:
                 for x in range(max(start, other_start) - start, min(end, other_end) - start):
                     counts[x] += 1
             nbases_overlapping += sum([1 for x in counts if x > 0])
 
         infile.close()
```

### Comparing `cgat-0.6.5/cgat/tools/extract_stats.py` & `cgat-0.7.0/cgat/tools/extract_stats.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/tools/fasta2bed.py` & `cgat-0.7.0/cgat/tools/fasta2bed.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/tools/fasta2fasta.py` & `cgat-0.7.0/cgat/tools/fasta2fasta.py`

 * *Files 0% similar despite different names*

```diff
@@ -218,15 +218,15 @@
         help="sequence type (aa or na) . This option determines "
         "which characters to use for masking.")
 
     parser.add_argument(
         "-l", "--template-identifier", dest="template_identifier",
         type=str,
         help="template for numerical identifier"
-        "for the operation --build-map. A %i is replaced by the position "
+        "for the operation --build-map. A %%i is replaced by the position "
         "of the sequence in the file.")
 
     parser.add_argument(
         "--map-tsv-file", dest="map_tsv_file",
         type=str,
         help="input filename with map for identifiers. The first row is a header")
```

### Comparing `cgat-0.6.5/cgat/tools/fasta2fastq.py` & `cgat-0.7.0/cgat/tools/fasta2fastq.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/tools/fasta2kmercontent.py` & `cgat-0.7.0/cgat/tools/fasta2kmercontent.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/tools/fasta2stats.py` & `cgat-0.7.0/cgat/tools/fasta2stats.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/tools/fasta2table.py` & `cgat-0.7.0/cgat/tools/fasta2table.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/tools/fasta2variants.py` & `cgat-0.7.0/cgat/tools/fasta2variants.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/tools/fasta2vcf.py` & `cgat-0.7.0/cgat/tools/fasta2vcf.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/tools/fastas2fasta.py` & `cgat-0.7.0/cgat/tools/fastas2fasta.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/tools/fastq2fasta.py` & `cgat-0.7.0/cgat/tools/fastq2fasta.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/tools/fastq2fastq.py` & `cgat-0.7.0/cgat/tools/fastq2fastq.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/tools/fastq2summary.py` & `cgat-0.7.0/cgat/tools/fastq2summary.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/tools/fastq2table.py` & `cgat-0.7.0/cgat/tools/fastq2table.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/tools/fastq2tpm.py` & `cgat-0.7.0/cgat/tools/fastq2tpm.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/tools/fastq2tsv.py` & `cgat-0.7.0/cgat/tools/fastq2tsv.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/tools/fastqs2fasta.py` & `cgat-0.7.0/cgat/tools/fastqs2fasta.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/tools/fastqs2fastq.py` & `cgat-0.7.0/cgat/tools/fastqs2fastq.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/tools/fastqs2fastqs.py` & `cgat-0.7.0/cgat/tools/fastqs2fastqs.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/tools/genome_bed.py` & `cgat-0.7.0/cgat/tools/genome_bed.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/tools/gff2bed.py` & `cgat-0.7.0/cgat/tools/gff2bed.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/tools/gff2coverage.py` & `cgat-0.7.0/cgat/tools/gff2coverage.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/tools/gff2fasta.py` & `cgat-0.7.0/cgat/tools/gff2fasta.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/tools/gff2gff.py` & `cgat-0.7.0/cgat/tools/gff2gff.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/tools/gff2histogram.py` & `cgat-0.7.0/cgat/tools/gff2histogram.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/tools/gff2psl.py` & `cgat-0.7.0/cgat/tools/gff2psl.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/tools/gff2stats.py` & `cgat-0.7.0/cgat/tools/gff2stats.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/tools/gff2table.py` & `cgat-0.7.0/cgat/tools/gff2table.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/tools/gff32gtf.py` & `cgat-0.7.0/cgat/tools/gff32gtf.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/tools/gtf2fasta.py` & `cgat-0.7.0/cgat/tools/gtf2fasta.py`

 * *Files 1% similar despite different names*

```diff
@@ -466,15 +466,14 @@
     E.info("started counting")
     outfile = E.open_output_file("counts")
     outputCounts(outfile, annotations)
     outfile.close()
 
     E.info("started output")
     for k in sorted(annotations.keys()):
-        # options.stdout.write(">%s\n%s\n" % (k, annotations[k].tostring()))
         options.stdout.write(">%s\n%s\n" % (k, "".join(annotations[k])))
 
 
 def main(argv=None):
     """script main.
 
     parses command line options in sys.argv, unless *argv* is given.
```

### Comparing `cgat-0.6.5/cgat/tools/gtf2gff.py` & `cgat-0.7.0/cgat/tools/gtf2gff.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/tools/gtf2gtf.py` & `cgat-0.7.0/cgat/tools/gtf2gtf.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/tools/gtf2table.py` & `cgat-0.7.0/cgat/tools/gtf2table.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/tools/gtf2tsv.py` & `cgat-0.7.0/cgat/tools/gtf2tsv.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/tools/gtfs2tsv.py` & `cgat-0.7.0/cgat/tools/gtfs2tsv.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/tools/index2bed.py` & `cgat-0.7.0/cgat/tools/index2bed.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/tools/index_fasta.py` & `cgat-0.7.0/cgat/tools/index_fasta.py`

 * *Files 0% similar despite different names*

```diff
@@ -156,15 +156,15 @@
                         action="store_true",
                         help="remove X/x from DNA sequences - they cause "
                         "errors in exonerate.")
 
     parser.add_argument("--allow-duplicates", dest="allow_duplicates",
                         action="store_true",
                         help="allow duplicate identifiers. Further occurances "
-                        "of an identifier are suffixed by an '_\\%i' ")
+                        "of an identifier are suffixed by an '_%%i' ")
 
     parser.add_argument("--regex-identifier", dest="regex_identifier",
                         type=str,
                         help="regular expression for extracting the "
                         "identifier from fasta description line.")
 
     parser.add_argument("--force-output", dest="force", action="store_true",
```

### Comparing `cgat-0.6.5/cgat/tools/split_fasta.py` & `cgat-0.7.0/cgat/tools/split_fasta.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/tools/split_file.py` & `cgat-0.7.0/cgat/tools/split_file.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/tools/split_gff.py` & `cgat-0.7.0/cgat/tools/split_gff.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/tools/table2stats.py` & `cgat-0.7.0/cgat/tools/table2stats.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/tools/table2table.py` & `cgat-0.7.0/cgat/tools/table2table.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/tools/tables2table.py` & `cgat-0.7.0/cgat/tools/tables2table.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/tools/vcf2tsv.py` & `cgat-0.7.0/cgat/tools/vcf2tsv.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/tools/vcf2vcf.py` & `cgat-0.7.0/cgat/tools/vcf2vcf.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/tools/vcf_compare_phase.py` & `cgat-0.7.0/cgat/tools/vcf_compare_phase.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/tools/vcf_stats.py` & `cgat-0.7.0/cgat/tools/vcf_stats.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/tools/vcf_vs_vcf.py` & `cgat-0.7.0/cgat/tools/vcf_vs_vcf.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/tools/vcfstats2db.py` & `cgat-0.7.0/cgat/tools/vcfstats2db.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat/tools/wig2bed.py` & `cgat-0.7.0/cgat/tools/wig2bed.py`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/cgat.egg-info/PKG-INFO` & `cgat-0.7.0/cgat.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,24 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: cgat
-Version: 0.6.5
+Version: 0.7.0
 Summary: cgat : the Computational Genomics Analysis Toolkit
 Home-page: http://www.cgat.org/cgat/Tools/
 Author: Andreas Heger
 Author-email: andreas.heger@gmail.com
 License: MIT
-Description: cgat : the Computational Genomics Analysis Toolkit
 Keywords: computational genomics
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
+License-File: LICENSE
+License-File: COPYING
+
+cgat : the Computational Genomics Analysis Toolkit
```

### Comparing `cgat-0.6.5/cgat.egg-info/SOURCES.txt` & `cgat-0.7.0/cgat.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+COPYING
 LICENSE
 MANIFEST.in
 README.md
 THANKS.txt
 install.sh
 requires.txt
 setup.py
@@ -28,24 +29,22 @@
 cgat/MEME.py
 cgat/Masker.py
 cgat/MatrixTools.py
 cgat/Motifs.py
 cgat/RLE.py
 cgat/RateEstimation.py
 cgat/SVGdraw.py
-cgat/SequencePairProperties.py
 cgat/SequenceProperties.py
 cgat/SetTools.py
 cgat/Sra.py
 cgat/Stats.py
 cgat/Tree.py
 cgat/TreeTools.py
 cgat/VCF.py
 cgat/Variants.py
-cgat/WrapperCodeML.py
 cgat/__init__.py
 cgat/cgat.py
 cgat/dictzip.py
 cgat/makeGeneset.py
 cgat/version.py
 cgat.egg-info/PKG-INFO
 cgat.egg-info/SOURCES.txt
@@ -64,61 +63,45 @@
 cgat/NCL/_cnestedlist.pxd
 cgat/NCL/cnestedlist.pyx
 cgat/NCL/default.h
 cgat/NCL/intervaldb.c
 cgat/NCL/intervaldb.h
 cgat/VCFTools/vcftools.pyx
 cgat/tools/__init__.py
-cgat/tools/bam2UniquePairs.py
 cgat/tools/bam2bam.py
 cgat/tools/bam2bam_split_reads.py
 cgat/tools/bam2bed.py
 cgat/tools/bam2depth.py
 cgat/tools/bam2fasta.py
 cgat/tools/bam2fastq.py
 cgat/tools/bam2geneprofile.py
-cgat/tools/bam2libtype.py
-cgat/tools/bam2peakshape.py
 cgat/tools/bam2stats.py
 cgat/tools/bam2wiggle.py
 cgat/tools/bam2window_stats.py
 cgat/tools/bam_compare_alignments.py
 cgat/tools/bam_pileup2tsv.py
 cgat/tools/bam_vs_bam.py
 cgat/tools/bam_vs_bed.py
 cgat/tools/bam_vs_gtf.py
 cgat/tools/bams2bam.py
 cgat/tools/bcl2fastq.py
-cgat/tools/bed2annotator.py
 cgat/tools/bed2bed.py
 cgat/tools/bed2fasta.py
 cgat/tools/bed2gff.py
 cgat/tools/bed2graph.py
-cgat/tools/bed2plot.py
 cgat/tools/bed2stats.py
 cgat/tools/bed2table.py
 cgat/tools/bed_vs_bed.py
 cgat/tools/beds2beds.py
 cgat/tools/beds2counts.py
-cgat/tools/cat_tables.py
 cgat/tools/cgat2dot.py
-cgat/tools/cgat2rdf.py
-cgat/tools/cgat_fasta2cDNA.py
 cgat/tools/cgat_get_options.py
 cgat/tools/cgat_rebuild_extensions.py
 cgat/tools/cgat_script_template.py
-cgat/tools/chain2psl.py
-cgat/tools/combine_tables.py
 cgat/tools/csv2csv.py
-cgat/tools/csv2db.py
-cgat/tools/csv_cut.py
-cgat/tools/csv_intersection.py
-cgat/tools/csv_rename.py
-cgat/tools/csv_select.py
-cgat/tools/csv_set.py
 cgat/tools/csvs2csv.py
 cgat/tools/data2histogram.py
 cgat/tools/diff_bam.py
 cgat/tools/diff_bed.py
 cgat/tools/diff_chains.py
 cgat/tools/diff_fasta.py
 cgat/tools/diff_gtf.py
@@ -155,24 +138,25 @@
 cgat/tools/gtf2gff.py
 cgat/tools/gtf2gtf.py
 cgat/tools/gtf2table.py
 cgat/tools/gtf2tsv.py
 cgat/tools/gtfs2tsv.py
 cgat/tools/index2bed.py
 cgat/tools/index_fasta.py
-cgat/tools/medip_merge_intervals.py
-cgat/tools/randomize_lines.py
-cgat/tools/rnaseq_junction_bam2bam.py
 cgat/tools/split_fasta.py
 cgat/tools/split_file.py
 cgat/tools/split_gff.py
 cgat/tools/table2stats.py
 cgat/tools/table2table.py
 cgat/tools/tables2table.py
-cgat/tools/transfac2transfac.py
 cgat/tools/vcf2tsv.py
 cgat/tools/vcf2vcf.py
 cgat/tools/vcf_compare_phase.py
 cgat/tools/vcf_stats.py
 cgat/tools/vcf_vs_vcf.py
 cgat/tools/vcfstats2db.py
-cgat/tools/wig2bed.py
+cgat/tools/wig2bed.py
+tests/testComponents.py
+tests/test_commandline.py
+tests/test_import.py
+tests/test_scripts.py
+tests/test_style.py
```

### Comparing `cgat-0.6.5/install.sh` & `cgat-0.7.0/install.sh`

 * *Files identical despite different names*

### Comparing `cgat-0.6.5/setup.py` & `cgat-0.7.0/setup.py`

 * *Files identical despite different names*

