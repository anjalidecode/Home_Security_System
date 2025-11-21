# 🏠 HOME SECURITY SYSTEM USING ESP32-CAM & TELEGRAM ALERTS

A smart Home Security System built using ESP32-CAM, capable of detecting:

- Intruder Motion
- Door Open Events
- Fire / Flame
- Smoke & Gas Leaks
- Captures Intruder Photo
- Sends Alerts to Telegram with Images

This project uses Telegram Bot API for instant alerts from anywhere.

## ⭐ FEATURES

- Arm/Disarm system using Telegram Bot
- Intruder detection using PIR sensor
- Door monitoring using Magnetic Reed Switch
- Gas/Smoke Leak detection (MQ sensors)
- Fire/Flame detection
- ESP32-CAM captures intruder images
- Instant Telegram alerts (messages + photos)
- Authorized Chat ID access control
- Works on WiFi, battery-friendly
- Fully open-source (CC BY-NC-SA 4.0)


## 🔧 HARDWARE COMPONENTS

- ESP32-CAM (AI Thinker)
- FTDI Programmer
- AM312 Mini PIR Sensor
- Reed Switch Door Sensor
- MQ-6 Gas/Smoke Sensor
- Flame Sensor Module
- 10kΩ Resistors (2x)
- Logic Level Shifter
- Breadboard + MB102 Power Supply
- Jumper Wires
- LiPo Battery / Power Bank


## 💻 SOFTWARE USED

- Arduino IDE
- ESP32 Board Manager
- Universal Telegram Bot Library
- ArduinoJson Library
- Telegram App
- (Optional) VS Code + PlatformIO

## 🚀 HOW IT WORKS

1. Sensors connect to ESP32-CAM.
2. ESP32-CAM connects to your WiFi network.
3. A Telegram Bot is created using BotFather.
4. ESP32 sends alerts via Bot API.
5. On detection:
   - Motion → Intruder Image Sent
   - Door Open → Alert Sent
   - Fire/Smoke/Gas → Warning Sent
6. System can be armed/disarmed using Telegram commands.
7. Only registered Chat IDs can use the bot.

## 🤖 SETTING UP TELEGRAM BOT

1️⃣ Create Bot  
Open Telegram → Search “BotFather”  
Command:
    /newbot
Receive your BOT TOKEN.

2️⃣ Get Chat ID  
Search “@myidbot”  
Command:
    /getid

3️⃣ Add to your ESP32 Code:
    String BOTtoken = "YOUR_BOT_TOKEN";
    String CHAT_ID = "YOUR_CHAT_ID";

⚠ DO NOT upload real tokens or WiFi passwords to GitHub.

## 📚 REQUIRED LIBRARIES

Install through Arduino Library Manager:

- ArduinoJson
- Universal Telegram Bot Library
- WiFiClientSecure

### Make your home smarter, safer, and always protected. 🛡️🏡
