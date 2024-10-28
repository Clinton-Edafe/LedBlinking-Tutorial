# Blinking an LED with an Arduino UNO - Step-by-Step Guide

## Description
This tutorial will guide you through the process of creating a simple Arduino project that makes an LED blink on and off. It's perfect for beginners looking to get started with Arduino programming.

## Table of Contents
1. [Components Required](#components-required)
2. [Circuit Setup](#circuit-setup)
3. [Code Upload](#code-upload)
4. [Observe the Result](#observe-the-result)

---

## Components Required
- 1 x Arduino UNO
- 1 x LED (any color)
- 1 x 220-ohm resistor
- Breadboard
- Jumper wires
- USB cable for Arduino UNO

---

## Circuit Setup
1. Connect the long leg (anode) of the LED to pin 13 on the Arduino.
2. Connect the short leg (cathode) of the LED to one side of the 220-ohm resistor.
3. Connect the other side of the resistor to the GND (ground) pin on the Arduino.

## Circuit Diagram
![Circuit](https://docs.arduino.cc/static/52c238dba09c2e40b69e0612ff02ef0f/a6d36/circuit.png)

## Schematic
![Circuit](https://docs.arduino.cc/static/c8dbeff786e52681c3d0e9ee9525e140/a6d36/schematic.png)

---

## Code Upload
1. Open the Arduino IDE on your computer.
2. Copy the following code into the editor:

   ```cpp
   // Blinking LED Code
   void setup() {
     pinMode(13, OUTPUT);  // Set digital pin 13 as an output
   }

   void loop() {
     digitalWrite(13, HIGH);  // Turn the LED on
     delay(1000);             // Wait for one second
     digitalWrite(13, LOW);   // Turn the LED off
     delay(1000);             // Wait for one second
   }
3. Upload the code to your Arduino board.

---

## Observe the Result:
- Once the code is uploaded, the LED should start blinking on and off at intervals of one second.