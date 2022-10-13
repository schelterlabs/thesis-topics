## Project Name

Improving the Stability of Data-Based Explanations for Fairness Debugging

## Description

Software systems that learn from user data with machine learning (ML) have become ubiquitous in recent years, and participate in many critical decision-making processes, e.g., about loans, job applications and medical treatments. Unfortunately, such applications often reproduce or even amplify existing discrimination [3,4] when no active countermeasures are taken. As part of the recent movement towards data-centric AI, researchers have proposed novel ways to identify training examples that negatively impact the fairness of a model trained on the data [1,5].

In this thesis we will focus on GOPHER [1], an approach that searches for subsets of the data whose removal would improve the fairness score of a classifier, as measured by the proposed "causal responsibility metric" and identifies patterns that explain why they are problematic. In order to accelerate the search, the underlying model is not retrained to quantify the change in the fairness outcomes, but the updated model parameters are estimated via influence functions [2], a well-known concept in robust statistics.

Recent work has shown that influence functions have several shortcomings, including having different results based on the choice of architecture, or on the choice of test data in the training-test split [6]. Additionally, the accuracy of influence functions also deteriorates if there are large groups or records which are responsible for the bad performance [7]. While none of these works focus specifically on fairness, all of these issues impact the real-world applicability of data-based explanations that GOPHER would produce.

The goal of this thesis would be to first empirically quantify the stability of the data-based explanations provided by GOPHER via an experimental study on several benchmark datasets. The next step would be to theoretically characterize the instability of GOPHER by adapting the analysis techniques from influence function literature [6,7] and provide some insights on how to improve its robustness.

References:
[1] Interpretable Data-Based Explanations for Fairness Debugging https://arxiv.org/pdf/2112.09745.pdf
[2]  Understanding Black-box Predictions via Influence Functions https://arxiv.org/abs/1703.04730
[3] Responsible Data Management, CACM 2022, https://dl.acm.org/doi/pdf/10.1145/3488717
[4] Why is my classifier discriminatory? https://arxiv.org/abs/1805.12002
[5] Data Debugging with Shapley Importance over End-to-End Machine Learning Pipelines https://arxiv.org/abs/2204.11131
[6] Influence Functions in Deep Learning Are Fragile https://arxiv.org/abs/2006.14651
[7] On the Accuracy of Influence Functions for Measuring Group Effects https://proceedings.neurips.cc/paper/2019/file/a78482ce76496fcf49085f2190e675b4-Paper.pdf


## Work Environment

The thesis will be supervised by dr. Sara Magliacane https://smaglia.wordpress.com/ and dr. Sebastian Schelter https://ssc.io , and the student will join the AI for Retail Lab https://icai.ai/airlab/. Our lab includes several PhD students and research engineers with a varied set of interests and expertise revolving around applied machine learning and scalable data management.

## Expectations
This is an ambitious project for a **self-motivated student capable of critical thinking** and willing to take on a research-heavy thesis. The student is expected to develop a written structured work plan, and discuss updates in regular meetings with the supervisor.

The aim of the thesis is a publication at a top AI/ML or data engineering conference, which has often happened in the past for student projects supervised within our group. It is strongly encouraged to publish the resulting analysis and software under an open source license. 

We accept applications for the project after October 7 (after the thesis fair). Please include your CV and your current study record in your application. 

Required technical skills:

* Good understanding of machine learning and data engineering, as shown by a strong study record in core courses such as ML 1&2
* Experience with Python, pandas and git

Optional technical skills (can be acquired during the project):
* Understanding of causality and various notions of fairness for automated decision making

## Research Tags
Fairness; data preparation for machine learning; data-centric AI; causality


 
 
