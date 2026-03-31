Here’s a clean, professional **`README.md`** you can directly use for your project 👇

---

# 🧠✋ Smart AI Drawing & Drowsiness Detection System

## 📌 Overview

This project is a **multi-functional AI-based system** that combines:

* 😴 **Drowsiness Detection (Eye Tracking)**
* ✋ **Hand Gesture Virtual Drawing**
* 🔢 **OCR-based Mathematical Expression Solver**

It uses computer vision and AI libraries to create an interactive real-time application using a webcam.

---

## 🚀 Features

### 😴 Drowsiness Detection

* Detects eye closure using **Eye Aspect Ratio (EAR)**
* Triggers alert if eyes remain closed for a threshold duration
* Plays an alarm sound using `pygame`

### ✋ Virtual Air Drawing

* Draw on screen using **hand gestures**
* Uses **MediaPipe Hands** for finger tracking
* Supports multiple colors:

  * 🔵 Blue
  * 🟢 Green
  * 🔴 Red
  * 🟡 Yellow
* Includes a **Clear Screen** button

### 🔢 OCR + Expression Solver

* Converts handwritten text (drawn on canvas) into digital text using **Tesseract OCR**
* Evaluates mathematical expressions automatically
* Displays result on screen

---

## 🛠️ Tech Stack

| Technology    | Purpose                              |
| ------------- | ------------------------------------ |
| `OpenCV`      | Computer vision & video processing   |
| `MediaPipe`   | Hand tracking                        |
| `dlib`        | Face detection & landmark extraction |
| `NumPy`       | Numerical computations               |
| `SciPy`       | Distance calculations                |
| `Pygame`      | Alarm sound system                   |
| `Pytesseract` | OCR (text recognition)               |

---

## 📂 Project Structure

```
project/
│── main.py
│── shape_predictor_68_face_landmarks.dat
│── beep.mp3
│── README.md
```

---

## ⚙️ Installation

### 1️⃣ Clone Repository

```bash
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
```

### 2️⃣ Install Dependencies

```bash
pip install opencv-python mediapipe numpy scipy dlib pygame pytesseract
```

### 3️⃣ Install Tesseract OCR

* Download from: [https://github.com/tesseract-ocr/tesseract](https://github.com/tesseract-ocr/tesseract)
* Add to system PATH

---

## 📥 Required Files

Download these before running:

* 📌 `shape_predictor_68_face_landmarks.dat`
  → [http://dlib.net/files/shape_predictor_68_face_landmarks.dat.bz2](http://dlib.net/files/shape_predictor_68_face_landmarks.dat.bz2)

* 🔊 Alert sound (`beep.mp3`)
  → Any short alarm sound

---

## ▶️ How to Run

```bash
python main.py
```

---

## 🎮 Controls

| Action       | Gesture                           |
| ------------ | --------------------------------- |
| Draw         | Move index finger                 |
| Stop Drawing | Bring thumb close to index finger |
| Select Color | Touch top bar                     |
| Clear Canvas | Click "CLEAR" button              |
| Exit         | Press `Q`                         |

---

## ⚡ How It Works

### 👁️ Eye Aspect Ratio (EAR)

* Calculates ratio of eye height to width
* If EAR < threshold → Eyes are closed
* Continuous closure → triggers alert

---

### ✋ Hand Tracking

* Detects 21 hand landmarks
* Uses index finger tip for drawing
* Tracks movement using deque (buffer)

---

### 🔤 OCR Processing

* Captures canvas periodically
* Converts image → text
* Evaluates math expressions using `eval()`

---

## ⚠️ Limitations

* OCR accuracy depends on handwriting clarity
* `eval()` can be unsafe for arbitrary input (use cautiously)
* Requires good lighting for detection
* Works best with a single user

---

## 🔮 Future Improvements

* Replace `eval()` with safe math parser
* Add gesture-based UI controls
* Improve OCR with deep learning models
* Add face recognition security layer
* Mobile or web deployment

---

## 👨‍💻 Author

**Abhyuday Singh**

---

## ⭐ Contribute

Feel free to fork this repo and improve it!
Pull requests are welcome.

---

## 📜 License

This project is for educational purposes.

---

If you want next level upgrade 🚀
I can also:

* Convert this into a **GitHub-ready repo with screenshots**
* Add **architecture diagram**
* Turn this into a **final-year project report / PPT**

Just tell me 👍
