# 🚗 Road Lane Localization Using OpenCV

## 📌 Project Overview

Road Lane Localization is a computer vision-based project that detects road lane markings from images and video streams using OpenCV. The system processes real-time video input to identify lane lines and overlay them on the road, which can assist in autonomous driving and lane departure warning systems.

This project was developed as a Mini Project at
**Vel Tech High Tech Dr. Rangarajan Dr. Sakunthala Engineering College**
Department of Information Technology

---

## 🎯 Objective

* Detect lane lines under different lighting and weather conditions.
* Perform real-time video frame processing.
* Improve robustness in challenging scenarios (sharp turns, faded lanes, shadows).
* Enhance detection using perspective transformation and thresholding techniques.
* Provide a base system for autonomous driving assistance.

---

## 🧠 Abstract

Lane detection is a critical component of autonomous driving systems. It provides essential semantic road information that helps in navigation and safety.

This project uses classical computer vision techniques such as:

* Edge Detection (Canny)
* Hough Transform
* Perspective Transformation
* Thresholding
* Camera Calibration

The system detects lane markings and overlays them onto the original video stream, improving road perception and assisting in lane guidance.

---

## 🔍 Existing System

* Uses Canny Edge Detection for preprocessing.
* Applies Hough Transform for line detection.
* Processes video frame-by-frame.
* Uses Region of Interest (ROI) masking.

### ❌ Limitations

* Limited adaptability to complex road conditions.
* Difficulty handling faded or non-standard lane markings.
* Limited contextual understanding (no traffic analysis).

---

## 🚀 Proposed Enhancements

* Improved robustness using adaptive thresholding.
* Lane direction detection.
* Traffic condition analysis (future scope).
* Enhanced accuracy in real-world scenarios.

---

## 🏗️ System Architecture

### Processing Pipeline:

1. Load Image / Video
2. Camera Calibration (Undistortion)
3. Perspective Transformation (Bird’s Eye View)
4. Thresholding
5. Edge Detection
6. Lane Line Detection
7. Overlay Lane on Original Frame
8. Display / Save Output

---

## 🧰 Technologies Used

* 🐍 Python
* 📷 OpenCV
* 🔢 NumPy
* 🎬 MoviePy
* 📊 Matplotlib
* 📓 Jupyter Notebook

---

## 💻 System Requirements

### Software:

* Python 3.x
* Jupyter Notebook
* OpenCV
* NumPy
* MoviePy
* Docopt

### Hardware:

* Multi-core Processor
* 8GB RAM (Recommended)
* High-resolution Camera (for real-time use)

---

## 📂 Project Structure

```
├── camera_cal/
├── CameraCalibration.py
├── Thresholding.py
├── PerspectiveTransformation.py
├── LaneLines.py
├── main.py
├── challenge_video.mp4
├── output.mp4
└── README.md
```

---

## ▶️ How to Run the Project

### 1️⃣ Install Dependencies

```bash
pip install opencv-python numpy matplotlib moviepy docopt
```

### 2️⃣ Run the Project

```bash
python main.py
```

### 3️⃣ Output

* Input: `challenge_video.mp4`
* Output: `output.mp4` (Lane detected video)

---

## 📸 Sample Output

The system overlays detected lane lines on the original road video frame in real-time.

---

## 📈 Methodology

* Convert image to grayscale
* Apply Gaussian Blur
* Perform Canny Edge Detection
* Apply ROI Mask
* Use Hough Transform for line detection
* Apply Perspective Transform
* Overlay final lane result

---

## 🔮 Future Scope

* Deep Learning-based lane detection (CNN / LSTM)
* Real-time traffic condition analysis
* Integration with autonomous vehicle systems
* Lane departure warning system
* Multi-lane tracking

---

## 📚 References

1. Haris, M.; Hou, J. *Obstacle Detection and Safe Navigation*, Sensors 2020.
2. Yang, W.; Zhang, X.; Lei, Q. *Lane Position Detection using LSTM*, Sensors 2020.
3. Mammeri, A.; Boukerche, A.; Tang, Z. *Real-Time Lane Localization*, 2015.
4. Sotelo, N.; Rodríguez, J.; Magdalena, L. *Color Vision-Based Lane Tracking*, 2004.


---

## 📌 Conclusion

This project demonstrates a reliable and structured approach to lane detection using classical computer vision techniques. It serves as a strong foundation for intelligent transportation systems and autonomous driving research.


