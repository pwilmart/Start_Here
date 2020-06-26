# Start_Here
### Navigation links (and brief descriptions) to my repositories.

* [Start_Here](https://github.com/pwilmart/Start_Here) - This repository

* [pwilmart.github.io](https://github.com/pwilmart/pwilmart.github.io) - Account website repository

---

## Software

* [PAW_pipeline](https://github.com/pwilmart/PAW_pipeline) - The PAW/Comet proteomics pipeline

* [fasta_utilities](https://github.com/pwilmart/fasta_utilities) - Utilities for downloading and prepping FASTA files

* [utilities](https://github.com/pwilmart/utilities) - Some miscellaneous utility scripts

* [annotations](https://github.com/pwilmart/annotations) - Scripts for adding UniProt annotations to results lists

* [PAW_BLAST](https://github.com/pwilmart/PAW_BLAST) - Scripts for BLAST ortholog matching

* [Z-score_GUI](https://github.com/pwilmart/Z-score_GUI) - Script for sliding-window Z-score analyses

---

## Analyses

* [PXD017823_Real-Time-Search](https://github.com/pwilmart/PXD017823_Real-Time-Search) - Analysis of some real time search data
  * [Schweppe_RTS_by-method](https://pwilmart.github.io/PXD017823_Real-Time-Search/Schweppe_RTS_by-method.html) - Compares the older SPS MS3 acquisition method to the new real time search (RTS) acquisition method
  > Note: RTS acquisition used a protein close-out feature to limit redundant acquisition of peptides from abundant proteins

  * [PXD017823_RTS_comparisons_IRS](https://pwilmart.github.io/PXD017823_Real-Time-Search/PXD017823_RTS_comparisons_IRS.html) - Compares cell line expression with edgeR for the RTS data (not the IRS adjusted values)
  * [PXD017823_Regular_comparisons] (https://pwilmart.github.io/PXD017823_Real-Time-Search/PXD017823_Regular_comparisons.html) - Compares cell line expression with edgeR for the regular SPS MS3 data (not the IRS adjusted values)
  * [PXD017823_RTS_comparisons_IRS](https://pwilmart.github.io/PXD017823_Real-Time-Search/PXD017823_RTS_comparisons_IRS.html) - Compares cell line expression with edgeR for the RTS data after IRS
  * [PXD017823_Regular_comparisons_IRS](https://pwilmart.github.io/PXD017823_Real-Time-Search/PXD017823_Regular_comparisons_IRS.html) - Compares cell line expression with edgeR for the regular SPS MS3 data after IRS


#### Internal Reference Scaling

* [IRS_validation](https://github.com/pwilmart/IRS_validation) - Validation and background for the Internal Reference Scaling method
  * [IRS_validation](https://pwilmart.github.io/TMT_analysis_examples/IRS_validation.html) - Notebook with more background on IRS and true IRS validation  
  * [auto_finder_BIND-473](https://pwilmart.github.io/TMT_analysis_examples/auto_finder_BIND-473.html) - Notebook showing how to verify that reference channels are correctly assigned

* [IRS_normalization](https://github.com/pwilmart/IRS_normalization) - Example of the IRS method
  * [understanding_IRS]() - Notebook covering normalization details
  * [statistical_testing]() - Notebook demonstrating edgeR testing
  * [statistical_testing_ratios]() - Notebook where ratios to the reference channel are computed and tested using limma
  * [statistical_testing_take2]() - More statistical testing of P0 vs P3 time points


* [Plubell_2017_PAW](https://github.com/pwilmart/Plubell_2017_PAW) - Reanalysis of original IRS paper's data

#### PAW TMT analyses

* [MaxQuant_and_PAW](https://github.com/pwilmart/MaxQuant_and_PAW) - Comparison of PAW and MaxQuant with same TMT data (KUR1502 project)
  * [Comet/PAW](https://pwilmart.github.io/TMT_analysis_examples/KUR1502_PAW.html) - Single-plex TMT analysis using my Comet/PAW pipeline
  * [Comet/PAW edgeR vs t-test](https://pwilmart.github.io/TMT_analysis_examples/KUR1502_PAW_t-test.html) - Comparison of edgeR to t-test statistical testing
  * [Comet/PAW edgeR vs limma](https://pwilmart.github.io/TMT_analysis_examples/KUR1502_PAW_limma.html) - Comparison of edgeR to limma statistical modeling
  * [Comet/PAW limma-voom]() - Comparison of edgeR to limma-voom (fancier normalization and trended variance)
  * [MaxQuant analysis](https://pwilmart.github.io/TMT_analysis_examples/KUR1502_MQ.html) - KUR1502 project analyzed with MaxQuant

* [Multiple_TMT_MQ](https://github.com/pwilmart/Multiple_TMT_MQ) - Example of IRS method using MaxQuant analysis of the developing mouse lens data
  * [Multiple-TMT with MQ](https://pwilmart.github.io/TMT_analysis_examples/multiple_TMT_MQ.html) - three TMT plexes combined with IRS from MaxQuant results

* [Dilution_series](https://github.com/pwilmart/Dilution_series) - Comparison of PSM, peptide, and protein level data for a dilution series of TMT-labeled mouse membrane proteome
  * [Dilution series](https://pwilmart.github.io/TMT_analysis_examples/MAN1353_peptides_proteins.html) - Dilution series of mouse brain TMT-labeled digest

#### Other TMT analyses

* [TMT_analysis_examples](https://github.com/pwilmart/TMT_analysis_examples) - Descriptions of various TMT analyses
  * Less complete repository "switchyard"

* [Yeast_CarbonSources](https://github.com/pwilmart/Yeast_CarbonSources) - Gygi Lab TMT data from yeast grown with different sugars
  * [Comet/PAW pipeline](https://pwilmart.github.io/TMT_analysis_examples/CarbonSources_part-1.html) - Re-analysis of data using Comet/PAW pipeline
  * [MaxQuant](https://pwilmart.github.io/TMT_analysis_examples/CarbonSources_MQ.html) - Re-analysis of same data with MaxQuant

* [Yeast_triple_KO_TMT](https://github.com/pwilmart/Yeast_triple_KO_TMT) - Gygi Lab yeast triple knockout (TKO) data
  * [Yeast TKO](https://pwilmart.github.io/TMT_analysis_examples/Triple_KO.html) - Comparison of platforms and methods for TMT interference


* [PXD001077_P-furiosus](https://github.com/pwilmart/PXD001077_P-furiosus) - Not yet completed

* [Metaplastic-BC_PXD014414](https://github.com/pwilmart/Metaplastic-BC_PXD014414) - Reanalysis of a 3-plex, 27-sample cancer study demonstrating IRS
  * [PXD014414_comparisons_major](https://pwilmart.github.io/Metaplastic-BC_PXD014414/PXD014414_comparisons_major.html) - Notebook for comparisons of normal to triple negative to metaplastic samples
  * [PXD014414_comparisons_subtypes](https://pwilmart.github.io/Metaplastic-BC_PXD014414/PXD014414_comparisons_subtypes.html) - Notebook for comparisons of metaplastic subtypes

* [BCP-ALL_QE-TMT_Nat-Comm-2019](https://github.com/pwilmart/BCP-ALL_QE-TMT_Nat-Comm-2019) - A 3-plex, 27-sample MS2-based TMT study of cancer data
  * [Nat-Comm-2019_TMT_QE_pools](https://pwilmart.github.io/TMT_analysis_examples/Nat-Comm-2019_TMT_QE_pools.html) - Uses single pooled channel for IRS method
  * [Nat-Comm-2019_TMT_QE_averages](https://pwilmart.github.io/TMT_analysis_examples/Nat-Comm-2019_TMT_QE_averages.html) - Slightly better IRS results using plex averages

#### MS2 Reporter Ions

* [PXD013277_E-coli_spike-ins_MS2-TMT](https://github.com/pwilmart/PXD013277_E-coli_spike-ins_MS2-TMT) - E. coli proteome spiked into a human background

* [SPS-MS3_vs_MS2_TMT](https://github.com/pwilmart/SPS-MS3_vs_MS2_TMT) - Comparison of MS2 TMT and SPS MS3 TMT for same data

* [JPR-201712_MS2-MS3](https://github.com/pwilmart/JPR-201712_MS2-MS3) - A comparison of MS2 and SPS MS3 data for an E. coli background

* [PXD004163_Notebooks](https://github.com/pwilmart/PXD004163_Notebooks/tree/master) - More MS2 data to illustrate using notebooks

#### Spectral Counting

* [Smith_SpC_2018](https://github.com/pwilmart/Smith_SpC_2018) - Quantitative analysis of large SpC dataset

* [Sea_lion_urine_SpC](https://github.com/pwilmart/Sea_lion_urine_SpC) - Analysis of sea lion urine samples

* [ABRF_iPRG_2015_SpC](https://github.com/pwilmart/ABRF_iPRG_2015_SpC) - Analysis of ABRF iPRG data from 2015 study

---

## Meetings

* [talk_to_repo_example](https://github.com/pwilmart/talk_to_repo_example) - How to turn meeting content into repositories

* [ABRF_2020](https://github.com/pwilmart/ABRF_2020) - How to use GitHub to support scientific research

* [ASMS-2013_search-engine-comparison](https://github.com/pwilmart/ASMS-2013_search-engine-comparison) - How to compare search engines

* [ASMS_2018](https://github.com/pwilmart/ASMS_2018) - The Internal Reference Scaling (IRS) method

* [Cascadia_2013](https://github.com/pwilmart/Cascadia_2013) - Extended parsimony protein grouping

* [Cascadia_2018](https://github.com/pwilmart/Cascadia_2018) - A tour of Jupyter notebooks

* [RECOMB-CP_2012](https://github.com/pwilmart/RECOMB-CP_2012) - How to analyze shotgun proteomics data

---

## Forked Repositories

* [Reference_Proteome_Manager](https://github.com/pwilmart/Reference_Proteome_Manager)

* [tmt-normalization](https://github.com/pwilmart/tmt-normalization)

* [spectrum_utils](https://github.com/pwilmart/spectrum_utils)

* [RawQuant](https://github.com/pwilmart/RawQuant)

* [RawTools](https://github.com/pwilmart/RawTools)

* [stats337](https://github.com/pwilmart/stats337)
