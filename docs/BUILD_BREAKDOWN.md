# Build Breakdown

The scene is assembled in 18 named stages. The order mirrors the calls in the procedural build script.

| Stage | Build area | Purpose |
|---:|---|---|
| 01 | Royal throne | Establishes the backrest, arch, pillars, seat, cushion and arm supports |
| 02 | Body | Creates the main body, belly and shoulders |
| 03 | Elephant head | Builds the head and cheeks |
| 04 | Ears | Adds outer and inner ear forms |
| 05 | Curved trunk | Uses a Bezier curve and a separate tip object |
| 06 | Eyes and eyebrows | Adds eye whites, pupils and eyebrow curves |
| 07 | Tusks | Adds two curved ivory tusks |
| 08 | Crown | Builds layered crown forms, bands and jewels |
| 09 | Four arms | Constructs the upper and lower arm forms |
| 10 | Palms and fingers | Adds hand shapes and finger details |
| 11 | Modak and lotus | Places symbolic objects in the hands |
| 12 | Dhoti | Adds the garment, waist border and pleat curves |
| 13 | Legs | Builds the visible thighs, lower legs and feet |
| 14 | Jewellery | Adds necklaces, chest jewel, armlets and bracelets |
| 15 | Halo | Creates concentric halo rings and decorative rays |
| 16 | Festival greeting | Adds the two-line greeting and underline decoration |
| 17 | Mushika | Builds the mouse companion and its small ornaments |
| 18 | Lighting and final setup | Adds the base, background, area lights, camera and render settings |

## Construction patterns

The source uses small reusable helpers to keep repeated geometry operations consistent:

- `sphere()` creates a UV sphere, applies scale and assigns a material.
- `cylinder()` aligns a cylinder between two 3D points using vector orientation.
- `cone()` creates tapered forms.
- `torus()` creates rings and circular ornaments.
- `curve()` creates a 3D Bezier curve with bevel thickness.
- `material()` centralises material colour, metallic and roughness settings.
- `stage()` prints progress before each major construction stage.

## Render configuration

The script configures an 850 × 1000 PNG render, uses Eevee Next when available, and falls back to Eevee for older Blender versions. Five area lights illuminate the composition.

> The script clears the active scene before building. Use a new or disposable Blender scene if you need to preserve existing work.
