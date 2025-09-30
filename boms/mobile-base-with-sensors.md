# Mobile Base + Sensors BOM v1.2

**Build Date:** Sept 2025
**Course:** Engineer Boldly: AI Robotics Sprint

⚠️ Note: Time costs and materials are best estimates ⚠️

- **Minimum Required Materials Cost:** $760
- **Electronics Board Assembly:** $200
- **Taxes \ Tariffs \ Shipping** $25
- **Mobile Base Assembly Time:** ~4 hours
- **Assembled Cost:** ~$985

## Overview
This Bill of Materials (BOM) covers all components required for building a mobile robotic platform with sensors, suitable for educational robotics courses. The build includes a differential drive mobile base, onboard computing, vision sensors, and an optional manipulator arm.

> 🤖 **Inspired by the [Portland Area Robotics Society Common Platform](https://github.com/portlandrobotics/common_platform)**
> This BOM builds upon the excellent work of our friends at P.A.R.T.S., adapting their proven Romi-based design for our educational robotics course.

<br/>

*Mobile base platform*

<img src="/images/stack_platform_unassembled.jpg" width="500"
     alt="Mobile base platform"
     width="500">


*Assembled chassis*

<img src="/images/stack_with_controller.jpg"
     alt="Mobile base platform assembly"
     width="500">

*Custom PCB showing integrated motor drivers and controller connections, Teensy MCU*

<img src="/images/stack_ports_plus_controller.jpg"
     alt="Custom PCB with ports and controller"
     width="500">


## Open Source Hardware Components

**📋 Complete Bill of Materials**
The detailed component list with part numbers, quantities, and suppliers is maintained in our GitHub repository: [BOM.csv](https://github.com/RoseCityRobotics/common_platform/blob/main/BOM.csv)

## Assembly Notes

### Power Distribution
- Main battery provides 14.8V for motors
- 5V regulator powers Raspberry Pi and sensors
- Teensy powered via USB from Raspberry Pi

### Communication
- Teensy handles real-time motor control
- Pi communicates with Teensy via USB serial
- IMU connects via I2C to Teensy
- Camera connects directly to Pi camera port

### Motor Control
- Differential drive configuration
- Encoder feedback for odometry
- TB9051FTG drivers support PWM speed control

## Required Tools
- Soldering iron and supplies
- Small screwdrivers (Phillips and flathead)
- Wire strippers
- Multimeter
- Hot glue gun (for cable management)

## Visual References

*Mobile base platform*

<img src="/images/stack_platform_unassembled.jpg"
     alt="Mobile base platform"
     width="450">

*Completed chassis - top view Halo, Chip Raspberry Pi AI HAT+*

<img src="/images/stack_top.jpg"
     alt="Assembled Platform - Top View"
     width="450">

*Completed chassis - ports view*

<img src="/images/stack_ports_plus_controller.jpg"
     alt="Assembled Platform - Ports and Controller"
     width="450">

*Completed chassis - side view - Play Station controller*

<img src="/images/stack_with_controller.jpg"
     alt="Assembled Platform - Side View"
     width="300">

*Raspberry Pi 5 with AI HAT+*

<img src="/images/raspberry_pi_ai.jpg"
     alt="Raspberry Pi 5 with AI HAT+"
     width="450">

*Raspberry Pi 5 Ports*

<img src="/images/raspberry_pi.jpg"
     alt="Raspberry Pi 5"
     width="450">

*Back view - showing rear components and connections*

<img src="/images/back_image.jpg"
     alt="Back view of mobile base"
     width="450">

*Side view with LiDAR sensor mounted*

<img src="/images/side_image_lidar.jpg"
     alt="Side view with LiDAR sensor"
     width="450">


### Thank you PARTS

<img src="https://raw.githubusercontent.com/portlandrobotics/common_platform/master/github/img/PARTS.png"
     alt="Portland Area Robotics Society (P.A.R.T.S.)"
     width="300">

*Portland Area RoboTics Society (PARTS)*
Our work is based on the [PARTS Common Platform](https://github.com/portlandrobotics/common_platform)


🔗 **[Rose City Robotics Fork - Common Platform](https://github.com/rosecityrobotics/common_platform)**
Complete open-source robotics platform with detailed assembly guides, 3D models, and ROS2 integration.

## Safety Considerations
- LiPo battery requires proper charging and storage
- Always use battery protection circuit
- Ensure proper power switch accessibility
- Include emergency stop functionality in software

📚 **Additional Documentation:**
- [PARTS Interactive BOM](https://github.com/rosecityrobotics/common_platform) - Detailed assembly guide
- [Hardware Documentation](https://github.com/rosecityrobotics/common_platform/tree/master/hardware) - PCB designs and schematics
- [Firmware Examples](https://github.com/rosecityrobotics/common_platform/tree/master/firmware) - Arduino and PlatformIO code

## Image Credits

Component images from [Pololu Corporation](https://www.pololu.com) product pages.

## Version History
- v1.1: Initial BOM for first in-person course (Sept 2025)
- v1.2: Final BOM for first in-person course (Sept 2025)

---
*Last updated: Sept 2025*
