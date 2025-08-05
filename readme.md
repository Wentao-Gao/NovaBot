
# 🌟 NovaBot

**NovaBot** is an evolving robotics platform that begins with low-level embedded control on the Pololu 3pi+ 32U4 and expands toward high-level AI capabilities—including voice, vision, and autonomous behavior—powered by Raspberry Pi and modern machine learning tools.

> From motion to cognition — this is a journey of growth, intelligence, and modular robotics.

---

## 🚀 Project Goals

- ✅ Start from Pololu 3pi+ embedded motion control
- ✅ Implement modular robot behaviors: LED, buzzer, motors, sensors
- ✅ Add UART communication between 3pi+ and Raspberry Pi
- ✅ Upgrade to high-level control using Python
- ✅ Extend to visual recognition, speech interaction, and path planning

---

## 📦 Current Feature Set (Stage 1: Embedded Control)

| Feature         | Description                          |
|----------------|--------------------------------------|
| Button Input    | Starts the robot with button A       |
| Motor Control   | Controls both wheels forward/backward|
| LED Feedback    | Yellow LED for status indication     |
| Buzzer Feedback | Plays simple startup melody          |
| OLED Display    | Shows current system status          |

---

## 🧰 Environment Setup

### Prerequisites

- ✅ [Arduino CLI](https://arduino.github.io/arduino-cli/)
- ✅ [VSCode](https://code.visualstudio.com/)
- ✅ [Pololu A-Star Board Package](https://github.com/pololu/a-star)
- ✅ [Pololu3piPlus32U4](https://github.com/pololu/3pi-plus-32u4-arduino-library)

### Arduino Core Installation

```bash
arduino-cli config add board_manager.additional_urls https://files.pololu.com/arduino/package_pololu_index.json
arduino-cli core update-index
arduino-cli core install pololu-a-star:avr
````

### Library Installation

```bash
arduino-cli lib install Pololu3piPlus32U4
```

---

## ⚙️ Project Structure

```
NovaBot/
├── NovaBot.ino               # Main Arduino sketch
└── .vscode/
    └── arduino.json          # Board/port configuration for VSCode
```

---

## 🔧 Build & Upload

### Compile

```bash
arduino-cli compile --fqbn pololu-a-star:avr:a-star32U4 .
```

### Upload

```bash
arduino-cli upload -p /dev/cu.usbmodem1101 --fqbn pololu-a-star:avr:a-star32U4 .
```

### Monitor Serial Output

```bash
arduino-cli monitor -p /dev/cu.usbmodem1101
```

---

## 🧠 Roadmap

| Stage      | Goal                                                      |
| ---------- | --------------------------------------------------------- |
| ✅ Stage 1  | Core embedded control (motors, sensors, buttons, display) |
| 🔄 Stage 2 | Communication interface to Raspberry Pi (UART/I2C)        |
| 🔜 Stage 3 | Raspberry Pi Python controller + Web dashboard            |
| 🔜 Stage 4 | Add speech recognition (e.g., Vosk / Whisper)             |
| 🔜 Stage 5 | Add camera + vision module (e.g., OpenCV or Edge YOLO)    |
| 🔜 Stage 6 | Autonomous navigation and AI decision-making              |

---

## 📸 Screenshots / Media (Optional)

> (Add photos/videos of your robot, OLED screen, terminal output, etc.)

---

## 💡 Inspiration

* The vision behind NovaBot is to explore how small robots can grow in intelligence—like a star going supernova—starting from basic motion to full-fledged autonomous reasoning and perception.

---

## 📜 License

MIT License

---

## 🙌 Credits

* Pololu Robotics — for amazing hardware
* Arduino CLI team — for headless development tooling
* You — for watching NovaBot grow ✨

```

---

## ✅ 提示

你可以将项目结构命名为：
```

NovaBot/
├── NovaBot.ino
├── README.md
└── .vscode/
└── arduino.json

