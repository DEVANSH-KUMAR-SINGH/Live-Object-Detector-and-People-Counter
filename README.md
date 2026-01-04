# Live Object Detector and People Counter

A real-time computer vision project that detects multiple objects and counts people using the **YOLOv8 object detection model** and **OpenCV**. This application can run through a webcam or video feed and is useful for crowd analytics, security monitoring, smart retail, automation systems, and occupancy tracking.

---

## 🚀 Features

- 🔍 Real-time object detection using **YOLOv8**
- 🧍 Automatic **people counting**
- 🎥 Works with **webcam or video input**
- 📊 Displays bounding boxes, labels, and confidence scores
- ⚡ Optimized for fast, real-time inference
- 🛠️ Modular code structure for easy customization

---

## 🧩 Tech Stack

- Python 3.10.9
- OpenCV  
- Ultralytics YOLOv8  
- cvzone  
- NumPy

---

## 📌 Use Cases

- Retail store footfall analytics
- Smart surveillance & security monitoring
- Event crowd measurement
- Workplace / facility occupancy tracking
- Automation & robotics applications

---

## 🧠 Learning Outcomes

- Understanding real-time object detection pipelines
- Integrating YOLO models with OpenCV
- Implementing object tracking and counting logic
- Working with video streams and performance optimization

---

## ⚙️ Environment, Tools, and GPU Setup

This project was developed in a structured Python environment with support for **GPU-accelerated YOLO inference**, modern development tools, and essential computer-vision libraries.

### ⚡ GPU Setup for Real-Time Performance
To accelerate YOLO inference on supported NVIDIA GPUs:
- Install the appropriate **NVIDIA GPU drivers** (e.g., RTX 4060 / similar)
- Install the **CUDA Toolkit (e.g., 11.x)** and **cuDNN libraries**
- Configure environment variables for CUDA paths
- Install **PyTorch with CUDA support** (matching your CUDA version)
- Verify YOLO runs using GPU — achieving significant speed improvements (~10–12 ms inference)

### 🛠️ Development Environment & Tools
- **Python** (recommended ~3.10, multiple versions manageable)
- **PyCharm Community Edition** (IDE)
- **Visual Studio Build Tools** (for CUDA / C++ dependencies on Windows)
- **CMake** (for compiling compatible libraries)

### 📦 Core Python Libraries
- **Ultralytics YOLOv8** — object detection framework  
- **OpenCV (cv2)** — video capture, frames processing, drawing utilities  
- **CVZone** — enhanced visualization overlays  
- **NumPy** — numerical / matrix operations  
- Additional dependencies are installed via `requirements.txt` (e.g., `scikit-image`, `filterpy`, etc.)

### 🗂️ Environment & Dependency Management
- Separate **virtual environments per project** (e.g., Python 3.7 vs 3.10)
- Install packages using `requirements.txt` to ensure reproducibility
- Maintain clean and portable project structure

### 📊 Model & Weights Handling
- YOLOv8 pretrained weights (nano, medium, large…)
- Weights are downloaded automatically by Ultralytics on first use
- Optionally stored in a custom **`yolo-weights/` folder** to avoid repeated downloads

---

## 🛠️ Installation

### 1️⃣ Clone the repository

```bash
git clone https://github.com/your-username/live-object-detector-people-counter.git
cd live-object-detector-people-counter
```

### 2️⃣ Create a virtual environment

```bash
python -m venv venv
source venv/bin/activate   # Mac / Linux
venv\Scripts\activate      # Windows
```

### 3️⃣ Install dependencies

```bash
pip install -r requirements.txt
```

### 📥 YOLOv8 Weights

- YOLOv8 pretrained weights are downloaded automatically the first time the model is initialized using the Ultralytics library — no manual download is required.
- If needed, you may also download .pt weight files directly from the official Ultralytics repository and place them in the project directory.

---

## ▶️ Usage

### Run Object Detection via Webcam

```bash
python yolo_webcam.py
```

### Run People Counter

```bash
python person_counter.py
```
To use a video file instead of a webcam, update the video source path in the script.

---

## 🤝 Contributions

Contributions and feature suggestions are welcome.
Feel free to open an issue or submit a pull request.

---

📜 License

This project is licensed under the MIT License.
See the LICENSE file for details.
