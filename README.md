# mavisp_data_collection

Here we post issues  or news for the following purposes:
- revision or importing of entries to mavisp database
- issues to fix with the toolkit for mavisp
- ideas for new development and methods to use in the framework
- news on changes in the mavisp_templates and protocols


NEWS



06/06/2025

A new version of the AlloSigMA2 workflow for the simple mode LONG_RANGE module is available aligned with the benchmark study under revision for JMB. Each new entry should be using
this workflow. We will annotate method and relevant cutoffs in the metadata. The updates of old entries will be carried out during the yearly updates of 2025 (June-August 2025). We also revised one of the scripts of the LONG_RANGE module in ensemble mode for the psn-path analysis for a modification that make the calculation independent from the starting structure. Use new templates for new runs and the update of the old entries is also ongoing.

The pdbminer_complexes tool was updated to enhance the binding-interface flag, now allowing detection of target chain(s) interfaces across all other chains in the complex, especially useful for multimeric complexes.

02/06/2025

We have updated Mol_Analysis for the quality control of the MD simulations and pre-md steps so that the average rmsd matrix is calculated more efficiently 

12/05/2025

Updated get_mutlist.py 

11/04/2025

A new metadata template is available where also the source of structure should be reported

08/04/2025

We have fixed a problem that made the MAVISp_automatization crash when multiple Gene ID where found to be associated with a protein's RefSeq identifier

03/03/2025
revised version of mavisp_automatization snakemake to fix a bug with PTM module for multi-domai proteins

08/01/2025 

revised version of mavisp_automatization snakemake to fix issues with PTM and RaSP experienced in December

18/01/2024

templates for step 6 of simulations_analysis corrected for the groups for rmsd calculation (i.e. mainchain)

05/12/2024
- new pancancer.py template for cases where cancermuts fail in retriving entrez ID

29/11/2024 
- new templates available for custom analysis with long-range modules in simple and ensemble mode for cofactor bindign sites or catalytic sites of enzymes

28/11/2024 
- fixed a bug in mavisp_automatization for the generation of the saturation mutlist

20/11/2024 

- new version of Mol_Analysis.py with fixed labels in pdf and with option to perform gmindist using a slicing of the trajectory

19/11/2024

- new templates file for mutatex_automatization
- new version of mavisp_automatization with support to custom PDB file in input 

14/11/2024 

- updates in mavisp_automatization that requries to update the template folder for data colleciton - includes a fix for the folder name in cancermuts_data and in
  the script for the domain annotations

05/11/2024 
- a new version of SLiMfast is available for data analysis which integrate the filtering step based on solvent accessibility 

24/10/2024

- the procheck step within structure_selection has been implemented in mavisp_automatization, new templates available for data collection on the local server
. a wrapper around simulations_analysis is available in the mavisp_templates on the local server 


05/10/2024

-- we have introduced in dot_plot.py loss/gain of function for GEMME
- the default to assign damaging effect for GEMME have been changed with a default value of -3 (loss-of-function) and 3 (gain-of-function) and using the "GEMME Score"
- the default to assign damaging effect for DeMaSk have been changed with a default value of -0.25 (loss-of-function) and 0.25 (gain-of-function)
- we should not import results on variants in MET1 since a mutation in this code would interrupt transcription and do not result in a full-lenght protein
- the templates for mavisp automatization have been updated including the proper script for clinvar_gene 

27/09/2024

- mavisp_automatization now includes also the pdbminer_complexes step

24/09/2024

- new procedure for selecting complexes for local interactions in the guideline document

13/09/2024

- we have introduced in dot_plot.py loss/gain of function for DeMaSk and efoldmine annotations
- the default to assign damaging effect for GEMME has been changed with a default value of 0.5 

05/07/2024
- the first release of mavisp saturation is available (simple mode) - importing for the ensemble mode is ongoing

24/05/2024
- new clinvar.py version with support of genomic coordinates

29/04/2024

- updated pdbminer_complexes to solve this issue: https://github.com/ELELAB/CSB-scripts/issues/418 

27/04/2024
- updated mavisp templates for long_range with distance cutoff set to 15 Ang after ASM publication and exploration of other similar cases

25/04/2024

- updated readme for step 7 of simulations_analysis to cover cases with residue type HISE, HISD and HISH from CHARMM36m simulations

22/04/2024
- step 5 of simulations_analysis has been updated including a script in python2 to add the chain identifier for mutatex calculations
- clinvar.py in clinvar_gene has been updated in light of this pull request: https://github.com/ELELAB/CSB-scripts/pull/371 - we have updated in both mavisp_templates and mavisp_automatization
- a new version of cancermuts is available in light of this PR: https://github.com/ELELAB/cancermuts/pull/198 which allows to interact with a local version of ELM through the recently
  published gget elm:  https://academic.oup.com/bioinformatics/article/40/3/btae095/7611647 - the template file for pancancer_clinvar_saturation.py has been modified in mavisp_templated and in mavisp_automatization since it is the one to use from now on. 


15/04/2024
- templates for ptm.md have been added to mavisp_templates in shared_projects

12/04/2024
- metadata has been revised to include also a config file needed to the data manager to streamline the importing of new entries (importing.yalm) that needs to be filled in
- step 7 for simulations_analysis has been revised to include the right python module to use (python2.7)
- from now on on new entries we will only support data collected with the saturation mutlist and using pancancer_clinvar_saturation.py for cancermuts
- in structure_selection there is a new tool pdbminer_complexes to use to verify if there are structures available without missing residues to reconstructs for local_interaction. it needs a pdbminer output from at least early 2024. 

11/04/2024
- denovo_phospho has been moved back to 'dev' since we need to include some changes in the design to make it less time consuming before starting a large data collection

10/04/2024
- the clinvar step after generation of mutlist is no longer needed and it has been archived
- the pocket_analysis step is no longer needed since allosigma workflow includes it 

15/03/2024
- from today we switch in the data collection for stability as a default to only rasp and mutatex - rosetta will be used only in focused studies on specific protein targets

  
