Swiggy-Delivery-Time-Prediction
==============================

Build ML model that can predict food delivery time

## 📌 Overview

This project builds a machine learning (ML) model to predict the time it takes to deliver food orders on Swiggy, a popular online food delivery service. The goal is to estimate delivery time in minutes using data from orders, locations, and other factors. This can help improve customer experience and optimize operations for delivery partners.
The project follows a standard data science workflow, starting from data collection to model training and evaluation. It uses Python and common libraries for data processing and ML.


## 🔑 Key Objectives

- Collect and prepare data on food delivery orders.
  
- Build features from raw data, such as distance between restaurant and customer.
  
- Train ML models to predict delivery time accurately.
  
- Evaluate model performance and create visualizations for insights.

## 🤖 Technologies Used

1. **Programming Language**: Python 3.x

2. **Data Processing**: Pandas, NumPy

3. **Machine Learning**: Scikit-learn (for models like regression)

4. **Visualization**: Matplotlib, Seaborn

5. **Environment Management**: Pip, requirements.txt

6. **Documentation**: Sphinx

7. **Project Structure**: Cookiecutter Data Science template


## 📂 Dataset
The dataset includes historical Swiggy order data with features like:

1. Order placement time
   
2. Restaurant and customer locations (latitude/longitude)
   
3. Order type and size
   
4. Traffic conditions 

Data is stored in the **data/raw** folder. Processed versions go to **data/processed** for modeling.



## Usage
Run the following commands using the Makefile:

1. **Prepare data**: make data

2. **Build features**: make features

3. **Train model**: make train

4. **Predict**: make predict

5. **Visualize results**: make visualize

For exploration, open Jupyter notebooks in the notebooks folder, such as 1.0-initial-data-exploration.ipynb.



🧱 Project Structure
------------

    ├── LICENSE
    ├── Makefile           <- Makefile with commands like `make data` or `make train`
    ├── README.md          <- The top-level README for developers using this project.
    ├── data
    │   ├── external       <- Data from third party sources.
    │   ├── interim        <- Intermediate data that has been transformed.
    │   ├── processed      <- The final, canonical data sets for modeling.
    │   └── raw            <- The original, immutable data dump.
    │
    ├── docs               <- A default Sphinx project; see sphinx-doc.org for details
    │
    ├── models             <- Trained and serialized models, model predictions, or model summaries
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


## ✅ Results
The model achieves [insert accuracy metric, e.g., RMSE of 5-10 minutes] on test data. Key findings include that distance and time of day are strong predictors of delivery time. Check **reports/figures/** for charts.

--------

<p><small>Project based on the <a target="_blank" href="https://drivendata.github.io/cookiecutter-data-science/">cookiecutter data science project template</a>. #cookiecutterdatascience</small></p>
