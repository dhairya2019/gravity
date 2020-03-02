# gravity
Description: 
The objective of this project is to measure the semantic similarity of the document uploaded by the user with existing documents and derive a score which determines the degree to which the document is plagiarized. 
This project intends to overcome the shortcomings of existing plagiarism detection techniques by using semantic analysis instead of syntactic analysis. We can detect semantic plagiarism with the help of Natural Language Processing (NLP) Tools. It is a branch of artificial intelligence that helps computers understand, interpret and manipulate human language. NLP draws from many disciplines, including computer science and computational linguistics, in its pursuit to fill the gap between human communication and computer understanding.   
Overall algorithm - First, we create a repository. The document in the repository can be a webpage. If it is a webpage, text from the url is extracted and stored in a file in repository. Then, store the document uploaded by user in our repository. Furthermore, preprocessing of documents is performed. The final step is computation of similarity percentage of documents. 
 Pre-processing: Since text is the most unstructured form of all the available data, various types of noise are present in it and the data is not readily analyzable without any pre-processing. The entire process of cleaning and standardization of text, making it noisefree and ready for analysis is known as text preprocessing.  Hence, we have developed a semantic plagiarism detector where there will be semantic checking which includes checking of synonyms. The underlying syntactic structure and semantic meaning of two documents can be compared to reveal their similarity.  
 Conversion of text to lower case: This is to avoid distinguishing between words simply on the basis of case. 
  Removal of punctuation except full stop: Punctuation can provide grammatical context which supports understanding but does not add any value. Full stops are not removed because they are needed later for sentence tokenization. 
  Removal of special characters and alphanumeric characters: They are not relevant to our analysis.  Removal of English stop words: Stop words are common words found in a language. Words like for, of, are etc are common stop words.  
 Stemming: Transforms to root word. Stemming uses an algorithm that removes common word endings for English words, such as “es”, “ed” and “’s”.  
 Lemmatization: Transformation to dictionary base form i.e., “produce” & “produced” become “produce”. 
Computing semantic similarity-  
 Break down the user and repository documents into sentences. 
  Take each sentence of the user document and one at a time compare it with each sentence of a document from repository.  
 Repeat this for all documents of repository; we get an array of similarity percentage scores for each document. 
  Once we get the individual percentage similarity, we take average of all to get the final similarity percentage 
EXPERIMENT AND RESULT- In the proposed algorithm, the documents are checked semantically sentence wise and the similarity percentage of user document with each document is shown and stored. Then, average of these documents is taken to generate the final similarity percentage with all documents. While conducting tests, two documents were compared and similarity score was generated. Say, user document has 45 sentences and document in repository has 60 sentences, each sentence in user document will be compared with each sentence in repository document. To generate the score, it will be divided by total number of sentences 45*60 = 2700. This is repeated for all documents in the repository. This will give us an overall score which gives us an idea of the degree of plagiarism whether it is low, moderate or high. 
 
Following packages are used to develop the project: 
Tqdm 
Nltk 
Matplotlib 
Networkx 
Datasketch 
 
This program finds the plagiarism by using the MinHash algorithms. 
MinHash is a technique widely used to compare texts for similarity. For example, in web search it is used to detect mirror sites.  Web search engines are interested in mirror detection because of two reasons. First of all, it significantly reduces cost of maintaining search engine. Search engines typically index contents of only the primary web site (highestly ranked) and ignore all its mirrors. Secondly, mirrors to well-known sites often indicate phishing, which raises red flags for security team. Another application of MinHash is plagiarism detection which universities and scientific magazines are interested to automatically recognize copypasted papers and thesises 
https://mccormickml.com/2015/06/12/minhash-tutorial-with-python-code/
