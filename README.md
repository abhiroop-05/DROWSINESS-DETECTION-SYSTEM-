
# 💤 Driver Drowsiness Detection System

An AI-powered system that monitors a driver’s eyes in real-time using a webcam feed to detect signs of drowsiness and trigger alerts. Built using deep learning with Keras and OpenCV, this system aims to reduce road accidents caused by fatigue.

---

## 🧩 Problem Statement

Driver fatigue is a leading cause of road accidents, especially during long-distance travel. Manually monitoring drowsiness is impractical. This system uses a deep learning model to automatically detect eye closure and trigger an audible alarm, helping prevent accidents due to drowsiness.

---

## 📹 Input Data

- **Live Webcam Feed**: Captures real-time video of the driver's face.
- **Eye Landmarks**: Extracted using OpenCV and dlib (or MediaPipe).
- **Eye Aspect Ratio (EAR)**: Used to determine eye closure over time.

---

## 🧠 Model Details

- **Architecture**: CNN trained to classify open vs closed eyes
- **Framework**: TensorFlow / Keras
- **Input Size**: 24×24 grayscale eye region
- **Layers**: Convolutional layers followed by Dense layers
- **Loss**: Binary Crossentropy
- **Optimizer**: Adam

### 🎯 Evaluation Metrics:
| Metric     | Value     |
|------------|-----------|
| Accuracy   | ~95%      |
| Precision  | ~94%      |
| Recall     | ~96%      |

---

## 🛠️ System Features

- 📹 Real-time webcam-based drowsiness monitoring
- 🔔 Audible alert if eyes remain closed beyond a threshold
- 📊 Eye aspect ratio (EAR) visualization
- 🧠 Lightweight and efficient Keras model
- ⚡ No internet required — fully offline system

---

## 🧪 Try It Locally

### 1️⃣ Clone this repository
```bash
git clone https://github.com/yourusername/drowsiness-detection.git
cd drowsiness-detection
```

### 2️⃣ Install dependencies
```bash
pip install -r requirements.txt
```

### 3️⃣ Run the notebook
```bash
jupyter notebook driver-drowsiness_notebook.ipynb
```

> Make sure your webcam is connected and working.

---

## 📦 Requirements

```bash
opencv-python
tensorflow
keras
numpy
pygame
matplotlib
```

You can save them using:

```bash
pip freeze > requirements.txt
```

---

## 🛠️ Technologies Used

- Python 3.x
- OpenCV
- Keras / TensorFlow
- NumPy
- Matplotlib
- Pygame (for sound alerts)
- Jupyter Notebook

---

## 🚧 Limitations & Future Work

- May not work well in low light or with glasses
- Could be extended with head pose estimation
- Integration with vehicle systems for automatic control (e.g., alert the car system)

---

⭐ **Star this project if it helped you stay awake!**
