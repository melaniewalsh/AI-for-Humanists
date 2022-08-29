---
permalink: /tutorials/
title: "Code Tutorials"
---

Below you can find code tutorials for working with BERT and the HuggingFace Library.

## Word Similarity

"Measuring Word Similarity with BERT  
(English Language Public Domain Poems)"  
[[Full Colab Notebook]](https://colab.research.google.com/drive/1r_eoi8CMea_a3YjWC1M4EmTqKMGVMbzQ?usp=sharing) [[Demo with Results Only](https://colab.research.google.com/drive/1DjtrD_MMW_Ezto0Q4zUvjT0IxKZg-rIt?usp=sharing)]

This notebook demonstrates how to use a pre-trained BERT model with the popular HuggingFace `transformers` Python library.

In this example, we look for words that have a similar vector to a query word from a collection of poems. The results are illustrative of what BERT vectors represent, but also of the limitations of the tokenization scheme that it uses.

"Measuring Word Similarity with BERT  
(Spanish Language Sonnets)"   
[Full Colab Notebook Coming Soon!] [[Demo with Results Only](https://colab.research.google.com/drive/192YOj8N9isRsEvOQwaI2WZ3pRSlUgAYb?usp=sharing)]

## Classification

"Training and Fine-Tuning BERT for Classification: Classfying Goodreads Reviews By Book Genre"  
[[Colab Notebook]](https://colab.research.google.com/drive/19jDqa5D5XfxPU6NQef17BC07xQdRnaKU?usp=sharing)

This notebook demonstrate how users can train and fine-tune a BERT model for classification with the popular HuggingFace `transformers` Python library. We fine-tune a BERT model on Goodreads reviews from the [UCSD Book Graph](https://sites.google.com/eng.ucsd.edu/ucsdbookgraph/reviews?authuser=0) with the goal of predicting the genre of the book being reviewed.
