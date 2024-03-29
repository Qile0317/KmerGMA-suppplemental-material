# KmerGMA-suppplemental-material
Repository for analysis scripts, data, and general supplemental information for Utställningen Ungaforskare (Swedish ntional highschool science fair) finals 2023. 

The project presentation can be found at: https://projectboard.world/project/kmergma-jl-homology-searching-for-germline-immunoglobulin-alleles-with-kmers

The repository is incomplete and will be updated very soon with more data and analysis scripts.

note: since the 12th of march, the main method and package has a very large volume of the changes and the results mentioned in the report may not be  100% replicated now. However, the new results are definitively better than the old versions.

# Repository organization
## Analysis_scripts
- `Kmer_dist_update_formula.ipynb`: a jupyter notebook of the derivation of a more computationally efficient formula for updating the kmer distance as the window iterates in KmerGMA. (see page 4, equation 4) The improved formula's running speed was also benchmarked and seems to be about 2.8 times faster and saves more memory. This is a *new discovery* since the report was sent in.

## Sequences
- `88_Alpaca_reference_V_genes.fasta`: the 88 alpaca reference sequences used in the report.
- `Novel_Alpaca_PseudoVgenes.fasta`: Two novel V genes discovered in the VicPac 3.2 Alpaca full coverage genome assembly. The fasta identifiers indicate the contig id of where the hit was found, followed by a kmer distance `Dist` to one of the RVs formed by RS subsets, indicated by `KFV = x`. `MatchPos` is a unitrange showing the location of the hit within the contig, `GenomePos` is the cumulative number of basepairs before the contig, and `Len` is the length of the aligned hit. The first fasta sequence was the novel pseudogene discovered and discussed in the report submission. The second sequence was a new one recently discovered by an improved KmerGMA algorithm (see page 6, *"Optional incorporation of multiple RVs"*)
- `10_KmerGMA_Alpaca_Vgenes_of_interest.fasta`: FASTA files of the 10 *aligned DNA* sequences of 10 V gene hits of interest that were looked at in the final report submission. The fasta identifiers are written in the same way as in the previous description. 

## Miscallaneous
- `Method_animation.ipynb`: Code I used to generate the animations that were used in my presentation video