<p align='center' >
  <img width="250px" loading="lazy" src = "https://github.com/Geral-cp-s/Sprint-Edge/assets/110639916/aa204473-bba7-4dc2-8db1-ea5744b8e9bc"/>
</p>
<h1 align="center">Global Vineyard Monitoring with FIWARE and ESP32</h1>

# Table of Contents
* [1 - Project Description](#descricao)
* [2 - Functionality](#funcionalidades)
  * [2.1 - Luminosity Data Capture](#funcionalidades1)
  * [2.2 - Data Transmission to FIWARE](#funcionalidades2)
  * [2.3 - Command Reception via Postman](#funcionalidades3)
  * [2.4 - Historical Data Dashboard](#funcionalidades4)
* [3 - Architecture and Components](#arquitetura)
  * [3.1 - Phisycal Components](#arquitetura1)
  * [3.2 - Communication](#arquitetura2)
  * [3.3 - Software](#arquitetura3)
* [4 - Dashboard](#dash)
* [5 - System Configuration](#config)
  * [5.1 - FIWARE Setup](#config1)
  * [5.2 - ESP32 Setup](#config2)
  * [5.3 - Python Dashboard Setup](#config3)
* [6 - Available Statistics](#estatisticas)
* [7 - Implementation Steps](#passo-passo)
  * [7.1 - FIWARE Configuration](#passo-passo1)
  * [7.2 - ESP32 Code Deployment](#passo-passo2)
* [8 - License](#licenca)
* [9 - Video](#video)
* [10 - Code Dashboard](#codigo1)
* [10 - Code Simulator](#codigo2)
* [11 - Access to the Simulator](#simulador)
* [12 - Authors](#autores)

<h2 id="Descricao">Project Description</h2>
<p>This project is part of Check Point 4, aiming to integrate a global vineyard monitoring solution using the FIWARE platform as the backend. The ESP32 DEVKIT 1, equipped with luminosity, humidity, and temperature sensors, collects data from the vineyard environment and sends it to FIWARE for processing and storage. Additionally, a Python-based dashboard is provided for analyzing historical data.</p>
<p>The solution demonstrates interoperability between IoT devices and FIWARE, with control commands sent to the ESP32 through Postman. The dashboard allows for real-time visualization of the vineyard’s environmental conditions and historical data analysis.</p>

<h2 id="funcionalidades">⚙️ System Operation</h2>
<h3 id="funcionalidades1">2.1 Luminosity Data Capture</h3>

- `Feature ` An ESP32 equipped with a luminosity sensor (LDR) captures light intensity data from the vineyard environment.

<h3 id="funcionalidades2">2.2 Data Transmission to FIWARE</h3>

- `Feature ` The captured data is transmitted to a FIWARE instance, where it is processed and stored for further analysis.
  
<h3 id="funcionalidades3">2.3 Command Reception via Postman</h3>

- `Feature ` The system allows for the sending of commands via Postman to the ESP32, such as turning the onboard LED on or off.
  
<h3 id="funcionalidades4">2.4 Historical Data Dashboard</h3>

- `Feature ` A Python-based dashboard allows for the visualization of historical data collected by the sensors, including luminosity, humidity, and temperature, providing a comprehensive overview of vineyard conditions over time.

  <h2 id="Componentes">🛠️ Architecture and Components</h2> 
<h3 id="componentes1">Physical Components</h3> 
<ul> 
  <li>ESP32: Microcontroller that manages the sensors and communication with the MQTT server and the display.</li> 
  <li>DHT 11: Temperature and humidity sensor.</li> 
  <li>LDR: Light-dependent resistor (luminosity sensor).</li> 
  <li>Power supply: for the ESP32.</li> 
</ul> 
<h3 id="componentes2">Communication</h3> 
<ul> 
  <li>MQTT Protocol for communication between the ESP32 and FIWARE.</li> 
  <li>Internet connection for communication with FIWARE.</li> 
  <li>Wi-Fi connectivity for the ESP32.</li>
</ul> 
<h3 id="componentes3">Software</h3> 
<ul> 
  <li>FIWARE for backend processing and data storage.</li> 
  <li>Postman for sending control commands to the ESP32.</li> 
  <li>Python for creating a dashboard to analyze historical data.</li> 
</ul>

<h2 id="dash">Dashboard</h2>
<img width="900px" loading="lazy" src = "https://github.com/user-attachments/assets/b9681d12-ffc8-4f75-8d61-7bb715aee0c3"/>


<h2 id="config">📡 System Configuration</h2> 
<h3 id="config1">FIWARE Setup</h3> 
<ol>
  <li>Install and configure FIWARE using a cloud provider.</li>
  <li>Set up security measures for the FIWARE instance.</li>
  <li>Perform health checks to ensure the instance is functioning properly.</li>
</ol>

<h3 id="config2">ESP32 Setup</h3> 
<ol>
  <li>Program the ESP32 DEVKIT 1 using the provided code.</li>
  <li>Ensure the device is connected to Wi-Fi and able to send data to FIWARE.</li>
</ol>

<h3 id="config3">Python Dashboard Setup</h3> 
<ol>
  <li>Install necessary Python libraries for data visualization.</li>
  <li>Run the dashboard script to visualize historical data collected by the sensors.</li>
</ol>

<h2 id="estatisticas">📊 Available Statistics</h2>
<p>The Python dashboard provides the following statistics:</p>
<ul> 
  <li>Current and historical luminosity levels.</li> 
  <li>Temperature and humidity levels.</li>
  <li>Graphical representation of data trends over time.</li>
</ul>

<h2 id="passo-passo">🚀 Implementation Steps</h2>
<h3 id="passo-passo1">FIWARE Configuration</h3> 
<ol> 
  <li>Download FIWARE Descomplicado and deploy it in a cloud service.</li>
  <li>Configure security measures and verify functionality using health checks.</li>
</ol> 
<h3 id="passo-passo2">ESP32 Code Deployment</h3> 
<ol> 
  <li>Upload the code to the ESP32 using Arduino IDE or another compatible platform.</li> 
  <li>Ensure the sensor data is being transmitted to FIWARE and is accessible.</li>
</ol>

<h2 id="licenca">📄 License</h2> 
<p>This project is licensed under the MIT License. See the LICENSE file for details.</p>

<h2 id="video">Video</h2>
https://youtu.be/50hYxLyjVj8

<h2 id="codigo1">Code Dashboard</h2>
https://github.com/Geral-cp-s/CP5-Edge/blob/main/dashboard.txt

<h2 id="codigo2">Code Simulator</h2> 
https://github.com/Geral-cp-s/CP5-Edge/blob/main/code.ino

<h2 id="Simulador">Access to the Simulator</h2>
https://wokwi.com/projects/410849473799433217

<h2 id="Autores">Authors</h2>

<div align="center">
  
| [<img loading="lazy" src="https://github.com/gvqsilva/CP2-Edge/assets/110639916/d022ed18-0057-4944-9e00-db796c6d2e45" width=115><br><sub>Gabriel Vasquez</sub>](https://github.com/gvqsilva)  |  [<img loading="lazy" src="https://github.com/gvqsilva/CP2-Web/assets/110639916/1eb7df1a-c0e8-4170-aabf-444cfb3c64f9" width=115><br><sub>Guilherme Araujo</sub>](https://github.com/guilhermearaujodec)  |  [<img loading="lazy" src="https://github.com/gvqsilva/CP2-Edge/assets/110639916/86514492-2b1e-4422-bdc0-0ec3c8be3dcc" width=115><br><sub>Augusto Douglas</sub>](https://github.com/gutomend)  |  [<img loading="lazy" src="https://github.com/gvqsilva/CP2-Edge/assets/110639916/4bb3084d-d1ff-4b49-ba37-96c8046f6e14" width=115><br><sub>Gustavo Oliveira</sub>](https://github.com/Gusta346) |
| :---: | :---: | :---: | :---: |

<ul>
  <li>Gabriel Vasquez - RM: 557056</li>
  <li>Guilherme Araujo - RM: 558926</li>
  <li>Gustavo Oliveira - RM: 559163</li>
  <li>Augusto Mendonça - RM: 558371</li>
</ul><br>

</div>
