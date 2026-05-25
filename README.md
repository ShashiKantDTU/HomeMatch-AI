# HomeMatch Application

## Overview
HomeMatch is an application designed to help buyers find their perfect real estate match. It leverages Large Language Models (LLMs) and Vector Databases to provide highly personalized property listings based on buyer preferences.

The application works in the following stages:
1. **Data Generation**: Uses an LLM to generate diverse and realistic real estate listings.
2. **Database Storage**: Embeds these listings and stores them in a ChromaDB vector database.
3. **Semantic Search**: Uses hard-coded buyer preferences to search the vector database and retrieve the most relevant properties.
4. **Augmented Response**: Uses an LLM to personalize the property description according to the buyer's preferences, without altering the factual details of the home.

## Prerequisites
- Python 3.10+
- An OpenAI API Key (or access to an OpenAI-compatible endpoint).

## Installation
Dependencies are listed in `requirements.txt`. Install them using:

```bash
pip install -r requirements.txt
```

## How to Run
1. Open `HomeMatch.ipynb` in your Jupyter Notebook environment (e.g. VS Code, Jupyter Lab).
2. Go to the first code cell and replace `"YOUR_OPENAI_API_KEY"` with your actual API key. If you are using Vocareum, uncomment the `OPENAI_API_BASE` line.
3. Run the cells in order.
   - The "Generating Real Estate Listings" cell will automatically save the generated output to `listings.json` in the same directory.
   - Proceeding cells will initialize the Vector Database, perform semantic search, and output personalized descriptions directly in the notebook outputs.

## Project Deliverables Included
- **`HomeMatch.ipynb`**: The main application code and examples.
- **`listings.json`**: Will be generated automatically upon running the notebook, providing synthetically generated listing data.
- **`README.md`**: This documentation file.
