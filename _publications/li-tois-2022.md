---
redirect_from: /publications/li-tois-2022
authors: [hang-li, ahmed-mourad, shengyao-zhuang, bevan-koopman, guido-zuccon]
title: "Pseudo Relevance Feedback with Deep Language Models and Dense Retrievers: Successes and Pitfalls"
venue: Accepted by the ACM Transactions on Information Systems (TOIS)
year: 2022
pdf: /publications/pdfs/li2022tois.pdf
links:
 - url: https://github.com/hanglics/Neural-Relevance-Feedback-Public/tree/master/Text_Based_PRF
   name: Code for Text-Based PRF
 - url: https://github.com/hanglics/Neural-Relevance-Feedback-Public/tree/master/Vector_Based_PRF
   name: Code for Vector-Based PRF
 - url: https://drive.google.com/drive/folders/1kOmNy5zZi34BZHEnRiGJmglyYIwvb7wH?usp=sharing
   name: Datasets
 - url: https://drive.google.com/drive/folders/1UdtGJpjdYQ8G6tzxhgnDsi2wU41Knv4x?usp=sharing
   name: Models
 - url: https://drive.google.com/drive/folders/1l7_P0T-HcloXwVZMvlM7jcnlmFk4itju?usp=sharing
   name: Results
---
---
## Abstract

Pseudo Relevance Feedback (PRF) is known to improve the effectiveness of bag-of-words retrievers. At the same time, deep language models have been shown to outperform traditional bag-of-words rerankers. However, it is unclear how to integrate PRF directly with emergent deep language models. In this article, we address this gap by investigating methods for integrating PRF signals into rerankers and dense retrievers based on deep language models. We consider text-based and vector-based PRF approaches, and investigate different ways of combining and scoring relevance signals. An extensive empirical evaluation was conducted across four different datasets and two task settings (retrieval and ranking).

Text-based PRF results show that the use of PRF had a mixed effect on deep rerankers across different datasets. We found that the best effectiveness was achieved when (i) directly concatenating each PRF passage with the query, searching with the new set of queries, and then aggregating the scores; (ii) using Borda to aggregate scores from PRF runs. 

Vector-based PRF results show that the use of PRF enhanced the effectiveness of deep rerankers and dense retrievers over several evaluation metrics. We found that higher effectiveness was achieved when (i) the query retains either the majority or the same weight within the PRF mechanism, and (ii) a shallower PRF signal (i.e., a smaller number of top-ranked passages) was employed, rather than a deeper signal. Our vector-based PRF method is computationally efficient; thus this represents a general PRF method others can use with deep rerankers and dense retrievers.