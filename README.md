# STM32C0-Nano Hardware Design Files
This is a very simple and cheap STM32C071 board.  

It is largely compatible to ATMega-based "Nano" boards - with 3.3V IOs:  
![Image](https://github.com/user-attachments/assets/46c74608-c11a-406d-b8aa-90d4ee6f17ce)

# Features
* Simple, very low cost (2L, all parts on top of PCB)
* Builtin USB (DFU) bootloader
* Full-speed USB, no crystal needed
(using the Clock Recovery System (CRS))
* 48MHz ARM® Cortex®-M0+ with 24KB SRAM and 128KB Flash memory
* 23+2 GPIOs with 2x SPIs, 2x UARTs, 2x I2C and lots of timer channels
* 9 analog input channels, internal voltage reference
* Fast 2.5MSps 12-bit Analog-to-digital converter (ADC)
* 2x user LEDs (not shared with other GPIOs)

# More Details
see <a href="https://znu.nz/c0">znu.nz/c0</a>

# Demo Firmware
* <a href="https://github.com/znuh/stm32-ACMtest">USB ACM Console + Blinkenlights</a>

# Note
If you build this yourself, you must set the **NBOOT_SEL** Bit in the Flash Option Bytes to **zero** (e.g. via SWD), or you cannot use **BOOT0** to invoke the bootloader during powerup.

# License
Designed by Benedikt Heinz &lt;hunz at mailbox.org&gt;

Creative Commons Attribution/Share-Alike, all text above must be included in any redistribution. See license.txt for additional details.
