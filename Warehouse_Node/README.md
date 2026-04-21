
# Warehouse Node (Node 2)

## Overview
This node represents the warehouse section of the Smart Factory IoT Monitoring System. It monitors environmental conditions, lighting, motion activity, and door access while supporting automated ventilation control.

## Components Used
- Arduino Uno (PicsimLab Simulation)
- DHT22 Temperature & Humidity Sensor
- LDR Light Sensor
- PIR Motion Sensor
- Reed Switch Door Sensor
- Relay Module (Ventilation)
- Status LEDs

## Features
- Monitors warehouse temperature and humidity
- Detects low light / dark conditions
- Detects motion activity using PIR sensor
- Detects door open / close status
- Automatically activates ventilation when humidity exceeds threshold
- Supports remote relay override from dashboard
- Sends telemetry data to ThingsBoard Cloud using MQTT

## Files Included
- `node2_warehouse.ino` – Main Arduino program
- `.cpp` files – Source code modules
- `.h` files – Header files
- `connections.pzw` – PicsimLab circuit design for Node 2
- Dashboard JSON file – ThingsBoard dashboard configuration


## Telemetry Parameters
- Temperature
- Humidity
- Light Level
- Dark Status
- Motion Detected
- Door Open
- Relay State
- Sensor Error
- Uptime

## Automation Logic
- Humidity ≥ 85% activates ventilation relay automatically
- Dashboard RPC command can manually override relay state

## Status LEDs
- Green = Normal
- Yellow = Warning / Dark Condition
- Red = Alert / Fault

## Simulation
Open the `connections.pzw` file in PicsimLab to run the Node 2 circuit simulation.
