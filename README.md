# Start_Here

## Table of Contents:

* [Software](#Software)
* [Analyses](#Analyses)
  * [Internal Reference Scaling](#IRS)
  * [Real Time Search](#RTS)
  * [PAW TMT Analyses](#PAW)
  * [Other TMT Analyses](#Other)
  * [MS2 Reporter Ions](#MS2)
  * [Spectral Counting](#SpC)
* [Meeting Content and Other Presentations](#Meetings)
* [Other Repositories](#Other_repos)

### Navigation links (and brief descriptions) to my repositories.

* [Start_Here](https://github.com/pwilmart/Start_Here) - This repository

* [pwilmart.github.io](https://github.com/pwilmart/pwilmart.github.io) - Account website repository (mostly blog entries)
  * [TMT-zero-replacement](https://pwilmart.github.io/blog/2018/12/12/TMT-zero-replacement) - Blog about replacing missing data in TMT datasets
  * [MaxQuant performance](https://pwilmart.github.io/blog/2019/03/10/MQ-performance) - Blog about how well MaxQuant performs for PSM identification
  * [Quant tool survey](https://pwilmart.github.io/blog/2019/03/12/Quantitative-survey) - Some thoughts about quantitative proteomics tools
  * [pipeline performance](https://pwilmart.github.io/blog/2019/09/08/Keeping-pipeline-flowing) - Some ideas about how to make pipelines more effective
  * [Humpty Dumpty](https://pwilmart.github.io/blog/2019/09/21/shotgun-quantification) - Bog about how to do quantification from shotgun proteomics data
  * [Orthologs and annotations](https://pwilmart.github.io/blog/2019/10/14/orthologs-annotations) - Blog about using ortholog mapping to annotate proteomics results
  * [TMT ratio distortion](https://pwilmart.github.io/blog/2020/01/05/TMT-ratio-distortions) - Understanding TMT ratio distortions
  * [FASTA files and protein inference](https://pwilmart.github.io/blog/2020/01/06/Proteomics-as-house-building) - Blog about how FASTA files and protein inference affect shotgun proteomics results
  * [Proteomics meta data](https://pwilmart.github.io/blog/2020/06/07/Sample-keys) - Thoughts about how to describe proteomic experimental designs
  * [Open Search](https://pwilmart.github.io/blog/2020/07/03/Open-search) - Some caveats to Open search data exploration
  * [Soup to nuts](https://pwilmart.github.io/blog/2020/07/12/Soup-to-nuts) - Overview of typical steps in peptide/protein ID pipelines
  * [How to Excel](https://pwilmart.github.io/blog/2020/07/24/How-to-Excel) - Why I like Excel
  * [Houston, we have a discrepancy](https://pwilmart.github.io/blog/2020/07/28/Houston-we-have-a-discrepancy) - Thoughts on the discrepancy between MSstatsTMT and my analyses
  * [Unique peptides and shotgun quantification](https://pwilmart.github.io/blog/2020/09/19/shotgun-quantification-part2) - How to use unique peptides in quantification
  * [Go big or go home?](https://pwilmart.github.io/blog/2021/04/22/Parent-ion-tolerance) - Are we shooting ourselves in the foot with narrow tolerance database searching?

---

## <a id="Software"></a>Software

* [PAW_pipeline](https://github.com/pwilmart/PAW_pipeline) - The PAW/Comet proteomics pipeline

* [fasta_utilities](https://github.com/pwilmart/fasta_utilities) - Utilities for downloading and prepping FASTA files

* [utilities](https://github.com/pwilmart/utilities) - Some miscellaneous utility scripts

* [annotations](https://github.com/pwilmart/annotations) - Scripts for adding UniProt annotations to results lists

* [PAW_BLAST](https://github.com/pwilmart/PAW_BLAST) - Scripts for BLAST ortholog matching

* [Z-score_GUI](https://github.com/pwilmart/Z-score_GUI) - Script for sliding-window Z-score analyses

---

## <a id="Analyses"></a>Analyses

#### <a id="IRS"></a>Internal Reference Scaling

* [IRS_validation](https://github.com/pwilmart/IRS_validation) - Method overview and validation of Internal Reference Scaling normalization
  * [IRS_validation](https://pwilmart.github.io/TMT_analysis_examples/IRS_validation.html) - Notebook with more background on the IRS method and experimental validation  
  * [auto_finder_BIND-473](https://pwilmart.github.io/TMT_analysis_examples/auto_finder_BIND-473.html) - Notebook showing how to verify that reference channels are correctly assigned

* [IRS_normalization](https://github.com/pwilmart/IRS_normalization) - Example of the IRS method using developing mouse lens data
  * [understanding_IRS](https://pwilmart.github.io/IRS_normalization/understanding_IRS.html) - Notebook covering normalization details
  * [statistical_testing](https://pwilmart.github.io/IRS_normalization/statistical_testing.html) - Notebook demonstrating edgeR testing
  * [statistical_testing_ratios](https://pwilmart.github.io/IRS_normalization/statistical_testing_ratios.html) - Notebook where ratios to the reference channel are computed and tested using limma
  * [statistical_testing_take2](https://pwilmart.github.io/IRS_normalization/statistical_testing_take2.html) - More statistical testing of P0 vs P3 time points

* [Plubell_2017_PAW](https://github.com/pwilmart/Plubell_2017_PAW) - Reanalysis of original IRS [MCP paper's](https://www.mcponline.org/content/16/5/873) data

#### <a id="RTS"></a>Real Time Search

* [PXD017823_Real-Time-Search](https://github.com/pwilmart/PXD017823_Real-Time-Search) - Analysis of some real time search SPS-MS3 TMT data from the Gygi Lab

  * [Schweppe_RTS_by-method](https://pwilmart.github.io/PXD017823_Real-Time-Search/Schweppe_RTS_by-method.html) - Compares the older SPS MS3 acquisition method to the new real time search (RTS) acquisition method (Note: RTS acquisition used a protein close-out feature to limit acquisition of peptides from abundant proteins)
  * [PXD017823_RTS_comparisons_IRS](https://pwilmart.github.io/PXD017823_Real-Time-Search/PXD017823_RTS_comparisons_IRS.html) - Compares cell line expression with edgeR for the RTS data (not the IRS adjusted values)
  * [PXD017823_Regular_comparisons](https://pwilmart.github.io/PXD017823_Real-Time-Search/PXD017823_Regular_comparisons.html) - Compares cell line expression with edgeR for the regular SPS MS3 data (not the IRS adjusted values)
  * [PXD017823_RTS_comparisons_IRS](https://pwilmart.github.io/PXD017823_Real-Time-Search/PXD017823_RTS_comparisons_IRS.html) - Compares cell line expression with edgeR for the RTS data after IRS
  * [PXD017823_Regular_comparisons_IRS](https://pwilmart.github.io/PXD017823_Real-Time-Search/PXD017823_Regular_comparisons_IRS.html) - Compares cell line expression with edgeR for the regular SPS MS3 data after IRS

#### <a id="PAW"></a>PAW TMT analyses

* [MaxQuant_and_PAW](https://github.com/pwilmart/MaxQuant_and_PAW) - Comparison of PAW and MaxQuant with same TMT data (KUR1502 project)
  * [Comet/PAW](https://pwilmart.github.io/TMT_analysis_examples/KUR1502_PAW.html) - Single-plex TMT analysis using my Comet/PAW pipeline
  * [Comet/PAW edgeR vs t-test](https://pwilmart.github.io/TMT_analysis_examples/KUR1502_PAW_t-test.html) - Comparison of edgeR to t-test statistical testing
  * [Comet/PAW edgeR vs limma](https://pwilmart.github.io/TMT_analysis_examples/KUR1502_PAW_limma.html) - Comparison of edgeR to limma statistical modeling
  * [Comet/PAW limma-voom](https://pwilmart.github.io/TMT_analysis_examples/KUR1502_PAW_limma-voom.html) - Comparison of edgeR to limma-voom (TMM normalization and trended variance)
  * [MaxQuant analysis](https://pwilmart.github.io/TMT_analysis_examples/KUR1502_MQ.html) - KUR1502 project analyzed with MaxQuant and edgeR

* [Multiple_TMT_MQ](https://github.com/pwilmart/Multiple_TMT_MQ) - Example of IRS method using MaxQuant analysis of the developing mouse lens data
  * [Multiple-TMT with MQ](https://pwilmart.github.io/TMT_analysis_examples/multiple_TMT_MQ.html) - Three TMT plexes combined with IRS using MaxQuant results

* [Dilution_series](https://github.com/pwilmart/Dilution_series) - Comparison of PSM, peptide, and protein level data for a dilution series of TMT-labeled mouse brain membrane proteins
  * [Dilution series notebook](https://pwilmart.github.io/TMT_analysis_examples/MAN1353_peptides_proteins.html) - Dilution series of mouse brain TMT-labeled digest

#### <a id="Other"></a>Other TMT analyses

* [TMT_analysis_examples](https://github.com/pwilmart/TMT_analysis_examples) - Descriptions of various TMT analyses
  * Another repository "switchyard"

* [Yeast_CarbonSources](https://github.com/pwilmart/Yeast_CarbonSources) - Gygi Lab TMT data from yeast grown with different sugars
  * [Comet/PAW pipeline](https://pwilmart.github.io/TMT_analysis_examples/CarbonSources_part-1.html) - Re-analysis of data using Comet/PAW pipeline
  * [MaxQuant](https://pwilmart.github.io/TMT_analysis_examples/CarbonSources_MQ.html) - Re-analysis of same data with MaxQuant

* [Yeast_triple_KO_TMT](https://github.com/pwilmart/Yeast_triple_KO_TMT) - Gygi Lab yeast triple knockout (TKO) data
  * [Yeast TKO](https://pwilmart.github.io/TMT_analysis_examples/Triple_KO.html) - Comparison of platforms and methods for understanding TMT interference


* [PXD001077_P-furiosus](https://github.com/pwilmart/PXD001077_P-furiosus) - Work in progress...

* [Metaplastic-BC_PXD014414](https://github.com/pwilmart/Metaplastic-BC_PXD014414) - Reanalysis of a 3-plex, 27-sample cancer study demonstrating IRS
  * [PXD014414_comparisons_major](https://pwilmart.github.io/Metaplastic-BC_PXD014414/PXD014414_comparisons_major.html) - Notebook for comparisons of normal, triple negative, and metaplastic samples
  * [PXD014414_comparisons_subtypes](https://pwilmart.github.io/Metaplastic-BC_PXD014414/PXD014414_comparisons_subtypes.html) - Notebook for comparisons of metaplastic subtypes
  * Some other statistical testing methods:
    * [PXD014414_comparisons_major_edgeR-glm](https://pwilmart.github.io/Metaplastic-BC_PXD014414/PXD014414_comparisons_major_edgeR-glm.html) - Uses the glm modeling in edgeR
    * [PXD014414_comparisons_major_TTEST](https://pwilmart.github.io/Metaplastic-BC_PXD014414/PXD014414_comparisons_major_TTEST.html) - Uses a 2-sample t-test
    * [PXD014414_comparisons_major_limma](https://pwilmart.github.io/Metaplastic-BC_PXD014414/PXD014414_comparisons_major_limma.html) - Uses limma on log2 intensities
    * [PXD014414_comparisons_major_voom-limma](https://pwilmart.github.io/Metaplastic-BC_PXD014414/PXD014414_comparisons_major_voom-limma.html) - Uses voom for variance estimate and limma

* [BCP-ALL_QE-TMT_Nat-Comm-2019](https://github.com/pwilmart/BCP-ALL_QE-TMT_Nat-Comm-2019) - A 3-plex, 27-sample MS2-based TMT study of cancer data
  * [Nat-Comm-2019_TMT_QE_pools](https://pwilmart.github.io/TMT_analysis_examples/Nat-Comm-2019_TMT_QE_pools.html) - Uses single pooled channel for IRS method
  * [Nat-Comm-2019_TMT_QE_averages](https://pwilmart.github.io/TMT_analysis_examples/Nat-Comm-2019_TMT_QE_averages.html) - Slightly better IRS results using plex averages

#### <a id="MS2"></a>MS2 Reporter Ions

* [PXD013277_E-coli_spike-ins_MS2-TMT](https://github.com/pwilmart/PXD013277_E-coli_spike-ins_MS2-TMT) - E. coli proteome spiked into a human background
  * [PXD013277_comparisons_human](https://pwilmart.github.io/PXD013277_E-coli_spike-ins_MS2-TMT/PXD013277_comparisons_human.html) - Notebook looking at unchanged human background
  * [PXD013277_comparisons_no-norm](https://pwilmart.github.io/PXD013277_E-coli_spike-ins_MS2-TMT/PXD013277_comparisons_no-norm.html) - Notebook with manually matched human protein levels between spike-in channels
  * [PXD013277_comparisons](https://pwilmart.github.io/PXD013277_E-coli_spike-ins_MS2-TMT/PXD013277_comparisons.html) - Notebook with generic edgeR workup (TMM normalization and exact testing)  

* [SPS-MS3_vs_MS2_TMT](https://github.com/pwilmart/SPS-MS3_vs_MS2_TMT) - Comparison of MS2 TMT and SPS MS3 TMT for same `MORG-75` data
  * [MORG-75_combined](https://pwilmart.github.io/TMT_analysis_examples/MORG-75_combined.html) - Unique use of IRS to combine TMT data between two Orbitrap platforms acquired with different methods
  * [MORG-75_Fusion](https://pwilmart.github.io/TMT_analysis_examples/MORG-75_Fusion.html) - Analysis of the SPS MS3 data
  * [MORG-75_QE](https://pwilmart.github.io/TMT_analysis_examples/MORG-75_QE.html) - Analysis of the Q Exactive MS2 TMT data

* [JPR-201712_MS2-MS3](https://github.com/pwilmart/JPR-201712_MS2-MS3) - A comparison of MS2 and SPS MS3 data for an E. coli background (analysis of the unchanged background)
  * [First analysis](https://pwilmart.github.io/TMT_analysis_examples/MS2MS3_peptides_proteins.html) - Original notebook of how similar the E. coli background is at PSM, peptide, and protein levels
  * [Second analysis](https://pwilmart.github.io/TMT_analysis_examples/JPR-2017_E-coli_MS2-MS3.html) - Newer notebook with a direct comparison of MS2 and SPS-MS3 data
  * [JPR-2017_serum](https://pwilmart.github.io/TMT_analysis_examples/JPR-2017_serum.html) - Notebook looking at depleted serum samples

* [PXD004163_Notebooks](https://github.com/pwilmart/PXD004163_Notebooks/tree/master) - More MS2 data to illustrate using notebooks
  * [PXD004163_comparisons_3-10](https://pwilmart.github.io/PXD004163_Notebooks/PXD004163_comparisons_3-10.html) - Re-analysis with Comet/PAW for the IPG 3-10 range data (72-fractions)
  * [PXD004163_comparisons_3.7-4.9](https://pwilmart.github.io/PXD004163_Notebooks/PXD004163_comparisons_3.7-4.9.html) - Re-analysis with Comet/PAW for the IPG 3.7-4.9 range data (72-fractions)
  * [PXD004163_comparisons_Mascot](https://pwilmart.github.io/PXD004163_Notebooks/PXD004163_comparisons_Mascot.html) - Notebook loading in the Mascot Quantitative Summary data file

#### <a id="SpC"></a>Spectral Counting

* [Smith_SpC_2018](https://github.com/pwilmart/Smith_SpC_2018) - Quantitative analysis of large SpC dataset
  * [Smith_2018_edgeR](https://pwilmart.github.io/TMT_analysis_examples/Smith_2018_edgeR.html) - Notebook with spectral counting data in a paired study design using edgeR

* [Sea_lion_urine_SpC](https://github.com/pwilmart/Sea_lion_urine_SpC) - Analysis of sea lion urine samples
  * [PXD009019_average_missing](https://pwilmart.github.io/TMT_analysis_examples/PXD009019_average_missing.html) - Notebook to determine the low SpC cutoff value
  * [PXD009019_QC_check](https://pwilmart.github.io/TMT_analysis_examples/PXD009019_QC_check.html) - Notebook with some quality control steps and outlier checking
  * [PXD009019_SpC_DE](https://pwilmart.github.io/TMT_analysis_examples/PXD009019_SpC_DE.html) - Notebook with the SpS differential expression analysis

* [ABRF_iPRG_2015_SpC](https://github.com/pwilmart/ABRF_iPRG_2015_SpC) - Analysis of ABRF iPRG data from 2015 study
  * [ABRF_2015_edgeR](https://pwilmart.github.io/TMT_analysis_examples/ABRF_2015_edgeR.html) - Spectral counting data analyzed with edgeR

---

## <a id="Meetings"></a>Meeting Content and Other Presentations

* [talk_to_repo_example](https://github.com/pwilmart/talk_to_repo_example) - How to turn meeting content into repositories

* [ABRF_2020](https://github.com/pwilmart/ABRF_2020) - How to use GitHub to support scientific research and education

* [ASMS-2013_search-engine-comparison](https://github.com/pwilmart/ASMS-2013_search-engine-comparison) - How to compare database search engines

* [ASMS_2018](https://github.com/pwilmart/ASMS_2018) - The Internal Reference Scaling (IRS) method

* [Cascadia_2013](https://github.com/pwilmart/Cascadia_2013) - Extended parsimony protein grouping

* [Cascadia_2018](https://github.com/pwilmart/Cascadia_2018) - A tour of Jupyter notebooks

* [RECOMB-CP_2012](https://github.com/pwilmart/RECOMB-CP_2012) - How to analyze shotgun proteomics data

* [Score_distributions_FDR](https://github.com/pwilmart/score_distributions_FDR) - Examples of how search engine score distribution overlap and relative magnitudes affect false discovery rate thesholds

* [Precursor_mass_corrections](https://github.com/pwilmart/precursor_mass_corrections) - Public data from the [Monocle paper](https://pubs.acs.org/doi/abs/10.1021/acs.jproteome.0c00563?casa_token=DzzesZv3fdAAAAAA:sDuBKpnjXwAlfU2A0G77wXOV0MDScWCLznDIxhWM5OZe7ONWKvtCEE2KP556moITh3uYA2QzEjor_w) re-analyzed with wide tolerance and the PAW pipeline

---

## <a id="Other_repos"></a>Other Repositories

* [OHSU-Proteomics](https://github.com/OHSU-Proteomics/Start_Here) - Tutorials, etc. from the OHSU Proteomics core

* [TMT Publications](https://github.com/OHSU-Proteomics/OHSU_TMT_Publications) - List of TMT papers (mostly OHSU) that use methods developed here

* [Cloud and desktop computing workflow timing](https://github.com/pwilmart/Cloud_desktop_benchmarks) - Some workflow timing data in support of [this paper](https://pubs.acs.org/doi/10.1021/acs.jproteome.0c00920).

### Forked Repositories

* [Reference_Proteome_Manager](https://github.com/pwilmart/Reference_Proteome_Manager)

* [tmt-normalization](https://github.com/pwilmart/tmt-normalization)

* [spectrum_utils](https://github.com/pwilmart/spectrum_utils)

* [RawQuant](https://github.com/pwilmart/RawQuant)

* [RawTools](https://github.com/pwilmart/RawTools)

* [stats337](https://github.com/pwilmart/stats337)
