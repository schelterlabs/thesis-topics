## Title
**Analyzing data quality of web-based datasets in NLP applications**

## Description 

Many Natural Language Processing (NLP) and Machine Learning (ML) applications such as Question Answering, Information Retrieval, Summarization and Translation rely on large text corpora obtrained from the Internet through web crawling. For example, many of the models used in these applications are trained on, or otherwise make use of, the large open-source web text repository [Common Crawl](https://commoncrawl.org) (CC) by aplying various heuristic data cleaning and pre-processing steps to the billions of raw, crawled web pages in CC. Most recently, the [Colossal Clean Crawled Corpus](https://jmlr.org/papers/volume21/20-074/20-074.pdf) (C4) was used to train models such as T5 and the Switch Transformer. However, a [study](https://aclanthology.org/2021.emnlp-main.98/) by Dodge et al. which analyized and documented the pre-processing steps found multiple issues with the C4 dataset, and particularly various artifacts in both the 'cleaned' content and the content that was removed from the originally crawled content, which resulted in unexpected downstream effects on the ML model performance and corresponding biases. 

While CC is widely used for Large Language Model (LLM) training in many NLP applications, the dataset is not well and fully analyzed partially due to its every growing size. On the other hand, better understanding of this large corpus can potentially enable the more thoughtful application of LLM in downstream tasks. Some analysis already exist -- e.g.  [What’s in the box? An analysis of undesirable content in the Common Crawl corpus](https://aclanthology.org/2021.acl-short.24/) and the references cited therein analyze different aspects of  Common Crawl content such as adult content or language distribution. 

Still, the quality of modern large-scale web-based datasets is largely unexplored and in this thesis we will tackle on the following reserach questions:

*  What types of content providers (e.g. current news, user generated blogs, fringe content, etc) are present (and missing) in web-based datasets, such as CC?
* Are there under/over-representation of certain content (and associated biases) in the CC corpus? 
* What are some dimensions of data quality that can be used to assess web content at scale? How do content providers compare along those dimensions? 

In addition to quantifying the impact the above questions may have on NLP applications, we will also explore the downstream implications for data stewardship, data provenance, responsible data management and ethical AI practices in the context of NLP web-based datasets.

## Work Environment

The thesis will be supervised by [Dr. Sebastian Schelter](https://ssc.io) and performed in collaboration with [Nedelina Teneva, PhD](https://megagon.ai/team/nedelina-teneva/), a researcher at Megagon Labs, Mountain View, CA. The student will join the [AI for Retail Lab](https://icai.ai/airlab/), which is a joint research effort between the [Information Retrieval Lab](https://irlab.science.uva.nl/) and the [Intelligent Data Engineering Lab](https://indelab.org) at the UvA.  Our lab includes several PhD students and research engineers with a varied set of interests and expertise revolving around applied machine learning and scalable data management.

## Expectations

This is an ambitious project for a *self-motivated student capable of critical thinking* and willing to take on a research-heavy thesis. The student is expected to develop a written structured work plan, and discuss updates in regular meetings with the supervisor. 

The student is strongly encouraged to publish the resulting analysis and software under an open source license. Furthermore, the thesis may result in a publication at a high-quality ML or NLP conference, which has often happened in the past for student projects supervised within our group.


Required technical skills:

 * Basic understanding of machine learning

 * Experience with Python, Git and exposure to distributed computing tools such as Spark, Dask or Map-Reduce 

 * Strong programming skills for working with a variety of text datasets (e.g., parsing HTML data)



Optional technical skills (can be acquired during the project):

 * Familiarity with neural based ML model development and training

 * Familiary with data quality issues and data cleaning techniques and their applications to NLP

 * Ability to work with large scale datasets and/or distributed computing tools

 * Ability to work with AWS infrastructure (specifically S3)


 ## Research Tags
 Natural Language Processing (NLP); NLP dataset quality; Ethics in AI; data-centric AI 

 
----- 
----- EXAMPLE ---- 

## Name

An Empirical Study of Data Errors in Fairness-Sensitive Datasets


## Description



*Automated Decision Systems.* The need for responsible data science intensifies with the growing impact of data and machine learning (ML) on society. Automated Decision Systems (ADS), socio-legal-technical systems that are used broadly in industry, non-profits, and government. ADS process data about people, help make decisions that are consequential to people’s lives, are designed with the stated goals of improving efficiency and promoting equitable access to opportunity, involve a combination of human and automated decision making, and are subject to auditing for legal compliance and to public disclosure. They may or may not use AI, and may or may not operate with a high degree of autonomy, but they rely heavily on data. (See [Responsible Data Management](http://www.vldb.org/pvldb/vol13/p3474-asudeh.pdf) for details). Unfortunately, ADS tend to reproduce and amplify existing discrimination (see [Why is my classifier discriminatory](https://arxiv.org/abs/1805.12002) for details) when used in practice. In recent years, the legal and ML community have studied various notions of fairness in decision making and developed a variety of methods to accordingly adjust input data, learning algorithms or predictions of ML models (see [A survey on bias and fairness in machine learning](https://arxiv.org/abs/1908.09635) for details).



*Impact of Data Errors on Fair Decision Making.* Unfortunately, real world data is typically subject to several data quality issues (see [Quantitative Data Cleaning for Large Databases](https://dsf.berkeley.edu/jmh/papers/cleaning-unece.pdf) for details) and rarely complete (see [An Analysis of Four Missing Data Treatment Methods for Supervised Learning](https://www.researchgate.net/publication/220355769_An_Analysis_of_Four_Missing_Data_Treatment_Methods_for_Supervised_Learning/link/0c960528d2ff18f065000000/download) for details). While data errors in general have a negative impact on the predictive performance on ML models, it is unclear what their impact on the fairness of the model predictions is. 



The thesis undertakes a first step in shining light on this problem by focusing on the following **research questions**:



 * What kind of data errors do we encounter in data used for automated decision making? How are they distributed in the data?

 * Are there differences in the distribution of data errors that we encounter for the data of historically disadvantaged groups compared to privileged groups?

 * How well do common data cleaning methods rectify these errors? Do we see differences in the cleaning performance for the data of historically disadvantaged groups compared to privileged groups?



The following list contains potential datasets to explore:



* __Lending__

  * https://github.com/ResponsiblyAI/responsibly/tree/master/responsibly/dataset/adult

  * https://github.com/ResponsiblyAI/responsibly/tree/master/responsibly/dataset/german

  * https://github.com/ResponsiblyAI/responsibly/tree/master/responsibly/dataset/fico

  * https://www.kaggle.com/c/GiveMeSomeCredit



 * __Criminal Justice__

   * https://github.com/ResponsiblyAI/responsibly/tree/master/responsibly/dataset/compas



 * __Health/Mental health__

   * https://archive.ics.uci.edu/ml/datasets/heart+disease

   * https://www.kaggle.com/xiaowenlimarketing/international-student-time-management?select=International+students+Time+management+data.csv

 

 ## Work Environment

 

 The thesis will be supervised by [dr. Sebastian Schelter](https://ssc.io), and the student will join the [AI for Retail Lab](https://icai.ai/airlab/), which is a joint research effort between the [Information Retrieval Lab](https://irlab.science.uva.nl/) and the [Intelligent Data Engineering Lab](https://indelab.org) at the UvA.  Our lab includes several PhD students and research engineers with a varied set of interests and expertise revolving around applied machine learning and scalable data management.

 

 ## Expectations

 

This is an ambitious project for a **self-motivated student capable of critical thinking** and willing to take on a research-heavy thesis. The student is expected to develop a written structured work plan, and discuss updates in regular meetings with the supervisor. 



It is strongly encouraged to publish the resulting analysis and software under an open source license. Furthermore, the thesis may result in a publication at a high-quality ML or data management conference, which has often happened in the past for student projects supervised within our group.



Required technical skills:

 * Basic understanding of machine learning

 * Experience with Python, pandas and git

 * Strong programming skills for working with a variety of potentially dirty datasets



Optional technical skills (can be acquired during the project):

 * Understanding of various notions of fairness for automated decision making

 * Understanding of common data quality issues and data cleaning techniques

 * Ability to work with relational databases





 ## Research Tags

 fairness in machine learning; responsible data science; data-centric AI; automated decision making; data quality; data cleaning 

 

 

