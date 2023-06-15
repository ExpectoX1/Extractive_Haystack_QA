# Extractive_Haystack_QA
An Extractive Question Answering Software that uses  Haystack to Answer Questions.
Extractive question answering is a model used to retrieve specific information from a given dataset and provide precise answers to questions. Instead of generating new responses, it identifies and extracts relevant portions of the text that directly address the question. The model scans the dataset, identifies potential answer candidates, and ranks them based on their relevance to the question. The selected answer is then extracted from the dataset and presented as the response. Extractive question answering is particularly useful when the dataset contains explicit answers or when the goal is to retrieve factual information from the text.
The Model used here is roberta-base-squad2. It is a model trained on the squad_v2 dataset. It is an extractive question-answering model which can answer questions by searching through the documents provided. 
The model developed used Haystack for document retrieval and searching through the documents. Libraries like BM25Retriever, FARMReader, ExtractiveQAPipelines, etc were used for sorting and searching through data. 
This model is computationally very inexpensive. It can parse through and predict answers in less than 2 seconds. The downfall of this model is that this model is “Extractive”, because of which the answers are mostly in a line or a single word. 
The accuracy of the model was found to be around 79%

## Environment Setup 
To run the .ipynb on a local machine the following has to be installed. 

`pip install 'farm-haystack[all]'`
`pip install tensorflow_probability==0.13.0`

A huge amount of sample txt docs will be downloaded when the code is run. 

