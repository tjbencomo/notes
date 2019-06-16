# VEP
## Usage
Basic usage
```
vep --cache --offline --assembly GRCh37 --dir $VEP_DATA --dir_cache $VEP_DATA  -i 101_somatic_filtered.vcf -o plugin_test 
```
Annotations with dbNSFP
```
vep --cache --offline --assembly GRCh37 --dir $VEP_DATA --dir_cache $VEP_DATA \
  --dir_plugins /home/groups/carilee/software/vep_data/Plugins/ -i 101_somatic_filtered.vcf \
  -o plugin_test --plugin dbNSFP,LRT_score
```
## Plugins
### dbNSFP
dbNSFP installation requires the dbNSFP version number be in the datafile name. 
The instructions on the VEP plugins 
[page](https://uswest.ensembl.org/info/docs/tools/vep/script/vep_plugins.html)
to download and create the datafile do not include the version in the filename.
This causes the perl script to error that the dbNSFP version cannot be found.
The datafile should be named like this
```
dbNSFP3.5.gz
```
