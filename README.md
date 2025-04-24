# 🏆 Who Is That Athlete? - Image Classification with Flask

This project is a **machine learning-powered web application** that can identify famous sport celebrities from an image. Built with Python, Flask, OpenCV, and scikit-learn, it uses both raw pixel data and wavelet transforms to predict the correct athlete.

---

## 🖼️ Preview

> 📸 Add screenshots of your web app UI here!

| Home Page               | Prediction Result             |
|------------------------|-------------------------------|
| ![homepage](screenshots/home.png) | ![result](screenshots/result.png) |

---

## 👨‍💻 Tech Stack

- **Frontend**: HTML, CSS, JavaScript, Dropzone.js  
- **Backend**: Python, Flask  
- **ML Model**: Scikit-learn Pipeline (StandardScaler + SVC)  
- **Image Processing**: OpenCV (Haar Cascades), PyWavelets  
- **Deployment**: Localhost (development mode)  

---

## 🚀 Features

- Upload an image with a face  
- Detects faces with 2 eyes using Haar Cascades  
- Extracts features using wavelet transforms  
- Classifies the face among 5 trained athletes  
- Returns probabilities and highlights top match  

---

## 🎯 Classes

| Index | Athlete Name      |
|-------|--------------------|
| 0     | Lionel Messi       |
| 1     | Maria Sharapova    |
| 2     | Roger Federer      |
| 3     | Serena Williams    |
| 4     | Virat Kohli        |

---

## 📦 Project Structure
whoisthat-athlete/
│
├── artifacts/                # Trained model and class mappings
│   ├── saved_model.pkl
│   └── class_dictionary.json
│
├── server/                   # Flask backend and logic
│   ├── server.py
│   ├── util.py
│   ├── wavelet.py
│   └── opencv/
│       └── haarcascades/     # Haar cascade XML files
│
├── static/                   # Frontend assets
│   ├── app.js
│   └── app.css
│
├── b64.txt                   # Base64 image for testing
├── requirements.txt
└── README.md



---

## 🧪 How to Run This Project Locally

> ✅ Make sure you have Python installed (3.7 or later)

### 1️⃣ Clone the repository

```bash
git clone https://github.com/yourusername/whoisthat-athlete.git
cd whoisthat-athlete
```

## Create and activate a virtual environment (optional but recommended)
# Windows
python -m venv venv
venv\Scripts\activate

# Mac/Linux
python3 -m venv venv
source venv/bin/activate

##  Install the dependencies
pip install -r requirements.txt

## Run the Flask server
cd server
python server.py

The server will start at:
👉 http://127.0.0.1:5000

## 5️⃣ Open your browser and test
Open index.html (in your root or frontend folder).
Upload an image and click submit to see predictions!


🧠 Model Info
Input image size: 32x32

Features: Raw pixels + Wavelet-transformed coefficients

Model: Scikit-learn SVC in a pipeline

Format: Saved using joblib


## 🙌 Author
Aswin Roshan Rajendran
📧 aswinroshan17@gmail.com
📍 Paris, France

## ⭐️ Show Some Love
If you like this project, feel free to ⭐️ the repo or fork it for your own experiments!


