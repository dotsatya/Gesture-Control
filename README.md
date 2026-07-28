# Gesture Control Presenter 🖐️

Control Google Slides with hand gestures using your laptop camera. This project combines Computer Vision and AI to detect simple hand poses and trigger presentation actions in real time.

## ✨ Features

- Detects one hand from a webcam feed
- Recognizes basic gestures for slide navigation
- Works with Google Slides in a browser
- Uses MediaPipe, OpenCV, and PyAutoGUI
- Beginner-friendly for learning AI + computer vision

## 🧠 Gesture Controls

| Gesture | Action |
| --- | --- |
| Open palm | Next slide |
| Three fingers | Previous slide |
| Two fingers | Start slideshow |
| Fist | Exit slideshow |

## 🛠️ Technologies Used

- Python
- OpenCV
- MediaPipe
- PyAutoGUI

## 📦 Installation

### 1. Clone the repository

```bash
git clone https://github.com/dotsatya/Gesture-Control.git
cd gesture-control
```

### 2. Install dependencies

On Windows:

```bash
py -m pip install -r requirements.txt
```

On macOS/Linux:

```bash
python3 -m pip install -r requirements.txt
```

### 3. Download the hand model

```bash
python setup_models.py
```

If you are on macOS or Linux, use `python3` instead of `python`.

## ▶️ Run the App

```bash
python main.py
```

Press `q` in the webcam window to quit the app.

## 🎯 How to Use

1. Open Google Slides in your browser.
2. Start the slideshow mode.
3. Run the Python application.
4. Place your hand in front of the webcam.
5. Use the supported gestures to control the presentation.

## 💻 System Notes

- For macOS, allow Accessibility and Input Monitoring permissions for Terminal, VS Code, or your IDE so keyboard shortcuts can work.
- The current implementation uses a Mac-style shortcut to start the slideshow. On Windows or Linux, you may need to adjust the shortcut in the code if it does not work as expected.
- Good lighting and a clear camera view improve gesture detection.

## 📂 Project Structure

```bash
gesture-control/
├── main.py
├── README.md
├── requirements.txt
├── setup_models.py
└── models/
    └── hand_landmarker.task
```

## 🧩 How It Works

1. The webcam feed is captured with OpenCV.
2. MediaPipe detects hand landmarks.
3. The app counts visible fingers.
4. Each gesture is mapped to a keyboard action.
5. PyAutoGUI sends the corresponding key press to control Google Slides.

## 🔮 Possible Improvements

- Swipe gestures
- Laser pointer mode
- Volume control
- Multi-hand support
- Custom gesture training

## 👨‍💻 Built With AI + Computer Vision

A simple hands-free interaction system powered by real-time gesture recognition.