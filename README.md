# Text-Similarity-uisng-Word-Embeddings

Goal: to compare the text documents doc1.txt and doc2.txt and display their similarity percentage. 

Method:
1. Read the two files doc1.txt and doc2.txt
2. tokenize their sentences and make one corpus for each file
3. Use Word embedding models (BERT or ELMo) to make each sentence into a vector
4. use Cosine similarity to compute the Similarity matrix. (this matrix has the similarity index of each sentence of doc1 in comparison to each sentence of doc2)
5. to find total similarity percentage:
        a. for each sentence of doc1 (this is the query sentence) find maxiumum similarity to any sentence of doc2 (doc2 is the comparison document) 
        b. store this maximum similarity of each sentence of doc1 in an array
        c. compute the average of all the maximum similarity obtained for each sentence in doc1. This is thought to be the total similarity between doc1 and doc2. 
