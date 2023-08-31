# SM23-IOT-03

Smart methods 2023 summer training (Internet of things task 3)

Data Collection and Transmission with DHT22 Sensor (for temperature and humidity) by using a Wi-Fi network with esp 32

# ESP32 DHT11/DHT22 Web Server – Temperature and Humidity

In this project, you’ll learn how to build an asynchronous ESP32 web server with the DHT11 or DHT22 that displays temperature and humidity using Arduino IDE.

ESP32 DHT11/DHT22 Web Server - Temperature and Humidity using Arduino IDE
The web server we’ll build updates the readings automatically without the need to refresh the web page.

# With this project you’ll learn:

How to read temperature and humidity from DHT sensors;
Build an asynchronous web server using the ESPAsyncWebServer library;
Update the sensor readings automatically without the need to refresh the web page.
For a more in-depth explanation on how to use the DHT22 and DHT11 temperature and humidity sensors with the ESP32, read our complete guide: ESP32 with DHT11/DHT22 Temperature and Humidity Sensor using Arduino IDE

# Asynchronous Web Server
To build the web server we’ll use the ESPAsyncWebServer library that provides an easy way to build an asynchronous web server. Building an asynchronous web server has several advantages as mentioned in the library GitHub page, such as:

“Handle more than one connection at the same time”;
“When you send the response, you are immediately ready to handle other connections while the server is taking care of sending the response in the background”;
“Simple template processing engine to handle templates”;
And much more.
Take a look at the library documentation on its GitHub page.

Parts Required
ESP32 DHT11 DHT22 Temperature and Humidity Arduino IDE Circuit Schematic

# To complete this tutorial you need the following parts:

ESP32 development board (read ESP32 development boards comparison)
DHT22 or DHT11 Temperature and Humidity Sensor
4.7k Ohm Resistor
Breadboard
Jumper wires
You can use the preceding links or go directly to MakerAdvisor.com/tools to find all the parts for your projects at the best price!

Note: if you’re using a module with a DHT sensor, it normally comes with only three pins. The pins should be labeled so that you know how to wire them. Additionally, many of these modules already come with an internal pull up resistor, so you don’t need to add one to the circuit.

# Installing Libraries
You need to install a couple of libraries for this project:

The DHT and the Adafruit Unified Sensor Driver libraries to read from the DHT sensor.
ESPAsyncWebServer and Async TCP libraries to build the asynchronous web server.
Follow the next instructions to install those libraries:

# Installing the DHT Sensor Library

To read from the DHT sensor using Arduino IDE, you need to install the DHT sensor library. Follow the next steps to install the library.

+ first we have to download the DHT Sensor library. 

+ seconed You should have a .zip folder in your Downloads folder
Unzip the .zip folder and you should get DHT-sensor-library-master folder
T+ Third: Rename your folder from DHT-sensor-library-master to DHT_sensor
Move the DHT_sensor folder to your Arduino IDE installation libraries folder

+ Finally, re-open your Arduino IDE
Installing the Adafruit Unified Sensor Driver

# install the Adafruit Unified Sensor Driver library to work with the DHT sensor. Follow the next steps to install the library.

first Download the Adafruit Unified Sensor library. You should have a .zip folder in your Downloads folder
Unzip the .zip folder and you should get Adafruit_sensor-master folder
Rename your folder from Adafruit_sensor-master to Adafruit_sensor
Move the Adafruit_sensor folder to your Arduino IDE installation libraries folder
Finally, re-open your Arduino IDE

# Installing the ESPAsyncWebServer library

Follow the next steps to install the ESPAsyncWebServer library:

Download the ESPAsyncWebServer library. You should have a .zip folder in your Downloads folder
Unzip the .zip folder and you should get ESPAsyncWebServer-master folder
Rename your folder from ESPAsyncWebServer-master to ESPAsyncWebServer
Move the ESPAsyncWebServer folder to your Arduino IDE installation libraries folder
Installing the Async TCP Library for ESP32

# The ESPAsyncWebServer library requires the AsyncTCP library to work. Follow the next steps to install that library:

Download the AsyncTCP library. You should have a .zip folder in your Downloads folder
Unzip the .zip folder and you should get AsyncTCP-master folder
Rename your folder from AsyncTCP-master to AsyncTCP
Move the AsyncTCP folder to your Arduino IDE installation libraries folder
Finally, re-open your Arduino IDE

#How the Code Works

![259288447-6a10f492-1ca7-4d9a-8799-f5b8af0c3b6e](https://github.com/Naif-Al-Ajlani/SM23-IOT-03/assets/98528261/6766016a-ffa8-47a3-8861-524a67402865)

code link: https://wokwi.com/projects/372550980634094593

In the following paragraphs we’ll explain how the code works. Keep reading if you want to learn more or jump to the Demonstration section to see the final result.

Importing libraries
First, import the required libraries. The WiFi, ESPAsyncWebServerand the ESPAsyncTCP are needed to build the web server. The Adafruit_Sensor and the DHTlibraries are needed to read from the DHT11 or DHT22 sensors.

# resources

+ https://lastminuteengineers.com/esp32-dht11-dht22-web-server-tutorial/#google_vignette 
+ https://randomnerdtutorials.com/esp32-dht11-dht22-temperature-humidity-web-server-arduino-ide/
+ You can watch the video tutorial or keep reading this page for the written instructions: https://www.youtube.com/watch?v=tDdL5urWvH4
