# Paleo Time Machine ⏳🌍
**Your backyard. 70 million years ago.**

A **sci-fi imagination engine** — slide time, watch your world reborn.
Powered by **Grok API**, **Firebase**, and **Mapbox**.

---

## Vision
**Step into your street as a Jurassic jungle — in VR, on your phone.**

| Future Feature | Tech |
|----------------|------|
| Full VR Immersion | WebXR + Gaussian Splats |
| Photorealistic Flora | AI-generated 3D (Luma AI) |
| Dynamic Weather & Fauna | Procedural |
| Time Capsule Sharing | AR/VR links |
| Educational Mode | Scotese, GPlates, citations |
| Offline PWA | 100k locations × 12 eras cached |
| Monetization | Premium eras, VR export, schools |

---

## Roadmap: MVP → Vision

| Phase | Goal | Time | Deliverables |
|-------|------|------|-------------|
| **0** | MVP: Map + Slider + Grok Text | 1 day | Live app, 6 eras, text scene |
| **1** | Visuals | 1 week | AI image, retro UI, share |
| **2** | 3D Preview | 2 weeks | Three.js terrain + flora |
| **3** | Science Layer | 3 weeks | GPlates + Scotese accuracy |
| **4** | VR Ready | 6 weeks | WebXR + Gaussian splat export |
| **5** | Scale & Share | Ongoing | PWA, classroom, API |

---

```markdown
paleo-time-machine/
├── functions/
│   └── index.js          # Single Cloud Function: generatePaleoScene (Grok proxy)
│   └── package.json      # firebase-functions, axios
│   └── .env.example      # GROK_API_KEY
├── public/
│   ├── index.html
│   └── favicon.ico
├── src/
│   ├── components/
│   │   ├── MapPicker.jsx     # Mapbox + search
│   │   ├── TimeMachineSlider.jsx  # 0–100 Ma, 6 era snaps
│   │   └── PaleoScene.jsx    # Text + AI image (placeholder)
│   ├── services/
│   │   └── grok.js           # httpsCallable → generatePaleoScene
│   ├── data/
│   │   └── eras.json         # 6 eras: 0, 5, 15, 50, 70, 100
│   ├── App.jsx
│   ├── main.jsx
│   └── firebase.js           # Firebase init
├── .env.example
├── .gitignore
├── firebase.json
├── package.json          # react, firebase, mapbox-gl, axios, react-slider
├── vite.config.js
└── README.md             # “Slide time. See your world reborn.”
```