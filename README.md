# 🎶 AI Music Genre Classifier

This repository contains a **machine learning project** that predicts the **genre of a song** based on its **audio features** such as tempo, energy, valence, danceability, and more. The audio features are fetched from **Spotify’s API**, providing real-world data for robust genre classification.



## 📑 Table of Contents

* [Introduction](#introduction)
* [Dataset](#dataset)
* [Objectives](#objectives)
* [Technologies Used](#technologies-used)
* [Installation](#installation)
* [Spotify API Setup](#spotify-api-setup)
* [Usage](#usage)
* [Model Overview](#model-overview)
* [Results and Evaluation](#results-and-evaluation)
* [Project Structure](#project-structure)
* [Future Work](#future-work)
* [Contributing](#contributing)
* [License](#license)
* [Contact](#contact)



## 📝 Introduction

Understanding **music genres** using audio features enhances music recommendation systems, playlist generation, and music analytics. This project uses **Spotify’s audio feature data** to train a genre classifier model that:

✅ Predicts song genres from numerical audio features

✅ Practices API integration for data retrieval

✅ Builds end-to-end machine learning pipelines for real applications



## 📚 Dataset

* **Source:** Fetched dynamically from **Spotify API** using song IDs or names

* **Features Include:**

  * tempo, energy, valence, danceability, acousticness, instrumentalness, liveness, loudness, speechiness, duration\_ms

* **Labels:** Song genre (pop, rock, hip hop, classical, etc.)

> *(For model training, curated datasets combining audio features and genre labels are used, then extended with live Spotify API data.)*



## 🎯 Objectives

✔️ Fetch audio features using **Spotify’s Web API**

✔️ Preprocess and clean data for model input

✔️ Train classification models to predict genres

✔️ Evaluate model performance with metrics and confusion matrices

✔️ Deploy the model for real-time predictions *(future extension)*



## ✨ Features

* Integration with **Spotify API** to fetch song features
* Data preprocessing and cleaning pipelines
* **Genre classification model** using scikit-learn classifiers (e.g. Random Forest, SVM, KNN)
* Model evaluation with accuracy, precision, recall, and F1-score
* *(Optional)* Interactive prediction for user-input song names



## 🛠️ Technologies Used

* **Python 3**
* **Spotify API (Spotipy)**
* **Pandas**
* **NumPy**
* **Scikit-learn**
* **Matplotlib**
* **Seaborn**
* **Jupyter Notebook**



## ⚙️ Installation

1. **Clone the repository**

```bash
git clone https://github.com/yourusername/AI_Music_Genre_Classifier.git
cd AI_Music_Genre_Classifier
```

2. **Create a virtual environment (optional)**

```bash
python -m venv venv
source venv/bin/activate  # macOS/Linux
venv\Scripts\activate     # Windows
```

3. **Install dependencies**

```bash
pip install -r requirements.txt
```

4. **Set up Spotify API credentials** (see below)



## 🔑 Spotify API Setup

1. Visit the [Spotify Developer Dashboard]()
2. Log in and create an **app** to obtain your **Client ID** and **Client Secret**
3. Set them as environment variables:

```bash
export SPOTIPY_CLIENT_ID='your_client_id'
export SPOTIPY_CLIENT_SECRET='your_client_secret'
```

*(Use `set` instead of `export` on Windows)*



## ▶️ Usage

1. Open `AI_Music_Genre_Classifier.ipynb` in Jupyter Notebook.
2. Run cells sequentially to:

* Authenticate Spotify API and fetch audio features
* Load training dataset and preprocess
* Train the classifier model
* Evaluate model performance
* *(Optional)* Test with live Spotify song inputs



## 🧠 Model Overview

* **Preprocessing:** Handling missing data, scaling numerical features
* **Models:**

  * Random Forest Classifier
  * Support Vector Machine (SVM)
  * K-Nearest Neighbors (KNN)
* **Evaluation:** Accuracy, Confusion Matrix, Classification Report



## 📊 Results and Evaluation

| Model         | Accuracy |
| ------------- | -------- |
| Random Forest | 85%      |
| SVM           | 80%      |
| KNN           | 77%      |

* Random Forest achieved the best performance in genre prediction.




## 📁 Project Structure

```
AI_Music_Genre_Classifier/
 ┣ data/
 ┃ ┗ training_data.csv
 ┣ models/
 ┃ ┗ genre_classifier.pkl
 ┣ AI_Music_Genre_Classifier.ipynb
 ┣ requirements.txt
 ┗ README.md
```



## 💡 Future Work

* Extend to **deep learning models** using Keras or PyTorch
* Deploy as a **Streamlit web app** for user input predictions
* Integrate **lyrics analysis** to improve genre classification
* Build a **recommendation system** based on genre and audio features



## 🤝 Contributing

Contributions are welcome to enhance models, data pipelines, or app deployment!

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/YourFeature`)
3. Commit your changes (`git commit -m 'Add YourFeature'`)
4. Push to your branch (`git push origin feature/YourFeature`)
5. Open a pull request



## 📄 License

This project is licensed under the MIT License. See [LICENSE](LICENSE) for details.



## 📬 Contact

**Ugama Benedicta Kelechi**
[LinkedIn](www.linkedin.com/in/ugama-benedicta-kelechi-codergirl-103041300) | [Email](mailto:ugamakelechi501@gmail.com) | [Portfolio](#)



### ⭐️ If you find this project insightful, please give it a star and share with data science, music tech, and ML learners!


