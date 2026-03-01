# Vision-Based Autonomous Mobile Robot (NI myRIO + LabVIEW)

## 📌 Project Overview
This project presents the design and implementation of a vision-based autonomous mobile robot system using NI myRIO and LabVIEW.  

The system integrates gyroscope feedback, encoder-based localization, motor control, fuzzy logic tuning, and real-time image recognition to achieve straight-line control, waypoint tracking, number recognition, color recognition, and trajectory detection.

The objective of this project is to develop a complete hardware–software co-designed autonomous system with closed-loop feedback control and computer vision capability.

---

## 🏗 System Architecture

### 🔹 Hardware Components
- NI myRIO
- MPU6050 Gyroscope
- L298N Motor Driver Module
- TT Motors with Encoders
- Webcam
- Battery Pack
- Breadboard and Mechanical Chassis Structure

### 🔹 Software Platform
- LabVIEW (Real-Time Control)
- Vision Assistant (Pattern Matching / Color Matching)
- Fuzzy Logic Control
- PWM Motor Control

---

## ⚙ Core Functionalities

### 1️⃣ Straight-Line Control
- Yaw angle feedback using MPU6050
- P-gain based turn duty cycle adjustment
- PWM motor speed control
- Dead-zone compensation

### 2️⃣ Waypoint Tracking
- Encoder-based distance calculation
- Position estimation (Xt, Yt)
- Multi-point array tracking logic
- Closed-loop correction

### 3️⃣ Vision-Based Recognition
- Pattern Matching for number recognition
- Color Pattern Matching for target tracking
- Edge detection for trajectory identification
- Real-time coordinate extraction for motor control feedback

### 4️⃣ Fuzzy Logic Control
- Adaptive turn control
- Rule-based duty cycle adjustment
- Gain tuning optimization

---

## 🔄 Control Flow

Sensor Input → myRIO → LabVIEW Processing →  
- Motor PWM Control  
- Direction Adjustment  
- Vision-Based Target Tracking  

Encoder & Gyroscope Feedback → Closed-Loop Correction  

---

## 🚧 Challenges and Solutions
- Gyroscope zero drift → Calibration compensation  
- Motor over-voltage instability → Gain reduction & voltage stabilization  
- Wiring instability → Multimeter validation & circuit reorganization  
- Network instability → External hotspot optimization  
- myRIO crash issues → Program modularization  
- Battery voltage drop → Pre-charge above rated voltage  
- Wheel slip issue → Surface and wheel optimization  
- Fuzzy overshoot issue → Gain range limitation and rule expansion  

---

## 📊 Experimental Results
- Stable straight-line movement
- Accurate waypoint tracking
- Successful number and color recognition
- Real-time trajectory detection
- Closed-loop feedback performance validation

---

## 🚀 Future Improvements
- Improved hardware reliability before implementation
- Optimized fuzzy control rules
- Velocity-based fuzzy tuning
- Pre-testing myRIO stability
- Enhanced power management system

---

## 📂 Project Structure
