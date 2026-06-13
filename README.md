# Movie Recommendation System 🎬

A full-stack, high-performance Movie Recommendation Engine featuring a vector-optimized **FastAPI** backend and an interactive **Streamlit** frontend interface. The system uses advanced natural language processing (NLP) and information retrieval techniques to provide lightning-fast, content-based movie recommendations.

## 🚀 Features
* **Content-Based Filtering:** Recommends movies using TF-IDF (Term Frequency-Inverse Document Frequency) text vectorization on movie metadata.
* **Math Optimization:** Utilizes high-performance `scipy.sparse` matrix dot products and `numpy.argpartition` sorting adjustments to bypass CPU processing overhead and prevent server timeouts.
* **Dual-Service Architecture:** Completely decoupled frontend (Streamlit) and backend (FastAPI) infrastructure for production-ready design.
* **Hybrid Fallback:** Gracefully falls back to local pre-computed dataset matrices if external movie database API requests drop or encounter latency issues.

---

## 🛠️ Tech Stack
* **Frontend:** Streamlit, Python
* **Backend:** FastAPI, Uvicorn
* **Data Science & ML:** Pandas, NumPy, Scikit-Learn, Scipy
* **Database & Serialization:** Pickle (`.pkl`)

---

## 📂 Project Structure
```text
Movie Recommendation System/
├── app.py                  # Streamlit Web User Interface
├── main.py                 # FastAPI Backend Routing & Recommendation Logic
├── requirements.txt        # Project Dependencies
├── .gitignore              # Git Ignore File Configuration
├── README.md               # Project Documentation
└── [Data Assets/ Models]   # Compressed matrix files (df.pkl, tfidf_matrix.pkl)
