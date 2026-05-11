<div align="center">

# SIMTER (Legacy Project)
### Real-Time Asset Monitoring System

Legacy embedded IoT project developed and presented during **PROJETE 2024 — Project Exhibition of ETE FMC**.

<img src="https://img.shields.io/github/repo-size/freitasj1/projetoSIMTER?style=for-the-badge"/>

<img src="https://img.shields.io/github/languages/count/freitasj1/projetoSIMTER?style=for-the-badge"/>

<img src="https://img.shields.io/github/commit-activity/y/freitasj1/projetoSIMTER?style=for-the-badge"/>

<img src="https://img.shields.io/github/last-commit/freitasj1/projetoSIMTER?style=for-the-badge"/>

</div>

---

# Overview

SIMTER (Real-Time Equipment Monitoring System) is an embedded IoT platform designed for real-time tracking and monitoring of physical assets in industrial and enterprise environments.

The project was developed by **Team 3105** and presented during **PROJETE 2024** at **ETE FMC (Escola Técnica de Eletrônica Francisco Moreira da Costa)**.

The system combines:

- BLE-based asset beacons
- ESP32 embedded devices
- Wi-Fi gateways
- Backend infrastructure
- Web management platform
- Inventory and monitoring tools

SIMTER was designed to help companies improve asset management, inventory automation, and equipment security through low-power wireless monitoring.

---

# Main Features

- Real-time asset presence monitoring
- BLE-based beacon communication
- Detection latency of approximately 5 seconds
- Custom encrypted payload communication
- Low-power operation using deep sleep
- Web platform for asset management and reports
- Integrated hardware and software ecosystem
- Expandable architecture for future indoor positioning systems

---

# System Architecture

The platform is divided into four main components:

## BLE Beacons

ESP32-based battery-powered devices responsible for periodically broadcasting encrypted BLE packets containing asset identification data.

### Features

- BLE advertising
- Deep sleep optimization
- Long battery life
- Low-cost deployment

---

## Gateways

ESP32-based gateway devices responsible for scanning nearby BLE packets and forwarding collected data to the backend server via HTTP requests over Wi-Fi.

### Features

- BLE scanning
- Wi-Fi connectivity
- HTTP communication
- Real-time forwarding

---

## Backend Server

Centralized infrastructure responsible for:

- Data processing
- Asset registration
- Event storage
- Presence validation
- Inventory management

---

## Web Platform

Web-based management interface used for:

- Asset monitoring
- Inventory reports
- Equipment tracking
- System administration

---

# Technologies Used

- ESP32
- Bluetooth Low Energy (BLE)
- Wi-Fi communication
- HTTP requests
- Embedded C/C++
- Backend development
- Frontend web development
- Database integration
- RFID experimentation
- Low-power embedded systems

---

# Power Optimization

One of the main goals of the project was achieving long-term battery operation for the BLE beacons.

## Beacon Power Cycle

- Transmission current: approximately 8 mA for 0.18 seconds
- Deep sleep current: approximately 80 µA for 4 seconds

With this operating cycle, the estimated battery life reached approximately:

- Up to 6 months using a 4000 mAh 18650 battery

---

# Project Gallery

## Hardware and Prototype

<div style="display: flex; justify-content: space-between;">
    <img src="https://github.com/freitasj1/projetoSIMTER/blob/main/img/20241004_110745.jpg" alt="Prototype 1" width="33%">
    <img src="https://github.com/freitasj1/projetoSIMTER/blob/main/img/20241004_110749.jpg" alt="Prototype 2" width="33%">
    <img src="https://github.com/freitasj1/projetoSIMTER/blob/main/img/DSC_0350.jpg" alt="Prototype 3" width="33%">
</div>

---

# Advantages

- Low-power wireless monitoring
- Automated inventory processes
- Reduced manual asset verification
- Indoor operation capability
- Scalable architecture
- Expandable BLE infrastructure
- Cost-effective deployment

---

# Prototype Hardware

Example prototype configuration:

- 5× ESP32 devices
- 5× 18650 batteries (4000 mAh)
- RC522 RFID module
- RFID tags for testing and experiments

---

# Repository Structure

This repository preserves several parts of the original project, including:

- Embedded firmware
- Gateway implementation
- Backend services
- Frontend platform
- Database integration
- Hardware references
- Experimental features
- Development materials

> Some sections remain organized according to the original educational development workflow.

---

# FAQ

## Does the system require internet access?

No.  
The system only requires a local network/router for communication between gateways and the backend server.

---

## Does the system provide real-time positioning?

Currently, the platform identifies asset presence within a monitored area.

Indoor triangulation and position estimation were considered as possible future improvements.

---

## Why use BLE instead of GPS?

BLE offers several advantages for indoor industrial monitoring:

- Much lower power consumption
- Better indoor operation
- Lower infrastructure cost
- Longer battery life
- Simpler deployment

---

## Can the system track people?

No.  
The project was designed exclusively for asset and equipment monitoring.

---

# Lessons Learned

SIMTER represented an important multidisciplinary engineering experience involving:

- Embedded systems development
- BLE communication systems
- ESP32 firmware development
- Backend/frontend integration
- Database systems
- IoT architecture
- Low-power optimization
- Wireless communication
- Hardware/software integration

The project also contributed to practical experience with collaborative engineering workflows and real-world system integration challenges.

---

# Contributors

| Name | Responsibilities |
|---|---|
| Enzo | Gateway Development and Backend |
| João Pedro | Backend, Frontend and Database |
| Mateus | Beacon and Gateway Development |
| Murilo | Cryptography and RFID Integration |

---

# License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

# Legacy Project Notice

This repository is maintained primarily for historical and educational purposes.

SIMTER represents an early-stage embedded IoT and wireless monitoring system developed during technical high school education.  
Although the project architecture and implementation reflect its educational context, the repository remains an important milestone involving:

- BLE systems
- ESP32 development
- IoT infrastructure
- Embedded networking
- Low-power firmware design
- Backend/frontend integration
- Real-time monitoring systems
- Hardware/software co-design
