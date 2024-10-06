# IoT-Based Wearable Health and Security Device

## Table of Contents
- [Notice]{#Important-Notice}
- [Overview](#overview)
- [Features](#features)
- [Architecture](#architecture)
- [Hardware Requirements](#hardware-requirements)
- [Software Requirements](#software-requirements)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)



## Important Notice

This project is based on IoT development, utilizing hardware like the **ESP8266**. The project involves various libraries with deep directory structures that are critical for its operation. However, due to **operating system limitations**, particularly on Windows, where the maximum file path length is 260 characters, **I have not uploaded the project to GitHub**. All files and project resources are stored locally on my system.

### Why This Happens:
- **Long File Names**: IoT packages like the **ESP8266** come with long directory structures, and certain files have long names to support various configurations and examples. 
- **Windows File System Limitations**: Windows imposes a file path length limit of 260 characters, starting from the drive (e.g., `C:\`). Some files in the libraries exceed this length, causing errors like `Filename too long`, which prevents the project from being uploaded to GitHub.

### Current Status:
- **All Files are Stored Locally**: None of the project files, including code, libraries, or dependencies, have been uploaded to this GitHub repository due to these constraints. The project exists only in my local development environment.

### Solution for Users:
- To work with this project, you will need to manually install the necessary IoT libraries (e.g., **ESP8266**) on your local machine.
- Ensure that you place the project in a **short directory path** on your system to avoid file path length issues (e.g., `C:\Projects\IoTDevice`).

If you have any questions or need assistance with setting up the project locally, feel free to contact me.


## Overview
This project focuses on developing a wearable IoT-based device designed for health monitoring and security purposes. The system uses various sensors to collect physiological data such as temperature, blood pressure, and pulse rate. In case of an emergency or abnormal readings, it sends real-time alerts to predefined contacts using GSM and GPS modules. This wearable device provides assistance during health crises or security threats, ensuring timely intervention.

## Features
- **Real-Time Monitoring**: Continuously tracks body temperature, pulse rate, and blood pressure.
- **Security Alerts**: Detects unusual behavior and sends location-based alerts to emergency contacts.
- **Automated Response**: Takes predefined actions based on collected data, such as notifying authorities or healthcare providers.
- **GPS Location Tracking**: Tracks the wearer's location for real-time assistance.
- **GSM Communication**: Sends alerts via SMS to designated contacts during emergencies.

## Architecture
The device operates using the following components:
1. **Sensors**: 
   - Temperature sensor (DS18B20)
   - Pulse rate sensor
   - Blood pressure sensor
2. **Microcontroller**: Arduino Uno for data acquisition and processing.
3. **Communication Modules**: GSM and GPS modules for sending alerts and tracking location.
4. **Data Transmission**: Physiological data is sent via GSM to emergency contacts and healthcare providers.

## Hardware Requirements
- Arduino Uno microcontroller
- DS18B20 temperature sensor
- Pulse rate sensor
- Blood pressure sensor
- GSM module
- GPS module
- Power supply (battery or USB)

## Software Requirements
- **Arduino IDE** for programming the Arduino board
- **GSM and GPS Libraries** for Arduino
- **Serial Monitor** for debugging and logging

## Installation
1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/iot-health-security-device.git
    cd iot-health-security-device
    ```
2. Install the necessary Arduino libraries for GSM and GPS communication.
3. Connect the hardware components to the Arduino as per the provided circuit diagram.

## Usage
1. Upload the code to your Arduino Uno using the Arduino IDE.
2. Power on the device.
3. The system will begin monitoring vital signs. If abnormal readings are detected, alerts will be automatically sent to predefined contacts.
4. You can view the status of the sensors via the Arduino Serial Monitor.

## Contributing
Contributions are welcome! Please follow these steps:
1. Fork the repository.
2. Create a new branch:
    ```bash
    git checkout -b feature-branch
    ```
3. Make your changes and commit them:
    ```bash
    git commit -m "Add new feature"
    ```
4. Push to the branch:
    ```bash
    git push origin feature-branch
    ```
5. Open a pull request.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
