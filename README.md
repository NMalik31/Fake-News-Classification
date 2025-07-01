# Fake News Classification

This repository contains my solution to the Fake News Classification problem. The main notebook (`Project_54_Fake_News_Classifier.ipynb`) implements a full pipeline for identifying fake and real news articles using NLP and machine learning. All custom text preprocessing and NLP utilities are modularized in `nlp_utils.py`.

## Project Highlights

- Built and evaluated supervised learning models to classify news articles as fake or real.
- Applied preprocessing techniques including contraction removal, tokenization, stemming, and lemmatization (see `nlp_utils.py`).
- Feature engineering using TF-IDF and CountVectorizer.
- Performed EDA and label distribution analysis.
- Used scikit-learn for model development and validation.

## Structure

```
.
├── Project_54_Fake_News_Classifier.ipynb   # Main notebook (NLP pipeline, EDA, modeling)
├── nlp_utils.py                            # All custom NLP/text-preprocessing functions
├── requirements.txt                        # Python dependencies (optional)
└── README.md
```

## Dataset

The dataset (`train.csv`) is not included here due to its size.  
I used the [Kaggle Fake News dataset](https://www.kaggle.com/c/fake-news/data).  
To reproduce results, download the train file from Kaggle and place it in the repo root.

## Usage

- All code is in the notebook.  
- Custom functions are imported from `nlp_utils.py`.
- Run locally with Jupyter or in Colab (the notebook includes Colab drive mounting code).
- Example import:
  ```python
  from nlp_utils import lemmatization_sentence
  ```

## Environment

- Python 3.x
- Main libraries: pandas, numpy, scikit-learn, nltk, seaborn

## .gitignore

I kept large datasets out of version control; see `.gitignore`:
```
train.csv
test.csv
data/
*.zip
```

## License

MIT

---

*This project is part of my portfolio. For details or collaboration, feel free to reach out or open an issue.*
