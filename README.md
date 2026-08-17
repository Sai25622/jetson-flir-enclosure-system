# Waterproof Jetson Orin & FLIR Firefly Enclosure 🌊📷

An industrial, fully weatherproof enclosure designed to house an Nvidia Jetson Orin compute board paired with a Tamron lens and FLIR Firefly camera sensor. Features active thermal management, articulated pivot arms, dedicated sealing gaskets, and a snap-on DIN rail interface.

![Enclosure Overview](ImagesAssembled_System.png)

## 📌 Key Engineering Features

* **Complete Sealing Protection:** Uses dedicated 3D-printed TPU gaskets including a **Main Enclosure Gasket**, a **Sensor Camera Gasket** for the FLIR lens module, and a **Sensor Wire Gasket** to seal the cable entry into the FLIR sensor.
* **Articulated Pivot Mount:** Adjustable **Pivot Arms** coupled with a **T-Mount Plate** allowing precise pan-and-tilt aiming of the sensor assembly.
* **DIN Rail Mounting:** The T-Mount Plate secures directly into a **DIN Rail Clip** that snaps onto standard 35mm (IEC 60715) industrial mounting rails.
* **Active Thermal Venting:** Integrated housing for the Jetson Orin's stock heatsink and fan with steeply angled 70° louvers to block rain ingress during active airflow.
* **Passive Water Drainage:** Banked interior flooring (10°–15°) with drip channels directing condensation safely away from core electronics.

---

## 🛠️ Bill of Materials (BOM)

### 3D Printed Parts
| Part | Qty | Material | Function |
| :--- | :---: | :--- | :--- |
| Main Enclosure Body | 1 | ASA / PETG | Primary weatherproof housing |
| Main Enclosure Gasket | 1 | TPU (85A–95A) | Tongue-and-groove enclosure seal |
| Sensor Camera Gasket | 1 | TPU (85A–95A) | Weatherproof seal for FLIR camera housing |
| Sensor Wire Gasket | 1 | TPU (85A–95A) | Cable pass-through gasket for FLIR wiring |
| Pivot Arms | 1 | PETG-CF / ASA | Articulated positioning arms |
| T-Mount Plate | 1 | PETG-CF / ASA | Interface between Pivot Arms and DIN clip |
| DIN Rail Clip | 1 | PETG-CF / ASA | Snaps onto 35mm DIN rail |

### Hardware & Fasteners
| Fastener / Part | Qty | Description & Supplier Link |
| :--- | :---: | :--- |
| **M4 x 25mm Hex Bolts** | 25 | [M4 x 25mm Hex Bolt SS304 (OnlyScrews)](https://onlyscrews.in/products/m4-x-30mm-hex-allen-socket-head-ss-304-screw) |
| **M4 Hex Nuts** | 25 | [M4 Hex Nut SS304 (OnlyScrews)](https://onlyscrews.in/products/m4-nut-ss-304) |
| **M4 Heat-Set Inserts** | 12 | Brass M4 heated inserts for mounting standoffs |

---

## 🔧 Assembly Sequence

1. **FLIR Sensor & Camera Assembly:**
   * Fit the **Sensor Camera Gasket** onto the housing rim and secure the FLIR Firefly camera sensor and Tamron lens inside `Camera_Housing.stl`.
   * Pass the FLIR wiring harness through the **Sensor Wire Gasket** to establish a watertight cable entry point before closing with `Camera_Bottom_Cap.stl`.

2. **Articulation & Mount Integration:**
   * Assemble the **Pivot Arms** to the camera housing using M4 x 25mm hex bolts and M4 nuts.
   * Attach the **T-Mount Plate** to the end of the Pivot Arms.
   * Secure the **T-Mount Plate** into the **DIN Rail Clip**.

3. **Internal Electronics Installation:**
   * Press the 12 **M4 Brass Heat-Set Inserts** into the internal mounting bosses of `Enclosure_Bottom_Housing.stl` using a soldering iron.
   * Secure the Jetson Orin compute unit onto the bottom standoffs using M4 bolts.

4. **Main Enclosure Sealing & Mounting:**
   * Press the **Main Enclosure Gasket** into the perimeter channel of `Enclosure_Bottom_Housing.stl`.
   * Align `Enclosure_Top_Cover.stl` and tighten down the outer M4 x 25mm hex bolts and nuts evenly in a cross pattern to compress the gasket.
   * Snap the assembled **DIN Rail Clip** directly onto your 35mm DIN rail.
