# Quo Vadis, Open Source? 
> Replication package of our paper "Quo Vadis, Open Source? The Limits of Open Source Growth" submitted to EMSE in 2021


## Introduction

With our study, we heavily rely on [Open Hub](https://www.openhub.net) (formerly known as Ohloh) and [its REST API](https://github.com/blackducksoftware/ohloh_api#ohloh-api-documentation). We collected our data during June 2021. This replication package aims to provide all necessary tools and (anonymized) data needed for a replication of our study or further research. 


## Requirements

We recommend a computer system with at least 10 GB storage and more than 32 GB RAM. 

If you want to recollect all data, you need Open Hub API keys which are not part of this repository but can be requested at [Open Hub](https://www.openhub.net/accounts/me/api_keys/new). On request, Open Hub grants you more requests per key for academic purposes. Depending on the number of daily API requests granted by Open Hub and your internet connection, the full crawling may take several days or even weeks. Those API keys must be stored as list (e.g. `['acf1bc432008d31f4a55bceb3a810758', 'e8482e1918181239ca183440ed7ced40']`) in the file `notebooks/api_keys.json`. 

For the tool-chain, you need:

1. Install jupyter using Python >= 3.2 (we are using `concurrent.futures` for crawling)
2. Install `pip3 install -r requirements.txt`

We also intend to provide a docker image soon.


## Structure

You will find three notebooks in the folder `notebooks`: `notebooks/01 Crawling.ipynb`, `notebooks/02 Preprocessing.ipynb`, and `notebooks/03 Visualizing.ipynb` which covers the three different stages of our analysis. Please notice that our API keys are not in this repository (see [Requirements](#requirements)). 

The data is stored in the subfolders of `data`, reflecting the raw data we have collected. The JSON files are named after their timestamp of collecting. Please notice that those datasets are already anonymized to comply to the [Black Duck Academic Use Agreement](https://web.archive.org/web/20170619090829/https://blog.openhub.net/academic-use-agreement). The required anonymization happens already in `notebooks/01 Crawling.ipynb`. 

All plots are stored in the folder `reports`. 


## Licenses

All code is licensed under MIT. Please consider the [Black Duck Academic Use Agreement](https://web.archive.org/web/20170619090829/https://blog.openhub.net/academic-use-agreement) regarding the data from Open Hub. 
