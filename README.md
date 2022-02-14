# presidents
WHAT WOULD A PRESIDENT SAY?
Give the Presidents your sentence. See how they would rephrase it.

## NOTE:
At the time of this commit sentenceBERT is still running.

### Dataset: 
US Presidential Speeches 

### Challenge: 
Given a random sentence as input, the program outputs top 3 similar sentences from different presidents.

### ML Problem:
Unsupervised, Text Similarity, 
Chosen Solution: Semantic Similarity

### Model Comparison - (Update):
WordEmbedding by gensim with GloVe algorithm VS
Sentence Embedding with sentenceBERT

### Similarity Metric
Soft Cosine Measure / Cosine Similarity

### Latest Findings (Update)
1. The dataset needs to be cleaned for e.g. in addition to President Speeches, the corpus included:
    - correspondence, notes about the speeches including the presidents' names,  the dates and location of the speeches etc., audience response.
    - some of these could be removed easily, others may take considerable time.
2. I removed duplicate sentences in preparation for the Sentence Embedding Model.
    - This was not done for Word Embedding. So did not keep all variables controlled in interest of time. 
3. There is an increase in the length of presidential speeches over time.
    - The John Adams inaugural address is an outlier.
    - E.g. when given an idiom it was hard to interpret model performance.

### Initial Findings
1. May have performed better with more stop words. (Need to validate with more model runs.)
2. The quality (qualification) of the query matters with semantics.
    - E.g. when given an idiom it was hard to interpret model performance.
3. To better interpret results need to explore the data more. For e.g.
    - Is there a preference for longer corpora?
    - Is their a bias for older or newer corpora?
        - If yes, is that ok.
