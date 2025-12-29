# Arduino Mega 2560 Coding

This repository serves as a collection of basic to intermediate-level projects designed for the **Arduino Mega 2560**. This repository focuses on complex component integration, sensor data fusion, hardware multiplexing, and utilizing the extended I/O capabilities of the Mega 2560 board.

## 🚀 Repository Overview

The projects in this repository demonstrate the transition from basic I/O to system-level programming. Key concepts include **I2C communication protocols**, **state machine logic** for alarm systems, **hardware multiplexing** for multi-digit displays, and **analog sensor calibration**.

## 📂 Project Modules

### 1. Advanced Digital I/O & Control Logic
*Focus: Logic gates emulation, non-blocking code, and extended pin usage.*
* **LED Pattern Generator:** Complex lighting sequences (Chaser, Bounce) controlled via state functions.
* **Analog-Digital Integration:** Dynamic delay and brightness control using potentiometers mixed with digital switches.

### 2. Display Multiplexing & Extended I/O
*Focus: Array-based port manipulation and high-pin-count management.*
* **Dual 7-Segment Control:** simultaneous control of multiple 7-segment displays using the Mega's **digital pins 22-28** (Double Row Header).
* **4-Digit Time Display:** Implementation of multiplexing logic to drive a 4-digit countdown timer with minutes and seconds.

### 3. Environmental Monitoring Systems
*Focus: Sensor fusion and I2C LCD visualization.*
* **Temperature & Humidity Station:** Integration of **DHT11** and **LM35** sensors.
* **Data Visualization:** Real-time data output to **I2C LCD (16x2 and 20x4)**, featuring custom character rendering and kelvin/celsius conversion logic.

### 4. Timekeeping & Automation Systems
*Focus: Real-Time Clocks (RTC), Interrupts, and High-Voltage Control.*
* **Precision Digital Clock:** Timekeeping using the **DS1302 RTC** module.
* **Programmable Alarm System:** A fully functional user-programmable alarm that triggers **5V Relays** (for high-voltage appliance control) and visual/audio indicators.

## 🛠️ Hardware Requirements

To replicate these systems, the following hardware is required:

* **Microcontroller:** Arduino Mega 2560 (Required for extended GPIO projects)
* **Sensors:** DHT11 (Humidity), LM35 (Temperature)
* **Displays:** 7-Segment Displays (Common Anode), 4-Digit 7-Segment Display, LCD 16x2 or 20x4 (with I2C backpack)
* **Timing:** DS1302 Real Time Clock Module
* **Actuators:** 5V Relay Module, Piezo Buzzer, LEDs
* **Components:** Push Buttons, Potentiometers (10kΩ), Resistors (220Ω, 1kΩ, 10kΩ), Breadboard, Jumper Wires

## 💻 Software & Libraries

This code is written in C++ for the Arduino IDE.

**Required Libraries:**
* `LiquidCrystal_I2C` – For I2C LCD control.
* `DHT` – For reading DHT11/DHT22 sensors.
* `DS1302` (by Rinky-Dink Electronics or similar) – For RTC communication.
* `Wire` – Standard Arduino I2C library.

## 🔧 Setup & Installation

1.  **Clone the Repo:**
    ```bash
    git clone https://github.com/Jarenas-py/arduino-mega-2560-coding
    ```
2.  **Select Board:** In Arduino IDE, go to **Tools > Board** and select **Arduino Mega or Mega 2560**.
3.  **Install Libraries:** Navigate to **Sketch > Include Library > Manage Libraries** and search for the required libraries listed above.
4.  **Wiring:** Refer to photos included in each project folder for the proper circuit wiring. TinkerCAD & Wokwi website were utilized for the digital visualization of the circuit.
5.  **Upload:** Connect your Mega 2560 via USB and upload the sketch.

## 👤 Author

**Joseph Arenas**
* *Course:* BET-CPET (Computer Engineering Technology)
* *Institution:* Technological University of the Philippines - Manila

---
*This repository showcases academic and practical applications of embedded systems using the Arduino platform.*
