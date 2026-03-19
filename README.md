## InvisioCloak

> **Disappear in real time. Pure computer vision, zero deep learning.**

A real-time invisibility cloak built with Python and OpenCV — no ML models, no GPU required. Just clean background subtraction, morphological masking, and alpha blending magic.

---



##  Features

- 🎥 Real-time invisibility effect via webcam
- 🧠 Background subtraction using median frame averaging (120 frames)
- 🎭 Morphological masking + Gaussian blending for seamless effect
- 🎚️ Live adjustable invisibility — 0% to 100%
- 📸 Screenshot capture with a single keypress
- 💻 Runs on any standard webcam — no GPU needed

---

## 🛠️ Tech Stack

![Python](https://img.shields.io/badge/Python-3.8+-blue?style=flat&logo=python)
![OpenCV](https://img.shields.io/badge/OpenCV-4.x-green?style=flat&logo=opencv)
![NumPy](https://img.shields.io/badge/NumPy-latest-orange?style=flat&logo=numpy)

---

## ⚙️ Installation & Usage

### 1. Clone the repository
git clone https://github.com/akshaykunjumon8606-crypto/invisio-cloak.git
cd invisio-cloak

### 2. Install dependencies
pip install opencv-python numpy

### 3. Run
python invisio_cloak.py

### 4. Controls

| Key | Action |
|-----|--------|
| + | Increase invisibility |
| - | Decrease invisibility |
| S | Save screenshot |
| Q | Quit |

---

## 🔬 How It Works

1. Background Capture — Step out of frame; the app captures 120 frames and computes a median background.
2. Person Detection — Each live frame is compared to the background using absolute pixel difference + thresholding.
3. Mask Refinement — Morphological operations remove noise and fill gaps; Gaussian blur softens edges.
4. Invisibility Blending — Person pixels are replaced with background pixels using adjustable alpha blending.

---

## 📁 Project Structure

invisio-cloak/
├── 04.py   # Main application
├── README.md
└── invisible0.png/       # Saved screenshots

---




