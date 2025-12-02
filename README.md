**# Multi-Thread-Parking-System**
This project demonstrates the design and implementation of an automated smart parking management system using an Arduino microcontroller, IR sensors, a servo motor, and an LCD display. The system monitors and manages parking availability across two floors, automates gate control, and guides users to available parking slots in real-time.

**📌 ✨ Features**

Detects vehicle presence at the entrance using an IR sensor

Automatically opens the gate via servo motor when parking space is available

Displays real-time parking availability on LCD (16×2)

Differentiates between Ground Floor and First Floor slots

Supports 8 parking slots (4 on each floor)

Provides live updates on slot occupancy

Alerts user with “Parking Full” when all slots are occupied

**📁 Project Overview**

This system uses IR sensors to detect whether a parking slot is vacant or occupied. When a vehicle arrives at the entrance:

Entrance IR sensor detects the vehicle

Arduino checks ground-floor slots first

If no slots are free, it checks the first floor

If a slot is available:

Displays floor & slot number on LCD

Opens the gate for 5 seconds

If no slot is free:

Displays “Parking Full”

The system ensures smooth, automated parking flow without human supervision.

**🧠 Technology Used**

Arduino Uno

IR Sensors (Entrance + Slot Sensors)

Servo Motor

16×2 I2C LCD Display

Jumper Wires & Mounting Hardware

**🛠️ Hardware Components**
Component	Quantity
Arduino Uno	1
IR Sensors	9 (1 entrance, 8 slot sensors)
Servo Motor (SG90/MG995)	1
LCD 16×2 with I2C module	1
Breadboard & Wires	as required
**🔌 Pin Connections**
Entrance Sensor
Component	Arduino Pin
Entrance IR Sensor	D2
**Ground Floor Sensors (4 slots)
Slot	Arduino Pin**
G1	D3
G2	D4
G3	D5
G4	D6
**First Floor Sensors (4 slots)
Slot	Arduino Pin**
F1	D7
F2	D8
F3	D9
F4	D10
Servo Motor
**Wire	Arduino Pin**
Signal	D11
Power	5V
Ground	GND
LCD I2C
**Wire	Arduino Pin**
SDA	A4
SCL	A5

**📸 How the System Works**

A vehicle arrives → entrance sensor triggers

Arduino checks parking availability

LCD displays the available slot (Ground or First Floor)

Gate opens automatically

Parking info updates in real time

