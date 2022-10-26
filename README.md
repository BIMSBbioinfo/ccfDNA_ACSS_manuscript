# **Cardiovascular disease biomarkers derived from circulating cell-free DNA methylation**



The following scripts are contained within this repository and provide the 
analysis workflows that lead to data and figures of the publication 
"Cardiovascular disease biomarkers derived from circulating cell-free DNA 
methylation". 

Raw tabix (and bigwig) files are publically available for 
discovery and validation cohort and can be downloaded via the links below. 

## **Scripts**
The main content of each script is stated below:


#### **cardiac_cfDNA_inital.Rmd**
- Alignment, coverage and methylation statistics discovery cohort
- Tiling of discovery cohort
- Comparative differential methylation (DM) analysis with healthy controls of discovery cohort
- GREAT gene set enrichment analysis for discovery differentially methylated regions (DMRs)


#### **cell_proportions.Rmd**
- Prediction of cell/tissue type proportions
- Plotting of Figure 2


#### **annotation_DMRs_discovery.Rmd**
- Annotation of DMRs to CpG islands, CpG shores, CpG shelves, and inter-CGI
- Annotation of DMRs to 1-5Kb, promoters, 5'UTRs, exons, introns, and 3'UTRs
- DisGNet enrichment analysis for discovery DMRs


#### **disease_spec_CpGs.Rmd**
- Design of probes for targeted sequencing of validation cohort using methylation atlas


#### **check_methyl_ACS.Rmd**
- Assign targeted sequenced results for validation cohort to coordinates
- Get statistics for validation cohort

#### **Targeted_Seq_Normalization_and_DMR_Validation.Rmd**
- Visualization and removal of sequencing bias between WGBS and targeted sequencing
- Validation of DMRS distinguishing between disease conditions (identified from discovery cohort)
- Plotting of Figure 6 and Suplementary Figure S6


#### **descriptive_stats.Rmd**
- Correlation analysis clinical markers
- Distribution clinical markers per disease condition
- Bisulfite conversion rates
- Average CpG coverage
- Amount ccfDNA analysis
- Identification of 254 DMRs associated with disease groups on linear models
- Plotting Figure 1, 3, 4, 5 and Supplementary Figure S1 and S2


#### **report_DMRs.Rmd**
- builds upon **ranking_v3.Rmd**
- DMR analysis comparing each disease group vs. healthy controls
- Plotting of Supplementary Figure S4


#### **ranking_v3.Rmd**
- annotates DMRs for the groups, adding gene info, GO, phenotype associations, DO and disgenet associations


#### **RoadMap_enrichment.Rmd**
- Enrichment analysis, Fisher's exact test for cell types on DMRs
- Plotting of Figure S5


#### **validation_ACS.Rmd**
- Transfer DMRs distinguishing between disease conditions from discovery to validation cohort
- Plotting of Supplementary Figure S3


## **Data availability**
All raw **methylKit objects** (tabix format) for the discovery and validation 
cohort can be downloaded from the respective files provided in the "data" folder 
within this repository. bigwig files are also available from the respective file 
for the discovery cohort only, however.


