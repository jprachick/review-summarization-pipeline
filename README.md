# Review Summarization Pipeline

This project is an end-to-end natural language processing (NLP) pipeline that analyzes customer reviews for restaurants using the Yelp Open Dataset. It includes:

- Feature extraction from review text  
- Sentiment analysis at both review and feature level  
- Abstractive summarization using transformer models

The goal is to extract actionable insights from large volumes of unstructured text and generate summaries that help users quickly understand customer opinions.

## Project Structure
<pre><code>```bash
review-summarization-pipeline/
├── Yelp JSON/                       # Your downloaded dataset (no changes needed)
├── notebooks/
│   ├── 01_data_cleaning_eda.ipynb  # Load & explore Yelp restaurant reviews
│   ├── 02_feature_extraction.ipynb # Extract product/restaurant features
│   ├── 03_sentiment_analysis.ipynb # Sentiment per review & per feature
│   └── 04_review_summarization.ipynb # Generate summaries using transformer models
├── src/                            # (Optional later) Python modules for each step
├── README.md                       # Project description, goals, instructions
├── requirements.txt                # Python dependencies
├── .gitignore                      # Ignore data, virtual envs, and VS Code stuff
└── LICENSE                         # MIT license (default)
```
</code></pre>

## Dataset

[Yelp Open Dataset](https://www.yelp.com/dataset)  
Stored locally under `Yelp JSON/yelp_dataset/`.

## Getting Started

1. Clone the repository
2. Set up a virtual environment and install dependencies
3. Run notebooks in order

## License

This project is licensed under the MIT License.