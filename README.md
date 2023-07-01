# esp8266wemos_rfidrc522
Connecting ESP8266 wemos china to rfid-rc522

## Requirements
You have to install Arduino IDE 1.6.10 or later. Links are listed below.
* **Arduino** > **Preferences** > "Additional Boards Manager URLs:" and add: **http://arduino.esp8266.com/stable/package_esp8266com_index.json**
* **Arduino** > **Tools** > **Board** > **Boards Manager** > type in **ESP8266** and install the board
* Download MFRC522 library and extract to Arduino library folder or you can use "Library Manager" on the IDE itself to install the MFRC522 library.

### Download Links
* [Arduino IDE](https://www.arduino.cc/en/Main/Software) - The development IDE
* [ESP8266 Core for Arduino IDE](https://github.com/esp8266/Arduino) - ESP8266 Core
* [MFRC522 Library](https://github.com/miguelbalboa/rfid) - MFRC522 RFID Library

## Simple Example

### Wiring RFID RC522 module
The following table shows the typical pin layout used:

| Signal        | MFRC522       |Wemos D1 Wifi Uno | WeMos D1 mini  | NodeMcu | Generic      |
|---------------|:-------------:|:----------------:|:--------------:| :------:|:------------:|
| RST/Reset     | RST           | D [1]           | D3 [1]         | D3 [1]  | GPIO-0 [1]   |
| SPI SS        | SDA [3]       | D [1]           | D8 [2]         | D8 [2]  | GPIO-15 [2]  |
| SPI MOSI      | MOSI          | D [1]           | D7             | D7      | GPIO-13      |
| SPI MISO      | MISO          | D [1]           | D6             | D6      | GPIO-12      |
| SPI SCK       | SCK           | D [1]           | D5             | D5      | GPIO-14      |
