# mavisp_data_collection

Here we post issues for the following purposes:
- revision or importing of entries to mavisp database
- issues to fix with the toolkit for mavisp
- ideas for new development and methods to use in the framework
- news on changes in the mavisp_templates and protocols


NEWS

12/04/2024
- metadata has been revised to include also a config file needed to the data manager to streamline the importing of new entries (importing.yalm) that needs to be filled in
- step 7 for simulations_analysis has been revised to include the right python module to use (python2.7)
- from now on on new entries we will only support data collected with the saturation mutlist and using pancancer_clinvar_saturation.py for cancermuts
- denovo_phospho has been moved back to 'dev' since we need to include some changes in the design to make it less time consuming before starting a large data collection

10/04/2024
- the clinvar step after generation of mutlist is no longer needed and it has been archived
- the pocket_analysis step is no longer needed since allosigma workflow includes it 

15/03/2024
- from today we switch in the data collection for stability as a default to only rasp and mutatex - rosetta will be used only in focused studies on specific protein targets

  
