# STM32F407 Modular Industrial PLC

A student-accessible, ruggedized industrial PLC platform built around the STM32F407VET6 microcontroller. Designed for educational lab environments, industrial communication protocols, and industrial automation tasks.

<img width="1289" height="682" alt="image" src="https://github.com/user-attachments/assets/7b7885c3-b70e-4867-8ba2-18b950225cf8" />

## Core Specifications
* **MCU:** STM32F407VET6 (ARM Cortex-M4 with FPU, 168 MHz, 512KB Flash, 192KB RAM).
* **Isolation:** 
  * 8 Opto-isolated digital inputs (PE0–PE7) using PC817 channels.
  * 8 Opto-isolated low-side digital outputs (PE8–PE15) using PC817 channels.
  * 4 Isolated high-speed PWM channels for precision motor/servo control (6N137 optocouplers).
* **Analog Interface:** 
  * 8 Buffered analog inputs (0–10V rated) with resistor dividers and 3.3V Zener clamping.
  * 2-Channel Analog DAC outputs (0–10V scale) driven via onboard LM358 op-amp stage.
* **Onboard Communication & Expansion:**
  * **RS-485:** Half-duplex transceiver (MAX3485) with selectable 120Ω termination resistor.
  * **Wi-Fi:** ESP-12S module connected via UART (USART3) with solder-jumper isolation paths.
  * **I2C Bus:** Routed to PB6 (SCL) and PB7 (SDA) for OLED/peripheral expansion.
  * **SPI Bus:** SPI2 routed to PB13 (SCK), PB14 (MISO), and PB15 (MOSI) for external IO expansion modules.
* **Memory & Storage:** Onboard 8 Mbit (1 MB) Winbond W25Q80DV NOR Flash connected via SPI1.
* **Programming & Debug:** Dedicated 4-pin SWD debug header (SWDIO/SWCLK) and USB-C DFU interface.

## Repository Organization
* `hardware/`: KiCad schematic files, PCB layout, Gerber outputs, and BOM.
* `firmware/`: MCU driver code and demonstration firmware (TBD).
* `datasheets/`: Reference datasheets for core integrated circuits.
