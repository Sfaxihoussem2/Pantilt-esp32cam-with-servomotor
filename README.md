# ESP32-CAM Pan-Tilt System with Servo Motors

**Camera positioning system that combines an ESP32-CAM with servo motors to provide remote pan and tilt control.**

---

## Project Overview

This project implements a motorized camera mount using an ESP32-CAM and two (or more) servo motors. It allows remote adjustment of the camera’s horizontal (pan) and vertical (tilt) orientation, making it useful for surveillance, robotics vision, inspection, or interactive camera applications.

---

## Key Features

- ESP32-CAM for video capture / streaming
- Servo-based pan and tilt control
- Remote control capability (typically via web interface or serial/WebSocket commands)
- Compact hardware suitable for prototyping and integration into larger systems

---

## Hardware

- ESP32-CAM (AI-Thinker or equivalent)
- 2× Servo motors (e.g., SG90 or MG90S for light loads)
- Pan-tilt mechanical bracket / 3D-printed mount
- Adequate power supply for servos (separate from camera if needed)
- Optional: external antenna, better power regulation

---

## Technologies

- C/C++ (Arduino framework)
- ESP32 camera driver
- Servo library / PWM control
- Wi-Fi and optional web server or WebSocket for remote commands

---

## Repository Structure

```
├── README.md
└── esp32cam with servo/     # Firmware and related files
```

---

## Getting Started

1. Assemble the pan-tilt mechanics and mount the ESP32-CAM securely.
2. Connect servo signal wires to available GPIOs on the ESP32-CAM (avoid pins used by the camera).
3. Provide a stable power source for the servos (common issue is brown-outs when servos draw current).
4. Open the sketch in the `esp32cam with servo` folder, configure Wi-Fi and pin assignments.
5. Upload the firmware and test movement commands while monitoring the serial output.

> **Tip:** Use a separate 5V supply for the servos and share only GND with the ESP32 to improve stability.

---

## Typical Use Cases

- Remote surveillance camera with adjustable view
- Robotics vision head
- Interactive or demo camera systems
- Integration with the other ESP32-CAM streaming projects in this account

---

## Future Improvements

- Web-based joystick or slider interface for pan/tilt
- Preset positions and smooth motion profiles
- Limits and calibration for mechanical range
- Combination with object tracking (move camera to follow a target)

---

## Author

**Houssem Eddine Sfaxi**  
Embedded Systems & IoT Engineer  
[GitHub](https://github.com/Sfaxihoussem2) · [Portfolio](https://sfaxihoussem2.github.io/My-portfolio/) · [LinkedIn](https://www.linkedin.com/in/houssem-sfaxi-3272a9280)

---

## License

Portfolio and educational project.
