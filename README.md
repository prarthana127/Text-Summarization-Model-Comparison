# Text-Summarization-Model-Comparison

## Project Overview
Text summarization is an essential task in natural language processing that involves reducing lengthy documents into clear and informative summaries. This project aims to compare different text summarization models, enabling users to identify the most suitable one for their specific requirements.

## Project Highlights
### Dataset: [Samsum dataset](https://huggingface.co/datasets/Samsung/samsum)

### Metrics Considered
The evaluation is based on several key metrics to assess the quality, coherence, and accuracy of the generated summaries:
- **BLEU Score** (Bilingual Evaluation Understudy)
- **BERT Score**
- **ROUGE-1, ROUGE-2, ROUGE-L** (Recall-Oriented Understudy for Gisting Evaluation)
- **Redundancy Score**

### Methodology - TOPSIS
The **Technique for Order of Preference by Similarity to Ideal Solution (TOPSIS)** is used for ranking the models. This method ensures a balanced evaluation by considering both the closeness to the ideal solution and the distance from the least favorable solution.

### Models Evaluated
The following pre-trained text summarization models are compared:
- `philschmid/bart-large-cnn-samsum`
- `facebook/bart-large-cnn`
- `philschmid/distilbart-cnn-12-6-samsum`
- `knkarthick/MEETING_SUMMARY`
- `google/bigbird-pegasus-large-arxiv`



## Results
The comparison results are ranked based on the TOPSIS method, considering the selected evaluation metrics. The final ranking helps identify the best-performing model for different summarization needs.
The following table presents the comparative evaluation of the models:

| Model | BLEU | BERT | ROUGE-1 | ROUGE-2 | ROUGE-L | Redundancy | TOPSIS Score | TOPSIS Rank |
|-------------------------------|------|------|---------|---------|---------|------------|--------------|-------------|
| `philschmid/bart-large-cnn-samsum` | 0.525 | 0.143 | 0.912 | 0.490 | 0.254 | 0.385 | 0.555 | 1 |
| `facebook/bart-large-cnn` | 0.458 | 0.057 | 0.874 | 0.334 | 0.110 | 0.239 | 0.386 | 4 |
| `philschmid/distilbart-cnn-12-6-samsum` | 0.512 | 0.139 | 0.909 | 0.471 | 0.239 | 0.362 | 0.547 | 2 |
| `knkarthick/MEETING_SUMMARY` | 0.519 | 0.137 | 0.910 | 0.468 | 0.236 | 0.355 | 0.546 | 3 |
| `google/bigbird-pegasus-large-arxiv` | 0.873 | 0.060 | 0.792 | 0.048 | 0.001 | 0.043 | 0.291 | 5 |
---------------------------------------------------------------------------------------------------------------









