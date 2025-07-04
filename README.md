# Smart-Medicine-Vending-System-Bridging-Gaps-in-Medicine-Access-and-Dispensing-Accountability
The Smart Medicine Vending System is an automated machine that dispenses medicines based on user input, using Python (Tkinter), Arduino, and Google Sheets for real-time control, user interaction, and inventory tracking.
**Overview**
An automated medicine dispensing solution that combines RFID authentication with precise servo-controlled dispensing and real-time cloud synchronization.

**Features**
1. RFID Patient Authentication: Secure login using programmed RFID cards
2. Automated Dispensing: 4-slot servo-controlled mechanism with stepper motor positioning
3. Cloud Integration: Real-time data logging to Google Sheets
4. User-Friendly Interface: Tkinter-based GUI for staff control
5. Comprehensive Logging: Full transaction history and inventory tracking
   
**Hardware Requirements**
Arduino Uno
RFID-RC522 module
4x SG90 servo motors (continuous rotation)
2x NEMA 17 stepper motors with drivers
2x limit switches
3D-printed dispensing mechanism

**Software Requirements**
Python 3.8+
Arduino IDE
Google Sheets API access

**Installation**
**Arduino Setup**
1. Upload the firmware from arduino/medical_vending.ino
2. Install required libraries:
arduino-cli lib install "MFRC522" "Servo"
**Python Setup**
git clone https://github.com/your-repo/smart-medical-vending.git
cd python
pip install -r requirements.txt
**Configuration**
1. Update patient RFID UIDs in arduino/medical_vending.ino
2. Place Google Sheets API credentials as credentials.json in the python folder
3. Adjust settings in config.json:
{
  "arduino_port": "COM4",
  "servo_rotation_time": 1000,
  "spreadsheet_id": "your-sheet-id"
}

**Usage**
Power on the Arduino and run python main.py
Patients scan their RFID card
Staff select medication from the GUI
System automatically dispenses and logs transaction

**Troubleshooting**
Servos not rotating: Verify pulse width settings
RFID not detecting cards: Check wiring (3.3V power)
Google Sheets sync issues: Reauthenticate service account

**Development Team**
DHARSHINI B
HARIKUMAARAN R
SURYA KUMAR M
SHRUTHI S
DIVYA DHARSHINI G
