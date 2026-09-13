# IoT Weather Station

An Arduino-based automatic weather station that reads live environmental data : temperature, humidity, soil moisture, and rainfall from a set of sensors and streams it over serial.

## Overview

This sketch runs on an Arduino connected to a DHT11 temperature/humidity sensor plus analog soil moisture and rain sensors. It continuously polls all four sensors and prints a formatted readout over serial, which can be viewed with any serial monitor (e.g., the Arduino IDE's built-in monitor, or a terminal program like CoolTerm).

## Hardware

- Arduino (Uno or compatible)
- DHT11 temperature & humidity sensor (digital pin 2)
- Soil moisture sensor (analog pin A0)
- Rain sensor (analog pin A1)

## Dependencies

This project uses the [Adafruit DHT sensor library](https://github.com/adafruit/DHT-sensor-library). Install it via the Arduino IDE's Library Manager (Sketch → Include Library → Manage Libraries → search "DHT sensor library") rather than installing manually — no need to vendor the library files into this repo.

## Running the Project

1. Wire up the sensors as described above.
2. Install the DHT sensor library via the Arduino Library Manager.
3. Upload `weather_station.ino` to your Arduino.
4. Open a serial monitor at 9600 baud to view live sensor readings.

## Status

This currently covers live sensor data collection. Prediction modeling and database storage are planned extensions, not yet implemented in this version.

## Author

Aishwarya Ramanath Shanbhag
