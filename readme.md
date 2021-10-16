# Medical Document Retrieval System

### Team members
* Gokul BJ
* Ganesh Kumaar S
* Surya P

#### Project Guide - Ms. S. Anitha
&nbsp;
## About the project

Medical data is one of the most searched for topics on the internet, and therefore it is important to have an efficient and accurate Information Retrieval system in place. In this project consists of a domain specific Information Retrieval System which has the best performing Parsing, Indexing and Ranking methods. Here we retrieve documents not only matching query terms but also make use of CUIs (Concept Unique Identifiers) of medical terms and similarity of word embeddings to improve the results.

&nbsp;
## Indexing the Input Data
The input files initially undergo data cleansing. Next, Parts of Speech (POS) and Named Entity Recognition (NER) tags are generated along with fasttext word embeddings which are all then indexed. 

&nbsp;
## Running a Query
When a query is given to the system, it undergoes preprocessing where the cleansed data, word embeddings, POS and NER tags are generated. Once this has been done, the system retrieves the documents based on the original query. The system also retrieves documents that have a matching CUI tags as well as documents which have word embeddings that are similar (Cosine similarity of fasttext embeddings). Then the results are ranked and displayed to the user.

&nbsp;
## Architecture Diagram

![img 1](https://user-images.githubusercontent.com/64645167/137593517-50467834-ea46-4e21-b037-54f599eab465.png)

&nbsp;
## Tools used

#### General
* Python
* Numpy
* Gensim
<!-- 
&nbsp; -->
#### NLP
* spaCy
* scispaCy
* nltk
<!-- 
&nbsp; -->
#### NLP models used for generating POS & NER
* en_core_sci_scibert (POS) (Pretrained model based on BERT)
* en_ner_craft_md (NER) (Taxonomical and chemical entities)
* en_ner_jnlpba_md (NER) (DNA, cell entities)
* en_ner_bc5cdr_md (NER) (Chemical disease entities)
* en_ner_bionlp13cg_md (NER) (Pathological formation, Gene / Gene product, Anatomical entities)
<!-- 
&nbsp; -->
#### Word Embeddings
* fasttext
<!-- 
&nbsp; -->
#### Medical Terminology
* UMLS (3M concepts)
* MeSH (30K entities)
* RxNorm (Clinical Drugs - 100K concepts)
* GO (Gene Ontology - 67K concepts)
* HPO (Human Phenotype Ontology - 16K concepts)
<!-- 
&nbsp; -->
#### Frontend
* Flask
* Jinja
* Ngrok

<!-- &nbsp;
## Results?

&nbsp;
## Future Work? -->

