# Cryogenic Magnetic Reluctance Measurement
**Accurate Measurements in Extreme Temperatures (-176°C.)**

<div align="center">
  <img src="https://github.com/user-attachments/assets/92795f09-ad5d-47af-aa83-36c146e18a15" alt="image" width="500"/>
</div>

# Introduction:
The Cryogenic Measurement System was designed and installed at ABBNIROO in 2016 for a Cryogenic Plants-Air Separation process in a petrochemical plant. The project was initiated to improve the efficiency and productivity of the process by providing reliable and accurate measurements in an extreme temperature environment.
The Cryogenic Plants-Air Separation process involves the separation of gases using extreme temperatures, with the cold box being a crucial component of the process responsible for generating liquid nitrogen. The cold box operates at temperatures as low as -176°C, making it a challenging environment for measurement and control systems.
To address this challenge, We designed and installed a specialized Cryogenic Measurement System that could operate in this extreme temperature environment. The system was designed using a combination of FPGA and microcontroller, with a magnetic reluctance sensor used for sensing magnetic field changes in the cryogenic system.

<div align="center">
  <img src="https://github.com/user-attachments/assets/0b3c6ca8-b5d6-427f-950f-a25321eef0cd" alt="image" width="500"/>
</div>

---
The Cryogenic Measurement System has been in operation since its installation in 2016, providing accurate measurements and control in an extreme temperature environment, thus improving the efficiency and productivity of the Cryogenic Plants-Air Separation process. This article provides an overview of the Cryogenic Measurement System, including its design, installation, and operation, highlighting the importance of accurate measurement and control systems in the petrochemical industry and the benefits of using specialized systems for extreme temperature environments.

<div align="center">
  <img src="https://github.com/user-attachments/assets/5bc5e86f-05cd-4690-828e-fe1f5e4b9886" alt="image" width="400"/>
</div>

---
# Hardware Design:
In the design of a cryogenic measurement system, selecting the right hardware and software tools is crucial to ensuring accurate measurements in extreme temperatures. The choice of hardware design tools can greatly influence the performance and reliability of the system.
For the cryogenic measurement system, we chose to use Altium Designer for schematic capture and printed circuit board (PCB) layout. Altium Designer is a powerful and versatile tool that enables designers to create complex mixed-signal and high-speed digital designs with ease.
One of the challenges in the design of the measurement system was dealing with the extreme temperatures involved. To compensate for the effects of the cryogenic temperatures on the magnetic reluctance sensor, we needed to use an FPGA and microcontroller to read and process the sensor data. Altium Designer's mixed-signal design capabilities were invaluable in the integration of the FPGA and microcontroller into the design.

<div align="center">
  <img src="https://github.com/user-attachments/assets/84bb5a7a-09a1-443d-9848-7cb5e206b2b1" alt="image" width="300"/>
</div>


signal integrity issues early in the design phase, allowing us to make the necessary adjustments before fabrication.
The SPICE software allowed us to perform mixed-signal simulation of the design before prototyping. This enabled us to verify the performance of the system before fabrication and ensure that it met the required specifications.

<div align="center">
  <img src="https://github.com/user-attachments/assets/4263fbe6-2603-4f28-84b5-239ae4e25841" alt="image" width="300"/>
</div>

---
## FPGA Design:
Field-Programmable Gate Arrays (FPGAs) are becoming increasingly popular for developing high-performance digital systems. The FPGA-based digital system can be easily customized, upgraded, and reprogrammed. This makes it an ideal choice for designing and implementing complex digital systems that require high performance and flexibility. In the Cryogenic Measurement System designed and installed for ABBNIROO, FPGAs were used for sensor readout and digital signal processing.
**FPGA Architecture**
The FPGA used in the Cryogenic Measurement System is a Xilinx Spartan-3 FPGA. The Spartan-3 FPGA is a low-cost FPGA that provides a flexible architecture for implementing complex digital systems. The Spartan-3 FPGA has a high-speed interface and a large number of programmable logic blocks (PLBs) that can be configured to perform various tasks.

<div align="center">
  <img src="https://github.com/user-attachments/assets/a74b8e12-8107-4f80-ae80-d20c28148370" alt="image" width="300"/>
</div>

