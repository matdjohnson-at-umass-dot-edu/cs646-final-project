# cs646-final-project

A repository containing the notebooks used to perform the computations associated with the UMass CS646 final project by Matthew Johnson.

The notebooks include preprocesing notebooks, a baseline evaluation notebook, and preliminarily notebooks for training and evaluating a binary classification model.

The preprocessing notebooks perform the following functions:

1) Preprocessing 1 - freeze image of BeIR MS Marco dataset, tokenize dataset using SimCSE, embed dataset using SimCSE
2) Preprocessing 2 - compute the per-query and per-passage average and sum of the embedded dataset
3) Preprocessing 3 - concatenate batches of averaged and summed embeddings
4) Preprocessing 4 - select negative examples for each positive example from the dataset using cosine similarity
5) Preprocessing 5 - filter out dataset entries where negative example and positive example cosine similarity was in the top 50 percentiles of such cosine similarities

The baseline evaluation notebook is "Cosine Similarity IR". The notebook computes the cosine similarity of queries with all embedded documents. All embedded documents are thosoe embedded in preprocessing 1, which is a subset of documents from the BeIR MS Marco dataset (approximately 0.125 of the dataset).

The notebooks for training and evaluating a binary classification model all include the word "Model". These notebooks will be updated through the end of finals week. The results of these notebooks are contained in [RESULTS.md](RESULTS.md).

The Google Drive for the project notebooks, the dataset data (including intermediate data stages), and the model parameters, is at the following link:

https://drive.google.com/drive/folders/1J8ipyZ2DbdNdyLH7q2MAcd03YynNoZcH?usp=sharing
