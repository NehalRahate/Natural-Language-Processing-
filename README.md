# Natural-Language-Processing-

Breif description-
Given Bag of Words 
In this Program we have a list of Comments with Marked 0 - 1 on it 
which hepls the model decide weather a new comment added is positive or negative 

Library Uses
1 - from nltk.corpus import stopwords = helps to extract only the meaningful words from the comments 
  * example :- Honeslty it didn't taste THAT fresh.
    stopword only extract - "honeslti tast fresh" 
2 - from nltk.stem.porter import PorterStemmer - Porter Stemmer is Used to smaller and simpler suffixes
   * example :- Honeslty it didn't taste THAT fresh.
    Stemmer will bring all words to its original form like - Honestly - honeslti
3 - import re
    Regular Expression :- This is used to :- review = re.sub('[^a-zA-Z]',' ',dataset['Review'][i]) # ^ symbol is used for Not sign    
    which remove Special Characters in the Comment which is not necessary 
     it also lower and split all the character
4 - Countvectorizer
    from sklearn.feature_extraction.text import CountVectorizer
    Countvectorizer makes it easy for text data to be used directly in machine learning and deep learning models such as text classification.

     example :- text = [‘Hello my name is james' , ’this is my python notebook’]
     I have 2 text inputs, what happens is that each input is preprocessed, tokenized, and represented as a sparse matrix.

     Hello | is | James | my | name | notebook | python | this
       1      1      1     1     1        0         0       0
       0      1      0     1     0        1         1       1


In the py code given with the repository the last code will give the output of every words in a column CSV file 
