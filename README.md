# Robotic Dog PCB

Custom-designed double-layer PCB for a 4-legged robotic dog's controller board.

## 📌 Overview

This board hosts the microcontroller and provides all the connections needed to drive the robot dog's legs, power system, and an additional sensor.

## 🛠️ Specifications

- **Microcontroller:** Arduino Uno 
- **Layers:** Double layer (top + bottom copper)
- **Servo outputs:** 4x headers (GND / V+ / Signal), one per leg
- **Power input:** Battery connector
- **Sensor port:** 1x header for ultrasonic wave sensor

## 📂 Connector Reference

| Label | Function |
|---|---|
| SERVO_FL | Front-left servo (GND / V+ / Signal) |
| SERVO_FR | Front-right servo (GND / V+ / Signal) |
| SERVO_BL | Back-left servo (GND / V+ / Signal) |
| SERVO_BR | Back-right servo (GND / V+ / Signal) |
| BATT | Battery input |
| SENSOR |ultrasonic wave sensor connection |

## 📐 Design Notes

- Components arranged logically: power section separated from signal/logic section, MCU centered as the hub.
- All ports labeled on silkscreen for clarity.
- Bottom layer used as a ground plane/fill to simplify routing and reduce noise on servo signal lines.
- Power traces routed wider than signal traces to handle servo current draw.

## 📂 Repository Structure

```
robotic-dog-pcb/
├── design.png
└── README.md
```

## 👤 Author
V
