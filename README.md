# 🌱 Smart Agriculture IoT System
----
## 📖 Overview
This project implements a **Precision Irrigation System** using **IoT + Weather API + MQTT**.  
It combines **soil sensors, weather forecasting, and automation** to optimize water usage.  

-----

The system has **two components**:
1. **ESP32 Node** – Collects **soil moisture, temperature, humidity** and controls pump locally.  
2. **Raspberry Pi Gateway** – Receives sensor data, fetches **real-time weather**, and makes smarter irrigation decisions.

-------------------------

## ⚙️ Features
- Soil moisture monitoring  
- DHT11 temperature & humidity sensing  
- MQTT communication between ESP32 & Raspberry Pi  
- Weather forecast integration (using [WeatherAPI](https://www.weatherapi.com/))  
- Smart irrigation decisions (avoids watering before rain 🌧)  
- Cloud-ready (can be extended to AWS IoT, Azure, ThingsBoard, etc.)  

## 🛠 Hardware Requirements
- **ESP32** (with MicroPython firmware)  
- **Soil moisture sensor** (analog)  
- **DHT11 sensor** (temp & humidity)  
- **Relay module + water pump**  
- **Raspberry Pi** (running Python 3)  

---

## 🧑‍💻 Software Requirements
- MicroPython on ESP32  
- Python 3 on Raspberry Pi  
- Install dependencies:
```bash
pip install paho-mqtt requests
