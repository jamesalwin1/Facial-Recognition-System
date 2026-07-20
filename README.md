# 🎯 Facial Recognition System using Deep Learning

![Python](https://img.shields.io/badge/Python-3.12-blue)
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.20-orange)
![OpenCV](https://img.shields.io/badge/OpenCV-4.x-green)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-1.6-red)

## 📖 Overview

This project implements a **Facial Recognition System** using Deep Learning and Machine Learning techniques. The system detects human faces using **MTCNN**, extracts facial embeddings using **EfficientNetB0**, and recognizes identities using a **Support Vector Machine (SVM)** classifier.

The project is trained on the **Labeled Faces in the Wild (LFW)** dataset and demonstrates a complete facial recognition pipeline from data preprocessing to prediction.

---

# 🚀 Features

- Face Detection using MTCNN
- Deep Feature Extraction using EfficientNetB0
- Multi-Class Face Recognition using SVM
- Automatic Dataset Processing
- Face Embedding Generation
- Model Saving and Loading
- Classification Report
- Confusion Matrix
- Prediction on Unseen Images

---

# 🛠️ Technologies Used

| Technology | Purpose |
|------------|---------|
| Python | Programming Language |
| TensorFlow | Deep Learning |
| TensorFlow Hub | EfficientNetB0 |
| OpenCV | Image Processing |
| MTCNN | Face Detection |
| NumPy | Numerical Computing |
| Scikit-learn | Machine Learning |
| Matplotlib | Visualization |

---

# 📂 Dataset

**Dataset:** Labeled Faces in the Wild (LFW)

The dataset contains facial images of people captured under different:

- Pose
- Lighting
- Expression
- Background

For this implementation:

- **423 unique identities** were used for training.
- Each identity contains **5–20 facial images** after filtering.

---

# 🔄 Project Workflow

```
LFW Dataset
      │
      ▼
Face Detection (MTCNN)
      │
      ▼
Face Cropping
      │
      ▼
Image Preprocessing
      │
      ▼
Feature Extraction
(EfficientNetB0)
      │
      ▼
Feature Vector
      │
      ▼
Support Vector Machine
      │
      ▼
Face Prediction
```

---

# 🧠 Model Architecture

### Face Detection

- MTCNN

### Feature Extraction

- EfficientNetB0 (TensorFlow Hub)

### Classifier

- Support Vector Machine (SVM)

---

# 📊 Results

### Training Configuration

| Parameter | Value |
|-----------|-------|
| Dataset | LFW |
| Persons Used | 423 |
| Feature Extractor | EfficientNetB0 |
| Classifier | SVM |
| Accuracy | **21.28%** |

Although the overall accuracy is **21.28%**, the model was trained on **423 different identities**, making the classification task significantly more challenging than models trained on smaller subsets of the dataset.

---

# 📸 Screenshots

## Prediction Demo

![Prediction Demo](screenshots/prediction_demo.png)

---

## Training Accuracy & Confusion Matrix

![Accuracy](screenshots/training_accuracy.png)

---

# 📁 Project Structure

```
Facial-Recognition-System/
│
├── Facial_Recognition.ipynb
├── README.md
├── requirements.txt
├── .gitignore
│
├── model/
│   └── face_recognition_model.pkl
│
└── screenshots/
    ├── prediction_demo.png
    └── training_accuracy.png
```

---

# ⚙️ Installation

## Clone Repository

```bash
git clone https://github.com/jamesalwin1/Facial-Recognition-System.git
```

Move into the project folder:

```bash
cd Facial-Recognition-System
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Launch the notebook:

```bash
jupyter notebook Facial_Recognition.ipynb
```

---

# 📥 Pre-trained Model

The trained model (`face_recognition_model.pkl`) is not included in this repository because it exceeds GitHub's file size limit.

Download it from Google Drive:

**🔗 Google Drive:**  
`https://drive.google.com/file/d/1KH1gC_CujIhtMqLhVHIoWiUgoveMxTa3/view?usp=drive_link`

After downloading:

1. Create a folder named `model`.
2. Place `face_recognition_model.pkl` inside the `model` folder.
3. Run the notebook normally.

---

# 🔮 Future Improvements

- Real-time webcam recognition
- Unknown face recognition
- Face verification
- Attendance Management System
- Flask/Streamlit Web Application

---

# 👨‍💻 Author

**James Alwin**

B.Tech – Artificial Intelligence and Data Science

GitHub: https://github.com/jamesalwin1

---

# ⭐ Support

If you found this project helpful, consider giving it a ⭐ on GitHub.
