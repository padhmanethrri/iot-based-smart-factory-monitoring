# Production Line Node (Node 1)

## Overview
This node monitors the production area of the factory and collects machine/environmental data.

## Sensors & Components
- DHT22 Temperature and Humidity Sensor
- LM35 Machine Temperature Sensor
- Vibration Sensor
- Push Button (Machine Status)
- Relay Module
- Green / Yellow / Red LEDs

## Functions
- Reads environmental temperature and humidity
- Detects machine temperature
- Monitors vibration levels
- Detects machine ON/OFF state
- Sends telemetry to ThingsBoard Cloud
- Supports remote relay control using RPC

## Files Included
- `.ino` main code
- `.cpp` source modules
- `.h` header files
- Connection images

## Status Indications
- Green LED = Normal
- Yellow LED = Warning
- Red LED = Critical / Fault
