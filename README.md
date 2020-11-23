# single-cell sequencing and annotation using scCATCH

## Description:

This repository consists of a R script for single-cell analysis using Seurat and annotation based on scCATCH.<br/>
It is divided into 3 parts:

### Part 1: Creation of Seurat Objects, Finding anchors and Integrating the data using Seurat
This block of commands performs the typical Seurat single cell functions by creating the Seurat object, filtering the data, finding the clusters and creating plots like UMAP for visualization.Then, it finds anchors and integrates the entire dataset for further analysis. <br/>

### Part 2: Annotation with scCATCH
scCATCH is used to realize the automatic annotation for each identified cluster. For this, please define the species, cancer type and tissue type accordingly.<br/>
https://github.com/ZJUFanLab/scCATCH <br/>

### Part 3: Finding gene markers in the clusters
This section of the code helps to display all the markers associated in each cluster and plotting them for noting the differential gene expression.<br/>


## Environment set-up 

### Packages for R:

   *Note 1:  Install the packages in the order listed below.* <br/>

   *Note 2:  When installing the following packages, if you are asked to select (a/s/n) or (y/n), please select “a” or "y" as applicable.* <br/>

   *Note 3: All the package names listed below are case sensitive!* <br/>

1. Install all the packages listed below from CRAN using **install.packages()** function. <br/>
  
  -devtools <br/>
  -Seurat <br/>
  -cowplot <br/>
  -ggplot2 <br/>
  -patchwork <br/>
  -metap <br/>
 
 
2. Install the scCATCH package from Bioconductor using the the BiocManager::install() function.

   ```
   BiocManager::install("scCATCH")
   ```
   
3. Finally, please check that all the packages were installed successfully by loading them one at a time using the library() function.

   ``` 
   library(Seurat)
   library(metap)
   library(scCATCH)
   ```
       

  
