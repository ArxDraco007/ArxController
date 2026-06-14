# ArxController

## What is this?
A fully custom controller. Customizable according to your console. Firmware, 3D Models, and PCB design.

## Why did I make this?
Making your own controller is absolutely amazing! The process gives you a complete learning of wiring peripherals, Double LDO circuits, Battery charging protection, and the ESP32-WROOM module. This journey has been absolutely wonderful, and I would recommend this project for all intermediate PCB designers.

## PICTURES-
<img width="1054" height="706" alt="image" src="https://github.com/user-attachments/assets/90c7a90e-b1f2-49ba-8843-6a940ddd1f84" />
<img width="1141" height="782" alt="image" src="https://github.com/user-attachments/assets/09f2d95d-872c-415f-a930-7705b119cab9" />
<img width="1920" height="1080" alt="controller" src="https://github.com/user-attachments/assets/52e48dbd-b1a0-403b-b2e4-0fc79b9d9964" />

## Zine - 
<img width="1304" height="1999" alt="zine" src="https://github.com/user-attachments/assets/31e19667-1f4c-46d8-bcbc-8301d5fd74c1" />

## Build Instructions -
Soldering -
Start by applying flux to the pads on the footprint where you'll be soldering. Tin one of the pads with a small amount of solder, then carefully place your component onto the footprint. Touch your iron to the tinned pad to reflow it and tack the component in place, then let go with your tweezers once it's sitting right. Move to the opposite pad and solder it properly to the component. Finally, go back to your first pad and add a bit more solder to make sure you've got a solid joint.
Firmware - 
Plug in the ESP32-S3 via USB-C, select Board "ESP32S3 Dev Module" and the correct Port, hold BOOT while plugging in (or while pressing RESET) if it doesn't auto-detect, then click Upload to flash it, and finally press RESET or replug to run the new firmware.

## BOM

