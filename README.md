# Classification of Financial Complaints and LLM-Based Summarization

# 📚 Overview

For this project I've gathered customer complaints taken from the US Consumer Complaints Database. The original dataset has the written complaints, a product label and 20 other features. 
Here I use only the `'issued label'` and the text of the `'complaint'`. Keeping the label will enable us to validate how well the zero-shot classifier has done the job.

## :rocket: Features

1. **Zero-Shot Classification**  

Using the `'DeBERTa-v3-large`' model, complaint texts are classified into predefined categories (e.g., 'account closure', 'login issue', 'deposit/withdrawal') without the need for training a specific model. 

2. **Text Summarization**
   
The `'facebook/bart-large`' and `'t5-based`' models is used to generate a meaningful summary of the complaint text, retaining the main points while shortening the text for quicker understanding

- **Semantic Similarity (Cosine Similarity)**

The `'SentenceTransformer`' model computes the semantic similarity between the complaint text and predefined labels or other texts. This helps assess how closely related the text is to specific categories.











