# Machine Learning Challenge 25/26 
[![DOI](https://zenodo.org/badge/1114744293.svg)](https://doi.org/10.5281/zenodo.18393435)
## Overview
This repository contains the submission of **Group 9**, composed of **Daniel Martins Borges (109474)** and **Duarte Pereira da Cruz (110181)**, for the **Machine Learning (IST) and NTT Data Challenge 2025/26**.

The primary deliverables are located in the [submission folder](./submission/), which contains both the [submitted notebook](./submission/notebook/Group09_notebook.ipynb) and the [submitted report](./submission/report/group9-report.pdf). For detailed information about the remaining folders, refer to the Repository Structure section below.

## Dataset 
The dataset is sourced from the repository available at:
https://github.com/ro-afonso/fake-news-pt-eu

## Installation Instructions
To set up the environment required to run the notebooks and load the trained models, follow the steps below.

**1. Create a virtual environment (recommended)**
```bash 
python3 -m venv .venv
source .venv/bin/activate     # Linux/macOS
.venv\Scripts\activate        # Windows
```
**2. Install dependencies**
From the root of the repository, run:
```bash
pip install -r requirements.txt
```
**3. Launch Jupyter Notebook**
```bash
jupyter notebook
```

## Repository Structure
### ```docs/```
Contains all documentation related to the challenge, including the official statement and internal notes.

### ```notebooks/```
Collection of notebooks used for data exploration, model training, and analysis.

#### ```notebooks/data/```
Contains the ```.csv``` files for the training, validation, and test datasets.

#### ```notebooks/no_punctuation/```
Notebooks for model training and analysis using a dataset cleaned by removing punctuation, special characters, extra whitespace, and converting all words to lowercase.

#### ```notebooks/no_punctuation_no_stop_words/```
Notebooks for model training and analysis using a dataset cleaned by removing punctuation, special characters, extra whitespace, Portuguese stop words, and converting all words to lowercase.

#### ```notebooks/punctuation/```
Notebooks for model training and analysis using a dataset cleaned by removing extra whitespace and converting all words to lowercase, while retaining punctuation.

#### ```notebooks/punctuation_no_stop_words/```
Notebooks for model training and analysis using a dataset cleaned by removing extra whitespace, removing Portuguese stop words, and converting all words to lowercase, while retaining punctuation.

#### ```notebooks/report_stuff/```
Notebooks used to generate the figures and supplementary materials included in the final report.

#### ```artifacts/```
Contains serialized vectorizers and trained models in ```.joblib``` format.

##### ```artifacts/no_punctuation/```
Includes vectorizers and the best-performing models trained on the corresponding preprocessed dataset. The notebooks used to generate these artifacts can be found [here](notebooks/no_punctuation/ex1.ipynb).

##### ```artifacts/no_punctuation_no_stop_words/```
Includes vectorizers and the best-performing models trained on the corresponding preprocessed dataset. The notebooks used to generate these artifacts can be found [here](notebooks/no_punctuation_no_stop_words/ex1.ipynb).

##### ```artifacts/punctuation/```
Includes vectorizers and the best-performing models trained on the corresponding preprocessed dataset. The notebooks used to generate these artifacts can be found [here](notebooks/punctuation/ex1.ipynb).

##### ```artifacts/punctuation_no_stop_words/```
Includes vectorizers and the best-performing models trained on the corresponding preprocessed dataset. The notebooks used to generate these artifacts can be found [here](notebooks/punctuation_no_stop_words/ex1.ipynb).

### ```report/```
Contains the final report and all associated assets.

#### ```report/assets```
Includes all visual elements and supplementary materials used in the report.

### ```submission/```
Contains the final submitted materials: the report and the consolidated notebook.

#### ```submission/notebook/```
Contains the final notebook representing the aggregated work from the ```no_punctuation_no_stop_words/``` notebooks and the ```report_stuff/``` notebooks.
