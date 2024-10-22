# How topics of STEM papers change with time, using Dynamic Embedded Topic Modeling 
Running dynamic embedded topic modeling on abstracts of arxiv articles

## Get the meta data, containing abstracts: 
https://www.kaggle.com/Cornell-University/arxiv (json format)

## Generate embedding 
`python word2vec/run_w2v.py`
This will take all words from abstracts, apply nlp processing (remove stop words, remove rare words, etc) and produce vector representations of all the words (default embedding dimension = 300), and save as embed.txt
More on word embedding is in the original paper: https://arxiv.org/pdf/1310.4546.pdf

## Preprocess text data 
run this script (modify path to json file appropriately)
https://github.com/quynhneo/DETM_arxiv_org/blob/master/scripts/data_undebates.py

## Run Dynamic Embedded Topic Modeling 
run `python main.py` in https://github.com/quynhneo/DETM_arxiv_org/blob/master/main.py
all settings are on top of the file 
