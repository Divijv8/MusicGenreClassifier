# 🎵 Music Genre Classification System

This project is an **end-to-end Music Genre Classification system** that uses **machine learning / deep learning techniques** to automatically classify audio tracks into their respective music genres based on extracted audio features.

The goal of the project is to demonstrate how **signal processing + machine learning** can be combined to solve a real-world audio classification problem.

---

## 🚀 Project Motivation

With the massive growth of digital music platforms, organizing and recommending music manually has become impractical.  
Music genre classification helps in:

- 🎧 Music recommendation systems  
- 📂 Automatic music library organization  
- 🎼 Music information retrieval (MIR)  
- 🤖 Intelligent audio-based applications  

This project focuses on building a **clean, interpretable, and effective genre classification pipeline** rather than using black-box APIs.

---

## 🧠 How the System Works

### 1️⃣ Audio Processing
- Raw audio files are loaded from the dataset
- Each audio file is split into manageable segments (if required)
- Audio signals are converted into numerical representations using **feature extraction**

---

### 2️⃣ Feature Extraction
The following **audio features** are extracted from each track:

- **MFCCs (Mel-Frequency Cepstral Coefficients)**  
- **Chroma Features**
- **Spectral Centroid**
- **Spectral Bandwidth**
- **Zero Crossing Rate**
- **RMS Energy**

These features capture:
- Timbre  
- Pitch distribution  
- Frequency characteristics  
- Rhythm and energy  

📌 Feature extraction converts raw sound waves into a format suitable for ML models.

---

### 3️⃣ Model Training
- Extracted features are used as input to the classification model
- The model learns patterns that differentiate music genres
- The trained model predicts the genre of unseen audio samples

---

### 4️⃣ Genre Prediction
- For a new audio file:
  - Features are extracted
  - Passed through the trained model
  - The most probable genre is returned as output

---

## 🏗️ Model Architecture

Depending on implementation, the project uses:

### 🔹 Machine Learning Approach
- **Classifier**: Random Forest / SVM / Logistic Regression
- Well-suited for structured feature vectors
- Easy to interpret and fast to train

### 🔹 Deep Learning Approach (if used)
- **Neural Network (Dense / CNN)**
- Learns complex feature interactions
- Better performance on large datasets

📌 **Why Feature-Based Models?**
- Computationally efficient
- Works well with limited datasets
- Easier to debug and explain than raw-audio deep models

---

## 🧪 Dataset

- **Dataset Used**: GTZAN Music Genre Dataset
- **Number of Genres**: 10  
  - Blues  
  - Classical  
  - Country  
  - Disco  
  - Hip-Hop  
  - Jazz  
  - Metal  
  - Pop  
  - Reggae  
  - Rock  

### Preprocessing Steps:
- Audio normalization
- Fixed-duration sampling
- Feature scaling (Standardization)

---

## 🖥️ Tech Stack

### Core Technologies
- **Python**
- **NumPy**
- **Pandas**
- **Librosa** (Audio Processing)
- **Scikit-learn**
- **TensorFlow / Keras** (if deep learning used)
- **Matplotlib / Seaborn** (Visualization)

---

## 📊 Evaluation Metrics

The model performance is evaluated using:
- **Accuracy**
- **Precision**
- **Recall**
- **F1-score**
- **Confusion Matrix**

These metrics help analyze:
- Genre-wise performance
- Misclassification patterns
- Model reliability

---

## 📁 Project Structure

```text
music-genre-classification/
│
├── data/
│   └── genres_original/
│
├── notebooks/
│   └── music_genre_classification.ipynb
│
├── models/
│   └── trained_model.pkl
│
├── utils/
│   └── feature_extraction.py
│
├── requirements.txt
└── README.md
```

## ⚙️ Setup Instructions

### 1️⃣ Clone the Repository

```bash
git clone [https://github.com/your-username/music-genre-classification.git](https://github.com/your-username/music-genre-classification.git)
cd music-genre-classification
```

### 2️⃣ Create Virtual Environment (Recommended)
```bash
python -m venv venv
```
## Activate Environment
Linux / macOS:
```bash
source venv/bin/activate
```
Windows:
```bash
venv\Scripts\activate
```

### 3️⃣ Install Dependencies
```bash
pip install -r requirements.txt
```

### 4️⃣ Run the Notebook / Script
```bash
jupyter notebook
```

Open the notebook and run cells sequentially to:
-> Extract features
-> Train the model
-> Evaluate results

### 🧩 Future Improvements
🎙️ Real-time audio genre prediction
🧠 CNNs on Mel-Spectrograms
📱 Web or mobile-based interface
🎶 Multi-label genre classification
🔊 Noise-robust training

### 📌 Key Learnings
Audio data requires signal processing knowledge
Feature quality directly impacts model performance
Classical ML models can perform surprisingly well on audio tasks
Proper evaluation is critical in multi-class classification problems

### 🤝 Acknowledgements
GTZAN Dataset
Librosa documentation
Scikit-learn community

### ⭐ If you found this project useful, consider starring the repository!


```
