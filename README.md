# 🧠 Feature Extraction Activity

This repository contains a Jupyter Notebook that performs **text normalization** and **feature extraction** on a dataset of reviews.  
It includes preprocessing steps like punctuation removal, spell checking, stopword removal, stemming, and lemmatization — followed by **Bag-of-Words (BoW)** and **TF-IDF** feature generation.


## 📁 Project Structure

The project is organized inside the `Feature Extraction/` directory.  
All input and output files are handled within this folder, and all generated CSV outputs are stored in the respective subfolders.

```

Feature Extraction/
├── lemmatization/
│   ├── .gitkeep
│   └── (Generated CSV outputs appear here)
├── stemmer/
│   ├── .gitkeep
│   └── (Generated CSV outputs appear here)
├── Fin_lab-PRProject_dataset.csv       # Input dataset
└── Paredes_Feature_Extraction.ipynb    # Main Jupyter notebook

Text Extraction/
.gitignore
README.md

```

---

## ⚙️ How to Run

All paths in the notebook are **relative**, so setup is straightforward.

1. **Install dependencies**  
   The first cell of the notebook automatically checks and installs the following packages:
```

pandas, nltk, autocorrect, scikit-learn, tqdm, better-profanity

```

2. **Open and run the notebook**  
Launch and execute:  
```

Feature Extraction/Paredes_Feature_Extraction.ipynb

````

3. **Processing steps**
- Reads dataset from `Feature Extraction/Fin_lab-PRProject_dataset.csv`
- Cleans and normalizes text:
  - Removes punctuation and unwanted characters  
  - Applies spell correction  
  - Removes stopwords  
  - Performs stemming and lemmatization  
- Generates and saves BoW and TF-IDF features into:
  ```
  Feature Extraction/lemmatization/
  Feature Extraction/stemmer/
  ```

---

## 📝 Repository Notes

- **`.gitignore`**  
Configured to ignore all `*.csv` files and the `Text Extraction/` folder.  
This prevents large datasets and generated outputs (e.g., `bow_features_lemmatized.csv`) from being committed.

- **`.gitkeep`**  
Since Git does not track empty directories, `.gitkeep` files act as placeholders.  
They ensure that the `lemmatization/` and `stemmer/` directories remain in the repository so the notebook can save its outputs properly.

---
````

---

Would you like me to include GitHub-style **badges** (like “Made with Python 🐍”, “Jupyter Notebook”, or “License: MIT”) at the top for a more professional look?
