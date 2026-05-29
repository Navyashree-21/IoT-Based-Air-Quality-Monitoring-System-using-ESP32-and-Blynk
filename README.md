# IoT-Based Air Quality Monitoring System using ESP32 and Blynk

## 📌 Project Overview

This project presents a real-time IoT-based Air Quality Monitoring System developed using ESP32, MQ135 Gas Sensor, DHT11 Temperature & Humidity Sensor, 16×2 I2C LCD, and the Blynk IoT platform.

The system continuously monitors environmental conditions and transmits sensor data to the Blynk cloud via Wi-Fi, enabling users to remotely monitor air quality, temperature, and humidity through a mobile application.

---

## 🚀 Features

- Real-time air quality monitoring
- Temperature and humidity measurement
- Wi-Fi-enabled cloud connectivity
- Remote monitoring using Blynk mobile application
- Local display using 16×2 I2C LCD
- Air quality classification (Good / Moderate / Poor)
- Non-blocking timer-based scheduling
- Low-cost and scalable IoT solution

---

## 🛠 Hardware Components

| Component | Quantity |
|------------|------------|
| ESP32 Development Board | 1 |
| MQ135 Gas Sensor | 1 |
| DHT11 Sensor | 1 |
| 16×2 I2C LCD | 1 |
| Breadboard | 1 |
| Jumper Wires | As Required |
| USB Cable | 1 |

---

## 💻 Software Requirements

- Arduino IDE
- ESP32 Board Package
- Blynk IoT Platform
- WiFi Library
- Blynk Library
- DHT Sensor Library
- hd44780 LCD Library

---

## 🏗 System Architecture

```text
MQ135 + DHT11
       ↓
     ESP32
       ↓
      Wi-Fi
       ↓
   Blynk Cloud
       ↓
 Mobile Application

       +
    I2C LCD
```

---

## ⚙ Working Principle

1. ESP32 initializes all connected sensors and peripherals.
2. MQ135 sensor measures air quality based on gas concentration.
3. DHT11 sensor measures temperature and humidity.
4. ESP32 processes the collected sensor data.
5. Data is transmitted to the Blynk cloud through Wi-Fi.
6. Blynk dashboard displays real-time values.
7. LCD displays sensor readings locally.
8. Air quality is classified as Good, Moderate, or Poor based on threshold values.
9. The process repeats continuously for real-time monitoring.

---

## 🔌 Pin Connections

### DHT11 Sensor

| DHT11 Pin | ESP32 Pin |
|------------|------------|
| VCC | 3.3V |
| GND | GND |
| DATA | GPIO4 |

### MQ135 Sensor

| MQ135 Pin | ESP32 Pin |
|------------|------------|
| VCC | 5V |
| GND | GND |
| AO | GPIO34 |

### I2C LCD

| LCD Pin | ESP32 Pin |
|------------|------------|
| VCC | 5V |
| GND | GND |
| SDA | GPIO21 |
| SCL | GPIO22 |

---

## 🌫 Air Quality Classification

| MQ135 ADC Value | Status |
|-----------------|---------|
| < 800 | Good |
| 800 – 1800 | Moderate |
| > 1800 | Poor |

> Note: These threshold values are experimentally selected and represent relative air quality estimation rather than exact gas concentration (PPM).

---

## 📊 Results

- Successfully monitored air quality, temperature, and humidity in real time.
- Displayed sensor values on both LCD and Blynk dashboard.
- Achieved reliable wireless communication using ESP32 Wi-Fi.
- Implemented cloud-based remote monitoring.
- Demonstrated threshold-based air quality indication.

---

## 📚 Concepts Used

- Internet of Things (IoT)
- Embedded Systems
- Sensor Interfacing
- ADC (Analog-to-Digital Conversion)
- I2C Communication Protocol
- Cloud Computing
- Wi-Fi Communication
- Real-Time Monitoring
- Non-Blocking Programming

---

## 🔮 Future Enhancements

- PM2.5 and PM10 dust monitoring
- GPS-based location tracking
- Data logging and cloud database integration
- Machine learning-based pollution prediction
- Solar-powered deployment
- Smart city-scale monitoring network

---

## 📸 Project Images

Add the following images inside the `images/` folder:

- Hardware Setup
- Block Diagram
- Flowchart
- Blynk Dashboard
- LCD Output

---

## 📂 Project Structure

```text
IoT-Air-Quality-Monitoring-System-ESP32
│
├── README.md
├── src
│   └── air_quality_monitoring.ino
│
├── images
│   ├── block_diagram.png
│   ├── flowchart.png
│   ├── hardware_setup.jpg
│   ├── lcd_output.jpg
│   └── blynk_dashboard.jpg
│
├── docs
│   └── Project_Report.pdf
│
└── LICENSE
```

---

## 👩‍💻 Author

**Navyashree S J**

Electronics and Communication Engineering (ECE)

Interested in Embedded Systems, IoT, VLSI Design, and Digital Design.

---