**FPGA-Based Sensor Readout**
The Cryogenic Measurement System uses magnetic reluctance sensors to measure the magnetic field changes in the Cryogenic system. The magnetic reluctance sensor produces a small signal that is proportional to the magnetic field changes. This signal is very weak and must be amplified and processed before it can be used for measurement.
To read the signal from the magnetic reluctance sensors, an FPGA-based sensor readout circuit was designed and implemented. The readout circuit includes a low-noise amplifier, a filter, and a digitizer. The low-noise amplifier amplifies the small signal from the magnetic reluctance sensors, the filter removes unwanted noise, and the digitizer converts the analog signal into a digital signal.
**FPGA-Based Digital Signal Processing**
The Cryogenic Measurement System uses FPGAs for digital signal processing. The FPGAs are responsible for performing signal processing tasks such as filtering, averaging, and compensation. The FPGAs also implement algorithms to compensate for the sensor drift, temperature changes, and other factors that can affect the accuracy of the measurements.
To achieve high-performance digital signal processing, the FPGAs are configured to use pipelining and parallel processing techniques. Pipelining and parallel processing techniques reduce the processing time by breaking the task into smaller sub-tasks and processing them simultaneously.

<div align="center">
  <img src="https://github.com/user-attachments/assets/751f4e65-c8b9-4aeb-93c3-2c0ffd53f86a" alt="image" width="300"/>
</div>

**Mixed Signal and High-Speed Signal Design**
The Cryogenic Measurement System is a mixed signal and high-speed signal design that includes analog and digital components. The analog components include magnetic reluctance sensors, low-noise amplifiers, and filters. The digital components include FPGAs, microcontrollers, and communication interfaces.

<div align="center">
  <img src="https://github.com/user-attachments/assets/410f5639-7831-4917-b96a-09c1fd51ba7f" alt="image" width="300"/>
</div>

To ensure proper signal integrity and avoid noise and distortion, the Cryogenic Measurement System uses various design techniques such as proper grounding, shielding, and signal routing. The design also includes impedance matching, termination, and decoupling techniques to ensure the reliable transmission of high-speed signals.

<div align="center">
  <img src="https://github.com/user-attachments/assets/27962c61-20f8-4046-b3f3-ea052af5fdad" alt="image" width="300"/>
</div>

## Microcontroller Design:
The Cryogenic Measurement System incorporates a powerful and reliable microcontroller to provide real-time data acquisition and control. The NXP LPC4088 is an Arm Cortex M4-based microcontroller that is capable of running at high speeds while consuming minimal power.
The microcontroller is responsible for controlling the overall operation of the Cryogenic Measurement System. It communicates with the FPGA to retrieve sensor data, performs signal conditioning and compensation, and processes the data for display and analysis. Additionally, it communicates with the outside world through various communication interfaces such as UART, I2C, and SPI.

<div align="center">
  <img src="https://github.com/user-attachments/assets/0f708be2-2c2f-4d87-8e84-5265ce93021c" alt="image" width="500"/>
</div>


One of the key features of the NXP LPC4088 microcontroller is its high level of integration. It incorporates a wide range of peripherals, including high-speed ADCs, DACs, timers, and PWMs, making it well-suited for real-time data acquisition and control applications. Moreover, its high-speed memory and flexible memory-mapped I/O architecture provide a highly responsive environment for data processing
The microcontroller is also equipped with a rich set of software development tools, including a fully integrated development environment (IDE), compilers, debuggers, and other software utilities. These tools provide an efficient and easy-to-use environment for developing and testing firmware and software applications for the Cryogenic Measurement System.
In addition, the NXP LPC4088 microcontroller is highly scalable, allowing it to meet the requirements of a wide range of applications. It can be used in standalone applications or as part of a larger system, making it a versatile choice for many different types of projects.

<div align="center">
  <img src="https://github.com/user-attachments/assets/50399a7d-bd50-4c80-9de8-753b9f3f6e8c" alt="image" width="300"/>
</div>

The NXP LPC4088 microcontroller is used in the Cryogenic Measurement System to compensate data for the cryogenic system. The microcontroller is responsible for processing the sensor data to ensure accurate measurements are taken. It compensates for any temperature or pressure changes in the cryogenic system, ensuring that the data captured is reliable and accurate.
## Magnetic Reluctance Sensor:
Magnetic reluctance sensors are widely used in various industries, including the petrochemical industry, due to their high accuracy and reliability. These sensors are based on the principle of magnetic reluctance, which is the measure of a magnetic circuit's resistance to magnetic flux.

<div align="center">
  <img src="https://github.com/user-attachments/assets/c86d2b53-1fbb-42d3-af6f-54fa428afb6b" alt="image" width="300"/>
</div>

