## Name

Learning Relational Database Schemas with Language Models

## Description

While automated machine learning has made great strides in recent years, the automatic preparation of relational data for machine learning (ML) has largely remained a labor-intensive process. A major bottleneck for automatic data integration and feature engineering is the lack of schema information for relational tabular data.

*Relational Database vs. Data Lakes* Relational databases are based on the relational model, an intuitive way of representing data in tables. The columns of a table hold attributes of the data, while primary and foreign key columns are used to establish relations to other tables. Columns and their relationships are specified explicitly in the database schema. This makes it possible to automatically join information across multiple tables for the purpose of feature engineering (See [Deep Feature Synthesis](https://ieeexplore.ieee.org/document/7344858)). However, in practice, data used for machine learning often resides in Data Lakes which are large repositories for raw data that opposed to relational databases do not have a relational schema. Relationships between tables are established ad-hoc by the person who queries the data. This makes data analytics or feature engineering more flexible for humans, but also more challenging to automate, as the knowledge about how individual tables relate to each other is implicit.

*GitSchemas* To tackle the problem of automatic data integration and feature engineering in data lakes, we created a dataset of real-world database schemas from public GitHub repositories. The dataset contains high-quality schema information from >50k databases, with >300k tables, >2M columns, and >140k foreign key relationships (See [GitSchemas](https://ssc.io/pdf/gitschemas.pdf)). This dataset shall help us to develop an NLP-based model that is able to predict relationships between tables based on their column names.

The thesis undertakes a first step in shining light on this problem by focusing on the following **research questions**:

 * Which NLP technique is most suitable for modeling a database schema (e.g. fine-tuning of pre-trained language models, full training of a special architecture, prompt engineering with large language models)?
 * How well can we predict foreign key relationships between tables with this model?
 * How can we minimize the model size with techniques like knowledge distillation or quantization to reduce its inference time while maintaining a high accuracy on the above task?

The following list contains some starting points for literature research:

 * TURL Table Understanding through Representation Learning https://arxiv.org/abs/2006.14806 
 * Finding Related Tables https://research.google/pubs/pub38124.pdf
 * A Machine Learning Approach for Foreign Key Detection http://hpi.de/fileadmin/user_upload/fachgebiete/naumann/publications/2009/WebDB09_crc.pdf

 ## Work Environment

 The thesis will be supervised by [dr. Sebastian Schelter](https://ssc.io) and Till Döhmen (MSc., main author of the GitSchemas Paper), and the student will join the [AI for Retail Lab](https://icai.ai/airlab/),
 which is a joint research effort between the [Information Retrieval Lab](https://irlab.science.uva.nl/) and the [Intelligent Data Engineering Lab](https://indelab.org) at the UvA.  Our lab includes several PhD students and research engineers with a varied set of interests and expertise revolving around applied machine learning and scalable data management.

 ## Expectations

This is an ambitious project for a **self-motivated student capable of critical thinking** and willing to take on a research-heavy thesis.
The student is expected to develop a written structured work plan, and discuss updates in regular meetings with the supervisor.

It is strongly encouraged to publish the resulting analysis and software under an open source license. Furthermore,
the thesis may result in a publication at a high-quality ML or data management conference, which has often happened in the past for student projects supervised within our group.

Required technical skills:
 * Basic understanding of natural language processing and machine learning
 * Experience with Python, pandas and git
 * Strong programming skills for working with a variety of potentially dirty datasets

Optional technical skills (can be acquired during the project):
 * Understanding of various notions of fine-tuning and training of natural language processing models, in particular Transformer-based models
 * Understanding of techniques to reduce model size (e.g. knowledge destillation, pruning, and quantization)
 * Ability to work with relational databases

 ## Research Tags
 natural language processing; feature engineering; relational databases; automated machine learning
