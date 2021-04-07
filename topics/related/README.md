# Table of contents

1. [General](#general) 
1. [Tabular Data Comprehension (TDC)](#tabular-data-comprehension)
1. [Robotic Process Automation (RPA)](#robotic-process-automation) 


## General


#### 2021

* [Variational Transformer Networks for Layout Generation](https://arxiv.org/pdf/2104.02416.pdf) 
  <details>
  <summary> Diego Martin Arroyo, Janis Postels, Federico Tombari <em>CVPR</em> 2021 </summary>
    Generative models able to synthesize layouts of different kinds (e.g. documents, user interfaces or furniture arrangements) are a useful tool to aid design processes and as a first step in the generation of synthetic data, among other tasks. We exploit the properties of self-attention layers to capture high level relationships between elements in a layout, and use these as the building blocks of the well-known Variational Autoencoder (VAE) formulation. Our proposed Variational Transformer Network (VTN) is capable of learning margins, alignments and other global design rules without explicit supervision. Layouts sampled from our model have a high degree of resemblance to the training data, while demonstrating appealing diversity. In an extensive evaluation on publicly available benchmarks for different layout types VTNs achieve state-of-the-art diversity and perceptual quality. Additionally, we show the capabilities of this method as part of a document layout detection pipeline. 
  </details>

* [GRIT: Generative Role-filler Transformers for Document-level Event Entity Extraction](https://arxiv.org/pdf/2008.09249.pdf)
  <details>
  <summary> Xinya Du, Alexander M. Rush, Claire Cardie <em>EACL</em> 2021 </summary>
    We revisit the classic problem of document-level role-filler entity extraction (REE) for template filling. We argue that sentence-level approaches are ill-suited to the task and introduce a generative transformer-based encoder-decoder framework (GRIT) that is designed to model context at the document level: it can make extraction decisions across sentence boundaries; is implicitly aware of noun phrase coreference structure, and has the capacity to respect cross-role dependencies in the template structure. We evaluate our approach on the MUC-4 dataset, and show that our model performs substantially better than prior work. We also show that our modeling choices contribute to model performance, e.g., by implicitly capturing linguistic knowledge such as recognizing coreferent entity mentions. 
  </details>


#### 2020

* [Multi-modal Information Extraction from Text, Semi-structured, and Tabular Data on the Web](https://www.aclweb.org/anthology/2020.acl-tutorials.6.pdf)
  <details>
  <summary> Xin Luna Dong, Hannaneh Hajishirzi, Colin Lockard, Prashant Shiralkar <em>ACL Tutorials</em> 2020 </summary>
    The World Wide Web contains vast quantities of textual information in several forms: unstructured text, template-based semi-structured webpages (which present data in key-value pairs and lists), and tables. Methods for extracting information from these sources and converting it to a structured form have been a target of research from the natural language processing (NLP), data mining, and database communities. While these researchers have largely separated extraction from web data into different problems based on the modality of the data, they have faced similar problems such as learning with limited labeled data, defining (or avoiding defining) ontologies, making use of prior knowledge, and scaling solutions to deal with the size of the Web. In this tutorial we take a holistic view toward information extraction, exploring the commonalities in the challenges and solutions developed to address these different forms of text. We will explore the approaches targeted at unstructured text that largely rely on learning syntactic or semantic textual patterns, approaches targeted at semi-structured documents that learn to identify structural patterns in the template, and approaches targeting web tables which rely heavily on entity linking and type information. While these different data modalities have largely been considered separately in the past, recent research has started taking a more inclusive approach toward textual extraction, in which the multiple signals offered by textual, layout, and visual clues are combined into a single extraction model made possible by new deep learning approaches. At the same time, trends within purely textual extraction have shifted toward full-document understanding rather than considering sentences as independent units. With this in mind, it is worth considering the information extraction problem as a whole to motivate solutions that harness textual semantics along with visual and semi-structured layout information. We will discuss these approaches and suggest avenues for future work.
  </details>

* [Layout-Aware Text Representations Harm Clustering Documents by Type](https://pdfs.semanticscholar.org/6e3f/adce5f4bea362cf0ca0165c300cec3afe042.pdf)
  <details>
  <summary> Catherine Finegan-Dollak, Ashish Verma <em>Insights</em> 2020 </summary>
    Clustering documents by type—grouping invoices with invoices and articles with articles—is a desirable first step for organizing large collections of document scans. Humans approaching this task use both the semantics of the text and the document layout to assist in grouping like documents. LayoutLM (Xu et al., 2019), a layout-aware transformer built on top of BERT with state-of-the-art performance on document-type classification, could reasonably be expected to outperform regular BERT (Devlin et al., 2018) for document-type clustering. However, we find experimentally that BERT significantly outperforms LayoutLM on this task (p <0.001). We analyze clusters to show where layout awareness is an asset and where it is a liability.
  </details>

* [Self-Supervised Representation Learning on Document Images](https://arxiv.org/pdf/2004.10605.pdf)
  <details>
  <summary> Adrian Cosma, Mihai Ghidoveanu, Michael Panaitescu-Liess, Marius Popescu <em>DAS</em> 2020 </summary>
    This work analyses the impact of self-supervised pre-training on document images in the context of document image classification. While previous approaches explore the effect of self-supervision on natural images, we show that patch-based pre-training performs poorly on document images because of their different structural properties and poor intra-sample semantic information. We propose two context-aware alternatives to improve performance on the Tobacco-3482 image classification task. We also propose a novel method for self-supervision, which makes use of the inherent multi-modality of documents (image and text), which performs better than other popular self-supervised methods, including supervised ImageNet pre-training, on document image classification scenarios with a limited amount of data.    
  </details>

#### Older

* **[Fonduer: Knowledge Base Construction from Richly Formatted Data](https://arxiv.org/pdf/1703.05028.pdf)**, \[[code](https://github.com/HazyResearch/fonduer)\] 
  <details>
  <summary> Sen Wu, Luke Hsiao, Xiao Cheng, Braden Hancock, Theodoros Rekatsinas, Philip Levis, Christopher Ré <em>International Conference on Management of Data</em> 2018 </summary>
    We focus on knowledge base construction (KBC) from richly formatted data. In contrast to KBC from text or tabular data, KBC from richly formatted data aims to extract relations conveyed jointly via textual, structural, tabular, and visual expressions. We introduce Fonduer, a machine-learning-based KBC system for richly formatted data. Fonduer presents a new data model that accounts for three challenging characteristics of richly formatted data: (1) prevalent document-level relations, (2) multimodality, and (3) data variety. Fonduer uses a new deep-learning model to automatically capture the representation (i.e., features) needed to learn how to extract relations from richly formatted data. Finally, Fonduer provides a new programming model that enables users to convert domain expertise, based on multiple modalities of information, to meaningful signals of supervision for training a KBC system. Fonduer-based KBC systems are in production for a range of use cases, including at a major online retailer. We compare Fonduer against state-of-the-art KBC approaches in four different domains. We show that Fonduer achieves an average improvement of 41 F1 points on the quality of the output knowledge base---and in some cases produces up to 1.87x the number of correct entries---compared to expert-curated public knowledge bases. We also conduct a user study to assess the usability of Fonduer's new programming model. We show that after using Fonduer for only 30 minutes, non-domain experts are able to design KBC systems that achieve on average 23 F1 points higher quality than traditional machine-learning-based KBC approaches. 
  </details>

* [Evaluation of Deep Convolutional Nets for Document Image Classification and Retrieval](https://arxiv.org/pdf/1502.07058.pdf)
  <details>
  <summary> Adam W. Harley, Alex Ufkes, Konstantinos G. Derpanis <em>ICDAR</em> 2015 </summary>
    This paper presents a new state-of-the-art for document image classification and retrieval, using features learned by deep convolutional neural networks (CNNs). In object and scene analysis, deep neural nets are capable of learning a hierarchical chain of abstraction from pixel inputs to concise and descriptive representations. The current work explores this capacity in the realm of document analysis, and confirms that this representation strategy is superior to a variety of popular hand-crafted alternatives. Experiments also show that (i) features extracted from CNNs are robust to compression, (ii) CNNs trained on non-document images transfer well to document analysis tasks, and (iii) enforcing region-specific feature-learning is unnecessary given sufficient training data. This work also makes available a new labelled subset of the IIT-CDIP collection, containing 400,000 document images across 16 categories, useful for training new CNNs for document analysis. 
  </details>


## Tabular Data Comprehension

[Back to top](#table-of-contents)

### Papers

#### 2021

* [Open Domain Question Answering over Tables via Dense Retrieval](https://arxiv.org/pdf/2103.12011.pdf), \[[code](https://github.com/google-research/tapas)\]
  <details>
  <summary> Jonathan Herzig, Thomas Müller, Syrine Krichene, Julian Martin Eisenschlos  <em>NAACL</em> 2021 </summary>
    Recent advances in open-domain QA have led to strong models based on dense retrieval, but only focused on retrieving textual passages. In this work, we tackle open-domain QA over tables for the first time, and show that retrieval can be improved by a retriever designed to handle tabular context. We present an effective pre-training procedure for our retriever and improve retrieval quality with mined hard negatives. As relevant datasets are missing, we extract a subset of NATURAL QUESTIONS (Kwiatkowski et al., 2019) into a Table QA dataset. We find that our retriever improves retrieval results from 72.0 to 81.1 recall@10 and end-to-end QA results from 33.8 to 37.7 exact match, over a BERT based retriever
  </details>
  
 #### 2020

* **[TURL: Table Understanding through Representation Learning](https://arxiv.org/pdf/2006.14806.pdf)**, \[[code](https://github.com/sunlab-osu/TURL)\]
  <details>
  <summary> Xiang Deng, Huan Sun, Alyssa Lees, You Wu, Cong Yu <em>VLDB</em> 2021 </summary>
    Relational tables on the Web store a vast amount of knowledge. Owing to the wealth of such tables, there has been tremendous progress on a variety of tasks in the area of table understanding. However, existing work generally relies on heavily-engineered task-specific features and model architectures. In this paper, we present TURL, a novel framework that introduces the pre-training/fine-tuning paradigm to relational Web tables. During pre-training, our framework learns deep contextualized representations on relational tables in an unsupervised manner. Its universal model design with pre-trained representations can be applied to a wide range of tasks with minimal task-specific fine-tuning. Specifically, we propose a structure-aware Transformer encoder to model the row-column structure of relational tables, and present a new Masked Entity Recovery (MER) objective for pre-training to capture the semantics and knowledge in large-scale unlabeled data. We systematically evaluate TURL with a benchmark consisting of 6 different tasks for table understanding (e.g., relation extraction, cell filling). We show that TURL generalizes well to all tasks and substantially outperforms existing methods in almost all instances. 
  </details>

* **[TAPAS: Weakly Supervised Table Parsing via Pre-training](https://arxiv.org/pdf/2004.02349.pdf)**, \[[code](https://github.com/google-research/tapas)\]
  <details>
  <summary> Jonathan Herzig, Paweł Krzysztof Nowak, Thomas Müller, Francesco Piccinno, Julian Martin Eisenschlos <em>ACL</em> 2020 </summary>
    Answering natural language questions over tables is usually seen as a semantic parsing task. To alleviate the collection cost of full logical forms, one popular approach focuses on weak supervision consisting of denotations instead of logical forms. However, training semantic parsers from weak supervision poses difficulties, and in addition, the generated logical forms are only used as an intermediate step prior to retrieving the denotation. In this paper, we present TAPAS, an approach to question answering over tables without generating logical forms. TAPAS trains from weak supervision, and predicts the denotation by selecting table cells and optionally applying a corresponding aggregation operator to such selection. TAPAS extends BERT's architecture to encode tables as input, initializes from an effective joint pre-training of text segments and tables crawled from Wikipedia, and is trained end-to-end. We experiment with three different semantic parsing datasets, and find that TAPAS outperforms or rivals semantic parsing models by improving state-of-the-art accuracy on SQA from 55.1 to 67.2 and performing on par with the state-of-the-art on WIKISQL and WIKITQ, but with a simpler model architecture. We additionally find that transfer learning, which is trivial in our setting, from WIKISQL to WIKITQ, yields 48.7 accuracy, 4.2 points above the state-of-the-art. 
  </details>

* **[TaBERT: Pretraining for Joint Understanding of Textual and Tabular Data](https://arxiv.org/pdf/2005.08314.pdf)**, \[[code](https://github.com/facebookresearch/TaBERT)\] 
  <details>
  <summary> Pengcheng Yin, Graham Neubig, Wen-tau Yih, Sebastian Riedel <em>ACL</em> 2020 </summary>
    Recent years have witnessed the burgeoning of pretrained language models (LMs) for text-based natural language (NL) understanding tasks. Such models are typically trained on free-form NL text, hence may not be suitable for tasks like semantic parsing over structured data, which require reasoning over both free-form NL questions and structured tabular data (e.g., database tables). In this paper we present TaBERT, a pretrained LM that jointly learns representations for NL sentences and (semi-)structured tables. TaBERT is trained on a large corpus of 26 million tables and their English contexts. In experiments, neural semantic parsers using TaBERT as feature representation layers achieve new best results on the challenging weakly-supervised semantic parsing benchmark WikiTableQuestions, while performing competitively on the text-to-SQL dataset Spider.
  </details>

* [Web Table Extraction, Retrieval and Augmentation: A Survey](https://arxiv.org/pdf/2002.00207.pdf)
  <details>
  <summary> Shuo Zhang, Krisztian Balog <em>ACM Transactions on Intelligent Systems and Technology</em> 2020 </summary>
    Tables are a powerful and popular tool for organizing and manipulating data. A vast number of tables can be found on the Web, which represents a valuable knowledge resource. The objective of this survey is to synthesize and present two decades of research on web tables. In particular, we organize existing literature into six main categories of information access tasks: table extraction, table interpretation, table search, question answering, knowledge base augmentation, and table augmentation. For each of these tasks, we identify and describe seminal approaches, present relevant resources, and point out interdependencies among the different tasks. 
  </details>

* [Structure-aware Pre-training for Table Understanding with Tree-based Transformers](https://arxiv.org/pdf/2010.12537.pdf)
  <details>
  <summary> Zhiruo Wang et al. <em>arXiv</em> 2020 </summary>
    Tables are widely used with various structures to organize and present data. Recent attempts on table understanding mainly focus on relational tables, yet overlook to other common table structures. In this paper, we propose TUTA, a unified pre-training architecture for understanding generally structured tables. Since understanding a table needs to leverage both spatial, hierarchical, and semantic information, we adapt the self-attention strategy with several key structure-aware mechanisms. First, we propose a novel tree-based structure called a bi-dimensional coordinate tree, to describe both the spatial and hierarchical information in tables. Upon this, we extend the pre-training architecture with two core mechanisms, namely the tree-based attention and tree-based position embedding. Moreover, to capture table information in a progressive manner, we devise three pre-training objectives to enable representations at the token, cell, and table levels. TUTA pre-trains on a wide range of unlabeled tables and fine-tunes on a critical task in the field of table structure understanding, i.e. cell type classification. Experiment results show that TUTA is highly effective, achieving state-of-the-art on four well-annotated cell type classification datasets.
  </details>

#### 2019

* [Auto-completion for Data Cells in Relational Tables](https://arxiv.org/pdf/1909.03443.pdf)
  <details>
  <summary> Shuo Zhang, Krisztian Balog <em>CIKM</em> 2019 </summary>
    We address the task of auto-completing data cells in relational tables. Such tables describe entities (in rows) with their attributes (in columns). We present the CellAutoComplete framework to tackle several novel aspects of this problem, including: (i) enabling a cell to have multiple, possibly conflicting values, (ii) supplementing the predicted values with supporting evidence, (iii) combining evidence from multiple sources, and (iv) handling the case where a cell should be left empty. Our framework makes use of a large table corpus and a knowledge base as data sources, and consists of preprocessing, candidate value finding, and value ranking components. Using a purpose-built test collection, we show that our approach is 40% more effective than the best baseline.
  </details>


* [Learning Semantic Annotations for Tabular Data](https://arxiv.org/pdf/1906.00781.pdf), \[[code](https://github.com/alan-turing-institute/SemAIDA)\]
  <details>
  <summary> Jiaoyan Chen et al. <em>IJCAI</em> 2019 </summary>
    The usefulness of tabular data such as web tables critically depends on understanding their semantics. This study focuses on column type prediction for tables without any meta data. Unlike traditional lexical matching-based methods, we propose a deep prediction model that can fully exploit a table's contextual semantics, including table locality features learned by a Hybrid Neural Network (HNN), and inter-column semantics features learned by a knowledge base (KB) lookup and query answering this http URL exhibits good performance not only on individual table sets, but also when transferring from one table set to another. 
  </details>

* [ColNet: Embedding the Semantics of Web Tables for Column Type Prediction](https://arxiv.org/pdf/1811.01304.pdf), \[[code](https://github.com/alan-turing-institute/SemAIDA)\]
  <details>
  <summary> Jiaoyan Chen et al. <em>AAAI</em> 2019 </summary>
    Automatically annotating column types with knowledge base (KB) concepts is a critical task to gain a basic understanding of web tables. Current methods rely on either table metadata like column name or entity correspondences of cells in the KB, and may fail to deal with growing web tables with incomplete meta information. In this paper we propose a neural network based column type annotation framework named ColNet which is able to integrate KB reasoning and lookup with machine learning and can automatically train Convolutional Neural Networks for prediction. The prediction model not only considers the contextual semantics within a cell using word representation, but also embeds the semantics of a column by learning locality features from multiple cells. The method is evaluated with DBPedia and two different web table datasets, T2Dv2 from the general Web and Limaye from Wikipedia pages, and achieves higher performance than the state-of-the-art approaches.  
  </details>

#### Older

* [EntiTables: Smart Assistance for Entity-Focused Tables](https://arxiv.org/pdf/1708.08721.pdf), \[[code](https://github.com/iai-group/sigir2017-table)\]
  <details>
  <summary> Shuo Zhang, Krisztian Balog <em>SIGIR</em> 2017 </summary>
    Tables are among the most powerful and practical tools for organizing and working with data. Our motivation is to equip spreadsheet programs with smart assistance capabilities. We concentrate on one particular family of tables, namely, tables with an entity focus. We introduce and focus on two specifc tasks: populating rows with additional instances (entities) and populating columns with new headings. We develop generative probabilistic models for both tasks. For estimating the components of these models, we consider a knowledge base as well as a large table corpus. Our experimental evaluation simulates the various stages of the user entering content into an actual table. A detailed analysis of the results shows that the models' components are complimentary and that our methods outperform existing approaches from the literature.
  </details>

### Datasets 

#### Information retrieval from tables


* [Open Question Answering over Tables and Text](https://arxiv.org/pdf/2010.10439.pdf), \[[code](https://github.com/wenhuchen/OTT-QA)\] 
  <details>
  <summary> Wenhu Chen et al. <em>ICLR</em> 2021 </summary>
     In open question answering (QA), the answer to a question is produced by retrieving and then analyzing documents that might contain answers to the question. Most open QA systems have considered only retrieving information from unstructured text. Here we consider for the first time open QA over both tabular and textual data and present a new large-scale dataset Open Table-Text Question Answering (OTT-QA) to evaluate performance on this task. Most questions in OTT-QA require multi-hop inference across tabular data and unstructured text, and the evidence required to answer a question can be distributed in different ways over these two types of input, making evidence retrieval challenging---our baseline model using an iterative retriever and BERT-based reader achieves an exact match score less than 10%. We then propose two novel techniques to address the challenge of retrieving and aggregating evidence for OTT-QA. The first technique is to use "early fusion" to group multiple highly relevant tabular and textual units into a fused block, which provides more context for the retriever to search for. The second technique is to use a cross-block reader to model the cross-dependency between multiple retrieved evidences with global-local sparse attention. Combining these two techniques improves the score significantly, to above 27%. 

* [FeTaQA: Free-form Table Question Answering](https://arxiv.org/pdf/2104.00369.pdf), \[[code](https://github.com/Yale-LILY/FeTaQA)\] 
  <details>
  <summary> Linyong Nan et al. <em>arXiv</em> 2021 </summary>
     Existing table question answering datasets contain abundant factual questions that primarily evaluate the query and schema comprehension capability of a system, but they fail to include questions that require complex reasoning and integration of information due to the constraint of the associated short-form answers. To address these issues and to demonstrate the full challenge of table question answering, we introduce FeTaQA, a new dataset with 10K Wikipedia-based {table, question, free-form answer, supporting table cells} pairs. FeTaQA yields a more challenging table question answering setting because it requires generating free-form text answers after retrieval, inference, and integration of multiple discontinuous facts from a structured knowledge source. Unlike datasets of generative QA over text in which answers are prevalent with copies of short text spans from the source, answers in our dataset are human-generated explanations involving entities and their high-level relations. We provide two benchmark methods for the proposed task: a pipeline method based on semantic-parsing-based QA systems and an end-to-end method based on large pretrained text generation models, and show that FeTaQA poses a challenge for both methods. 
  
  
* [TabFact: A Large-scale Dataset for Table-based Fact Verification](https://openreview.net/pdf?id=rkeJRhNYDH), \[[code](https://github.com/wenhuchen/Table-Fact-Checking)\] 
  <details>
  <summary> Wenhu Chen, Hongmin Wang, Jianshu Chen, Yunkai Zhang, Hong Wang,Shiyang Li, Xiyou Zhou, William Yang Wang <em>ICLR</em> 2020 </summary>
    The problem of verifying whether a textual hypothesis holds based on the given evidence, also known as fact verification, plays an important role in the study of natural language understanding and semantic representation. However, existing studies are mainly restricted to dealing with unstructured evidence (e.g., natural language sentences and documents, news, etc), while verification under structured evidence, such as tables, graphs, and databases, remains unexplored. This paper specifically aims to study the fact verification given semi-structured data as evidence. To this end, we construct a large-scale dataset called TabFact with 16k Wikipedia tables as the evidence for 118k human-annotated natural language statements, which are labeled as either ENTAILED or REFUTED. TabFact is challenging since it involves both soft linguistic reasoning and hard symbolic reasoning. To address these reasoning challenges, we design two different models: Table-BERT and Latent Program Algorithm (LPA). Table-BERT leverages the state-of-the-art pre-trained language model to encode the linearized tables and statements into continuous vectors for verification. LPA parses statements into LISP-like programs and executes them against the tables to obtain the returned binary value for verification. Both methods achieve similar accuracy but still lag far behind human performance. We also perform a comprehensive analysis to demonstrate great future opportunities.
  </details>

* [Search-based Neural Structured Learning for Sequential Question Answering](https://www.aclweb.org/anthology/P17-1167.pdf), \[[Github](https://github.com/microsoft/DynSP)\], \[[page](https://www.microsoft.com/en-us/download/details.aspx?id=54253)\]
  <details>
  <summary> Mohit Iyyer, Wen-tau Yih, Ming-Wei Chang <em>ACL</em> 2017</summary>
    Recent work in semantic parsing for question answering has focused on long and complicated questions, many of which would seem unnatural if asked in a normal conversation between two humans. In an effort to explore a conversational QA setting, we present a more realistic task: answering sequences of simple but inter-related questions. We collect a dataset of 6,066 question sequences that inquire about semi-structured tables from Wikipedia, with 17,553 question-answer pairs in total. To solve this sequential question answering task, we propose a novel dynamic neural semantic parsing framework trained using a weakly supervised reward-guided search. Our model effectively leverages the sequential context to outperform state-of-the-art QA systems that are designed to answer highly complex questions.
  </details>

* **[Compositional Semantic Parsing on Semi-Structured Tables](https://www.aclweb.org/anthology/P15-1142.pdf)**, \[[page](https://ppasupat.github.io/WikiTableQuestions/)\]
  <details>
  <summary> Panupong Pasupat, Percy Liang <em>ACL</em> 2015 </summary>
    Two important aspects of semantic parsing for question answering are the breadth of the knowledge source and the depth of logical compositionality. While existing work trades off one aspect for another, this paper simultaneously makes progress on both fronts through a new task: answering complex questions on semi-structured tables using question-answer pairs as supervision. The central challenge arises from two compounding factors: the broader domain results in an open-ended set of relations, and the deeper compositionality results in a combinatorial explosion in the space of logical forms. We propose a logical-form driven parsing algorithm guided by strong typing constraints and show that it obtains significant improvements over natural baselines. For evaluation, we created a new dataset of 22,033 complex questions on Wikipedia tables, which is made publicly available. 
  </details>

#### Collections of not annotated tables

* **[A Large Public Corpus of Web Tables containing Time and Context Metadata](http://gdac.uqam.ca/WWW2016-Proceedings/companion/p75.pdf)**, \[[page](http://webdatacommons.org/webtables/)]
  <details>
  <summary> Oliver Lehmberg et al. <em>WWW</em> 2016</summary>
    The Web contains vast amounts of HTML tables. Most of these tables are used for layout purposes, but a small subset of the tables is relational, meaning that they contain structured data describing a set of entities [2]. As these relational Web tables cover a very wide range of different topics, there is a growing body of research investigating the utility of Web table data for completing cross-domain knowledge bases [6], for extending arbitrary tables with additional attributes [7, 4], as well as for translating data values [5]. The existing research shows the potentials of Web tables. However, comparing the performance of the different systems is difficult as up till now each system is evaluated using a different corpus of Web tables and as most of the corpora are owned by large search engine companies and are thus not accessible to the public. In this poster, we present a large public corpus of Web tables which contains over 233 million tables and has been extracted from the July 2015 version of the CommonCrawl. By publishing the corpus as well as all tools that we used to extract it from the crawled data, we intend to provide a common ground for evaluating Web table systems. The main difference of the corpus compared to an earlier corpus that we extracted from the 2012 version of the CommonCrawl as well as the corpus extracted by Eberius et al. [3] from the 2014 version of the CommonCrawl is that the current corpus contains a richer set of metadata for each table. This metadata includes table-specific information such as table orientation, table caption, header row, and key column, but also context information such as the text before and after the table, the title of the HTML page, as well as timestamp information that was found before and after the table. The context information can be useful for recovering the semantics of a table [7]. The timestamp information is crucial for fusing time-depended data, such as alternative population numbers for a city [8].
  </details>

* [Top-k entity augmentation using consistent set covering](https://wwwdb.inf.tu-dresden.de/misc/publications/rea.pdf), \[[page](https://wwwdb.inf.tu-dresden.de/misc/dwtc/)\]
  <details>
  <summary> Julian Eberius et al. <em>SSDBM</em> 2015 </summary>
    Entity augmentation is a query type in which, given a set of entities and a large corpus of possible data sources, the values of a missing attribute are to be retrieved. State of the art methods return a single result that, to cover all queried entities, is fused from a potentially large set of data sources. We argue that queries on large corpora of heterogeneous sources using information retrieval and automatic schema matching methods can not easily return a single result that the user can trust, especially if the result is composed from a large number of sources that user has to verify manually. We therefore propose to process these queries in a Top-k fashion, in which the system produces multiple minimal consistent solutions from which the user can choose to resolve the uncertainty of the data sources and methods used. In this paper, we introduce and formalize the problem of consistent, multi-solution set covering, and present algorithms based on a greedy and a genetic optimization approach. We then apply these algorithms to Web table-based entity augmentation. The publication further includes a Web table corpus with 100M tables, and a Web table retrieval and matching system in which these algorithms are implemented. Our experiments show that the consistency and minimality of the augmentation results can be improved using our set covering approach, without loss of precision or coverage and while producing multiple alternative query results.
  </details>

* [Methods for exploring and mining tables on Wikipedia](https://www.researchgate.net/publication/261849268_Methods_for_exploring_and_mining_tables_on_Wikipedia), \[[page](https://downey-n1.cs.northwestern.edu/public/)\]
  <details>
  <summary> Chandra Bhagavatula, Thanapon Noraset, Doug Downey <em>ACM SIGKDD</em> 2013 </summary>
    Knowledge bases extracted automatically from the Web present new opportunities for data mining and exploration. Given a large, heterogeneous set of extracted relations, new tools are needed for searching the knowledge and uncovering relationships of interest. We present WikiTables, a Web application that enables users to interactively explore tabular knowledge extracted from Wikipedia. In experiments, we show that WikiTables substantially outperforms baselines on the novel task of automatically joining together disparate tables to uncover "interesting" relationships between table columns. We find that a "Semantic Relatedness" measure that leverages the Wikipedia link structure accounts for a majority of this improvement. Further, on the task of keyword search for tables, we show that WikiTables performs comparably to Google Fusion Tables despite using an order of magnitude fewer tables. Our work also includes the release of a number of public resources, including over 15 million tuples of extracted tabular data, manually annotated evaluation sets, and public APIs.
  </details>


## Robotic Process Automation

[Back to top](#table-of-contents)

* [Automated Discovery of Data Transformations for Robotic Process Automation](https://arxiv.org/pdf/2001.01007.pdf)
  <details>
  <summary> Volodymyr Leno, Marlon Dumas, Marcello La Rosa, Fabrizio Maria Maggi, Artem Polyvyanyy <em> AAAI-20 workshop on IPA </em> 2020 </summary>
    Robotic Process Automation (RPA) is a technology for automating repetitive routines consisting of sequences of user interactions with one or more applications. In order to fully exploit the opportunities opened by RPA, companies need to discover which specific routines may be automated, and how. In this setting, this paper addresses the problem of analyzing User Interaction (UI) logs in order to discover routines where a user transfers data from one spreadsheet or (Web) form to another. The paper maps this problem to that of discovering data transformations by example - a problem for which several techniques are available. The paper shows that a naive application of a state-of-the-art technique for data transformation discovery is computationally inefficient. Accordingly, the paper proposes two optimizations that take advantage of the information in the UI log and the fact that data transfers across applications typically involve copying alphabetic and numeric tokens separately. The proposed approach and its optimizations are evaluated using UI logs that replicate a real-life repetitive data transfer routine. 
  </details>

* [A Unified Conversational Assistant Framework for Business Process Automation](https://arxiv.org/pdf/2001.03543.pdf)
  <details>
  <summary> Yara Rizk, Abhishek Bhandwalder, S. Boag, T. Chakraborti, Vatche Isahagian, Y. Khazaeni, Falk Pollock, M. Unuvar <em>-</em> 2020 </summary>
    Business process automation is a booming multi-billion-dollar industry that promises to remove menial tasks from workers' plates -- through the introduction of autonomous agents -- and free up their time and brain power for more creative and engaging tasks. However, an essential component to the successful deployment of such autonomous agents is the ability of business users to monitor their performance and customize their execution. A simple and user-friendly interface with a low learning curve is necessary to increase the adoption of such agents in banking, insurance, retail and other domains. As a result, proactive chatbots will play a crucial role in the business automation space. Not only can they respond to users' queries and perform actions on their behalf but also initiate communication with the users to inform them of the system's behavior. This will provide business users a natural language interface to interact with, monitor and control autonomous agents. In this work, we present a multi-agent orchestration framework to develop such proactive chatbots by discussing the types of skills that can be composed into agents and how to orchestrate these agents. Two use cases on a travel preapproval business process and a loan application business process are adopted to qualitatively analyze the proposed framework based on four criteria: performance, coding overhead, scalability, and agent overlap.
  </details>

* [Robotic Process Automation - A Systematic Literature Review and Assessment Framework](https://arxiv.org/pdf/2012.11951.pdf)
  <details>
  <summary> Judith Wewerka, Manfred Reichert <em>-</em> 2020 </summary>
    Robotic Process Automation (RPA) is the automation of rule-based routine processes to increase efficiency and to reduce costs. Due to the utmost importance of process automation in industry, RPA attracts increasing attention in the scientific field as well. This paper presents the state-of-the-art in the RPA field by means of a Systematic Literature Review (SLR). In this SLR, 63 publications are identified, categorised, and analysed along well-defined research questions. From the SLR findings, moreover, a framework for systematically analysing, assessing, and comparing existing as well as upcoming RPA works is derived. The discovered thematic clusters advise further investigations in order to develop an even more detailed structural research approach for RPA. 
  </details>

* [Robotic Process Automation](https://link.springer.com/article/10.1007/s12599-018-0542-4)
  <details>
  <summary> Wil M. P. van der Aalst, Martin Bichler, Armin Heinzl <em>Business & Information Systems Engineering</em> 2018 </summary>
    A foundational question for many BISE (Business and Information Systems Engineering) authors and readers is “What should be automated and what should be done by humans?” This question is not new. However, developments in data science, machine learning, and artificial intelligence force us to revisit this question continuously. Robotic Process Automation (RPA) is one of these developments. RPA is an umbrella term for tools that operate on the user interface of other computer systems in the way a human would do. RPA aims to replace people by automation done in an “outside-in’’ manner. This differs from the classical “inside-out” approach to improve information systems. Unlike traditional workflow technology, the information system remains unchanged. Gartner defines Robotic Process Automation (RPA) as follows: “RPA tools perform [if, then, else] statements on structured data, typically using a combination of user interface interactions, or by connecting to APIs to drive client servers, mainframes or HTML code. An RPA tool operates by mapping a process in the RPA tool language for the software robot to follow, with runtime allocated to execute the script by a control dashboard.” (Tornbohm 2017). Hence, RPA tools aim to reduce the burden of repetitive, simple tasks on employees (Aguirre and Rodriguez 2017). Commercial vendors of RPA tools have witnessed a surge in demand. Moreover, many new vendors entered the market in the last 2 years. This is no surprise as most organizations are still looking for ways to cut costs and quickly link legacy applications together. RPA is currently seen as a way to quickly achieve a high Return on Investment (RoI). There are dedicated RPA vendors like AutomationEdge, Automation Anywhere, Blue Prism, Kryon Systems, Softomotive, and UiPath that only offer RPA software (Le Clair 2017; Tornbohm 2017). There are also many other vendors that have embedded RPA functionality in their software or that are offering several tools (not just RPA). For example, Pegasystems and Cognizant provide RPA next to traditional BPM, CRM, and BI functionality. The goal of this editorial is to reflect on these developments and to discuss RPA research challenges for the BISE community.
  </details>

* [Robotic Process Automation of Unstructured Data with Machine Learning](https://pdfs.semanticscholar.org/bb4c/ec661f4d5d0b83c49353b896f16ed7bdd55e.pdf)
  <details>
  <summary> Anna Wróblewska, Tomasz Stanisławek, Bartłomiej Prus-Zajączkowski, Łukasz Garncarek <em>FedCSCIS</em> 2018 </summary>
    In this paper we present our work in progress on building an artificial intelligence system dedicated to tasks regarding the processing of formal documents used in various kinds of business procedures. The main challenge is to build machine learning (ML) models to improve the quality and efficiency of business processes involving image processing, optical character recognition (OCR), text mining and information extraction. In the paper we introduce the research and application field, some common techniques used in this area and our preliminary results and conclusions.
  </details>

