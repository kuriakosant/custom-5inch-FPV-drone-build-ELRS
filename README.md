# 🛸 5" FPV Freestyle Build (DJI O4 Lite + ELRS)

My first custom 5-inch FPV freestyle drone.

> [!WARNING]
> **🚧 Work In Progress**
> This repository is currently a work in progress. Most files are missing while I collect everything (product lists, schematics, wiring diagrams, etc.). Once I gather all the necessary materials, I will upload them here.

This repository will contain the full parts list, wiring schematics, and Betaflight configuration files for reproducibility.

## 📊 Quick Specs
| Component | Part | Price | Link |
| :--- | :--- | :--- | :--- |
| **Frame** | | | |
| **FC/ESC Stack** | [e.g., SpeedyBee F405 V3 Stack] | | |
| **Motors** | | | |
| **Digital VTX** | DJI O4 Lite Air Unit | | |
| **Camera** | Flywoo Wide Angle Lens (O4) | | |
| **Receiver** | Happymodel EP2 (ELRS 2.4GHz) | | |
| **Battery** | 6S 1500–1850mAh | | |
| **Firmware** | Betaflight 4.5.x | | |

---

## ⚡ Wiring Diagram
> [!TIP]
> Always check your pinouts with a multimeter before plugging in the battery for the first time!

![Wiring Diagram](./media/wiring-diagram.png)

* **UART 1:** Serial RX (ELRS)
* **UART 2:** VTX MSP (Displayport)
* **UART 6:** GPS (if applicable)

---

## ⚙️ Software Configuration

### Betaflight CLI
I have included two types of configuration files in the `/config` folder:
1.  `diff_all.txt`: Only the changes from default (Recommended for most users).
2.  `dump.txt`: The full firmware state.

### PID & Filter Tuning
* **Master Multiplier:** 1.1
* **Filters:** [Explain if you use RPM filtering or presets]
* **Rates:** [e.g., Actual Rates: 600 deg/s Center, 0.10 Expo]

---

## 🛠️ Build Notes
* **Capacitor:** Used a 35V 1000uF Low ESR cap to minimize video noise.
* **TPU Parts:** Printed in 95A TPU. Files are located in the `/3D-Prints` folder.
* **Prop Direction:** Props-out configuration to keep the camera lens cleaner.
* **DJI O4:** Requires correct MSP setup for OSD. RockSteady OFF recommended for wide-angle lens (causes jitter otherwise).

## 🎥 Flight Footage
Check out the maiden flight here: [Link to YouTube/Instagram]

---

## 🤝 Support
If you have questions about this specific build or need help with the configuration, feel free to open an **Issue** or a **Discussion**!
