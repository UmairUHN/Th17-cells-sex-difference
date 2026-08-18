# Transcriptional profiling of male, female and FCG mice derived MOG<sub>[35-55] </sub>-specific Th17 cells in an adoptive transfer model of chronic experimental autoimmune encephalomyelitis 
## Project Overview
This project investigates how **sex chromosomes and sex hormones influence the pathogenicity of Th17 cells** in a chronic autoimmune setting. Using experimental autoimmune encephalomyelitis (EAE), a mouse model of multiple sclerosis, we examined why Th17 cells derived from male and female animals can differ in their ability to induce disease.

Our findings indicate that the increased pathogenicity of male-derived Th17 cells is influenced by both **sex chromosome complement and hormonal environment**, and that these effects are associated with distinct transcriptional and epigenetic regulators.

## Experimental Approach

To dissect the individual contributions of sex chromosomes and sex hormones, we used the **Four Core Genotypes (FCG) mouse model**, which separates chromosomal sex (XX vs. XY) from gonadal sex. These mice were further backcrossed with the **1C6 TCR-transgenic model**, allowing us to generate Th17 cells with a MOG[35-55] specific T-cell receptor background.

By comparing Th17 cells derived from FCG × 1C6 mice with different combinations of sex chromosomes and hormonal environments, we were able to investigate the relative contributions of:

* **Sex chromosome complement (XX vs. XY)**
* **Sex hormone environment**

RNA-seq was used to characterize transcriptional differences between Th17 cell populations with distinct pathogenic potentials and to identify candidate molecular regulators.

## Major Findings

### 1. Male-derived Th17 cells exhibit increased pathogenicity

We initially observed that **male-derived Th17 cells induced more severe EAE** compared with their female counterparts. This suggested that biological sex can influence the pathogenic potential of Th17 cells rather than simply affecting the recipient's response to inflammation.

### 2. Both sex chromosomes and sex hormones influence disease severity

Using the FCG × 1C6 model, we separated the effects of chromosomal sex from the effects of the hormonal environment. Our data indicated that **XX chromosome complement and the female hormonal environment were associated with reduced EAE severity**, demonstrating that both sex chromosomes and sex hormones contribute to the regulation of Th17 pathogenicity.

This experimental design allowed us to distinguish effects that would otherwise be difficult to separate in conventional XX-female/XY-male comparisons.

### 3. SUv39H1 and Pygo1 emerge as candidate regulators

To investigate the molecular mechanisms underlying sex-dependent differences in Th17 pathogenicity, we examined transcriptional differences between Th17 cell populations.

This analysis identified **Suv39h1** and **Pygo1** as putative regulators associated with sex-driven differences in Th17 pathogenicity. These findings suggest that sex-dependent regulation of Th17 cells may involve both **epigenetic mechanisms and Wnt-associated transcriptional pathways**.

### 4. Evidence for parental transgenerational effects

Interestingly, comparisons of FCG × 1C6 mice with similar chromosomal and hormonal characteristics in parent mice (1C6), revealed additional differences in Th17 pathogenicity. These observations suggested the presence of **parent-of-origin/parental genetic effects** that cannot be explained solely by sex chromosome complement or hormonal status.

This finding highlights an additional layer of genetic regulation that may influence the pathogenic phenotype of Th17 cells.

### 5. RUNX2 as a candidate regulator of Th17 pathogenicity

Finally, by comparing RNA-seq profiles from **more pathogenic and less pathogenic Th17 cell populations**, we identified **Runx2** as another putative regulator associated with the pathogenic Th17 phenotype.

Together, these analyses provide candidate molecular mechanisms that may explain why otherwise similar Th17 populations can exhibit substantially different pathogenic potential.

## 6. XY Translocation Effects in FCG Mice

Recent work has identified potential **XY chromosome translocation effects in FCG mice**, including the possibility that genes normally located on the X chromosome may be present in different copy-number configurations between FCG genotypes. Such effects represent a potential confounding factor when interpreting phenotypes attributed solely to sex chromosome complement.

