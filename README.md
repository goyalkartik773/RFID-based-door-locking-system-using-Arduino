# RFID-based-door-locking-system-using-Arduino
An RFID-based door locking system uses an Arduino and an RC522 reader to authenticate RFID cards. When a valid card UID is detected, Arduino triggers a servo/solenoid lock to open the door. Invalid cards are rejected, making it a secure, low-cost and contactless access control system.

# 📌 Project Preview
🖼️ Image
</br>
<img src="https://raw.githubusercontent.com/goyalkartik773/RFID-based-door-locking-system-using-Arduino/main/coaImg.jpeg" width="500">

# 🎥 Video Demo
<video src="https://raw.githubusercontent.com/goyalkartik773/RFID-based-door-locking-system-using-Arduino/main/demo.mp4" 
       controls 
       width="500">
</video>


# 🔧 Features

Contactless door authentication using RFID
Works with RC522 reader and Arduino
Supports multiple authorized UIDs
Auto-locking mechanism
LED/Buzzer feedback system
Can use servo or solenoid lock
Affordable and easy to replicate

# 🛠️ Components Used

Arduino UNO / Nano
RFID Module RC522
RFID Tags/Cards
Servo Motor / Solenoid Lock
Buzzer
LEDs (Red/Green)
Jumper wires
External power supply (if using solenoid lock)

# 🔌 Circuit Connections
RFID RC522 → Arduino UNO
RC522 Pin	Arduino Pin
SDA	D10
SCK	D13
MOSI	D11
MISO	D12
RST	D9
3.3V	3.3V
GND	GND
Servo Motor
Servo Pin	Arduino Pin
Signal	D3
VCC	5V
GND	GND

# circuit diagram as circuit.png
<img src="https://raw.githubusercontent.com/goyalkartik773/RFID-based-door-locking-system-using-Arduino/main/circuit.png](https://github.com/goyalkartik773/RFID-based-door-locking-system-using-Arduino/blob/main/circuit.png" width="500">

# 💻 How It Works
RFID reader scans the tag/card.
Sends its UID to Arduino using SPI communication.
Arduino compares UID with authorized list in code.
Match → Door Unlocks (servo rotates or solenoid activates).
No Match → Access Denied.
System auto-locks after a programmed delay.

# ▶️ Getting Started
1. Install Libraries
Go to Arduino IDE → Sketch → Include Library → Manage Libraries
Search and install:
MFRC522
SPI
Servo
2. Upload Code
Open code.ino
Add authorized UIDs
Upload to Arduino

# 📂 Folder Structure
RFID-based-door-locking-system-using-Arduino/
│── README.md
│── code.ino
│── project.jpg
│── demo.mp4
│── circuit.png
│── LICENSE

# 🧪 Testing

Place RFID card near RC522.

Green LED + Servo movement → Access granted

Red LED/Buzzer → Access denied
