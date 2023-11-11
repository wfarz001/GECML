# GECML
This is a course project where the goal was to develop data pre-processing pipeline and machine learning model to identify tumor using genomic expression and clinical data.
Please refer to the presentation file for details and steps.

Genomic Expression and Clinical data unsupervised clustering to build machine learning model for survival analysis.
The Cancer Genome Atlas(TCGA) research networks avails large collection of clinical and molecular phenotypes of 10,000 tumor patients with 33 different tumor type.

TCGA data have some bioinformatics challenges which includes data retrieval, integration of clinical data with molecular data (RNA,DNA methylation).

R/Bioconductor package called TCGAniolinks address these challenges through a guided workflow for users.

The workflow allows query, download and performance analysis.

TCGAbiolinks aids in querying, downloading, analyzing and integrating TCGA data within a single collective Bioconductor package.
![image](https://github.com/wfarz001/GECML/assets/105995578/3b912a87-cef5-4b83-8cc2-de530de5a4c7)
The aim of the TCGABiolinks divided into four folds:


Facilitate data retrieval via TCGA’s DCCWS( Data Coordination Center’s Web Service)

Prepare data using appropriate pre-processing strategies

Provide opportunities to conduct standard analysis and advanced integrative analyses

Allow users to download specific version of the data and easily produce research results


TCGABiolinks functions can be grouped into three levels: Data, Analysis and Visualization.

Data handles retrieval and query of TCGA data and consists of three main functions: GDCquery, GDCdownload, GDCprepare.

TCGAanalyze comprises two type of analysis: molecular and clinical analysis. TCGAanalyze_Normalization allows to normalize mRNA transcripts and miRNA using EDASeq package.

TCGAanalyze_DEA allows users to identify differential expression or regions between two populations or conditions.
![image](https://github.com/wfarz001/GECML/assets/105995578/6396e5b8-8a37-44f6-b7d8-4a5fcee65fd1)
The visualization section allow to visualize the results generated by analysis section using heatmap, clusters, principal component analysis (PCA).

Two case studies are conducted to perform classical analysis using clinical and genomic data from the Cancer Genome Atlas (TCGA).

The following steps are followed for the two case studies:

        1. Downloading the data (clinical and expression) from TCGA

        2. Processing the Data (normalization) and saving it locally using table format

        3. Unsupervised analysis includes differential analysis, PCA and clustering

        4. Building a machine learning model(classifier) to predict cancer.

        5. Perform survival analysis of molecular markers detected in previous analysis.
![image](https://github.com/wfarz001/GECML/assets/105995578/836c348e-e396-4eeb-92fb-bafef414aeaa)
