# 🧤 Sign Language Converter with Smart Glove & Web App

A real-time Indian Sign Language translation system using a smart glove and web interface. This project aims to bridge the communication gap between the hearing and speech-impaired community and the rest of the world using sensor-based gesture recognition and AI.

---

## 🚀 Features

- ✋ **Smart Glove Hardware**: Detects hand gestures using flex sensors and sends data to the computer via serial communication.
- 🔊 **Real-Time Translation**: Converts signs to readable text and audible speech using Python and ML.
- 🌐 **Web Interface**: Streamlit-based dashboard to display live translations, user guide, and feedback system.
- 🧠 **Custom ML Models**: Trained on hand movement data for accurate recognition.
- 🔗 **End-to-End System**: Integrates hardware, software, and AI for a seamless user experience.

---

## 🛠️ Tech Stack

| Component         | Technology                                |
|------------------|-------------------------------------------|
| Language          | Python, Embedded C                        |
| Hardware          | Arduino, Flex Sensors, Accelerometer      |
| ML/AI             | Scikit-learn, Custom Classifiers          |
| Web App           | Streamlit                                 |
| Communication     | Serial (USB), PySerial                    |
| Visualization     | Matplotlib, Streamlit Charts              |
| Others            | NumPy, Pandas, MediaPipe (optional)       |

---

## 🧩 Hardware Requirements

- Arduino Uno/Nano
- 5 Flex Sensors (one for each finger)
- Jumper Wires
- Resistors (10kΩ)
- Bluetooth Module / USB Cable (for serial communication)
- Glove or hand strap for mounting sensors

---

## 🧪 How It Works

1. **Glove Setup**: Flex sensors detect finger bending and send analog signals to Arduino.
2. **Data Processing**: Arduino sends processed values over serial to the PC.
3. **Prediction**: Python reads serial data and classifies it using a pre-trained ML model.
4. **Output**: Result is displayed on the Streamlit web app and converted to speech using `pyttsx3`.

---


## 📦 Installation Guide

### ✅ Prerequisites
- Python 3.8 or above
- A webcam-enabled device

### 🔧 Setup Steps

**1. Clone the repository**
```bash
git clone https://github.com/your-username/SignSarthi.git
cd SignSarthi
```

**2. Install dependencies**
```bash
pip install -r requirements.txt
```

**3. Run the translator**
```bash
python app.py
```

**4. Open the Frontend**
Open the `index.html` file from the `frontend/` folder in your browser to interact with the UI built using HTML, CSS, and JavaScript.

---

## 🧠 Software Model Overview

- **MediaPipe**: Detects hand landmarks to generate input data.
- **CNN & LSTM Models**: Classify static and dynamic gestures respectively.
- **Text & Speech Output**: gTTS and REST APIs convert recognized ISL gestures into speech.
- **Multi-Language Translation**: Supports Indian languages for text output via external APIs.
- **Frontend Interface**: Built using HTML, CSS, and JavaScript for real-time interaction with the backend model.


```bash
# Clone the repository
git clone https://github.com/YourUsername/Sign-Language-Converter.git
cd Sign-Language-Converter

# Install Python dependencies
pip install -r requirements.txt

# Upload Arduino sketch
# (Use Arduino IDE or PlatformIO to flash code to Arduino)

# Run the web app
streamlit run app.py
