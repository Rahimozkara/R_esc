AM32 Single ESC
⚠️ Disclaimer & Project Status: This is an educational project designed by an engineering student. Please note that the current hardware revision has not yet been physically tested. Manufacture, flash, and use at your own risk.

📖 About the Project
This is an open-source, high-performance single Electronic Speed Controller (ESC) designed for FPV drones and custom robotics. It is fully compatible with the AM32 firmware, providing smooth and efficient brushless DC (BLDC) motor control.

✨ Features
Firmware: AM32 Open Source Firmware

Microcontroller: STM32F051

Estimated Continuous Current: ~20A

Supported Protocols: DShot300 / DShot600 / PWM

Application: FPV Drones & Custom Robotics

🛠️ Hardware Design & Known Issues
The schematic and PCB layout for this project were designed using KiCad. The board layout is optimized for efficient power delivery and stable thermal dissipation.

🛑 Important Hardware Note (Current Sensing):
In the current schematic, an INA199A1DCKR current sense amplifier is used, which features a gain of 50 V/V. However, the default AM32 firmware code expects a current sensor with a gain of 65 V/V.

Recommendation: To ensure accurate current readings, you must either adjust the multiplier in the AM32 firmware code to account for the 50x gain, or replace this IC with a 65x gain variant in future PCB revisions.

🚀 How to Manufacture
All necessary hardware files for manufacturing are included in this repository. You can directly use the provided Gerber files for PCB fabrication.

💻 Flashing & Setup
Initial firmware flashing can be done via the SWD pads located on the board using an ST-Link. Once the bootloader is installed, further firmware updates and configuration can be easily managed via Betaflight passthrough.

📄 License
This project is open-source. Feel free to use, modify, and contribute! 
<img width="518" height="304" alt="Ekran görüntüsü 2026-03-10 211703" src="https://github.com/user-attachments/assets/f2e4a318-e114-48ec-bbf3-b4928a793aec" />

