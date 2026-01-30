<div align="center">
  <p>
    <img width="100%" src="assets/banner.png" alt="Object Tracking System Banner">
  </p>

<h1>Object Detection and Tracking System</h1>

A real-time object detection and multi-object tracking system using deep learning and computer vision.

</div>

---

## 🌍 Overview

This project implements a **real-time Object Detection and Tracking System** capable of:

- Detecting objects in images and video streams  
- Assigning unique IDs to objects  
- Tracking their movement across frames  
- Maintaining object identity over time  

It is designed for applications such as:
- Surveillance systems  
- Traffic monitoring  
- Autonomous vehicles  
- Crowd analysis  
- Sports analytics  

---

## ⚙️ Tech Stack

- **Deep Learning:** YOLO (Ultralytics)  
- **Tracking Algorithms:** SORT / DeepSORT / ByteTrack  
- **Backend:** Python  
- **Frameworks:** PyTorch, OpenCV  
- **Visualization:** Matplotlib, OpenCV GUI  

---

## 🚀 Installation & Setup

### 1. Clone repository
```bash
git clone https://github.com/yourusername/object-tracking-system.git
cd object-tracking-system
2. Create virtual environment
bash
Copy code
python -m venv venv
source venv/bin/activate   # Linux/Mac
venv\Scripts\activate      # Windows
3. Install dependencies
bash
Copy code
pip install -r requirements.txt
▶️ Run Application
Image detection
bash
Copy code
python detect.py --source image.jpg
Video tracking
bash
Copy code
python track.py --source video.mp4
Webcam tracking
bash
Copy code
python track.py --source 0
🔄 Workflow
Input video/image/webcam stream

YOLO detects objects frame-by-frame

Tracking algorithm assigns IDs

Objects are tracked across frames

Output video with bounding boxes and IDs

🧠 Algorithms Used
YOLO (You Only Look Once) – for object detection

SORT (Simple Online Realtime Tracking) – Kalman filter + Hungarian algorithm

DeepSORT – appearance-based re-identification

ByteTrack – robust multi-object tracking

📸 Sample Results
Detection Output

Tracking Output

🔐 Features
Real-time FPS processing

Multiple object tracking

Unique ID assignment

Occlusion handling

Works with video, webcam, and images

Export output video

🧪 Performance
FPS: ~25–40 (GPU)

Accuracy: YOLO pretrained on COCO

Tracking stability using ByteTrack/DeepSORT

📂 Project Structure
kotlin
Copy code
object-tracking-system/
│
├── data/
├── models/
├── track.py
├── detect.py
├── requirements.txt
├── assets/
└── README.md
📜 License
This project is for educational and research purposes only.

