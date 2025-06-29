# ESP32-IoT-Weather-Station
An ESP-32 IoT based embedded system that hosts it's own WiFi network and web page to display
real time weather and time data through a responsive web-based UI
</br>
*created by Bryan Diaz | Focus: Embedded Systems, IoT, hardware*

# Project Overview
Fully functional prototype of an IoT embedded system built using the ESP-32 and it's Soft Access Point mode
to create it's own WiFi network allowing user's that are connected to access a web-page to monitor sensor data.

This system is designed to be simple, compact, and efficient where it doens't have to rely on being connected to an external WiFi network in order to display data.
I built this to further explore concepts of embedded systems along with the goal of broadening my expirence with different types of microcontrollers and their methods.

This systems displays weather and time realted data onto a web-page hosted by the ESP-32 that was made using embedded HTML,CSS, and JavaScript to give the user a nice and clean UI that they have option the change using a button to better suit their enviorment.

# Technologies and Componenets
## Hardware Related
+ ESP-32
+ MQ-135 (air quality sensor)
+ DHT-11 (tempature and humidity sensor)
+ DS3231 real time clock module
+ Perboard & Breadboard
+ Soldering

## Software Related
+ Arduino IDE
+ C++ (custom functions to retrieve and send data to webpage)
+ *Embedded Web Technologies (used for UI)*
    + HTML
    + CSS
    + JavaScript (SetInterval & fetch functions: requests data every second and sends it to webpage to get live chaning data)
+ Soft AP Configuration (ESP-32 is programmed to be a WiFi and webserver access point)
  </br>
  </br>
+ Various libraries:
    + RTCLib
    + DHT
    + WiFi (wifi library for ESP-32)
    + WebServer (webserver library for ESP-32)
 
## Wire Setup
+ *[Wiring Schematic](IoTWeatherStationDiagram.png)*

# System Features
+ No WiFi needed to operate
+ ESP-32 creates it's own WiFi network
+ Web-Interface: once user is connected to network; user can connect to webpage by searching IP into any search engine
+ *Displays Time and Weather related data on clean embedded UI*
+ User responsive UI/ Theme toggle (via button on webpage)

# Brief Notes
After making the initial prototype on a breadboard I decided to transfer the circuit onto a perfboard so this system could be more usable and permanent. I assembled everything with the idea of minimizing wire clutter along with mainting good power distribution throughout the entire system.
*When setting the RTC module for date and time: user has to set it twice (first = initial set) (second = //comment out initial set so it doesn't reset upon plug in of device)*

# System DEMO
<img src = "https://github.com/user-attachments/assets/2c198dd4-7f36-4538-a97c-18a471ddff9d" width = "500" height = "450"/> 
</br>
<img src = "https://github.com/user-attachments/assets/1f4d39b4-e37c-43df-b9d2-100bac5804b2" width = "500" height = "450"/> <img src = "https://github.com/user-attachments/assets/2cbf61d6-d23c-4c61-bc88-beb428092c60" width = "500" height = "450"/>




