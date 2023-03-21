# KmerGMA-suppplemental-material
Repository for analysis scripts, data, and general supplemental information for Utställningen Ungaforskare finals 2023.

The repository is incomplete and will be updated very soon with more data and analysis scripts.

However, it is noteoworthy that since the 12th of march, the main method and package has a very large volume of the changes and the results mentioned in the report may not be  100% replicated now. However, the new results are definitively better than the old versions.

# Repository organization
## Analysis_scripts
- `Kmer_dist_update_formula.ipynb`: a jupyter notebook of the derivation of a more computationally efficient formula for updating the kmer distance as the window iterates in KmerGMA. The improved formula's running speed was also benchmarked and seems to be about2.8 times and saves more memory. This is a new discovery since the report was sent in.

## Sequences
- `88_Alpaca_reference_V_genes.fasta`: the 88 alpaca references sequences used in the report.
- `Novel_Alpaca_PseudoVgenes.fasta`: Two novel V genes discovered in the VicPac 3.2 Alpaca full coverage genome assembly. The fasta identifiers indicate the contig id of where the hit was found, followed by a kmer distance `Dist` to one of the RVs formed by RS subsets, indicated by `KFV = x`. `MatchPos` is a unitrange showing the location of the hit within the contig, `GenomePos` is the cumulative number of basepairs before the contig, and `Len` is the length of the aligned hit. 

## Miscallaneous
Currently just contains a jupyter notebook I used to generate the animations that were used in my presentation video