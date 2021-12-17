# Sequencing

# Exome Target Regions
When analyzing exome data, most programs require a BED file with the capture regions. 
GATK uses this to only call mutations within these regions. CNVKit uses these regions determine off-target
bins to estimate copy number. The target region depends on sequencing company that designed the probes.

Stanford Dermatology seems to use Agilent, specifically the SureSelect whole exome capture kits.
To access the BED files for each probe kit, go to the [Agilent SureDesign website](https://earray.chem.agilent.com/suredesign/)
and login or create an account. Login and then go to Find Designs, choose the appropriate probe type, and then select 
Agilent catalog. This will display all the different kits and allow you to download the appropriate files.

AstraZeneca has a great [repository](https://github.com/AstraZeneca-NGS/reference_data) with capture region BED files
for several kits (including Agilent).

# GEO Submission
This script uploads data to GEO and can be run non-interactively on a cluster
```
# File: upload.sh
#
# GEO_server_address/password - ftp login info provided by GEO
# upload_dir - location where they want you to upload the data; usually [username]/uploads
# dir_to_upload - directory that you want to upload (-R includes sub-directories]
# swap mirror for put command for a single file
lftp  -c "open [GEO_server_address/password]; cd [upload_dir]; mirror -R [dir_to_upload]"
```
