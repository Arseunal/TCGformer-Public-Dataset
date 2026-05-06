# Public Dataset for TCGformer

This repository contains a publicly available, unrestricted dataset used to verify the code execution of the **TCGformer** model.

## ⚠️ Important Data Provenance & Privacy Notice
The original empirical analysis presented in our manuscript ("TCGformer: A temporal causal graph enhanced transformer model for multivariate financial time series forecasting") utilized proprietary financial data sourced from the China Stock Market and Accounting Research (CSMAR) Database. 

Due to strict commercial licensing and copyright restrictions imposed by CSMAR, we are legally prohibited from extracting and distributing the original raw or preprocessed data on public repositories.

To fully comply with Open Science and Open Data policies, and to allow researchers to test, execute, and reproduce our model's logic, we provide this equivalent, publicly available dataset sourced from https://finance.yahoo.com.

This public dataset has been formatted identically to our original proprietary dataset to ensure seamless plug-and-play compatibility with our released codebase.

## Files Included
price_fillna_paper4.csv & return_fillna_paper4.csv: The time series data containing the features and targets for the model.
temporal_adj_matrices.pkl: The temporal graph structures required for the GNN routing mechanism.

## Usage
You can place these files directly into the `dataset/` directory of the TCGformer codebase. The model scripts (e.g., `run.py`) will automatically process them as they share the same data structure as the original study.

For researchers who hold an active institutional subscription to the CSMAR database (https://data.csmar.com/), you may download the original data matching the timeframes and tickers described in our paper to fully replicate the exact numerical results.
