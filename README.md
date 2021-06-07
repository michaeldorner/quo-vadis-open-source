# Quo Vadis, Open Source? 
> Replication package of our paper "Quo Vadis, Open Source? The Limits of Open Source Growth" submitted to EMSE in 2021. 


# Requirements

We recommend a computer system with at least 10 GB storage and more than 32 GB RAM. If you want to recollect all data, you need Open Hub API keys which are not part of this repository, but can requested at www.openhub.com (please see [Introduction](# Introduction) for more details).

For the tool-chain, you need:

1. Install jupyter using Python >= 3.2 (we are using concurrent.futures for crawling)
2. Install `pip3 install -r requirements.txt`

We also intend to provide a docker image soon.


# Introduction

You will find three notebooks in the folder `notebooks`: `notebooks/01 Crawling.ipynb`, `notebooks/02 Preprocessing.ipynb`, and `notebooks/03 Visualizing.ipynb` which covers the three different stages of our analysis. Obviously, API keys are not in this repository. Create an Open Hub account and create API keys. On request, Open Hub grants you more requests per key for academic use. Those new API keys must be stored as list (e.g. `['acf1bc432008d31f4a55bceb3a810758', 'e8482e1918181239ca183440ed7ced40']`) in the file `notebooks/api_keys.json`. 

The data is stored in the subfolders of `data`, reflecting the raw data we have collected. The JSON files are named after their timestamp of collecting. Please notice that those datasets are already anonymized to confirm to the [Black Duck Academic Use Agreement](https://web.archive.org/web/20170619090829/https://blog.openhub.net/academic-use-agreement). The required anonymization happens already in `notebooks/01 Crawling.ipynb`. 

All plots are stored in the folder `reports`. 
