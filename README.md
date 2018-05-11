# Metab
eDNA metabarcoding: From raw data to RDA
_(Currently in development)_

## Description
With the democratisation of high-throughput sequencing, the use of DNA as an identification method has become standard practice. The marker genes (16S rRNA, 18S rRNA, ITS, etc.) can be compared to databases and give an overview of the communities present in your samples. No more cultivating, isolating and identifying based on morphology and chemical reactions ! However time-gaining DNA sequencing may be, the full process of turning raw DNA reads into exploitable taxonomic units can be tricky. Due to the quick turnover in bioinformatics techniques and the profusion of methods available, it can be hard to decide on a pipeline. In this workshop, we would like to present to you a complete reproducible workflow in R dedicated to the processing of raw DNA sequences using the _DADA2_ package, followed by community analysis and visualisation using the _Phyloseq_ package.

Depuis la démocratisation du séquençage à haut débit, l'utilisation de l'ADN comme méthode d'identification est devenue une pratique courante. Grâce à des gènes marqueurs (ARNr 16S, ARNr 18S, ITS, etc.) et des bases de données taxonomiques, il est possible d’identifier les communautés présentes dans vos échantillons. Plus besoin de cultiver, isoler et identifier en fonction de la morphologie et des réactions chimiques! Cependant, le processus complet de d’identification des séquences d'ADN en unités taxonomiques exploitables peut s’avérer difficile en raison de l’évolution rapide des techniques bioinformatiques et de la profusion de méthodes disponibles. Dans cet atelier, nous vous présenterons un flux opérationnel accessible et reproductible en langage R dédié au traitement de séquences d'ADN brutes à l'aide de la librairie _DADA2_. Cette étape sera suivi d’une analyse et d’une visualisation de la communauté à l'aide de la librairie _Phyloseq_.

## Install packages
```
source('http://bioconductor.org/biocLite.R')
biocLite('phyloseq')
biocLite('dada2')
install.packages(c('ggplot2', 'vegan', 'gtools')
```

## Tutorials
Dada: [https://alexiscarter.github.io/metab/Dada_script.html](https://alexiscarter.github.io/metab/Dada_script.html)  
Phyloseq: [https://alexiscarter.github.io/metab/Phyloseq_script.html](https://alexiscarter.github.io/metab/Phyloseq_script.html)

## To download the repository
[https://github.com/alexiscarter/metab/archive/master.zip](https://github.com/alexiscarter/metab/archive/master.zip)  
It includes data and scripts.
<br>

Set the working directory before starting the tutorials:  
```
setwd("YourPath/metab-master")
```

## Authors
Simon Morvan and Alexis Carteron,
Université de Montréal

## Data  
From A. Carteron, S. Joly, M. Beigas, B.L. Turner, E. Laliberté. Major Changes in Soil Fungal Communities Across Soil Horizons and Between Adjacent Forests. In preparation  
Amplicons obtained through DNA amplification targeting the ITS region (fungal specific) and sequenced on an Illumina MiSeq plateform (paired-end 300 bp).  
Orignial sequenced data were subsampled, randomly selecting 1,000 pair-end reads per sample (i.e. 128,000 reads in total) to facilite running time in local machine. [_Seqtk_](https://github.com/lh3/seqtk) was used for the subsampling step.

## Acknowledgements
Largely inspired by the tutorials of [_DADA2_](https://benjjneb.github.io/dada2/index.html) and [_Phyloseq_](https://joey711.github.io/phyloseq/)

Corresponding articles:

* Callahan B. J., McMurdie P. J., Rosen M. J., Han A. W., Johnson A. J. A., & Holmes S. P. (2016) DADA2: high-resolution sample inference from Illumina amplicon data. Nature methods, 13(7), 581-583

* McMurdie P. J. & Holmes S. P. (2013) Phyloseq: An R Package for Reproducible Interactive Analysis and Graphics of Microbiome Census Data. PLoS ONE. 8(4):e61217
