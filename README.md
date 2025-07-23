# DIY Voice Assistant with ESPHome

A DIY voice assistant built with **ESPHome** and **ESP32**, featuring **wake word detection**, **I2S microphone input**, and seamless **Home Assistant integration** for hands-free smart home control. This project turns an ESP32 into a fully functional voice interface, capable of controlling lights, scenes, and other devices in your smart home.

---

## ✨ Features

- **Wake word detection** (e.g., “Hey Jarvis”) using ESPHome pipelines.
- **Hands-free Home Assistant control** via local API.
- **I2S microphone** for high-quality voice capture.
- **Speaker output** via I2S DAC/amplifier for feedback.
- **DIY-friendly hardware** with minimal components.
- **OTA updates** and easy configuration through ESPHome.

---

## 🛠 Hardware Requirements

- **ESP32 development board** (e.g., ESP-WROOM-32 DevKit).
- **I2S Microphone** (e.g., INMP441).
- **I2S amplifier + speaker** (e.g., MAX98357A + 3W speaker).
- **Jumper wires** and breadboard (or custom PCB).
- **5V USB power source**.

---

## ⚡ Quick Start (Home Assistant)

### 1. **Install ESPHome Add-on**
- Open **Home Assistant > Settings > Add-ons**.
- Search for **ESPHome** and install it.

### 2. **Create a New Device**
- Go to the ESPHome dashboard (inside Home Assistant).  
- Click **“+ New Device”** and follow the wizard:  
  - Enter the device name (e.g., `voice_assistant`).  
  - Select **ESP32** as the platform.  
  - Enter your Wi-Fi credentials.
 
### 3. **Replace the Default Config**
- Open the newly created device config in the ESPHome editor.  
- Replace its contents with the `voice_assistant.yaml` from this repo.  
- Adjust pins if your hardware differs.

### 4. **Flash Your ESP32**
- Connect your ESP32 via USB to your Home Assistant server (or use OTA if previously flashed).  
- Click **“Install”** and follow the on-screen instructions.

---

## 🎨 Wiring Diagram
Check voice-assistant.png for pin connections.

---

## 🤝 Contributing
Pull requests and suggestions are welcome! Open an issue if you find a bug or want to propose a new feature.

---

### 📜 License
This project is licensed under the MIT License.
