## Name

Robust and dialect-independent parsing of schema information from SQL scripts

## Description

The aim of the thesis is to develop a robust and database dialect-independent SQL parser that can reliably extract schema information from SQL scripts in the wild.

SQL is a database language for defining data structures in relational databases and for editing (inserting, changing, deleting) and querying data stocks based on them. In the decades of development of the SQL standard and various SQL implementations from various database vendors [1], a proliferation of SQL dialects has emerged. This makes it very difficult to parse SQL scripts platform-independent and extract important information.

We collected a corpus of almost 400k SQL scripts from GitHub [2] that contains essential knowledge about how databases are used in practice and how (in which schema) they are typically modeled. This knowledge can be extremely useful for large cloud and database providers, for example to be able to offer users intelligent suggestions for data modeling and transformation tasks.

State-of-the-art parsers like pglast (Postgres) are amazingly sensitive and unable to interpret SQL scripts that contain even the slightest deviation from the respective standard. Projects like simple-ddl-parser [3] take a step in the direction of database-vendor independent interpretation of SQL, but still only show a marginal parsing success rate on GitSchemas of 30%.

This work will most likely require a to build a system that combines classical SQL lexer and parser [4] [5] [6] with a more robust natural language processing (NLP)-based parsing approach.

References:
[1] https://en.wikipedia.org/wiki/SQL#Standardization_history/
[2] Döhmen, Till, et al. "GitSchemas: A Dataset for Automating Relational Data Preparation Tasks." 2022 IEEE 38th International Conference on Data Engineering Workshops (ICDEW). IEEE, 2022. (https://github.com/tdoehmen/gitschemas)
[3] https://github.com/xnuinside/simple-ddl-parser
[4] https://tokern.io/blog/open-source-sql-parsers/
[5] https://www.alibabacloud.com/blog/design-and-practice-of-self-developed-sql-parser_598414
[6] Sunkle, Sagar, et al. "Generating highly customizable SQL parsers." Proceedings of the 2008 EDBT workshop on software engineering for tailor-made data management. 2008. (https://dl.acm.org/doi/pdf/10.1145/1385486.1385495?casa_token=FaklLapchTsAAAAA:6j0ynfNbFSIOKRFWmOaoQiF3UKTJtZAwlY3oQiEj-l43vsV_OF6ZJsNuvnN18lId7T4BVAjXCZr)
 
 ## Work Environment

 The thesis will be supervised by [dr. Sebastian Schelter](https://ssc.io) and Till Döhmen (MSc., main author of the GitSchemas Paper), and the student will join the [AI for Retail Lab](https://icai.ai/airlab/),
 which is a joint research effort between the [Information Retrieval Lab](https://irlab.science.uva.nl/) and the [Intelligent Data Engineering Lab](https://indelab.org) at the UvA.  Our lab includes several PhD students and research engineers with a varied set of interests and expertise revolving around applied machine learning and scalable data management.

 ## Expectations

This is an ambitious project for a **self-motivated student capable of critical thinking** and willing to take on a research-heavy thesis.
The student is expected to develop a written structured work plan, and discuss updates in regular meetings with the supervisor.

It is strongly encouraged to publish the resulting analysis and software under an open source license. Furthermore,
the thesis may result in a publication at a high-quality ML or data management conference, which has often happened in the past for student projects supervised within our group.

Required technical skills:
 * Basic understanding of parsers
 * Experience with a programming language like Python, Java, Rust or C++
 * Data anyltics skills for working with a large corpus of textual data

Optional technical skills (can be acquired during the project):
 * Basic understanding of natural language processing
 * Experience in writing and reading complex SQL queries

 ## Research Tags
 parsing; sql; databases; natural language processing
