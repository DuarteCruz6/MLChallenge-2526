# Machine Learning Challenge 25/26
## About
Submission of group 9, Daniel Martins Borges (109474) and Duarte Pereira da Cruz (110181)

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

## Structure
### Docs Folder
Folder containing all documents related to the challenge, including the statement and some notes we took.

### Notebooks Folder
#### Data Subfolder
Folder containing .csv files corresponding to the test dataset, the training dataset and the validation dataset.

#### No_Punctuation Subfolder
Folder containing the notebooks used for training and analysing each model in order to answer the questions in the statement. This dataset cleaning involved removing every punctuation, every special character, every extra whitespace and also making all words lowercase.

#### No_Punctuation_No_Stop_Words Subfolder
Folder containing the notebooks used for training and analysing each model in order to answer the questions in the statement. This dataset cleaning involved removing every punctuation, every special character, every extra whitespace, removing portuguese stop words and also making all words lowercase.

#### Punctuation Subfolder
Folder containing the notebooks used for training and analysing each model in order to answer the questions in the statement. This dataset cleaning involved removing every extra whitespace and also making all words lowercase.

#### Punctuation_No_Stop_Words Subfolder
Folder containing the notebooks used for training and analysing each model in order to answer the questions in the statement. This dataset cleaning involved removing every extra whitespace, removing portuguese stop words and also making all words lowercase.

#### Report Subfolder
Folder containing notebooks used to build the assets used in the report.

#### Artifacts Subfolder
##### No_Punctuation Subfolder
Folder containing .joblib files including the vectorizer and the best models of each type trained on the correspondent vectorizer. This dataset cleaning involved removing every punctuation, every special character, every extra whitespace and also making all words lowercase. Check the correspondent notebook folder [here](notebooks/no_punctuation/ex1.ipynb).

##### No_Punctuation_No_Stop_Words Subfolder
Folder containing .joblib files including the vectorizer and the best models of each type trained on the correspondent vectorizer. This dataset cleaning involved removing every punctuation, every special character, every extra whitespace, removing portuguese stop words and also making all words lowercase. Check the correspondent notebook folder [here](notebooks/no_punctuation_no_stop_words/ex1.ipynb).

##### Punctuation Subfolder
Folder containing .joblib files including the vectorizer and the best models of each type trained on the correspondent vectorizer. This dataset cleaning involved removing every extra whitespace and also making all words lowercase. Check the correspondent notebook folder [here](notebooks/punctuation/ex1.ipynb).

#### Punctuation_No_Stop_Words Subfolder
Folder containing .joblib files including the vectorizer and the best models of each type trained on the correspondent vectorizer. This dataset cleaning involved removing every extra whitespace, removing portuguese stop words and also making all words lowercase. Check the correspondent notebook folder [here](notebooks/punctuation_no_stop_words/ex1.ipynb).

### Report Folder
Folder containing the report and its assets.

#### Assets Subfolder
Folder containing the assets used in the report.