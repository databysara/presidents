## WHAT WOULD A PRESIDENT SAY? 
Give the Presidents your sentence. See how they would rephrase it.


## Dataset:
US Presidential Speeches

## Challenge:
Given a random sentence as input, the program outputs top 3 similar sentences from different presidents.

## ML Problem:
Unsupervised, Text Similarity, Chosen Solution: Semantic Similarity

## Model Comparison:
WordEmbedding by gensim with GloVe algorithm VS Sentence Embedding with sentenceBERT

## Similarity Metric
Soft Cosine Measure / Cosine Similarity

## Results  
### Sentence Embedding Model using SentenceBERT
- The results were good! The top 3 sentences accurately conveyed the meaning of the input sentence.
    - query = "I believe I our children are our future."
- The top 3 results gave a cosine similarity of 0.889 to 0.956
- The model took over 24 hours to run.
- The long run time of the model prevented further exploration of the model for example with different queries..

### Word Embedding Model using GloVe  
- The results did not resemble the query in spite of the soft cosine similarity being 0.982 to 1.0.
    - query = 'I believe that the young people in America are our future.'
- The model was much less complex.
- The model did not convey the meaning of the input sentences.

### Limitations
- The dataset requires significant cleaning.
- Some cleaning was completed in the time aloted.