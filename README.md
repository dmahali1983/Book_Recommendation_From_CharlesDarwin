# Book Recommendation System:
# Description:
To this purpose, we will develop the bases of a content-based book recommendation system, which will determine which books are close to each other based on how similar the discussed topics are. The methods we will use are commonly used in text- or documents-heavy industries such as legal, tech or customer support to perform some common task such as text classification or handling search engine queries.
# Read / load book details:
we need to load the content of these books into Python and do some basic pre-processing to facilitate the downstream analyses. We call such a collection of texts a corpus. We will also store the titles for these books for future reference and print their respective length to get a gauge for their contents.
# Find "Origin of Species":
For the next parts of this analysis, we will often check the results returned by our method for a given book. For consistency, we will refer to Darwin's most famous book: "On the Origin of Species." Let's find to which index this book is associated.
## Preprocessing:
# Tokenize the corpus:
As a next step, we need to transform the corpus into a format that is easier to deal with for the downstream analyses. We will tokenize our corpus, i.e., transform each text into a list of the individual words (called tokens) it is made of. To check the output of our process, we will print the first 20 tokens of "On the Origin of Species".
# Apply Stemming:
it is a common practice to use a stemming process, which will group together the inflected forms of a word so they can be analysed as a single item: the stem. In our On the Origin of Species example, the words related to the concept of selection would be gathered under the select stem.
As we are analysing 20 full books, the stemming algorithm can take several minutes to run and, in order to make the process faster, we will directly load the final results from a pickle file and review the method used to generate it.
# Bag of words:
we will create bag-of-words models (BoW) of each of our texts. The BoW models will represent our books as a list of all uniques tokens they contain associated with their respective number of occurrences.
# Identifying common words:
# Build TF-IDF Model:
we will use a tf-idf model (term frequency–inverse document frequency). This model defines the importance of each word depending on how frequent it is in this text and how infrequent it is in all the other documents. As a result, a high tf-idf score for a word will indicate that this word is specific to this text.
# Build cosine similary Distance Matrix:
we will use a tf-idf model (term frequency–inverse document frequency). This model defines the importance of each word depending on how frequent it is in this text and how infrequent it is in all the other documents. As a result, a high tf-idf score for a word will indicate that this word is specific to this text.

 
