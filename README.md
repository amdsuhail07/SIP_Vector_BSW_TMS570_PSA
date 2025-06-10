# BSW_TMS570_PSA

Automotive Basic Software (BSW) modules for the Texas Instruments TMS570 microcontroller platform, tailored for PSA (Peugeot Société Anonyme) automotive requirements. This repository provides core communication, transport, and diagnostic layers, including PSA-specific network management and application interfaces.

## Features

- **PSA Station Manager:** Application interface and management for PSA Low Speed Fault Tolerant Bus ([BSW/Nm/Stat_mgr.h](BSW/Nm/Stat_mgr.h))
- **CAN Communication:** Includes Vector Interaction Layer ([BSW/Il/il.c](BSW/Il/il.c), [BSW/Il/il_def.h](BSW/Il/il_def.h))
- **Transport Protocol:** ISO 15765-2 (CAN TP) transport layer ([BSW/Tp/tpmc.c](BSW/Tp/tpmc.c))
- **XCP Support:** XCP on CAN transport and protocol layers ([BSW/Xcp/xcp_can.c](BSW/Xcp/xcp_can.c), [BSW/Xcp/xcp_can.h](BSW/Xcp/xcp_can.h), [BSW/Xcp/XcpProf.c](BSW/Xcp/XcpProf.c), [BSW/Xcp/_xcp_appl.c](BSW/Xcp/_xcp_appl.c))
- **Low-Level Utilities:** Vector standard library, ARM-specific ([BSW/VStdLib/vstdlib_lib.asm](BSW/VStdLib/vstdlib_lib.asm))
- **Delivery Documentation:** Includes delivery and build information ([Doc/DeliveryInformation/DeliveryDescription_CBD1300660.html](Doc/DeliveryInformation/DeliveryDescription_CBD1300660.html))

## Project Structure (partial)
```
BSW/
  ├── Il/          # Interaction Layer (il.c, il_def.h)
  ├── Tp/          # Transport Protocol (tpmc.c)
  ├── Xcp/         # XCP Protocol and CAN adaption (xcp_can.c, xcp_can.h, XcpProf.c, _xcp_appl.c)
  ├── Nm/          # PSA Station Manager (Stat_mgr.h)
  └── VStdLib/     # Vector standard library (vstdlib_lib.asm)
Doc/
  └── DeliveryInformation/ # Delivery documentation
```
> **Note:** Only a subset of files/folders is shown.  
> For the full structure, browse the repo.

## Documentation

- **Delivery Description:**  
  [Doc/DeliveryInformation/DeliveryDescription_CBD1300660.html](Doc/DeliveryInformation/DeliveryDescription_CBD1300660.html)

## Getting Started

### Prerequisites

- **Hardware:** TI TMS570 series microcontroller (e.g., 0812BPGEQQ1)
- **Compiler:** Texas Instruments 4.9.5
- **Environment:** Suitable for integration with Vector CANbedded stack and PSA automotive projects

### Usage

- Integrate the BSW modules with your automotive ECU application.
- Use the Station Manager (`BSW/Nm/Stat_mgr.h`) for PSA-specific network management.
- Include the Interaction and Transport Layer modules for CAN communication and diagnostics.
- The XCP modules enable measurement and calibration over CAN.

## License

This project is licensed under the MIT License.  
See [LICENSE](LICENSE) for details.

## Disclaimer

Some files are provided “as is” and without warranty.  
See module headers and delivery documentation for details.

---

*If you add new documentation, place it in the `Doc/` directory and update this README.*
