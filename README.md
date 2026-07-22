# Event Extraction Papers

A curated bibliography of research on **Event Extraction (EE)** and closely related event-centric Natural Language Processing tasks.

The collection covers the evolution of the field from pattern- and rule-based information extraction to statistical and neural models, document-level extraction, generative approaches, large language models (LLMs), multilingual and multimodal extraction, event coreference, and event structure induction.

> **Last major update:** July 2026  
> **Scope:** Event detection, event argument extraction, end-to-end event extraction, document- and cross-document event extraction, multilingual/cross-lingual EE, multimodal EE, event coreference, event-event relations, event schemas, datasets, benchmarks, and tools.  
> This is a **curated rather than exhaustive** list.

## Task abbreviations

| Tag | Meaning |
|---|---|
| `ED` | Event Detection / trigger identification and classification |
| `EAE` | Event Argument Extraction |
| `EE` | End-to-end or general Event Extraction |
| `DEE` | Document-level Event Extraction |
| `CDEE` | Cross-document / multi-document Event Extraction |
| `ECR` | Event Coreference Resolution |
| `MEE` | Multimodal / Multimedia Event Extraction |
| `OpenEE` | Open-domain or open-schema Event Extraction |
| `LLM` | Large Language Model-based approach |

Research papers are listed under **one primary methodological category**. Cross-cutting properties are represented with tags. A paper may additionally be referenced in **Datasets**, **Tools**, or **Surveys/Evaluation** when it introduces a resource.

---

## Table of Contents

