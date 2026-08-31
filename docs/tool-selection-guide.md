# Choosing a Microbial Pangenome Approach

This guide helps select a method based on the biological question and the data available. It is a starting point, not a substitute for a sensitivity analysis.

## First decide what variation matters

| Primary question | Recommended representation | Starting tools |
|---|---|---|
| Which gene families are shared or variable? | Gene-cluster pangenome | Panaroo, PPanGGOLiN, PIRATE, PEPPAN, Roary |
| How does gene order or genomic context vary? | Gene-neighborhood graph | PPanGGOLiN, Panakeia, clinker |
| Which nucleotide alleles and structural variants are present? | Sequence or variation graph | PanGraph, PGGB, vg, ODGI |
| Is a gene associated with a phenotype after population correction? | Gene or k-mer association model | pyseer; Scoary for exploratory screening |
| Does recombination obscure a core-genome phylogeny? | Recombination-aware core alignment | Gubbins, ClonalFrameML, IQ-TREE |

## Choose the input set carefully

Use a coherent taxonomic scope. Screen assemblies for completeness, contamination, chimerism, and duplication before comparative analysis. Standardize annotation whenever possible, because inconsistent gene calling can look like biological accessory-gene variation.

A practical preparation set is:

1. Confirm taxonomy with GTDB-Tk and estimate relatedness with ANI.
2. Dereplicate near-identical genomes when sampling is uneven.
3. Evaluate quality with CheckM2, GUNC, and assembly statistics.
4. Annotate all genomes with the same software version and database.
5. Record every inclusion rule and parameter.

## Match the method to the dataset

| Situation | Good starting choice | Why |
|---|---|---|
| Closely related bacterial isolates, consistent high-quality GFF files | Roary or Panaroo | Fast gene-family analysis; Panaroo is useful when assemblies are fragmented |
| Diverse species-level collection | PIRATE or PEPPAN | Better suited to heterogeneous sequence divergence and paralogy |
| Thousands of genomes or an incrementally growing collection | PPanGGOLiN, PanTA, or PGAP2 | Designed for scale, partitioning, or incremental updates |
| Complete or high-quality assemblies, with structural variation as a key result | PanGraph or PGGB | Retains nucleotide-level and structural alternatives beyond presence/absence |
| A specific genomic island, resistance locus, or biosynthetic cluster | clinker plus an appropriate pangenome graph | Preserves local gene order, orientation, and context |

## Report enough for reproducibility

At minimum, report genome accession numbers, taxonomy and QC rules, annotation method, homology thresholds, core definition, treatment of paralogs, software versions, commands, and downstream filtering. Interpret core, shell, cloud, unique, open, and closed categories as sample- and threshold-dependent observations.

## Read before choosing

- [Panaroo](https://doi.org/10.1186/s13059-020-02090-4)
- [PPanGGOLiN](https://doi.org/10.1371/journal.pcbi.1007732)
- [PIRATE](https://doi.org/10.1093/gigascience/giz119)
- [PEPPAN](https://doi.org/10.1186/s13059-020-02195-w)
- [PanGraph](https://doi.org/10.1099/mgen.0.001034)
- [A gentle introduction to pangenomics](https://doi.org/10.1093/bib/bbae588)
