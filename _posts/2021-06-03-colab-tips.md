---
title: "Google Colab Notebook Tips"
categories:
  - Quick Tips
tags:
  - Colab Notebooks
author: Maria Antoniak
---

Here are some tips for running BERT in a Google Colab notebook. If you run into strange error messages, if your model takes forever to train, or if your notebook keeps crashing, you should check make sure you're following each of these tips!

* When preparing your data, you must use a tokenizer that matches your pre-trained model (cased vs uncased, BERT vs DistilBERT, sequential vs model, etc.).
* Re-load / re-initialize models before re-fine-tuning with different parameters.
* To save space, delete your models when you’re done with them.
* To avoid running out of memory, use lower batch sizes and use DistilBERT.
* To take advantage of GPU, attach model to device and set the runtime to GPU.
* When using very small datasets, lower the number of warmup steps.
* Use a very small learning rate (~5x10-5).
* Factory reset the Colab runtime if CUDA is running out of memory.
