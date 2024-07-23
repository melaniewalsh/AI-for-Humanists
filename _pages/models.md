---
permalink: /guides/models/
title: "Models"
toc_label: " "
toc_icon: "star"
toc_sticky: true
toc: true
---

The core of modern AI is that you start with a large neural network model that has been trained for a long time on a large data set. Patterns in the real world start to be represented by numeric relationships in the neural network parameters. We can then take these base models and use them for new applications.

The advantage of using pre-trained models is that they are able to deal with complex and ambiguous data because they are able to draw indirectly on millions of other examples. The disadvantage is that the larger the model, the more difficult it can be to access. 

## Large, Cloud-only models

These models are the most capable, but also the least open and accessible. They are large enough that they can only be run in dedicated data centers.
You can access them through a web-based chat interface interactively (ie you type something and then see the result) or process larger numbers of examples through an API (ie you ask it to process a spreadsheet of examples while you do something else).
They often have a low level of free access with monthly fees for more capable/large-scale access.

These models are the best for uses where you are describing in words the output you want (*zero-shot* learning) or providing a small number of examples (*few-shot*).

As a cloud-based system, all your information must be processed on a system owned by a large web company. While there is some question about whether a company like OpenAI will ever do anything with that data, if they do decide to, there is nothing you can really do to stop them. It's up to you to decide if you're ok with that.

### ChatGPT 3.5 / GPT 4

These models are provided by OpenAI, and are operated by Microsoft.

### Claude

Similar to ChatGPT, provided by Anthropic, which has ties to Amazon.

### Gemini

Similar to ChatGPT, provided by Google.

## Medium, Locally runnable models

These models are large and capable, but smaller than the fully cloud-based models like ChatGPT. They can be run locally on recent laptops, such as the Apple Macbook M series using systems like Nomic [GPT4All](https://www.nomic.ai/gpt4all) and [ollama](https://ollama.com/).

While models at this scale are sometimes noticeably less capable than the largest cloud-only models, they can still handle instruction-based interaction (*zero-shot*).

Since these systems run locally, they do not expose your data to any third parties, and they can access files locally on your disk if you choose to.
Locally running mid-scale LLMs are often *quantized* to reduce their file and memory size.

### Llama 3

This is a highly capable model that comes in 8B and 30B parameter models, provided by Meta. You must sign a license with Meta to use them.

### Gemma

This family of models from Google is an open-weight version of their Gemini family.

### Nomic embed

This model, from the developers of GPT4All, is a powerful tool for mapping documents to numeric vector representations.

## Smaller, fine-tunable models

At this scale, up to around 1B parameters, you can load the original model in a Python notebook and create a customized *fine-tuned* version that is specifically suited to your needs.
These models are generally noticeably less capable than the medium-scale models, and may not provide good results for instruction-based interaction.
They may be better suited towards producing embeddings or serving as the base for a classifier.

### BERT / DistillBERT

The one that started it all! From Google. Less capability for non-English text, and somewhat out of date (2018), but still capable. BERT was only trained to fill in missing words, it cannot generate new text.

*Distilled* models are smaller, faster models trained to emulate the output of larger models. DistilBERT is a good base for classifiers.

### RoBERTa / XLM-RoBERTa

A strong alternative to BERT with a more expressive tokenizer. The XLM version supports dozens of languages.

### GPT-2

The ancestor of ChatGPT from OpenAI. It is the best small model for generating text.

### T5 / mT5 / byT5

These models from Google are encoder-decoder models that balance between encoding text as vectors and generating new text. They are a good option for information extraction tools. The mT5 multilingual model has a more flexible tokenizer than base T5. The byT5 model operates only at the level of individual bytes, so it gets great ability to deal with arbitrary text in exchange for less efficient operation.


