# 🎬 Movie Recommendation System

A **content-based movie recommendation system** built using **TF-IDF similarity**, **FastAPI**, and **TMDB API**.

This project allows users to search for movies and get:

* 🎯 Similar movie recommendations (TF-IDF)
* 🎭 Genre-based recommendations
* 🖼️ Movie posters from TMDB
* 🔎 Movie search functionality

---

# 🚀 Features

✅ Content-based movie recommendation
✅ TF-IDF vector similarity
✅ TMDB API integration
✅ FastAPI backend
✅ Real-time movie search
✅ Poster & movie metadata support

---

# 🛠️ Tech Stack

* **Python**
* **FastAPI**
* **Scikit-learn**
* **Pandas**
* **NumPy**
* **TMDB API**
* **HTTPX**
* **Pydantic**
* **Streamlit**

---

# 📂 Project Files

| File                  | Description             |
| --------------------- | ----------------------- |
| `main.py`             | FastAPI backend server  |
| `app.py`              | Application entry point |
| `movies.ipynb`        | Model training notebook |
| `df.pkl`              | Processed movie dataset |
| `indices.pkl`         | Title index mapping     |
| `tfidf.pkl`           | TF-IDF vectorizer       |
| `tfidf_matrix.pkl`    | TF-IDF matrix           |
| `movies_metadata.csv` | Original movie dataset  |
| `requirements.txt`    | Python dependencies     |

---

# ⚙️ Installation & Setup

## Step 1 — Clone Repository

```bash
git clone https://github.com/Vighnesh1240/Movie-Recommendation.git
cd Movie-Recommendation
```

---

## Step 2 — Create Virtual Environment

```bash
python -m venv movie_recommender_env
```

Activate:

```bash
movie_recommender_env\Scripts\activate
```

---

## Step 3 — Install Dependencies

```bash
pip install -r requirements.txt
```

---

## Step 4 — Add TMDB API Key

Create `.env` file:

```text
TMDB_API_KEY=your_api_key_here
```

Get API key from:

https://www.themoviedb.org/

---

## ▶️ Run FastAPI Server

```bash
uvicorn main:app --reload
```

Open in browser:

```
http://127.0.0.1:8000/docs
```

---

# 🎯 Example API Endpoints

## Health Check

```
GET /health
```

---

## Search Movie

```
GET /tmdb/search?query=avatar
```

---

## TF-IDF Recommendation

```
GET /recommend/tfidf?title=Avatar
```

---

## Genre Recommendation

```
GET /recommend/genre?tmdb_id=550
```

---

# 🧠 How It Works

1. Movie metadata is processed using **TF-IDF vectorization**
2. Cosine similarity finds similar movies
3. TMDB API fetches posters and details
4. FastAPI serves recommendations

---

# 📊 Dataset Used

* TMDB Movies Dataset
* Includes metadata like:

  * Title
  * Overview
  * Genres
  * Ratings

---

# 🖼️ Future Improvements

* Streamlit frontend UI
* User-based recommendations
* Hybrid recommendation system
* Deployment to cloud

---

# 👨‍💻 Author

**Vighnesh**

GitHub:
https://github.com/Vighnesh1240

---

# ⭐ If You Like This Project

Give it a **star ⭐ on GitHub**!
