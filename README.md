# 🧑‍🚀 AstroFix: Zero-G Protocol

[![WebXR](https://img.shields.io/badge/Platform-WebXR-5A3E85.svg)](#)
[![MediaPipe](https://img.shields.io/badge/Computer_Vision-MediaPipe-00B2A9.svg)](https://developers.google.com/mediapipe)
[![Web Speech API](https://img.shields.io/badge/Voice_UI-Web_Speech_API-F7DF1E.svg)](#)
[![A-Frame](https://img.shields.io/badge/Framework-A--Frame-EF2D5E.svg)](https://aframe.io/)
[![JavaScript](https://img.shields.io/badge/Language-JavaScript_ES6+-F7DF1E.svg)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)

> An immersive WebXR prototype exploring the future of multimodal Human-Computer Interaction (HCI) through gesture tracking and voice commands.

**AstroFix: Zero-G Protocol** is an interactive browser-based simulation of a futuristic zero-gravity spaceship repair sequence. Developed as an HCI mini-project, this application completely replaces traditional hardware inputs (keyboard/mouse) with **Hand Tracking** and a **Voice User Interface (VUI)**, allowing users to operate complex virtual systems just like an astronaut would.

## ✨ Multimodal Interaction Features

* **✋ Active Hand Tracking (MediaPipe):** Your physical hand acts as a virtual joystick. Move your hand to seamlessly rotate the VR camera in a full 360-degree environment.
* **🤏 Pinch-to-Interact:** Perform a physical "Pinch" gesture (index finger + thumb) to interact with 3D objects, simulating physical grabbing and manipulation in zero gravity.
* **🎙️ Voice User Interface (VUI):** Fully integrated native browser speech recognition. Trigger sequences and execute commands by speaking directly to the console.
* **🌌 5-Stage Escape Room Protocol:** An engaging, sequential puzzle requiring users to locate, diagnose, and repair critical ship systems (Power, Coolant, Communications, and Core) across the 3D space.
* **🔊 Spatial Feedback Mechanics:** Visual reticles, holographic text overlays, and audio cues respond instantly to hand positions and voice inputs to maximize immersion.

---

## 🏗️ Technology Stack

This prototype runs entirely client-side, leveraging modern browser APIs for low-latency machine learning and 3D rendering.

* **A-Frame:** The core WebXR framework utilized to construct the 3D scene, entities, lighting, and raycast interactions.
* **MediaPipe Hands:** A Google ML library running locally in the browser to trace 21 3D hand landmarks via standard webcam input in real-time.
* **Web Speech API:** HTML5 native voice recognition used to transcribe spoken audio and execute commands.
* **Vite:** Next-generation frontend tooling used for fast, optimized local development and serving.
* **Vanilla JavaScript:** Powers all state logic and the custom hand-to-camera matrix rotation mathematics without bulky framework dependencies.

---

## 🎮 Mission Briefing (How to Play)

1. **System Initialization:** When the environment loads, click **ENABLE GESTURE CONTROL**.
2. **Diagnostics:** Press and hold the `SPACEBAR`. Wait for the console to confirm "Mic Live", then say _"Diagnostics"_.
3. **Power Routing:** Follow the HUD prompts. Look right by moving your hand left/right. Locate the Power Node and **Pinch** to restore power.
4. **Coolant Flush:** Look left, locate the Coolant tube, and **Pinch** to flush the system.
5. **Comms Alignment:** Look upward toward the ceiling, locate the satellite dish, and **Pinch** to align the array.
6. **Core Reboot:** Return your view to the center console, grab the floating Plasma Tool via **Pinch**, and complete the protocol!

---

## 🚀 Getting Started

Ready to run this project on your own machine? Due to camera and microphone permission requirements, this application must be run on a local server. 

For comprehensive installation and setup instructions, please refer to the [**Setup Guide**](./SETUP_GUIDE.md).

---

## 📝 License & Academic Context

This project was created for educational purposes as an **HCI (Human-Computer Interaction)** coursework assignment. The primary research focus was evaluating the cognitive load and usability of combining VUI with spatial gesture tracking in environments without traditional haptic feedback. Feel free to fork, use, and modify!
