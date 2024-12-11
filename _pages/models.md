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

How should you pick a model? There is an active and competitive market for AI models; many companies are highly motivated to attract attention to their models. Evaluating models is also difficult, because they can be used for so many different uses. You may see quantitative scores on "tasks", and these are informative, but don't assume that metrics like these determine how a model meets your goals. Ultimately, the models within each of the following sections should be roughly comparable.

## Large, Cloud-only models

These models are the most capable, but also the least open and accessible. They are large enough that they can only be run in dedicated data centers.
You can access them through a web-based chat interface interactively (ie you type something and then see the result) or process larger numbers of examples through an API (ie you ask it to process a spreadsheet of examples while you do something else).
They often have a low level of free access with monthly fees for more capable/large-scale access.

These models are the best for uses where you are describing in words the output you want (*zero-shot* learning) or providing a small number of examples (*few-shot*).

As a cloud-based system, all your information must be processed on a system owned by a large web company. While there is some question about whether a company like OpenAI will ever do anything with that data, if they do decide to, there is nothing you can really do to stop them. It's up to you to decide if you're ok with that.

### ChatGPT 3.5 / GPT 4 / GPT o1

These models are provided by OpenAI, and are operated by Microsoft. The o1 models, introduced in September 2024, are meant to provide more in-depth reasoning capabilities.

### Claude

Similar to ChatGPT, Claude is provided by Anthropic, which has ties to Amazon.

### Gemini

Similar to ChatGPT, but provided by Google.

## Medium, Locally runnable models

These models are large and capable, but smaller than the fully cloud-based models like ChatGPT. They can be run locally on recent laptops, such as the Apple Macbook M series using systems like Nomic [GPT4All](https://www.nomic.ai/gpt4all) and [ollama](https://ollama.com/).

While models at this scale are sometimes noticeably less capable than the largest cloud-only models, they can still handle instruction-based interaction (*zero-shot*).

Since these systems run locally, they do not expose your data to any third parties, and they can access files locally on your disk if you choose to.
Locally running mid-scale LLMs are often *quantized* to reduce their file and memory size.

### Llama 3

This is a highly capable model that comes in 8B and 30B parameter models, provided by Meta. <b>Our current recommendation for the best balance between cost and capability is the Llama 3.1 8B model.</b> You must sign a license with Meta to use them. Llama 3.1 is an updated version of Llama 3, intended to have better multilingual support. Llama 3.2 adds additional parameter sizes. The 1B and 3B models are smaller and may be more efficient for simpler tasks. The 11B and 90B sizes add text/image multimodal capabilities. On the higher end, the 3.1 405B model seems to be the most capable open-weight model, but this requires significant hardware and technical experience to run. Llama 3.3 adds a new 70B model, for which there is some early evidence that it has nearly equivalent performance to the 405B model with much lower (but still large) hardware requirements. A Mac Studio with an M2 Ultra and 128G unified memory would be the most accessible way to run the 70B model, around US$4000.

### Gemma

This family of models from Google is an open-weight version of their Gemini family.

### Florence 2

This is a powerful [multimodal image and text model](https://huggingface.co/microsoft/Florence-2-large/blob/main/sample_inference.ipynb). It has been used for OCR page segmentation and has limited ability to perform OCR itself. It can also be used to identify *and describe* objects in photographic and printed images.

### Nomic embed

This model, from the developers of GPT4All, is a powerful tool for mapping documents to numeric vector representations.

## Smaller, fine-tunable models

At this scale, up to around 1B parameters, you can load the original model in a Python notebook and create a customized *fine-tuned* version that is specifically suited to your needs.
These models are generally noticeably less capable than the medium-scale models, and may not provide good results for instruction-based interaction.
They may be better suited towards producing embeddings or serving as the base for a classifier.

### BERT / DistillBERT

The one that started it all! From Google. Less capability for non-English text, and somewhat out of date (2018), but still capable. BERT was only trained to fill in missing words, so it cannot generate new text.

*Distilled* models are smaller, faster models trained to emulate the output of larger models. DistilBERT is a good base for classifiers.

### DeBERTa / RoBERTa / XLM-RoBERTa

A strong alternative to BERT with a more expressive tokenizer. The XLM version supports dozens of languages. Several people report especially good results from [DeBERTa](https://huggingface.co/docs/transformers/en/model_doc/deberta) (thanks to @venkatasg.net for this tip!).

### GLiNER

The [GLiNER](https://huggingface.co/gliner-community) family of models is specially tuned for named entity recognition, and has its own python library. William Mattingly (@wjbmattingly.bsky.social) reports great results as a base model for lots of other text annotation and extraction tasks, such as [this notebook](https://huggingface.co/knowledgator/gliner-multitask-v1.0).

### GPT-2

The ancestor of ChatGPT from OpenAI. It is the best small model for generating text.

### T5 / mT5 / byT5

These models from Google are encoder-decoder models that balance encoding text as vectors and generating new text. They are a good option for information extraction. The mT5 multilingual model has a more flexible tokenizer than base T5. The byT5 model operates only at the level of individual bytes, so it gets great ability to deal with arbitrary text in exchange for less efficient operation. The byT5 model has been especially successful for OCR correction because the task requires analyzing character-level patterns. 