| Reference | Qty | Value | Footprint | Source | Buy Link |
|---|---|---|---|---|---|
| R2,R3 | 2 | 5.1k | Resistor_SMD:R_0603_1608Metric | Robu.in | [Link](https://robu.in/product/rc0603jr-075k1l-yageo-res-thick-film-0603-5-1k-ohm-5-0-1w1-10w-%C2%B1100ppm-c-pad-smd-t-r/) |
| R4 | 1 | 1.2k | Resistor_SMD:R_0603_1608Metric | LCSC | [Link](https://www.lcsc.com/search?q=0603+1.2K+ohm+resistor) |
| R5,R6,R7 | 3 | 1k | Resistor_SMD:R_0603_1608Metric | Robu.in | [Link](https://robu.in/product/1k-ohm-1-4w-0603-surface-mount-chip-resistor-pack-of-100/) |
| R8,R9 | 2 | 100R | Resistor_SMD:R_0603_1608Metric | LCSC | [Link](https://www.lcsc.com/search?q=0603+100R+1%25+resistor) |
| R10,R11,R12,R13,R14,R15,R16 | 7 | 100k | Resistor_SMD:R_0603_1608Metric | Robu.in | [Link](https://robu.in/product/100k-ohm-1-4w-0603-surface-mount-chip-resistor-pack-of-100/) |
| SW1 | 1 | EN (Tactile SMD) | Button_Switch_SMD:SW_SPST_TS-1088-xR020 | LCSC | [Link](https://www.lcsc.com/search?q=TS-1088) |
| SW2 | 1 | SW_PWR (Header) | Connector_PinSocket_2.54mm:PinSocket_1x03_P2.54mm_Vertical | Robu.in | [Link](https://robu.in/product/2-54mm-female-header-1x40-pin-strip/) |
| SW3 | 1 | BOOT (Tactile SMD) | custom_footprints:SW_SPST_TS-1088-xR020 | LCSC | [Link](https://www.lcsc.com/search?q=TS-1088) |
| SW4 | 1 | BTN_L (Shoulder switch) | custom_footprints:TS-1224VW | LCSC | [Link](https://www.lcsc.com/search?q=TS-1224VW) |
| SW5 | 1 | BTN_UP (Tactile 8mm) | custom_footprints:SW_PUSH_8mm_H5mm_custom | Robu.in | [Link](https://robu.in/product/6x6x5mm-tactile-push-button-switch-pack-of-10/) |
| SW6 | 1 | BTN_LEFT (Tactile 8mm) | custom_footprints:SW_PUSH_8mm_H5mm_custom | Robu.in | [Link](https://robu.in/product/6x6x5mm-tactile-push-button-switch-pack-of-10/) |
| SW7 | 1 | BTN_DOWN (Tactile 8mm) | custom_footprints:SW_PUSH_8mm_H5mm_custom | Robu.in | [Link](https://robu.in/product/6x6x5mm-tactile-push-button-switch-pack-of-10/) |
| SW8 | 1 | BTN_RIGHT (Tactile 8mm) | custom_footprints:SW_PUSH_8mm_H5mm_custom | Robu.in | [Link](https://robu.in/product/6x6x5mm-tactile-push-button-switch-pack-of-10/) |
| SW9 | 1 | BTN_START (Tactile 8mm) | custom_footprints:SW_PUSH_8mm_H5mm_custom | Robu.in | [Link](https://robu.in/product/6x6x5mm-tactile-push-button-switch-pack-of-10/) |
| SW10 | 1 | BTN_R (Shoulder switch) | custom_footprints:TS-1224VW | LCSC | [Link](https://www.lcsc.com/search?q=TS-1224VW) |
| SW11 | 1 | BTN_X (Tactile 8mm) | custom_footprints:SW_PUSH_8mm_H5mm_custom | Robu.in | [Link](https://robu.in/product/6x6x5mm-tactile-push-button-switch-pack-of-10/) |
| SW12 | 1 | BTN_A (Tactile 8mm) | custom_footprints:SW_PUSH_8mm_H5mm_custom | Robu.in | [Link](https://robu.in/product/6x6x5mm-tactile-push-button-switch-pack-of-10/) |
| SW13 | 1 | BTN_B (Tactile 8mm) | custom_footprints:SW_PUSH_8mm_H5mm_custom | Robu.in | [Link](https://robu.in/product/6x6x5mm-tactile-push-button-switch-pack-of-10/) |
| SW14 | 1 | BTN_Y (Tactile 8mm) | custom_footprints:SW_PUSH_8mm_H5mm_custom | Robu.in | [Link](https://robu.in/product/6x6x5mm-tactile-push-button-switch-pack-of-10/) |
| SW15 | 1 | BTN_SELECT (Tactile 8mm) | custom_footprints:SW_PUSH_8mm_H5mm_custom | Robu.in | [Link](https://robu.in/product/6x6x5mm-tactile-push-button-switch-pack-of-10/) |
| SW16 | 1 | BTN_SYS (Tactile 8mm) | custom_footprints:SW_PUSH_8mm_H5mm_custom | Robu.in | [Link](https://robu.in/product/6x6x5mm-tactile-push-button-switch-pack-of-10/) |
| TP1,TP3,TP5 | 3 | TestPoint | TestPoint:TestPoint_Pad_D2.0mm | Robu.in | [Link](https://robu.in/product/2mm-pin-female-header-1x40/) |
| TP4 | 1 | AMS_3V3 (TestPoint) | TestPoint:TestPoint_Pad_D2.0mm | Robu.in | [Link](https://robu.in/product/2mm-pin-female-header-1x40/) |
| U1 | 1 | ESP32-S3-WROOM-1-N16R8 | RF_Module:ESP32-S3-WROOM-1 | Robu.in | [Link](https://robu.in/product/espressif-esp32-s3-wroom-1-n16r8-module/) |
| U2 | 1 | MIC5219-3.3YM5 | Package_TO_SOT_SMD:SOT-23-5 | Robu.in | [Link](https://robu.in/product/mic5219-3-3ym5-tr-microchip-fixed-ldo-voltage-regulator-2-5v-to-12v-350mv-dropout-3-3vout-500maout-sot-23-5/) |
| U3 | 1 | TP4056-42-ESOP8 | Package_SO:SOIC-8-1EP_3.9x4.9mm_P1.27mm_EP2.41x3.3mm_ThermalVias | Robu.in | [Link](https://robu.in/product/tp4056-top-power-asic-4-2v-1a-standalone-linear-li-ion-battery-charger-with-thermal-regulation-sop8/) |
| U4 | 1 | DW01A | Package_TO_SOT_SMD:SOT-23-6 | Robu.in | [Link](https://robu.in/product/dw01a-4-3v-lithium-ion-lithium-polymer-battery-protection-ic-6pin-sot-23/) |
| U5 | 1 | AMS1117-3.3 | Package_TO_SOT_SMD:SOT-223-3_TabPin2 | Robu.in | [Link](https://robu.in/product/ams1117-3-3-slkor-800ma-70db120hz-fixed-3-3v-positive-electrode-18v-sot-223-voltage-regulators-linear-low-drop-out-ldo-regulators-rohs/) |
| U6 | 1 | PCM5102APWR | TSSOP-20 | Robu.in | [Link](https://robu.in/product/pcm5102apwr-texas-instruments-digital-to-analogue-converter-32-bit-384-ksps-i2s-3v-to-3-6v-tssop-20-pins/) |
| U7 | 1 | TPA2012D2 | QFN-16 | LCSC | [Link](https://www.lcsc.com/search?q=TPA2012D2) |
| U8 | 1 | ILI9341 TFT 2.4/2.8" Display Module | SPI 240x320 | LCSC | [Link](https://www.lcsc.com/search?q=ILI9341+2.8+SPI) |
| U9 | 1 | MAX17048G+T10 | SOT-23-6 (USOP-8) | LCSC | [Link](https://www.lcsc.com/search?q=MAX17048) |
| U10 | 1 | XC6220 LDO | SOT-23-5 | LCSC | [Link](https://www.lcsc.com/search?q=XC6220) |
| - | 1 | microSD Card Slot (Push-Push) | SMD microSD Socket | Robu.in | [Link](https://robu.in/product/micro-sd-card-tf-card-memory-card-socket-push-push-type-smd/) |
| - | 1 | USB-C Connector (16-pin) | USB_C_Receptacle_USB2.0_16P | Robu.in | [Link](https://robu.in/product/usb-type-c-16-pin-female-connector-smd/) |
| HW1-HW4   |   4 | M3 × 22mm Machine Screw | Mechanical:MountingHardware | element14 | [Link](https://in.element14.com/tr-fastenings/tr00008755-000/screw-flat-csk-head-sltd-m3-22mm/dp/4156380) |
| HW5-HW8   |   4 | M3 Hex Nut              | Mechanical:MountingHardware | FlyRobo | [Link](https://www.flyrobo.in/m3-ss-hex-nut-10pcs?srsltid=AfmBOopC71qpsOIubiWPyQa1-qcC8mzI4XCSzNWDzo-gBculU_eEorxn)              |

