Transformers

Transformers = Smart models that use attention to understand entire sentences at once, not word-by-word.

Transformers are a type of deep learning model designed to understand and generate sequences of data — like text, code, or even images.

They were introduced in the 2017 paper "Attention is All You Need" by Google.

Core Ideas:

Attention Mechanism:
Instead of reading input one word at a time (like RNNs), transformers look at all words at once and focus attention on the most important parts.

Parallel Processing:
They process all input tokens at the same time, making training much faster.

Encoding Relationships:
They understand the relationships between words, no matter how far apart they are.

Why Transformers Matter:
They power almost all modern AI models today — like BERT, GPT-4, T5, Gemini, and many more.

They made language understanding, translation, summarization, and AI chatbots much smarter and faster.


We'll be using the all-MiniLM-L6-v2 model here.

The all-MiniLM-L6-v2 model is an all-round (all) model trained on a large and diverse dataset of over 1 billion training samples and generates state-of-the-art sentence embeddings of 384 dimensions.

It is a language model (LM) that has 6 transformer encoder layers (L6) and is a smaller model (Mini) trained to mimic the performance of a larger model (BERT).

Potential use-cases include text classification, sentiment analysis, and semantic search.

Categorization: We'll use K-Means Clustering to categorize the data.

We did the following in the case study:

Encoded the dataset using the all-MiniLM-L6-v2 transformer model to generate embeddings of 384 dimensions

Queried the dataset to find news articles similar to the query text we passed

Categorized the news articles using K-Means Clustering on the transformer encodings

Compared the predicted categories of the news articles to the actual categories

Analyzed the incorrect predictions to understand where the model went wrong

Our model can correctly categorize 96% of the news articles.

one can try tagging news articles with more than one category for better categorization.

One can find the cluster centers to which the news article is the closest and assign one or more categories accordingly
Another approach that can be tried out would be fine-tuning the model to this particular data with category labels (one or more than one) to try and improve the overall performance.

In addition, the startup can use other transformer models to generate summaries of the news articles, which can provide a gist of the news content.
