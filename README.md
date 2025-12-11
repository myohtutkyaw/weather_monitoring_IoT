🌤️ IoT Weather Monitoring System with ESP32
Microcontroller Project

📌 Project Overview

This project implements a smart IoT-based weather monitoring system that measures:

Temperature

Humidity

Atmospheric Pressure

Using an ESP32, DHT21 (AM2301A), BMP280, and the Blynk IoT platform, the system sends real-time sensor data to the cloud, where users can visualize live and historical readings from both mobile and web dashboards.
(Page 1–2) 

Weather_Monitoring

🎯 Objectives

(Page 2) 

Weather_Monitoring

Build an IoT system that tracks environmental temperature, humidity, and pressure in real time.

Allow remote access and monitoring through Blynk App and Blynk Web Dashboard.

Enable historical data logging and alert notifications.

🔧 Components Used

(Page 3) 

Weather_Monitoring

ESP32 Dev Module

DHT21 / AM2301A – Humidity & Temperature Sensor

BMP280 – Barometric Pressure Sensor

Blynk App + Blynk Web Console

Arduino IDE

🗂️ Required Firmware Data

To connect the ESP32 to Blynk Cloud, the firmware must include:
(Page 4) 

Weather_Monitoring

Template ID

Auth Token (device identifier)

Wi-Fi SSID & Password

Program logic to read sensors and send data

⚡ Circuit Prototyping

(Page 5) 

Weather_Monitoring

Connections
BMP280 → ESP32 (SPI communication)

SCK → GPIO 18

MISO → GPIO 19

MOSI → GPIO 23

CS → GPIO 5

DHT21 → ESP32 (Single-wire)

Signal → GPIO 25

The slide also includes a prototype image and example code snippet showing virtual pins V0, V1, V4 for sensor uploads.

🔄 System Data Flow

(Page 6) 

Weather_Monitoring

1. Data Collection
DHT21 and BMP280 measure temperature, humidity, and pressure.

2. Data Transmission
ESP32 sends sensor readings to Blynk Cloud over Wi-Fi.

3. Data Visualization
Blynk dashboards show live data + historical charts.

4. Alerts
Notifications triggered if temperature exceeds a threshold.

Pipeline:
sensor → ESP32 → Blynk Cloud → Dashboard

📊 Blynk Dashboard Overview

(Page 7) 

Weather_Monitoring

Datastreams

V0 – Temperature

V1 – Humidity

V4 – Pressure

Web Dashboard Widgets

Gauge (live values)

Chart (historical data)

Mobile App Widgets

Enhanced Gauge

Chart for trends over time

Slides include sample visuals for both mobile and web dashboards.

✅ Features Summary

Real-time monitoring

IoT cloud dashboard

Multi-device access (phone & PC)

Data history + chart visualization

Overheat alert notifications

Simple wiring & low-cost components
