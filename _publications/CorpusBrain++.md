---
title: "CorpusBrain++: A Continual Generative Pre-Training Framework for Knowledge-Intensive Language Tasks"
collection: publications
permalink: /publication/2009-10-01-paper-title-number-1
excerpt: 'Continual learning of generative retrieval models for knowledge-intensive language tasks.'
date: 2024-2-26
venue: 'Submitted to ACM TOIS (under review)'
paperurl: 'https://arxiv.org/pdf/2402.16767'
citation: '@article{guo2024corpusbrain++,
  title={CorpusBrain++: A Continual Generative Pre-Training Framework for Knowledge-Intensive Language Tasks},
  author={Guo, Jiafeng and Zhou, Changjiang and Zhang, Ruqing and Chen, Jiangui and de Rijke, Maarten and Fan, Yixing and Cheng, Xueqi},
  journal={arXiv preprint arXiv:2402.16767},
  year={2024}
}'
---

Knowledge-intensive language tasks (KILTs) typically require retrieving relevant documents from trustworthy corpora, e.g., Wikipedia, to produce specific answers. Very recently, a pre-trained generative retrieval model for KILTs, named CorpusBrain, was proposed and reached new state-of-the-art retrieval performance. However, most existing research on KILTs, including CorpusBrain, has predominantly focused on a static document collection, overlooking the dynamic nature of real-world scenarios, where new documents are continuously being incorporated into the source corpus. To address this gap, it is crucial to explore the capability of retrieval models to effectively handle the dynamic retrieval scenario inherent in KILTs. 

In this work, we first introduce the continual document learning (CDL) task for KILTs and build a novel benchmark dataset named KILT++ based on the original KILT dataset for evaluation. Then, we conduct a comprehensive study over the use of pre-trained CorpusBrain on KILT++. Unlike the promising results in the stationary scenario, CorpusBrain is prone to catastrophic forgetting in the dynamic scenario, hence hampering the retrieval performance. To alleviate this issue, we propose CorpusBrain++, a continual generative pretraining framework that enhances the original model in two key aspects: (i) We employ a backbone-adapter architecture: the dynamic adapter is learned for each downstream KILT task via task-specific pre-training objectives; the backbone parameters which are task-shared are kept unchanged to offer foundational retrieval capacity. (ii) We leverage the experience replay strategy based on exemplar documents that are similar to new documents, to prevent catastrophic forgetting of old documents. Empirical results demonstrate the significant effectiveness and remarkable efficiency of CorpusBrain++ in comparison to both traditional and generative IR methods.