**Cloud-Integrated Vehicle Speed Detection System Using IR Sensors** 

---

# Cloud-Integrated Vehicle Speed Detection System Using IR Sensors

An IoT-based system designed to measure vehicle speed using IR sensors and send real-time data to the cloud for monitoring and analysis. This system helps in detecting over-speeding and enables smart traffic management.

---

## 🚀 Features

* 📡 Real-time vehicle speed detection using IR sensors
* ☁️ Cloud integration for data storage and monitoring
* ⚡ Instant speed calculation based on sensor timing
* 🚨 Over-speed detection alerts
* 📊 Data visualization on dashboard 
* 🔌 Microcontroller-based system (ESP32/Arduino)

---

## 🛠️ Tech Stack

### Hardware

* ESP32 / Arduino
* IR Sensors (2 modules)
* Jumper wires, Breadboard
* Power Supply

### Software

* Embedded C / Arduino IDE
* Node.js 
* React.js

### Cloud

* MongoDB 

### Communication

* Wi-Fi (ESP32)
---

## ⚙️ Working Principle

1. Two IR sensors are placed at a fixed distance on the road.
2. When a vehicle passes:

   * First sensor detects → timer starts
   * Second sensor detects → timer stops
3. Speed is calculated using:

```id="speedcalc1"
Speed = Distance / Time
```

4. The calculated speed is:

   * Displayed locally (optional LCD/Serial Monitor)
   * Sent to cloud database via ESP32 Wi-Fi module

---
## ⚙️ Installation & Setup

### 1️⃣ Hardware Setup

* Connect IR sensors to ESP32/Arduino
* Place sensors at a known distance (e.g., 10 cm or 1 meter)
* Ensure proper alignment for accurate detection

---

### 3️⃣ Configure Wi-Fi & Cloud

Update credentials in your code:

```cpp id="wifi1"
const char* ssid = "YOUR_WIFI_NAME";
const char* password = "YOUR_WIFI_PASSWORD";
---

### 4️⃣ Run the System

* Power ON the microcontroller
* Open Serial Monitor
* Observe speed values
* Check cloud dashboard for real-time updates

---

## 📊 Output

* Vehicle speed displayed in **km/h or m/s**
* Over-speed alerts triggered when limit exceeded
* Data stored in cloud for analysis

---

## ⚠️ Limitations

* Accuracy depends on sensor placement
* Environmental factors (dust, light interference)
* Limited range of IR sensors

