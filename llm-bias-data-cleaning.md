## Name

Uncovering and Mitigating Bias in Large Language Models applied to Data Cleaning


## Description

Large Language Models (LLMs) to generate natural language such as GPT-3 belong to the most astonishing and promising technological advances of the recent years. Currently, their potential to improve upon long-standing difficult tasks in various academic fields is explored by many researchers. One exciting such direction is to understand the potential of LLMs for data cleaning for tabular data. Data cleaning consists of various tasks, such as error detection (e.g., is the value in the 'country' column correct, given the value in the 'city' and 'street' columns?), deduplication (e.g., do two different product names refer to the same real world product?) or data imputation (e.g., what is the correct value for an empty 'country' attribute, given a 'city' value)? Unfortunately, language models have also been shown to contain reproduce existing bias in the language data on which they are trained. The goal of this thesis is to uncover and potentially mitigage such bias when applying LLMs for data cleaning tasks.

The thesis undertakes a first step in shining light on this problem by focusing on the following **research questions**:

 * Can we uncover bias and unfairness issues when using LLMs for data cleaning? E.g., do they work less well for cleaning tasks involving text with non-western names and terms?
 * Can we find ways to mitigate such bias, e.g., by augmenting the training/fine-tuning data for the LLMs with appropriate examples?

The following literature is helpful to further understand the topic

 * Can Foundation Models Wrangle Your Data?, CIDR 2021, https://arxiv.org/pdf/2205.09911.pdf
 * On the Dangers of Stochastic Parrots: Can Language Models Be Too Big? https://dl.acm.org/doi/10.1145/3442188.3445922
 * Responsible Data Management, CACM 2022, https://dl.acm.org/doi/pdf/10.1145/3488717
 

 ## Work Environment
 
 The thesis will be supervised by [dr. Sebastian Schelter](https://ssc.io), and the student will join the [AI for Retail Lab](https://icai.ai/airlab/), which is a joint research effort between the [Information Retrieval Lab](https://irlab.science.uva.nl/) and the [Intelligent Data Engineering Lab](https://indelab.org) at the UvA.  Our lab includes several PhD students and research engineers with a varied set of interests and expertise revolving around applied machine learning and scalable data management.
 
 ## Expectations
 
This is an ambitious project for a **self-motivated student capable of critical thinking** and willing to take on a research-heavy thesis. The student is expected to develop a written structured work plan, and discuss updates in regular meetings with the supervisor. 

It is strongly encouraged to publish the resulting analysis and software under an open source license. Furthermore, the thesis may result in a publication at a high-quality ML or data management conference, which has often happened in the past for student projects supervised within our group.

Required technical skills:
 * Basic understanding of machine learning and NLP
 * Experience with Python, pandas and git
 * Strong programming skills for working with a variety of potentially dirty datasets

Optional technical skills (can be acquired during the project):
 * Understanding of various notions of fairness for automated decision making
 * Understanding of common data quality issues and data cleaning techniques
 

 ## Research Tags
 fairness in machine learning; responsible data science; data-centric AI; automated decision making; data quality; data cleaning 
 
 
