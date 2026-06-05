# Automated Crop Detection Cart

An autonomous cart designed for agricultural crop detection, built around
an STM32 microcontroller. The system uses ultrasonic and IR sensors to
detect crop height in real-time and automates cart navigation accordingly.
Built as a university microprocessors course project.

**February 2025 – June 2025**

---

## Overview

This project is a fully functional autonomous cart prototype designed to
simulate crop detection in an agricultural environment. The STM32
microcontroller processes data from ultrasonic and IR sensors to
differentiate crop heights and trigger automated navigation responses.
DC motors controlled via H-bridges handle cart movement, adjusting
direction and speed based on live sensor input. The system was tested
and calibrated across multiple agricultural simulation environments
to ensure reliable real-time performance.

---

## Features

- Real-time crop height detection using ultrasonic and IR sensors
- Automated cart navigation driven by live sensor data
- DC motor control via H-bridge for direction and speed adjustment
- Embedded C logic to differentiate between crop heights and
  trigger corresponding selection responses
- Sensors calibrated for accuracy across varying simulation environments
- Fully functional prototype delivering autonomous pick-and-navigate behavior

---

## Hardware Components

| Component                        | Quantity |
|----------------------------------|----------|
| STM32 Microcontroller            | 1        |
| HC-SR04 Ultrasonic Sensor        | 1        |
| IR Sensors                       | 1        |
| DC Motors                        | 2        |
| H-Bridge Motor Driver            | 1        |
| Breadboard                       | 1        |
| Jumper Wires                     | —        |


---

## Software & Tools

- Embedded C
- STM32CubeIDE
- Proteus Simulation
- Libraries used: in code folder

---

## How It Works

1. On power-up, the STM32 initializes all sensors and motor drivers
2. The ultrasonic sensor continuously measures distance to detect
   crop presence and estimate height
3. IR sensors provide additional input for short-range crop detection
   and surface differentiation
4. The microcontroller processes both sensor inputs and classifies
   the detected crop height
5. Based on the classification, the H-bridge motor driver adjusts
   cart movement — stopping, turning, or continuing forward
6. The system loops continuously, enabling fully autonomous navigation
   through a simulated crop environment

---

## Simulation

A circuit simulation was designed in Proteus prior to physical assembly
to validate component wiring and logic before committing to the hardware build.

**Tools used:** Proteus
 : <img width="828" height="578" alt="Screenshot 2026-06-05 134740" src="https://github.com/user-attachments/assets/9a4c40d2-67ed-4d37-99bf-612f2ea6b358" />

