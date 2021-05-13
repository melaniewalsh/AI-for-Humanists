---
permalink: /tutorials/
title: "Tutorials"
---

Below you can find code tutorials for working with BERT and the HuggingFace Library.

## Word Similarity

"BERT Word Search: Measuring Word Similarity with BERT"  
[[Colab Notebook]](https://colab.research.google.com/drive/18SKxCwdiWqcX4wXjLMpBDSzMuoZ2Sd1I?usp=sharing)

This notebook demonstrates how to use a pre-trained BERT model with the popular HuggingFace `transformers` Python library.

In this example, we look for words that have a similar vector to a query word from a collection of poems. The results are illustrative of what BERT vectors represent, but also of the limitations of the tokenization scheme that it uses.

## Classification

"Training and Fine-Tuning BERT for Classification: Classfying Goodreads Reviews By Book Genre"  
[[Colab Notebook]](https://colab.research.google.com/drive/1tZo9U-CQ0HqalV9UrO-2UPc5zbWOEaKS?usp=sharing)

This notebook demonstrate how users can train and fine-tune a BERT model for classification with the popular HuggingFace `transformers` Python library. We fine-tune a BERT model on Goodreads reviews from the [UCSD Book Graph](https://sites.google.com/eng.ucsd.edu/ucsdbookgraph/reviews?authuser=0) with the goal of predicting the genre of the book being reviewed.