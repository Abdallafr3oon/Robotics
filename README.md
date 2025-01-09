# Hexapod Robot Control

This repository contains the code to control a hexapod robot using an ESP32 microcontroller and servo motors. The hexapod robot is designed to move forward by controlling its legs with servo motors.

## Table of Contents
- [Introduction](#introduction)
- [Hardware Requirements](#hardware-requirements)
- [Software Requirements](#software-requirements)
- [Setup](#setup)
- [Usage](#usage)
- [Code Explanation](#code-explanation)

## Introduction
The hexapod robot is a six-legged robot that can perform various movements by controlling its legs using servo motors. This project uses an ESP32 microcontroller to control the servo motors and make the robot move forward.

## Hardware Requirements
- ESP32 microcontroller
- Servo motors (12x for a hexapod)
- Adafruit PCA9685 PWM Servo Driver
- Power supply for the servos and ESP32
- Jumper wires and breadboard (optional)

## Software Requirements
- Arduino IDE
- ESP32Servo library
- Adafruit PWM Servo Driver library

## Setup
1. **Connect the Hardware:**
   - Connect the servo motors to the Adafruit PCA9685 PWM Servo Driver.
   - Connect the PCA9685 to the ESP32 using I2C (SDA and SCL pins).
   - Ensure that the power supply is connected to both the ESP32 and the servo driver.

2. **Install the Required Libraries:**
   - Install the `ESP32Servo` library from the Arduino Library Manager.
   - Install the `Adafruit PWM Servo Driver` library from the Arduino Library Manager.

3. **Upload the Code:**
   - Open the provided code in the Arduino IDE.
   - Select the correct board (ESP32) and port.
   - Upload the code to the ESP32.

## Usage
Once the code is uploaded and the hardware is set up, the hexapod robot will start moving forward. The robot's legs will move in a sequence to simulate forward motion.

## Code Explanation
The code provided controls the servo motors to make the hexapod robot move forward. Here's a brief explanation of the key parts of the code:

- **Servo Initialization:**
  ```cpp
  Servo a1, a2, a3, a4;
  Servo b1, b2, b3, b4;
  Servo c1, c2, c3, c4;
