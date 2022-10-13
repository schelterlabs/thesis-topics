##### Proposal
AI Thesis project proposal

##### Name
Efficient Inspection of Data Preprocessing in Native Machine Learning Pipelines using DuckDB

##### Description
Machine Learning (ML) is increasingly used to automate impactful decisions, and the risks arising from this wide-spread use are garnering attention from policy makers, scientists, and the media. ML applications are often brittle with respect to their input data, which leads to concerns about their correctness, reliability, and fairness.

It is a difficult and tedious task to ensure at development time that the end-to-end ML pipelines for such applications adhere to sound experimentation practices and compliance requirements. Identifying issues like technical bias introduced during data preprocessing currently requires a high degree of discipline, knowledge and time from data scientists.

While issue detection in areas like fairness cannot be fully automated, computational tools can help pinpoint particular types of data issues. We recently proposed [mlinspect](https://github.com/stefan-grafberger/mlinspect), a library that enables lightweight lineage-based inspection of ML preprocessing pipelines. We believe mlinspect can serve as a common platform to automatically apply issue detection techniques from specialised libraries. To facilitate this, mlinspect offers an easy-to-use interface to integrate new analysis techniques as inspections.

However, inspections in mlinspect are currently implemented using iterators in Python. In our [most recent publication about mlinspect](https://stefan-grafberger.com/mlinspect-journal.pdf), we propose optimizable inspections based on dataframe operators. A drawback of our old Python-based inspections is the high runtime overhead inherited from Python and a lack of vectorization, which typically requires calling external C code. To address this issue, we want an alternative, less general but more efficient method for executing inspections using an in-process database like DuckDB. 

DuckDB is an in-process SQL OLAP database management system that seemingly integrates with the Python ecosystem. Thanks to [efficient data transfer](https://dl.acm.org/doi/pdf/10.1145/2618243.2618265) and [some recently added features](https://github.com/duckdb/duckdb/pull/3700), it should now be possible to transparently leverage DuckDB for joint execution of native ML pipelines and the mlinspect inspections using dataframe operations.

Recently, another research group already proposed using [a database like Umbra to execute Python ML pipelines and selected mlinspect functionality](https://db.in.tum.de/~schuele/data/mlinspect.pdf?lang=en). However, that approach has severe limitations due to data transfer costs of non-embedded databases and not trying to offer a extensible general interface for new inspections.

As part of this thesis project, you will investigate joint execution of ML pipelines and mlinspect inspection techniques in DuckDB.

Feel free to reach out if you have any questions.

##### Initial literature
* [Data distribution debugging in machine learning pipelines](https://stefan-grafberger.com/mlinspect-journal.pdf)
* [Blue Elephants Inspecting Pandas](https://db.in.tum.de/~schuele/data/mlinspect.pdf?lang=en)
* [DuckDB: an Embeddable Analytical Database](https://duckdb.org/pdf/SIGMOD2019-demo-duckdb.pdf)
* [Data Management for Data Science Towards Embedded Analytics](https://duckdb.org/pdf/CIDR2020-raasveldt-muehleisen-duckdb.pdf)
* [Efficient Data Management and Statistics with Zero-Copy Integration](https://dl.acm.org/doi/pdf/10.1145/2618243.2618265)


##### Potential public datasets to explore
* [See example pipelines from ArgusEyes](https://github.com/schelterlabs/arguseyes/tree/master/arguseyes/example_pipelines)
* [See example pipelines from mlinspect](https://github.com/stefan-grafberger/mlinspect/tree/master/example_pipelines)


##### Work environment
The thesis will be supervised by [Stefan Grafberger](https://stefan-grafberger.com/), and the student will join the [AI for Retail Lab](https://stefan-grafberger.com/), which is a joint research effort between the [Information Retrieval Lab](https://irlab.science.uva.nl/) and the [Intelligent Data Engineering Lab](https://indelab.org/) at the UvA. Our lab includes several PhD students and research engineers with a varied set of interests and expertise revolving around applied machine learning and scalable data management.

##### Expectations
This is an ambitious project for a self-motivated student capable of critical thinking and willing to take on a research-heavy thesis. The student is expected to develop a written structured work plan, and discuss updates in regular meetings with the supervisor.

It is strongly encouraged to publish the resulting analysis and software under an open source license. Furthermore, the thesis may result in a publication at a high-quality ML or data management conference, which has often happened in the past for student projects supervised within our group.

Required technical skills:
* Basic understanding of machine learning
* Experience with Python, pandas, scikit-learn, and git
* Strong programming skills for working with our research library mlinspect, which conducts code instrumentation and monkey-patches third-party libraries

Optional technical skills (can be acquired during the project):
* Understanding of common preprocessing operations in ML pipelines
* Basic knowledge of relational databases, and efficient data processing
* Experience with CI/CD tools like GitHub Actions and unit testing

##### Research Tags
machine learning pipelines; data management; data-centric AI; data preprocessing  
