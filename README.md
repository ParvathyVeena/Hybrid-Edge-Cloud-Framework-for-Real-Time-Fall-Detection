# Hybrid-Edge-Cloud-Framework-for-Real-Time-Fall-Detection
Real-time fall detection using YOLOv8, MediaPipe and Pushbullet API.


```markdown
# Hybrid Edge-Cloud Fall Detection System

A real-time fall detection application built with Python, OpenCV, and Computer Vision models integrated into a web interface. The system processes video streams to detect fall events and send automated alerts using API integrations.

---

## 🌟 Key Features

* **Real-Time Video Analytics:** Processes input video streams and webcam feeds for instantaneous fall detection.
* **Alert & Notification System:** Integrates Pushbullet API / webhook alerts to trigger immediate emergency notifications.
* **Web Dashboard:** Simple Flask-based web interface to monitor video feeds, view detection logs, and manage user authentication.
* **Modular Architecture:** Designed to run edge inferencing locally while offloading alert events to cloud notification services.

---


---


### Prerequisites

* Python 3.8 or higher installed on your system.
* A webcam (for real-time stream monitoring) or test `.mp4` video files.

### Installation & Setup


1. **Set up a virtual environment:**
```bash
# On Windows
python -m venv .venv
.venv\Scripts\activate

# On macOS/Linux
python3 -m venv .venv
source .venv/bin/activate

```


2. **Install dependencies:**
```bash
pip install -r requirements.txt

```


3. **Configure environment settings:**
* Rename `conf.json.example` to `conf.json` (or create `conf.json`).
* Add your API keys and configuration credentials:
```json
{
  "PUSHBULLET_API_KEY": "YOUR_PUSHBULLET_ACCESS_TOKEN",
  "CAMERA_SOURCE": 0
}

```





---

## 💡 Running the Application

Execute the core script to launch the detection engine and local web server:

```bash
python fall_detection.py

```

Open your browser and navigate to `http://127.0.0.1:5000` (or the port specified in terminal execution) to access the dashboard.

---
