# mavisp_data_collection

Here we post issues  or news for the following purposes:
- revision or importing of entries to mavisp database
- issues to fix with the toolkit for mavisp
- ideas for new development and methods to use in the framework
- news on changes in the mavisp_templates and protocols


NEWS

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

  
