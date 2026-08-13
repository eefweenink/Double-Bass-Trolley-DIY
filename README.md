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

For reference, [this Amazon listing](https://www.amazon.nl/Achterwiel-reservewiel-fietsbanden-veelzijdige-toepassing/dp/B0F9J1QZNZ) shows what these wheels look like. I found mine on **Marktplaats** (a Dutch second-hand marketplace), attached to a child’s bike.

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

![Bearing Housing Diagram](https://github.com/user-attachments/assets/f6f2151c-ef38-4caa-b25a-f2cb528da07c)

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

![Dimensions Diagram](https://github.com/user-attachments/assets/5e16f7d9-d866-42dc-8dd8-d8afd1b01106)

> *The bearing housing and shim rings can be 3D printed or made of metal. My suggestion is to 3D print the bearing housing and use metal shims (see BOM list).*
>
> ## Materials Used

### Structural Components
- **Aluminum tube**:
  - **Outer diameter**: 33.3 mm
  - **Wall thickness**: 3 mm
  - **Purpose**: Used as the axle for mounting the wheels (see [Securing the Wheel](#securing-the-wheel)). Together with three other sections, it forms a sturdy rectangular frame that serves as the base of the trolley.
  - **Dimensions**:
    - **Axle length**: 38 cm (for my double bass in its bag).
    - **Vertical tubes**: 50 cm each (two pieces) May also be longer, about 65 cm so the top crossbar comes above the upper bout.
    - **Top crossbar**: ~31.3 cm (calculated as `38 cm - (2 × 3.33 mm)`).

- **Tyreen tubing**:
  - **Diameter**: 20.2 mm
  - **Purpose**: Used to build the side supports. This tubing has a **fixed curvature**, so it is important to rotate the pieces favorably during assembly.

---

### 3D-Printed and Fastening Components
- **PETG filament**:
  - All couplings and connecting parts are 3D-printed using PETG.
  - **Printer volume**: 12 × 12 × 12 cm (all parts fit within this build volume, so no large printer is required).

- **Fastening cord**:
  - **Material**: 3.5 mm **paracord** (with a tensile strength of **150 kg**, more than sufficient for a double bass).
  - **Setup**:
    - **Lower loop**: Passes through the tubes and around the end pin.
    - **Upper loop**: Passes through the tubes and, using a **"spin elastic/span band"**, secures the neck.
    - Both loops pull in **opposite directions**, pressing the tube system firmly together toward the center.

---
### Additional Hardware
- **Metal hook**: Used to attach the cord to the end pin.
- **2 × M12 bolts**: For securing the wheel assembly.
- **4 × shim rings**: Prevent the force from the wheel mounting from pressing on the outer side of the bearings.


## End Hook and Accessories for Easy Spin Attachment
#<img width="2670" height="3846" alt="IMG_3240" src="https://github.com/user-attachments/assets/3ff9284a-0137-4ee9-8b57-7990a13b5342" />
The trolley is secured at the bottom with a hook around the **end pin**. Finding a well-fitting hook for this purpose isn’t straightforward, but this [hook from Amazon](https://www.amazon.nl/dp/B0C6HJWLKB) works reasonably well.

However, during use, the cord tends to slip between the iron wires of the hook, causing it to bend out of shape. To solve this, I designed a **protective "donut"** that shields the hook.
<img width="3019" height="2720" alt="IMG_3239" src="https://github.com/user-attachments/assets/e60de541-bafc-4bba-b381-36871a0630ea" />

### Printing the Donut
To print the donut:
1. **Positioning the hook**: The hook must be placed at the correct height inside the donut. This is easily achieved by using a **pause feature in the slicer**.
2. **Support structure**: Add **manual support** (only for the bottom surface, using the "tree" support type) to the donut in the slicer.
3. **Alignment tool**: Use a **1 mm thin rod** of the correct length to ensure the donut is printed at the right height.
4. **Printing process**:
   - Pause the print at the designated height.
   - Insert the hook neatly into the donut.
   - Resume the print.
<img width="476" height="315" alt="Scherm­afbeelding 2026-08-13 om 20 52 30" src="https://github.com/user-attachments/assets/5d585123-909d-4dd2-b0f4-106b4e60eb2b" />
<img width="2116" height="4028" alt="IMG_3238" src="https://github.com/user-attachments/assets/aaf13291-55de-4b98-9899-0a866331aeb5" />

> **Note**: The same design is used to create rings for the **top section**, making it easy to hook in the spin elastic.

<img width="411" height="341" alt="Scherm­afbeelding 2026-08-13 om 20 54 21" src="https://github.com/user-attachments/assets/eee11015-f3ec-4dbb-ac85-6c3cfd709f16" />

![Hook and Donut Assembly](image_url_1)
![Slicer Setup](image_url_2)
