# Finding top 10 trending news topics
<br> Dataset is Herald news article in year 2015 - 2017 </br>
Approach
1. Preprocessing text
 - Remove non-en characters
 - Remove punctuation except apostrophe
 - Replace multiple space with a single space
 - Replace frequent words with a similar term
 - Convert to lowercase
 - Convert contraction
 - Lemmatize and remove stopwords
2. Summarize news body
  Alternative methods
  - TextRank 
  - WordFrequency (Extract sentence that contains high frequency words)
3. Considering a period of 7 days consecutively
4. Determine TF-IDF matrix
5. Clustering by DBSCAN
6. Sort the clusters by the number of element
7. Combine summary of each news in the same cluster together
8. Extract keywords using Yake
