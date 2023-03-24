
Have you ever noticed how when you seach for a product on Amazon, similar products are shown below it. An example of this is when you search for self-help books, Amazon shows other self-help books that might interest you. This is the job of a recommendation system.

Recommendation Systems are a type of information filtering systems as they improve the quality of search results and provides items that are more relevant to the search item or are realted to the search history of the user. Recommendation system finds similarity between the product a user clicks on and the other products and then recommends if their is some sustainable similarity.

Youtube recommends videos and even decides which video to play next on autoplay. Facebook and Instagram recommend friends and pages to folow. Instagram also recommends reels that you might be interested in. Netflix recommends movies based on user taste and genre selection, it even recommends thumbnails of movies based on user data. Amazon, BigBasket and other E-Commerce websites recommend ads and products based on the items we buy or search for.

In this notebook, we will be building a product recommendor with detailed explanations.

So Let's Start!!! There are basically three types of recommender systems:-

Demographic Filtering- They offer generalized recommendations to every user, based on movie popularity and/or genre. The System recommends the same movies to users with similar demographic features. Since each user is different , this approach is considered to be too simple. The basic idea behind this system is that movies that are more popular and critically acclaimed will have a higher probability of being liked by the average audience.

Content Based Filtering- They suggest similar items based on a particular item. This system uses item metadata, such as genre, director, description, actors, etc. for movies, to make these recommendations. The general idea behind these recommender systems is that if a person liked a particular item, he or she will also like an item that is similar to it.

Collaborative Filtering- This system matches persons with similar interests and provides recommendations based on this matching. Collaborative filters do not require item metadata like its content-based counterparts.


TF-IDF stands for term frequency-inverse document frequency.

What is TF(Term Frequency):

Term frequency works by looking at the frequency of a particular term you are concerned with relative to the document. There are multiple measures, or ways, of defining frequency: Number of times the word appears in a document (raw count).

Term frequency adjusted for the length of the document (raw count of occurences divided by number of words in the document). Logarithmically scaled frequency (e.g. log(1 + raw count)). Boolean frequency (e.g. 1 if the term occurs, or 0 if the term does not occur, in the document).

What is IDF (inverse document frequency)?

Inverse document frequency looks at how common (or uncommon) a word is amongst the corpus. IDF is calculated as follows where t is the term (word) we are looking to measure the commonness of and N is the number of documents (d) in the corpus (D)..
The denominator is simply the number of documents in which the term, t, appears in.

IDF = log(N/df)

where N is the total number of documents in the corpus, and df is the number of documents that contain the term
