# Hi, I'm Armaan 👋

I'm a Mechatronics Engineering student at the University of Waterloo with a focus on **embedded systems, robotics, control systems**, and **hardware-software integeration**. I enjoy building systems that interact with the real world — whether that’s flight computers for rockets, wearable human-body communication devices, or autonomous robots.

I like working across the stack:
- **Firmware & Real-Time Systems** (C / C++ / FreeRTOS / STM32 / Apollo / ESP32)
- **Electronics & PCB Design** (KiCad / Altium / RF & mixed-signal basics)
- **Controls, Signal Processing & State Estimation** (Matlab, Simulink/Simscape)
- **Mechanical Design & Prototyping** (SolidWorks, Ansys FEA)
- **Python for tooling, simulation & visualization**

For more projects and details, see my portfolio:  
➡️ **https://www.armaansengupta.ca**  

---

## 🚀 Personal Projects

### **Waterloo Rocketry — Flight Controls & Avionics**
<img width="960" height="540" alt="Render8 - Transparent" src="https://github.com/user-attachments/assets/66f75393-6337-44ef-96fb-903af4becb5e" />

Designing and implementing **real-time control firmware** and **state estimation** for high-powered rockets.  
- Developed C code for an STM32 using FreeRTOS to manipulate aerodynamic control surfaces 
- Modelled mechanism to synchronously extend 3 fins from rocket using one input source (Solidworks)
- Designed 4 layer central processing board PCB in KiCad improving power efficiency from 66% to 95% and incorporated an onboard IMU over I2C, as well as an external AHRS through UART (KiCad)
- Used Ansys fluid to determine center of pressure and (CD) to validate rocket stability
**Tech:** STM32, C, FreeRTOS, I2C/SPI, Kalman, Control Systems, KiCad, Solidworks
  
