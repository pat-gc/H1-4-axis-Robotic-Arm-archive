# H1-4-axis-Robotic-Arm-archive

A 4-degree-of-freedom robotic arm I designed and built in 6 weeks for my IB Personal Project.

<img width="1110" height="636" alt="image" src="https://github.com/user-attachments/assets/1c76d511-760f-48a0-aa36-b59e732d185b" />

The arm has a **70 cm reach** and a **200 g payload capacity**. It was built mostly from salvaged parts, with around **$50 spent on new electronics**.

## Hardware

- NEMA 17 stepper motors
- Raspberry Pi Pico (RP2040)
- TMC2209 stepper motor drivers
- Custom 3D-printed parts
- 2020 aluminum extrusions
- GT2 belts and pulleys
- Linear rails and bearings
- 12 V power supply

The elbow uses a **10:1 belt reduction** (14-tooth to 140-tooth pulley) to increase torque without needing a larger motor.

## Software

I wrote custom firmware for the RP2040 to control the stepper motors through serial commands, including step generation and motor timing.

## Problems Encountered

The biggest issues were electrical.

Since I couldn't afford a custom PCB, I wired everything manually using prototyping boards and soldered connections.

The first version worked for a few minutes before the motor drivers burned out. I suspected problems with grounding and power distribution.

After replacing the drivers and rebuilding the wiring, the arm worked again. However, during the final exhibition, some drivers began failing and solder joints broke.

The mechanical system worked, but the electronics weren't reliable enough for extended operation.

## What I'd Improve

- Design a custom PCB with proper power distribution
- Add electrical protection and better connectors
- Improve cable management and strain relief
- Add position feedback and homing
- Implement inverse kinematics and coordinated motion control

## Result

I completed and demonstrated the original prototype within **6 weeks**, using mostly reused components and approximately **$50 in new electronics**.

The arm successfully moved under software control, although electrical reliability remained an issue.

**Status:** Prototype completed; further improvements planned.

<img width="3024" height="4032" alt="IMG_1086" src="https://github.com/user-attachments/assets/367f9986-3b35-4781-9f82-cc6a8ea4359c" />
*yep, 3D printer broke down before I could add a proper grabber
*


