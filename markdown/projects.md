# Projects

## Elucidating the genetic variation of the Faroese population

The [Faroe Islands](https://en.wikipedia.org/wiki/Faroe_Islands) is a small archipelago in the North Atlantic with about 50 000 inhabitants. This population has remained relatively isolated for about a thousand years, which may have led to substantial [genetic drift](https://en.wikipedia.org/wiki/Genetic_drift). The population underwent a founding event about a thousand years ago and has had a population size under 5000 until about 300 years ago, and from about 1850 to 1950 the population experienced explosive growth.

In my PhD thesis, I will analyze whole-exome linked-read sequencing data of Faroese individuals from the [FarGen](https://www.fargen.fo) project (currently about 450 samples and growing). I will apply diffusion approximation methods such as [moments](https://bitbucket.org/simongravel/moments/src/master/) by [Simon Gravel's group](http://simongravel.lab.mcgill.ca/Home.html) (Jouganous et al. 2017 [DOI](https://doi.org/10.1534/genetics.117.200493)) to understand how different demographic events may have led to the distribution of allele frquencies that we see today. I will also apply identity-by-descent (IBD) methods to understand recent demography, such as [IBDNe](https://faculty.washington.edu/browning/ibdne.html) by Browning et al. 2016 ([DOI](https://doi.org/10.1016/j.ajhg.2015.07.012) to understand effective population size, and methods such as FastIBD (from [Beagle](https://faculty.washington.edu/browning/beagle/beagle.html)) from Browning et al. 2007 ([DOI](https://doi.org/10.1086/521987)) to understand population structure. The findings will be corroborated with simulation, for example coalescent simulations with [msprime](https://msprime.readthedocs.io/en/stable/) by Kelleher et al. 2016 ([DOI](https://doi.org/10.1371/journal.pcbi.1004842)) and forward-simulations with [fwdpy11](https://fwdpy11.readthedocs.io/en/stable/) by Thornton et al. 2014 ([DOI](https://doi.org/10.1534/genetics.114.165019)).

We expect this project to give insight into possible genetic mechanisms behind increased prevalence observed in hereditary diseases on the islands, and inform FarGen's efforts to understand the genetic architecture of rare as well as common hereditary diseases.

## Linked-read bioinformatics

[Linked-reads](https://www.10xgenomics.com/linked-reads/) from 10x Genomics are a promising technology that promise to resolve ambiguous alignments and phase haplotypes. Most publication use 10x Genomic's own software, which is open source but still proprietary, and which lacks transparancy. Therefor I opt to use other open source tools such as [EMA](https://github.com/arshajii/ema/) and [HapCUT2](https://github.com/vibansal/HapCUT2). In order to be satisfied with our linked-read pipeline, we will have to extensively test and compare these tools. Currently a work in process, this project includes a pipeline for basecalling/demultiplexing data (`demuxlink`) and a pipeline for alignment and variant calling (`exolink`):

* [demuxlink](https://github.com/olavurmortensen/demuxlink)
* [exolink](https://github.com/ilegusavnid/exolink)


