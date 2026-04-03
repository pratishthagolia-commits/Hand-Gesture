# ✊🖐✌️ Rock Paper Scissors — Hand Gesture Edition

A real-time Rock Paper Scissors game that uses your webcam and computer vision to read your hand gestures. No buttons, no clicking — just you, your hand, and the camera.

Built with Python, OpenCV, and MediaPipe.

---

## How It Works

The game tracks your right hand through your webcam and recognizes three gestures:

| Gesture | Move |
|--------|------|
| ✊ All fingers closed | Stone |
| 🖐 All fingers open | Paper |
| ✌️ Index + middle fingers up | Scissors |

Each round follows a **Rock → Paper → Scissors** countdown. When **SHOW NOW!** appears, lock in your move. The computer picks randomly, and the winner is decided instantly on screen.

The game runs for **3 rounds** and shows the final score at the end.

---

## 🫶 Korean Finger Heart

Flash a Korean finger heart anytime during the game — thumb and index finger crossed and close together, other fingers down — and the game will respond with a little message back.

---

## Requirements

```
Python 3.8+
opencv-python
mediapipe
numpy
```

Install dependencies:

```bash
pip install opencv-python mediapipe numpy
```

---

## Run

```bash
python rps.py
```

Make sure your webcam is connected. Press **Q** anytime to quit.

---

## Notes

- Only your **right hand** is tracked
- Gestures are read during the short **SHOW NOW!** window at the end of each countdown
- Lighting and background can affect detection accuracy — a plain background works best
