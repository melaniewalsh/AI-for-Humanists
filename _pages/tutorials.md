---
permalink: /tutorials/
title: "Code Tutorials"
toc_label: " "
toc_icon: "star"
toc_sticky: true
toc: true
layout: single
toc_min_header: 1
toc_max_header: 3
---

Below you can find code tutorials for working with large language models.

Most of the code tutorials are written in Python and use the popular `transformers` library from [Hugging Face](https://huggingface.co/docs/transformers/en/index). Additionally, most of the tutorials are written in Colab notebooks because Colab offers free (and optionally paid) access to [GPUs](../glossary/#gpu) — a special kind of hardware that is often required when using LLMs.

## Local LLMs

### Working with Local LLMs (On Your Own Computer!) — Ollama and Llama 3

📔 [[Colab Notebook]](https://colab.research.google.com/drive/1V09aQmReB1iMDuTLIWArWODGbHlOK-kQ?usp=sharing)

This [code notebook](https://colab.research.google.com/drive/1V09aQmReB1iMDuTLIWArWODGbHlOK-kQ?usp=sharing) (which should ideally be downloaded on your own computer) demonstrates how you can use local LLMs with Ollama to create structured data from unstructured text, as well as to chat and generate poems or create document embeddings.

While people tend to think of AI as something controlled by a handful of very large companies, there are many free and open-source LLMs that you can download and run on your own computer.

**Quick Colab Demo**: This notebook should ideally be run from your own computer, but we've prepared [a version](https://colab.research.google.com/drive/1DV8bfxL2WILUXw6Ux4NAsltDojirWrWC?usp=sharing) that will work in Colab for quick demo purposes.

## Word and Document Embeddings

---

### Measuring Document Similarity with LLMs

📔 [[Colab Notebook]](https://colab.research.google.com/drive/1-aOfk6mVFUA3PH_s6P-lCaM9xKLJ0dLz?usp=sharing)

This [code notebook](https://colab.research.google.com/drive/1-aOfk6mVFUA3PH_s6P-lCaM9xKLJ0dLz?usp=sharing) demonstrates how you can use LLMs to explore which texts, or documents, are similar to each other in a given dataset. We explore narrative vs. non-narrative texts, historical poetry, and ChatGPT-generated poetry.

---

### Measuring Word Similarity with BERT

📔 [[Full Colab Notebook]](https://colab.research.google.com/drive/1r_eoi8CMea_a3YjWC1M4EmTqKMGVMbzQ?usp=sharing) [[Demo with Results Only](https://colab.research.google.com/drive/1DjtrD_MMW_Ezto0Q4zUvjT0IxKZg-rIt?usp=sharing)]

This [code notebook](https://colab.research.google.com/drive/1r_eoi8CMea_a3YjWC1M4EmTqKMGVMbzQ?usp=sharing) demonstrates how to use a pre-trained BERT model to measure word similarity.

In this example, we look for words that have a similar vector to a query word from a collection of poems. The results are illustrative of what BERT vectors represent, but also of the limitations of the tokenization scheme that it uses.

---

### Measuring Word Similarity with BERT (Spanish)

📔 [Full Colab Notebook Coming Soon!] [[Demo with Results Only](https://colab.research.google.com/drive/192YOj8N9isRsEvOQwaI2WZ3pRSlUgAYb?usp=sharing)]

---

## Text Classification

---

### Zero-Shot Prompting with LLMs

📔 [[Colab Notebook]](https://colab.research.google.com/drive/1QIG-3bIo1BHVWWlS22-1XItlZRrGSMNe?usp=sharing)

This [code notebook](https://colab.research.google.com/drive/1QIG-3bIo1BHVWWlS22-1XItlZRrGSMNe?usp=sharing) demonstrate how users can set up a **zero-shot classification** task with an LLM and how they can evaluate different **prompting** strategies. With the current batch of powerful language models, this zero-short paradigm should be the first thing to try when evaluating a new task.

In this tutorial, we specifically explore how you can prompt a model to predict the genre of a book based on its Goodreads review and to predict whether a given passage is narrative or non-narrative text. But you should be able to use and modify this workflow for your own text classification needs.

---

### Training and Fine-Tuning BERT for Classification: Classifying Goodreads Reviews By Book Genre

📔 [[Colab Notebook]](https://colab.research.google.com/drive/19jDqa5D5XfxPU6NQef17BC07xQdRnaKU?usp=sharing)

This [code notebook](https://colab.research.google.com/drive/19jDqa5D5XfxPU6NQef17BC07xQdRnaKU?usp=sharing) demonstrates how users can train and fine-tune a BERT model for text classification. We fine-tune a BERT model on Goodreads reviews from the [UCSD Book Graph](https://sites.google.com/eng.ucsd.edu/ucsdbookgraph/reviews?authuser=0) with the goal of predicting the genre of the book being reviewed.

---
