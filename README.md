# 🤖 🤖 Sumo Robot: Batman Amman

## 🏆 Overview  
Welcome to the repository for the **BatmanAmman Sumo Robot**, a project designed for the **National Sumo Robot Competition**. Our team engineered an autonomous combat robot capable of detecting opponents and making strategic moves to dominate sumo matches.

---

## 📜 Project Details  

### **Team Name**  
**BatmanAmman**

---

### **Design and Components**  
- **3D Modeling**: Designed using **Fusion 360**  
- **Main Controller**:  
  - Initially planned: Raspberry Pi 5 Model B  
  - Final implementation: Arduino Mega  
- **Programming Languages**:  
  - Planned: Python  
  - Final: Arduino C++  
- **Computer Vision**:  
  - Planned: Custom YOLO-based model for opponent detection (not implemented due to hardware delays)  
- **Motors and Wheels**:  
  - JSumo Titan Motors (200 RPM) with high-traction rubber wheels  
- **Sensors**:  
  - **6 IR Sensors**: SUMO JS200XF Infrared Long Range Sensors  
  - **4 QTR Sensors**: Edge detection  
  - **Camera**: Raspberry Pi Camera Module 3 Noir (Wide Angle)  
- **Motor Drivers**: 2× Dual H-Bridge Drivers  
- **Microcontroller**: Arduino Mega  
- **Switches**: 4-Position DIP Switch  
- **Batteries**:  
  - 3000 mAh LiPo Battery (motors)  
  - 9V LiPo Battery (Arduino)  

---

## 🔄 Project Timeline and Changes  

### **Initial Setup**  
- Began with **Raspberry Pi 5 Model B** as the main controller.  
- Developed a Python-based program integrating **computer vision** to enhance attack accuracy.  

### **Challenges**  
- The **Coral TPU**, critical for the computer vision model, did not arrive on time.  
- This forced a pivot to a **sensor-based system** using Arduino for the final implementation.  

### **Final Setup**  
- Switched to **Arduino Mega** with 2× Dual H-Bridge drivers.  
- Successfully completed the robot using **Arduino C++** for reliable performance.  

### **Future Plans**  
- Integrate reinforcement learning and advanced computer vision features (dependent on Coral TPU availability).  
- Develop modular, wireless diagnostic systems for real-time performance monitoring.  

---

## 🖼️ Design Showcase  
<div align="center">
  <img src="https://raw.githubusercontent.com/mozaloom/Sumo-Robot-Batman-Amman/main/Prototype/IMG.PNG" alt="BatmanAmman Prototype" width="500"/>
</div>

---

## ⚙️ Installation and Usage  

### **Hardware Setup**  
1. **Assemble the Robot**: Use the designed 3D parts to construct the robot.  
2. **Connect Components**: Follow the provided wiring diagram in the hardware files.  
3. **Install Batteries**:  
   - Connect the **3000 mAh LiPo battery** to power the motors.  
   - Use the **9V LiPo battery** to power the Arduino.  

### **Software Setup**  

#### **Arduino Code**  
- Upload the provided code to the **Arduino Mega** using the Arduino IDE.  
- Navigate to the `arduino` directory to locate the final implementation files.  

#### **Python Code (Planned)**  
- The Python code for reinforcement learning and advanced features is currently under development.  


<div align="center">

![Arduino](https://img.shields.io/badge/Arduino-00979D?style=flat&logo=Arduino&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=Python&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-27338e?style=flat&logo=OpenCV&logoColor=white)
![Raspberry Pi](https://img.shields.io/badge/Raspberry%20Pi-C51A4A?style=flat&logo=Raspberry-Pi&logoColor=white)
![JSumo](https://img.shields.io/badge/JSumo-000000?style=flat&logo=JSumo&logoColor=white)

</div>

---

## 🌟 Highlights  

| Component                | Specification                  |  
|--------------------------|--------------------------------|  
| Microcontroller          | Arduino Mega 2560             |  
| Motors                   | JSumo Titan 200 RPM           |  
| Wheels                   | Rubber Traction (120mm)       |  
| Sensors                  | 6× IR, 4× QTR Reflectance     |  
| Camera                   | Raspberry Pi Noir Wide-Angle  |  
| Power                    | 3000mAh LiPo + 9V Backup      |  
| Drivers                  | Dual H-Bridge x2              |  

---

## 🚨 Challenges & Solutions  

| Challenge                | Solution                      |  
|--------------------------|-------------------------------|  
| Coral TPU Delay          | Switched to sensor-based system with Arduino. |  
| Motor Synchronization    | Implemented a PID feedback loop. |  
| Battery Drain            | Added power isolation circuits for efficiency. |  
| Sensor Interference      | Shielded wiring to reduce noise. |  

---

## 🔮 Future Roadmap  
1. Integrate **Coral TPU** for delayed vision-based strategies.  
2. Develop **reinforcement learning** algorithms for adaptive strategies.  
3. Add **wireless diagnostics** for performance monitoring.  
4. Create **modular sensor pods** for enhanced versatility.  

---

<div align="center">
  <em>By Mohammed Zaloom</em>
</div>

