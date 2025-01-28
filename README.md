# 🤖 Sumo Robot Batman

A championship-winning autonomous sumo robot that combines computer vision, Arduino-based control systems, and intelligent battle strategies. Winner of the National Sumo Robot Competition in Jordan.

<div align="center">

[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
![Arduino](https://img.shields.io/badge/Arduino-00979D?style=flat&logo=Arduino&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-27338e?style=flat&logo=OpenCV&logoColor=white)

</div>

## 🌟 Features

- **Bio-inspired Design**: Custom titanium scoop inspired by ant mandibles for superior opponent control
- **Computer Vision System**: Real-time opponent detection using YOLOv8
- **Hybrid Control**: Combines Arduino-based hardware control with Python-based intelligence
- **Battle Strategies**: Advanced movement and attack patterns implemented in C++
- **Sensor Fusion**: Integrated IR sensors and computer vision for reliable opponent tracking

## 🏗️ Project Structure

```
sumo-robot-batman/
├── src/
│   ├── Arduino-Code/          # Core robot control systems
│   │   ├── Attack.cpp/h       # Attack strategy implementation
│   │   ├── Edge.cpp/h         # Edge detection logic
│   │   ├── IR.cpp/h           # Infrared sensor handling
│   │   ├── Motor.cpp/h        # Motor control functions
│   │   ├── Search.cpp/h       # Opponent search algorithms
│   │   └── SumoMovement.cpp/h # Movement control system
│   ├── Computer-Vision-Camera/ # Vision system components
│   │   ├── predict.py         # YOLOv8 inference
│   │   └── requirements.txt   # Vision system dependencies
│   └── Python-Code/           # High-level control
│       ├── actuators_sensors.py # Hardware interface
│       ├── attack.py           # Attack pattern generation
│       ├── main.py            # Main control loop
│       └── search.py          # Search strategy
└── Prototype/                 # Design files and documentation
```

## 🔧 Requirements

### Hardware
- Arduino Mega 2560
- HD USB Camera
- IR Sensors (x4)
- DC Motors with Encoders
- Custom Titanium Scoop
- LiPo Battery

### Software
- Arduino IDE
- Python 3.8+
- OpenCV
- YOLOv8
- Required Python packages:
  ```bash
  pip install -r src/Computer-Vision-Camera/requirements.txt
  ```

## 🚀 Setup and Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/mozaloom/Sumo-Robot-Batman-Amman.git
   ```

2. Install Arduino dependencies:
   - Upload the Arduino code to your board
   - Install required libraries through Arduino IDE

3. Setup Python environment:
   ```bash
   cd src/Computer-Vision-Camera
   pip install -r requirements.txt
   ```

4. Configure camera settings:
   ```bash
   python calibrate_camera.py  # Adjust camera parameters
   ```

## 🎮 Usage

1. Power up the robot and ensure all connections are secure
2. Start the computer vision system:
   ```bash
   python src/Computer-Vision-Camera/predict.py
   ```
3. Launch the main control program:
   ```bash
   python src/Python-Code/main.py
   ```

## 🏆 Achievements

- 🥇 National Sumo Robot Competition Champion
- 🏆 Undefeated streak against 12 consecutive opponents
- 🌟 Best Design Award for bio-inspired scoop mechanism

## 🛠️ Technical Specifications

- **Weight**: Competition regulation weight
- **Dimensions**: Within official sumo robot specifications
- **Processing**: Dual system (Arduino + Onboard Computer)
- **Vision System**: YOLOv8 with custom training for opponent detection
- **Battery Life**: 45+ minutes in combat mode

## 👥 Contributing

Contributions are welcome! Please read our [Contributing Guidelines](CONTRIBUTING.md) for details on how to submit pull requests.

## 📜 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- IEEE BAU Chapter for support and resources
- National Robotics Competition organizers
- The robotics community in Jordan

---

<div align="center">

*Built with 🦾 by Mohammed Zaloom*

</div>