➡️ [Github Repo](https://github.com/waterloo-rocketry/cansw_processor_airbrakes)

➡️ [Summary of work done](https://www.armaansengupta.ca/rocketry)

➡️ [Recording of my Technical Presentation](https://youtu.be/SJO39WQ7Uv0)

### **Stewart Platform (3RRS Parallel Manipulator)**
#### Beam Balancer (1D balancing)
Precursor to 2D balancing on the Stewart Platform

<!-- https://github.com/user-attachments/assets/43cd8d4b-1a0e-4b65-b54a-896c95f36b8b -->

https://github.com/user-attachments/assets/217bb178-2515-490d-b472-e8f45d9d0ff4
<!-- <img width="1920" height="1080" alt="BeamBalancer_v1_2025-Sep-23_05-06-24PM-000_CustomizedView1830236967_png_alpha" src="https://github.com/user-attachments/assets/859bed5d-b440-46a3-9f53-88d14fb876c6" /> -->

- Modeled mechanism in SolidWorks
- Designed and tuned control system to stabilize ball at center position
- Wrote embedded firmware for servo actuation and real-time control
- Used OpenCV for ball position tracking and feedback
- **Tech:** C for firmware, Python + OpenCV for vision, SolidWorks CAD, PID control tuning, RC servo actuation, USB/serial telemetry

➡️ [Video demo](https://youtube.com/shorts/xsgP9gpsP7k)

#### Stewart Platform (2d Balancing)
Work in progress, but here is a sneak peak of the controller/simulation developed in Simulink + Simscape, the inverse kinematics developed in Python, and the ball position sensing using a ForceN force/torque sensor with some custom Python code:

➡️ [Inverse kinematics video demo](https://youtu.be/Ilx4d0JpWdY)

➡️ [Simscape/Simulink control system simulation demo](https://youtu.be/-PhUBZktgj0)

➡️ [Ball position sensing using force + torque sensor from ForceN](https://youtube.com/shorts/4DZ4b8GL0lY?feature=share)

**Tech:** MATLAB/Simulink + Simscape for dynamics + control, Python for inverse kinematics + sensor/servo interface, Force/Torque sensing, Embedded C for actuator control, SolidWorks CAD

### **Automated Measurment System**

https://github.com/user-attachments/assets/4df2ce54-e8ce-4e35-bba4-809914436cb7

- Wrote C code to control both motors (clamp + turntable), derive object dimensions from encoder values, and user GUI
- Designed and implemented a custom 2 wire communication protocol (C++ & C) (similar to I2C)
- Determined object orientation in OpenCV (Python)
- Accurately rotated objects 100% of the time during testing as well as measured results within 0.3mm of true value
**Tech:** C, C++, Python, OpenCV, Encoder feedback, Motor control firmware
  
➡️ [Video demo](https://youtu.be/MB9A7U8ksmc)

➡️ [Technical writeup](https://drive.google.com/file/d/1Ytp4l94ol0VdSAHArLPGi6ToqCvMx83w/view)

### **LiDAR Data Processing**
<img width="1836" height="814" alt="image" src="https://github.com/user-attachments/assets/f468b698-fdc3-4e41-bd0a-bef9da29bdc2" />

- Used Python with laspy, open3D, and numpy
  - laspy: tool for LiDAR data handling and analysis
  - open3D: 3D data processing and visualization
- Manipulation, cleansing, filtering, and analysis of LiDAR point cloud data
- Applied voxel grouping to downsize the data
- Removed artifacts such as dust using a nearest neighbour outlier algorithm
- Found the furthest point within a region to any other point in the data set using a custom algorithm to vastly decrease time complexity (essential for 1M+ points)

**Tech:** Python, laspy, Open3D, NumPy, point cloud filtering & voxel downsampling, nearest-neighbor outlier removal, custom optimized spatial search algorithms

➡️ [Project repo + explination of work](https://github.com/Armaan-Sengupta/Fyelabs-Project/blob/master/README.md)

➡️ [View the point cloud I worked with in browser](http://lidarview.com/?url=armaan-sengupta.github.io/Fyelabs-Project/CaliforniaBuildingsOnly.las)

➡️ [View LiDAR implementation on physical hardware](https://www.armaansengupta.ca/fyelabs#:~:text=out%2C%20as%20shown-,below,-%3A)

## **VIEW MORE PROJECTS ON [MY WEBSITE](https://www.armaansengupta.ca/)**
---

## 🧰 Core Skills

| Area | Tools / Tech |
|------|--------------|
| Embedded Firmware & RTOS | C, C++, FreeRTOS, Bare-metal, CMake, Pytest |
| Microcontrollers & Platforms | STM32, NXP, Ambiq Apollo, ESP32, AVR |
| Communication & Interfaces | I2C, SPI, UART, CAN, PWM, BLE, MIPI DSI, JTAG |
| Electronics & Hardware | KiCad, Altium, EasyEDA, JLCPCB, Oscilloscope & Logic Analyzer Debug |
| Control Systems & Estimation | PID, Model-based control, Kalman Filters, Simulink/Simscape, MATLAB |
| Data, Simulation & Visualization | Python (NumPy, Pandas, SciPy, Open3D, laspy, Matplotlib), PostgreSQL |
| Mechanical & CAD | SolidWorks, Fusion 360, Inventor, Onshape, Ansys, 3D Printing & CNC workflows |

---

## 🔗 Links

- **Portfolio:** https://www.armaansengupta.ca
- **LinkedIn:** https://www.linkedin.com/in/armaan-sengupta/
- **Youtube:** https://www.youtube.com/@armaansengupta
- **GitHub:** you’re here :)

---

## 📬 Contact

Feel free to reach out — I like talking about **embedded systems, rocketry, robotics, wearables, and control systems**.  
If you're working on something interesting, I probably want to hear about it.

[senguptaarmaan@gmail.com](mailto:senguptaarmaan@gmail.com?subject=Hey%20I%20saw%20you%20were%20working%20on%20xyz%2C%20and%20I%20was%20intrested%20in%20abc)
