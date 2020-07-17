# Document_Type_Classifier
Used standard ML algorithms and NLP techniques to classify news articles belonging to the BBC dataset into one of the following categories - Business, Sports,Technology, Entertainment and Politics.
The dataset comprises of 2225 of 2225 articles, each labeled under one of 5 categories: business, entertainment, politics, sport or tech. The goal was to build a system that can accurately classify previously unseen news articles into the right category.

The data-preprocessig steps comprised of -
1) Removal of Stop Words - Words such as articles and some verbs in the English language are usually considered stop words as they do not contribute much to the meaning of a sentence.
   Used the stopwords list from NLTK's corpus.
   
2) Lemmatization - Used NLTK's Wordnet Lemmatizer to remove inflectional endings from words and return the dictionary form, known as the lemma.

Also used sklearn's chi2 package to perform Chi-Square analysis. This gives us the most correlated unigrams and bigrams in each category.

Used Term-Frequency Inverse-Document Frequency (TF-IDF) to convert text into feature vectors.

Finally, used three representative ML algorithms (Random Forest, Multinomial NB, Logistic Regression) to classify documents to one of the categories. 
Used K-Fold crosss-validation for the same.
