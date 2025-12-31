# AetherFlow-Gesture-Controlled-3D-Particle-Synth
AetherFlow is a high-performance 3D particle engine built with Three.js and MediaPipe. It uses real-time Computer Vision to track hand gestures, allowing users to morph 10,000+ particles into shapes like hearts and planets via custom GLSL shaders. A fusion of generative art and AI-driven interaction.
🚀 Features

    Real-time Hand Tracking: Leverages MediaPipe Hands to track 21 3D landmarks at 60 FPS.

    GPU-Accelerated Morphing: Uses custom GLSL Shaders (Vertex & Fragment) to transition 10,000+ particles smoothly between shapes without CPU overhead.

    Gesture-Based Interaction:

        Pinch (Thumb + Index): Morphs particles into a glowing Heart.

        Victory Sign (2 Fingers): Morphs particles into Saturn with its rings.

        Three-Finger Spread: Morphs particles into an oscillating 3D Flower.

        Open Palm: Triggers a Fireworks explosion and resets the system.

    Dynamic Responsive UI: Smoothly follows hand movement (Landmark 9) across the screen.

🛠️ Tech Stack

    Three.js: 3D Engine for WebGL rendering.

    MediaPipe: Cross-platform ML for hand landmark detection.

    GLSL: Custom Shaders for high-performance particle math.

    JavaScript (ES6+): Module-based logic and gesture heuristics.

💻 How to Run

Because the project uses Webcam API and ES Modules, it must be served over a local server.

    Clone the Repository:
    Bash

git clone https://github.com/your-username/3d-gesture-particles.git

Run with Local Server:

    If using VS Code: Install the Live Server extension. Right-click index.html and select "Open with Live Server".

    If using Python:
    Bash

        python -m http.server 8000

    Permissions: Allow the browser to access your webcam when prompted.

🧠 What I Learned

This project demonstrates proficiency in several advanced domains:

    Computer Vision Integration: Learning how to map 2D camera coordinates into a 3D coordinate system.

    Shader Programming: Writing logic in the Vertex Shader to handle complex mathematical shapes (Parametric equations) on the GPU.

    Gesture Logic: Implementing Euclidean distance and landmark state checking to define user intent.

    Performance Optimization: Using BufferGeometry and ShaderMaterial to maintain high frame rates while managing thousands of individual objects.
