# VCF2MAF
## Usage
Basic usage
`--ref-fasta` should be the fasta used to align the variants. Don't use the one provided in the VCF2MAF repo,
use the ref-fasta files in the `refs/` directory. 

Depending on your path setup, if the `vep` executable and data isn't stored
in `$HOME/.vep`, you'll need to tell `vcf2maf.pl` where to look with `--vep-path`
and `--vep-data`.
