![alt text](iitkgplogo.jpg)

**Knowledge Graph Embedding and Similar Fact Retrieval Using TransE and TransR**

**Project Description:**
This project involves developing a custom implementation of two knowledge graph embedding techniques, TransE and TransR, to tackle key tasks in knowledge graph analysis. The objectives of the project are as follows:

**Implementation of Knowledge Graph Embeddings:**

Develop custom implementations of TransE and TransR models to generate vector embeddings for entities and relations in a knowledge graph.

**1-Hop Question-Answering:**
Utilize the embeddings to infer missing entities in the knowledge graph, solving 1-hop question-answering problems.

**Performance Evaluation:**
Compare the effectiveness of TransE and TransR models using suitable evaluation metrics to measure their performance in handling knowledge graph-based tasks.

**Similar Fact Retrieval:**
Design a model to identify and rank the top-5 most similar facts to a given fact, enabling fact-based similarity searches and analysis.
By integrating knowledge graph embedding techniques with real-world applications like question-answering and fact retrieval, the project aims to explore the utility and comparative performance of TransE and TransR in knowledge graph reasoning.

**Dataset Description**
Use the Nations and Kinships datasets for the 1-hop question-answering and Nations dataset for the similar fact retrieval task.

***Nations***: The Nations dataset is a small knowledge graph with 14 entities, 55 relations, and 1992 triples describing countries and their political relationships.

***Kinships***:The Kinships dataset describes relationships between members of the Australian tribe Alyawarra and consists of 10,686 triples. It contains 104 entities representing members of the tribe and 26 relationship types that represent kinship terms such as Adiadya or Umbaidya.

**Tasks**

***Setup and Preprocessing***:

● Install the pyKEEN library.

● Loadthe datasets from the pyKEEN library extracting triples for training, validation and testing. (https://pykeen.readthedocs.io/en/stable/reference/datasets.html)

***TransE and TransR Implementation Specifications***: 

● Embedding dimensions: 100.

● Margin: : Vary 1.0 to 5.0 with step size 1.0 for Nations dataset and take 1.0 for Kinships dataset.

● Optimizer: Adam, learning rate 0.001, train for 50 epochs.

● Usemargin-based ranking loss.

● UseBernoulli Negative sampling (without using the built-in library function) for generating the negative samples.Refer:https://pykeen.readthedocs.io/en/stable/reference/negative_sampling.html
