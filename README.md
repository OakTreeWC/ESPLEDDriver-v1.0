# ESPLEDDriver-v1.0 (In Progress)
ESPLEDDriver is an ESP Powered LED Driver Board for both Addressable and Non-Addressable LEDS. It features a ESP32-WROOM, with either a built in antenna or u.fl port, as well as 4 mosfet channels for powering monochrome and multicolor leds. 
All GPIO pins are exposed directly to the IO headers on the right side, and all power/led related IO can be found on the left side via the screw terminals.
Components have been sized accordingly to support 5-30V input, and up to 5 amps of current draw.

[![View PCB on KiCanvas](https://hack.club/pcb-badge)](https://kicanvas.org/?repo=https://github.com/OakTreeWC/ESPLEDDriver-v1.0/tree/main/PCB)

## Firmware
Due to the PD complexity of adding a USBC port to this project, I refrained from adding one. However, that does mean that programming the board requires using a USB to UART adapter.

In terms of firmware to be run on this, I will be using WLED, but ESPHome or any other ESP based software can be used to control it as well.

## Usage
This can be used in multiple ways, but what I believe is the most interesting (and fun) way to do it is to just integrate it with [Home Assistant](https://www.home-assistant.io/). If you really wanted to though, you could just use the Web Interface of WLED, or make your own firmware with its own API or something. The possibilities are literally endless, which is what makes the ESP platform so great.

## I/O
|Pin Number|Function|
|----------|--------|
|0|Addressable LED Data Line|
|4|Non-Addressable LED Channel 1/Red|
|5|Non-Addressable LED Channel 2/Green|
|6|Non-Addressable LED Channel 3/Blue|
|7|Non-Addressable LED Channel 4/White|

All other non-strapping pins are just free, so one may use them for any other purpose.

## Bill Of Materials
W.I.P

## AI Usage Declaration
AI was used in the making of this project, in component research, schematic/pcb verification, general sanity checks, as well as some copilot commit notes (for readme)

## Gallery
<img width="3504" height="1398" alt="image" src="https://github.com/user-attachments/assets/d69baed3-e03a-434a-8e2d-4b0e415f2f66" />
<img width="3529" height="1429" alt="image" src="https://github.com/user-attachments/assets/7e1de9e2-824e-4bb6-82de-5f0e51a534b5" />