- [Foundations: Pattern, Rule and Knowledge-Based Methods](#foundations-pattern-rule-and-knowledge-based-methods)
- [Statistical and Structured Machine Learning](#statistical-and-structured-machine-learning)
- [Neural and Pretrained Event Extraction](#neural-and-pretrained-event-extraction)
- [Generative, Prompt-Based and LLM Event Extraction](#generative-prompt-based-and-llm-event-extraction)
- [Few-Shot, Zero-Shot and Low-Resource Event Extraction](#few-shot-zero-shot-and-low-resource-event-extraction)
- [Document-Level and Cross-Document Event Extraction](#document-level-and-cross-document-event-extraction)
- [Multilingual and Cross-Lingual Event Extraction](#multilingual-and-cross-lingual-event-extraction)
- [Multimodal Event Extraction](#multimodal-event-extraction)
- [Semi-Supervised, Weakly Supervised and Unsupervised Learning](#semi-supervised-weakly-supervised-and-unsupervised-learning)
- [Open-Domain Event Extraction and Schema Induction](#open-domain-event-extraction-and-schema-induction)
- [Event Coreference](#event-coreference)
- [Event Relations, Temporal Structure and Causality](#event-relations-temporal-structure-and-causality)
- [Surveys and Evaluation Studies](#surveys-and-evaluation-studies)
- [Datasets and Benchmarks](#datasets-and-benchmarks)
- [Tools and Repositories](#tools-and-repositories)
- [Linguistic Foundations](#linguistic-foundations)
- [Other Lists](#other-lists)
- [Contributing](#contributing)

---

# Foundations: Pattern, Rule and Knowledge-Based Methods

## 1993

- [Automatically Constructing a Dictionary for Information Extraction Tasks](https://aaai.org/Papers/AAAI/1993/AAAI93-121.pdf) — Ellen Riloff. `IE` `pattern learning`

## 1995

- [Acquisition of Linguistic Patterns for Knowledge-Based Information Extraction](https://ieeexplore.ieee.org/document/469825) — Jun-Tae Kim, D. I. Moldovan. `IE` `pattern learning`
- [Automatically Acquiring Conceptual Patterns without an Annotated Corpus](https://aclanthology.org/W95-0112/) — Ellen Riloff, Jay Shoen. `IE` `weak supervision`
- [Learning Information Extraction Patterns from Examples](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.597.3832&rep=rep1&type=pdf) — Scott B. Huffman. `IE` `pattern induction`

## 1998

- [Multistrategy Learning for Information Extraction](https://www.semanticscholar.org/paper/Multistrategy-Learning-for-Information-Extraction-Freitag/29c99d263b5e05aae6bb96f004f025dcc9b5caae) — Dayne Freitag. `IE`

## 1999

- [Learning Dictionaries for Information Extraction by Multi-Level Bootstrapping](https://www.researchgate.net/publication/221603776_Learning_Dictionaries_for_Information_Extraction_by_Multi-Level_Bootstrapping) — Ellen Riloff, Rosie Jones. `IE` `bootstrapping`

## 2000

- [REES: A Large-Scale Relation and Event Extraction System](https://aclanthology.org/A00-1011/) — Chinatsu Aone, Mila Ramos-Santacruz. `EE` `rule-based`
- [Automatic Acquisition of Domain Knowledge for Information Extraction](https://aclanthology.org/C00-2136/) — Roman Yangarber, Ralph Grishman, Pasi Tapanainen, Silja Huttunen. `IE` `pattern discovery`

## 2001

- [Adaptive Information Extraction from Text by Rule Induction and Generalisation](https://www.semanticscholar.org/paper/Adaptive-Information-Extraction-from-Text-by-Rule-Ciravegna/436087083293ca8728fb96d2e05c011fff2c7751) — Fabio Ciravegna. `IE` `rule induction`

## 2002

- [Event Pattern Discovery from the Stock Market Bulletin](https://link.springer.com/chapter/10.1007/3-540-36182-0_30) — Fang Li, Huanye Sheng, Dongmo Zhang. `EE` `financial`

## 2003

- [Bottom-Up Relational Learning of Pattern Matching Rules for Information Extraction](https://www.researchgate.net/publication/220321036_Bottom-Up_Relational_Learning_of_Pattern_Matching_Rules_for_Information_Extraction) — Mary Elaine Califf, Raymond J. Mooney. `IE`
- [An Improved Extraction Pattern Representation Model for Automatic IE Pattern Acquisition](https://aclanthology.org/P03-1029/) — Kiyoshi Sudo, Satoshi Sekine, Ralph Grishman. `IE`

## 2005

- [Automatic Event and Relation Detection with Seeds of Varying Complexity](https://www.aaai.org/Papers/Workshops/2006/WS-06-07/WS06-07-004.pdf) — Feiyu Xu, Hans Uszkoreit, Hong Li. `EE`
- [A Semantic Approach to IE Pattern Induction](https://www.semanticscholar.org/paper/A-Semantic-Approach-to-IE-Pattern-Induction-Stevenson-Greenwood/f30b903047284e8a253b2da38530b99b6db13317) — Mark Stevenson, Mark A. Greenwood. `IE`

## 2008

- [Real-Time News Event Extraction for Global Crisis Monitoring](https://link.springer.com/chapter/10.1007/978-3-540-69858-6_21) — Hristo Tanev, Jakub Piskorski, Martin Atkinson. `EE` `news`

## 2009

- [Biomedical Event Extraction without Training Data](https://aclanthology.org/W09-1405/) — Andreas Vlachos, Paula Buttery, Diarmuid Ó Séaghdha, Ted Briscoe. `EE` `biomedical`
- [Syntactic Dependency Based Heuristics for Biological Event Extraction](https://aclanthology.org/W09-1418/) — Halil Kilicoglu, Sabine Bergler. `EE` `biomedical`

## 2010

- [Semi-Automatic Financial Events Discovery Based on Lexico-Semantic Patterns](https://personal.eur.nl/frasincar/papers/IJWET2010/ijwet2010.pdf) — Jethro Borsje, Frederik Hogenboom, Flavius Frasincar. `EE` `financial`
- [Filtered Ranking for Bootstrapping in Event Extraction](https://aclanthology.org/C10-1077/) — Shasha Liao, Ralph Grishman. `EE` `bootstrapping`

## 2011

- [Effective Bio-Event Extraction Using Trigger Words and Syntactic Dependencies](https://onlinelibrary.wiley.com/doi/abs/10.1111/j.1467-8640.2011.00401.x) — Halil Kilicoglu, Sabine Bergler. `EE` `biomedical`

## 2012

- [Ontology-Based Information and Event Extraction for Business Intelligence](https://link.springer.com/chapter/10.1007/978-3-642-33185-5_10) — Ernest Arendarenko, Tuomo Kakkonen. `EE` `business`
- [A Real-Time News Event Extraction Framework for Vietnamese](https://ieeexplore.ieee.org/document/6299414) — Mai-Vu Tran et al. `EE` `Vietnamese`

## 2015

- [A Domain-independent Rule-based Framework for Event Extraction](https://aclanthology.org/P15-4022/) — Marco A. Valenzuela-Escárcega, Gus Hahn-Powell, Mihai Surdeanu, Thomas Hicks. `EE` `ODIN`

## 2018

- [Including New Patterns to Improve Event Extraction Systems](https://pdfs.semanticscholar.org/dc04/f814fb210edf62a6237c52eb88ac98a5b732.pdf) — Kai Cao, Xiang Li, Weicheng Ma, Ralph Grishman. `ED`
- [Rule Based Event Extraction System from Newswires and Social Media Text in Indian Languages](https://www.researchgate.net/publication/329735770_Rule_based_Event_Extraction_System_from_Newswires_and_Social_Media_Text_in_Indian_Languages_EventXtract-IL_for_English_and_Hindi_Data) — Anita Saroj, Rajesh Kumar Munodtiya, Sukomal Pal. `EE` `multilingual`

---

# Statistical and Structured Machine Learning

## 2002

- [A Maximum Entropy Approach to Information Extraction from Semi-Structured and Free Text](https://www.aaai.org/Papers/AAAI/2002/AAAI02-118.pdf) — Hai Leong Chieu, Hwee Tou Ng. `IE`

## 2006

- [The Stages of Event Extraction](https://aclanthology.org/W06-0901/) — David Ahn. `EE`  
  A foundational decomposition of event extraction into trigger/event detection and argument-related subtasks.

## 2007

- [Extracting Violent Events From On-Line News for Ontology Population](https://link.springer.com/chapter/10.1007/978-3-540-72035-5_22) — Jakub Piskorski, Hristo Tanev, Pinar Oezden Wennerberg. `EE`

## 2009

- [Extracting Complex Biological Events with Rich Graph-Based Feature Sets](https://aclanthology.org/W09-1402/) — Jari Björne et al. `EE` `biomedical`
- [Language Specific Issue and Feature Exploration in Chinese Event Extraction](https://pdfs.semanticscholar.org/b6ce/13412a9cadb6c57f1349ad389affbdea2321.pdf) — Zheng Chen, Heng Ji. `EE` `Chinese`
- [A Markov Logic Approach to Bio-Molecular Event Extraction](https://aclanthology.org/W09-1406/) — Sebastian Riedel et al. `EE` `joint inference`

## 2010

- [Event Extraction with Complex Event Classification Using Rich Features](https://www.worldscientific.com/doi/abs/10.1142/S0219720010004586) — Makoto Miwa, Rune Sætre, Jin-Dong Kim, Jun'ichi Tsujii. `EE` `biomedical`
- [Complex Event Extraction at PubMed Scale](https://academic.oup.com/bioinformatics/article/26/12/i382/282442) — Jari Björne et al. `EE` `biomedical`

## 2011

- [Word Sense Disambiguation for Event Trigger Word Detection in Biomedicine](https://bmcbioinformatics.biomedcentral.com/articles/10.1186/1471-2105-12-S2-S4) — David Martinez, Timothy Baldwin. `ED`
- [Using Cross-Entity Inference to Improve Event Extraction](https://aclanthology.org/P11-1113/) — Yu Hong et al. `EE`
- [Acquiring Topic Features to Improve Event Extraction](https://aclanthology.org/R11-1002/) — Shasha Liao, Ralph Grishman. `EE`
- [Fast and Robust Joint Models for Biomedical Event Extraction](https://aclanthology.org/D11-1001/) — Sebastian Riedel, Andrew McCallum. `EE` `joint`
- [Coreference Based Event-Argument Relation Extraction on Biomedical Text](https://jbiomedsem.biomedcentral.com/articles/10.1186/2041-1480-2-S5-S6) — Katsumasa Yoshikawa et al. `EAE`
- [Biomedical Event Extraction from Abstracts and Full Papers using Search-based Structured Prediction](https://aclanthology.org/W11-1805/) — Andreas Vlachos, Mark Craven. `EE`
- [Biomedical Events Extraction Using the Hidden Vector State Model](https://www.sciencedirect.com/science/article/pii/S0933365711001060) — Deyu Zhou, Yulan He. `EE`
- [Event Extraction as Dependency Parsing](https://aclanthology.org/P11-1163/) — David McClosky, Mihai Surdeanu, Christopher Manning. `EE`
- [Robust Biomedical Event Extraction with Dual Decomposition and Minimal Domain Adaptation](https://aclanthology.org/W11-1807/) — Sebastian Riedel, Andrew McCallum. `EE`

## 2012

- [Boosting Automatic Event Extraction from the Literature using Domain Adaptation and Coreference Resolution](https://academic.oup.com/bioinformatics/article/28/13/1759/234417) — Makoto Miwa, Paul Thompson, Sophia Ananiadou. `EE`
- [Employing Compositional Semantics and Discourse Consistency in Chinese Event Extraction](https://aclanthology.org/D12-1092/) — Peifeng Li et al. `ED` `Chinese`
- [Joint Modeling of Trigger Identification and Event Type Determination in Chinese Event Extraction](https://aclanthology.org/C12-1100/) — Peifeng Li et al. `ED`
- [Joint Modeling for Chinese Event Extraction with Rich Linguistic Features](https://aclanthology.org/C12-1033/) — Chen Chen, Vincent Ng. `EE`

## 2013

- [A Hybrid Approach for Biomedical Event Extraction](https://aclanthology.org/W13-2017/) — Xuan Quang Pham, Minh Quang Le, Bao Quoc Ho. `EE`
- [Joint Modeling of Argument Identification and Role Determination in Chinese Event Extraction with Discourse-Level Information](https://www.ijcai.org/Proceedings/13/Papers/313.pdf) — Peifeng Li, Qiaoming Zhu, Guodong Zhou. `EAE`
- [Joint Event Extraction via Structured Prediction with Global Features](https://aclanthology.org/P13-1008/) — Qi Li, Heng Ji, Liang Huang. `EE` `joint`
- [Biomedical Event Extraction by Multi-class Classification of Pairs of Text Entities](https://aclanthology.org/W13-2006/) — Xiao Liu, Antoine Bordes, Yves Grandvalet. `EE`

## 2014

- [A Novel Feature Selection Strategy for Enhanced Biomedical Event Extraction Using the Turku System](https://www.hindawi.com/journals/bmri/2014/205239/) — Jingbo Xia, Alex Chengyu Fang, Xing Zhang. `EE`
- [Relieving the Computational Bottleneck: Joint Inference for Event Extraction with High-Dimensional Features](https://aclanthology.org/D14-1090/) — Deepak Venugopal et al. `EE`

## 2015

- [Improving Event Detection with Active Learning](https://aclanthology.org/R15-1010/) — Kai Cao, Xiang Li, Miao Fan, Ralph Grishman. `ED`
- [Disease Event Detection Based on Deep Modality Analysis](https://aclanthology.org/P15-3005/) — Yoshiaki Kitagawa et al. `ED`
- [Event Extraction as Frame-Semantic Parsing](https://aclanthology.org/S15-1018/) — Alex Judea, Michael Strube. `EE`

## 2016

- [RBPB: Regularization-Based Pattern Balancing Method for Event Extraction](https://aclanthology.org/P16-1116/) — Lei Sha et al. `EE`
- [A Probabilistic Soft Logic Based Approach to Exploiting Latent and Global Information in Event Classification](https://ojs.aaai.org/index.php/AAAI/article/view/10356) — Shulin Liu et al. `ED`

---

# Neural and Pretrained Event Extraction

## 2015

- [Event Detection and Domain Adaptation with Convolutional Neural Networks](https://aclanthology.org/P15-2060/) — Thien Huu Nguyen, Ralph Grishman. `ED` `CNN` — [code](https://github.com/ThanhChinhBK/event_detector)
- [Event Extraction via Dynamic Multi-Pooling Convolutional Neural Networks](https://aclanthology.org/P15-1017/) — Yubo Chen et al. `EE` `CNN`
- [Event Nugget Detection, Classification and Coreference Resolution using Deep Neural Networks and eXtreme Gradient Boosting](https://github.com/UKPLab/tac2015-event-detection) — Nils Reimers, Iryna Gurevych. `ED` `ECR`

## 2016

- [Modeling Skip-Grams for Event Detection with Convolutional Neural Networks](https://aclanthology.org/D16-1085/) — Thien Huu Nguyen, Ralph Grishman. `ED`
- [Joint Event Extraction Based on Skip-Window Convolutional Neural Networks](https://link.springer.com/chapter/10.1007/978-3-319-50496-4_27) — Zhengkuan Zhang, Weiran Xu, Qianqian Chen. `EE`
- [Joint Event Extraction via Recurrent Neural Networks](https://aclanthology.org/N16-1034/) — Thien Huu Nguyen, Kyunghyun Cho, Ralph Grishman. `EE` — [code](https://github.com/anoperson/jointEE-NN)
- [Event Nugget Detection with Forward-Backward Recurrent Neural Networks](https://aclanthology.org/P16-2060/) — Reza Ghaeini et al. `ED`
- [Event Extraction via Bidirectional Long Short-Term Memory Tensor Neural Network](https://link.springer.com/chapter/10.1007/978-3-319-47674-2_17) — Yubo Chen et al. `EE`
- [A Convolution BiLSTM Neural Network Model for Chinese Event Extraction](https://link.springer.com/chapter/10.1007/978-3-319-50496-4_23) — Ying Zeng et al. `EE` `Chinese`

## 2017

- [Improving Event Detection via Information Sharing among Related Event Types](https://link.springer.com/chapter/10.1007/978-3-319-69005-6_11) — Shulin Liu et al. `ED`
- [Biomedical Event Extraction using Abstract Meaning Representation](https://aclanthology.org/W17-2315/) — Sudha Rao et al. `EE` `AMR`
- [Exploiting Argument Information to Improve Event Detection via Supervised Attention Mechanisms](https://aclanthology.org/P17-1164/) — Shulin Liu et al. `ED`
- [Identifying Civilians Killed by Police with Distantly Supervised Entity-Event Extraction](https://aclanthology.org/D17-1163/) — Katherine Keith et al. `EE`

## 2018

- [Similar but not the Same: Word Sense Disambiguation Improves Event Detection via Neural Representation Matching](https://aclanthology.org/D18-1517/) — Weiyi Lu, Thien Huu Nguyen. `ED`
- [Exploiting Contextual Information via Dynamic Memory Network for Event Detection](https://aclanthology.org/D18-1127/) — Shaobo Liu et al. `ED`
- [Nugget Proposal Networks for Chinese Event Detection](https://aclanthology.org/P18-1145/) — Hongyu Lin et al. `ED` `Chinese`
- [Jointly Extracting Event Triggers and Arguments by Dependency-Bridge RNN and Tensor-Based Argument Interaction](https://ojs.aaai.org/index.php/AAAI/article/view/12009) — Lei Sha et al. `EE`
- [One for All: Neural Joint Modeling of Entities and Events](https://arxiv.org/abs/1812.00195) — Trung Minh Nguyen, Thien Huu Nguyen. `EE`
- [Jointly Multiple Events Extraction via Attention-based Graph Information Aggregation](https://arxiv.org/abs/1809.09078) — Xiao Liu, Zhunchen Luo, Heyan Huang. `EE` — [code](https://github.com/lx865712528/EMNLP2018-JMEE)
- [Graph Convolutional Networks With Argument-Aware Pooling for Event Detection](https://ojs.aaai.org/index.php/AAAI/article/view/12032) — Thien Huu Nguyen, Ralph Grishman. `ED`
- [Self-regulation: Employing a Generative Adversarial Network to Improve Event Detection](https://aclanthology.org/P18-1048/) — Yu Hong et al. `ED`
- [Collective Event Detection via Hierarchical and Bias Tagging Networks with Gated Multi-level Attention Mechanisms](https://aclanthology.org/D18-1158/) — Yubo Chen et al. `ED`
- [Prior Knowledge Integrated with Self-attention for Event Detection](https://link.springer.com/chapter/10.1007/978-3-030-01012-6_21) — Yan Li et al. `ED`
- [Neural Methods for Event Extraction](https://theses.hal.science/tel-01943841/) — Emanuela Boros. `thesis` `EE`

## 2019

- [Cost-sensitive Regularization for Label Confusion-aware Event Detection](https://aclanthology.org/P19-1521/) — Hongyu Lin et al. `ED`
- [Context Awareness and Embedding for Biomedical Event Extraction](https://academic.oup.com/bioinformatics/article/36/3/868/5544930) — Shankai Yan, Ka-Chun Wong. `EE`
- [Biomedical Event Extraction based on Knowledge-driven Tree-LSTM](https://aclanthology.org/N19-1145/) — Diya Li, Lifu Huang, Heng Ji, Jiawei Han. `EE`
- [Exploiting the Ground-Truth: An Adversarial Imitation Based Knowledge Distillation Approach for Event Detection](https://ojs.aaai.org/index.php/AAAI/article/view/4649) — Jian Liu, Yubo Chen, Kang Liu. `ED`
- [Joint Entity and Event Extraction with Generative Adversarial Imitation Learning](https://direct.mit.edu/dint/article/1/2/99/10019/) — Tongtao Zhang, Heng Ji, Avirup Sil. `EE`
- [Extracting Entities and Events as a Single Task Using a Transition-Based Neural Model](https://www.ijcai.org/proceedings/2019/753) — Junchi Zhang et al. `EE`
- [Distilling Discrimination and Generalization Knowledge for Event Detection via Delta-Representation Learning](https://aclanthology.org/P19-1429/) — Yaojie Lu et al. `ED`
- [Event Detection with Trigger-Aware Lattice Neural Network](https://aclanthology.org/D19-1033/) — Ning Ding et al. `ED`
- [HMEAE: Hierarchical Modular Event Argument Extraction](https://aclanthology.org/D19-1584/) — Xiaozhi Wang et al. `EAE`
- [Entity, Relation, and Event Extraction with Contextualized Span Representations](https://aclanthology.org/D19-1585/) — David Wadden et al. `EE` — [DyGIE++](https://github.com/dwadden/dygiepp)
- [Event Detection with Multi-Order Graph Convolution and Aggregated Attention](https://aclanthology.org/D19-1582/) — Haoran Yan et al. `ED`
- [GADGET: Using Gated GRU for Biomedical Event Trigger Detection](https://ieeexplore.ieee.org/document/8852355) — Cheng Zeng et al. `ED`

## 2020

- [Event Detection with Relation-Aware Graph Convolutional Neural Networks](https://arxiv.org/abs/2002.10757) — Shiyao Cui et al. `ED`
- [Biomedical Event Extraction with a Novel Combination Strategy Based on Hybrid Deep Neural Networks](https://bmcbioinformatics.biomedcentral.com/articles/10.1186/s12859-020-3376-2) — Lvxing Zhu, Haoran Zheng. `EE`
- [Improving Event Detection via Open-domain Trigger Knowledge](https://aclanthology.org/2020.acl-main.522/) — Meihan Tong et al. `ED`
- [Global Locality in Biomedical Relation and Event Extraction](https://aclanthology.org/2020.bionlp-1.21/) — Elaheh ShafieiBavani et al. `EE`
- [Towards Open Domain Event Trigger Identification using Adversarial Domain Adaptation](https://aclanthology.org/2020.acl-main.681/) — Aakanksha Naik, Carolyn Rosé. `ED`
- [Exploring Interpretability in Event Extraction: Multitask Learning of a Neural Event Classifier and an Explanation Decoder](https://aclanthology.org/2020.acl-srw.23/) — Zheng Tang, Gus Hahn-Powell, Mihai Surdeanu. `EE`
- [Event Detection: Gate Diversity and Syntactic Importance Scores for Graph Convolution Neural Networks](https://aclanthology.org/2020.emnlp-main.435/) — Viet Dac Lai et al. `ED`
- [Edge-Enhanced Graph Convolution Networks for Event Detection with Syntactic Relation](https://aclanthology.org/2020.findings-emnlp.211/) — Shiyao Cui et al. `ED`
- [Graph Transformer Networks with Syntactic and Semantic Structures for Event Argument Extraction](https://aclanthology.org/2020.findings-emnlp.326/) — Amir Pouran Ben Veyseh et al. `EAE`
- [Biomedical Event Extraction with Hierarchical Knowledge Graphs](https://aclanthology.org/2020.findings-emnlp.114/) — Kung-Hsiang Huang, Mu Yang, Nanyun Peng. `EE`
- [Resource-Enhanced Neural Model for Event Argument Extraction](https://aclanthology.org/2020.findings-emnlp.318/) — Jie Ma et al. `EAE`

## 2021

- [CLEVE: Contrastive Pre-training for Event Extraction](https://aclanthology.org/2021.acl-long.491/) — Ziqi Wang et al. `EE` `pretraining`
- [Unleash GPT-2 Power for Event Detection](https://aclanthology.org/2021.acl-long.490/) — Amir Pouran Ben Veyseh, Viet Dac Lai, Franck Dernoncourt, Thien Huu Nguyen. `ED` `PLM`
- [Event Detection as Question Answering with Entity Information](https://aclanthology.org/2021.ranlp-main.37/) — Emanuela Boros, Jose G. Moreno, Antoine Doucet. `ED` `QA` `zero-shot`
- [Trigger is Not Sufficient: Exploiting Frame-aware Knowledge for Implicit Event Argument Extraction](https://aclanthology.org/2021.acl-long.360/) — Kaiwen Wei et al. `EAE`

---

# Generative, Prompt-Based and LLM Event Extraction

This section covers models whose primary contribution is to formulate EE as generation, template filling, question answering/prompting, code generation, instruction following, or LLM reasoning.

## 2019

- [Exploring Pre-trained Language Models for Event Extraction and Generation](https://aclanthology.org/P19-1522/) — Sen Yang et al. `EE` `generation`

## 2020

- [Event Extraction by Answering (Almost) Natural Questions](https://aclanthology.org/2020.acl-main.202/) — Xinya Du, Claire Cardie. `EAE` `QA`
- [Event Extraction as Machine Reading Comprehension](https://aclanthology.org/2020.emnlp-main.128/) — Jian Liu et al. `EE` `MRC`
- [Event Extraction as Multi-turn Question Answering](https://aclanthology.org/2020.findings-emnlp.73/) — Fayuan Li et al. `EE` `QA`

## 2021

- [Text2Event: Controllable Sequence-to-Structure Generation for End-to-end Event Extraction](https://aclanthology.org/2021.acl-long.217/) — Yaojie Lu et al. `EE` `generation`  
  Introduces a sequence-to-structure formulation with constrained decoding for end-to-end event extraction.
- [Document-Level Event Argument Extraction by Conditional Generation](https://aclanthology.org/2021.naacl-main.69/) — Sha Li, Heng Ji, Jiawei Han. `EAE` `DEE` `generation`  
  Uses informative templates and conditional generation for arguments that may occur across sentences.

## 2022

- [DEGREE: A Data-Efficient Generation-Based Event Extraction Model](https://aclanthology.org/2022.naacl-main.138/) — I-Hung Hsu et al. `EE` `generation` `low-resource`  
  Uses event descriptions and natural-language templates to jointly support trigger and argument extraction.
- [Prompt for Extraction? PAIE: Prompting Argument Interaction for Event Argument Extraction](https://aclanthology.org/2022.acl-long.466/) — Yubo Ma et al. `EAE` `prompting` `DEE`  
  Uses event-role prompts and span selectors for sentence- and document-level argument extraction.
- [Dynamic Prefix-Tuning for Generative Template-based Event Extraction](https://aclanthology.org/2022.acl-long.358/) — Xiao Liu, Heyan Huang, Ge Shi, Bo Wang. `EE` `prefix-tuning`
- [Unified Structure Generation for Universal Information Extraction](https://aclanthology.org/2022.acl-long.395/) — Yaojie Lu et al. `EE` `UIE` `generation`  
  Unifies entities, relations, and events under a schema-driven text-to-structure generation framework.
- [Multilingual Generative Language Models for Zero-Shot Cross-Lingual Event Argument Extraction](https://aclanthology.org/2022.acl-long.317/) — Kuan-Hao Huang et al. `EAE` `generation` `cross-lingual`

## 2023

- [Code4Struct: Code Generation for Few-Shot Event Structure Prediction](https://aclanthology.org/2023.acl-long.202/) — Xingyao Wang, Sha Li, Heng Ji. `EAE` `LLM` `code generation` `few-shot`  
  Represents event ontologies as code structures and asks code-capable LLMs to instantiate them.
- [AMPERE: AMR-Aware Prefix for Generation-Based Event Argument Extraction Model](https://aclanthology.org/2023.acl-long.615/) — I-Hung Hsu et al. `EAE` `generation` `AMR`
- [Revisiting Event Argument Extraction: Can EAE Models Learn Better when Being Aware of Event Co-occurrences?](https://aclanthology.org/2023.acl-long.701/) — Yuxin He et al. `EAE` `TabEAE` `generation`
- [Contextualized Soft Prompts for Extraction of Event Arguments](https://aclanthology.org/2023.findings-acl.266/) — Chien Van Nguyen, Hieu Man, Thien Huu Nguyen. `EAE` `prompting`

## 2024

- [Thinking about How to Extract: Energizing LLMs' Emergence Capabilities for Document-Level Event Argument Extraction](https://aclanthology.org/2024.findings-acl.328/) — Kai Shuang, Ji Zhou, Qiwei Wang, Jinyu Guo. `LLM` `EAE` `DEE`  
  Studies reasoning-oriented LLM prompting for document-level event arguments.
- [ULTRA: Unleash LLMs' Potential for Event Argument Extraction through Hierarchical Modeling and Pair-wise Self-Refinement](https://aclanthology.org/2024.findings-acl.487/) — Xinliang Frederick Zhang et al. `LLM` `EAE`  
  Combines hierarchical processing, span-boundary support, and self-refinement.
- [LC4EE: LLMs as Good Corrector for Event Extraction](https://aclanthology.org/2024.findings-acl.715/) — Mengna Zhu et al. `LLM` `EE` `correction`  
  Uses LLMs as a correction layer over predictions from event extraction systems.
- [Demonstration Retrieval-Augmented Generative Event Argument Extraction](https://aclanthology.org/2024.lrec-main.412/) — Shuang He et al. `EAE` `generation` `retrieval`
- [Debate as Optimization: Adaptive Conformal Prediction and Diverse Retrieval for Event Extraction](https://aclanthology.org/2024.findings-emnlp.958/) — Sijia Wang, Lifu Huang. `LLM` `EE` `retrieval`
- [Revisiting Event Extraction to Capture Complex Arguments](https://aclanthology.org/2024.emnlp-main.673/) — Omar Sharif et al. `EAE` `LLM` `discourse`

## 2025

- [Instruction-Tuning LLMs for Event Extraction with Annotation Guidelines](https://aclanthology.org/2025.findings-acl.677/) — Saurabh Srivastava, Sweta Pati, Ziyu Yao. `LLM` `EE` `instruction tuning`  
  Incorporates event annotation guidelines directly into instruction tuning for trigger and argument extraction.
- [Towards Event Extraction with Massive Types: LLM-based Collaborative Annotation and Partitioning Extraction](https://aclanthology.org/2025.emnlp-main.1743/) — Wenxuan Liu et al. `LLM` `EE` `large ontology`  
  Targets extraction with very large event-type inventories using LLM-assisted annotation and type partitioning.
- [Adaptive Schema-aware Event Extraction with Retrieval-Augmented Generation](https://aclanthology.org/2025.findings-emnlp.419/) — Sheng Liang, Hang Lv, Zhihao Wen, Yaxiong Wu, Yongyue Zhang, Hao Wang, Yong Liu. `LLM` `RAG` `EE`
- [REAR: Reinforced Reasoning Optimization for Event Argument Extraction with Relation-Aware Support](https://aclanthology.org/2025.findings-emnlp.421/) — Jianwen Luo, Yu Hong, Shuai Yang, Jianmin Yao. `LLM` `EAE` `reinforcement learning`
- [Reflective Agreement: Combining Self-Mixture of Agents with a Sequence Tagger for Robust Event Extraction](https://aclanthology.org/2025.emnlp-main.1550/) — Fatemeh Haji, Mazal Bethany, Cho-Yu Jason Chiang, Anthony Rios, Peyman Najafirad. `LLM` `agents` `EE`
- [Exploring the Performance of Large Language Models for Event Extraction](https://aclanthology.org/2025.ranlp-1.143/) — Hristo Tanev et al. `LLM` `EE`
- [REGen: A Reliable Evaluation Framework for Generative Event Argument Extraction](https://aclanthology.org/2025.findings-emnlp.649/) — Omar Sharif, Joseph Gatto, Madhusudan Basak, Sarah Masud Preum. `EAE` `evaluation`

## 2026

- [When Tasks Share Structure: A Comparative Study of Training Strategies for Generative Event Extraction](https://aclanthology.org/2026.eeuca-1.5/) — Rishi Ravikumar, Riza Batista-Navarro. `LLM` `EE` `generation`
- [A Self-Reflective LLM-based Architecture for Semi-Open Event Extraction](https://aclanthology.org/2026.eeuca-1.8/) — Hristo Tanev, Michel de Bollivier, Bertrand De Longueville. `LLM` `OpenEE`
- [Boundary-Aware LLM Augmentation for Low-Resource Event Argument Extraction](https://aclanthology.org/2026.eacl-long.230/) — Zhaoyue Sun, Gabriele Pergola, Yulan He. `LLM` `EAE` `data augmentation` `low-resource`

---

# Few-Shot, Zero-Shot and Low-Resource Event Extraction

## 2015

- [Seed-Based Event Trigger Labeling: How Far Can Event Descriptions Get Us?](https://aclanthology.org/P15-2061/) — Ofer Bronstein et al. `ED` `minimal supervision`

## 2016

- [A Two-stage Approach for Extending Event Detection to New Types via Neural Networks](https://aclanthology.org/W16-1618/) — Thien Huu Nguyen et al. `ED` `new types`

## 2018

- [Zero-Shot Transfer Learning for Event Extraction](https://aclanthology.org/P18-1201/) — Lifu Huang et al. `EE` `zero-shot`

## 2019

- [Meta-Learning with Dynamic-Memory-Based Prototypical Network for Few-Shot Event Detection](https://arxiv.org/abs/1910.11621) — Shumin Deng et al. `ED` `few-shot`

## 2020

- [Towards Few-Shot Event Mention Retrieval: An Evaluation Framework and a Siamese Network Approach](https://aclanthology.org/2020.lrec-1.216/) — Bonan Min, Yee Seng Chan, Lingjun Zhao. `few-shot`
- [Extensively Matching for Few-shot Learning Event Detection](https://aclanthology.org/2020.nuse-1.5/) — Viet Dac Lai, Thien Huu Nguyen, Franck Dernoncourt. `ED`
- [Exploiting the Matching Information in the Support Set for Few Shot Event Classification](https://arxiv.org/abs/2002.05295) — Viet Dac Lai, Franck Dernoncourt, Thien Huu Nguyen. `ED`

## 2023

- [Few-shot Event Detection: An Empirical Study and a Unified View](https://aclanthology.org/2023.acl-long.628/) — Yubo Ma, Zehao Wang, Yixin Cao, Aixin Sun. `ED` `few-shot`
- [Few-Shot Document-Level Event Argument Extraction](https://aclanthology.org/2023.acl-long.446/) — Xianjun Yang, Yujie Lu, Linda Petzold. `EAE` `DEE` `few-shot`

## 2025

- [How do LLMs' Preferences Affect Event Argument Extraction? CAT: Addressing Preference Traps in Unsupervised EAE](https://aclanthology.org/2025.findings-acl.1000/) — Yunhao Wei, Kai Shuang, Zhiyi Li, Chenrui Mao. `LLM` `EAE` `unsupervised`
- [Document-Level Event-Argument Data Augmentation for Few-Shot Cross-Domain Learning](https://aclanthology.org/2025.acl-long.1221/) — Joseph Gatto et al. `LLM` `EAE` `DEE` `augmentation`
- [Rule-Guided Extraction: A Hierarchical Rule Optimization Framework for Document-Level Event Argument Extraction](https://aclanthology.org/2025.findings-emnlp.1154/) — Yue Zuo, Yuxiao Fei, Wanting Ning, Jiayi Huang, Yubo Feng, Lishuang Li. `LLM` `EAE` `ICL`

---

# Document-Level and Cross-Document Event Extraction

## 2008

- [Refining Event Extraction through Cross-Document Inference](https://aclanthology.org/P08-1030/) — Heng Ji, Ralph Grishman. `EE` `CDEE`

## 2010

- [Using Document Level Cross-Event Inference to Improve Event Extraction](https://aclanthology.org/P10-1081/) — Shasha Liao, Ralph Grishman. `EE` `DEE`

## 2012

- [Modeling Textual Cohesion for Event Extraction](https://ojs.aaai.org/index.php/AAAI/article/view/8341) — Ruihong Huang, Ellen Riloff. `EE` `discourse`

## 2013

- [Argument Inference from Relevant Event Mentions in Chinese Argument Extraction](https://aclanthology.org/P13-1145/) — Peifeng Li et al. `EAE` `DEE`

## 2016

- [Incremental Global Event Extraction](https://aclanthology.org/C16-1215/) — Alex Judea, Michael Strube. `EE` `DEE`
- [Joint Extraction of Events and Entities within a Document Context](https://aclanthology.org/N16-1033/) — Bishan Yang, Tom M. Mitchell. `EE` `DEE`

## 2017

- [Exploiting Document Level Information to Improve Event Detection via Recurrent Neural Networks](https://aclanthology.org/I17-1036/) — Shaoyang Duan et al. `ED` `DEE`

## 2018

- [Document Embedding Enhanced Event Detection with Hierarchical and Supervised Attention](https://aclanthology.org/P18-2066/) — Yue Zhao et al. `ED` `DEE`

## 2019

- [Doc2EDAG: An End-to-End Document-level Framework for Chinese Financial Event Extraction](https://aclanthology.org/D19-1032/) — Shun Zheng, Wei Cao, Wei Xu, Jiang Bian. `DEE` `financial`

## 2020

- [A Two-Step Approach for Implicit Event Argument Detection](https://aclanthology.org/2020.acl-main.667/) — Zhisong Zhang et al. `EAE` `cross-sentence`
- [Document-Level Event Role Filler Extraction using Multi-Granularity Contextualized Encoding](https://aclanthology.org/2020.acl-main.714/) — Xinya Du, Claire Cardie. `DEE`

## 2021

- [Document-Level Event Extraction via Heterogeneous Graph-Based Interaction Model with a Tracker](https://aclanthology.org/2021.acl-long.274/) — Runxin Xu et al. `DEE`
- [Document-level Event Extraction via Parallel Prediction Networks](https://aclanthology.org/2021.acl-long.492/) — Hang Yang et al. `DEE`

## 2022

- [A Two-Stream AMR-enhanced Model for Document-level Event Argument Extraction](https://aclanthology.org/2022.naacl-main.366/) — Runxin Xu et al. `EAE` `DEE` `AMR`
- [CLIO: Role-interactive Multi-event Head Attention Network for Document-level Event Extraction](https://aclanthology.org/2022.coling-1.221/) — Yubing Ren et al. `DEE`

## 2023

- [Retrieve-and-Sample: Document-level Event Argument Extraction via Hybrid Retrieval Augmentation](https://aclanthology.org/2023.acl-long.17/) — Yubing Ren et al. `EAE` `DEE` `retrieval`
- [Enhancing Document-level Event Argument Extraction with Contextual Clues and Role Guidance](https://aclanthology.org/2023.findings-acl.817/) — Wei Liu et al. `EAE` `DEE`

## 2024

- [Harvesting Events from Multiple Sources: Towards a Cross-Document Event Extraction Paradigm](https://aclanthology.org/2024.findings-acl.114/) — Qiang Gao et al. `CDEE`
- [CMNEE: A Large-Scale Document-Level Event Extraction Dataset Based on Open-Source Chinese Military News](https://aclanthology.org/2024.lrec-main.299/) — Mengna Zhu, Zijie Xu, Kaisheng Zeng, Kaiming Xiao, Mao Wang, Wenjun Ke, Hongbin Huang. `DEE` `dataset` `Chinese`
- [Beyond Single-Event Extraction: Towards Efficient Document-Level Multi-Event Argument Extraction](https://aclanthology.org/2024.findings-acl.564/) — Wanlong Liu, Li Zhou, DingYi Zeng, Yichen Xiao, Shaohuan Cheng, Chen Zhang, Grandee Lee, Malu Zhang, Wenyu Chen. `EAE` `DEE` `multi-event`

## 2025

- [Multi-Document Event Extraction Using Large and Small Language Models](https://aclanthology.org/2025.emnlp-main.972/) — Qingkai Min et al. `CDEE` `LLM`

---

# Multilingual and Cross-Lingual Event Extraction

## 2009

- [Can One Language Bootstrap the Other: A Case Study on Event Extraction](https://aclanthology.org/W09-2209/) — Zheng Chen, Heng Ji. `EE` `cross-lingual`

## 2014

- [Bilingual Event Extraction: A Case Study on Trigger Type Determination](https://aclanthology.org/P14-2136/) — Zhu Zhu, Shoushan Li, Guodong Zhou, Rui Xia. `ED`

## 2015

- [Modeling Event Extraction via Multilingual Data Sources](https://www.semanticscholar.org/paper/Modeling-Event-Extraction-via-Multilingual-Data-Hsi-Carbonell/fabcbadcb824a7bbe51f21a8492f9ba234cb695d) — Andrew Hsi, Jaime G. Carbonell, Yiming Yang. `EE`

## 2016

- [Leveraging Multilingual Training for Limited Resource Event Extraction](https://aclanthology.org/C16-1114/) — Andrew Hsi et al. `EE`
- [A Language-Independent Neural Network for Event Detection](https://aclanthology.org/P16-2011/) — Xiaocheng Feng et al. `ED`

## 2018

- [Event Detection via Gated Multilingual Attention Mechanism](https://ojs.aaai.org/index.php/AAAI/article/view/12022) — Jian Liu et al. `ED`

## 2019

- [Cross-lingual Structure Transfer for Relation and Event Extraction](https://aclanthology.org/D19-1030/) — Ananya Subburathinam et al. `EE`
- [Neural Cross-Lingual Event Detection with Minimal Parallel Resources](https://aclanthology.org/D19-1068/) — Jian Liu et al. `ED`

## 2020

- [Cross-lingual Structure Transfer for Zero-resource Event Extraction](https://aclanthology.org/2020.lrec-1.243/) — Di Lu et al. `EE` `zero-resource`
- [A Platform for Event Extraction in Hindi](https://aclanthology.org/2020.lrec-1.273/) — Sovan Kumar Sahoo et al. `EE` `Hindi`
- [Event Extraction from Unstructured Amharic Text](https://aclanthology.org/2020.lrec-1.258/) — Ephrem Tadesse et al. `EE` `Amharic`

## 2026

- [A Dual-View Analysis of Multiple Languages in Colonial Newspapers](https://aclanthology.org/2026.findings-acl.1029/) — Zhan Su, Xiaoya Chen, Fengran Mo, Ida L. Vos, Prayag Tiwari, Yazhou Zhang, Qian Zheng, Natália da Silva Perez. `EE` `historical documents` `multilingual` `VQA`

---

# Multimodal Event Extraction

## 2016

- [Cross-media Event Extraction and Recommendation](https://aclanthology.org/N16-3015/) — Di Lu et al. `MEE`
- [Event Specific Multimodal Pattern Mining for Knowledge Base Construction](https://dl.acm.org/doi/10.1145/2964284.2964287) — Hongzhi Li et al. `MEE` `schema induction`

## 2017

- [Improving Event Extraction via Multimodal Integration](https://dl.acm.org/doi/10.1145/3123266.3123294) — Tongtao Zhang et al. `MEE`

## 2020

- [Cross-media Structured Common Space for Multimedia Event Extraction](https://aclanthology.org/2020.acl-main.230/) — Manling Li et al. `MEE`
- [Image Enhanced Event Detection in News Articles](https://ojs.aaai.org/index.php/AAAI/article/view/6437) — Meihan Tong et al. `ED` `multimodal`

## 2021

- [Joint Multimedia Event Extraction from Video and Article](https://aclanthology.org/2021.findings-emnlp.8/) — Brian Chen et al. `MEE` `video` `text`

## 2025

- [Multimedia Event Extraction with LLM Knowledge Editing](https://aclanthology.org/2025.emnlp-main.205/) — Jing Yu et al. `MEE` `LLM`

## 2026

- [CVRH: Cross-modal Variational Role Hypergraph Network via Semantic Enhancement for Multi-modal Event Argument Extraction](https://aclanthology.org/2026.findings-acl.978/) — Bangze Pan et al. `MEE` `EAE`

---

# Semi-Supervised, Weakly Supervised and Unsupervised Learning

## 1998

- [A Study on Retrospective and On-line Event Detection](https://dl.acm.org/doi/10.1145/290941.290953) — Yiming Yang, Tom Pierce, Jaime Carbonell. `event discovery`

## 2001

- [Combining Semantic and Syntactic Document Classifiers to Improve First Story Detection](https://dl.acm.org/doi/10.1145/383952.384068) — Nicola Stokes, Joe Carthy. `event detection`

## 2003

- [Ontology-based Fuzzy Event Extraction Agent for Chinese E-news Summarization](https://www.sciencedirect.com/science/article/pii/S0957417403000629) — Chang-Shing Lee et al. `EE`

## 2004

- [Event Threading within News Topics](https://ciir-publications.cs.umass.edu/getpdf.php?id=390) — Ramesh Nallapati et al. `event discovery`

## 2011

- [Can Document Selection Help Semi-supervised Learning? A Case Study On Event Extraction](https://aclanthology.org/P11-2045/) — Shasha Liao, Ralph Grishman. `EE`
- [Using Prediction from Sentential Scope to Build a Pseudo Co-Testing Learner for Event Extraction](https://aclanthology.org/I11-1080/) — Shasha Liao, Ralph Grishman. `EE` `active learning`
- [Event Discovery in Social Media Feeds](https://aclanthology.org/P11-1040/) — Edward Benson, Aria Haghighi, Regina Barzilay. `unsupervised`

## 2012

- [Automatic Event Extraction with Structured Preference Modeling](https://aclanthology.org/P12-1088/) — Wei Lu, Dan Roth. `EE` `unsupervised`

## 2013

- [Semi-supervised Method for Biomedical Event Extraction](https://pubmed.ncbi.nlm.nih.gov/24565105/) — Wang et al. `EE`
- [Wide Coverage Biomedical Event Extraction Using Multiple Partially Overlapping Corpora](https://bmcbioinformatics.biomedcentral.com/articles/10.1186/1471-2105-14-175) — Makoto Miwa et al. `EE`

## 2014

- [Event Extraction Using Distant Supervision](https://aclanthology.org/L14-1091/) — Kevin Reschke et al. `EE`

## 2017

- [Automatically Labeled Data Generation for Large Scale Event Extraction](https://aclanthology.org/P17-1038/) — Yubo Chen et al. `EE`
- [Scale Up Event Extraction Learning via Automatic Training Data Generation](https://arxiv.org/abs/1712.03665) — Ying Zeng et al. `EE`

## 2018

- [Semi-Supervised Event Extraction with Paraphrase Clusters](https://aclanthology.org/N18-2058/) — James Ferguson et al. `EE`

## 2019

- [Adversarial Training for Weakly Supervised Event Detection](https://aclanthology.org/N19-1105/) — Xiaozhi Wang et al. `ED`
- [Financial Event Extraction Using Wikipedia-Based Weak Supervision](https://aclanthology.org/D19-5102/) — Liat Ein-Dor et al. `EE`

## 2020

- [Semi-supervised New Event Type Induction and Event Detection](https://aclanthology.org/2020.emnlp-main.53/) — Lifu Huang, Heng Ji. `ED` `type induction`
- [Weakly Supervised Subevent Knowledge Acquisition](https://aclanthology.org/2020.emnlp-main.430/) — Wenlin Yao et al. `subevents`

---

# Open-Domain Event Extraction and Schema Induction

## 2012

- [Skip N-grams and Ranking Functions for Predicting Script Events](https://aclanthology.org/E12-1034/) — Bram Jans et al. `scripts`

## 2014

- [Unsupervised Techniques for Extracting and Clustering Complex Events in News](https://aclanthology.org/W14-2905/) — Delia Rusu et al. `OpenEE`
- [Modelling Events through Memory-based, Open-IE Patterns for Abstractive Summarization](https://aclanthology.org/P14-1084/) — Daniele Pighin et al. `OpenEE`

## 2015

- [Generative Event Schema Induction with Entity Disambiguation](https://aclanthology.org/P15-1019/) — Kiem-Hieu Nguyen et al. `schema induction`
- [Storybase: Towards Building a Knowledge Base for News Events](https://aclanthology.org/P15-4023/) — Zhaohui Wu, Chen Liang, C. Lee Giles. `event KB`

## 2016

- [Liberal Event Extraction and Event Schema Induction](https://aclanthology.org/P16-1025/) — Lifu Huang et al. `OpenEE` `schema induction`

## 2018

- [Open-domain Event Detection using Distant Supervision](https://aclanthology.org/C18-1075/) — Jun Araki, Teruko Mitamura. `OpenEE`

## 2019

- [Open Event Extraction from Online Text using a Generative Adversarial Network](https://aclanthology.org/D19-1027/) — Rui Wang, Deyu Zhou, Yulan He. `OpenEE`
- [Open Domain Event Extraction Using Neural Latent Variable Models](https://github.com/lx865712528/ACL2019-ODEE) — Xiao Liu et al. `OpenEE`

## 2020

- [Connecting the Dots: Event Graph Schema Induction with Path Language Modeling](https://aclanthology.org/2020.emnlp-main.50/) — Manling Li et al. `schema induction`

---

# Event Coreference

## 1997

- [Event Coreference for Information Extraction](https://aclanthology.org/W97-1311/) — Kevin Humphreys, Robert Gaizauskas, Saliha Azzam. `ECR`

## 2007

- [Unrestricted Coreference: Identifying Entities and Events in OntoNotes](https://ieeexplore.ieee.org/document/4338380) — Sameer S. Pradhan et al. `ECR`

## 2008

- [A Linguistic Resource for Discovering Event Structures and Resolving Event Coreference](http://www.lrec-conf.org/proceedings/lrec2008/pdf/734_paper.pdf) — Cosmin Adrian Bejan, Sanda M. Harabagiu. `ECR`

## 2009

- [Nonparametric Bayesian Models for Unsupervised Event Coreference Resolution](https://proceedings.neurips.cc/paper/2009/hash/70fcb77e6349f4467edd7227baa73222-Abstract.html) — Cosmin Adrian Bejan et al. `ECR`
- [Graph-based Event Coreference Resolution](https://aclanthology.org/W09-3208/) — Zheng Chen, Heng Ji. `ECR`
- [A Pairwise Event Coreference Model, Feature Impact and Evaluation for Event Coreference Resolution](https://aclanthology.org/W09-4303/) — Zheng Chen, Heng Ji, Robert Haralick. `ECR`

## 2010

- [Unsupervised Event Coreference Resolution with Rich Linguistic Features](https://aclanthology.org/P10-1145/) — Cosmin Adrian Bejan, Sanda M. Harabagiu. `ECR`

## 2011

- [A Unified Event Coreference Resolution by Integrating Multiple Resolvers](https://aclanthology.org/I11-1012/) — Bin Chen et al. `ECR`

## 2012

- [Joint Entity and Event Coreference Resolution across Documents](https://aclanthology.org/D12-1045/) — Heeyoung Lee et al. `ECR` `cross-document`
- [Improving Event Co-reference by Context Extraction and Dynamic Feature Weighting](https://ieeexplore.ieee.org/document/6188406) — Katie McConky et al. `ECR`

## 2013

- [A Structured Distributional Semantic Model for Event Co-reference](https://aclanthology.org/P13-2083/) — Kartik Goyal et al. `ECR`

## 2014

- [Evaluation for Partial Event Coreference](https://aclanthology.org/W14-2910/) — Jun Araki, Eduard Hovy, Teruko Mitamura. `ECR` `evaluation`
- [Unsupervised Event Coreference Resolution](https://aclanthology.org/J14-2004/) — Cosmin Adrian Bejan, Sanda Harabagiu. `ECR`
- [SinoCoreferencer: An End-to-End Chinese Event Coreference Resolver](https://aclanthology.org/L14-1099/) — Chen Chen, Vincent Ng. `ECR` `Chinese`
- [Supervised Within-Document Event Coreference using Information Propagation](https://aclanthology.org/L14-1513/) — Zhengzhong Liu, Jun Araki, Eduard Hovy, Teruko Mitamura. `ECR`

## 2015

- [Chinese Event Coreference Resolution: An Unsupervised Probabilistic Model Rivaling Supervised Resolvers](https://aclanthology.org/N15-1116/) — Chen Chen, Vincent Ng. `ECR`
- [Translating Granularity of Event Slots into Features for Event Coreference Resolution](https://aclanthology.org/W15-0801/) — Agata Cybulska, Piek Vossen. `ECR`
- [A Hierarchical Distance-dependent Bayesian Model for Event Coreference Resolution](https://aclanthology.org/Q15-1037/) — Bishan Yang, Claire Cardie, Peter Frazier. `ECR`
- [Cross-document Event Coreference Resolution based on Cross-media Features](https://aclanthology.org/D15-1020/) — Tongtao Zhang et al. `ECR` `multimodal`

## 2016

- [Joint Inference for Event Coreference Resolution](https://aclanthology.org/C16-1308/) — Jing Lu et al. `ECR`
- [Joint Inference over a Lightly Supervised Information Extraction Pipeline](https://aclanthology.org/D16-1208/) — Chen Chen, Vincent Ng. `ECR`
- [Event Coreference Resolution with Multi-Pass Sieves](https://aclanthology.org/L16-1631/) — Jing Lu, Vincent Ng. `ECR`

## 2017

- [Event Coreference Resolution by Iteratively Unfolding Inter-dependencies among Events](https://aclanthology.org/D17-1226/) — Prafulla Kumar Choubey, Ruihong Huang. `ECR`
- [Joint Learning for Event Coreference Resolution](https://aclanthology.org/P17-1009/) — Jing Lu, Vincent Ng. `ECR`
- [Learning Antecedent Structures for Event Coreference Resolution](https://ieeexplore.ieee.org/document/8260622) — Jing Lu, Vincent Ng. `ECR`

---

# Event Relations, Temporal Structure and Causality

## 2009

- [Predicting Unknown Time Arguments Based on Cross-Event Propagation](https://dl.acm.org/doi/10.1145/1667583.1667697) — Prashant Gupta, Heng Ji. `temporal`

## 2014

- [An Annotation Framework for Dense Event Ordering](https://aclanthology.org/P14-2082/) — Taylor Cassidy et al. `temporal`
- [Cross-narrative Temporal Ordering of Medical Events](https://aclanthology.org/P14-1094/) — Preethi Raghavan et al. `temporal`
- [Toward Future Scenario Generation: Extracting Event Causality Exploiting Semantic Relation, Context, and Association Features](https://aclanthology.org/P14-1093/) — Chikara Hashimoto et al. `causality`

## 2016

- [Building a Cross-document Event-Event Relation Corpus](https://aclanthology.org/W16-1701/) — Yu Hong et al. `event-event relations`
- [Temporal Anchoring of Events for the TimeBank Corpus](https://aclanthology.org/P16-1207/) — Nils Reimers, Nazanin Dehghani, Iryna Gurevych. `temporal`

## 2017

- [The Rich Event Ontology](https://aclanthology.org/W17-2712/) — Susan Brown, Claire Bonial, Leo Obrst, Martha Palmer. `ontology` `event relations`

## 2019

- [Joint Event and Temporal Relation Extraction with Shared Representations and Structured Prediction](https://aclanthology.org/D19-1041/) — Rujun Han, Qiang Ning, Nanyun Peng. `temporal`
- [Detecting Subevents using Discourse and Narrative Features](https://aclanthology.org/P19-1471/) — Mohammed Aldawsari, Mark Finlayson. `subevents`

## 2020

- [Domain Knowledge Empowered Structured Neural Net for End-to-End Event Temporal Relation Extraction](https://arxiv.org/abs/2009.07373) — Rujun Han, Yichao Zhou, Nanyun Peng. `temporal`
- [Severing the Edge Between Before and After: Neural Architectures for Temporal Ordering of Events](https://aclanthology.org/2020.emnlp-main.436/) — Miguel Ballesteros et al. `temporal`

---

# Surveys and Evaluation Studies

- [An Overview of Event Extraction from Text](http://ceur-ws.org/Vol-779/derive2011_submission_1.pdf) — Frederik Hogenboom et al.
- [A Survey of Techniques for Event Detection in Twitter](https://onlinelibrary.wiley.com/doi/10.1111/coin.12017) — Farzindar Atefeh, Wael Khreich.
- [A Survey of Event Extraction Methods from Text for Decision Support Systems](https://www.sciencedirect.com/science/article/pii/S0167923616300173) — Frederik Hogenboom et al.
- [A Survey of Open Domain Event Extraction](https://pdfs.semanticscholar.org/0eef/643c744ac3e4ffd68d4328b5f445dbf9e10e.pdf) — Zecheng Zhang, Yuncheng Wu, Zesheng Wang.
- [A Survey of Textual Event Extraction from Social Networks](https://www.semanticscholar.org/paper/A-Survey-of-Textual-Event-Extraction-from-Social-Mejri-Akaichi/2ed13ebbad66c3a8599dd9aa7c20fbdaaee22b11) — Mohamed Mejri, Jalel Akaichi.
- [Survey on Event Extraction Technology in Information Extraction Research Area](https://ieeexplore.ieee.org/document/8729158) — Liying Zhan, Xuping Jiang.
- [A Survey of Event Extraction From Text](https://ieeexplore.ieee.org/document/8918013) — Wei Xiang, Bang Wang.
- [On the Pitfalls of Event Extraction Evaluation](https://aclanthology.org/2023.findings-acl.586/) — Haoyu Peng, Xiaozhi Wang, Feng Yao et al.  
  Highlights preprocessing, evaluation, and reproducibility discrepancies in EE.
- [Generative Approaches to Event Extraction: Survey and Outlook](https://aclanthology.org/2024.futured-1.7/) — Émilie Simon et al.  
  Reviews the transition from discriminative extraction to generative and template-based paradigms.
- [TEXTEE: Benchmark, Reevaluation, Reflections, and Future Challenges in Event Extraction](https://aclanthology.org/2024.findings-acl.760/) — Kuan-Hao Huang et al.  
  Provides standardized preprocessing, evaluation, and implementations across a broad collection of EE datasets and models.
- [Evaluation Pitfalls and Challenges in Multimedia Event Extraction](https://aclanthology.org/2026.acl-long.1426/) — Philipp Seeberger et al. `MEE`

---

# Datasets and Benchmarks

## General Event Extraction

- [MUC Data Sets](https://www-nlpir.nist.gov/related_projects/muc/muc_data/muc_data_index.html)
- [ACE Program](https://www.ldc.upenn.edu/collaborations/past-projects/ace)
- [ACE-2 Corpus](https://catalog.ldc.upenn.edu/LDC2003T11)
- [ACE 2005 Corpus](https://catalog.ldc.upenn.edu/LDC2006T06)
- [Light & Rich ERE](https://aclanthology.org/W15-0812/)
- [TAC KBP 2015 Event Track](https://tac.nist.gov/2015/KBP/Event/index.html)
- [MAVEN: A Massive General Domain Event Detection Dataset](https://aclanthology.org/2020.emnlp-main.129/) — 4,480 Wikipedia documents, 118k+ event mentions, 168 event types in the final benchmark release.
- [GENEVA: Benchmarking Generalizability for Event Argument Extraction](https://aclanthology.org/2023.acl-long.203/) — hundreds of event types and argument roles.
- [MAVEN-ARG](https://aclanthology.org/2024.acl-long.224/) — event argument annotations extending large-scale event understanding resources.
- [TEXTEE](https://aclanthology.org/2024.findings-acl.760/) — standardized benchmark/evaluation suite spanning many EE datasets.

## Document-Level Event Extraction

- [Roles Across Multiple Sentences (RAMS)](https://nlp.jhu.edu/rams/)
- [WikiEvents](https://aclanthology.org/2021.naacl-main.69/) — document-level event arguments and coreference-oriented annotations.
- [FewDocAE](https://aclanthology.org/2023.acl-long.446/) — few-shot document-level EAE benchmark.
- [CMNEE](https://aclanthology.org/2024.lrec-main.299/) — large-scale document-level event extraction.
- [DEIE: Benchmarking Document-level Event Information Extraction](https://aclanthology.org/2024.lrec-main.410/)

## Event Coreference and Event Relations

- [ECB+ Corpus](https://www.newsreader-project.eu/results/data/the-ecb-corpus/)
- [NewsReader MEANTIME Corpus](https://www.newsreader-project.eu/results/data/wikinews/)
- [OntoNotes Release 5.0](https://catalog.ldc.upenn.edu/LDC2013T19)
- [Richer Event Description](https://catalog.ldc.upenn.edu/LDC2016T23)
- [EventStatus Corpus](https://catalog.ldc.upenn.edu/LDC2017T09)

## Temporal Event Resources

- [TimeBank 1.2](https://catalog.ldc.upenn.edu/LDC2006T08)
- [AQUAINT TimeML](https://github.com/cnorthwood/ternip/tree/master/sample_data/aquaint_timeml_1.0)
- [TempEval-3](https://www.cs.york.ac.uk/semeval-2013/task1/)
- [FactBank 1.0](https://catalog.ldc.upenn.edu/LDC2009T23)

## Semantic and Structural Resources

- [FrameNet](https://framenet.icsi.berkeley.edu/)
- [NomBank v1.0](https://catalog.ldc.upenn.edu/LDC2008T23)
- [PropBank](https://catalog.ldc.upenn.edu/LDC2004T14)
- [Treebank-3](https://catalog.ldc.upenn.edu/LDC99T42)
- [Abstract Meaning Representation Annotation](https://catalog.ldc.upenn.edu/LDC2014T12)

## Biomedical

- [Multi-Level Event Extraction (MLEE)](http://nactem.ac.uk/MLEE/)
- BioNLP Shared Task corpora (GENIA, Infectious Diseases, Epigenetics and related event datasets)

## Domain-Specific and Multilingual

- [CASIE: Cybersecurity Event Information](https://github.com/Ebiquity/CASIE)
- [A French Corpus for Event Detection on Twitter / Event2018](https://aclanthology.org/2020.lrec-1.763/)
- [A Dataset for Multi-lingual Epidemiological Event Extraction](https://aclanthology.org/2020.lrec-1.509/)
- [FloDusTA: Saudi Tweets Dataset for Flood, Dust Storm, and Traffic Accident Events](https://aclanthology.org/2020.lrec-1.174/)
- [Manovaad](https://aclanthology.org/2020.lrec-1.609/)
- [Cybersecurity Event Detection Dataset](https://aclanthology.org/2020.emnlp-main.433/)
- [COVID-19 Twitter Event Corpus](https://github.com/viczong/extract_COVID19_events_from_Twitter)
- [SentiFM Company-specific Economic News Event Dataset](https://osf.io/enu2k/)
- [SciEvent](https://aclanthology.org/2025.emnlp-main.871/) — scientific-domain event extraction.

---

# Tools and Repositories

- [OmniEvent](https://github.com/THU-KEG/OmniEvent) — event extraction toolkit and standardized implementations.
- [TEXTEE](https://github.com/ej0cl6/TextEE) — standardized event extraction benchmark/toolkit.
- [NewsReader](http://www.newsreader-project.eu/results/software/) — event-centric NLP pipeline components.
- [FRED](http://wit.istc.cnr.it/stlab-tools/fred/) — machine reading and linked-data generation.
- [Turku Event Extraction System (TEES)](https://github.com/jbjorne/TEES) — biomedical event and relation extraction.
- [bert-event-extraction](https://github.com/nlpcl-lab/bert-event-extraction) — BERT-based ACE 2005 event extraction.
- [ACE2005 preprocessing](https://github.com/nlpcl-lab/ace2005-preprocessing)
- [Transformer-based pretrained model for event extraction](https://github.com/Hanlard/Transformer-based-pretrained-model-for-event-extraction)
- [EventMiner](https://github.com/hltcoe/EventMiner)
- [JMEE](https://github.com/lx865712528/EMNLP2018-JMEE)
- [Open Domain Event Extraction Using Neural Latent Variable Models](https://github.com/lx865712528/ACL2019-ODEE)
- [CMU Multilingual Event Extractor](https://github.com/ahsi/Multilingual_Event_Extraction)
- [DyGIE++](https://github.com/dwadden/dygiepp)
- [Zero-Shot Event Extraction](https://github.com/wilburOne/ZeroShotEvent)
- [Incremental Event Detection](https://github.com/CPF-NLPR/IncrementalED)
- [Image Enhanced Event Extraction](https://github.com/shuaiwa16/image-enhanced-event-extraction)
- [EE as MRC](https://github.com/jianliu-ml/EEasMRC)
- [TabEAE](https://github.com/Stardust-hyx/TabEAE)
- [GEANet Biomedical Event Extraction](https://github.com/PlusLabNLP/GEANet-BioMed-Event-Extraction)

---

# Linguistic Foundations

These works are not necessarily computational event extraction papers, but they provide important linguistic and semantic foundations for defining events, event structure, aspect, telicity, and temporal reference.

1. [Verbs and Times](http://semantics.uchicago.edu/scalarchange/vendler57.pdf) — Zeno Vendler.
2. [Events, Processes, and States](https://user.phil.hhu.de/~filip/Mourelatos%2078:81.PDF) — Alexander P. D. Mourelatos.
3. [Aspect and Quantification](https://brill.com/view/book/edcoll/9789004373112/BP000004.xml) — Lauri Carlson.
4. [The Algebra of Events](https://www.researchgate.net/publication/226895496_The_Algebra_of_Events) — Emmon Bach.
5. [Temporal Ontology and Temporal Reference](https://aclanthology.org/J88-2003/) — Marc Moens, Mark Steedman.
6. [Aspectual Shift as Type Coercion](https://onlinelibrary.wiley.com/doi/abs/10.1111/1467-968X.00020) — Stephen G. Pulman.
7. [Events as Grammatical Objects](https://press.uchicago.edu/ucp/books/book/distributed/E/bo3645761.html) — Carol L. Tenny, James Pustejovsky (eds.).
8. [The Origins of Telicity](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.550.9185&rep=rep1&type=pdf) — Manfred Krifka.
9. [The Syntax of Event Structure](https://www.cs.rochester.edu/u/james/Papers/Pustejovsky-event-structure.pdf) — James Pustejovsky.
10. [Four Thousand Ships Passed Through the Lock](http://semantics.uchicago.edu/kennedy/classes/s07/events/krifka90.pdf) — Manfred Krifka.
11. [Nominal Reference, Temporal Constitution and Quantification in Event Semantics](https://pdfs.semanticscholar.org/aa5a/5634bca33fab72c287b9594d6bbe2b0593ee.pdf) — Manfred Krifka.
12. [Event Structures in Linguistic Form and Interpretation](https://www.degruyter.com/document/doi/10.1515/9783110925449/html) — Johannes Dölling, Tatjana Heyde-Zybatow, Martin Schäfer.
13. [Time in Language, Language in Time](https://www.researchgate.net/publication/290107347_Time_in_Language_Language_in_Time) — Wolfgang Klein.

---

# Other Lists

- [DL_EventExtractionPapers](https://github.com/carrie0307/DL_EventExtractionPapers)
- [event-extraction-paper](https://github.com/ll0iecas/event-extraction-paper)
- [KG-NLP-Papers](https://github.com/Clearailhc/KG-NLP-Papers)

---

# Contributing

Contributions are welcome.

When adding a paper:

1. Prefer the **ACL Anthology, publisher, DOI, or official project page** over secondary mirrors.
2. Place the paper in the category corresponding to its **main methodological contribution**.
3. Add cross-cutting properties as tags rather than duplicating the paper across sections.
4. Use the following format:

```markdown
- [Paper Title](URL) — Author One, Author Two. `EE` `document-level` `LLM`
  Optional one-sentence description of the main contribution.
```

For recent papers, please include a short contribution summary. For historical papers, title, authors, link, and tags are sufficient.

---

## Citation / maintenance note

Event extraction has accumulated several partially overlapping task definitions: event detection, trigger classification, argument extraction, template filling, document-level event extraction, open-domain extraction, event coreference, temporal relations, and multimedia event understanding. The categories above therefore reflect the **primary research contribution** of each work rather than mutually exclusive task definitions.
