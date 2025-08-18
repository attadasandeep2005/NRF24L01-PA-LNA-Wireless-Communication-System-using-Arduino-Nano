
# NRF24L01+PA+LNA | 6-Channel Wireless Transmitter & Receiver Using Arduino Nano 

This project is a 6-channel wireless transmitter and receiver system built using the **NRF24L01+PA+LNA** module and **Arduino Nano**. It's designed to provide robust and long-range wireless communication for controlling robots, drones, or other RC applications.

## 🔧 Features

- 📡 Long-range communication using **NRF24L01+PA+LNA**
- 🎮 6 analog or digital input channels from transmitter
- 🔌 Easy-to-use Arduino Nano boards on both ends
- 🔄 Real-time data transmission with minimal latency
- 📥 Modular and customizable code
- ⚙️ Can be extended to more channels and features

## 📷 Project Setup Preview

> Yet to be Uploaded  
> Includes both transmitter and receiver circuits


## 🔌 Hardware Required

| Component              | Quantity |
|------------------------|----------|
| Arduino Nano           | 2        |
| NRF24L01+PA+LNA Module | 2        |
| Joystick / Potentiometer / Switch | 6 inputs |
| Connecting Wires       | As needed |
| 5V Regulated Power Supply | 2        |
| Capacitors (10µF recommended) | 2        |
| Antenna (optional but recommended) | 2 |

## 🛠️ Circuit Overview

**Transmitter Side:**
- 6 input channels connected to analog/digital pins
- NRF24L01 connected via SPI (CE, CSN, MOSI, MISO, SCK)

**Receiver Side:**
- Receives 6-channel data and maps it to digital/analog outputs
- Controls motors, servos, or actuators based on input values

> NOTE: Make sure to use a **capacitor (100-470µF)** across VCC and GND near the NRF module to avoid voltage drops.

## 🔌 Pin Configuration (Example)

| NRF24L01 | Arduino Nano |
|----------|---------------|
| VCC      | 3.3V (with regulator) |
| GND      | GND           |
| CE       | D9            |
| CSN      | D10           |
| SCK      | D13           |
| MOSI     | D11           |
| MISO     | D12           |

## 🧠 How It Works

1. Transmitter reads 6 inputs (joysticks/switches).
2. Sends the data packet wirelessly via NRF24L01.
3. Receiver collects the data and maps it to outputs (PWM, digital HIGH/LOW).
4. Used to control robots, cars, servos, lights, etc.

## 🚀 Applications

- Remote-controlled robots
- Wireless data logging
- RC cars, drones, and boats
- DIY IoT automation systems
- Wireless actuator control

## 💡 Future Improvements

- Add LCD/OLED display for feedback
- Battery voltage monitoring
- Failsafe implementation
- Bi-directional communication
- Enclosure design and 3D printing

## 📜 License

This project is open-source and free to use under the MIT License. Contributions and improvements are welcome!

---

> 🔧 Feel free to modify this project as per your requirement.  
> 📬 For queries, raise an issue or drop a comment!