In the Cryogenic Measurement System designed for the cold box in the petrochemical industry, a magnetic reluctance sensor was used to detect changes in the magnetic field within the cryogenic system. This sensor works by measuring the change in the reluctance of a magnetic circuit when a magnetic field is applied. The magnetic reluctance is directly proportional to the magnetic flux and inversely proportional to the magnetic permeability of the circuit material.
The magnetic reluctance sensor consists of two main parts: the sensing element and the processing circuitry. The sensing element is usually a coil of wire wrapped around a magnetic core. When a magnetic field is applied to the magnetic core, it induces a voltage in the coil, which is proportional to the rate of change of the magnetic flux.
The processing circuitry amplifies the voltage signal generated by the sensing element and converts it into a digital signal. This digital signal is then processed by the microcontroller and sent to the FPGA for further processing and analysis.
One of the advantages of using a magnetic reluctance sensor is that it is relatively immune to electrical noise and interference. This makes it ideal for use in harsh environments, such as the cryogenic system in the cold box, where there may be a significant amount of electrical noise. Additionally, magnetic reluctance sensors have a wide operating temperature range, making them suitable for use in extreme temperature environments.

<div align="center">
  <img src="https://github.com/user-attachments/assets/f8fa67c7-15d6-4e4f-8948-b27568ae1be4" alt="image" width="300"/>
</div>

## Mechanical Design and Sensor Stand:

A specialized sensor stand was designed in CATIA software to accurately measure the rotation speed and vibration of the impeller shaft. The sensor stand is installed on the main diffuser of the compressor, where the impeller shaft passes through. The stand is designed to withstand the extreme cryogenic temperatures of the environment.
<div align="center">
  <img src="https://github.com/user-attachments/assets/d7215622-b81a-489b-b707-a1db486f2397" alt="image" width="300"/>
</div>
The sensor stand features a magnetic reluctance sensor, which detects the rotation speed of the impeller shaft by measuring changes in magnetic field strength. The sensor is positioned close to the shaft but does not touch it, allowing for accurate measurements without affecting the impeller's operation.

<div align="center">
  <img src="https://github.com/user-attachments/assets/267fde11-56f1-45c7-9a34-598fe056dd4d" alt="image" width="400"/>
</div>
<div align="center">
  <img src="https://github.com/user-attachments/assets/7b990c1d-95e8-4527-b059-16c900278cac" alt="image" width="400"/>
</div>


The mechanical design of the sensor stand was optimized to ensure stable and reliable measurement even in the extreme cryogenic environment. The stand is made of high-quality materials that can withstand low temperatures, and the design incorporates measures to prevent heat transfer from the warm environment to the sensor stand, which could affect the accuracy of the measurements.

<div align="center">
  <img src="https://github.com/user-attachments/assets/ad66db74-5ed6-44bf-a429-d2edd68d8ccd" alt="image" width="400"/>
</div>

The Cryogenic Measurement System designed and installed at ABBNIROO has been in operation since 2016 and has been a remarkable success. The system has been operating flawlessly without any failure, providing accurate real-time data to the plant operators.

<div align="center">
  <img src="https://github.com/user-attachments/assets/b3010900-9399-457b-b598-2dcd0b5469d5" alt="image" width="400"/>
</div>

The system's FPGA and microcontroller-based hardware design, along with the Magnetic Reluctance Sensor and its stand, have proven to be highly reliable and accurate in the challenging cryogenic environment. The Altium-designed PCBs have also demonstrated excellent signal integrity and stability, ensuring precise measurement and control of the cryogenic process.
The specialized Keil software design used for the microcontroller has provided efficient and reliable communication between the different components of the system, allowing for real-time data acquisition and control.

## Reliable Operation and Continuous Performance:

The success of the Cryogenic Measurement System has resulted in increased efficiency and productivity in the Cryogenic Plants-Air Separation process, improving the overall performance of the petrochemical plant. The system's ability to provide accurate real-time data has allowed operators to optimize the process, resulting in reduced energy consumption and improved product quality.

<div align="center">
  <img src="https://github.com/user-attachments/assets/9d31307d-d3d2-462c-8b0f-fb2f25fdb9b1" alt="image" width="400"/>
</div>

## Acknowledgments
We would like to express our deepest gratitude to everyone who contributed to the success of this project. First and foremost, we would like to thank ABBNIROO for their unwavering support throughout the project. Their expertise in the petrochemical industry and their commitment to excellence have been invaluable to the success of the project.
We would also like to extend our appreciation to the team members who worked tirelessly to design, install, and maintain the Cryogenic Measurement System. Their hard work, dedication, and expertise were instrumental in ensuring the system's accuracy and reliability in extreme temperatures.

<div align="center">
  <img src="https://github.com/user-attachments/assets/332126e9-b106-4d73-a545-5232f3742f55" alt="image" width="400"/>
</div>

Lastly, we would like to thank our colleagues at the +55°C environment who worked alongside us during the installation and testing phases. Their support and encouragement helped us overcome the challenges of working in such extreme conditions.
Thank you all for your invaluable contributions to the project's success. We are proud to report that the Cryogenic Measurement System has been working flawlessly since its installation in 2016, even in the harshest environments.


