High Frequency Trading Analysis
==============================

Project Overview: This project analyzes how bid-ask spreads affect trading behavior in high-frequency trading environments. Using LOBSTER limit order book data for Apple Inc. (AAPL) on June 21, 2012, the analysis focuses on understanding the relationship between spread size and execution activity. The notebook includes data loading, feature creation (e.g., spread and execution ratio), statistical hypothesis testing (correlation and t-test), and several visualizations.

Project Structure: This project uses the Cookiecutter Data Science structure:
data/raw/: Original message and order book CSV files
notebooks/: One notebook (EDA.ipynb) containing all analysis
reports/figures/: Output charts and plots
src/: Folder for future modular Python code
README.md: This documentation file

Dependencies: Python 3.9+ pandas numpy scipy matplotlib seaborn jupyter

Install all dependencies using:
pip install -r requirements.txt
Setup Instructions:
conda create -n hft-env python=3.9
conda activate hft-env
pip install -r requirements.txt
How to Run: Open the analysis notebook:
jupyter notebook notebooks/EDA.ipynb
The notebook includes: Loading LOBSTER message and order book data, Calculating spread and execution frequency, Plotting distributions and market behavior, Running Pearson correlation and t-tests, Saving visual outputs to reports/figures/

Reproducibility: The project is fully reproducible. All source data is in data/raw/, and no external data sources or randomness are used. You can rerun the notebook from start to finish to regenerate all results and figures.

Project Organization
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


--------

<p><small>Project based on the <a target="_blank" href="https://drivendata.github.io/cookiecutter-data-science/">cookiecutter data science project template</a>. #cookiecutterdatascience</small></p>
