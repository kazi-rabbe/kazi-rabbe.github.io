---
layout: post
title: FLEX Fitness System
description:  FLEX, or the Fitness-Feedback Lifting Experience, is a smart belt and double arm band system tailored for weightlifters. The fitness wearables integrate an array of sensors that identify improper form and insufficient muscle activation to provide real-time correctional haptic feedback and prevent injury. This data, delivered via in-app analytics, helps maximize results in the gym. The user’s role is to strap on and tighten the belt and bands while ensuring correct muscle placement, enter the app, calibrate it, select their desired exercise, and simply begin working out.
skills: 
- Solidworks CAD
- Rhino 3D
main-image: /FLEX.jpg
---

# Background
There is a need within the industry for a product
that provides real-time sensory feedback to muscle activity
so as to prevent injury and maximize results in the gym. This
is exactly what FLEX aims to do: provide real-time feedback
for users to adjust their form to optimize their muscle growth
and avoid injury through a belt and band system. To do this, we prioritized
mobility, adjustability, and ease of use--all packaged into a
product with sleek form factor.

# The Creation Process
## Sensor Selection
Various sensors were tested using an Arduino to evaluate their functionality for different components of the wearable system. Square force-sensitive resistors (FSRs) were chosen for core muscle sensing due to their superior resolution when tested with an air pump apparatus. For the armband, a flexible FSR was selected over alternatives like conductive rubber, the Loomia pressure matrix, and strain gauges, as it provided reliable readings while allowing movement. To monitor back posture, force-resistive flex sensors were assessed using 3D-printed curvature blocks, with the 4.40-inch SparkFun flex sensor showing the best resolution. 

## Form Factor
The design prioritized flexibility, compactness, and lightweight construction for wearable comfort, avoiding rigid materials except where necessary. Rigid components like the controller and battery were cushioned with foam and enclosed in silicone housing to comply with UL 1642 standards. Through iterative development, mass and volume were reduced to achieve a final 1cm thickness by optimizing foam, silicone, and electronic component selection. Conductive threading was used for discreet wiring of haptic motors, but stranded core wires were chosen for more durable sensor connections. The final design balanced spatial efficiency with seamless integration of functional components.

## Wireless Communication
The device uses the Raspberry Pi Zero 2 for wireless connectivity, ensuring obstruction-free operation during workouts. It integrates with the Blynk IoT platform, which provides real-time feedback on core engagement, posture, muscle activation, and arm tilt via a smartphone dashboard. During prototyping, programming was primarily done using the Serial USB port upload method for efficiency.

## Repeatability
To ensure consistent sensor readings, flex sensor data was recorded across multiple trials while users bent forward to a 30-degree lean. A one-way ANOVA test confirmed consistent sensor readings across multiple trials (p = 0.3068), ensuring reliable detection of back curvature.

## Heat Transfer
A heat transfer FEA study in SolidWorks was performed to maintain safe operating temperatures for the belt. Materials were assigned based on their properties, and a mesh convergence test ensured accurate results. Thermal loads and temperature limits were analyzed according to IEEE Standard 360-2022, allowing for design adjustments if necessary to prevent overheating. Initial FEA results showed excessive heat, prompting design adjustments such as increasing silicone rubber thickness. A 3mm thickness was found optimal, reducing temperature while maintaining flexibility.

## Power Analysis
Power consumption analysis led to the selection of 150 mAh batteries, which provide adequate runtime (2.5 hours for the belt, 1.1 hours for the band) while avoiding excessive heat risks.

[Click to learn more](https://www.canva.com/design/DAGgQ0ZwQMQ/fS4ipzphQ-U35H5JEPUKRA/view?utm_content=DAGgQ0ZwQMQ&utm_campaign=designshare&utm_medium=link2&utm_source=uniquelinks&utlId=h7acc439f47)
