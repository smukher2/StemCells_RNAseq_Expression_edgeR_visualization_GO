## This github repository is made open access in hope that it will enable researchers replicate and/or adapt it for their work. So if you use or adapt the results, inferences and computational pipelines presented here, I will be grateful if you please help by citing it as follows. 

### Github alternative link for download from protocol exchange: https://dx.doi.org/10.21203/rs.3.pex-977/v1

# Please help by citing this article and methods as follows (two citations): 
### Mukherjee, S. Quiescent stem cell marker genes in glioma gene networks are sufficient to distinguish between normal and glioblastoma (GBM) samples. Sci Rep 10, 10937 (2020). https://doi.org/10.1038/s41598-020-67753-5

### Mukherjee, S. Quiescent stem cell marker genes in glioma gene networks are sufficient to distinguish between normal and glioblastoma (GBM) samples Protocol Exchange (2020). https://dx.doi.org/10.21203/rs.3.pex-977/v1



# Author Information
Shradha Mukherjee*#
Address correspondence to: Shradha Mukherjee, PhD; Alias Goldy; Garland Avenue, Downtown Los Angeles, Los Angeles, CA 90017, U.S. Email: smukher2@gmail.com
* First author and # Corresponding author

Shradha Mukherjee, PhD in Biochemistry,                                                                                                                                       
MS in Chemistry, MAS in Health Informatics 

CV/Resume Link https://github.com/smukher2/Shradha_Mukherjee_Resume                                                                                      
Researchgate Link https://www.researchgate.net/profile/Shradha_Mukherjee                                                         
Github Link https://github.com/smukher2                                                                                                                                       
Pubmed Link https://www.ncbi.nlm.nih.gov/pubmed/?term=Shradha+Mukherjee   
Youtube Channel Link https://www.youtube.com/user/smukher2/playlists



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

