# SIP_Vector_BSW_TMS570_PSA

![GitHub release](https://img.shields.io/github/v/release/amdsuhail07/SIP_Vector_BSW_TMS570_PSA?color=blue&style=flat-square) ![License](https://img.shields.io/github/license/amdsuhail07/SIP_Vector_BSW_TMS570_PSA?color=green&style=flat-square)

Welcome to the **SIP_Vector_BSW_TMS570_PSA** repository. This project provides essential Automotive Basic Software (BSW) modules designed specifically for the Texas Instruments TMS570 microcontroller platform, catering to the needs of PSA (Peugeot Société Anonyme). The repository includes core communication, transport, and diagnostic layers, featuring PSA-specific network management and application interfaces.

## Table of Contents

- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Directory Structure](#directory-structure)
- [Contributing](#contributing)
- [License](#license)
- [Support](#support)

## Features

This repository includes several key features:

- **PSA Station Manager:** Manages application interfaces for the PSA Low Speed Fault Tolerant Bus. See [BSW/Nm/Stat_mgr.h](BSW/Nm/Stat_mgr.h) for details.
  
- **CAN Communication:** Implements the Vector Interaction Layer. Check out [BSW/Il/il.c](BSW/Il/il.c) and [BSW/Il/il_def.h](BSW/Il/il_def.h) for more information.

- **Transport Protocol:** Provides ISO 15765-2 (CAN TP) transport layer. See [BSW/Tp/tpmc.c](BSW/Tp/tpmc.c) for the implementation.

- **XCP Support:** Offers XCP on CAN transport and protocol layers. Refer to [BSW/Xcp/xcp_can.c](BSW/Xcp/xcp_can.c), [BSW/Xcp/xcp_can.h](BSW/Xcp/xcp_can.h), [BSW/Xcp/XcpProf.c](BSW/Xcp/XcpProf.c), and [BSW/Xcp/_xcp_appl.c](BSW/Xcp/_xcp_appl.c) for details.

- **Low-Level Utilities:** Includes the Vector standard library tailored for ARM architectures. See [BSW/VStdLib/vstdlib_li](BSW/VStdLib/vstdlib_li) for more information.

## Installation

To get started with the **SIP_Vector_BSW_TMS570_PSA**, follow these steps:

1. **Clone the repository:**

   ```bash
   git clone https://github.com/amdsuhail07/SIP_Vector_BSW_TMS570_PSA.git
   ```

2. **Navigate to the project directory:**

   ```bash
   cd SIP_Vector_BSW_TMS570_PSA
   ```

3. **Install dependencies:** 

   Make sure you have the necessary development tools and libraries installed. You may need to install tools specific to the TMS570 platform.

4. **Build the project:** 

   Use your preferred build system to compile the project. Ensure you have the correct environment set up for ARM development.

5. **Download and execute the latest release:** 

   Visit the [Releases section](https://github.com/amdsuhail07/SIP_Vector_BSW_TMS570_PSA/releases) to download the latest version. Follow the instructions provided there to execute the software.

## Usage

After installation, you can start using the modules. Here are some examples of how to utilize the core features:

### PSA Station Manager

To use the PSA Station Manager, include the header file in your application:

```c
#include "BSW/Nm/Stat_mgr.h"
```

You can then initialize the manager and handle the communication as per the requirements of your application.

### CAN Communication

For CAN communication, include the relevant files:

```c
#include "BSW/Il/il.c"
#include "BSW/Il/il_def.h"
```

This will allow you to send and receive messages over the CAN bus.

### Transport Protocol

For using the ISO 15765-2 transport protocol, include:

```c
#include "BSW/Tp/tpmc.c"
```

Implement the transport layer in your application logic as needed.

### XCP Support

To use XCP, include the following files:

```c
#include "BSW/Xcp/xcp_can.c"
#include "BSW/Xcp/xcp_can.h"
```

This will provide you with the necessary functions to implement XCP communication.

## Directory Structure

The repository has a structured layout for easy navigation:

```
SIP_Vector_BSW_TMS570_PSA/
│
├── BSW/
│   ├── Il/
│   │   ├── il.c
│   │   └── il_def.h
│   ├── Nm/
│   │   └── Stat_mgr.h
│   ├── Tp/
│   │   └── tpmc.c
│   └── Xcp/
│       ├── xcp_can.c
│       ├── xcp_can.h
│       ├── XcpProf.c
│       └── _xcp_appl.c
└── BSW/VStdLib/
    └── vstdlib_li
```

## Contributing

We welcome contributions to enhance the functionality of this repository. If you want to contribute, please follow these steps:

1. **Fork the repository.**
2. **Create a new branch:**

   ```bash
   git checkout -b feature/YourFeature
   ```

3. **Make your changes and commit them:**

   ```bash
   git commit -m "Add your feature"
   ```

4. **Push to your branch:**

   ```bash
   git push origin feature/YourFeature
   ```

5. **Create a pull request.**

We appreciate your input and will review your contribution promptly.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Support

If you encounter any issues or have questions, feel free to open an issue in the repository. You can also visit the [Releases section](https://github.com/amdsuhail07/SIP_Vector_BSW_TMS570_PSA/releases) for the latest updates and downloads.

## Topics

This repository covers various topics relevant to automotive software development, including:

- autosar
- can-bus
- canbus
- electric-power-steering
- embedded-c
- embedded-systems
- iso26262
- motor-control
- texas-instruments
- tms570
- uds

## Acknowledgments

We thank the developers and contributors of the various libraries and standards that make this project possible. Your hard work is appreciated.

---

For more information and to keep up with the latest releases, visit the [Releases section](https://github.com/amdsuhail07/SIP_Vector_BSW_TMS570_PSA/releases).