# Diet Soda | Pure Zero Refreshment

An interactive 3D hero landing page for a fictional beverage brand, featuring real-time 3D models with Google `<model-viewer>`, physics-inspired cursor repulsion, and choreographed flavor transitions.

![Diet Soda Preview](https://api.getlayers.ai/storage/v1/object/public/public/assets/soda-14ff8a788d/Green%20Soda.png)

## ✨ Features

- **Interactive 3D Centerpiece**: High-fidelity 3D soda can rendered via Google's `<model-viewer>` web component that dynamically tilts towards the cursor in real time.
- **Dynamic 3D Berry & Leaf Parallax**:
  - Multi-layer parallax drift (foreground berries, background berries, leaves).
  - Continuous sinusoidal floating motion.
  - Interactive pointer force field that repels nearby berries within a 400px radius.
- **Choreographed Flavor Switching**:
  - Seamless background radial gradient morph between **Diet Classic** (teal) and **Zero Lime** (blue).
  - 720° can spin with motion blur, swapping PBR metallic-roughness base textures at the peak.
  - Berries implode to the center, swap 3D models (`cherry.glb` ↔ `blueberry.glb`), and explode back out to randomized positions.
- **Ambient Elements**: Endlessly rising translucent bubbles with random scaling, rotation, and drift.
- **Glassmorphism UI**: Frosted glass navigation bar, product cards with hover animations, typography in *Galada*, *Inter*, and *Manrope*, and signature `#fbcfe8` pink accents.
- **Zero Build Step**: Fully self-contained in a single `index.html` file using CDN-delivered GSAP and Google `<model-viewer>`.

## 🚀 Getting Started

Simply open `index.html` in any modern web browser or serve it with a local HTTP server:

```bash
# Using Python
python -m http.server 8000

# Or using npx serve
npx serve .
```

Then visit [http://localhost:8000](http://localhost:8000).

## 🛠️ Tech Stack

- **HTML5 & CSS3**: Modern CSS Grid/Flexbox, CSS custom properties, and keyframe animations.
- **GSAP (GreenSock)**: Smooth timeline animations and property morphing.
- **Google `<model-viewer>`**: Fast, accessible WebGL 3D model rendering.
- **Google Fonts**: Galada, Inter, Manrope, and Outfit.
