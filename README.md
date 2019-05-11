# Predicting Voting Behavior of Supreme Court Nominees

AM231 Final Project

The goal of our project is to train a model to predict how Supreme Court nominees will vote on court cases if confirmed. 

We used three datasets -- information about nominees available at nomination time, their confirmation text hearings, and information about the future cases they hear and vote on.

## Dataset cleaning

TODO

## Feature set generation
This is how we generated our data. We would have included this in the python notebook but due to memory errors we had to run these through scripts on our local machines.

### Merge Justice and Case data

```
python demographic_approach/extract_scdb_data.py
```

### Basic 1-grams (bag of words)

```
python nlp_approach/ngram_feature_extraction.py
```

### n-grams with TF-IDF transform

```
python nlp_approach/ngram_feature_extraction_tfidf.py
```

### Word Embeddings

`nlp_approach/generate_mean_embeddings.ipynb`

## Model Training and Evaluation

This can be found and viewed in  `nominee_predict_models.ipynb`

## Authors

* Michael Fine, Jenny Huang, Chris Rohlicek


## Acknowledgments

* Thanks to Professor Ba for all his guidance!
