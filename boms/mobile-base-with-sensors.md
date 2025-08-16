# Mobile Base + Sensors BOM v1.0

**Build Date:** Aug 2025
**Course:** Engineer Boldly: AI Robotics Sprint

⚠️ Note: Time costs and materials are best estimates ⚠️

- **Materials Cost:** $700
- **Electronics Board Assembly Time:** 4 hours
- **Mobile Base Assembly Time:** not yet tested
- **Assembled Cost:** $1,???

## Overview
This Bill of Materials (BOM) covers all components required for building a mobile robotic platform with sensors, suitable for educational robotics courses. The build includes a differential drive mobile base, onboard computing, vision sensors, and an optional manipulator arm.


> 🤖 **Inspired by the [Portland Area Robotics Society Common Platform](https://github.com/portlandrobotics/common_platform)**
> This BOM builds upon the excellent work of our friends at P.A.R.T.S., adapting their proven Romi-based design for our educational robotics course.

<br/>

<img src="https://raw.githubusercontent.com/portlandrobotics/common_platform/master/github/img/romi-2.jpg"
     alt="Mobile base platform assembly"
     width="500">

*Mobile base platform assembly - Image from Portland Area Robotics Society*

## Component Categories

### Core Platform
| Item | Description | Quantity | Unit Price | Total | Supplier |
|:-----|:------------|:--------:|:----------:|:-----:|:---------|
| [Romi Chassis Kit](https://www.pololu.com/category/203/romi-chassis-kits) | Primary chassis platform | 1 | $39.95 | $39.95 | Pololu |
| [Romi Chassis Caster](https://www.pololu.com/product/3530) | Rear support caster wheel | 1 | $3.95 | $3.95 | Pololu |
| [Romi Encoder Pair](https://www.pololu.com/product/3542) | Wheel encoder sensors | 1 | $9.95 | $9.95 | Pololu |
| [SparkFun Chassis](https://www.sparkfun.com/products/16405) | **[Optional]** Alternate chassis platform | 1 | $14.95 | $14.95 | SparkFun |

### Motor Control & Power

<img src="https://raw.githubusercontent.com/portlandrobotics/common_platform/master/github/img/PARTS-board.png"
     alt="PARS Custom PCB"
     width="400">

*Portland Robotics custom carrier PCB showing integrated motor drivers and Teensy mount*

| Item | Description | Quantity | Unit Price | Total | Supplier |
|:-----|:------------|:--------:|:----------:|:-----:|:---------|
| [TB9051FTG Motor Driver](https://www.pololu.com/product/2997/resources) | Single brushed DC motor driver | 2 | $11.95 | $23.90 | Pololu |
| [5V Step-Down Regulator](https://www.pololu.com/product/2858/resources) | Pololu D24V22F5 2.5A regulator | 1 | $8.95 | $8.95 | Pololu |
| [SPDT Slide Switch](https://www.pololu.com/product/1408) | Power switches | 2 | $1.69 | $3.38 | Pololu |
| [IRFU5505PBF MOSFET](https://www.digikey.com/product-detail/en/infineon-technologies/IRFU5505PBF/IRFU5505PBF-ND/812417) | Power switching transistor | 2 | $0.86 | $1.72 | Digikey |
| [LiPo Battery](https://www.getfpv.com/lumenier-5200mah-4s-35c-lipo-battery.html) | 14.8V 5200mAh power source | 1 | $93.49 | $93.49 | GetFPV |

### Computing & Processing
| Item | Description | Quantity | Unit Price | Total | Supplier |
|:-----|:------------|:--------:|:----------:|:-----:|:---------|
| [Teensy 4.0](https://www.pjrc.com/store/teensy40.html) | Real-time motor control MCU | 1 | $23.80 | $23.80 | PJRC |
| [Raspberry Pi 5 16GB](https://www.pishop.us/product/raspberry-pi-5-16gb/) | Main computer with cooler & PSU | 1 | $144.90 | $144.90 | PiShop |
| [Raspberry Pi AI HAT+](https://www.pishop.us/product/raspberry-pi-ai-hat-26-tops/) | 26 TOPS AI acceleration | 1 | $119.95 | $119.95 | PiShop |

### Sensors
| Item | Description | Quantity | Unit Price | Total | Supplier |
|:-----|:------------|:--------:|:----------:|:-----:|:---------|
| [MPU-9250 IMU](https://www.amazon.com/HiLetgo-Gyroscope-Acceleration-Accelerator-Magnetometer/dp/B01I1J0Z7Y) | 9DOF inertial measurement unit | 1 | $14.99 | $14.99 | Amazon |
| [Pi HQ Camera](https://www.pishop.us/product/imx219-83-stereo-camera-8mp-binocular-camera-module-depth-vision/) | High quality camera module | 1 | $53.95 | $53.95 | PiShop |

**Camera Accessories (Included):**
- SKU: 942-1: 2.7mm 12MP Wide-Angle Lens
- SKU: 819-1: Universal Tilt-Adjustable Mount

### Custom PCB & Integration
| Item | Description | Quantity | Unit Price | Total | Supplier |
|:-----|:------------|:--------:|:----------:|:-----:|:---------|
| Motor Control PCB | Custom PCB for Teensy & drivers | 1 | $40.00 | $40.00 | Custom |

### Optional Manipulator

<img src="/images/arm-kit-romi.jpg"
     alt="Robot Arm Kit for Romi"
     width="350">

*Robot Arm Kit for Romi - Optional manipulator attachment*

| Item | Description | Quantity | Unit Price | Total | Supplier |
|:-----|:------------|:--------:|:----------:|:-----:|:---------|
| [Robot Arm Kit](https://www.pololu.com/product/3550) | Romi-compatible robot arm | 1 | $99.95 | $99.95 | Pololu |

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

<img src="https://raw.githubusercontent.com/portlandrobotics/common_platform/master/github/img/romi.png"
     alt="Assembled PARS Platform"
     width="450">

*Completed chassis*

### Thank you P.A.R.T.S

<img src="https://raw.githubusercontent.com/portlandrobotics/common_platform/master/github/img/PARTS.png"
     alt="Portland Area Robotics Society (P.A.R.T.S.)"
     width="300">

*Portland Area Robotics Society (P.A.R.T.S.)*

🔗 **[P.A.R.T.S. Common Platform](https://github.com/portlandrobotics/common_platform)**
Complete open-source robotics platform with detailed assembly guides, 3D models, and ROS2 integration.

## Safety Considerations
- LiPo battery requires proper charging and storage
- Always use battery protection circuit
- Ensure proper power switch accessibility
- Include emergency stop functionality in software

📚 **Additional Documentation:**
- [PARTS Interactive BOM](https://github.com/portlandrobotics/common_platform) - Detailed assembly guide
- [Hardware Documentation](https://github.com/portlandrobotics/common_platform/tree/master/hardware) - PCB designs and schematics
- [Firmware Examples](https://github.com/portlandrobotics/common_platform/tree/master/firmware) - Arduino and PlatformIO code

## Image Credits
Platform images sourced from the [Portland Area Robotics Society Common Platform Repository](https://github.com/portlandrobotics/common_platform) under MIT License.
Component images from [Pololu Corporation](https://www.pololu.com) product pages.

## Version History
- v1.0: Initial BOM for first in-person course (Aug 2025)

---
*Last updated: August 2025*
