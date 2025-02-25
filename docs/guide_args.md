![Screenshot](img/slim/guide_logo6.png) 

This page contains all command available in BridgePRS. 

!!! tips
    
    When constructing new parameters, we follow the following rule: if the command has effect on any file that is not the target, 
    it will have a prefix of the file name. For example, `--base-info` applies INFO score filtering on the base file, `--ld-info` perform INFO score filtering on the LD reference file and `--info` applies the INFO score filtering on the target file. 


## Input Population Files/Arguments


- `--sumstats_prefix`  Path to sumstats data 

- `--phenotype_files`
     phenotype test and validation data    


- `--pop_config(s)`
     population configuration file(s) 

- `--pop or --pops`
     population names (AFR, EUR, etc) 

- `--snp_file` List of QCed SNP ids 


## System Level Toggles/Arguments 


- `--cores` By default bridgePRS is parralelized across (n-1) cores 

- `-o`  Output folder for BridgePRS 



- `--platform`  Force platform (Linux or MacOS) 


- `--verbose`  Toggle Verbose Mode On   


- `--noPlots`  Skip Post-Pipeline Analysis (Plotting) 

- `--restart`  Repeat previously completed steps


## Parameter Arguments 


- `--fst` fst value        

- `--max_clump_size`
     Max Size for Clumping      

- `--thinned_snplist`
     Thinned snp list for large clumps    

## Internal File Arguments 

- `--model_file`  model result generated from the build-model subprogram 

- `--clump_prefix` prefix for files generated by clump step   


- `--eval_prefix`  prefix for files generated by eval step   

- `--optimize_prefix`   prefix for files generated by optimize step   

- `--predict_prefix`   prefix for files generated by predict step   

- `--results`  prs result files 





## File Column Names 


### Phenotype Files 


- `--phenotype`  Phenotype File Field: phenotype 
- `--covariates` Phenotype File Field: covariates      


### Sumstats Files 



- `--ssf-alt`
     Sumstats Field: alt allele      

- `--ssf-beta`
     Sumstats Field: beta       

- `--ssf-maf`
     Sumstats Field: MAF       

- `--ssf-p`
     Sumstats field: P-value       

- `--ssf-ref`
     Sumstats Field: reference allele      

- `--ssf-se`
     Sumstats field: standard error      

- `--ssf-snpid`
     Sumstats field: snpID       

- `--ssf-ss`
     Sumstats Field: Sample Size      

- `--sumstat_prefix`
     path to sumstats file prefixes     

- `--sumstats_suffix`
     Sumstats Suffix        





