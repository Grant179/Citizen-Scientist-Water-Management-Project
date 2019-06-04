
# Table of Content

* [Quick start with Waterproof Ultrasonic Sensor](https://github.com/Bilal-Arshad/Citizen-Scientist-Water-Management-Project/blob/master/README.md#quick-start-with-waterproof-ultrasonic-sensor)
  * [Working principle of Ultrasonic Sensor]()
  * [Experiment :- Find the level of water in the container](https://github.com/Bilal-Arshad/Citizen-Scientist-Water-Management-Project#experiment---find-the-level-of-water-in-the-container)
  * [Try Different Application for Ultrasonic Sensor](https://github.com/Bilal-Arshad/Citizen-Scientist-Water-Management-Project#try-different-application-for-ultrasonic-sensor)
  * [Applications](https://github.com/Bilal-Arshad/Citizen-Scientist-Water-Management-Project#applications)
* [Quick start with Waterproof Digital Temperature Sensor](https://github.com/Bilal-Arshad/Citizen-Scientist-Water-Management-Project#quick-start-with-waterproof-digital-temperature-sensor)
  * [Working principle of Waterproof Digital Temperature Sensor]()
  * [Experiment :- Find the Temperature of water in the container/Cup](https://github.com/Bilal-Arshad/Citizen-Scientist-Water-Management-Project#experiment---find-the-temperature-of-water-in-the-containercup)
* [Quick start with Turbidity Sensor](https://github.com/Bilal-Arshad/Citizen-Scientist-Water-Management-Project#quick-start-with-turbidity-sensor)
  * [Working principle of Waterproof Digital Temperature Sensor]()
  * [Experiment :- Find the Turbidity of Water](https://github.com/Bilal-Arshad/Citizen-Scientist-Water-Management-Project#experiment---find-the-turbidity-of-water)
  

## Quick start with Waterproof Ultrasonic Sensor
* Plug ultrasonic sensor to your Seeeduino board by following this tutorial : [Understanding Ultrasonic Sensor](https://wiki.dfrobot.com/Weather_-_proof_Ultrasonic_Sensor_with_Separate_Probe_SKU___SEN0208)
* Copy the [Sample Code](https://github.com/Bilal-Arshad/Citizen-Scientist-Water-Management-Project/blob/master/Code%20for%20Sensors/Water%20level%20estimation%20(Ultrasonic%20sensor)) and paste into your Arduino IDE and upload
* Open the serial Monitor on your Adruino IDE

![](https://github.com/Bilal-Arshad/Citizen-Scientist-Water-Management-Project/blob/master/img/Getting_Started4.png)

* Move your sensor up and down your table and see variation in the distance on your serial Monitor.


### Working principle of Ultrasonic Sensor

* The sensor transmits a pulse at time 0, that pulse gets reflected by an object. The sensor receives the signal and converts it to an electric signal. The next pulse can be transmitted when there is no echo. The time period is called cycle period. If a 10 microseconds width trigger pulse is sent to the signal pin, the ultrasonic module will output 8 * 40KHz ultrasonic signals and detect the echo back. The width of received echo is proportional to distance between object and ultrasnoic sensor. The distance can be calculated by using following formula:

![](https://github.com/Bilal-Arshad/Citizen-Scientist-Water-Management-Project/blob/master/img/formula.PNG)  


### Experiment :- Find the level of water in the container
1. Adjust or hold your Ultrasonic Sensor at any position looking down on your desk.
2. Find the Container and fill it with water, see the output in cm's on your serial monitor.
3. Note down the stable reading in your worksheet.
4. Throw half of the water and test it again, making sure Ultrasonic sensor hasn't moved since last test.
5. Note down the stable reading in your worksheet.
6. Compare both reading and find the difference between them.
7. The difference between them is the water loss in cm.
8. Keep the water in the container for next Experiment

### Try Different Application for Ultrasonic Sensor

![](https://github.com/Bilal-Arshad/Citizen-Scientist-Water-Management-Project/blob/master/img/Getting_Started5.png)

[Reference Source of an Image](https://www.alibaba.com/product-detail/digital-ultrasonic-level-meter-with-reasonable_2004064037.html)

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
* Install the OneWire library to your arduino IDE: Sketch -> Include Library -> Manage Libraries -> search for MAX31850 OneWire library -> install the latest version -> close the window.
* Restart the Arduino IDE.
* Copy the [Sample Code](https://github.com/Bilal-Arshad/Citizen-Scientist-Water-Management-Project/blob/master/Code%20for%20Sensors/Measuring%20Temperature%20of%20Water) and paste into your Arduino IDE and upload


### Working principle of Waterproof Digital Temperature Sensor

* The 1-Wire interface Temperatuer Sensor requires only one port for communication and needs no other external components to work. Thermometer resolution is programmed from 9 - 12 bits and it converts 12-bit temperature to digital word in less than 750ms.

### Experiment :- Find the Temperature of water in the container/Cup
* Temperature testing is the process of measuring temperature levels in water. Temperature is a key factor in water chemistry. Temperature affects the dissolved oxygen levels in water, the rate of photosynthesis, metabolic rates of organisms, etc. Aquatic organisms depend on particular temperature ranges for their health. Each species of organism thrives in a specific temperature range, and many animals use temperature as a signal for when to reproduce and when to migrate.
* Find the application from Ultrasonic sensor Section and adopt that application to temperature sensor.

![](https://github.com/Bilal-Arshad/Citizen-Scientist-Water-Management-Project/blob/master/img/8.PNG)

## Quick start with Turbidity Sensor
* Plug ultrasonic sensor to your Seeeduino board by following this tutorial : [Understanding Turidity Sensor](https://wiki.dfrobot.com/Turbidity_sensor_SKU__SEN0189)
* Copy the [Sample Code](https://github.com/Bilal-Arshad/Citizen-Scientist-Water-Management-Project/blob/master/Code%20for%20Sensors/Measuring%20Turbidity%20in%20Water) and paste into your Arduino IDE and upload
* Note Important -> Connect Turbidity sensor with 3.3V instead of 5V on your Seeeduino Board, to obtain accurate results.

### Working principle of Waterproof Digital Temperature Sensor

* The turbidity sensor uses light to detect suspended particles in water by measuring the light transmittance and scattering rate, which changes with the amount of total suspended solids (TSS) in water. As the TSS increases, the liquid turbidity level increases.
* Understanding Output of Sensor -> The output value will decrease when in liquids with a high turbidity.

### Experiment :- Find the Turbidity of Water
* Turbidity is a measure of the degree to which the water loses its transparency due to the presence of suspended particulates. The more total suspended solids in the water, the murkier it seems and the higher the turbidiy.
* Take 2 * Cups, fill one cup with clean water and the other cup with dirty water (to make water dity, you can choose to mix soil in the water).
* Read Documentation of the sensor, and sink your sensor in the clean water, Record stable reading in your notebook.
* Now sink the sensor in dirty water, Record stable reading in your notebook.
* Compare both recordings and explain those readings to your teacher.

![](https://github.com/Bilal-Arshad/Citizen-Scientist-Water-Management-Project/blob/master/img/3.jpg)
[Reference Source of an Image](https://engineering.ubc.ca/spotlight/research/customized-and-community-driven-clean-water-solutions)
