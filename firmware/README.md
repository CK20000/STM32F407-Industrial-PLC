# STM32F407 PLC Firmware

Firmware source code will be added here. 

### Planned Stack
* **HAL/LL Driver Base:** STM32CubeF4 / Bare-metal C/C++.
* **Peripherals:** 
  * `USART2`: RS-485 Transceiver (Modbus RTU).
  * `USART3`: ESP-12S AT Commands / Wi-Fi bridge.
  * `SPI1`: W25Q80DV NVM storage.
  * `ADC1/2`: 8-Channel DMA scanning for 0–10V inputs.
  * `GPIO Port E`: Isolated digital I/O handling.