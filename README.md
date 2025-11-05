# 🎬 Movie Recommender System

[![Streamlit App](https://img.shields.io/badge/Deployed%20on-Streamlit-brightgreen?logo=streamlit)](https://share.streamlit.io/)  
[![Python](https://img.shields.io/badge/Python-3.9%2B-blue.svg?logo=python)](https://www.python.org/)  
[![License](https://img.shields.io/badge/License-MIT-lightgrey.svg)](LICENSE)

A **content-based movie recommender system** built with **Streamlit**, designed to suggest movies similar to a user-selected title using precomputed similarity scores.

---

## 🚀 **Live Demo**
🔗 [**Click here to try the app on Streamlit Cloud**] https://zubii07-recommender-system-app-q0pzke.streamlit.app/


---

## 🧠 **About the Project**

This web app uses natural language processing and vector similarity techniques to recommend movies based on content (title, genres, and overview).  

It leverages:
- **Pandas** for data manipulation  
- **Scikit-learn / NLP techniques** for feature extraction  
- **Pickle** for serialized model storage  
- **Streamlit** for a simple, interactive UI

---

## 🧩 **How It Works**

1. The app loads preprocessed movie data (`movies.pkl`, `movies_dict.pkl`)  
2. It fetches a large **similarity matrix** (`similarity.pkl`) hosted externally via Dropbox  
3. When you select a movie, it finds the most similar titles using cosine similarity  
4. The recommendations are displayed instantly with movie posters and names

---

## 🗂️ **Project Structure**
```bash
movie-recommender/
│
├── app.py # Streamlit app entry point
├── movies.pkl # Preprocessed movie data
├── movies_dict.pkl # Metadata dictionary
├── requirements.txt # Dependencies
├── .gitignore # Ignored files and folders
├── README.md # Project documentation
└── model.ipynb (optional) # Notebook for model training
````

---

## 🧰 **Installation and Setup**

Clone this repository:
```bash
git clone https://github.com/Zubii07/Recommender-System.git
cd movie-recommender
````

Install dependencies:

```bash
pip install -r requirements.txt
```

Run the app locally:

```bash
streamlit run app.py
```

---

## ☁️ **Deployment**

This project is deployed on **Streamlit Cloud**.
During deployment:

* Small `.pkl` files are stored in the repo
* The large `similarity.pkl` is fetched dynamically from **Dropbox**

If you wish to redeploy:

1. Fork this repo or clone it
2. Push to your own GitHub account
3. Deploy via [Streamlit Cloud](https://share.streamlit.io)

---

## 📦 **Dependencies**

Main packages used:

* `streamlit`
* `pandas`
* `numpy`
* `scikit-learn`
* `requests`
* `pickle`

All dependencies are listed in [`requirements.txt`](./requirements.txt).

---

## 🧑‍💻 **Author**

**M Zohaib**

If you like this project, consider giving it a ⭐ on GitHub — it helps others find it!

---

## ⚖️ **License**

This project is open source and available under the [MIT License](LICENSE).


---

```



