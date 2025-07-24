# 🎬 Movie Recommendation System

This is a content-based movie recommender built using **NLP and cosine similarity**. It recommends similar movies based on a given input title using metadata like genre, cast, director, keywords, etc.

---

## 🚀 Features
- Recommends top 5 similar movies based on content similarity
- Uses `CountVectorizer` for text vectorization and `cosine_similarity` for distance measurement
- Trained on a cleaned dataset of movie metadata
- Outputs serialized using `pickle` for deployment

---

## 🧠 Tech Stack
- Python
- Pandas, NumPy
- Scikit-learn
- Pickle

---

## 🛠️ How It Works

1. Data is cleaned and merged into a single 'tags' field per movie.
2. `CountVectorizer` transforms tags into feature vectors.
3. `cosine_similarity()` compares the input movie's vector to all others.
4. Top 5 similar movies (excluding the input) are returned.

---


## 🔍 Example Output

```python
recommend('Batman Begins')

# Output:
The Dark Knight  
Batman  
Batman v Superman: Dawn of Justice  
Batman & Robin  
City By The Sea

