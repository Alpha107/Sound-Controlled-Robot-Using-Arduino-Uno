# Sound Controlled Robot Using Arduino Uno

A remote-controlled robot that responds to sound commands such as claps or loud noises. This project demonstrates analog signal processing and motor control based on audio input.

---

## Introduction
The Sound Controlled Robot is designed to move based on sound signals, such as clapping. A microphone module detects sound intensity and converts it into an electrical signal, which is processed by the Arduino Uno. Based on the detected sound pattern, the Arduino controls the motors to move the robot forward, stop, or change direction.

This project helps in understanding analog sensor interfacing, threshold detection, and motor control. Sound-controlled robots are useful in assistive robotics, interactive applications, and basic automation systems.

---

## Components Used

| Component | Description | Purpose |
|-----------|------------|--------|
| Microphone Module | Sound sensor | Detects sound input |
| 4-Wheel Chassis | Mechanical base with wheels | Robot structure |
| BO Motors (4) | DC geared motors | Vehicle movement |
| Arduino Uno | ATmega328P microcontroller | Main controller |
| Motor Driver | L298N Dual H-Bridge | Controls motor direction and speed |
| Jumper Wires | Electrical connections | Circuit wiring |
| Batteries | Li-ion / AA | Power supply |
| Battery Holders | Secure battery placement | Power management |
| LEDs | Indicator lights | Show robot status |
| Resistors | Current limiting | Protect LEDs and circuits |
| Buzzer | Audio alert | Feedback for sound input |

---

## System Diagrams

### Block Diagram

<img width="499" height="525" alt="Screenshot 2026-04-23 152205" src="https://github.com/user-attachments/assets/b3b1fdd6-14c1-4396-b64b-546c1007e780" />

*The microphone module detects sound and sends signals to the Arduino. Based on sound intensity, Arduino controls the motor driver to move the robot. LEDs and buzzer provide feedback.*

### Circuit Diagram
![Circuit Diagram](images/circuit_diagram.png)  
*Microphone module is connected to analog pins of Arduino. Motor driver receives PWM and direction signals from Arduino. LEDs and buzzer connected via resistors indicate status. Separate battery lines power the motors and controller.*

---

## Problems Faced
- Microphone sensitivity caused false triggers  
- Difficulty distinguishing between different sound patterns  
- Environmental noise affecting performance  
- Motor vibration interfering with sensor readings  
- Power noise affecting analog signal stability  

---

## Future Improvements
- Implement sound pattern recognition for better control  
- Add filtering to reduce noise interference  
- Use multiple microphones for directional sound detection  
- Integrate Wi-Fi or Bluetooth control as backup  
- Replace L298N with a more efficient motor driver  
- Use ESP32 for advanced sound processing  

---

## Conclusion
The Sound Controlled Robot using Arduino Uno successfully demonstrates robotic movement triggered by sound input. The project enhanced skills in analog sensor processing, motor control, and real-time decision making. Despite environmental noise challenges, the robot responded reliably to sound commands, providing a fun and interactive robotics project.

