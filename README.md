## Enrichment analysis of KEGG pathways using clusterProfiler packge in R
This repository shows how to perform enrichment analysis of KEGG pathways in non-model organisms using the 
[clusterProfiler](https://bioconductor.org/packages/release/bioc/html/clusterProfiler.html) in R. 
Please visit https://yulab-smu.top/biomedical-knowledge-mining-book/ for any doubt or detailed instructions
to set up parameters of your enrichment analysis or visualize your results in fancy plots. 

Programs and files required before initiating with this tutorial:

-R and RStudio installed in your computer
 
-:package: clusterProfiler package installed in R

-:egg: from genome functional annotation outputs with eggnog, to generate an input file, must tab-separated and header (column names), see example:

Example of input file 1:

|ID          | KEGG (ko:Knumber)|
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

-list of IDs to be analyzed, file in .txt

Example 1 of input file 2:

|ID          |
|:----------:|
|Tatro_005212-T1|
|Tatro_000081-T1|
|Tatro_002393-T1|
|Tatro_010760-T1|
|Tatro_000038-T1|
|Tatro_003445-T1|
|...|

Example 2
|ID                |	logFC |	logCPM|	F|	PValue|	FDR|
|:----------------:|:-----------:|:-----:|:-:|:---------:|:--:|
|Tatro_002208-T1|	-1.84328735162963|	5.40075099864936|	97.0384436563709|	1.75668775562383e-09|	5.52001735279739e-06|
|Tatro_011096-T1|	-1.20328045897947|	5.52454556561384|	95.2782228064919|	2.06982179380337e-09|	5.52001735279739e-06|
|Tatro_008592-T1|	-1.54031007632897|	6.41900167215348|	93.4725834448608|	2.4555237334508e-09|	5.52001735279739e-06|
|Tatro_011193-T1|	-1.7769276895162|	5.59275713588909|	87.8612261215152|	4.25120273152264e-09|	7.64536299237032e-06|
|Tatro_007063-T1|	-1.39013488320348|	6.72042447802748|	70.9803765515046|	2.67995471686695e-08|	1.6686234407108e-05|

## Perform KEGG pathway enrichment analysis in R
[Here](https://orlanc.github.io/cp_enrichment/R_enrichment/kegg_pathway_enrichment) you can see the R script for the enrichment analysis using *clusterprofiler*.
