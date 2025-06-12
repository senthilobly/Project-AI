
# AI Based Smart Home Safety System - ARIN

# 🏠 AI-Powered Home Safety System

This project is an AI/ML-based home safety solution using real-time face recognition, motion detection, and visitor classification. The system identifies the house owner, friends, and strangers (like couriers or potential intruders) using a camera feed. It also tracks visit frequency to categorize familiar faces automatically.

---

## 🚀 Features

- ✅ Detects and recognizes known faces (Owner, Family, Friend).
- 👀 Tracks visitors and classifies them as:
  - Owner / Family
  - Frequent Visitors (Friends)
  - Delivery Person / Stranger / Unknown
- 🔐 Detects intrusion based on motion and unknown presence.
- 📈 Maintains a visit history using `visitor_log.json`.
- 🧠 Uses **DeepFace** for facial recognition.
- 🎥 Works with webcam or camera feed.

---

## 🧠 How It Works

1. Loads known faces from `faces/` folder.
2. Captures video stream using OpenCV.
3. On detecting motion:
   - Recognizes the person using DeepFace.
   - Updates visit count in a log.
   - Categorizes them appropriately.
4. Displays alerts on terminal for unknown persons.

---

## 🛠 Installation

### 1. Clone the repo

```bash
git clone https://github.com/yourusername/home-safety-ai.git
cd home-safety-ai


### Install Dependencies

pip install opencv-python deepface imutils numpy
