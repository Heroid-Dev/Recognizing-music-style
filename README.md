# 🎵 Music Genre Classification with Machine Learning


## 📘 Overview
With the growth of digital technologies and the increasing amount of multimedia data, **automatic music analysis** has become an interesting and practical area in **data science** and **machine learning**.
The goal of this project is to **design and implement an AI system to classify music genres** using audio features extracted from music tracks.


## 🧠 Project Steps


### 1. Data Collection and Preprocessing
- Data was sourced from the [GTZAN Dataset](https://www.kaggle.com/code/jvedarutvija/music-genre-classification/input).
- The dataset contains tracks from various genres, such as pop, jazz, classical, metal, etc.
- The following features were extracted from each track:
- **MFCCs**
- **Spectrogram**
- **RMS**
- **Tempo**
- **Mean Time Pattern**
- **Boss Power**
- **Number Strong Note**


### 2. Model Training
Three machine learning models were trained for genre classification:


| Algorithm | Description | Accuracy |
|-----------|-------------|----------|
| K-Nearest Neighbors (KNN) | Predicts genre based on nearest neighbors | ≈ 43% |
| Decision Tree | Builds a decision tree based on features | ≈ 40% |
| Neural Networks (TensorFlow) | Multi-layer dense neural network | 54% – 60% |


### 3. Results & Analysis
- Neural networks outperformed the other two models.
- Adding features like `zero_crossing_rate`, `rolloff`, and `spectral_contrast` reduced accuracy, so they were excluded in the final version.
- Deep models are better at learning complex patterns in multimedia data.


## 📊 Technologies Used
- **Python** 🐍
- **TensorFlow**
- **scikit-learn**
- **NumPy & Pandas**
- **Librosa** (audio feature extraction)
- **Matplotlib / Seaborn**


## 🧩 Folder Structure
```
├── Data/
│ └── genres_original/
├── Features/
├── Models/
├── Notebooks/
│ └── music_genre_classification.ipynb
├── README.md
└── requirements.txt
```


## ⚙️ How to Run
1. Clone the repository:
```bash
git clone https://github.com/username/music-genre-classification.git
cd music-genre-classification
```
2. Install dependencies:
```bash
pip install -r requirements.txt
```
3. Open the Jupyter Notebook:
```bash
jupyter notebook
```
4. Run the cells to train models and visualize results.


## 🏁 Conclusion
- Neural networks achieve higher accuracy for music genre classification.
- Feature selection plays a crucial role in model performance.
- Removing less informative features can improve results.


[GTZAN Music Genre Dataset (Kaggle)](https://www.kaggle.com/code/jvedarutvija/music-genre-classification/input)
