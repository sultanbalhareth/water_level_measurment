📌 Project Overview



This project is an IoT-based Water Level Monitoring System designed to measure the liquid level in water tanks, chemical containers, or other liquid storage units.



 The system continuously reads the water level using a dedicated sensor and sends the data to an online dashboard.



🌐 How It Works



The ESP-WROOM-32 microcontroller acts as a CoAP client, collecting sensor data and sending it over the network.



A Node-RED web application functions as the CoAP server, receiving the data and updating a visual dashboard.



The dashboard displays the tank level as a percentage from 0–100%.

Cloud services from Microsoft Azure support backend integrations and connectivity.



🔧 Components & Tools Used



ESP-WROOM-32 microcontroller

Breadboards (x2)

Water level sensor

330Ω resistor

KiCad (for circuit design)

Node-RED (server + dashboard)

Microsoft Azure

Arduino IDE


**** Notes ****

1- You can install Node-RED locally or on cloud
2- Install CoAP library
