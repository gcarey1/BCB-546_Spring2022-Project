Kuralt-2022
================
Razan Alsayed Omar
2022-05-07

## Introduction

This study’s main focus was to document genetic information on
ground-dwelling invertebrates in Krokar which is a virgin forest in
Slovenia. It is a part of the Dinaric Alps that ranges from Italy to
Albania \~ 400 miles long. Krokar is also the largest virgin forest in
Slovenia and has the most diverse soil invertebrates in Europe. However,
soil fauna of this forest isn’t thoroughly studied and there aren’t many
genetic libraries from this area. Therefore, this group decided to
address this lack of faunistic and genetic data. This is important as
this region is vulnerable to climate change can affect morphology,
vegetation and soils. Therefore, knowing the current status of the
invertebrate communities is important to identify any changes to the
climate and habitat as well as assess the human impact on these
communities and habitat. Ground-dwelling invertebrates play an important
role in forest soil processes like nutrient cycling and predators like
spiders, which is one of the organisms included in this study, has a
very important role in maintaining the fauna of the habitat due to its
mid-level placement in the trophic pyramid as they are sensitive to
changes to their habitat so it is important to document the genetic
information on these invertebrates.

The authors main aims were to generate a checklist of soil and
ground-dwelling predatory invertebrates in Krokar and to create a
DNA-barcode library of these invertebrates.

The authors did this by first collecting soil samples from Krokar and an
adjacent secondary forest, identifying specimens using a
stereomicroscope, extracting DNA from the specimens and sequencing them
and amplifying the COI gene for DNA barcoding, sequence alignment and
phylogenetic tree was made using Geneious Prime TreeBuilder, and all
their data was deposited into GenBank and BOLD.

The three invertebrates they analyzed and documented were: spiders,
centipedes, beetles.

The main figure in this paper was the phylogenetic tree they created.
This tree is what we tried to replicate for this project.

## Technical details

We worked to replicate the phylogenetic tree from our chosen paper. We
accomplished this using R, Python, and ClustalW. Initial data inspection
and all parts of our process up until sequence alignment was completed
in R. This is documented in our “Arthropod_markdown.md” file. We relied
on a number of packages, including tidyverse, to read BOLD sequence
identifiers from the BOLD database and into our dataframe, and
eventually output a fasta file (“phylo_bold.fasta”) which contains
sequences with which to make our tree.

After this point, we moved into Python. We used the biopython package to
align sequences, create an unrooted phylogenetic tree which we output as
a .nwk file (tree.nwk). This file was then imported into MEGA X v
11.0.11 so it can be converted and exported as a PNG file called
treefinal.png.

## Summarization of replication of results

Replication of Analyses

The “analysis” in this case consisted of a single phylogenetic tree. Our
project was an attempt to replicate this phylogenetic tree to the
specifications provided by the authors using their provided sequences.
These specifications were:

Built a COI tree using Geneious Prime Tree Builder (Geneious version
2022.0 created by Biomatters) Distance matrix was calculated using
Global alignment with free end gaps and 70% similarity (IUB)(5.0/-4.5)
cost matrix The tree was built with Tamura-Nei genetic distance and the
Neighbour-Joining tree build method.

We also inferred that their tree is an unrooted tree. These are a
limited number of details to fully replicate the author’s phylogenetic
tree, however we were able to provide a tree at the completion of the
project. Whether or not it is an exact replica of the original, this
tree serves the same purpose as the original: to describe the
invertebrates of Krokar forest.
