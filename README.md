# AutoRunWRFChem IRR+IPR MOZART(chem_opt=201) (noPBL nudging)  for 4.1.5

scripts for running WRF-Chem 4.1.5 with both IRR and IPR supported.
For MOZART (chem_opt=201) mechanisms.
Auto create namelist for real.exe and wrf.exe

# wetscav_onoff=0,cldchem_onoff=0
Here I shut down both wetscav and cldchem, ensuring mz201 is comparable with cbmz170.
Because wet scavenging in stratocumulus clouds and aqueous chemistry in stratocumulus clouds are not supported in cbmz170.

# To Run:

source 01_envVar_set_mz201_415_noNudgingPBL_IRR_IPR.sh source ~/.bash_profile

bash 02_realnoChem.sh && bash 03_wesely.sh && bash 04_megan.sh && bash 05_realChem.sh && bash 06_mozbc.sh

