# Manary — Quran Reciter & Verse Identification System

Manary is an AI-powered system that analyzes Quran recitation audio to identify the reciter, detect the corresponding Surah and Ayah, and provide Tafsir (verse explanation). The system integrates speech processing, machine learning, and external APIs to deliver an end-to-end intelligent pipeline.

---

## 🎯 Features

- **Reciter Identification**  
  Classifies Quran reciters using MFCC features and ECAPA-TDNN speaker embeddings.

- **Verse Detection**  
  Converts recitation audio into Arabic text using Whisper (ASR).

- **Verse Matching**  
  Matches transcribed text with a Quran dataset to identify Surah and Ayah.

- **Tafsir Retrieval**  
  Retrieves verse interpretation using Quran Cloud API / Groq API.

- **End-to-End Pipeline**  
  Audio → Preprocessing → Feature Extraction → Reciter → Verse → Tafsir

---

## 📊 Dataset

- **Audio Dataset**
  - 5 Quran reciters  
  - 6 audio recordings per reciter (balanced dataset)

- **Reciters Included**
  - Abdul Basit Abdul Samad  
  - Mishary Al-Afasy  
  - Abdulrahman Al-Sudais  
  - Islam Sobhi  
  - Additional reciter included  

- **Text Dataset**
  - Quran dataset (CSV format) with Surah and Ayah information  

---

## 🛠️ Technologies Used

- Python  
- Librosa — Audio preprocessing & MFCC extraction  
- Scikit-learn — Classification models  
- Whisper — Arabic speech-to-text (ASR)  
- SpeechBrain (ECAPA-TDNN) — Speaker embeddings  
- Quran Cloud API / Groq API — Tafsir retrieval  
- NumPy / Pandas — Data processing  

---

## 📦 Installation

1. Clone the repository:
```bash
git clone https://github.com/lamaalekresh9/manary-quran-reciter-and-verse-identification.git
cd manary-quran-reciter-and-verse-identification
---
2. Install dependencies:
pip install numpy pandas librosa scikit-learn
---

Install dependencies:
notebook/Manary_labeled_final.ipynb
---

Run all cells sequentially
Provide an audio input
The system will output:
Reciter name
Surah
Ayah
Tafsir explanation

## 🚀 Usage

1. Open the notebook:  
   `notebook/Manary_labeled_final.ipynb`

2. Run all cells sequentially  

3. Provide an audio input  

4. The system will output:
- Reciter name  
- Surah  
- Ayah  
- Tafsir explanation  

---

## 🧠 Methodology

### 1. Audio Preprocessing
- Convert to mono  
- Resample to 16 kHz  
- Trim audio segments  

### 2. Feature Engineering
- MFCC features for baseline model  
- ECAPA-TDNN embeddings for advanced representation  

### 3. Model Training
- Logistic Regression for reciter classification  
- ECAPA-based embeddings for improved performance  

### 4. Verse Identification
- Whisper converts audio → text  
- Text matched with Quran dataset  

### 5. Tafsir Integration
- Retrieve tafsir via API after verse identification  
- Enhances interpretability and user understanding  

### 6. Evaluation
- Accuracy, Precision, Recall, F1-score  
- Confusion matrix  
- Retrieval performance  

---

## ⚠️ Limitations

- Small dataset (may lead to overfitting)  
- Audio quality differences introduce noise  
- ASR errors (e.g., similar phrases like Bismillah) affect verse matching  

---

## 📌 Notes

- Large files are handled using Git LFS  
- Notebook preview may not render on GitHub but works in Colab/Jupyter  

---

## 👩‍💻 Authors

- Lama Binekresh  
- Yara Altwajari  
- Norah Aljasser  

Prince Sultan University

Authors
Lama Binekresh
Yara Altwajari
Norah Aljasser

Prince Sultan University
