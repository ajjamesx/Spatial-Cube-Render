# 🌌 3D Cube Animation with Dynamic Sky, Lighting, and Texture Mapping

This project features a 3D rotating cube rendered on an HTML canvas, set against a sky that changes based on the time of day. It blends real-time animation, lighting simulation, starfield effects, and texture-mapped geometry to create an immersive visual experience.

## ✨ Features

- **Rotating Cube**  
  - Real-time rotation on both X and Y axes using transformation matrices
  - Stable geometry without stretching or distortion

- **Dynamic Sky Gradient**  
  - Sky tones change according to the user's system time
  - Smooth transitions between morning, day, evening, and night

- **Glowing Sun**  
  - A radial-gradient sun moves across the canvas based on the current hour
  - Intensity and placement reflect time of day

- **Twinkling Stars**  
  - Randomly generated stars fade in and out after sunset
  - Each star flickers independently for realism

- **Face Lighting with Ambient Simulation**  
  - Each cube face is shaded using the dot product of its normal and a rotating light vector
  - Ambient light ensures no face is completely dark

- **Texture Mapping**  
  - All six cube faces use the same texture (`box.jpg`)
  - Texture drawn using approximate projection and clipping per face
  - Lighting intensity adjusts alpha transparency of texture rendering


## 🖥️ Running the Demo

This project uses canvas-based rendering — no dependencies, no WebGL!

### 🔧 Option 1: Python (Recommended for local testing)

```bash
# From your project directory:
python -m http.server

# Then open in your browser:
http://localhost:8000/index.html


## 🧱 Tech Stack

- HTML5 & CSS
- Vanilla JavaScript
- Canvas API (2D rendering)

No libraries or frameworks required.

## 🚀 Getting Started

1. Clone or download this repository.
2. Ensure your texture image is named `box.jpg` and placed in the root directory.
3. Open `index.html` in any modern browser.

You’ll instantly see a rotating, shaded, textured cube beneath a dynamic atmosphere.

## 🧠 Code Highlights

- `Cube.rotate()` for dual-axis rotation
- `Cube.draw(ctx)` applies per-face lighting and image projection
- `drawSkyGradient()` and `drawSun()` react to system time
- `stars[]` array handles flicker animation
- Lighting uses surface normals and a light vector that orbits

## 📁 File Structure
 textured-cube-project ├── index.html ├ box.jpg

## 🛠 Author

Created by **Anuj James**  
Explore more multimedia and interactive experiments: [github.com/ajjamesx](https://github.com/ajjamesx)

---


