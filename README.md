# Face Recognition System 👤

## 📌 Overview

This project is a **Face Recognition System** built using Python and OpenCV. It captures facial images using a webcam, trains a model on the dataset, and performs real-time face recognition.

The system works in **three main steps**:

1. Dataset Generation
2. Model Training
3. Real-time Face Recognition

---

## 🚀 Features

* Capture face dataset using webcam
* Train model using LBPH algorithm
* Real-time face recognition
* Detects unknown faces
* Simple pipeline using Jupyter Notebook

---

## 🛠️ Tech Stack

* Python
* OpenCV
* NumPy
* PIL (Python Imaging Library)
* Jupyter Notebook

---

## ⚙️ Working Process

### 1️⃣ Dataset Generation

* Captures images from webcam
* Detects face using Haar Cascade
* Converts to grayscale
* Stores images in `data/` folder

📁 Example format:

```bash
data/user.1.1.jpg
data/user.1.2.jpg
...
```

---

### 2️⃣ Model Training

* Reads images from `data/` folder
* Converts images to NumPy arrays
* Extracts IDs from file names
* Trains model using **LBPH Face Recognizer**
* Saves trained model as:

```bash
classifier.xml
```

---

### 3️⃣ Face Recognition

* Loads trained classifier
* Detects faces in real-time
* Predicts ID and confidence
* Displays:

  * Name → if recognized
  * "UNKNOWN" → if not recognized

---

## 📁 Project Structure

```bash
face-recognizer/
│── FACE RECOGNITION APP.ipynb
│── classifier.xml
│── haarcascade_frontalface_default.xml
│── README.md
│── .gitignore
```

---

## ▶️ How to Run

### Step 1: Install dependencies

```bash
pip install opencv-python numpy pillow
```

---

### Step 2: Generate Dataset

* Open notebook
* Run `generate_dataset()`
* It will capture ~200 images using webcam

---

### Step 3: Train Model

Run:

```python
train_classifier("data")
```

---

### Step 4: Run Face Recognition

* Run final section of notebook
* Webcam will open
* Press **Enter key** to exit

---

## 📸 Output

(Add screenshots of:

* Dataset collection
* Face detection
* Recognition result)

---

## ⚠️ Important Notes

* Dataset (`data/` folder) is not included to keep repository lightweight
* Make sure webcam is enabled
* Press **Enter (key code 13)** to stop camera

---

## 🔮 Future Improvements

* Add GUI interface
* Store multiple users with names
* Improve accuracy with deep learning
* Deploy as web application

---

## 👨‍💻 Author

Jyotirmaya Swain
