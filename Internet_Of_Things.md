

# Table of Content
* [Connecting your sensors with Internet of things and controll your sensors remotely](https://github.com/Bilal-Arshad/Citizen-Scientist-Water-Management-Project/blob/master/Internet_Of_Things.md#connecting-your-sensors-with-internet-of-things-and-controll-your-sensors-remotely)
  * [Adapt & Run Code](https://github.com/Bilal-Arshad/Citizen-Scientist-Water-Management-Project/blob/master/Internet_Of_Things.md#adapt--run-code)
* [Visualize your Data on Dashboard using Cayenne LPP](https://github.com/Bilal-Arshad/Citizen-Scientist-Water-Management-Project/blob/master/Internet_Of_Things.md#visualize-your-data-on-dashboard-using-cayenne-lpp)
  * [Sign up with My Devices](https://github.com/Bilal-Arshad/Citizen-Scientist-Water-Management-Project/blob/master/Internet_Of_Things.md#sign-up-with-my-devices)
  * [Modification of Setting device with LoRa code](https://github.com/Bilal-Arshad/Citizen-Scientist-Water-Management-Project/blob/master/Internet_Of_Things.md#modification-of-setting-device-with-lora-code)
  * [Test your ultrasonic sensor on Cayenne LPP](https://github.com/Bilal-Arshad/Citizen-Scientist-Water-Management-Project/blob/master/Internet_Of_Things.md#test-your-ultrasonic-sensor-on-cayenne-lpp)


## Connecting your sensors with Internet of things and controll your sensors remotely
* Making your sensors to speak with internet, and by the end of this tutorial you should be able to visualize data at your home for the sensor plugged at your school.
* First create an account, then create an application and then register your device.
 * Go to [The Things Network](https://www.thethingsnetwork.org/) and register an account.
 * Go to [Console](https://console.thethingsnetwork.org/) and select “Application”.
 * On the next screen click “+add application”
 * In the next screen pick a meaning full name for your application in lowercase letters for Application ID and write something in description. Under Handler Registration pick an option available. See image below
 
 ![](https://github.com/Bilal-Arshad/Citizen-Scientist-Water-Management-Project/blob/master/img/Getting_Started9.png)
 
 * On the next screen click “register device”
 * For “Device ID” pick a meaningful name in lowercase letters
 * On the left side of the DevEUI field click on the arrow icons. The icon changes into a pen and this will cause the ID to be generated. This is necessary since the API doesn’t offer a way to read out the devices MAC address. See image below
 * In App EUI pick the ID of the application we created earlier
 
 ![](https://github.com/Bilal-Arshad/Citizen-Scientist-Water-Management-Project/blob/master/img/Getting_Started10.png)
 
### Adapt & Run Code 
 
 * Now Make sure your Seeeduino LoRaWAN is connected with your computer.
 * Copy and paste this [Code](https://github.com/Bilal-Arshad/Citizen-Scientist-Water-Management-Project/blob/master/Code%20for%20Sensors/Setting%20device%20with%20LoRa) on your Arduino IDE and follow all of the comments and make adjustments to code according to your device configuration on The Things Network platform.
 * After running your code, you should see something like this in your serial monitor.
 
 ![](https://github.com/Bilal-Arshad/Citizen-Scientist-Water-Management-Project/blob/master/img/Getting_Started11.PNG)
 
 * Now to collect data, navigate to The Things Network website, select application 
 * Click on the Application that you have created -> navigate to Data option and click -> under Data you would see that you are receiving data from your Seeeduino Microcontroller.
 * Stay on this page for next part.
 
## Visualize your Data on Dashboard using Cayenne LPP

* Now we would like to create a User friendly interface, which can receive data and display that data nicely on dashboard.
* This dashboard will be receiving real time data, as longer your sensor is connected with LoRaWAN internet protocol.
* On The Things Network Console, navigate to Integrations -> add integration -> find myDevices and select this option.
* After selecting myDevices, you need to write process ID for your device, it can be any unique text, see below in image.

![](https://github.com/Bilal-Arshad/Citizen-Scientist-Water-Management-Project/blob/master/img/Getting_Started12.PNG)

* Select Add Integration.

![](https://github.com/Bilal-Arshad/Citizen-Scientist-Water-Management-Project/blob/master/img/Getting_Started13.PNG)

### Sign up with My Devices
* To start using dashboard, you have to make an account on myDevices.
* To make an account, please click this [link](https://accounts.mydevices.com/auth/realms/cayenne/protocol/openid-connect/auth?response_type=code&scope=email+profile&client_id=cayenne-web-app&state=UYSHaX9t9bmcWWSkiXvvsdtfiN4IhWCfORtEGJfq&redirect_uri=https%3A%2F%2Fcayenne.mydevices.com%2Fauth%2Fcallback)
* Fill out the details and sign in

![](https://github.com/Bilal-Arshad/Citizen-Scientist-Water-Management-Project/blob/master/img/Getting_Started14.PNG)

* Log-in and click on LoRa

![](https://github.com/Bilal-Arshad/Citizen-Scientist-Water-Management-Project/blob/master/img/Getting_Started15.png)

* Select The Things Network at the bottom of the left menu bar, click on Cayenne LPP and fill in your DevEUI of your device, which you can find in the [Console](https://console.thethingsnetwork.org/applications)

![](https://github.com/Bilal-Arshad/Citizen-Scientist-Water-Management-Project/blob/master/img/Getting_Started16.png)

### Modification of Setting device with LoRa code
* In this section we will modify code that we wrote before for connecting sensor with The Things Network Platform, to satisfy requirements for visualization of data on dashboard.
* First Step : Include Cayenne LPP library in your Arduino IDE, Go to Arduino IDE -> Sketch -> Include Library -> Manage Libraries -> Search for CayenneLPP -> click install
* Second Step : Restart Arduino
* Third Step : Copy and past this [code]() into your Arduino IDE
* Fourth Step : Compare and explain difference between both algorithms.
Hint these lines are extras; (#include <CayenneLPP.h> , CayenneLPP lpp(51); , lpp.reset(); ,  lpp.addTemperature(1, value); , lora.transferPacket(lpp.getBuffer(), lpp.getSize())

### Test your ultrasonic sensor on Cayenne LPP
* In this section we will use our previous knowledge, and add code of ultrasonic sensor to Setting device with LoRa, and run as one algorithm. By doing this, we will be sending ultrasonic sensor data to dashboard.
* Copy and Paste this [code](https://github.com/Bilal-Arshad/Citizen-Scientist-Water-Management-Project/blob/master/Code%20for%20Sensors/Ultrasonic_sensor%2BCayenneLPP) into your Arduino IDE.
* Connect the Ultrasonic Sensor and navigate to myDevices platform, and visualize your sensor output.
