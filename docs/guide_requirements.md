![Screenshot](img/slim/guide_logo2.png)

# Requirements 

BridgePRS depends on R, plink, and a python wrapper.  Installation is described in detail in the following sections.  Alternatively, if python3+ is already available, 
the BridgePRS installer can be used to automate the process. 



## R 

BridgePRS requires the following **R** [**version 3.6.3+**] ([Download](https://www.r-project.org/)) packages:   
**BEDMatrix, boot, data.table, doMC, glmnet, MASS, optparse, parallel, and R.utils**

!!! tips "R Packages"
    These packages can be installed from inside an R terminal using the command: 
        ```
        $ R 
        > install.packages(c("BEDMatrix","boot","data.table","doMC","glmnet","MASS","optparse","parallel","R.utils")) 
        ```


## Plink 
BridgePRS requires a version of plink compatible with your machine. ([download](https://www.cog-genomics.org/plink/))

By default BridgePRS includes a version of plink for Linux and MacOs and will attempt to locate the correct version. 
To override this behavior and use a specific version of plink please use the flag `--plinkPath` $PLINKPATH to direct BridgePRS 
to the file location.  

!!! warning "Extra MacOs Security:"   
    MacOs often block executables if they are not approved from the app store.                 

    You may have to change your settings to allow Plink to be called  



## Python
The BridgePRS wrapper requires python3+ ([download](https://www.python.org/downloads/)) and matplotlib 
package ([download](https://matplotlib.org/stable/users/installing/index.html)) is required to create plots (options). 

If python3+ is not available, BridgePRS can be ran using shell scripts, as described in the README file.   

If python3+ is available, all other dependencies can be ran using the BridgePRS 






## BridgePRS Installer 

!!! Note "The BridgePRS Installer" 


    If BridgePRS has been downloaded and made executable (as described in our [quickstart tutorial](quikstart_prep.md)) 
    then the following command can be used to allow bridgePRS to check system compatibility and prompt you to 
    install missing software:  
    
    === "$ ./bridgePRS check requirements" 

    ```
    BridgePRS Begins at Sat Sep 30 23:45:46 2023 
    Bridge Command-Line:  ../bridgePRS check requirements
    Checking Requirements:
               System:  platform=linux,  cores(available)=8,          cores(used)=1       (TIP: Using More Than One Core Will Improve Performace (e.g. ---cores 7))
                Plink:  found=true,      path=/home/tade/Bin/plink
                    R:  found=true,      path=/usr/bin/R,             version=3.6.3       (packages=up to date)                                            
              Python3:  found=true,      path=/usr/bin/python3,     matplotlib=true
    Complete
    ```

















