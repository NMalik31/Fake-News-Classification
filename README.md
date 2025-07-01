# Fake News Classification

This repository contains my work on classifying fake and real news articles using NLP and machine learning. The main code is in `Project_54_Fake_News_Classifier.ipynb`, with all text preprocessing and custom NLP utilities modularized in `nlp_utils.py`.

## Project Highlights

- Supervised learning models to predict fake vs. real news.
- Custom preprocessing: contraction handling, tokenization, stemming, lemmatization (see `nlp_utils.py`).
- Feature extraction with TF-IDF and CountVectorizer.
- EDA and label distribution analysis.

## Repository Structure

```
.
├── Project_54_Fake_News_Classifier.ipynb   # Main notebook
├── nlp_utils.py                            # Custom NLP/text-preprocessing functions
├── requirements.txt                        # (optional) dependencies
└── README.md
```

## Dataset

**Note:** The train dataset is not included in this repo due to its size and privacy.  
It is a local file on my machine, not from Kaggle or a public source.  
If you want to run the notebook, place your own `train.csv` with the columns:  
`id, title, author, text, label`  
in the project root directory.

## Usage

- All code and workflow are in the notebook.
- Custom functions are imported from `nlp_utils.py`
- Notebook can be run locally (Jupyter) or on Colab.
- Example import:
  ```python
  from nlp_utils import lemmatization_sentence
  ```

## Environment

- Python 3.x
- pandas, numpy, scikit-learn, nltk, seaborn

## .gitignore

Large datasets are excluded from version control:

```
train.csv
test.csv
data/
*.zip
```

## License

MIT

---

*Project for my portfolio. For more info or collaboration, please reach out or open an issue.*
