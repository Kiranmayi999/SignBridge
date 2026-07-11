# SignBridge

SignBridge is a full-stack Indian Sign Language (ISL) learning and communication platform designed to bridge the communication gap between the deaf and hearing communities. The platform combines computer vision, deep learning, and multilingual translation to enable real-time ISL alphabet recognition, Text-to-Sign translation, speech synthesis, and interactive learning through a modern web interface.

## Features

- **Real-Time ISL Alphabet Recognition:** Recognize ISL alphabet gestures using a webcam and convert sequential gestures into text.
- **Text-to-Sign Translation:** Convert text into corresponding ISL sign videos for visual communication.
- **Text-to-Speech:** Convert translated or recognized text into spoken audio for enhanced accessibility.
- **ISL Learning Cards:** Learn ISL through interactive learning cards and categorized educational content.
- **Multilingual Dictionary:** Search words across multiple languages and explore their corresponding ISL signs.
- **Media-Based Learning:** Improve understanding using sign videos and visual learning resources.

## Workflow

- Users can learn ISL, translate text, or perform real-time gesture recognition.
- Webcam frames are processed by the Python backend using TensorFlow and OpenCV for ISL alphabet recognition.
- Text translation requests are handled by the Node.js backend, which retrieves the corresponding sign videos and translations.
- The system displays translated text, sign videos, or synthesized speech based on the selected module.

## Tech Stack

### Frontend
- React.js
- Material UI
- React Router
- React Webcam
- Axios

### Backend
- Node.js
- Express.js
- Flask

### AI & Computer Vision
- Python
- TensorFlow
- Keras
- OpenCV
- CVZone

## Project Structure

```text
SignBridge/
├── Cards/
│   ├── backend/
│   ├── public/
│   └── src/
│
├── StoT/
│   └── backend/
│       ├── models/
│       └── python/
│
└── README.md
```

## Installation

### Clone Repository

```bash
git clone https://github.com/<your-username>/SignBridge.git
cd SignBridge
```

### Frontend

```bash
cd Cards
npm install
npm start
```

### Node.js Backend

```bash
cd Cards/backend
npm install
node server.js
```

### Python Backend

```bash
cd StoT/backend/python
pip install -r requirements.txt
python app.py
```

## Note

Large assets such as trained TensorFlow models, ISL video datasets, and media files are excluded from version control using `.gitignore`.

To run the project locally, place the required assets in:

```text
Cards/public/isl_videos/
Cards/public/train1/
StoT/backend/models/
```

## License

MIT License
