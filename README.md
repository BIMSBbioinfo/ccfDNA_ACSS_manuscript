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


#### **ranking_v3.Rmd
- annotates DMRs for the groups, adding gene info, GO, phenotype associations, DO and disgenet associations


#### **RoadMap_enrichment.Rmd
- Enrichment analysis, Fisher's exact test for cell types on DMRs
- Plotting of Figure S5


#### **validation_ACS.Rmd**
- Transfer DMRs distinguishing between disease conditions from discovery to validation cohort
- Plotting of Supplementary Figure S3


## **Data availability**
All raw **methylKit objects** (tabix format) can be downloaded from the following links:

#### **Discovery cohort**
- Sample_AC1: https://bimsbstatic.mdc-berlin.de/akalin/ccfDNA_ACSS_manuscript/methylKit_objects_discovery_cohort/AC1_CpG_filtered.txt.bgz
- Sample_AC2: https://bimsbstatic.mdc-berlin.de/akalin/ccfDNA_ACSS_manuscript/methylKit_objects_discovery_cohort/AC2_CpG_filtered.txt.bgz
- Sample_AC3: https://bimsbstatic.mdc-berlin.de/akalin/ccfDNA_ACSS_manuscript/methylKit_objects_discovery_cohort/AC3_CpG_filtered.txt.bgz
- Sample_AC4: https://bimsbstatic.mdc-berlin.de/akalin/ccfDNA_ACSS_manuscript/methylKit_objects_discovery_cohort/AC4_CpG_filtered.txt.bgz
- Sample_AC5: https://bimsbstatic.mdc-berlin.de/akalin/ccfDNA_ACSS_manuscript/methylKit_objects_discovery_cohort/AC5_CpG_filtered.txt.bgz
- Sample_AC6: https://bimsbstatic.mdc-berlin.de/akalin/ccfDNA_ACSS_manuscript/methylKit_objects_discovery_cohort/AC6_CpG_filtered.txt.bgz
- Sample_AC7: https://bimsbstatic.mdc-berlin.de/akalin/ccfDNA_ACSS_manuscript/methylKit_objects_discovery_cohort/AC7_CpG_filtered.txt.bgz
- Sample_AC8: https://bimsbstatic.mdc-berlin.de/akalin/ccfDNA_ACSS_manuscript/methylKit_objects_discovery_cohort/AC8_CpG_filtered.txt.bgz
- Sample_AC9: https://bimsbstatic.mdc-berlin.de/akalin/ccfDNA_ACSS_manuscript/methylKit_objects_discovery_cohort/AC9_CpG_filtered.txt.bgz
- Sample_AC10: https://bimsbstatic.mdc-berlin.de/akalin/ccfDNA_ACSS_manuscript/methylKit_objects_discovery_cohort/AC10_CpG_filtered.txt.bgz
- Sample_AC11: https://bimsbstatic.mdc-berlin.de/akalin/ccfDNA_ACSS_manuscript/methylKit_objects_discovery_cohort/AC11_CpG_filtered.txt.bgz
- Sample_AC12: https://bimsbstatic.mdc-berlin.de/akalin/ccfDNA_ACSS_manuscript/methylKit_objects_discovery_cohort/AC12_CpG_filtered.txt.bgz
- Sample_AC13: https://bimsbstatic.mdc-berlin.de/akalin/ccfDNA_ACSS_manuscript/methylKit_objects_discovery_cohort/AC13_CpG_filtered.txt.bgz
- Sample_AC14: https://bimsbstatic.mdc-berlin.de/akalin/ccfDNA_ACSS_manuscript/methylKit_objects_discovery_cohort/AC14_CpG_filtered.txt.bgz
- Sample_AC15: https://bimsbstatic.mdc-berlin.de/akalin/ccfDNA_ACSS_manuscript/methylKit_objects_discovery_cohort/AC15_CpG_filtered.txt.bgz
- Sample_AP1: https://bimsbstatic.mdc-berlin.de/akalin/ccfDNA_ACSS_manuscript/methylKit_objects_discovery_cohort/AP1_CpG_filtered.txt.bgz
- Sample_AP2: https://bimsbstatic.mdc-berlin.de/akalin/ccfDNA_ACSS_manuscript/methylKit_objects_discovery_cohort/AP2_CpG_filtered.txt.bgz
- Sample_AP3: https://bimsbstatic.mdc-berlin.de/akalin/ccfDNA_ACSS_manuscript/methylKit_objects_discovery_cohort/AP3_CpG_filtered.txt.bgz
- Sample_AP4: https://bimsbstatic.mdc-berlin.de/akalin/ccfDNA_ACSS_manuscript/methylKit_objects_discovery_cohort/AP4_CpG_filtered.txt.bgz
- Sample_AP5: https://bimsbstatic.mdc-berlin.de/akalin/ccfDNA_ACSS_manuscript/methylKit_objects_discovery_cohort/AP5_CpG_filtered.txt.bgz
- Sample_AP6: https://bimsbstatic.mdc-berlin.de/akalin/ccfDNA_ACSS_manuscript/methylKit_objects_discovery_cohort/AP6_CpG_filtered.txt.bgz
- Sample_H26: https://bimsbstatic.mdc-berlin.de/akalin/ccfDNA_ACSS_manuscript/methylKit_objects_discovery_cohort/H26_CpG_filtered.txt.bgz
- Sample_H28: https://bimsbstatic.mdc-berlin.de/akalin/ccfDNA_ACSS_manuscript/methylKit_objects_discovery_cohort/H28_CpG_filtered.txt.bgz
- Sample_N1: https://bimsbstatic.mdc-berlin.de/akalin/ccfDNA_ACSS_manuscript/methylKit_objects_discovery_cohort/N1_CpG_filtered.txt.bgz
- Sample_N2: https://bimsbstatic.mdc-berlin.de/akalin/ccfDNA_ACSS_manuscript/methylKit_objects_discovery_cohort/N2_CpG_filtered.txt.bgz
- Sample_N3: https://bimsbstatic.mdc-berlin.de/akalin/ccfDNA_ACSS_manuscript/methylKit_objects_discovery_cohort/N3_CpG_filtered.txt.bgz
- Sample_N4: https://bimsbstatic.mdc-berlin.de/akalin/ccfDNA_ACSS_manuscript/methylKit_objects_discovery_cohort/N4_CpG_filtered.txt.bgz
- Sample_N5: https://bimsbstatic.mdc-berlin.de/akalin/ccfDNA_ACSS_manuscript/methylKit_objects_discovery_cohort/N5_CpG_filtered.txt.bgz
- Sample_N6: https://bimsbstatic.mdc-berlin.de/akalin/ccfDNA_ACSS_manuscript/methylKit_objects_discovery_cohort/N6_CpG_filtered.txt.bgz


