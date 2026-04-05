# 3-Mini-MICS-6814-Gas-Sensor-Piggyback
![image alt](https://github.com/0mollo/3-Mini-MICS-6814-Gas-Sensor-Piggyback/blob/main/MICS%206814%20Top%20View.png) ![image alt](https://github.com/0mollo/3-Mini-MICS-6814-Gas-Sensor-Piggyback/blob/main/MICS%206814%20Bottom%20View.png)

Interfacing the **MICS-6814 Triple MOS Gas Sensor Module** with the **ESP32-C3 Mini**.

This repository is intended to help anyone, including a complete beginner, understand:

- what this piggyback does
- how to connect it
- how to power it
- how to test it
- where it can be used
- what software is required



## 1. Overview

The **MICS-6814** is a **triple MOS gas sensor** module commonly used to observe the presence or variation of gases such as:

- **Carbon Monoxide (CO)**
- **Ammonia (NH₃)**
- **Nitrogen Dioxide (NO₂)**

This piggyback PCB adapts the module neatly to the **ESP32-C3 Mini**, making the wiring cleaner, more reliable, and easier to reproduce.

The board is designed so that the three gas output channels from the sensor module are brought directly to the selected GPIO pins of the **C3-Mini**.



## 2. Board Identity

- **Board Name:** C3-Mini MICS-6814 Gas Sensor Piggyback
- **Version:** V1.1
- **Target Controller:** ESP32-C3 Mini
- **Sensor Module:** MICS-6814 Triple MOS Gas Sensor Module



## 3. What This Piggyback Does

This piggyback board:

- provides a compact mounting arrangement for the MICS-6814 module
- maps the module outputs to the ESP32-C3 Mini
- simplifies prototyping and testing
- reduces loose jumper wiring
- makes documentation and reuse easier

It is especially useful for:

- hardware prototyping
- sensor testing
- educational projects
- air quality experiments
- embedded systems demonstrations



## 4. Pin Mapping

The MICS-6814 module is mapped to the ESP32-C3 Mini as follows:

| MICS-6814 Module Pin | Function | ESP32-C3 Mini Pin |
|---|---|---|
| +5V | Power input | 5V |
| GND | Ground | GND |
| CO | Carbon Monoxide output | GPIO4 |
| NH3 | Ammonia output | GPIO0 |
| NO2 | Nitrogen Dioxide output | GPIO1 |



## 5. Connection Summary

### Sensor to ESP32-C3 Mini

- `+5V  -> 5V`
- `GND  -> GND`
- `CO   -> GPIO4`
- `NH3  -> GPIO0`
- `NO2  -> GPIO1`



  Notes:
  - This sketch reads raw sensor values.
  - Raw values are useful for testing and trend observation.
  - They are not direct gas concentration values in ppm.
  ## 6. Schematic layout
  [See file](https://github.com/0mollo/3-Mini-MICS-6814-Gas-Sensor-Piggyback/blob/main/MICS-6814%20Gas%20sensor.pdf)
 
  ### Arduino Test Code
[See](https://github.com/0mollo/3-Mini-MICS-6814-Gas-Sensor-Piggyback/blob/main/Arduino%20Test%20Code.docx)
