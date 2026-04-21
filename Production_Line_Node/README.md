# Production Line Node (Node 1)

## Overview
This node represents the production line section of the Smart Factory IoT Monitoring System. It is responsible for monitoring machine health, environmental conditions, and equipment status in real time.

## Components Used
- Arduino Uno (PicsimLab Simulation)
- DHT22 Temperature & Humidity Sensor
- LM35 Temperature Sensor
- Vibration Sensor
- Push Button (Machine ON/OFF Status)
- Relay Module
- Green, Yellow, Red Status LEDs

## Features
- Reads temperature and humidity data
- Monitors machine surface temperature using LM35
- Detects vibration levels for machine condition monitoring
- Detects machine running status
- Controls relay through cloud RPC commands
- Sends telemetry data to ThingsBoard Cloud using MQTT
- LED status indication for normal, warning, and fault states

## Files Included
- `node1_production.ino` – Main Arduino program
- `.cpp` files – Source code modules
- `.h` files – Header files
- `connections.pzw` – PicsimLab circuit design for Node 1
- Python file – Supporting integration (utility script)


## Telemetry Parameters
- Temperature
- Humidity
- LM35 Temperature
- Vibration Value
- Machine Status
- Relay State
- Sensor Error
- Uptime

## Status LEDs
- Green = Normal Operation
- Yellow = Warning / Sensor Issue
- Red = Critical Condition

## Simulation
Open the `connections.pzw` file in PicsimLab to run the Node 1 circuit simulation.
