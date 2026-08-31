# Curated Reading List

This reading list supports the entries in the main repository. It favors primary papers, methodological evaluations, and conceptual reviews that are useful when designing, benchmarking, or interpreting microbial pangenome analyses.

## How to use this list

A pangenome study should begin with the biological question and sampling design, not a preferred software package. For every analysis, record:

1. Genome source, inclusion criteria, taxonomy, and dereplication method.
2. Assembly quality and contamination criteria.
3. Annotation software, database version, and parameters.
4. Homology clustering method and identity/coverage thresholds.
5. Definition of core and accessory categories.
6. Treatment of paralogs, fragmented genes, and recombination.
7. Software versions, commands, random seeds, and all downstream filters.

## Foundations and terminology

1. Tettelin H, et al. 2005. Genome analysis of multiple pathogenic isolates of *Streptococcus agalactiae*: implications for the microbial “pan-genome”. *PNAS*. [doi:10.1073/pnas.0506758102](https://doi.org/10.1073/pnas.0506758102)  
   Foundational microbial pan-genome paper.

2. Medini D, et al. 2005. The microbial pan-genome. *Current Opinion in Genetics & Development*. [doi:10.1016/j.gde.2005.09.006](https://doi.org/10.1016/j.gde.2005.09.006)  
   Early conceptual framework.

3. Vernikos G, et al. 2015. Ten years of pan-genome analyses. *Current Opinion in Microbiology*. [doi:10.1016/j.mib.2014.11.016](https://doi.org/10.1016/j.mib.2014.11.016)  
   Historical review of microbial pangenome analysis.

4. McInerney JO, et al. 2017. Why prokaryotes have pangenomes. *Nature Microbiology*. [doi:10.1038/nmicrobiol.2017.140](https://doi.org/10.1038/nmicrobiol.2017.140)  
   Evolutionary framing of gene-content diversity.

5. Matthews CA, et al. 2024. A gentle introduction to pangenomics. *Briefings in Bioinformatics*. [doi:10.1093/bib/bbae588](https://doi.org/10.1093/bib/bbae588)  
   Clear terminology across gene, sequence, and graph pangenomes.

## Gene-cluster pangenome methods

6. Page AJ, et al. 2015. Roary: rapid large-scale prokaryote pan genome analysis. *Bioinformatics*. [doi:10.1093/bioinformatics/btv421](https://doi.org/10.1093/bioinformatics/btv421)  
   Fast, widely used gene-cluster framework.

7. Tonkin-Hill G, et al. 2020. Producing polished prokaryotic pangenomes with the Panaroo pipeline. *Genome Biology*. [doi:10.1186/s13059-020-02090-4](https://doi.org/10.1186/s13059-020-02090-4)  
   Addresses annotation and assembly artifacts through a gene-neighborhood graph.

8. Gautreau G, et al. 2020. PPanGGOLiN: depicting microbial diversity via a partitioned pangenome graph. *PLoS Computational Biology*. [doi:10.1371/journal.pcbi.1007732](https://doi.org/10.1371/journal.pcbi.1007732)  
   Models persistent, shell, and cloud gene families while using genomic neighborhoods.

9. Bayliss SC, et al. 2019. PIRATE: a fast and scalable pangenomics toolbox for clustering diverged orthologues in bacteria. *GigaScience*. [doi:10.1093/gigascience/giz119](https://doi.org/10.1093/gigascience/giz119)  
   Multi-threshold clustering for populations with heterogeneous sequence divergence.

10. Zhou Z, et al. 2020. Accurate reconstruction of bacterial pan- and core genomes with PEPPAN. *Genome Biology*. [doi:10.1186/s13059-020-02195-w](https://doi.org/10.1186/s13059-020-02195-w)  
    Scalable pangenome reconstruction with explicit ortholog/paralog handling.

11. Le DQ, et al. 2024. Efficient inference of large prokaryotic pangenomes with PanTA. *Genome Biology*. [doi:10.1186/s13059-024-03362-z](https://doi.org/10.1186/s13059-024-03362-z)  
    Incremental, large-collection pangenome inference.

12. Bu C, et al. 2025. PGAP2: a comprehensive toolkit for prokaryotic pan-genome analysis. *Nature Communications*. [doi:10.1038/s41467-025-64846-5](https://doi.org/10.1038/s41467-025-64846-5)  
    Recent framework with quality-aware pangenome analysis features.

## Sequence and graph pangenomes

13. Garrison E, et al. 2018. Variation graph toolkit improves read mapping by representing genetic variation in the reference. *Nature Biotechnology*. [doi:10.1038/nbt.4227](https://doi.org/10.1038/nbt.4227)  
    Core variation-graph representation and toolkit.

14. Guarracino A, et al. 2022. ODGI: understanding pangenome graphs. *Bioinformatics*. [doi:10.1093/bioinformatics/btac328](https://doi.org/10.1093/bioinformatics/btac328)  
    Efficient graph manipulation and path-aware visualization.

15. Noll N, et al. 2023. PanGraph: scalable bacterial pan-genome graph construction. *PLoS Computational Biology*. [doi:10.1371/journal.pcbi.1011105](https://doi.org/10.1371/journal.pcbi.1011105)  
    Graph construction targeted to bacterial sequence and structural diversity.

16. Liao WW, et al. 2023. A draft human pangenome reference. *Nature*. [doi:10.1038/s41586-023-05896-x](https://doi.org/10.1038/s41586-023-05896-x)  
    A non-microbial exemplar of modern reference pangenome practice.

17. Computational Pan-Genomics Consortium. 2018. Computational pan-genomics: status, promises and challenges. *Briefings in Bioinformatics*. [doi:10.1093/bib/bbw089](https://doi.org/10.1093/bib/bbw089)  
    Broad computational framework, including graph representations.

## Data quality, taxonomy, and annotation

18. Jain C, et al. 2018. High throughput ANI analysis of 90K prokaryotic genomes reveals clear species boundaries. *Nature Communications*. [doi:10.1038/s41467-018-07641-9](https://doi.org/10.1038/s41467-018-07641-9)  
    FastANI and ANI-based species delimitation.

19. Parks DH, et al. 2020. A complete domain-to-species taxonomy for Bacteria and Archaea. *Nature Biotechnology*. [doi:10.1038/s41587-020-0501-8](https://doi.org/10.1038/s41587-020-0501-8)  
    Genome Taxonomy Database framework.

20. Chklovski A, et al. 2023. CheckM2: a rapid, scalable, and accurate tool for assessing microbial genome quality using machine learning. *Nature Methods*. [doi:10.1038/s41592-023-01870-3](https://doi.org/10.1038/s41592-023-01870-3)  
    Genome completeness and contamination estimation.

21. Orakov A, et al. 2021. GUNC: detection of chimerism and contamination in prokaryotic genomes. *Genome Biology*. [doi:10.1186/s13059-021-02593-3](https://doi.org/10.1186/s13059-021-02593-3)  
    Contamination and chimerism detection.

22. Schwengers O, et al. 2021. Bakta: rapid and standardized annotation of bacterial genomes via alignment-free sequence identification. *Microbial Genomics*. [doi:10.1099/mgen.0.000685](https://doi.org/10.1099/mgen.0.000685)  
    Standardized annotation designed for comparability.

## Benchmarking and interpretation

23. Urhan A, et al. 2021. A comparative study of pan-genome methods for microbial genomics. *Microbial Genomics*. [doi:10.1099/mgen.0.000690](https://doi.org/10.1099/mgen.0.000690)  
    Comparison of several gene-cluster pangenome methods.

24. Hyun JC, et al. 2022. Comparative pangenomics: analysis of 12 microbial pathogen pangenomes reveals gene conservation and diversity. *Genome Biology*. [doi:10.1186/s13059-021-02529-9](https://doi.org/10.1186/s13059-021-02529-9)  
    Comparative pangenome methodology across pathogens.

25. Dunne WM, et al. 2021. The pangenome is a useful but imperfect representation of bacterial diversity. *Trends in Microbiology*. [doi:10.1016/j.tim.2021.03.009](https://doi.org/10.1016/j.tim.2021.03.009)  
    Interpretative cautions and limitations.

26. Rouli L, et al. 2015. The bacterial pangenome as a new tool for analysing bacterial diversity. *New Microbes and New Infections*. [doi:10.1016/j.nmni.2015.06.005](https://doi.org/10.1016/j.nmni.2015.06.005)  
    Practical concepts for bacterial pangenome interpretation.

## Metapangenomics and visualization

27. Delmont TO, et al. 2020. Anvi'o: an advanced analysis and visualization platform for 'omics data. *PeerJ*. [doi:10.7717/peerj.1319](https://doi.org/10.7717/peerj.1319)  
    Integrated analysis and visualization platform.

28. Hadfield J, et al. 2018. Phandango: an interactive viewer for bacterial population genomics. *Bioinformatics*. [doi:10.1093/bioinformatics/btx610](https://doi.org/10.1093/bioinformatics/btx610)  
    Tree-aligned visualization of gene presence, metadata, recombination, and associations.

29. Seemann T. 2014. Prokka: rapid prokaryotic genome annotation. *Bioinformatics*. [doi:10.1093/bioinformatics/btu153](https://doi.org/10.1093/bioinformatics/btu153)  
    Widely used annotation baseline.

30. Arnoux J, et al. 2026. PANORAMA: a robust pangenome-based method for predicting and comparing biological systems across species. *PLoS Computational Biology*. [doi:10.1371/journal.pcbi.1013856](https://doi.org/10.1371/journal.pcbi.1013856)  
    A recent pangenome-graph application for system prediction and comparison.

## Suggested reading order

1. Tettelin 2005, Matthews 2024, and McInerney 2017 for concepts.
2. FastANI, GTDB, CheckM2, GUNC, and Bakta before building a pangenome.
3. Roary, Panaroo, PPanGGOLiN, PIRATE, and PEPPAN for gene-family methods.
4. PanGraph, PGGB, vg, and ODGI for sequence and graph methods.
5. Urhan 2021 and Hyun 2022 before making biological claims from a single tool or threshold.
