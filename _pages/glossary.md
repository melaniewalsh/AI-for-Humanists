---
permalink: /glossary/
title: "Glossary"
toc_label: " "
toc_icon: "star"
toc_sticky: true
toc: true
---

## Attention
Attention is an important component of GPT, BERT, and other transformer models. At a high level, attention tells the model which pieces of input to "pay attention to" when making predictions. At a low level, attention is just a vector of weights over the inputs. Intuitively, you might expect that the model might "attend" to the words like "best" and "favorite" when doing sentiment analysis (though these attention decisions are often much less intuitive). You can read more about attention in this great [tutorial](https://towardsdatascience.com/deconstructing-bert-part-2-visualizing-the-inner-workings-of-attention-60a16d86b5c1).

## Fine-Tune
LLMs are "pre-trained" on large datasets of texts, such as Wikipedia, books, StackOverflow, and other texts from the internet. However, if you want to improve and tweak language models to perform better on *specific kinds of texts*, you can "fine-tune" the model.

Fine-tuning is the process of training a pre-trained model with additional data so that it can perform better in a certain context. For example, we fine-tune a DistilBERT model with Goodreads reviews in one of our [code tutorials](../tutorials/#classification).

## GPU
A GPU, or “graphics processing unit,” is a specialized electronic circuit for computer hardware.  Because GPUs allows for parallel processing, they are often used for intensive graphics rendering tasks, like gaming, video editing, and, increasingly, machine learning.

Working with the full-scale version of an LLM typically requires access to a GPU. However, most Apple computers do not include GPUs. To use LLMs on a computer without a GPU, researchers will typically either need to use a smaller model, such as DistilBERT, or get access to a GPU through Google Colab (where they are offered for free) or through a computing cluster.


## Label
To train and test a natural language processing model for a specific [task](#task), you often need labeled data. Labels are categories that are assigned to texts or documents, which indicate the "correct" answer(s) for that task.

If you were training a model to recognize the genre of books, you would label the data with the "correct" genres for each book — you might label Jane Austen's *Pride and Prejudice* "romance" and Stephen King's *The Shining* "horror." These labels help teach the model to recognize genre according to your labeling scheme.

Labels are also used to test the performance of the model. For example, in the case of genre classification, you would temporarily remove labels for a certain portion of books that the model had never seen before and then ask the model to label those books based on what it had learned. Then you would assess how many labels it got "right" out of the total possible.

There can be zero, one, or more labels for each document in a dataset.

## Task

If you start reading natural language processing and machine learning research, you'll start to see the word "task" cropping up everywhere. You can think of a task as an objective or assignment that a computer is trying to accomplish.

When you see the phrase "NLP tasks," this refer to tasks that are very common and well-defined across the research community — such as part-of-speech tagging, Named Entity Recognition (NER), sentiment analysis, text generation, or question answering. 

NLP tasks are formulated either explicitly or implicitly as competitions. For example, many conferences have workshops or "shared task" events where different research teams compete for the highest performance on a shared labeled dataset. Such tasks have pros and cons, as they both push the research community towards better results but also constrain progress to the shared datasets and labels, which sometimes contain biases or are missing important examples.


## Transformers
Transformers are a class of neural network models that are very effective for natural language processing. The transformer architecture was first introduced in Vaswani et. al's 2017 paper ["Attention Is All You Need"](https://arxiv.org/abs/1706.03762). Importantly, transformers process all the inputs simultaneously (rather than sequentially, like in LSTMs) and are great at parallelization (breaking up our task into parallel pieces), allowing us to process more data more quickly.

The GPT models build  upon the transformer architecture, as does BERT (Bidirectional Encoder Representations from **Transformers**) and others. Additionally, HuggingFace's Python library is called [Transformers](https://huggingface.co/transformers/) because it enables you to work with dozens of models that use transformer architecture, such as GPT-2, BERT, and RoBERTa.

## Token
Tokenization is the process of splitting text into smaller units. A token is an individual unit of text, often a word. However, when working with LLMs, tokens will often consist of words as well as "word pieces" and "special tokens."

For example, the sentence *"Mrs. Dalloway said she would buy the flowers herself"* might be split into **14** individual tokens:

> [CLS], mrs, ., dal, ##low, ##ay, said, she, would, buy, the, flowers, herself, [SEP]

The tokens include three separate "word pieces" for the word "Dalloway" as well as a special token that indicates the beginning of the document [CLS] and a special token that separates sentences [SEP].
 
 | Special Token | Meaning |
 |---- | ----|
 | [CLS] |	Start token of every document |
| [SEP]	| Separator between each sentence |
 | [PAD]	| Padding at the end of the document as many times as necessary, up to 512 tokens |
| \##	| Start of a "word piece" |

Text can be automatically tokenized with HuggingFace modules such as [`BERTTokenizerFast`](https://huggingface.co/transformers/model_doc/bert.html#berttokenizerfast).

## Type
A type is a unique string representation of a word. For example, the sentence *"GPT is big and is also useful"* contains **six** types.

## Vector
A vector is a list of numbers that represents a word or sentence.

You might think of a vector as a list of numbered coordinates that maps a word/sentence to a specific point in space, where points that are closer together are more similar to each other.

