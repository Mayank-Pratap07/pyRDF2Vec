# pyRDF2Vec
It is python implementation and extension of RDF2Vec to create a 2D feature matrix from a Knowledge Graph for downstream ML tasks.

# What is RDF2Vec?
RDF2Vec is an unsupervised technique that builds further on Word2Vec, where an embedding is learned per word, in two ways:
1. the word based on its context: Continuous Bag-of-Words (CBOW);
2. the context based on a word: Skip-Gram (SG).
To create this embedding, RDF2Vec first creates "sentences" which can be fed to Word2Vec by extracting walks of a certain depth from a Knowledge Graph.
