# PhysioGo – AI-Powered Exercise Tracking for Physiotherapy 💪🤖

**PhysioGo** is an AI-based physiotherapy assistant that tracks and analyzes physical exercises in real-time using human pose estimation. Built using Flutter and Python, PhysioGo enables patients to perform rehab exercises at home while receiving instant posture feedback and progress tracking — promoting faster recovery and better outcomes.

---

## 🧠 Key Features

- 🎯 **Real-Time Pose Detection** using MediaPipe / MoveNet
- 🧍‍♂️ **Posture Correction Feedback**
- 📊 **Performance Analytics and Progress Tracking**
- 🌐 **Cross-platform App (Android/Web) built with Flutter**
- 🔁 **Python Backend for AI Pose Processing**
- 👨‍⚕️ **Designed for Remote Physiotherapy & Rehabilitation**

---






## 🛠️ Tech Stack

<div style="display: flex; align-items: center; gap: 100px;">
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/flutter/flutter-original.svg" alt="Flutter" width="60" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/python/python-original.svg" alt="Python" width="60" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/firebase/firebase-plain.svg" alt="Firebase" width="60" />
</div>

## Technologies Used



| Layer         | Technology            |
|---------------|------------------------|
| Frontend      | Flutter                |
| Backend       | Python, FastAPI / Flask |
| Pose Estimation | MediaPipe    |
| Communication | WebSocket / REST API   |
| Deployment    | Koyeb |

---

## 🚀 How It Works

1. The user opens the PhysioGo app and starts a guided exercise.
2. The device camera captures the user's movements.
3. Frames are sent to a Python backend for real-time pose estimation.
4. The app receives posture feedback and progress data.
5. Visual feedback is displayed to help the user correct form.

---

## 📸 Screenshots

*(Add screenshots or demo GIFs here showing the interface and pose detection in action)*

---

## 📁 Project Structure (simplified)

```bash
physiogo/
├── frontend/            # Flutter app
├── backend/             # Python + MediaPipe or MoveNet
├── models/              # Trained models / pose logic
├── assets/              # UI assets and icons
├── README.md            # This file
