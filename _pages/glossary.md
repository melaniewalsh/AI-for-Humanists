---
permalink: /glossary/
title: "Glossary"
toc_label: " "
toc_icon: "star"
toc_sticky: true
toc: true
---

## Attention


## Context


## Downstream (Task)


## Fine-tune


## GPU
A GPU, or “graphics processing unit,” is a specialized electronic circuit for computer hardware.  Because GPUs allows for parallel processing, they are often used for intensive graphics rendering tasks, like gaming, video editing, and, increasingly, machine learning.

Working with the full-scale version of BERT typically requires access to a GPU. However, most Apple computers do not include GPUs. To use BERT on a computer without a GPU, researchers will typically either need to use a smaller BERT model, such as DistilBERT, or get access to a GPU through Google Colab (where they are offered for free) or through a computing cluster.

## Head


## Hidden States


## Hyperparameters


## Label

Labels are categories developed by researchers for particular tasks and datasets. The researchers then annotate the datasets with the labels. Sometimes there is one label for each document in the dataset, but sometimes there can be zero, one, or more labels for each document in the dataset. These different labeling structures are important to remember when training and evaluating your models.

## Layers


## Task

In the fields of natural language processing and machine learning, research is often divided into sets of well-defined tasks. Tasks might include part-of-speech tagging, sentence parsing, or sentiment analysis. Each task is usually associated with one or more labeled datasets that are used by everyone in the research community. These tasks are formulated either explicitly or implicitly as competitions; for example, many conferences have workshops or "shared task" events where different research teams compete for the highest performance on a shared labeled dataset. A popular exmple of this model is the dat ascience competition website Kaggle. These tasks have pros and cons, as they both push the reserach community towards better results but also constrain progress to the shared datasets and labels (which sometimes contain biases or are missing important examples).

## Transformers


## Token
A token is an individual instance of a word. For example, the sentence *"BERT is big and is also useful"* contains **seven** tokens.

## Type
A type is a unique string representation of a word. For example, the sentence *"BERT is big and is also useful"* contains **six** types.

## Vector
A vector is just a list of numbers. This is how we translate data for computers to understand. For example, we might translate a sentence in a vector (list) of word counts as input to a classifier.
