# Awesome Document Understanding [![Awesome](https://awesome.re/badge-flat.svg)](https://awesome.re)

A curated list of resources for Document Understanding (DU) topic related to Intelligent Document Processing (IDP), which is relative to Robotic Process Automation (RPA) from unstructured data, especially form Visually Rich Documents (VRDs). 

**Note 1: bolded positions are more important then others.**

**Note 2: due to the novelty of the field, this list is under construction - contributions are welcome (thank you in advance!).** Please remember to use following convention: 
* [Title of a publication / dataset / resource title](https://arxiv.org), \[[code/data/Website](https://github.com/example/test) ![](https://img.shields.io/github/stars/example/test.svg?style=social)\] 
  <details>
  <summary> List of authors <em>Conference/Journal name</em> Year </summary>
    Dataset size: Train(no of examples), Dev(no of examples), Test(no of examples) [Optional for dataset papers/resources]; Abstract/short description ...
  </details>
<br/><br/> 


<p align="center">
  <a href="https://openreview.net/forum?id=rNs2FvJGDK">
    <img src="images/du_example.png">
  </a>
</p>
<br/><br/>

# Table of contents

1. [Introduction](#introduction) 
1. [Research topics](#research-topics)
    1. [Key Information Extraction (KIE)](topics/kie/README.md)
    1. [Document Layout Analysis (DLA)](topics/dla/README.md)
    1. [Document Question Answering (DQA)](topics/dqa/README.md)  
    1. [Scientific Document Understanding (SDU)](topics/sdu/README.md)
    1. [Optical Character Recognition (OCR)](topics/ocr/README.md)       
    1. [Related](topics/related/README.md)  
        1. [General](topics/related/README.md#general) 
        1. [Tabular Data Comprehension (TDC)](topics/related/README.md#tabular-data-comprehension)
        1. [Robotic Process Automation (RPA)](topics/related/README.md#robotic-process-automation) 
1. [Others](#others)
    1. [Resources](#resources)
        1. [Datasets for Pre-training Language Models](#datasets-for-pre-training-language-models)
        1. [PDF processing tools](#pdf-processing-tools)
    1. [Conferences / workshops](#conferences-workshops) 
    1. [Blogs](#blogs)
    1. [Solutions](#solutions)
1. [Examples](#examples)
    1. [Visually Rich Documents (VRDs)](#visually-rich-documents) 
    1. [Key Information Extraction (KIE)](#key-information-extraction)
    1. [Document Layout Analysis (DLA)](#document-layout-analysis) 
    1. [Document Question Answering (DQA)](#document-question-answering)
1. [Inspirations](#inspirations)


# Introduction 

Documents are a core part of many businesses in many fields such as law, finance, and technology among others. Automatic understanding of documents such as invoices, contracts, and resumes is lucrative, opening up many new avenues of business. The fields of natural language processing and computer vision have seen tremendous progress through the development of deep learning such that these methods have started to become infused in contemporary document understanding systems. [source](https://arxiv.org/abs/2011.13534)


### Papers

#### 2023

* [DocILE Benchmark for Document Information Localization and Extraction](https://arxiv.org/abs/2302.05658), \[[Website](https://docile.rossum.ai)\] \[[benchmark](https://rrc.cvc.uab.es/?ch=26)\] \[[code](https://github.com/rossumai/docile) ![](https://img.shields.io/github/stars/rossumai/docile.svg?style=social)\] 
  <details>
  <summary> Štěpán Šimsa, Milan Šulc, Michal Uřičář, Yash Patel, Ahmed Hamdi, Matěj Kocián, Matyáš Skalický, Jiří Matas, Antoine Doucet, Mickaël Coustaty, Dimosthenis Karatzas <em>arxiv pre-print</em> 2023 </summary>
    This paper introduces the DocILE benchmark with the largest dataset of business documents for the tasks of Key Information Localization and Extraction and Line Item Recognition. It contains 6.7k annotated business documents, 100k synthetically generated documents, and nearly~1M unlabeled documents for unsupervised pre-training. The dataset has been built with knowledge of domain- and task-specific aspects, resulting in the following key features: (i) annotations in 55 classes, which surpasses the granularity of previously published key information extraction datasets by a large margin; (ii) Line Item Recognition represents a highly practical information extraction task, where key information has to be assigned to items in a table; (iii) documents come from numerous layouts and the test set includes zero- and few-shot cases as well as layouts commonly seen in the training set. The benchmark comes with several baselines, including RoBERTa, LayoutLMv3 and DETR-based Table Transformer. These baseline models were applied to both tasks of the DocILE benchmark, with results shared in this paper, offering a quick starting point for future work. The dataset and baselines are available at this https URL.
  </details>

#### 2022

* [Business Document Information Extraction: Towards Practical Benchmarks](https://arxiv.org/abs/2206.11229) 
  <details>
  <summary> Matyáš Skalický, Štěpán Šimsa, Michal Uřičář, Milan Šulc <em>CLEF</em> 2022 </summary>
    Information extraction from semi-structured documents is crucial for frictionless business-to-business (B2B) communication. While machine learning problems related to Document Information Extraction (IE) have been studied for decades, many common problem definitions and benchmarks do not reflect domain-specific aspects and practical needs for automating B2B document communication. We review the landscape of Document IE problems, datasets and benchmarks. We highlight the practical aspects missing in the common definitions and define the Key Information Localization and Extraction (KILE) and Line Item Recognition (LIR) problems. There is a lack of relevant datasets and benchmarks for Document IE on semi-structured business documents as their content is typically legally protected or sensitive. We discuss potential sources of available documents including synthetic data.  
  </details>


#### 2021 

* [Document AI: Benchmarks, Models and Applications](https://arxiv.org/abs/2111.08609) 
  <details>
  <summary> Lei Cui, Yiheng Xu, Tengchao Lv, Furu Wei <em>arxiv</em> 2021 </summary>
    Document AI, or Document Intelligence, is a relatively new research topic that refers to the techniques for automatically reading, understanding, and analyzing business documents. It is an important research direction for natural language processing and computer vision. In recent years, the popularity of deep learning technology has greatly advanced the development of Document AI, such as document layout analysis, visual information extraction, document visual question answering, document image classification, etc. This paper briefly reviews some of the representative models, tasks, and benchmark datasets. Furthermore, we also introduce early-stage heuristic rule-based document analysis, statistical machine learning algorithms, and deep learning approaches especially pre-training methods. Finally, we look into future directions for Document AI research. 
  </details>

* **[Efficient Automated Processing of the Unstructured Documents using Artificial Intelligence: A Systematic Literature Review and Future Directions](https://ieeexplore.ieee.org/abstract/document/9402739)**
  <details>
  <summary> Dipali Baviskar, Swati Ahirrao, Vidyasagar Potdar, Ketan Kotecha <em>IEEE Access</em> 2021 </summary>
    The unstructured data impacts 95% of the organizations and costs them millions of dollars annually. If managed well, it can significantly improve business productivity. The traditional information extraction techniques are limited in their functionality, but AI-based techniques can provide a better solution. A thorough investigation of AI-based techniques for automatic information extraction from unstructured documents is missing in the literature. The purpose of this Systematic Literature Review (SLR) is to recognize, and analyze research on the techniques used for automatic information extraction from unstructured documents and to provide directions for future research. The SLR guidelines proposed by Kitchenham and Charters were adhered to conduct a literature search on various databases between 2010 and 2020. We found that: 1. The existing information extraction techniques are template-based or rule-based, 2. The existing methods lack the capability to tackle complex document layouts in real-time situations such as invoices and purchase orders, 3.The datasets available publicly are task-specific and of low quality. Hence, there is a need to develop a new dataset that reflects real-world problems. Our SLR discovered that AI-based approaches have a strong potential to extract useful information from unstructured documents automatically. However, they face certain challenges in processing multiple layouts of the unstructured documents. Our SLR brings out conceptualization of a framework for construction of high-quality unstructured documents dataset with strong data validation techniques for automated information extraction. Our SLR also reveals a need for a close association between the businesses and researchers to handle various challenges of the unstructured data analysis.
  </details>

#### 2020 

* **[A Survey of Deep Learning Approaches for OCR and Document Understanding](https://arxiv.org/abs/2011.13534)**
  <details>
  <summary> Nishant Subramani, Alexandre Matton, Malcolm Greaves, Adrian Lam <em>ML-RSA Workshop at NeurIPS</em> 2020 </summary>
    Documents are a core part of many businesses in many fields such as law, finance, and technology among others. Automatic understanding of documents such as invoices, contracts, and resumes is lucrative, opening up many new avenues of business. The fields of natural language processing and computer vision have seen tremendous progress through the development of deep learning such that these methods have started to become infused in contemporary document understanding systems. In this survey paper, we review different techniques for document understanding for documents written in English and consolidate methodologies present in literature to act as a jumping-off point for researchers exploring this area. 
  </details>

* **[Conversations with Documents. An Exploration of Document-Centered Assistance](https://arxiv.org/pdf/2002.00747.pdf)**
  <details>
  <summary> Maartje ter Hoeve, Robert Sim, Elnaz Nouri, Adam Fourney, Maarten de Rijke, Ryen W. White <em>CHIIR</em> 2020 </summary>
    The role of conversational assistants has become more prevalent in helping people increase their productivity. Document-centered assistance, for example to help an individual quickly review a document, has seen less significant progress, even though it has the potential to tremendously increase a user's productivity. This type of document-centered assistance is the focus of this paper. Our contributions are three-fold: (1) We first present a survey to understand the space of document-centered assistance and the capabilities people expect in this scenario. (2) We investigate the types of queries that users will pose while seeking assistance with documents, and show that document-centered questions form the majority of these queries. (3) We present a set of initial machine learned models that show that (a) we can accurately detect document-centered questions, and (b) we can build reasonably accurate models for answering such questions. These positive results are encouraging, and suggest that even greater results may be attained with continued study of this interesting and novel problem space. Our findings have implications for the design of intelligent systems to support task completion via natural interactions with documents. 
  </details>

#### 2018

* [Future paradigms of automated processing of business documents](https://www.sciencedirect.com/science/article/pii/S0268401217309994)
  <details>
  <summary> Matteo Cristania, Andrea Bertolasob, Simone Scannapiecoc, Claudio Tomazzolia <em>International Journal of Information Management</em> 2018 </summary>
    In this paper we summarize the results obtained so far in the communities interested in the development of automated processing techniques as applied to business documents, and devise a few evolutions that are demanded by the current stage of either those techniques by themselves or by collateral sector advancements. It emerges a clear picture of a field that has put an enormous effort in solving problems that changed a lot during the last 30 years, and is now rapidly evolving to incorporate document processing into workflow management systems on one side and to include features derived by the introduction of cloud computing technologies on the other side. We propose an architectural schema for business document processing that comes from the two above evolution lines.
  </details>

#### Older 

* [Machine Learning for Intelligent Processing of Printed Documents](https://www.semanticscholar.org/paper/Machine-Learning-for-Intelligent-Processing-of-Esposito-Malerba/1f23b61f04d450ffc49ec6371bb5b30d198cdc5b)
  <details>
  <summary> F. Esposito, D. Malerba, F. Lisi <em>-</em> 2004 </summary>
    A paper document processing system is an information system component which transforms information on printed or handwritten documents into a computer-revisable form. In intelligent systems for paper document processing this information capture process is based on knowledge of the specific layout and logical structures of the documents. This article proposes the application of machine learning techniques to acquire the specific knowledge required by an intelligent document processing system, named WISDOM++, that manages printed documents, such as letters and journals. Knowledge is represented by means of decision trees and first-order rules automatically generated from a set of training documents. In particular, an incremental decision tree learning system is applied for the acquisition of decision trees used for the classification of segmented blocks, while a first-order learning system is applied for the induction of rules used for the layout-based classification and understanding of documents. Issues concerning the incremental induction of decision trees and the handling of both numeric and symbolic data in first-order rule learning are discussed, and the validity of the proposed solutions is empirically evaluated by processing a set of real printed documents.
  </details>


* [Document Understanding: Research Directions](https://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.40.9880&rep=rep1&type=pdf)
  <details>
  <summary> S. Srihari, S. Lam, V. Govindaraju, R. Srihari, J. Hull <em>-</em> 1994 </summary>
    A document image is a visual representation of a printed page such as a journal article page, a facsimile cover page, a technical document, an office letter, etc. Document understanding as a research endeavor consists of studying all processes involved in taking a document through various representations: from a scanned physical document to high-level semantic descriptions of the document. Some of the types of representation that are useful are: editable descriptions, descriptions that enable exact reproductions and high-level semantic descriptions about document content. This report is a definition of five research subdomains within document understanding as pertaining to predominantly printed documents. The topics described are: modular architectures for document understanding; decomposition and structural analysis of documents; model-based OCR; table, diagram and image understanding; and performance evaluation under distortion and noise. 
  </details>



# Research topics

* [Key Information Extraction (KIE)](topics/kie/README.md)
* [Document Layout Analysis (DLA)](topics/dla/README.md)
* [Document Question Answering (DQA)](topics/dqa/README.md)
* [Scientific Document Understanding (SDU)](topics/sdu/README.md)  
* [Optical Character Recogtion (OCR)](topics/ocr/README.md)
* [Related](topics/related/README.md)
  * [General](topics/related/README.md#general) 
  * [Tabular Data Comprehension (TDC)](topics/related/README.md#tabular-data-comprehension)
  * [Robotic Process Automation (RPA)](topics/related/README.md#robotic-process-automation) 

# Others

## Resources

[Back to top](#table-of-contents)

#### Datasets for Pre-training Language Models

1. [The RVL-CDIP Dataset](https://adamharley.com/rvl-cdip/) - dataset consists of 400,000 grayscale images in 16 classes, with 25,000 images per class
1. [The Industry Documents Library](https://www.industrydocuments.ucsf.edu/) - a portal to millions of documents created by industries that influence public health, hosted by the UCSF Library
1. [Color Document Dataset](https://ivi.fnwi.uva.nl/isis/UvA-CDD/) - from the Intelligent Sensory Information Systems, University of Amsterdam
1. [The IIT CDIP Collection](https://data.nist.gov/od/id/mds2-2531) - dataset consists of documents from the states' lawsuit against the tobacco industry in the 1990s, consists of around 7 million documents


#### PDF processing tools

1. [borb](https://github.com/jorisschellekens/borb) ![](https://img.shields.io/github/stars/jorisschellekens/borb.svg?style=social) - is a pure python library to read, write and manipulate PDF documents. It represents a PDF document as a JSON-like datastructure of nested lists, dictionaries and primitives (numbers, string, booleans, etc).
1. [pawls](https://github.com/allenai/pawls) ![](https://img.shields.io/github/stars/allenai/pawls.svg?style=social) - PDF Annotations with Labels and Structure is software that makes it easy to collect a series of annotations associated with a PDF document
1. [pdfplumber](https://github.com/jsvine/pdfplumber) ![](https://img.shields.io/github/stars/jsvine/pdfplumber.svg?style=social) - Plumb a PDF for detailed information about each text character, rectangle, and line. Plus: Table extraction and visual debugging
1. [Pdfminer.six](https://github.com/pdfminer/pdfminer.six) ![](https://img.shields.io/github/stars/pdfminer/pdfminer.six.svg?style=social) - Pdfminer.six is a community maintained fork of the original PDFMiner. It is a tool for extracting information from PDF documents. It focuses on getting and analyzing text data 
1. [Layout Parser](https://github.com/Layout-Parser/layout-parser) ![](https://img.shields.io/github/stars/Layout-Parser/layout-parser.svg?style=social) - Layout Parser is a deep learning based tool for document image layout analysis tasks
1. [Tabulo](https://github.com/interviewBubble/Tabulo) ![](https://img.shields.io/github/stars/interviewBubble/Tabulo.svg?style=social) - Table extraction from images
1. [OCRmyPDF](https://github.com/jbarlow83/OCRmyPDF) ![](https://img.shields.io/github/stars/jbarlow83/OCRmyPDF.svg?style=social) - OCRmyPDF adds an OCR text layer to scanned PDF files, allowing them to be searched or copy-pasted
1. [PDFBox](https://github.com/apache/pdfbox) ![](https://img.shields.io/github/stars/apache/pdfbox.svg?style=social) - The Apache PDFBox library is an open source Java tool for working with PDF documents. This project allows creation of new PDF documents, manipulation of existing documents and the ability to extract content from documents
1. [PdfPig](https://github.com/UglyToad/PdfPig) ![](https://img.shields.io/github/stars/UglyToad/PdfPig.svg?style=social) - This project allows users to read and extract text and other content from PDF files. In addition the library can be used to create simple PDF documents containing text and geometrical shapes. This project aims to port PDFBox to C#
1. [parsing-prickly-pdfs](https://porter.io/github.com/jsfenfen/parsing-prickly-pdfs) ![](https://img.shields.io/github/stars/jsfenfen/parsing-prickly-pdfs.svg?style=social) - Resources and worksheet for the NICAR 2016 workshop of the same name
1. [pdf-text-extraction-benchmark](https://github.com/ckorzen/pdf-text-extraction-benchmark) ![](https://img.shields.io/github/stars/ckorzen/pdf-text-extraction-benchmark.svg?style=social) - PDF tools benchmark
1. [Born digital pdf scanner](https://github.com/applicaai/digital-born-pdf-scanner) ![](https://img.shields.io/github/stars/applicaai/digital-born-pdf-scanner.svg?style=social) - checking if pdf is born-digital
1. [OpenContracts](https://github.com/JSv4/OpenContracts) ![](https://img.shields.io/github/stars/JSv4/OpenContracts?style=social) Apache2-licensed, PDF annotating platform for visually-rich documents that preserves the original layout and exports x,y positional data for tokens as well as span starts and stops. Based on PAWLs, but with a Python-based backend and readily deployable on your local machine, company intranet or the web via Docker Compose.
1. [deepdoctection](https://github.com/deepdoctection/deepdoctection) ![](https://img.shields.io/github/stars/deepdoctection/deepdoctection?style=social) **deep**doctection is a Python library that orchestrates document extraction and document layout analysis tasks for images and pdf documents using deep learning models. It does not implement models but enables you to build pipelines using highly acknowledged libraries for object detection, OCR and selected NLP tasks and provides an integrated framework for fine-tuning, evaluating and running models. 

## Conferences, workshops

[Back to top](#table-of-contents)

#### General/ Business / Finance

1. **International Conference on Document Analysis and Recognition (ICDAR)** [[2021](https://icdar2021.org/), [2019](http://icdar2019.org/), [2017](http://u-pat.org/ICDAR2017/index.php)]
1. Workshop on Document Intelligence (DI) [[2021](https://document-intelligence.github.io/DI-2021/), [2019](https://sites.google.com/view/di2019)]
1. Financial Narrative Processing Workshop (FNP) [[2021](http://wp.lancs.ac.uk/cfie/fnp2021/), [2020](http://wp.lancs.ac.uk/cfie/fincausal2020/), [2019](https://www.aclweb.org/anthology/volumes/W19-64/) ]   
1. Workshop on Economics and Natural Language Processing (ECONLP) [[2021](https://julielab.de/econlp/2021/), [2019](https://sites.google.com/view/econlp-2019), [2018](https://www.aclweb.org/anthology/W18-31.pdf) ]   
1. INTERNATIONAL WORKSHOP ON DOCUMENT ANALYSIS SYSTEMS (DAS) [[2020](https://www.vlrlab.net/das2020/), [2018](https://das2018.cvl.tuwien.ac.at/en/), [2016](https://www.primaresearch.org/das2016/)]
1. [ACM International Conference on AI in Finance (ICAIF)](https://ai-finance.org/)   
1. [The AAAI-21 Workshop on Knowledge Discovery from Unstructured Data in Financial Services](https://aaai-kdf.github.io/kdf2021/)
1. [CVPR 2020 Workshop on Text and Documents in the Deep Learning Era](https://cvpr2020text.wordpress.com/accepted-papers/)
1. [KDD Workshop on Machine Learning in Finance (KDD MLF 2020)](https://sites.google.com/view/kdd-mlf-2020)
1. [FinIR 2020: The First Workshop on Information Retrieval in Finance](https://finir2020.github.io/)   
1. [2nd KDD Workshop on Anomaly Detection in Finance (KDD 2019)](https://sites.google.com/view/kdd-adf-2019)
1. [Document Understanding Conference (DUC 2007)](https://duc.nist.gov/pubs.html)

#### Scientific Document Understanding

1. [The AAAI-21 Workshop on Scientific Document Understanding (SDU 2021)](https://sites.google.com/view/sdu-aaai21/home)
1. [First Workshop on Scholarly Document Processing (SDProc 2020)](https://ornlcda.github.io/SDProc/)
1. International Workshop on SCIentific DOCument Analysis (SCIDOCA) [[2020](http://research.nii.ac.jp/SCIDOCA2020/), [2018](http://www.jaist.ac.jp/event/SCIDOCA/2018/), [2017](https://aclweb.org/portal/content/second-international-workshop-scientific-document-analysis) ]

## Blogs

[Back to top](#table-of-contents)

1. [A Survey of Document Understanding Models](https://www.pragmatic.ml/a-survey-of-document-understanding-models/), 2021
1. [Document Form Extraction](https://www.crosstab.io/product-comparisons/document-form-extraction), 2021
1. [How to automate processes with unstructured data](https://levity.ai/blog/automate-processes-with-unstructured-data), 2021
1. [A Comprehensive Guide to OCR with RPA and Document Understanding](https://nanonets.com/blog/ocr-with-rpa-and-document-understanding-uipath/), 2021
1. [Information Extraction from Receipts with Graph Convolutional Networks](https://nanonets.com/blog/information-extraction-graph-convolutional-networks/), 2021
1. [How to extract structured data from invoices](https://nanonets.com/blog/extract-structured-data-from-invoice/), 2021
1. [Extracting Structured Data from Templatic Documents](https://ai.googleblog.com/2020/06/extracting-structured-data-from.html), 2020
1. [To apply AI for good, think form extraction](http://jonathanstray.com/to-apply-ai-for-good-think-form-extraction), 2020
1. [UiPath Document Understanding Solution Architecture and Approach](https://medium.com/@lahirufernando90/uipath-document-understanding-solution-architecture-and-approach-934a9a26630a), 2020
1. [How Can I Automate Data Extraction from Complex Documents?](https://www.infrrd.ai/blog/how-can-i-automate-data-extraction-from-complex-documents), 2020
1. [LegalTech: Information Extraction in legal documents](https://naturaltech.medium.com/legaltech-information-extraction-in-legal-documents-e1843a60bc8d), 2020

## Solutions

[Back to top](#table-of-contents)

Big companies: 
1. [Abby](https://www.abbyy.com/flexicapture/)
1. [Accenture](https://www.accenture.com/us-en/services/applied-intelligence/document-understanding-solutions)
1. [Amazon](https://aws.amazon.com/about-aws/whats-new/2020/11/introducing-document-understanding-solution/)
1. [Google](https://cloud.google.com/document-ai)
1. [Microsoft](https://azure.microsoft.com/en-us/services/cognitive-services/)
1. [Uipath](https://www.uipath.com/product/document-understanding)

Smaller:
1. [Applica.ai](https://applica.ai/)
1. [Base64.ai](https://base64.ai)
1. [Docstack](https://www.docstack.com/ai-document-understanding)
1. [Element AI](https://www.elementai.com/products/document-intelligence)
1. [Indico](https://indico.io)
1. [Instabase](https://instabase.com/)
1. [Konfuzio](https://konfuzio.com/en/)
1. [Metamaze](https://metamaze.eu)
1. [Nanonets](https://nanonets.com)
1. [Rossum](https://rossum.ai/)
1. [Silo](https://silo.ai/how-document-understanding-improves-invoice-contract-and-resume-processing/)

# Examples

## Visually Rich Documents

[Back to top](#table-of-contents)

In VRDs the importance of the layout information is crucial to understand the whole document correctly (this is the case with almost all business documents). For humans spatial information improves readability and speeds document understanding.

#### Invoice / Resume / Job Ad 

<p align="center">
  <a href="https://arxiv.org/pdf/2005.11017.pdf">
    <img src="images/vrd_examples_2v2.png">
  </a>
</p>
<br/><br/>

#### NDA / Annual reports 

<p align="center">
  <a href="https://arxiv.org/abs/2003.02356">
    <img src="images/vrd_examples_1.png">
  </a>
</p>
<br/><br/>


## Key Information Extraction

[Back to top](#table-of-contents)

The aim of this task is to extract texts of a number of key fields from a given collection of documents containing similar key entities. 

<br/>

#### Scanned Receipts 

<p align="center">
  <a href="https://medium.com/analytics-vidhya/extracting-structured-data-from-invoice-96cf5e548e40">
    <img src="images/kie_examples_1.png">
  </a>
</p>
<br/><br/>

#### NDA / Annual reports 

Examples of a real business applications and data for Kleister datasets (The key entities are in blue)

<p align="center">
  <a href="https://arxiv.org/abs/2003.02356">
    <img src="images/kie_examples_2.png">
  </a>
</p>
<br/><br/>

#### Multimedia Online Flyers

An example of a commercial real estate flyer and  manually  entered  listing  information © ProMaker Commercial Real Estate LLC, © BrokerSavant Inc.

<p align="center">
  <a href="https://www.aclweb.org/anthology/N15-1032.pdf">
    <img src="images/kie_examples_3.png">
  </a>
</p>
<br/><br/>

#### Value-added tax invoice

<p align="center">
  <a href="https://arxiv.org/pdf/1903.11279.pdf">
    <img src="images/kie_examples_4.png">
  </a>
</p>
<br/><br/>

#### Webpages

<p align="center">
  <a href="https://www.microsoft.com/en-us/research/wp-content/uploads/2016/02/StructedDataExtraction_SIGIR2011.pdf">
    <img src="images/kie_examples_5.png">
  </a>
</p>
<br/><br/>


## Document Layout Analysis

[Back to top](#table-of-contents)

In computer vision or natural language processing, document layout analysis is the process of identifying and categorizing the regions of interest in the scanned image of a text document. A reading system requires the segmentation of text zones from non-textual ones and the arrangement in their correct reading order. Detection and labeling of the different zones (or blocks) as text body, illustrations, math symbols, and tables embedded in a document is called geometric layout analysis. But text zones play different logical roles inside the document (titles, captions, footnotes, etc.) and this kind of semantic labeling is the scope of the logical layout analysis. (https://en.wikipedia.org/wiki/Document_layout_analysis)


#### Scientific publication 

<p align="center">
  <a href="https://arxiv.org/pdf/1908.07836.pdf">
    <img src="images/dla_examples_1.png">
  </a>
</p>
<br/><br/>


<p align="center">
  <a href="https://arxiv.org/pdf/2006.01038.pdf">
    <img src="images/dla_examples_2.png">
  </a>
</p>
<br/><br/>


#### Historical newspapers

<p align="center">
  <a href="https://primaresearch.org/www/assets/papers/ICDAR2015_Clausner_ENPDataset.pdf">
    <img src="images/dla_examples_3.png">
  </a>
</p>
<br/><br/>


#### Business documents 

Red: text block, Blue: figure.

<p align="center">
  <a href="http://personal.psu.edu/duh188/papers/ICDAR2017_DAFANG.pdf">
    <img src="images/dla_examples_4.png">
  </a>
</p>
<br/><br/>


## Document Question Answering 

[Back to top](#table-of-contents)  


#### DocVQA example 

<p align="center">
  <a href="https://arxiv.org/pdf/2007.00398.pdf">
    <img src="images/dqa_example_2.png">
  </a>
</p>
<br/><br/>


#### [Tilt model](https://arxiv.org/pdf/2102.09550.pdf) demo

<p align="center">
  <a href="https://arxiv.org/pdf/2102.09550.pdf">
    <img src="images/dqa_example_1.gif">
  </a>
</p>
<br/><br/>

# Inspirations

[Back to top](#table-of-contents)

**Domain**
1. https://github.com/kba/awesome-ocr ![](https://img.shields.io/github/stars/kba/awesome-ocr.svg?style=social)
1. https://github.com/Liquid-Legal-Institute/Legal-Text-Analytics ![](https://img.shields.io/github/stars/Liquid-Legal-Institute/Legal-Text-Analytics.svg?style=social)
1. https://github.com/icoxfog417/awesome-financial-nlp ![](https://img.shields.io/github/stars/icoxfog417/awesome-financial-nlp.svg?style=social)
1. https://github.com/BobLd/DocumentLayoutAnalysis ![](https://img.shields.io/github/stars/BobLd/DocumentLayoutAnalysis.svg?style=social)
1. https://github.com/bikash/DocumentUnderstanding ![](https://img.shields.io/github/stars/bikash/DocumentUnderstanding.svg?style=social)
1. https://github.com/harpribot/awesome-information-retrieval ![](https://img.shields.io/github/stars/harpribot/awesome-information-retrieval.svg?style=social)
1. https://github.com/roomylee/awesome-relation-extraction ![](https://img.shields.io/github/stars/roomylee/awesome-relation-extraction.svg?style=social)
1. https://github.com/caufieldjh/awesome-bioie ![](https://img.shields.io/github/stars/caufieldjh/awesome-bioie.svg?style=social)
1. https://github.com/HelloRusk/entity-related-papers ![](https://img.shields.io/github/stars/HelloRusk/entity-related-papers.svg?style=social)
1. https://github.com/pliang279/awesome-multimodal-ml ![](https://img.shields.io/github/stars/pliang279/awesome-multimodal-ml.svg?style=social)
1. https://github.com/thunlp/LegalPapers ![](https://img.shields.io/github/stars/thunlp/LegalPapers.svg?style=social)
1. https://github.com/heartexlabs/awesome-data-labeling ![](https://img.shields.io/github/stars/heartexlabs/awesome-data-labeling.svg?style=social)

**General AI/DL/ML** 
1. https://github.com/jsbroks/awesome-dataset-tools ![](https://img.shields.io/github/stars/jsbroks/awesome-dataset-tools.svg?style=social)
1. https://github.com/EthicalML/awesome-production-machine-learning ![](https://img.shields.io/github/stars/EthicalML/awesome-production-machine-learning.svg?style=social)
1. https://github.com/eugeneyan/applied-ml ![](https://img.shields.io/github/stars/eugeneyan/applied-ml.svg?style=social)
1. https://github.com/awesomedata/awesome-public-datasets ![](https://img.shields.io/github/stars/awesomedata/awesome-public-datasets.svg?style=social)
1. https://github.com/keon/awesome-nlp ![](https://img.shields.io/github/stars/keon/awesome-nlp.svg?style=social)
1. https://github.com/thunlp/PLMpapers ![](https://img.shields.io/github/stars/thunlp/PLMpapers.svg?style=social)
1. https://github.com/jbhuang0604/awesome-computer-vision#awesome-lists ![](https://img.shields.io/github/stars/jbhuang0604/awesome-computer-vision.svg?style=social)
1. https://github.com/papers-we-love/papers-we-love ![](https://img.shields.io/github/stars/papers-we-love/papers-we-love.svg?style=social)
1. https://github.com/BAILOOL/DoYouEvenLearn ![](https://img.shields.io/github/stars/BAILOOL/DoYouEvenLearn.svg?style=social)
1. https://github.com/hibayesian/awesome-automl-papers ![](https://img.shields.io/github/stars/hibayesian/awesome-automl-papers.svg?style=social)
