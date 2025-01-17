# Available Student Projects

---

## PhD Projects

We are currently recruiting PhD students wishing to start in 2019 at the University of Queensland (UQ), Brisbane. PhD projects are available in the areas of interest of ielab: 

* Formal Models of Information Retrieval (search methods and techniques, user models, evaluation)
* Health Search and domain-specific search


Funding covering tuition fees and scholarship is available, through a competitive process, via UQ. In addition, we have two PhD scholarships (including tuition fees) for the following:

* One full scholarship available for Consumer Health Search, for start in 2019
* One full scholarship available for any topic of interest for ielab, for start in 2019


To express interest in joining ielab as a PhD student, contact Dr Guido Zuccon at zucconguido@gmail.com

---

## Undergraduates, Honours and Masters Projects

The following projects are available for undergraduates, honours and masters students; some projects could be the basis for extension for a PhD project. 

### An exploration of BM25F

BM25F extends the BM25 weighting model to the case of fielded retrieval (e.g. in the presence of documents that have fields, like a web page).

BM25F is a rather standard technique, and has been implemented in various IR tools such as Lucene, Elasticsearch, Lemur and Terrier. However, our initial investigation has shown that the BM25F implementation of Elasticsearch and Terrier differs between each other and from that of the original BM25F model proposed by Robertson and Zaragoza. 

This project will investigate these differences both formally and empirically. The project will further extend a series of experiments we have setup on a number of test collections, and across a number of experimental variables. 
You will have to understand the current code that we have implemented, run this for the additional experiments that are required, and extend the code when relevant. The code is in Python and R; some modifications to the Elasticsearch/Terrier tools are required (they are implemented in Java).

The tasks to be performed in this project include:

1. implementing the original BM25F model in Elasticsearch and Terrier. This requires a good understanding of Java as we will need to hack the Elasticsearch and Terrier source code.
2. Use CLEF 2016, HARD 2003, HARD 2005, TREC WebTrack 2014-2015 to compare performance of BM25F implementations: Terrier, Elasticsearch BM25F and Original BM25F.
3. Extend current experiments we have performed to the use of anchor text data
4. Summarise the results professionally in a written form, by extending a current research article draft

This project is likely to result in a co-authored journal publication at the end of the project.

------------------------------------------------------------

### Clickbait detection on Twitter [assigned @ Xioran Chu]

Clickbait refers to social media posts that are, at the expense of being informative and objective, designed to entice its readers into clicking an accompanying link.
This project aims to devise computational approaches for the identification of clickbaits. The outcome will be a machine learning classifier that rates how click baiting a social media post is. For each social media post, the content of the post itself as well as the main content of the linked target web page are provided.

------------------------------------------------------------

### Survey and implementation of SEO techniques [assigned @ Hayden Mills; one more place available]

Search Engine Optimisation (SEO) aims to tweak web pages to increase their ranking on a target search engine, e.g. Google. SEO is a large market and is based on “black-magic”; SEO experts have suggested a number of techniques to guarantee to be ranked on top positions, some of these are trivial, others are no-where near what a search engine like Google would care about, others do make sense. All techniques have in common that their effectiveness has not been empirically demonstrated nor scientifically investigated. 

In this project, you will go through the relevant literature regarding SEO, including some of the non-academic, gray-literature books that have been published. You will collect the techniques that have been put forward for SEO, along with any evidence of their effectiveness. In the second part of the project, you will implement (preferably in Python) a number of the techniques you have surveyed and test them across a collection of web pages. We do not ask you collect as yet the effectiveness of these techniques in a formal way, but ensure that the techniques you implemented are working correctly.

Tasks:

1. survey the literature and write a short summary of the techniques that have been proposed
2. implement selected techniques
3. setup a test collection to test the effectiveness of the techniques

This project is unlikely to produce a publication within the scope of the project or within short time from its conclusion.

------------------------------------------------------------


### A study of Health Cards

When searching for health information online, Google at times displays so called Health Cards, i.e. a collection of summarised, highly curated information related to a symptom, condition or disease. 

This project will explore:

1. what triggers an health card: given a wide range of health search queries, you will record whether an health card is triggered. At this stage, you will also record the health card
2. what information is in an health card? 
3. are health cards tackling the right conditions? You will use the data collected above, to study whether the health card is relevant to the symptom, condition or disease. You may required help from a medical expert for this (we provide you with this), but you still will have to facilitate the medical expert in his analysis (may need to develop a small interface for the expert to evaluate the correctness). 
4. how are health cards helping users taking decisions, and are they improving the decision? In this part you will devise a user study for evaluating the effectiveness of the health cards. You will not run the user study (if not for testing the protocol), but you will have to setup an appropriate system and protocol. (This may require the development of appropriate web interfaces). 

This project requires the development of data acquisition methods, in Python, along with data analysis methods, both in Python and R.

This project may produce a small publication at the end of the project, or in the immediate period after the project is concluded. 

------------------------------------------------------------

### Simulating Users to Train Systems

Recent advances in user modelling have resulted in the creation of models that can be used to simulate user behaviour related to querying, clicking/assessing and stopping search. It has been argued that these models could be used to evaluate search effectiveness. 

In this project, we take a different view and are interested to explore the use of these models to generate data to train learning-based search engines such as learning to rank systems and deep learning systems. These systems in fact showed promising search effectiveness, but require a large quantity of training data, which is often impossible to acquire for small, specialised search engines (think about domain specific), and also for academic and research purposes. 

The tasks in this project are:

