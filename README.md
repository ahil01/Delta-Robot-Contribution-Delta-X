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

![Uploading Screenshot 2026-08-16 010600.png…]()

Feature,Base Delta X,Custom Upgraded Build,Impact / Advantage
Control Board,8-bit / Basic MCU,32-Bit Dedicated Board,"Smoother microstepping, faster lookahead, higher step frequencies"
SBC Coprocessor,None / Host PC dependent,Raspberry Pi Onboard,"Standalone operation, onboard OpenCV/AI model inference"
Motors & Drive,Standard NEMA 17,Zero-Backlash NEMA 23,"Greater payload capacity, zero backlash, pinpoint repeatability"
Vision Module,Fixed / Optional,Variable-Angle Vision Mount,Flexible workspace coverage and adaptive depth/angle tracking
Chassis & Arms,Standard 3D printed / standard tubing,Optimized Lightweight & Rigid Frame,"Reduced inertia, dampens resonance, higher acceleration rates"
Kinematics,Standard 3-DOF Parallel,Identical Kinematics,Full software and toolpath compatibility with standard Delta workflows


