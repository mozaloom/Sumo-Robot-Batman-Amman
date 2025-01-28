
# 🤖 Sumo Robot: Batman Amman

**National Sumo Robot Competition Champion**  
Autonomous combat robot engineered for strategic sumo matches through opponent detection and adaptive movement

<div align="center">
  <img src="https://raw.githubusercontent.com/mozaloom/Sumo-Robot-Batman-Amman/main/Prototype/IMG.PNG" alt="BatmanAmman Prototype" width="500"/>
</div>

<div align="center">
  [![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
  ![Arduino](https://img.shields.io/badge/Arduino-00979D?style=flat&logo=Arduino&logoColor=white)
  ![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
  ![OpenCV](https://img.shields.io/badge/OpenCV-27338e?style=flat&logo=OpenCV&logoColor=white)
</div>

## 🏆 Overview
**Team BatmanAmman** presents our championship-winning sumo robot, designed to autonomously detect opponents and execute strategic movements in competitive matches. Originally conceived with advanced computer vision, we successfully pivoted to a robust sensor-based system when faced with hardware challenges.

## 🌟 Key Features
- **Dual Control Systems**: Raspberry Pi + Arduino redundancy
- **Multi-Sensor Detection**: 6 IR + 4 QTR sensors
- **JSumo Titan Motors**: 200 RPM with rubber traction
- **Titanium Battle Scoop**: Bio-inspired impact design
- **Dual Battery System**: 3000mAh + 9V LiPo power

## 🔧 Hardware Architecture
```ascii
                         ┌───────────────┐
                         │  Raspberry Pi │
                         │  (Vision Hub) │
                         └───────┬───────┘
                                 │
┌──────────┐              ┌──────▼───────┐             ┌───────────┐
│  IR      ├──────────────►              │◄────────────┤ Motor     │
│ Sensors  │              │  Arduino Mega│             │ Controllers
└──────────┘              │              │             └───────────┘
                          └──────┬───────┘
                 ┌───────────────┴───────────────┐
                 │                               │
            ┌────┴─────┐                  ┌──────▼────┐
            │ QTR      │                  │ Power     │
            │ Sensors  │                  │ System    │
            └──────────┘                  └───────────┘
```

## 🔄 Development Journey

### Initial Design (Planned)
```python
# Vision-based strategy concept
from cv2 import YOLOv8

def main():
    while match_active:
        opponent = detect_opponent()
        if opponent:
            execute_attack(opponent.coordinates)
```
- **Components**:
  - Raspberry Pi 5 Model B
  - Coral TPU Accelerator
  - Wide-Angle Noir Camera
- **Features**:
  - Custom YOLOv8 model
  - Reinforcement learning integration
  - Real-time match analytics

### Final Implementation
```cpp
// Arduino battle-tested code
void loop() {
  readSensors();
  if (enemyDetected) {
    chargeAttack();
  } else {
    searchPattern();
  }
  avoidEdges();
}
```
- **Components**:
  - Arduino Mega 2560
  - 2× Dual H-Bridge Drivers
  - JS200XF IR Sensor Array
- **Features**:
  - 1ms response time
  - Contact-based tactics
  - Fail-safe edge detection

## 🛠️ Technical Specifications

| Component               | Specification                  |
|-------------------------|--------------------------------|
| Microcontroller         | Arduino Mega 2560             |
| Motors                  | JSumo Titan 200 RPM           |
| Wheels                  | Rubber Traction (120mm)       |
| Sensors                 | 6× IR, 4× QTR Reflectance     |
| Camera                  | Raspberry Pi Noir Wide-Angle  |
| Power                   | 3000mAh LiPo + 9V Backup      |
| Drivers                 | Dual H-Bridge x2              |

## ⚙️ Installation Guide

### Hardware Setup
1. **Mechanical Assembly**:
   - Mount motors with M4 bolts
   - Install titanium scoop using 3D-printed brackets
   - Secure sensors at 15° downward angles

2. **Electrical Connections**:
   ```plaintext
   Arduino Mega Pinout:
   - D2-D7: IR Sensors
   - A0-A3: QTR Sensors
   - PWM 9-12: Motor Drivers
   ```

3. **Power Management**:
   - Connect 3000mAh battery to motor drivers
   - Wire 9V battery to Arduino Vin

### Software Configuration
```bash
# For Arduino deployment
git clone https://github.com/mozaloom/Sumo-Robot-Batman-Amman
cd Arduino-Code
platformio run --target upload
```

## 🏅 Competition Performance
- **Match Record**: 12 Wins - 0 Losses
- **Fastest Victory**: 2.8 seconds
- **Sensor Accuracy**:
  - 98.4% opponent detection
  - 99.1% edge avoidance
- **Power Efficiency**: 57 minutes runtime

## 🚨 Challenges & Solutions
| Challenge               | Solution                      |
|-------------------------|-------------------------------|
| Coral TPU Delay         | Pivoted to IR sensor fusion   |
| Motor Synchronization   | Implemented PID feedback loop |
| Battery Drain           | Added power isolation circuit |
| Sensor Interference     | Shielded wiring harness       |

## 🔮 Future Roadmap
- Integrate delayed Coral TPU
- Develop machine learning strategies
- Implement wireless diagnostics
- Create modular sensor pods


---

<div align="center">
  <em>By Mohammed Zaloom</em>
</div>
```
