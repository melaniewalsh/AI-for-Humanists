---
permalink: /guides/usecases/
title: "Use Cases"
toc_label: " "
toc_icon: "star"
toc_sticky: true
toc: true
---

# Examples of uses for AI models

## Managing sources

### OCR and image to text

- **[Leveraging LLMs for Post-OCR Correction of Historical Newspapers](https://aclanthology.org/2024.lt4hala-1.14.pdf)** by Alan Thomas, Robert Gaizauskas, and Haiping Lu (2024)

    - *This paper compares the ability of a prompted Llama 2 model and a fine-tuned BART model to correct character-level errors in the OCR of 19th C British newspaper articles.*

- **[Uncovering the Handwritten Text in the Margins: End-to-end Handwritten Text Detection and Recognition](https://arxiv.org/pdf/2303.05929)** by Liang Cheng, Jonas Frankemölle, Adam Axelsson, and Ekta Vats (2024)

    - *This paper presents a pipeline for computationally extracting marginalia and an evaluation of the pipeline on the early book collection in the Uppsala University Library.*

- **[Enhancing HTR of Historical Texts through Scholarly Editions: A Case Study from an Ancient Collation of the Hebrew Bible](https://ceur-ws.org/Vol-3558/paper6310.pdf)** by Luigi Bambaci and Daniel Stökl Ben Ezra (2023)

    - *A case study that makes use of OCR, image alignment, and more to produce an electronic scholarly edition of Kennicott's Hebrew bible.*

### Parsing difficult text

### Translation

### Speech to text

- **[Careless Whisper: Speech-to-Text Hallucination Harms](https://dl.acm.org/doi/pdf/10.1145/3630106.3658996)** by Allison Koenecke, Anna Seo Gyeong Choi, Katelyn X. Mei, Hilke Schellmann, and Mona Sloane (2024)

    - *This paper explores hallucinations and other errors in one of the largest and most popular speech-to-text systems, OpenAI's Whisper, and, despite the model's overall high performance, finds systematic errors that are likely to disproportionately effect speakers with aphasia.*

## Adding annotations

### Classification / coding

- **[Modeling Legal Reasoning: LM Annotation at the Edge of Human Agreement](https://aclanthology.org/2023.emnlp-main.575.pdf)** by Rosamond Thalken, Edward H. Stiglitz, David Mimno, and Matthew Wilkens (2023)

    - *This paper discusses how to use LLMs effectively for annotating modes of legal reasoning in a corpus of United States Supreme Court Decisions.*

- **[Says Who? Effective Zero-Shot Annotation for Focalization](https://arxiv.org/pdf/2409.11390)** by Rebecca M. M. Hicke, Yuri Bizzoni, Pascale Feldkamp, and Ross Deans Kristensen-McLachlan (2024)

    - *This paper describes how to effective annotate literary texts for focalization in low-resource (compute and annotations) settings. It provides a case study with Stephen King novels to show the use of large scale focalization annotations.*

- **[Sonnet or Not, Bot? Poetry Evaluation for Large Language Models](https://arxiv.org/pdf/2406.18906)** by Melanie Walsh, Anna Preus, and Maria Antoniak (2024)

    - *This paper introduces an evaluation dataset for how well LLMs can recognize different stylistic and structural characteristics of poetry and reports on the performance of several popular LLMs.*

- **[Where Do People Tell Stories Online? Story Detection Across Online Communities](https://maria-antoniak.github.io/resources/2024_ac_where_stories.pdf)** by Maria Antoniak, Joel Mire, Maarten Sap, Elliott Ash, and Andrew Piper (2024)

    - *This paper examines whether narrative can be identified in social media posts using a range of detection methods that include fine-tuned and zero and few-shot prompted LLMs.*

- **[Automate or Assist? The Role of Computational Models in Identifying Gendered Discourse in US Capital Trial Transcripts](https://arxiv.org/pdf/2407.12500)** by Andrea W Wen-Yi, Kathryn Adamson, Nathalie Greenfield, Rachel Goldberg, Sandra Babcock, David Mimno, and Allison Koenecke (2024)

    - *This paper examines the capability of a small, in-domain model (LEGAL-BERT) to annotate for gender bias in US capital trials.*

- **[Distinguishing Fictional Voices: a Study of Authorship Verification Models for Quotation Attribution](https://arxiv.org/pdf/2401.16968)** by Gaspard Michel, Elena V. Epure, Romain Hennequin, and Christophe Cerisara

    - *This paper looks at attributing dialogue to novel characters using character representations build by encoding their quotes.*

- **[Stage Direction Classification in French Theater: Transfer Learning Experiments](https://hal.science/hal-04520702/)** by Alexia Schneider and Pablo Ruiz Fabo

    - *This paper develops and evaluates methodologies for automatically identifying and classifying stage directions in French drama.*

### Named entity recognition

- **[Recognising Occupational Titles in German Parliamentary Debates](https://aclanthology.org/2024.latechclfl-1.21.pdf)** by Johanna Binnewitt (2024)

    - *This paper compares fine-tuned BERT to dictionary-based methods for extracting occupational titles from German parliamentary debates, finding that the BERT outperforms the dictionary method on recall.*

- **[People and Places of the Past - Named Entity Recognition in Swedish Labour Movement Documents from Historical Sources](https://aclanthology.org/2024.latechclfl-1.17.pdf)** by Crina Tudor and Eva Pettersson (2024)

    - *This work compares the ability of several models to perform NER on documents in historical Swedish, a low-resource langauge.*

### Stylometry

- **[T5 meets Tybalt: Authorship Attribution in Early Modern English Drama Using Large Language Models](https://ceur-ws.org/Vol-3558/paper2757.pdf)** by Rebecca M. M. Hicke and David Mimno (2023)

    - *This paper explores the ability of medium-sized large language models to perform authorship attribution with very short segments of text in the difficult setting of Early Modern English drama.*

## Getting an overview

### Corpus visualization

### Word representations and similarity

- **[Diachronic Word Embeddings Reveal Statistical Laws of Semantic Change](https://aclanthology.org/P16-1141.pdf)** by William L. Hamilton, Jure Leskovec, and Dan Jurafsky (2016)

    - *This work develops a method for using word embeddings to track semantic drift over time and uses it to develop two quantitative laws of semantic change.*

- **[Semantics derived automatically from language corpora contain human-like biases](https://www.science.org/doi/10.1126/science.aal4230)** by Aylin Caliskan, Joanna J. Bryson, and Arvind Narayanan (2017)

    - *This paper uses static word embeddings trained on web corpora to show that machine learning methods can result in human-like biases.*

- **[Discovering Differences in the Representation of People using Contextualized Semantic Axes](https://aclanthology.org/2022.emnlp-main.228.pdf)** by Li Lucy, Divya Tadimeti, and David Bamman (2022)

    - *This work uses contextual embeddings from BERT to construct semantic axes along which words can be placed and validates that this method can separate instances of the same word type and track how word associations have drifted in several corpora over time.*