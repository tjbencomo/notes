# Sequencing

# Exome Target Regions
When analyzing exome data, most programs require a BED file with the capture regions. 
GATK uses this to only call mutations within these regions. CNVKit uses these regions determine off-target
bins to estimate copy number. The target region depends on sequencing company that designed the probes.

Stanford Dermatology seems to use Agilent, specifically the SureSelect whole exome capture kits.
To access the BED files for each probe kit, go to the [Agilent SureDesign website](https://earray.chem.agilent.com/suredesign/)
and login or create an account. Login and then go to Find Designs, choose the appropriate probe type, and then select 
Agilent catalog. This will display all the different kits and allow you to download the appropriate files.
