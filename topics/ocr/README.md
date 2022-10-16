## Table of contents

1. [Benchmarks](#benchmarks)
1. [Papers](#papers)
1. [Datasets](#datasets)
1. [Useful links](#useful-links)


## Benchmarks 

1. Best OCR by Text Extraction Accuracy in 2021, https://research.aimultiple.com/ocr-accuracy/
1. Best OCR Software of 2021, https://nanonets.com/blog/ocr-software-best-ocr-software/ 
1. Comparison of OCR tools: how to choose the best tool for your project, https://medium.com/dida-machine-learning/comparison-of-ocr-tools-how-to-choose-the-best-tool-for-your-project-bd21fb9dce6b
1. Our Search for the Best OCR Tool, and What We Found, 2019, https://source.opennews.org/articles/so-many-ocr-options/ (https://github.com/factful/ocr_testing)


## Papers 

* [DavarOCR: A Toolbox for OCR and Multi-Modal Document Understanding](https://arxiv.org/abs/2207.06695), \[[code/](https://github.com/hikopensource/Davar-Lab-OCR) \]
  <details>
  <summary> Liang Qiao, Hui Jiang, Ying Chen, Can Li, Pengfei Li, Zaisheng Li, Baorui Zou, Dashan Guo, Yingda Xu, Yunlu Xu, Zhanzhan Cheng, Yi Niu <em>ACM MM</em> 2022 </summary>
    This paper presents DavarOCR, an open-source toolbox for OCR and document understanding tasks. DavarOCR currently implements 19 advanced algorithms, covering 9 different task forms. DavarOCR provides detailed usage instructions and the trained models for each algorithm. Compared with the previous opensource OCR toolbox, DavarOCR has relatively more complete support for the sub-tasks of the cutting-edge technology of document understanding. In order to promote the development and application of OCR technology in academia and industry, we pay more attention to the use of modules that different sub-domains of technology can share.  
  </details> 

* [TrOCR: Transformer-based Optical Character Recognition with Pre-trained Models](https://arxiv.org/abs/2109.10282), \[[code/data](https://github.com/microsoft/unilm/tree/master/trocr) \]
  <details>
  <summary> Minghao Li, Tengchao Lv, Lei Cui, Yijuan Lu, Dinei Florencio, Cha Zhang, Zhoujun Li, Furu Wei <em>arxiv</em> 2021 </summary>
    Text recognition is a long-standing research problem for document digitalization. Existing approaches for text recognition are usually built based on CNN for image understanding and RNN for char-level text generation. In addition, another language model is usually needed to improve the overall accuracy as a post-processing step. In this paper, we propose an end-to-end text recognition approach with pre-trained image Transformer and text Transformer models, namely TrOCR, which leverages the Transformer architecture for both image understanding and wordpiece-level text generation. The TrOCR model is simple but effective, and can be pre-trained with large-scale synthetic data and fine-tuned with human-labeled datasets. Experiments show that the TrOCR model outperforms the current state-of-the-art models on both printed and handwritten text recognition tasks.  
  </details>

* [Lights, Camera, Action! A Framework to Improve NLP Accuracy over OCR documents](https://arxiv.org/abs/2108.02899)
  <details>
  <summary> Amit Gupte, Alexey Romanov, Sahitya Mantravadi, Dalitso Banda, Jianjie Liu, Raza Khan, Lakshmanan Ramu Meenal, Benjamin Han, Soundar Srinivasan <em> Document Intelligence Workshop at KDD</em> 2021 </summary>
    Document digitization is essential for the digital transformation of our societies, yet a crucial step in the process, Optical Character Recognition (OCR), is still not perfect. Even commercial OCR systems can produce questionable output depending on the fidelity of the scanned documents. In this paper, we demonstrate an effective framework for mitigating OCR errors for any downstream NLP task, using Named Entity Recognition (NER) as an example. We first address the data scarcity problem for model training by constructing a document synthesis pipeline, generating realistic but degraded data with NER labels. We measure the NER accuracy drop at various degradation levels and show that a text restoration model, trained on the degraded data, significantly closes the NER accuracy gaps caused by OCR errors, including on an out-of-domain dataset. For the benefit of the community, we have made the document synthesis pipeline available as an open-source project. 
  </details>

* [Text Recognition in the Wild: A Survey](https://arxiv.org/pdf/2005.03492.pdf)
  <details>
  <summary> Xiaoxue Chen, Lianwen Jin, Yuanzhi Zhu, Canjie Luo, T. Wang <em>arxiv</em> 2020 </summary>
    The history of text can be traced back over thousands of years. Rich and precise semantic information carried by text is important in a wide range of vision-based application scenarios. Therefore, text recognition in natural scenes has been an active research field in computer vision and pattern recognition. In recent years, with the rise and development of deep learning, numerous methods have shown promising in terms of innovation, practicality, and efficiency. This paper aims to (1) summarize the fundamental problems and the state-of-the-art associated with scene text recognition; (2) introduce new insights and ideas; (3) provide a comprehensive review of publicly available resources; (4) point out directions for future work. In summary, this literature review attempts to present the entire picture of the field of scene text recognition. It provides a comprehensive reference for people entering this field, and could be helpful to inspire future research. Related resources are available at our Github repository: this https URL.
  </details>


## Datasets 

1. Total-Text [paper](http://cs-chan.com/doc/IJDAR2019.pdf) [repo](https://github.com/cs-chan/Total-Text-Dataset) - scene text detection dataset
1. [Synth90k](https://www.robots.ox.ac.uk/~vgg/data/text/#sec-synth) - popular dataset of single-word synthetic images (90k words, 9M images)
1. [SROIE](https://rrc.cvc.uab.es/?ch=13) - scanned receipts OCR and information extraction
1. [FUNSD](https://guillaumejaume.github.io/FUNSD/) - A dataset for Text Detection, Optical Character Recognition, Spatial Layout Analysis and Form Understanding
1. [RDCL2019](https://www.primaresearch.org/RDCL2019/) - ICDAR Competition on Recognition of Documents with Complex Layouts
1. [REID2019](https://www.primaresearch.org/REID2019/) - ICDAR Competition on Recognition of Early Indian printed Documents
1. [RETAS OCR EVALUATION DATASET](https://ciir.cs.umass.edu/downloads/ocr-evaluation/) - scanned books from Gutenberg project

## Useful links 

1. **https://github.com/mindee/doctr - alternative for Tesseract project!**
2. https://mindee.com/
3. https://github.com/open-mmlab/mmocr 
4. https://github.com/Belval/TextRecognitionDataGenerator 
5. http://tc11.cvc.uab.es/datasets/type/
6. https://www.primaresearch.org/
7. http://iapr-tc11.org/mediawiki/index.php?title=IAPR-TC11:Reading_Systems
