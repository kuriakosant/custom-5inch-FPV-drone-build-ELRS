# 🛸 SUKHOI: 5" Digital Freestyle Build
### DJI O4 Lite + ELRS + GPS Rescue 

The **SUKHOI** is a custom-engineered 5-inch FPV drone optimized for high-fidelity digital video and reliable long-range freestyle. Built on the **PhiSital Mark5 DC** frame, it features a full **DJI O4 Lite** stack with custom CNC cooling and a wide-angle lens for cinematic performance.

> [!NOTE]
> This repository serves as a full hardware manifest, wiring guide, and Betaflight configuration log for the SUKHOI project.

---

## 📊 Technical Specifications

### Core Components
| Component | Part | Note |
| :--- | :--- | :--- |
| **Frame** | PhiSital Mark5 DC O4 Pro | 5" Carbon Fiber / DeadCat Geometry |
| **FC & ESC Stack** | SpeedyBee F405 V4 55A/60A | 30x30 Stack / Bluetooth Config |
| **Motors** | iFlight XING E Pro 2207 | 1800KV (6S Optimized) |
| **VTX** | DJI O4 Lite Air Unit | CNC Housing + 13cm Extender |
| **Camera Lens** | Flywoo Wide Angle (O4) | Enhanced FOV for freestyle |
| **Receiver** | HappyModel EP1 RX | 2.4GHz ExpressLRS |
| **GPS Module** | BN-880 GNSS | Dual GPS/GLONASS + Built-in Flash |
| **Buzzer** | VIFLY Finder 2 V2 | Self-powered tracker (Lost Model Alarm) |
| **Props** | HQprop Ethix S5 | 5040 3-Blade |

### Power System
* **Primary Batteries:** GNB 6S 1850mAh (120C/240C) for long flight times.
* **Agility Batteries:** GNB 6S 1500mAh (120C/240C) for freestyle sessions.
* **Capacitor:** 35V 1000uF Low ESR (Required for clean DJI O4 power).

---

## ⚡ Ground Station & Support Gear
* **Radio:** Jumper T15 ELRS (Internal 2.4G)
* **Radio Power:** Samsung INR21700 40T (4000mAh)
* **Charger:** ToolkitRC M7 200W DC + ADP100 Adapter
* **Field Charging:** XT30 to XT60 Adapters for cross-platform compatibility.

---

## ⚙️ Software & Telemetry

### Betaflight 4.5.x Configuration
* **UART 1:** Serial RX (ELRS)
* **UART 2:** VTX MSP (Displayport for DJI OSD)
* **UART 3:** VIFLY Finder Control
* **UART 6:** GPS (BN-880 @ 57600 baud)

### PID & Filter Tuning
* **Gyro/PID Loop:** 8kHz / 4kHz
* **DSHOT:** DShot600 (Bidirectional enabled)
* **GPS Rescue:** Configured for 50m minimum altitude and "Sanity Check" enabled.

---

## 🛠️ Build & Maintenance Notes
* **Thermal Management:** The DJI O4 Lite uses an **Axisflying CNC housing** to dissipate heat during high-wattage transmission.
* **Antenna Array:** * 1x Black Bear 5.8G Lollipop (LHCP) 155mm
    * 1x Black Bear 5.8G Lollipop (LHCP) 115mm
* **Lens Care:** RockSteady is set to **OFF** in-goggle to prevent the "jitter" effect common with aftermarket wide-angle lenses.
* **Safety:** VIFLY Finder 2 ensures recovery even if the main battery is ejected during a crash.

---

## 📂 Repository Contents
* `/config`: `diff_all.txt` and `dump.txt` for Betaflight 4.5.
* `/3D-Prints`: TPU mounts for the BN-880 GPS and Immortal-T antenna.
* `/media`: Wiring diagrams and high-res build photos.

---

## 🤝 Support
Open an **Issue** if you have questions about the SUKHOI component compatibility or Betaflight CLI settings.