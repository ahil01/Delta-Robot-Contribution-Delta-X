# Delta-Robot-Contribution-Delta-X

A rigid, vision-guided Delta robot built for speed and precision. Powered by a 32-bit controller and Raspberry Pi, it features zero-backlash NEMA 23 actuation, a lightweight structural design, and an adjustable-angle camera—delivering industrial pick-and-place performance with standard parallel kinematic efficiency.

---

## Key Features & Upgrades

### 1. High-Torque Motion & Actuation
* **NEMA 23 Stepper Motors:** Upgraded from smaller steppers to provide higher torque, faster accelerations, and payload headroom.
* **Anti-Backlash Joints:** Integrated zero-backlash ball joints/linkages to eliminate slop and ensure repeatable sub-millimeter positioning.
* **Reinforced Arm Assembly:** Thicker carbon/aluminum upper and lower arm rods designed to eliminate deflection during rapid moves.
* 
<img width="216" height="233" alt="neam 23" src="https://github.com/user-attachments/assets/3db07be1-dd11-4a73-a9eb-f0f424b12e11" />

<img width="1212" height="788" alt="Screenshot 2026-08-20 110954" src="https://github.com/user-attachments/assets/581cf054-e96b-4adf-b411-a22d2ee27453" />
<img width="1917" height="1073" alt="Screenshot 2026-08-16 010918" src="https://github.com/user-attachments/assets/f38e2c75-d724-4948-8bae-cdaeeb3bc4e9" />
<img width="1149" height="753" alt="Screenshot 2026-08-16 194044" src="https://github.com/user-attachments/assets/dce87ba7-acf3-48cf-baee-bcefb1a2ac9e" />


### 2. Rigid 2040 Extrusion Frame
* **Structural Stability:** Built using heavy **2040 aluminum extrusion profiles** to dampen high-frequency vibrations during aggressive pick-and-place trajectories.
* **Magnetic Quick-Release Base:** Modular top base held magnetically for quick servicing, maintenance, and toolhead adjustments.
* <img width="1262" height="769" alt="Screenshot 2026-08-16 172514" src="https://github.com/user-attachments/assets/7ee78890-fad6-43f8-9df7-0b4554150132" />

* <img width="1402" height="713" alt="Screenshot 2026-08-16 160925" src="https://github.com/user-attachments/assets/8582c84d-dee1-488a-a7f5-cced2006d4cf" />



### 3. Modern 32-Bit Electronics & Connectivity
* **MKS Pico Controller:** 32-bit board running silent **TMC2209 stepper drivers** in UART mode for ultra-quiet operation and precise microstepping.
* **Raspberry Pi Integration:** Onboard SBC handling high-level motion planning, Wi-Fi, Bluetooth, and computer vision feeds.
* **Adjustable Vision Mount:** Integrated camera bracket with angle adjustment for automated object detection and sorting.

<img width="554" height="554" alt="rasp 5" src="https://github.com/user-attachments/assets/ed1e4b0f-c0dd-475c-8a7e-4626461ba208" />

 <img width="1800" height="1600" alt="mks" src="https://github.com/user-attachments/assets/92cc35c0-5f4e-4b2a-aff0-4ece4e95b60b" />
  <img width="725" height="724" alt="Screenshot 2026-08-16 154953" src="https://github.com/user-attachments/assets/a60250cc-110b-4c9f-b11d-7fb2a01e2f09" />





### 4. 3D Printability & Hardware Fastening
* **Heat-Set Threaded Inserts:** Replaced loose hex nuts across all structural parts with standard brass heat-set insertion nuts for durable, repeatable assembly.
* **FDM-Optimized Geometry:** Redesigned printed brackets to print cleanly with minimal supports and maximum layer-bond strength along load axes.![Uploading mks.jpg…]()
<img width="1482" height="783" alt="Screenshot 2026-08-20 111124" src="https://github.com/user-attachments/assets/5fa5a924-5939-43db-8e57-f8bb002d30c8" />


---

## Repository Structure

```text
├── Cad File/          # STEP, CAD, and 3D printable meshes (STL/3MF)
├── Electronic/        # Wiring schematics, pinout diagrams, and board pin configurations
├── Firmware/          # Pre-configured firmware and delta kinematics configuration
├── Img/               # Assembly photos, renders, and demonstration media
├── Thermal Analysis/  # Finite element / thermal simulation data
├── platformio.ini     # PlatformIO build configuration
└── README.md          # Project documentation
