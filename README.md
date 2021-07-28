

# public-ADMTF-data-notebooks
This repository contain the ***datasets***, ***notebooks*** and ***model*** necessaries to process the data of ***ADMTF*** (Automatic Diagnosing of Migraines and Trigger Factors) thesis.

### Dataset files:

  * ***'/DMS_datasets/S1_File_Preprocesed.xlsx'*** Google Sheet data table with original data from [Analysis of Trigger Factors in Episodic Migraineurs Using a Smartphone Headache Diary Applications](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0149577) article, especific URL from download original excel file here: [Dataset of 62 patients, 1099 Headache Diary Records, and 4579 Diary Records.](https://doi.org/10.1371/journal.pone.0149577.s001) This file was processed with Google Sheets macros to get ***Tab-totalDiary4578Filtered***
  * ***'/DMS_datasets/totalDiary4578Filtered.csv'*** CSV file exported from google sheet data table ***'S1_File_Preprocesed.xlsx (Tab-totalDiary4578Filtered)'*** 
  * ***'migraines_db_table.csv'*** CSV file with all migraines available data which has been extracted from ***'/DMS_datasets/totalDiary4578Filtered.csv'***.

### Notebooks and  Repository:

 In this repository are the main *Jupyter notebooks* used for *ADMTF* thesis, which are:

* ***'ADMTF ML Models for Diagnosing Migraine Situations (DMS).ipynb'***. This notebook included the processing to get the convenient machine learning model, in this case the selected model has been a ***Balanced Logistic Regression with optimal threshold setting***   

* ***'ADMTF_Stress_LackSleep_Eval (SLSE).ipynb'***. This notebook included the processing of datasets download from ***Apple Watch*** to get the charts with the evolution of ***stress*** and ***lack of sleep*** as the migraine triggers factors.
* ***'DFrame_To_MySQLDBase_TableMigraines (DFTDB).ipynb'***. This notebook include the processing of migraines dataset to prepare it to included into MySQL database.
* ***'Plot_Triggers_Migraines_Results (PTM).ipynb'***. This notebook including the processing to get the Plotly visualizations to compare visually which triggers factors are prevalent (causing migraines) for each individual person and all people in datashet.

### Logistic Regression model file:

* ***'ADMTF_LR_Model.pkl'*** Package file with the logistic regression machine learning model calculated.

