# **Maplet_in_Microbiome_Analysis**

Maplet is an R package for statistical data analysis specifically focusing on metabolomics datasets (Chetnik et al. "maplet: An extensible for modular and reproducible omics pipelines". Bioinformatics, 2021). 

To get started with Maplet, you need to install the latest stable version of maplet using the following command:

```
devtools::install_github(repo="krumsieklab/maplet@v1.2.1", subdir="maplet")
```

Additional information about the installation of maplet and examples on how to use maplet can be found on the github page of the package [here](https://github.com/krumsieklab/maplet). 


# **The Aim of this Project**

The usage of multi-omics and bioinformatics approaches in the gut microbiome and metabolome field has gained more attention recently. 

Here, we used "Maplet" and R to analyze a publicly available dataset from the paper "Gut microbiome structure and metabolic activity in inflammatory bowel disease" (Franzosa et al., 2019). [Link to publication](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC6342642/pdf/nihms-1510763.pdf). 

We did that to: 
     
      1- Check the feasibility of using Maplet in metabolome and gut microbiome data analysis 
      2- Check the reproducibility of the results generated from the article 

# **Getting Started with the Project**

To get started, we first downloaded and saved the supplementary dataset from the above paper. 

You can find the available supplementary data [here](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC6342642/).

The supplementary files show the results of two metabolome and microbiome datasets for patients with CD, UC, or control (PRISM: 155 samples and validation cohort: 65 samples) - as a start we focused in this exercise on the PRISM samples. 

We then used the supplementary files to create a new excel file with all the necessary data we need for our analysis under the name: **"Metabolome_data.xlsx"**. 

The new excel file "Metabolome_data.xlsx" has the metadata, metabolite abundance, and features of the 155 PRISM samples in three separate sheets (Metabolome_metadata_PRISM, Metabolite_abundance_PRISM, and the Metabolite_features)

**You can find the "Metabolome_data.xlsx" file under the "Metabolites_Dataset" folder above** 

# **Starting the Analysis**

We first loaded the "Metabolome_data.xlsx" data and annotations in R

We preprocessed the data based on the three diagnosis and performed :(quotient normalization, imputation, and missing values filtering) and generated an html report of the pre-processing results

The html report gives a summary output of all the functions/ tests performed on the data

**Below is a screenshot of the html report generated** 

![Screen Shot 2023-07-22 at 11 45 35 AM](https://github.com/RKA2020/Maplet_Gut_Data/assets/127655038/fbc58eb7-2ae9-4410-ac0b-a020e8c4ea9f)

The codes for the preprocessing part and the full html report can be found in R_Codes folder under the file:(STARTING_The_METABOTOOLS_PIPELINE) 
                 

