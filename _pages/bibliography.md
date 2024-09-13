---
permalink: /bibliography/
title: "Annotated Bibliography"
toc_label: " "
toc_icon: "star"
toc_sticky: true
toc: true
---

This is a crowdsourced annotated bibliography of research and resources related to BERT-like models. 

If you'd like to add to the bibliography, you can do so in [this Dropbox document](https://www.dropbox.com/scl/fi/w9w2bs55o0fm1upl2hrhz/BERT-for-Humanists-Annotated-Bibliography.paper?dl=0&rlkey=7qtjce0tilgg42sn7kywwqloh). We will update the bibliography on this web page periodically.

# Technical Readings

- **[BERT: Pre-Training of Deep Bidirectional Transformers for Language Understanding](https://arxiv.org/pdf/1810.04805.pdf)** by Jacob Devlin, Ming-Wei Chan, Kenton Lee, and Kristina Toutonova (2018)

    - *Original paper that introduced BERT, authored by Google AI developers* 

- **[Contextual Embeddings: When are They Worth It?](https://www.aclweb.org/anthology/2020.acl-main.236/)** by Simran Arora, Avner May, Jian Zhang, Christopher Ré (2020) 

-  **[DistilBERT, a distilled version of BERT: smaller, faster, cheaper and lighter](https://arxiv.org/abs/1910.01108)** by Victor Sanh, Lysandre Debut, Julien Chaumond and Thomas Wolf (2020) 

    - *Helpful for teaching students how to use BERT-like models without extensive computational resources*

-  **[A Primer in BERTology: What We Know About How BERT Works](https://www.mitpressjournals.org/doi/full/10.1162/tacl_a_00349#)** by Anna Rogers, Olga Kovaleva and Anna Rumshisky (2020)

    - *A survey of 150+ studies of BERT that explores what BERT* *“knows”* *and how it might be improved. Very technical and invested in model architecture* 

# Tutorials & Primers

- **[The Illustrated BERT, ELMo, and Co. (How NLP Cracked Transfer Learning)](http://jalammar.github.io/illustrated-bert/)** by Jay Alammar (December 2018)

    - *Helpful but very technical for a humanities audience* 

- **[The Illustrated Transformer](https://jalammar.github.io/illustrated-transformer/)** by Jay Alammar (June 2017)
    - *A helpful, but technical, dive into the transformer architecture*

# Risks & Ethical Concerns

- **[On the Dangers of Stochastic Parrots: Can Language Models Be Too Big? 🦜](https://dl.acm.org/doi/10.1145/3442188.3445922)** by Emily M. Bender, Timnit Gebru, Angelina McMillan-Major, and Shmargaret Shmitchell (2021)

    - *This paper discusses the risks and ethical concerns of large language models like BERT, including biased and poorly documented training data as well as financial and environmental costs*

- **[Extracting Data From Large Language Models](https://arxiv.org/pdf/2012.07805.pdf)** by Nicholas Carlini et al. (December 2020)

    - *This paper demonstrates that personal data can be extracted by an adversary from LLMs whose training data contains that information.*

- **[Privacy Considerations in Large Language Models](https://ai.googleblog.com/2020/12/privacy-considerations-in-large.html)** by Nicholas Carlini (December 2020)

    - *A blog post describing the results of Extracting Data From Large Language Models (above) in a more approachable manner.*

# Applied Humanities

- **[Speak, Memory: An Archaeology of Books Known to ChatGPT/GPT-4](https://aclanthology.org/2023.emnlp-main.453/)** by Kent Chang, Mackenzie Cramer, Sandeep Soni and David Bamman (2023) [[Code](https://github.com/bamman-group/gpt4-books)]

    - *This paper presents a task for determining what novels a LLM has memorized and uses it to assess which and what kinds of books have been memorized by GPT models.*

-  **[Do Humanists Need BERT?](https://tedunderwood.com/2019/07/15/do-humanists-need-bert/10)** by Ted Underwood (July 2019)

    - *Overview of BERT and an assessment of its usefulness when applied to sentiment analysis of movie reviews and genre classification of books* 

-  **[Literary Event Detection](https://doi.org/10.18653/v1/P19-1353)** by Matthew Sims, Jong Ho Park, and David Bamman (2019)

    - *This paper releases an annotated dataset of events in literature and evaluates several models on their prediction abilities.*

- **[An Annotated Dataset of Coreference in English Literature](https://arxiv.org/abs/1912.01140)** by David Bamman, Olivia Lewke, and Anya Mansoor (2020)

    - *This paper releases a dataset of coreference annotations in English literature texts, a valuable resource for training and evaluating literary coreference systems.*

- **[Latin BERT: A Contextual Language Model for Classical Philology](https://arxiv.org/abs/2009.10053)** by David Bamman and Patrick Burns (2022)

    - *This paper presents a version of BERT for Latin.*

- **[Adapting vs. Pre-Training Language Models for Historical Languages](https://jdmdh.episciences.org/9690/pdf)** by Enrique Manjavacas and Lauren Fonteyn (2022) [[Models](https://macberth.netlify.app)]

    - *This paper assesses whether it is more effective to adapt pre-existing LLMs for use with Historical English or train new models from scratch and releases the best performing model, MacBERTh.*

- **[Unsupervised Domain Adaptation of Contextualized Embeddings for Labeling](https://www.aclweb.org/anthology/D19-1433/)** by Xiaochuang Han and Jacob Eisenstein (2019) 

    - *Domain adaptive fine-tuning on Early Modern English and Twitter*

- **[What about Grammar? Using BERT Embeddings to Explore Functional-Semantic Shifts of Semi-Lexical and Grammatical Constructions](http://ceur-ws.org/Vol-2723/short15.pdf)** by Lauren Fonteyn (2020) 

    - *This paper uses BERT embeddings to detect shifts in word usage.*

# Critical Humanities

- **[Playing With Unicorns: AI Dungeon and Citizen NLP](http://www.digitalhumanities.org/dhq/vol/14/4/000533/000533.html)** by Minh Hua and Rita Raley (2020)

    - *This paper explores what AI-human collaborations could and should look like by exploring the indie text adventure game AI Dungeon 2.*

# Tools

- **[transformers](https://huggingface.co/transformers/index.html)** from HuggingFace

    - *An API for accessing and training ML models. Includes access to popular models such as [BERT](https://huggingface.co/docs/transformers/model_doc/bert), [T5](https://huggingface.co/docs/transformers/model_doc/t5), [LLaMA](https://huggingface.co/docs/transformers/model_doc/llama), and much more.*

-  **[Easy-Bert](https://github.com/robrua/easy-bert)** by Rob Rua

    - *A simple API for accessing BERT* 

-  **[CLIP-as-Service](https://github.com/jina-ai/clip-as-service)** from Jina AI

    - *A service for easy image and text embedding* 

# Educational Resources

- **[Using BERT for next sentence prediction**](https://github.com/sinykin/QTM-340/blob/master/notebooks/class21-BERT-next-sentence-inclass-ds.ipynb) by Ted Underwood *(adapted and used in Dan Sinykin's Emory course "Practical Approaches to Data Science with Text" in 2020)*

    - *A notebook for teaching students about BERT*