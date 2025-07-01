# Fake News Classification

This project is a machine learning pipeline for classifying news articles as real or fake, using natural language processing (NLP) techniques and supervised learning. The workflow is implemented in a Jupyter Notebook (`Project_54_Fake_News_Classifier.ipynb`) and uses a custom Python module (`nlp_utils.py`) for text preprocessing utilities.

---

## Table of Contents

- [Project Structure](#project-structure)
- [Features](#features)
- [Getting Started](#getting-started)
- [Dataset](#dataset)
- [Usage](#usage)
- [Example](#example)
- [Notes](#notes)
- [License](#license)
- [Acknowledgments](#acknowledgments)

---

## Project Structure

```
.
├── Project_54_Fake_News_Classifier.ipynb   # Main Jupyter Notebook
├── nlp_utils.py                            # Custom text preprocessing utilities
├── requirements.txt                        # (Optional) Python dependencies
└── README.md                               # Project documentation
```

---

## Features

- **Data loading and cleansing:** Handles missing values and prepares the dataset.
- **Text preprocessing:** Custom utilities for contraction removal, tokenization, stemming, and lemmatization (`nlp_utils.py`).
- **Exploratory data analysis (EDA):** Visualization and label distribution analysis.
- **Feature engineering:** TF-IDF and Count Vectorization.
- **Model training and evaluation:** Supervised machine learning for fake news detection.

---

## Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/NMalik31/Fake-News-Classification.git
cd Fake-News-Classification
```

### 2. Install dependencies

You can install the required packages using pip:

```bash
pip install numpy pandas scikit-learn matplotlib seaborn nltk
```
Or install from `requirements.txt` if provided:

```bash
pip install -r requirements.txt
```

### 3. Download the Dataset

**The training dataset (`train.csv`) is too large to be included in this repository.**  
Please download the dataset from its source (e.g., [Kaggle - Fake News Dataset](https://www.kaggle.com/c/fake-news/data)) and place the file(s) in the project root directory.

_**Update the file paths in the notebook if your dataset is located elsewhere.**_

---

## Dataset

- The project expects a CSV file (e.g., `train.csv`) with columns: `id`, `title`, `author`, `text`, `label`.
- **Do NOT upload large datasets to the repository.**  
  Instead, add dataset files to `.gitignore` and instruct users via the README.

**Example .gitignore:**
```
train.csv
test.csv
data/
*.zip
```

---

## Usage

- The notebook will walk you through data exploration, text preprocessing, feature extraction, model training, and evaluation.
- Custom NLP functions are defined in `nlp_utils.py` and imported into the notebook:

```python
from nlp_utils import w_tokenization, stemming, lemmatization_sentence
```

---

## Example

Load the training data:
```python
import pandas as pd
df = pd.read_csv('train.csv')
```

Use a custom function:
```python
from nlp_utils import lemmatization_sentence
lemmatized_text = lemmatization_sentence("The cats are running fast.")
print(lemmatized_text)
```

---

## Notes

- Ensure both `Project_54_Fake_News_Classifier.ipynb` and `nlp_utils.py` are in the same directory when running the notebook.
- Download required NLTK resources if prompted (e.g., `punkt`, `wordnet`, `averaged_perceptron_tagger`).
- The notebook is compatible with both local Jupyter and Google Colab environments.

---

## License

This project is open-source and available under the MIT License.

---

## Acknowledgments

- Inspired by best practices in data science and NLP.
- Thanks to open-source contributors in the Python and NLP communities.

---

*For questions or contributions, please open an issue or submit a pull request.*
