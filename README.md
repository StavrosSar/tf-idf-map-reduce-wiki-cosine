# tf-idf-map-reduce-wiki-cosine

Finding TF-IDF between 3 wikipedia articles and then comparing their cosine similarity to find which articles  are similar. Also, I've used MapReduce to speed the process due to the larg data of earch article.

# Wikipedia Article Keyword Extraction and Similarity

This repository contains a Python script designed to extract keywords from Wikipedia articles and calculate the similarity between them. The script utilizes multi-threading to efficiently fetch and process articles, and employs TF-IDF vectorization to identify significant keywords and measure article similarity.

## Table of Contents

- Overview
- Requirements
- Data
- Usage
- Script Details
  - Fetching Wikipedia Articles
  - Preprocessing
  - Map Phase
  - Reduce Phase
  - Calculating Similarity
- License

## Overview

This script performs the following tasks:

1. **Fetches Wikipedia Articles**: Retrieves content from Wikipedia articles in parallel.
2. **Preprocesses Data**: Cleans and tokenizes the text data, removing stopwords and unnecessary symbols.
3. **Extracts Keywords**: Uses TF-IDF vectorization to identify and extract the top keywords from each article.
4. **Calculates Similarity**: Computes the cosine similarity between the articles to determine their relatedness.

## Requirements

To run this script, you'll need Python 3.x and the following libraries:

- `concurrent.futures`
- `re`
- `requests`
- `nltk`
- `scikit-learn`

You can install the required libraries using `pip`:

```bash
pip install nltk scikit-learn
