# studious-OGB
# Arduino LED Blink Simulation Project

A simple embedded systems project that simulates a LED blinking at asymmetric intervals using an Arduino uno on Tinkercard. In this simulation, the LED remains ON for 2 seconds and OFF for 1 second.

This project is ideal for understanding basic microcontroller GPIO (General Purpose Input/Output) pins, digital write states, and standard time delays.

---

 Features
* Asymmetric Timing:Custom loop configurations deviation from standard 50/50 blink cycles (2s ON, 1s OFF).
* Simulation-Ready:Fully compatible with virtual simulation environments like Tinkercad.
* Beginner-Friendly: Clear, well-commented hardware layout and embedded C++ code structure.

---

 Components Used (Virtual)
* Microcontroller: Arduino Uno 
* Output Device: 1x Red LED
* Current-Limiting Resistor:** 1x 220Ω Resistor (to protect the LED from burning out)
* Connections:** Breadboard & Jumper wires

---

## Circuit Schematic Look
* LED Anode (Long leg / Positive): Connected to Digital Pin 13 via a 220Ω resistor.
* LED Cathode (Short leg / Negative):** Connected directly to the Arduino GND pin.

---

## Arduino Source Code

```cpp
/*
  Asymmetric LED Blink Simulation
  Turns on an LED on for two seconds, then off for one second, repeatedly.
*/



void setup() {
  // Initialize the digital pin as an output signal
  pinMode(13, OUTPUT);
}

void loop() {
  digitalWrite(13, HIGH);   // Turn the LED on (High voltage level)
  delay(2000);                  // Wait for 2000 milliseconds (2 seconds)
  
  digitalWrite(13, LOW);    // Turn the LED off (Low voltage level)
  delay(1000);                  // Wait for 1000 milliseconds (1 second)
}
