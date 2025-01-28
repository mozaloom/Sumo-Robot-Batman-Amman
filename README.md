Here's the adjusted README with the requested changes:

```markdown
# 🤖 Sumo Robot Batman

A championship-winning autonomous sumo robot featuring redundant systems and adaptive control strategies. Winner of the National Sumo Robot Competition in Jordan.

<div align="center">
  <img src="https://raw.githubusercontent.com/mozaloom/Sumo-Robot-Batman-Amman/main/Prototype/IMG.PNG" alt="Prototype" width="500"/>
</div>

<div align="center">

[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
![Arduino](https://img.shields.io/badge/Arduino-00979D?style=flat&logo=Arduino&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-27338e?style=flat&logo=OpenCV&logoColor=white)

</div>

## 🌟 Features

- **Dual System Architecture**: Plan A (RPi) and Plan B (Arduino) redundancy
- **Bio-inspired Design**: Titanium scoop inspired by ant mandibles
- **Multi-mode Vision**: From YOLOv8 tracking to basic IR detection
- **Battle Strategies**: Context-aware attack patterns
- **Fail-safe Systems**: Automatic degradation to simpler modes

## 🔄 System Plans

### Plan A: Raspberry Pi Master System (Primary)
- **Components**: 
  - Raspberry Pi 4 (Main brain)
  - HD Camera with YOLOv8
  - Full sensor array integration
- **Capabilities**:
  - 360° opponent tracking
  - Predictive movement algorithms
  - Energy-aware decision making
  - Real-time competition analytics

### Plan B: Arduino Emergency System (Fallback)
- **Components**:
  - Arduino Mega 2560
  - Quad IR sensor array
  - Emergency power system
- **Capabilities**:
  - Basic edge detection
  - Contact-based attack patterns
  - Ultra-low latency response
  - Extended battery operation

## 💡 Operation Modes

### 1. Full Cognitive Mode (Plan A)
```python
if opponent_detected():
    execute_advanced_attack()
elif ring_edge_detected():
    perform_evasive_maneuver()
else:
    search_pattern()
```
- Raspberry Pi handles strategic decisions
- Arduino manages real-time motor control
- 5ms sensor fusion processing

### 2. Hybrid Vision Mode (Plan B+)
- Activates when Plan A partially fails
- Arduino takes control with USB camera input
- Basic OpenCV blob detection
- Maintains 80% combat effectiveness

### 3. Pure Reflex Mode (Plan B)
```cpp
void loop() {
  checkIRsensors();
  avoidEdges();
  if (enemyDetected) {
    chargeAttack();
  }
}
```
- Fully Arduino-based operation
- IR sensor-driven responses
- 1ms reaction time guarantee
- 60+ minute runtime

## 🏗️ Hardware Architecture
```ascii

┌──────────┐             ┌──────▼───────┐             ┌───────────┐
│  HD      ├─────────────►              │◄────────────┤ Motor     │
│ Camera   │             │   Raspberry  │
                         │      Pi 4    │             │ Controllers
└──────────┘             │              │             └───────────┘
                         └──────┬───────┘
                ┌───────────────┴───────────────┐
                │                               │
           ┌────┴─────┐                   ┌─────▼────┐
           │ IR Array │                   │ Power    │
           │ (4x)     │                   │ Managment│
           └──────────┘                   └──────────┘
```


