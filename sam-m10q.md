---
layout: default
---


## SAM M10Q GNSS Module
Jul 2025 - Aug 2025


<div style="display: grid; grid-template-columns: repeat(6, 1fr); gap: 10px; max-width: 240px; margin-bottom: 24px;">
    <img src="assets/img/stm32cubeide-logo.png" alt="STM32CubeIDE" style="width: 28px;">
    <img src="assets/img/UBC/UBCRocketsLogo.png" alt="UBC Rocket" style="width: 30px;">
    <img src="assets/img/altium-logo.png" alt="Altium Designer" style="width: 120px;">
</div>

<div style="display: flex; overflow-x: auto; gap: 10px; padding: 10px; max-width: 100%; aspect">
  <img src="/assets/img/UBC/SAM.png" alt="Testing the module" style="border-radius: 10px; height: 280px;">
  <img src="/assets/img/UBC/GPS-V2.png" alt="SAM PCB" style="height: 280px; border-radius: 10px;">
  <!-- Add more images here -->
</div>



This was a very straightforward project, the rocket collects location and time data from GNSS satellites (GPS, Beidou, etc.) and sends it back via the onboard radio. My part was to design the PCB that hosts the SAM-M10Q GNSS module and later program it to fetch the location and time data. The module starts transmission as soon as it's powered and connected via UART.

The return messages are written in NMEA format, which starts with different sentence types, such as GNGLL (shows latitude and longtitude), GNRMC (shows location and time), GNGSA (shows available satellites). I had to locate the lines starting with GNRMC and reformat them so they could be used by the FC.

<img src="/assets/img/UBC/SAM-output.jpg" alt="Branching" width="500" style="border-radius: 10px; vertical-align: middle;">

015201.00 was the time when I was testing it. 4916.00492 N and 12315.14884 W represent the geolocation in DMM (Degrees and Decimal Minutes) format. 140825 is the date (August 14, 2025). 
 
The default settings allow the module to work right out of the box. However, we needed a faster update and output rate, which required modifying the stored configuration items (similar to registers). The way to configure them is included in here
 <a href="https://github.com/MarcusLeoTKM/SAM-M10Q">
SAM GitHub project
    <img src="assets/img/link.png" alt="link" style="width: 10px;">

<div style="margin-top:10px"></div>
[Back](./)
