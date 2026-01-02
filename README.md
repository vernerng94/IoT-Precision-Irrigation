# 🌱 IoT Precision Irrigation System

An ESP32-based smart irrigation system that monitors soil moisture, temperature, and humidity to automate watering for sustainable agriculture.

## 📋 Project Overview
- **Module:** PSB602IT Internet of Things
- **Student:** CU Index: 15999038 / 705W5GSG
- **Hardware:** ESP32, DHT22, Soil Moisture Sensor, Relay Module
- **Cloud:** ThingSpeak for data visualization and control
- **Threshold:** Automatic irrigation when soil moisture < 25%

## 🛠️ Hardware Components
1. ESP32 Development Board
2. DHT22 Temperature & Humidity Sensor
3. Capacitive Soil Moisture Sensor
4. 5V Relay Module
5. Water Pump/Solenoid Valve
6. Power Supply

## 🔧 Installation & Setup

### 1. Upload Code to ESP32
- Open `IoT_Irrigation.ino` in Arduino IDE
- Install required libraries:
  - WiFi
  - HTTPClient
  - DHT Sensor Library
- Update WiFi credentials and ThingSpeak API key
- Upload to ESP32

### 2. Hardware Connections
| ESP32 Pin | Component       |
|-----------|-----------------|
| GPIO 34   | Soil Moisture   |
| GPIO 4    | DHT22           |
| GPIO 23   | Relay Control   |
| 3.3V/5V   | Sensor Power    |
| GND       | Ground          |

### 3. ThingSpeak Setup
1. Create account at [thingspeak.com](https://thingspeak.com)
2. Create a new channel with 3 fields:
   - Field 1: Soil Moisture (%)
   - Field 2: Temperature (°C)
   - Field 3: Humidity (%)
3. Copy your Write API Key into the code

## 📊 Features
- Real-time soil moisture monitoring
- Automatic irrigation when moisture < 25%
- Temperature and humidity tracking
- Data logging to ThingSpeak
- Remote monitoring capability
- Serial console debugging

## 📁 Repository Structure
