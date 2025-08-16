# Hardware Builds Repository

A collection of robot build documentation, including Bills of Materials (BOMs), assembly guides, and supporting resources for educational robotics projects.

## Repository Structure

```
hardware-builds/
├── README.md                 # This file
├── boms/                     # Bill of Materials documents
│   └── mobile-base-sensors-v1.md
├── builds/                   # Complete build documentation
├── guides/                   # Step-by-step assembly guides
├── images/                   # Photos and diagrams
└── resources/               # Supporting materials
    ├── datasheets/          # Component datasheets
    └── schematics/          # Circuit diagrams and PCB files
```

## Directory Descriptions

### `/boms/`
Contains detailed Bills of Materials for various robot builds. Each BOM includes:
- Complete component lists with suppliers and pricing
- Assembly notes and power requirements
- Tool requirements and safety considerations
- Version history for tracking changes

### `/builds/`
Complete build documentation combining BOMs, guides, and additional resources for specific robot configurations.

### `/guides/`
Step-by-step assembly instructions, including:
- Hardware assembly procedures
- Software setup and configuration
- Troubleshooting guides
- Testing and calibration procedures

### `/images/`
Visual documentation including:
- Assembly photos
- Wiring diagrams
- Component identification images
- Completed build photos

### `/resources/`
Supporting technical documentation:
- **`datasheets/`**: Component specifications and technical data
- **`schematics/`**: Circuit diagrams, PCB layouts, and electrical designs

## Current Builds

### Mobile Base + Sensors v1.0
**Purpose:** Educational robotics platform for first in-person course
**BOM:** [`boms/mobile-base-sensors-v1.md`](boms/mobile-base-sensors-v1.md)

**Key Features:**
- Differential drive mobile platform
- Raspberry Pi 5 with AI HAT+ for computation
- Stereo vision camera system
- 9DOF IMU for navigation
- Optional robot arm attachment
- Real-time motor control via Teensy 4.0

## Contributing

When adding new builds or updating existing documentation:

1. **BOMs**: Create versioned files in `/boms/` with detailed component information
2. **Images**: Store in `/images/` with descriptive filenames
3. **Guides**: Use clear step numbering and include safety warnings
4. **Resources**: Organize datasheets and schematics in appropriate subdirectories

## Safety Notes

⚠️ **Important Safety Considerations:**
- Always follow proper LiPo battery handling procedures
- Ensure emergency stops are accessible and functional
- Use appropriate safety equipment when soldering or assembling
- Verify power connections before applying power
- Keep datasheets accessible during assembly

## License

This repository contains educational materials for robotics instruction. Please respect component manufacturer trademarks and licensing when using this documentation.

---
*Repository maintained for educational robotics courses*
