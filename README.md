# 🌊 AUV-HydroMap-6D

> **Low-Cost Autonomous Underwater Vehicle for 6D Hydrodynamic Current Mapping**  
> *Engineering Project — ISEN Méditerranée*

---

## 📌 Overview

**AUV-HydroMap-6D** is an open-source, low-cost (< €200) autonomous underwater vehicle designed to map water current vectors in 6 dimensions $(X, Y, Z, V, \theta, \phi)$ using embedded sensor fusion and drift compensation.

---

## 👥 Team

Mohamed Adel — Project Lead / Hardware & Embedded Firmware Engineer: PCB Design (KiCad 10.0) & Low-Level C/C++ (STM32)

Gaspar — Mechanical Engineer: 3D CAD & Submarine Integration

Bilel — Cloud & Mobile Software Engineer: Mobile App & Cloud Infrastructure

---

## 🛠️ Tech Stack

* **Embedded Systems:** STM32 (CLion / STM32Cube) & ESP32 (MicroPython / Thonny)
* **Hardware:** KiCad 10.0
* **Mechanical CAD:** 3D Modeling (STEP / STL)
* **Software:** Mobile App & Cloud Infrastructure

---

## 📊 6D Vector Matrix

| Variable | Description | Source / Sensor |
| :--- | :--- | :--- |
| **X, Y** | Horizontal position | Surface GPS + Tether link |
| **Z** | Depth | MS5837 pressure sensor |
| **V** | Flow velocity | Flowmeter / Dynamic pressure |
| **$\theta$** | Heading angle | 9-axis IMU |
| **$\phi$** | Vertical angle | IMU + Differential pressure |

---

## 📁 Repository Structure

```text
.
├── cad/            # 3D CAD Models & Enclosures (STEP, STL)
├── docs/           # System Architecture & Specs
├── hardware/       # PCB Schematics & Layout (KiCad 10.0)
├── src/            # Firmware & Software Codebase
│   ├── stm32/      # Low-Level C/C++ Firmware (CLion + STM32Cube)
│   ├── esp32/      # Telemetry Firmware (MicroPython / Thonny)
│   └── mobile/     # Mobile App Codebase
└── README.md       # Project Documentation
