# STM32F407 Modular Industrial PLC

A student-accessible, ruggedized industrial PLC platform built around the STM32F407VET6 microcontroller. Designed for educational lab environments, industrial communication protocols, and industrial automation tasks.

<img width="773" height="813" alt="image" src="https://github.com/user-attachments/assets/c0478a95-5cea-4e24-bb1f-b9777cde5e3c" />

## Core Specifications
* **MCU:** STM32F407VET6 (ARM Cortex-M4 with FPU, 168 MHz, 512KB Flash, 192KB RAM).
* **Isolation:** Optocoupler-isolated digital inputs and low-side outputs.
* **Industrial Bus:** RS-485 half-duplex communication (MAX3485) with selectable 120Ω termination.
* **Wireless:** ESP-12S Wi-Fi module tied via isolated solder-jumper UART paths.
* **Analog Interface:** 8 buffered analog inputs (0–10V rated) with overvoltage protection.
* **Memory:** Onboard W25Q80DV NOR Flash for non-volatile parameter storage.
* **Programming:** SWD debug header (SWDIO/SWCLK) and USB-C DFU interface.

## Repository Organization
* `hardware/`: KiCad schematic files, PCB layout, Gerber outputs, and BOM.
* `firmware/`: MCU driver code and demonstration firmware (TBD).
* `datasheets/`: Reference datasheets for core integrated circuits.

## License
Open-source hardware released under the CERN-OHL-S v2 license.
