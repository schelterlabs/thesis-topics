## Name

Understanding the Characteristics and Robustness of Data Preparation Pipelines for Machine Learning

## Description

Research in machine learning is based on a set of static, well-known and widely understood benchmark datasets. In real world ML applications however, the training and evaluation data for the ML model must first be created by a data preparation pipeline. Such a pipeline consumes from several often heterogeneous data sources (e.g., log files, external APIs, tables in a database), combines and cleans the data, and encodes it into feature vectors afterwards. Even though such pipelines are required for any large-scale ML application, they are not well understood by the research community, due to its focus on static benchmark datasets. Often, problems with the ML application can be traced back to problems with the data and/or operations applied by the pipeline. In this thesis, we aim to collect a large set of such pipelines, and analyse them to understand their characteristics and their robustness. The goal of thesis should be to create a publicly shareable dataset of data preparation pipelines, an empirical study of their characteristics and robustness and, optionally, to design novel methods to increase their robustness.

The thesis undertakes a first step in shining light on this problem by focusing on the following **research questions**:

 * What are the characteristics of common data preparation pipelines for ML? What kind of operations are common, how long are these pipelines typically, how many data sources do the consume? Do the characteristics differ based on the type of data and model in use?
 * How robust are the resulting models to changes in the data (e.g., data distribution shifts or data errors) or to changes in the pipeline (e.g., different feature encoders)

The following list contains potential pipeline repositories to explore:

 * OpenML Flows https://www.openml.org/search?type=flow&sort=runs
 * DataScope https://github.com/DS3Lab/datascope-pipelines
 * Github https://github.com/search?q=ColumnTransformer+extension%3Apy+language%3APython+-filename%3Atest_column_transformer.py&type=Code&ref=advsearch&l=&l=

The following literature is helpful to further understand the topic

 * Data Science through the Looking Glass and what we found there, SIGMOD Record 2022, https://arxiv.org/pdf/1912.09536.pdf 
 * Data Validation for Machine Learning https://proceedings.mlsys.org/book/2019/file/5878a7ab84fb43402106c575658472fa-Paper.pdf
 * Data Lifecycle Challenges in Production Machine Learning: A Survey, SIGMOD Record 2018 https://dl.acm.org/doi/abs/10.1145/3299887.3299891
 * Production Machine Learning Pipelines: Empirical Analysis and Optimization Opportunities, SIGMOD 2021, https://dl.acm.org/doi/pdf/10.1145/3448016.3457566
 * Data distribution debugging in machine learning pipelines, VLDBJ 2022, https://stefan-grafberger.com/mlinspect-journal.pdf\

 
 ## Work Environment
 
 The thesis will be supervised by [dr. Sebastian Schelter](https://ssc.io) and [Stefan Grafberger](https://stefan-grafberger.com/), and the student will join the [AI for Retail Lab](https://icai.ai/airlab/), which is a joint research effort between the [Information Retrieval Lab](https://irlab.science.uva.nl/) and the [Intelligent Data Engineering Lab](https://indelab.org) at the UvA.  Our lab includes several PhD students and research engineers with a varied set of interests and expertise revolving around applied machine learning and scalable data management.
 
 ## Expectations
 
This is an ambitious project for a **self-motivated student capable of critical thinking** and willing to take on a research-heavy thesis. The student is expected to develop a written structured work plan, and discuss updates in regular meetings with the supervisor. 

It is strongly encouraged to publish the resulting analysis and software under an open source license. Furthermore, the thesis may result in a publication at a high-quality data engineering or ML conference, which has often happened in the past for student projects supervised within our group.

Required technical skills:
 * Basic understanding of data engineering and machine learning
 * Experience with Python, pandas and git
 * Strong programming skills for working with a variety of potentially dirty datasets

Optional technical skills (can be acquired during the project):
 * Understanding of common data quality issues and data cleaning techniques
 * Ability to work with relational databases


 ## Research Tags
 data preparation for machine learning; data-centric AI; 
 
 
