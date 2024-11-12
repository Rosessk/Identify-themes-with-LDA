# Identify-themes-with-LDA

I used LDA to identify topics in which people appear to be optimistic or joyful.
There are 4 main steps:

1. Preprocessing
I applied preprocessing and used the TfidfModel class to compute TF-IDF vectors, instead of using a simple bag-of-words approach.

2. Model and Training
   
For training the LDA model, selecting the number of topics was important and required. I chose the number of topics based on the coherence score, which relies on the distributional hypothesis.

3. Topic Naming

After training the model, it was necessary to identify the top N words for each topic. These top words provide insight into the main themes of each topic. I will use the top 10 words with the highest probability in each topic. These words help to understand each topic's central theme and relevance within the document corpus. I assigned each topic a name based on my interpretation of themes.

4. Emotion Identification
   
I used the LDA model to analyse the probabilities of different topics appearing in documents labeled with various emotions. Each document was evaluated to determine which topic had the highest probability, reflecting the emotions associated with those documents
