# 🤖 Autonomous Human & Object Following Robot

An **autonomous robot** capable of **real-time object and human tracking**, built using the **Arduino Nicla Vision** platform.  
The system leverages on-board computer vision, sensor fusion, and wireless communication to follow targets intelligently while monitoring its position through odometry.

---

![Arduino](https://img.shields.io/badge/Arduino-Nicla_Vision-00979D?logo=arduino&logoColor=white)
![Python](https://img.shields.io/badge/Python-3.x-3776AB?logo=python&logoColor=white)
![TinyML](https://img.shields.io/badge/TinyML-FOMO-orange)
![YOLOv11](https://img.shields.io/badge/YOLO-v11-yellow)
![WiFi](https://img.shields.io/badge/WiFi-Enabled-blue)
![License](https://img.shields.io/badge/License-MIT-green)

---

## 🚀 Features

- **🧠 Real-Time Vision Processing**  
  Implemented object and human tracking on the **Arduino Nicla Vision** using its onboard **RGB camera** and **ToF (Time-of-Flight) sensor**.

- **🎯 Tracking Algorithms**  
  Designed a control system that determines robot movement based on **bounding box coordinates** and **ToF distance measurements**.

- **🤖 Machine Learning Integration**  
  Transitioned from traditional **color-based blob detection** to **TinyML-based recognition** using a **custom-trained FOMO model** for **human face detection**.

- **🌐 Server-Side YOLOv11 Processing**  
  Experimented with **YOLOv11** for server-side face detection and comparison with embedded ML results.

- **🦾 Motion & Control**  
  Developed a **differential drive system** incorporating **odometry** for accurate position tracking and **real-time data visualization**.

- **📡 Wireless Communication**  
  Established **WiFi communication** between the Nicla Vision and the Arduino for coordinated control and data exchange.

---


---

## ⚙️ How It Works

1. **Detection** — The Nicla Vision captures frames via its RGB camera and processes them using a **FOMO TinyML model** for face/object recognition.  
2. **Distance Measurement** — The ToF sensor measures depth to determine proximity to the target.  
3. **Decision Making** — The bounding box position and ToF data are sent to the Arduino via WiFi.  
4. **Motion Control** — The Arduino computes control signals for the **differential drive motors** to follow the target.  
5. **Feedback** — Odometry and sensor data are visualized in real-time for debugging and analysis.

---

## 🧰 Hardware Used

- 🟦 **Arduino Nicla Vision** (RGB Camera + ToF Sensor)  
- ⚙️ **Arduino Board** (for motion control & sensor integration)  
- 🛞 **Differential Drive Motors** with encoders  
- 🔋 **Battery / Power Module**  
- 📡 **WiFi Communication Module (Nicla Vision WiFi - Adafruit WINC1500 WiFi shielf)**
- 🖵 **TFT display and LEDs to display robot status and different functions**

---

## 🧠 Software Stack

- **Arduino IDE / MicroPython (OpenMV IDE)**
- **YOLOv11 (Server-Side Testing)**
- **FOMO (TinyML Model)**
- **Edge Impulse / OpenCV (for training & evaluation)**
- **WiFi communication protocols (TCP/UDP)**
- **Python for integration & visualization**

---

## 🧪 Results

✅ Real-time face and object tracking  
✅ Smooth following behavior based on ToF distance  
✅ Reliable WiFi communication between Nicla Vision and Arduino  
✅ Successful migration from basic blob detection → advanced TinyML-based vision  

---



