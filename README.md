# Review Summarization Pipeline

This project demonstrates how to generate abstractive summaries of real Amazon product reviews using transformer-based language models. The goal is to evaluate multiple pre-trained models and compare their ability to generate coherent, relevant, and concise summaries of customer sentiment.

## Models Compared

- **PEGASUS (google/pegasus-xsum):** Optimized for short news-style summaries. Tends to hallucinate if the input is long or off-domain.
- **BART (facebook/bart-large-cnn):** Performs well on product reviews and longer content. More extractive and grounded in input text.

## Sample Output

| Model | Summary Behavior |
|-------|------------------|
| **PEGASUS** | Hallucinates content (e.g. invented journalists/books) |
| **BART** | Faithful to input, better captures review content |

View detailed comparisons in [`outputs/model_comparison_summaries.csv`](outputs/model_comparison_summaries.csv)

## Tech Stack

- Python 3.10
- PyTorch 2.1.2
- Transformers 4.37.2
- Jupyter Notebook
- pandas / tqdm

## Repo Structure
review-summarization-pipeline/
├── notebooks/
│   └── 01_exploration_and_summarization.ipynb
├── outputs/
│   └── model_comparison_summaries.csv
├── data/
│   └── Reviews.csv
├── README.md
└── requirements.txt
