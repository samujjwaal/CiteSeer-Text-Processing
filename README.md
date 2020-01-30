# CiteSeer Collection Text Processing

This project was done as a homework assignment for CS582: Information Retrieval course at the University of Illinois at Chicago during the Spring 2020 term.

----

The [dataset](citeseer "CiteSeer UMD collection") used was the CiteSeer UMD collection which is a standard text document collection, consisting of abstracts of Computer Science research articles from the CiteSeer digital library.

---

The tasks in the [assignment](Tasks.pdf "Assignment description") included:

1. Preprocess the document collection, wherein the text was tokenized on whitespace and punctuations were removed.
2. Determine the frequency of occurrence for all the words in the collection, and answer the following questions:
   * What is the total number of words in the collection?
   * What is the vocabulary size?
   * What are the top 20 words in the ranking?
   * From these top 20 words, which ones are stop-words?
   * What is the minimum number of unique words accounting for 15% of the total number of words in the collection?
3. Integrate the Porter Stemmer in the preprocess step and also eliminate stop words from the collection, and answer the questions from task 2 again.
   

Check out the [Jupyter Notebook](citeseer.ipynb "CiteSeer Collection Text Processing") to see the python implementation of the tasks.

----

**Results**

For Task 2:

* Total number of words in the collection : 488663
* Vocabulary size (number of unique words) : 17322
* Top 20 words in the ranking :
  'the', 'of', 'and', 'a', 'to', 'in', 'for', 'is', 'we', 'that', 'this', 'on', 'are', 'an', 'with', 'as', 'by', 'data', 'based', 'be'
* Stop-words out of the top 20 words : (all except 'data' and 'based')
   'the', 'of', 'and', 'a', 'to', 'in', 'for', 'is', 'we', 'that', 'this', 'on', 'are', 'an', 'with', 'as', 'by', 'be'
* Minimum no. of unique words accounting for 15% of the total number of words: 6



For Task 3:

* Total number of words in the collection : 304289
* Vocabulary size (number of unique words) : 11335
* Top 20 words in the ranking :
  'system', 'use', 'agent', 'base', 'data', 'inform', 'model', 'paper', 'queri', 'user', 'learn', '1', 'algorithm', 'problem', 'web', 'comput', 'applic', 'approach', 'present', 'databas'
* Stop-words out of the top 20 words : None (as all stop-words were removed while tokenizing)
* Minimum no. of unique words accounting for 15% of the total number of words: 23