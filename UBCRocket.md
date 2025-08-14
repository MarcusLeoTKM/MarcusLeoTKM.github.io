---
layout: default
---

## UBC Rocket
May 2025 - Aug 2025


<div style="display: grid; grid-template-columns: repeat(6, 1fr); gap: 10px; max-width: 240px; margin-bottom: 24px;">
    <img src="assets/img/UBC/UBCRocketsLogo.png" alt="UBC Rocket" style="width: 30px;">
</div>

I had four awesome months at UBC Rocket, participated in two projects and a test launch in Oregon. I did a lot of soldering work and had some very valuable hands-on time with PCBs. 

Later on, I started using Altium to make my own boards, including the <a href="./sam-m10q.html">SAM M10Q GNSS Module</a>. In the end, I programmed and tested it using a nucleo board, the STM32 L4R5ZIT6 via UART. It’s ready to be flown in this year’s rocket at Launch Canada.
<div style="margin-bottom: 30px;"></div>

### Soldering
Soldered Radio, BMS, Buck Converter, GNSS Module and Vector Thrust boards.

A little technique for soldering a 0402 component is to first apply a thin layer of solder to the pads using a soldering iron, then, place the 0402 on the pad and use a heat gun to melt the solder underneath, allowing the component to attach. No hot plate needed.

<div style="display: flex; overflow-x: auto; gap: 10px; padding: 10px; max-width: 100%; aspect">
  <img src="/assets/img/UBC/Radio.png" alt="NAS view 1" style="height: 280px; border-radius: 10px;">
  <img src="/assets/img/UBC/BuckConverter.png" alt="NAS view 2" style="height: 280px; border-radius: 10px;">
  <!-- Add more images here -->
</div>

<div style="margin-top: 40px"></div>

### PCB Design
 <a href="./sam-m10q.html">
SAM-M10Q GNSS module 
    <img src="assets/img/link.png" alt="link" style="width: 10px;">



For optimal RF performance, the manual suggests using a 5 by 5 cm layout with stitching vias.

<div style="display: flex; overflow-x: auto; gap: 10px; padding: 10px; max-width: 100%; aspect">
  <img src="/assets/img/UBC/GPS-V2.png" alt="NAS view 1" style="height: 280px; border-radius: 10px;">
  <!-- Add more images here -->
</div>

<div style="margin-top: 40px"></div>

[Back](./)
