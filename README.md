# Chat-intents
ChatIntents provides a method for automatically clustering and applying group labels to short text documents containing dialogue intents. It uses [UMAP](https://umap-learn.readthedocs.io/en/latest/index.html) for performing dimensionality reduction on user-supplied document embeddings and [HDSBCAN](https://hdbscan.readthedocs.io/en/latest/#) for performing the clustering. Hyperparameters are tuned by performing a Bayesian search (using [hyperopt](https://github.com/hyperopt/hyperopt)) 

# Sentence embeddings:
The chatintents package doesn't include or specify how to create the sentence embeddings of the documents. Two popular pre-trained embedding models, as shown in the notebooks, are the Unversal Sentence Encoder ([USE](https://www.tensorflow.org/hub/tutorials/semantic_similarity_with_tf_hub_universal_encoder)) and [Sentence Transformers](https://huggingface.co/sentence-transformers).
