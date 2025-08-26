# Movie Semantic Search Assignment

This repository contains my solution for the **semantic search on movie plots** assignment using SentenceTransformers (`all-MiniLM-L6-v2`).

## Project Overview
The project builds a semantic search engine for movie plots. Given a query (e.g., *"spy thriller in Paris"*), the system finds and returns the most relevant movie plots from a dataset using embeddings and cosine similarity.

## Setup

1. Clone the repository:
   ```bash
   git clone https://github.com/mickeygems/movie-search-assignment.git
   cd movie-search-assignment
   ```

2. Create a virtual environment and activate it:
   ```bash
   python -m venv venv
   source venv/bin/activate    # On Linux/Mac
   venv\Scripts\activate     # On Windows
   ```

3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Run the Jupyter notebook:
   ```bash
   jupyter notebook movie_search_solution.ipynb
   ```

## Testing

To verify correctness, run the included unit tests:

```bash
python -m unittest tests/test_movie_search.py -v
```

This will check:
- Output format
- Top-N results length
- Similarity ordering
- Relevance of search results

## Usage

You can test the function directly inside the notebook:

```python
search_movies("spy thriller in Paris", top_n=3)
```


---

## File Structure

```
.
├── README.md                     # Instructions
├── movie_search.py               # Python module with 
├── movies.csv                    # Dataset of movies and plots
├── requirements.txt              # Dependencies
└── tests/
    └── test_movie_search.py      # Unit tests
```

---
