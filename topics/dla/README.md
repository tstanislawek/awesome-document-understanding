## Table of contents

1. [Overview](#overview)
1. [Papers](#papers)
1. [Datasets](#datasets)


## Overview 

Document Layout Analysis is a Computer Vision approach to the problem of detection of specific objects in a document, such as:
* tables
* form fields
* clusters of text
* stamps
* images (i.e. logos...),
* barcodes,
* hand written parts,
* headers,
* check boxes,
* etc.


## Papers


* [Global Table Extractor (GTE): A Framework for Joint Table Identification and Cell Structure Recognition Using Visual Context](https://openaccess.thecvf.com/content/WACV2021/papers/Zheng_Global_Table_Extractor_GTE_A_Framework_for_Joint_Table_Identification_WACV_2021_paper.pdf)
  <details>
  <summary> Xinyi Zheng, Douglas Burdick, Lucian Popa, Xu Zhong, Nancy Xin Ru Wang <em>WACV</em> 2021 </summary>
    Documents are often the format of choice for knowledge sharing and preservation in business and science, within which are tables that capture most of the critical data. Unfortunately, most documents are stored and distributed as PDF or scanned images, which fail to preserve table formatting. Recent vision-based deep learning approaches have been proposed to address this gap, but most still cannot achieve state-of-the-art results. We present Global Table Extractor (GTE), a vision-guided systematic framework for joint table detection and cell structured recognition, which could be built on top of any object detection model. With GTE-Table, we invent a new penalty based on the natural cell containment constraint of tables to train our table network aided by cell location predictions. GTE-Cell is a new hierarchical cell detection network that leverages table styles. Further, we design a method to automatically label table and cell structure in existing documents to cheaply create a large corpus of training and test data. We use this to enhance PubTabNet with cell labels and create FinTabNet, real-world and complex scientific and financial datasets with detailed table structure annotations to help train and test structure recognition. Our deep learning framework surpasses previous state-of-the-art results on the ICDAR 2013 and ICDAR 2019 table competition test dataset in both table detection and cell structure recognition. Further experiments demonstrate a greater than 45% improvement in cell structure recognition when compared to a vanilla RetinaNet object detection model in our new out-of-domain financial dataset (Fintabnet). 
  </details>

* **[CascadeTabNet: An approach for end to end table detection and structure recognition from image-based documents](https://arxiv.org/pdf/2004.12629.pdf)**, \[[code](https://github.com/DevashishPrasad/CascadeTabNet)\]
  <details>
  <summary> Devashish Prasad, Ayan Gadpal, Kshitij Kapadni, Manish Visave, Kavita Sultanpure <em>CVPR Workshop</em> 2020 </summary>
    CascadTabNet is an automatic table recognition method for interpretation of tabular data in document images. We present an improved deep learning-based end to end approach for solving both problems of table detection and structure recognition using a single Convolution Neural Network (CNN) model. CascadeTabNet is a Cascade mask Region-based CNN High-Resolution Network (Cascade mask R-CNN HRNet) based model that detects the regions of tables and recognizes the structural body cells from the detected tables at the same time. We evaluate our results on ICDAR 2013, ICDAR 2019 and TableBank public datasets. We achieved 3rd rank in ICDAR 2019 post-competition results for table detection while attaining the best accuracy results for the ICDAR 2013 and TableBank dataset. We also attain the highest accuracy results on the ICDAR 2019 table structure recognition dataset.    
  </details>

* [Document Structure Extraction for Forms using Very High Resolution Semantic Segmentation](https://www.researchgate.net/profile/Mausoom-Sarkar/publication/337590348_Document_Structure_Extraction_for_Forms_using_Very_High_Resolution_Semantic_Segmentation/links/5e6c91bc299bf12e23c35820/Document-Structure-Extraction-for-Forms-using-Very-High-Resolution-Semantic-Segmentation.pdf)
  <details>
  <summary> Mausoom Sarkar et al. <em>ECCV</em> 2020 </summary>
    In this work, we look at the problem of structure extraction from document images with a specific focus on forms. Forms as a document class have not received much attention, even though they comprise a significant fraction of documents and enable several applications. Forms possess a rich, complex, hierarchical, and high-density semantic structure that poses several challenges to semantic segmentation methods. We propose a prior based deep CNN-RNN hierarchical network architecture that enables document structure extraction using very high resolution(1800 x 1000) images. We divide the document image into overlapping horizontal strips such that the network segments a strip and uses its prediction mask as prior while predicting the segmentation for the subsequent strip. We perform experiments establishing the effectiveness of our strip based network architecture through ablation methods and comparison with low-resolution variations. We introduce our new rich human-annotated forms dataset, and we show that our method significantly outperforms other segmentation baselines in extracting several hierarchical structures on this dataset. We also outperform other baselines in table detection task on the Marmot dataset. Our method is currently being used in a world-leading customer experience management software suite for automated conversion of paper and PDF forms to modern HTML based forms.
  </details>

* [Visual Segmentation for Information Extraction from Heterogeneous Visually Rich Documents](https://www.researchgate.net/publication/333859687_Visual_Segmentation_for_Information_Extraction_from_Heterogeneous_Visually_Rich_Documents)
  <details>
  <summary> Ritesh Sarkhel, Arnab  Nandi <em>SIGMOD</em> 2019</summary>
    Physical and digital documents often contain visually rich information. With such information, there is no strict ordering or positioning in the document where the data values must appear. Along with textual cues, these documents often also rely on salient visual features to define distinct semantic boundaries and augment the information they disseminate. When performing information extraction (IE), traditional techniques fall short, as they use a text-only representation and do not consider the visual cues inherent to the layout of these documents. We propose VS2, a generalized approach for information extraction from heterogeneous visually rich documents. There are two major contributions of this work. First, we propose a robust segmentation algorithm that decomposes a visually rich document into a bag of visually isolated but semantically coherent areas, called logical blocks. Document type agnostic low-level visual and semantic features are used in this process. Our second contribution is a distantly supervised search-and-select method for identifying the named entities within these documents by utilizing the context boundaries defined by these logical blocks. Experimental results on three heterogeneous datasets suggest that the proposed approach significantly outperforms its text-only counterparts on all datasets. Comparing it against the state-of-the-art methods also reveal that VS2 performs comparably or better on all datasets.
  </details>

* [One-shot field spotting on colored forms using subgraph isomorphism](https://hal.archives-ouvertes.fr/hal-01249470/file/bare_conf.pdf)
  <details>
  <summary> Maroua Hammami et al. <em>ICDAR</em> 2015</summary>
    This paper presents an approach for spotting textual fields in commercial and administrative colored forms. We proceed by locating these fields thanks to their neighboring context which is modeled with a structural representation. First, informative zones are extracted. Second, forms are represented by graphs. In these graphs, nodes represent colored rectangular shapes while edges represent neighboring relations. Finally, the neighboring context of the queried region of interest is modeled as a graph. Subgraph isomorphism is applied in order to locate this ROI in the structural representation of a whole document. Evaluated on a 130-document image dataset, experimental results show up that our approach is efficient and that the requested information is found even if its position is changed.
  </details>


## Datasets 

* [DocBank: A Benchmark Dataset for Document Layout Analysis](https://arxiv.org/pdf/2006.01038.pdf), \[[code/data](https://github.com/doc-analysis/DocBank)\]
    <details>
    <summary> Minghao Li et al. <em>COLING</em> 2020 </summary>
        DocBank is a new large-scale dataset that is constructed using a weak supervision approach. It enables models to integrate both the textual and layout information for downstream tasks. The current DocBank dataset totally includes 500K document pages, where 400K for training, 50K for validation and 50K for testing.
    </details>


* [Tablebank: Table benchmark for image-based table detection and recognition](https://www.aclweb.org/anthology/2020.lrec-1.236/), \[[code/data](https://github.com/doc-analysis/TableBank)\]
  <details>
  <summary> Minghao Li, Lei Cui, Shaohan Huang, Furu Wei, Ming Zhou, Zhoujun Li <em>LREC</em> 2020 </summary>
    We present TableBank, a new image-based table detection and recognition dataset built with novel weak supervision from Word and Latex documents on the internet. Existing research for image-based table detection and recognition usually fine-tunes pre-trained models on out-of-domain data with a few thousand human-labeled examples, which is difficult to generalize on real-world applications. With TableBank that contains 417K high quality labeled tables, we build several strong baselines using state-of-the-art models with deep neural networks. We make TableBank publicly available and hope it will empower more deep learning approaches in the table detection and recognition task. The dataset and models can be downloaded from https://github.com/doc-analysis/TableBank.
  </details>

* [HJDataset: A Large Dataset of Historical Japanese Documents with Complex Layouts](https://arxiv.org/pdf/2004.08686.pdf), \[[code](https://github.com/dell-research-harvard/HJDataset/)\] 
  <details>
  <summary> Zejiang Shen, Kaixuan Zhang, Melissa Dell <em>CVPR2020 Workshop</em> 2020 </summary>
    Deep learning-based approaches for automatic document layout analysis and content extraction have the potential to unlock rich information trapped in historical documents on a large scale. One major hurdle is the lack of large datasets for training robust models. In particular, little training data exist for Asian languages. To this end, we present HJDataset, a Large Dataset of Historical Japanese Documents with Complex Layouts. It contains over 250,000 layout element annotations of seven types. In addition to bounding boxes and masks of the content regions, it also includes the hierarchical structures and reading orders for layout elements. The dataset is constructed using a combination of human and machine efforts. A semi-rule based method is developed to extract the layout elements, and the results are checked by human inspectors. The resulting large-scale dataset is used to provide baseline performance analyses for text region detection using state-of-the-art deep learning models. And we demonstrate the usefulness of the dataset on real-world document digitization tasks. 
  </details>


* [PubLayNet: largest dataset ever for document layout analysis](https://arxiv.org/abs/1908.07836), \[[code](https://github.com/ibm-aur-nlp/PubLayNet)\]
    <details>
    <summary> Xu Zhong, Jianbin Tang, Antonio Jimeno Yepes <em>ICDAR</em> 2019 </summary>
      Recognizing the layout of unstructured digital documents is an important step when parsing the documents into structured machine-readable format for downstream applications. Deep neural networks that are developed for computer vision have been proven to be an effective method to analyze layout of document images. However, document layout datasets that are currently publicly available are several magnitudes smaller than established computing vision datasets. Models have to be trained by transfer learning from a base model that is pre-trained on a traditional computer vision dataset. In this paper, we develop the PubLayNet dataset for document layout analysis by automatically matching the XML representations and the content of over 1 million PDF articles that are publicly available on PubMed Central. The size of the dataset is comparable to established computer vision datasets, containing over 360 thousand document images, where typical document layout elements are annotated. The experiments demonstrate that deep neural networks trained on PubLayNet accurately recognize the layout of scientific articles. The pre-trained models are also a more effective base mode for transfer learning on a different document domain. We release the dataset to support development and evaluation of more advanced models for document layout analysis. 
    </details>


* [ICDAR2017 Competition on Recognition of Early Indian Printed Documents – REID2017](https://www.primaresearch.org/www/assets/papers/ICDAR2017_Clausner_REID2017.pdf), \[[Website](https://www.primaresearch.org/datasets/REID2017)\]
  <details>
  <summary> Christian Clausner, Apostolos Antonacopoulos, Tom Derrick, Stefan Pletschacher <em>ICDAR</em> 2017 </summary>
    This paper presents an objective comparative evaluation of page analysis and recognition methods for historical documents with text mainly in Bengali language and script. It describes the competition (modus operandi, dataset and evaluation methodology) held in the context of ICDAR2017, presenting the results of the evaluation of seven methods – three submitted and four variations of open source state-of-the-art systems. The focus is on optical character recognition (OCR) performance. Different evaluation metrics were used to gain an insight into the algorithms, including new character accuracy metrics to better reflect the difficult circumstances presented by the documents. The results indicate that deep learning approaches are the most promising, but there is still a considerable need to develop robust methods that deal with challenges of historic material of this nature. 
  </details>


* [A Realistic Dataset for Performance Evaluation of Document Layout Analysis](https://www.semanticscholar.org/paper/A-Realistic-Dataset-for-Performance-Evaluation-of-Antonacopoulos-Bridson/c4288ec46736acbe7ca1fc54d43f94b19b602450), \[[Website](http://www.primaresearch.org/datasets/Layout_Analysis)\]
  <details>
  <summary> Apostolos Antonacopoulos, David Bridson, Christos Papadopoulos, Stefan Pletschacher <em>ICDAR</em> 2009 </summary>
    There is a significant need for a realistic dataset on which to evaluate layout analysis methods and examine their performance in detail. This paper presents a new dataset (and the methodology used to create it) based on a wide range of contemporary documents. Strong emphasis is placed on comprehensive and detailed representation of both complex and simple layouts, and on colour originals. In-depth information is recorded both at the page and region level. Ground truth is efficiently created using a new semi-automated tool and stored in a new comprehensive XML representation, the PAGE format. The dataset can be browsed and searched via a web-based front end to the underlying database and suitable subsets (relevant to specific evaluation goals) can be selected and downloaded.  
  </details>
