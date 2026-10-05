# IoT-Autonomous-Robot
# Fire Detection and Quick Response Robot Using Arduino

An Arduino-based robotic system designed to detect fire and smoke and provide a quick response using multiple sensors, actuators, and communication modules.

## Overview

Fire hazards require fast detection and response to minimize damage to life and property. This project develops a low-cost robotic system that combines fire and smoke sensing with robotic mobility and remote monitoring.

The system uses an Arduino UNO as the main controller. Flame and smoke sensors are used for fire detection, while an ultrasonic sensor assists with distance measurement and obstacle-related control. The robot can provide alerts and communicate sensor information through wireless communication modules.

An ESP32-CAM can also be integrated to provide real-time video monitoring.

## Objectives

- Detect fire and smoke using multiple sensors.
- Process sensor data using an Arduino UNO.
- Provide real-time alerts when fire or smoke is detected.
- Enable robotic movement using DC motors.
- Use an ultrasonic sensor for distance measurement.
- Provide wireless monitoring and communication.
- Explore real-time video monitoring using ESP32-CAM.

## Hardware Components

- Arduino UNO
- Flame Sensor / IR Sensor
- MQ-2 Smoke Sensor
- HC-05 Bluetooth Module
- ESP32-CAM
- Ultrasonic Sensor
- DC Motors
- SG90 Servo Motor
- L293D Motor Driver
- MT3608 Boost Converter
- Li-Ion Battery and Holder
- Buzzer
- LED
- Robot Chassis

## Software and Tools

- Arduino IDE
- Embedded C / Arduino Programming
- Arduino Libraries
- Bluetooth Communication
- ESP32-CAM

## Working Principle

The system collects information from the flame and smoke sensors and sends the sensor readings to the Arduino UNO.

The Arduino processes the sensor information and determines whether a fire or smoke condition is present. When a potential fire hazard is detected, the system can activate warning indicators and send information through the communication module.

The ultrasonic sensor measures the distance to nearby objects. The Arduino uses this information for motor-control decisions.

The robot uses an L293D motor driver to control its DC motors, allowing it to move within the environment.

The ESP32-CAM can be used to provide video streaming for remote monitoring.

## System Architecture

The main controller of the system is the Arduino UNO.

The Arduino receives inputs from:

- Flame sensor
- Smoke sensor
- Ultrasonic sensor

It controls:

- DC motors through the L293D motor driver
- Servo motor
- Warning indicators

The system can also communicate through Bluetooth and interface with an ESP32-CAM for remote monitoring.

## Project Workflow

1. Power the system.
2. Initialize the Arduino and connected sensors.
3. Read flame and smoke sensor values.
4. Process the sensor readings.
5. Detect possible fire or smoke conditions.
6. Activate appropriate alerts.
7. Measure distance using the ultrasonic sensor.
8. Control robot movement using the motor driver.
9. Send sensor information through the communication interface.
10. Monitor the environment using the camera module when available.

## Results

The prototype was successfully implemented using an Arduino-based robotic platform.

The project demonstrated:

- Fire and smoke detection
- Sensor data monitoring
- Ultrasonic distance measurement
- DC motor control
- Robotic movement
- Wireless communication
- Real-time monitoring capability

The project report describes a detection success rate of over 90% and a response time of less than five seconds under the tested conditions.

## Applications

- Fire monitoring
- Hazardous-area monitoring
- Industrial safety
- Remote surveillance
- Emergency response systems
- Residential fire-safety applications

## Future Scope

Possible improvements include:

- Increasing sensor detection range
- Adding additional gas and environmental sensors
- Using AI/ML for improved fire detection
- Reducing false alarms
- Improving autonomous navigation
- Enhancing obstacle avoidance
- Improving wireless communication
- Expanding real-time video monitoring

## Repository Structure

```text
Fire-Detection-and-Quick-Response-Robot/
│
├── README.md
├── Code/
│   ├── Fire_Smoke_Detection.ino
│   └── Ultrasonic_Motor_Control.ino
├── Circuit/
│   └── Block_Diagram.png
├── Results/
│   ├── Robot_Setup.jpg
│   ├── Robot_Front_View.jpg
│   └── Sensor_Output.png
└── Documentation/
    └── Project_Report.pdf
