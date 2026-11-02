<div align="center">

# SHREE GANESHA
### A Procedural 3D Creation · Blender × Python

*Where code takes shape, and creativity becomes geometry.*

<br/>

<img src="assets/ganesha-preview.png" alt="Lord Ganesha — procedural 3D artwork" width="420" />

<br/>

**A devotional 3D scene created through procedural modelling and Python scripting.**

[Overview](#the-vision) · [Features](#inside-the-scene) · [Technical approach](#under-the-hood) · [Run it](#getting-started)

</div>

---

## The vision

**SHREE GANESHA** is a creative coding project that explores how a complex 3D composition can be assembled programmatically with Blender's Python API (`bpy`).

Rather than placing every object manually, the scene is constructed from reusable Python functions. Each function creates, positions, scales and shades individual elements before they come together as one composition.

The result is a seated Ganesha figure surrounded by an ornate throne, layered crown, decorative halo and festival details.

> **Code becomes geometry. Geometry becomes a story.**

## Inside the scene

| Composition | Details |
|---|---|
| **The divine form** | Elephant head, expressive eyes, ears, curved trunk, tusks and body |
| **Four arms** | Upper arms, forearms, palms, fingers and hand-held objects |
| **Royal crown** | Layered forms, decorative bands, jewels and a crown point |
| **Ornate throne** | Backrest, arch, pillars, seat, cushion and arm supports |
| **Attire & ornaments** | Dhoti, pleats, necklace, armlets, bracelets and anklets |
| **Sacred accents** | Halo, lotus, modak and Mushika |
| **Final composition** | Festival greeting, lighting, camera and render configuration |

## The build sequence

The script organises construction into **18 named stages**, making the scene easier to follow and debug:

1. Royal throne
2. Ganesha's body
3. Elephant head
4. Ears
5. Curved trunk
6. Eyes and eyebrows
7. Tusks
8. Detailed crown
9. Four arms
10. Palms and fingers
11. Modak and lotus
12. Dhoti
13. Legs
14. Golden jewellery
15. Halo
16. Festival greeting
17. Mushika
18. Lighting and final scene setup

## Under the hood

- **Blender Python API (`bpy`)** — procedural scene construction.
- **Mathutils** — vector calculations and camera/light orientation.
- **Mesh primitives** — UV spheres, cylinders, cones, cubes, planes and tori.
- **Bezier curves** — curved forms and decorative details.
- **Materials** — named material definitions with colour, metallic and roughness properties.
- **Lighting & camera** — a multi-light setup and a dedicated perspective camera.
- **Rendering** — Eevee Next with a fallback for earlier Eevee versions.

## Getting started

### Requirements

- Blender with Python scripting support.
- Blender's bundled `bpy` and `mathutils` modules.

### Run inside Blender

1. Open Blender and switch to the **Scripting** workspace.
2. Open `ganesha.py` in the Text Editor.
3. Select **Run Script**.
4. Follow the 18 build stages in the system console.

### Run from a terminal

```bash
blender --background --python ganesha.py
```

Run the command from the project directory. The script configures an 850 × 1000 PNG render and saves the Blender scene using a relative output path.

> **Note:** The script clears the active Blender scene before building. Run it in a new or disposable scene if you need to preserve existing work.

## Project structure

```text
Ganesha-3D-Blender-Python/
├── assets/
│   └── ganesha-preview.png
├── docs/
│   ├── BUILD_BREAKDOWN.md
│   └── PROJECT_OVERVIEW.md
├── ganesha.py
├── Ganesha_Chaturthi_Final.blend
├── .gitignore
└── README.md
```

## Why this project matters

This project sits at the intersection of **Python programming, procedural modelling and visual storytelling**. It demonstrates a different use of programming: not only automating workflows or building applications, but also creating a detailed visual composition from reusable code.

---

<div align="center">

### गणपति बाप्पा मोरया 🙏

*Created with Blender + Python.*

</div>
