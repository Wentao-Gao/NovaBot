
# 🚗 Pololu 3pi+ Starter Project

This repository provides a minimal yet complete example for getting started with the [Pololu 3pi+ 32U4 Robot](https://www.pololu.com/product/3575), using `arduino-cli` and VSCode on macOS (or other platforms). It includes basic functionality like button-controlled motor movement, OLED output, LED indicators, and buzzer sounds.

---

## 📦 Project Features

- ✅ Button A to start the robot
- ✅ Buzzer plays startup sound
- ✅ Yellow LED indicator when active
- ✅ Motors: forward and backward loop
- ✅ OLED displays status

---

## 🧰 Requirements

- [Arduino CLI](https://arduino.github.io/arduino-cli/)
- [VSCode](https://code.visualstudio.com/)
- [Pololu A-Star Board Package](https://github.com/pololu/a-star)
- USB connection to Pololu 3pi+ 32U4
- Arduino libraries:
  - `Pololu3piPlus32U4`

---

## 📂 Project Structure

```

3pi\_base/
├── 3pi\_base.ino            # Main Arduino sketch
└── .vscode/
└── arduino.json        # Board and port configuration

````

---

## 🚀 Quick Start

### 1. Clone this repository
```bash
git clone https://github.com/your-username/3pi_base.git
cd 3pi_base
````

### 2. Install board core

```bash
arduino-cli config add board_manager.additional_urls https://files.pololu.com/arduino/package_pololu_index.json
arduino-cli core update-index
arduino-cli core install pololu-a-star:avr
```

### 3. Install required libraries

```bash
arduino-cli lib install Pololu3piPlus32U4
```

### 4. Compile and upload

```bash
arduino-cli compile --fqbn pololu-a-star:avr:a-star32U4 .
arduino-cli upload -p /dev/cu.usbmodem1101 --fqbn pololu-a-star:avr:a-star32U4 .
```

### 5. (Optional) Open serial monitor

```bash
arduino-cli monitor -p /dev/cu.usbmodem1101
```

---

## 🧠 Functional Overview

```cpp
buttonA.waitForPress();     // Waits for user to press Button A
buzzer.play(...);           // Plays startup melody
ledYellow(1);               // Turns on yellow LED
motors.setSpeeds(...);      // Controls both wheels
display.print(...);         // Shows text on OLED screen
```

---

## 📈 Suggested Next Steps

* Add line sensor reading and follow black line
* Implement serial commands for remote control
* Add obstacle avoidance using IR sensors
* Use OLED screen for sensor debug info
* Sync with ESP32 or Raspberry Pi over UART

---

## 📜 License

MIT License

---

## 🙌 Acknowledgments

* [Pololu Robotics](https://www.pololu.com/)
* [Arduino CLI](https://arduino.github.io/arduino-cli/)

````



