# PiPocket_Software

Transform Your TV/monitor into a Smart Computer/Smart TV/Smart Gaming Console etc.

Powered with Raspberry Pi Compute Module 4, a powerful and versatile computing solution in a compact form factor. Customize your PiPocket with different CM4 option selections like 2GB, 4GB or 8GB versions to make your go-to solution for high-performance computing in a compact and adaptable package.
Stop juggling HDMI cables and cumbersome setups! Say goodbye to those hassles. piPocket plugs directly into the HDMI port of your TV or monitor, requiring only a USB-C power source. From streaming your favorite content on Netflix and Prime Video to enjoying music and exploring an array of operating systems like Raspberry Pi OS, Windows, Android, Ubuntu, Linux, and more, piPocket is your all-in-one smart solution.

## Features:
- Compatible with Raspberry Pi CM4 compute module both No-eMMC and eMMC* (pre-programmed) version
- HDMI plug to connect with TV/Monitor screen directly 
- Onboard TFcard support so easily connect your favourite compatible Operating System loaded micro SDcard.
- USB Type A to connect HID devices like keyboard, mouse, gaming remote, USB WiFi/Bluetooth dongle, USB Audio dongle, etc.
- Type C for Power
- Power and Activity Status LEDs
- IR Receiver to configure and setup with TV remote control

**_*Note:_ CM4 with eMMC type can be programmed using CM4 IO Board, and avoid using SDcard with eMMC type otherwise you will damage CM4 since both TFcard and eMMC pins shared.** 

## Pinout: 
<img src="https://cdn.shopify.com/s/files/1/1217/2104/files/2_49.png?v=1729244767" >

**Note: CM4 not included default image only for reference.**

## Preparing and Installing OS for PiPocket
<img src="https://github.com/sbcshop/PiPocket_Software/blob/main/images/cm4_variants.png" width="" height="">

### Steps Recommended for **no-eMMC version of CM4**
- For this step we need following things :
  - microSD card recommended size 32GB and above 
  - microSD card Reader
  - Raspberry Imager software, Download and install from [here](https://www.raspberrypi.com/software/)
- Insert card reader along with sdcard to PC and open Raspberry Imager
- Checkout document guide [here](https://github.com/sbcshop/PiPocket_Software/blob/main/Documents/Prepare%20OS%20for%20PiPocket%20CM4%20Compute%20Module.pdf) to install Specific OS which you are interested to try. You can choose between Raspbian OS, media OS like Kodi or gamming OS like Recalbox, etc.
- By default USB port is disabled in few CM4 OS to save power, and PiPocket have two Multiplexed Type A for using keyboard, mouse and any other HID. You will have to enable, which can be done by editing the boot config file (/boot/config.txt). If already present then skip, this is known issue for gaming OS.
  
  <img src=https://github.com/sbcshop/PiPocket_Software/blob/main/images/config_edit.png width="730" height="431" >

  Add following line to activate,
  ```
  dtoverlay=dwc2,dr_mode=host 
  ```
- Now, sdcard ready with OS installation so remove from PC and insert into PiPocket equipped with **CM4 no-eMMC**. Connect PiPocket to you HDMI screen along with keyboard & mouse and then power device using type C.
- **WARNING: DO NOT USE SDCARD IF CM4 IS eMMC VERSION, otherwise you will PERMANENTLY DAMAGE CM4 because eMMC SoC and SDCARD pins shared.**

  
## Resources: 
* [Schematic](https://github.com/sbcshop/StackyFi_Hardware/blob/main/Design%20Data/StackyFi%20SCH.pdf)
* [Hardware Files](https://github.com/sbcshop/StackyFi_Hardware)
* [Step File](https://github.com/sbcshop/StackyFi_Hardware/blob/main/Mechanical%20Data/StackyFi%20STEP.step)
* [CM4 Compute Module Datasheet](https://datasheets.raspberrypi.com/cm4/cm4-datasheet.pdf)
    
## Related Products  

  * [CM4 Compute Module IO Board](https://shop.sb-components.co.uk/products/compute-module-4-io-board-1)

    ![CM4 Compute Module IO Board](https://shop.sb-components.co.uk/cdn/shop/products/ComputeModule4IOBoard_3.jpg?v=1603359036&width=150)

  * [CM4 Compute Module ](https://shop.sb-components.co.uk/products/compute-module-4-board)

    ![CM4_compute_module](https://shop.sb-components.co.uk/cdn/shop/products/CM41_1024x1024_d28f9d00-0447-448b-8d22-f0a4df7d720e.jpg?v=1603697366&width=150)
  
  * [CM4 Module with Antenna](https://shop.sb-components.co.uk/products/raspberry-pi-compute-module-4-antenna-kit)

    ![CM4_compute_module](https://shop.sb-components.co.uk/cdn/shop/products/5dfe3c7f-6ede-4bae-8079-57a06e1258c1_CM_4_AERIAL_028_0e92f365-7ffa-4a92-bf3a-ee392d3542d2.jpg?v=1612261511&width=150)
  
        
## Product License

This is ***open source*** product. Kindly check LICENSE.md file for more information.

Please contact support@sb-components.co.uk for technical support.
<p align="center">
  <img width="360" height="100" src="https://cdn.shopify.com/s/files/1/1217/2104/files/Logo_sb_component_3.png?v=1666086771&width=300">
</p>
