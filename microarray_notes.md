# Microarray Notes

## Multiple Probes Per Gene
Description of how to handle multiple probes per gene:

* [https://www.reddit.com/r/bioinformatics/comments/544zqi/multiple_probes_for_one_gene/d7zpcxj/?utm_source=share&utm_medium=web2x](https://www.reddit.com/r/bioinformatics/comments/544zqi/multiple_probes_for_one_gene/d7zpcxj/?utm_source=share&utm_medium=web2x)

What the `at`, `s_at`, and `x_at` mean at the end of probe set IDs:

* [https://www.biostars.org/p/16093/](https://www.biostars.org/p/16093/)
* [https://dintor.eurac.edu/doc/doc/HSGeneAtlas.html](https://dintor.eurac.edu/doc/doc/HSGeneAtlas.html)
* [https://cbdm.uni-mainz.de/files/2016/02/GE_microarrays.pdf](https://cbdm.uni-mainz.de/files/2016/02/GE_microarrays.pdf)

## Selecting The Optimal Probe
The [`jetset`](https://cran.r-project.org/web/packages/jetset/index.html) package identifies the best probe to represent each gene 
for a select number of microarray platforms.
These probes were selected based on quality/precision for the specific gene. Very useful package.

## Handling Unannotated Probes
Sometimes the microarray platform on GEO will be missing transcript/gene annotations. 
[EBI](https://www.ebi.ac.uk/training/online/courses/array-express-discover-functional-genomics-data-quickly-and-easily/next-steps-towards-data-analysis/opening-and-processing-raw-data-files/microarray-experiments/tools-for-conversion-of-probe-ids/)
provides an overview of how to annotate these probes. 

* See if probe mappings are provided by ENSEMBL in the BioMart portal - look for the platform type in the Attributes section
* If probe mappings do not already exist, there are several re-annotation tools that will align the probe sequence to the genome and determine the best matching gene. This approach will require more work as better to look for pre-existing annotations if possible

