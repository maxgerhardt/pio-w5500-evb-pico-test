# PlatformIO W5500-EVB-Pico Test

## Description

Test project for the WIZnet W5500-EVB-Pico board. Has built a Ethernet chip and jack!

## Prerequisites

WIZnet W5500-EVB-Pico board, micro-USB cable for power, ethernet cable for connecting it to a router, a router running a standard DHCP server.

For flashing via `picotool`, "WinUSB" drivers must be loaded for the RP2040 Boot Interface 1 using Zadig. (Plug the device in with BOOTSEL button pressed).

## Expected output

After "Upload and Monitor", it should say something like

```
--- Terminal on COM15 | 115200 8-N-1
--- Available filters and text transformations: colorize, debug, default, direct, hexlify, log2file, nocontrol, printable, send_on_enter, time
--- More details at https://bit.ly/pio-monitor-filters
--- Quit: Ctrl+C | Menu: Ctrl+T | Help: Ctrl+T followed by Ctrl+H
.........IP address: 192.168.0.208
MDNS responder started
HTTP server started
```

And upon visiting that page with a webbrowser, you should 

![web](w5500_web.png)

