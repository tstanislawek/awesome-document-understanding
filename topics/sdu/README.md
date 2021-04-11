## Table of contents

1. [Papers](#papers)
1. [Datasets](#datasets)


## Papers 

#### 2021

* [On Generating Extended Summaries of Long Documents](https://arxiv.org/abs/2012.14136v1), \[[code](https://github.com/Georgetown-IR-Lab/ExtendedSumm/)\] 
  <details>
  <summary> Sajad Sotudeh, Arman Cohan, Nazli Goharian <em>SDU</em> 2021 </summary>
    Prior work in document summarization has mainly focused on generating short summaries of a document. While this type of summary helps get a high-level view of a given document, it is desirable in some cases to know more detailed information about its salient points that can't fit in a short summary. This is typically the case for longer documents such as a research paper, legal document, or a book. In this paper, we present a new method for generating extended summaries of long papers. Our method exploits hierarchical structure of the documents and incorporates it into an extractive summarization model through a multi-task learning approach. We then present our results on three long summarization datasets, arXiv-Long, PubMed-Long, and Longsumm. Our method outperforms or matches the performance of strong baselines. Furthermore, we perform a comprehensive analysis over the generated results, shedding insights on future research for long-form summary generation task. Our analysis shows that our multi-tasking approach can adjust extraction probability distribution to the favor of summary-worthy sentences across diverse sections.
  </details>

#### 2020

* [Acronym Identification and Disambiguation Shared Tasksfor Scientific Document Understanding](https://arxiv.org/pdf/2012.11760.pdf), \[[code/data](https://github.com/amirveyseh/AAAI-21-SDU-shared-task-2-AD)\]
  <details>
  <summary> Amir Pouran Ben Veyseh, Franck Dernoncourt, Quan Hung Tran, Thien Huu Nguyen <em>COLING</em> 2020 </summary>
    Acronyms are the short forms of longer phrases and they are frequently used in writing, especially scholarly writing, to save space and facilitate the communication of information. As such, every text understanding tool should be capable of recognizing acronyms in text (i.e., acronym identification) and also finding their correct meaning (i.e., acronym disambiguation). As most of the prior works on these tasks are restricted to the biomedical domain and use unsupervised methods or models trained on limited datasets, they fail to perform well for scientific document understanding. To push forward research in this direction, we have organized two shared task for acronym identification and acronym disambiguation in scientific documents, named AI@SDU and AD@SDU, respectively. The two shared tasks have attracted 52 and 43 participants, respectively. While the submitted systems make substantial improvements compared to the existing baselines, there are still far from the human-level performance. This paper reviews the two shared tasks and the prominent participating systems for each of them.
  </details>

* [AxCell: Automatic Extraction of Resultsfrom Machine Learning Papers](https://arxiv.org/abs/2004.14356), \[[code](https://github.com/paperswithcode/axcell)\]
  <details>
  <summary> Marcin Kardas, Piotr Czapla, Pontus Stenetorp, Sebastian Ruder, Sebastian Riedel, Ross Taylor, Robert Stojnic <em>EMNLP</em> 2020 </summary>
    Tracking progress in machine learning has become increasingly difficult with the recent explosion in the number of papers. In this paper, we present AxCell, an automatic machine learning pipeline for extracting results from papers. AxCell uses several novel components, including a table segmentation subtask, to learn relevant structural knowledge that aids extraction. When compared with existing methods, our approach significantly improves the state of the art for results extraction. We also release a structured, annotated dataset for training models for results extraction, and a dataset for evaluating the performance of models on this task. Lastly, we show the viability of our approach enables it to be used for semi-automated results extraction in production, suggesting our improvements make this task practically viable for the first time. Code is available on GitHub. 
  </details>


* [A New Neural Search and Insights Platform for Navigating and Organizing AI Research](https://www.aclweb.org/anthology/2020.sdp-1.23.pdf), \[[Website](https://search.zeta-alpha.com/)\]
  <details>
  <summary> Marzieh Fadaee, Olga Gureenkova, Fernando Rejon Barrera, Carsten Schnober, Wouter Weerkamp, Jakub Zavrel <em>arxiv</em> 2020 </summary>
    To provide AI researchers with modern tools for dealing with the explosive growth of the research literature in their field, we introduce a new platform, AI Research Navigator, that combines classical keyword search with neural retrieval to discover and organize relevant literature. The system provides search at multiple levels of textual granularity, from sentences to aggregations across documents, both in natural language and through navigation in a domain-specific Knowledge Graph. We give an overview of the overall architecture of the system and of the components for document analysis, question answering, search, analytics, expert search, and recommendations. 
  </details>

### Datasets

* [SciREX: A Challenge Dataset for Document-Level Information Extraction](https://www.aclweb.org/anthology/2020.acl-main.670.pdf) \[[code/data](https://github.com/allenai/SciREX)\]
  <details>
  <summary> Sarthak Jain, Madeleine van Zuylen, Hannaneh Hajishirzi, Iz Beltagy <em>ACL</em> 2020  </summary>
    Extracting information from full documents is an important problem in many domains, but most previous work focus on identifying relationships within a sentence or a paragraph. It is challenging to create a large-scale information extraction (IE) dataset at the document level since it requires an understanding of the whole document to annotate entities and their document-level relationships that usually span beyond sentences or even sections. In this paper, we introduce SciREX, a document level IE dataset that encompasses multiple IE tasks, including salient entity identification and document level N-ary relation identification from scientific articles. We annotate our dataset by integrating automatic and human annotations, leveraging existing scientific knowledge resources. We develop a neural model as a strong baseline that extends previous state-of-the-art IE models to document-level IE. Analyzing the model performance shows a significant gap between human performance and current baselines, inviting the community to use our dataset as a challenge to develop document-level IE models.  
  </details>

* [TableArXiv: Scientific Table Search Using Keyword Queries](https://arxiv.org/abs/1707.03423) \[[Website](http://boston.lti.cs.cmu.edu/eager/table-arxiv/)\]
  <details>
  <summary> Kyle Yingkai Gao, Jamie Callan <em>arxiv</em> 2017  </summary>
    Tables are common and important in scientific documents, yet most text-based document search systems do not capture structures and semantics specific to tables. How to bridge different types of mismatch between keywords queries and scientific tables and what influences ranking quality needs to be carefully investigated. This paper considers the structure of tables and gives different emphasis to table components. On the query side, thanks to external knowledge such as knowledge bases and ontologies, key concepts are extracted and used to build structured queries, and target quantity types are identified and used to expand original queries. A probabilistic framework is proposed to incorporate structural and semantic information from both query and table sides. We also construct and release TableArXiv, a high quality dataset with 105 queries and corresponding relevance judgements for scientific table search. Experiments demonstrate significantly higher accuracy overall and at the top of the rankings than several baseline methods. 
  </details>