#### **Validation cohort**
- Sample_2017: https://bimsbstatic.mdc-berlin.de/akalin/ccfDNA_ACSS_manuscript/methylKit_objects_validation_cohort/2017_1_val_1_bt2.sorted.deduped_cpg.txt.bgz
- Sample_2018: https://bimsbstatic.mdc-berlin.de/akalin/ccfDNA_ACSS_manuscript/methylKit_objects_validation_cohort/2018_1_val_1_bt2.sorted.deduped_cpg.txt.bgz
- Sample_2019: https://bimsbstatic.mdc-berlin.de/akalin/ccfDNA_ACSS_manuscript/methylKit_objects_validation_cohort/2019_1_val_1_bt2.sorted.deduped_cpg.txt.bgz
- Sample_2026: https://bimsbstatic.mdc-berlin.de/akalin/ccfDNA_ACSS_manuscript/methylKit_objects_validation_cohort/2026_1_val_1_bt2.sorted.deduped_cpg.txt.bgz
- Sample_2027: https://bimsbstatic.mdc-berlin.de/akalin/ccfDNA_ACSS_manuscript/methylKit_objects_validation_cohort/2027_1_val_1_bt2.sorted.deduped_cpg.txt.bgz
- Sample_2033: https://bimsbstatic.mdc-berlin.de/akalin/ccfDNA_ACSS_manuscript/methylKit_objects_validation_cohort/2033_1_val_1_bt2.sorted.deduped_cpg.txt.bgz
- Sample_3052: https://bimsbstatic.mdc-berlin.de/akalin/ccfDNA_ACSS_manuscript/methylKit_objects_validation_cohort/3052_1_val_1_bt2.sorted.deduped_cpg.txt.bgz
- Sample_3131: https://bimsbstatic.mdc-berlin.de/akalin/ccfDNA_ACSS_manuscript/methylKit_objects_validation_cohort/3131_1_val_1_bt2.sorted.deduped_cpg.txt.bgz
- Sample_3158: https://bimsbstatic.mdc-berlin.de/akalin/ccfDNA_ACSS_manuscript/methylKit_objects_validation_cohort/3158_1_val_1_bt2.sorted.deduped_cpg.txt.bgz
- Sample_VF: https://bimsbstatic.mdc-berlin.de/akalin/ccfDNA_ACSS_manuscript/methylKit_objects_validation_cohort/VF_1_val_1_bt2.sorted.deduped_cpg.txt.bgz
- Sample_SK: https://bimsbstatic.mdc-berlin.de/akalin/ccfDNA_ACSS_manuscript/methylKit_objects_validation_cohort/SK_1_val_1_bt2.sorted.deduped_cpg.txt.bgz




All **bigwig files** for the discovery cohort are available from the following links:

