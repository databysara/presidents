# presidents
WHAT WOULD A PRESIDENT SAY?
Give the Presidents your sentence. See how they would rephrase it.

### Dataset: 
US Presidential Speeches 

### Challenge: 
Given a random sentence as input, the program outputs top 3 similar sentences from different presidents.

### ML Problem:
Unsupervised, Text Similarity, 
Chosen Solution: Semantic Similarity

### Model:
WordEmbedding by gensim 
with GloVe algorithm

### Similarity Metric
Soft Cosine Measure

### Findings
1. May have performed better with more stop words. (Need to validate with more model runs.)
2. The quality (qualification) of the query matters with semantics.
    - E.g. when given an idiom it was hard to interpret model performance.
3. To better interpret results need to explore the data more. For e.g.
    - Is there a preference for longer corpora?
    - Is their a bias for older or newer corpora?
        - If yes, is that ok.
