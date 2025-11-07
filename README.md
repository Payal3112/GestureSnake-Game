# GestureSnake Game 🐍👋

**GestureSnake** is a modern twist on the classic Nokia Snake game, controlled entirely via **hand gestures** using a webcam. Built with Python, OpenCV, MediaPipe, and Pygame, this project demonstrates real-time computer vision and interactive gameplay.

---

## Features

### 🎮 Classic Snake Gameplay
- Authentic Nokia-style graphics with green monochrome theme  
- Grid-based movement with rectangular snake segments  
- Snake grows when eating fruit  
- Collision detection (walls and self)  
- Score tracking and game over screen  

### 👋 Hand Gesture Controls
- **Swipe Up / Down / Left / Right** – Move the snake  
- **Pinch Gesture (Thumb + Index Finger)** – Speed boost  
- **Additional Gestures Added** – Example: fist to pause, open palm to resume  
- Face detection overlay for fun feedback  
- Visual feedback of hand landmarks and detected gestures  

### 🪟 Dual Window Interface
- **Game Window** – Classic Snake gameplay  
- **Gesture Window** – Live webcam feed with hand tracking  

---

## Installation

### 1. Clone or Download
2. Create and Activate Virtual Environment (Python 3.10 recommended)
   ```bash
   python -m venv venv
# Windows PowerShell
.\venv\Scripts\Activate.ps1
# Windows CMD
venv\Scripts\activate.bat
# macOS/Linux
source venv/bin/activate
3. Install Dependencies
pip install -r requirements.txt

Running the Game
python main.py


Game window will appear

Webcam window shows your hand and gestures

Use gestures to control the snake
Controls
Gesture	Action
Swipe Up	Move snake up
Swipe Down	Move snake down
Swipe Left	Move snake left
Swipe Right	Move snake right
Pinch (Thumb + Index)	Speed boost
Fist	Pause game
Open Palm	Resume game

Keyboard Controls:

ESC – Quit game

Show UP gesture – Restart game after game over

Q in gesture window – Quit

File Structure
GestureSnake/
├── main.py                 # Game entry point
├── snake_game.py           # Snake game implementation
├── gesture_controller.py   # Hand gesture detection
├── requirements.txt        # Python package dependencies
├── setup.py                # Optional dependency installer
├── README.md               # Project documentation
└── LICENSE                 # MIT License

Development Notes

Add new gestures – Extend detect_gestures() in gesture_controller.py

Change game speed – Modify base_speed and boost_speed in snake_game.py

Change colors – Update color constants in snake_game.py

Technical Details
Game Engine

Pygame for graphics and window management

Grid-based movement (20x20 pixel cells)

60 FPS display, variable game speed

Computer Vision

MediaPipe Hands for real-time hand landmark detection

MediaPipe Face Detection for face tracking

OpenCV for webcam capture and gesture visualization

Architecture

Threaded design: game and gesture detection run in parallel

Modular: separate classes for game logic and gesture control

License
This project’s code is licensed under the MIT License.
Dependencies:


OpenCV – BSD 3-Clause


MediaPipe – Apache 2.0


Pygame – LGPL



Author
Created by Payal Payal


Bringing classic games into the modern age with gesture control


GitHub: https://github.com/<your-username>



Enjoy playing GestureSnake with hand gestures! 🐍👋

---

If you want, I can also **write a ready-to-push `LICENSE` file with MIT template** for this project, so it’s fully professional and you can directly send it to DRDO for your winter internship application.  

Do you want me to do that next?

```bash


git clone https://github.com/<your-username>/GestureSnake.git
cd GestureSnake
