# Quo Vadis, Open Source? 
Replication package 

# Introduction
This is the replication package of our paper "Quo Vadis, Open Source?" submitted to EMSE. 

# Install

1. Install jupyter using Python >3.5
2. Install `pip3 install -r requirements.txt`


# Use

There are three notebooks: `notebooks/01 Crawling.ipynb`, `notebooks/02 Preprocessing.ipynb`, and `notebooks/03 Visualizing.ipynb` which covers the different stages of our analysis. Obviously, API keys are not in this repository. Create an Open Hub account and create API keys. On request, Open Hub grants you more requests per key for academic use. Those new API keys must be stored as list (e.g. `['acf1bc432008d31f4a55bceb3a810758', 'e8482e1918181239ca183440ed7ced40']`) in the file `notebooks/api_keys.json`. 


The data is stored in the subfolders of `data`, reflecting the raw data we have collected. The JSON files are named after their timestamp of collecting. Please notice that those datasets are already anonymized to confirm to the [Black Duck Academic Use Agreement](https://web.archive.org/web/20170619090829/https://blog.openhub.net/academic-use-agreement). 

All plots are stored in the folder `reports`. 
