# Extractive Summarizer Model

To identify and extract the most important sentences from a text based on statistical relevance (TF-IDF scores), creating a concise summary while preserving the original sentence structure.

**Implementation Steps:**

**Text Tokenization:**

Use NLTK to split the text into sentences and further into words.

**Preprocessing:**

Remove stopwords using NLTK's English stopword list.
Retain only alphanumeric words and convert them to lowercase for uniformity.

**TF-IDF Scoring:**

Utilize Scikit-learn’s TfidfVectorizer to calculate the importance of each word in the context of its sentence.
Compute scores for sentences by summing the TF-IDF values of all words within the sentence.

**Sentence Ranking:**

Rank sentences by their scores in descending order.

**Summary Generation:**

Select the top N sentences based on user input (e.g., 3 sentences).
Combine the selected sentences into a summary.

**Required Libraries:**

**nltk** - for text tokenization and stopword removal.

**scikit-learn** - for TF-IDF computation.

**numpy** - for numerical operations like sorting.
