```markdown
# Feature_Extraction Activity

This repository contains a Jupyter notebook that performs text normalization and feature extraction on a dataset of reviews.

## File Structure

The project is structured within the `Feature Extraction/` directory. The notebook (`.ipynb`) reads the dataset (`.csv`) from its own directory and saves all outputs to the `lemmatization/` and `stemmer/` sub-folders.

```

├── Feature Extraction/
│   ├── lemmatization/
│   │   ├── .gitkeep
│   │   └── (Generated CSV outputs appear here)
│   ├── stemmer/
│   │   ├── .gitkeep
│   │   └── (Generated CSV outputs appear here)
│   ├── Fin\_lab-PRProject\_dataset.csv  (The input dataset)
│   └── Paredes\_Feature\_Extraction.ipynb (The main notebook)
├── Text Extraction/
├── .gitignore
└── README.md

```

## How to Run

All paths in the notebook are relative, so setup is simple:

1.  Ensure you have all required Python packages installed. The first cell of the notebook handles installing: `pandas`, `nltk`, `autocorrect`, `scikit-learn`, `tqdm`, and `better-profanity`.
2.  Open and run the `Feature Extraction/Paredes_Feature_Extraction.ipynb` notebook.
3.  The notebook will:
    * Read the dataset from `Feature Extraction/Fin_lab-PRProject_dataset.csv`.
    * Perform all text cleaning (punctuation removal, spellcheck, stopword removal, stemming, and lemmatization).
    * Save the final Bag-of-Words (BoW) and TF-IDF feature files into the `Feature Extraction/lemmatization/` and `Feature Extraction/stemmer/` folders.

## Repository Notes

* **`.gitignore`**: The `.gitignore` file is configured to **ignore all `*.csv` files** and the `Text Extraction/` folder. This is intentional. It prevents the large dataset and the generated CSV output files (like `bow_features_lemmatized.csv`) from being committed to the repository.
* **`.gitkeep` Files**: Git does not track empty directories. The `.gitkeep` files are placeholder files inside the `lemmatization/` and `stemmer/` folders. They exist to ensure that Git tracks these directories, so the notebook has a place to save its output.
```
