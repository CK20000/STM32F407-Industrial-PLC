# STM32F407 Industrial PLC - Hardware Documentation

This directory contains all electronic and mechanical design files for the STM32F407VE Industrial PLC board.

## Block Overview
* **Microcontroller:** STM32F407VET6 (LQFP-100) running at 168 MHz.
* **Power Supply:** USB-C (5V) / External 12V terminal block with onboard buck regulation.
* **Communications:** RS-485 (MAX3485), ESP-12S (Wi-Fi), USB 2.0 FS, I2C, SPI.
* **Storage:** 8 Mbit (1 MB) Winbond W25Q80DV SPI Flash.
* **Analog Inputs:** 8-Channel 0–10V scale (PC0–PC5, PB0–PB1) with resistor dividers and 3.3V Zener clamping.
* **Digital I/O:** 8 Opto-isolated Inputs (PE0–PE7) and 8 Opto-isolated Outputs (PE8–PE15) using PC817 channels.

## Board Layout & Routing Rules
1. **Isolation Barrier:** A 3mm copper keepout zone separates Field Ground (12V/24V) from MCU Ground (3.3V) underneath the optocouplers.
2. **RF Keepout:** No ground planes or traces are present beneath the ESP-12S PCB antenna section.
3. **Power Traces:** 3.3V and 5V power rails use minimum 0.5mm trace widths.