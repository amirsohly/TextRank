# TextRank
This code snippet performs several tasks related to text summarization and PageRank algorithm:
## 1
It imports the necessary libraries: spacy for natural language processing, pytextrank for text summarization, and numpy for mathematical operations.
## 2
It defines a text variable containing a long passage of text.
## 3
It loads the English language model using spacy.load("en_core_web_sm").
## 4
It uses the summarize function from the gensim.summarization module to generate summaries of the text. The summarize function is called with different parameters to demonstrate different summarization techniques:
  #### summarize(text) generates a summary of the text using a default ratio of 0.2.
  #### summarize(text, split=True) generates a list of sentences that form the summary.
  #### summarize(text, ratio=0.5) generates a summary that contains 50% of the original text.
  #### summarize(text, word_count=100) generates a summary that contains 100 words.

## 5
It uses the keywords function from the gensim.summarization module to extract keywords from the text.
## 6
It defines a function called pagerank that implements the PageRank algorithm. The function takes a similarity matrix (sim_mat) as input and calculates the PageRank scores for each item in the matrix.
## 7
It initializes a similarity matrix (sim_mat) with zeros and assigns similarity values between items.
## 8
It calls the pagerank function with the sim_mat as input to calculate the PageRank scores.
## 9
It prints the PageRank scores (prob).
## 10
It generates a ranked list of sentence indexes based on the PageRank scores (ranked_sentence_indexes).
