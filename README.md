Overview
This repository contains the codebase for an Automated Moon Tracker designed for astrophotography. The project integrates Arduino and Python scripts to control a pan and tilt device, allowing precise tracking of celestial objects such as the International Space Station (ISS) in real-time.

Key Features
Utilizes the Open Notify API for obtaining real-time ISS location data.
Implements SGP4 orbit determination principles for accurate tracking calculations.
Incorporates speed control mechanisms for smooth pan and tilt movements.
Integration with the Stellarium software for cultural astronomy research.
Circuit compartment for secure housing of the tracking system's electronics.
Code Structure
Arduino Script (Arduino_Code.ino): Controls the stepper motors and manages motor movements based on received pan and tilt angles. Dynamic speed control and EEPROM usage for continuous tracking.

Python Script (Python_Code.py): Calculates distance, azimuth, and elevation between the tracker and the ISS. Communicates with the Arduino board through serial connection, sending pan and tilt angles.

Usage
Upload the Arduino script to the Arduino microcontroller.
Run the Python script on the main control system (e.g., Raspberry Pi or computer).
Monitor tracking details through the serial console and adjust parameters as needed.
Dependencies
AccelStepper Library (for Arduino)
Stellarium Software (for cultural astronomy research)
