# Double Bass Trolley DIY
**Manual + Downloads to Build Your Own Double Bass Trolley** *(Work in Progress)*

---

## Introduction

About ten years ago, I purchased one of the last available **Double Trolley** models by [Marc Grue](https://www.doubletrolley.com). It was a fantastic combination: a trolley with large, sturdy wheels that made it easy to walk—even up and down stairs—with an integrated stool. While the seat took some getting used to (it’s a bit small), it worked perfectly for me.

However, over time, my Double Trolley has started to wear out. Unfortunately, it’s no longer available for purchase, and secondhand models are nearly impossible to find. I understand why: if something works well, you don’t just let it go.

After years of searching for a suitable replacement without success, I decided to take matters into my own hands and build one myself. For now, this design does not include a stool, but the flexibility of 3D printing means I can easily adapt it later. I might even integrate it with an existing stool, allowing me to transport both my double bass and stool as a single unit.

This is my current design, which I’m actively testing. My goal is to share the design, bill of materials (BOM), and STL files so that other double bassists can build and enjoy their own version.

Regards,
Eef

![Double Bass Trolley Design](https://github.com/user-attachments/assets/1983f12f-a4c4-4e38-a17f-96b05220d5da)

---

## Wheel Selection and Bearing Housing

### Wheel Choice
Without wheels, there’s no trolley. **12-inch wheels** are ideal: large enough to clear bumps but not so large that they compromise flexibility. This size also makes them perfect for navigating stairs.
For reference, [this Amazon listing](https://www.amazon.nl/Achterwiel-reservewiel-fietsbanden-veelzijdige-toepassing/dp/B0F9J1QZNZ) shows what these wheels look like.
*(I found them on a second-hand marketplace attached to a child’s bike.)*

---

### Wheel Construction
The wheel (plastic) contains two **6001ZZ bearings** pressed into either side, with the following dimensions:
- **Outer diameter**: 28 mm
- **Inner diameter**: 12 mm
- **Height**: 8 mm
- **Outer diameter of the inner ring**: 16.5 mm

---

### Securing the Wheel
To secure the wheel unilaterally in a tube, I use **M12 bolts** and 3D-printed bushings/plugs. The assembly (from left to right) consists of:
1. A **seal** that fits inside/on the tube.
2. A **flexible ring** that fits snugly into the bushing.
3. A **cone** that pushes the ring outward, clamping it in place.
4. A **self-locking nut** that holds the wheel in place while pressing all components together.

![Assembly Diagram](https://github.com/user-attachments/assets/54c2eb06-50b7-433d-84c9-6775a9440de2)

To ensure this works with a single bolt, the design must include a column of components that can push against each other **without displacing or clamping the bearings**. This is achieved with the following structure:
- **Green**: The axle (an M12 bolt).
- **Red**: The bearings.
- **Blue**:
  - **Shim rings** (middle section): Must fit precisely on the inner ring of the bearing.
  - **Bearing housing**: Fits snugly on the inner ring and transfers pressure to the tube seal.
  - 
<img width="394" height="202" alt="image" src="https://github.com/user-attachments/assets/f6f2151c-ef38-4caa-b25a-f2cb528da07c" />

---
### Dimensions and Tolerances
- **General tolerance**: ±0.1 mm
- **Shim rings**:
  - **Inner diameter**: Slightly larger than 12 mm (target: **12.1 mm**).
  - **Outer diameter**: Maximum **17 mm**.
  - **Thickness**: **1.5–2 mm**.
- **Bearing housing**:
  - **Inner diameter**: Slightly larger than 12 mm (target: **12.1 mm**).
  - **Outer diameter**: Can be larger (up to **20 mm**; a wall thickness of **3–4 mm** is substantial).
    - *Note*: If the outer diameter exceeds 17 mm, **chamfer the ends** to avoid pressing on the wrong parts of the bearings.
  - **Thickness**: **34 mm** (so the total height of two bearings (2 × 8 mm) + housing equals **50 mm**).
    - **Important**: Measure first! Depending on the wheels, the thickness might need slight adjustment to avoid pressure on the bearings. Use your slicer to scale the model to the correct size if necessary.
    - <img width="390" height="164" alt="image" src="https://github.com/user-attachments/assets/5e16f7d9-d866-42dc-8dd8-d8afd1b01106" /> 
_    (could be all 3d printed, or in metal. My suggestion is to print the bearing housing and use metal shims (see BOM-list))_

