Automatic Drainage Monitoring and Control System

This project presents an IoT-based automated system designed for real-time monitoring and control of urban manholes. It aims to prevent urban flooding, clogs, and hazardous gas accumulations by shifting drainage maintenance from reactive to proactive. 

Key Features

Real-Time Monitoring: Continuously tracks water level (percentage), temperature, pressure, altitude, and methane gas concentration.

Automated Control: A motor-driven drainage system automatically activates when water levels exceed a safe threshold to prevent overflows.

Dual-Alert System: Sends immediate notifications via SMS, Email, and the Blynk App when blockages or hazardous gases are detected.

GPS Integration: Includes the precise location and unique ID of the manhole in every alert to ensure a swift response from municipal authorities.

Non-Volatile Storage: Uses EEPROM to save calibration data, ensuring the system retains its settings after power cycles.

Hardware Components

Microcontroller: Arduino (for sensor logic) and ESP8266 (for Wi-Fi/IoT connectivity).

Sensors:Ultrasonic Sensor (Water Level).MQ-4 (Methane Gas Detection).BMP180 (Pressure and Temperature).

Actuators: Motor-driven pump.

Communication: GPS Module (Location) and Wi-Fi Module.

System Logic
The system operates based on defined safety thresholds:

Low Level (<30%): Pump remains OFF/Auto-ready.

High Level (>85%): Pump deactivates to prevent over-pumping or once levels are safe.

Alert Trigger: If gases exceed safe limits or a blockage is detected, an alert with GPS coordinates is sent.