#### **Discovery cohort**
- Sample_AC1: https://bimsbstatic.mdc-berlin.de/akalin/ccfDNA_ACSS_manuscript/bigwig_objects_discovery_cohort/AC1.bw
- Sample_AC2: https://bimsbstatic.mdc-berlin.de/akalin/ccfDNA_ACSS_manuscript/bigwig_objects_discovery_cohort/AC2.bw
- Sample_AC3: https://bimsbstatic.mdc-berlin.de/akalin/ccfDNA_ACSS_manuscript/bigwig_objects_discovery_cohort/AC3.bw
- Sample_AC4: https://bimsbstatic.mdc-berlin.de/akalin/ccfDNA_ACSS_manuscript/bigwig_objects_discovery_cohort/AC4.bw
- Sample_AC5: https://bimsbstatic.mdc-berlin.de/akalin/ccfDNA_ACSS_manuscript/bigwig_objects_discovery_cohort/AC5.bw
- Sample_AC6: https://bimsbstatic.mdc-berlin.de/akalin/ccfDNA_ACSS_manuscript/bigwig_objects_discovery_cohort/AC6.bw
- Sample_AC7: https://bimsbstatic.mdc-berlin.de/akalin/ccfDNA_ACSS_manuscript/bigwig_objects_discovery_cohort/AC7.bw
- Sample_AC8: https://bimsbstatic.mdc-berlin.de/akalin/ccfDNA_ACSS_manuscript/bigwig_objects_discovery_cohort/AC8.bw
- Sample_AC9: https://bimsbstatic.mdc-berlin.de/akalin/ccfDNA_ACSS_manuscript/bigwig_objects_discovery_cohort/AC9.bw
- Sample_AC10: https://bimsbstatic.mdc-berlin.de/akalin/ccfDNA_ACSS_manuscript/bigwig_objects_discovery_cohort/AC10.bw
- Sample_AC11: https://bimsbstatic.mdc-berlin.de/akalin/ccfDNA_ACSS_manuscript/bigwig_objects_discovery_cohort/AC11.bw
- Sample_AC12: https://bimsbstatic.mdc-berlin.de/akalin/ccfDNA_ACSS_manuscript/bigwig_objects_discovery_cohort/AC12.bw
- Sample_AC13: https://bimsbstatic.mdc-berlin.de/akalin/ccfDNA_ACSS_manuscript/bigwig_objects_discovery_cohort/AC13.bw
- Sample_AC14: https://bimsbstatic.mdc-berlin.de/akalin/ccfDNA_ACSS_manuscript/bigwig_objects_discovery_cohort/AC14.bw
- Sample_AC15: https://bimsbstatic.mdc-berlin.de/akalin/ccfDNA_ACSS_manuscript/bigwig_objects_discovery_cohort/AC15.bw
- Sample_AP1: https://bimsbstatic.mdc-berlin.de/akalin/ccfDNA_ACSS_manuscript/bigwig_objects_discovery_cohort/AP1.bw
- Sample_AP2: https://bimsbstatic.mdc-berlin.de/akalin/ccfDNA_ACSS_manuscript/bigwig_objects_discovery_cohort/AP2.bw
- Sample_AP3: https://bimsbstatic.mdc-berlin.de/akalin/ccfDNA_ACSS_manuscript/bigwig_objects_discovery_cohort/AP3.bw
- Sample_AP4: https://bimsbstatic.mdc-berlin.de/akalin/ccfDNA_ACSS_manuscript/bigwig_objects_discovery_cohort/AP4.bw
- Sample_AP5: https://bimsbstatic.mdc-berlin.de/akalin/ccfDNA_ACSS_manuscript/bigwig_objects_discovery_cohort/AP5.bw
- Sample_AP6: https://bimsbstatic.mdc-berlin.de/akalin/ccfDNA_ACSS_manuscript/bigwig_objects_discovery_cohort/AP6.bw
- Sample_H26: https://bimsbstatic.mdc-berlin.de/akalin/ccfDNA_ACSS_manuscript/bigwig_objects_discovery_cohort/H26.bw
- Sample_H28: https://bimsbstatic.mdc-berlin.de/akalin/ccfDNA_ACSS_manuscript/bigwig_objects_discovery_cohort/H28.bw
- Sample_N1: https://bimsbstatic.mdc-berlin.de/akalin/ccfDNA_ACSS_manuscript/bigwig_objects_discovery_cohort/N1.bw
- Sample_N2: https://bimsbstatic.mdc-berlin.de/akalin/ccfDNA_ACSS_manuscript/bigwig_objects_discovery_cohort/N2.bw
- Sample_N3: https://bimsbstatic.mdc-berlin.de/akalin/ccfDNA_ACSS_manuscript/bigwig_objects_discovery_cohort/N3.bw
- Sample_N4: https://bimsbstatic.mdc-berlin.de/akalin/ccfDNA_ACSS_manuscript/bigwig_objects_discovery_cohort/N4.bw
- Sample_N5: https://bimsbstatic.mdc-berlin.de/akalin/ccfDNA_ACSS_manuscript/bigwig_objects_discovery_cohort/N5.bw
- Sample_N6: https://bimsbstatic.mdc-berlin.de/akalin/ccfDNA_ACSS_manuscript/bigwig_objects_discovery_cohort/N6.bw


