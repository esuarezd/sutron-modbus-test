# IoT Meteorological Station – Modbus TCP Notebook

This notebook demonstrates how to read meteorological data from a Sutron XLINK 100
via a Waveshare RS232/485/422-to-Ethernet Modbus gateway.  
The goal is to integrate sensor data into an Energy IoT / Microgrid monitoring platform.

## Hardware
- Sutron XLINK 100 (RS-232 output, Modbus RTU Slave)
- Waveshare RS232/485/422 TO POE ETH (B) (Modbus TCP ↔ RTU Gateway)
- Kipp & Zonen sensors (RS-485) and WS-600 compact weather station (SDI-12)

## Software
- Python 3.11+
- pymodbus
- pandas
- matplotlib
- jupyter

## Usage
1. Configure the gateway as Modbus TCP Server → RTU (baud 19200, 8E1)
2. Run the notebook to scan Modbus registers.
3. Identify valid registers and export readings to CSV.

