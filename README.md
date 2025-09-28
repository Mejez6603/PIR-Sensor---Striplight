# PIR-Sensor-&-Striplight

An Arduino-based automation project that uses a **PIR motion sensor** and a **5V LED strip light** to create a simple motion-activated lighting system.  
When motion is detected, the strip turns ON for **20 seconds** and then turns OFF if no motion is detected.  
The timer resets if continuous motion is detected.

---

## ✨ Features
- Automatic motion detection using PIR sensor  
- LED strip turns ON for 20 seconds after motion  
- Timer resets if new motion is detected  
- Configurable delay time (default: 20s)  
- Simple hardware setup (no relay or MOSFET required if strip is small)  
- Works with **active-low PIR modules**  

---

## 🛠 Technologies Used
- **Arduino Uno** (or compatible board)  
- **PIR Motion Sensor** (active-low type)  
- **5V LED strip light** (non-programmable)  
- **Arduino IDE** (for code upload)  
- **C++ (Arduino language)**  

---

## 🚀 Getting Started

### Prerequisites
- [Arduino IDE](https://www.arduino.cc/en/software) installed  
- Arduino Uno board + USB cable  
- PIR sensor and 5V LED strip  

### Installation
1. Clone this repository:  
   ```bash
   git clone https://github.com/yourusername/PIR-Sensor-Striplight.git
   cd PIR-Sensor-Striplight
2. Open `PIR_StripLight.ino` in Arduino IDE
3. Connect Arduino Uno via USB
4. Upload the sketch

---

## 💡 Usage

1. Power the Arduino board.
2. Wait for the PIR sensor to warm up (~30–60 seconds).
3. Walk in front of the PIR sensor.
4. The strip will turn ON for 20 seconds.
5. If more motion is detected, the timer resets.

---

## 📂 Project Structure

```
PIR-Sensor-&-Striplight/
│
├── PIR_StripLight.ino     # Main Arduino code
├── README.md              # Documentation
└── wiring.png             # Wiring diagram (optional, add later)
```

---

## 📦 Packaging for Distribution

* Source code is available in this repository.
* To share:

  * Provide the `.ino` file
  * Or zip the full project folder
  * Optionally include wiring diagram image for clarity

---

## 🔮 Future Enhancements

* Add **configurable delay time** via potentiometer
* Use a **relay or MOSFET** to handle higher-power LED strips
* Add **LDR sensor** to only trigger at night
* Implement **power-saving mode** with Arduino sleep functions
* Add a **buzzer or sound alert** when motion is detected

---

## 📝 Changelog

**v1.0.0 (Initial Release)**

* Basic PIR + LED strip integration
* Motion resets 20-second timer
* Active-low PIR support

---

## 💻 System Requirements

* Arduino Uno (or any 5V-compatible Arduino board)
* PIR sensor (active-low type)
* 5V non-programmable LED strip (max power depends on Arduino 5V pin capability)
* Arduino IDE (v1.8+ or Arduino IDE 2.0)

---

## 🛠 Troubleshooting

* **Light always ON:**
  Your PIR may be active-high. Invert the logic (`val == HIGH` instead of `val == LOW`).
* **Light never turns ON:**
  Check PIR warm-up time (30–60 seconds).
* **Random triggering:**
  Lower PIR sensitivity or shield from direct sunlight/heat sources.
* **Arduino resets when strip turns on:**
  Strip current draw may exceed Arduino’s 5V regulator. Use an external 5V supply with common ground.

---

## 🙏 Acknowledgements

* Arduino Community
* Open-source contributors for PIR tutorials
* Inspiration from basic IoT motion-light projects
* TINKERCAD
* Nooby
* Firelink
* SBBC PC
* Rita's PC
* To my dog and cat

---

## 📜 License

This project is licensed under the **MIT License** — free to use, modify, and distribute.
See [LICENSE](LICENSE) for details.

```

