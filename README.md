Aid for Victims of Crimes: LA Support Strategies
=============================================

> By utilizing LAPD crime records to develop predictive models, we have now established a tool for anticipating the age and gender of individuals impacted by criminal activities. This dataset captures instances of criminal activities in Los Angeles since 2020. The information is derived from crime reports originally documented on paper, which presented several challenges in the completeness and structure of the collected data.**
> 
>To navigate this and achieve working models, several techniques were applied, such as imputation, encoding, vectorization, and assessment of feature importance. Two models were derived due to the nature of the target variables (i.e., gender is categorical, and age is numerical). The final products are a Random Forest and Gradient Boosting model.

Project Organization
------------

    ├── LICENSE
    ├── README.md          <- The top-level README for developers using this project.
    ├── data
    │   ├── Links to Data.txt   <- Project data stored on Google cloud  
    │       ├── data            <- Navigate to this using the Project Data Link within 'Links to Data.txt'
    │             ├── interim   <- Intermediate data that has been transformed (Various versions available)
    │                 
    │                 └── 2010-2023 Crime_Traffic_Collisions_Data_R1 .csv     <- 1st revision of data during wrangling/cleaning
    │                 └── 2010-2023 Crime_Traffic_Collisions_Data_R2 .csv     <- 2nd revision of data during wrangling/cleaning
    │                 └── victim_age_feature_data_unscaled.csv                <- split preprocessed input data before scaling
    │                 └── victim_age_target_data_unscaled.csv                 <- split preprocessed target data before scaling
    │                 └── victim_sex_feature_data_unscaled.csv                <- split preprocessed input data before scaling
    │                 └── victim_sex_target_data_unscaled.csv                 <- split preprocessed target data before scaling
    │    
    │             ├── processed  <- The final, canonical data sets for modeling.                                  
    │                  └── victim_age_feature_data_processed.csv           <- fully preprocessed data ready to train model
    │                  └── victim_age_target_data_processed.csv            <- fully preprocessed data ready to train model
    │                  └── victim_sex_feature_data_processed.csv           <- fully preprocessed data ready to train model
    │                  └── victim_sex_target_data_processed.csv            <- fully preprocessed data ready to train model
    │                  
    │             ├── raw    <- Data from third party sources
    │                   └── 2010-2023 Crime_Traffic_Collisions_Data .csv  <- The original, immutable data dump.   
    │
    ├── docs               <- A default Sphinx project; see sphinx-doc.org for details
    │
    ├── models             <- Trained and serialized models
    │   ├── Links to Data.txt   <- pkl files stored on Google cloud  
    │
    ├── notebooks          <- Jupyter notebooks. Naming convention is a number (for ordering),
    │                         the creator's initials, and a short `-` delimited description, e.g.
    │                         `1.0-jqp-initial-data-exploration`.
    │
    ├── references         <- Data dictionaries, manuals, and all other explanatory materials.
    │
    ├── reports            <- Generated analysis as HTML, PDF, LaTeX, etc.
    │   └── figures        <- Generated graphics and figures to be used in reporting
    │
    ├── requirements.txt   <- The requirements file for reproducing the analysis environment, e.g.
    │                         generated with `pip freeze > requirements.txt`
    │
    ├── setup.py           <- makes project pip installable (pip install -e .) so src can be imported
    ├── src                <- Source code for use in this project.
    │   ├── __init__.py    <- Makes src a Python module
    │   │
    │   ├── data           <- Scripts to download or generate data
    │   │   └── make_dataset.py
    │   │
    │   ├── features       <- Scripts to turn raw data into features for modeling
    │   │   └── build_features.py
    │   │
    │   ├── models         <- Scripts to train models and then use trained models to make
    │   │   │                 predictions
    │   │   ├── predict_model.py
    │   │   └── train_model.py
    │   │
    │   └── visualization  <- Scripts to create exploratory and results oriented visualizations
    │       └── visualize.py
    │
    └── tox.ini            <- tox file with settings for running tox; see tox.readthedocs.io


--------

<p><small>Project based on the <a target="_blank" href="https://drivendata.github.io/cookiecutter-data-science/">cookiecutter data science project template</a>. #cookiecutterdatascience</small></p>
