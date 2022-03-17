# Copyright (c) AARI Corporation, All Right Served
# Author Wei-Min Shen, 3-11-2020

===== HARDWARE =====

for programming:
MAC<-(usb)->[STLINK/V2]<-(swd)->[Bluepill/STM32F103C8]<-(pc13)->LED

===== SOFTWARE (see Makefile) =====

arm-none-eabi-{gcc,ldf,as}
ST-Flash utility (https://github.com/texane/stlink)

===== Objective =====

This is the minimal code to turn LED on PC13 using registers

===== Operation Procedure =====

0. Type "make" to make $(TARGET).{elf,bin}
1. Type "make flash" to load into Bluepill via STLINK V2 dongle
2. Now, you shall see the LED is turned on Bluepill

===== THE END =====

