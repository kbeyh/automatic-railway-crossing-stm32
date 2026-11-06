
# 🚆 Automatic Railway Level Crossing Opening and Closing System Using STM32

An embedded systems project that demonstrates the automation of railway level crossing gates using an STM32 microcontroller, IR sensors, a servo motor and warning indicators.

## 📌 Project Overview

The Automatic Railway Level Crossing System is designed to automate the opening and closing of railway gates based on train detection.

Traditional railway crossings may depend on manual gate operation, which requires continuous monitoring and timely human intervention.

This project demonstrates an automated solution using an STM32 Blue Pill microcontroller. IR sensors detect the approaching train and its clearance, while a servo motor controls the railway gate.

A buzzer and LED indicators provide visual and audible warnings to road users.

## 🎯 Objectives

- Develop an automatic railway gate control system using STM32.
- Detect approaching trains using IR sensors.
- Automatically close the railway gate when a train approaches.
- Activate warning signals using a buzzer and red LED.
- Detect train clearance using a second IR sensor.
- Automatically reopen the railway gate after the train passes.
- Understand embedded systems and microcontroller-based automation.

## ⚙️ Hardware Components

| Component | Function |
|---|---|
| STM32 Blue Pill | Main processing and control unit |
| STM32F103C8T6 | Microcontroller |
| IR Sensor 1 | Detects approaching trains |
| IR Sensor 2 | Detects train clearance |
| SG90 Servo Motor | Controls railway gate movement |
| Buzzer | Provides audio warning |
| Red LED | Indicates gate closed condition |
| Green LED | Indicates gate open condition |
| ST-Link V2 | Programs the STM32 |
| Breadboard | Hardware connections |
| Jumper Wires | Component interfacing |
| Resistors | LED current limiting |
| Regulated 5V Supply | Servo motor power supply |

## 💻 Software Requirements

- Embedded C
- STM32CubeIDE
- STM32 Development Environment
- ST-Link Programmer

## 🔄 Working Principle

The system operates through the following sequence:

**1. Initial Condition**
- Railway gate remains open.
- Green LED is ON.
- Red LED and buzzer are OFF.

**2. Train Detection**
- The first IR sensor detects an approaching train.
- The sensor sends a signal to the STM32 controller.

**3. Warning Activation**
- Red LED turns ON.
- Buzzer gets activated.

**4. Gate Closing**
- STM32 sends a control signal to the SG90 servo motor.
- The railway gate moves to the closed position.

**5. Train Passing**
- Gate remains closed while the train passes through the crossing.

**6. Train Clearance**
- The second IR sensor detects the train after it passes the crossing.

**7. Gate Opening**
- Buzzer turns OFF.
- Red LED turns OFF.
- Servo motor raises the gate.
- Green LED turns ON.

## 🏗️ System Architecture

The system consists of three major sections:

**Input Section**
- IR Sensor 1
- IR Sensor 2

**Processing Section**
- STM32 Blue Pill Microcontroller

**Output Section**
- SG90 Servo Motor
- Buzzer
- Red LED
- Green LED

### System Block Diagram

IR Sensors → STM32 Blue Pill → Servo Motor, Buzzer and LED Indicators

## 🧪 Testing

The system is evaluated under four operating conditions:

| Test Case | Expected Result |
|---|---|
| No train detected | Gate remains open |
| Train detected | Warning activated and gate closes |
| Train passing | Gate remains closed |
| Train clearance detected | Warning stops and gate opens |

## 🚀 Future Improvements

- Advanced train detection sensors.
- Wireless communication.
- Obstacle detection on railway tracks.
- Emergency alert system.
- Backup power supply.
- Real-time railway crossing monitoring.

## 📚 Project Documentation

The complete academic project report is available in the `Report` folder.

## 👨‍💻 Project Team

Developed as a Microcontrollers academic microproject.

**Department of Computer Science and Engineering**

MES College of Engineering, Kuttippuram.

**Team Members:**
- Adithyan KB
- Ayisha Minha PM
- Fathima Jebin KP
- Fathima Mehrin MV
- Pranav MP

**Project Guide:** Ms. Fathima Sanam U V

**Academic Year:** 2026–2027

## ⚠️ Disclaimer

This project is an educational prototype developed for academic demonstration. It is not designed or certified for deployment in actual railway infrastructure.

## ⭐ Acknowledgement

This project was developed as part of the Microcontrollers course (PBCST504).
