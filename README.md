# 🔍 Face Recognition System using Python

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-27338e?style=for-the-badge&logo=OpenCV&logoColor=white)
![Status](https://img.shields.io/badge/Status-Active-brightgreen?style=for-the-badge)

A real-time **face recognition system** that identifies and labels known individuals from a live webcam feed. Built using Python's `face_recognition` library powered by **dlib's deep learning model**.

---

## 📸 Demo

```
[Live Webcam Feed]
  → Known faces loaded from image dataset
  → Each frame scanned for faces
  → Matched face labeled with name
  → Unknown faces labeled as "Unknown"
```

---

## ⚙️ How It Works

1. **Encoding Known Faces** — Loads reference images and computes 128-dimension face encodings
2. **Live Feed Capture** — Streams webcam frames in real-time
3. **Face Detection** — Detects face locations in each frame
4. **Encoding Comparison** — Compares live face encodings against known encodings using Euclidean distance
5. **Label Display** — Draws a bounding box and name label for each matched face

---

## 🛠️ Tech Stack

| Tool | Purpose |
|---|---|
| Python 3.x | Core programming language |
| face_recognition | Deep learning-based face encoding & matching |
| OpenCV | Real-time video capture and display |
| dlib | Underlying facial landmark detection |

---

## 📦 Installation

```bash
# Clone the repository
git clone https://github.com/arunkumararavindhakshan05-sudo/Face_recognition.git
cd Face_recognition

# Install dependencies
pip install face_recognition opencv-python
```

> ⚠️ **Note:** `face_recognition` requires `dlib` which needs CMake. On Windows, install [Visual Studio Build Tools](https://visualstudio.microsoft.com/visual-cpp-build-tools/) before running pip install.

---

## ▶️ Usage

1. Add reference images to the `known_faces/` folder, named as `PersonName.jpg`
2. Run the script:

```bash
python face_recognition_live.py
```

**Controls:**
- Press **`Q`** — Quit the camera feed

---

## 📁 Project Structure

```
Face_recognition/
│
├── known_faces/              # Folder with reference images (Name.jpg)
├── face_recognition_live.py  # Main script
└── README.md
```

---

## 🔮 Future Improvements

- [ ] Add a database to store and manage known faces
- [ ] Log recognition events with timestamps
- [ ] Build a web interface using Flask
- [ ] Add anti-spoofing (liveness detection)

---

## 👤 Author

**Arunkumar Aravindhakshan**
🔗 [LinkedIn](https://linkedin.com/in/arunkumar-aravindhakshan) | [GitHub](https://github.com/arunkumararavindhakshan05-sudo)
