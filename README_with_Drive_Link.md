# 🫀 ECG-Based Activity Recognition using Deep Learning

This project classifies physical activities from ECG signals using deep learning. Spectrogram images are generated from ECG data collected via wearable devices and used to train a convolutional neural network (CNN). The final system focuses on binary classification between Sitting and Jogging activities, achieving high accuracy (~93%).

---

## 📁 Project Structure

```bash
ecg-activity-classification/
├── Binary_ECG_Activity_Classification_Final.ipynb   # ✅ Final notebook (complete pipeline)
├── models/                                          # ✅ Saved models (.h5 files)
│   └── binary_model.h5
├── images_binary/                                   # ✅ Spectrograms for sitting/jogging
│   ├── sitting/
│   └── jogging/
├── scripts/
│   ├── ecg_gla_database.py                          # API to load ECG dataset
│   └── usage_example.py
├── requirements.txt
└── README.md
```

---

## 📊 Model Overview

| Model             | Type        | Classes         | Accuracy |
|------------------|-------------|------------------|----------|
| CNN (custom)     | Binary      | Sitting/Jogging  | ~93%     |

✅ Final implementation focuses on binary classification where ECG patterns are more distinct and performance is high.

---

## 🔬 Dataset

- 25 subjects
- 5 activities recorded: Sitting, Jogging, Hand Bike, Walking, Maths
- 2-minute sessions per activity
- 250 Hz, 24-bit resolution
- Spectrograms created from 5-second ECG segments

---

## 🔗 Full Project Folder (with models & data)

Due to size limits, the complete project folder (including trained model files and spectrogram data) is hosted externally:

📂 [Download the full project on Google Drive](https://drive.google.com/drive/folders/10g9FFipjUH_AqPSNVj89VyyqqS6RIvD_?usp=sharing)

After downloading:
- Place model files into the /models directory
- Use the notebook to run end-to-end classification

---

## ⚙️ How to Run

1. Clone the repository
2. Install dependencies:

```bash
pip install -r requirements.txt
```

3. Run the Jupyter Notebook:
```bash
jupyter notebook Binary_ECG_Activity_Classification_Final.ipynb
```

---

## 📉 Evaluation Metrics

- Precision, Recall, F1-Score
- Confusion Matrix
- Accuracy/loss plots per epoch

Example (Sitting vs Jogging):

- Accuracy: 93%
- Sitting F1: 0.92
- Jogging F1: 0.93

---

## 🚧 Future Work

- Improve multiclass performance (currently ~45%)
- Apply wavelet transforms or other time-frequency techniques
- Deploy model in real-time ECG classification system
