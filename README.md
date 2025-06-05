# 📱 PhysioGo – AI-Powered Exercise Tracking for Physiotherapy 💪🤖

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

<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/flutter/flutter-original.svg" alt="Flutter" width="60" />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/python/python-original.svg" alt="Python" width="60" />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/firebase/firebase-plain.svg" alt="Firebase" width="60" />




## 🧰 Technologies Used



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
<h2 align="center">📥 Login Screen</h2>
<p align="center">
  <img src="https://github.com/ak-abdullah/FYP-Demo/blob/main/images/login.png?raw=true" alt="Login" width="350" />
</p>

<h2 align="center">📝 Sign Up Screen</h2>
<p align="center">
  <img src="https://github.com/ak-abdullah/FYP-Demo/blob/main/images/sign%20up.png?raw=true" alt="Sign Up" width="350" />
</p>

<h2 align="center">🏠 Homepage</h2>
<p align="center">
  <img src="https://github.com/ak-abdullah/FYP-Demo/blob/main/images/homepage.png?raw=true" alt="Homepage" width="350" />
</p>

<h2 align="center">📝 Form Screen</h2>
<p align="center">
  <img src="https://github.com/ak-abdullah/FYP-Demo/blob/main/images/form.png?raw=true" alt="Form" width="350" />
</p>

<h2 align="center">⚙️ Settings Screen</h2>
<p align="center">
  <img src="https://github.com/ak-abdullah/FYP-Demo/blob/main/images/settings.png?raw=true" alt="Settings" width="350" />
</p>
<h2 align="center">💬 Chat Screen</h2>
<p align="center">
  <img src="https://github.com/ak-abdullah/FYP-Demo/blob/main/images/PatientMessageList.png?raw=true" alt="Settings" width="350" />
</p>




---

## 📁 Project Structure (simplified)

```bash
physiogo/
├── frontend/            # Flutter app
├── backend/             # Python + MediaPipe
├── assets/              # UI assets and icons
├── splash.yaml/         # Splash Screen
├── pubspec.yaml         # Dependencies
