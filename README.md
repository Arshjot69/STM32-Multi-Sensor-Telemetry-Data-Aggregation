STM32 Multi-Sensor Telemetry Data Aggregation

This project demonstrates how to acquire data from multiple on-board sensors using an STM32 microcontroller and organize the collected information into a structured telemetry frame. The implementation illustrates real-time embedded data aggregation and telemetry handling commonly used in IoT edge-node and monitoring systems.

Features
Multi-sensor data acquisition
Structured telemetry frame generation
Real-time environmental and motion data collection
STM32 HAL library implementation
STM32CubeIDE compatible project
Embedded telemetry processing
Project Overview

The firmware interfaces with multiple onboard sensors such as temperature, humidity, pressure, and accelerometer modules. Sensor readings are periodically collected, processed, and combined into a structured telemetry frame suitable for communication, logging, or cloud transmission.

This project helps in understanding:

Multi-sensor integration
Embedded data aggregation
Telemetry frame formatting
STM32 peripheral management
IoT edge-node data handling
Hardware Requirements
STM32 Development Board
On-board or External Sensors:
HTS221 (Temperature & Humidity)
LPS22HB (Pressure)
LSM6DSL (Accelerometer/Gyroscope)
Connecting Wires (if external modules are used)
USB Cable for programming and power
Software Requirements
STM32CubeIDE
STM32CubeMX
Working Principle
System clock and communication peripherals are initialized.
All onboard sensors are configured and activated.
Sensor readings are periodically acquired from each module.
The collected data is processed into readable values.
Sensor values are combined into a structured telemetry frame.
The telemetry frame can be transmitted, displayed, or logged for monitoring applications.
Example Telemetry Frame
{
  "temperature": 28.5,
  "humidity": 65.2,
  "pressure": 1012.4,
  "acceleration_x": 0.12,
  "acceleration_y": -0.03,
  "acceleration_z": 9.81
}
Applications
IoT edge-node systems
Environmental monitoring
Industrial automation
Smart sensing platforms
Real-time telemetry systems
