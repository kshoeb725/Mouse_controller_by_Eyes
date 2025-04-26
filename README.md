

# Eye-Controlled Mouse with Python 🖱️👁️

This project uses your **webcam** and the **MediaPipe FaceMesh** model to **control your mouse cursor using eye movements** and **click by blinking**. It's built with Python, OpenCV, and PyAutoGUI.

## 🔧 Features

- Move your mouse cursor by moving your ** Right eyes**.
- Left-click by **blinking your left eye**.
- Real-time video processing with **OpenCV**.
- Uses **MediaPipe FaceMesh** for facial landmark detection.

## 📦 Requirements

Make sure you have the following Python packages installed:

```bash
pip install opencv-python mediapipe pyautogui
```

## 🧠 How It Works

- The script uses the **FaceMesh** model from MediaPipe to detect facial landmarks.
- It tracks specific points around your **right eye** to move the mouse.
- It checks the **vertical distance between two eyelid landmarks** on the left eye to detect a blink and perform a click.

## ▶️ How to Run

1. Save the script in a file, e.g., `eye_mouse.py`
2. Run the script:

```bash
python eye_mouse.py
```

3. A window will open showing your webcam feed.
4. Move your **right eye** to move the mouse.
5. **Blink your left eye** to click.

## ⚠️ Notes

- The script uses the **474–478** landmark indices for the right eye and **145, 159** for blink detection.
- Works best in **good lighting** and when **only one face is visible** to the camera.
- The screen resolution is detected automatically using `pyautogui.size()`.

## 📷 Demo

*(You can add a video or GIF here showing it in action.)*

## 📄 License

This project is open-source and available under the MIT License.

