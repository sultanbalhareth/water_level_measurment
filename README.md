💧 IoT-Based Water Level Monitoring System

An open-source embedded systems + IoT project that measures and monitors liquid levels (water, chemicals, tanks, etc.) using an ESP32, CoAP protocol, and a Node-RED dashboard.

 

📌 Project Overview

This project provides a real-time water level monitoring solution.
A water level sensor reads the tank level, the ESP-WROOM-32 sends the data using the CoAP protocol, and a Node-RED web dashboard displays the level percentage from 0% to 100%.

It is ideal for IoT learning, smart home systems, industrial monitoring, and embedded systems practice.

 

🚀 Features

Real-time water level measurement (0–100%)

ESP32 as a CoAP client

Node-RED as a CoAP server + dashboard UI

Lightweight CoAP communication

Azure cloud integration support

Fully open-source and extendable

 

🛠️ Hardware Components
Component	Quantity
ESP-WROOM-32 microcontroller	1
Breadboard	2
Water level sensor	1
330 Ω resistor	1

 

🧰 Software & Tools

KiCad (circuit design)

Arduino IDE (ESP32 programming)

Node-RED (server & dashboard)

Microsoft Azure (cloud support)

 

🔌 System Architecture
Water Level Sensor → ESP32 (CoAP Client) → Node-RED (CoAP Server) → Dashboard (0–100%)


 

📡 Communication Flow

ESP32 reads analog sensor values

Converts them into % level

Sends the value to Node-RED using CoAP

Node-RED updates the real-time dashboard

 

🖥️ Dashboard Preview

(Add screenshots here if you have any)
Example:

/images/dashboard.png


 

🔧 Installation & Setup
1️⃣ Install Arduino Libraries

Make sure your ESP32 board package is installed.

Install these libraries:

CoAP library for Arduino

WiFi library for ESP32

2️⃣ Flash the ESP32

Upload the provided .ino file using Arduino IDE.

3️⃣ Setup Node-RED

Install the CoAP nodes in Node-RED:

npm install node-red-contrib-coap


Import the provided Node-RED flow from the repo.

4️⃣ Configure CoAP

Set ESP32 as client

Set Node-RED server URL to:

coap://<your-node-red-ip>:5683

5️⃣ Run the Dashboard

Start Node-RED:

node-red


Open the dashboard:

http://<your-ip>:1880/ui


 

📁 Folder Structure
├── circuit/          → KiCad schematic files
├── code/             → ESP32 firmware (Arduino)
├── node-red/         → JSON flow export
├── images/           → Dashboard & circuit images
└── README.md


 

🧪 Future Improvements

Add MQTT support

Add automatic tank refill feature

Add SMS/WhatsApp alerts (using Azure or Twilio)

Add mobile app dashboard

 

🤝 Contributing

Contributions, suggestions, and improvements are welcome!
Feel free to open a pull request or DM me for collaboration.

 

📄 License

This project is open-source under the MIT License.

 

⭐ Acknowledgments

Thanks to Allah for enabling the completion of this project.

If you want, I can also:

✅ Add badges (e.g., build, license, version)
✅ Add images for your circuit and dashboard
✅ Write an “About the Author” section
✅ Create a professional project logo
