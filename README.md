# NOIR / FRAME — Haute Photography & Creative Studio

<p align="center">
  <strong>An Awwwards-caliber, responsive digital experience bridging spatial photography, GLSL shader art, and tactile user interface engineering.</strong>
</p>

<p align="center">
  <a href="https://manikar984.github.io/animated-photography-website/">
    <img src="https://img.shields.io/badge/LIVE%20DEMO-VISIT%20WEBSITE-d8ff35?style=for-the-badge&logo=googlechrome&logoColor=080808&labelColor=080808" alt="Live Demo" />
  </a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/WebGL-Three.js_r128-000000?style=for-the-badge&logo=three.js&logoColor=white" alt="Three.js" />
  <img src="https://img.shields.io/badge/Motion-GSAP_3.12-88CE02?style=for-the-badge&logo=greensock&logoColor=white" alt="GSAP" />
  <img src="https://img.shields.io/badge/Physics-Lenis_Scroll-111111?style=for-the-badge" alt="Lenis" />
  <img src="https://img.shields.io/badge/Audio-Tone.js_Synthesizer-f59e0b?style=for-the-badge" alt="Tone.js" />
  <img src="https://img.shields.io/badge/Styling-Tailwind_CSS-38bdf8?style=for-the-badge&logo=tailwindcss&logoColor=white" alt="Tailwind CSS" />
  <img src="https://img.shields.io/badge/License-MIT-d8ff35?style=for-the-badge&labelColor=080808" alt="License: MIT" />
</p>

---

## 🔗 Live Experience

Experience the live interactive build directly in your browser:  
👉 **[https://manikar984.github.io/animated-photography-website/](https://manikar984.github.io/animated-photography-website/)**

---

## ✦ Overview

**NOIR / FRAME** is an independent haute photography, moving image, and spatial design laboratory operating between Los Angeles, New York, and Tokyo. 

This repository houses the studio's flagship web experience, heavily inspired by modern design pioneers such as **Lusion.co** and **Fantasy.co**. Built with zero bloated framework overhead, it unites high-performance WebGL shaders, kinetic physics-driven typography, procedural audio, and responsive layouts across phones, tablets, and ultra-wide desktop displays.

---

## ✨ Key Features & Architecture

### 1. WebGL Organic Shader Core (Lusion-Tier)
- **GLSL Simplex Noise Vertex Displacement**: A real-time undulating 3D metallic torus knot geometry that calculates procedural organic ripples based on time, velocity, and pointer coordinates.
- **Fresnel Chromatic Rim Calculation**: Dynamic edge-lighting that shifts across iridescent acid lime (`#d8ff35`) highlights and obsidian deep-field reflections (`#0a0a0c`).
- **Adaptive Stardust Particle Field**: Depth-layered ambient motes responding with subtle inertial drag and scroll momentum.

### 2. Multi-Device Responsive System
- **Desktop / Ultra-Wide Displays**:
  - **1:1 Hardware Tracking Cursor**: Zero-lag reticle dot utilizing hardware-direct GPU `translate3d` tracking paired with an elastic kinetic trailing ring (`lerp: 0.25`).
  - **3D Card Perspective Tilt**: Interactive raycast mouse tracking with dynamic radial sheen glare (`--mouse-x`, `--mouse-y`).
  - **Quick-Inspector Lens**: Floating image follower showcasing photographic previews on hover.
- **Tablets & Touch Laptops**:
  - Dynamically adjusted Three.js camera distance and field of view (FOV).
  - Touch-drag interaction that translates gestures into smooth rotation matrices.
- **Mobile Phones (Handheld)**:
  - Custom hardware cursor automatically unbinds to preserve native touch responsiveness.
  - Fluid fluid-clamp typography preventing awkward character breaks.
  - Stacked editorial grid layouts with optimized lazy-loading assets.

### 3. Dynamic Index Radar & "Drawing Board" Reveal
- **Morphing 'X' Close Trigger**: A custom 3-line hamburger button that collapses, translates, and rotates into an illuminated neon lime `'X'` with cubic-bezier easing.
- **Architectural Drafting Board Layer**: Opening the navigation reveals a white blueprint paper backdrop complete with draft pins, measurement markings, and technical silver-halide plate annotations.
- **Photographic Emulsion Transition**: Hovering (desktop) or tapping (mobile/tablet) navigation links smoothly manifests the target photo onto the drafting paper with liquid circular clip-path expansion.

### 4. Kinetic Scroll & Procedural Audio
- **Lenis Smooth Scroll Engine**: Inertia deceleration scroll curve mapped directly to GSAP's RAF ticker (`lagSmoothing: 0`).
- **ScrollTrigger Orchestration**: Parallax container offsets and automated numeric metric counters.
- **Tone.js Sound Architecture**:
  - Built-in polyphonic sine synthesizer producing crystalline harmonic chimes upon interaction.
  - Low-frequency 55Hz ambient analog hum creating cinematic auditory depth (toggled via HUD controls).

---

## 📐 Responsive Breakpoint Matrix

| Viewport | Device Target | Key Behaviors & Adjustments |
| :--- | :--- | :--- |
| **`< 640px`** | Mobile Phones (iOS / Android) | Cursor disabled, full-screen vertical navigation, instant tap photo transitions, 1-column layouts, camera Z = `6.2`. |
| **`640px — 1024px`** | Tablets (iPad / Surface) | Touch-first, 2-column portfolio view, touch-emulated camera inertia, camera Z = `5.4`. |
| **`> 1024px`** | Desktops & Monitors | Zero-lag pointer engine, 3D card tilt, hover-driven photo reveal on drafting sheet, camera Z = `4.8`. |

---

## 🛠️ Tech Stack & Dependencies

| Layer | Technology | Purpose |
| :--- | :--- | :--- |
| **Structure** | HTML5 / Semantic Elements | Accessible and SEO-optimized document tree |
| **Styling** | Tailwind CSS / Custom CSS | Modern utility layout with custom keyframe animations |
| **3D Rendering** | [Three.js (r128)](https://threejs.org/) | WebGL scene graph, camera orchestration, buffer geometry |
| **Shaders** | Native GLSL | Custom vertex and fragment shaders (Noise + Fresnel) |
| **Animation** | [GSAP 3.12.5](https://greensock.com/gsap/) | High-performance transform tweening |
| **Scroll Trigger** | [GSAP ScrollTrigger](https://greensock.com/scrolltrigger/) | Scroll-synchronized viewport reveals and counters |
| **Kinetic Scroll** | [Lenis 1.1.9](https://lenis.darkroom.engineering/) | Smooth wheel inertia physics |
| **Sound Engine** | [Tone.js 14.7.77](https://tonejs.github.io/) | Procedural Web Audio API sound synthesis |

---

## 🚀 Getting Started

Because the project utilizes WebGL shaders and the Web Audio API, modern browsers require files to be served via an HTTP/HTTPS protocol rather than the local file system (`file://`).

### 1. Clone the Repository
```bash
git clone [https://github.com/manikar984/animated-photography-website.git](https://github.com/manikar984/animated-photography-website.git)
cd animated-photography-website
