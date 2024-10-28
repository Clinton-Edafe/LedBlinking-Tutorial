# Tutorial

## Title: Blinking an LED with an Arduino UNO - Step-by-Step Guide

### Description
This tutorial will guide you through the process of creating a simple Arduino project that makes an LED blink on and off. It's perfect for beginners looking to get started with Arduino programming.

---

### Steps:

#### Components Required:
- 1 x Arduino UNO
- 1 x LED (any color)
- 1 x 220-ohm resistor
- Breadboard
- Jumper wires
- USB cable for Arduino UNO

---

#### Circuit Setup:
1. Connect the long leg (anode) of the LED to pin 13 on the Arduino.
2. Connect the short leg (cathode) of the LED to one side of the 220-ohm resistor.
3. Connect the other side of the resistor to the GND (ground) pin on the Arduino.

---

#### Code Upload:
1. Open the Arduino IDE on your computer.
2. Copy the following code into the editor:

   ```cpp
   // Blinking LED Code
   void setup() {
     pinMode(13, OUTPUT);  // Set digital pin 13 as an output
   }
3. Upload the code to your Arduino board.
   void loop() {
     digitalWrite(13, HIGH);  // Turn the LED on
     delay(1000);             // Wait for one second
     digitalWrite(13, LOW);   // Turn the LED off
     delay(1000);             // Wait for one second
   }

- - -

#### Observe the Result:
Once the code is uploaded, the LED should start blinking on and off at intervals of one second.