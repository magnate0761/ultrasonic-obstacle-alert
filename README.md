# Ultrasonic Obstacle Detection and Alert System

Mini project for **23CSE201 – Procedural Programming Using C**, B.Tech CSE, Amrita Vishwa Vidyapeetham, Nagercoil.

## Overview
An Arduino Nano continuously measures distance using an HC-SR04 ultrasonic sensor. When an obstacle comes within 40 cm, a buzzer and LED are triggered as an alert, and live distance readings are printed to the Serial Monitor.

## Hardware
- Arduino Nano V3.0 (ATmega328P, CH340)
- HC-SR04 Ultrasonic Sensor Module
- 5V Active Piezo Buzzer
- LED
- Breadboard + jumper wires
- 9V battery with snap connector (Vin)

## Pin Connections
| Component Pin | Arduino Pin |
|---|---|
| HC-SR04 VCC | 5V |
| HC-SR04 GND | GND |
| HC-SR04 Trig | D6 |
| HC-SR04 Echo | D7 |
| LED (+) | D4 |
| Buzzer (+) | D5 |

## How It Works
1. Trigger a 10 µs pulse on the Trig pin.
2. Measure echo pulse duration with `pulseIn()`.
3. Convert to distance in cm.
4. If distance < 40 cm → buzzer + LED ON, else OFF.
5. Print distance to Serial Monitor (9600 baud).

## Files
- `ultrasonic_obstacle_alert.ino` – Arduino sketch
- `circuit_photo.jpg` – photo of the assembled breadboard circuit

## Author
Arjun — NC.SC.U4CSE25206
