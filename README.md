# 🔫 Bullet Frenzy – 3D OpenGL Game (Lab 03)

**Course**: CSE 423 – Computer Graphics  
**Semester**: Spring 2025  
**Department**: Computer Science and Engineering  
**Assignment**: Lab 03 – OpenGL 3D Introduction and Transformation

## 🧠 Overview

Bullet Frenzy is a 3D game developed using Python and PyOpenGL to demonstrate core concepts of 3D graphics, transformations, and perspective projections. Players control a gun-equipped character that can move, rotate, shoot bullets, and engage enemies in a bounded 3D grid world. The game showcases translation, rotation, scaling, and real-time interactions with perspective projection.

---

## 🎮 Game Features

- **Player Movement & Gun Rotation**
  - W/S to move forward/backward
  - A/D to rotate the player
  - Left mouse click to shoot bullets

- **Camera Controls**
  - Arrow keys to move and rotate the camera
  - Right mouse click toggles first-/third-person view

- **Cheat Mode**
  - `C` toggles auto-rotate + shoot at enemies in sight
  - `V` enables automatic camera following in cheat mode

- **Game Mechanics**
  - Score increases by hitting enemies
  - Player loses a life on contact with enemies
  - Game ends after 5 lives lost or 10 missed bullets
  - `R` key resets the game state (score, lives, missed shots)

- **Enemy Behavior**
  - 5 enemies follow the player
  - Hit enemies respawn randomly
  - Enemies pulse (expand/shrink) dynamically

---

## 🛠️ Core OpenGL Concepts Applied

- **Transformations**
  - `glTranslatef` for movement
  - `glRotatef` for orientation
  - `glScalef` (not used here but covered)

- **Camera & Perspective**
  - `gluLookAt()` to simulate a 3D camera
  - `gluPerspective()` to implement depth and field of view

- **Scene Control**
  - `glPushMatrix` / `glPopMatrix` to isolate transformations
  - `glColor3f`, `glBegin`, `glEnd`, and GLUT primitives for rendering

---

## 🧩 Components

- 🧍 **Player**: Composed of sphere (head), cylinders (arms/legs/gun), and a cuboid (body)
- 🧠 **Enemies**: Red pulsating spheres with black heads
- 🟩 **Grid Floor**: Dynamic checkerboard pattern
- 🧱 **Boundaries**: Colored vertical walls enclosing the play area

---

## 🚀 Run Instructions

### ✅ Requirements
- Python 3.x
- `PyOpenGL`
- `numpy`

### ▶️ How to Run
```bash
pip install PyOpenGL PyOpenGL_accelerate numpy
python your_filename.py
