# 🔌 Electronics – Uno R4 Wi-Fi Hydroponics Controller

This directory contains all circuit-related documentation and design files for the custom hydroponics monitoring and control system. Powered by an **Arduino Uno R4 Wi-Fi**, this system integrates environmental sensors, pump automation, and real-time data logging.

---

## ⚙️ System Overview

The system monitors and controls:

- **Sensors**
  - DHT22 – Air Temperature & Humidity
  - DS18B20 – Water Temperature
  - Analog Water Level Sensor
  - Turbidity Sensor
  - Analog pH Sensor

- **Actuators**
  - 5 Relays controlling:
    - Nutrient Pump
    - pH Up Pump
    - pH Down Pump
    - Water Top-Off Pump
    - Circulation Pump

- **User Interface**
  - OLED Display (I²C)
  - Optional Buttons (Menu/Reset)
  - Status LEDs

- **Data Storage**
  - MicroSD Card (SPI) for sensor data logging

---

## 📌 Key Files

- `PINOUT.md` – Full GPIO mapping for all components
- `BOM.md` – Bill of Materials with part names, categories, quantities, and optional vendor links
- `schematic.fzz` – Fritzing schematic (breadboard view)
- `pcb_layout.fzz` – Optional PCB layout file
- `wiring_diagram.png` – Color-coded wiring diagram for physical setup

---

## 🧠 Expansion Possibilities

- EC (Electrical Conductivity) Sensor
- Light or CO₂ Sensors for environmental tuning
- RTC (Real-Time Clock) for scheduled dosing and time logs
- UART debug header or RS-485 communication port
- Neopixel or RGB status indicators
- Modular power and I²C headers for external expansions

---

## 📜 License

All design files in this directory are released under the [MIT License](../LICENSE). Free to use, remix, and improve for non-commercial and educational purposes.

---

## 📁 Folder Structure

