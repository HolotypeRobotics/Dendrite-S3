At the moment this repository is still in development, and hould not be used.

# Dendrite-S3
<p align="center">
  <img src="https://github.com/HolotypeRobotics/Dendrite-S3/blob/main/pcb/pinout.png" />
</p>

The Dendrite-S3 is a robotics development board powered by the ESP32-S3, featuring an on-board LiPo charge/discharge circuit, and 34 GPIO.

## Getting Started

### Installation

#### Prerequisites

- ROS2
- VSCode with Platform.io
- 
1. **Clone the Repository**

2. **Build the Project:**

3. **Flash to Microcontroller:**

4. **Run the Micro-ROS Agent**

5. **Verify Communication:**

## Project Outline

At its core, this is a ROS2 program that runs on the esp32-s3. It subscribe to "Action Matrix", and "Attention Matrix". The '''Action Matrix''' is the list of next action for each actuator. The '''Attention Matrix''' is the list of queries for each sensor. 0 if none. Its lifecycle consists of boot, running, and shutdown states. During the running state, it will:

1. Preform all actions in the action matrix 
2. Query all sensors in the Attention matrix
3. publish all the sensor data. This will all occur in the spin function.

The sensors will all use zephyr drivers.

## Contributing
Please see our contributing.md


