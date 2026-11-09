# RAG Project

A hands-on Retrieval-Augmented Generation (RAG) project in Python. It walks through the full RAG pipeline step by step: embeddings, vector search, retrieval and answer generation.

> Status: work in progress. I am extending the base project with my own features (see [My Additions](#my-additions)).

## What This Project Covers

- What RAG is and why it is useful
- How text embeddings capture meaning
- Vector databases and retrieval
- Generating answers from retrieved context with a language model
- Building a simple end-to-end RAG system
- Advanced RAG techniques

The `lessons/` folder explains each topic in order (01 to 06), and `utils/` holds the reusable code for embeddings, retrieval and generation.

## Project Structure

```
rag-project/
├── lessons/          # Step-by-step lessons (01-06)
├── utils/            # embeddings.py, retrieval.py, generation.py
├── examples/         # Example scripts
├── data/             # Sample data
├── demo.py           # Demo script
├── requirements.txt  # Python dependencies
├── .env.example      # Template for environment variables
├── QUICKSTART.md
├── STRUCTURE.md
└── GLOSSARY.md
```

## Getting Started

**Prerequisites:** Python 3.10+ and basic Python knowledge.

```bash
# 1. Clone the repository
git clone https://github.com/sujalsinghrajput8679-jpg/rag-project.git
cd rag-project

# 2. Create and activate a virtual environment (Windows)
python -m venv venv
venv\Scripts\activate

# 3. Install dependencies
pip install -r requirements.txt

# 4. Set up environment variables
copy .env.example .env
# Open .env and add your API key(s)

# 5. Run the demo
python demo.py
```

On Mac/Linux, use `source venv/bin/activate` and `cp .env.example .env` instead.

> Never commit your `.env` file. It is already listed in `.gitignore`.

## My Additions

Features I am adding on top of the base project:

- [ ] Support for multiple PDFs
- [ ] Simple web UI (Streamlit)
- [ ] My own dataset
- [ ] Deployment on AWS (Lambda + API Gateway)

## Tech Stack

- Python
- See `requirements.txt` for the full list of libraries
