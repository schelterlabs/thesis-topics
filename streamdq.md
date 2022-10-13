##### Proposal
AI Thesis project proposal

##### Name
Automating data quality checks involving order and time for large data streams

##### Description
Modern companies and institutions rely on data to guide
every single business process and decision. Missing or incorrect information seriously compromises any decision process downstream. Therefore, a crucial, but tedious task for everyone involved in data processing is to verify the quality of their data. 

In collaboration with bol.com, we developed a system for automating the verification of data quality in streaming scenarios at scale. Our system, StreamDQ, provides a declarative API, which combines common quality constraints with user-defined validation code, and thereby enables ‘unit tests’ for data. StreamDQ efficiently executes the resulting constraint validation workload by translating it to a pipeline for a streaming dataflow engine. StreamDQ is built on top of Apache Flink. Apache Flink is a distributed streaming data-flow engine written in Java and Scala.

So far, existing data quality libraries like [Deequ](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=&cad=rja&uact=8&ved=2ahUKEwj6oe-slcn5AhUNxQIHHaI1A6wQFnoECAQQAQ&url=https%3A%2F%2Fgithub.com%2Fawslabs%2Fdeequ&usg=AOvVaw0zAA9OtFfIWS8RvCqgU3dt) and [great-expectations](https://github.com/great-expectations/great_expectations) focus on batch use cases. However, in streaming scenarios, new types of data quality checks are required in addition to the checks typically used in batch scenarios. In contrast to batch scenarios, we now need to consider notions of order and time as first-class citizen. Some examples: 

* The value in a particular column should be monotonically increasing.
* For each event of some `EventType.RemovedProperty`, there should be a matching predecessing event of `EventType.AddedProperty` for that entity.
* Some value in a time column should always be lower than the current time.

Your project will be to explore new, streaming-specific types of data quality checks, design a user-friendly API for them, efficiently implement them in StreamDQ, and experimentally evalute the implementation.

##### Initial literature
* [Automating Large-Scale Data Quality Verification](https://www.vldb.org/pvldb/vol11/p1781-schelter.pdf)
* [The Stratosphere platform for big data analytics](https://link.springer.com/content/pdf/10.1007/s00778-014-0357-y.pdf)
* [Apache Flink™: Stream and Batch Processing in a Single Engine](https://asterios.katsifodimos.com/assets/publications/flink-deb.pdf)

##### Potential public datasets to explore
* [Wikimedia EventStream (streams like wikimedia.page-properties-change might be especially interesting)](https://stream.wikimedia.org/v2/ui/#/)
* [Wikipedia Clickstream](https://meta.wikimedia.org/wiki/Research:Wikipedia_clickstream)
* [Yahoo Streaming Benchmark](https://github.com/yahoo/streaming-benchmarks)
* [Amazon Customer Reviews](https://s3.amazonaws.com/amazon-reviews-pds/readme.html)
* Depending on the type of checks you implement, you may need to modify existing datasets to add specific attributes or properties you want to test or write a generator for synthetic data

##### Work environment
The thesis will be supervised by [Stefan Grafberger](https://stefan-grafberger.com/), and the student will join the [AI for Retail Lab](https://stefan-grafberger.com/), which is a joint research effort between the [Information Retrieval Lab](https://irlab.science.uva.nl/) and the [Intelligent Data Engineering Lab](https://indelab.org/) at the UvA. Our lab includes several PhD students and research engineers with a varied set of interests and expertise revolving around applied machine learning and scalable data management.

##### Expectations
This is an ambitious project for a self-motivated student capable of critical thinking and willing to take on a research-heavy thesis. The student is expected to develop a written structured work plan, and discuss updates in regular meetings with the supervisor.

It is strongly encouraged to publish the resulting analysis and software under an open source license. Furthermore, the thesis may result in a publication at a high-quality ML or data management conference, which has often happened in the past for student projects supervised within our group.

Required technical skills:
* Basic understanding of distributed data processing
* Strong programming skills and git experience
* Quickly learn how to program in Kotlin


Optional technical skills (can be acquired during the project):
* Working with Apache Flink
* Ability to work with larger datasets

##### Research Tags
data quality; stream-processing; data-centric AI 