1. implement user simulation models. Some of these models have been already implemented by a third party (Java or Python)
2. implement and deploy learning to rank and deep learning models. Some of these models (learning to rank) are available in tools such as Terrier, but others are not and require implementation. (Java and Python)
3. devise experiments to train models with simulated data and evaluate them on real data, available in existing test collections
4. evaluate the models under different conditions and write up the results in a professional manner

This project may produce a publication at the end of the project, or in the immediate period after the project is concluded; however the implementation and empirical work is quite large, thus there may be not enough time to work on a publication within the scope of the internship

------------------------------------------------------------

### Integrating Complex Operations with Word Embeddings into Retrieval Models [assigned @ Nathan O'Sullivan]

Word Embeddings are a technique to represent words and phrases by mapping them to vectors of real numbers. Popular examples of these techniques are *skipgrams* and *Glove*. We have devised a technique to exploit word embeddings to improve retrieval, calledn NTLM ([ADCS 2015 paper](https://github.com/ielab/adcs2015-NTLM)). This project will expand that work by considering complex operations with word embeddings (e.g. sums and subtractions to represent negations, aggregations to encode the meaning of entities, etc).

The tasks in this project are:

1. familiarise with existing Java code that implements NTLM
2. implement the complex operations with word embeddings and integrate them into retrieval methods. These include: negation, aggregation, analogy.
3. Devise and execute a set of IR experiments to formally evaluate the models
4. write up the results in a professional manner

This project may produce a publication at the end of the project, or in the immediate period after the project is concluded.

------------------------------------------------------------

### Using Word Embeddings for Stemming

This project will consider the use of word embedding representations to perform stemming of text in documents. Stemming refers to the practice of conflating multiple variations of a root word to its stem: for example applying stemming to `play`, `plays`, `playing` returns the stem `play`. Popular stemming algorithms include Portern and Krovetz stemming; these are rule-based stemming methods. Statistical stemmers do exist.

Word Embeddings are a technique to represent words and phrases by mapping them to vectors of real numbers. Popular examples of these techniques are *Skipgrams* and *Glove*. Word embeddings methods allow to perform operations with these vector representations. One such operation is analogy. For example, the expression `man : woman = king : ?x` can be evaluated as `?x = argmax(woman - man + king)`. Our idea is to use the same concept beyond the analogy operation to learn representations of words that share similar stems. 
The project will thoroughly study how this novel approach to stemming influences retrieval effectiveness. 


The tasks in this project are:

1. Formally define the word embedding stemming technique
2. Implement this novel technique and integrate it within a search engine toolkit like Terrier or Lucene/Elastic
3. Review existing stemming techniques
4. Identify implementations of these techniques in the selected search engine toolkit; implement missing techniques
5. Formally evaluate the stemming techniques and analysis the effect of the word embeddings stemming method


This project may produce a publication at the end of the project, or in the immediate period after the project is concluded.

------------------------------------------------------------

### Literature Review on Table Search (with possible extension)

Table search refers to the retrieval of tables in answer to natural languege queries. This project will produce a thorough, formal literature review and summay of table search techniques, and related methods (e.g., table mining, table extension, and table completion). 

This project is highly likely to produce a publication at the end of the project, or in the immediate period after the project is concluded. Because of the nature of this project, the ideal candidate will have strong English writing skills (please demonstrate this at the moment of applying). 

This project may be further extended in a subsequent project that implements identified methods and formally evaluates and compares them.

------------------------------------------------------------

### Literature Reviews on Selected topics in Information Retrieval

This project is specifically designed for IFN701 students that intend to undertake an academic literature review.
In this project you will choose from one of the IR topics/problems listed below (or propose a topic of your own) and perform a rigourous literature review which includes: define the protocol for the review, analyse research publications, compile an annotated bibliography, write up a review of the selected literature.

Topics/problems include:

* Consumer Health Search [(read here for detials)](https://dl.acm.org/citation.cfm?id=3082061)
* Medical Information Retrieval [(read here for detials)](https://dl.acm.org/citation.cfm?id=3082061)
* Automatic creation of systematic reviews using IR, NLP and text mining
* Stemming techniques, including statistical stemming
* Methods for the computation of semantic similarity


------------------------------------------------------------

### Systematic Evaluation of Open Source Search Engines

This project will perform a thorough, systematic evaluation of open source search engines, including (but not limited to) Terrier, Lucene/Sorl, Indri, Elasticsearch.
Prior work has been published in this area. The project will first review this prior work, identifying common trends among them, along with limitations. Then, an evaluation protocol will be defined, including the selection of test collections, evaluation measures (both for effectiveness and efficiency), etc.

This project is highly likely to produce a publication at the end of the project, or in the immediate period after the project is concluded. Because of the nature of this project, the ideal candidate will have good English writing skills (please demonstrate this at the moment of applying). 

------------------------------------------------------------

### A software package for information retrieval evaluation

Evaluation is paramount for IR research. Many evaluation measures exist, each modelling users in a different way and exploring different properties of tasks and interactions. Evaluation measures have been coded up in a number of software packages that are used by the IR community: [trec_eval](http://trec.nist.gov/trec_eval/), [ndeval](http://trec.nist.gov/data/web/10/ndeval.c), [gdeval](trec.nist.gov/data/web/10/gdeval.pl), [inst_eval](https://github.com/ielab/inst_eval), [UBIRE](https://github.com/ielab/ubire). Each of these tools implement only a limited subset of measures, requires different inputs, use different syntax, etc. Direct programmatic integration is often not possible.

This project will develop a new tool for IR evaluation, aiming to:

* provide a reference, complete implementation of IR measures
* support different formats of runs, qrels
* provide APIs endpoints so that the tool could be used programmatically
* include statistical significance testing methods
* include parameter tuning methods like cross validation and loocv

This software should be implemented in Python.
