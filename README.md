<div align="center">

  # ⚛️ HOLOFLUX
  **A Sonic & Gesture-Controlled Holographic Core**

  [![Three.js](https://img.shields.io/badge/Three.js-Black?style=for-the-badge&logo=three.js&logoColor=white)](https://threejs.org/)
  [![MediaPipe](https://img.shields.io/badge/MediaPipe-Vision-00aabb?style=for-the-badge&logo=google&logoColor=white)](https://developers.google.com/mediapipe)
  [![WebGL](https://img.shields.io/badge/WebGL-GLSL-red?style=for-the-badge&logo=opengl&logoColor=white)](https://get.webgl.org/)
  [![Web Audio API](https://img.shields.io/badge/Web_Audio_API-Synthesizer-purple?style=for-the-badge&logo=rss&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/API/Web_Audio_API)

  <br />
  
  <img src="./preview.jpg" alt="HoloFlux Preview" width="100%" style="border-radius: 20px; box-shadow: 0 20px 50px rgba(0,0,0,0.5); border: 1px solid rgba(255,255,255,0.1);">

  <h3>
    <a href="https://holoflux-gesture-engine.vercel.app/">🔴 LAUNCH LIVE EXPERIENCE</a>
    <span> | </span>
    <a href="https://github.com/ossamamehmood/holoflux-gesture-engine/issues">🐛 Report Bug</a>
  </h3>
</div>

---

## 🔮 The Experience

**HoloFlux** is a next-generation web experiment that creates a **tangible digital interface**.

It renders **55,000+ interactive particles** on the GPU that react to your physical hand movements in real-time. Unlike standard demos, HoloFlux features a **Procedural Audio Engine** that synthesizes sound effects on the fly based on your gestures, creating a synesthetic loop of sight, sound, and touch.

> **"Iron Man's Interface in the Browser."**

---

## ✨ Key Features

### 🧠 AI & Physics
* **Skeletal Tracking:** Zero-latency hand recognition using Google's **MediaPipe**.
* **GPU Simulation:** A custom GLSL Vertex Shader handles 55k particle physics calculations per frame.
* **Optical Flow:** Particles react to hand velocity, direction, and gesture states.

### 🔊 Sonic Surge Engine (New v5.0)
* **Procedural Audio:** No MP3 files. All sounds (hover chirps, gravity drops, time-freeze drones) are synthesized in real-time using the **Web Audio API**.
* **Dynamic Mixing:** Audio frequencies shift based on interaction intensity.

### 💎 iOS 26 Glass UI
* **Hyper-Realistic Glass:** Features optical refraction, noise texturing, and diamond-cut borders.
* **Liquid Gradients:** Infinite flowing color streams across text and UI elements.
* **Spectral Emojis:** Custom filtered iconography to match the holographic aesthetic.

---

## 🎮 Command Guide

This system uses a **State Machine** to detect complex hand poses.

| Gesture | State | Visual Effect | Audio FX |
| :--- | :--- | :--- | :--- |
| **🖐️ Open Palm** | **EXPLODE** | A violent shockwave scatters particles outward. | Sawtooth Shockwave |
| **✊ Closed Fist** | **IMPLODE** | Generates a massive Black Hole gravity well. | Sine Wave Drop |
| **👌 Pinch** | **FREEZE** | **"Matrix Mode."** Stops time instantly. | High-Pass Drone |
| **✌️ Peace Sign** | **MORPH** | Cycles geometry: `Sphere` → `Heart` → `Saturn`. | Resonant Chime |
| **☝️ Point** | **INTERACT** | Standard interaction. Swirl particles like water. | Dynamic Swirl |

---

## 🚀 Quick Start

This project is a **Zero-Dependency** static site. You don't need `npm install` or complex build steps.

### Local Development
1.  **Clone the repo**
    ```bash
    git clone [https://github.com/ossamamehmood/holoflux-gesture-engine.git](https://github.com/ossamamehmood/holoflux-gesture-engine.git)
    cd holoflux-gesture-engine
    ```

2.  **Run a local server** *Note: Camera access requires a server context; you cannot just open the HTML file.*
    ```bash
    # If you have Python
    python3 -m http.server

    # OR if you have Node.js
    npx serve
    ```

3.  **Open Browser**
    Go to `http://localhost:8000`

---

## 🛠️ Tech Stack

* **Three.js:** 3D Rendering Engine.
* **MediaPipe:** Computer Vision (Hand Tracking).
* **GLSL:** Custom Shaders for Particle Physics.
* **Web Audio API:** Real-time Sound Synthesis.
* **GSAP:** UI Animations.

---

## 📜 License

Distributed under the MIT License. See `LICENSE` for more information.

<br />

<div align="center">
  <b>Designed & Engineered by <a href="https://ossamamehmood.com">Ossama Mehmood</a></b>
</div>
