Board's hardware specs
======================

+ Low-power MCU => Cortex M0+ looks to be a good candidate
	+ Low voltage operation?
+ USB port with UART and debugging session
+ Additional small debug port (No-mount or so)
+ Power :
	+ LiPo battery input
	+ USB
	+ Charge LiPo when connected to USB? (Nice to have)
+ Small size
	+ Adafruit Feather form factor?
+ 4x mounting holes
+ Interfaces:
	+ 1x UART
	+ 1x SPI
	+ 1x I2C
	+ ?x GPIOs
	+ 2x ADC?
+ Cheap!
+ 0603 and easy-to-solder packages!
+ Wireless comms?

ICs to consider
===============

+ FT2332 => expensive...
+ uC, check:
	+ STM32L072xx => USB, LQFP
	+ STM32L073xx => USB, LCD, LQFP

Boot
====

+ Check if USB bootloader is available => Looks like it is


Eval Board
==========

+ Consider [this one](https://www.mouser.es/ProductDetail/STMicroelectronics/NUCLEO-L073RZ/?qs=kWQV1gtkNneI%252BACNZmqKJA%3D%3D)


SW
===

+ Check RTOS support:
	+ NuttX
		+ [This one](https://nuttx-docs.readthedocs.io/en/latest/nuttx/main.html) yes
	+ **Zephyr**
		+ [This one](https://docs.zephyrproject.org/latest/boards/arm/nucleo_l073rz/doc/index.html) yes
