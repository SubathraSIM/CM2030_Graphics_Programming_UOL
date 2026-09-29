# CM2030 Graphics Programming - University of London

Coursework for **CM2030 Graphics Programming** (BSc Computer Science, University of London), covering interactive 2D graphics, physics simulation, and real-time image processing in JavaScript.

| Assessment | Project | Key topics |
|---|---|---|
| [Midterm](./GP_mid_term) | Snooker game | Physics engine, collision detection, user interaction |
| [Endterm](./End_term) | Webcam image processing app | Thresholding, colour space conversion, segmentation |

**Tech:** JavaScript · p5.js · Matter.js

---

## Midterm - Snooker Game

A playable snooker table built with p5.js and the Matter.js physics engine.

- Table, cushions, and pockets drawn to standard snooker proportions
- Cue ball controlled by the player with aim and shot power
- Realistic ball-to-ball and ball-to-cushion collisions with friction and restitution
- Multiple ball layout modes (e.g. standard setup and randomised positions)
- Potted balls detected and handled according to game rules

---

## Endterm - Image Processing with Colour Spaces

An interactive image processing application that applies multiple filters to a live webcam feed or an uploaded image, displayed side by side in a grid.

**Core features**
- Independent thresholding of the **R, G, and B channels** using sliders
- Colour space conversion to **YCbCr** and **HSV**, with thresholding on the converted images
- Comparison of RGB thresholding against colour space–based thresholding. Separating brightness from colour gave more consistent results under changing lighting.

**Extensions**
1. **HSL conversion and thresholding:** hue-based filtering for more precise colour segmentation
2. **Background segmentation:** background subtraction with a colour picker to replace the background
3. **Load external images:** apply all filters to uploaded photos, not just the webcam
4. **Capture button:** save the full processed grid as a JPEG
5. **Zoom in/out:** click any filter in the grid to enlarge it and inspect details

**Challenges solved**
- Inconsistent thresholds across lighting conditions → adjustable sliders
- Stray artefacts in the segmentation mask → light blurring of the mask
- Keeping a clean multi-image layout → calculated grid positioning

---

## How to run

1. Clone the repo
2. Open `index.html` in the `midterm` or `endterm` folder using a local server (e.g. VS Code Live Server)
3. For the endterm, allow webcam access when prompted
