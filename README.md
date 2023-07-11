# peds_cancer_genes_vs_constraint
Code related to data wrangling, analysis, and visualization for the manuscript "The Evolutionary Impact of Childhood Cancer on the Human Gene Pool".

This repository contains compiled standalone source code. The code is entirely reproducible using publicly available data and software. 
The authors have only run the code using Windows 10, but the code language, Rmarkdown, should allow use on any operating system running R (version 4.2.2) through RStudio (version 2022.07.1) or later versions, i.e. incl. Mac and Linux.
The code does not require any non-standard hardware, although some data imports are large, hence 16GB of RAM or more is recommended. One exception to this is preparation of gnomAD data; as commented in the code, this was done using simple filter commands (as detailed in code comments), yet due to the size of the original publicly available data (see Data Availability Statement), this particular step was performed on a high-performance cluster, using a node with 144GB of RAM. This speeds up the step.
Installation of required software may be done following instructions from Posit (open source) at https://posit.co/download/rstudio-desktop/. Install time is typically counted in minutes.
The expected output of the code is metrics and visuals identical to those presented in the accompanying article. Exceptions are those where random data is extracted from large dataset; these are annotated using comments in the code.
One setup, the code should take less than an hour to run.


The code, written in Rmarkdown, has several dependencies; 
1) R (version 4.2.2) through RStudio (version 2022.07.1) + the libraries loaded in the setup chunk of the code,
2) the metadata, compiled in a single MS Excel sheet which is published as a supplement to the paper.
3) select data sets available from the links provided in comments in the relevant chunks of this code & in the Data Availability Statements provided in the published article.

Rerunning the code will require first downloading data and code, and then rewriting code to import all the downloaded data in accordance with points 2 & 3 above. Running chuck one-by-one will alert you to missing data/paths which will require updating to you path. 

Any questions or comments may be directed to me, Ulrik Stoltze (ulrik.kristoffer.stoltze@regionh.dk), as the corresponding author of the work.
