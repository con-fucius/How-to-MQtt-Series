# How-to-MQTT-series: LED Control with NodeMCU
## Project Statement
MQTT (Message Queuing Telemetry Transport) is a messaging application that supports asynchronous communication between parties. MQTT broker is responsible for receiving all messages,filtering,decision making and sending messages to subscribed clients.

This project demonstrates how to use MQTT  for asynchronous communication between devices. The NodeMCU (ESP8266 module) connects to an MQTT broker to send and receive messages, enabling remote control of an LED. This project serves as a beginner-friendly guide for understanding MQTT and IoT integration.

---

## Project Overview

- **MQTT Functionality**:
  - Asynchronous messaging protocol for lightweight communication.
  - MQTT broker handles message reception, filtering, and delivery to subscribed clients.

- **Objective**:
  - Connect a NodeMCU module to an MQTT broker.
  - Use the MQTT protocol to send messages and control an LED.

---

## Components Used

### 1. **NodeMCU (ESP8266 Module)**  
   - Operating Voltage: 3.3V  
   - Input Voltage: 7–12V  
   - Digital I/O Pins: 16  
   - Analog Input Pins: 1  
   - Interfaces: UART, SPI, I2C  
   - Memory: 4 MB Flash, 64 KB SRAM  
   - Clock Speed: 80 MHz  

### 2. **LED**  
   - Controlled via MQTT messages.  

### 3. **Resistor (220Ω)**  
   - Limits current to the LED to prevent damage.  

### 4. **Breadboard and Connecting Wires**  
   - Facilitates circuit assembly.  

### 5. **Programming Cable**  
   - Used to program the NodeMCU.

---

## Setup and Usage

### 1. **Hardware Setup**:
   - Connect the LED and resistor to the NodeMCU on the breadboard.
   - Use jumper wires for connections:
     - Connect the LED anode (+) to a digital pin on the NodeMCU.
     - Connect the cathode (-) to the resistor, then to the ground (GND) pin.

### 2. **Software Setup**:
   - Install the Arduino IDE and configure it for NodeMCU.
   - Add the necessary MQTT libraries (e.g., `PubSubClient`).
   - Write code to:
     - Connect to the MQTT broker.
     - Subscribe to a topic for receiving messages.
     - Control the LED based on received messages.

### 3. **MQTT Broker**:
   - Set up an MQTT broker (e.g., Mosquitto or HiveMQ).
   - Publish messages to control the LED (e.g., `"LED_ON"` or `"LED_OFF"`).

---

## Applications

- **IoT Development**:  
   Learn the fundamentals of MQTT for IoT device communication.  

- **Remote Control Systems**:  
   Extend this project to control multiple devices over MQTT.  

- **Home Automation**:  
   Use MQTT to build smart home solutions.  

---

## License

This project is open-source and free for personal or educational use. Feel free to modify and share.

---
