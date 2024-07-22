## Language Modeling with N-Grams

### Unigram, Bigram, and Trigram Models

Developed and evaluate three types of n-gram models: unigram, bigram, and trigram. Each model represents a different level of complexity and context in capturing the statistical properties of language:

- **Unigram Model**: This simplest model predicts each word independently based on its frequency in the training corpus. It does not consider the context of previous words.

- **Bigram Model**: This model considers pairs of consecutive words, providing a more contextual prediction compared to the unigram model. It captures some of the sequential structure of language.

- **Trigram Model**: The most complex of the three, this model considers triples of consecutive words. It captures richer context and is better at understanding sequences and structures in text.

### Smoothing Techniques

To handle the problem of zero probabilities for unseen n-grams in the test data, implemented smoothing techniques. Smoothing adjusts the probabilities of n-grams to account for the presence of unseen sequences, ensuring that the model can handle out-of-vocabulary words effectively.

- **K-Smoothing**: Used k-smoothing (add-k smoothing) to adjust unigram and bigram probabilities. The goal is to find the optimal value of k that minimizes perplexity, a measure of how well the model predicts the test data.

### Evaluation

The models are evaluated using perplexity, a metric that measures how well the language model predicts a given set of test data. Lower perplexity indicates better predictive performance. Compared the performance of the unigram, bigram, and trigram models and analyze how smoothing affects the perplexity.

### Data

The project utilizes the Brown Corpus, a well-known text corpus for linguistic research. It includes training, testing, and development datasets, which are processed to build and evaluate the language models.
