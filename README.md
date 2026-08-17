# Waterproof Jetson Orin & FLIR Firefly Enclosure 🌊📷

An industrial, fully weatherproof enclosure designed to house an Nvidia Jetson Orin compute board paired with a Tamron lens and FLIR Firefly camera sensor. Features active thermal management, an articulated camera neck, and 35mm DIN rail compatibility.

![Enclosure Overview](Images/Assembled_System.png)

## 📌 Key Engineering Features

* **Active Thermal Venting:** Integrated housing for the Jetson Orin's stock heatsink and fan, incorporating 70° steeply angled exterior louvers to prevent direct water ingress during active airflow.
* **Passive Water-Shedding Geometry:** Features internal floor planes banked at 10°–15° directing moisture toward a dedicated bottom drip vent, accompanied by exterior runoff lips to break surface tension away from main seams.
* **Articulated Camera Neck:** External high-friction ball-and-socket joint enabling full pan/tilt field-of-view adjustment secured via a knurled locking nut without exposing the main electronics cavity.
* **Custom Printed TPU Gasket:** Interlocking tongue-and-groove channel designed for a 3D-printed flexible TPU gasket seal.
* **DIN Rail Mountable:** Integrated rear bracket formatted for standard 35mm (IEC 60715) industrial mounting rails.

---

## 🛠️ Bill of Materials (BOM)

| Item | Qty | Recommended Material / Spec | Notes |
| :--- | :--- | :--- | :--- |
| Enclosure Shell | 1 | ASA / PETG | Highly UV and temperature resistant |
| Sealing Gasket | 1 | TPU (85A–95A) | 3D-printed continuous flex seal |
| DIN Mount Bracket| 1 | PETG-CF / ASA | High-creep resistance for static load |
| Hardware Fasteners| — | Stainless Steel M3 Screws | Corrosion-resistant assembly hardware |
| Heat-Set Inserts | 4 | M3 Brass Inserts | Melted into lower housing standoffs |

---

## 📂 Repository Layout

* `/CAD_Files/STEP`: Parametric master files for CAD modification.
* `/CAD_Files/STL`: Sliced mesh files ready for 3D printing.
* `/Simulations`: Fluid dynamics and water ingress test reports.
* `/Images`: Renders, exploded views, and assembly photos.

---

## 🔧 Assembly Sequence

1. **Camera Module:** Install the FLIR Firefly sensor and Tamron lens into `Camera_Housing.stl` and close with `Camera_Bottom_Cap.stl`.
2. **Articulated Neck:** Secure `Ball_Socket_Arm.stl` to the recess on `Enclosure_Bottom_Housing.stl`. Pass `Ball_Socket_Collar.stl` over the sphere, adjust camera angle, and thread `Ball_Socket_Lock_Nut.stl` to clamp in position.
3. **Main Electronics:** Press M3 heat-set inserts into the interior standoffs of `Enclosure_Bottom_Housing.stl`. Secure the Jetson Orin board.
4. **Sealing & Closure:** Place the printed `TPU_Sealing_Gasket.stl` into the tongue-and-groove channel. Align `Enclosure_Top_Cover.stl` and torque down corner M3 screws in a cross pattern.
5. **DIN Installation:** Bolt `DIN_Rail_Mount_Bracket.stl` to the rear heat-set inserts and clip the assembly onto the 35mm DIN rail.
