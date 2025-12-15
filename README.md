<div align="center">

  # ⚛️ HOLOFLUX
  **The "Minority Report" Interface for the Web**

  [![Three.js](https://img.shields.io/badge/Three.js-Black?style=for-the-badge&logo=three.js&logoColor=white)](https://threejs.org/)
  [![MediaPipe](https://img.shields.io/badge/MediaPipe-Vision-00aabb?style=for-the-badge&logo=google&logoColor=white)](https://developers.google.com/mediapipe)
  [![WebGL](https://img.shields.io/badge/WebGL-GLSL-red?style=for-the-badge&logo=opengl&logoColor=white)](https://get.webgl.org/)
  [![License](https://img.shields.io/badge/License-MIT-yellow.svg?style=for-the-badge)](LICENSE)

  <br />

  <img src="https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExcDdtY3h6Y2t6Y2t6Y2t6Y2t6Y2t6Y2t6Y2t6Y2t6Y2t6Y2t6&ep=v1_gifs_search&rid=giphy.gif" alt="Demo GIF" width="100%" style="border-radius: 10px; box-shadow: 0 0 20px rgba(0,255,255,0.2);">

  <h3>
    <a href="https://holoflux-gesture-engine.vercel.app/">🔴 LIVE DEMO</a>
    <span> | </span>
    <a href="https://github.com/ossamamehmood/holoflux-gesture-engine/issues">🐛 Report Bug</a>
  </h3>
</div>

---

## 🔮 What is Holoflux?

**Holoflux** is an experimental WebGL interface that bridges the gap between **Computer Vision** and **High-Performance Graphics**. 

It renders **55,000 interactive particles** that react to your physical hand movements in real-time. By combining Google's MediaPipe (for skeletal tracking) with custom GLSL Shaders (for physics), Holoflux achieves a "God Mode" experience where you can physically grasp, explode, and freeze digital matter directly in your browser.

> **"Any sufficiently advanced technology is indistinguishable from magic."** — *Arthur C. Clarke*

## ✨ Features

* **🧠 AI Skeletal Tracking:** Zero-latency hand recognition using MediaPipe.
* **⚡ 55k+ GPU Particles:** A custom Vertex Shader handles millions of physics calculations per frame with zero CPU lag.
* **🕸️ State Machine Engine:** Intelligently distinguishes between complex gestures (Pinch vs. Fist vs. Palm).
* **🌑 Low-Light Capable:** Uses Lerp (Linear Interpolation) smoothing algorithms to filter out webcam noise in dark environments.
* **💎 Cinematic Post-Processing:** Integrated UnrealBloomPass for that neon, sci-fi aesthetic.

<p align="center">
  <img alt="" style="{max-height: 20px}" src="./.github/holoflux.gif">
</p>

---

## 🖐️ The Gesture Guide

This system uses a custom **"Iron Man"** interaction model. Use these hand signs to control the physics engine:

| Gesture | Action | Visual Effect |
| :--- | :--- | :--- |
| **🖐️ Open Palm** | **EXPLODE** | A violent shockwave scatters particles outward with turbulence noise. |
| **✊ Closed Fist** | **IMPLODE** | Generates a massive gravity well (Black Hole) that reconstructs the shape. |
| **👌 Pinch** | **FREEZE** | **"Matrix Mode."** Instantly stops time and freezes particles in mid-air. |
| **✌️ Peace Sign** | **MORPH** | Cycles the geometry: `Sphere` → `Heart` → `Saturn` → `Galaxy`. |
| **☝️ Point** | **SWIRL** | Standard interaction. Gently displace particles like water. |

---

## 🚀 Quick Start

This project is built as a **Single File Experience** to demonstrate the power of raw WebGL without build-step complexity.

### 1. Clone
```bash
git clone [https://github.com/your-username/holoflux-gesture-engine.git](https://github.com/your-username/holoflux-gesture-engine.git)
cd holoflux-gesture-engine
