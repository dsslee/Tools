```
|--- README.md                  <-- top-level README for developers
|
|--- dataset
|       |--- 01_raw             <-- Immutable input data
|       |--- 02_raw_cleaned     <-- cleaned version of raw
|       |--- 03_processed       <-- data used to develop model
|       |--- 04_models          <-- trained models
|       |--- 05_model_outputs   <-- model ouput
|       |--- 06_reports         <-- log 
|       
|--- notebooks                  <--- jupyter notebooks: EDA + experimental codes
|       |                             naming convention: year_initial_shortDescription
|       |                                                ex. YYYYMMDD_ds_eda1.ipynb
|       |-- n01_EDA             <--- collection of EDA notebooks
|       |
|       |-- n02_experiments     <--- when experiment code is complete, 
|                                    migrate to the src under appropriate sub-folder
|
|--- src
|     |--- __init__.py  
|     |
|     |--- s00_utils                <--- makes src a python module
|     |
|     |--- s01_data                 <--- scripts to reading and writing data etc
|     |
|     |--- s02_processing          <--- scripts to turn cleaned data to modelling input
|     |
|     |--- s03_model                <--- scripts for model architecture 
|     |
|     |--- s04_train                <--- scripts to train models and use to make predictions
|     |
|     |--- s05_model_evaluation     <--- scripts to analyze model performance and model selection
|     |
|     |--- s06_reports              <--- scripts to generate reports such as log
|     |
|     |--- s07_visualization        <--- scripts to create frequently used plots
|
|
|--- .gitignore
|
```
