# ⚛️ Particle Core: The Holographic Gesture Engine

> **"Minority Report meets the Browser."**
> A real-time, interactive 3D particle system controlled entirely by your hand gestures.

![Three.js](https://img.shields.io/badge/Three.js-Black?style=for-the-badge&logo=three.js&logoColor=white)
![MediaPipe](https://img.shields.io/badge/MediaPipe-00aabb?style=for-the-badge&logo=google&logoColor=white)
![WebGL](https://img.shields.io/badge/WebGL-GLSL-red?style=for-the-badge)

## 🌌 What is this?
**Particle Core** is an advanced web experiment that combines **Computer Vision** (MediaPipe) with **High-Performance WebGL** (Three.js + GLSL Shaders). 

It generates **55,000+ individual particles** that form complex 3D shapes (Globes, Hearts, Galaxies). Using your webcam, it detects your hand structure in real-time, allowing you to manipulate physics, destroy objects, and freeze time—just like Iron Man's holographic interface.

## ✨ Key Features

* **🖐️ AI Hand Tracking:** Zero-latency tracking of finger joints using Google's MediaPipe.
* **⚡ 55k+ GPU Particles:** Entirely rendered via custom **GLSL Vertex Shaders**. No CPU lag.
* **🌓 Low-Light Optimized:** Uses "Lerp" smoothing algorithms to work perfectly even in dark rooms.
* **💎 Bloom & Post-Processing:** Cinematic glow effects using UnrealBloomPass.
* **🧠 Smart State Machine:** Distinguishes between pointing, grabbing, and pinching automatically.

---

## 🎮 The Gesture Guide (God Mode)

The system includes a **Gesture Recognition Engine**. Use these hand signs to control the physics:

| Gesture | Action | Effect |
| :--- | :--- | :--- |
| **☝️ Point** | **Interact** | Gently swirl particles like water. |
| **🖐️ Open Palm** | **DESTROY** | A violent shockwave scatters particles outward. (Includes turbulence noise). |
| **✊ Closed Fist** | **REBUILD** | Creates a massive Black Hole gravity well that sucks particles back together. |
| **👌 Pinch** | **FREEZE** | **"Matrix Mode"**. Stops time and freezes the explosion in mid-air. |
| **✌️ Peace** | **MORPH** | Cycles to the next 3D template (Sphere → Heart → Saturn → Galaxy). |

---

## 🚀 Quick Start

This project is a **single-file masterpiece**. You don't need a complex build step.

### Option 1: The Easy Way (Vercel/Netlify)
1.  Upload `index.html` to a GitHub repository.
2.  Connect it to Vercel.
3.  **Done.** (Camera access requires HTTPS, which Vercel provides automatically).

### Option 2: Local Development
1.  Clone this repo:
    ```bash
    git clone [https://github.com/your-username/particle-core-hologram.git](https://github.com/your-username/particle-core-hologram.git)
    ```
2.  You **cannot** just double-click `index.html` (Camera permissions block local file access). You must run a local server.
3.  If you have Python installed:
    ```bash
    python3 -m http.server
    ```
4.  Open `http://localhost:8000`.

---

## 🧠 How it Works (Under the Hood)

### 1. The Physics (GLSL Shaders)
We do not calculate the position of 55,000 particles in JavaScript (that would be too slow). Instead, we pass the **Hand Coordinates** to the GPU as a "Uniform". The GPU then runs a physics calculation on *every single pixel simultaneously* using a custom Vertex Shader.

### 2. The Vision (MediaPipe)
We use the `HandLandmarker` task to extract 21 skeletal points from your video feed.
* **Fist Detection:** We calculate the Euclidean distance between fingertips and the wrist.
* **Pinch Detection:** We calculate the distance between the Index Tip and Thumb Tip.

### 3. The Smoother (Linear Interpolation)
Webcams are jittery. We use a **Lerp (Linear Interpolation)** function:
`currentX += (targetX - currentX) * 0.1`
This ensures the hologram movement feels "heavy" and smooth, rather than shaky.

---

## 🛠️ Technologies Used
* **Three.js** - 3D Engine
* **Google MediaPipe** - AI Computer Vision
* **GLSL** - Custom Shader Language
* **GSAP** - Animation transitions

---

## 📜 License
MIT License. Feel free to fork, modify, and create your own JARVIS interface.

---

<p align="center">
  <b>🌟 Star this repo if it made you feel like Tony Stark! 🌟</b>
</p>
