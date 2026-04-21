# AstroFix: Zero-G Protocol

**AstroFix: Zero-G Protocol** is an immersive WebXR (Virtual Reality) prototype designed to explore multimodal Human-Computer Interaction (HCI). Developed as an HCI mini-project, this application simulates a futuristic zero-gravity spaceship repair sequence using **Hand Tracking (Gestures)** and **Voice Commands (VUI)**—completely replacing traditional keyboard and mouse controls.

## 🚀 Features

* **Active Hand Tracking (MediaPipe):** Your physical hand acts as a virtual joystick. Move your hand to rotate the VR camera in a full 360-degree environment without needing a mouse or VR headset.
* **Pinch-to-Interact:** Perform a physical "Pinch" gesture with your index finger and thumb to interact with 3D objects, simulating physical grabbing in zero gravity.
* **Voice User Interface (VUI):** Fully integrated Web Speech API allows you to trigger sequences and execute commands by speaking directly to the console.
* **5-Stage Escape Room Protocol:** A sequential, engaging puzzle requiring users to locate, diagnose, and repair ship systems (Power, Coolant, Communications, and Core) by looking around the 3D space.
* **Spatial Feedback Mechanics:** Visual reticles, holographic text overlays, and audio cues respond instantly to hand position and voice inputs, maximizing user immersion.

## 🛠️ Technology Stack

* **A-Frame:** The core WebXR framework used to construct the 3D scene, entities, lighting, and raycast interactions.
* **MediaPipe Hands:** A Google ML library running locally in the browser to trace 21 3D hand landmarks via standard webcam input in real-time.
* **Web Speech API:** HTML5 native voice recognition used to transcribe spoken audio.
* **Vite:** Next-generation frontend tooling used for fast local development and serving.
* **Vanilla JavaScript:** Powers all state logic and the custom hand-to-camera matrix rotation mathematics without bulky framework dependencies.

## 🎮 How to Play

1. When the page loads, click **ENABLE GESTURE CONTROL**.
2. **Diagnostics:** Press and hold `SPACEBAR`, wait for the console to say "Mic Live" and say _"Diagnostics"_.
3. **Power Routing:** Follow the prompt on the screen. Look Right by moving your hand left/right. Find the Power Node and **Pinch** to restore power.
4. **Coolant Flush:** Look Left, find the Coolant tube, and **Pinch** to flush it.
5. **Comms Alignment:** Look Upwards at the ceiling, find the satellite dish, and **Pinch** to align it.
6. **Core Reboot:** Look back to the center console, find the floating Plasma Tool, and **Pinch** to complete the protocol!

## 📦 Getting Started

Ready to run this project on your own machine? See the detailed instructions in the [**Setup Guide**](./SETUP_GUIDE.md).

## 📝 License

This project is created for educational purposes as an HCI (Human-Computer Interaction) coursework assignment. Feel free to use and modify it!
