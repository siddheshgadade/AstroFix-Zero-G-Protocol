# Setup Guide & Installation

Follow these steps to get the **AstroFix: Zero-G Protocol** running locally on your own machine. 

Since this project relies on accessing your Webcam and Microphone via the browser, it must be run on a secure `localhost` web server, rather than just opening the HTML file directly.

## Prerequisites

Before starting, ensure you have the following installed on your computer:
1. **Node.js** (v16 or higher) - Download and install from [nodejs.org](https://nodejs.org/).
2. A modern web browser with Webcam & Microphone access (Google Chrome is highly recommended for best Web Speech API compatibility).
3. A functional Webcam and Microphone.

---

## 1. Installation

1. **Clone or Download the Repository:**
   Download the project files from GitHub and extract them to a folder on your computer.

2. **Open your Terminal:**
   Open a terminal, command prompt, or VS Code terminal, and navigate to the project folder. For example:
   ```bash
   cd path/to/HCI_project
   ```

3. **Install Dependencies:**
   Run the following command to download the local server tools (Vite):
   ```bash
   npm install
   ```

---

## 2. Running the Application

Once everything is installed, starting the server is incredibly easy!

1. In the terminal, run the following command to spin up the local development server:
   ```bash
   npm run dev
   ```
2. The terminal will output a local network address. It will usually look something like this:
   ```
   ➜  Local:   http://localhost:5173/
   ```
3. `Ctrl + Click` that link, or copy and paste `http://localhost:5173/` into your web browser.

---

## 3. Initial Configuration (Important!)

Browsers impose strict security constraints for privacy reasons. The very first time you load the page, you must grant permissions:

1. **Camera Permission:** Your browser will ask for permission to use your Camera. **Allow** this, or the MediaPipe Hand Tracker will not function.
2. **Microphone Permission:** When you press the `SPACEBAR` for the very first time to trigger a voice diagnostic, the browser will ask for Permission to use your Microphone. **Allow** this, or you will not be able to issue voice commands!

### Troubleshooting

* **Pinch Not Detecting?** Ensure you are in a relatively well-lit room. MediaPipe requires contrast to easily spot the difference between your hand and the background.
* **Camera Isn't Moving?** Make sure you clicked the "ENABLE GESTURE CONTROL" button to start the initialization. It may take 2-4 seconds for the ML model to download and boot up to begin tracking your hand.
* **Voice Diagnostic Fails?** The Web Speech API works best on Chromium-based browsers (Chrome, Edge). Make sure you are not using Safari or an older browser that doesn't support the native Web Speech element.

Enjoy repairing the ship!
