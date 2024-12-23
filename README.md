# 🚗 Project 11: Microprocessor Application System  
This repository contains the implementation and code for **Team 11**’s project in the Microprocessor Application System course. The project integrates multiple embedded systems and control mechanisms to build a fully functional, intelligently controlled vehicle.  

---

## 🔧 Project Overview  
The project utilizes the **Hiwonder Ackermann Steering** system with an **Arduino MEGA** microcontroller, focusing on the following key components:  
- **Regenerative Braking System**: Efficiently recycles kinetic energy back into the battery using a rectifier circuit and switching calculations.  
- **PID Control**: Implements fine-tuned Proportional-Integral-Derivative control for DC motors, ensuring precise synchronization and target speed tracking.  
- **Wireless Communication**: Seamless communication between subsystems for better coordination.  
- **Line Tracing**: Uses servo-controlled steering to follow predefined paths.  

The vehicle is a **Rear-Wheel Drive (RWD)** model with front steering, and all subsystems are designed to interact cohesively to optimize performance and efficiency.  

---

## ⚙️ System Architecture  
### 1️⃣ Arduino MEGA (Main Controller)  
- Handles **DC motor control** with PID for:  
  - **Motor Synchronization**: Ensures both motors operate in harmony.  
  - **Target Speed Control**: Dynamically adjusts motor speed.  
- Coordinates data flow between subsystems and manages interrupts for smooth operation.

### 2️⃣ Arduino UNO (Regenerative Braking System)  
- Manages the **regenerative braking circuit** using a relay module.  
- Includes logic for switching voltage in and out to charge the batteries while powering the motors.  

### 3️⃣ Arduino UNO (Servo Control and Line Tracing)  
- Controls **steering mechanisms** and executes **line tracing** using servo motors.  
- Implements precise path-following algorithms for autonomous navigation.

---

## 🗂️ Repository Structure  
- **`Arduino_mega_dc/`**:  
  Contains the code for the **main motor control**, including:  
  - **PID for motor synchronization.**  
  - **PID for target speed tracking.**  

- **`Arduino_uno_regen/`**:  
  Contains the code for the **regenerative braking system**, handling:  
  - Voltage switching via the relay module.  
  - Efficient power management and battery charging logic.  

- **`Arduino_uno_servo/`**:  
  Contains the code for **servo control** and **line tracing**, managing:  
  - Steering mechanisms.  
  - Lane-following algorithms.  

- **`subsystems/`**:  
  Contains code trials and experimental implementations of various subsystems.

---

## 📜 Circuit Design for Regenerative System  
The regenerative braking system design integrates a **rectifier circuit** for voltage regulation and switching calculations for power flow control. The complete circuit diagram and design details can be found in the project documentation.

---

## ✨ Features  
- **PID Visualization**: Showcases the effect of proportional, integral, and derivative gains individually.  
- **Hardware Optimization**: Efficient hardware division for managing multiple systems and interrupts.  
- **Real-Time Synchronization**: Seamless coordination between motors, braking, and steering subsystems.  

---

