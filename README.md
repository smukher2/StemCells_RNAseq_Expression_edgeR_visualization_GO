Format: the pipelines are provided as 1)Rmarkdown files knit to html 2) Rmarkdown files knit to pdf and 3) Rmarkdown or rmd files that can be opened and run on Rstudio by just hitting the "run current chunk" button

This pipeline shows steps from input count data-(to)->Differential gene expression (edgeR)-(to)->Visualization-(to)->GO analysis, pathway analysis and DisGeNet analysis
1) Differential gene expression analysis with edgeR
2) Visualization with boxplots, heat-map and corelation matrix
3) GO analysis, DisGeNet, KEGG pathway and Reactome pathway analysis
This pipeline can be applied to any RNA-seq count data.

Sample dataset is obtained from: 
1) GSE68270, Hippocampal activated stem cell and neuron data was obtained from Walker TL, Overall RW, Vogler S, Sykes AM et al. Lysophosphatidic Acid Receptor Is a Functional Marker of Adult Hippocampal Precursor Cells. Stem Cell Reports 2016 Apr 12;6(4):552-565. PMID: 27050949
2) GSE52564, Cortex neurons, astrocytes, oligodendrocyte precursor cells, newly formed oligodendrocytes, myelinating oligodendrocytes, microglia and endothelial cells data was obtained from Zhang Y, Chen K, Sloan SA, Bennett ML et al. An RNA-sequencing transcriptome and splicing database of glia, neurons, and vascular cells of the cerebral cortex. J Neurosci 2014 Sep 3;34(36):11929-47. PMID: 25186741
Disclaimer: I have not contrinuted to the above publication. 

Details on input data files:
1) Raw reads were downloaded from GSE52564 and GSE68270 NCBI/GEO, processed and mapped on mm9 genome with Tophat2. Finally, counts were generated with HTseq and merged to a single file 'merged_scVSnonsc_counts.txt'  

2) A metadata file was created matching the columns of the input count file 'merged_scVSnonsc_counts.txt' and is saved as 'scVSnonsc_metadata.txt'. 

