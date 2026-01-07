# MQTT Data Collection and Visualization

Assignment for Applied Computer Science course at FH Technikum Wien.

## Description

This project collects sensor data from an MQTT broker and visualizes the power measurements.

## Files

- `subscriber.ipynb` - Collects data from MQTT topic and saves to CSV
- `visualize.ipynb` - Reads CSV file and creates a plot
- `data.csv` - Collected sensor data
- `plot.png` - Power measurement visualization

## How to Run

1. Install required libraries:
```
pip install paho-mqtt matplotlib
```

2. Run `subscriber.ipynb` first to collect data (runs for 2 minutes)

3. Run `visualize.ipynb` to create the plot

## MQTT Settings

- Broker: test.mosquitto.org
- Port: 8883 (TLS)
- Topic: /fhtw/appcsmqtt

## Data Format

CSV file contains:
- time (timestamp in milliseconds)
- u1 (voltage)
- power (watts)
- freq (frequency in Hz)

## Requirements

- Python 3.x
- paho-mqtt
- matplotlib

## Author

Hongqian Li
Jan 2026