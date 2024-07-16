# The genomic underpinnings of convergence in toucans and hornbills (Supplementary Information)

# Abstract
Does phenotypic convergence arise due to parallel mutations on orthologous genes or does selection find different genomic routes to achieve similar outcomes? Convergent evolution is ubiquitous across the tree of life, and may be driven by selection on alternative genes, selection on the same genes, or molecular convergence due to mutational bias in regulatory or coding regions. We tested these alternate hypotheses in two large bodied, large billed, frugivorous tropical bird lineages, toucans and hornbills, a textbook example of phenotypic convergence. We compare positive selection and protein similarity in a set of well-annotated exons to identify the molecular underpinnings of phenotypic convergence in the avian clade Cavitaves. Using dN/dS ratios, we identified candidate genes under positive selection, and candidate genes with convergent protein structure. We identified genes that exhibit both convergent amino acid sequences and signatures of positive selection and mapped the functional relationship of these gene sets and their associated gene-ontology (GO) terms. We found that genes under parallel selection were part of functional networks related to bill and facial development, suggesting that convergence in toucans and hornbills may in part be driven by mutations on the same genes. We also suggest permutation and filtering methods to account for bias of exon sets in functional analyses.

# Supplementary Methodological Information

We PacBio sequenced a _Ramphastos vitellinus ariel_
and compared that genome to publically available whole genomes for 23 other taxa, including a zebra finch reference downloaded from NCBI

PacBio scaffolds were mapped to Zebra Finch pseudo-chromosomes using RagTag.

Orthologs identified using BUSCO, amino acids and nucleotides aligned using MACSE

Species tree constructed using 2.8 Mb concatenated alginment of BUSCO nucleotide sequences in RaxML
(All nodes had 100% bootstrap support).

Amino Acid trees constructed using IQtree. 

Topology outliers selected using custom R script, but also used methods from phylogenetics packages (phytools, ape, geiger) etc.
Retained genes with discordant topologies where Tocuans and Hornbills were more closely related than expected based on species tree.

dN/dS test was run using the ABSREL model in HyPhy (Examines dN/dS ratios within genes on certain test branches)
Compared dN/dS at nodes preceding splits within Toucans and Hornbills to background dN/dS.
Genes were considered under selection based on FDR Corrected P Values < .05. 

GO terms mapped for candidate genes for both candidate sets and for cross-referenced candidate set (from OrthoDB v 10.1)

Overrepresentation analysis was performed using clusterProfiler's enrichGO method, Bonferroni corrected P. 

Term semantic similarity clustering and plotting was performed in REVIGO. 

# Acknowledgements

Images from HBW, Kacau Oliveira, San Diego Zoo.

Thank you to the Weckstein Lab (Emily Griffith, Kamila Kuabara, Matthew Soesanto, Calvin Keeys, Nate Rice, Dan Thomas) for their insight and feedback improving this work. 
Thank you to Drexel's BEES department, whose generous travel funding made attending and presenting at this conference possible. 

# Contact

Any questions or comments? Please reach out at jon.treadwell.merwin@drexel.edu

Follow me: @merwinjon








