---
layout: post
title: Robotics Studio
description:  Modeled and built a quadrupedal robot capable of moving
skills: 
- SolidWorks CAD
main-image: /robot-isometric.png
---

## Design Process
During the design phase, I took inspiration from Black Mirror's metalhead as well as Boston Dynamics' Spot. I was constrained to using 8 servo motors, and thus although a metalhead type design would not be possible, I still wanted to pursue a futuristic design that emulated the femur and tibia's function in the human body.

## Key Components
To achieve motion capabilities in my design, I integrated a power and control system consisting of a battery, Raspberry Pi, power converter, motor controller, and eight DC servo motors. Each component played a crucial role in ensuring smooth and precise motion control.

### Power System:
I used a rechargeable battery to provide a stable power source for all components. The battery was selected based on the voltage and current requirements of the motors and control electronics, ensuring sufficient power for extended operation.
Since different components required varying voltage levels, a power converter was incorporated to regulate the voltage appropriately. This ensured that both the Raspberry Pi and the motors received the necessary power without overloading the system.

### Control System:
The Raspberry Pi served as the central processing unit, handling control algorithms, motion sequencing, and communication with peripheral components. It was programmed using Python to send precise pulse-width modulation (PWM) signals for motor control.
The Raspberry Pi interfaced with a motor controller, which acted as an intermediary between the low-power control signals and the high-power requirements of the DC servo motors. The motor controller ensured smooth operation by regulating speed, torque, and direction based on input commands.

### Motion Execution:
I utilized eight DC servo motors, each selected for their high precision and torque capabilities. These servos were strategically positioned to enable the desired degrees of freedom in motion.
The motors operated based on PWM signals from the motor controller, allowing for fine-tuned movement adjustments. Feedback from the servos ensured accurate positioning and dynamic response to control inputs.
By integrating these components, I created a system capable of precise and responsive motion, essential for applications requiring automation, robotics, or controlled actuation.
