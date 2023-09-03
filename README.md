# **Cardiovascular disease biomarkers derived from circulating cell-free DNA methylation**



The following scripts are contained within this repository and provide the 
analysis workflows that lead to data and figures of the publication 
"Cardiovascular disease biomarkers derived from circulating cell-free DNA 
methylation". 

Raw tabix (and bigwig) files with associated metadata are publically available for 
discovery and validation cohort and can be downloaded via the links [below](#data-availability). 

## **Scripts**
The main content of each script is stated below:


#### [**cardiac_cfDNA_initial.Rmd**](scripts/cardiac_cfDNA_initial.Rmd)
- Alignment, coverage and methylation statistics discovery cohort
- Tiling of discovery cohort
- Comparative differential methylation (DM) analysis with healthy controls of discovery cohort
- GREAT gene set enrichment analysis for discovery differentially methylated regions (DMRs)


#### [**cell_proportions.Rmd**](scripts/cell_proportions.Rmd)
- Prediction of cell/tissue type proportions
- Plotting of Figure 2


#### [**annotation_DMRs_discovery.Rmd**](scripts/annotation_DMRs_discovery.Rmd)
- Annotation of DMRs to CpG islands, CpG shores, CpG shelves, and inter-CGI
- Annotation of DMRs to 1-5Kb, promoters, 5'UTRs, exons, introns, and 3'UTRs
- DisGNet enrichment analysis for discovery DMRs


#### [**disease_spec_CpGs.Rmd**](scripts/disease_spec_CpGs.Rmd)
- Design of probes for targeted sequencing of validation cohort using methylation atlas


#### [**check_methyl_ACS.Rmd**](scripts/check_methyl_ACS.Rmd)
- Assign targeted sequenced results for validation cohort to coordinates
- Get statistics for validation cohort

#### [**Targeted_Seq_Normalisation_and_DMR_Validation.Rmd**](scripts/Targeted_Seq_Normalisation_and_DMR_Validation.Rmd)
- Visualization and removal of sequencing bias between WGBS and targeted sequencing
- Validation of DMRS distinguishing between disease conditions (identified from discovery cohort)
- Plotting of Figure 6 and Suplementary Figure S6


#### [**descriptive_stats.Rmd**](scripts/descriptive_stats.Rmd)
- Correlation analysis clinical markers
- Distribution clinical markers per disease condition
- Bisulfite conversion rates
- Average CpG coverage
- Amount ccfDNA analysis
- Identification of 254 DMRs associated with disease groups on linear models
- Plotting Figure 1, 3, 4, 5 and Supplementary Figure S1 and S2


#### [**report_DMRs.Rmd**](scripts/report_DMRs.Rmd)
- builds upon **ranking_v3.Rmd**
- DMR analysis comparing each disease group vs. healthy controls
- Plotting of Supplementary Figure S4


#### [**ranking_v3.Rmd**](scripts/ranking_v3.Rmd)
- annotates DMRs for the groups, adding gene info, GO, phenotype associations, DO and disgenet associations


#### [**RoadMap_enrichment.Rmd**](scripts/RoadMap_enrichment.Rmd)
- Enrichment analysis, Fisher's exact test for cell types on DMRs
- Plotting of Figure S5


#### [**validation_ACS.Rmd**](scripts/validation_ACS.Rmd)
- Transfer DMRs distinguishing between disease conditions from discovery to validation cohort
- Plotting of Supplementary Figure S3



#### [**building_multivariate_predictive_model_narrowDMRs_ACS.Rmd**](scripts/building_multivariate_predictive_model_narrowDMRs_ACS.Rmd)
- Build predictive models to test multivariate predictive power of the 193 DMRs shared from discovery analysis and validation amples.

#### [**evaluate_cellType_signature_matrix.Rmd**](scripts/evaluate_cellType_signature_matrix.Rmd)
-  evaluate the performance of our extended reference atlas/ CpG signature matrix compared to the comprehensive reference atlas generated by Moss et al (2018).


## **Data availability**
Download links for raw **methylKit objects** (tabix format) are provided for the [discovery](data/methylKit_objects_discovery_cohort.tsv) and [validation cohort](data/methylKit_objects_validation_cohort.tsv). Corresponding patient metadata are provided as tsv files for [discovery](data/PatientCharacteristics_ccfDNA_Manuscript_cfDNA_WGBS.tsv) and [validation](data/PatientCharacteristics_ccfDNA_Manuscript_cfDNA_target_validation.tsv) cohorts.
Links to **BigWig** files are available for the [discovery cohort](data/bigwig_files_discovery_cohort.tsv).


