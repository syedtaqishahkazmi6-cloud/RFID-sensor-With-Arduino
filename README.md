Project: RFID Task Trigger System

This project uses an MFRC522 RFID module and an Arduino Nano to read unique card IDs and execute specific software or hardware tasks based on which tag is scanned.

**Hardware Requirements**

* Arduino Nano
* MFRC522 RFID Reader
* RFID Tags/Cards (13.56 MHz)  
* Jumper Wires

Wiring Diagram

⚠️ CRITICAL: The MFRC522 operates at 3.3V. Connecting it to the 5V pin on the Arduino Nano may permanently damage the sensor.

MFRC522 Pin	Arduino Nano Pin	Note

VCC	3.3V	

Power (Do NOT use 5V)  



RST	D9	

Reset pin (configurable)  



GND	GND	

Ground  



IRQ	Unused	

Leave disconnected  



MISO	D12	

SPI Master In Slave Out  



MOSI	D11	

SPI Master Out Slave In  



SCK	D13	

SPI Serial Clock

SDA (SS)	D10	

Signal Select (configurable)

Software Installation

To run this project, you must install the MFRC522 library:  



Open the Arduino IDE.  



Navigate to Sketch > Include Library > Manage Libraries...



&#x20; 



Search for "MFRC522".  



Install the version maintained by GitHubCommunity.



How to Use

Identify UIDs: Upload the example code below and open the Serial Monitor (set to 9600 Baud).  



Scan Tags: Scan your RFID cards one by one. The Serial Monitor will display the UID (e.g., 33 5A 72 1B).  



Assign Actions: Replace the placeholder UIDs in the if statements with your actual card IDs to trigger custom functions.

