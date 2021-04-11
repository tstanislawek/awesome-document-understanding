## Table of contents

1. [Papers](#papers)
1. [Datasets](#datasets)



## Papers 

* **[Going Full-TILT Boogie on Document Understanding with Text-Image-Layout Transformer](https://arxiv.org/abs/2102.09550)**, 
  <details>
  <summary> Rafał Powalski, Łukasz Borchmann, Dawid Jurkiewicz, Tomasz Dwojak, Michał Pietruszka, Gabriela Pałka <em>arxiv</em> 2021 </summary>
    We address the challenging problem of Natural Language Comprehension beyond plain-text documents by introducing the TILT neural network architecture which simultaneously learns layout information, visual features, and textual semantics. Contrary to previous approaches, we rely on a decoder capable of unifying a variety of problems involving natural language. The layout is represented as an attention bias and complemented with contextualized visual information, while the core of our model is a pretrained encoder-decoder Transformer. Our novel approach achieves state-of-the-art results in extracting information from documents and answering questions which demand layout understanding (DocVQA, CORD, WikiOps, SROIE). At the same time, we simplify the process by employing an end-to-end model.
  </details>

* **[Open Question Answering over Tables and Text](https://arxiv.org/abs/2010.10439)**, \[[code](https://github.com/wenhuchen/OTT-QA) ![](https://img.shields.io/github/stars/wenhuchen/OTT-QA.svg?style=social)\] 
  <details>
  <summary> Wenhu Chen, Ming-Wei Chang, Eva Schlinger, William Wang, William W. Cohen <em>ICLR</em> 2021 </summary>
    In open question answering (QA), the answer to a question is produced by retrieving and then analyzing documents that might contain answers to the question. Most open QA systems have considered only retrieving information from unstructured text. Here we consider for the first time open QA over both tabular and textual data and present a new large-scale dataset Open Table-and-Text Question Answering (OTT-QA) to evaluate performance on this task. Most questions in OTT-QA require multi-hop inference across tabular data and unstructured text, and the evidence required to answer a question can be distributed in different ways over these two types of input, making evidence retrieval challenging -- our baseline model using an iterative retriever and BERT-based reader achieves an exact match score less than 10%. We then propose two novel techniques to address the challenge of retrieving and aggregating evidence for OTT-QA. The first technique is to use "early fusion" to group multiple highly relevant tabular and textual units into a fused block, which provides more context for the retriever to search for. The second technique is to use a cross-block reader to model the cross-dependency between multiple retrieved evidence with global-local sparse attention. Combining these two techniques improves the score significantly, to above 27%. 
  </details>

* [Finding the Evidence: Localization-aware Answer Prediction for Text Visual Question Answering](https://arxiv.org/abs/2010.02582)
  <details>
  <summary> Wei Han, Hantao Huang, Tao Han <em>COLING</em> 2020 </summary>
    Image text carries essential information to understand the scene and perform reasoning. Text-based visual question answering (text VQA) task focuses on visual questions that require reading text in images. Existing text VQA systems generate an answer by selecting from optical character recognition (OCR) texts or a fixed vocabulary. Positional information of text is underused and there is a lack of evidence for the generated answer. As such, this paper proposes a localization-aware answer prediction network (LaAP-Net) to address this challenge. Our LaAP-Net not only generates the answer to the question but also predicts a bounding box as evidence of the generated answer. Moreover, a context-enriched OCR representation (COR) for multimodal fusion is proposed to facilitate the localization task. Our proposed LaAP-Net outperforms existing approaches on three benchmark datasets for the text VQA task by a noticeable margin. 
  </details>

## Datasets 

* **[DocVQA: A Dataset for VQA on Document Images](https://arxiv.org/pdf/2007.00398.pdf)**, [Website](http://docvqa.org/)
  <details>
  <summary> Minesh Mathew, Dimosthenis Karatzas, C.V. Jawahar <em>WACV</em> 2021</summary>
    We present a new dataset for Visual Question Answering (VQA) on document images called DocVQA. The dataset consists of 50,000 questions defined on 12,000+ document images. Detailed analysis of the dataset in comparison with similar datasets for VQA and reading comprehension is presented. We report several baseline results by adopting existing VQA and reading comprehension models. Although the existing models perform reasonably well on certain types of questions, there is large performance gap compared to human performance (94.36% accuracy). The models need to improve specifically on questions where understanding structure of the document is crucial. The dataset, code and leaderboard are available at this http URL
  </details>

* [WebSRC: A Dataset for Web-Based Structural Reading Comprehension](https://arxiv.org/pdf/2101.09465.pdf), [Website](https://speechlab-sjtu.github.io/WebSRC/), [code/data](https://github.com/speechlab-sjtu/WebSRC) ![](https://img.shields.io/github/stars/speechlab-sjtu/WebSRC.svg?style=social)
  <details>
  <summary> Lu Chen et al. <em>arXiv</em> 2021</summary>
    Web search is an essential way for human to obtain information, but it's still a great challenge for machines to understand the contents of web pages. In this paper, we introduce the task of web-based structural reading comprehension. Given a web page and a question about it, the task is to find an answer from the web page. This task requires a system not only to understand the semantics of texts but also the structure of the web page. Moreover, we proposed WebSRC, a novel Web-based Structural Reading Comprehension dataset. WebSRC consists of 0.44M question-answer pairs, which are collected from 6.5K web pages with corresponding HTML source code, screenshots, and metadata. Each question in WebSRC requires a certain structural understanding of a web page to answer, and the answer is either a text span on the web page or yes/no. We evaluate various strong baselines on our dataset to show the difficulty of our task. We also investigate the usefulness of structural information and visual features. Our dataset and task are publicly available at this https URL. 
  </details>
