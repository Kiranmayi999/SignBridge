# SignBridge: Interactive Indian Sign Language (ISL) Platform

SignBridge is a full-stack Indian Sign Language (ISL) learning and communication platform designed to improve accessibility between the deaf and hearing communities. By combining computer vision, deep learning, multilingual translation, and modern web technologies, the platform enables users to learn ISL, recognize hand gestures in real time, translate text into sign language, and communicate through accessible digital tools.

---

## 🚀 Key Features

### 🔤 Real-Time ISL Alphabet Recognition
Detects ISL alphabet gestures using computer vision and deep learning models, enabling sequential gesture recognition to generate text in real time.

### ✍️ Text-to-Sign Translation
Converts user-entered text into corresponding ISL sign videos, providing an intuitive visual representation for communication and learning.

### 🔊 Text-to-Speech
Converts translated or recognized text into spoken audio, improving accessibility and enhancing user interaction.

### 📚 Interactive ISL Learning Cards
Provides media-rich learning cards with visual demonstrations to help users learn ISL alphabets, words, and commonly used signs.

### 📖 Multilingual ISL Dictionary
Offers a searchable multilingual dictionary that links words and phrases to their corresponding ISL signs and video assets.

### 🎥 Media-Based Learning
Utilizes sign videos and educational media to provide an engaging visual learning experience for beginners and learners.

### 💻 Modern Web Interface
Built as a responsive Single Page Application (SPA) using React.js for seamless navigation across learning, translation, and communication modules.

---

# 💻 Tech Stack

## Frontend
- React.js
- React Router
- Material UI
- Axios
- React Webcam

## Backend
- Node.js
- Express.js
- Flask
- REST APIs

## AI & Computer Vision
- Python
- TensorFlow
- Keras
- OpenCV
- CVZone
- NumPy

## APIs & NLP
- Google Translate API
- Google Text-to-Speech API
- NLTK

## Data & Assets
- JSON-based multilingual dictionary
- ISL video assets
- Trained deep learning models

---

# 🏗️ System Architecture

```text
                 React Frontend
                       │
        ┌──────────────┴──────────────┐
        │                             │
 Node.js Backend               Flask ML Service
        │                             │
 Google APIs              TensorFlow + OpenCV
        │                             │
 Translation & TTS     ISL Gesture Recognition
```

---

# 📂 Repository Structure

```text
SignBridge/
├── Cards/
│   ├── backend/          # Node.js backend
│   ├── public/           # ISL videos, dictionary data, static assets
│   └── src/              # React components and pages
│
├── StoT/
│   └── backend/
│       ├── models/       # TensorFlow models
│       └── python/       # Gesture recognition scripts
│
└── README.md
```

---

# ⚙️ System Workflow

1. **Input Capture** – Users interact with the application through text input or a live webcam feed.

2. **Request Processing** – The React frontend routes requests to the appropriate backend service:
   - **Node.js** for translation and speech services.
   - **Flask** for gesture recognition and AI inference.

3. **AI Processing** – TensorFlow and OpenCV perform real-time ISL alphabet recognition, while backend services retrieve sign videos, translations, or speech output.

4. **Output Generation** – The application dynamically displays translated text, ISL sign videos, or synthesized speech, providing an interactive communication and learning experience.

---

# 🛠️ Installation

## Prerequisites

- Node.js
- npm
- Python 3.x
- Git

### Clone Repository

```bash
git clone https://github.com/your-username/SignBridge.git
cd SignBridge
```

### Install Frontend

```bash
cd Cards
npm install
npm start
```

### Install Node.js Backend

```bash
cd backend
npm install
node server.js
```

### Install Python Backend

```bash
cd ../../StoT/backend/python
pip install -r requirements.txt
python app.py
```

---

# ⚠️ Large Assets

Large binary assets are excluded from version control using `.gitignore`.

Required assets include:

- ISL video dataset
- Trained TensorFlow models
- Training media
- Dictionary assets

Place them inside:

```text
Cards/public/isl_videos/
Cards/public/train1/
StoT/backend/models/
```

---

# 🎯 Applications

- Indian Sign Language Learning
- Accessibility Assistance
- Inclusive Education
- Communication Support
- Assistive Technology

---
