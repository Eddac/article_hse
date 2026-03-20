# Socio-Emotional Skills and Peer Networks in Higher Education
This repository contains the data and scripts required to reproduce the analyses presented in the manuscript submitted to the British Journal of Educational Psychology.

Repository Structure
Data/: Contains anonymized datasets in CSV/RDS formats.

Scripts/: R Markdown and Quarto files for data processing and analysis.

Analysis Pipeline
To replicate the results, please execute the scripts in the following numerical order:

01_data_cleaning.Rmd: Initial data preparation, including handling of missing values, variable renaming, and dataset merging.

02_network_construction.Rmd: Social Network Analysis (SNA) processing. Transforms raw sociometric nominations into directed, weighted igraph objects for the 8 classroom networks.

03_statics.Rmd: Main statistical modeling. Includes descriptive statistics of the sample and the Multiple Linear Regression models (Table 1) predicting Social Capital and GPA.

04_network_graphics.qmd: Psychometric Network Analysis. Estimation of Gaussian Graphical Models (EBICglasso) and generation of Figures 2, 3, and 4.

05_reliability_scales.Rmd: Psychometric evaluation of the instruments. Includes internal consistency metrics (Cronbach's Alpha and McDonald's Omega) for all SES and Personality scales.

Software Requirements
These analyses were performed in R (v4.3+) using the following core packages:

igraph & tidygraph (SNA)

qgraph & bootnet (Network Psychometrics)

tidyverse (Data Wrangling)

psych (Reliability)
