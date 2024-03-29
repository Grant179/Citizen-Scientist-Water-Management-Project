# Citizen-Scientist-Water-Management-Project

Measuring the Quality and Quantity of water and use LoRaWAN protocol to see real time data and make predictions on flood warning.

The Aim of this exercise is to get familiarize with the water control and management sensors and how anyone can receive and visualize the data in real time.

Monitoring of water quality and quantity is essential in efficient management of the surface and ground water resources to maximize reliability for users in an efficient, effective, safe and financially responsible manner. To monitor these resources, one requires large amount of information and data. The monitoring involves a combination of automatic digital sensors and logging devices as well as manual sampling and analysis.

# Table of Content
* [Content of your Kit](https://github.com/Bilal-Arshad/Citizen-Scientist-Water-Management-Project/blob/master/README.md#content-of-your-kit)
* [Know Your Seeeduino Board](https://github.com/Bilal-Arshad/Citizen-Scientist-Water-Management-Project/blob/master/Basic_Introduction_to_software_and_hardware.md#know-your-hardware)
* [Programming with Seeeduino](https://github.com/Bilal-Arshad/Citizen-Scientist-Water-Management-Project/blob/master/README.md#programming-with-seeeduino)
* [Quick Start](https://github.com/Bilal-Arshad/Citizen-Scientist-Water-Management-Project#quick-start)
  * [Open the Blink Example](https://github.com/Bilal-Arshad/Citizen-Scientist-Water-Management-Project/blob/master/README.md#quick-start)
  * [Upload the Program](https://github.com/Bilal-Arshad/Citizen-Scientist-Water-Management-Project/blob/master/README.md#open-the-blink-example)
  * [Result](https://github.com/Bilal-Arshad/Citizen-Scientist-Water-Management-Project/blob/master/Basic_Introduction_to_software_and_hardware.md#result)

## Content of your Kit:

* Seeeduino LoRaWAN : [Documentation](http://wiki.seeedstudio.com/Seeeduino_LoRAWAN/)
* Turbidity Sensor : [Documentation](https://wiki.dfrobot.com/Turbidity_sensor_SKU__SEN0189)
* Waterproof Ultrasonic Sensor : [Documentation](https://wiki.dfrobot.com/Weather_-_proof_Ultrasonic_Sensor_with_Separate_Probe_SKU___SEN0208)
* Waterproof Digital Temperature Sensor : [Documentation](https://wiki.dfrobot.com/Waterproof_DS18B20_Digital_Temperature_Sensor__SKU_DFR0198_)
* Breadboard : [Documentation](https://www.sciencebuddies.org/science-fair-projects/references/how-to-use-a-breadboard)
* Wires
* USB Cable


## Know Your Seeeduino Board

![](https://github.com/Bilal-Arshad/Citizen-Scientist-Water-Management-Project/blob/master/img/6.PNG)

1. Micro USB - Programming and supply power to the board
2. Grove connectors
3. JST2.0 Lipo battery input (3.7V) and charge status led
4. DFU Button - Firmware mode button
5. Reset Button
6. Arduino Pinout
7. ICSP pins
8. Firmware mode led
9. Wire antenna
A. uFL antenna
B. RF module - RHF76-052AM
C. ARM Cortex M0 processor - ATSAMD21G18
D. LEDs
* RX/TX - blink when data on UART(from/to USB)
* L - an led connect to D13
* PWR - power
* To get More informatin on Hardware please see [Source Reference](http://wiki.seeedstudio.com/Seeeduino_LoRAWAN/)  

## Programming with Seeeduino
* Get and install the Arduino IDE:  https://www.arduino.cc/en/main/software
* Launch the Arduino IDE
* Under File -> Preferences -> Additional Boards Manager URLs -> paste this link -> https://raw.githubusercontent.com/Seeed-Studio/Seeed_Platform/master/package_seeeduino_boards_index.json and validate
* Add the Seeeduino LoRaWAN to Arduino IDE: Tools -> Board -> Boards manager -> search for Seeed SAMD Boards -> install the latest version.
* Select the board: Tools -> Board -> Seeeduino LoRaWAN
* Select the port: Tools -> Port -> Click on the port that Seeeduino LoRaWAN is attached.

### Quick Start
* Launch the Arduino IDE on your computer
* Connect the Seeeduino board to your computer using the USB cable. The green power LED (labeled PWR) should go on. (When Seeeduino works independently, you can select USB or power adapter to power for Seeeduino.)
* Select the board and port as descibed above in Programming with Seeeduino Section.
#### Open the Blink Example
* We are going to develop very simple program of blinking light
* Open the LED blink example sketch: File>Examples>01.Basics>Blink.

![](https://github.com/Bilal-Arshad/Citizen-Scientist-Water-Management-Project/blob/master/img/1.PNG)

#### Upload the Program
* Now, simply click the "Upload" button in the Arduino IDE environment. Wait for few seconds - you should see the RX and TX leds on the board flashing ( it means the code is uploading on the microcontroller). If the upload is successul, the message "Done uploading" will appear in the status bar.

![](https://github.com/Bilal-Arshad/Citizen-Scientist-Water-Management-Project/blob/master/img/7.PNG)

#### Result
* A few seconds after the upload finishes, you should see the pin 13 (L) LED on the board start to blink (in Yellow). if it does, congratulations! You've gotten Seeeduino up-and-running.



