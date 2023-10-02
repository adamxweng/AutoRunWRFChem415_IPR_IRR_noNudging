# AutoRunWRFChem IRR+IPR (noPBL nudging)  for 4.1.5

scripts for running WRF-Chem 4.1.5 with both IRR and IPR supported.
For MOZART (chem_opt=202) mechanisms.
Auto create namelist for real.exe and wrf.exe

# To Run:

source 01_envVar_set_415_noNudgingPBL_IRR_IPR.sh source ~/.bash_profile

bash 02_realnoChem.sh && bash 03_wesely.sh && bash 04_megan.sh && bash 05_realChem.sh && bash 06_mozbc.sh

