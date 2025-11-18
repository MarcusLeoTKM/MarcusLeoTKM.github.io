---
layout: default
---

## Business Card V2
Jun 2025 - Jul 2025


<div style="display: grid; grid-template-columns: repeat(6, 1fr); gap: 10px; max-width: 240px; margin-bottom: 24px;">
    <img src="assets/img/stm32cubeide-logo.png" alt="STM32CubeIDE" style="width: 28px;">
    <img src="assets/img/BusinessCard/logo.jpg" alt="STM32CubeIDE" style="width: 28px;">
    <img src="assets/img/altium-logo.png" alt="Altium Designer" style="width: 120px; horizontal-align: middle;">
</div>
          
<img src="/assets/img/BusinessCard/BusinessReal.jpeg" alt="SAM PCB" style="height: 280px; border-radius: 10px;">

This is my own business card, designed to be the size of a credit card, easy to carry and quick to show. The board is programmed (using an external ST-Link device) to blink when plugged into USB. 

<img src="/assets/img/BusinessCard/Flashed.jpeg" alt="SAM PCB" style="height: 280px; border-radius: 10px; margin-top:10px">


<div style="margin-top:20px"></div>
### Next Steps
<div style="margin-top:10px"></div>
While the current version functions as a "LED" board, my goal is to turn it into a  controller that I can carry with me and use to program peripheral devices anytime.
The board already supports several communication protocols, including SPI and I2C.
The next step is to have data readings to appear on my host computer. This would involve adding a UART-to-USB chip, the supporting circuitry, and having a USB port for wired communication.
<div style="margin-top:10px"></div>
[Back](./AESN.html)
