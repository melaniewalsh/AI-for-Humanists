---
permalink: /tutorials/
title: "Code Tutorials"
toc_label: " "
toc_icon: "star"
toc_sticky: true
toc: true
layout: single
---

Below you can find code tutorials for working with large language models.

## Word and Document Embeddings

### * Measuring Document Similarity with LLMs  (Sentence-T5 Model)
[[Colab Notebook]](https://colab.research.google.com/drive/1-aOfk6mVFUA3PH_s6P-lCaM9xKLJ0dLz?usp=sharing)

This notebook demonstrates how you can use LLMs to explore which texts in a dataset are similar to each other. Examples include narrative vs. non-narrative texts, historial poetry, and ChatGPT-generated poetry.

### * Measuring Word Similarity with BERT  
(English Language Public Domain Poems)"  
[[Full Colab Notebook]](https://colab.research.google.com/drive/1r_eoi8CMea_a3YjWC1M4EmTqKMGVMbzQ?usp=sharing) [[Demo with Results Only](https://colab.research.google.com/drive/1DjtrD_MMW_Ezto0Q4zUvjT0IxKZg-rIt?usp=sharing)]

This notebook demonstrates how to use a pre-trained BERT model with the popular HuggingFace `transformers` Python library.

In this example, we look for words that have a similar vector to a query word from a collection of poems. The results are illustrative of what BERT vectors represent, but also of the limitations of the tokenization scheme that it uses.

### * Measuring Word Similarity with BERT (Spanish Language Sonnets)   
[Full Colab Notebook Coming Soon!] [[Demo with Results Only](https://colab.research.google.com/drive/192YOj8N9isRsEvOQwaI2WZ3pRSlUgAYb?usp=sharing)]

## Text Classification

### * Text Classification and Zero-Shot Prompting with LLMs (FLAN-T5)  
[[Colab Notebook]](https://colab.research.google.com/drive/1QIG-3bIo1BHVWWlS22-1XItlZRrGSMNe?usp=sharing)

This notebook demonstrate how users can set up a **zero-shot classification** task with an LLM and how they can evaluate different **prompting** strategies. With the current batch of powerful language models, this zero-short paradigm should be the first thing to try when evaluating a new task.

In this tutorial, we specifically explore how you can prompt a model to predict the genre of a book based on its Goodreads review and to predict whether a given passage is narrative or non-narrative text. But you should be able to use and modify this workflow for your own text classification needs.

### * Training and Fine-Tuning BERT for Classification: Classfying Goodreads Reviews By Book Genre  
[[Colab Notebook]](https://colab.research.google.com/drive/19jDqa5D5XfxPU6NQef17BC07xQdRnaKU?usp=sharing)

This notebook demonstrate how users can train and fine-tune a BERT model for classification with the popular HuggingFace `transformers` Python library. We fine-tune a BERT model on Goodreads reviews from the [UCSD Book Graph](https://sites.google.com/eng.ucsd.edu/ucsdbookgraph/reviews?authuser=0) with the goal of predicting the genre of the book being reviewed.


