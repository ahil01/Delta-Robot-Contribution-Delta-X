# Delta-Robot-Contribution-Delta-X
A rigid, vision-guided Delta robot built for speed and precision. Powered by a 32-bit controller and Raspberry Pi, it features zero-backlash NEMA 23 actuation, a lightweight structural design, and an adjustable-angle camera—delivering industrial pick-and-place performance with standard parallel kinematic efficiency.
<img width="913" height="771" alt="f" src="https://github.com/user-attachments/assets/9ee11bd6-ca5e-4e64-8cf5-4b8befd44484" />

High-Precision, Vision-Enabled High-Speed Delta RobotAn advanced iteration of the open-source Delta X platform, redesigned from the ground up for high-speed pick-and-place, computer vision tasks, and industrial reliability. While preserving the core parallel kinematics, this build upgrades the mechanical rigidity, motion control architecture, and vision capabilities.

# Key Engineering UpgradesDistributed Compute & Motion Architecture:
Distributed Compute & Motion Architecture: Integrated a 32-bit motion controller paired with a Raspberry Pi coprocessor. This separates high-frequency real-time kinematic calculations and step generation from high-level computer vision and trajectory planning.

<img width="554" height="554" alt="Circuit" src="https://github.com/user-attachments/assets/56cddccb-577e-4def-b32f-212c24dd7763" />

Zero-Backlash High-Torque Actuation: Upgraded to high-torque NEMA 23 stepper motors paired with zero-backlash drive systems, eliminating mechanical slop, enhancing repeatability, and preventing step skips during rapid acceleration.

<img width="1917" height="1073" alt="Screenshot 2026-08-16 010918" src="https://github.com/user-attachments/assets/c4ed02f6-db0a-4fe1-84b1-9670c305f842" />

Lightweight & High-Rigidity Arm Assembly: Re-engineered the arm structure to minimize moving inertia while maximizing torsional rigidity, allowing for significantly higher acceleration curves without frame deflection or end-effector vibration.

<img width="1918" height="905" alt="Screenshot 2026-08-15 000900" src="https://github.com/user-attachments/assets/803a8377-73f4-4dbd-9c3a-93cd50954505" />

Dynamic-Angle Vision System: Equipped with an adjustable-angle camera mount, enabling top-down, tilted, and real-time object tracking for adaptable sorting, classification, and inspection pipelines.

<img width="1919" height="1079" alt="Screenshot 2026-08-16 010600" src="https://github.com/user-attachments/assets/a9217b82-0a51-41a6-8f77-0d2a1cdefa47" />

# UPGRADE FEATURES

🦾 1. Mechanical & Structural Design
80% 3D-Printable Architecture: Fully redesigned components optimized for FDM/FFF 3D printing with clean overhangs and minimal support requirements.

Fast & Foolproof Assembly: Uses modular interlocking joints, standardized fasteners (e.g., M3/M4 heat-set inserts and bolts), and keyed alignments for quick, repeatable assembly without complex jigs.

High Rigidity-to-Weight Ratio: Reinforced load paths and internal geometric ribbing significantly increase torsional and bending stiffness while keeping moving mass minimal.

Vibration & Resonance Damping: Minimized end-effector inertia eliminates overshoot and resonance ringing during high-acceleration stops.

<img width="1149" height="753" alt="Screenshot 2026-08-16 194044" src="https://github.com/user-attachments/assets/6aa293fe-6b4e-48b9-8187-138a53bde880" />


⚡ 2. Actuation & Precision Motion
High-Torque NEMA 23 Motors: Upgraded from standard NEMA 17 to NEMA 23 stepper motors, delivering significantly higher holding torque and dynamic payload capacity.

Zero-Backlash Drive Mechanism: Precision transmission design completely eliminates mechanical backlash, ensuring accurate micro-positioning and zero slop on directional reversals.

Enhanced Acceleration Profiles: High torque-to-inertia ratio allows aggressive acceleration and deceleration curves without missed steps.

🧠 3. Compute & Control Architecture
Distributed Hybrid Processing:

Raspberry Pi Coprocessor: Handles high-level computer vision pipelines (OpenCV), motion planning, coordinate mapping, and network/GUI interfaces.

Dedicated 32-Bit Motion Controller: Manages real-time trigonometric kinematics calculations, high-frequency step pulse generation, lookahead buffering, and endstop interrupts with microsecond precision.

Deterministic Low-Latency Communication: Fast UART/Serial bridge between Raspberry Pi and the 32-bit controller ensures seamless G-code and trajectory execution.

👁️ 4. Dynamic Vision SystemAdjustable-Angle Camera Mount: Hardware-integrated camera bracket with variable tilt angle to accommodate top-down workspace inspection, oblique conveyor tracking, or tilted bin picking.Real-Time Object Detection & Sorting: Directly streams low-latency video to the onboard Raspberry Pi for color detection, contour extraction, bounding box estimation, and orientation detection.Adaptive Coordinate Calibration: Software-calibrated coordinate transformation mapping visual pixel coordinates directly into the Delta robot's Cartesian ($X, Y, Z$) coordinate frame


📐 5. Kinematics & Compatibility
Preserved 3-DOF Parallel Kinematics: Retains standard Delta parallel geometry, maintaining identical kinematic equations.

Universal G-Code Compatibility: Works with standard trajectory generators, slicers, and automation toolpaths without requiring custom kinematics drivers.





