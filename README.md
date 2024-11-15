Proteomics and Phosphoproteomics Analysis Project

This repository contains the code and documentation for conducting proteomics and phosphoproteomics analyses in R, generating visualizations, and performing API queries to STRING in Python. The project focuses on analyzing proteomic and phosphoproteomic data from various experiments, aiming to identify patterns, variations, and correlations to better understand the biological effects of different experimental conditions.

#############################################################################################
Author

Contact: julia.verheul@ibima.eu

This project was developed by Julia Verheul, a PhD student in the Neuropsychopharmacology group at IBIMA in Málaga.
#############################################################################################
Project Description

The project includes two main analyses:

    Alcohol Effect: Analysis of the impact of alcohol consumption on male rats, focusing on proteomic changes in the hippocampus.
    Alcohol Effect and Acute Immobilization Stress: A combined analysis to study the effect of alcohol exposure along with acute immobilization stress in male rats, focusing on alterations in the hippocampus.
#############################################################################################

Repository Structure

    data/: Folder containing processed data files and/or intermediate results. Both proteomics and phosphoproteomics data in this folder are normalized and ready for analysis.
    scripts/: Contains R scripts for the main analyses, including statistical analysis and heatmap generation.
    python/: Contains Python scripts for API queries, including interactions with the STRING database to retrieve additional data on proteins of interest.
    results/: Folder for storing final results and generated graphics, including specific results for phosphoproteomics.
#############################################################################################

Requirements

This project uses R and Python for data analysis, as well as the SEAOP software. Be sure to install the following packages and software before running the scripts:

R Package Installation

install.packages(c("effsize", "readxl", "data.table", "dplyr", "xlsx", "openxlsx", "igraph", 
                   "ggraph", "ggplot2", "ggrepel", "pheatmap", "RColorBrewer", 
                   "FactoMineR", "factoextra", "edgeR"))

SEAOP Installation

For statistical analysis and outlier detection, this project requires SEAOP. Make sure to follow the installation instructions in its repository to configure it properly before running the analyses.
https://academic.oup.com/bib/article/25/3/bbae129/7638267?login=true
https://github.com/whisperH/SEAOP)

Execution

    Data Preparation: Place your data in the data/ folder.
    Analysis in R: Use the scripts in the scripts/ folder to perform the main analysis, including statistical analysis, filtering, and heatmap generation.
    API Queries in Python: Run the scripts in the python/ folder to perform STRING database queries and obtain additional data on proteins of interest.
    Interpretation of Results: Generated results are saved in the results/ folder for interpretation.

