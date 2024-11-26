# MPU6050-CPP-ARM-RaspberryPi

This Blog shows the minimal C++ code for interfacing with the MPU6050 sensor on ARM and Raspberry Pi devices.

[Repositorie of the MPU6050 C++ Interface for ARM and Raspberry Pi](https://github.com/NazTechs/MPU6050-CPP-ARM-RaspberryPi) - Access the complete code and documentation on GitHub.

## Overview

The MPU6050 is a commonly used accelerometer and gyroscope module. This code provides basic functionalities to initialize the sensor, read raw data from the accelerometer and gyroscope, and calculate sensor measurements. It serves as a starting point for incorporating MPU6050 functionality into C++ projects on ARM platforms.

<p align="center">
  <img src="https://github.com/soheil1156/MPU6050-CPP-ARM-RaspberryPi/assets/24310606/d553139f-1310-4e88-9187-4dfab78e82e3" alt="Vibration Analysis" width="400">
</p>

## Features

- Initialization of the MPU6050 sensor
- Reading raw data from the accelerometer and gyroscope
- Calculation of sensor measurements
- ARM and Raspberry Pi compatibility

## Building the Software and Installing Dependencies

To build and run the MPU6050-CPP-ARM-RaspberryPi software, follow these steps:

1. Ensure that you have the necessary dependencies installed on your ARM or Raspberry Pi device. This code relies on the following libraries:
   - Linux I2C Development Libraries
   - C++ Compiler (e.g., GCC)

   If these libraries are not already installed, you can install them using the package manager for your specific Linux distribution. For example, on Debian-based systems, you can use the following command:

   ```bash
   sudo apt-get install libi2c-dev g++
   
2. Clone the repository to your local machine:
   ```bash
   git clone https://github.com/soheil1156/MPU6050-CPP-ARM-RaspberryPi.git
3. Navigate to the project directory:
   ```bash
   cd MPU6050-CPP-ARM-RaspberryPi
4. Build the code using the provided Makefile:
  ```bash
     make

This command will invoke the Makefile, which contains the necessary build instructions. It will compile the code and create an executable named MPU6050.
5. Run the executable:
  ```bash
    ./MPU6050
  ```
The code will interface with the MPU6050 sensor and display the sensor measurements.
## MATLAB Vibration Analysis
<p align="center"> <img src="https://github.com/soheil1156/MPU6050-CPP-ARM-RaspberryPi/assets/24310606/cbcf55cc-7cac-4c32-bfa9-b4ef32ef300c" alt="Vibration Analysis" width="400"> </p>
Description: This image showcases the results of a vibration analysis conducted using MATLAB. The analysis was performed using the MPU6050-CPP-ARM-RaspberryPi software developed in C++. The image demonstrates the vibration waveform and provides insights into the vibration characteristics.

## Contributing
Contributions to this repository are welcome. If you have any improvements or bug fixes, feel free to submit a pull request. For major changes, please open an issue first to discuss the proposed changes.

## License
This project is licensed under the MIT License. Feel free to use and modify the code for your own projects.
<!-- Google Tag Manager (noscript) -->
<noscript><iframe src="https://www.googletagmanager.com/ns.html?id=GTM-K93SNNGZ"
height="0" width="0" style="display:none;visibility:hidden"></iframe></noscript>
<!-- End Google Tag Manager (noscript) -->

## Acknowledgements
MPU6050 Datasheet: Official datasheet for the MPU6050 sensor.
Linux I2C Documentation: Documentation for using I2C on Linux.
