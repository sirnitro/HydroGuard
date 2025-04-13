# 🌱 Hydroponics Monitoring & Maintenance System

A smart, Wi-Fi-enabled hydroponics automation system built with the Arduino Uno R4 WiFi. It monitors key environmental factors and automates nutrient and pH management to maintain optimal conditions for plant growth.

---

## 📡 Features

- Real-time monitoring of:
  - 🌡 Air temperature and humidity (DHT11)
  - 🌊 Water temperature
  - 📏 Reservoir water level
  - 🧪 Nutrient concentration (Turbidity sensor)
  - 🧬 pH level
- Automatic relay-controlled pumps for:
  - Nutrient dosing
  - pH Up & Down adjustment
  - Water refilling
  - Circulation watering
- Web interface with:
  - Live sensor data
  - Manual relay override
  - Configurable threshold controls
  - EEPROM-based settings persistence

---

## 🧰 Hardware Used

- **Arduino Uno R4 WiFi**
- **DHT11 Sensor** – External temperature & humidity
- **DS18B20 or analog temp sensor** – Water temperature
- **Water Level Sensor** – Reservoir monitoring
- **Turbidity Sensor** – Nutrient level
- **pH Sensor** – Acidity monitoring
- **Relay Module (5-Channel)** – Pump control

---

## 🌐 Web Interface

Hosted on the Uno R4's internal web server, the dashboard provides:

- Sensor value display
- Config threshold inputs
- Manual pump control buttons
- Mobile-responsive layout
- JSON-based state exchange for AJAX polling

---

## 🛠 Setup & Usage

1. Clone this repo to your local machine.
2. Open the `.ino` file in the Arduino IDE.
3. Connect and configure the hardware as per the wiring diagram (see `/docs`).
4. Upload the sketch to your Uno R4 WiFi.
5. Access the web interface using the device's IP address on your local network.
6. Calibrate pH and turbidity sensors as needed (instructions in `/docs`).

---

## 🗂 Project Structure

