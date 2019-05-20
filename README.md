# Citizen-Scientist-Water-Management-Project

Measuring the Quality and Quantity of water and use LoRaWAN protocol to see real time data and make predictions on flood warning.

The Aim of this exercise is to get familiarize with the water control and management sensors and how anyone can receive and visualize the data in real time.

Monitoring of water quality and quantity is essential in efficient management of the surface and ground water resources to maximize reliability for users in an efficient, effective, safe and financially responsible manner. To monitor these resources, one requires large amount of information and data. The monitoring involves a combination of automatic digital sensors and logging devices as well as manual sampling and analysis.

# Table of Content
* [Content of your Kit](https://github.com/Bilal-Arshad/Citizen-Scientist-Water-Management-Project/blob/master/README.md#content-of-your-kit)
* [Programming with Seeeduino](https://github.com/Bilal-Arshad/Citizen-Scientist-Water-Management-Project/blob/master/README.md#programming-with-seeeduino)
* [Quick Start](https://github.com/Bilal-Arshad/Citizen-Scientist-Water-Management-Project#quick-start)
  * [Open the Blink Example](https://github.com/Bilal-Arshad/Citizen-Scientist-Water-Management-Project/blob/master/README.md#quick-start)
  * [Upload the Program](https://github.com/Bilal-Arshad/Citizen-Scientist-Water-Management-Project/blob/master/README.md#open-the-blink-example)
* [Quick start with Waterproof Ultrasonic Sensor](https://github.com/Bilal-Arshad/Citizen-Scientist-Water-Management-Project/blob/master/README.md#quick-start-with-waterproof-ultrasonic-sensor)
  * [Experiment :- Find the level of water in the container](https://github.com/Bilal-Arshad/Citizen-Scientist-Water-Management-Project#experiment---find-the-level-of-water-in-the-container)
  * [Try Different Application for Ultrasonic Sensor](https://github.com/Bilal-Arshad/Citizen-Scientist-Water-Management-Project#try-different-application-for-ultrasonic-sensor)
  * [Applications](https://github.com/Bilal-Arshad/Citizen-Scientist-Water-Management-Project#applications)
* [Quick start with Waterproof Digital Temperature Sensor](https://github.com/Bilal-Arshad/Citizen-Scientist-Water-Management-Project#quick-start-with-waterproof-digital-temperature-sensor)
  * [Experiment :- Find the Temperature of water in the container/Cup](https://github.com/Bilal-Arshad/Citizen-Scientist-Water-Management-Project#experiment---find-the-temperature-of-water-in-the-containercup)
* [Quick start with Turbidity Sensor](https://github.com/Bilal-Arshad/Citizen-Scientist-Water-Management-Project#quick-start-with-turbidity-sensor)
  * [Experiment :- Find the Turbidity of Water](https://github.com/Bilal-Arshad/Citizen-Scientist-Water-Management-Project#experiment---find-the-turbidity-of-water)


## Content of your Kit:

* Seeeduino LoRaWAN : [Documentation](http://wiki.seeedstudio.com/Seeeduino_LoRAWAN/)
* Turbidity Sensor : [Documentation](https://wiki.dfrobot.com/Turbidity_sensor_SKU__SEN0189)
* Waterproof Ultrasonic Sensor : [Documentation](https://wiki.dfrobot.com/Weather_-_proof_Ultrasonic_Sensor_with_Separate_Probe_SKU___SEN0208)
* Waterproof Digital Temperature Sensor : [Documentation](https://wiki.dfrobot.com/Waterproof_DS18B20_Digital_Temperature_Sensor__SKU_DFR0198_)
* Breadboard : [Documentation](https://www.sciencebuddies.org/science-fair-projects/references/how-to-use-a-breadboard)
* Wires
* USB Cable

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

![](https://github.com/Bilal-Arshad/Citizen-Scientist-Water-Management-Project/blob/master/img/Getting_Started1.png)

#### Upload the Program
* Now, simply click the "Upload" button in the Arduino IDE environment. Wait for few seconds - you should see the RX and TX leds on the board flashing ( it means the code is uploading on the microcontroller). If the upload is successul, the message "Done uploading" will appear in the status bar.

![](https://github.com/Bilal-Arshad/Citizen-Scientist-Water-Management-Project/blob/master/img/Getting_Started2.png)

## Quick start with Waterproof Ultrasonic Sensor
* Plug ultrasonic sensor to your Seeeduino board by following this tutorial : [Understanding Ultrasonic Sensor](https://wiki.dfrobot.com/Weather_-_proof_Ultrasonic_Sensor_with_Separate_Probe_SKU___SEN0208)
* Copy the [Sample Code](https://github.com/Bilal-Arshad/Citizen-Scientist-Water-Management-Project/blob/master/Code%20for%20Sensors/Water%20level%20estimation%20(Ultrasonic%20sensor)) and paste into your Arduino IDE and [upload](https://github.com/Bilal-Arshad/Citizen-Scientist-Water-Management-Project#upload-the-program)
* Open the serial Monitor on your Adruino IDE

![](https://github.com/Bilal-Arshad/Citizen-Scientist-Water-Management-Project/blob/master/img/Getting_Started4.png)

* Move your sensor up and down your table and see variation in the distance on your serial Monitor.

### Experiment :- Find the level of water in the container
* Adjust or hold your Ultrasonic Sensor at any position looking down on your desk.
* Find the Container and fill it with water, see the output in cm's on your serial monitor.
* Note down the stable reading in your worksheet.
* Throw half of the water and test it again, making sure Ultrasonic sensor hasn't moved since last test.
* Note down the stable reading in your worksheet.
* Compare both reading and find the difference between them.
* The difference between them is the water loss in cm.
* Keep the water in the container for next Experiment

### Try Different Application for Ultrasonic Sensor

![](https://github.com/Bilal-Arshad/Citizen-Scientist-Water-Management-Project/blob/master/img/Getting_Started5.png)
* this image is retrieved from https://www.alibaba.com/product-detail/digital-ultrasonic-level-meter-with-reasonable_2004064037.html
### Applications
* Water tank level measurement
* Fuel tank level measurement
* Food tank level measurement
* Seal water level measurement
* Powder and Solid level application
* Sewage and industry wastewater treatment
* Oil and Fuel level measurement
* Hazardous zone level measurement
* Oil tanker, small fuel tank level measurement
* Other distance and level application

## Quick start with Waterproof Digital Temperature Sensor
* Plug Digital Temperature Sensor to your Seeeduino board following this tutorial : [Understanding Temperature Sensor](https://wiki.dfrobot.com/Waterproof_DS18B20_Digital_Temperature_Sensor__SKU_DFR0198_)
* Copy the [Sample Code](https://github.com/Bilal-Arshad/Citizen-Scientist-Water-Management-Project/blob/master/Code%20for%20Sensors/Measuring%20Temperature%20of%20Water) and paste into your Arduino IDE and [upload](https://github.com/Bilal-Arshad/Citizen-Scientist-Water-Management-Project#upload-the-program)

### Experiment :- Find the Temperature of water in the container/Cup
* Temperature testing is the process of measuring temperature levels in water. Temperature is a key factor in water chemistry. Temperature affects the dissolved oxygen levels in water, the rate of photosynthesis, metabolic rates of organisms, etc. Aquatic organisms depend on particular temperature ranges for their health. Each species of organism thrives in a specific temperature range, and many animals use temperature as a signal for when to reproduce and when to migrate.
* Find the application from Ultrasonic sensor Section and adopt that application to temperature sensor.

![](https://github.com/Bilal-Arshad/Citizen-Scientist-Water-Management-Project/blob/master/img/Getting_Started7.jpg)

## Quick start with Turbidity Sensor
* Plug ultrasonic sensor to your Seeeduino board by following this tutorial : [Understanding Turidity Sensor](https://wiki.dfrobot.com/Turbidity_sensor_SKU__SEN0189)
* Copy the [Sample Code](https://github.com/Bilal-Arshad/Citizen-Scientist-Water-Management-Project/blob/master/Code%20for%20Sensors/Measuring%20Turbidity%20in%20Water) and paste into your Arduino IDE and [upload](https://github.com/Bilal-Arshad/Citizen-Scientist-Water-Management-Project#upload-the-program)


### Experiment :- Find the Turbidity of Water
* Turbidity is a measure of the degree to which the water loses its transparency due to the presence of suspended particulates. The more total suspended solids in the water, the murkier it seems and the higher the turbidiy.
* Take 2 * Cups, fill one cup with clean water and the other cup with dirty water (to make water dity, you can choose to mix soil in the water).
* Read Documentation of the sensor, and dipp your sensor in the clean water, Record stable reading in your notebook.
* Now dipp the sensor in dirty water, Record stable reading in your notebook.
* Compare both recordings and explain those readings to your teacher.

![](https://github.com/Bilal-Arshad/Citizen-Scientist-Water-Management-Project/blob/master/img/Getting_Started8.jpg)

