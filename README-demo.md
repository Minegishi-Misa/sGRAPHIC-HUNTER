# sGRAPHIC-HUNTER single cell analysis
Code from Minegishi et al. (2022) - "Genetic optical labeling of neighboring cells interrogates cell–cell interactions in metastatic niches." 


## System requirements
All code has been tested on R version 4.1.2 on MacOS 10.15 and 12.5. 


## Installation guide
Rstudio is downloaded from https://www.rstudio.com/. 
The libraries required for the analysis are listed at the beginning of the R scripts. 
The typical install time is within 30 min. 


## Demo

####  Data analysis 
To download the data analysis code, git clone using the following command: 

    git clone https://github.com/Minegishi-Misa/sGRAPHIC-HUNTER.git


## Scripts 

HUNTER_hepatocyte-cancercell.R outputs figures corresconding to Fig.3, 4, and S13 to S15 in the manuscripts of Minegishi et al. (2022).

10x_liver-cell-analysis.R outputs figures corresponding to Fig. S10c. 

## 10x format data

10x format to be loaded in Seurat is available from https://riken-share.ent.box.com/s/r7noivs3qn33y1etalbr4lx9v0mltga8. 
The directories correspond to the respective samples as follows:

- 20220411_scHUNTER: Index sorted single-cell data 

    hepatocyte
    |plate|condition|GFPlabel|mouse
    |--|--|--|--
    |P16|E0771 transplanted GFP posi|positive|transplanted
    |P17|control GFP nega|negative|control
    |P18|E0771 transplanted GFP nega|negative|transplanted
    |P19|E0771 transplanted GFP posi|positive|transplanted
    |P24|control GFP nega|negative|control
    |P25|control GFP nega|negative|control


    E0771 (breast cancer cell)
    |plate|condition
    |--|--
    |p02|E0771 vitro
    |P15|E0771 vivo
    |p20|E0771 vitro

- TK10x-01-P: 10x data of hepatocytes havested from the liver transduced with N-GR

- TK10x-02-S: 10x data of non-parenchymal cells harested from the liver transduced with N-GR

Expected outputs are commented as corresponding figure numbers at the end of each analysis code. 
Execution of all analyses takes less than a few days.
SCENIC analysis takes the most time.


####  Raw sequence data
 All demultiplexed sequencing data have been deposited on the Sequencing Read Archive and are available for download under accession PRJNA841462.


The code is released under the GNU Public License (GPL 3.0).


