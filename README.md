# PhysioGo

![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![Flutter](https://img.shields.io/badge/Flutter-02569B?style=flat&logo=flutter&logoColor=white)
![Firebase](https://img.shields.io/badge/Firebase-FFCA28?style=flat&logo=firebase&logoColor=black)
![MediaPipe](https://img.shields.io/badge/MediaPipe-0097A7?style=flat&logo=google&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white)

AI-powered physiotherapy app that lets patients do rehab exercises at home while getting real-time feedback on their form. Built as my Final Year Project at FAST-NUCES.

The core idea: a physiotherapist assigns exercises, the patient opens the app, the camera tracks their pose using MediaPipe, and the system counts reps, detects form errors, and reports progress back to the therapist. No clinic visit needed for routine sessions.

---

## ⚡ How it works

```mermaid
flowchart TD
    A[Patient starts exercise in app] --> B[Camera captures movement]
    B --> C[Frames sent to Python backend via WebSocket]
    C --> D[MediaPipe Pose Estimation]
    D --> E[Joint angle analysis and rep counting]
    E --> F[Form error detection]
    F --> G[Real-time feedback sent back to app]
    G --> H[Progress saved to Firebase]
    H --> I[Physiotherapist views progress on dashboard]

    style A fill:#1e293b,color:#f8fafc,stroke:#334155
    style D fill:#0f172a,color:#f8fafc,stroke:#6366f1
    style I fill:#0f172a,color:#f8fafc,stroke:#22c55e
```

---

## 🛠️ Stack

| Layer | Technology |
|---|---|
| Mobile App | Flutter (Android and Web) |
| Pose Estimation | MediaPipe |
| Backend | Python, FastAPI |
| Real-time Communication | WebSocket, WebRTC |
| Database and Auth | Firebase (Firestore, Authentication) |
| Deployment | Docker, Koyeb |

---

## 📸 Screenshots

<p align="center">
  <img src="https://github.com/ak-abdullah/FYP-Demo/blob/main/images/login.png?raw=true" width="220" />
  &nbsp;&nbsp;
  <img src="https://github.com/ak-abdullah/FYP-Demo/blob/main/images/sign%20up.png?raw=true" width="220" />
  &nbsp;&nbsp;
  <img src="https://github.com/ak-abdullah/FYP-Demo/blob/main/images/homepage.png?raw=true" width="220" />
</p>

<p align="center">
  <img src="https://github.com/ak-abdullah/FYP-Demo/blob/main/images/form.png?raw=true" width="220" />
  &nbsp;&nbsp;
  <img src="https://github.com/ak-abdullah/FYP-Demo/blob/main/images/settings.png?raw=true" width="220" />
  &nbsp;&nbsp;
  <img src="https://github.com/ak-abdullah/FYP-Demo/blob/main/images/PatientMessageList.png?raw=true" width="220" />
</p>

---

## 📁 Project structure

```
physiogo/
├── frontend/            # Flutter app
│   ├── lib/
│   │   ├── screens/     # patient and therapist views
│   │   ├── services/    # API and Firebase calls
│   │   └── models/      # data models
├── backend/             # Python pose estimation server
│   ├── pose/            # MediaPipe processing
│   ├── websocket/       # real-time frame handling
│   └── api/             # REST endpoints
├── assets/              # UI assets and icons
└── pubspec.yaml         # Flutter dependencies
```

---

## 🚀 Running locally

**Backend**

```bash
cd backend
pip install -r requirements.txt
uvicorn main:app --reload
```

**Frontend**

```bash
flutter pub get
flutter run
```

Add your `google-services.json` to `android/app/` before running.

---

## 💡 What I learned building this

Real-time pose estimation over WebSocket is harder than it looks. The main challenge was keeping latency low enough that feedback feels instant. Sending every frame was too slow so I implemented frame skipping and only processed every Nth frame based on the exercise type.

Rep counting is a geometry problem. Most exercises reduce to tracking a specific joint angle crossing a threshold. Getting that threshold right for different body types and camera angles took a lot of iteration.

WebRTC for the video stream and WebSocket for the feedback channel is the right split. Mixing both on one connection causes issues under load.

---

## 📬 Contact

Built by Abdullah Khalid

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/-abdullah-khalid)
[![Email](https://img.shields.io/badge/Email-D14836?style=flat&logo=gmail&logoColor=white)](mailto:abdullahkh.cs@gmail.com)
[![Portfolio](https://img.shields.io/badge/Portfolio-000000?style=flat&logo=github&logoColor=white)](https://ak-abdullah.github.io/Resume/)
