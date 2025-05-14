# 🎵 Music Recommendation System

## 📊 Overview

This Music Recommendation System is a machine learning project that recommends songs based on textual features like song titles, artist names, and genres. It is built using **content-based filtering**, a technique that analyzes item descriptions instead of user behavior.

### 🧠 How It Works

The system uses the following steps to generate music recommendations:

1. **TF-IDF (Term Frequency-Inverse Document Frequency):**
   - This is a text vectorization method used to convert string data (like song titles and genres) into numerical format.
   - TF-IDF assigns higher weight to rare words and reduces the weight of common words.
   - In this project, it’s used to represent each song as a vector of important words.

2. **Cosine Similarity:**
   - After vectorizing the song data with TF-IDF, cosine similarity is used to measure how "similar" two songs are.
   - Cosine similarity computes the angle between two vectors. A smaller angle (closer to 1.0) means the songs are more alike.
   - This allows the system to recommend songs that are textually similar to the one the user likes.

### 📂 Dataset

The dataset contains song metadata such as title, artist, and genre. It is used for both training and generating recommendations.

🔗 Click here to download the dataset: (https://www.kaggle.com/datasets/notshrirang/spotify-million-song-dataset/data)


## 📁 Project Structure
```
music-recommender/
│
├── link to data/ kaggle link
├── venv/
├── preprocess.py
├── recommend.py 
├── main.py # Streamlit app
├── requirements.txt # Python dependencies
└── README.md # Project documentation
```


## 🚀 Features

- Collaborative filtering and/or content-based recommendation
- Clean and reproducible data preprocessing
- Streamlit web interface for user-friendly interaction
- Easy local and cloud deployment

---


## 🛠️ Getting Started

Follow these steps to run the project locally.

---

### ✅ 1. Clone the Repository

```
git clone https://github.com/your-username/music-recommender.git
cd music-recommender
```

### ✅ 2. Create and Activate a Virtual Environment
```
python3 -m venv venv
source venv/bin/activate
```

### ✅ 3. Install Dependencies
```
pip install --upgrade pip
pip install -r requirements.txt
```

### ✅ 4. Prepare and Train the Data
Make sure your dataset is in the data/ directory, then run:
```
python preprocess.py
```

### ✅ 5. Run the Streamlit App
```
streamlit run main.py
```

