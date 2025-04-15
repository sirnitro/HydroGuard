# 🌿 Uno R4 Wi-Fi Hydroponics System — Pinout Map

This pinout map outlines the hardware configuration for the Uno R4 Wi-Fi-based hydroponics monitoring and control system. It includes sensors, relays, display, SD card logging, and optional components.

---

## 🔌 Power Distribution

| **Component**     | **Power Pin** | **Notes**                            |
|------------------|---------------|--------------------------------------|
| All Sensors      | VCC → 5V      | Verify individual sensor voltage     |
| All Components   | GND → GND     | Common ground reference              |
| SD Card Module   | VCC → 3.3V or 5V | Check module specs (many regulate internally) |

---

## 🧠 Microcontroller: Uno R4 Wi-Fi

### 📥 Inputs

| **Component**           | **Pin** | **Type**     | **Notes**                                   |
|------------------------|---------|--------------|---------------------------------------------|
| DHT22 (Air Temp/Humidity) | D2    | Digital In   | Requires 10k pull-up to VCC                 |
| DS18B20 (Water Temp)    | D3      | Digital In   | 4.7k pull-up to VCC (1-Wire)                |
| Water Level Sensor      | A0      | Analog In    | Resistive/capacitive type                   |
| Turbidity Sensor        | A1      | Analog In    |                                             |
| pH Sensor               | A2      | Analog In    | Use signal conditioning                     |
| Button (Optional)       | D19 (A5)| Digital In   | Use `INPUT_PULLUP`                          |

---

### 📤 Outputs

| **Component**             | **Pin** | **Type**     | **Notes**                         |
|--------------------------|---------|--------------|-----------------------------------|
| Relay 1 – Nutrients      | D4      | Digital Out  | Active LOW                        |
| Relay 2 – pH Up          | D5      | Digital Out  | Active LOW                        |
| Relay 3 – pH Down        | D6      | Digital Out  | Active LOW                        |
| Relay 4 – Water Top-Off  | D7      | Digital Out  | Active LOW                        |
| Relay 5 – Circulation    | D8      | Digital Out  | Active LOW                        |
| Status LED (Optional)    | D9      | Digital Out  | Use 220Ω resistor inline          |

---

## 📟 I²C Bus (Display and Expansions)

| **Device**       | **SDA Pin** | **SCL Pin** | **Notes**             |
|------------------|-------------|-------------|------------------------|
| OLED Display      | D20         | D21         | 0x3C default address   |

---

## 💾 SPI Bus (SD Card)

| **Signal** | **Pin** | **Description**    |
|------------|---------|--------------------|
| CS         | D10     | Chip Select         |
| MOSI       | D11     | Master Out Slave In |
| MISO       | D12     | Master In Slave Out |
| SCK        | D13     | Clock               |

---

## 📌 Reserved / Expansion Ideas

- A3–A4: Extra analog inputs
- D14–D18: Free for additional relays or comms
- I2C: Connect EC, light, or CO₂ sensors
- UART: Debug output or external controller