In particular, **Tlr7** has been highlighted as a potential gene of interest in this context. To determine whether potential XY translocation effects could influence the interpretation of our findings, we performed an additional RNA-seq analysis using data generated from **FCG × 1C6-derived Th17 cells**.

We evaluated the genes reported in **PMID: 39394207** and examined their expression across the relevant FCG genotypes. Of the genes identified in that study, none showed significant differences at the protein level in our experimental system. However, several genes showed significant differences at the RNA level.

The **directionality and magnitude of these transcriptional differences** were further examined to determine whether they were consistent with potential chromosome-translocation effects. Although some transcriptional differences were detected, these genes did not represent the major transcriptional regulators associated with the pathogenic Th17 phenotype identified in our analyses.

These results indicate that potential XY translocation-associated effects should be considered when interpreting experiments using FCG mice. However, within our dataset, these effects **do not appear to account for the principal transcriptional differences associated with Th17 pathogenicity** and therefore do not substantially alter the biological interpretation of the findings presented in this project.


## Overall Model

Our findings support a model in which **Th17 cell pathogenicity is shaped by multiple interacting biological factors**, including sex chromosome complement, sex hormones, parental genetic effects, and cell-intrinsic transcriptional and epigenetic programs.

The project therefore provides a framework for understanding how biological sex can influence autoimmune disease through direct effects on pathogenic immune-cell states.


## Data and Analysis

The repository is intended to provide a **transparent and reproducible record of the computational analyses underlying the study**.

**Session Information**

All computational analyses for this project were performed in R/RStudio. The computational environment, including the R version, operating system, and package versions used for the analyses, is documented below to facilitate reproducibility.

The raw FASTQ files (Deposited in the bioproject with accession ID GSE268964) were processed with tirmmoteric and the data was aligned to the mouse genomic reference by kallisto as described in the manuscript. The subsequent analysis was performed in the R studio with the foll

The analyses were performed using R version 4.4.2 on Windows 10 (x64). The primary Bioconductor and CRAN packages used included DESeq2, clusterProfiler, enrichplot, EnhancedVolcano, tximport, ggplot2, tidyverse, GenomicFeatures, AnnotationHub, and related dependencies.

The complete session information is provided below:

> sessionInfo()
R version 4.4.2 (2024-10-31 ucrt)
Platform: x86_64-w64-mingw32/x64
Running under: Windows 10 x64 (build 19045)

Matrix products: default


locale:
[1] LC_COLLATE=English_United States.utf8 
[2] LC_CTYPE=English_United States.utf8   
[3] LC_MONETARY=English_United States.utf8
[4] LC_NUMERIC=C                          
[5] LC_TIME=English_United States.utf8    

time zone: America/New_York
tzcode source: internal

attached base packages:
[1] stats4    stats     graphics  grDevices utils     datasets 
[7] methods   base     

other attached packages:
 [1] enrichplot_1.26.6                        
 [2] ggstance_0.3.7                           
 [3] EnhancedVolcano_1.24.0                   
 [4] ggrepel_0.9.6                            
 [5] TxDb.Mmusculus.UCSC.mm10.knownGene_3.10.0
 [6] GenomicFeatures_1.58.0                   
 [7] clusterProfiler_4.14.6                   
 [8] data.table_1.17.0                        
 [9] org.Mm.eg.db_3.20.0                      
[10] AnnotationHub_3.14.0                     
[11] BiocFileCache_2.14.0                     
[12] dbplyr_2.5.0                             
[13] AnnotationDbi_1.68.0                     
[14] lubridate_1.9.4                          
[15] forcats_1.0.0                            
[16] stringr_1.5.1                            
[17] dplyr_1.1.4                              
[18] purrr_1.0.4                              
[19] readr_2.1.5                              
[20] tidyr_1.3.1                              
[21] tibble_3.2.1                             
[22] ggplot2_3.5.1                            
[23] tidyverse_2.0.0                          
[24] tximport_1.34.0                          
[25] DESeq2_1.46.0                            
[26] SummarizedExperiment_1.36.0              
[27] Biobase_2.66.0                           
[28] MatrixGenerics_1.18.1                    
[29] matrixStats_1.5.0                        
[30] GenomicRanges_1.58.0                     
[31] GenomeInfoDb_1.42.3                      
[32] IRanges_2.40.1                           
[33] S4Vectors_0.44.0                         
[34] BiocGenerics_0.52.0                      

