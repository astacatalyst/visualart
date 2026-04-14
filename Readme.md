# Neon Aura AR - Advanced Hand Tracking Experience

Welcome to **Neon Aura AR**, an interactive, browser-based Augmented Reality experience. This project relies on your webcam to track hand movements and translates them into a glowing, audio-visual interactive playground.

## Features

- **Advanced Hand Tracking:** Uses Google's MediaPipe library to track up to two hands with high precision.
- **Dynamic Visuals:** 
  - Real-time skeleton drawing with neon bloom effects.
  - Interactive "shockwaves" and particles triggered by your fingers.
  - Dynamic lightning arcs bridging your hands when held close together.
  - A matrix-like raining background that accelerates as you move your hands faster.
- **Audio Feedback:** 
  - Dynamic ambient hum that adjusts volume and pitch based on the distance between your hands.
  - A subtle "zap" sound whenever a pinch gesture is detected.
- **Theming:** Includes multiple customizable themes (Rainbow, Cyberpunk, Lava, Ocean, Galaxy) which recolor the effects, background, and particles in real-time.
- **Gesture Detection:** Detects simple gestures like open-hand, fist, and pinch, alongside interactive metrics (spreading of hands).

## How to Run

Because this is a vanilla HTML/JS/CSS project, you do not need any complex setup or build steps.

1. Firstly, **clone this repository** or **fork this repository** to your local machine.
2. Ensure you have an active internet connection (the project relies on MediaPipe libraries sourced from a CDN).
3. The next step is to **run the `index.html` file** by opening it in any modern web browser (Edge, Chrome, Firefox, Safari).
   - *Note: Some browsers require pages utilizing the camera to be served over `localhost` or via `https`. We recommend using a simple local server like VS Code's "Live Server" extension.*
4. Upon starting, click the **"Enter Experience"** button and *Accept* the browser prompts asking for microphone/camera permissions. 
5. Start moving your hands in front of the camera and enjoy!

## Technologies Used

- **HTML5 Canvas:** For all particle rendering, lighting effects, and drawing.
- **Web Audio API:** Creating continuous hums and generated audio synth zaps dynamically.
- **MediaPipe Hands:** Used to extract pose landmarks from hands via webcam asynchronously.

## Controls

- Move your hands in the frame to leave trailing particles and generate sparks.
- Bring your hands together to watch electricity bridge your fingers.
- **Pinch** (Thumb + Index finger) to create a shockwave effect.
- Try different hand spreads to alter the UI metrics.
- Click the floating bubbles at the bottom to cycle between different visual themes.
