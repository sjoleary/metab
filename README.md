# Metab
eDNA metabarcoding: From raw data to RDA
_(Currently in development)_

## Description
With the democratisation of high-throughput sequencing, the use of DNA as an identification method has become standard practice. The marker genes (16S rRNA, 18S rRNA, ITS, etc.) can be compared to databases and give an overview of the communities present in your samples. No more cultivating, isolating and identifying based on morphology and chemical reactions ! However time-gaining DNA sequencing may be, the full process of turning raw DNA reads into exploitable taxonomic units can be tricky. Due to the quick turnover in bioinformatics techniques and the profusion of methods available, it can be hard to decide on a pipeline. In this workshop, we would like to present to you a complete reproducible workflow in R dedicated to the processing of raw DNA sequences using the _DADA2_ package, followed by community analysis and visualisation using the _Phyloseq_ package.

Depuis la démocratisation du séquençage à haut débit, l'utilisation de l'ADN comme méthode d'identification est devenue une pratique courante. Grâce à des gènes marqueurs (ARNr 16S, ARNr 18S, ITS, etc.) et des bases de données taxonomiques, il est possible d’identifier les communautés présentes dans vos échantillons. Plus besoin de cultiver, isoler et identifier en fonction de la morphologie et des réactions chimiques! Cependant, le processus complet de d’identification des séquences d'ADN en unités taxonomiques exploitables peut s’avérer difficile en raison de l’évolution rapide des techniques bioinformatiques et de la profusion de méthodes disponibles. Dans cet atelier, nous vous présenterons un flux opérationnel accessible et reproductible en langage R dédié au traitement de séquences d'ADN brutes à l'aide de la librairie _DADA2_. Cette étape sera suivi d’une analyse et d’une visualisation de la communauté à l'aide de la librairie _Phyloseq_.

## Authors
Simon Morvan and Alexis Carteron,
Université de Montréal

## Data
Amplicons obtained through DNA amplification targeting the ITS region (fungal specific) and sequenced on an Illumina MiSeq plateform (paired-end 300 bp) 

## Acknowledgements
Largely inspired by the tutorials of [_DADA2_](https://benjjneb.github.io/dada2/index.html) and [_Phyloseq_](https://joey711.github.io/phyloseq/)

## Install packages
```
source('http://bioconductor.org/biocLite.R')
biocLite('phyloseq')
biocLite("dada2")
install.packages(c("ggplot2", "vegan")
```