loaded via a namespace (and not attached):
  [1] RColorBrewer_1.1-3       rstudioapi_0.17.1       
  [3] jsonlite_1.9.1           magrittr_2.0.3          
  [5] ggtangle_0.0.6           farver_2.1.2            
  [7] BiocIO_1.16.0            fs_1.6.5                
  [9] zlibbioc_1.52.0          vctrs_0.6.5             
 [11] Rsamtools_2.22.0         memoise_2.0.1           
 [13] RCurl_1.98-1.16          SQUAREM_2021.1          
 [15] ggtree_3.14.0            mixsqp_0.3-54           
 [17] S4Arrays_1.6.0           curl_6.2.1              
 [19] truncnorm_1.0-9          SparseArray_1.6.2       
 [21] gridGraphics_0.5-1       plyr_1.8.9              
 [23] cachem_1.1.0             GenomicAlignments_1.42.0
 [25] igraph_2.1.4             lifecycle_1.0.4         
 [27] pkgconfig_2.0.3          Matrix_1.7-2            
 [29] R6_2.6.1                 fastmap_1.2.0           
 [31] gson_0.1.0               GenomeInfoDbData_1.2.13 
 [33] digest_0.6.37            aplot_0.2.5             
 [35] colorspace_2.1-1         patchwork_1.3.0         
 [37] irlba_2.3.5.1            RSQLite_2.3.9           
 [39] labeling_0.4.3           invgamma_1.1            
 [41] filelock_1.0.3           timechange_0.3.0        
 [43] httr_1.4.7               abind_1.4-8             
 [45] compiler_4.4.2           bit64_4.6.0-1           
 [47] withr_3.0.2              BiocParallel_1.40.0     
 [49] DBI_1.2.3                R.utils_2.13.0          
 [51] rappdirs_0.3.3           DelayedArray_0.32.0     
 [53] rjson_0.2.23             tools_4.4.2             
 [55] ape_5.8-1                R.oo_1.27.0             
 [57] glue_1.8.0               restfulr_0.0.15         
 [59] nlme_3.1-166             GOSemSim_2.32.0         
 [61] grid_4.4.2               reshape2_1.4.4          
 [63] snow_0.4-4               fgsea_1.32.2            
 [65] generics_0.1.3           gtable_0.3.6            
 [67] tzdb_0.4.0               R.methodsS3_1.8.2       
 [69] hms_1.1.3                XVector_0.46.0          
 [71] BiocVersion_3.20.0       pillar_1.10.1           
 [73] yulab.utils_0.2.0        splines_4.4.2           
 [75] treeio_1.30.0            lattice_0.22-6          
 [77] rtracklayer_1.66.0       bit_4.5.0.1             
 [79] tidyselect_1.2.1         GO.db_3.20.0            
 [81] locfit_1.5-9.12          Biostrings_2.74.1       
 [83] gridExtra_2.3            stringi_1.8.4           
 [85] UCSC.utils_1.2.0         lazyeval_0.2.2          
 [87] ggfun_0.1.8              yaml_2.3.10             
 [89] codetools_0.2-20         qvalue_2.38.0           
 [91] BiocManager_1.30.25      ggplotify_0.1.2         
 [93] cli_3.6.4                munsell_0.5.1           
 [95] Rcpp_1.0.14              png_0.1-8               
 [97] XML_3.99-0.18            parallel_4.4.2          
 [99] blob_1.2.4               DOSE_4.0.0              
[101] bitops_1.0-9             tidytree_0.4.6          
[103] scales_1.3.0             crayon_1.5.3            
[105] rlang_1.1.5              ashr_2.2-63             
[107] cowplot_1.1.3            fastmatch_1.1-6         
[109] KEGGREST_1.46.0         
>
> The loaded packages, specific code and meta data for each figure is described in the separate sections.
