✋ Hand Gesture Volume Control Using Computer Vision

A real-time hand gesture–based system volume controller built using OpenCV, MediaPipe, and PyCaw.
This project allows users to control their system volume by simply adjusting the distance between their thumb and index finger.

🎯 Features

🎥 Real-time webcam hand tracking

✋ Accurate thumb–index finger distance detection

🔊 Smooth system volume control (Windows)

📊 Visual volume bar and percentage indicator

⚡ Low latency & intuitive interaction

🖥️ Touch-free Human–Computer Interaction (HCI)

🛠️ Technologies Used

Python

OpenCV – Webcam capture & visualization

MediaPipe Hands – Hand landmark detection

PyCaw – System audio control (Windows)

NumPy – Interpolation & calculations

Math – Distance measurement

📷 How It Works

Webcam captures live video.

MediaPipe detects hand landmarks.

The distance between:

Thumb tip (Landmark 4)

Index finger tip (Landmark 8)
is calculated.

Distance is mapped to system volume range.

System volume changes dynamically in real time.

A visual volume bar and percentage is displayed.

📐 Gesture Logic
Gesture	Action
Fingers close	Low volume
Fingers far apart	High volume
Fingers very close	Visual alert (red line)
🚀 Installation
1️⃣ Clone the repository
git clone https://github.com/hemanth1325/Gesture-Volume-Control-master
cd hand-gesture-volume-control

2️⃣ Create virtual environment (recommended)
python -m venv venv
source venv/bin/activate   # Windows: venv\Scripts\activate

3️⃣ Install dependencies
pip install opencv-python mediapipe numpy pycaw comtypes


⚠️ Note: PyCaw works only on Windows OS.

▶️ Running the Application
python app.py

Controls:

Show your hand in front of the webcam

Adjust thumb–index finger distance to change volume

Press Q to quit

📊 Visual Indicators

🔲 Vertical volume bar

🔢 Volume percentage display

🔴 Red line appears when fingers are very close

🧠 Key Concepts Implemented

Hand landmark extraction

Euclidean distance calculation

Linear interpolation (numpy.interp)

System-level audio control

Real-time computer vision pipeline

🌱 Future Enhancements

✋ Multi-hand support

🖥️ Cross-platform volume control

🔈 Gesture-based mute/unmute

🎚️ Smooth volume damping

🎨 UI improvements

📱 Gesture-controlled media player

📜 License

This project is licensed under the MIT License.

🙌 Acknowledgments

MediaPipe – Real-time hand tracking

OpenCV – Computer vision framework

PyCaw – Windows audio control API
