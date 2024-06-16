# <font color=lightblue>Lab 02 - Introduction To Data Science/ CSC14119</font>

General information
- Affiliation: Department of Computer Science, Faculty of Information Technology, University of Science, Vietnam National University, Ho Chi Minh City
- *LICENSE*
```
Lab 02 - Introduction To Data Science/ CSC14119 © 2023 by Department of Computer Science, Faculty of Information Technology, University of Science, Vietnam National University, Ho Chi Minh City is licensed under Attribution-NonCommercial-NoDerivatives 4.0 International
```

## <font color=lightblue>Laboratory instructions</font>

### <font color=lightblue>Set up your coding environment with Anaconda</font>

First, you should [download and install Anaconda](https://www.anaconda.com/download) for your operating systems. Then, starting install your development environment using ```requirements.txt```. 

**Note**: Suppose that you want to use Python 3.9, I built this requirement packages list base on Python 3.9. So if you want to install these packages in other Python version, please check all packages again via command ```conda search -c conda-forge -f  <package name>``` to verify the version of each package and change it in ```requirements.txt``` file. 

```bash
# create conda virtual environment
conda create --name min_ds-env python=3.9 -y

# activate created conda virtual environment
conda activate min_ds-env

# install dependencies
pip install -r requirements.txt
```

## <font color=lightblue>Laboratory structure explanation</font>

This lab project structure is built under the [Cookiecutter Data Science](https://github.com/drivendata/cookiecutter-data-science) - A logical, reasonably standardized, but flexible project structure for doing and sharing data science work. 

```
├── LICENSE-CC-BY-NC-ND-4.0.md
├── min_ds-env.yml
├── Makefile                 <- Makefile with commands like `make data` or `make train`
├── README.md                <- The top-level README for developers using this project.
├── data
│   ├── external             <- Data from third party sources.
│   ├── interim              <- Intermediate data that has been transformed.
│   ├── processed            <- The final, canonical data sets for modeling.
│   └── raw                  <- The original, immutable data dump.
│
│
├── models                   <- Trained and serialized models, model predictions, or model summaries
│
├── notebooks                <- Jupyter notebooks. Naming convention is a number (for ordering),
│                               the creator's initials, and a short `-` delimited description, e.g.
│                               `1.0-initial-data-exploration`.
│
├── references                <- Data dictionaries, manuals, and all other explanatory materials.
│
├── reports                   <- Generated analysis as HTML, PDF, LaTeX, etc. or your written by template such as https://github.com/Wandmalfarbe/pandoc-latex-template
│   └── figures               <- Generated graphics and figures to be used in reporting
│
├── requirements.txt          <- The requirements file for reproducing the analysis environment
│
├── src                       <- Source code for use in this project.
│   ├── __init__.py           <- Makes src a Python module
│   │
│   ├── data_module           <- Scripts to download or generate data
│   │   └── make_dataset.py
│   │
│   ├── features_module       <- Scripts to turn raw data into features for modeling
│   │   └── build_features.py
│   │
│   ├── models_module         <- Scripts to train models and then use trained models to make
│   │   │                        predictions
│   │   ├── predict_model.py
│   │   └── train_model.py
│   │
│   └── visualization_module  <- Scripts to create exploratory and results oriented visualizations
│       └── visualize.py
```

