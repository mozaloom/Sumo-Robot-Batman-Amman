# 🤖 Sumo Robot Batman

A championship-winning autonomous sumo robot featuring redundant systems and adaptive control strategies. Winner of the National Sumo Robot Competition in Jordan.

<div align="center">

[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
![Arduino](https://img.shields.io/badge/Arduino-00979D?style=flat&logo=Arduino&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-27338e?style=flat&logo=OpenCV&logoColor=white)

</div>

## 🌟 Features

- **Redundant Control Systems**: Multiple operation modes for reliability
- **Bio-inspired Design**: Custom titanium scoop inspired by ant mandibles
- **Computer Vision System**: Real-time opponent detection using YOLOv8
- **Battle Strategies**: Advanced movement and attack patterns
- **Sensor Fusion**: Integrated IR sensors and computer vision
- **Fail-safe Mechanisms**: Automatic fallback systems

## 💡 Operation Modes

### 1. Full System Mode (Primary)
- Raspberry Pi + Arduino + Computer Vision
- Full sensor fusion and advanced strategies
- Real-time opponent tracking with YOLOv8
- Maximum competitive advantage

### 2. Arduino + Basic Vision Mode
- Fallback if Raspberry Pi fails
- Arduino handles core control
- Basic USB camera for simplified vision
- Reduced but effective functionality

### 3. Pure Arduino Mode (Emergency)
- Ultimate fallback mode
- Relies on IR sensors and basic strategies
- Completely autonomous operation
- Battle-tested reliability

## 🏗️ Project Structure

```
sumo-robot-batman/
├── src/
│   ├── Arduino-Code/          # Standalone & fallback systems
│   │   ├── Attack.cpp/h       # Core attack strategies
│   │   ├── Edge.cpp/h         # Ring edge detection
│   │   ├── IR.cpp/h           # Sensor management
│   │   ├── Motor.cpp/h        # Direct motor control
│   │   ├── Search.cpp/h       # Basic search patterns
│   │   └── SumoMovement.cpp/h # Movement control
│   ├── Computer-Vision-Camera/ # Advanced vision system
│   │   ├── predict.py         # YOLOv8 processing
│   │   └── requirements.txt   # Dependencies
│   └── Python-Code/           # High-level control
│       ├── actuators_sensors.py # Hardware interface
│       ├── attack.py          # Strategic attacks
│       ├── main.py           # System orchestration
│       └── search.py         # Advanced search
└── Prototype/                # Design files
```

## 🔧 Requirements

### Hardware
- Arduino Mega 2560
- Raspberry Pi 4 (Optional for full mode)
- HD USB Camera
- IR Sensors (x4)
- DC Motors with Encoders
- Custom Titanium Scoop
- LiPo Battery
- Voltage Regulators
- Emergency Switch

### Software Dependencies
- Arduino IDE
- Python 3.8+
- OpenCV
- YOLOv8

## 🚀 Setup Instructions

### Full System Mode
1. Set up Raspberry Pi:
   ```bash
   # Install dependencies
   pip install -r src/Computer-Vision-Camera/requirements.txt
   ```
2. Upload Arduino code:
   - Use Arduino IDE
   - Select appropriate mode in config.h

### Arduino + Basic Vision Mode
1. Modify Arduino code:
   ```cpp
   // In config.h
   #define OPERATION_MODE BASIC_VISION
   ```
2. Upload modified code
3. Connect USB camera directly to Arduino

### Pure Arduino Mode
1. Configure Arduino:
   ```cpp
   // In config.h
   #define OPERATION_MODE PURE_ARDUINO
   ```
2. Verify IR sensor connections
3. Upload standalone code

## 🎮 Operation Guide

### Mode Switching
1. **Full System to Basic Vision**:
   ```bash
   # If Raspberry Pi fails:
   1. Press mode switch
   2. System auto-detects and switches
   3. LED indicates current mode
   ```

2. **Emergency Arduino Mode**:
   ```bash
   # For complete fallback:
   1. Hold mode switch 3 seconds
   2. Wait for confirmation LED
   3. Robot operates on IR only
   ```

### Starting the Robot
1. Select operation mode
2. Power up systems
3. Place in ring
4. Wait for ready signal

## 🏆 Competition Success

- Won national championship using all 3 modes
- Demonstrated system resilience
- 12-0 undefeated streak
- Best Technical Design Award

## 📊 Performance Metrics

| Mode | Vision Range | Response Time | Battery Life |
|------|-------------|---------------|--------------|
| Full | 2m | 20ms | 30min |
| Basic Vision | 1m | 40ms | 45min |
| Pure Arduino | 30cm | 10ms | 60min |

## 🔍 Troubleshooting

- **Vision System Fails**: Auto-switches to Basic Vision Mode
- **Camera Issues**: Falls back to Pure Arduino Mode
- **Sensor Problems**: Redundant sensors take over
- **Power Issues**: Emergency power management kicks in

## 👥 Contributing

Contributions welcome! See [Contributing Guidelines](CONTRIBUTING.md).

## 📜 License

MIT License - see [LICENSE](LICENSE)

---

<div align="center">

*Built with 🦾 by Mohammed Zaloom*

</div>
