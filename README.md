# Q&A RAG Project

A question-answering system using Retrieval-Augmented Generation (RAG) with Amazon Electronics reviews dataset.

## Overview

This project demonstrates a complete RAG pipeline:

1. **Data Processing**: Loads and preprocesses Amazon Electronics reviews dataset
2. **Text Splitting**: Chunks documents for embedding
3. **Embeddings**: Uses HuggingFace sentence-transformers for vector embeddings
4. **Vector Store**: Creates FAISS index for similarity search
5. **LLM Integration**: Uses HuggingFace text-generation pipeline
6. **RAG Chain**: Combines retrieval and generation to answer user queries

## Dataset

- Amazon Electronics reviews TSV file (`amazon_reviews_us_Electronics_v1_00.tsv`)
- Contains 1000 reviews with product ID, title, star rating, and review body
- Additional mock price column added for demonstration

## Notebook

The main analysis and pipeline is documented in `question.ipynb`, which includes:

- Exploratory data analysis (EDA)
- Distribution of star ratings and mock prices
- Review length analysis
- Top 10 most reviewed products
- Vector store creation
- RAG chain setup
- Interactive recommendation function

## Usage

```bash
# Open the Jupyter notebook
jupyter notebook question.ipynb

# Or run the interactive chatbot
python3 -c "from main import main; main()"
```

## Project Structure

```
.
├── question.ipynb          # Main Jupyter notebook with RAG pipeline
├── amazon_reviews_us_Electronics_v1_00.tsv  # Dataset
├── .DS_Store
└── README.md               # This file
```

## Commit History

50 commits were made throughout July 2026, gradually building the notebook with markdown updates and code enhancements.

## Author

- **Name**: fiacredev
- **Email**: fiacredeveloper@gmail.com