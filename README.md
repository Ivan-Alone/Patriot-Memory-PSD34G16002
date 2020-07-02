# Patriot Memory PSD34G16002 DDR3 4GB

Mini project to add compatibility for this RAM with more motherboards on G41 chipset (particularly **MSI G41M-P28**)
All achived by changing Timings of this RAM to **JEDEC PC3-12800K 1600MHz**

**[README на русском](https://github.com/Ivan-Alone/Patriot-Memory-PSD34G16002/blob/master/README.RU.md)**


## SPD Binaries

#### Original Patriot SPD Binary

[Patriot Memory PSD34G16002 DDR3-1600K.bin](https://github.com/Ivan-Alone/Patriot-Memory-PSD34G16002/raw/master/Patriot%20Memory%20PSD34G16002%20DDR3-1600K.bin)

#### Modded (changed Timings to JEDEC PC3-12800K 1600MHz) Patriot SPD Binary

[Patriot Memory PSD34G16002 DDR3-1600K-MOD.bin](https://github.com/Ivan-Alone/Patriot-Memory-PSD34G16002/raw/master/Patriot%20Memory%20PSD34G16002%20DDR3-1600K%20-%20MOD.bin)



## Flashing

You can flash modded SPD to your memory using **[TechPowerUp SPDTool](https://github.com/Ivan-Alone/Patriot-Memory-PSD34G16002/raw/master/SPDTool_063.zip)** (or Thaiphoon Burner, that you must buy or crack; *not every chipset is supported by SPDTool*)

**Warning**: Flash *ONLY* **PSD34G16002** modules, I cant promise support of any other!



## Flashing Information

You need other motherboard (other PC), that can initialise this memory for flashing SPD, or you can try sleeping-flash method (at one's own risk).


1. **Flashing using other motherboard/PC**

    1.1. Install memory, power-on PC, boot in Windows.

    1.2. Run SPDTool (or cracked/bought Thaiphoon Burner; also you can flash SPD on Linux using *i2c-tools*, google it!), click **File** > **Open** to open Modded binary, next **File** > **Write** > ***Your PSD34G16002 module in list***. Press OK and wait for flashing. **Warning: Do not confuse memory modules, otherwise there is a chance to flash another module incorrectly!**

    1.3. Now you can install this module to your G41 motherboard. All done.


2. **Sleeping-flash method ***(at one's own risk)*****

    2.1. You must have at least one memory module that supported by your motherboard (ex. 2GB DDR3). Install it (ONLY supported!) and boot Windows. When you reached Desktop, put the computer to Sleep. 

    2.2. **NOTE: Your PC MUST go to state with blinking Power LED. If not - go to BIOS and change ACPI Sleep state from *****S1*** **to** ***S3*****, or vice versa**

    2.3. When PC is blinking by led, install this unsupported memory. Next - turn on PC. 

    2.4. When you on Desktop again, you can now follow **1.2 Flashing using other motherboard/PC** instruction above.

    2.5. Reboot your PC, and it must boot correctly, with your long awaited RAM. All done.


 
