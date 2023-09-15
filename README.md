## Enrichment analysis of KEGG pathways using clusterProfiler packge in R
This repository shows how to perform enrichment analysis of KEGG pathways in non-model organisms using the 
[clusterProfiler](https://bioconductor.org/packages/release/bioc/html/clusterProfiler.html) in R. 
Please visit https://yulab-smu.top/biomedical-knowledge-mining-book/ for any doubt or detailed instructions
to set up parameters of your enrichment analysis or visualize your results in fancy plots. 

Programs and files required before initiating with this tutorial:
:R: R and RStudio installed in your computer 
:package: clusterProfiler package installed in R
:egg: from genome functional annotation output with eggnog to generate an input file, must tab-separated and header (column names), see example:

Example of inputfile:

|ID          | KEGG ko (Knumber)|
|:----------:|:----------:|
|Tatro_000080-T1|ko:K14779|
|Tatro_000081-T1|ko:K04567|
|Tatro_000082-T1|ko:K11340,ko:K11400,ko:K11652|
|Tatro_000083-T1|-|
|Tatro_000084-T1|ko:K17732|
|Tatro_000085-T1|ko:K03133|
|Tatro_000089-T1|-|
|Tatro_000090-T1|ko:K20299|
|Tatro_000091-T1|ko:K00344,ko:K00384|
