# 🎬 Movie Recommendation System  
*A Content-Based Movie Recommender using Machine Learning & NLP*

🚀 **Live Application**  
👉 https://movie-recommender-system-idvh.onrender.com

---

## 📌 Project Overview
This project is a **content-based movie recommendation system** that suggests movies similar to a user’s selected movie.  
It uses **Natural Language Processing (NLP)** techniques and **cosine similarity** to analyze movie metadata and deliver relevant recommendations.

The application is built using **Python** and deployed as an interactive **Streamlit web app**.

---

## ✨ Key Features
- 🎯 Content-based movie recommendations
- 🧠 NLP-driven similarity computation
- 📊 Cosine similarity for ranking movies
- ⚡ Fast inference using a precomputed similarity matrix
- 🌐 Fully deployed and publicly accessible

---

## 🛠️ Tech Stack
- **Python**
- **Pandas**
- **NumPy**
- **Scikit-learn**
- **Pickle**
- **Streamlit**
- **Render (Deployment)**

---

## 📂 Project Structure

## 📂 Project Structure

```text
movie-recommender-system/
│
├── app.py                  # Streamlit application
├── movies_dict.pkl         # Preprocessed movie metadata
├── similarity.pkl          # Precomputed similarity matrix
├── requirements.txt        # Project dependencies
├── setup.sh                # Deployment configuration
├── .gitignore              # Git ignore rules
└── README.md               # Project documentation
```

---

## 🧠 How the Recommendation System Works
1. Movie metadata is converted into textual features
2. Feature vectors are generated using NLP techniques
3. **Cosine similarity** is computed between all movies
4. When a user selects a movie, the system recommends the **top similar movies**

To ensure fast performance, the similarity matrix is **precomputed and stored**.

---

## 📦 Model Artifact
The file `similarity.pkl` contains the **precomputed cosine similarity matrix** used by the application.

The matrix was **optimized (converted to float32)** to reduce memory usage while maintaining recommendation quality.  
This enables efficient inference and smooth deployment.

---

## ▶️ Run the Project Locally

### 1️⃣ Clone the repository
```bash
git clone https://github.com/anshswarn15/movie-recommender-system.git
cd movie-recommender-system
```

### Create and activate a virtual environment
```bash
python -m venv myenv
source myenv/bin/activate   # macOS / Linux
myenv\Scripts\activate     # Windows
```

### Install dependencies
```bash
pip install -r requirements.txt
```

### Run the application
```bash
streamlit run app.py
```
