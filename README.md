# Soil health cluster analysis based on national monitoring of soil indicators
This repository contains the Python code and instructions necessary to replicate the analysis presented in the Soil Health Cluster Analysis paper using the Osyris Replicate python package. The paper analyzes a comprehensive national-scale dataset of topsoil properties in Wales, UK, demonstrating how different land uses impact soil health and function, and proposes a new way of classifying soils based on their functional properties rather than traditional soil genesis classifications. 

## Steps to Replicate the Analysis

### Getting started
Install and import the package

`pip install osreplicate`\
`from osreplicate import Paper`

### Access the paper you want to replicate
Provide the papers alias to start analyzing

`analysis = Paper('ejss/Soil Health Cluster Analysis')`

### Get the datasets
Locally download any available datasets associated with this paper

`analysis.get_data()`

### Replicate the paper
Automatically run the full analysis on the available datasets and reproduce the figures from the paper

`analysis.run()`

### Mix and match      
Access core analysis methods from to the paper

`analysis. get_summary_statistics_by_habitat(data)`\
`analysis.plot_soil_properties(data)`\
`classify_soils_using_cluster_analysis(data, properties)`\
`correlate_clusters_with_habitats(cluster_data, habitat_data)`\
