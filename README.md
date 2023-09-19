# CAIxIEEE-TinyML-Workshop
All the relevant links and such

# Software setup (Arduino)

- Step 1. Download and Install the latest version of Arduino IDE according to your operating system

  https://www.arduino.cc/en/software

- Step 2. Launch the Arduino application

  “Arduino IDE”

- Step 3. Add Seeed Studio XIAO nRF52840 (Sense) board package to your Arduino IDE
- Navigate to File > Preferences, and fill "Additional Boards Manager URLs" with the url below:
  https://files.seeedstudio.com/arduino/package_seeeduino_boards_index.json
- (On macOS): Navigate to Arduino IDE > Settings… > and fill “Additional Boards Manager URLs" with the URL below
  https://files.seeedstudio.com/arduino/package_seeeduino_boards_index.json

  <img  src="./images/Arduino_step3.png">

----

- Step 4: Navigate to Tools > Board > Boards Manager..., type the keyword "seeed nrf52" in the search box, select the latest version of the board you want, and install it. (Install Both)
We NEED Seeed nRF52 mbed-enabled Boards installed to work the classifier

<img  src="./images/Arduino_step4.png">

----

- Step 5. Select your board and port
Board: After installing the board package, navigate to Tools > Board and choose the board you want, continue to select "Seeed XIAO nRF52840 Sense". Now we have finished setting up the Seeed Studio XIAO nRF52840 (Sense) for Arduino IDE

<img  src="./images/Arduino_step5.png">

- Port: Navigate to Tools > Port and select the serial port name of the connected Seeed Studio XIAO nRF52840 (Sense). 
- This is something like COM3 or higher for Windows and /dev/… for Mac
  - Note: For me (macOS) it’s:  /dev/cu. usbmodem101 (Seeed XIAO BLE - nRF52840, Seeed XIAO BLE Sense - nRF52840)
<img  src="./images/Arduino_step6.png">
- Board and Port are now setup correctly!
---

# Software setup (Tensorflow and Machine Learning Model)
- Step 1. Download [Seeed_Arduino_LSM6DS3](Seeed_Arduino_LSM6DS3-master.zip) library as a zip file
Note: Make sure you download both in a Folder you have direct/easy access to
- Step 2. Open Arduino IDE, navigate to Sketch > Include Library > Add .ZIP Library... and open both the downloaded zip files one after the other
