# CancerAPA
[![Github Release](https://img.shields.io/badge/release-v1.0-brightgreen)](https://github.com/3UTR/CancerAPA)
[![python Release](https://img.shields.io/badge/python-2.7.14-brightgreen)](https://www.python.org/downloads/)
[![R Release](https://img.shields.io/badge/R-3.6.2-brightgreen)](https://cran.r-project.org/)
[![bedtools Release](https://img.shields.io/badge/bedtools-v2.25.0-brightgreen)](https://github.com/arq5x/bedtools2)
[![Samtools Release](https://img.shields.io/badge/samtools-v1.9-brightgreen)](http://www.htslib.org/)
[![plink Release](https://img.shields.io/badge/plink-1.9-beta-brightgreen)](https://www.cog-genomics.org/plink/）


### Pan-cancer GWAS APA analysis
Analysis shared by ["A distinct class of pan-cancer susceptibility genes revealed by alternative polyadenylation transcriptome-wide association study"](https://medrxiv.org/cgi/content/short/2023.02.28.23286554v1)
# Introduction
In this study, we performed the first large-scale and systematic analysis assessing the genetic effects of APA on 25 cancer types in 49 human tissues from the Genotype-Tissue Expression(GTEx).
# Outline
* GWAS clump using [plink](https://www.cog-genomics.org/plink/) and fine-mapping using [CAUSALdb](https://github.com/mulinlab/CAUSALdb-finemapping-pip)
* GWAS heritabiltiy estimates and genetic correlaiton using [LDSC](https://github.com/bulik/ldsc)
* 3aQTL calling and fine-mapping using [CAVIAR](https://github.com/fhormoz/caviar)
* Integreation of cancer GWAS and 3aQTLs to assess the 3aQTL for their contributions to disease susceptibility
  * Partitioned heritabiltiy estimates using [LDSC](https://github.com/bulik/ldsc) and heritablity enrichment esitimates using [fgwas](https://github.com/joepickrell/fgwas)
  * Transcriptome-wide association analysis using [FUSION](http://gusevlab.org/projects/fusion/)
  
## Prerequisites
1. `Python (version >= v2.7.14)`
2. `R (v3.6.2)`
3. `PEER (v1.3), https://github.com/PMBio/peer`
4. `bedtools (v2.25.0-119-ga0dc5db)`
5. `samtools (v1.9)`
6. `plink 1.9 beta`
