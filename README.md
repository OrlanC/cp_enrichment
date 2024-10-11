## Enrichment analysis of KEGG pathways using clusterProfiler packge in R
This repository shows how to perform enrichment analysis of KEGG pathways in non-model organisms using the 
[clusterProfiler](https://bioconductor.org/packages/release/bioc/html/clusterProfiler.html) in R. 
Please visit https://yulab-smu.top/biomedical-knowledge-mining-book/ for any doubt or detailed instructions
to set up parameters of your enrichment analysis or visualize your results in fancy plots. 

Programs and files required before initiating with this tutorial:

-R and RStudio installed in your computer
 
-:package: clusterProfiler package installed in R

-:egg: To generate an input file from genome functional annotation outputs with eggnog. This input file must tab-separated and header (column names), see example:

Example of input file 1:

|ID          | KEGG (ko:Knumber)|
|:----------:|:----------:|
|Tatro_000080-T1|ko:K14779|
|Tatro_000081-T1|ko:K04567|
|Tatro_000082-T1|ko:K11340,ko:K11400,ko:K11652|
|Tatro_000083-T1|-|

-List of IDs to be analyzed like input file 2 in .txt

Example 1 of input file 2:

|ID          |
|:----------:|
|Tatro_005212-T1|
|Tatro_000081-T1|
|Tatro_002393-T1|
|Tatro_003445-T1|
|...|

Example 2 of input file 2:

|ID                |	logFC |	logCPM|	F|	PValue|	FDR|
|:----------------:|:-----------:|:-----:|:-:|:---------:|:--:|
|Tatro_002208-T1|-1.843|5.400|97.038|1.756e-09|5.520e-06|
|Tatro_011096-T1|-1.203|5.524|95.278|2.069e-09|5.520e-06|
|Tatro_008592-T1|-1.540|6.419|93.472|2.455e-09|5.520e-06|

## Perform KEGG pathway enrichment analysis in R
[Here](https://orlanc.github.io/cp_enrichment/R_enrichment/kegg_pathway_enrichment.html) you can see the R script for the enrichment analysis using *clusterprofiler*.
