# Glassy
### Transform any image into a stylized corrugated glass poster with irregular vertical ribs, glue-like distortion, and a centered acrylic window — all powered by pure HTML Canvas (no WebGL, no libraries, fully client-side).

link: https://triloux.github.io/glassy/

This effect is inspired by modern graphic posters that use rippled acrylic sheets to bend and smear the subject in a fluid, glass-like way.

---

## 🚀 Features

| Feature |
|--------|
| Upload any image (portrait recommended for best results) |
| Centered distortion window (70% of the canvas) |
| Irregular vertical glass ribs |
| Micro-ripples to mimic liquid/glue distortions |
| Subtle downward “drip” bias for realism |
| Adjustable rib density |
| Adjustable distortion strength |
| Clean white/chrome border around the glass area |
| Fully client-side — no backend, no dependencies |
| Works offline |

---

## 🧩 How it Works

Inside the central square, each vertical slice of the image is remapped with:

- A base sine wave
- Micro-high-frequency ripples
- A rib-shape function to vary rib thickness
- A downward “drip” term
- Rib shading to simulate acrylic curvature

The result is a more chaotic, gluey, and realistic corrugated-glass effect compared to simple sine-wave distortions.

---

## 📁 Using Locally

- Open the project in a browser (index.html)
- Upload any image (Choose image)

Adjust:

- Glass density → spacing of ribs
- Distortion strength → how wavy/melty the ribs feel
- Click Apply glass effect
- Save your artwork with Download PNG

Clone or download the repo:

Open:

```
index.html
```

That’s it. No build tools, no dependencies.

---

## 🧱 Tech Stack

- Distortion is fully implemented in CPU 2D Canvas (no WebGL)
- getImageData and remapping operations create the effect
- Distortion only affects the central 70% square
- Outer area remains crisp and undistorted
- Rounded-rectangle borders and shadows are drawn via Canvas paths

📷 Recommended Input

- Bright mid-contrast portraits
- Centered subjects
- Simple backgrounds

These produce the most dramatic rib distortion.

---

## 📦 Project Structure

```
/
├── index.html       # Entire app in one file
├── README.md
└── assets/          # (optional future expansion)
```

---

## 📝 License

MIT License — free to use, modify, and ship.

---

## ⭐ Like this project?

Consider starring the repo so more people can find it!
